# Comparing `tmp/gptstonks_wrappers-0.0.1.tar.gz` & `tmp/gptstonks_wrappers-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptstonks_wrappers-0.0.1.tar", last modified: Mon Apr 15 17:22:56 2024, max compression
+gzip compressed data, was "gptstonks_wrappers-0.0.1b0.tar", last modified: Mon Apr 15 17:13:21 2024, max compression
```

## Comparing `gptstonks_wrappers-0.0.1.tar` & `gptstonks_wrappers-0.0.1b0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2812 2024-04-15 16:48:42.259960 gptstonks_wrappers-0.0.1/README.md
--rw-r--r--   0        0        0     1535 2024-04-15 17:22:56.001831 gptstonks_wrappers-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       28 2024-04-15 17:02:37.148728 gptstonks_wrappers-0.0.1/tests/env.sh
--rw-r--r--   0        0        0     5700 2024-04-15 16:40:42.021406 gptstonks_wrappers-0.0.1/tests/kernels/test_auto_llama_index.py
--rw-r--r--   0        0        0     3553 2024-04-15 16:40:42.024739 gptstonks_wrappers-0.0.1/tests/kernels/test_auto_multistep_query_engine.py
--rw-r--r--   0        0        0      566 2024-04-15 16:40:42.028072 gptstonks_wrappers-0.0.1/tests/llms/test_chat_model_llm_iface.py
--rw-r--r--   0        0        0      311 2024-04-13 11:16:30.507370 gptstonks_wrappers-0.0.1/tests/llms/test_guidance_wrapper.py
--rw-r--r--   0        0        0     4629 1970-01-01 00:00:00.000000 gptstonks_wrappers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2812 2024-04-15 16:48:42.259960 gptstonks_wrappers-0.0.1b0/README.md
+-rw-r--r--   0        0        0     1954 2024-04-15 17:13:21.547405 gptstonks_wrappers-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0       28 2024-04-15 17:02:37.148728 gptstonks_wrappers-0.0.1b0/tests/env.sh
+-rw-r--r--   0        0        0     5700 2024-04-15 16:40:42.021406 gptstonks_wrappers-0.0.1b0/tests/kernels/test_auto_llama_index.py
+-rw-r--r--   0        0        0     3553 2024-04-15 16:40:42.024739 gptstonks_wrappers-0.0.1b0/tests/kernels/test_auto_multistep_query_engine.py
+-rw-r--r--   0        0        0      566 2024-04-15 16:40:42.028072 gptstonks_wrappers-0.0.1b0/tests/llms/test_chat_model_llm_iface.py
+-rw-r--r--   0        0        0      311 2024-04-13 11:16:30.507370 gptstonks_wrappers-0.0.1b0/tests/llms/test_guidance_wrapper.py
+-rw-r--r--   0        0        0     4641 1970-01-01 00:00:00.000000 gptstonks_wrappers-0.0.1b0/PKG-INFO
```

### Comparing `gptstonks_wrappers-0.0.1/README.md` & `gptstonks_wrappers-0.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `gptstonks_wrappers-0.0.1/pyproject.toml` & `gptstonks_wrappers-0.0.1b0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,42 @@
+[tool.pytest.ini_options]
+addopts = [
+    "--color=yes",
+    "--durations=0",
+    "--strict-markers",
+    "--doctest-modules",
+]
+filterwarnings = [
+    "ignore::DeprecationWarning",
+    "ignore::UserWarning",
+]
+log_cli = "True"
+markers = [
+    "slow: slow tests",
+]
+minversion = "6.0"
+testpaths = "tests/"
+
+[tool.coverage.report]
+exclude_lines = [
+    "pragma: nocover",
+    "raise NotImplementedError",
+    "raise NotImplementedError()",
+    "if __name__ == .__main__.:",
+]
+
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
 [project]
 name = "gptstonks-wrappers"
-version = "0.0.1"
+version = "0.0.1-beta"
 description = "Useful wrappers around common AI tools: LangChain, LlamaIndex, etc."
 authors = [
     { name = "GPTStonks Team", email = "gptstonks@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10,<3.12"
 classifiers = [
@@ -48,20 +80,9 @@
     "pytest-cov[toml]>=4.1.0",
     "pytest-asyncio>=0.23.5",
     "duckduckgo-search>=4.5.0",
     "wikipedia>=1.4.0",
 ]
 
 [project.urls]
-Homepage = "https://github.com/GPTStonks/gptstonks"
-"Bug Tracker" = "https://github.com/GPTStonks/gptstonks/issues"
-
-[tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
-]
-
-[build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
+Homepage = "https://github.com/GPTStonks/gptstonks-core"
+"Bug Tracker" = "https://github.com/GPTStonks/gptstonks-core/issues"
```

### Comparing `gptstonks_wrappers-0.0.1/tests/kernels/test_auto_llama_index.py` & `gptstonks_wrappers-0.0.1b0/tests/kernels/test_auto_llama_index.py`

 * *Files identical despite different names*

### Comparing `gptstonks_wrappers-0.0.1/tests/kernels/test_auto_multistep_query_engine.py` & `gptstonks_wrappers-0.0.1b0/tests/kernels/test_auto_multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `gptstonks_wrappers-0.0.1/tests/llms/test_chat_model_llm_iface.py` & `gptstonks_wrappers-0.0.1b0/tests/llms/test_chat_model_llm_iface.py`

 * *Files identical despite different names*

### Comparing `gptstonks_wrappers-0.0.1/PKG-INFO` & `gptstonks_wrappers-0.0.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gptstonks-wrappers
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Useful wrappers around common AI tools: LangChain, LlamaIndex, etc.
 Author-Email: GPTStonks Team <gptstonks@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Project-URL: Homepage, https://github.com/GPTStonks/gptstonks
-Project-URL: Bug tracker, https://github.com/GPTStonks/gptstonks/issues
+Project-URL: Homepage, https://github.com/GPTStonks/gptstonks-core
+Project-URL: Bug tracker, https://github.com/GPTStonks/gptstonks-core/issues
 Requires-Python: <3.12,>=3.10
 Requires-Dist: rank-bm25>=0.2.2
 Requires-Dist: llama-index>=0.10.13
 Requires-Dist: langchain>=0.0.353
 Requires-Dist: llama-index-llms-openai>=0.1.6
 Requires-Dist: llama-index-retrievers-bm25>=0.1.3
 Requires-Dist: rich<13.0.0,>=12.6.0; extra == "guidance"
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: gptstonks-wrappers Version: 0.0.1 Summary: Useful
+Metadata-Version: 2.1 Name: gptstonks-wrappers Version: 0.0.1b0 Summary: Useful
 wrappers around common AI tools: LangChain, LlamaIndex, etc. Author-Email:
 GPTStonks Team
 gmail.com> License: MIT Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Project-URL: Homepage, https://github.com/GPTStonks/gptstonks
-Project-URL: Bug tracker, https://github.com/GPTStonks/gptstonks/issues
-Requires-Python: <3.12,>=3.10 Requires-Dist: rank-bm25>=0.2.2 Requires-Dist:
-llama-index>=0.10.13 Requires-Dist: langchain>=0.0.353 Requires-Dist: llama-
-index-llms-openai>=0.1.6 Requires-Dist: llama-index-retrievers-bm25>=0.1.3
-Requires-Dist: rich<13.0.0,>=12.6.0; extra == "guidance" Requires-Dist:
-transformers>=4.33.0; extra == "guidance" Requires-Dist: peft>=0.5.0; extra ==
-"guidance" Requires-Dist: accelerate>=0.22.0; extra == "guidance" Requires-
-Dist: bitsandbytes>=0.41.1; extra == "guidance" Requires-Dist:
-sentencepiece>=0.1.99; extra == "guidance" Requires-Dist: guidance>=0.0.64;
-extra == "guidance" Requires-Dist: auto-gptq>=0.4.2; extra == "guidance"
-Requires-Dist: optimum>=1.12.0; extra == "guidance" Requires-Dist: llama-index-
-embeddings-huggingface>=0.1.3; extra == "huggingface" Requires-Dist: llama-
-index-llms-huggingface>=0.1.3; extra == "huggingface" Requires-Dist:
-pytest>=8.0.2; extra == "testing" Requires-Dist: sentence-transformers>=2.2.2;
-extra == "testing" Requires-Dist: pytest-cov[toml]>=4.1.0; extra == "testing"
-Requires-Dist: pytest-asyncio>=0.23.5; extra == "testing" Requires-Dist:
-duckduckgo-search>=4.5.0; extra == "testing" Requires-Dist: wikipedia>=1.4.0;
-extra == "testing" Provides-Extra: guidance Provides-Extra: huggingface
-Provides-Extra: testing Description-Content-Type: text/markdown
+:: OS Independent Project-URL: Homepage, https://github.com/GPTStonks/
+gptstonks-core Project-URL: Bug tracker, https://github.com/GPTStonks/
+gptstonks-core/issues Requires-Python: <3.12,>=3.10 Requires-Dist: rank-
+bm25>=0.2.2 Requires-Dist: llama-index>=0.10.13 Requires-Dist:
+langchain>=0.0.353 Requires-Dist: llama-index-llms-openai>=0.1.6 Requires-Dist:
+llama-index-retrievers-bm25>=0.1.3 Requires-Dist: rich<13.0.0,>=12.6.0; extra
+== "guidance" Requires-Dist: transformers>=4.33.0; extra == "guidance"
+Requires-Dist: peft>=0.5.0; extra == "guidance" Requires-Dist:
+accelerate>=0.22.0; extra == "guidance" Requires-Dist: bitsandbytes>=0.41.1;
+extra == "guidance" Requires-Dist: sentencepiece>=0.1.99; extra == "guidance"
+Requires-Dist: guidance>=0.0.64; extra == "guidance" Requires-Dist: auto-
+gptq>=0.4.2; extra == "guidance" Requires-Dist: optimum>=1.12.0; extra ==
+"guidance" Requires-Dist: llama-index-embeddings-huggingface>=0.1.3; extra ==
+"huggingface" Requires-Dist: llama-index-llms-huggingface>=0.1.3; extra ==
+"huggingface" Requires-Dist: pytest>=8.0.2; extra == "testing" Requires-Dist:
+sentence-transformers>=2.2.2; extra == "testing" Requires-Dist: pytest-cov
+[toml]>=4.1.0; extra == "testing" Requires-Dist: pytest-asyncio>=0.23.5; extra
+== "testing" Requires-Dist: duckduckgo-search>=4.5.0; extra == "testing"
+Requires-Dist: wikipedia>=1.4.0; extra == "testing" Provides-Extra: guidance
+Provides-Extra: huggingface Provides-Extra: testing Description-Content-Type:
+text/markdown
                                     [Logo]
 _[_J_o_i_n_ _W_a_i_t_l_i_s_t_ _B_a_d_g_e_]_[_Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l_ _B_a_d_g_e_]_[_X_ _F_o_l_l_o_w_ _U_s_ _B_a_d_g_e_]_[_D_i_s_c_o_r_d_ _B_a_d_g_e_]
                                 _[_D_o_c_k_e_r_ _B_a_d_g_e_]
       _[_H_u_g_g_i_n_g_ _F_a_c_e_ _B_a_d_g_e_]_[_L_a_n_g_C_h_a_i_n_ _B_a_d_g_e_]_[_F_a_s_t_A_P_I_ _B_a_d_g_e_]_[_O_p_e_n_B_B_ _B_a_d_g_e_]
 # GPTStonks Wrappers ## Description GPTStonks Wrappers provides Auto models,
 similar to the `transformers` library, but for common AI tools instead of
 models: LangChain, LlamaIndex, etc. ## Development 1. Install [PDM](https://
```

