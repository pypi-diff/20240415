# Comparing `tmp/quant2-0.1.1.tar.gz` & `tmp/quant2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant2-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quant2-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quant2-0.1.1.tar` & `quant2-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.1/LICENSE
--rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.1/README.md
--rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.1/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
--rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.1/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
--rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.1/quant/README.md
--rw-r--r--   0        0        0      559 2024-04-14 09:53:16.441728 quant2-0.1.1/quant/__init__.py
--rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.1/quant/__main__.py
--rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.1/quant/evaluate/__init__.py
--rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.1/quant/evaluate/table20240326.py
--rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.1/quant/evaluate/utils.py
--rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.1/quant/football/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.1/quant/football/data/__init__.py
--rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.1/quant/football/data/dataset.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.1/quant/football/data/functional.py
--rw-r--r--   0        0        0     1329 2024-04-08 11:39:25.763545 quant2-0.1.1/quant/football/data/preprocessing.py
--rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.1/quant/football/data/stats.py
--rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.1/quant/football/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.1/quant/football/infer/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-11 17:24:14.938089 quant2-0.1.1/quant/football/infer/fastapi_app.py
--rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.1/quant/football/infer/fastapi_app_test.py
--rw-r--r--   0        0        0     7795 2024-04-12 06:41:29.194262 quant2-0.1.1/quant/football/infer/football_infer_overunder_v1.py
--rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.1/quant/football/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.1/quant/football/models/mtnet.py
--rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.1/quant/football/models/stnet.py
--rw-r--r--   0        0        0      379 2024-04-14 08:54:29.067337 quant2-0.1.1/quant/football/transforms/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-14 08:09:52.271038 quant2-0.1.1/quant/football/transforms/table20240326.py
--rw-r--r--   0        0        0     8511 2024-04-14 08:07:38.143730 quant2-0.1.1/quant/football/transforms/table20240410.py
--rw-r--r--   0        0        0     8704 2024-04-14 09:34:13.443355 quant2-0.1.1/quant/football/transforms/table20240414.py
--rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.1/quant/layers/__init__.py
--rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.1/quant/layers/layer_scale.py
--rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.1/quant/layers/mlp.py
--rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.1/quant/layers/normalization.py
--rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.1/quant/layers/swiglu_ffn.py
--rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.1/quant/utils/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.1/quant/utils/archive.py
--rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.1/quant/utils/config.py
--rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.1/quant/utils/io.py
--rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.1/quant/utils/logging.py
--rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.1/tests/football/data/test_utils.py
--rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.1/tools/analysis_tools/analyze_cls_results.py
--rw-r--r--   0        0        0     2278 2024-04-14 09:52:37.848169 quant2-0.1.1/tools/experimental/make_dataset.py
--rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.1/tools/experimental/make_split.py
--rw-r--r--   0        0        0     6456 2024-04-14 03:08:49.930582 quant2-0.1.1/tools/experimental/nni_football.py
--rw-r--r--   0        0        0      450 2024-04-14 03:58:35.586525 quant2-0.1.1/tools/experimental/nni_football_config.yaml
--rw-r--r--   0        0        0     1578 2024-04-13 16:51:58.165877 quant2-0.1.1/tools/experimental/nni_football_config_search_space.json
--rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.1/tools/experimental/nni_model.py
--rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.1/tools/experimental/nni_model_config.yaml
--rw-r--r--   0        0        0     2854 2024-04-12 06:25:44.029850 quant2-0.1.1/tools/fb_cls_test.py
--rw-r--r--   0        0        0     5945 2024-04-13 12:40:38.861046 quant2-0.1.1/tools/fb_cls_train.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.2/LICENSE
+-rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.2/README.md
+-rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.2/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
+-rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.2/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
+-rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.2/quant/README.md
+-rw-r--r--   0        0        0      559 2024-04-15 20:46:19.279693 quant2-0.1.2/quant/__init__.py
+-rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.2/quant/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.2/quant/evaluate/__init__.py
+-rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.2/quant/evaluate/table20240326.py
+-rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.2/quant/evaluate/utils.py
+-rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.2/quant/football/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.2/quant/football/data/__init__.py
+-rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.2/quant/football/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.2/quant/football/data/functional.py
+-rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.2/quant/football/data/preprocessing.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.2/quant/football/data/stats.py
+-rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.2/quant/football/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.2/quant/football/infer/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-11 17:24:14.938089 quant2-0.1.2/quant/football/infer/fastapi_app.py
+-rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.2/quant/football/infer/fastapi_app_test.py
+-rw-r--r--   0        0        0     7798 2024-04-15 11:06:59.301368 quant2-0.1.2/quant/football/infer/football_infer_overunder_v1.py
+-rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.2/quant/football/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.2/quant/football/models/mtnet.py
+-rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.2/quant/football/models/stnet.py
+-rw-r--r--   0        0        0      379 2024-04-14 08:54:29.067337 quant2-0.1.2/quant/football/transforms/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-14 08:09:52.271038 quant2-0.1.2/quant/football/transforms/table20240326.py
+-rw-r--r--   0        0        0     8511 2024-04-14 08:07:38.143730 quant2-0.1.2/quant/football/transforms/table20240410.py
+-rw-r--r--   0        0        0     8795 2024-04-15 14:39:32.419111 quant2-0.1.2/quant/football/transforms/table20240414.py
+-rw-r--r--   0        0        0     8336 2024-04-15 20:50:57.893655 quant2-0.1.2/quant/football/transforms/table20240415.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.2/quant/layers/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.2/quant/layers/layer_scale.py
+-rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.2/quant/layers/mlp.py
+-rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.2/quant/layers/normalization.py
+-rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.2/quant/layers/swiglu_ffn.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.2/quant/utils/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.2/quant/utils/archive.py
+-rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.2/quant/utils/config.py
+-rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.2/quant/utils/io.py
+-rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.2/quant/utils/logging.py
+-rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.2/tests/football/data/test_utils.py
+-rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.2/tools/analysis_tools/analyze_cls_results.py
+-rw-r--r--   0        0        0     2632 2024-04-15 16:14:46.557801 quant2-0.1.2/tools/experimental/make_dataset.py
+-rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.2/tools/experimental/make_split.py
+-rw-r--r--   0        0        0     6485 2024-04-15 11:07:06.081414 quant2-0.1.2/tools/experimental/nni_football.py
+-rw-r--r--   0        0        0      476 2024-04-15 19:50:59.765841 quant2-0.1.2/tools/experimental/nni_football_config.yaml
+-rw-r--r--   0        0        0     1556 2024-04-15 20:08:48.206604 quant2-0.1.2/tools/experimental/nni_football_config_search_space.json
+-rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.2/tools/experimental/nni_model.py
+-rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.2/tools/experimental/nni_model_config.yaml
+-rw-r--r--   0        0        0     2855 2024-04-15 11:07:14.941468 quant2-0.1.2/tools/fb_cls_test.py
+-rw-r--r--   0        0        0     6353 2024-04-15 11:07:20.811492 quant2-0.1.2/tools/fb_cls_train.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.2/PKG-INFO
```

### Comparing `quant2-0.1.1/.gitignore` & `quant2-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/LICENSE` & `quant2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg` & `quant2-0.1.2/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg` & `quant2-0.1.2/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/pyproject.toml` & `quant2-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/README.md` & `quant2-0.1.2/quant/README.md`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/__init__.py` & `quant2-0.1.2/quant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 help_doc_str = """\
 usage: quant [--version] [--help]
 
 shell command:
     quant -h
```

### Comparing `quant2-0.1.1/quant/evaluate/table20240326.py` & `quant2-0.1.2/quant/evaluate/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/evaluate/utils.py` & `quant2-0.1.2/quant/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/football/data/dataset.py` & `quant2-0.1.2/quant/football/data/dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/football/data/preprocessing.py` & `quant2-0.1.2/quant/football/data/preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         with_centering = True
         x_add = 0.0 - x_min
 
         if x_range > 1e-6:
             with_scaling = True
             x_mul = 1.0 / x_range
     elif method == "maxabs":
-        x_max_abs = np.abs(arr).max()
+        x_max_abs = np.abs(arr).max().item()
 
         if x_max_abs > 1e-6:
             with_scaling = True
             x_mul = 1.0 / x_max_abs
 
     return x_add, x_mul, with_centering, with_scaling
```

### Comparing `quant2-0.1.1/quant/football/data/utils.py` & `quant2-0.1.2/quant/football/data/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/football/infer/fastapi_app.py` & `quant2-0.1.2/quant/football/infer/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/football/infer/football_infer_overunder_v1.py` & `quant2-0.1.2/quant/football/infer/football_infer_overunder_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
     def _load_config(self, model_archive):
         model_archive = pathlib.Path(model_archive)  # tarfile
         cache_dir = make_dir(f".cache/{model_archive.stem}", exist_ok=False)
 
         extract_tar(model_archive, cache_dir)
 
-        cfg_files = list(cache_dir.glob("**/infer.cfg"))
-        assert cfg_files, "You must provide a `infer.cfg` file."
+        cfg_files = list(cache_dir.glob("**/infer.json"))
+        assert cfg_files, "You must provide a `infer.json` file."
 
         cache_dir = cfg_files[0].parent
 
-        infer_cfg = load_json(cache_dir / "infer.cfg")
+        infer_cfg = load_json(cache_dir / "infer.json")
 
         # filters: 规则序列, preprocess: 参数序列, model: 配置字典, postprocess: 参数字典
         for key in ["filters", "preprocess", "model", "postprocess"]:
             if isinstance(infer_cfg[key], str):
                 infer_cfg[key] = load_json(cache_dir / infer_cfg[key])
 
         return infer_cfg, cache_dir
```

### Comparing `quant2-0.1.1/quant/football/models/stnet.py` & `quant2-0.1.2/quant/football/models/stnet.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/football/transforms/table20240326.py` & `quant2-0.1.2/quant/football/transforms/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/football/transforms/table20240410.py` & `quant2-0.1.2/quant/football/transforms/table20240410.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/football/transforms/table20240414.py` & `quant2-0.1.2/quant/football/transforms/table20240414.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     assert isinstance(encoder, dict), f"{type(encoder)=} is not <dict>."
 
     X, Y, Z = [], [], []
     for _season, _home, _away, _vals, _outs, _qkey in zip(season_id, team_home, team_away, features_in, scores, qkeys):
         if _season not in encoder["season"] or _home not in encoder["team"] or _away not in encoder["team"]:
             continue
 
+        # 进球,换人,黄牌,红牌,乌龙,点球,射失点球,两黄变红,视频裁判
         _home_score = sum([sum(_vals[i:sub_len:cycle_size]) for i in [0, 4, 5]])
         _away_score = sum([sum(_vals[sub_len:][i:sub_len:cycle_size]) for i in [0, 4, 5]])
         _curr_score = [_home_score + _away_score, _home_score, _away_score]  # 当前总进球数,主队进球数,客队进球数
 
         base_goals = _curr_score[0] if prediction_method == "incremental" else 0
 
         X.append(encoder["season"][_season] + encoder["team"][_home] + encoder["team"][_away] + _vals + _curr_score)
```

### Comparing `quant2-0.1.1/quant/layers/mlp.py` & `quant2-0.1.2/quant/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/layers/normalization.py` & `quant2-0.1.2/quant/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/layers/swiglu_ffn.py` & `quant2-0.1.2/quant/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/utils/archive.py` & `quant2-0.1.2/quant/utils/archive.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/utils/config.py` & `quant2-0.1.2/quant/utils/config.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/utils/io.py` & `quant2-0.1.2/quant/utils/io.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/quant/utils/logging.py` & `quant2-0.1.2/quant/utils/logging.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/tools/analysis_tools/analyze_cls_results.py` & `quant2-0.1.2/tools/analysis_tools/analyze_cls_results.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/tools/experimental/make_dataset.py` & `quant2-0.1.2/tools/experimental/make_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import quant
 from pathlib import Path
 from quant.football.data.utils import train_test
-from quant.football.transforms import table20240410 as table_factory
+from quant.football.transforms import table20240414 as table_factory
 from quant.utils.io import load_pkl, make_dir, save_json, save_pkl
 print(f"{quant.__version__=}")
 
 
-def make_datasets(file, date_min, date_sep, date_max, name_suffix, *preprocess_args):
+def make_datasets(file, date_min, date_sep, date_max, name_suffix, points, *preprocess_args):
     # 加载数据
     dataset = load_pkl(file)
     print(f"[1] {len(dataset)=}, {len(dataset[0])=}")
 
     # 检测得分数据是否对齐
     good_data, bad_data, bad_info = table_factory.check_samples(dataset)
     print(f"[2] {len(good_data)=}, {len(bad_data)=}, {bad_info[:3]}")
@@ -24,37 +24,47 @@
     print(f"[4] {len(train_data)=}")
 
     # 准备数据目录
     out_dir = Path(file).parent.as_posix() + name_suffix
     out_dir = make_dir(out_dir, exist_ok=False)
 
     # 转换并导出训练数据集(按需计算预处理参数)
-    X, Y, Z, *preprocess_args = table_factory.export_dataset(train_data, *preprocess_args)
+    if points is None:
+        X, Y, Z, *preprocess_args = table_factory.export_dataset(train_data, *preprocess_args)
+    else:
+        X, Y, Z, *preprocess_args = table_factory.export_dataset(train_data, points, *preprocess_args)
     print(f"[Train] save {len(X)} rows, {len(X[0])} cols")
     save_pkl(out_dir / "train.pkl", [X, Y, Z])
 
     # 转换并导出测试数据集(使用训练数据集的预处理参数)
-    X, Y, Z, *preprocess_args = table_factory.export_dataset(test_data, *preprocess_args)
+    if points is None:
+        X, Y, Z, *preprocess_args = table_factory.export_dataset(test_data, *preprocess_args)
+    else:
+        X, Y, Z, *preprocess_args = table_factory.export_dataset(test_data, points, *preprocess_args)
     print(f"[Test] save {len(X)} rows, {len(X[0])} cols")
     save_pkl(out_dir / "test.pkl", [X, Y, Z])
 
     # 打印编码器嵌入字典的大小
     encoder = preprocess_args[1]
     print(f"[Embedding] season {encoder['season']['__len__']}, team {encoder['team']['__len__']}")
 
     # 保存预处理参数
-    save_json(out_dir / "preprocess.cfg", preprocess_args)
+    save_json(out_dir / "preprocess.json", preprocess_args)
 
     return out_dir
 
 
 # 转换特征+拆分数据集+导出数据到文件
 file = "path_of_samples_file"
 
 date_min = "2023-01-01"
 date_sep = "2024-01-01"
 date_max = "2024-04-01"
 
 name_suffix = "_train_2301_2312_2403_s5_label_whole_c15_maxabs_direct"
+
+points = [i + 0.5 for i in range(15, 90)]
+points = None
+
 preprocess_args = [5, "label", True, 15, "maxabs", "direct"]
 
-make_datasets(file, date_min, date_sep, date_max, name_suffix, *preprocess_args)
+make_datasets(file, date_min, date_sep, date_max, name_suffix, points, *preprocess_args)
```

### Comparing `quant2-0.1.1/tools/experimental/make_split.py` & `quant2-0.1.2/tools/experimental/make_split.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/tools/experimental/nni_football.py` & `quant2-0.1.2/tools/experimental/nni_football.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     epochs = runtime.get("epochs", 90)
     device = runtime.get("device", "cuda")
     log_interval = runtime.get("log_interval", 10)
 
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    torch.backends.cudnn.deterministic = True
-    torch.backends.cudnn.benchmark = False
+    torch.backends.cudnn.deterministic = False
+    torch.backends.cudnn.benchmark = True
 
     if device == "cuda" and torch.cuda.is_available():
         device = torch.device("cuda")
     else:
         device = torch.device("cpu")
 
     dataset_type = data.pop("type")
@@ -114,18 +114,18 @@
     scheduler_type = scheduler.pop("type")
     if scheduler_type == "StepLR":
         from torch.optim.lr_scheduler import StepLR
         scheduler = StepLR(optimizer, **scheduler)
     else:
         raise NotImplementedError(f"Not supported <{scheduler_type}>.")
 
-    trial_name = f"{nni.get_experiment_id()}_{nni.get_sequence_id():04d}"
+    trial_name = time.strftime("%Y%m%d") + f"_{nni.get_experiment_id()}_{nni.get_sequence_id():04d}"
     out_dir = Path("runs") / data_root.name / trial_name
     out_dir.mkdir(parents=True, exist_ok=True)
-    copy_file(data_root, out_dir, "*.cfg")
+    copy_file(data_root, out_dir, "*.json")
 
     logger = get_logger(__name__, False, out_dir / "log.txt")
 
     best_acc, best_epoch = 0.0, -1
     for epoch in range(1, epochs + 1):
         train(model, device, train_loader, loss_fn, optimizer,
               epoch, log_interval, verbose, logger)
@@ -151,15 +151,15 @@
         "out_dir": str(out_dir),
         "date": time.strftime("%Y-%m-%d %H:%M:%S"),
         "best_acc": best_acc,
         "best_epoch": best_epoch,
         "last_acc_test": last_acc_test,
         "last_acc_train": last_acc_train,
     }
-    save_json(out_dir / "model.cfg", _cfg, indent=4)
+    save_json(out_dir / "model.json", _cfg, indent=4)
 
     return best_acc, _cfg
 
 
 if __name__ == "__main__":
     options = {}
     for arg in sys.argv[1:]:
```

### Comparing `quant2-0.1.1/tools/experimental/nni_football_config_search_space.json` & `quant2-0.1.2/tools/experimental/nni_football_config_search_space.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9055059523809526%*

 * *Differences: {"'data.batch_size'": "{'_value': {delete: [6, 4, 1, 0]}}",*

 * * "'data.data_root'": "{'_value': "*

 * *                     "['/datasets/table20240415_train_2301_2312_2403_lb_5_15_label_whole_c20_maxabs_direct']}",*

 * * "'model.drop'": "{'_type': 'choice', '_value': {insert: [(1, 0.1), (2, 0.2), (3, 0.3), (4, 0.5), "*

 * *                 '(5, 0.7)], delete: [1]}}',*

 * * "'model.hidden_features'": "{'_value': {insert: [(6, 640), (7, 768)], delete: [14, 13, 12, 10, 8, "*

 * *                            '6, 4, 2, 1, 0]}}',*

 * * "'model.in […]*

```diff
@@ -1,25 +1,21 @@
 {
     "data.batch_size": {
         "_type": "choice",
         "_value": [
-            32,
-            64,
             96,
             128,
-            160,
             192,
-            224,
             256
         ]
     },
     "data.data_root": {
         "_type": "choice",
         "_value": [
-            "/datasets/table20240410_2301to2403_train_2301_2312_2403_s5_label_whole_c15_maxabs"
+            "/datasets/table20240415_train_2301_2312_2403_lb_5_15_label_whole_c20_maxabs_direct"
         ]
     },
     "data.type": {
         "_type": "choice",
         "_value": [
             "FootballDatasetV2"
         ]
@@ -28,85 +24,87 @@
         "_type": "choice",
         "_value": [
             true,
             false
         ]
     },
     "model.drop": {
-        "_type": "uniform",
+        "_type": "choice",
         "_value": [
             0.0,
-            0.9
+            0.1,
+            0.2,
+            0.3,
+            0.5,
+            0.7
         ]
     },
     "model.enable_skip": {
         "_type": "choice",
         "_value": [
             true,
             false
         ]
     },
     "model.hidden_features": {
         "_type": "choice",
         "_value": [
-            32,
-            64,
-            96,
             128,
-            160,
             192,
-            224,
             256,
-            288,
             320,
-            352,
             384,
-            416,
-            448,
-            480,
-            512
+            512,
+            640,
+            768
         ]
     },
     "model.in_features": {
         "_type": "choice",
         "_value": [
-            128
+            122
         ]
     },
     "model.n_layers": {
-        "_type": "randint",
+        "_type": "choice",
         "_value": [
             1,
-            10
+            5,
+            10,
+            20
         ]
     },
     "model.out_features": {
         "_type": "choice",
         "_value": [
-            15
+            20
         ]
     },
     "model.season_embedding_dim": {
-        "_type": "randint",
+        "_type": "choice",
         "_value": [
+            3,
             5,
-            50
+            10
         ]
     },
     "model.season_embeddings": {
         "_type": "choice",
         "_value": [
             300
         ]
     },
     "model.team_embedding_dim": {
-        "_type": "randint",
+        "_type": "choice",
         "_value": [
             10,
-            150
+            30,
+            50,
+            70,
+            100
         ]
     },
     "model.team_embeddings": {
         "_type": "choice",
         "_value": [
             4000
         ]
@@ -116,26 +114,25 @@
         "_value": [
             "STNetV4"
         ]
     },
     "optimizer.lr": {
         "_type": "uniform",
         "_value": [
-            1e-05,
-            0.5
+            0.0002,
+            0.005
         ]
     },
     "optimizer.type": {
         "_type": "choice",
         "_value": [
-            "SGD",
             "AdamW"
         ]
     },
     "optimizer.weight_decay": {
         "_type": "uniform",
         "_value": [
-            1e-05,
-            0.5
+            0.0001,
+            0.05
         ]
     }
 }
```

### Comparing `quant2-0.1.1/tools/experimental/nni_model.py` & `quant2-0.1.2/tools/experimental/nni_model.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.1/tools/fb_cls_test.py` & `quant2-0.1.2/tools/fb_cls_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def test_dataset(test_file, checkpoint_dir, output_dir=None, device="cuda"):
     if device == "cuda" and torch.cuda.is_available():
         device = torch.device("cuda")
     else:
         device = torch.device("cpu")
 
     checkpoint_dir = Path(checkpoint_dir)
-    model_cfg = load_json(checkpoint_dir / "model.cfg")
+    model_cfg = load_json(checkpoint_dir / "model.json")
     model = load_model(model_cfg["model"], checkpoint_dir / "best.pt")
     model = model.to(device)
     model.eval()
 
     results, correct = [], 0
 
     suffix = Path(test_file).suffix
```

### Comparing `quant2-0.1.1/tools/fb_cls_train.py` & `quant2-0.1.2/tools/fb_cls_train.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,70 +96,78 @@
         loss_fn = CrossEntropyLoss(**loss).to(device)
     else:
         raise NotImplementedError(f"Not supported <{loss_type}>.")
 
     optimizer_type = optimizer.pop("type")
     if optimizer_type == "SGD":
         from torch.optim import SGD
+        optimizer.setdefault("momentum", 0.9)
         optimizer = SGD(model.parameters(), **optimizer)
     elif optimizer_type == "AdamW":
         from torch.optim import AdamW
+        optimizer.setdefault("betas", (0.9, 0.999))
+        if isinstance(optimizer["betas"], str):
+            optimizer["betas"] = eval(optimizer["betas"])
         optimizer = AdamW(model.parameters(), **optimizer)
     else:
         raise NotImplementedError(f"Not supported <{optimizer_type}>.")
 
     scheduler_type = scheduler.pop("type")
     if scheduler_type == "StepLR":
         from torch.optim.lr_scheduler import StepLR
         scheduler = StepLR(optimizer, **scheduler)
     else:
         raise NotImplementedError(f"Not supported <{scheduler_type}>.")
 
-    out_dir = Path("runs") / data_root.name / time.strftime("%Y%m%d%H%M%S")
+    trial_name = time.strftime("%Y%m%d%H%M%S")
+    out_dir = Path("runs") / data_root.name / trial_name
     out_dir.mkdir(parents=True, exist_ok=True)
-    copy_file(data_root, out_dir, "*.cfg")
+    copy_file(data_root, out_dir, "*.json")
 
     logger = get_logger(__name__, False, out_dir / "log.txt")
 
     best_acc, best_epoch = 0.0, -1
     for epoch in range(1, epochs + 1):
         train(model, device, train_loader, loss_fn, optimizer,
               epoch, log_interval, verbose, logger)
         curr_acc = test(model, device, test_loader, loss_fn,
                         verbose, logger)
         if curr_acc > best_acc:
             best_acc, best_epoch = curr_acc, epoch
             torch.save(model.state_dict(), out_dir / "best.pt")
         scheduler.step()
     torch.save(model.state_dict(), out_dir / "last.pt")
+    last_acc_test = curr_acc
 
     print_log("[best model]", verbose, logger)
     print_log(f"\noutput dir: {out_dir}", verbose, logger)
     print_log(f"{best_acc=:.4f}, {best_epoch=:03d}\n", verbose, logger)
 
     print_log("[check train dataset]", verbose, logger)
     check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=128)
-    acc_train = test(model, device, check_loader, loss_fn,
-                     verbose, logger)
+    last_acc_train = test(model, device, check_loader, loss_fn,
+                          verbose, logger)
 
     _cfg["log"] = {
         "out_dir": str(out_dir),
         "date": time.strftime("%Y-%m-%d %H:%M:%S"),
         "best_acc": best_acc,
         "best_epoch": best_epoch,
-        "acc_train": acc_train,
+        "last_acc_test": last_acc_test,
+        "last_acc_train": last_acc_train,
     }
-    save_json(out_dir / "model.cfg", _cfg, indent=4)
+    save_json(out_dir / "model.json", _cfg, indent=4)
 
     return best_acc, _cfg
 
 
 if __name__ == "__main__":
     options = {}
     for arg in sys.argv[1:]:
         key, val = arg.split("=", maxsplit=1)
         options[key] = eval(val)
 
     cfg = get_config(options.get("config", None))
     cfg = merge_from_dict(cfg, options)
 
-    main(cfg)
+    best_acc, _cfg = main(cfg, verbose=False)
+    print({"default": best_acc, "log": _cfg["log"]})
```

### Comparing `quant2-0.1.1/PKG-INFO` & `quant2-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant2
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: prettytable
 Requires-Dist: scikit-learn
```

