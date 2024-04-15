# Comparing `tmp/acetone-nnet-0.0.1.dev4.tar.gz` & `tmp/acetone_nnet-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone-nnet-0.0.1.dev4.tar", last modified: Fri Apr 12 13:34:30 2024, max compression
+gzip compressed data, was "acetone_nnet-0.0.1.dev5.tar", last modified: Mon Apr 15 06:51:47 2024, max compression
```

## Comparing `acetone-nnet-0.0.1.dev4.tar` & `acetone_nnet-0.0.1.dev5.tar`

### file list

```diff
@@ -1,81 +1,137 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.768263 acetone-nnet-0.0.1.dev4/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev4/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev4/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev4/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-12 13:34:30.767264 acetone-nnet-0.0.1.dev4/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.1.dev4/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1580 2024-04-12 13:34:24.000000 acetone-nnet-0.0.1.dev4/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-12 13:34:30.768263 acetone-nnet-0.0.1.dev4/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.755263 acetone-nnet-0.0.1.dev4/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.758263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1770 2024-04-12 12:00:11.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.760263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4055 2024-04-12 11:42:25.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1857 2024-04-12 09:31:09.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.762263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2768 2024-04-12 11:57:51.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/AddBias.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.763263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4317 2024-04-12 11:58:31.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3989 2024-04-12 11:57:49.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.764263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2986 2024-04-12 11:58:12.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6119 2024-04-12 11:50:48.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5332 2024-04-12 11:50:34.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5441 2024-04-12 11:50:07.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2964 2024-04-12 11:57:46.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4570 2024-04-12 11:57:44.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2371 2024-04-12 11:57:41.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3924 2024-04-12 11:57:39.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7997 2024-04-12 11:57:36.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2259 2024-04-12 11:57:16.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3189 2024-04-12 11:57:12.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.764263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3322 2024-04-12 11:49:27.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3743 2024-04-12 11:49:07.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3779 2024-04-12 11:48:34.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4011 2024-04-12 11:48:17.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.765263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4888 2024-04-12 11:57:59.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.766263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10445 2024-04-12 11:47:27.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4995 2024-04-12 11:47:33.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4264 2024-04-12 11:47:40.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2167 2024-04-12 11:57:31.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 09:52:53.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23576 2024-04-12 13:27:05.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.766263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.766263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.766263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17154 2024-04-12 12:33:03.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.766263 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3765 2024-04-12 06:47:10.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6008 2024-04-12 12:31:18.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.767264 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26621 2024-04-12 12:31:18.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.767264 acetone-nnet-0.0.1.dev4/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 13:34:30.767264 acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-12 13:34:30.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3254 2024-04-12 13:34:30.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-12 13:34:30.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-12 13:34:30.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-12 13:34:30.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-12 13:34:30.000000 acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.163144 acetone_nnet-0.0.1.dev5/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone_nnet-0.0.1.dev5/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.0.1.dev5/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.0.1.dev5/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-15 06:51:47.162144 acetone_nnet-0.0.1.dev5/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone_nnet-0.0.1.dev5/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1906 2024-04-15 06:51:28.000000 acetone_nnet-0.0.1.dev5/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-15 06:51:47.163144 acetone_nnet-0.0.1.dev5/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.743139 acetone_nnet-0.0.1.dev5/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.976142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1770 2024-04-12 12:00:11.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.980142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 06:45:47.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1852 2024-04-12 14:35:58.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.985142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/AddBias.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.987142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4324 2024-04-15 06:50:30.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.988142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2986 2024-04-15 06:50:24.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.989142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.989142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.990142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 06:49:26.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 09:52:53.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23719 2024-04-15 06:42:39.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.990142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.991142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.991142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17154 2024-04-12 12:33:03.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.991142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.992142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25232 2024-04-12 14:49:23.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:46.992142 acetone_nnet-0.0.1.dev5/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.027143 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.057143 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.108143 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.123144 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.125144 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.147144 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2122 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.155144 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.158144 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      689 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      741 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 06:51:47.162144 acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-15 06:51:46.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6328 2024-04-15 06:51:46.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-15 06:51:46.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-15 06:51:46.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-15 06:51:46.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-15 06:51:46.000000 acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone-nnet-0.0.1.dev4/COPYING` & `acetone_nnet-0.0.1.dev5/COPYING`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/LICENSE` & `acetone_nnet-0.0.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/PKG-INFO` & `acetone_nnet-0.0.1.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.1.dev4/README.md` & `acetone_nnet-0.0.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/pyproject.toml` & `acetone_nnet-0.0.1.dev5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = true
+
 [project]
 name = "acetone-nnet"
-version = "0.0.1.dev4"
+version = "0.0.1.dev5"
 requires-python = ">=3.10"
 
 authors = [
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
     { name="Claire PAGETTI", email="Claire.Pagetti@onera.fr" },
@@ -38,15 +41,22 @@
     "pystache==0.6.5",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-mypkg = ["*.txt"]
+acetone_nnet = ["templates/**.c.tpl",
+    "templates/normalization/*.c.tpl",
+    "templates/memory_layout/*.c.tpl",
+    "templates/layers/*.c.tpl",
+    "templates/layers/Resize/*.c.tpl",
+    "templates/layers/Pad/*.c.tpl",
+    "templates/layers/Gemm/*.c.tpl",
+    "templates/layers/Conv/*.c.tpl"]
 
 [project.scripts]
 cli-acetone = "acetone.src.cli_acetone:cli_acetone"
 cli_compare = "acetone.src.cli_compare:cli_compare"
 
 [project.urls]
 Repository = "https://github.com/onera/acetone/"
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/__init__.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/Layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,28 +16,30 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 import numpy as np
 from abc import ABC, abstractmethod
+from .. import templates
 
 class Layer(ABC):
     
     def __init__(self):
 
         self.idx = 0
         self.size = 0
         self.name = ''
         self.next_layer = [] 
         self.previous_layer = []
         self.path = None
         self.sorted = None
         self.output_str = ''
         self.fused_layer = None
+        self.template_path = templates.__file__[:-11]
       
         super().__init__()
 
     @abstractmethod
     def generate_inference_code_layer(self):
         pass
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,9 +36,9 @@
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
 
 __all__ = (
     "CodeGenerator",
     "ActivationFunctions", "Linear", "Sigmoid", "ReLu", "TanH", "Exponential", "Logarithm", "Clip",
     "Layer",
-    set(layers.__all__)
+    layers.__all__
 )
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         if(self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path)+'[i]',self.idx,'i')
 
-        with open('./templates/layers/template_AddBiase.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_AddBiase.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def forward_path_layer(self, input):
         input = input.reshape(self.previous_layer[0].size)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             previous_dict['input_width'] = self.input_shapes[k][3]
             previous_dict['input_height'] = self.input_shapes[k][2]
             previous_dict['input_channels'] = self.input_shapes[k][1]
             if(k != len(self.previous_layer) -1):
                 previous_dict['operator'] = self.specific_operator
             mustach_hash['broadcast'].append(previous_dict)
         
-        with open('./templates/layers/template_Broadcast.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Broadcast.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     @abstractmethod
     def forward_path_layer(self, inputs):
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             layer_to_concat['borne_sup'] = borne_sup
             layer_to_concat['borne_inf'] = borne_inf
             mustach_hash['concat'].append(layer_to_concat)
 
             borne_inf += self.input_shapes[k][self.axis]
 
 
-        with open('./templates/layers/template_Concatenate.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Concatenate.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def forward_path_layer(self, inputs):
         output = inputs[0]
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         mustach_hash['activation_function'] = self.activation_function.write_activation_str('output')
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output',self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Conv/template_Conv_gemm_nn.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_Conv_gemm_nn.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def write_gemm_nt(self, m, n, k, A, B, C, direct):
 
@@ -84,15 +84,15 @@
         mustach_hash['activation_function'] = self.activation_function.write_activation_str('output')
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output',self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Conv/template_Conv_gemm_nt.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_Conv_gemm_nt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def write_gemm_tn(self, m, n, k, A, B, C, direct):
 
@@ -113,15 +113,15 @@
         mustach_hash['activation_function'] = self.activation_function.write_activation_str('output')
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output',self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Conv/template_Conv_gemm_tn.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_Conv_gemm_tn.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def write_gemm_tt(self, m, n, k, A, B, C, direct):
 
@@ -142,12 +142,12 @@
         mustach_hash['activation_function'] = self.activation_function.write_activation_str('sum')
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path),self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Conv/template_Conv_gemm_tt.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_Conv_gemm_tt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,12 +93,12 @@
         gemm_code = self.algo_gemm_mapping[self.conv_algorithm](self.nb_filters, self.patches_width, self.patches_height, 'weights_' + self.name + '_' + str("{:02d}".format(self.idx)), 'ppatches_' + self.name + '_' + str("{:02d}".format(self.idx)), "output_"+str(self.path), True)
         mustach_hash['gemm_code'] = gemm_code
 
         if('cst' not in self.previous_layer[0].output_str):
             mustach_hash['cst'] = True
             mustach_hash['prev_size'] = self.input_channels*self.input_height*self.input_width
             
-        with open('./templates/layers/Conv/template_Conv_indirect_gemm.c.tpl', 'r') as template_file:
+        with open(self.template_path+'layers/Conv/template_Conv_indirect_gemm.c.tpl', 'r') as template_file:
             template = template_file.read()
         template_file.close()        
         
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         mustach_hash['pad_left'] = self.pad_left
         mustach_hash['input_height'] = self.input_height
         mustach_hash['input_width'] = self.input_width
         mustach_hash['road'] = self.path
         mustach_hash['patches_width'] = self.patches_width
         mustach_hash['output_str'] = output_str
 
-        with open('./templates/layers/Conv/template_im2col.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_im2col.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def write_im2row(self):
 
@@ -87,15 +87,15 @@
         mustach_hash['pad_left'] = self.pad_left
         mustach_hash['input_height'] = self.input_height
         mustach_hash['input_width'] = self.input_width
         mustach_hash['road'] = self.path
         mustach_hash['patches_width'] = self.patches_width
         mustach_hash['output_str'] = output_str
 
-        with open('./templates/layers/Conv/template_im2row.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_im2row.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def generate_inference_code_layer(self):
 
@@ -112,12 +112,12 @@
         mustach_hash['gemm_code'] = self.algo_gemm_mapping[self.conv_algorithm](self.nb_filters, self.patches_width, self.patches_height, 'weights_' + self.name + '_' + str("{:02d}".format(self.idx)), "output_"+str(self.path),'tensor_temp',False)
 
         if('cst' not in self.previous_layer[0].output_str):
             mustach_hash['cst'] = True
             mustach_hash['input_size'] = self.input_channels*self.input_height*self.input_width
         
 
-        with open('./templates/layers/Conv/template_Conv_std_gemm.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_Conv_std_gemm.c.tpl','r') as template_file:
             tempalte = template_file.read()
         template_file.close()
 
         return pystache.render(tempalte, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.local_var,self.idx,'i')
 
             if(self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
         
-        with open('./templates/layers/template_Dense.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Dense.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def forward_path_layer(self, input):
         input = input.reshape(self.previous_layer[0].size)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         if(self.axis[1] == 2):
             mustach_hash['indice_right'] = 'k + '+ str(self.input_shapes[1][self.axis[1]]) + ' * (j + ' + str(self.output_width) + ' * i)'
         elif(self.axis[1] == 1):
             mustach_hash['indice_right'] = 'j + '+ str(self.output_width) + ' * (k + ' + str(self.input_shapes[1][self.axis[1]]) + ' * i)'
         elif(self.axis[1] == 0):
             mustach_hash['indice_right'] = 'j + '+ str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * k)'
         
-        with open('./templates/layers/template_Dot.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Dot.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def forward_path_layer(self, inputs):
         inputs[0] = inputs[0].reshape(self.input_shapes[0][1],self.input_shapes[0][2],self.input_shapes[0][3])
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             mustach_hash['input_height'] = self.input_shape[2]
             mustach_hash['input_width'] = self.input_shape[3]
             mustach_hash['name'] = self.name
             mustach_hash['idx'] = "{:02d}".format(self.idx)
             mustach_hash['path'] = self.path
             mustach_hash['size'] = self.size
 
-        with open('./templates/layers/template_Flatten.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Flatten.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def forward_path_layer(self, input):
         if(self.data_format == 'channels_last'):
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         if(self.activation_function.name == 'linear'):
             mustach_hash['linear'] = True
 
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tensor_temp[position]',self.idx,'position')
 
-        with open('./templates/layers/template_Gather.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Gather.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
         
     def forward_path_layer(self,input):
         input = input.reshape(self.input_channels,self.input_height,self.input_width)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         mustach_hash['beta'] = self.beta
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output',self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Gemm/template_gemm_nn.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Gemm/template_gemm_nn.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def write_gemm_nt(self, m, n, k, A, B):
 
@@ -105,15 +105,15 @@
         mustach_hash['beta'] = self.beta
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output',self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Gemm/template_gemm_nt.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Gemm/template_gemm_nt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def write_gemm_tn(self, m, n, k, A, B):
 
@@ -131,15 +131,15 @@
         mustach_hash['beta'] = self.beta
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output',self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Gemm/template_gemm_tn.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Gemm/template_gemm_tn.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def write_gemm_tt(self, m, n, k, A, B):
 
@@ -157,15 +157,15 @@
         mustach_hash['beta'] = self.beta
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path),self.idx,'i*'+str(self.ldC)+' + j')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
 
-        with open('./templates/layers/Gemm/template_gemm_tt.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Gemm/template_gemm_tt.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def forward_path_layer(self,input):
         input = input.reshape(self.input_height,self.input_width)
@@ -183,12 +183,12 @@
         mustach_hash['comment'] = self.activation_function.comment
         mustach_hash['size'] = self.size
         mustach_hash['road'] = self.path
 
         mustach_hash['patches_size'] = self.output_width*self.output_height
         mustach_hash['gemm_code'] = self.algo_gemm_mapping[self.transpo](self.output_height, self.output_width, self.input_width, 'weights_' + self.name + '_' + str("{:02d}".format(self.idx)), self.previous_layer[0].output_str)
 
-        with open('./templates/layers/Gemm/template_Gemm.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Gemm/template_Gemm.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             mustach_hash['input_width'] = self.input_shape[3]
         else:
             mustach_hash['size'] = self.size
 
 
 
 
-        with open('./templates/layers/template_Input_Layer.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Input_Layer.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def forward_path_layer(self, input):
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.local_var,self.idx,'i')
 
             if(self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
         
-        with open('./templates/layers/template_MatMul.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_MatMul.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
         
     def forward_path_layer(self, input):
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,13 +60,13 @@
 
         if(self.activation_function.name == 'linear'):
             mustach_hash['linear'] = True
         
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
 
-        with open('./templates/layers/Pad/template_Constant_Pad.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Pad/template_Constant_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,38 +13,42 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
+
 from .Pad import Pad
 
 import pystache
 
-#The Edge mode of the Pad layers
-#Pads with the edge values of array.
-class Edge_pad(Pad):
+#The Wrap mode of the Pad layers
+#Pads with the wrap of the vector along the axis. 
+#The first values are used to pad the end and the end values are used to pad the beginning.
+class Wrap_pad(Pad):
+    
+    def __init__(self, idx, size, mode, pads, constant_value, axes, input_shape):
+        super().__init__(idx, size, mode, pads, constant_value, axes, input_shape)
+        self.mode = 'wrap'
     
-    def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
-        super().__init__(idx, size, pads, constant_value, axes, input_shape,activation_function)
-        self.mode = 'edge'
-
-
     def write_padding(self):
         mustach_hash = {}
 
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
         mustach_hash['pads_left'] = self.pads[3]
         mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
         mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
         mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
-
-        with open('./templates/layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
+        mustach_hash['input_channels'] = self.input_shape[1]
+        mustach_hash['input_width'] = self.input_shape[3]
+        mustach_hash['input_height'] = self.input_shape[2]
+        
+        with open(self.template_path+'layers/Pad/template_Wrap_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
 
     def generate_inference_code_layer(self):
@@ -75,12 +79,12 @@
 
         if(self.activation_function.name == 'linear'):
             mustach_hash['linear'] = True
         
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
 
-        with open('./templates/layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
         mustach_hash['pads_left'] = self.pads[3]
         mustach_hash['channels_max'] = self.input_shape[1] - 1
         mustach_hash['height_max'] = self.input_shape[2] - 1
         mustach_hash['width_max'] = self.input_shape[3] - 1
         
-        with open('./templates/layers/Pad/template_Reflect_Pad.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Pad/template_Reflect_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
 
     def generate_inference_code_layer(self):
@@ -75,12 +75,12 @@
 
         if(self.activation_function.name == 'linear'):
             mustach_hash['linear'] = True
         
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
 
-        with open('./templates/layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,42 +13,38 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
-
 from .Pad import Pad
 
 import pystache
 
-#The Wrap mode of the Pad layers
-#Pads with the wrap of the vector along the axis. 
-#The first values are used to pad the end and the end values are used to pad the beginning.
-class Wrap_pad(Pad):
-    
-    def __init__(self, idx, size, mode, pads, constant_value, axes, input_shape):
-        super().__init__(idx, size, mode, pads, constant_value, axes, input_shape)
-        self.mode = 'wrap'
+#The Edge mode of the Pad layers
+#Pads with the edge values of array.
+class Edge_pad(Pad):
     
+    def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
+        super().__init__(idx, size, pads, constant_value, axes, input_shape,activation_function)
+        self.mode = 'edge'
+
+
     def write_padding(self):
         mustach_hash = {}
 
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
         mustach_hash['pads_left'] = self.pads[3]
         mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
         mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
         mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
-        mustach_hash['input_channels'] = self.input_shape[1]
-        mustach_hash['input_width'] = self.input_shape[3]
-        mustach_hash['input_height'] = self.input_shape[2]
-        
-        with open('./templates/layers/Pad/template_Wrap_Pad.c.tpl','r') as template_file:
+
+        with open(self.template_path+'layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
 
     def generate_inference_code_layer(self):
@@ -79,12 +75,12 @@
 
         if(self.activation_function.name == 'linear'):
             mustach_hash['linear'] = True
         
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tenser_temp[j + ' + str(self.output_width) + ' * (i + ' + str(self.output_height) + ' * f)]')
 
-        with open('./templates/layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Pad/template_Pad_Non_Constant.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.output_var,self.idx,'j + '+str(self.output_width)+'*(i + '+str(self.output_height)+'*f)')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
         
-        with open('./templates/layers/template_Pooling2D.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Pooling2D.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     def forward_path_layer(self, input):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 #The Cubic mode of the Resize layers
 #Use a (bi)cubic interpolation to find the new value
 class ResizeCubic(Resize):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode = 'cubic'
-        self.template_dict = {'1D':'./templates/layers/Resize/template_ResizeCubic1D.c.tpl',
-                              '2D':'./templates/layers/Resize/template_ResizeCubic2D.c.tpl'}
+        self.template_dict = {'1D':self.template_path+'layers/Resize/template_ResizeCubic1D.c.tpl',
+                              '2D':self.template_path+'layers/Resize/template_ResizeCubic2D.c.tpl'}
     
     def forward_path_layer(self, input):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
         input= np.transpose(input,(1,2,0))#Function resize in tensorflow take a format channel last
         output = tf.image.resize(input, [self.output_height,self.output_width], method='bicubic') #No numpy method for this layer
         output= np.transpose(output,(2,0,1))
         return self.activation_function.compute(output)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 #The mode Linear of the Resize layers
 #The value in the output tensor are found thanks to a (bi)linear interpolation
 class ResizeLinear(Resize):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode = 'linear'
-        self.template_dict = {'1D':'./templates/layers/Resize/template_ResizeLinear1D.c.tpl',
-                              '2D':'./templates/layers/Resize/template_ResizeLinear2D.c.tpl'}
+        self.template_dict = {'1D':self.template_path+'layers/Resize/template_ResizeLinear1D.c.tpl',
+                              '2D':self.template_path+'layers/Resize/template_ResizeLinear2D.c.tpl'}
         
     def generate_inference_code_layer(self):
 
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         mustach_hash['coordinate_transformation_mode_y'] = self.coordinate_transformation_mode_mapping[self.coordinate_transformation_mode]('j',3,'y')
         mustach_hash['nearest_mode_x'] = self.nearest_mode_mapping[self.nearest_mode]('x0','x')
         mustach_hash['nearest_mode_y'] = self.nearest_mode_mapping[self.nearest_mode]('y0','y')
 
         if(self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('tensor_temp[j + ' + str(self.output_width) + '*(i + ' + str(self.output_height) + '*f)]',self.idx,'j + ' + str(self.output_width) + '*(i + ' + str(self.output_height) + '*f)')
 
-        with open('./templates/layers/Resize/template_ResizeNearest.c.tpl') as template_file:
+        with open(self.template_path+'layers/Resize/template_ResizeNearest.c.tpl') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)    
     
     def forward_path_layer(self, input):
         input = input.reshape(self.input_channels, self.input_height, self.input_width)
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         mustach_hash['size'] = self.size
         mustach_hash['road'] = self.path
         mustach_hash['output_str'] = output_str
 
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path)+'[j]', self.idx, 'j')
 
-        with open('./templates/layers/template_Softmax.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def forward_path_layer(self, input):
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 import os
 import numpy as np
 from pathlib import Path
 from abc import ABC
 import pystache
 
+from .. import templates
+
 from ..format_importer.parser import parser
 
 from .layers import (
     Dense, Dot, Softmax, Gather, Gemm, MatMul, Concatenate, Pad, Broadcast,
     ResizeLinear, ResizeCubic, ResizeNearest, 
     Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pooling2D, MaxPooling2D, AveragePooling2D
@@ -39,14 +41,15 @@
 
         self.file = file
         self.test_dataset_file = test_dataset_file
         self.function_name = function_name
         self.nb_tests = nb_tests
         self.conv_algorithm = conv_algorithm
         self.normalize = normalize
+        self.template_path = templates.__file__[:-11]
 
         if (not self.normalize):
             l, dtype, dtype_py, data_format, maxpath, dict_cst = parser(self.file, self.conv_algorithm)
         elif(self.normalize):
             l, dtype, dtype_py, data_format, maxpath, dict_cst, Normalizer = parser(self.file, self.conv_algorithm, self.normalize)
             self.Normalizer = Normalizer
         
@@ -201,15 +204,15 @@
         return s
 
     def generate_testdataset_files(self):
 
         testdataset_header = open(self.c_files_directory + '/test_dataset.h' , "w+")
         testdataset_source = open(self.c_files_directory + '/test_dataset.c' , "w+")
 
-        with open('./templates/template_test_dataset_header.c.tpl','r') as template_file:
+        with open(self.template_path+'template_test_dataset_header.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         testdataset_header.write(pystache.render(template, {'nb_tests':self.nb_tests, 'nb_inputs':self.layers[0].size, 'nb_outputs':self.layers[-1].size, 'data_type':self.data_type}))
 
         dataset = '{'
         if self.test_dataset is None:
@@ -217,38 +220,38 @@
         else:
             for j in range(self.test_dataset.shape[0]):
                 dataset += self.flatten_array_orderc(self.test_dataset[j]) +','
             dataset = dataset[:-1]
         
         dataset += '};\n'
 
-        with open('./templates/template_test_dataset_source.c.tpl','r') as template_file:
+        with open(self.template_path+'template_test_dataset_source.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         testdataset_source.write(pystache.render(template,{'data_type':self.data_type, 'dataset':dataset}))
 
     def generate_main_file(self):
 
-        with open('./templates/template_main_file.c.tpl','r') as template_file:
+        with open(self.template_path+'template_main_file.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         self.main_file.write(pystache.render(template, {'data_type':self.data_type}))
 
     def generate_makefile(self):
 
         header_files = []
         source_files = []
         for filename in self.files_to_gen:
             if '.c' in filename : source_files.append(filename)
             elif '.h' in filename : header_files.append(filename)
             else : pass
 
-        with open('./templates/template_Makefile.tpl','r') as template_file:
+        with open(self.template_path+'template_Makefile.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         self.makefile.write(pystache.render(template, {'source_files':' '.join(source_files), 'header_files':' '.join(header_files), 'function_name':self.function_name}))
 
     def generate_c_files(self, c_files_directory):  
 
@@ -343,34 +346,34 @@
         output_hash = {}
         output_hash['path'] = self.layers[-1].path
         if ((self.data_format == 'channels_last') and (hasattr(self.layers[-1],'output_channels'))):
             output_hash['output_channels'] = self.layers[-1].output_channels
             output_hash['output_height'] = self.layers[-1].output_height
             output_hash['output_width'] = self.layers[-1].output_width
 
-            with open('./templates/memory_layout/template_channels_last_output.c.tpl','r') as template_file:
+            with open(self.template_path+'memory_layout/template_channels_last_output.c.tpl','r') as template_file:
                 template = template_file.read()
             template_file.close()
             mustach_hash['ouput_str'] = pystache.render(template, output_hash)
 
         else:
             output_hash['output_size'] = self.layers[-1].size
             if((self.data_format == 'channels_first')):
                 output_hash['comment'] = 'Returning the output in channels first (ACETONE compute the result in channels first)'
             else:
                 output_hash['comment'] = 'Returning the output (output flatten)'
             
-            with open('./templates/memory_layout/template_channels_first_output.c.tpl','r') as template_file:
+            with open(self.template_path+'memory_layout/template_channels_first_output.c.tpl','r') as template_file:
                 template = template_file.read()
             template_file.close()
             mustach_hash['ouput_str'] = pystache.render(template, output_hash)
             
 
 
-        with open('./templates/template_source_file.c.tpl', 'r') as template_file:
+        with open(self.template_path+'template_source_file.c.tpl', 'r') as template_file:
             template = template_file.read()
         template_file.close()
 
         if(self.normalize):
             mustach_hash['pre_processing'] = self.Normalizer.write_pre_processing()
             mustach_hash['post_processing'] = self.Normalizer.write_post_processing()
         
@@ -439,15 +442,15 @@
             
             if (to_print):
                 mustach_hash['layers'].append(layer_hash)
         
         if(self.normalize):
             mustach_hash['normalization_cst'] = self.Normalizer.write_normalization_cst_in_header_file()
         
-        with open('./templates/template_header_file.c.tpl', 'r') as template_file:
+        with open(self.template_path+'template_header_file.c.tpl', 'r') as template_file:
             template = template_file.read()
         template_file.close()
 
         self.header_file.write(pystache.render(template,mustach_hash))
     
     def generate_globalvars_file(self):
 
@@ -504,15 +507,15 @@
                 layer_hash['patches_size'] = layer.patches_size
                 layer_hash['patches'] = layer.create_ppatches()
                 to_print = True
             
             if (to_print):
                 mustach_hash['layers'].append(layer_hash)
         
-        with open('./templates/template_global_var_file.c.tpl', 'r') as template_file:
+        with open(self.template_path+'template_global_var_file.c.tpl', 'r') as template_file:
             template = template_file.read()
         template_file.close()
 
         self.globalvars_file.write(pystache.render(template,mustach_hash))
 
         if(self.normalize):
             self.globalvars_file.write(self.Normalizer.write_normalization_cst_in_globalvars_file())
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,54 +17,56 @@
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 import pystache
 import numpy as np
 from abc import ABC
+from ... import templates
 
 class Normalizer(ABC):
 
     def __init__(self, input_size, output_size, mins, maxes, means, ranges):
         self.input_size = input_size
         self.output_size = output_size
         self.mins = mins
         self.maxes = maxes
         self.means = means
         self.ranges = ranges
+        self.template_path = templates.__file__[:-11]
         super().__init__()
 
     def array_to_str(self,array):
         s = "{"
         for element in array:
             s += str(element) + ", "
         s = s[:-2] + "}"
         return s
 
     def write_pre_processing(self):
-        with open('./templates/normalization/template_pre_processing.c.tpl','r') as template_file:
+        with open(self.template_path+'normalization/template_pre_processing.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template,{'input_size':self.input_size})
 
 
     def write_post_processing(self):
-        with open('./templates/normalization/template_post_processing.c.tpl','r') as template_file:
+        with open(self.template_path+'normalization/template_post_processing.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template,{'output_size':self.output_size})
 
     def write_normalization_cst_in_header_file(self):
         mustach_hash= {}
 
         mustach_hash['input_size'] = self.input_size
 
-        with open('./templates/normalization/template_normalization_cst_in_header_file.c.tpl','r') as template_file:
+        with open(self.template_path+'normalization/template_normalization_cst_in_header_file.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
     def write_normalization_cst_in_globalvars_file(self):
         mustach_hash= {}
@@ -73,15 +75,15 @@
         mustach_hash['input_min'] = self.array_to_str(self.mins)
         mustach_hash['input_max'] = self.array_to_str(self.maxes)
         mustach_hash['input_mean'] = self.array_to_str(self.means[:-1])
         mustach_hash['input_range'] = self.array_to_str(self.ranges[:-1])
         mustach_hash['output_mean'] = self.means[-1]
         mustach_hash['output_range'] = self.ranges[-1]
 
-        with open('./templates/normalization/template_normalization_cst_in_global_var_file.c.tpl','r') as template_file:
+        with open(self.template_path+'normalization/template_normalization_cst_in_global_var_file.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return  pystache.render(template, mustach_hash)
 
     def pre_processing(self, nn_input):
         inputs = nn_input.flatten()
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 
 
 import tensorflow as tf
 import numpy as np
 
 from . import nnet_normalize
 
-from ...code_generator.layers.Dense import Dense
-from ...code_generator.layers.Input import InputLayer
+from ...code_generator.layers import Dense, InputLayer
 from ...code_generator.activation_functions import Linear, ReLu
 
 tf.keras.backend.set_floatx('float32')
 
 
 def load_nnet(file_to_parse, normalize):
     """
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,56 +18,58 @@
  ******************************************************************************
 """
 
 
 import numpy as np
 import onnx
 
-from ...code_generator.layers.Pooling_layers import AveragePooling2D, MaxPooling2D
-from ...code_generator.layers.Conv_layers import Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm 
-from ...code_generator.layers.Pad_layers import EdgePad, WrapPad, ReflectPad, ConstantPad
-from ...code_generator.layers.Broadcast_layers import Add, Multiply, Subtract, Divide, Maximum, Minimum, Average
-from ...code_generator.layers.Resize_layers import ResizeCubic, ResizeLinear, ResizeNearest
-from ...code_generator.layers import  Concatenate, Input, Softmax,  Dot, Gather, Gemm, MatMul, AddBias
+from ...code_generator.layers import (
+    AveragePooling2D, MaxPooling2D,
+    Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
+    Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
+    Add, Multiply, Subtract, Divide, Maximum, Minimum, Average,
+    ResizeCubic, ResizeLinear, ResizeNearest,
+    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias
+)
 
-from ...code_generator import activation_functions
+from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm
 
 ###### Utility functions ######
 
 def create_conv2d_obj(algorithm, **kwargs):
        
     if '6loops' in algorithm:
-        return Conv2D_6loops.Conv2D_6loops(**kwargs)
+        return Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
-        return Conv2D_std_gemm.Conv2D_std_gemm(**kwargs)   
+        return Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
-        return Conv2D_indirect_gemm.Conv2D_indirect_gemm(**kwargs)
+        return Conv2D_indirect_gemm(**kwargs)
         
 
 def create_resize_obj(mode, **kwargs):
     if mode == b'nearest':
-        return ResizeNearest.ResizeNearest(**kwargs)
+        return ResizeNearest(**kwargs)
     
     elif mode == b'linear':
-        return ResizeLinear.ResizeLinear(**kwargs)
+        return ResizeLinear(**kwargs)
     
     elif mode == b'cubic':
-        return ResizeCubic.ResizeCubic(**kwargs)
+        return ResizeCubic(**kwargs)
 
 def create_pad_obj(mode, **kwargs):
     if mode == b'constant':
-        return ConstantPad.Constant_Pad(**kwargs)
+        return Constant_Pad(**kwargs)
     elif mode == b'edge':
-        return EdgePad.Edge_pad(**kwargs)
+        return Edge_pad(**kwargs)
     elif mode == b'wrap':
-        return WrapPad.Wrap_pad(**kwargs)
+        return Wrap_pad(**kwargs)
     elif mode == b'reflect':
-        return ReflectPad.Reflect_pad(**kwargs)
+        return Reflect_pad(**kwargs)
 
 #Go find the constant named initialzer_name in model(an onnx model)
 def look_for_initializer(initializer_name,model):
     if (initializer_name == ''):
         return []
     for initializer in model.graph.initializer:
         if (initializer.name == initializer_name):
@@ -115,23 +117,23 @@
 
 #Create an input layers 
 def create_Input_Layer(input_layer,idx,dict_output):
         dict_output[input_layer.name] = idx
         output_shape = [input_layer.type.tensor_type.shape.dim[i].dim_value for i in range(len(input_layer.type.tensor_type.shape.dim))]
         size = find_size(output_shape)
         
-        return Input.InputLayer(idx,size,output_shape,'channels_first')
+        return InputLayer(idx,size,output_shape,'channels_first')
 
 #Create a layer Softmax
 def create_Softmax(node,idx,dict_input,dict_output,model):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Softmax.Softmax(idx = idx,
+    return Softmax(idx = idx,
                             size = size)
 
 
 #Create a layer Conv
 def create_Conv(node,idx,dict_input,dict_output,model,conv_algorithm):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
@@ -164,33 +166,33 @@
                                 kernel_w= attributs['kernel_shape'][1], 
                                 dilation_rate= attributs['dilations'], 
                                 nb_filters= initializers[0].dims[0],
                                 input_shape= input_shape, 
                                 output_shape= output_shape,
                                 weights= np.moveaxis(onnx.numpy_helper.to_array(initializers[0]), 0,3),
                                 biases= biases,
-                                activation_function= activation_functions.Linear())
+                                activation_function= Linear())
     
 
 #Create a layer Concat
 def create_Concat(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
-    return Concatenate.Concatenate(idx,
-                                size, 
-                                attributs['axis'],
-                                input_shapes,
-                                output_shape,
-                                activation_function= activation_functions.Linear())
+    return Concatenate(idx,
+                        size, 
+                        attributs['axis'],
+                        input_shapes,
+                        output_shape,
+                        activation_function= Linear())
     
 #Create a layer Resize
 def create_Resize(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
@@ -236,15 +238,15 @@
                              keep_aspect_ratio_policy = attributs['keep_aspect_ratio_policy'],
                              target_size = targ_size,
                              boolean_resize = bool_resize,
                              roi = roi,
                              extrapolation_value = attributs['extrapolation_value'],
                              nearest_mode = attributs['nearest_mode'],
                              cubic_coeff_a=attributs['cubic_coeff_a'],
-                             activation_function = activation_functions.Linear())
+                             activation_function = Linear())
     
 #create a layer Pad
 def create_Pad(node,idx,dict_input,dict_output,model):
     axes = []
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
@@ -259,33 +261,33 @@
     return create_pad_obj(mode = attributs['mode'],
                           idx = idx,
                           size = size,
                           pads = onnx.numpy_helper.to_array(initializers[0]),
                           constant_value = onnx.numpy_helper.to_array(initializers[1]),
                           axes = axes,
                           input_shape = input_shape,
-                          activation_function = activation_functions.Linear())
+                          activation_function = Linear())
 
 
 #create a layer Gather
 def create_Gather(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     initializer = look_for_initializer(node.input[1],model)
-    return Gather.Gather(idx = idx,
-                         size = size,
-                         axis = attributs['axis'],
-                         indices = onnx.numpy_helper.to_array(initializer),
-                         input_shape = input_shape,
-                         output_shape = output_shape,
-                         activation_function = activation_functions.Linear())
+    return Gather(idx = idx,
+                    size = size,
+                    axis = attributs['axis'],
+                    indices = onnx.numpy_helper.to_array(initializer),
+                    input_shape = input_shape,
+                    output_shape = output_shape,
+                    activation_function = Linear())
 
 #create a layer Gemm
 def create_Gemm(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
@@ -300,25 +302,25 @@
         attributs['transA'] = 0
     if('transB' not in attributs):
         attributs['transB'] = 0
     if('alpha' not in attributs):
         attributs['alpha'] = 1.0
     if('beta' not in attributs):
         attributs['beta'] = 1.0
-    return Gemm.Gemm(idx = idx,
-                       size = size,
-                       alpha = attributs['alpha'],
-                       beta = attributs['beta'],
-                       transA = attributs['transA'],
-                       transB = attributs['transB'],
-                       weights = onnx.numpy_helper.to_array(B_tensor),
-                       bias = onnx.numpy_helper.to_array(C_tensor),
-                       input_shape = input_shape,
-                       output_shape = output_shape,
-                       activation_function = activation_functions.Linear())
+    return Gemm(idx = idx,
+                size = size,
+                alpha = attributs['alpha'],
+                beta = attributs['beta'],
+                transA = attributs['transA'],
+                transB = attributs['transB'],
+                weights = onnx.numpy_helper.to_array(B_tensor),
+                bias = onnx.numpy_helper.to_array(C_tensor),
+                input_shape = input_shape,
+                output_shape = output_shape,
+                activation_function = Linear())
 
 def create_MatMul(node,idx,dict_input,dict_output,model):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_output[node.output[0]] = idx
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
@@ -334,32 +336,32 @@
         if(left_tensor and not right_tensor):
             #the weigth is the right tensor:  MatMul(W,T)
             side = False
             weights = onnx.numpy_helper.to_array(left_tensor)
             weights = np.reshape(weights, (1,1,get_shape(node.input[0],model)[-1],output_shape[-1]))
             dict_input[idx] = [node.input[0]]
             input_shape = get_shape(node.input[0],model)
-        return MatMul.MatMul(idx = idx,
-                             size = size,
-                             input_shape = input_shape,
-                             weights = weights,
-                             side = side,
-                             activation_function = activation_functions.Linear())
+        return MatMul(idx = idx,
+                        size = size,
+                        input_shape = input_shape,
+                        weights = weights,
+                        side = side,
+                        activation_function = Linear())
     else:
         dict_input[idx] = node.input
         input_shapes =[]
         for input in node.input:
             input_shapes.append(get_shape(input,model))
         # to check
-        return Dot.Dot(idx = idx,
-                       size = size,
-                       axis = [-1,-2],
-                       input_shapes = input_shapes,
-                       output_shape = output_shape,
-                       activation_function = activation_functions.Linear())
+        return Dot(idx = idx,
+                    size = size,
+                    axis = [-1,-2],
+                    input_shapes = input_shapes,
+                    output_shape = output_shape,
+                    activation_function = Linear())
 
 ### Pooling layers ###
 
 #Create a layer MaxPool
 def create_MaxPool(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
@@ -369,22 +371,22 @@
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
         attributs['dilations'] = 1
     if (('auto_pad' not in attributs) or ( attributs['auto_pad'] == 'NOTSET')):
         attributs['auto_pad'] = attributs['pads']
     if ('strides' not in attributs):
         attributs['strides'] = [1,1]
-    return MaxPooling2D.MaxPooling2D(idx = idx,
-                                size = size,
-                                padding =attributs['auto_pad'],
-                                strides = attributs['strides'][0],
-                                pool_size = attributs['kernel_shape'][0],
-                                input_shape = input_shape,
-                                output_shape = output_shape,
-                                activation_function = activation_functions.Linear())
+    return MaxPooling2D(idx = idx,
+                        size = size,
+                        padding =attributs['auto_pad'],
+                        strides = attributs['strides'][0],
+                        pool_size = attributs['kernel_shape'][0],
+                        input_shape = input_shape,
+                        output_shape = output_shape,
+                        activation_function = Linear())
 
 #cerate a layer AveragePool
 def create_AveragePool(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
@@ -392,38 +394,38 @@
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
         attributs['dilations'] = 1
     if (('auto_pad' not in attributs) or ( attributs['auto_pad'] == 'NOTSET')):
         attributs['auto_pad'] = attributs['pads']
     if ('strides' not in attributs):
         attributs['strides'] = [1,1]
-    return AveragePooling2D.AveragePooling2D(idx=idx,
-                                   size=size, 
-                                   padding=attributs['auto_pad'],
-                                   strides=attributs['strides'][0], 
-                                   pool_size=attributs['kernel_shape'][0], 
-                                   input_shape=input_shape,
-                                   output_shape=output_shape,
-                                   activation_function = activation_functions.Linear())
+    return AveragePooling2D(idx=idx,
+                            size=size, 
+                            padding=attributs['auto_pad'],
+                            strides=attributs['strides'][0], 
+                            pool_size=attributs['kernel_shape'][0], 
+                            input_shape=input_shape,
+                            output_shape=output_shape,
+                            activation_function = Linear())
 
 #Create a layer GlobalAveragePool
 def create_GlobalAveragePool(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return AveragePooling2D.AveragePooling2D(idx = idx,
-                                    size = size,
-                                    padding = [0,0,0,0],
-                                    strides = 0,
-                                    pool_size = input_shape[2],
-                                    input_shape = input_shape,
-                                    output_shape = output_shape,
-                                    activation_function = activation_functions.Linear())
+    return AveragePooling2D(idx = idx,
+                            size = size,
+                            padding = [0,0,0,0],
+                            strides = 0,
+                            pool_size = input_shape[2],
+                            input_shape = input_shape,
+                            output_shape = output_shape,
+                            activation_function = Linear())
 
 ### Broadcats layers ###
 
 #create a layer Add
 def create_Add(node,idx,dict_input,dict_output,model):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
@@ -431,120 +433,120 @@
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
     if(not right_tensor and not left_tensor):
         input_shapes =[]
         for input in node.input:
             input_shapes.append(get_shape(input,model))
         dict_input[idx] = node.input
-        return Add.Add(idx=idx,
-                        size=size,
-                        input_shapes=input_shapes,
-                        output_shape=output_shape,
-                        activation_function= activation_functions.Linear())
+        return Add(idx=idx,
+                    size=size,
+                    input_shapes=input_shapes,
+                    output_shape=output_shape,
+                    activation_function= Linear())
     else:
         if(right_tensor):
             biases = onnx.numpy_helper.to_array(right_tensor)
             dict_input[idx] = [node.input[1]]
         elif(left_tensor):
             biases = onnx.numpy_helper.to_array(left_tensor)
             dict_input[idx] = [node.input[0]]
-        return AddBias.Add_Bias(idx = idx,
-                                  size = size,
-                                  biases = biases,
-                                  activation_function = activation_functions.Linear())
+        return Add_Bias(idx = idx,
+                            size = size,
+                            biases = biases,
+                            activation_function = Linear())
     
 #create a layer Div
 def create_Div(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Divide.Divide(idx=idx,
-                      size=size,
-                      input_shapes=input_shapes,
-                      output_shape=output_shape,
-                      activation_function= activation_functions.Linear())
+    return Divide(idx=idx,
+                    size=size,
+                    input_shapes=input_shapes,
+                    output_shape=output_shape,
+                    activation_function= Linear())
 
 #create a layer Mul
 def create_Mul(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Multiply.Multiply(idx=idx,
-                      size=size,
-                      input_shapes=input_shapes,
-                      output_shape=output_shape,
-                      activation_function= activation_functions.Linear())
+    return Multiply(idx=idx,
+                    size=size,
+                    input_shapes=input_shapes,
+                    output_shape=output_shape,
+                    activation_function= Linear())
 
 #create a layer Sub
 def create_Sub(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Subtract.Subtract(idx=idx,
-                      size=size,
-                      input_shapes=input_shapes,
-                      output_shape=output_shape,
-                      activation_function= activation_functions.Linear())
+    return Subtract(idx=idx,
+                    size=size,
+                    input_shapes=input_shapes,
+                    output_shape=output_shape,
+                    activation_function= Linear())
     
 #create a layer Max
 def create_Max(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Maximum.Maximum(idx=idx,
-                      size=size,
-                      input_shapes=input_shapes,
-                      output_shape=output_shape,
-                      activation_function= activation_functions.Linear())
+    return Maximum(idx=idx,
+                    size=size,
+                    input_shapes=input_shapes,
+                    output_shape=output_shape,
+                    activation_function= Linear())
 
 #create a layer Min
 def create_Min(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Minimum.Minimum(idx=idx,
-                      size=size,
-                      input_shapes=input_shapes,
-                      output_shape=output_shape,
-                      activation_function= activation_functions.Linear())
+    return Minimum(idx=idx,
+                    size=size,
+                    input_shapes=input_shapes,
+                    output_shape=output_shape,
+                    activation_function= Linear())
 
 #create a layer Average
 def create_Avg(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Average.Average(idx=idx,
-                      size=size,
-                      input_shapes=input_shapes,
-                      output_shape=output_shape,
-                      activation_function= activation_functions.Linear())
+    return Average(idx=idx,
+                    size=size,
+                    input_shapes=input_shapes,
+                    output_shape=output_shape,
+                    activation_function= Linear())
 
 ###### Dict of all the functions ######
 layer_type = {"Softmax":create_Softmax,
          "Conv":create_Conv, 
          "Resize":create_Resize,
          "Pad":create_Pad,
          "Concat":create_Concat,
@@ -584,45 +586,45 @@
                   "Shape":bypass,
                   "BatchNormalization":bypass}
 
 ###### Function to fuse to ONNX layers ######
 
 #Fuse the activation layer ReLu with the prior layer
 def fuse_ReLu(node,dict_output,model,layers):
-    layers[dict_output[node.input[0]]].activation_function = activation_functions.ReLu()
+    layers[dict_output[node.input[0]]].activation_function = ReLu()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Tanh with the prior layer
 def fuse_Tanh(node,dict_output,model,layers):
-    layers[dict_output[node.input[0]]].activation_function = activation_functions.TanH()
+    layers[dict_output[node.input[0]]].activation_function = TanH()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Sigmoide with the prior layer
 def fuse_Sigmoid(node,dict_output,model,layers):
-    layers[dict_output[node.input[0]]].activation_function = activation_functions.Sigmoid()
+    layers[dict_output[node.input[0]]].activation_function = Sigmoid()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Sigmoide with the prior layer
 def fuse_Exp(node,dict_output,model,layers):
-    layers[dict_output[node.input[0]]].activation_function = activation_functions.Exponential()
+    layers[dict_output[node.input[0]]].activation_function = Exponential()
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Sigmoide with the prior layer
 def fuse_Log(node,dict_output,model,layers):
-    layers[dict_output[node.input[0]]].activation_function = activation_functions.Logarithm()
+    layers[dict_output[node.input[0]]].activation_function = Logarithm()
     bypass(node,dict_output,model)
 
 #Fuse a layer Clip with the prior layer
 def fuse_Clip(node,dict_output,model,layers):
     min, max = float('-inf'), float('inf')
     if(node.input[1]):
         min = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))[0]
     if(node.input[2]):
         max = onnx.numpy_helper.to_array(look_for_initializer(node.input[2],model))[0]
-    layers[dict_output[node.input[0]]].activation_function = activation_functions.Clip(max=max,min=min)
+    layers[dict_output[node.input[0]]].activation_function = Clip(max=max,min=min)
     bypass(node,dict_output,model)
     
     
 ###### Dict of all the functions ######
 activation_layers = {"Relu":fuse_ReLu,
                      "Tanh":fuse_Tanh,
                      "Sigmoid":fuse_Sigmoid,
```

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev4/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.0.1.dev5/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

