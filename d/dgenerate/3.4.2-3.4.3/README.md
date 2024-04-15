# Comparing `tmp/dgenerate-3.4.2.tar.gz` & `tmp/dgenerate-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgenerate-3.4.2.tar", last modified: Sun Apr 14 00:10:54 2024, max compression
+gzip compressed data, was "dgenerate-3.4.3.tar", last modified: Mon Apr 15 08:11:45 2024, max compression
```

## Comparing `dgenerate-3.4.2.tar` & `dgenerate-3.4.3.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.045385 dgenerate-3.4.2/
--rw-rw-rw-   0        0        0   194011 2024-04-14 00:10:54.044384 dgenerate-3.4.2/PKG-INFO
--rw-rw-rw-   0        0        0   190022 2024-04-14 00:04:31.000000 dgenerate-3.4.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.920374 dgenerate-3.4.2/dgenerate/
--rw-rw-rw-   0        0        0     5581 2024-04-14 00:04:31.000000 dgenerate-3.4.2/dgenerate/__init__.py
--rw-rw-rw-   0        0        0   103339 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/arguments.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.926425 dgenerate-3.4.2/dgenerate/batchprocess/
--rw-rw-rw-   0        0        0     2079 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/batchprocess/__init__.py
--rw-rw-rw-   0        0        0    21197 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/batchprocess/batchprocessor.py
--rw-rw-rw-   0        0        0    24283 2024-04-09 06:26:12.000000 dgenerate-3.4.2/dgenerate/batchprocess/configrunner.py
--rw-rw-rw-   0        0        0     5993 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/batchprocess/configrunnerplugin.py
--rw-rw-rw-   0        0        0     3212 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/batchprocess/configrunnerpluginloader.py
--rw-rw-rw-   0        0        0     3071 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/batchprocess/image_process_directive.py
--rw-rw-rw-   0        0        0     1888 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/dgenerate.py
--rw-rw-rw-   0        0        0     6090 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/events.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.927488 dgenerate-3.4.2/dgenerate/extras/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.928488 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/
--rw-rw-rw-   0        0        0      599 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.929490 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/canny/
--rw-rw-rw-   0        0        0     1389 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/canny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.931538 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/
--rw-rw-rw-   0        0        0     3087 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.932538 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/__init__.py
--rw-rw-rw-   0        0        0     7710 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py
--rw-rw-rw-   0        0        0    10963 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/util.py
--rw-rw-rw-   0        0        0     4697 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/wholebody.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.933538 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/yolox_config/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/yolox_config/__init__.py
--rw-rw-rw-   0        0        0     7784 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.933538 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/hed/
--rw-rw-rw-   0        0        0     5861 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/hed/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.934539 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/
--rw-rw-rw-   0        0        0     4489 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.938053 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/
--rw-rw-rw-   0        0        0     6440 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py
--rw-rw-rw-   0        0        0     8784 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/__init__.py
--rw-rw-rw-   0        0        0    23459 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py
--rw-rw-rw-   0        0        0     1156 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
--rw-rw-rw-   0        0        0     2099 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py
--rw-rw-rw-   0        0        0    17304 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.939053 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.941569 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/
--rw-rw-rw-   0        0        0     3179 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py
--rw-rw-rw-   0        0        0    10958 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py
--rw-rw-rw-   0        0        0     1718 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py
--rw-rw-rw-   0        0        0    29583 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py
--rw-rw-rw-   0        0        0     7558 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.943569 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/options/
--rw-rw-rw-   0        0        0      137 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/options/__init__.py
--rw-rw-rw-   0        0        0     9520 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py
--rw-rw-rw-   0        0        0     1084 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.944568 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/util/
--rw-rw-rw-   0        0        0       84 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/util/__init__.py
--rw-rw-rw-   0        0        0     3215 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.945569 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/lineart/
--rw-rw-rw-   0        0        0     5972 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/lineart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.945569 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/lineart_anime/
--rw-rw-rw-   0        0        0     8393 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.947078 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mediapipe_face/
--rw-rw-rw-   0        0        0     1997 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py
--rw-rw-rw-   0        0        0     7281 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.949087 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/
--rw-rw-rw-   0        0        0     3676 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/__init__.py
--rw-rw-rw-   0        0        0     5445 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/api.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.953603 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/__init__.py
--rw-rw-rw-   0        0        0      383 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/base_model.py
--rw-rw-rw-   0        0        0     9584 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/blocks.py
--rw-rw-rw-   0        0        0     3263 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-rw-   0        0        0     2785 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py
--rw-rw-rw-   0        0        0     5334 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-rw-   0        0        0     8103 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/transforms.py
--rw-rw-rw-   0        0        0    15116 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/vit.py
--rw-rw-rw-   0        0        0     4771 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.954604 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/
--rw-rw-rw-   0        0        0     2895 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.956603 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/models/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/models/__init__.py
--rw-rw-rw-   0        0        0     9969 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-rw-   0        0        0     9454 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-rw-   0        0        0    24773 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.957112 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/
--rw-rw-rw-   0        0        0     3755 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.959119 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/
--rw-rw-rw-   0        0        0      618 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/__init__.py
--rw-rw-rw-   0        0        0     3065 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.961628 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-rw-rw-   0        0        0    10682 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.967696 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-rw-rw-   0        0        0     2493 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-rw-rw-   0        0        0     6131 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.973205 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-rw-rw-   0        0        0      210 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.975205 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-rw-rw-   0        0        0     4307 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-rw-rw-   0        0        0     2373 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-rw-rw-   0        0        0     4723 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-rw-rw-   0        0        0     3473 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-rw-rw-   0        0        0    12397 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-rw-rw-   0        0        0    27197 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-rw-rw-   0        0        0    61375 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-rw-rw-   0        0        0     2904 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-rw-rw-   0        0        0    15373 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-rw-rw-   0        0        0      734 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-rw-rw-   0        0        0       23 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-rw-rw-   0        0        0     2814 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-rw-rw-   0        0        0     5941 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-rw-rw-   0        0        0     3016 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-rw-rw-   0        0        0      870 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-rw-rw-   0        0        0     5017 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-rw-rw-   0        0        0     1784 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-rw-rw-   0        0        0     1349 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-rw-rw-   0        0        0     6798 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-rw-rw-   0        0        0     1094 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-rw-rw-   0        0        0     5842 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.978716 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/
--rw-rw-rw-   0        0        0     9711 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/__init__.py
--rw-rw-rw-   0        0        0    12688 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/body.py
--rw-rw-rw-   0        0        0    13854 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/face.py
--rw-rw-rw-   0        0        0     3299 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/hand.py
--rw-rw-rw-   0        0        0     8960 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/model.py
--rw-rw-rw-   0        0        0    14125 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/util.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.980717 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/pidi/
--rw-rw-rw-   0        0        0     3215 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/pidi/__init__.py
--rw-rw-rw-   0        0        0    22524 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/pidi/model.py
--rw-rw-rw-   0        0        0     6407 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/processor.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.982762 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/
--rw-rw-rw-   0        0        0     3456 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/__init__.py
--rw-rw-rw-   0        0        0    15520 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py
--rw-rw-rw-   0        0        0     4854 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.987994 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/
--rw-rw-rw-   0        0        0      431 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py
--rw-rw-rw-   0        0        0    14815 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py
--rw-rw-rw-   0        0        0     6791 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py
--rw-rw-rw-   0        0        0     8808 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py
--rw-rw-rw-   0        0        0     7458 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py
--rw-rw-rw-   0        0        0    25423 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
--rw-rw-rw-   0        0        0     8637 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py
--rw-rw-rw-   0        0        0    11902 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/predictor.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.989992 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/
--rw-rw-rw-   0        0        0      202 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/__init__.py
--rw-rw-rw-   0        0        0    13058 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py
--rw-rw-rw-   0        0        0     5956 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py
--rw-rw-rw-   0        0        0     4074 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.989992 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/shuffle/
--rw-rw-rw-   0        0        0     3430 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/shuffle/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.992045 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/tests/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/tests/__init__.py
--rw-rw-rw-   0        0        0     3083 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/tests/test_processor.py
--rw-rw-rw-   0        0        0     1858 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py
--rw-rw-rw-   0        0        0     5580 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/util.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.992045 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/
--rw-rw-rw-   0        0        0     2997 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.993045 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.995046 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/
--rw-rw-rw-   0        0        0     1178 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.997046 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/
--rw-rw-rw-   0        0        0     1178 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
--rw-rw-rw-   0        0        0    15627 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:53.997046 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
--rw-rw-rw-   0        0        0    14192 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.002341 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.007342 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
--rw-rw-rw-   0        0        0     7105 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
--rw-rw-rw-   0        0        0     3542 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
--rw-rw-rw-   0        0        0     1084 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
--rw-rw-rw-   0        0        0      346 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
--rw-rw-rw-   0        0        0      965 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
--rw-rw-rw-   0        0        0     1628 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
--rw-rw-rw-   0        0        0     7533 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
--rw-rw-rw-   0        0        0     7120 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
--rw-rw-rw-   0        0        0      383 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
--rw-rw-rw-   0        0        0    13231 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
--rw-rw-rw-   0        0        0     6265 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
--rw-rw-rw-   0        0        0     2785 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
--rw-rw-rw-   0        0        0     5334 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
--rw-rw-rw-   0        0        0     8794 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
--rw-rw-rw-   0        0        0     8103 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
--rw-rw-rw-   0        0        0     2441 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py
--rw-rw-rw-   0        0        0     7513 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.010438 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/
--rw-rw-rw-   0        0        0     1176 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
--rw-rw-rw-   0        0        0     8901 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
--rw-rw-rw-   0        0        0     4959 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
--rw-rw-rw-   0        0        0     6901 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
--rw-rw-rw-   0        0        0     4254 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
--rw-rw-rw-   0        0        0     3529 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.011438 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/
--rw-rw-rw-   0        0        0     1300 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
--rw-rw-rw-   0        0        0    12880 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.012727 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
--rw-rw-rw-   0        0        0     1306 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
--rw-rw-rw-   0        0        0    16596 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.013728 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/
--rw-rw-rw-   0        0        0     1178 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py
--rw-rw-rw-   0        0        0      657 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
--rw-rw-rw-   0        0        0    16747 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.014727 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/
--rw-rw-rw-   0        0        0     3583 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
--rw-rw-rw-   0        0        0     5825 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/filelock.py
--rw-rw-rw-   0        0        0     7335 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/image.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.018235 dgenerate-3.4.2/dgenerate/image_process/
--rw-rw-rw-   0        0        0     2588 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/image_process/__init__.py
--rw-rw-rw-   0        0        0    10151 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/image_process/arguments.py
--rw-rw-rw-   0        0        0     7682 2024-04-10 20:52:32.000000 dgenerate-3.4.2/dgenerate/image_process/invoker.py
--rw-rw-rw-   0        0        0    19590 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/image_process/renderloop.py
--rw-rw-rw-   0        0        0     7924 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/image_process/renderloopconfig.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.029266 dgenerate-3.4.2/dgenerate/imageprocessors/
--rw-rw-rw-   0        0        0     4055 2024-04-10 20:52:32.000000 dgenerate-3.4.2/dgenerate/imageprocessors/__init__.py
--rw-rw-rw-   0        0        0    12211 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/canny.py
--rw-rw-rw-   0        0        0     1952 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/exceptions.py
--rw-rw-rw-   0        0        0     9077 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/hed.py
--rw-rw-rw-   0        0        0     7531 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/imageops.py
--rw-rw-rw-   0        0        0    15785 2024-04-10 20:52:32.000000 dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessor.py
--rw-rw-rw-   0        0        0     5308 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessorchain.py
--rw-rw-rw-   0        0        0     4777 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessorloader.py
--rw-rw-rw-   0        0        0     6313 2024-04-07 03:50:32.000000 dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessormixin.py
--rw-rw-rw-   0        0        0     9582 2024-04-10 20:52:32.000000 dgenerate-3.4.2/dgenerate/imageprocessors/leres.py
--rw-rw-rw-   0        0        0     8078 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/linart_anime.py
--rw-rw-rw-   0        0        0     8101 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/lineart.py
--rw-rw-rw-   0        0        0     8848 2024-04-10 20:52:32.000000 dgenerate-3.4.2/dgenerate/imageprocessors/midas.py
--rw-rw-rw-   0        0        0     8616 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/mlsd.py
--rw-rw-rw-   0        0        0     7558 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/normal_bae.py
--rw-rw-rw-   0        0        0     9273 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/openpose.py
--rw-rw-rw-   0        0        0     8517 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/pidi.py
--rw-rw-rw-   0        0        0     8712 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/imageprocessors/sam.py
--rw-rw-rw-   0        0        0    17489 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/imageprocessors/upscaler.py
--rw-rw-rw-   0        0        0    14553 2024-04-09 05:35:19.000000 dgenerate-3.4.2/dgenerate/invoker.py
--rw-rw-rw-   0        0        0    85324 2024-04-07 03:50:32.000000 dgenerate-3.4.2/dgenerate/mediainput.py
--rw-rw-rw-   0        0        0     9840 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/mediaoutput.py
--rw-rw-rw-   0        0        0     7701 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/memoize.py
--rw-rw-rw-   0        0        0    12201 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/memory.py
--rw-rw-rw-   0        0        0     6236 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/messages.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.034774 dgenerate-3.4.2/dgenerate/pipelinewrapper/
--rw-rw-rw-   0        0        0     5718 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/__init__.py
--rw-rw-rw-   0        0        0    29441 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/cache.py
--rw-rw-rw-   0        0        0     3101 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/constants.py
--rw-rw-rw-   0        0        0    15329 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/enums.py
--rw-rw-rw-   0        0        0    23862 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/hfutil.py
--rw-rw-rw-   0        0        0    67453 2024-04-13 20:35:26.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/pipelines.py
--rw-rw-rw-   0        0        0    71673 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/uris.py
--rw-rw-rw-   0        0        0     2844 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/util.py
--rw-rw-rw-   0        0        0    98798 2024-04-14 00:00:14.000000 dgenerate-3.4.2/dgenerate/pipelinewrapper/wrapper.py
--rw-rw-rw-   0        0        0    29178 2024-04-10 20:52:32.000000 dgenerate-3.4.2/dgenerate/plugin.py
--rw-rw-rw-   0        0        0     3519 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/prompt.py
--rw-rw-rw-   0        0        0    51975 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/renderloop.py
--rw-rw-rw-   0        0        0    56859 2024-04-13 06:02:43.000000 dgenerate-3.4.2/dgenerate/renderloopconfig.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.037774 dgenerate-3.4.2/dgenerate/subcommands/
--rw-rw-rw-   0        0        0     3196 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/subcommands/__init__.py
--rw-rw-rw-   0        0        0     1935 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/subcommands/exceptions.py
--rw-rw-rw-   0        0        0     2636 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/subcommands/image_process.py
--rw-rw-rw-   0        0        0     2536 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/subcommands/subcommand.py
--rw-rw-rw-   0        0        0     2727 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/subcommands/subcommandloader.py
--rw-rw-rw-   0        0        0    35238 2023-12-14 08:15:38.000000 dgenerate-3.4.2/dgenerate/textprocessing.py
--rw-rw-rw-   0        0        0    16790 2024-04-10 20:52:32.000000 dgenerate-3.4.2/dgenerate/types.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.040874 dgenerate-3.4.2/dgenerate.egg-info/
--rw-rw-rw-   0        0        0   194011 2024-04-14 00:10:53.000000 dgenerate-3.4.2/dgenerate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13330 2024-04-14 00:10:53.000000 dgenerate-3.4.2/dgenerate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 00:10:53.000000 dgenerate-3.4.2/dgenerate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-14 00:10:53.000000 dgenerate-3.4.2/dgenerate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1343 2024-04-14 00:10:53.000000 dgenerate-3.4.2/dgenerate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-14 00:10:53.000000 dgenerate-3.4.2/dgenerate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 00:10:54.045385 dgenerate-3.4.2/setup.cfg
--rw-rw-rw-   0        0        0    10812 2024-04-13 06:02:43.000000 dgenerate-3.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.037774 dgenerate-3.4.2/tests/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:10:54.040874 dgenerate-3.4.2/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.2/tests/unit/__init__.py
--rw-rw-rw-   0        0        0     9682 2023-12-14 08:15:38.000000 dgenerate-3.4.2/tests/unit/concept_uri_parser_test.py
--rw-rw-rw-   0        0        0    10155 2023-12-14 08:15:38.000000 dgenerate-3.4.2/tests/unit/image_seed_parse_test.py
--rw-rw-rw-   0        0        0    18395 2023-12-14 08:15:38.000000 dgenerate-3.4.2/tests/unit/plugin_loading_test.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.898287 dgenerate-3.4.3/
+-rw-rw-rw-   0        0        0   194011 2024-04-15 08:11:45.897287 dgenerate-3.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0   190022 2024-04-15 08:07:56.000000 dgenerate-3.4.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.752227 dgenerate-3.4.3/dgenerate/
+-rw-rw-rw-   0        0        0     5581 2024-04-15 08:07:56.000000 dgenerate-3.4.3/dgenerate/__init__.py
+-rw-rw-rw-   0        0        0   103339 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/arguments.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.760702 dgenerate-3.4.3/dgenerate/batchprocess/
+-rw-rw-rw-   0        0        0     2079 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/batchprocess/__init__.py
+-rw-rw-rw-   0        0        0    21197 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/batchprocess/batchprocessor.py
+-rw-rw-rw-   0        0        0    24283 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/batchprocess/configrunner.py
+-rw-rw-rw-   0        0        0     5993 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/batchprocess/configrunnerplugin.py
+-rw-rw-rw-   0        0        0     3212 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/batchprocess/configrunnerpluginloader.py
+-rw-rw-rw-   0        0        0     3071 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/batchprocess/image_process_directive.py
+-rw-rw-rw-   0        0        0     1888 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/dgenerate.py
+-rw-rw-rw-   0        0        0     6090 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/events.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.761700 dgenerate-3.4.3/dgenerate/extras/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.763700 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/
+-rw-rw-rw-   0        0        0      599 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.763700 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/canny/
+-rw-rw-rw-   0        0        0     1389 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/canny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.766832 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/
+-rw-rw-rw-   0        0        0     3087 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.767834 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/__init__.py
+-rw-rw-rw-   0        0        0     7710 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py
+-rw-rw-rw-   0        0        0    10963 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/util.py
+-rw-rw-rw-   0        0        0     4697 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/wholebody.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.768834 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/yolox_config/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/yolox_config/__init__.py
+-rw-rw-rw-   0        0        0     7784 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.769345 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/hed/
+-rw-rw-rw-   0        0        0     5861 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/hed/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.770350 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/
+-rw-rw-rw-   0        0        0     4489 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.774351 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/
+-rw-rw-rw-   0        0        0     6440 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py
+-rw-rw-rw-   0        0        0     8784 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/__init__.py
+-rw-rw-rw-   0        0        0    23459 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py
+-rw-rw-rw-   0        0        0     1156 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
+-rw-rw-rw-   0        0        0     2099 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py
+-rw-rw-rw-   0        0        0    17304 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.776005 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.779037 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/
+-rw-rw-rw-   0        0        0     3179 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py
+-rw-rw-rw-   0        0        0    10958 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py
+-rw-rw-rw-   0        0        0     1718 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py
+-rw-rw-rw-   0        0        0    29583 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py
+-rw-rw-rw-   0        0        0     7558 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.781043 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/options/
+-rw-rw-rw-   0        0        0      137 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/options/__init__.py
+-rw-rw-rw-   0        0        0     9520 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py
+-rw-rw-rw-   0        0        0     1084 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.782042 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/util/
+-rw-rw-rw-   0        0        0       84 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/util/__init__.py
+-rw-rw-rw-   0        0        0     3215 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.783042 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/lineart/
+-rw-rw-rw-   0        0        0     5972 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/lineart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.784042 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/lineart_anime/
+-rw-rw-rw-   0        0        0     8393 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.785042 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mediapipe_face/
+-rw-rw-rw-   0        0        0     1997 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py
+-rw-rw-rw-   0        0        0     7281 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.786042 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/
+-rw-rw-rw-   0        0        0     3676 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/__init__.py
+-rw-rw-rw-   0        0        0     5445 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/api.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.791574 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/__init__.py
+-rw-rw-rw-   0        0        0      383 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/base_model.py
+-rw-rw-rw-   0        0        0     9584 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/blocks.py
+-rw-rw-rw-   0        0        0     3263 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py
+-rw-rw-rw-   0        0        0     2785 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py
+-rw-rw-rw-   0        0        0     5334 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8103 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/transforms.py
+-rw-rw-rw-   0        0        0    15116 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/vit.py
+-rw-rw-rw-   0        0        0     4771 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.792575 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/
+-rw-rw-rw-   0        0        0     2895 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.794577 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/models/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/models/__init__.py
+-rw-rw-rw-   0        0        0     9969 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9454 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    24773 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.794577 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/
+-rw-rw-rw-   0        0        0     3755 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.796082 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/
+-rw-rw-rw-   0        0        0      618 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/__init__.py
+-rw-rw-rw-   0        0        0     3065 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.798088 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-rw-rw-   0        0        0    10682 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.805599 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-rw-rw-   0        0        0     2493 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-rw-rw-   0        0        0     6131 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.812569 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-rw-rw-   0        0        0      210 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.815725 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-rw-rw-   0        0        0     4307 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-rw-rw-   0        0        0     2792 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-rw-rw-   0        0        0     2373 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-rw-rw-   0        0        0     4723 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-rw-rw-   0        0        0     3473 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-rw-rw-   0        0        0    12397 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-rw-rw-   0        0        0    27197 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-rw-rw-   0        0        0    61375 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-rw-rw-   0        0        0     2904 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-rw-rw-   0        0        0    15373 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-rw-rw-   0        0        0      734 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-rw-rw-   0        0        0       23 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-rw-rw-   0        0        0     2814 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-rw-rw-   0        0        0     5941 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-rw-rw-   0        0        0     3016 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-rw-rw-   0        0        0      870 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-rw-rw-   0        0        0     5017 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-rw-rw-   0        0        0     1784 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-rw-rw-   0        0        0     1349 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-rw-rw-   0        0        0     6798 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-rw-rw-   0        0        0     1094 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-rw-rw-   0        0        0     5842 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.819381 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/
+-rw-rw-rw-   0        0        0     9711 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/__init__.py
+-rw-rw-rw-   0        0        0    12688 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/body.py
+-rw-rw-rw-   0        0        0    13854 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/face.py
+-rw-rw-rw-   0        0        0     3299 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/hand.py
+-rw-rw-rw-   0        0        0     8960 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/model.py
+-rw-rw-rw-   0        0        0    14125 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.820416 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/pidi/
+-rw-rw-rw-   0        0        0     3215 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/pidi/__init__.py
+-rw-rw-rw-   0        0        0    22524 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/pidi/model.py
+-rw-rw-rw-   0        0        0     6407 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/processor.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.823155 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/
+-rw-rw-rw-   0        0        0     3456 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/__init__.py
+-rw-rw-rw-   0        0        0    15520 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py
+-rw-rw-rw-   0        0        0     4854 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.828896 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/
+-rw-rw-rw-   0        0        0      431 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/__init__.py
+-rw-rw-rw-   0        0        0     1522 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py
+-rw-rw-rw-   0        0        0    14815 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py
+-rw-rw-rw-   0        0        0     6791 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py
+-rw-rw-rw-   0        0        0     8808 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py
+-rw-rw-rw-   0        0        0     7458 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py
+-rw-rw-rw-   0        0        0    25423 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
+-rw-rw-rw-   0        0        0     8637 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py
+-rw-rw-rw-   0        0        0    11902 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/predictor.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.832075 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/
+-rw-rw-rw-   0        0        0      202 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/__init__.py
+-rw-rw-rw-   0        0        0    13058 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py
+-rw-rw-rw-   0        0        0     5956 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py
+-rw-rw-rw-   0        0        0     4074 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.832603 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/shuffle/
+-rw-rw-rw-   0        0        0     3430 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/shuffle/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.834180 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/tests/__init__.py
+-rw-rw-rw-   0        0        0     3083 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/tests/test_processor.py
+-rw-rw-rw-   0        0        0     1858 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py
+-rw-rw-rw-   0        0        0     5580 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.835239 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/
+-rw-rw-rw-   0        0        0     2997 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.835239 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.839707 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/
+-rw-rw-rw-   0        0        0     1178 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.840705 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/
+-rw-rw-rw-   0        0        0     1178 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
+-rw-rw-rw-   0        0        0    15627 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.841771 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-rw-rw-   0        0        0    14192 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.846768 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.852882 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-rw-rw-   0        0        0        0 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-rw-rw-   0        0        0     7105 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-rw-rw-   0        0        0     3542 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-rw-rw-   0        0        0     1084 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-rw-rw-   0        0        0      346 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-rw-rw-   0        0        0      965 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-rw-rw-   0        0        0     1628 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-rw-rw-   0        0        0     7533 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-rw-rw-   0        0        0     7120 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-rw-rw-   0        0        0      383 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-rw-rw-   0        0        0    13231 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-rw-rw-   0        0        0     6265 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-rw-rw-   0        0        0     2785 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-rw-rw-   0        0        0     5334 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8794 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-rw-rw-   0        0        0     8103 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-rw-rw-   0        0        0     2441 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py
+-rw-rw-rw-   0        0        0     7513 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.855883 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/
+-rw-rw-rw-   0        0        0     1176 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
+-rw-rw-rw-   0        0        0     8901 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
+-rw-rw-rw-   0        0        0     4959 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
+-rw-rw-rw-   0        0        0     6901 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-rw-rw-   0        0        0     4254 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-rw-rw-   0        0        0     3529 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.856882 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/
+-rw-rw-rw-   0        0        0     1300 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-rw-rw-   0        0        0    12880 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.858883 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
+-rw-rw-rw-   0        0        0     1306 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-rw-rw-   0        0        0    16596 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.860884 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/
+-rw-rw-rw-   0        0        0     1178 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
+-rw-rw-rw-   0        0        0    16747 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.861401 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/
+-rw-rw-rw-   0        0        0     3583 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+-rw-rw-rw-   0        0        0     5825 2024-04-13 06:02:43.000000 dgenerate-3.4.3/dgenerate/filelock.py
+-rw-rw-rw-   0        0        0     7335 2024-04-13 06:02:43.000000 dgenerate-3.4.3/dgenerate/image.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.864791 dgenerate-3.4.3/dgenerate/image_process/
+-rw-rw-rw-   0        0        0     2588 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/image_process/__init__.py
+-rw-rw-rw-   0        0        0    10151 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/image_process/arguments.py
+-rw-rw-rw-   0        0        0     7682 2024-04-10 20:52:32.000000 dgenerate-3.4.3/dgenerate/image_process/invoker.py
+-rw-rw-rw-   0        0        0    19590 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/image_process/renderloop.py
+-rw-rw-rw-   0        0        0     7924 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/image_process/renderloopconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.877818 dgenerate-3.4.3/dgenerate/imageprocessors/
+-rw-rw-rw-   0        0        0     4055 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/__init__.py
+-rw-rw-rw-   0        0        0    12211 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/canny.py
+-rw-rw-rw-   0        0        0     1952 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/imageprocessors/exceptions.py
+-rw-rw-rw-   0        0        0     9077 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/hed.py
+-rw-rw-rw-   0        0        0     7531 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/imageprocessors/imageops.py
+-rw-rw-rw-   0        0        0    15785 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessor.py
+-rw-rw-rw-   0        0        0     5308 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessorchain.py
+-rw-rw-rw-   0        0        0     4777 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessorloader.py
+-rw-rw-rw-   0        0        0     6313 2024-04-07 03:50:32.000000 dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessormixin.py
+-rw-rw-rw-   0        0        0     9582 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/leres.py
+-rw-rw-rw-   0        0        0     8078 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/linart_anime.py
+-rw-rw-rw-   0        0        0     8101 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/lineart.py
+-rw-rw-rw-   0        0        0     8848 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/midas.py
+-rw-rw-rw-   0        0        0     8616 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/mlsd.py
+-rw-rw-rw-   0        0        0     7558 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/normal_bae.py
+-rw-rw-rw-   0        0        0     9273 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/openpose.py
+-rw-rw-rw-   0        0        0     8517 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/pidi.py
+-rw-rw-rw-   0        0        0     8712 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/imageprocessors/sam.py
+-rw-rw-rw-   0        0        0    17489 2024-04-13 06:02:43.000000 dgenerate-3.4.3/dgenerate/imageprocessors/upscaler.py
+-rw-rw-rw-   0        0        0    14553 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/invoker.py
+-rw-rw-rw-   0        0        0    85324 2024-04-07 03:50:32.000000 dgenerate-3.4.3/dgenerate/mediainput.py
+-rw-rw-rw-   0        0        0     9840 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/mediaoutput.py
+-rw-rw-rw-   0        0        0     7701 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/memoize.py
+-rw-rw-rw-   0        0        0    12201 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/memory.py
+-rw-rw-rw-   0        0        0     6236 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/messages.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.884260 dgenerate-3.4.3/dgenerate/pipelinewrapper/
+-rw-rw-rw-   0        0        0     5718 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/__init__.py
+-rw-rw-rw-   0        0        0    29441 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/cache.py
+-rw-rw-rw-   0        0        0     3101 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/constants.py
+-rw-rw-rw-   0        0        0    15329 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/enums.py
+-rw-rw-rw-   0        0        0    23862 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/hfutil.py
+-rw-rw-rw-   0        0        0    67453 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/pipelines.py
+-rw-rw-rw-   0        0        0    71673 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/uris.py
+-rw-rw-rw-   0        0        0     2844 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/util.py
+-rw-rw-rw-   0        0        0    99054 2024-04-15 08:06:28.000000 dgenerate-3.4.3/dgenerate/pipelinewrapper/wrapper.py
+-rw-rw-rw-   0        0        0    29178 2024-04-10 20:52:32.000000 dgenerate-3.4.3/dgenerate/plugin.py
+-rw-rw-rw-   0        0        0     3519 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/prompt.py
+-rw-rw-rw-   0        0        0    51975 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/renderloop.py
+-rw-rw-rw-   0        0        0    56859 2024-04-15 07:43:33.000000 dgenerate-3.4.3/dgenerate/renderloopconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.889776 dgenerate-3.4.3/dgenerate/subcommands/
+-rw-rw-rw-   0        0        0     3196 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/subcommands/__init__.py
+-rw-rw-rw-   0        0        0     1935 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/subcommands/exceptions.py
+-rw-rw-rw-   0        0        0     2636 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/subcommands/image_process.py
+-rw-rw-rw-   0        0        0     2536 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/subcommands/subcommand.py
+-rw-rw-rw-   0        0        0     2727 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/subcommands/subcommandloader.py
+-rw-rw-rw-   0        0        0    35238 2023-12-14 08:15:38.000000 dgenerate-3.4.3/dgenerate/textprocessing.py
+-rw-rw-rw-   0        0        0    16790 2024-04-10 20:52:32.000000 dgenerate-3.4.3/dgenerate/types.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.894288 dgenerate-3.4.3/dgenerate.egg-info/
+-rw-rw-rw-   0        0        0   194011 2024-04-15 08:11:45.000000 dgenerate-3.4.3/dgenerate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13330 2024-04-15 08:11:45.000000 dgenerate-3.4.3/dgenerate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:11:45.000000 dgenerate-3.4.3/dgenerate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-15 08:11:45.000000 dgenerate-3.4.3/dgenerate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1343 2024-04-15 08:11:45.000000 dgenerate-3.4.3/dgenerate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 08:11:45.000000 dgenerate-3.4.3/dgenerate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:11:45.898287 dgenerate-3.4.3/setup.cfg
+-rw-rw-rw-   0        0        0    10812 2024-04-13 06:02:43.000000 dgenerate-3.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.890776 dgenerate-3.4.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:11:45.893288 dgenerate-3.4.3/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-12-14 08:15:38.000000 dgenerate-3.4.3/tests/unit/__init__.py
+-rw-rw-rw-   0        0        0     9682 2023-12-14 08:15:38.000000 dgenerate-3.4.3/tests/unit/concept_uri_parser_test.py
+-rw-rw-rw-   0        0        0    10155 2023-12-14 08:15:38.000000 dgenerate-3.4.3/tests/unit/image_seed_parse_test.py
+-rw-rw-rw-   0        0        0    18395 2023-12-14 08:15:38.000000 dgenerate-3.4.3/tests/unit/plugin_loading_test.py
```

### Comparing `dgenerate-3.4.2/PKG-INFO` & `dgenerate-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6765  : 2.1..Name: dge
 00000020: 6e65 7261 7465 0d0a 5665 7273 696f 6e3a  nerate..Version:
-00000030: 2033 2e34 2e32 0d0a 5375 6d6d 6172 793a   3.4.2..Summary:
+00000030: 2033 2e34 2e33 0d0a 5375 6d6d 6172 793a   3.4.3..Summary:
 00000040: 2042 6174 6368 2069 6d61 6765 2067 656e   Batch image gen
 00000050: 6572 6174 696f 6e20 616e 6420 6d61 6e69  eration and mani
 00000060: 7075 6c61 7469 6f6e 2074 6f6f 6c20 7375  pulation tool su
 00000070: 7070 6f72 7469 6e67 2053 7461 626c 6520  pporting Stable 
 00000080: 4469 6666 7573 696f 6e20 616e 6420 7265  Diffusion and re
 00000090: 6c61 7465 6420 7465 6368 6e69 7175 6573  lated techniques
 000000a0: 202f 2061 6c67 6f72 6974 686d 732c 2077   / algorithms, w
@@ -249,18 +249,18 @@
 00000f80: 203d 3d20 2272 6561 6474 6865 646f 6373   == "readthedocs
 00000f90: 220d 0a0d 0a2e 2e20 7c44 6f63 756d 656e  "...... |Documen
 00000fa0: 7461 7469 6f6e 2053 7461 7475 737c 2069  tation Status| i
 00000fb0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f72  mage:: https://r
 00000fc0: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
 00000fd0: 726f 6a65 6374 732f 6467 656e 6572 6174  rojects/dgenerat
 00000fe0: 652f 6261 6467 652f 3f76 6572 7369 6f6e  e/badge/?version
-00000ff0: 3d76 332e 342e 320d 0a20 2020 3a74 6172  =v3.4.2..   :tar
+00000ff0: 3d76 332e 342e 330d 0a20 2020 3a74 6172  =v3.4.3..   :tar
 00001000: 6765 743a 2068 7474 703a 2f2f 6467 656e  get: http://dgen
 00001010: 6572 6174 652e 7265 6164 7468 6564 6f63  erate.readthedoc
-00001020: 732e 696f 2f65 6e2f 7633 2e34 2e32 2f0d  s.io/en/v3.4.2/.
+00001020: 732e 696f 2f65 6e2f 7633 2e34 2e33 2f0d  s.io/en/v3.4.3/.
 00001030: 0a0d 0a4f 7665 7276 6965 770d 0a3d 3d3d  ...Overview..===
 00001040: 3d3d 3d3d 3d0d 0a0d 0a7c 446f 6375 6d65  =====....|Docume
 00001050: 6e74 6174 696f 6e20 5374 6174 7573 7c0d  ntation Status|.
 00001060: 0a0d 0a2a 2a64 6765 6e65 7261 7465 2a2a  ...**dgenerate**
 00001070: 2069 7320 6120 636f 6d6d 616e 6420 6c69   is a command li
 00001080: 6e65 2074 6f6f 6c20 616e 6420 6c69 6272  ne tool and libr
 00001090: 6172 7920 666f 7220 6765 6e65 7261 7469  ary for generati
@@ -379,15 +379,15 @@
 000017a0: 2062 7574 2065 7874 7261 6f72 6469 6e61   but extraordina
 000017b0: 7269 6c79 2073 6c6f 772e 0d0a 0d0a 466f  rily slow.....Fo
 000017c0: 7220 6c69 6272 6172 7920 646f 6375 6d65  r library docume
 000017d0: 6e74 6174 696f 6e20 7669 7369 7420 6072  ntation visit `r
 000017e0: 6561 6474 6865 646f 6373 203c 6874 7470  eadthedocs <http
 000017f0: 3a2f 2f64 6765 6e65 7261 7465 2e72 6561  ://dgenerate.rea
 00001800: 6474 6865 646f 6373 2e69 6f2f 656e 2f76  dthedocs.io/en/v
-00001810: 332e 342e 322f 3e60 5f2e 0d0a 0d0a 2d2d  3.4.2/>`_.....--
+00001810: 332e 342e 332f 3e60 5f2e 0d0a 0d0a 2d2d  3.4.3/>`_.....--
 00001820: 2d2d 0d0a 0d0a 2a20 486f 7720 746f 2069  --....* How to i
 00001830: 6e73 7461 6c6c 0d0a 2020 2020 2a20 6057  nstall..    * `W
 00001840: 696e 646f 7773 2049 6e73 7461 6c6c 605f  indows Install`_
 00001850: 0d0a 2020 2020 2a20 604c 696e 7578 206f  ..    * `Linux o
 00001860: 7220 5753 4c20 496e 7374 616c 6c60 5f0d  r WSL Install`_.
 00001870: 0a0d 0a2a 2055 7361 6765 2045 7861 6d70  ...* Usage Examp
 00001880: 6c65 730d 0a20 2020 202a 2060 4261 7369  les..    * `Basi
@@ -4662,15 +4662,15 @@
 00012350: 6661 756c 7420 7661 6c75 653a 2022 7573  fault value: "us
 00012360: 6564 5f70 6572 6365 6e74 203e 2037 3022  ed_percent > 70"
 00012370: 2046 6f72 0d0a 2020 2020 2020 2020 2020   For..          
 00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012390: 2020 5379 6e74 6178 2053 6565 3a20 5b68    Syntax See: [h
 000123a0: 7474 7073 3a2f 2f64 6765 6e65 7261 7465  ttps://dgenerate
 000123b0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000123c0: 656e 2f76 332e 342e 322f 6467 656e 6572  en/v3.4.2/dgener
+000123c0: 656e 2f76 332e 342e 332f 6467 656e 6572  en/v3.4.3/dgener
 000123d0: 6174 655f 7375 626d 6f64 756c 6573 2e68  ate_submodules.h
 000123e0: 746d 0d0a 2020 2020 2020 2020 2020 2020  tm..            
 000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012400: 6c23 6467 656e 6572 6174 652e 7069 7065  l#dgenerate.pipe
 00012410: 6c69 6e65 7772 6170 7065 722e 4341 4348  linewrapper.CACH
 00012420: 455f 4d45 4d4f 5259 5f43 4f4e 5354 5241  E_MEMORY_CONSTRA
 00012430: 494e 5453 5d0d 0a20 2020 2020 202d 706d  INTS]..      -pm
@@ -4713,15 +4713,15 @@
 00012680: 655f 7369 7a65 203e 2028 6176 6169 6c61  e_size > (availa
 00012690: 626c 6520 2a0d 0a20 2020 2020 2020 2020  ble *..         
 000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000126b0: 2020 2030 2e37 3529 2220 466f 7220 5379     0.75)" For Sy
 000126c0: 6e74 6178 2053 6565 3a20 5b68 7474 7073  ntax See: [https
 000126d0: 3a2f 2f64 6765 6e65 7261 7465 2e72 6561  ://dgenerate.rea
 000126e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f76  dthedocs.io/en/v
-000126f0: 332e 342e 322f 6467 656e 6572 6174 655f  3.4.2/dgenerate_
+000126f0: 332e 342e 332f 6467 656e 6572 6174 655f  3.4.3/dgenerate_
 00012700: 7375 620d 0a20 2020 2020 2020 2020 2020  sub..           
 00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012720: 206d 6f64 756c 6573 2e68 746d 6c23 6467   modules.html#dg
 00012730: 656e 6572 6174 652e 7069 7065 6c69 6e65  enerate.pipeline
 00012740: 7772 6170 7065 722e 5049 5045 4c49 4e45  wrapper.PIPELINE
 00012750: 5f43 4143 4845 5f4d 454d 4f52 595f 434f  _CACHE_MEMORY_CO
 00012760: 4e53 5452 4149 4e54 535d 0d0a 2020 2020  NSTRAINTS]..    
@@ -4762,15 +4762,15 @@
 00012990: 653a 2022 756e 6574 5f73 697a 6520 3e20  e: "unet_size > 
 000129a0: 2861 7661 696c 6162 6c65 202a 2030 2e37  (available * 0.7
 000129b0: 3529 2220 466f 7220 5379 6e74 6178 2053  5)" For Syntax S
 000129c0: 6565 3a20 5b68 7474 7073 3a2f 2f64 6765  ee: [https://dge
 000129d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000129e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
 000129f0: 7261 7465 2e72 6561 6474 6865 646f 6373  rate.readthedocs
-00012a00: 2e69 6f2f 656e 2f76 332e 342e 322f 6467  .io/en/v3.4.2/dg
+00012a00: 2e69 6f2f 656e 2f76 332e 342e 332f 6467  .io/en/v3.4.3/dg
 00012a10: 656e 6572 6174 655f 7375 626d 6f64 756c  enerate_submodul
 00012a20: 6573 2e68 746d 6c23 6467 656e 6572 6174  es.html#dgenerat
 00012a30: 652e 7069 7065 6c69 6e65 7772 6170 0d0a  e.pipelinewrap..
 00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a50: 2020 2020 2020 2020 2020 2020 7065 722e              per.
 00012a60: 554e 4554 5f43 4143 4845 5f4d 454d 4f52  UNET_CACHE_MEMOR
 00012a70: 595f 434f 4e53 5452 4149 4e54 535d 0d0a  Y_CONSTRAINTS]..
@@ -4811,15 +4811,15 @@
 00012ca0: 653a 2022 7661 655f 7369 7a65 203e 2028  e: "vae_size > (
 00012cb0: 6176 6169 6c61 626c 6520 2a20 302e 3735  available * 0.75
 00012cc0: 2922 2046 6f72 2053 796e 7461 7820 5365  )" For Syntax Se
 00012cd0: 653a 205b 6874 7470 733a 2f2f 6467 656e  e: [https://dgen
 00012ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012cf0: 2020 2020 2020 2020 2020 2020 2020 6572                er
 00012d00: 6174 652e 7265 6164 7468 6564 6f63 732e  ate.readthedocs.
-00012d10: 696f 2f65 6e2f 7633 2e34 2e32 2f64 6765  io/en/v3.4.2/dge
+00012d10: 696f 2f65 6e2f 7633 2e34 2e33 2f64 6765  io/en/v3.4.3/dge
 00012d20: 6e65 7261 7465 5f73 7562 6d6f 6475 6c65  nerate_submodule
 00012d30: 732e 6874 6d6c 2364 6765 6e65 7261 7465  s.html#dgenerate
 00012d40: 2e70 6970 656c 696e 6577 7261 7070 0d0a  .pipelinewrapp..
 00012d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012d60: 2020 2020 2020 2020 2020 2020 6572 2e56              er.V
 00012d70: 4145 5f43 4143 4845 5f4d 454d 4f52 595f  AE_CACHE_MEMORY_
 00012d80: 434f 4e53 5452 4149 4e54 535d 0d0a 2020  CONSTRAINTS]..  
@@ -4862,15 +4862,15 @@
 00012fd0: 6f6e 7472 6f6c 5f6e 6574 5f73 697a 6520  ontrol_net_size 
 00012fe0: 3e20 2861 7661 696c 6162 6c65 202a 2030  > (available * 0
 00012ff0: 2e37 3529 2220 466f 720d 0a20 2020 2020  .75)" For..     
 00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013010: 2020 2020 2020 2053 796e 7461 7820 5365         Syntax Se
 00013020: 653a 205b 6874 7470 733a 2f2f 6467 656e  e: [https://dgen
 00013030: 6572 6174 652e 7265 6164 7468 6564 6f63  erate.readthedoc
-00013040: 732e 696f 2f65 6e2f 7633 2e34 2e32 2f64  s.io/en/v3.4.2/d
+00013040: 732e 696f 2f65 6e2f 7633 2e34 2e33 2f64  s.io/en/v3.4.3/d
 00013050: 6765 6e65 7261 7465 5f73 7562 6d6f 6475  generate_submodu
 00013060: 6c65 732e 6874 6d0d 0a20 2020 2020 2020  les.htm..       
 00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013080: 2020 2020 206c 2364 6765 6e65 7261 7465       l#dgenerate
 00013090: 2e70 6970 656c 696e 6577 7261 7070 6572  .pipelinewrapper
 000130a0: 2e43 4f4e 5452 4f4c 5f4e 4554 5f43 4143  .CONTROL_NET_CAC
 000130b0: 4845 5f4d 454d 4f52 595f 434f 4e53 5452  HE_MEMORY_CONSTR
@@ -4955,27 +4955,27 @@
 000135a0: 6c20 6874 7470 733a 2f2f 646f 776e 6c6f  l https://downlo
 000135b0: 6164 2e70 7974 6f72 6368 2e6f 7267 2f77  ad.pytorch.org/w
 000135c0: 686c 2f63 7531 3231 2f22 0d0a 0d0a 2020  hl/cu121/"....  
 000135d0: 2020 2320 4966 2079 6f75 2077 616e 7420    # If you want 
 000135e0: 6120 7370 6563 6966 6963 2076 6572 7369  a specific versi
 000135f0: 6f6e 0d0a 0d0a 2020 2020 7069 7078 2069  on....    pipx i
 00013600: 6e73 7461 6c6c 2064 6765 6e65 7261 7465  nstall dgenerate
-00013610: 3d3d 332e 342e 3220 5e0d 0a20 2020 202d  ==3.4.2 ^..    -
+00013610: 3d3d 332e 342e 3320 5e0d 0a20 2020 202d  ==3.4.3 ^..    -
 00013620: 2d70 6970 2d61 7267 7320 222d 2d65 7874  -pip-args "--ext
 00013630: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
 00013640: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
 00013650: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
 00013660: 3132 312f 220d 0a0d 0a20 2020 2023 2059  121/"....    # Y
 00013670: 6f75 2063 616e 2069 6e73 7461 6c6c 2077  ou can install w
 00013680: 6974 686f 7574 2070 6970 7820 696e 746f  ithout pipx into
 00013690: 2079 6f75 7220 6f77 6e20 656e 7669 726f   your own enviro
 000136a0: 6e6d 656e 7420 6c69 6b65 2073 6f0d 0a0d  nment like so...
 000136b0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
 000136c0: 2064 6765 6e65 7261 7465 3d3d 332e 342e   dgenerate==3.4.
-000136d0: 3220 2d2d 6578 7472 612d 696e 6465 782d  2 --extra-index-
+000136d0: 3320 2d2d 6578 7472 612d 696e 6465 782d  3 --extra-index-
 000136e0: 7572 6c20 6874 7470 733a 2f2f 646f 776e  url https://down
 000136f0: 6c6f 6164 2e70 7974 6f72 6368 2e6f 7267  load.pytorch.org
 00013700: 2f77 686c 2f63 7531 3231 2f0d 0a0d 0a0d  /whl/cu121/.....
 00013710: 0a49 7420 6973 2072 6563 6f6d 6d65 6e64  .It is recommend
 00013720: 6564 2074 6f20 696e 7374 616c 6c20 6467  ed to install dg
 00013730: 656e 6572 6174 6520 7769 7468 2070 6970  enerate with pip
 00013740: 7820 6966 2079 6f75 2061 7265 206a 7573  x if you are jus
@@ -5157,26 +5157,26 @@
 00014240: 6973 2e63 6f6d 2f6a 6178 2d72 656c 6561  is.com/jax-relea
 00014250: 7365 732f 6a61 785f 6375 6461 5f72 656c  ses/jax_cuda_rel
 00014260: 6561 7365 732e 6874 6d6c 220d 0a0d 0a20  eases.html".... 
 00014270: 2020 2023 2049 6620 796f 7520 7761 6e74     # If you want
 00014280: 2061 2073 7065 6369 6669 6320 7665 7273   a specific vers
 00014290: 696f 6e0d 0a0d 0a20 2020 2070 6970 7820  ion....    pipx 
 000142a0: 696e 7374 616c 6c20 6467 656e 6572 6174  install dgenerat
-000142b0: 653d 3d33 2e34 2e32 205c 0d0a 2020 2020  e==3.4.2 \..    
+000142b0: 653d 3d33 2e34 2e33 205c 0d0a 2020 2020  e==3.4.3 \..    
 000142c0: 2d2d 7069 702d 6172 6773 2022 2d2d 6578  --pip-args "--ex
 000142d0: 7472 612d 696e 6465 782d 7572 6c20 6874  tra-index-url ht
 000142e0: 7470 733a 2f2f 646f 776e 6c6f 6164 2e70  tps://download.p
 000142f0: 7974 6f72 6368 2e6f 7267 2f77 686c 2f63  ytorch.org/whl/c
 00014300: 7531 3231 2f22 0d0a 0d0a 2020 2020 2320  u121/"....    # 
 00014310: 5370 6563 6966 6963 2076 6572 7369 6f6e  Specific version
 00014320: 2077 6974 6820 666c 6178 2f6a 6178 2073   with flax/jax s
 00014330: 7570 706f 7274 0d0a 0d0a 2020 2020 7069  upport....    pi
 00014340: 7078 2069 6e73 7461 6c6c 2064 6765 6e65  px install dgene
 00014350: 7261 7465 5b66 6c61 785d 3d3d 332e 342e  rate[flax]==3.4.
-00014360: 3220 5c0d 0a20 2020 202d 2d70 6970 2d61  2 \..    --pip-a
+00014360: 3320 5c0d 0a20 2020 202d 2d70 6970 2d61  3 \..    --pip-a
 00014370: 7267 7320 222d 2d65 7874 7261 2d69 6e64  rgs "--extra-ind
 00014380: 6578 2d75 726c 2068 7474 7073 3a2f 2f64  ex-url https://d
 00014390: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
 000143a0: 6f72 672f 7768 6c2f 6375 3132 312f 205c  org/whl/cu121/ \
 000143b0: 0d0a 2020 2020 2d66 2068 7474 7073 3a2f  ..    -f https:/
 000143c0: 2f73 746f 7261 6765 2e67 6f6f 676c 6561  /storage.googlea
 000143d0: 7069 732e 636f 6d2f 6a61 782d 7265 6c65  pis.com/jax-rele
@@ -5184,23 +5184,23 @@
 000143f0: 6c65 6173 6573 2e68 746d 6c22 0d0a 0d0a  leases.html"....
 00014400: 2020 2020 2320 596f 7520 6361 6e20 696e      # You can in
 00014410: 7374 616c 6c20 7769 7468 6f75 7420 7069  stall without pi
 00014420: 7078 2069 6e74 6f20 796f 7572 206f 776e  px into your own
 00014430: 2065 6e76 6972 6f6e 6d65 6e74 206c 696b   environment lik
 00014440: 6520 736f 0d0a 0d0a 2020 2020 7069 7033  e so....    pip3
 00014450: 2069 6e73 7461 6c6c 2064 6765 6e65 7261   install dgenera
-00014460: 7465 3d3d 332e 342e 3220 2d2d 6578 7472  te==3.4.2 --extr
+00014460: 7465 3d3d 332e 342e 3320 2d2d 6578 7472  te==3.4.3 --extr
 00014470: 612d 696e 6465 782d 7572 6c20 6874 7470  a-index-url http
 00014480: 733a 2f2f 646f 776e 6c6f 6164 2e70 7974  s://download.pyt
 00014490: 6f72 6368 2e6f 7267 2f77 686c 2f63 7531  orch.org/whl/cu1
 000144a0: 3231 2f0d 0a0d 0a20 2020 2023 204f 7220  21/....    # Or 
 000144b0: 7769 7468 2066 6c61 780d 0a0d 0a20 2020  with flax....   
 000144c0: 2070 6970 3320 696e 7374 616c 6c20 6467   pip3 install dg
 000144d0: 656e 6572 6174 655b 666c 6178 5d3d 3d33  enerate[flax]==3
-000144e0: 2e34 2e32 202d 2d65 7874 7261 2d69 6e64  .4.2 --extra-ind
+000144e0: 2e34 2e33 202d 2d65 7874 7261 2d69 6e64  .4.3 --extra-ind
 000144f0: 6578 2d75 726c 2068 7474 7073 3a2f 2f64  ex-url https://d
 00014500: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
 00014510: 6f72 672f 7768 6c2f 6375 3132 312f 205c  org/whl/cu121/ \
 00014520: 0d0a 2020 2020 2d66 2068 7474 7073 3a2f  ..    -f https:/
 00014530: 2f73 746f 7261 6765 2e67 6f6f 676c 6561  /storage.googlea
 00014540: 7069 732e 636f 6d2f 6a61 782d 7265 6c65  pis.com/jax-rele
 00014550: 6173 6573 2f6a 6178 5f63 7564 615f 7265  ases/jax_cuda_re
@@ -5745,23 +5745,23 @@
 00016700: 2066 6f72 2062 7265 7669 7479 2e0d 0a0d   for brevity....
 00016710: 0a59 6f75 2063 616e 2064 6f77 6e6c 6f61  .You can downloa
 00016720: 6420 7468 656d 2068 6572 653a 0d0a 0d0a  d them here:....
 00016730: 202a 2060 6d79 2d69 6d61 6765 2d73 6565   * `my-image-see
 00016740: 642e 706e 6720 3c68 7474 7073 3a2f 2f72  d.png <https://r
 00016750: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
 00016760: 7465 6e74 2e63 6f6d 2f54 6572 696b 732f  tent.com/Teriks/
-00016770: 6467 656e 6572 6174 652f 7633 2e34 2e32  dgenerate/v3.4.2
+00016770: 6467 656e 6572 6174 652f 7633 2e34 2e33  dgenerate/v3.4.3
 00016780: 2f65 7861 6d70 6c65 732f 6d65 6469 612f  /examples/media/
 00016790: 646f 672d 6f6e 2d62 656e 6368 2e70 6e67  dog-on-bench.png
 000167a0: 3e60 5f0d 0a20 2a20 606d 792d 6d61 736b  >`_.. * `my-mask
 000167b0: 2d69 6d61 6765 2e70 6e67 203c 6874 7470  -image.png <http
 000167c0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
 000167d0: 6572 636f 6e74 656e 742e 636f 6d2f 5465  ercontent.com/Te
 000167e0: 7269 6b73 2f64 6765 6e65 7261 7465 2f76  riks/dgenerate/v
-000167f0: 332e 342e 322f 6578 616d 706c 6573 2f6d  3.4.2/examples/m
+000167f0: 332e 342e 332f 6578 616d 706c 6573 2f6d  3.4.3/examples/m
 00016800: 6564 6961 2f64 6f67 2d6f 6e2d 6265 6e63  edia/dog-on-benc
 00016810: 682d 6d61 736b 2e70 6e67 3e60 5f0d 0a0d  h-mask.png>`_...
 00016820: 0a54 6865 2063 6f6d 6d61 6e64 2062 656c  .The command bel
 00016830: 6f77 2067 656e 6572 6174 6573 2061 2063  ow generates a c
 00016840: 6174 2073 6974 7469 6e67 206f 6e20 6120  at sitting on a 
 00016850: 6265 6e63 6820 7769 7468 2074 6865 2069  bench with the i
 00016860: 6d61 6765 7320 6672 6f6d 2074 6865 206c  mages from the l
@@ -8356,15 +8356,15 @@
 00020a30: 7374 2069 6e66 6572 656e 6365 2073 7465  st inference ste
 00020a40: 702e 0d0a 0d0a 0d0a 5468 6573 6520 6578  p.......These ex
 00020a50: 616d 706c 6573 2075 7365 3a20 6076 6572  amples use: `ver
 00020a60: 6d65 6572 5f63 616e 6e79 5f65 6467 6564  meer_canny_edged
 00020a70: 2e70 6e67 203c 6874 7470 733a 2f2f 7261  .png <https://ra
 00020a80: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
 00020a90: 656e 742e 636f 6d2f 5465 7269 6b73 2f64  ent.com/Teriks/d
-00020aa0: 6765 6e65 7261 7465 2f76 332e 342e 322f  generate/v3.4.2/
+00020aa0: 6765 6e65 7261 7465 2f76 332e 342e 332f  generate/v3.4.3/
 00020ab0: 6578 616d 706c 6573 2f6d 6564 6961 2f76  examples/media/v
 00020ac0: 6572 6d65 6572 5f63 616e 6e79 5f65 6467  ermeer_canny_edg
 00020ad0: 6564 2e70 6e67 3e60 5f0d 0a0d 0a0d 0a2e  ed.png>`_.......
 00020ae0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2062  . code-block:: b
 00020af0: 6173 680d 0a0d 0a20 2020 2023 2054 6f72  ash....    # Tor
 00020b00: 6368 2065 7861 6d70 6c65 2c20 7573 6520  ch example, use 
 00020b10: 2276 6572 6d65 6572 5f63 616e 6e79 5f65  "vermeer_canny_e
@@ -8944,15 +8944,15 @@
 00022ef0: 7769 7468 2061 206d 6f64 656c 202b 2061  with a model + a
 00022f00: 2043 6f6e 7472 6f6c 4e65 742e 0d0a 0d0a   ControlNet.....
 00022f10: 5468 6973 2069 6d61 6765 206f 6620 6120  This image of a 
 00022f20: 6068 6f72 7365 203c 6874 7470 733a 2f2f  `horse <https://
 00022f30: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
 00022f40: 6e74 656e 742e 636f 6d2f 5465 7269 6b73  ntent.com/Teriks
 00022f50: 2f64 6765 6e65 7261 7465 2f76 332e 342e  /dgenerate/v3.4.
-00022f60: 322f 6578 616d 706c 6573 2f6d 6564 6961  2/examples/media
+00022f60: 332f 6578 616d 706c 6573 2f6d 6564 6961  3/examples/media
 00022f70: 2f68 6f72 7365 322e 6a70 6567 3e60 5f0d  /horse2.jpeg>`_.
 00022f80: 0a69 7320 7573 6564 2069 6e20 7468 6520  .is used in the 
 00022f90: 6578 616d 706c 6520 6265 6c6f 7720 7769  example below wi
 00022fa0: 7468 2061 2043 6f6e 7472 6f6c 4e65 7420  th a ControlNet 
 00022fb0: 7468 6174 2069 7320 7472 6169 6e65 6420  that is trained 
 00022fc0: 746f 2067 656e 6572 6174 6520 696d 6167  to generate imag
 00022fd0: 6573 2066 726f 6d20 6361 6e6e 7920 6564  es from canny ed
@@ -9183,15 +9183,15 @@
 00023de0: 5468 6520 696d 6167 6520 7573 6564 2069  The image used i
 00023df0: 6e20 7468 6520 6578 616d 706c 6520 6265  n the example be
 00023e00: 6c6f 7720 6973 2074 6869 7320 606c 6f77  low is this `low
 00023e10: 2072 6573 6f6c 7574 696f 6e20 6361 7420   resolution cat 
 00023e20: 3c68 7474 7073 3a2f 2f72 6177 2e67 6974  <https://raw.git
 00023e30: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
 00023e40: 6f6d 2f54 6572 696b 732f 6467 656e 6572  om/Teriks/dgener
-00023e50: 6174 652f 7633 2e34 2e32 2f65 7861 6d70  ate/v3.4.2/examp
+00023e50: 6174 652f 7633 2e34 2e33 2f65 7861 6d70  ate/v3.4.3/examp
 00023e60: 6c65 732f 6d65 6469 612f 6c6f 775f 7265  les/media/low_re
 00023e70: 735f 6361 742e 706e 673e 605f 0d0a 0d0a  s_cat.png>`_....
 00023e80: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
 00023e90: 6261 7368 0d0a 0d0a 2020 2020 2320 5468  bash....    # Th
 00023ea0: 6520 696d 6167 6520 7072 6f64 7563 6564  e image produced
 00023eb0: 2077 6974 6820 7468 6973 206d 6f64 656c   with this model
 00023ec0: 2077 696c 6c20 6265 0d0a 2020 2020 2320   will be..    # 
@@ -10183,15 +10183,15 @@
 00027c60: 6c6c 6f77 696e 6720 6973 2061 2063 6f6e  llowing is a con
 00027c70: 6669 6720 6669 6c65 2065 7861 6d70 6c65  fig file example
 00027c80: 2074 6861 7420 636f 7665 7273 2076 6572   that covers ver
 00027c90: 7920 6261 7369 6320 7379 6e74 6178 2063  y basic syntax c
 00027ca0: 6f6e 6365 7074 733a 0d0a 0d0a 2e2e 2063  oncepts:...... c
 00027cb0: 6f64 652d 626c 6f63 6b3a 3a20 6a69 6e6a  ode-block:: jinj
 00027cc0: 610d 0a0d 0a20 2020 2023 2120 6467 656e  a....    #! dgen
-00027cd0: 6572 6174 6520 332e 342e 320d 0a0d 0a20  erate 3.4.2.... 
+00027cd0: 6572 6174 6520 332e 342e 330d 0a0d 0a20  erate 3.4.3.... 
 00027ce0: 2020 2023 2049 6620 6120 6861 7368 2d62     # If a hash-b
 00027cf0: 616e 6720 7665 7273 696f 6e20 6973 2070  ang version is p
 00027d00: 726f 7669 6465 6420 696e 2074 6865 2066  rovided in the f
 00027d10: 6f72 6d61 7420 6162 6f76 650d 0a20 2020  ormat above..   
 00027d20: 2023 2061 2077 6172 6e69 6e67 2077 696c   # a warning wil
 00027d30: 6c20 6265 2070 726f 6475 6365 6420 6966  l be produced if
 00027d40: 2074 6865 2076 6572 7369 6f6e 2079 6f75   the version you
@@ -10450,15 +10450,15 @@
 00028d10: 6162 6c65 7320 7365 7420 7769 7468 2074  ables set with t
 00028d20: 6865 2060 605c 7365 7460 6020 6469 7265  he ``\set`` dire
 00028d30: 6374 6976 6520 7769 6c6c 2061 6c73 6f20  ctive will also 
 00028d40: 6265 206d 656e 7469 6f6e 6564 2069 6e20  be mentioned in 
 00028d50: 7468 6973 206f 7574 7075 742e 0d0a 0d0a  this output.....
 00028d60: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
 00028d70: 6a69 6e6a 610d 0a0d 0a20 2020 2023 2120  jinja....    #! 
-00028d80: 6467 656e 6572 6174 6520 332e 342e 320d  dgenerate 3.4.2.
+00028d80: 6467 656e 6572 6174 6520 332e 342e 330d  dgenerate 3.4.3.
 00028d90: 0a0d 0a20 2020 2023 2049 6e76 6f63 6174  ...    # Invocat
 00028da0: 696f 6e20 7769 6c6c 2070 726f 6365 6564  ion will proceed
 00028db0: 2061 7320 6e6f 726d 616c 0d0a 0d0a 2020   as normal....  
 00028dc0: 2020 7374 6162 696c 6974 7961 692f 7374    stabilityai/st
 00028dd0: 6162 6c65 2d64 6966 6675 7369 6f6e 2d32  able-diffusion-2
 00028de0: 2d31 202d 2d70 726f 6d70 7473 2022 6120  -1 --prompts "a 
 00028df0: 6d61 6e20 7761 6c6b 696e 6720 6f6e 2074  man walking on t
@@ -11236,15 +11236,15 @@
 0002be30: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
 0002be40: 7468 6520 7370 6563 6966 6965 6420 6469  the specified di
 0002be50: 7265 6374 6976 6573 2e20 5468 6520 6261  rectives. The ba
 0002be60: 636b 736c 6173 6820 6d61 7920 6265 206f  ckslash may be o
 0002be70: 6d69 7474 6564 2e0d 0a0d 0a0d 0a2e 2e20  mitted......... 
 0002be80: 636f 6465 2d62 6c6f 636b 3a3a 206a 696e  code-block:: jin
 0002be90: 6a61 0d0a 0d0a 2020 2020 2321 2064 6765  ja....    #! dge
-0002bea0: 6e65 7261 7465 2033 2e34 2e32 0d0a 0d0a  nerate 3.4.2....
+0002bea0: 6e65 7261 7465 2033 2e34 2e33 0d0a 0d0a  nerate 3.4.3....
 0002beb0: 2020 2020 2320 596f 7520 6361 6e20 6465      # You can de
 0002bec0: 6669 6e65 2079 6f75 7220 6f77 6e20 7465  fine your own te
 0002bed0: 6d70 6c61 7465 2076 6172 6961 626c 6573  mplate variables
 0002bee0: 2077 6974 6820 7468 6520 5c73 6574 2064   with the \set d
 0002bef0: 6972 6563 7469 7665 0d0a 2020 2020 2320  irective..    # 
 0002bf00: 7468 6520 5c73 6574 2064 6972 6563 7469  the \set directi
 0002bf10: 7665 2064 6f65 7320 6e6f 7420 646f 2061  ve does not do a
@@ -11689,15 +11689,15 @@
 0002da80: 796f 750d 0a63 616e 2067 6c6f 6220 6469  you..can glob di
 0002da90: 7265 6374 6f72 6965 7320 7573 696e 6720  rectories using 
 0002daa0: 6675 6e63 7469 6f6e 7320 6672 6f6d 2074  functions from t
 0002dab0: 6865 2067 6c6f 6220 6d6f 6475 6c65 206c  he glob module l
 0002dac0: 696b 6520 736f 3a0d 0a0d 0a2e 2e20 636f  ike so:...... co
 0002dad0: 6465 2d62 6c6f 636b 3a3a 206a 696e 6a61  de-block:: jinja
 0002dae0: 0d0a 0d0a 2020 2020 2321 2064 6765 6e65  ....    #! dgene
-0002daf0: 7261 7465 2033 2e34 2e32 0d0a 0d0a 2020  rate 3.4.2....  
+0002daf0: 7261 7465 2033 2e34 2e33 0d0a 0d0a 2020  rate 3.4.3....  
 0002db00: 2020 2320 5468 6520 6d6f 7374 2062 6173    # The most bas
 0002db10: 6963 2075 7361 6765 2069 7320 6675 6c6c  ic usage is full
 0002db20: 2065 7870 616e 7369 6f6e 206f 6620 6576   expansion of ev
 0002db30: 6572 7920 6669 6c65 0d0a 0d0a 2020 2020  ery file....    
 0002db40: 5c73 6574 206d 7966 696c 6573 207b 7b20  \set myfiles {{ 
 0002db50: 7175 6f74 6528 676c 6f62 2e67 6c6f 6228  quote(glob.glob(
 0002db60: 276d 795f 696d 6167 6573 2f2a 2e70 6e67  'my_images/*.png
@@ -11734,15 +11734,15 @@
 0002dd50: 636f 6d6d 616e 6420 6060 696d 6167 652d  command ``image-
 0002dd60: 7072 6f63 6573 7360 6020 6861 7320 6120  process`` has a 
 0002dd70: 636f 6e66 6967 2064 6972 6563 7469 7665  config directive
 0002dd80: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2e   implementation.
 0002dd90: 0d0a 0d0a 0d0a 2e2e 2063 6f64 652d 626c  ........ code-bl
 0002dda0: 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d 0a20  ock:: jinja.... 
 0002ddb0: 2020 2023 2120 6467 656e 6572 6174 6520     #! dgenerate 
-0002ddc0: 332e 342e 320d 0a0d 0a20 2020 2023 2070  3.4.2....    # p
+0002ddc0: 332e 342e 330d 0a0d 0a20 2020 2023 2070  3.4.3....    # p
 0002ddd0: 7269 6e74 2074 6865 2068 656c 7020 6d65  rint the help me
 0002dde0: 7373 6167 6520 6f66 202d 2d73 7562 2d63  ssage of --sub-c
 0002ddf0: 6f6d 6d61 6e64 2069 6d61 6765 2d70 726f  ommand image-pro
 0002de00: 6365 7373 2c20 7468 6973 2064 6f65 730d  cess, this does.
 0002de10: 0a20 2020 2023 206e 6f74 2063 6175 7365  .    # not cause
 0002de20: 2074 6865 2063 6f6e 6669 6720 746f 2065   the config to e
 0002de30: 7869 740d 0a0d 0a20 2020 205c 696d 6167  xit....    \imag
@@ -11794,15 +11794,15 @@
 0002e110: 596f 7520 6361 6e20 6578 6974 2061 2063  You can exit a c
 0002e120: 6f6e 6669 6720 6561 726c 7920 6966 206e  onfig early if n
 0002e130: 6565 6420 6265 2075 7369 6e67 2074 6865  eed be using the
 0002e140: 2060 605c 6578 6974 6060 2064 6972 6563   ``\exit`` direc
 0002e150: 7469 7665 0d0a 0d0a 0d0a 2e2e 2063 6f64  tive........ cod
 0002e160: 652d 626c 6f63 6b3a 3a20 6a69 6e6a 610d  e-block:: jinja.
 0002e170: 0a0d 0a20 2020 2023 2120 6467 656e 6572  ...    #! dgener
-0002e180: 6174 6520 332e 342e 320d 0a0d 0a20 2020  ate 3.4.2....   
+0002e180: 6174 6520 332e 342e 330d 0a0d 0a20 2020  ate 3.4.3....   
 0002e190: 2023 2065 7869 7420 7468 6520 7072 6f63   # exit the proc
 0002e1a0: 6573 7320 7769 7468 2072 6574 7572 6e20  ess with return 
 0002e1b0: 636f 6465 2031 2c20 7768 6963 6820 696e  code 1, which in
 0002e1c0: 6469 6361 7465 7320 616e 2065 7272 6f72  dicates an error
 0002e1d0: 0d0a 0d0a 2020 2020 5c70 7269 6e74 2022  ....    \print "
 0002e1e0: 736f 6d65 2065 7272 6f72 206f 6363 7572  some error occur
 0002e1f0: 7265 6422 0d0a 2020 2020 5c65 7869 7420  red"..    \exit 
@@ -11952,42 +11952,42 @@
 0002eaf0: 6520 7072 6f63 6573 736f 7220 706c 7567  e processor plug
 0002eb00: 696e 7320 6361 6e20 6265 2066 6f75 6e64  ins can be found
 0002eb10: 0d0a 696e 2074 6865 2060 2277 7269 7469  ..in the `"writi
 0002eb20: 6e67 5f70 6c75 6769 6e73 2f69 6d61 6765  ng_plugins/image
 0002eb30: 5f70 726f 6365 7373 6f72 2220 3c68 7474  _processor" <htt
 0002eb40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 0002eb50: 5465 7269 6b73 2f64 6765 6e65 7261 7465  Teriks/dgenerate
-0002eb60: 2f74 7265 652f 7633 2e34 2e32 2f65 7861  /tree/v3.4.2/exa
+0002eb60: 2f74 7265 652f 7633 2e34 2e33 2f65 7861  /tree/v3.4.3/exa
 0002eb70: 6d70 6c65 732f 7772 6974 696e 675f 706c  mples/writing_pl
 0002eb80: 7567 696e 732f 696d 6167 655f 7072 6f63  ugins/image_proc
 0002eb90: 6573 736f 723e 605f 0d0a 666f 6c64 6572  essor>`_..folder
 0002eba0: 206f 6620 7468 6520 6578 616d 706c 6573   of the examples
 0002ebb0: 2066 6f6c 6465 722e 0d0a 0d0a 5468 6520   folder.....The 
 0002ebc0: 736f 7572 6365 2063 6f64 6520 666f 7220  source code for 
 0002ebd0: 7468 6520 6275 696c 7420 696e 2060 6361  the built in `ca
 0002ebe0: 6e6e 7920 3c68 7474 7073 3a2f 2f67 6974  nny <https://git
 0002ebf0: 6875 622e 636f 6d2f 5465 7269 6b73 2f64  hub.com/Teriks/d
 0002ec00: 6765 6e65 7261 7465 2f62 6c6f 622f 7633  generate/blob/v3
-0002ec10: 2e34 2e32 2f64 6765 6e65 7261 7465 2f69  .4.2/dgenerate/i
+0002ec10: 2e34 2e33 2f64 6765 6e65 7261 7465 2f69  .4.3/dgenerate/i
 0002ec20: 6d61 6765 7072 6f63 6573 736f 7273 2f63  mageprocessors/c
 0002ec30: 616e 6e79 2e70 793e 605f 2070 726f 6365  anny.py>`_ proce
 0002ec40: 7373 6f72 2c0d 0a74 6865 2060 6f70 656e  ssor,..the `open
 0002ec50: 706f 7365 203c 6874 7470 733a 2f2f 6769  pose <https://gi
 0002ec60: 7468 7562 2e63 6f6d 2f54 6572 696b 732f  thub.com/Teriks/
 0002ec70: 6467 656e 6572 6174 652f 626c 6f62 2f76  dgenerate/blob/v
-0002ec80: 332e 342e 322f 6467 656e 6572 6174 652f  3.4.2/dgenerate/
+0002ec80: 332e 342e 332f 6467 656e 6572 6174 652f  3.4.3/dgenerate/
 0002ec90: 696d 6167 6570 726f 6365 7373 6f72 732f  imageprocessors/
 0002eca0: 6f70 656e 706f 7365 2e70 793e 605f 2070  openpose.py>`_ p
 0002ecb0: 726f 6365 7373 6f72 2c20 616e 6420 7468  rocessor, and th
 0002ecc0: 6520 7369 6d70 6c65 0d0a 6070 696c 6c6f  e simple..`pillo
 0002ecd0: 7720 696d 6167 6520 6f70 6572 6174 696f  w image operatio
 0002ece0: 6e73 203c 6874 7470 733a 2f2f 6769 7468  ns <https://gith
 0002ecf0: 7562 2e63 6f6d 2f54 6572 696b 732f 6467  ub.com/Teriks/dg
 0002ed00: 656e 6572 6174 652f 626c 6f62 2f76 332e  enerate/blob/v3.
-0002ed10: 342e 322f 6467 656e 6572 6174 652f 696d  4.2/dgenerate/im
+0002ed10: 342e 332f 6467 656e 6572 6174 652f 696d  4.3/dgenerate/im
 0002ed20: 6167 6570 726f 6365 7373 6f72 732f 696d  ageprocessors/im
 0002ed30: 6167 656f 7073 2e70 793e 605f 2070 726f  ageops.py>`_ pro
 0002ed40: 6365 7373 6f72 7320 6361 6e20 616c 736f  cessors can also
 0002ed50: 0d0a 6265 206f 6620 7265 6665 7265 6e63  ..be of referenc
 0002ed60: 6520 6173 2074 6865 7920 6172 6520 7772  e as they are wr
 0002ed70: 6974 7465 6e20 6173 2069 6e74 6572 6e61  itten as interna
 0002ed80: 6c20 696d 6167 6520 7072 6f63 6573 736f  l image processo
@@ -11996,15 +11996,15 @@
 0002edb0: 7469 6e67 2063 6f6e 6669 6720 6469 7265  ting config dire
 0002edc0: 6374 6976 6573 2063 616e 2062 6520 666f  ctives can be fo
 0002edd0: 756e 6420 696e 2074 6865 0d0a 6022 7772  und in the..`"wr
 0002ede0: 6974 696e 675f 706c 7567 696e 732f 636f  iting_plugins/co
 0002edf0: 6e66 6967 5f64 6972 6563 7469 7665 2220  nfig_directive" 
 0002ee00: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
 0002ee10: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-0002ee20: 7261 7465 2f74 7265 652f 7633 2e34 2e32  rate/tree/v3.4.2
+0002ee20: 7261 7465 2f74 7265 652f 7633 2e34 2e33  rate/tree/v3.4.3
 0002ee30: 2f65 7861 6d70 6c65 732f 7772 6974 696e  /examples/writin
 0002ee40: 675f 706c 7567 696e 732f 636f 6e66 6967  g_plugins/config
 0002ee50: 5f64 6972 6563 7469 7665 3e60 5f20 666f  _directive>`_ fo
 0002ee60: 6c64 6572 0d0a 6f66 2074 6865 2065 7861  lder..of the exa
 0002ee70: 6d70 6c65 7320 666f 6c64 6572 2e0d 0a0d  mples folder....
 0002ee80: 0a43 7572 7265 6e74 6c79 2074 6865 206f  .Currently the o
 0002ee90: 6e6c 7920 696e 7465 726e 616c 2064 6972  nly internal dir
@@ -12014,15 +12014,15 @@
 0002eed0: 5c69 6d61 6765 5f70 726f 6365 7373 6060  \image_process``
 0002eee0: 2064 6972 6563 7469 7665 2c0d 0a77 686f   directive,..who
 0002eef0: 2773 2073 6f75 7263 6520 6669 6c65 2060  's source file `
 0002ef00: 6361 6e20 6265 206c 6f63 6174 6564 2068  can be located h
 0002ef10: 6572 6520 3c68 7474 7073 3a2f 2f67 6974  ere <https://git
 0002ef20: 6875 622e 636f 6d2f 5465 7269 6b73 2f64  hub.com/Teriks/d
 0002ef30: 6765 6e65 7261 7465 2f62 6c6f 622f 7633  generate/blob/v3
-0002ef40: 2e34 2e32 2f64 6765 6e65 7261 7465 2f62  .4.2/dgenerate/b
+0002ef40: 2e34 2e33 2f64 6765 6e65 7261 7465 2f62  .4.3/dgenerate/b
 0002ef50: 6174 6368 7072 6f63 6573 732f 696d 6167  atchprocess/imag
 0002ef60: 655f 7072 6f63 6573 735f 6469 7265 6374  e_process_direct
 0002ef70: 6976 652e 7079 3e60 5f2c 0d0a 7468 6520  ive.py>`_,..the 
 0002ef80: 736f 7572 6365 2066 696c 6520 666f 7220  source file for 
 0002ef90: 7468 6973 2064 6972 6563 7469 7665 2069  this directive i
 0002efa0: 7320 7465 7273 6520 6173 206d 6f73 7420  s terse as most 
 0002efb0: 6f66 2060 605c 696d 6167 655f 7072 6f63  of ``\image_proc
@@ -12035,15 +12035,15 @@
 0002f020: 7768 6963 6820 6973 2061 6c73 6f20 7573  which is also us
 0002f030: 6564 2066 6f72 2060 602d 2d73 7562 2d63  ed for ``--sub-c
 0002f040: 6f6d 6d61 6e64 2069 6d61 6765 2d70 726f  ommand image-pro
 0002f050: 6365 7373 6060 2069 730d 0a60 6973 2069  cess`` is..`is i
 0002f060: 6d70 6c65 6d65 6e74 6564 2068 6572 6520  mplemented here 
 0002f070: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
 0002f080: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-0002f090: 7261 7465 2f62 6c6f 622f 7633 2e34 2e32  rate/blob/v3.4.2
+0002f090: 7261 7465 2f62 6c6f 622f 7633 2e34 2e33  rate/blob/v3.4.3
 0002f0a0: 2f64 6765 6e65 7261 7465 2f69 6d61 6765  /dgenerate/image
 0002f0b0: 5f70 726f 6365 7373 3e60 5f2e 0d0a 0d0a  _process>`_.....
 0002f0c0: 4669 6c65 2043 6163 6865 2043 6f6e 7472  File Cache Contr
 0002f0d0: 6f6c 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ol..============
 0002f0e0: 3d3d 3d3d 3d3d 0d0a 0d0a 6467 656e 6572  ======....dgener
 0002f0f0: 6174 6520 7769 6c6c 2063 6163 6865 2060  ate will cache `
 0002f100: 602d 2d69 6d61 6765 2d73 6565 6473 6060  `--image-seeds``
```

### Comparing `dgenerate-3.4.2/README.rst` & `dgenerate-3.4.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 00000000: 2e2e 207c 446f 6375 6d65 6e74 6174 696f  .. |Documentatio
 00000010: 6e20 5374 6174 7573 7c20 696d 6167 653a  n Status| image:
 00000020: 3a20 6874 7470 733a 2f2f 7265 6164 7468  : https://readth
 00000030: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
 00000040: 7473 2f64 6765 6e65 7261 7465 2f62 6164  ts/dgenerate/bad
 00000050: 6765 2f3f 7665 7273 696f 6e3d 7633 2e34  ge/?version=v3.4
-00000060: 2e32 0d0a 2020 203a 7461 7267 6574 3a20  .2..   :target: 
+00000060: 2e33 0d0a 2020 203a 7461 7267 6574 3a20  .3..   :target: 
 00000070: 6874 7470 3a2f 2f64 6765 6e65 7261 7465  http://dgenerate
 00000080: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000090: 656e 2f76 332e 342e 322f 0d0a 0d0a 4f76  en/v3.4.2/....Ov
+00000090: 656e 2f76 332e 342e 332f 0d0a 0d0a 4f76  en/v3.4.3/....Ov
 000000a0: 6572 7669 6577 0d0a 3d3d 3d3d 3d3d 3d3d  erview..========
 000000b0: 0d0a 0d0a 7c44 6f63 756d 656e 7461 7469  ....|Documentati
 000000c0: 6f6e 2053 7461 7475 737c 0d0a 0d0a 2a2a  on Status|....**
 000000d0: 6467 656e 6572 6174 652a 2a20 6973 2061  dgenerate** is a
 000000e0: 2063 6f6d 6d61 6e64 206c 696e 6520 746f   command line to
 000000f0: 6f6c 2061 6e64 206c 6962 7261 7279 2066  ol and library f
 00000100: 6f72 2067 656e 6572 6174 696e 6720 696d  or generating im
@@ -129,15 +129,15 @@
 00000800: 206f 7065 7261 7469 6f6e 7320 6275 7420   operations but 
 00000810: 6578 7472 616f 7264 696e 6172 696c 7920  extraordinarily 
 00000820: 736c 6f77 2e0d 0a0d 0a46 6f72 206c 6962  slow.....For lib
 00000830: 7261 7279 2064 6f63 756d 656e 7461 7469  rary documentati
 00000840: 6f6e 2076 6973 6974 2060 7265 6164 7468  on visit `readth
 00000850: 6564 6f63 7320 3c68 7474 703a 2f2f 6467  edocs <http://dg
 00000860: 656e 6572 6174 652e 7265 6164 7468 6564  enerate.readthed
-00000870: 6f63 732e 696f 2f65 6e2f 7633 2e34 2e32  ocs.io/en/v3.4.2
+00000870: 6f63 732e 696f 2f65 6e2f 7633 2e34 2e33  ocs.io/en/v3.4.3
 00000880: 2f3e 605f 2e0d 0a0d 0a2d 2d2d 2d0d 0a0d  />`_.....----...
 00000890: 0a2a 2048 6f77 2074 6f20 696e 7374 616c  .* How to instal
 000008a0: 6c0d 0a20 2020 202a 2060 5769 6e64 6f77  l..    * `Window
 000008b0: 7320 496e 7374 616c 6c60 5f0d 0a20 2020  s Install`_..   
 000008c0: 202a 2060 4c69 6e75 7820 6f72 2057 534c   * `Linux or WSL
 000008d0: 2049 6e73 7461 6c6c 605f 0d0a 0d0a 2a20   Install`_....* 
 000008e0: 5573 6167 6520 4578 616d 706c 6573 0d0a  Usage Examples..
@@ -4413,15 +4413,15 @@
 000113c0: 2076 616c 7565 3a20 2275 7365 645f 7065   value: "used_pe
 000113d0: 7263 656e 7420 3e20 3730 2220 466f 720d  rcent > 70" For.
 000113e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000113f0: 2020 2020 2020 2020 2020 2020 2053 796e               Syn
 00011400: 7461 7820 5365 653a 205b 6874 7470 733a  tax See: [https:
 00011410: 2f2f 6467 656e 6572 6174 652e 7265 6164  //dgenerate.read
 00011420: 7468 6564 6f63 732e 696f 2f65 6e2f 7633  thedocs.io/en/v3
-00011430: 2e34 2e32 2f64 6765 6e65 7261 7465 5f73  .4.2/dgenerate_s
+00011430: 2e34 2e33 2f64 6765 6e65 7261 7465 5f73  .4.3/dgenerate_s
 00011440: 7562 6d6f 6475 6c65 732e 6874 6d0d 0a20  ubmodules.htm.. 
 00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011460: 2020 2020 2020 2020 2020 206c 2364 6765             l#dge
 00011470: 6e65 7261 7465 2e70 6970 656c 696e 6577  nerate.pipelinew
 00011480: 7261 7070 6572 2e43 4143 4845 5f4d 454d  rapper.CACHE_MEM
 00011490: 4f52 595f 434f 4e53 5452 4149 4e54 535d  ORY_CONSTRAINTS]
 000114a0: 0d0a 2020 2020 2020 2d70 6d63 2045 5850  ..      -pmc EXP
@@ -4463,15 +4463,15 @@
 000116e0: 653a 2022 7069 7065 6c69 6e65 5f73 697a  e: "pipeline_siz
 000116f0: 6520 3e20 2861 7661 696c 6162 6c65 202a  e > (available *
 00011700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011710: 2020 2020 2020 2020 2020 2020 2020 302e                0.
 00011720: 3735 2922 2046 6f72 2053 796e 7461 7820  75)" For Syntax 
 00011730: 5365 653a 205b 6874 7470 733a 2f2f 6467  See: [https://dg
 00011740: 656e 6572 6174 652e 7265 6164 7468 6564  enerate.readthed
-00011750: 6f63 732e 696f 2f65 6e2f 7633 2e34 2e32  ocs.io/en/v3.4.2
+00011750: 6f63 732e 696f 2f65 6e2f 7633 2e34 2e33  ocs.io/en/v3.4.3
 00011760: 2f64 6765 6e65 7261 7465 5f73 7562 0d0a  /dgenerate_sub..
 00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011780: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
 00011790: 6c65 732e 6874 6d6c 2364 6765 6e65 7261  les.html#dgenera
 000117a0: 7465 2e70 6970 656c 696e 6577 7261 7070  te.pipelinewrapp
 000117b0: 6572 2e50 4950 454c 494e 455f 4341 4348  er.PIPELINE_CACH
 000117c0: 455f 4d45 4d4f 5259 5f43 4f4e 5354 5241  E_MEMORY_CONSTRA
@@ -4513,15 +4513,15 @@
 00011a00: 6e65 745f 7369 7a65 203e 2028 6176 6169  net_size > (avai
 00011a10: 6c61 626c 6520 2a20 302e 3735 2922 2046  lable * 0.75)" F
 00011a20: 6f72 2053 796e 7461 7820 5365 653a 205b  or Syntax See: [
 00011a30: 6874 7470 733a 2f2f 6467 650d 0a20 2020  https://dge..   
 00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011a50: 2020 2020 2020 2020 206e 6572 6174 652e           nerate.
 00011a60: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00011a70: 6e2f 7633 2e34 2e32 2f64 6765 6e65 7261  n/v3.4.2/dgenera
+00011a70: 6e2f 7633 2e34 2e33 2f64 6765 6e65 7261  n/v3.4.3/dgenera
 00011a80: 7465 5f73 7562 6d6f 6475 6c65 732e 6874  te_submodules.ht
 00011a90: 6d6c 2364 6765 6e65 7261 7465 2e70 6970  ml#dgenerate.pip
 00011aa0: 656c 696e 6577 7261 700d 0a20 2020 2020  elinewrap..     
 00011ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011ac0: 2020 2020 2020 2070 6572 2e55 4e45 545f         per.UNET_
 00011ad0: 4341 4348 455f 4d45 4d4f 5259 5f43 4f4e  CACHE_MEMORY_CON
 00011ae0: 5354 5241 494e 5453 5d0d 0a20 2020 2020  STRAINTS]..     
@@ -4562,15 +4562,15 @@
 00011d10: 6165 5f73 697a 6520 3e20 2861 7661 696c  ae_size > (avail
 00011d20: 6162 6c65 202a 2030 2e37 3529 2220 466f  able * 0.75)" Fo
 00011d30: 7220 5379 6e74 6178 2053 6565 3a20 5b68  r Syntax See: [h
 00011d40: 7474 7073 3a2f 2f64 6765 6e0d 0a20 2020  ttps://dgen..   
 00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011d60: 2020 2020 2020 2020 2065 7261 7465 2e72           erate.r
 00011d70: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00011d80: 2f76 332e 342e 322f 6467 656e 6572 6174  /v3.4.2/dgenerat
+00011d80: 2f76 332e 342e 332f 6467 656e 6572 6174  /v3.4.3/dgenerat
 00011d90: 655f 7375 626d 6f64 756c 6573 2e68 746d  e_submodules.htm
 00011da0: 6c23 6467 656e 6572 6174 652e 7069 7065  l#dgenerate.pipe
 00011db0: 6c69 6e65 7772 6170 700d 0a20 2020 2020  linewrapp..     
 00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011dd0: 2020 2020 2020 2065 722e 5641 455f 4341         er.VAE_CA
 00011de0: 4348 455f 4d45 4d4f 5259 5f43 4f4e 5354  CHE_MEMORY_CONST
 00011df0: 5241 494e 5453 5d0d 0a20 2020 2020 202d  RAINTS]..      -
@@ -4613,15 +4613,15 @@
 00012040: 6c5f 6e65 745f 7369 7a65 203e 2028 6176  l_net_size > (av
 00012050: 6169 6c61 626c 6520 2a20 302e 3735 2922  ailable * 0.75)"
 00012060: 2046 6f72 0d0a 2020 2020 2020 2020 2020   For..          
 00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012080: 2020 5379 6e74 6178 2053 6565 3a20 5b68    Syntax See: [h
 00012090: 7474 7073 3a2f 2f64 6765 6e65 7261 7465  ttps://dgenerate
 000120a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000120b0: 656e 2f76 332e 342e 322f 6467 656e 6572  en/v3.4.2/dgener
+000120b0: 656e 2f76 332e 342e 332f 6467 656e 6572  en/v3.4.3/dgener
 000120c0: 6174 655f 7375 626d 6f64 756c 6573 2e68  ate_submodules.h
 000120d0: 746d 0d0a 2020 2020 2020 2020 2020 2020  tm..            
 000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000120f0: 6c23 6467 656e 6572 6174 652e 7069 7065  l#dgenerate.pipe
 00012100: 6c69 6e65 7772 6170 7065 722e 434f 4e54  linewrapper.CONT
 00012110: 524f 4c5f 4e45 545f 4341 4348 455f 4d45  ROL_NET_CACHE_ME
 00012120: 4d4f 5259 5f43 4f4e 5354 5241 494e 5453  MORY_CONSTRAINTS
@@ -4706,26 +4706,26 @@
 00012610: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
 00012620: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
 00012630: 3132 312f 220d 0a0d 0a20 2020 2023 2049  121/"....    # I
 00012640: 6620 796f 7520 7761 6e74 2061 2073 7065  f you want a spe
 00012650: 6369 6669 6320 7665 7273 696f 6e0d 0a0d  cific version...
 00012660: 0a20 2020 2070 6970 7820 696e 7374 616c  .    pipx instal
 00012670: 6c20 6467 656e 6572 6174 653d 3d33 2e34  l dgenerate==3.4
-00012680: 2e32 205e 0d0a 2020 2020 2d2d 7069 702d  .2 ^..    --pip-
+00012680: 2e33 205e 0d0a 2020 2020 2d2d 7069 702d  .3 ^..    --pip-
 00012690: 6172 6773 2022 2d2d 6578 7472 612d 696e  args "--extra-in
 000126a0: 6465 782d 7572 6c20 6874 7470 733a 2f2f  dex-url https://
 000126b0: 646f 776e 6c6f 6164 2e70 7974 6f72 6368  download.pytorch
 000126c0: 2e6f 7267 2f77 686c 2f63 7531 3231 2f22  .org/whl/cu121/"
 000126d0: 0d0a 0d0a 2020 2020 2320 596f 7520 6361  ....    # You ca
 000126e0: 6e20 696e 7374 616c 6c20 7769 7468 6f75  n install withou
 000126f0: 7420 7069 7078 2069 6e74 6f20 796f 7572  t pipx into your
 00012700: 206f 776e 2065 6e76 6972 6f6e 6d65 6e74   own environment
 00012710: 206c 696b 6520 736f 0d0a 0d0a 2020 2020   like so....    
 00012720: 7069 7020 696e 7374 616c 6c20 6467 656e  pip install dgen
-00012730: 6572 6174 653d 3d33 2e34 2e32 202d 2d65  erate==3.4.2 --e
+00012730: 6572 6174 653d 3d33 2e34 2e33 202d 2d65  erate==3.4.3 --e
 00012740: 7874 7261 2d69 6e64 6578 2d75 726c 2068  xtra-index-url h
 00012750: 7474 7073 3a2f 2f64 6f77 6e6c 6f61 642e  ttps://download.
 00012760: 7079 746f 7263 682e 6f72 672f 7768 6c2f  pytorch.org/whl/
 00012770: 6375 3132 312f 0d0a 0d0a 0d0a 4974 2069  cu121/......It i
 00012780: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
 00012790: 2069 6e73 7461 6c6c 2064 6765 6e65 7261   install dgenera
 000127a0: 7465 2077 6974 6820 7069 7078 2069 6620  te with pipx if 
@@ -4908,25 +4908,25 @@
 000132b0: 6d2f 6a61 782d 7265 6c65 6173 6573 2f6a  m/jax-releases/j
 000132c0: 6178 5f63 7564 615f 7265 6c65 6173 6573  ax_cuda_releases
 000132d0: 2e68 746d 6c22 0d0a 0d0a 2020 2020 2320  .html"....    # 
 000132e0: 4966 2079 6f75 2077 616e 7420 6120 7370  If you want a sp
 000132f0: 6563 6966 6963 2076 6572 7369 6f6e 0d0a  ecific version..
 00013300: 0d0a 2020 2020 7069 7078 2069 6e73 7461  ..    pipx insta
 00013310: 6c6c 2064 6765 6e65 7261 7465 3d3d 332e  ll dgenerate==3.
-00013320: 342e 3220 5c0d 0a20 2020 202d 2d70 6970  4.2 \..    --pip
+00013320: 342e 3320 5c0d 0a20 2020 202d 2d70 6970  4.3 \..    --pip
 00013330: 2d61 7267 7320 222d 2d65 7874 7261 2d69  -args "--extra-i
 00013340: 6e64 6578 2d75 726c 2068 7474 7073 3a2f  ndex-url https:/
 00013350: 2f64 6f77 6e6c 6f61 642e 7079 746f 7263  /download.pytorc
 00013360: 682e 6f72 672f 7768 6c2f 6375 3132 312f  h.org/whl/cu121/
 00013370: 220d 0a0d 0a20 2020 2023 2053 7065 6369  "....    # Speci
 00013380: 6669 6320 7665 7273 696f 6e20 7769 7468  fic version with
 00013390: 2066 6c61 782f 6a61 7820 7375 7070 6f72   flax/jax suppor
 000133a0: 740d 0a0d 0a20 2020 2070 6970 7820 696e  t....    pipx in
 000133b0: 7374 616c 6c20 6467 656e 6572 6174 655b  stall dgenerate[
-000133c0: 666c 6178 5d3d 3d33 2e34 2e32 205c 0d0a  flax]==3.4.2 \..
+000133c0: 666c 6178 5d3d 3d33 2e34 2e33 205c 0d0a  flax]==3.4.3 \..
 000133d0: 2020 2020 2d2d 7069 702d 6172 6773 2022      --pip-args "
 000133e0: 2d2d 6578 7472 612d 696e 6465 782d 7572  --extra-index-ur
 000133f0: 6c20 6874 7470 733a 2f2f 646f 776e 6c6f  l https://downlo
 00013400: 6164 2e70 7974 6f72 6368 2e6f 7267 2f77  ad.pytorch.org/w
 00013410: 686c 2f63 7531 3231 2f20 5c0d 0a20 2020  hl/cu121/ \..   
 00013420: 202d 6620 6874 7470 733a 2f2f 7374 6f72   -f https://stor
 00013430: 6167 652e 676f 6f67 6c65 6170 6973 2e63  age.googleapis.c
@@ -4935,22 +4935,22 @@
 00013460: 732e 6874 6d6c 220d 0a0d 0a20 2020 2023  s.html"....    #
 00013470: 2059 6f75 2063 616e 2069 6e73 7461 6c6c   You can install
 00013480: 2077 6974 686f 7574 2070 6970 7820 696e   without pipx in
 00013490: 746f 2079 6f75 7220 6f77 6e20 656e 7669  to your own envi
 000134a0: 726f 6e6d 656e 7420 6c69 6b65 2073 6f0d  ronment like so.
 000134b0: 0a0d 0a20 2020 2070 6970 3320 696e 7374  ...    pip3 inst
 000134c0: 616c 6c20 6467 656e 6572 6174 653d 3d33  all dgenerate==3
-000134d0: 2e34 2e32 202d 2d65 7874 7261 2d69 6e64  .4.2 --extra-ind
+000134d0: 2e34 2e33 202d 2d65 7874 7261 2d69 6e64  .4.3 --extra-ind
 000134e0: 6578 2d75 726c 2068 7474 7073 3a2f 2f64  ex-url https://d
 000134f0: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
 00013500: 6f72 672f 7768 6c2f 6375 3132 312f 0d0a  org/whl/cu121/..
 00013510: 0d0a 2020 2020 2320 4f72 2077 6974 6820  ..    # Or with 
 00013520: 666c 6178 0d0a 0d0a 2020 2020 7069 7033  flax....    pip3
 00013530: 2069 6e73 7461 6c6c 2064 6765 6e65 7261   install dgenera
-00013540: 7465 5b66 6c61 785d 3d3d 332e 342e 3220  te[flax]==3.4.2 
+00013540: 7465 5b66 6c61 785d 3d3d 332e 342e 3320  te[flax]==3.4.3 
 00013550: 2d2d 6578 7472 612d 696e 6465 782d 7572  --extra-index-ur
 00013560: 6c20 6874 7470 733a 2f2f 646f 776e 6c6f  l https://downlo
 00013570: 6164 2e70 7974 6f72 6368 2e6f 7267 2f77  ad.pytorch.org/w
 00013580: 686c 2f63 7531 3231 2f20 5c0d 0a20 2020  hl/cu121/ \..   
 00013590: 202d 6620 6874 7470 733a 2f2f 7374 6f72   -f https://stor
 000135a0: 6167 652e 676f 6f67 6c65 6170 6973 2e63  age.googleapis.c
 000135b0: 6f6d 2f6a 6178 2d72 656c 6561 7365 732f  om/jax-releases/
@@ -5496,22 +5496,22 @@
 00015770: 6272 6576 6974 792e 0d0a 0d0a 596f 7520  brevity.....You 
 00015780: 6361 6e20 646f 776e 6c6f 6164 2074 6865  can download the
 00015790: 6d20 6865 7265 3a0d 0a0d 0a20 2a20 606d  m here:.... * `m
 000157a0: 792d 696d 6167 652d 7365 6564 2e70 6e67  y-image-seed.png
 000157b0: 203c 6874 7470 733a 2f2f 7261 772e 6769   <https://raw.gi
 000157c0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
 000157d0: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-000157e0: 7261 7465 2f76 332e 342e 322f 6578 616d  rate/v3.4.2/exam
+000157e0: 7261 7465 2f76 332e 342e 332f 6578 616d  rate/v3.4.3/exam
 000157f0: 706c 6573 2f6d 6564 6961 2f64 6f67 2d6f  ples/media/dog-o
 00015800: 6e2d 6265 6e63 682e 706e 673e 605f 0d0a  n-bench.png>`_..
 00015810: 202a 2060 6d79 2d6d 6173 6b2d 696d 6167   * `my-mask-imag
 00015820: 652e 706e 6720 3c68 7474 7073 3a2f 2f72  e.png <https://r
 00015830: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
 00015840: 7465 6e74 2e63 6f6d 2f54 6572 696b 732f  tent.com/Teriks/
-00015850: 6467 656e 6572 6174 652f 7633 2e34 2e32  dgenerate/v3.4.2
+00015850: 6467 656e 6572 6174 652f 7633 2e34 2e33  dgenerate/v3.4.3
 00015860: 2f65 7861 6d70 6c65 732f 6d65 6469 612f  /examples/media/
 00015870: 646f 672d 6f6e 2d62 656e 6368 2d6d 6173  dog-on-bench-mas
 00015880: 6b2e 706e 673e 605f 0d0a 0d0a 5468 6520  k.png>`_....The 
 00015890: 636f 6d6d 616e 6420 6265 6c6f 7720 6765  command below ge
 000158a0: 6e65 7261 7465 7320 6120 6361 7420 7369  nerates a cat si
 000158b0: 7474 696e 6720 6f6e 2061 2062 656e 6368  tting on a bench
 000158c0: 2077 6974 6820 7468 6520 696d 6167 6573   with the images
@@ -8107,15 +8107,15 @@
 0001faa0: 6665 7265 6e63 6520 7374 6570 2e0d 0a0d  ference step....
 0001fab0: 0a0d 0a54 6865 7365 2065 7861 6d70 6c65  ...These example
 0001fac0: 7320 7573 653a 2060 7665 726d 6565 725f  s use: `vermeer_
 0001fad0: 6361 6e6e 795f 6564 6765 642e 706e 6720  canny_edged.png 
 0001fae0: 3c68 7474 7073 3a2f 2f72 6177 2e67 6974  <https://raw.git
 0001faf0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
 0001fb00: 6f6d 2f54 6572 696b 732f 6467 656e 6572  om/Teriks/dgener
-0001fb10: 6174 652f 7633 2e34 2e32 2f65 7861 6d70  ate/v3.4.2/examp
+0001fb10: 6174 652f 7633 2e34 2e33 2f65 7861 6d70  ate/v3.4.3/examp
 0001fb20: 6c65 732f 6d65 6469 612f 7665 726d 6565  les/media/vermee
 0001fb30: 725f 6361 6e6e 795f 6564 6765 642e 706e  r_canny_edged.pn
 0001fb40: 673e 605f 0d0a 0d0a 0d0a 2e2e 2063 6f64  g>`_........ cod
 0001fb50: 652d 626c 6f63 6b3a 3a20 6261 7368 0d0a  e-block:: bash..
 0001fb60: 0d0a 2020 2020 2320 546f 7263 6820 6578  ..    # Torch ex
 0001fb70: 616d 706c 652c 2075 7365 2022 7665 726d  ample, use "verm
 0001fb80: 6565 725f 6361 6e6e 795f 6564 6765 642e  eer_canny_edged.
@@ -8694,15 +8694,15 @@
 00021f50: 6765 6e65 7261 7469 6f6e 2077 6974 6820  generation with 
 00021f60: 6120 6d6f 6465 6c20 2b20 6120 436f 6e74  a model + a Cont
 00021f70: 726f 6c4e 6574 2e0d 0a0d 0a54 6869 7320  rolNet.....This 
 00021f80: 696d 6167 6520 6f66 2061 2060 686f 7273  image of a `hors
 00021f90: 6520 3c68 7474 7073 3a2f 2f72 6177 2e67  e <https://raw.g
 00021fa0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
 00021fb0: 2e63 6f6d 2f54 6572 696b 732f 6467 656e  .com/Teriks/dgen
-00021fc0: 6572 6174 652f 7633 2e34 2e32 2f65 7861  erate/v3.4.2/exa
+00021fc0: 6572 6174 652f 7633 2e34 2e33 2f65 7861  erate/v3.4.3/exa
 00021fd0: 6d70 6c65 732f 6d65 6469 612f 686f 7273  mples/media/hors
 00021fe0: 6532 2e6a 7065 673e 605f 0d0a 6973 2075  e2.jpeg>`_..is u
 00021ff0: 7365 6420 696e 2074 6865 2065 7861 6d70  sed in the examp
 00022000: 6c65 2062 656c 6f77 2077 6974 6820 6120  le below with a 
 00022010: 436f 6e74 726f 6c4e 6574 2074 6861 7420  ControlNet that 
 00022020: 6973 2074 7261 696e 6564 2074 6f20 6765  is trained to ge
 00022030: 6e65 7261 7465 2069 6d61 6765 7320 6672  nerate images fr
@@ -8934,15 +8934,15 @@
 00022e50: 6d61 6765 2075 7365 6420 696e 2074 6865  mage used in the
 00022e60: 2065 7861 6d70 6c65 2062 656c 6f77 2069   example below i
 00022e70: 7320 7468 6973 2060 6c6f 7720 7265 736f  s this `low reso
 00022e80: 6c75 7469 6f6e 2063 6174 203c 6874 7470  lution cat <http
 00022e90: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
 00022ea0: 6572 636f 6e74 656e 742e 636f 6d2f 5465  ercontent.com/Te
 00022eb0: 7269 6b73 2f64 6765 6e65 7261 7465 2f76  riks/dgenerate/v
-00022ec0: 332e 342e 322f 6578 616d 706c 6573 2f6d  3.4.2/examples/m
+00022ec0: 332e 342e 332f 6578 616d 706c 6573 2f6d  3.4.3/examples/m
 00022ed0: 6564 6961 2f6c 6f77 5f72 6573 5f63 6174  edia/low_res_cat
 00022ee0: 2e70 6e67 3e60 5f0d 0a0d 0a2e 2e20 636f  .png>`_...... co
 00022ef0: 6465 2d62 6c6f 636b 3a3a 2062 6173 680d  de-block:: bash.
 00022f00: 0a0d 0a20 2020 2023 2054 6865 2069 6d61  ...    # The ima
 00022f10: 6765 2070 726f 6475 6365 6420 7769 7468  ge produced with
 00022f20: 2074 6869 7320 6d6f 6465 6c20 7769 6c6c   this model will
 00022f30: 2062 650d 0a20 2020 2023 2074 776f 2074   be..    # two t
@@ -9934,15 +9934,15 @@
 00026cd0: 6e67 2069 7320 6120 636f 6e66 6967 2066  ng is a config f
 00026ce0: 696c 6520 6578 616d 706c 6520 7468 6174  ile example that
 00026cf0: 2063 6f76 6572 7320 7665 7279 2062 6173   covers very bas
 00026d00: 6963 2073 796e 7461 7820 636f 6e63 6570  ic syntax concep
 00026d10: 7473 3a0d 0a0d 0a2e 2e20 636f 6465 2d62  ts:...... code-b
 00026d20: 6c6f 636b 3a3a 206a 696e 6a61 0d0a 0d0a  lock:: jinja....
 00026d30: 2020 2020 2321 2064 6765 6e65 7261 7465      #! dgenerate
-00026d40: 2033 2e34 2e32 0d0a 0d0a 2020 2020 2320   3.4.2....    # 
+00026d40: 2033 2e34 2e33 0d0a 0d0a 2020 2020 2320   3.4.3....    # 
 00026d50: 4966 2061 2068 6173 682d 6261 6e67 2076  If a hash-bang v
 00026d60: 6572 7369 6f6e 2069 7320 7072 6f76 6964  ersion is provid
 00026d70: 6564 2069 6e20 7468 6520 666f 726d 6174  ed in the format
 00026d80: 2061 626f 7665 0d0a 2020 2020 2320 6120   above..    # a 
 00026d90: 7761 726e 696e 6720 7769 6c6c 2062 6520  warning will be 
 00026da0: 7072 6f64 7563 6564 2069 6620 7468 6520  produced if the 
 00026db0: 7665 7273 696f 6e20 796f 7520 6172 6520  version you are 
@@ -10201,15 +10201,15 @@
 00027d80: 2073 6574 2077 6974 6820 7468 6520 6060   set with the ``
 00027d90: 5c73 6574 6060 2064 6972 6563 7469 7665  \set`` directive
 00027da0: 2077 696c 6c20 616c 736f 2062 6520 6d65   will also be me
 00027db0: 6e74 696f 6e65 6420 696e 2074 6869 7320  ntioned in this 
 00027dc0: 6f75 7470 7574 2e0d 0a0d 0a2e 2e20 636f  output....... co
 00027dd0: 6465 2d62 6c6f 636b 3a3a 206a 696e 6a61  de-block:: jinja
 00027de0: 0d0a 0d0a 2020 2020 2321 2064 6765 6e65  ....    #! dgene
-00027df0: 7261 7465 2033 2e34 2e32 0d0a 0d0a 2020  rate 3.4.2....  
+00027df0: 7261 7465 2033 2e34 2e33 0d0a 0d0a 2020  rate 3.4.3....  
 00027e00: 2020 2320 496e 766f 6361 7469 6f6e 2077    # Invocation w
 00027e10: 696c 6c20 7072 6f63 6565 6420 6173 206e  ill proceed as n
 00027e20: 6f72 6d61 6c0d 0a0d 0a20 2020 2073 7461  ormal....    sta
 00027e30: 6269 6c69 7479 6169 2f73 7461 626c 652d  bilityai/stable-
 00027e40: 6469 6666 7573 696f 6e2d 322d 3120 2d2d  diffusion-2-1 --
 00027e50: 7072 6f6d 7074 7320 2261 206d 616e 2077  prompts "a man w
 00027e60: 616c 6b69 6e67 206f 6e20 7468 6520 6d6f  alking on the mo
@@ -10987,15 +10987,15 @@
 0002aea0: 7461 7469 6f6e 2066 6f72 2074 6865 2073  tation for the s
 0002aeb0: 7065 6369 6669 6564 2064 6972 6563 7469  pecified directi
 0002aec0: 7665 732e 2054 6865 2062 6163 6b73 6c61  ves. The backsla
 0002aed0: 7368 206d 6179 2062 6520 6f6d 6974 7465  sh may be omitte
 0002aee0: 642e 0d0a 0d0a 0d0a 2e2e 2063 6f64 652d  d......... code-
 0002aef0: 626c 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d  block:: jinja...
 0002af00: 0a20 2020 2023 2120 6467 656e 6572 6174  .    #! dgenerat
-0002af10: 6520 332e 342e 320d 0a0d 0a20 2020 2023  e 3.4.2....    #
+0002af10: 6520 332e 342e 330d 0a0d 0a20 2020 2023  e 3.4.3....    #
 0002af20: 2059 6f75 2063 616e 2064 6566 696e 6520   You can define 
 0002af30: 796f 7572 206f 776e 2074 656d 706c 6174  your own templat
 0002af40: 6520 7661 7269 6162 6c65 7320 7769 7468  e variables with
 0002af50: 2074 6865 205c 7365 7420 6469 7265 6374   the \set direct
 0002af60: 6976 650d 0a20 2020 2023 2074 6865 205c  ive..    # the \
 0002af70: 7365 7420 6469 7265 6374 6976 6520 646f  set directive do
 0002af80: 6573 206e 6f74 2064 6f20 616e 7920 7368  es not do any sh
@@ -11440,15 +11440,15 @@
 0002caf0: 6361 6e20 676c 6f62 2064 6972 6563 746f  can glob directo
 0002cb00: 7269 6573 2075 7369 6e67 2066 756e 6374  ries using funct
 0002cb10: 696f 6e73 2066 726f 6d20 7468 6520 676c  ions from the gl
 0002cb20: 6f62 206d 6f64 756c 6520 6c69 6b65 2073  ob module like s
 0002cb30: 6f3a 0d0a 0d0a 2e2e 2063 6f64 652d 626c  o:...... code-bl
 0002cb40: 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d 0a20  ock:: jinja.... 
 0002cb50: 2020 2023 2120 6467 656e 6572 6174 6520     #! dgenerate 
-0002cb60: 332e 342e 320d 0a0d 0a20 2020 2023 2054  3.4.2....    # T
+0002cb60: 332e 342e 330d 0a0d 0a20 2020 2023 2054  3.4.3....    # T
 0002cb70: 6865 206d 6f73 7420 6261 7369 6320 7573  he most basic us
 0002cb80: 6167 6520 6973 2066 756c 6c20 6578 7061  age is full expa
 0002cb90: 6e73 696f 6e20 6f66 2065 7665 7279 2066  nsion of every f
 0002cba0: 696c 650d 0a0d 0a20 2020 205c 7365 7420  ile....    \set 
 0002cbb0: 6d79 6669 6c65 7320 7b7b 2071 756f 7465  myfiles {{ quote
 0002cbc0: 2867 6c6f 622e 676c 6f62 2827 6d79 5f69  (glob.glob('my_i
 0002cbd0: 6d61 6765 732f 2a2e 706e 6727 2929 207d  mages/*.png')) }
@@ -11484,15 +11484,15 @@
 0002cdb0: 6e65 7261 7465 2073 7562 2d63 6f6d 6d61  nerate sub-comma
 0002cdc0: 6e64 2060 6069 6d61 6765 2d70 726f 6365  nd ``image-proce
 0002cdd0: 7373 6060 2068 6173 2061 2063 6f6e 6669  ss`` has a confi
 0002cde0: 6720 6469 7265 6374 6976 6520 696d 706c  g directive impl
 0002cdf0: 656d 656e 7461 7469 6f6e 2e0d 0a0d 0a0d  ementation......
 0002ce00: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
 0002ce10: 206a 696e 6a61 0d0a 0d0a 2020 2020 2321   jinja....    #!
-0002ce20: 2064 6765 6e65 7261 7465 2033 2e34 2e32   dgenerate 3.4.2
+0002ce20: 2064 6765 6e65 7261 7465 2033 2e34 2e33   dgenerate 3.4.3
 0002ce30: 0d0a 0d0a 2020 2020 2320 7072 696e 7420  ....    # print 
 0002ce40: 7468 6520 6865 6c70 206d 6573 7361 6765  the help message
 0002ce50: 206f 6620 2d2d 7375 622d 636f 6d6d 616e   of --sub-comman
 0002ce60: 6420 696d 6167 652d 7072 6f63 6573 732c  d image-process,
 0002ce70: 2074 6869 7320 646f 6573 0d0a 2020 2020   this does..    
 0002ce80: 2320 6e6f 7420 6361 7573 6520 7468 6520  # not cause the 
 0002ce90: 636f 6e66 6967 2074 6f20 6578 6974 0d0a  config to exit..
@@ -11545,15 +11545,15 @@
 0002d180: 616e 2065 7869 7420 6120 636f 6e66 6967  an exit a config
 0002d190: 2065 6172 6c79 2069 6620 6e65 6564 2062   early if need b
 0002d1a0: 6520 7573 696e 6720 7468 6520 6060 5c65  e using the ``\e
 0002d1b0: 7869 7460 6020 6469 7265 6374 6976 650d  xit`` directive.
 0002d1c0: 0a0d 0a0d 0a2e 2e20 636f 6465 2d62 6c6f  ....... code-blo
 0002d1d0: 636b 3a3a 206a 696e 6a61 0d0a 0d0a 2020  ck:: jinja....  
 0002d1e0: 2020 2321 2064 6765 6e65 7261 7465 2033    #! dgenerate 3
-0002d1f0: 2e34 2e32 0d0a 0d0a 2020 2020 2320 6578  .4.2....    # ex
+0002d1f0: 2e34 2e33 0d0a 0d0a 2020 2020 2320 6578  .4.3....    # ex
 0002d200: 6974 2074 6865 2070 726f 6365 7373 2077  it the process w
 0002d210: 6974 6820 7265 7475 726e 2063 6f64 6520  ith return code 
 0002d220: 312c 2077 6869 6368 2069 6e64 6963 6174  1, which indicat
 0002d230: 6573 2061 6e20 6572 726f 720d 0a0d 0a20  es an error.... 
 0002d240: 2020 205c 7072 696e 7420 2273 6f6d 6520     \print "some 
 0002d250: 6572 726f 7220 6f63 6375 7272 6564 220d  error occurred".
 0002d260: 0a20 2020 205c 6578 6974 2031 0d0a 0d0a  .    \exit 1....
@@ -11703,41 +11703,41 @@
 0002db60: 6365 7373 6f72 2070 6c75 6769 6e73 2063  cessor plugins c
 0002db70: 616e 2062 6520 666f 756e 640d 0a69 6e20  an be found..in 
 0002db80: 7468 6520 6022 7772 6974 696e 675f 706c  the `"writing_pl
 0002db90: 7567 696e 732f 696d 6167 655f 7072 6f63  ugins/image_proc
 0002dba0: 6573 736f 7222 203c 6874 7470 733a 2f2f  essor" <https://
 0002dbb0: 6769 7468 7562 2e63 6f6d 2f54 6572 696b  github.com/Terik
 0002dbc0: 732f 6467 656e 6572 6174 652f 7472 6565  s/dgenerate/tree
-0002dbd0: 2f76 332e 342e 322f 6578 616d 706c 6573  /v3.4.2/examples
+0002dbd0: 2f76 332e 342e 332f 6578 616d 706c 6573  /v3.4.3/examples
 0002dbe0: 2f77 7269 7469 6e67 5f70 6c75 6769 6e73  /writing_plugins
 0002dbf0: 2f69 6d61 6765 5f70 726f 6365 7373 6f72  /image_processor
 0002dc00: 3e60 5f0d 0a66 6f6c 6465 7220 6f66 2074  >`_..folder of t
 0002dc10: 6865 2065 7861 6d70 6c65 7320 666f 6c64  he examples fold
 0002dc20: 6572 2e0d 0a0d 0a54 6865 2073 6f75 7263  er.....The sourc
 0002dc30: 6520 636f 6465 2066 6f72 2074 6865 2062  e code for the b
 0002dc40: 7569 6c74 2069 6e20 6063 616e 6e79 203c  uilt in `canny <
 0002dc50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 0002dc60: 6f6d 2f54 6572 696b 732f 6467 656e 6572  om/Teriks/dgener
-0002dc70: 6174 652f 626c 6f62 2f76 332e 342e 322f  ate/blob/v3.4.2/
+0002dc70: 6174 652f 626c 6f62 2f76 332e 342e 332f  ate/blob/v3.4.3/
 0002dc80: 6467 656e 6572 6174 652f 696d 6167 6570  dgenerate/imagep
 0002dc90: 726f 6365 7373 6f72 732f 6361 6e6e 792e  rocessors/canny.
 0002dca0: 7079 3e60 5f20 7072 6f63 6573 736f 722c  py>`_ processor,
 0002dcb0: 0d0a 7468 6520 606f 7065 6e70 6f73 6520  ..the `openpose 
 0002dcc0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
 0002dcd0: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-0002dce0: 7261 7465 2f62 6c6f 622f 7633 2e34 2e32  rate/blob/v3.4.2
+0002dce0: 7261 7465 2f62 6c6f 622f 7633 2e34 2e33  rate/blob/v3.4.3
 0002dcf0: 2f64 6765 6e65 7261 7465 2f69 6d61 6765  /dgenerate/image
 0002dd00: 7072 6f63 6573 736f 7273 2f6f 7065 6e70  processors/openp
 0002dd10: 6f73 652e 7079 3e60 5f20 7072 6f63 6573  ose.py>`_ proces
 0002dd20: 736f 722c 2061 6e64 2074 6865 2073 696d  sor, and the sim
 0002dd30: 706c 650d 0a60 7069 6c6c 6f77 2069 6d61  ple..`pillow ima
 0002dd40: 6765 206f 7065 7261 7469 6f6e 7320 3c68  ge operations <h
 0002dd50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 0002dd60: 6d2f 5465 7269 6b73 2f64 6765 6e65 7261  m/Teriks/dgenera
-0002dd70: 7465 2f62 6c6f 622f 7633 2e34 2e32 2f64  te/blob/v3.4.2/d
+0002dd70: 7465 2f62 6c6f 622f 7633 2e34 2e33 2f64  te/blob/v3.4.3/d
 0002dd80: 6765 6e65 7261 7465 2f69 6d61 6765 7072  generate/imagepr
 0002dd90: 6f63 6573 736f 7273 2f69 6d61 6765 6f70  ocessors/imageop
 0002dda0: 732e 7079 3e60 5f20 7072 6f63 6573 736f  s.py>`_ processo
 0002ddb0: 7273 2063 616e 2061 6c73 6f0d 0a62 6520  rs can also..be 
 0002ddc0: 6f66 2072 6566 6572 656e 6365 2061 7320  of reference as 
 0002ddd0: 7468 6579 2061 7265 2077 7269 7474 656e  they are written
 0002dde0: 2061 7320 696e 7465 726e 616c 2069 6d61   as internal ima
@@ -11747,15 +11747,15 @@
 0002de20: 636f 6e66 6967 2064 6972 6563 7469 7665  config directive
 0002de30: 7320 6361 6e20 6265 2066 6f75 6e64 2069  s can be found i
 0002de40: 6e20 7468 650d 0a60 2277 7269 7469 6e67  n the..`"writing
 0002de50: 5f70 6c75 6769 6e73 2f63 6f6e 6669 675f  _plugins/config_
 0002de60: 6469 7265 6374 6976 6522 203c 6874 7470  directive" <http
 0002de70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
 0002de80: 6572 696b 732f 6467 656e 6572 6174 652f  eriks/dgenerate/
-0002de90: 7472 6565 2f76 332e 342e 322f 6578 616d  tree/v3.4.2/exam
+0002de90: 7472 6565 2f76 332e 342e 332f 6578 616d  tree/v3.4.3/exam
 0002dea0: 706c 6573 2f77 7269 7469 6e67 5f70 6c75  ples/writing_plu
 0002deb0: 6769 6e73 2f63 6f6e 6669 675f 6469 7265  gins/config_dire
 0002dec0: 6374 6976 653e 605f 2066 6f6c 6465 720d  ctive>`_ folder.
 0002ded0: 0a6f 6620 7468 6520 6578 616d 706c 6573  .of the examples
 0002dee0: 2066 6f6c 6465 722e 0d0a 0d0a 4375 7272   folder.....Curr
 0002def0: 656e 746c 7920 7468 6520 6f6e 6c79 2069  ently the only i
 0002df00: 6e74 6572 6e61 6c20 6469 7265 6374 6976  nternal directiv
@@ -11764,15 +11764,15 @@
 0002df30: 6e20 6973 2074 6865 2060 605c 696d 6167  n is the ``\imag
 0002df40: 655f 7072 6f63 6573 7360 6020 6469 7265  e_process`` dire
 0002df50: 6374 6976 652c 0d0a 7768 6f27 7320 736f  ctive,..who's so
 0002df60: 7572 6365 2066 696c 6520 6063 616e 2062  urce file `can b
 0002df70: 6520 6c6f 6361 7465 6420 6865 7265 203c  e located here <
 0002df80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 0002df90: 6f6d 2f54 6572 696b 732f 6467 656e 6572  om/Teriks/dgener
-0002dfa0: 6174 652f 626c 6f62 2f76 332e 342e 322f  ate/blob/v3.4.2/
+0002dfa0: 6174 652f 626c 6f62 2f76 332e 342e 332f  ate/blob/v3.4.3/
 0002dfb0: 6467 656e 6572 6174 652f 6261 7463 6870  dgenerate/batchp
 0002dfc0: 726f 6365 7373 2f69 6d61 6765 5f70 726f  rocess/image_pro
 0002dfd0: 6365 7373 5f64 6972 6563 7469 7665 2e70  cess_directive.p
 0002dfe0: 793e 605f 2c0d 0a74 6865 2073 6f75 7263  y>`_,..the sourc
 0002dff0: 6520 6669 6c65 2066 6f72 2074 6869 7320  e file for this 
 0002e000: 6469 7265 6374 6976 6520 6973 2074 6572  directive is ter
 0002e010: 7365 2061 7320 6d6f 7374 206f 6620 6060  se as most of ``
@@ -11786,15 +11786,15 @@
 0002e090: 2069 7320 616c 736f 2075 7365 6420 666f   is also used fo
 0002e0a0: 7220 6060 2d2d 7375 622d 636f 6d6d 616e  r ``--sub-comman
 0002e0b0: 6420 696d 6167 652d 7072 6f63 6573 7360  d image-process`
 0002e0c0: 6020 6973 0d0a 6069 7320 696d 706c 656d  ` is..`is implem
 0002e0d0: 656e 7465 6420 6865 7265 203c 6874 7470  ented here <http
 0002e0e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
 0002e0f0: 6572 696b 732f 6467 656e 6572 6174 652f  eriks/dgenerate/
-0002e100: 626c 6f62 2f76 332e 342e 322f 6467 656e  blob/v3.4.2/dgen
+0002e100: 626c 6f62 2f76 332e 342e 332f 6467 656e  blob/v3.4.3/dgen
 0002e110: 6572 6174 652f 696d 6167 655f 7072 6f63  erate/image_proc
 0002e120: 6573 733e 605f 2e0d 0a0d 0a46 696c 6520  ess>`_.....File 
 0002e130: 4361 6368 6520 436f 6e74 726f 6c0d 0a3d  Cache Control..=
 0002e140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0002e150: 3d0d 0a0d 0a64 6765 6e65 7261 7465 2077  =....dgenerate w
 0002e160: 696c 6c20 6361 6368 6520 6060 2d2d 696d  ill cache ``--im
 0002e170: 6167 652d 7365 6564 7360 6020 6669 6c65  age-seeds`` file
```

### Comparing `dgenerate-3.4.2/dgenerate/__init__.py` & `dgenerate-3.4.3/dgenerate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 # LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
 # HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 # LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '3.4.2'
+__version__ = '3.4.3'
 
 import collections.abc
 import sys
 import typing
 import warnings
 
 warnings.filterwarnings('ignore', module='dgenerate.extras.controlnet_aux')
```

### Comparing `dgenerate-3.4.2/dgenerate/arguments.py` & `dgenerate-3.4.3/dgenerate/arguments.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/batchprocess/__init__.py` & `dgenerate-3.4.3/dgenerate/batchprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/batchprocess/batchprocessor.py` & `dgenerate-3.4.3/dgenerate/batchprocess/batchprocessor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/batchprocess/configrunner.py` & `dgenerate-3.4.3/dgenerate/batchprocess/configrunner.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/batchprocess/configrunnerplugin.py` & `dgenerate-3.4.3/dgenerate/batchprocess/configrunnerplugin.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/batchprocess/configrunnerpluginloader.py` & `dgenerate-3.4.3/dgenerate/batchprocess/configrunnerpluginloader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/batchprocess/image_process_directive.py` & `dgenerate-3.4.3/dgenerate/batchprocess/image_process_directive.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/dgenerate.py` & `dgenerate-3.4.3/dgenerate/dgenerate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/events.py` & `dgenerate-3.4.3/dgenerate/events.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/canny/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/canny/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/dwpose_config/dwpose-l_384x288.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/util.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/wholebody.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/wholebody.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/dwpose/yolox_config/yolox_l_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/hed/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/lineart/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/lineart/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/lineart_anime/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mediapipe_face/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mediapipe_face/mediapipe_face_common.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/api.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/blocks.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/transforms.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/midas/vit.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/midas/utils.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/mlsd/utils.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/body.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/body.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/face.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/face.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/hand.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/hand.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/model.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/open_pose/util.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/open_pose/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/pidi/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/pidi/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/pidi/model.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/pidi/model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/processor.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/processor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/predictor.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/shuffle/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/tests/test_processor.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/tests/test_processor_pytest.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/util.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/builder.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/depth_model.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/attractor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/model_io.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/config.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py` & `dgenerate-3.4.3/dgenerate/extras/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/filelock.py` & `dgenerate-3.4.3/dgenerate/filelock.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/image.py` & `dgenerate-3.4.3/dgenerate/image.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/image_process/__init__.py` & `dgenerate-3.4.3/dgenerate/image_process/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/image_process/arguments.py` & `dgenerate-3.4.3/dgenerate/image_process/arguments.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/image_process/invoker.py` & `dgenerate-3.4.3/dgenerate/image_process/invoker.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/image_process/renderloop.py` & `dgenerate-3.4.3/dgenerate/image_process/renderloop.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/image_process/renderloopconfig.py` & `dgenerate-3.4.3/dgenerate/image_process/renderloopconfig.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/__init__.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/canny.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/canny.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/exceptions.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/exceptions.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/hed.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/hed.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/imageops.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/imageops.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessor.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessor.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessorchain.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessorchain.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessorloader.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessorloader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/imageprocessormixin.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/imageprocessormixin.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/leres.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/leres.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/linart_anime.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/linart_anime.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/lineart.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/lineart.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/midas.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/midas.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/mlsd.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/mlsd.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/normal_bae.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/normal_bae.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/openpose.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/openpose.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/pidi.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/pidi.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/sam.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/sam.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/imageprocessors/upscaler.py` & `dgenerate-3.4.3/dgenerate/imageprocessors/upscaler.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/invoker.py` & `dgenerate-3.4.3/dgenerate/invoker.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/mediainput.py` & `dgenerate-3.4.3/dgenerate/mediainput.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/mediaoutput.py` & `dgenerate-3.4.3/dgenerate/mediaoutput.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/memoize.py` & `dgenerate-3.4.3/dgenerate/memoize.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/memory.py` & `dgenerate-3.4.3/dgenerate/memory.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/messages.py` & `dgenerate-3.4.3/dgenerate/messages.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/__init__.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/cache.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/cache.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/constants.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/constants.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/enums.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/enums.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/hfutil.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/hfutil.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/pipelines.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/pipelines.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/uris.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/uris.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/util.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/util.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/pipelinewrapper/wrapper.py` & `dgenerate-3.4.3/dgenerate/pipelinewrapper/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1674,14 +1674,16 @@
         pipeline_args.pop('negative_crops_coords_top_left', None)
 
     def _call_torch_s_cascade(self, pipeline_args, user_args: DiffusionArguments):
         prompt: _prompt.Prompt() = _types.default(user_args.prompt, _prompt.Prompt())
         pipeline_args['prompt'] = prompt.positive if prompt.positive else ''
         pipeline_args['negative_prompt'] = prompt.negative
 
+        pipeline_args['num_images_per_prompt'] = _types.default(user_args.batch_size, 1)
+
         pipeline_args['generator'] = \
             torch.Generator(device=self._device).manual_seed(
                 _types.default(user_args.seed, _constants.DEFAULT_SEED))
 
         prior = _pipelines.call_pipeline(
             pipeline=self._pipeline,
             device=self._device,
@@ -1700,20 +1702,25 @@
             image_embeddings = prior.image_embeddings
 
         if user_args.s_cascade_decoder_prompt:
             prompt: _prompt.Prompt() = user_args.s_cascade_decoder_prompt
             pipeline_args['prompt'] = prompt.positive if prompt.positive else ''
             pipeline_args['negative_prompt'] = prompt.negative
 
-        return PipelineWrapperResult(
-            _pipelines.call_pipeline(
-                image_embeddings=image_embeddings,
+        pipeline_args['num_images_per_prompt'] = 1
+
+        output_images = []
+        for embedding in image_embeddings:
+            output_images += _pipelines.call_pipeline(
+                image_embeddings=embedding.unsqueeze(0),
                 pipeline=self._s_cascade_decoder_pipeline,
                 device=self._device,
-                **pipeline_args).images)
+                **pipeline_args).images
+
+        return PipelineWrapperResult(output_images)
 
     def _call_torch(self, pipeline_args, user_args: DiffusionArguments):
         prompt: _prompt.Prompt() = _types.default(user_args.prompt, _prompt.Prompt())
         pipeline_args['prompt'] = prompt.positive if prompt.positive else ''
         pipeline_args['negative_prompt'] = prompt.negative
 
         self._get_sdxl_conditioning_args(self._pipeline, pipeline_args, user_args)
```

### Comparing `dgenerate-3.4.2/dgenerate/plugin.py` & `dgenerate-3.4.3/dgenerate/plugin.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/prompt.py` & `dgenerate-3.4.3/dgenerate/prompt.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/renderloop.py` & `dgenerate-3.4.3/dgenerate/renderloop.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/renderloopconfig.py` & `dgenerate-3.4.3/dgenerate/renderloopconfig.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/subcommands/__init__.py` & `dgenerate-3.4.3/dgenerate/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/subcommands/exceptions.py` & `dgenerate-3.4.3/dgenerate/subcommands/exceptions.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/subcommands/image_process.py` & `dgenerate-3.4.3/dgenerate/subcommands/image_process.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/subcommands/subcommand.py` & `dgenerate-3.4.3/dgenerate/subcommands/subcommand.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/subcommands/subcommandloader.py` & `dgenerate-3.4.3/dgenerate/subcommands/subcommandloader.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/textprocessing.py` & `dgenerate-3.4.3/dgenerate/textprocessing.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate/types.py` & `dgenerate-3.4.3/dgenerate/types.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate.egg-info/PKG-INFO` & `dgenerate-3.4.3/dgenerate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2064 6765  : 2.1..Name: dge
 00000020: 6e65 7261 7465 0d0a 5665 7273 696f 6e3a  nerate..Version:
-00000030: 2033 2e34 2e32 0d0a 5375 6d6d 6172 793a   3.4.2..Summary:
+00000030: 2033 2e34 2e33 0d0a 5375 6d6d 6172 793a   3.4.3..Summary:
 00000040: 2042 6174 6368 2069 6d61 6765 2067 656e   Batch image gen
 00000050: 6572 6174 696f 6e20 616e 6420 6d61 6e69  eration and mani
 00000060: 7075 6c61 7469 6f6e 2074 6f6f 6c20 7375  pulation tool su
 00000070: 7070 6f72 7469 6e67 2053 7461 626c 6520  pporting Stable 
 00000080: 4469 6666 7573 696f 6e20 616e 6420 7265  Diffusion and re
 00000090: 6c61 7465 6420 7465 6368 6e69 7175 6573  lated techniques
 000000a0: 202f 2061 6c67 6f72 6974 686d 732c 2077   / algorithms, w
@@ -249,18 +249,18 @@
 00000f80: 203d 3d20 2272 6561 6474 6865 646f 6373   == "readthedocs
 00000f90: 220d 0a0d 0a2e 2e20 7c44 6f63 756d 656e  "...... |Documen
 00000fa0: 7461 7469 6f6e 2053 7461 7475 737c 2069  tation Status| i
 00000fb0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f72  mage:: https://r
 00000fc0: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
 00000fd0: 726f 6a65 6374 732f 6467 656e 6572 6174  rojects/dgenerat
 00000fe0: 652f 6261 6467 652f 3f76 6572 7369 6f6e  e/badge/?version
-00000ff0: 3d76 332e 342e 320d 0a20 2020 3a74 6172  =v3.4.2..   :tar
+00000ff0: 3d76 332e 342e 330d 0a20 2020 3a74 6172  =v3.4.3..   :tar
 00001000: 6765 743a 2068 7474 703a 2f2f 6467 656e  get: http://dgen
 00001010: 6572 6174 652e 7265 6164 7468 6564 6f63  erate.readthedoc
-00001020: 732e 696f 2f65 6e2f 7633 2e34 2e32 2f0d  s.io/en/v3.4.2/.
+00001020: 732e 696f 2f65 6e2f 7633 2e34 2e33 2f0d  s.io/en/v3.4.3/.
 00001030: 0a0d 0a4f 7665 7276 6965 770d 0a3d 3d3d  ...Overview..===
 00001040: 3d3d 3d3d 3d0d 0a0d 0a7c 446f 6375 6d65  =====....|Docume
 00001050: 6e74 6174 696f 6e20 5374 6174 7573 7c0d  ntation Status|.
 00001060: 0a0d 0a2a 2a64 6765 6e65 7261 7465 2a2a  ...**dgenerate**
 00001070: 2069 7320 6120 636f 6d6d 616e 6420 6c69   is a command li
 00001080: 6e65 2074 6f6f 6c20 616e 6420 6c69 6272  ne tool and libr
 00001090: 6172 7920 666f 7220 6765 6e65 7261 7469  ary for generati
@@ -379,15 +379,15 @@
 000017a0: 2062 7574 2065 7874 7261 6f72 6469 6e61   but extraordina
 000017b0: 7269 6c79 2073 6c6f 772e 0d0a 0d0a 466f  rily slow.....Fo
 000017c0: 7220 6c69 6272 6172 7920 646f 6375 6d65  r library docume
 000017d0: 6e74 6174 696f 6e20 7669 7369 7420 6072  ntation visit `r
 000017e0: 6561 6474 6865 646f 6373 203c 6874 7470  eadthedocs <http
 000017f0: 3a2f 2f64 6765 6e65 7261 7465 2e72 6561  ://dgenerate.rea
 00001800: 6474 6865 646f 6373 2e69 6f2f 656e 2f76  dthedocs.io/en/v
-00001810: 332e 342e 322f 3e60 5f2e 0d0a 0d0a 2d2d  3.4.2/>`_.....--
+00001810: 332e 342e 332f 3e60 5f2e 0d0a 0d0a 2d2d  3.4.3/>`_.....--
 00001820: 2d2d 0d0a 0d0a 2a20 486f 7720 746f 2069  --....* How to i
 00001830: 6e73 7461 6c6c 0d0a 2020 2020 2a20 6057  nstall..    * `W
 00001840: 696e 646f 7773 2049 6e73 7461 6c6c 605f  indows Install`_
 00001850: 0d0a 2020 2020 2a20 604c 696e 7578 206f  ..    * `Linux o
 00001860: 7220 5753 4c20 496e 7374 616c 6c60 5f0d  r WSL Install`_.
 00001870: 0a0d 0a2a 2055 7361 6765 2045 7861 6d70  ...* Usage Examp
 00001880: 6c65 730d 0a20 2020 202a 2060 4261 7369  les..    * `Basi
@@ -4662,15 +4662,15 @@
 00012350: 6661 756c 7420 7661 6c75 653a 2022 7573  fault value: "us
 00012360: 6564 5f70 6572 6365 6e74 203e 2037 3022  ed_percent > 70"
 00012370: 2046 6f72 0d0a 2020 2020 2020 2020 2020   For..          
 00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012390: 2020 5379 6e74 6178 2053 6565 3a20 5b68    Syntax See: [h
 000123a0: 7474 7073 3a2f 2f64 6765 6e65 7261 7465  ttps://dgenerate
 000123b0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000123c0: 656e 2f76 332e 342e 322f 6467 656e 6572  en/v3.4.2/dgener
+000123c0: 656e 2f76 332e 342e 332f 6467 656e 6572  en/v3.4.3/dgener
 000123d0: 6174 655f 7375 626d 6f64 756c 6573 2e68  ate_submodules.h
 000123e0: 746d 0d0a 2020 2020 2020 2020 2020 2020  tm..            
 000123f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012400: 6c23 6467 656e 6572 6174 652e 7069 7065  l#dgenerate.pipe
 00012410: 6c69 6e65 7772 6170 7065 722e 4341 4348  linewrapper.CACH
 00012420: 455f 4d45 4d4f 5259 5f43 4f4e 5354 5241  E_MEMORY_CONSTRA
 00012430: 494e 5453 5d0d 0a20 2020 2020 202d 706d  INTS]..      -pm
@@ -4713,15 +4713,15 @@
 00012680: 655f 7369 7a65 203e 2028 6176 6169 6c61  e_size > (availa
 00012690: 626c 6520 2a0d 0a20 2020 2020 2020 2020  ble *..         
 000126a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000126b0: 2020 2030 2e37 3529 2220 466f 7220 5379     0.75)" For Sy
 000126c0: 6e74 6178 2053 6565 3a20 5b68 7474 7073  ntax See: [https
 000126d0: 3a2f 2f64 6765 6e65 7261 7465 2e72 6561  ://dgenerate.rea
 000126e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f76  dthedocs.io/en/v
-000126f0: 332e 342e 322f 6467 656e 6572 6174 655f  3.4.2/dgenerate_
+000126f0: 332e 342e 332f 6467 656e 6572 6174 655f  3.4.3/dgenerate_
 00012700: 7375 620d 0a20 2020 2020 2020 2020 2020  sub..           
 00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012720: 206d 6f64 756c 6573 2e68 746d 6c23 6467   modules.html#dg
 00012730: 656e 6572 6174 652e 7069 7065 6c69 6e65  enerate.pipeline
 00012740: 7772 6170 7065 722e 5049 5045 4c49 4e45  wrapper.PIPELINE
 00012750: 5f43 4143 4845 5f4d 454d 4f52 595f 434f  _CACHE_MEMORY_CO
 00012760: 4e53 5452 4149 4e54 535d 0d0a 2020 2020  NSTRAINTS]..    
@@ -4762,15 +4762,15 @@
 00012990: 653a 2022 756e 6574 5f73 697a 6520 3e20  e: "unet_size > 
 000129a0: 2861 7661 696c 6162 6c65 202a 2030 2e37  (available * 0.7
 000129b0: 3529 2220 466f 7220 5379 6e74 6178 2053  5)" For Syntax S
 000129c0: 6565 3a20 5b68 7474 7073 3a2f 2f64 6765  ee: [https://dge
 000129d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000129e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
 000129f0: 7261 7465 2e72 6561 6474 6865 646f 6373  rate.readthedocs
-00012a00: 2e69 6f2f 656e 2f76 332e 342e 322f 6467  .io/en/v3.4.2/dg
+00012a00: 2e69 6f2f 656e 2f76 332e 342e 332f 6467  .io/en/v3.4.3/dg
 00012a10: 656e 6572 6174 655f 7375 626d 6f64 756c  enerate_submodul
 00012a20: 6573 2e68 746d 6c23 6467 656e 6572 6174  es.html#dgenerat
 00012a30: 652e 7069 7065 6c69 6e65 7772 6170 0d0a  e.pipelinewrap..
 00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012a50: 2020 2020 2020 2020 2020 2020 7065 722e              per.
 00012a60: 554e 4554 5f43 4143 4845 5f4d 454d 4f52  UNET_CACHE_MEMOR
 00012a70: 595f 434f 4e53 5452 4149 4e54 535d 0d0a  Y_CONSTRAINTS]..
@@ -4811,15 +4811,15 @@
 00012ca0: 653a 2022 7661 655f 7369 7a65 203e 2028  e: "vae_size > (
 00012cb0: 6176 6169 6c61 626c 6520 2a20 302e 3735  available * 0.75
 00012cc0: 2922 2046 6f72 2053 796e 7461 7820 5365  )" For Syntax Se
 00012cd0: 653a 205b 6874 7470 733a 2f2f 6467 656e  e: [https://dgen
 00012ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00012cf0: 2020 2020 2020 2020 2020 2020 2020 6572                er
 00012d00: 6174 652e 7265 6164 7468 6564 6f63 732e  ate.readthedocs.
-00012d10: 696f 2f65 6e2f 7633 2e34 2e32 2f64 6765  io/en/v3.4.2/dge
+00012d10: 696f 2f65 6e2f 7633 2e34 2e33 2f64 6765  io/en/v3.4.3/dge
 00012d20: 6e65 7261 7465 5f73 7562 6d6f 6475 6c65  nerate_submodule
 00012d30: 732e 6874 6d6c 2364 6765 6e65 7261 7465  s.html#dgenerate
 00012d40: 2e70 6970 656c 696e 6577 7261 7070 0d0a  .pipelinewrapp..
 00012d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012d60: 2020 2020 2020 2020 2020 2020 6572 2e56              er.V
 00012d70: 4145 5f43 4143 4845 5f4d 454d 4f52 595f  AE_CACHE_MEMORY_
 00012d80: 434f 4e53 5452 4149 4e54 535d 0d0a 2020  CONSTRAINTS]..  
@@ -4862,15 +4862,15 @@
 00012fd0: 6f6e 7472 6f6c 5f6e 6574 5f73 697a 6520  ontrol_net_size 
 00012fe0: 3e20 2861 7661 696c 6162 6c65 202a 2030  > (available * 0
 00012ff0: 2e37 3529 2220 466f 720d 0a20 2020 2020  .75)" For..     
 00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013010: 2020 2020 2020 2053 796e 7461 7820 5365         Syntax Se
 00013020: 653a 205b 6874 7470 733a 2f2f 6467 656e  e: [https://dgen
 00013030: 6572 6174 652e 7265 6164 7468 6564 6f63  erate.readthedoc
-00013040: 732e 696f 2f65 6e2f 7633 2e34 2e32 2f64  s.io/en/v3.4.2/d
+00013040: 732e 696f 2f65 6e2f 7633 2e34 2e33 2f64  s.io/en/v3.4.3/d
 00013050: 6765 6e65 7261 7465 5f73 7562 6d6f 6475  generate_submodu
 00013060: 6c65 732e 6874 6d0d 0a20 2020 2020 2020  les.htm..       
 00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013080: 2020 2020 206c 2364 6765 6e65 7261 7465       l#dgenerate
 00013090: 2e70 6970 656c 696e 6577 7261 7070 6572  .pipelinewrapper
 000130a0: 2e43 4f4e 5452 4f4c 5f4e 4554 5f43 4143  .CONTROL_NET_CAC
 000130b0: 4845 5f4d 454d 4f52 595f 434f 4e53 5452  HE_MEMORY_CONSTR
@@ -4955,27 +4955,27 @@
 000135a0: 6c20 6874 7470 733a 2f2f 646f 776e 6c6f  l https://downlo
 000135b0: 6164 2e70 7974 6f72 6368 2e6f 7267 2f77  ad.pytorch.org/w
 000135c0: 686c 2f63 7531 3231 2f22 0d0a 0d0a 2020  hl/cu121/"....  
 000135d0: 2020 2320 4966 2079 6f75 2077 616e 7420    # If you want 
 000135e0: 6120 7370 6563 6966 6963 2076 6572 7369  a specific versi
 000135f0: 6f6e 0d0a 0d0a 2020 2020 7069 7078 2069  on....    pipx i
 00013600: 6e73 7461 6c6c 2064 6765 6e65 7261 7465  nstall dgenerate
-00013610: 3d3d 332e 342e 3220 5e0d 0a20 2020 202d  ==3.4.2 ^..    -
+00013610: 3d3d 332e 342e 3320 5e0d 0a20 2020 202d  ==3.4.3 ^..    -
 00013620: 2d70 6970 2d61 7267 7320 222d 2d65 7874  -pip-args "--ext
 00013630: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
 00013640: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
 00013650: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
 00013660: 3132 312f 220d 0a0d 0a20 2020 2023 2059  121/"....    # Y
 00013670: 6f75 2063 616e 2069 6e73 7461 6c6c 2077  ou can install w
 00013680: 6974 686f 7574 2070 6970 7820 696e 746f  ithout pipx into
 00013690: 2079 6f75 7220 6f77 6e20 656e 7669 726f   your own enviro
 000136a0: 6e6d 656e 7420 6c69 6b65 2073 6f0d 0a0d  nment like so...
 000136b0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
 000136c0: 2064 6765 6e65 7261 7465 3d3d 332e 342e   dgenerate==3.4.
-000136d0: 3220 2d2d 6578 7472 612d 696e 6465 782d  2 --extra-index-
+000136d0: 3320 2d2d 6578 7472 612d 696e 6465 782d  3 --extra-index-
 000136e0: 7572 6c20 6874 7470 733a 2f2f 646f 776e  url https://down
 000136f0: 6c6f 6164 2e70 7974 6f72 6368 2e6f 7267  load.pytorch.org
 00013700: 2f77 686c 2f63 7531 3231 2f0d 0a0d 0a0d  /whl/cu121/.....
 00013710: 0a49 7420 6973 2072 6563 6f6d 6d65 6e64  .It is recommend
 00013720: 6564 2074 6f20 696e 7374 616c 6c20 6467  ed to install dg
 00013730: 656e 6572 6174 6520 7769 7468 2070 6970  enerate with pip
 00013740: 7820 6966 2079 6f75 2061 7265 206a 7573  x if you are jus
@@ -5157,26 +5157,26 @@
 00014240: 6973 2e63 6f6d 2f6a 6178 2d72 656c 6561  is.com/jax-relea
 00014250: 7365 732f 6a61 785f 6375 6461 5f72 656c  ses/jax_cuda_rel
 00014260: 6561 7365 732e 6874 6d6c 220d 0a0d 0a20  eases.html".... 
 00014270: 2020 2023 2049 6620 796f 7520 7761 6e74     # If you want
 00014280: 2061 2073 7065 6369 6669 6320 7665 7273   a specific vers
 00014290: 696f 6e0d 0a0d 0a20 2020 2070 6970 7820  ion....    pipx 
 000142a0: 696e 7374 616c 6c20 6467 656e 6572 6174  install dgenerat
-000142b0: 653d 3d33 2e34 2e32 205c 0d0a 2020 2020  e==3.4.2 \..    
+000142b0: 653d 3d33 2e34 2e33 205c 0d0a 2020 2020  e==3.4.3 \..    
 000142c0: 2d2d 7069 702d 6172 6773 2022 2d2d 6578  --pip-args "--ex
 000142d0: 7472 612d 696e 6465 782d 7572 6c20 6874  tra-index-url ht
 000142e0: 7470 733a 2f2f 646f 776e 6c6f 6164 2e70  tps://download.p
 000142f0: 7974 6f72 6368 2e6f 7267 2f77 686c 2f63  ytorch.org/whl/c
 00014300: 7531 3231 2f22 0d0a 0d0a 2020 2020 2320  u121/"....    # 
 00014310: 5370 6563 6966 6963 2076 6572 7369 6f6e  Specific version
 00014320: 2077 6974 6820 666c 6178 2f6a 6178 2073   with flax/jax s
 00014330: 7570 706f 7274 0d0a 0d0a 2020 2020 7069  upport....    pi
 00014340: 7078 2069 6e73 7461 6c6c 2064 6765 6e65  px install dgene
 00014350: 7261 7465 5b66 6c61 785d 3d3d 332e 342e  rate[flax]==3.4.
-00014360: 3220 5c0d 0a20 2020 202d 2d70 6970 2d61  2 \..    --pip-a
+00014360: 3320 5c0d 0a20 2020 202d 2d70 6970 2d61  3 \..    --pip-a
 00014370: 7267 7320 222d 2d65 7874 7261 2d69 6e64  rgs "--extra-ind
 00014380: 6578 2d75 726c 2068 7474 7073 3a2f 2f64  ex-url https://d
 00014390: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
 000143a0: 6f72 672f 7768 6c2f 6375 3132 312f 205c  org/whl/cu121/ \
 000143b0: 0d0a 2020 2020 2d66 2068 7474 7073 3a2f  ..    -f https:/
 000143c0: 2f73 746f 7261 6765 2e67 6f6f 676c 6561  /storage.googlea
 000143d0: 7069 732e 636f 6d2f 6a61 782d 7265 6c65  pis.com/jax-rele
@@ -5184,23 +5184,23 @@
 000143f0: 6c65 6173 6573 2e68 746d 6c22 0d0a 0d0a  leases.html"....
 00014400: 2020 2020 2320 596f 7520 6361 6e20 696e      # You can in
 00014410: 7374 616c 6c20 7769 7468 6f75 7420 7069  stall without pi
 00014420: 7078 2069 6e74 6f20 796f 7572 206f 776e  px into your own
 00014430: 2065 6e76 6972 6f6e 6d65 6e74 206c 696b   environment lik
 00014440: 6520 736f 0d0a 0d0a 2020 2020 7069 7033  e so....    pip3
 00014450: 2069 6e73 7461 6c6c 2064 6765 6e65 7261   install dgenera
-00014460: 7465 3d3d 332e 342e 3220 2d2d 6578 7472  te==3.4.2 --extr
+00014460: 7465 3d3d 332e 342e 3320 2d2d 6578 7472  te==3.4.3 --extr
 00014470: 612d 696e 6465 782d 7572 6c20 6874 7470  a-index-url http
 00014480: 733a 2f2f 646f 776e 6c6f 6164 2e70 7974  s://download.pyt
 00014490: 6f72 6368 2e6f 7267 2f77 686c 2f63 7531  orch.org/whl/cu1
 000144a0: 3231 2f0d 0a0d 0a20 2020 2023 204f 7220  21/....    # Or 
 000144b0: 7769 7468 2066 6c61 780d 0a0d 0a20 2020  with flax....   
 000144c0: 2070 6970 3320 696e 7374 616c 6c20 6467   pip3 install dg
 000144d0: 656e 6572 6174 655b 666c 6178 5d3d 3d33  enerate[flax]==3
-000144e0: 2e34 2e32 202d 2d65 7874 7261 2d69 6e64  .4.2 --extra-ind
+000144e0: 2e34 2e33 202d 2d65 7874 7261 2d69 6e64  .4.3 --extra-ind
 000144f0: 6578 2d75 726c 2068 7474 7073 3a2f 2f64  ex-url https://d
 00014500: 6f77 6e6c 6f61 642e 7079 746f 7263 682e  ownload.pytorch.
 00014510: 6f72 672f 7768 6c2f 6375 3132 312f 205c  org/whl/cu121/ \
 00014520: 0d0a 2020 2020 2d66 2068 7474 7073 3a2f  ..    -f https:/
 00014530: 2f73 746f 7261 6765 2e67 6f6f 676c 6561  /storage.googlea
 00014540: 7069 732e 636f 6d2f 6a61 782d 7265 6c65  pis.com/jax-rele
 00014550: 6173 6573 2f6a 6178 5f63 7564 615f 7265  ases/jax_cuda_re
@@ -5745,23 +5745,23 @@
 00016700: 2066 6f72 2062 7265 7669 7479 2e0d 0a0d   for brevity....
 00016710: 0a59 6f75 2063 616e 2064 6f77 6e6c 6f61  .You can downloa
 00016720: 6420 7468 656d 2068 6572 653a 0d0a 0d0a  d them here:....
 00016730: 202a 2060 6d79 2d69 6d61 6765 2d73 6565   * `my-image-see
 00016740: 642e 706e 6720 3c68 7474 7073 3a2f 2f72  d.png <https://r
 00016750: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
 00016760: 7465 6e74 2e63 6f6d 2f54 6572 696b 732f  tent.com/Teriks/
-00016770: 6467 656e 6572 6174 652f 7633 2e34 2e32  dgenerate/v3.4.2
+00016770: 6467 656e 6572 6174 652f 7633 2e34 2e33  dgenerate/v3.4.3
 00016780: 2f65 7861 6d70 6c65 732f 6d65 6469 612f  /examples/media/
 00016790: 646f 672d 6f6e 2d62 656e 6368 2e70 6e67  dog-on-bench.png
 000167a0: 3e60 5f0d 0a20 2a20 606d 792d 6d61 736b  >`_.. * `my-mask
 000167b0: 2d69 6d61 6765 2e70 6e67 203c 6874 7470  -image.png <http
 000167c0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
 000167d0: 6572 636f 6e74 656e 742e 636f 6d2f 5465  ercontent.com/Te
 000167e0: 7269 6b73 2f64 6765 6e65 7261 7465 2f76  riks/dgenerate/v
-000167f0: 332e 342e 322f 6578 616d 706c 6573 2f6d  3.4.2/examples/m
+000167f0: 332e 342e 332f 6578 616d 706c 6573 2f6d  3.4.3/examples/m
 00016800: 6564 6961 2f64 6f67 2d6f 6e2d 6265 6e63  edia/dog-on-benc
 00016810: 682d 6d61 736b 2e70 6e67 3e60 5f0d 0a0d  h-mask.png>`_...
 00016820: 0a54 6865 2063 6f6d 6d61 6e64 2062 656c  .The command bel
 00016830: 6f77 2067 656e 6572 6174 6573 2061 2063  ow generates a c
 00016840: 6174 2073 6974 7469 6e67 206f 6e20 6120  at sitting on a 
 00016850: 6265 6e63 6820 7769 7468 2074 6865 2069  bench with the i
 00016860: 6d61 6765 7320 6672 6f6d 2074 6865 206c  mages from the l
@@ -8356,15 +8356,15 @@
 00020a30: 7374 2069 6e66 6572 656e 6365 2073 7465  st inference ste
 00020a40: 702e 0d0a 0d0a 0d0a 5468 6573 6520 6578  p.......These ex
 00020a50: 616d 706c 6573 2075 7365 3a20 6076 6572  amples use: `ver
 00020a60: 6d65 6572 5f63 616e 6e79 5f65 6467 6564  meer_canny_edged
 00020a70: 2e70 6e67 203c 6874 7470 733a 2f2f 7261  .png <https://ra
 00020a80: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
 00020a90: 656e 742e 636f 6d2f 5465 7269 6b73 2f64  ent.com/Teriks/d
-00020aa0: 6765 6e65 7261 7465 2f76 332e 342e 322f  generate/v3.4.2/
+00020aa0: 6765 6e65 7261 7465 2f76 332e 342e 332f  generate/v3.4.3/
 00020ab0: 6578 616d 706c 6573 2f6d 6564 6961 2f76  examples/media/v
 00020ac0: 6572 6d65 6572 5f63 616e 6e79 5f65 6467  ermeer_canny_edg
 00020ad0: 6564 2e70 6e67 3e60 5f0d 0a0d 0a0d 0a2e  ed.png>`_.......
 00020ae0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2062  . code-block:: b
 00020af0: 6173 680d 0a0d 0a20 2020 2023 2054 6f72  ash....    # Tor
 00020b00: 6368 2065 7861 6d70 6c65 2c20 7573 6520  ch example, use 
 00020b10: 2276 6572 6d65 6572 5f63 616e 6e79 5f65  "vermeer_canny_e
@@ -8944,15 +8944,15 @@
 00022ef0: 7769 7468 2061 206d 6f64 656c 202b 2061  with a model + a
 00022f00: 2043 6f6e 7472 6f6c 4e65 742e 0d0a 0d0a   ControlNet.....
 00022f10: 5468 6973 2069 6d61 6765 206f 6620 6120  This image of a 
 00022f20: 6068 6f72 7365 203c 6874 7470 733a 2f2f  `horse <https://
 00022f30: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
 00022f40: 6e74 656e 742e 636f 6d2f 5465 7269 6b73  ntent.com/Teriks
 00022f50: 2f64 6765 6e65 7261 7465 2f76 332e 342e  /dgenerate/v3.4.
-00022f60: 322f 6578 616d 706c 6573 2f6d 6564 6961  2/examples/media
+00022f60: 332f 6578 616d 706c 6573 2f6d 6564 6961  3/examples/media
 00022f70: 2f68 6f72 7365 322e 6a70 6567 3e60 5f0d  /horse2.jpeg>`_.
 00022f80: 0a69 7320 7573 6564 2069 6e20 7468 6520  .is used in the 
 00022f90: 6578 616d 706c 6520 6265 6c6f 7720 7769  example below wi
 00022fa0: 7468 2061 2043 6f6e 7472 6f6c 4e65 7420  th a ControlNet 
 00022fb0: 7468 6174 2069 7320 7472 6169 6e65 6420  that is trained 
 00022fc0: 746f 2067 656e 6572 6174 6520 696d 6167  to generate imag
 00022fd0: 6573 2066 726f 6d20 6361 6e6e 7920 6564  es from canny ed
@@ -9183,15 +9183,15 @@
 00023de0: 5468 6520 696d 6167 6520 7573 6564 2069  The image used i
 00023df0: 6e20 7468 6520 6578 616d 706c 6520 6265  n the example be
 00023e00: 6c6f 7720 6973 2074 6869 7320 606c 6f77  low is this `low
 00023e10: 2072 6573 6f6c 7574 696f 6e20 6361 7420   resolution cat 
 00023e20: 3c68 7474 7073 3a2f 2f72 6177 2e67 6974  <https://raw.git
 00023e30: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
 00023e40: 6f6d 2f54 6572 696b 732f 6467 656e 6572  om/Teriks/dgener
-00023e50: 6174 652f 7633 2e34 2e32 2f65 7861 6d70  ate/v3.4.2/examp
+00023e50: 6174 652f 7633 2e34 2e33 2f65 7861 6d70  ate/v3.4.3/examp
 00023e60: 6c65 732f 6d65 6469 612f 6c6f 775f 7265  les/media/low_re
 00023e70: 735f 6361 742e 706e 673e 605f 0d0a 0d0a  s_cat.png>`_....
 00023e80: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
 00023e90: 6261 7368 0d0a 0d0a 2020 2020 2320 5468  bash....    # Th
 00023ea0: 6520 696d 6167 6520 7072 6f64 7563 6564  e image produced
 00023eb0: 2077 6974 6820 7468 6973 206d 6f64 656c   with this model
 00023ec0: 2077 696c 6c20 6265 0d0a 2020 2020 2320   will be..    # 
@@ -10183,15 +10183,15 @@
 00027c60: 6c6c 6f77 696e 6720 6973 2061 2063 6f6e  llowing is a con
 00027c70: 6669 6720 6669 6c65 2065 7861 6d70 6c65  fig file example
 00027c80: 2074 6861 7420 636f 7665 7273 2076 6572   that covers ver
 00027c90: 7920 6261 7369 6320 7379 6e74 6178 2063  y basic syntax c
 00027ca0: 6f6e 6365 7074 733a 0d0a 0d0a 2e2e 2063  oncepts:...... c
 00027cb0: 6f64 652d 626c 6f63 6b3a 3a20 6a69 6e6a  ode-block:: jinj
 00027cc0: 610d 0a0d 0a20 2020 2023 2120 6467 656e  a....    #! dgen
-00027cd0: 6572 6174 6520 332e 342e 320d 0a0d 0a20  erate 3.4.2.... 
+00027cd0: 6572 6174 6520 332e 342e 330d 0a0d 0a20  erate 3.4.3.... 
 00027ce0: 2020 2023 2049 6620 6120 6861 7368 2d62     # If a hash-b
 00027cf0: 616e 6720 7665 7273 696f 6e20 6973 2070  ang version is p
 00027d00: 726f 7669 6465 6420 696e 2074 6865 2066  rovided in the f
 00027d10: 6f72 6d61 7420 6162 6f76 650d 0a20 2020  ormat above..   
 00027d20: 2023 2061 2077 6172 6e69 6e67 2077 696c   # a warning wil
 00027d30: 6c20 6265 2070 726f 6475 6365 6420 6966  l be produced if
 00027d40: 2074 6865 2076 6572 7369 6f6e 2079 6f75   the version you
@@ -10450,15 +10450,15 @@
 00028d10: 6162 6c65 7320 7365 7420 7769 7468 2074  ables set with t
 00028d20: 6865 2060 605c 7365 7460 6020 6469 7265  he ``\set`` dire
 00028d30: 6374 6976 6520 7769 6c6c 2061 6c73 6f20  ctive will also 
 00028d40: 6265 206d 656e 7469 6f6e 6564 2069 6e20  be mentioned in 
 00028d50: 7468 6973 206f 7574 7075 742e 0d0a 0d0a  this output.....
 00028d60: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
 00028d70: 6a69 6e6a 610d 0a0d 0a20 2020 2023 2120  jinja....    #! 
-00028d80: 6467 656e 6572 6174 6520 332e 342e 320d  dgenerate 3.4.2.
+00028d80: 6467 656e 6572 6174 6520 332e 342e 330d  dgenerate 3.4.3.
 00028d90: 0a0d 0a20 2020 2023 2049 6e76 6f63 6174  ...    # Invocat
 00028da0: 696f 6e20 7769 6c6c 2070 726f 6365 6564  ion will proceed
 00028db0: 2061 7320 6e6f 726d 616c 0d0a 0d0a 2020   as normal....  
 00028dc0: 2020 7374 6162 696c 6974 7961 692f 7374    stabilityai/st
 00028dd0: 6162 6c65 2d64 6966 6675 7369 6f6e 2d32  able-diffusion-2
 00028de0: 2d31 202d 2d70 726f 6d70 7473 2022 6120  -1 --prompts "a 
 00028df0: 6d61 6e20 7761 6c6b 696e 6720 6f6e 2074  man walking on t
@@ -11236,15 +11236,15 @@
 0002be30: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
 0002be40: 7468 6520 7370 6563 6966 6965 6420 6469  the specified di
 0002be50: 7265 6374 6976 6573 2e20 5468 6520 6261  rectives. The ba
 0002be60: 636b 736c 6173 6820 6d61 7920 6265 206f  ckslash may be o
 0002be70: 6d69 7474 6564 2e0d 0a0d 0a0d 0a2e 2e20  mitted......... 
 0002be80: 636f 6465 2d62 6c6f 636b 3a3a 206a 696e  code-block:: jin
 0002be90: 6a61 0d0a 0d0a 2020 2020 2321 2064 6765  ja....    #! dge
-0002bea0: 6e65 7261 7465 2033 2e34 2e32 0d0a 0d0a  nerate 3.4.2....
+0002bea0: 6e65 7261 7465 2033 2e34 2e33 0d0a 0d0a  nerate 3.4.3....
 0002beb0: 2020 2020 2320 596f 7520 6361 6e20 6465      # You can de
 0002bec0: 6669 6e65 2079 6f75 7220 6f77 6e20 7465  fine your own te
 0002bed0: 6d70 6c61 7465 2076 6172 6961 626c 6573  mplate variables
 0002bee0: 2077 6974 6820 7468 6520 5c73 6574 2064   with the \set d
 0002bef0: 6972 6563 7469 7665 0d0a 2020 2020 2320  irective..    # 
 0002bf00: 7468 6520 5c73 6574 2064 6972 6563 7469  the \set directi
 0002bf10: 7665 2064 6f65 7320 6e6f 7420 646f 2061  ve does not do a
@@ -11689,15 +11689,15 @@
 0002da80: 796f 750d 0a63 616e 2067 6c6f 6220 6469  you..can glob di
 0002da90: 7265 6374 6f72 6965 7320 7573 696e 6720  rectories using 
 0002daa0: 6675 6e63 7469 6f6e 7320 6672 6f6d 2074  functions from t
 0002dab0: 6865 2067 6c6f 6220 6d6f 6475 6c65 206c  he glob module l
 0002dac0: 696b 6520 736f 3a0d 0a0d 0a2e 2e20 636f  ike so:...... co
 0002dad0: 6465 2d62 6c6f 636b 3a3a 206a 696e 6a61  de-block:: jinja
 0002dae0: 0d0a 0d0a 2020 2020 2321 2064 6765 6e65  ....    #! dgene
-0002daf0: 7261 7465 2033 2e34 2e32 0d0a 0d0a 2020  rate 3.4.2....  
+0002daf0: 7261 7465 2033 2e34 2e33 0d0a 0d0a 2020  rate 3.4.3....  
 0002db00: 2020 2320 5468 6520 6d6f 7374 2062 6173    # The most bas
 0002db10: 6963 2075 7361 6765 2069 7320 6675 6c6c  ic usage is full
 0002db20: 2065 7870 616e 7369 6f6e 206f 6620 6576   expansion of ev
 0002db30: 6572 7920 6669 6c65 0d0a 0d0a 2020 2020  ery file....    
 0002db40: 5c73 6574 206d 7966 696c 6573 207b 7b20  \set myfiles {{ 
 0002db50: 7175 6f74 6528 676c 6f62 2e67 6c6f 6228  quote(glob.glob(
 0002db60: 276d 795f 696d 6167 6573 2f2a 2e70 6e67  'my_images/*.png
@@ -11734,15 +11734,15 @@
 0002dd50: 636f 6d6d 616e 6420 6060 696d 6167 652d  command ``image-
 0002dd60: 7072 6f63 6573 7360 6020 6861 7320 6120  process`` has a 
 0002dd70: 636f 6e66 6967 2064 6972 6563 7469 7665  config directive
 0002dd80: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2e   implementation.
 0002dd90: 0d0a 0d0a 0d0a 2e2e 2063 6f64 652d 626c  ........ code-bl
 0002dda0: 6f63 6b3a 3a20 6a69 6e6a 610d 0a0d 0a20  ock:: jinja.... 
 0002ddb0: 2020 2023 2120 6467 656e 6572 6174 6520     #! dgenerate 
-0002ddc0: 332e 342e 320d 0a0d 0a20 2020 2023 2070  3.4.2....    # p
+0002ddc0: 332e 342e 330d 0a0d 0a20 2020 2023 2070  3.4.3....    # p
 0002ddd0: 7269 6e74 2074 6865 2068 656c 7020 6d65  rint the help me
 0002dde0: 7373 6167 6520 6f66 202d 2d73 7562 2d63  ssage of --sub-c
 0002ddf0: 6f6d 6d61 6e64 2069 6d61 6765 2d70 726f  ommand image-pro
 0002de00: 6365 7373 2c20 7468 6973 2064 6f65 730d  cess, this does.
 0002de10: 0a20 2020 2023 206e 6f74 2063 6175 7365  .    # not cause
 0002de20: 2074 6865 2063 6f6e 6669 6720 746f 2065   the config to e
 0002de30: 7869 740d 0a0d 0a20 2020 205c 696d 6167  xit....    \imag
@@ -11794,15 +11794,15 @@
 0002e110: 596f 7520 6361 6e20 6578 6974 2061 2063  You can exit a c
 0002e120: 6f6e 6669 6720 6561 726c 7920 6966 206e  onfig early if n
 0002e130: 6565 6420 6265 2075 7369 6e67 2074 6865  eed be using the
 0002e140: 2060 605c 6578 6974 6060 2064 6972 6563   ``\exit`` direc
 0002e150: 7469 7665 0d0a 0d0a 0d0a 2e2e 2063 6f64  tive........ cod
 0002e160: 652d 626c 6f63 6b3a 3a20 6a69 6e6a 610d  e-block:: jinja.
 0002e170: 0a0d 0a20 2020 2023 2120 6467 656e 6572  ...    #! dgener
-0002e180: 6174 6520 332e 342e 320d 0a0d 0a20 2020  ate 3.4.2....   
+0002e180: 6174 6520 332e 342e 330d 0a0d 0a20 2020  ate 3.4.3....   
 0002e190: 2023 2065 7869 7420 7468 6520 7072 6f63   # exit the proc
 0002e1a0: 6573 7320 7769 7468 2072 6574 7572 6e20  ess with return 
 0002e1b0: 636f 6465 2031 2c20 7768 6963 6820 696e  code 1, which in
 0002e1c0: 6469 6361 7465 7320 616e 2065 7272 6f72  dicates an error
 0002e1d0: 0d0a 0d0a 2020 2020 5c70 7269 6e74 2022  ....    \print "
 0002e1e0: 736f 6d65 2065 7272 6f72 206f 6363 7572  some error occur
 0002e1f0: 7265 6422 0d0a 2020 2020 5c65 7869 7420  red"..    \exit 
@@ -11952,42 +11952,42 @@
 0002eaf0: 6520 7072 6f63 6573 736f 7220 706c 7567  e processor plug
 0002eb00: 696e 7320 6361 6e20 6265 2066 6f75 6e64  ins can be found
 0002eb10: 0d0a 696e 2074 6865 2060 2277 7269 7469  ..in the `"writi
 0002eb20: 6e67 5f70 6c75 6769 6e73 2f69 6d61 6765  ng_plugins/image
 0002eb30: 5f70 726f 6365 7373 6f72 2220 3c68 7474  _processor" <htt
 0002eb40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 0002eb50: 5465 7269 6b73 2f64 6765 6e65 7261 7465  Teriks/dgenerate
-0002eb60: 2f74 7265 652f 7633 2e34 2e32 2f65 7861  /tree/v3.4.2/exa
+0002eb60: 2f74 7265 652f 7633 2e34 2e33 2f65 7861  /tree/v3.4.3/exa
 0002eb70: 6d70 6c65 732f 7772 6974 696e 675f 706c  mples/writing_pl
 0002eb80: 7567 696e 732f 696d 6167 655f 7072 6f63  ugins/image_proc
 0002eb90: 6573 736f 723e 605f 0d0a 666f 6c64 6572  essor>`_..folder
 0002eba0: 206f 6620 7468 6520 6578 616d 706c 6573   of the examples
 0002ebb0: 2066 6f6c 6465 722e 0d0a 0d0a 5468 6520   folder.....The 
 0002ebc0: 736f 7572 6365 2063 6f64 6520 666f 7220  source code for 
 0002ebd0: 7468 6520 6275 696c 7420 696e 2060 6361  the built in `ca
 0002ebe0: 6e6e 7920 3c68 7474 7073 3a2f 2f67 6974  nny <https://git
 0002ebf0: 6875 622e 636f 6d2f 5465 7269 6b73 2f64  hub.com/Teriks/d
 0002ec00: 6765 6e65 7261 7465 2f62 6c6f 622f 7633  generate/blob/v3
-0002ec10: 2e34 2e32 2f64 6765 6e65 7261 7465 2f69  .4.2/dgenerate/i
+0002ec10: 2e34 2e33 2f64 6765 6e65 7261 7465 2f69  .4.3/dgenerate/i
 0002ec20: 6d61 6765 7072 6f63 6573 736f 7273 2f63  mageprocessors/c
 0002ec30: 616e 6e79 2e70 793e 605f 2070 726f 6365  anny.py>`_ proce
 0002ec40: 7373 6f72 2c0d 0a74 6865 2060 6f70 656e  ssor,..the `open
 0002ec50: 706f 7365 203c 6874 7470 733a 2f2f 6769  pose <https://gi
 0002ec60: 7468 7562 2e63 6f6d 2f54 6572 696b 732f  thub.com/Teriks/
 0002ec70: 6467 656e 6572 6174 652f 626c 6f62 2f76  dgenerate/blob/v
-0002ec80: 332e 342e 322f 6467 656e 6572 6174 652f  3.4.2/dgenerate/
+0002ec80: 332e 342e 332f 6467 656e 6572 6174 652f  3.4.3/dgenerate/
 0002ec90: 696d 6167 6570 726f 6365 7373 6f72 732f  imageprocessors/
 0002eca0: 6f70 656e 706f 7365 2e70 793e 605f 2070  openpose.py>`_ p
 0002ecb0: 726f 6365 7373 6f72 2c20 616e 6420 7468  rocessor, and th
 0002ecc0: 6520 7369 6d70 6c65 0d0a 6070 696c 6c6f  e simple..`pillo
 0002ecd0: 7720 696d 6167 6520 6f70 6572 6174 696f  w image operatio
 0002ece0: 6e73 203c 6874 7470 733a 2f2f 6769 7468  ns <https://gith
 0002ecf0: 7562 2e63 6f6d 2f54 6572 696b 732f 6467  ub.com/Teriks/dg
 0002ed00: 656e 6572 6174 652f 626c 6f62 2f76 332e  enerate/blob/v3.
-0002ed10: 342e 322f 6467 656e 6572 6174 652f 696d  4.2/dgenerate/im
+0002ed10: 342e 332f 6467 656e 6572 6174 652f 696d  4.3/dgenerate/im
 0002ed20: 6167 6570 726f 6365 7373 6f72 732f 696d  ageprocessors/im
 0002ed30: 6167 656f 7073 2e70 793e 605f 2070 726f  ageops.py>`_ pro
 0002ed40: 6365 7373 6f72 7320 6361 6e20 616c 736f  cessors can also
 0002ed50: 0d0a 6265 206f 6620 7265 6665 7265 6e63  ..be of referenc
 0002ed60: 6520 6173 2074 6865 7920 6172 6520 7772  e as they are wr
 0002ed70: 6974 7465 6e20 6173 2069 6e74 6572 6e61  itten as interna
 0002ed80: 6c20 696d 6167 6520 7072 6f63 6573 736f  l image processo
@@ -11996,15 +11996,15 @@
 0002edb0: 7469 6e67 2063 6f6e 6669 6720 6469 7265  ting config dire
 0002edc0: 6374 6976 6573 2063 616e 2062 6520 666f  ctives can be fo
 0002edd0: 756e 6420 696e 2074 6865 0d0a 6022 7772  und in the..`"wr
 0002ede0: 6974 696e 675f 706c 7567 696e 732f 636f  iting_plugins/co
 0002edf0: 6e66 6967 5f64 6972 6563 7469 7665 2220  nfig_directive" 
 0002ee00: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
 0002ee10: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-0002ee20: 7261 7465 2f74 7265 652f 7633 2e34 2e32  rate/tree/v3.4.2
+0002ee20: 7261 7465 2f74 7265 652f 7633 2e34 2e33  rate/tree/v3.4.3
 0002ee30: 2f65 7861 6d70 6c65 732f 7772 6974 696e  /examples/writin
 0002ee40: 675f 706c 7567 696e 732f 636f 6e66 6967  g_plugins/config
 0002ee50: 5f64 6972 6563 7469 7665 3e60 5f20 666f  _directive>`_ fo
 0002ee60: 6c64 6572 0d0a 6f66 2074 6865 2065 7861  lder..of the exa
 0002ee70: 6d70 6c65 7320 666f 6c64 6572 2e0d 0a0d  mples folder....
 0002ee80: 0a43 7572 7265 6e74 6c79 2074 6865 206f  .Currently the o
 0002ee90: 6e6c 7920 696e 7465 726e 616c 2064 6972  nly internal dir
@@ -12014,15 +12014,15 @@
 0002eed0: 5c69 6d61 6765 5f70 726f 6365 7373 6060  \image_process``
 0002eee0: 2064 6972 6563 7469 7665 2c0d 0a77 686f   directive,..who
 0002eef0: 2773 2073 6f75 7263 6520 6669 6c65 2060  's source file `
 0002ef00: 6361 6e20 6265 206c 6f63 6174 6564 2068  can be located h
 0002ef10: 6572 6520 3c68 7474 7073 3a2f 2f67 6974  ere <https://git
 0002ef20: 6875 622e 636f 6d2f 5465 7269 6b73 2f64  hub.com/Teriks/d
 0002ef30: 6765 6e65 7261 7465 2f62 6c6f 622f 7633  generate/blob/v3
-0002ef40: 2e34 2e32 2f64 6765 6e65 7261 7465 2f62  .4.2/dgenerate/b
+0002ef40: 2e34 2e33 2f64 6765 6e65 7261 7465 2f62  .4.3/dgenerate/b
 0002ef50: 6174 6368 7072 6f63 6573 732f 696d 6167  atchprocess/imag
 0002ef60: 655f 7072 6f63 6573 735f 6469 7265 6374  e_process_direct
 0002ef70: 6976 652e 7079 3e60 5f2c 0d0a 7468 6520  ive.py>`_,..the 
 0002ef80: 736f 7572 6365 2066 696c 6520 666f 7220  source file for 
 0002ef90: 7468 6973 2064 6972 6563 7469 7665 2069  this directive i
 0002efa0: 7320 7465 7273 6520 6173 206d 6f73 7420  s terse as most 
 0002efb0: 6f66 2060 605c 696d 6167 655f 7072 6f63  of ``\image_proc
@@ -12035,15 +12035,15 @@
 0002f020: 7768 6963 6820 6973 2061 6c73 6f20 7573  which is also us
 0002f030: 6564 2066 6f72 2060 602d 2d73 7562 2d63  ed for ``--sub-c
 0002f040: 6f6d 6d61 6e64 2069 6d61 6765 2d70 726f  ommand image-pro
 0002f050: 6365 7373 6060 2069 730d 0a60 6973 2069  cess`` is..`is i
 0002f060: 6d70 6c65 6d65 6e74 6564 2068 6572 6520  mplemented here 
 0002f070: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
 0002f080: 636f 6d2f 5465 7269 6b73 2f64 6765 6e65  com/Teriks/dgene
-0002f090: 7261 7465 2f62 6c6f 622f 7633 2e34 2e32  rate/blob/v3.4.2
+0002f090: 7261 7465 2f62 6c6f 622f 7633 2e34 2e33  rate/blob/v3.4.3
 0002f0a0: 2f64 6765 6e65 7261 7465 2f69 6d61 6765  /dgenerate/image
 0002f0b0: 5f70 726f 6365 7373 3e60 5f2e 0d0a 0d0a  _process>`_.....
 0002f0c0: 4669 6c65 2043 6163 6865 2043 6f6e 7472  File Cache Contr
 0002f0d0: 6f6c 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ol..============
 0002f0e0: 3d3d 3d3d 3d3d 0d0a 0d0a 6467 656e 6572  ======....dgener
 0002f0f0: 6174 6520 7769 6c6c 2063 6163 6865 2060  ate will cache `
 0002f100: 602d 2d69 6d61 6765 2d73 6565 6473 6060  `--image-seeds``
```

### Comparing `dgenerate-3.4.2/dgenerate.egg-info/SOURCES.txt` & `dgenerate-3.4.3/dgenerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/dgenerate.egg-info/requires.txt` & `dgenerate-3.4.3/dgenerate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/setup.py` & `dgenerate-3.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/tests/unit/concept_uri_parser_test.py` & `dgenerate-3.4.3/tests/unit/concept_uri_parser_test.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/tests/unit/image_seed_parse_test.py` & `dgenerate-3.4.3/tests/unit/image_seed_parse_test.py`

 * *Files identical despite different names*

### Comparing `dgenerate-3.4.2/tests/unit/plugin_loading_test.py` & `dgenerate-3.4.3/tests/unit/plugin_loading_test.py`

 * *Files identical despite different names*

