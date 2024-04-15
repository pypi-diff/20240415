# Comparing `tmp/acetone_nnet-0.1.tar.gz` & `tmp/acetone_nnet-0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.1.tar", last modified: Mon Apr 15 07:18:08 2024, max compression
+gzip compressed data, was "acetone_nnet-0.1.dev1.tar", last modified: Mon Apr 15 11:19:50 2024, max compression
```

## Comparing `acetone_nnet-0.1.tar` & `acetone_nnet-0.1.dev1.tar`

### file list

```diff
@@ -1,138 +1,144 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.627286 acetone_nnet-0.1/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone_nnet-0.1/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.1/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.1/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7484 2024-04-15 07:18:08.627286 acetone_nnet-0.1/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone_nnet-0.1/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1883 2024-04-15 07:18:01.000000 acetone_nnet-0.1/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-15 07:18:08.627286 acetone_nnet-0.1/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.605286 acetone_nnet-0.1/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.609286 acetone_nnet-0.1/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1770 2024-04-12 12:00:11.000000 acetone_nnet-0.1/src/acetone_nnet/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone_nnet-0.1/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.611286 acetone_nnet-0.1/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 06:45:47.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1852 2024-04-12 14:35:58.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.613286 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/AddBias.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.614286 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4324 2024-04-15 06:50:30.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.615286 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2986 2024-04-15 06:50:24.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.616286 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.616286 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.617286 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 06:49:26.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 09:52:53.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23719 2024-04-15 06:42:39.000000 acetone_nnet-0.1/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.617286 acetone_nnet-0.1/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.617286 acetone_nnet-0.1/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.617286 acetone_nnet-0.1/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17138 2024-04-15 07:13:20.000000 acetone_nnet-0.1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.618286 acetone_nnet-0.1/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.618286 acetone_nnet-0.1/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25232 2024-04-12 14:49:23.000000 acetone_nnet-0.1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone_nnet-0.1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone_nnet-0.1/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.618286 acetone_nnet-0.1/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.620286 acetone_nnet-0.1/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.1/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.621286 acetone_nnet-0.1/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.623286 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.623286 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.625286 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.626286 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2122 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.626286 acetone_nnet-0.1/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.626286 acetone_nnet-0.1/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      689 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      741 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 07:18:08.627286 acetone_nnet-0.1/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7484 2024-04-15 07:18:08.000000 acetone_nnet-0.1/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6377 2024-04-15 07:18:08.000000 acetone_nnet-0.1/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-15 07:18:08.000000 acetone_nnet-0.1/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-15 07:18:08.000000 acetone_nnet-0.1/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-15 07:18:08.000000 acetone_nnet-0.1/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-15 07:18:08.000000 acetone_nnet-0.1/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.748450 acetone_nnet-0.1.dev1/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev1/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev1/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev1/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7670 2024-04-15 11:19:50.748450 acetone_nnet-0.1.dev1/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6391 2024-04-15 08:20:07.000000 acetone_nnet-0.1.dev1/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1890 2024-04-15 11:19:37.000000 acetone_nnet-0.1.dev1/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-15 11:19:50.748450 acetone_nnet-0.1.dev1/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.728450 acetone_nnet-0.1.dev1/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.731450 acetone_nnet-0.1.dev1/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1770 2024-04-15 11:18:54.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2120 2024-04-15 08:00:26.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/__main__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.733450 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1852 2024-04-12 14:35:58.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.735450 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/AddBias.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.736450 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4324 2024-04-15 06:50:30.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.737450 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 09:11:58.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.738450 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.738450 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.739450 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2150 2024-04-15 09:56:16.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23719 2024-04-15 06:42:39.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.739450 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.739450 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.740450 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17138 2024-04-15 07:13:20.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.740450 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.740450 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25232 2024-04-12 14:49:23.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.740450 acetone_nnet-0.1.dev1/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.741450 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.743450 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.744450 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.745450 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.746451 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.747450 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2122 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.747450 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.747450 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      689 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      741 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-15 11:19:50.748450 acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7670 2024-04-15 11:19:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6730 2024-04-15 11:19:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-15 11:19:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      120 2024-04-15 11:19:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-15 11:19:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-15 11:19:50.000000 acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.1/COPYING` & `acetone_nnet-0.1.dev1/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/LICENSE` & `acetone_nnet-0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/PKG-INFO` & `acetone_nnet-0.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.1
+Version: 0.1.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
@@ -43,14 +43,25 @@
 This directory also contains the [requirements.txt](./requirements.txt) which list the package versionning used in the framework.
 
 The [test](./test/) directory includes several tests for the framework and the data to run them.
 
 The [src](./src/) folder contains the backend code of ACETONE.
 
 ## Installation
+
+### User mode
+
+Install le package using `pip`
+```
+pip install acetone-nnet
+```
+
+
+### Development Mode
+
 Clone the GitHub repo on your computer
 
 ```
 git clone https://github.com/onera/acetone.git
 ```
 
 Then install the packages listed in [`requirements.txt`](./requirements.txt)
@@ -84,30 +95,30 @@
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-python3 src/cli_acetone.py tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated .tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+python3 -m acetone_nnet tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
-make -C tests/models/lenet5/lenet5_example all
+make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
-./tests/models/lenet5/lenet5_example/lenet5 ./tests/models/lenet5/lenet5_example/output_acetone.txt
+./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-python3 src/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/output_acetone.txt 1
+python3 src/acetone_nnet/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
 To run all of them, use the following command:
```

### Comparing `acetone_nnet-0.1/README.md` & `acetone_nnet-0.1.dev1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,25 @@
 This directory also contains the [requirements.txt](./requirements.txt) which list the package versionning used in the framework.
 
 The [test](./test/) directory includes several tests for the framework and the data to run them.
 
 The [src](./src/) folder contains the backend code of ACETONE.
 
 ## Installation
+
+### User mode
+
+Install le package using `pip`
+```
+pip install acetone-nnet
+```
+
+
+### Development Mode
+
 Clone the GitHub repo on your computer
 
 ```
 git clone https://github.com/onera/acetone.git
 ```
 
 Then install the packages listed in [`requirements.txt`](./requirements.txt)
@@ -57,30 +68,30 @@
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-python3 src/cli_acetone.py tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated .tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+python3 -m acetone_nnet tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
-make -C tests/models/lenet5/lenet5_example all
+make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
-./tests/models/lenet5/lenet5_example/lenet5 ./tests/models/lenet5/lenet5_example/output_acetone.txt
+./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-python3 src/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/output_acetone.txt 1
+python3 src/acetone_nnet/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
 To run all of them, use the following command:
```

### Comparing `acetone_nnet-0.1/pyproject.toml` & `acetone_nnet-0.1.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.1"
+version = "0.1.dev1"
 requires-python = ">=3.10"
 
 authors = [
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
     { name="Claire PAGETTI", email="Claire.Pagetti@onera.fr" },
@@ -51,13 +51,13 @@
     "templates/layers/*.tpl",
     "templates/layers/Resize/*.tpl",
     "templates/layers/Pad/*.tpl",
     "templates/layers/Gemm/*.tpl",
     "templates/layers/Conv/*.tpl"]
 
 [project.scripts]
-cli-acetone = "acetone.src.cli_acetone:cli_acetone"
-cli_compare = "acetone.src.cli_compare:cli_compare"
+cli-acetone = "acetone_nnet.cli_acetone:cli_acetone"
+cli_compare = "acetone_nnet.cli_compare:cli_compare"
 
 [project.urls]
 Repository = "https://github.com/onera/acetone/"
 "Bug Tracker" = "https://github.com/onera/acetone/issues"
```

### Comparing `acetone_nnet-0.1/src/acetone_nnet/__init__.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/cli_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 def cli_compare(reference_file, c_file, nb_tests, precision):
     _, max_diff_file = compare_files(reference_file, c_file, nb_tests, precision)
     
     print("   Max absolute error for %s test(s): %s" % (nb_tests, max_diff_file))
 
 
-if __name__ == "__cli_compare__":
+if __name__ == "__main__":
 
     parser = argparse.ArgumentParser(description='Program to verify the semantic preservation of ')
 
     parser.add_argument("reference_file", help="File with the inference output of the reference machine learning framework")
     parser.add_argument("c_file", help="File with the inference output of the studied machine learning framework")
     parser.add_argument("nb_tests", help="Number of inferences process to compare")
     parser.add_argument("--precision", help="Precision of the data studied. Default is float32")
```

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,12 +56,12 @@
 
         if (self.fused_layer):
             mustach_hash['fused_layer'] = self.fused_layer.write_activation_str(self.local_var,self.idx,'j + '+str(self.output_width)+'*(i + '+str(self.output_height)+'*f)')
 
             if (self.activation_function.name == 'linear'):
                 mustach_hash['linear'] = True
         
-        with open('./templates/layers/Conv/template_Conv_6loops.c.tpl','r') as template_file:
+        with open(self.template_path+'layers/Conv/template_Conv_6loops.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
```

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/code_generator/neural_network.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.1.dev1/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.1
+Version: 0.1.dev1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
@@ -43,14 +43,25 @@
 This directory also contains the [requirements.txt](./requirements.txt) which list the package versionning used in the framework.
 
 The [test](./test/) directory includes several tests for the framework and the data to run them.
 
 The [src](./src/) folder contains the backend code of ACETONE.
 
 ## Installation
+
+### User mode
+
+Install le package using `pip`
+```
+pip install acetone-nnet
+```
+
+
+### Development Mode
+
 Clone the GitHub repo on your computer
 
 ```
 git clone https://github.com/onera/acetone.git
 ```
 
 Then install the packages listed in [`requirements.txt`](./requirements.txt)
@@ -84,30 +95,30 @@
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-python3 src/cli_acetone.py tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated .tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+python3 -m acetone_nnet tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
-make -C tests/models/lenet5/lenet5_example all
+make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
-./tests/models/lenet5/lenet5_example/lenet5 ./tests/models/lenet5/lenet5_example/output_acetone.txt
+./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-python3 src/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/output_acetone.txt 1
+python3 src/acetone_nnet/cli_compare.py ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
 To run all of them, use the following command:
```

### Comparing `acetone_nnet-0.1/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.1.dev1/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 AUTHORS.md
 COPYING
 LICENSE
 README.md
 pyproject.toml
 src/acetone_nnet/__init__.py
+src/acetone_nnet/__main__.py
 src/acetone_nnet/cli_acetone.py
 src/acetone_nnet/cli_compare.py
 src/acetone_nnet.egg-info/PKG-INFO
 src/acetone_nnet.egg-info/SOURCES.txt
 src/acetone_nnet.egg-info/dependency_links.txt
 src/acetone_nnet.egg-info/entry_points.txt
 src/acetone_nnet.egg-info/requires.txt
@@ -31,31 +32,36 @@
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
 src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
 src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
 src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
 src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
 src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
 src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
 src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
 src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
 src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
 src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
 src/acetone_nnet/format_importer/parser.py
 src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
 src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
 src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
 src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
 src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
 src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
```

