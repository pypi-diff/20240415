# Comparing `tmp/sae_lens-0.2.1.tar.gz` & `tmp/sae_lens-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-0.2.1.tar", max compression
+gzip compressed data, was "sae_lens-0.2.2.tar", max compression
```

## Comparing `sae_lens-0.2.1.tar` & `sae_lens-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-04-13 15:04:32.245435 sae_lens-0.2.1/LICENSE
--rw-r--r--   0        0        0    14571 2024-04-13 15:04:32.245435 sae_lens-0.2.1/README.md
--rw-r--r--   0        0        0     1585 2024-04-13 15:04:33.185433 sae_lens-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-13 15:04:33.185433 sae_lens-0.2.1/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15355 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0      579 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    19076 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     4251 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    16559 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2804 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     8745 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/config.py
--rw-r--r--   0        0        0     5732 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1527 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     3675 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/optim.py
--rw-r--r--   0        0        0     7187 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2132 2024-04-13 15:04:32.257435 sae_lens-0.2.1/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    13294 2024-04-13 15:04:32.261435 sae_lens-0.2.1/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-13 15:04:32.261435 sae_lens-0.2.1/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-13 15:04:32.261435 sae_lens-0.2.1/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    17227 2024-04-13 15:04:32.261435 sae_lens-0.2.1/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     4888 2024-04-13 15:04:32.261435 sae_lens-0.2.1/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-13 15:04:32.261435 sae_lens-0.2.1/sae_lens/training/utils.py
--rw-r--r--   0        0        0    15857 1970-01-01 00:00:00.000000 sae_lens-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-15 14:53:42.825325 sae_lens-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2134 2024-04-15 14:53:42.825325 sae_lens-0.2.2/README.md
+-rw-r--r--   0        0        0     1585 2024-04-15 14:53:43.801319 sae_lens-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-15 14:53:43.801319 sae_lens-0.2.2/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:53:42.833325 sae_lens-0.2.2/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15355 2024-04-15 14:53:42.833325 sae_lens-0.2.2/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0      595 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    19076 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     5562 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    16559 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2804 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     8793 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/config.py
+-rw-r--r--   0        0        0     5732 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1528 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     3675 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     7187 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2318 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    13592 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    17227 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     4888 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 sae_lens-0.2.2/PKG-INFO
```

### Comparing `sae_lens-0.2.1/LICENSE` & `sae_lens-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/pyproject.toml` & `sae_lens-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "0.2.1"
+version = "0.2.2"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sae_lens-0.2.1/sae_lens/__init__.py` & `sae_lens-0.2.2/sae_lens/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-0.2.1/sae_lens/analysis/dashboard_runner.py` & `sae_lens-0.2.2/sae_lens/analysis/dashboard_runner.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 import time
 import uuid
 
 import pandas as pd
 import plotly
 import plotly.express as px
 import torch
+import wandb
 from sae_vis.data_config_classes import (
     ActsHistogramConfig,
     Column,
     FeatureTablesConfig,
     SaeVisConfig,
     SaeVisLayoutConfig,
     SequencesConfig,
 )
 from sae_vis.data_fetching_fns import get_feature_data
 from torch.nn.functional import cosine_similarity
 from tqdm import tqdm
 
-import wandb
 from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
 
 
 class DashboardRunner:
 
     def __init__(
         self,
```

### Comparing `sae_lens-0.2.1/sae_lens/analysis/feature_statistics.py` & `sae_lens-0.2.2/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-0.2.2/sae_lens/analysis/neuronpedia_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,7 +15,9 @@
     url = url + "?name=" + name
     list_feature = [
         {"modelId": model, "layer": f"{layer}-{dataset}", "index": str(feature)}
         for feature in features
     ]
     url = url + "&features=" + urllib.parse.quote(json.dumps(list_feature))
     webbrowser.open(url)
+
+    return url
```

### Comparing `sae_lens-0.2.1/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-0.2.2/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/analysis/tsea.py` & `sae_lens-0.2.2/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-0.2.2/sae_lens/toolkit/pretrained_saes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+from typing import Optional, Tuple
 
 import torch
 from huggingface_hub import hf_hub_download, list_files_info
 from safetensors import safe_open
 from tqdm import tqdm
 
 from sae_lens.training.config import LanguageModelSAERunnerConfig
@@ -13,44 +14,83 @@
 def load_sparsity(path: str) -> torch.Tensor:
     sparsity_path = os.path.join(path, "sparsity.safetensors")
     with safe_open(sparsity_path, framework="pt", device="cpu") as f:  # type: ignore
         sparsity = f.get_tensor("sparsity")
     return sparsity
 
 
-def get_gpt2_res_jb_saes() -> (
-    tuple[dict[str, SparseAutoencoder], dict[str, torch.Tensor]]
-):
+def download_sae_from_hf(
+    repo_id: str = "jbloom/GPT2-Small-SAEs-Reformatted",
+    folder_name: str = "blocks.0.hook_resid_pre",
+    force_download: bool = False,
+) -> Tuple[str, str, Optional[str]]:
+
+    FILENAME = f"{folder_name}/cfg.json"
+    cfg_path = hf_hub_download(
+        repo_id=repo_id, filename=FILENAME, force_download=force_download
+    )
+
+    FILENAME = f"{folder_name}/sae_weights.safetensors"
+    sae_path = hf_hub_download(
+        repo_id=repo_id, filename=FILENAME, force_download=force_download
+    )
+
+    try:
+        FILENAME = f"{folder_name}/sparsity.safetensors"
+        sparsity_path = hf_hub_download(
+            repo_id=repo_id, filename=FILENAME, force_download=force_download
+        )
+    except:  # noqa
+        sparsity_path = None
+
+    return cfg_path, sae_path, sparsity_path
+
+
+def load_sae_from_local_path(path: str) -> Tuple[SparseAutoencoder, torch.Tensor]:
+    sae = SparseAutoencoder.load_from_pretrained(path)
+    sparsity = load_sparsity(path)
+    return sae, sparsity
+
+
+def get_gpt2_res_jb_saes(
+    hook_point: Optional[str] = None,
+    device: str = "cpu",
+) -> tuple[dict[str, SparseAutoencoder], dict[str, torch.Tensor]]:
+    """
+    Download the sparse autoencoders for the GPT2-Small model with residual connections
+    from the repository of jbloom. You can specify a hook_point to download only one
+    of the sparse autoencoders if desired.
+
+    """
 
     GPT2_SMALL_RESIDUAL_SAES_REPO_ID = "jbloom/GPT2-Small-SAEs-Reformatted"
     GPT2_SMALL_RESIDUAL_SAES_HOOK_POINTS = [
         f"blocks.{layer}.hook_resid_pre" for layer in range(12)
     ] + ["blocks.11.hook_resid_post"]
 
+    if hook_point is not None:
+        assert hook_point in GPT2_SMALL_RESIDUAL_SAES_HOOK_POINTS, (
+            f"hook_point must be one of {GPT2_SMALL_RESIDUAL_SAES_HOOK_POINTS}"
+            f"but got {hook_point}"
+        )
+        GPT2_SMALL_RESIDUAL_SAES_HOOK_POINTS = [hook_point]
+
     saes = {}
     sparsities = {}
     for hook_point in tqdm(GPT2_SMALL_RESIDUAL_SAES_HOOK_POINTS):
-        # download the files required:
-        FILENAME = f"{hook_point}/cfg.json"
-        hf_hub_download(repo_id=GPT2_SMALL_RESIDUAL_SAES_REPO_ID, filename=FILENAME)
-
-        FILENAME = f"{hook_point}/sae_weights.safetensors"
-        path = hf_hub_download(
-            repo_id=GPT2_SMALL_RESIDUAL_SAES_REPO_ID, filename=FILENAME
-        )
 
-        FILENAME = f"{hook_point}/sparsity.safetensors"
-        path = hf_hub_download(
-            repo_id=GPT2_SMALL_RESIDUAL_SAES_REPO_ID, filename=FILENAME
+        _, sae_path, _ = download_sae_from_hf(
+            repo_id=GPT2_SMALL_RESIDUAL_SAES_REPO_ID, folder_name=hook_point
         )
 
         # Then use our function to download the files
-        folder_path = os.path.dirname(path)
-        sae = SparseAutoencoder.load_from_pretrained(folder_path)
+        folder_path = os.path.dirname(sae_path)
+        sae = SparseAutoencoder.load_from_pretrained(folder_path, device=device)
         sparsity = load_sparsity(folder_path)
+        sparsity = sparsity.to(device)
         saes[hook_point] = sae
         sparsities[hook_point] = sparsity
 
     return saes, sparsities
 
 
 def convert_connor_rob_sae_to_our_saelens_format(
```

### Comparing `sae_lens-0.2.1/sae_lens/training/activations_store.py` & `sae_lens-0.2.2/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/training/cache_activations_runner.py` & `sae_lens-0.2.2/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/training/config.py` & `sae_lens-0.2.2/sae_lens/training/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from typing import Any, Optional, cast
 
 import torch
-
 import wandb
 
 DTYPE_MAP = {
     "torch.float32": torch.float32,
     "torch.float64": torch.float64,
     "torch.float16": torch.float16,
     "torch.bfloat16": torch.bfloat16,
@@ -50,14 +49,15 @@
     # SAE Parameters
     b_dec_init_method: str = "geometric_median"
     expansion_factor: int | list[int] = 4
     from_pretrained_path: Optional[str] = None
     d_sae: Optional[int] = None
 
     # Training Parameters
+    mse_loss_normalization: Optional[str] = None
     l1_coefficient: float | list[float] = 1e-3
     lp_norm: float | list[float] = 1
     lr: float | list[float] = 3e-4
     lr_scheduler_name: str | list[str] = (
         "constant"  # constant, cosineannealing, cosineannealingwarmrestarts
     )
     lr_warm_up_steps: int | list[int] = 500
```

### Comparing `sae_lens-0.2.1/sae_lens/training/evals.py` & `sae_lens-0.2.2/sae_lens/training/evals.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import partial
 from typing import Any, Mapping, cast
 
 import pandas as pd
 import torch
+import wandb
 from transformer_lens import HookedTransformer
 from transformer_lens.utils import get_act_name
 
-import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 @torch.no_grad()
 def run_evals(
     sparse_autoencoder: SparseAutoencoder,
```

### Comparing `sae_lens-0.2.1/sae_lens/training/geometric_median.py` & `sae_lens-0.2.2/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/training/lm_runner.py` & `sae_lens-0.2.2/sae_lens/training/lm_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, cast
 
 import wandb
+
 from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
 
 # from sae_lens.training.activation_store import ActivationStore
 from sae_lens.training.train_sae_on_language_model import train_sae_on_language_model
```

### Comparing `sae_lens-0.2.1/sae_lens/training/optim.py` & `sae_lens-0.2.2/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/training/sae_group.py` & `sae_lens-0.2.2/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/training/session_loader.py` & `sae_lens-0.2.2/sae_lens/training/session_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,36 +35,41 @@
 
         sae_group = SparseAutoencoderDictionary(self.cfg)
 
         return model, sae_group, activations_loader
 
     @classmethod
     def load_pretrained_sae(
-        cls, path: str
+        cls, path: str, device: str = "cpu"
     ) -> Tuple[HookedTransformer, SparseAutoencoderDictionary, ActivationsStore]:
         """
         Loads a session for analysing a pretrained sparse autoencoder.
         """
 
         # load the SAE
         sparse_autoencoder = SparseAutoencoder.load_from_pretrained(path)
+        sparse_autoencoder.to(device)
+        sparse_autoencoder.cfg.device = device
 
         # load the model, SAE and activations loader with it.
         session_loader = cls(sparse_autoencoder.cfg)
         model, sae_group, activations_loader = (
             session_loader.load_sae_training_group_session()
         )
 
         return model, sae_group, activations_loader
 
-    def get_model(self, model_name: str):
+    def get_model(self, model_name: str) -> HookedTransformer:
         """
         Loads a model from transformer lens.
 
         Abstracted to allow for easy modification.
         """
 
         # Todo: add check that model_name is valid
 
-        model = HookedTransformer.from_pretrained(model_name)
+        model = HookedTransformer.from_pretrained(
+            model_name,
+            device=self.cfg.device,
+        )
 
         return model
```

### Comparing `sae_lens-0.2.1/sae_lens/training/sparse_autoencoder.py` & `sae_lens-0.2.2/sae_lens/training/sparse_autoencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,17 @@
                 self.W_dec,
                 "... d_sae, d_sae d_in -> ... d_in",
             )
             + self.b_dec
         )
 
         # add config for whether l2 is normalized:
-        per_item_mse_loss = _per_item_mse_loss_with_target_norm(sae_out, x)
+        per_item_mse_loss = _per_item_mse_loss_with_target_norm(
+            sae_out, x, self.cfg.mse_loss_normalization
+        )
         ghost_grad_loss = torch.tensor(0.0, dtype=self.dtype, device=self.device)
         # gate on config and training so evals is not slowed down.
         if (
             self.use_ghost_grads
             and self.training
             and dead_neuron_mask is not None
             and dead_neuron_mask.sum() > 0
@@ -350,32 +352,37 @@
         ghost_out = feature_acts_dead_neurons_only @ self.W_dec[dead_neuron_mask, :]
         l2_norm_ghost_out = torch.norm(ghost_out, dim=-1)
         norm_scaling_factor = l2_norm_residual / (1e-6 + l2_norm_ghost_out * 2)
         ghost_out = ghost_out * norm_scaling_factor[:, None].detach()
 
         # 3.
         per_item_mse_loss_ghost_resid = _per_item_mse_loss_with_target_norm(
-            ghost_out, residual.detach()
+            ghost_out, residual.detach(), self.cfg.mse_loss_normalization
         )
         mse_rescaling_factor = (
             per_item_mse_loss / (per_item_mse_loss_ghost_resid + 1e-6)
         ).detach()
         per_item_mse_loss_ghost_resid = (
             mse_rescaling_factor * per_item_mse_loss_ghost_resid
         )
 
         return per_item_mse_loss_ghost_resid.mean()
 
 
 def _per_item_mse_loss_with_target_norm(
-    preds: torch.Tensor, target: torch.Tensor
+    preds: torch.Tensor,
+    target: torch.Tensor,
+    mse_loss_normalization: Optional[str] = None,
 ) -> torch.Tensor:
     """
     Calculate MSE loss per item in the batch, without taking a mean.
     Then, normalizes by the L2 norm of the centered target.
     This normalization seems to improve performance.
     """
-    target_centered = target - target.mean(dim=0, keepdim=True)
-    normalization = target_centered.norm(dim=-1, keepdim=True)
-    return torch.nn.functional.mse_loss(preds, target, reduction="none") / (
-        normalization + 1e-6
-    )
+    if mse_loss_normalization == "dense_batch":
+        target_centered = target - target.mean(dim=0, keepdim=True)
+        normalization = target_centered.norm(dim=-1, keepdim=True)
+        return torch.nn.functional.mse_loss(preds, target, reduction="none") / (
+            normalization + 1e-6
+        )
+    else:
+        return torch.nn.functional.mse_loss(preds, target, reduction="none")
```

### Comparing `sae_lens-0.2.1/sae_lens/training/toy_model_runner.py` & `sae_lens-0.2.2/sae_lens/training/toy_model_runner.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Any, cast
 
 import einops
 import torch
-
 import wandb
+
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 from sae_lens.training.toy_models import Config as ToyConfig
 from sae_lens.training.toy_models import Model as ToyModel
 from sae_lens.training.train_sae_on_toy_model import train_toy_sae
 
 
 @dataclass
```

### Comparing `sae_lens-0.2.1/sae_lens/training/toy_models.py` & `sae_lens-0.2.2/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.1/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-0.2.2/sae_lens/training/train_sae_on_language_model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from dataclasses import dataclass
 from typing import Any, cast
 
 import torch
+import wandb
 from safetensors.torch import save_file
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from tqdm import tqdm
 from transformer_lens import HookedTransformer
 
-import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.evals import run_evals
 from sae_lens.training.geometric_median import compute_geometric_median
 from sae_lens.training.optim import get_scheduler
 from sae_lens.training.sae_group import SparseAutoencoderDictionary
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
```

### Comparing `sae_lens-0.2.1/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-0.2.2/sae_lens/training/train_sae_on_toy_model.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, cast
 
 import torch
+import wandb
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-import wandb
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 def train_toy_sae(
     sparse_autoencoder: SparseAutoencoder,
     activation_store: torch.Tensor,  # TODO: this type seems strange / wrong
     batch_size: int = 1024,
```

### Comparing `sae_lens-0.2.1/sae_lens/training/utils.py` & `sae_lens-0.2.2/sae_lens/training/utils.py`

 * *Files identical despite different names*

