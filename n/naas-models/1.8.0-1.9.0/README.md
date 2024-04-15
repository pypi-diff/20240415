# Comparing `tmp/naas_models-1.8.0.tar.gz` & `tmp/naas_models-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naas_models-1.8.0.tar", max compression
+gzip compressed data, was "naas_models-1.9.0.tar", max compression
```

## Comparing `naas_models-1.8.0.tar` & `naas_models-1.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      140 2024-03-27 10:33:42.564569 naas_models-1.8.0/README.md
--rw-r--r--   0        0        0       36 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/__init__.py
--rw-r--r--   0        0        0    12696 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/aimodel_pb2.py
--rw-r--r--   0        0        0    32941 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/chat_pb2.py
--rw-r--r--   0        0        0     1551 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/common_pb2.py
--rw-r--r--   0        0        0     3160 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/credit_pb2.py
--rw-r--r--   0        0        0     2638 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/iam_pb2.py
--rw-r--r--   0        0        0        0 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/__init__.py
--rw-r--r--   0        0        0     6570 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/aimodel_p2p.py
--rw-r--r--   0        0        0    16150 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/chat_p2p.py
--rw-r--r--   0        0        0      411 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/common_p2p.py
--rw-r--r--   0        0        0     2458 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/credit_p2p.py
--rw-r--r--   0        0        0     1885 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/iam_p2p.py
--rw-r--r--   0        0        0     5441 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/registry_p2p.py
--rw-r--r--   0        0        0     3587 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/secret_p2p.py
--rw-r--r--   0        0        0     6929 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/space_p2p.py
--rw-r--r--   0        0        0    10253 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/validate_p2p.py
--rw-r--r--   0        0        0    17198 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/pydantic/workspace_p2p.py
--rw-r--r--   0        0        0    12685 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/registry_pb2.py
--rw-r--r--   0        0        0     8755 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/secret_pb2.py
--rw-r--r--   0        0        0    17760 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/space_pb2.py
--rw-r--r--   0        0        0    20979 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/validate_pb2.py
--rw-r--r--   0        0        0    36748 2024-03-27 10:33:42.564569 naas_models-1.8.0/naas_models/workspace_pb2.py
--rw-r--r--   0        0        0      485 2024-03-27 10:33:54.572643 naas_models-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 naas_models-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      140 2024-04-12 09:46:05.289244 naas_models-1.9.0/README.md
+-rw-r--r--   0        0        0       36 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/__init__.py
+-rw-r--r--   0        0        0    12786 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/aimodel_pb2.py
+-rw-r--r--   0        0        0    32941 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/chat_pb2.py
+-rw-r--r--   0        0        0     1551 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/common_pb2.py
+-rw-r--r--   0        0        0     3160 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/credit_pb2.py
+-rw-r--r--   0        0        0     2638 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/iam_pb2.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/__init__.py
+-rw-r--r--   0        0        0     6677 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/aimodel_p2p.py
+-rw-r--r--   0        0        0    16150 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/chat_p2p.py
+-rw-r--r--   0        0        0      411 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/common_p2p.py
+-rw-r--r--   0        0        0     2458 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/credit_p2p.py
+-rw-r--r--   0        0        0     1885 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/iam_p2p.py
+-rw-r--r--   0        0        0     5441 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/registry_p2p.py
+-rw-r--r--   0        0        0     3587 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/secret_p2p.py
+-rw-r--r--   0        0        0     6929 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/space_p2p.py
+-rw-r--r--   0        0        0    10253 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/validate_p2p.py
+-rw-r--r--   0        0        0    17198 2024-04-12 09:46:05.289244 naas_models-1.9.0/naas_models/pydantic/workspace_p2p.py
+-rw-r--r--   0        0        0    12685 2024-04-12 09:46:05.293244 naas_models-1.9.0/naas_models/registry_pb2.py
+-rw-r--r--   0        0        0     8755 2024-04-12 09:46:05.293244 naas_models-1.9.0/naas_models/secret_pb2.py
+-rw-r--r--   0        0        0    17760 2024-04-12 09:46:05.293244 naas_models-1.9.0/naas_models/space_pb2.py
+-rw-r--r--   0        0        0    20979 2024-04-12 09:46:05.293244 naas_models-1.9.0/naas_models/validate_pb2.py
+-rw-r--r--   0        0        0    36748 2024-04-12 09:46:05.293244 naas_models-1.9.0/naas_models/workspace_pb2.py
+-rw-r--r--   0        0        0      485 2024-04-12 09:46:18.017124 naas_models-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 naas_models-1.9.0/PKG-INFO
```

### Comparing `naas_models-1.8.0/naas_models/aimodel_pb2.py` & `naas_models-1.9.0/naas_models/aimodel_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import naas_models.validate_pb2 as validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\raimodel.proto\x12\x07\x61imodel\x1a\x0evalidate.proto\"\x97\x02\n\x07\x41IModel\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x12\x11\n\x04name\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x15\n\x08provider\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05image\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07\x65nabled\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x04type\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x17\n\nrestricted\x18\x07 \x01(\x08H\x06\x88\x01\x01\x12\x17\n\nname_alias\x18\x08 \x01(\tH\x07\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_nameB\x0b\n\t_providerB\x08\n\x06_imageB\n\n\x08_enabledB\x07\n\x05_typeB\r\n\x0b_restrictedB\r\n\x0b_name_alias\"\x8f\x02\n\x12\x43ompletionResponse\x12\x1f\n\x08model_id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x12\x13\n\x0b\x63ompletions\x18\x02 \x03(\t\x12\x19\n\x0cinput_tokens\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12\x1a\n\routput_tokens\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10image_resolution\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0bimage_steps\x18\x06 \x01(\x05H\x04\x88\x01\x01\x42\x0b\n\t_model_idB\x0f\n\r_input_tokensB\x10\n\x0e_output_tokensB\x13\n\x11_image_resolutionB\x0e\n\x0c_image_steps\"\xab\x01\n\x14\x41IModelResponseError\x12(\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x15.aimodel.AIModelErrorH\x00\x88\x01\x01\x12\x13\n\x06status\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06reason\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x07message\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x07\n\x05_codeB\t\n\x07_statusB\t\n\x07_reasonB\n\n\x08_message\"d\n\x12\x41IModelListRequest\x12\x16\n\tpage_size\x18\x01 \x01(\x05H\x00\x88\x01\x01\x12\x18\n\x0bpage_number\x18\x02 \x01(\x05H\x01\x88\x01\x01\x42\x0c\n\n_page_sizeB\x0e\n\x0c_page_number\"\xa0\x01\n\x13\x41IModelListResponse\x12\"\n\x08\x61imodels\x18\x01 \x03(\x0b\x32\x10.aimodel.AIModel\x12\x18\n\x0bpage_number\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\x0e\n\x0c_page_numberB\x08\n\x06_error\"5\n\x11\x41IModelGetRequest\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x42\x05\n\x03_id\"\x85\x01\n\x12\x41IModelGetResponse\x12&\n\x07\x61imodel\x18\x01 \x01(\x0b\x32\x10.aimodel.AIModelH\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\n\n\x08_aimodelB\x08\n\x06_error\"^\n\x18\x41IModelCompletionRequest\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x12\x14\n\x07payload\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x05\n\x03_idB\n\n\x08_payload\"\x9d\x01\n\x19\x41IModelCompletionResponse\x12\x34\n\ncompletion\x18\x01 \x01(\x0b\x32\x1b.aimodel.CompletionResponseH\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\r\n\x0b_completionB\x08\n\x06_error\"\x89\x02\n\x1b\x41IModelAdminCreationRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08provider\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x12\n\x05image\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x07\x65nabled\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x04type\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x17\n\nrestricted\x18\x06 \x01(\x08H\x05\x88\x01\x01\x12\x17\n\nname_alias\x18\x07 \x01(\tH\x06\x88\x01\x01\x42\x07\n\x05_nameB\x0b\n\t_providerB\x08\n\x06_imageB\n\n\x08_enabledB\x07\n\x05_typeB\r\n\x0b_restrictedB\r\n\x0b_name_alias\"\x8f\x01\n\x1c\x41IModelAdminCreationResponse\x12&\n\x07\x61imodel\x18\x01 \x01(\x0b\x32\x10.aimodel.AIModelH\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\n\n\x08_aimodelB\x08\n\x06_error\"=\n\x19\x41IModelAdminDeleteRequest\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x42\x05\n\x03_id\"Y\n\x1a\x41IModelAdminDeleteResponse\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x00\x88\x01\x01\x42\x08\n\x06_error*\xa4\x01\n\x0c\x41IModelError\x12\x0c\n\x08NO_ERROR\x10\x00\x12\x12\n\x0e\x41LREADY_EXISTS\x10\x01\x12\r\n\tNOT_FOUND\x10\x02\x12\x0f\n\x0bNOT_UPDATED\x10\x03\x12\x12\n\x0eNOT_AUTHORIZED\x10\x04\x12\x1a\n\x16\x41IMODEL_OUT_OF_CREDITS\x10\x05\x12\"\n\x1e\x41IMODEL_DONT_HANDLE_COMPLETION\x10\x06\x42\x30Z.github.com/jupyter-naas/naas-models/go/aimodelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\raimodel.proto\x12\x07\x61imodel\x1a\x0evalidate.proto\"\xc7\x02\n\x07\x41IModel\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x12\x11\n\x04name\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x15\n\x08provider\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x12\n\x05image\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07\x65nabled\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x11\n\x04type\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x17\n\nrestricted\x18\x07 \x01(\x08H\x06\x88\x01\x01\x12\x17\n\nname_alias\x18\x08 \x01(\tH\x07\x88\x01\x01\x12\x1b\n\x0e\x63ontext_window\x18\t \x01(\x05H\x08\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_nameB\x0b\n\t_providerB\x08\n\x06_imageB\n\n\x08_enabledB\x07\n\x05_typeB\r\n\x0b_restrictedB\r\n\x0b_name_aliasB\x11\n\x0f_context_window\"\x8f\x02\n\x12\x43ompletionResponse\x12\x1f\n\x08model_id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x12\x13\n\x0b\x63ompletions\x18\x02 \x03(\t\x12\x19\n\x0cinput_tokens\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12\x1a\n\routput_tokens\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10image_resolution\x18\x05 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0bimage_steps\x18\x06 \x01(\x05H\x04\x88\x01\x01\x42\x0b\n\t_model_idB\x0f\n\r_input_tokensB\x10\n\x0e_output_tokensB\x13\n\x11_image_resolutionB\x0e\n\x0c_image_steps\"\xab\x01\n\x14\x41IModelResponseError\x12(\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x15.aimodel.AIModelErrorH\x00\x88\x01\x01\x12\x13\n\x06status\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x06reason\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x07message\x18\x04 \x01(\tH\x03\x88\x01\x01\x42\x07\n\x05_codeB\t\n\x07_statusB\t\n\x07_reasonB\n\n\x08_message\"d\n\x12\x41IModelListRequest\x12\x16\n\tpage_size\x18\x01 \x01(\x05H\x00\x88\x01\x01\x12\x18\n\x0bpage_number\x18\x02 \x01(\x05H\x01\x88\x01\x01\x42\x0c\n\n_page_sizeB\x0e\n\x0c_page_number\"\xa0\x01\n\x13\x41IModelListResponse\x12\"\n\x08\x61imodels\x18\x01 \x03(\x0b\x32\x10.aimodel.AIModel\x12\x18\n\x0bpage_number\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\x0e\n\x0c_page_numberB\x08\n\x06_error\"5\n\x11\x41IModelGetRequest\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x42\x05\n\x03_id\"\x85\x01\n\x12\x41IModelGetResponse\x12&\n\x07\x61imodel\x18\x01 \x01(\x0b\x32\x10.aimodel.AIModelH\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\n\n\x08_aimodelB\x08\n\x06_error\"^\n\x18\x41IModelCompletionRequest\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x12\x14\n\x07payload\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x05\n\x03_idB\n\n\x08_payload\"\x9d\x01\n\x19\x41IModelCompletionResponse\x12\x34\n\ncompletion\x18\x01 \x01(\x0b\x32\x1b.aimodel.CompletionResponseH\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\r\n\x0b_completionB\x08\n\x06_error\"\x89\x02\n\x1b\x41IModelAdminCreationRequest\x12\x11\n\x04name\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08provider\x18\x02 \x01(\tH\x01\x88\x01\x01\x12\x12\n\x05image\x18\x03 \x01(\tH\x02\x88\x01\x01\x12\x14\n\x07\x65nabled\x18\x04 \x01(\x08H\x03\x88\x01\x01\x12\x11\n\x04type\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x17\n\nrestricted\x18\x06 \x01(\x08H\x05\x88\x01\x01\x12\x17\n\nname_alias\x18\x07 \x01(\tH\x06\x88\x01\x01\x42\x07\n\x05_nameB\x0b\n\t_providerB\x08\n\x06_imageB\n\n\x08_enabledB\x07\n\x05_typeB\r\n\x0b_restrictedB\r\n\x0b_name_alias\"\x8f\x01\n\x1c\x41IModelAdminCreationResponse\x12&\n\x07\x61imodel\x18\x01 \x01(\x0b\x32\x10.aimodel.AIModelH\x00\x88\x01\x01\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x01\x88\x01\x01\x42\n\n\x08_aimodelB\x08\n\x06_error\"=\n\x19\x41IModelAdminDeleteRequest\x12\x19\n\x02id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01H\x00\x88\x01\x01\x42\x05\n\x03_id\"Y\n\x1a\x41IModelAdminDeleteResponse\x12\x31\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.aimodel.AIModelResponseErrorH\x00\x88\x01\x01\x42\x08\n\x06_error*\xa4\x01\n\x0c\x41IModelError\x12\x0c\n\x08NO_ERROR\x10\x00\x12\x12\n\x0e\x41LREADY_EXISTS\x10\x01\x12\r\n\tNOT_FOUND\x10\x02\x12\x0f\n\x0bNOT_UPDATED\x10\x03\x12\x12\n\x0eNOT_AUTHORIZED\x10\x04\x12\x1a\n\x16\x41IMODEL_OUT_OF_CREDITS\x10\x05\x12\"\n\x1e\x41IMODEL_DONT_HANDLE_COMPLETION\x10\x06\x42\x30Z.github.com/jupyter-naas/naas-models/go/aimodelb\x06proto3')
 
 _AIMODELERROR = DESCRIPTOR.enum_types_by_name['AIModelError']
 AIModelError = enum_type_wrapper.EnumTypeWrapper(_AIMODELERROR)
 NO_ERROR = 0
 ALREADY_EXISTS = 1
 NOT_FOUND = 2
 NOT_UPDATED = 3
@@ -143,36 +143,36 @@
   _COMPLETIONRESPONSE.fields_by_name['model_id']._serialized_options = b'\372B\005r\003\260\001\001'
   _AIMODELGETREQUEST.fields_by_name['id']._options = None
   _AIMODELGETREQUEST.fields_by_name['id']._serialized_options = b'\372B\005r\003\260\001\001'
   _AIMODELCOMPLETIONREQUEST.fields_by_name['id']._options = None
   _AIMODELCOMPLETIONREQUEST.fields_by_name['id']._serialized_options = b'\372B\005r\003\260\001\001'
   _AIMODELADMINDELETEREQUEST.fields_by_name['id']._options = None
   _AIMODELADMINDELETEREQUEST.fields_by_name['id']._serialized_options = b'\372B\005r\003\260\001\001'
-  _AIMODELERROR._serialized_start=2053
-  _AIMODELERROR._serialized_end=2217
+  _AIMODELERROR._serialized_start=2101
+  _AIMODELERROR._serialized_end=2265
   _AIMODEL._serialized_start=43
-  _AIMODEL._serialized_end=322
-  _COMPLETIONRESPONSE._serialized_start=325
-  _COMPLETIONRESPONSE._serialized_end=596
-  _AIMODELRESPONSEERROR._serialized_start=599
-  _AIMODELRESPONSEERROR._serialized_end=770
-  _AIMODELLISTREQUEST._serialized_start=772
-  _AIMODELLISTREQUEST._serialized_end=872
-  _AIMODELLISTRESPONSE._serialized_start=875
-  _AIMODELLISTRESPONSE._serialized_end=1035
-  _AIMODELGETREQUEST._serialized_start=1037
-  _AIMODELGETREQUEST._serialized_end=1090
-  _AIMODELGETRESPONSE._serialized_start=1093
-  _AIMODELGETRESPONSE._serialized_end=1226
-  _AIMODELCOMPLETIONREQUEST._serialized_start=1228
-  _AIMODELCOMPLETIONREQUEST._serialized_end=1322
-  _AIMODELCOMPLETIONRESPONSE._serialized_start=1325
-  _AIMODELCOMPLETIONRESPONSE._serialized_end=1482
-  _AIMODELADMINCREATIONREQUEST._serialized_start=1485
-  _AIMODELADMINCREATIONREQUEST._serialized_end=1750
-  _AIMODELADMINCREATIONRESPONSE._serialized_start=1753
-  _AIMODELADMINCREATIONRESPONSE._serialized_end=1896
-  _AIMODELADMINDELETEREQUEST._serialized_start=1898
-  _AIMODELADMINDELETEREQUEST._serialized_end=1959
-  _AIMODELADMINDELETERESPONSE._serialized_start=1961
-  _AIMODELADMINDELETERESPONSE._serialized_end=2050
+  _AIMODEL._serialized_end=370
+  _COMPLETIONRESPONSE._serialized_start=373
+  _COMPLETIONRESPONSE._serialized_end=644
+  _AIMODELRESPONSEERROR._serialized_start=647
+  _AIMODELRESPONSEERROR._serialized_end=818
+  _AIMODELLISTREQUEST._serialized_start=820
+  _AIMODELLISTREQUEST._serialized_end=920
+  _AIMODELLISTRESPONSE._serialized_start=923
+  _AIMODELLISTRESPONSE._serialized_end=1083
+  _AIMODELGETREQUEST._serialized_start=1085
+  _AIMODELGETREQUEST._serialized_end=1138
+  _AIMODELGETRESPONSE._serialized_start=1141
+  _AIMODELGETRESPONSE._serialized_end=1274
+  _AIMODELCOMPLETIONREQUEST._serialized_start=1276
+  _AIMODELCOMPLETIONREQUEST._serialized_end=1370
+  _AIMODELCOMPLETIONRESPONSE._serialized_start=1373
+  _AIMODELCOMPLETIONRESPONSE._serialized_end=1530
+  _AIMODELADMINCREATIONREQUEST._serialized_start=1533
+  _AIMODELADMINCREATIONREQUEST._serialized_end=1798
+  _AIMODELADMINCREATIONRESPONSE._serialized_start=1801
+  _AIMODELADMINCREATIONRESPONSE._serialized_end=1944
+  _AIMODELADMINDELETEREQUEST._serialized_start=1946
+  _AIMODELADMINDELETEREQUEST._serialized_end=2007
+  _AIMODELADMINDELETERESPONSE._serialized_start=2009
+  _AIMODELADMINDELETERESPONSE._serialized_end=2098
 # @@protoc_insertion_point(module_scope)
```

### Comparing `naas_models-1.8.0/naas_models/chat_pb2.py` & `naas_models-1.9.0/naas_models/chat_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/common_pb2.py` & `naas_models-1.9.0/naas_models/common_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/credit_pb2.py` & `naas_models-1.9.0/naas_models/credit_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/iam_pb2.py` & `naas_models-1.9.0/naas_models/iam_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/aimodel_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/aimodel_p2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,26 @@
     AIMODEL_DONT_HANDLE_COMPLETION = 6
 
 
 
 
 class AIModel(BaseModel):
 
-    _one_of_dict = {"AIModel._enabled": {"fields": {"enabled"}}, "AIModel._id": {"fields": {"id"}}, "AIModel._image": {"fields": {"image"}}, "AIModel._name": {"fields": {"name"}}, "AIModel._name_alias": {"fields": {"name_alias"}}, "AIModel._provider": {"fields": {"provider"}}, "AIModel._restricted": {"fields": {"restricted"}}, "AIModel._type": {"fields": {"type"}}}
+    _one_of_dict = {"AIModel._context_window": {"fields": {"context_window"}}, "AIModel._enabled": {"fields": {"enabled"}}, "AIModel._id": {"fields": {"id"}}, "AIModel._image": {"fields": {"image"}}, "AIModel._name": {"fields": {"name"}}, "AIModel._name_alias": {"fields": {"name_alias"}}, "AIModel._provider": {"fields": {"provider"}}, "AIModel._restricted": {"fields": {"restricted"}}, "AIModel._type": {"fields": {"type"}}}
     _check_one_of = root_validator(pre=True, allow_reuse=True)(check_one_of)
 
     id: UUID = FieldInfo(default="") 
     name: str = FieldInfo(default="") 
     provider: str = FieldInfo(default="") 
     image: str = FieldInfo(default="") 
     enabled: bool = FieldInfo(default=False) 
     type: str = FieldInfo(default="") 
     restricted: bool = FieldInfo(default=False) 
     name_alias: str = FieldInfo(default="") 
+    context_window: int = FieldInfo(default=0) 
 
 
 
 
 class CompletionResponse(BaseModel):
 
     _one_of_dict = {"CompletionResponse._image_resolution": {"fields": {"image_resolution"}}, "CompletionResponse._image_steps": {"fields": {"image_steps"}}, "CompletionResponse._input_tokens": {"fields": {"input_tokens"}}, "CompletionResponse._model_id": {"fields": {"model_id"}}, "CompletionResponse._output_tokens": {"fields": {"output_tokens"}}}
```

### Comparing `naas_models-1.8.0/naas_models/pydantic/chat_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/chat_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/credit_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/credit_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/iam_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/iam_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/registry_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/registry_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/secret_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/secret_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/space_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/space_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/validate_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/validate_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/pydantic/workspace_p2p.py` & `naas_models-1.9.0/naas_models/pydantic/workspace_p2p.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/registry_pb2.py` & `naas_models-1.9.0/naas_models/registry_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/secret_pb2.py` & `naas_models-1.9.0/naas_models/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/space_pb2.py` & `naas_models-1.9.0/naas_models/space_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/validate_pb2.py` & `naas_models-1.9.0/naas_models/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/naas_models/workspace_pb2.py` & `naas_models-1.9.0/naas_models/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `naas_models-1.8.0/PKG-INFO` & `naas_models-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naas-models
-Version: 1.8.0
+Version: 1.9.0
 Summary: Library containing all models used in the naas ecosystem. You can use this library to know how to talk to our micro services.
 Author: Maxime Jublou
 Author-email: maxime@naas.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

