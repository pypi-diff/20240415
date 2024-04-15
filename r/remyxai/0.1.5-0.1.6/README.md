# Comparing `tmp/remyxai-0.1.5-py3-none-any.whl.zip` & `tmp/remyxai-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7778 bytes, number of entries: 10
+Zip file size: 9838 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 23-Dec-25 07:08 remyxai/__init__.py
--rw-rw-r--  2.0 unx     3054 b- defN 23-Dec-25 07:16 remyxai/api.py
--rw-rw-r--  2.0 unx     6398 b- defN 23-Dec-25 07:16 remyxai/cli.py
+-rw-rw-r--  2.0 unx     7068 b- defN 24-Apr-15 06:04 remyxai/api.py
+-rw-rw-r--  2.0 unx     7178 b- defN 24-Apr-15 05:59 remyxai/cli.py
 -rw-rw-r--  2.0 unx     4987 b- defN 23-Dec-25 07:08 remyxai/utils.py
--rw-rw-r--  2.0 unx     1065 b- defN 23-Dec-25 07:28 remyxai-0.1.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4311 b- defN 23-Dec-25 07:28 remyxai-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Dec-25 07:28 remyxai-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Dec-25 07:28 remyxai-0.1.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Dec-25 07:28 remyxai-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      768 b- defN 23-Dec-25 07:28 remyxai-0.1.5.dist-info/RECORD
-10 files, 20729 bytes uncompressed, 6472 bytes compressed:  68.8%
+-rw-rw-r--  2.0 unx     1065 b- defN 24-Apr-15 06:08 remyxai-0.1.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5723 b- defN 24-Apr-15 06:08 remyxai-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-15 06:08 remyxai-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 24-Apr-15 06:08 remyxai-0.1.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-15 06:08 remyxai-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      768 b- defN 24-Apr-15 06:08 remyxai-0.1.6.dist-info/RECORD
+10 files, 26935 bytes uncompressed, 8532 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: remyxai/cli.py
 Comment: 
 
 Filename: remyxai/utils.py
 Comment: 
 
-Filename: remyxai-0.1.5.dist-info/LICENSE
+Filename: remyxai-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: remyxai-0.1.5.dist-info/METADATA
+Filename: remyxai-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: remyxai-0.1.5.dist-info/WHEEL
+Filename: remyxai-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: remyxai-0.1.5.dist-info/entry_points.txt
+Filename: remyxai-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: remyxai-0.1.5.dist-info/top_level.txt
+Filename: remyxai-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: remyxai-0.1.5.dist-info/RECORD
+Filename: remyxai-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## remyxai/api.py

```diff
@@ -1,10 +1,15 @@
 import os
+import time
 import shutil
 import requests
+import tempfile
+import subprocess
+import numpy as np
+from tritonclient.http import InferenceServerClient, InferInput, InferRequestedOutput
 
 REMYXAI_API_KEY = os.environ.get("REMYXAI_API_KEY")
 if not REMYXAI_API_KEY:
     raise ValueError("REMYXAI_API_KEY not found in environment variables. Please set it with your API key.")
 
 BASE_URL = "https://engine.remyx.ai/api/v1.0/"
 
@@ -72,14 +77,102 @@
 
 def train_generator(model_name: str, hf_dataset: str):
     url = f"{BASE_URL}task/generate/{model_name}"
     params = {"hf_dataset": hf_dataset}
     response = requests.post(url, headers=HEADERS, params=params)
     return response.json()
 
+# Deployments
+def download_deployment_package(model_name, output_path):
+    """Download the deployment package for a specified model."""
+    url = f"{BASE_URL}deployment/download/{model_name}"
+    response = requests.get(url, headers=HEADERS, stream=True)
+    if response.status_code == 200:
+        with open(output_path, 'wb') as f:
+            shutil.copyfileobj(response.raw, f)
+        print(f"Deployment package downloaded successfully: {output_path}")
+        return response  # Return response for further processing if needed
+    else:
+        print(f"Failed to download deployment package: {response.status_code}")
+        print(response.json())  # Assuming the error message is in JSON format
+        return None
+
+def deploy_model(model_name, action='up'):
+    """Deploy or tear down a model using Docker Compose based on the action."""
+    with tempfile.TemporaryDirectory() as tmpdirname:
+        model_dir = os.path.join(tmpdirname, model_name)  # This is where we expect to build the Docker image.
+        compose_file_path = os.path.join(model_dir, 'docker-compose.yml')
+        zip_path = os.path.join(tmpdirname, f"{model_name}_deployment_package.zip")
+
+        if action == 'up':
+            if download_deployment_package(model_name, zip_path):
+                # Unzip the package directly into the model_dir to ensure the structure is correct
+                os.makedirs(model_dir, exist_ok=True)  # Make sure the target directory exists
+                subprocess.run(['unzip', '-o', zip_path, '-d', model_dir], check=True)
+
+                # Check the contents just to verify
+                print("Unzipped files:", os.listdir(model_dir))  # For debugging
+
+                # Generate Docker Compose YAML if it does not exist
+                if not os.path.exists(compose_file_path):
+                    with open(compose_file_path, 'w') as f:
+                        f.write(f"""
+version: '3.8'
+services:
+  tritonserver:
+    build:
+      context: ./
+      dockerfile: Dockerfile
+    image: {model_name}:latest
+    container_name: {model_name}_triton_server
+    runtime: nvidia
+    ports:
+      - "8000:8000"
+      - "8001:8001"
+      - "8002:8002"
+    shm_size: 24G
+    restart: unless-stopped
+                        """)
+
+                # Deploy using Docker Compose
+                os.chdir(model_dir)  # Change to the directory where the Dockerfile and docker-compose.yml are
+                subprocess.run(['docker', 'compose', 'up', '--build', '-d'], check=True)
+                print("Deployment successful")
+        elif action == 'down':
+            if os.path.exists(compose_file_path):
+                os.chdir(model_dir)  # Ensure commands run in the correct directory
+                subprocess.run(['docker', 'compose', 'down'], check=True)
+                print("Service has been successfully taken down.")
+            else:
+                print("Error: Deployment not found.")
+
+# Infer
+def run_inference(model_name, prompt, server_url="localhost:8000", model_version="1"):
+    triton_client = InferenceServerClient(url=server_url, verbose=False)
+
+    # Convert the prompt to bytes and wrap in a numpy array
+    prompt_np = np.array([prompt.encode('utf-8')], dtype=object)
+
+    # Create input for PROMPT.
+    prompt_in = InferInput(name="PROMPT", shape=[1], datatype="BYTES")
+    prompt_in.set_data_from_numpy(prompt_np, binary_data=True)
+
+    results_out = InferRequestedOutput(name="RESULTS", binary_data=False)
+
+    start_time = time.time()
+    response = triton_client.infer(model_name=model_name,
+                                   model_version=model_version,
+                                   inputs=[prompt_in],
+                                   outputs=[results_out])
+
+    elapsed_time = time.time() - start_time
+    results = response.get_response()["outputs"][0]["data"][0]
+    return results, elapsed_time
+
+
 # User
 def get_user_profile():
     url = f"{BASE_URL}user"
     response = requests.get(url, headers=HEADERS)
     return response.json()
 
 def get_user_credits():
```

## remyxai/cli.py

```diff
@@ -1,74 +1,71 @@
 from .api import *
 from .utils import labeler
 import argparse
+import time
 from pprint import pprint
+import subprocess
 
 def main():
     parser = argparse.ArgumentParser(description="Model management script")
 
-    # Define top-level actions
     subparsers_action = parser.add_subparsers(dest="action", help="Top-level actions")
 
-    # Define 'model' action
     model_parser = subparsers_action.add_parser("model", help="Model-related actions")
 
-    # Define subactions for 'model' action
     subparsers_model = model_parser.add_subparsers(dest="subaction", help="Model subactions")
 
-    # Define 'list' subaction
     list_parser = subparsers_model.add_parser("list", help="List your models")
 
-    # Define 'summary' subaction
     summary_parser = subparsers_model.add_parser("summarize", help="Summarize a model")
     summary_parser.add_argument("--model_name", required=True, help="Name of the model to provide a summary")
 
-    # Define 'download' subaction
     download_parser = subparsers_model.add_parser("download", help="Download and convert a model")
     download_parser.add_argument("--model_name", required=True, help="Name of the model to delete")
     download_parser.add_argument("--model_format", required=True, help="of the model to delete")
 
-    # Define 'delete' subaction
     delete_parser = subparsers_model.add_parser("delete", help="Delete a model")
     delete_parser.add_argument("--model_name", required=True, help="Name of the model to delete")
 
-    # Define 'classify' action
     classify_parser = subparsers_action.add_parser("classify", help="Classifier-related actions")
     classify_parser.add_argument("--model_name", required=True, help="Name of the model")
     classify_parser.add_argument("--labels", required=True, help="Comma separated list of labels, e.g. 'cat,dog'")
     classify_parser.add_argument("--model_size", required=True, help="Integer value for model size from 1=small up to 5=large")
     classify_parser.add_argument("--hf_dataset", required=False, default=None, help="(Optional) Name of the HuggingFace dataset to use for training")
 
-    # Define 'detect' action
     detect_parser = subparsers_action.add_parser("detect", help="Detector-related actions")
     detect_parser.add_argument("--model_name", required=True, help="Name of the model")
     detect_parser.add_argument("--labels", required=True, help="Comma separated list of labels, e.g. 'cat,dog'")
     detect_parser.add_argument("--model_size", required=True, help="Integer value for model size from 1=small up to 5=large")
     detect_parser.add_argument("--hf_dataset", required=False, default=None, help="(Optional) Name of the HuggingFace dataset to use for training")
 
-    # Define 'generate' action
     generate_parser = subparsers_action.add_parser("generate", help="Generator-related actions")
     generate_parser.add_argument("--model_name", required=True, help="Name of the model")
     generate_parser.add_argument("--hf_dataset", required=True, default=None, help="Name of the HuggingFace dataset to use for training")
 
-    # Define 'user' action
+    deploy_parser = subparsers_action.add_parser("deploy", help="Deploy or tear down a model using Docker Compose")
+    deploy_parser.add_argument("--model_name", required=True, help="Name of the model to deploy or tear down")
+    deploy_parser.add_argument("command", nargs='?', default="up", choices=['up', 'down'], help="Specify 'up' to deploy or 'down' to tear down the model")
+
+    infer_parser = subparsers_action.add_parser("infer", help="Submit an inference request to Triton server")
+    infer_parser.add_argument("--model_name", type=str, required=True, help="Model name for the inference")
+    infer_parser.add_argument("--prompt", type=str, required=True, help="Prompt to be used for the inference")
+    infer_parser.add_argument("--server_url", type=str, default="localhost:8000", help="URL of the Triton Inference Server")
+    infer_parser.add_argument("--model_version", type=str, default="1", help="Version of the model")
+
     user_parser = subparsers_action.add_parser("user", help="User-related actions")
 
-    # Define subactions for 'user' action
     subparsers_user = user_parser.add_subparsers(dest="subaction", help="User subactions")
     profile_parser = subparsers_user.add_parser("profile", help="Get user profile")
     credits_parser = subparsers_user.add_parser("credits", help="Get user credits and subscription info if it exists")
     
-    # Define 'utils' action
     utils_parser = subparsers_action.add_parser("utils", help="Utility actions")
     
-    # Define subactions for 'utils' action
     subparsers_utils = utils_parser.add_subparsers(dest="subaction", help="Utility subactions")
 
-    # Define 'labeler' subaction
     labeler_parser = subparsers_utils.add_parser("label", help="Extract labels from a directory of images")
     labeler_parser.add_argument("--labels", required=True, help="Comma separated list of labels, e.g. 'cat,dog'")
     labeler_parser.add_argument("--image_dir", required=True, help="Directory of images in '.jpg', '.jpeg', '.png' format")
     labeler_parser.add_argument("--model_name", default=None, help="Name of the model")
 
     args = parser.parse_args()
 
@@ -100,14 +97,22 @@
         training_detector = train_detector(args.model_name, labels, args.model_size, args.hf_dataset)
         pprint(training_detector)
 
     elif args.action == "generate":                                                                            
         training_generator = train_generator(args.model_name, args.hf_dataset)
         pprint(training_generator)
 
+    elif args.action == "deploy":
+        deploy_model(args.model_name, args.command)
+
+    elif args.action == "infer":
+        result, time_elapsed = run_inference(args.model_name, args.prompt, args.server_url, args.model_version)
+        print("--- %s seconds ---" % time_elapsed)
+        print(result)
+
     elif args.action == "user":
         if args.subaction == "profile":
             profile = get_user_profile()
             pprint(profile)
         elif args.subaction == "credits":
             user_credits = get_user_credits()
             pprint(user_credits)
```

## Comparing `remyxai-0.1.5.dist-info/LICENSE` & `remyxai-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

