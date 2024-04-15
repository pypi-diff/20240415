# Comparing `tmp/netspresso_trainer-0.1.2.tar.gz` & `tmp/netspresso_trainer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netspresso_trainer-0.1.2.tar", last modified: Wed Jan 17 05:47:02 2024, max compression
+gzip compressed data, was "netspresso_trainer-0.2.0.tar", last modified: Mon Apr 15 01:10:44 2024, max compression
```

## Comparing `netspresso_trainer-0.1.2.tar` & `netspresso_trainer-0.2.0.tar`

### file list

```diff
@@ -1,206 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.715618 netspresso_trainer-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-01-17 05:47:02.715618 netspresso_trainer-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 05:47:02.715618 netspresso_trainer-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.687618 netspresso_trainer-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.691618 netspresso_trainer-0.1.2/src/netspresso_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.695618 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    34020 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/cfg/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.695618 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.695618 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28951 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/augmentation/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/augmentation/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/augmentation/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.695618 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/classification/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/classification/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/classification/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.695618 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/detection/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/detection/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/detection/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.699618 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.699618 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.699618 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/netspresso.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.699618 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.699618 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.699618 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/detection/retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/detection/yolox.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.699618 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/losses/segmentation/pidnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.703618 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.703618 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/classification/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.703618 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/detection/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.703618 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/segmentation/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.703618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.703618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.703618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/core/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/darknet.py
--rw-r--r--   0 runner    (1001) docker     (127)    16297 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/efficientformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11295 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mixnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    16497 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/experimental/pidnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/classification/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/classification/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/classification/core/fc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/classification/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/classification/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/anchor_free_decoupled_head.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/detection/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.707618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/experimental/fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/experimental/yolopafpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.711618 netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/base_metaformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/depth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/pidnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.711618 netspresso_trainer-0.1.2/src/netspresso_trainer/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/optimizers/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/optimizers/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/optimizers/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.711618 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.711618 netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/register.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.715618 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/cosine_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/cosine_warm_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/poly_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/step_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/trainer_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/trainer_cli_multi_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/trainer_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/trainer_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/trainer_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.715618 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/fx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-01-17 05:46:56.000000 netspresso_trainer-0.1.2/src/netspresso_trainer/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 05:47:02.691618 netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-01-17 05:47:02.000000 netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-01-17 05:47:02.000000 netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 05:47:02.000000 netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-17 05:47:02.000000 netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-17 05:47:02.000000 netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-17 05:47:02.000000 netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.609402 netspresso_trainer-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.617402 netspresso_trainer-0.2.0/src/netspresso_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.617402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31598 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/image_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/custom/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/detection/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.621402 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/evaluator_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/evaluator_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/inferencer_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/inferencer_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/pose_estimation/rtmcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/pidnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.625403 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/pose_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/pose_estimation/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/darknet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/efficientformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11601 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/pidnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.629402 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/core/fc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/classification/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/anchor_free_decoupled_head.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/pose_estimation/experimental/rtmcc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.633403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/yolopafpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/base_metaformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/pidnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.637403 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/pose_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/task_processors/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/pose_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_warm_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/poly_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/step_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/trainer_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/trainer_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.641403 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/engine_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/fx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/model_ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-15 01:10:35.000000 netspresso_trainer-0.2.0/src/netspresso_trainer/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:10:44.617402 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 01:10:44.000000 netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/top_level.txt
```

### Comparing `netspresso_trainer-0.1.2/LICENSE` & `netspresso_trainer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/PKG-INFO` & `netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: netspresso_trainer
-Version: 0.1.2
+Name: netspresso-trainer
+Version: 0.2.0
 Summary: NetsPresso Python Package
 Home-page: https://github.com/Nota-NetsPresso/netspresso-trainer
 Author: NetsPresso
 Author-email: netspresso@nota.ai
 License: UNKNOWN
 Description: <div align="center">
             <img src="./assets/netspresso_trainer_header_tmp.png" width="800"/>
@@ -24,24 +24,54 @@
           <a href="https://github.com/Nota-NetsPresso/netspresso-trainer/issues">Issues</a> •
           <a href="https://nota-netspresso.github.io/netspresso-trainer">Docs</a>
         </p>
         </div>
         
         _____
         
-        
         ## Table of contents
         
         <!-- toc -->
         
-        - [Getting started](#getting-started)
         - [Installation](#installation)
+        - [Getting started](#getting-started)
         
         <!-- tocstop -->
         
+        ## Installation (Stable)
+        
+        ### Prerequisites
+        
+        - Python `3.8` | `3.9` | `3.10`
+        - PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
+        
+        ### Install with pypi
+        
+        ```bash
+        pip install netspresso_trainer
+        ```
+        
+        ### Install with GitHub
+        
+        ```bash
+        pip install git+https://github.com/Nota-NetsPresso/netspresso-trainer.git@master
+        ```
+        
+        To install with editable mode,
+        
+        ```bash
+        git clone -b master https://github.com/Nota-NetsPresso/netspresso-trainer.git
+        pip install -e netspresso-trainer
+        ```
+        
+        ### Set-up with docker
+        
+        Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
+        For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
+        
         ## Getting started
         
         Write your training script in `train.py` like:
         
         ```python
         from netspresso_trainer import train_cli
         
@@ -74,45 +104,14 @@
           --environment config/environment.yaml
         ```
         
         Please refer to [`scripts/example_train.sh`](./scripts/example_train.sh).
         
         NetsPresso Trainer is compatible with [NetsPresso](https://netspresso.ai/) service. We provide NetsPresso Trainer tutorial that contains whole procedure from model train to model compression and benchmark. Please refer to our [colab tutorial](https://colab.research.google.com/drive/1RBKMCPEa4x-4X31zqzTS8WgQI9TQt3e-?usp=sharing).
         
-        ## Installation
-        
-        ### Prerequisites
-        
-        - Python `3.8` | `3.9` | `3.10`
-        - PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
-        
-        ### Install with pypi (stable)
-        
-        ```bash
-        pip install netspresso_trainer
-        ```
-        
-        ### Install with GitHub
-        
-        ```bash
-        pip install git+https://github.com:Nota-NetsPresso/netspresso-trainer.git@stable
-        ```
-        
-        To install with editable mode,
-        
-        ```bash
-        git clone https://github.com:Nota-NetsPresso/netspresso-trainer.git .
-        pip install -e netspresso-trainer
-        ```
-        
-        ### Set-up with docker
-        
-        Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
-        For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
-        
         ## Tensorboard
         
         We provide basic tensorboard to track your training status. Run the tensorboard with the following command: 
         
         ```bash
         tensorboard --logdir ./outputs --port 50001 --bind_all
         ```
```

### Comparing `netspresso_trainer-0.1.2/README.md` & `netspresso_trainer-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,54 @@
   <a href="https://github.com/Nota-NetsPresso/netspresso-trainer/issues">Issues</a> •
   <a href="https://nota-netspresso.github.io/netspresso-trainer">Docs</a>
 </p>
 </div>
 
 _____
 
-
 ## Table of contents
 
 <!-- toc -->
 
-- [Getting started](#getting-started)
 - [Installation](#installation)
+- [Getting started](#getting-started)
 
 <!-- tocstop -->
 
+## Installation (Stable)
+
+### Prerequisites
+
+- Python `3.8` | `3.9` | `3.10`
+- PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
+
+### Install with pypi
+
+```bash
+pip install netspresso_trainer
+```
+
+### Install with GitHub
+
+```bash
+pip install git+https://github.com/Nota-NetsPresso/netspresso-trainer.git@master
+```
+
+To install with editable mode,
+
+```bash
+git clone -b master https://github.com/Nota-NetsPresso/netspresso-trainer.git
+pip install -e netspresso-trainer
+```
+
+### Set-up with docker
+
+Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
+For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
+
 ## Getting started
 
 Write your training script in `train.py` like:
 
 ```python
 from netspresso_trainer import train_cli
 
@@ -66,45 +96,14 @@
   --environment config/environment.yaml
 ```
 
 Please refer to [`scripts/example_train.sh`](./scripts/example_train.sh).
 
 NetsPresso Trainer is compatible with [NetsPresso](https://netspresso.ai/) service. We provide NetsPresso Trainer tutorial that contains whole procedure from model train to model compression and benchmark. Please refer to our [colab tutorial](https://colab.research.google.com/drive/1RBKMCPEa4x-4X31zqzTS8WgQI9TQt3e-?usp=sharing).
 
-## Installation
-
-### Prerequisites
-
-- Python `3.8` | `3.9` | `3.10`
-- PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
-
-### Install with pypi (stable)
-
-```bash
-pip install netspresso_trainer
-```
-
-### Install with GitHub
-
-```bash
-pip install git+https://github.com:Nota-NetsPresso/netspresso-trainer.git@stable
-```
-
-To install with editable mode,
-
-```bash
-git clone https://github.com:Nota-NetsPresso/netspresso-trainer.git .
-pip install -e netspresso-trainer
-```
-
-### Set-up with docker
-
-Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
-For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
-
 ## Tensorboard
 
 We provide basic tensorboard to track your training status. Run the tensorboard with the following command: 
 
 ```bash
 tensorboard --logdir ./outputs --port 50001 --bind_all
 ```
```

### Comparing `netspresso_trainer-0.1.2/pyproject.toml` & `netspresso_trainer-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/setup.py` & `netspresso_trainer-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     install_requires=requirements,
     package_dir={"": "src"},
     packages=find_packages("src", exclude=("tests",)),
     package_data={"": ["VERSION"]},
     python_requires=">=3.8",
     entry_points={
         "console_scripts": [
-            "netspresso-train = netspresso_trainer.trainer_cli:train_cli",
+            "netspresso-train = netspresso_trainer.trainer_main:train_cli",
         ],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/augmentation/transforms.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/augmentation/transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 
 import cv2
 import numpy as np
 import PIL.Image as Image
 
 from ..utils.constants import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
-from . import custom as TC
+from .custom import image_proc as TC
 from .registry import TRANSFORM_DICT
 
 EDGE_SIZE = 4
 Y_K_SIZE = 6
 X_K_SIZE = 6
 
 
@@ -26,21 +26,31 @@
     # edge_pad == True
     edge = edge[Y_K_SIZE:-Y_K_SIZE, X_K_SIZE:-X_K_SIZE]
     edge = np.pad(edge, ((Y_K_SIZE, Y_K_SIZE), (X_K_SIZE, X_K_SIZE)), mode='constant')
     edge = (cv2.dilate(edge, kernel, iterations=1) > 50) * 1.0
     return Image.fromarray((edge.copy() * 255).astype(np.uint8))
 
 
+def transforms_check(transforms):
+    names = [t.name.lower() for t in transforms]
+    if 'mixing' in names:
+        if names[-1] == 'mixing':
+            return transforms[:-1]
+        else:
+            raise ValueError("Mixing transform is in the middle of transforms. This must be in the last of transforms list.")
+    return transforms
+
+
 def transforms_custom(conf_augmentation, training):
-    assert conf_augmentation.img_size > 32
     phase_conf = conf_augmentation.train if training else conf_augmentation.inference
 
     preprocess = []
-    if phase_conf.transforms:
-        for augment in phase_conf.transforms:
+    if phase_conf:
+        checked_transforms = transforms_check(phase_conf)
+        for augment in checked_transforms:
             name = augment.name.lower()
             augment_kwargs = list(augment.keys())
             augment_kwargs.remove('name')
             augment_kwargs = {k:augment[k] for k in augment_kwargs}
             transform = TRANSFORM_DICT[name](**augment_kwargs)
             preprocess.append(transform)
 
@@ -51,16 +61,17 @@
     return TC.Compose(preprocess)
 
 
 def train_transforms_pidnet(conf_augmentation, training):
     preprocess = []
     phase_conf = conf_augmentation.train if training else conf_augmentation.inference
 
-    if phase_conf.transforms:
-        for augment in phase_conf.transforms:
+    if phase_conf:
+        checked_transforms = transforms_check(phase_conf)
+        for augment in checked_transforms:
             name = augment.name.lower()
             augment_kwargs = list(augment.keys())
             augment_kwargs.remove('name')
             augment_kwargs = {k:augment[k] for k in augment_kwargs}
             transform = TRANSFORM_DICT[name](**augment_kwargs)
             preprocess.append(transform)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/base.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,33 @@
 
     def __init__(self, conf_data, conf_augmentation, model_name, idx_to_class, split, samples, transform, with_label, **kwargs):
         super(BaseCustomDataset, self).__init__()
         self.conf_data = conf_data
         self.conf_augmentation = conf_augmentation
         self.model_name = model_name
 
-        self.transform = transform
+        self.transform = transform(conf_augmentation)
         self.samples = samples
 
         self._root = conf_data.path.root
         self._idx_to_class = idx_to_class
         self._num_classes = len(self._idx_to_class)
         self._split = split
         self._with_label = with_label
 
+        self.cache = False
+
     @abstractmethod
     def __getitem__(self, index):
         pass
 
+    @abstractmethod
+    def cache_dataset(self, sampler, distributed):
+        pass
+
     def __len__(self):
         return len(self.samples)
 
     @property
     def num_classes(self):
         return self._num_classes
 
@@ -48,22 +54,22 @@
     def mode(self):
         return self._split
 
     @property
     def with_label(self):
         return self._with_label
 
-
 class BaseHFDataset(data.Dataset):
 
-    def __init__(self, conf_data, conf_augmentation, model_name, root, split, with_label):
+    def __init__(self, conf_data, conf_augmentation, model_name, root, split, transform, with_label):
         super(BaseHFDataset, self).__init__()
         self.conf_data = conf_data
         self.conf_augmentation = conf_augmentation
         self.model_name = model_name
+        self.transform = transform(conf_augmentation)
         self._root = root
         self._split = split
         self._with_label = with_label
 
     def _load_dataset(self, root, subset_name=None, cache_dir=None):
         from datasets import load_dataset
         if cache_dir is not None:
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/builder.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,18 +36,20 @@
         data_sampler = DATA_SAMPLER[task](conf_data, train_valid_split_ratio=TRAIN_VALID_SPLIT_RATIO)
 
         train_samples, valid_samples, test_samples, misc = data_sampler.load_samples()
         idx_to_class = misc['idx_to_class'] if 'idx_to_class' in misc else None
         label_value_to_idx = misc['label_value_to_idx'] if 'label_value_to_idx' in misc else None
         test_with_label = misc['test_with_label'] if 'test_with_label' in misc else None
 
-        train_dataset = CUSTOM_DATASET[task](
-            conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='train',
-            samples=train_samples, transform=train_transform, label_value_to_idx=label_value_to_idx
-        )
+        train_dataset = None
+        if train_samples is not None:
+            train_dataset = CUSTOM_DATASET[task](
+                conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='train',
+                samples=train_samples, transform=train_transform, label_value_to_idx=label_value_to_idx
+            )
 
         valid_dataset = None
         if valid_samples is not None:
             valid_dataset = CUSTOM_DATASET[task](
                 conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='valid',
                 samples=valid_samples, transform=target_transform, label_value_to_idx=label_value_to_idx
             )
@@ -67,14 +69,15 @@
         data_sampler = DATA_SAMPLER[task](conf_data, train_valid_split_ratio=TRAIN_VALID_SPLIT_RATIO)
 
         train_samples, valid_samples, test_samples, misc = data_sampler.load_huggingface_samples()
         idx_to_class = misc['idx_to_class'] if 'idx_to_class' in misc else None
         label_value_to_idx = misc['label_value_to_idx'] if 'label_value_to_idx' in misc else None
         test_with_label = misc['test_with_label'] if 'test_with_label' in misc else None
 
+        # Assumed hugging face dataset always has training split
         train_dataset = HUGGINGFACE_DATASET[task](
             conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='train',
             huggingface_dataset=train_samples, transform=train_transform, label_value_to_idx=label_value_to_idx
         )
 
         valid_dataset = None
         if valid_samples is not None:
@@ -86,142 +89,117 @@
         test_dataset = None
         if test_samples is not None:
             test_dataset = HUGGINGFACE_DATASET[task](
                 conf_data, conf_augmentation, model_name, idx_to_class=idx_to_class, split='test',
                 huggingface_dataset=test_samples, transform=target_transform, label_value_to_idx=label_value_to_idx
             )
 
-    if not distributed or dist.get_rank() == 0:
-        logger.info(f"Summary | Dataset: <{conf_data.name}> (with {data_format} format)")
-        logger.info(f"Summary | Training dataset: {len(train_dataset)} sample(s)")
-        if valid_dataset is not None:
-            logger.info(f"Summary | Validation dataset: {len(valid_dataset)} sample(s)")
-        if test_dataset is not None:
-            logger.info(f"Summary | Test dataset: {len(test_dataset)} sample(s)")
-
     return train_dataset, valid_dataset, test_dataset
 
 
-def build_dataloader(conf, task: str, model_name: str, train_dataset, eval_dataset, profile=False):
+def build_dataloader(conf, task: str, model_name: str, dataset, phase, profile=False):
+    is_training = phase == 'train'
 
-    if task == 'classification':
-        conf_mix_transform = getattr(conf.augmentation, 'mix_transforms', None)
-        if conf_mix_transform:
-            mix_transforms = []
-            for mix_transform_conf in conf.augmentation.mix_transforms:
-                name = mix_transform_conf.name.lower()
+    #TODO: Temporarily set ``cache_data`` as optional since this is experimental
+    cache_data = conf.environment.cache_data if hasattr(conf.environment, 'cache_data') else False
 
-                mix_kwargs = list(mix_transform_conf.keys())
+    if task == 'classification':
+        # TODO: ``phase`` should be removed later.
+        transforms = getattr(conf.augmentation, phase, None)
+        if transforms:
+            name = transforms[-1].name.lower()
+            if name == 'mixing':
+                mix_kwargs = list(transforms[-1].keys())
                 mix_kwargs.remove('name')
-                mix_kwargs = {k:mix_transform_conf[k] for k in mix_kwargs}
-                mix_kwargs['num_classes'] = train_dataset.num_classes
-
-                transform = TRANSFORM_DICT[name](**mix_kwargs)
-                mix_transforms.append(transform)
-
-            train_collate_fn = partial(classification_mix_collate_fn, mix_transforms=mix_transforms)
-            eval_collate_fn = partial(classification_onehot_collate_fn, num_classes=train_dataset.num_classes)
+                mix_kwargs = {k:transforms[-1][k] for k in mix_kwargs}
+                mix_kwargs['num_classes'] = dataset.num_classes
+                mix_transforms = TRANSFORM_DICT[name](**mix_kwargs)
+
+                collate_fn = partial(classification_mix_collate_fn, mix_transforms=mix_transforms)
+            else:
+                collate_fn = partial(classification_onehot_collate_fn, num_classes=dataset.num_classes)
         else:
-            train_collate_fn = None
-            eval_collate_fn = None
-
-        train_loader = create_loader(
-            train_dataset,
-            conf.data.name,
-            logger,
-            input_size=conf.augmentation.img_size,
-            batch_size=conf.training.batch_size,
-            is_training=True,
-            num_workers=conf.environment.num_workers if not profile else 1,
-            distributed=conf.distributed,
-            collate_fn=train_collate_fn,
-            pin_memory=False,
-            world_size=conf.world_size,
-            rank=conf.rank,
-            kwargs=None
-        )
+            collate_fn = partial(classification_onehot_collate_fn, num_classes=dataset.num_classes)
 
-        eval_loader = create_loader(
-            eval_dataset,
+        dataloader = create_loader(
+            dataset,
             conf.data.name,
             logger,
-            input_size=conf.augmentation.img_size,
-            batch_size=conf.training.batch_size,
-            is_training=False,
+            batch_size=conf.environment.batch_size,
+            is_training=is_training,
             num_workers=conf.environment.num_workers if not profile else 1,
             distributed=conf.distributed,
-            collate_fn=eval_collate_fn,
+            collate_fn=collate_fn,
             pin_memory=False,
             world_size=conf.world_size,
             rank=conf.rank,
+            cache_data=cache_data,
             kwargs=None
         )
     elif task == 'segmentation':
         collate_fn = None
 
-        train_loader = create_loader(
-            train_dataset,
-            conf.data.name,
-            logger,
-            batch_size=conf.training.batch_size,
-            is_training=True,
-            num_workers=conf.environment.num_workers if not profile else 1,
-            distributed=conf.distributed,
-            collate_fn=collate_fn,
-            pin_memory=False,
-            world_size=conf.world_size,
-            rank=conf.rank,
-            kwargs=None
-        )
+        if phase == 'train':
+            batch_size = conf.environment.batch_size
+        else:
+            batch_size = conf.environment.batch_size if model_name == 'pidnet' and not conf.distributed else 1
 
-        eval_loader = create_loader(
-            eval_dataset,
+        dataloader = create_loader(
+            dataset,
             conf.data.name,
             logger,
-            batch_size=conf.training.batch_size if model_name == 'pidnet' and not conf.distributed else 1,
-            is_training=False,
+            batch_size=batch_size,
+            is_training=is_training,
             num_workers=conf.environment.num_workers if not profile else 1,
             distributed=conf.distributed,
-            collate_fn=None,
+            collate_fn=collate_fn,
             pin_memory=False,
             world_size=conf.world_size,
             rank=conf.rank,
+            cache_data=cache_data,
             kwargs=None
         )
     elif task == 'detection':
         collate_fn = detection_collate_fn
 
-        train_loader = create_loader(
-            train_dataset,
+        if phase == 'train':
+            batch_size = conf.environment.batch_size
+        else:
+            batch_size = conf.environment.batch_size if not conf.distributed else 2
+
+        dataloader = create_loader(
+            dataset,
             conf.data.name,
             logger,
-            batch_size=conf.training.batch_size,
-            is_training=True,
+            batch_size=batch_size,
+            is_training=is_training,
             num_workers=conf.environment.num_workers if not profile else 1,
             distributed=conf.distributed,
             collate_fn=collate_fn,
             pin_memory=False,
             world_size=conf.world_size,
             rank=conf.rank,
+            cache_data=cache_data,
             kwargs=None
         )
+    elif task == 'pose_estimation':
+        collate_fn = None
 
-        eval_loader = create_loader(
-            eval_dataset,
+        dataloader = create_loader(
+            dataset,
             conf.data.name,
             logger,
-            # TODO: support batch size 1 inference
-            batch_size=conf.training.batch_size if not conf.distributed else 2,
-            is_training=False,
+            batch_size=conf.environment.batch_size,
+            is_training=is_training,
             num_workers=conf.environment.num_workers if not profile else 1,
             distributed=conf.distributed,
             collate_fn=collate_fn,
             pin_memory=False,
             world_size=conf.world_size,
             rank=conf.rank,
+            cache_data=cache_data,
             kwargs=None
         )
-
     else:
         raise AssertionError(f"Task ({task}) is not understood!")
 
-    return train_loader, eval_loader
+    return dataloader
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/classification/huggingface.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/classification/huggingface.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,19 @@
         root = conf_data.metadata.repo
         super(ClassificationHFDataset, self).__init__(
             conf_data,
             conf_augmentation,
             model_name,
             root,
             split,
+            transform,
             with_label
         )
         # Make sure that you additionally install `requirements-data.txt`
 
-        self.transform = transform
-
         self.samples = huggingface_dataset
         self.idx_to_class = idx_to_class
         self.class_to_idx = {v: k for k, v in self.idx_to_class.items()}
 
         self.image_feature_name = conf_data.metadata.features.image
         self.label_feature_name = conf_data.metadata.features.label
 
@@ -54,11 +53,11 @@
     def __getitem__(self, index):
         img: Image.Image = self.samples[index][self.image_feature_name]
         target: Union[int, str] = self.samples[index][self.label_feature_name] if self.label_feature_name in self.samples[index] else None
         if isinstance(target, str):
             target: int = self.class_to_idx[target]
 
         if self.transform is not None:
-            out = self.transform(conf_augmentation=self.conf_augmentation)(img)
+            out = self.transform(img)
         if target is None:
             target = -1
-        return out['image'], target
+        return index, out['image'], target
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/detection/dataset.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/pose_estimation/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,98 +15,72 @@
 from ..utils.misc import natural_key
 
 
 def load_custom_class_map(id_mapping: List[str]):
     idx_to_class: Dict[int, str] = dict(enumerate(id_mapping))
     return idx_to_class
 
-def detection_collate_fn(original_batch):
-    pixel_values = []
-    bbox = []
-    label = []
-    org_shape = []
-    for data_sample in original_batch:
-        if 'pixel_values' in data_sample:
-            pixel_values.append(data_sample['pixel_values'])
-        if 'bbox' in data_sample:
-            bbox.append(data_sample['bbox'])
-        if 'label' in data_sample:
-            label.append(data_sample['label'])
-        if 'org_shape' in data_sample:
-            org_shape.append(data_sample['org_shape'])
-    outputs = {}
-    if len(pixel_values) != 0:
-        pixel_values = torch.stack(pixel_values, dim=0)
-        outputs.update({'pixel_values': pixel_values})
-    if len(bbox) != 0:
-        outputs.update({'bbox': bbox})
-    if len(label) != 0:
-        outputs.update({'label': label})
-    if len(org_shape) != 0:
-        outputs.update({'org_shape': org_shape})
 
-    return outputs
-
-class DetectionDataSampler(BaseDataSampler):
+class PoseEstimationDataSampler(BaseDataSampler):
     def __init__(self, conf_data, train_valid_split_ratio):
-        super(DetectionDataSampler, self).__init__(conf_data, train_valid_split_ratio)
+        super(PoseEstimationDataSampler, self).__init__(conf_data, train_valid_split_ratio)
 
     def load_data(self, split='train'):
+        assert split in ['train', 'valid', 'test'], f"split should be either {['train', 'valid', 'test']}."
         data_root = Path(self.conf_data.path.root)
         split_dir = self.conf_data.path[split]
         image_dir: Path = data_root / split_dir.image
-        annotation_dir: Path = data_root / split_dir.label
+        annotation_dir: Optional[Path] = data_root / split_dir.label if split_dir.label is not None else None
         images: List[str] = []
         labels: List[str] = []
         images_and_targets: List[Dict[str, str]] = []
-        if split in ['train', 'valid']:
+        if annotation_dir is not None:
             for ext in IMG_EXTENSIONS:
                 for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}')):
                     ann_path_maybe = annotation_dir / file.with_suffix('.txt').name
                     if not ann_path_maybe.exists():
                         continue
                     images.append(str(file))
                     labels.append(str(ann_path_maybe))
                 # TODO: get paired data from regex pattern matching (self.conf_data.path.pattern)
 
             images = sorted(images, key=lambda k: natural_key(k))
             labels = sorted(labels, key=lambda k: natural_key(k))
             images_and_targets.extend([{'image': str(image), 'label': str(label)} for image, label in zip(images, labels)])
 
-        elif split == 'test':
+        else:
             for ext in IMG_EXTENSIONS:
                 images_and_targets.extend([{'image': str(file), 'label': None}
                                         for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}'))])
             images_and_targets = sorted(images_and_targets, key=lambda k: natural_key(k['image']))
-        else:
-            raise AssertionError(f"split should be either {['train', 'valid', 'test']}")
 
         return images_and_targets
 
     def load_samples(self):
-        assert self.conf_data.path.train.image is not None
         assert self.conf_data.id_mapping is not None
         id_mapping: Optional[list] = list(self.conf_data.id_mapping)
         idx_to_class = load_custom_class_map(id_mapping=id_mapping)
 
+        exists_train = self.conf_data.path.train.image is not None
         exists_valid = self.conf_data.path.valid.image is not None
         exists_test = self.conf_data.path.test.image is not None
 
+        train_samples = None
         valid_samples = None
         test_samples = None
 
-        train_samples = self.load_data(split='train')
+        if exists_train:
+            train_samples = self.load_data(split='train')
         if exists_valid:
             valid_samples = self.load_data(split='valid')
         if exists_test:
             test_samples = self.load_data(split='test')
 
         if not exists_valid:
             num_train_splitted = int(len(train_samples) * self.train_valid_split_ratio)
-            train_samples, valid_samples = \
-                random_split(train_samples, [num_train_splitted, len(train_samples) - num_train_splitted],
-                                generator=torch.Generator().manual_seed(42))
+            train_samples, valid_samples = random_split(train_samples, [num_train_splitted, len(train_samples) - num_train_splitted],
+                                                        generator=torch.Generator().manual_seed(42))
 
         return train_samples, valid_samples, test_samples, {'idx_to_class': idx_to_class}
 
     def load_huggingface_samples(self):
         raise NotImplementedError
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/registry.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,31 +4,37 @@
 from .base import BaseCustomDataset, BaseDataSampler, BaseHFDataset
 from .classification import (
     ClassficationDataSampler,
     ClassificationCustomDataset,
     ClassificationHFDataset,
 )
 from .detection import DetectionCustomDataset, DetectionDataSampler
+from .pose_estimation import (
+    PoseEstimationCustomDataset,
+    PoseEstimationDataSampler,
+)
 from .segmentation import (
     SegmentationCustomDataset,
     SegmentationDataSampler,
     SegmentationHFDataset,
 )
 
 CREATE_TRANSFORM = create_transform
 
 CUSTOM_DATASET: Dict[str, Type[BaseCustomDataset]] = {
     'classification': ClassificationCustomDataset,
     'segmentation': SegmentationCustomDataset,
-    'detection': DetectionCustomDataset
+    'detection': DetectionCustomDataset,
+    'pose_estimation': PoseEstimationCustomDataset,
 }
 
 HUGGINGFACE_DATASET: Dict[str, Type[BaseHFDataset]] = {
     'classification': ClassificationHFDataset,
     'segmentation': SegmentationHFDataset
 }
 
 DATA_SAMPLER: Dict[str, Type[BaseDataSampler]] = {
     'classification': ClassficationDataSampler,
     'segmentation': SegmentationDataSampler,
-    'detection': DetectionDataSampler
+    'detection': DetectionDataSampler,
+    'pose_estimation': PoseEstimationDataSampler,
 }
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/dataset.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,54 +48,55 @@
 
 
 class SegmentationDataSampler(BaseDataSampler):
     def __init__(self, conf_data, train_valid_split_ratio):
         super(SegmentationDataSampler, self).__init__(conf_data, train_valid_split_ratio)
 
     def load_data(self, split='train'):
+        assert split in ['train', 'valid', 'test'], f"split should be either {['train', 'valid', 'test']}."
         data_root = Path(self.conf_data.path.root)
         split_dir = self.conf_data.path[split]
         image_dir: Path = data_root / split_dir.image
-        annotation_dir: Path = data_root / split_dir.label
+        annotation_dir: Optional[Path] = data_root / split_dir.label if split_dir.label is not None else None
         images: List[str] = []
         labels: List[str] = []
         images_and_targets: List[Dict[str, str]] = []
-        if split in ['train', 'valid']:
+        if annotation_dir is not None:
             for ext in IMG_EXTENSIONS:
                 images.extend([str(file) for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}'))])
                 # TODO: get paired data from regex pattern matching (conf_data.path.pattern)
                 labels.extend([str(file) for file in chain(annotation_dir.glob(f'*{ext}'), annotation_dir.glob(f'*{ext.upper()}'))])
 
             images = sorted(images, key=lambda k: natural_key(k))
             labels = sorted(labels, key=lambda k: natural_key(k))
             images_and_targets.extend([{'image': str(image), 'label': str(label)} for image, label in zip(images, labels)])
 
-        elif split == 'test':
+        else:
             for ext in IMG_EXTENSIONS:
                 images_and_targets.extend([{'image': str(file), 'label': None}
                                            for file in chain(image_dir.glob(f'*{ext}'), image_dir.glob(f'*{ext.upper()}'))])
             images_and_targets = sorted(images_and_targets, key=lambda k: natural_key(k['image']))
-        else:
-            raise AssertionError(f"split should be either {['train', 'valid', 'test']}")
 
         return images_and_targets
 
     def load_samples(self):
-        assert self.conf_data.path.train.image is not None
         assert isinstance(self.conf_data.id_mapping, (ListConfig, DictConfig))
 
         idx_to_class, label_value_to_idx = load_custom_class_map(id_mapping=self.conf_data.id_mapping)
 
+        exists_train = self.conf_data.path.train.image is not None
         exists_valid = self.conf_data.path.valid.image is not None
         exists_test = self.conf_data.path.test.image is not None
 
+        train_samples = None
         valid_samples = None
         test_samples = None
 
-        train_samples = self.load_data(split='train')
+        if exists_train:
+            train_samples = self.load_data(split='train')
         if exists_valid:
             valid_samples = self.load_data(split='valid')
         if exists_test:
             test_samples = self.load_data(split='test')
 
         if not exists_valid:
             num_train_splitted = int(len(train_samples) * self.train_valid_split_ratio)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/huggingface.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/huggingface.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         root = conf_data.metadata.repo
         super(SegmentationHFDataset, self).__init__(
             conf_data,
             conf_augmentation,
             model_name,
             root,
             split,
+            transform,
             with_label
         )
 
-        self.transform = transform
         self.idx_to_class = idx_to_class
         self.samples = huggingface_dataset
 
         assert "label_value_to_idx" in kwargs
         self.label_value_to_idx = kwargs["label_value_to_idx"]
 
         self.label_image_mode: Literal['RGB', 'L', 'P'] = str(conf_data.label_image_mode).upper() \
@@ -68,31 +68,31 @@
 
         mask = np.zeros((label.size[1], label.size[0]), dtype=np.uint8)
         for label_value in self.label_value_to_idx:
             class_mask = (label_array == np.array(label_value)).all(axis=-1)
             mask[class_mask] = self.label_value_to_idx[label_value]
         mask = Image.fromarray(mask, mode='L')  # single mode array (PIL.Image) compatbile with torchvision transform API
 
-        org_img = img.copy()
         w, h = img.size
 
         if label is None:
-            out = self.transform(self.conf_augmentation)(image=img)
-            return {'pixel_values': out['image'], 'name': img_name, 'org_img': org_img, 'org_shape': (h, w)}
+            out = self.transform(image=img)
+            return {'pixel_values': out['image'], 'name': img_name, 'org_shape': (h, w)}
 
         outputs = {}
 
         if self.model_name == 'pidnet':
             edge = generate_edge(np.array(label))
-            out = self.transform(self.conf_augmentation)(image=img, mask=mask, edge=edge)
+            out = self.transform(image=img, mask=mask, edge=edge)
             outputs.update({'pixel_values': out['image'], 'labels': out['mask'], 'edges': out['edge'].float(), 'name': img_name})
         else:
-            out = self.transform(self.conf_augmentation)(image=img, mask=mask)
+            out = self.transform(image=img, mask=mask)
             outputs.update({'pixel_values': out['image'], 'labels': out['mask'], 'name': img_name})
 
+        outputs.update({'indices': index})
         if self._split in ['train', 'training']:
             return outputs
 
         assert self._split in ['val', 'valid', 'test']
         # outputs.update({'org_img': org_img, 'org_shape': (h, w)})  # TODO: return org_img with batch_size > 1
         outputs.update({'org_shape': (h, w)})
         return outputs
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/segmentation/local.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/segmentation/local.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import os
+from functools import partial
+from multiprocessing.pool import ThreadPool
 from pathlib import Path
 from typing import Literal
 
 import numpy as np
 import PIL.Image as Image
+import torch.distributed as dist
+from loguru import logger
 
 from ..augmentation.transforms import generate_edge, reduce_label
 from ..base import BaseCustomDataset
 
 
 class SegmentationCustomDataset(BaseCustomDataset):
 
@@ -19,49 +23,75 @@
         )
         assert "label_value_to_idx" in kwargs
         self.label_value_to_idx = kwargs["label_value_to_idx"]
 
         self.label_image_mode: Literal['RGB', 'L', 'P'] = str(conf_data.label_image_mode).upper() \
             if conf_data.label_image_mode is not None else 'L'
 
-    def __getitem__(self, index):
-        img_path = Path(self.samples[index]['image'])
-        ann_path = Path(self.samples[index]['label']) if 'label' in self.samples[index] else None
-        img = Image.open(img_path).convert('RGB')
+    def cache_dataset(self, sampler, distributed):
+        if (not distributed) or (distributed and dist.get_rank() == 0):
+            logger.info(f'Caching | Loading samples of {self.mode} to memory... This can take minutes.')
+
+        def _load(i, samples):
+            image = Image.open(Path(samples[i]['image'])).convert('RGB')
+            label = self.samples[i]['label']
+            if label is not None:
+                label = Image.open(Path(label)).convert(self.label_image_mode)
+            return i, image, label
+
+        num_threads = 8 # TODO: Compute appropriate num_threads
+        load_imgs = ThreadPool(num_threads).imap(
+            partial(_load, samples=self.samples),
+            sampler
+        )
+        for i, image, label in load_imgs:
+            self.samples[i]['image'] = image
+            self.samples[i]['label'] = label
 
-        org_img = img.copy()
+        self.cache = True
 
-        w, h = img.size
+    def __getitem__(self, index):
+        if self.cache:
+            img = self.samples[index]['image']
+            label = self.samples[index]['label']
+        else:
+            img_path = self.samples[index]['image']
+            ann_path = self.samples[index]['label']
+            img = Image.open(Path(img_path)).convert('RGB')
+            label = Image.open(Path(ann_path)).convert(self.label_image_mode) if ann_path is not None else None
 
-        if ann_path is None:
-            out = self.transform(self.conf_augmentation)(image=img)
-            return {'pixel_values': out['image'], 'name': img_path.name, 'org_img': org_img, 'org_shape': (h, w)}
+        w, h = img.size
 
         outputs = {}
+        outputs.update({'indices': index})
+        if label is None:
+            out = self.transform(image=img)
+            outputs.update({'pixel_values': out['image'], 'org_shape': (h, w)})
+            return outputs
+
 
-        label = Image.open(ann_path).convert(self.label_image_mode)
         label_array = np.array(label)
         label_array = label_array[..., np.newaxis] if label_array.ndim == 2 else label_array
         # if self.conf_augmentation.reduce_zero_label:
         #     label = reduce_label(np.array(label))
 
         mask = np.zeros((label.size[1], label.size[0]), dtype=np.uint8)
         for label_value in self.label_value_to_idx:
             class_mask = (label_array == np.array(label_value)).all(axis=-1)
             mask[class_mask] = self.label_value_to_idx[label_value]
 
         mask = Image.fromarray(mask, mode='L')  # single mode array (PIL.Image) compatbile with torchvision transform API
 
         if 'pidnet' in self.model_name:
             edge = generate_edge(np.array(mask))
-            out = self.transform(self.conf_augmentation)(image=img, mask=mask, edge=edge)
-            outputs.update({'pixel_values': out['image'], 'labels': out['mask'], 'edges': out['edge'].float(), 'name': img_path.name})
+            out = self.transform(image=img, mask=mask, edge=edge)
+            outputs.update({'pixel_values': out['image'], 'labels': out['mask'], 'edges': out['edge'].float()})
         else:
-            out = self.transform(self.conf_augmentation)(image=img, mask=mask)
-            outputs.update({'pixel_values': out['image'], 'labels': out['mask'], 'name': img_path.name})
+            out = self.transform(image=img, mask=mask)
+            outputs.update({'pixel_values': out['image'], 'labels': out['mask']})
 
         if self._split in ['train', 'training']:
             return outputs
 
         assert self._split in ['val', 'valid', 'test']
         # outputs.update({'org_img': org_img, 'org_shape': (h, w)})  # TODO: return org_img with batch_size > 1
         outputs.update({'org_shape': (h, w)})
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/utils/loader.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .constants import IMAGENET_DEFAULT_MEAN, IMAGENET_DEFAULT_STD
 from .misc import expand_to_chs
+from .sampler import DistributedEvalSampler
 
 NUM_RGB_CHANNEL = 3
 
 
 def fast_collate(batch):
     """ A fast collation function optimized for uint8 images (np array or torch) and int64 targets (labels)"""
     assert isinstance(batch[0], tuple)
@@ -63,15 +64,14 @@
             np.random.seed(worker_info.seed % (2 ** 32 - 1))
 
 
 def create_loader(
         dataset,
         dataset_name,
         logger,
-        input_size=None,
         batch_size=1,
         is_training=False,
         num_aug_repeats=0,
         num_aug_splits=0,
         num_workers=1,
         distributed=False,
         collate_fn=None,
@@ -79,18 +79,24 @@
         fp16=False,
         tf_preprocessing=False,
         use_multi_epochs_loader=False,
         persistent_workers=True,
         worker_seeding='all',
         world_size=1,
         rank=0,
+        cache_data=False,
         kwargs=None
 ):
+    if is_training:
+        sampler = torch.utils.data.distributed.DistributedSampler(dataset, num_replicas=world_size, rank=rank, drop_last=True)
+    else:
+        sampler = DistributedEvalSampler(dataset, num_replicas=world_size, rank=rank)
 
-    sampler = torch.utils.data.distributed.DistributedSampler(dataset, num_replicas=world_size, rank=rank)
+    if cache_data:
+        dataset.cache_dataset(sampler, distributed)
 
     loader_args = {
         'batch_size': batch_size,
         'shuffle': not isinstance(dataset, torch.utils.data.IterableDataset) and sampler is None and is_training,
         'num_workers': num_workers,
         'sampler': sampler,
         'collate_fn': collate_fn,
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/dataloaders/utils/misc.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/dataloaders/utils/misc.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/builder.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 
 import numpy as np
 import PIL.Image as Image
 import torch
 from omegaconf import OmegaConf
 
 from ..utils.record import AverageMeter
-from .base import BaseCSVLogger
 from .image import ImageSaver
-from .registry import CSV_LOGGER, VISUALIZER
+from .registry import VISUALIZER
 from .stdout import StdOutLogger
 from .tensorboard import TensorboardLogger
 from .visualizer import magic_image_handler
 
-START_EPOCH_ZERO_OR_ONE = 1
 
 class TrainingLogger():
     def __init__(
         self,
         conf,
         task: Literal['classification', 'segmentation', 'detection'],
         model: str,
@@ -38,54 +36,40 @@
 
         self.project_id = conf.logging.project_id if conf.logging.project_id is not None else f"{self.task}_{self.model}"
 
         self._result_dir = result_dir
         OmegaConf.save(config=self.conf, f=(result_dir / "hparams.yaml"))
 
         self.use_tensorboard: bool = self.conf.logging.tensorboard
-        self.use_csvlogger: bool = self.conf.logging.csv
         self.use_imagesaver: bool = self.conf.logging.image
         self.use_stdout: bool = self.conf.logging.stdout
-        self.use_netspresso: bool = False  # TODO: NetsPresso training board
 
-        self.csv_logger: Optional[BaseCSVLogger] = \
-            CSV_LOGGER[task](model=model, result_dir=self._result_dir) if self.use_csvlogger else None
-        self.image_saver: Optional[ImageSaver] = \
-            ImageSaver(model=model, result_dir=self._result_dir) if self.use_imagesaver else None
-        self.tensorboard_logger: Optional[TensorboardLogger] = \
-            TensorboardLogger(task=task, model=model, result_dir=self._result_dir,
-                              step_per_epoch=step_per_epoch, num_sample_images=num_sample_images) if self.use_tensorboard else None
-        self.stdout_logger: Optional[StdOutLogger] = \
-            StdOutLogger(task=task, model=model, total_epochs=conf.training.epochs, result_dir=self._result_dir) if self.use_stdout else None
-
-        self.netspresso_api_client = None
-        if self.use_netspresso:
-            from loggers.netspresso import ModelSearchServerHandler
-            self.netspresso_api_client: Optional[ModelSearchServerHandler] = ModelSearchServerHandler(task=task, model=model)
+        self.loggers = []
+        if self.use_imagesaver:
+            self.loggers.append(ImageSaver(model=model, result_dir=self._result_dir))
+        if self.use_tensorboard:
+            self.tensorboard_logger = TensorboardLogger(task=task, model=model, result_dir=self._result_dir,
+                                                        step_per_epoch=step_per_epoch, num_sample_images=num_sample_images)
+            self.loggers.append(self.tensorboard_logger)
+        if self.use_stdout:
+            total_epochs = conf.training.epochs if hasattr(conf, 'training') else None
+            self.loggers.append(StdOutLogger(task=task, model=model, total_epochs=total_epochs, result_dir=self._result_dir))
 
         if task in VISUALIZER:
             pallete = conf.data.pallete if 'pallete' in conf.data else None
             self.label_converter = VISUALIZER[task](class_map=class_map, pallete=pallete)
 
     @property
     def result_dir(self):
         return self._result_dir
 
     def update_epoch(self, epoch: int):
         self.epoch = epoch
-        if self.use_csvlogger:
-            self.csv_logger.epoch = self.epoch
-        if self.use_imagesaver:
-            self.image_saver.epoch = self.epoch
-        if self.use_tensorboard:
-            self.tensorboard_logger.epoch = self.epoch
-        if self.use_stdout:
-            self.stdout_logger.epoch = self.epoch
-        if self.use_netspresso:
-            self.netspresso_api_client.epoch = self.epoch
+        for logger in self.loggers:
+            logger.epoch = self.epoch
 
     @staticmethod
     def _to_numpy(tensor: torch.Tensor):
         return tensor.detach().cpu().numpy()
 
     def _convert_scalar_as_readable(self, scalar_dict: Dict):
         for k, v in scalar_dict.items():
@@ -141,80 +125,43 @@
         if isinstance(images_dict_or_list, dict):
             images_dict = images_dict_or_list
             images_dict = self._convert_imagedict_as_readable(images_dict)
             return images_dict
 
         raise TypeError(f"Unsupported type for image logger!!! Current type: {type(images_dict_or_list)}")
 
-    def log(self, train_losses, train_metrics, valid_losses=None, valid_metrics=None,
-            train_images=None, valid_images=None, learning_rate=None, elapsed_time=None):
-        train_losses = self._convert_scalar_as_readable(train_losses)
-        train_metrics = self._convert_scalar_as_readable(train_metrics)
-
-        if valid_losses is not None:
-            valid_losses = self._convert_scalar_as_readable(valid_losses)
-        if valid_metrics is not None:
-            valid_metrics = self._convert_scalar_as_readable(valid_metrics)
-        if train_images is not None:
-            train_images = self._convert_images_as_readable(train_images)
-        if valid_images is not None:
-            valid_images = self._convert_images_as_readable(valid_images)
-
-        if self.use_csvlogger:
-            self.csv_logger(
-                train_losses=train_losses,
-                train_metrics=train_metrics,
-                valid_losses=valid_losses,
-                valid_metrics=valid_metrics
-            )
-        if self.use_imagesaver:
-            self.image_saver(
-                train_images=train_images,
-                valid_images=valid_images
-            )
-        if self.use_tensorboard:
-            self.tensorboard_logger(
-                train_losses=train_losses,
-                train_metrics=train_metrics,
-                valid_losses=valid_losses,
-                valid_metrics=valid_metrics,
-                train_images=train_images,
-                valid_images=valid_images,
-                learning_rate=learning_rate,
-                elapsed_time=elapsed_time
-            )
-        if self.use_stdout:
-            self.stdout_logger(
-                train_losses=train_losses,
-                train_metrics=train_metrics,
-                valid_losses=valid_losses,
-                valid_metrics=valid_metrics,
-                learning_rate=learning_rate,
-                elapsed_time=elapsed_time
-            )
-        if self.use_netspresso:
-            # TODO: async handler if it takes much more time
-            self.netspresso_api_client(
-                train_losses=train_losses,
-                train_metrics=train_metrics,
-                valid_losses=valid_losses,
-                valid_metrics=valid_metrics,
+    def log(
+        self,
+        prefix: Literal['training', 'validation', 'evaluation', 'inference'],
+        epoch: Optional[int] = None,
+        samples: Optional[List] = None,
+        losses : Optional[Dict] = None,
+        metrics: Optional[Dict] = None,
+        learning_rate: Optional[float] = None,
+        elapsed_time: Optional[float] = None,
+    ):
+        if not self.use_imagesaver: # TODO: This is uneffective way
+            samples = None
+
+        if losses is not None:
+            losses = self._convert_scalar_as_readable(losses)
+        if metrics is not None:
+            metrics = self._convert_scalar_as_readable(metrics)
+        if samples is not None:
+            samples = self._convert_images_as_readable(samples)
+
+        for logger in self.loggers:
+            logger(
+                prefix=prefix,
+                epoch=epoch,
+                losses=losses,
+                metrics=metrics,
+                images=samples,
                 learning_rate=learning_rate,
                 elapsed_time=elapsed_time
             )
 
     def log_end_of_traning(self, final_metrics=None):
         if final_metrics is None:
             final_metrics = {}
         if self.use_tensorboard:
             self.tensorboard_logger.log_hparams(self.conf, final_metrics=final_metrics)
-
-
-def build_logger(conf, task: str, model_name: str, step_per_epoch: int, class_map: Dict[int, str], num_sample_images: int, result_dir: Union[Path, str], epoch: Optional[int] = None):
-    training_logger = TrainingLogger(conf,
-                                     task=task, model=model_name,
-                                     step_per_epoch=step_per_epoch,
-                                     class_map=class_map, num_sample_images=num_sample_images,
-                                     result_dir=result_dir,
-                                     epoch=epoch)
-
-    return training_logger
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/image.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,51 +7,44 @@
 
 class ImageSaver:
     def __init__(self, model, result_dir) -> None:
         super(ImageSaver, self).__init__()
         self.model = model
         self.save_dir: Path = Path(result_dir) / "result_image"
         self.save_dir.mkdir(exist_ok=True)
-        self._epoch = None
-
-    def init_epoch(self):
-        self._epoch = 0
-
-    @property
-    def epoch(self):
-        return self._epoch
-
-    @epoch.setter
-    def epoch(self, value: int) -> None:
-        self._epoch = int(value)
 
     def save_ndarray_as_image(self, image_array: np.ndarray, filename: Union[str, Path], dataformats: Literal['HWC', 'CHW'] = 'HWC'):
         assert image_array.ndim == 3
         if dataformats != 'HWC' and dataformats == 'CHW':
             image_array = image_array.transpose((1, 2, 0))
 
         # HWC
         assert image_array.shape[-1] in [1, 3]
         Image.fromarray(image_array.astype(np.uint8)).save(filename)
         return True
 
-    def save_result(self, image_dict: Dict, prefix='train'):
+    def save_result(self, image_dict: Dict, prefix, epoch):
         prefix_dir: Path = self.save_dir / prefix
         prefix_dir.mkdir(exist_ok=True)
 
         for k, v in image_dict.items():
             assert isinstance(v, np.ndarray)
             assert v.ndim in [3, 4], \
                 f"Array for saving as image should have dim of 3 or 4! Current: {v.ndim}"
             if v.ndim == 3:
-                self.save_ndarray_as_image(v, f"{prefix_dir}/{self._epoch:04d}_{k}.png", dataformats='HWC')
+                self.save_ndarray_as_image(v, f"{prefix_dir}/{epoch:04d}_{k}.png", dataformats='HWC')
             for idx, image in enumerate(v):
-                filename = f"{prefix_dir}/{self._epoch:04d}_{idx:03d}_{k}.png"
+                if epoch is None:
+                    filename = f"{prefix_dir}/{idx:03d}_{k}.png"
+                else:
+                    filename = f"{prefix_dir}/{epoch:04d}_{idx:03d}_{k}.png"
                 self.save_ndarray_as_image(image, filename, dataformats='HWC') # TODO: get dataformats option from outside
 
-    def __call__(self, train_images=None, valid_images=None):
-        if train_images is not None:
-            self.save_result(train_images, prefix='train')
-        if valid_images is not None:
-            self.save_result(valid_images, prefix='valid')
-
-
+    def __call__(
+        self,
+        prefix: Literal['training', 'validation', 'evaluation', 'inference'],
+        epoch: Optional[int] = None,
+        images: Optional[List] = None,
+        **kwargs
+    ):
+        if images is not None:
+            self.save_result(images, prefix=prefix, epoch=epoch)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/tensorboard.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/tensorboard.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from omegaconf import OmegaConf
 from torch.utils.tensorboard import SummaryWriter
 from torch.utils.tensorboard.summary import hparams
 
@@ -17,26 +17,14 @@
 
         self.result_dir = Path(result_dir)
         self.result_dir.mkdir(exist_ok=True)
         self.step_per_epoch = step_per_epoch
         self.num_sample_images = num_sample_images
 
         self.tensorboard = SummaryWriter(self.result_dir / "tensorboard")
-        self._epoch = None
-
-    def init_epoch(self):
-        self._epoch = 0
-
-    @property
-    def epoch(self):
-        return self._epoch
-
-    @epoch.setter
-    def epoch(self, value: int) -> None:
-        self._epoch = int(value)
 
     def _as_numpy(self, value: Union[np.ndarray, torch.Tensor]) -> np.ndarray:
         if isinstance(value, np.ndarray):
             return value
         if isinstance(value, torch.Tensor):
             value = value.detach()
             value = value.cpu() if value.is_cuda else value
@@ -101,30 +89,32 @@
         exp, ssi, sei = hparams(hparam_dict=hp_for_log, metric_dict=final_metrics)
         self.tensorboard.file_writer.add_summary(exp)
         self.tensorboard.file_writer.add_summary(ssi)
         self.tensorboard.file_writer.add_summary(sei)
         for k, v in final_metrics.items():
             self.tensorboard.add_scalar(k, v)
 
-    def __call__(self,
-                 train_losses, train_metrics, valid_losses, valid_metrics,
-                 train_images, valid_images, learning_rate, elapsed_time,
-                 ) -> None:
-
-        self.log_scalars_with_dict(train_losses, mode='train')
-        self.log_scalars_with_dict(train_metrics, mode='train')
-        if train_images is not None:
-            self.log_images_with_dict(train_images, mode='train')
-
-        if valid_losses is not None:
-            self.log_scalars_with_dict(valid_losses, mode='valid')
-        if valid_metrics is not None:
-            self.log_scalars_with_dict(valid_metrics, mode='valid')
-        if isinstance(valid_images, dict):  # TODO: array with multiple dicts
-            self.log_images_with_dict(valid_images, mode='valid')
+    def __call__(
+        self,
+        prefix: Literal['training', 'validation', 'evaluation', 'inference'],
+        epoch: Optional[int] = None,
+        images: Optional[List] = None,
+        losses : Optional[Dict] = None,
+        metrics: Optional[Dict] = None,
+        learning_rate: Optional[float] = None,
+        elapsed_time: Optional[float] = None,
+        **kwargs
+    ):
+        self._epoch = 0 if epoch is None else epoch
+        if losses is not None:
+            self.log_scalars_with_dict(losses, mode=prefix)
+        if metrics is not None:
+            self.log_scalars_with_dict(metrics, mode=prefix)
+        if isinstance(images, dict):  # TODO: array with multiple dicts
+            self.log_images_with_dict(images, mode=prefix)
 
         if learning_rate is not None:
             self.log_scalar('learning_rate', learning_rate, mode='misc')
         if elapsed_time is not None:
             self.log_scalar('elapsed_time', elapsed_time, mode='misc')
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/loggers/visualizer.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/loggers/visualizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,37 @@
             c = c >> 3
 
         cmap[i] = np.array([r, g, b])
 
     cmap = cmap / 255 if normalized else cmap
     return cmap
 
+
+class ClassificationVisualizer:
+    def __init__(self, class_map, pallete=None) -> None:
+        self.n = len(class_map)
+        self.class_map = class_map
+
+    def __call__(self, results: List[Tuple[np.ndarray, np.ndarray]], images=None):
+        return_images = []
+        for image, label in zip(images, results):
+            image = image.copy()
+            class_name = self.class_map[label[0]] # Class is determined with top1 score
+
+            x1, y1 = 0, 0
+            text_size, _ = cv2.getTextSize(str(class_name), cv2.FONT_HERSHEY_SIMPLEX, 0.5, 1)
+            text_w, text_h = text_size
+            image = cv2.rectangle(image, (x1, y1), (x1+text_w, y1+text_h+5), color=(0, 0, 255), thickness=-1)
+            image = cv2.putText(image, str(class_name), (x1, y1+text_h), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255, 255, 255), 1)
+
+            return_images.append(image[np.newaxis, ...])
+        return_images = np.concatenate(return_images, axis=0)
+        return return_images
+
+
 class DetectionVisualizer:
     def __init__(self, class_map, pallete=None):
         n = len(class_map)
         if pallete is None:
             self.cmap = _voc_color_map(n)
         else:
             self.cmap = np.array(pallete[:n], dtype=np.uint8)
@@ -116,14 +139,32 @@
             return np.concatenate(result_images, axis=0)
         elif len(results.shape) == 2:
             return self._convert(results)
         else:
             raise IndexError(f"gray_image.shape should be either 2 or 3, but {results.shape} were indexed.")
 
 
+class PoseEstimationVisualizer:
+    def __init__(self, class_map, pallete=None):
+        len(class_map)
+
+    def __call__(self, results, images=None):
+        return_images = []
+        for image, result in zip(images, results):
+            image = image.copy()
+            for keypoint in result:
+                x = round(keypoint[0])
+                y = round(keypoint[1])
+                image = cv2.line(image, (x, y), (x, y), color=(0, 0, 255), thickness=5)
+
+            return_images.append(image[np.newaxis, ...])
+        return_images = np.concatenate(return_images, axis=0)
+        return return_images
+
+
 def _as_image_array(img: np.ndarray):
     min_, max_ = np.amin(img), np.amax(img)
     is_int_array = img.dtype in [np.uint8, np.uint16, np.int8, np.int16, np.int32, np.int64]
     try_uint8 = (min_ >= 0 and max_ <= 255)
 
     if is_int_array and try_uint8:
         img = img.astype(np.uint8)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/losses/builder.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
 class LossFactory:
     def __init__(self, conf_model, **kwargs) -> None:
         self.loss_func_dict = {}
         self.loss_weight_dict = {}
 
         self.conf_model = conf_model
-        self._build_losses()
+        self._build_losses(**kwargs)
 
         self._dirty_backward: bool = False
         self.loss_val_per_epoch: Dict[str, Dict[str, AverageMeter]] = {}
         self._clear_epoch_start()
 
-    def _build_losses(self):
+    def _build_losses(self, **kwargs):
 
         for loss_element in self.conf_model.losses:
             criterion = loss_element.criterion
             loss_config = {k: v for k, v in loss_element.items() if k not in ['criterion', 'weight']}
-            loss = LOSS_DICT[criterion](**loss_config)
+            loss = LOSS_DICT[criterion](**loss_config, **kwargs)
 
             self.loss_func_dict.update({criterion: loss})
             loss_weight = loss_element.weight if loss_element.weight is not None else 1.0
             self.loss_weight_dict.update({criterion: loss_weight})
 
     def _clear_step_start(self):
         self.total_loss_for_backward: Union[int, torch.Tensor] = 0
@@ -43,18 +43,18 @@
             for phase in PHASE_LIST
         }
         self._clear_step_start()
 
     def _assert_argument(self, kwargs):
         pass
 
-    def backward(self):
+    def backward(self, grad_scaler: torch.cuda.amp.GradScaler):
         assert not self._dirty_backward
         self.total_loss_for_backward.requires_grad_(True)
-        self.total_loss_for_backward.mean().backward()
+        grad_scaler.scale(self.total_loss_for_backward.mean()).backward()
         self._dirty_backward = True
 
     def result(self, phase='train'):
         phase = phase.lower()
         return self.loss_val_per_epoch[phase]
 
     def reset_values(self):
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/losses/common.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 
 
 class CrossEntropyLoss(nn.Module):
     def __init__(self, weight: Optional[Tensor]=None, size_average=None, ignore_index: int=-100,
-                 reduce=None, label_smoothing: float=0.0):
+                 reduce=None, label_smoothing: float=0.0, **kwargs):
         super(CrossEntropyLoss, self).__init__()
         self.loss_fn = nn.CrossEntropyLoss(weight=weight, size_average=size_average, ignore_index=ignore_index,
                                            reduce=reduce, reduction='mean', label_smoothing=label_smoothing)
 
     def forward(self, out: Dict, target: Dict) -> Dict:
         pred = out['pred']
         target = target['target']
         loss = self.loss_fn(pred, target)
         return loss
 
 
 class SigmoidFocalLoss(nn.Module):
-    def __init__(self, alpha, gamma):
+    def __init__(self, alpha, gamma, **kwargs):
         super(SigmoidFocalLoss, self).__init__()
         self.alpha = alpha
         self.gamma = gamma
 
     def forward(self, out: Dict, target: Dict, reduction='mean'):
         pred = out['pred']
         target = target['target']
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/losses/detection/retinanet.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/retinanet.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from torchvision.models.detection._utils import BoxCoder, Matcher
 from torchvision.ops import boxes as box_ops
 
 from ..common import SigmoidFocalLoss
 
 
 class RetinaNetLoss(nn.Module):
-    def __init__(self) -> None:
+    def __init__(self, **kwargs) -> None:
         super().__init__()
         fg_iou_thresh = 0.5
         bg_iou_thresh = 0.4
         self.proposal_matcher = Matcher(
                 fg_iou_thresh,
                 bg_iou_thresh,
                 allow_low_quality_matches=True,
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/losses/detection/yolox.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/detection/yolox.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,21 +39,35 @@
     bboxes[:, 3] = bboxes[:, 3] - bboxes[:, 1]
     bboxes[:, 0] = bboxes[:, 0] + bboxes[:, 2] * 0.5
     bboxes[:, 1] = bboxes[:, 1] + bboxes[:, 3] * 0.5
     return bboxes
 
 
 class YOLOXLoss(nn.Module):
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, l1_activate_epoch, cur_epoch=None, **kwargs) -> None:
         super(YOLOXLoss, self).__init__()
+        self.l1_loss = nn.L1Loss(reduction="none")
         self.bcewithlog_loss = nn.BCEWithLogitsLoss(reduction="none")
         self.iou_loss = IOUloss(reduction="none")
 
+        self.l1_activate_epoch = l1_activate_epoch
+        self.cur_epoch = cur_epoch
+
+        self.use_l1 = False
+
+    def use_l1_update(self):
+        if self.cur_epoch is None:
+            return True
+        if self.cur_epoch.value >= self.l1_activate_epoch:
+            return True
+        return False
 
     def forward(self, out: List, target: Dict) -> torch.Tensor:
+        self.use_l1 = self.use_l1_update()
+
         out = out['pred']
         x_shifts = []
         y_shifts = []
         expanded_strides = []
 
         self.grids = [torch.zeros(1)] * len(out)
         self.num_classes = target['num_classes']
@@ -77,28 +91,51 @@
             )
             out_for_loss.append(o)
 
         # YOLOX model learns box cxcywh format directly,
         # but our detection dataloader gives xyxy format.
         for i in range(len(target)):
             target[i]['boxes'] = xyxy2cxcywh(target[i]['boxes'])
-        total_loss, iou_loss, conf_loss, cls_loss, num_fg = self.get_losses(
+
+        # Ready for l1 loss
+        origin_preds = []
+        for o in out:
+            reg_output = o[:, :4]
+
+            batch_size = reg_output.shape[0]
+            hsize, wsize = reg_output.shape[-2:]
+            reg_output = reg_output.view(
+                batch_size, 1, 4, hsize, wsize
+            )
+            reg_output = reg_output.permute(0, 1, 3, 4, 2).reshape(
+                batch_size, -1, 4
+            )
+            origin_preds.append(reg_output.clone())
+
+        total_loss, iou_loss, conf_loss, cls_loss, l1_loss, num_fg = self.get_losses(
                     None,
                     x_shifts,
                     y_shifts,
                     expanded_strides,
                     target,
                     torch.cat(out_for_loss, 1),
-                    [],
+                    origin_preds,
                     dtype=out[0].dtype,
                 )
 
         # TODO: return as dict
         return total_loss
 
+    def get_l1_target(self, l1_target, gt, stride, x_shifts, y_shifts, eps=1e-8):
+        l1_target[:, 0] = gt[:, 0] / stride - x_shifts
+        l1_target[:, 1] = gt[:, 1] / stride - y_shifts
+        l1_target[:, 2] = torch.log(gt[:, 2] / stride + eps)
+        l1_target[:, 3] = torch.log(gt[:, 3] / stride + eps)
+        return l1_target
+
     def get_losses(
         self,
         imgs,
         x_shifts,
         y_shifts,
         expanded_strides,
         target,
@@ -123,31 +160,33 @@
         # calculate targets
         nlabel = (labels.sum(dim=2) > 0).sum(dim=1)  # number of objects
 
         total_num_anchors = outputs.shape[1]
         x_shifts = torch.cat(x_shifts, 1)  # [1, n_anchors_all]
         y_shifts = torch.cat(y_shifts, 1)  # [1, n_anchors_all]
         expanded_strides = torch.cat(expanded_strides, 1)
-        #if self.use_l1:
-        #    origin_preds = torch.cat(origin_preds, 1)
+        if self.use_l1:
+            origin_preds = torch.cat(origin_preds, 1)
 
         cls_targets = []
         reg_targets = []
+        l1_targets = []
         obj_targets = []
         fg_masks = []
 
         num_fg = 0.0
         num_gts = 0.0
 
         for batch_idx in range(outputs.shape[0]):
             num_gt = int(nlabel[batch_idx])
             num_gts += num_gt
             if num_gt == 0:
                 cls_target = outputs.new_zeros((0, self.num_classes))
                 reg_target = outputs.new_zeros((0, 4))
+                l1_target = outputs.new_zeros((0, 4))
                 outputs.new_zeros((0, 4))
                 obj_target = outputs.new_zeros((total_num_anchors, 1))
                 fg_mask = outputs.new_zeros(total_num_anchors).bool()
             else:
                 gt_bboxes_per_image = labels[batch_idx, :num_gt, 1:5]
                 gt_classes = labels[batch_idx, :num_gt, 0]
                 bboxes_preds_per_image = bbox_preds[batch_idx]
@@ -207,65 +246,60 @@
                 num_fg += num_fg_img
 
                 cls_target = F.one_hot(
                     gt_matched_classes.to(torch.int64), self.num_classes
                 ) * pred_ious_this_matching.unsqueeze(-1)
                 obj_target = fg_mask.unsqueeze(-1)
                 reg_target = gt_bboxes_per_image[matched_gt_inds]
-                #if self.use_l1:
-                #    l1_target = self.get_l1_target(
-                #        outputs.new_zeros((num_fg_img, 4)),
-                #        gt_bboxes_per_image[matched_gt_inds],
-                #        expanded_strides[0][fg_mask],
-                #        x_shifts=x_shifts[0][fg_mask],
-                #        y_shifts=y_shifts[0][fg_mask],
-                #    )
+                if self.use_l1:
+                   l1_target = self.get_l1_target(
+                       outputs.new_zeros((num_fg_img, 4)),
+                       gt_bboxes_per_image[matched_gt_inds],
+                       expanded_strides[0][fg_mask],
+                       x_shifts=x_shifts[0][fg_mask],
+                       y_shifts=y_shifts[0][fg_mask],
+                   )
 
             cls_targets.append(cls_target)
             reg_targets.append(reg_target)
             obj_targets.append(obj_target.to(dtype))
             fg_masks.append(fg_mask)
-            #if self.use_l1:
-            #    l1_targets.append(l1_target)
+            if self.use_l1:
+               l1_targets.append(l1_target)
 
         cls_targets = torch.cat(cls_targets, 0)
         reg_targets = torch.cat(reg_targets, 0)
         obj_targets = torch.cat(obj_targets, 0)
         fg_masks = torch.cat(fg_masks, 0)
-        #if self.use_l1:
-        #    l1_targets = torch.cat(l1_targets, 0)
+        if self.use_l1:
+           l1_targets = torch.cat(l1_targets, 0)
 
         num_fg = max(num_fg, 1)
         loss_iou = (
             self.iou_loss(bbox_preds.view(-1, 4)[fg_masks], reg_targets)
         ).sum() / num_fg
         loss_obj = (
             self.bcewithlog_loss(obj_preds.view(-1, 1), obj_targets)
         ).sum() / num_fg
         loss_cls = (
             self.bcewithlog_loss(
                 cls_preds.view(-1, self.num_classes)[fg_masks], cls_targets
             )
         ).sum() / num_fg
-        #if self.use_l1:
-        #    loss_l1 = (
-        #        self.l1_loss(origin_preds.view(-1, 4)[fg_masks], l1_targets)
-        #    ).sum() / num_fg
-        #else:
-        #    loss_l1 = 0.0
+        loss_l1 = self.l1_loss(origin_preds.view(-1, 4)[fg_masks], l1_targets).sum() / num_fg if self.use_l1 else 0.0
 
         reg_weight = 5.0
-        loss = reg_weight * loss_iou + loss_obj + loss_cls# + loss_l1
+        loss = reg_weight * loss_iou + loss_obj + loss_cls + loss_l1
 
         return (
             loss,
             reg_weight * loss_iou,
             loss_obj,
             loss_cls,
-            #loss_l1,
+            loss_l1,
             num_fg / max(num_gts, 1),
         )
 
     @torch.no_grad()
     def get_assignments(
         self,
         batch_idx,
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/losses/segmentation/pidnet.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/losses/segmentation/pidnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     def forward(self, out: Dict, target: Dict) -> torch.Tensor:
         bd_gt = target['bd_gt']
         extra_d = out['extra_d']
         return self.weighted_bce(extra_d, bd_gt)
 
 
 class PIDNetLoss(nn.Module):
-    def __init__(self, ignore_index=IGNORE_INDEX_NONE_VALUE, weight=None):
+    def __init__(self, ignore_index=IGNORE_INDEX_NONE_VALUE, weight=None, **kwargs):
         super().__init__()
 
         self.cross_entropy_loss = PIDNetCrossEntropy(ignore_index=ignore_index)
         self.boundary_loss = BoundaryLoss()
         self.cross_entropy_with_boundary = PIDNetBoundaryAwareCrossEntropy(ignore_index=ignore_index)
 
     def forward(self, out: Dict, target: Dict):
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/builder.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,45 @@
 from typing import Any, Dict
 
 import torch
 
-from ..utils.record import AverageMeter
 from .registry import PHASE_LIST, TASK_METRIC
 
 
 class MetricFactory:
     def __init__(self, task, conf_model, **kwargs) -> None:
         self.task = task
         self.conf_model = conf_model
 
         assert self.task in TASK_METRIC
         self.metric_cls = TASK_METRIC[self.task]
 
-        self.metric_fn = self.metric_cls(**kwargs)
-        self._clear_epoch_start()
-
-    def _clear_epoch_start(self):
-        self.metric_meter_dict: Dict[str, Dict[str, AverageMeter]] = {
-            phase: {
-                metric_key: AverageMeter(metric_key, ':6.2f')
-                for metric_key in self.metric_cls.metric_names
-            }
-            for phase in PHASE_LIST
-        }
+        # TODO: This code assumes there is only one loss module. Fix here later.
+        if hasattr(conf_model.losses[0], 'ignore_index'):
+            kwargs['ignore_index'] = conf_model.losses[0].ignore_index
+        self.metrics = {phase: self.metric_cls(**kwargs) for phase in PHASE_LIST}
 
     def reset_values(self):
-        self._clear_epoch_start()
-
-    def calc(self, pred: torch.Tensor, target: torch.Tensor, phase='train', **kwargs: Any) -> None:
-        self.__call__(pred=pred, target=target, phase=phase, **kwargs)
-
-    def __call__(self, pred: torch.Tensor, target: torch.Tensor, phase: str, **kwargs: Any) -> None:
+        for phase in PHASE_LIST:
+            [meter.reset() for _, meter in self.metrics[phase].metric_meter.items()]
 
-        metric_result_dict = self.metric_fn.calibrate(pred, target)
+    def update(self, pred: torch.Tensor, target: torch.Tensor, phase: str, **kwargs: Any) -> None:
+        if len(pred) == 0: # Removed dummy batch has 0 len
+            return
         phase = phase.lower()
-        assert phase in PHASE_LIST, f"{phase} is not defined at our phase list ({PHASE_LIST})"
-        for metric_key in self.metric_meter_dict[phase]:
-            assert metric_key in metric_result_dict
-            self.metric_meter_dict[phase][metric_key].update(float(metric_result_dict[metric_key]))
+        self.metrics[phase].calibrate(pred, target)
 
     def result(self, phase='train'):
-        return self.metric_meter_dict[phase.lower()]
+        return {metric_name: meter.avg for metric_name, meter in self.metrics[phase].metric_meter.items()}
 
     @property
     def metric_names(self):
-        return self.metric_fn.metric_names
+        return self.metrics[list(self.metrics.keys())[0]].metric_names
 
     @property
     def primary_metric(self):
-        return self.metric_fn.primary_metric
+        return self.metrics[list(self.metrics.keys())[0]].primary_metric
 
 
 def build_metrics(task: str, conf_model, **kwargs) -> MetricFactory:
     metric_handler = MetricFactory(task, conf_model, **kwargs)
     return metric_handler
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/classification/metric.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/classification/metric.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from typing import List
 
+import numpy as np
 import torch
 
 from ..base import BaseMetric
 
 TOPK_MAX = 20
 
 
 @torch.no_grad()
 def accuracy_topk(pred, target):
     """Computes the accuracy over the k top predictions for the specified values of k"""
-    batch_size = target.size(0)
-    maxk = pred.size(-1)
-    pred = pred.t()
-    correct = pred.eq(target.reshape(1, -1).expand_as(pred))
-    return lambda topk: correct[:min(topk, maxk)].reshape(-1).float().sum(0) * 100. / batch_size
+    maxk = pred.shape[-1]
+    pred = pred.T
+    class_num = pred.shape[0]
+    correct = np.equal(pred, np.tile(target, (class_num, 1)))
+    return lambda topk: correct[:min(topk, maxk)].reshape(-1).astype('float').sum(0)
 
 
 class ClassificationMetric(BaseMetric):
-    metric_names: List[str] = ['Acc@1', 'Acc@5']
-    primary_metric: str = 'Acc@1'
+    SUPPORT_METRICS: List[str] = ['Acc@1', 'Acc@5']
 
     def __init__(self, **kwargs):
-        super().__init__()
+        # TODO: Select metrics by user
+        metric_names = ['Acc@1', 'Acc@5']
+        primary_metric = 'Acc@1'
+
+        assert set(metric_names).issubset(ClassificationMetric.SUPPORT_METRICS)
+        super().__init__(metric_names=metric_names, primary_metric=primary_metric)
 
     def calibrate(self, pred, target, **kwargs):
-        result_dict = {k: 0. for k in self.metric_names}
         topk_callable = accuracy_topk(pred, target)
 
-        result_dict['Acc@1'] = topk_callable(topk=1)
-        result_dict['Acc@5'] = topk_callable(topk=5)
-        return result_dict
+        Acc1_correct = topk_callable(topk=1)
+        Acc5_correct = topk_callable(topk=5)
+
+        self.metric_meter['Acc@1'].update(Acc1_correct, n=pred.shape[0])
+        self.metric_meter['Acc@5'].update(Acc5_correct, n=pred.shape[0])
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/detection/metric.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/detection/metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,19 +161,22 @@
                 recall[:, iou_level_idx], precision[:, iou_level_idx]
             )
 
     return average_precisions
 
 
 class DetectionMetric(BaseMetric):
-    metric_names: List[str] = ['map50', 'map75', 'map50_95']
-    primary_metric: str = 'map50'
+    SUPPORT_METRICS: List[str] = ['map50', 'map75', 'map50_95']
 
     def __init__(self, **kwargs):
-        super().__init__()
+        # TODO: Select metrics by user
+        metric_names: List[str] = ['map50', 'map75', 'map50_95']
+        primary_metric: str = 'map50'
+        assert set(metric_names).issubset(DetectionMetric.SUPPORT_METRICS)
+        super().__init__(metric_names=metric_names, primary_metric=primary_metric)
 
     def calibrate(self, predictions, targets, **kwargs):
         result_dict = {k: 0. for k in self.metric_names}
 
         iou_thresholds = np.linspace(0.5, 0.95, 10)
         stats = []
 
@@ -205,15 +208,20 @@
                     )
                 )
 
         # Compute average precisions if any matches exist
         if stats:
             concatenated_stats = [np.concatenate(items, 0) for items in zip(*stats)]
             average_precisions = average_precisions_per_class(*concatenated_stats)
-            result_dict['map50'] = average_precisions[:, 0].mean()
-            result_dict['map75'] = average_precisions[:, 5].mean()
-            result_dict['map50_95'] = average_precisions.mean()
+            #result_dict['map50'] = average_precisions[:, 0].mean()
+            #result_dict['map75'] = average_precisions[:, 5].mean()
+            #result_dict['map50_95'] = average_precisions.mean()
+            self.metric_meter['map50'].update(average_precisions[:, 0].mean())
+            self.metric_meter['map75'].update(average_precisions[:, 5].mean())
+            self.metric_meter['map50_95'].update(average_precisions.mean())
         else:
-            result_dict['map50'], result_dict['map75'], result_dict['map50_95'] = 0, 0, 0
-            average_precisions = []
+            #result_dict['map50'], result_dict['map75'], result_dict['map50_95'] = 0, 0, 0
+            self.metric_meter['map50'].update(0)
+            self.metric_meter['map75'].update(0)
+            self.metric_meter['map50_95'].update(0)
 
         return result_dict
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/metrics/segmentation/metric.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/metrics/segmentation/metric.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from typing import List
 
 import numpy as np
-import torch
 
-from ...utils.record import AverageMeter
 from ..base import BaseMetric
 
 IGNORE_INDEX_NONE_VALUE = -100
 
 
 class SegmentationMetric(BaseMetric):
-    metric_names: List[str] = ['iou', 'pixel_acc']
-    primary_metric: str = 'iou'
+    SUPPORT_METRICS: List[str] = ['iou', 'pixel_acc']
 
     def __init__(self, num_classes=None, ignore_index=IGNORE_INDEX_NONE_VALUE):
-        super().__init__()
+        # TODO: Select metrics by user
+        metric_names = ['iou', 'pixel_acc']
+        primary_metric = 'iou'
+
+        assert set(metric_names).issubset(SegmentationMetric.SUPPORT_METRICS)
+        super().__init__(metric_names=metric_names, primary_metric=primary_metric)
         self.ignore_index = ignore_index if ignore_index is not None else IGNORE_INDEX_NONE_VALUE
         self.K = num_classes
 
-    def intersection_and_union_gpu(self, output, target):
+    def intersection_and_union(self, output, target):
 
         # 'K' classes, output and target sizes are N or N * L or N * H * W, each value in range 0 to K - 1.
-        assert (output.dim() in [1, 2, 3])
+        assert (len(output.shape) in [1, 2, 3])
 
         assert output.shape == target.shape
-        output = output.view(-1)
-        target = target.view(-1)
+        output = output.reshape(-1)
+        target = target.reshape(-1)
         output[target == self.ignore_index] = self.ignore_index
         intersection = output[output == target]
-        area_intersection = torch.histc(intersection, bins=self.K, min=0, max=self.K-1)
-        area_output = torch.histc(output, bins=self.K, min=0, max=self.K-1)
-        area_target = torch.histc(target, bins=self.K, min=0, max=self.K-1)
+        #area_intersection = torch.histc(intersection, bins=self.K, min=0, max=self.K-1)
+        #area_output = torch.histc(output, bins=self.K, min=0, max=self.K-1)
+        #area_target = torch.histc(target, bins=self.K, min=0, max=self.K-1)
+        area_intersection = np.histogram(intersection, bins=np.linspace(0, self.K, self.K+1))[0]
+        area_output = np.histogram(output, bins=np.linspace(0, self.K, self.K+1))[0]
+        area_target = np.histogram(target, bins=np.linspace(0, self.K, self.K+1))[0]
         area_union = area_output + area_target - area_intersection
 
-        intersection, union, target, output = \
-            area_intersection.cpu().numpy(), area_union.cpu().numpy(), area_target.cpu().numpy(), area_output.cpu().numpy()
+        intersection, union, target, output = area_intersection, area_union, area_target, area_output
 
         return {
             'intersection': intersection,
             'union': union,
             'target': target,
             'output': output
         }
 
     def calibrate(self, pred, target, **kwargs):
-        result_dict = {k: AverageMeter(k) for k in self.metric_names}
-        B = pred.size(0)
-
-        metrics = self.intersection_and_union_gpu(pred, target)
-        result_dict['iou'].update(sum(metrics['intersection']) / (sum(metrics['union']) + 1e-10), n=B)
-        result_dict['pixel_acc'].update(sum(metrics['intersection']) / (sum(metrics['target']) + 1e-10), n=B)
+        B = pred.shape[0]
 
-        return {k: v.avg for k, v in result_dict.items()}
+        metrics = self.intersection_and_union(pred, target)
+        self.metric_meter['iou'].update(sum(metrics['intersection']) / (sum(metrics['union']) + 1e-10), n=B)
+        self.metric_meter['pixel_acc'].update(sum(metrics['intersection']) / (sum(metrics['target']) + 1e-10), n=B)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/core/resnet.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/core/resnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from omegaconf import DictConfig
 import torch
 import torch.nn as nn
 from torch import Tensor
 
 from ...op.custom import BasicBlock, Bottleneck, ConvLayer
 from ...utils import BackboneOutput
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
 
 __all__ = ['resnet']
 
-SUPPORTING_TASK = ['classification', 'segmentation']
+SUPPORTING_TASK = ['classification', 'segmentation', 'detection', 'pose_estimation']
 
 BLOCK_FROM_LITERAL: Dict[str, Type[nn.Module]] = {
     'basicblock': BasicBlock,
     'bottleneck': Bottleneck,
 }
 
 
@@ -26,28 +27,31 @@
 
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ) -> None:
+        # Check task compatibility
+        self.task = task.lower()
+        assert self.task in SUPPORTING_TASK, f'ResNet is not supported on {self.task} task now.'
+        self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
         super(ResNet, self).__init__()
 
         block: Literal['basicblock', 'bottleneck'] = params.block_type
         norm_layer: Optional[str] = params.norm_type
 
         # Fix as constant
         zero_init_residual: bool = False
         groups: int = 1
         width_per_group: int = 64
         expansion: Optional[int] = None
 
-        self.task = task.lower()
         block = BLOCK_FROM_LITERAL[block.lower()]
-        self.use_intermediate_features = self.task in ['segmentation', 'detection']
 
         if norm_layer is None:
             norm_layer = 'batch_norm'
         self._norm_layer = norm_layer
 
         self.inplanes = 64
         self.dilation = 1
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/darknet.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/darknet.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,35 +6,39 @@
 
 from omegaconf import DictConfig
 import torch
 from torch import nn
 
 from ...op.custom import ConvLayer, CSPLayer, Focus, SPPBottleneck
 from ...utils import BackboneOutput
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
 
 __all__ = ['cspdarknet']
-SUPPORTING_TASK = ['detection']
+SUPPORTING_TASK = ['classification', 'segmentation', 'detection', 'pose_estimation']
 
 
 class CSPDarknet(nn.Module):
 
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
         #depthwise=False,
     ) -> None:
+        # Check task compatibility
+        self.task = task.lower()
+        assert self.task in SUPPORTING_TASK, f'CSPDarknet is not supported on {self.task} task now.'
+        self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
         super().__init__()
+
         out_features=("dark3", "dark4", "dark5")
         assert out_features, "please provide output features of Darknet"
 
-        self.task = task.lower()
-        self.use_intermediate_features = self.task in ['segmentation', 'detection']
-
         dep_mul = params.dep_mul
         wid_mul = params.wid_mul
         act_type = params.act_type
 
         self.out_features = out_features
         Conv = ConvLayer
 
@@ -113,14 +117,22 @@
         self.avgpool = nn.AdaptiveAvgPool2d(1)
 
         predefined_out_features = {'dark2': base_channels * 2, 'dark3': base_channels * 4, 
                                    'dark4': base_channels * 8, 'dark5': base_channels * 16}
         self._feature_dim = predefined_out_features['dark5']
         self._intermediate_features_dim = [predefined_out_features[out_feature] for out_feature in out_features]
 
+        # Initialize
+        def init_bn(M):
+            for m in M.modules():
+                if isinstance(m, nn.BatchNorm2d):
+                    m.eps = 1e-3
+                    m.momentum = 0.03
+        self.apply(init_bn)
+
     def forward(self, x):
         outputs_dict = {}
         x = self.stem(x)
         outputs_dict["stem"] = x
         x = self.dark2(x)
         outputs_dict["dark2"] = x
         x = self.dark3(x)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/efficientformer.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/efficientformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,19 @@
     MetaFormerEncoder,
     MultiHeadAttention,
     Pooling,
 )
 from ...op.custom import ConvLayer
 from ...op.depth import DropPath
 from ...utils import BackboneOutput
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
 
-SUPPORTING_TASK = ['classification', 'segmentation', 'detection']
+__all__ = ['efficientformer']
+
+SUPPORTING_TASK = ['classification', 'segmentation', 'detection', 'pose_estimation']
 
 
 class EfficientFormerStem(nn.Module):
     def __init__(self, in_channels, out_channels):
         super().__init__()
         self.stem = nn.Sequential(
             ConvLayer(in_channels, out_channels // 2, kernel_size=3, stride=2, padding=1, bias=True,
@@ -331,15 +334,20 @@
 
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ) -> None:
-        
+        # Check task compatibilty
+        self.task = task.lower()
+        assert self.task in SUPPORTING_TASK, f'EfficientFormer is not supported on {self.task} task now.'
+        self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
+        # Get params
         num_blocks = [stage.num_blocks for stage in stage_params]
         hidden_sizes = [stage.channels for stage in stage_params]
 
         num_attention_heads = params.num_attention_heads
         attention_hidden_size = params.attention_channels
         attention_dropout_prob = params.attention_dropout_prob
         attention_ratio = params.attention_value_expansion_ratio
@@ -357,16 +365,14 @@
         pool_size = 3
         downsamples = [True for _ in stage_params]
         use_layer_scale = True
         attention_bias_resolution = 16
         drop_path_rate = 0.
 
         super().__init__(hidden_sizes)
-        self.task = task.lower()
-        self.use_intermediate_features = self.task in ['segmentation', 'detection']
 
         image_channels = 3
         self.patch_embed = EfficientFormerStem(in_channels=image_channels, out_channels=hidden_sizes[0])
 
         self.encoder = EfficientFormerEncoder(
             self.use_intermediate_features, num_blocks, hidden_sizes,
             num_attention_heads, attention_hidden_size, attention_dropout_prob,
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mixnet.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from torch import nn
 from torch.nn import functional as F
 from torchvision.ops.misc import SqueezeExcitation as SEBlock
 
 from ...op.registry import ACTIVATION_REGISTRY
 from ...op.custom import ConvLayer
 from ...utils import BackboneOutput
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
+
+__all__ = ['mixnet']
+
+SUPPORTING_TASK = ['classification', 'segmentation', 'detection', 'pose_estimation']
 
 
 # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
 # GPConv: Grouped Point-wise Convolution for MixDepthBlock
 # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
 class GPConv(nn.Module):
     def __init__(self, in_planes, out_planes, num_groups):
@@ -148,17 +153,20 @@
 class MixNet(nn.Module):
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ):
-        super(MixNet, self).__init__()
+        # Check task compatibility
         self.task = task.lower()
-        self.use_intermediate_features = self.task in ['segmentation', 'detection']
+        assert self.task in SUPPORTING_TASK, f'MixNet is not supported on {self.task} task now.'
+        self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
+        super(MixNet, self).__init__()
 
         stem_channels = params.stem_channels
         width_multi = params.wid_mul
         depth_multi = params.dep_mul
         self.dropout_rate = params.dropout_rate
 
         out_channels = self._round_filters(stem_channels, width_multi)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mixtransformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import torch
 import torch.nn as nn
 
 from ...op.base_metaformer import Image2Sequence, MetaFormer, MetaFormerBlock, MetaFormerEncoder, MultiHeadAttention
 from ...op.custom import ConvLayer
 from ...op.registry import ACTIVATION_REGISTRY
 from ...utils import BackboneOutput
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
 
-SUPPORTING_TASK = ['classification', 'segmentation']
+__all__ = ['mixtransformer']
 
+SUPPORTING_TASK = ['classification', 'segmentation', 'detection', 'pose_estimation']
 TEMP_HIDDEN_SZIE_AS_CONSTANT = 256
 
 
 class SegformerOverlapPatchEmbeddings(nn.Module):
     """Construct the overlapping patch embeddings."""
 
     def __init__(self, patch_size, stride, in_channels, hidden_size):
@@ -138,14 +140,19 @@
 class MixTransformer(MetaFormer):
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ) -> None:
+        # Check task compatibility
+        self.task = task.lower()
+        assert self.task in SUPPORTING_TASK, f'MixTransformer is not supported on {self.task} task now.'
+        self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
         super().__init__([stage.attention_chananels for stage in stage_params])
         self.task = task
         self.use_intermediate_features = self.task in ['segmentation', 'detection']
 
         intermediate_ratio = params.ffn_intermediate_expansion_ratio
         hidden_activation_type = params.ffn_act_type
         hidden_dropout_prob = params.ffn_dropout_prob
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilenetv3.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,32 +7,36 @@
 from omegaconf import DictConfig
 import torch
 import torch.nn as nn
 from torch import Tensor
 
 from ...op.custom import ConvLayer, InvertedResidual
 from ...utils import BackboneOutput
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
 
 __all__ = ['mobilenetv3']
 
-SUPPORTING_TASK = ['classification', 'segmentation']
+SUPPORTING_TASK = ['classification', 'segmentation', 'detection', 'pose_estimation']
 
 
 class MobileNetV3(nn.Module):
 
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ) -> None:
+        # Check task compatibility
+        self.task = task.lower()
+        assert self.task in SUPPORTING_TASK, f'MobileNetV3 is not supported on {self.task} task now.'
+        self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
         super(MobileNetV3, self).__init__()
 
-        self.task = task.lower()
-        self.use_intermediate_features = self.task in ['segmentation', 'detection']
         norm_type = 'batch_norm'
         act_type = 'hard_swish'
 
         # building first layer
         firstconv_output_channels = stage_params[0].in_channels[0]
         self.conv_first = ConvLayer(
             in_channels=3,
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/mobilevit.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/mobilevit.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 
 from ...op.base_metaformer import ChannelMLP, MetaFormer, MetaFormerBlock, MetaFormerEncoder, MultiHeadAttention
 from ...op.custom import ConvLayer, GlobalPool, InvertedResidual
 from ...utils import BackboneOutput, FXTensorType
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
 
 __all__ = ['mobilevit']
 SUPPORTING_TASK = ['classification']
 
+
 class MobileViTEmbeddings(nn.Module):
     def __init__(self, image_channels, hidden_size):
         super().__init__()
         
         image_channels = 3  # {RGB}
         self.conv = ConvLayer(
             in_channels=image_channels,
@@ -36,26 +38,28 @@
         )
     
     def forward(self, x):
         # x: B x 3(={RGB}) x H x W
         x = self.conv(x)  # B x C x H//2 x W//2
         return x
 
+
 class MobileViTTransformerBlock(MetaFormerBlock):
     # Original: TransformerEncoder
     def __init__(self, hidden_size, num_attention_heads, attention_dropout_prob, intermediate_size, hidden_dropout_prob, layer_norm_eps) -> None:
         super().__init__(hidden_size, layer_norm_eps)
         self.layernorm_before = nn.LayerNorm(hidden_size, eps=layer_norm_eps)
         self.layernorm_after = nn.LayerNorm(hidden_size, eps=layer_norm_eps)
         self.token_mixer = MultiHeadAttention(hidden_size, num_attention_heads,
                                               attention_scale=(hidden_size // num_attention_heads) ** -0.5,
                                               attention_dropout_prob=attention_dropout_prob,
                                               use_qkv_bias=True)
         self.channel_mlp = ChannelMLP(hidden_size, intermediate_size, hidden_dropout_prob)
 
+
 class MobileViTBlock(nn.Module):
     # Original: MobileViTBlock
     def __init__(self, num_transformer_blocks, in_channels, hidden_size, local_kernel_size,
                  patch_h, patch_w, num_attention_heads, attention_dropout_prob, intermediate_size, hidden_dropout_prob,
                  layer_norm_eps, use_fusion_layer=True) -> None:
         super().__init__()
         self.patch_h = patch_h
@@ -248,14 +252,15 @@
 
         out = self.proj(out)
 
         if self.use_fusion_layer:
             out = self.fusion(torch.cat((x, out), dim=1))  # skip concat
         return out
 
+
 class MobileViTEncoder(MetaFormerEncoder):
     def __init__(
         self,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ) -> None:
         super().__init__()
@@ -362,14 +367,19 @@
 class MobileViT(MetaFormer):
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ) -> None:
+        # Check task compatibility
+        self.task = task.lower()
+        assert self.task in SUPPORTING_TASK, f'MobileViT is not supported on {self.task} task now.'
+        #self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
         exp_channels = min(params.output_expansion_ratio * stage_params[-1].out_channels, 960)
         hidden_sizes = [stage.out_channels for stage in stage_params] + [exp_channels]
         super().__init__(hidden_sizes)
         
         self.task = task
         self.intermediate_features = self.task in ['segmentation', 'detection']
         
@@ -388,10 +398,11 @@
         
     def forward(self, x: FXTensorType):
         x = self.patch_embed(x)
         x = self.encoder(x)
         x = self.conv_1x1_exp(x)
         feat = self.pool(x)
         return BackboneOutput(last_feature=feat)
-    
+
+
 def mobilevit(task, conf_model_backbone):
     return MobileViT(task, conf_model_backbone.params, conf_model_backbone.stage_params)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/backbones/experimental/vit.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/backbones/experimental/vit.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,20 @@
     MetaFormer,
     MetaFormerBlock,
     MetaFormerEncoder,
     MultiHeadAttention,
 )
 from ...op.custom import ConvLayer, SinusoidalPositionalEncoding
 from ...utils import BackboneOutput
+from ..registry import USE_INTERMEDIATE_FEATURES_TASK_LIST
 
 __all__ = ['vit']
 SUPPORTING_TASK = ['classification']
 
+
 class ViTEmbeddings(nn.Module):
     def __init__(self, image_channels, patch_size, hidden_size, hidden_dropout_prob, use_cls_token=True, vocab_size=1000):
         super().__init__()
         
         image_channels = 3  # {RGB}
         
         kernel_size = patch_size
@@ -68,14 +70,15 @@
             patch_emb = torch.cat((cls_tokens, patch_emb), dim=1)  # B x (H'*W' + 1) x C
 
         patch_emb = self.pos_embed(patch_emb)  # B x (H'*W' + 1) x C
         
         patch_emb = self.dropout(patch_emb)  # B x (H'*W' + 1) x C
         return patch_emb  # B x (H'*W' + 1) x C
 
+
 class ViTBlock(MetaFormerBlock):
     def __init__(self, hidden_size, num_attention_heads, attention_dropout_prob, intermediate_size, hidden_dropout_prob, layer_norm_eps) -> None:
         super().__init__(hidden_size, layer_norm_eps)
         self.layernorm_before = nn.LayerNorm(hidden_size, eps=layer_norm_eps)
         self.layernorm_after = nn.LayerNorm(hidden_size, eps=layer_norm_eps)
         self.token_mixer = MultiHeadAttention(hidden_size, num_attention_heads,
                                                   attention_scale=(hidden_size // num_attention_heads) ** -0.5,
@@ -88,21 +91,27 @@
 class ViTEncoder(MetaFormerEncoder):
     def __init__(self, num_blocks, hidden_size, num_attention_heads, attention_dropout_prob, intermediate_size, hidden_dropout_prob, layer_norm_eps) -> None:
         super().__init__()
         self.blocks = nn.Sequential(
             *[ViTBlock(hidden_size, num_attention_heads, attention_dropout_prob, intermediate_size, hidden_dropout_prob, layer_norm_eps) for _ in range(num_blocks)]
         )
 
+
 class VisionTransformer(MetaFormer):
     def __init__(
         self,
         task: str,
         params: Optional[DictConfig] = None,
         stage_params: Optional[List] = None,
     ) -> None:
+        # Check task compatibility
+        self.task = task.lower()
+        assert self.task in SUPPORTING_TASK, f'ViT is not supported on {self.task} task now.'
+        #self.use_intermediate_features = self.task in USE_INTERMEDIATE_FEATURES_TASK_LIST
+
         patch_size = params.patch_size
         hidden_size = params.attention_channels
         num_blocks = params.num_blocks
         num_attention_heads = params.num_attention_heads
         attention_dropout_prob = params.attention_dropout_prob
         intermediate_size = params.ffn_intermediate_channels
         hidden_dropout_prob = params.ffn_dropout_prob
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/base.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,7 +80,18 @@
 
     def forward(self, x, label_size=None, targets=None):
         features: BackboneOutput = self.backbone(x)
         if hasattr(self, 'neck'):
             features: BackboneOutput = self.neck(features['intermediate_features'])
         out: DetectionModelOutput = self.head(features['intermediate_features'])
         return out
+
+class PoseEstimationModel(TaskModel):
+    def __init__(self, conf_model, backbone, neck, head, freeze_backbone=False) -> None:
+        super().__init__(conf_model, backbone, neck, head, freeze_backbone)
+
+    def forward(self, x, label_size=None, targets=None):
+        features: BackboneOutput = self.backbone(x)
+        if hasattr(self, 'neck'):
+            features: BackboneOutput = self.neck(features['intermediate_features'])
+        out: DetectionModelOutput = self.head(features['intermediate_features'])
+        return out
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/builder.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     return model
 
 
 def load_backbone_and_head_model(
         conf_model, task, backbone_name, head_name, num_classes,
         model_checkpoint, use_pretrained, freeze_backbone,
-        img_size
     ):
     if task not in TASK_MODEL_DICT:
         raise ValueError(
             f"No such task(s) named: {task}. This should be included in SUPPORTING_TASK_LIST ({SUPPORTING_TASK_LIST})")
 
     # Backbone construction
     backbone_fn: Callable[..., nn.Module] = MODEL_BACKBONE_DICT[backbone_name]
@@ -54,32 +53,30 @@
         neck = neck_fn(intermediate_features_dim=backbone.intermediate_features_dim, conf_model_neck=conf_model.architecture.neck)
         intermediate_features_dim = neck.intermediate_features_dim
 
     # Head construction
     head_module = MODEL_HEAD_DICT[task][head_name]
     if task == 'classification':
         head = head_module(num_classes=num_classes, feature_dim=backbone.feature_dim, conf_model_head=conf_model.architecture.head)
-    elif task in ['segmentation', 'detection']:
-        img_size = img_size if isinstance(img_size, (int, None)) else tuple(img_size)
+    elif task in ['segmentation', 'detection', 'pose_estimation']:
         head = head_module(num_classes=num_classes,
                                 intermediate_features_dim=intermediate_features_dim,
-                                label_size=img_size,
                                 conf_model_head=conf_model.architecture.head)
 
     # Assemble model and load checkpoint
     model = TASK_MODEL_DICT[task](conf_model, backbone, neck, head, freeze_backbone)
     if use_pretrained:
         model = load_from_checkpoint(
             model, model_checkpoint,
             load_checkpoint_head=conf_model.checkpoint.load_head,
         )
     return model
 
 
-def build_model(conf_model, task, num_classes, model_checkpoint, use_pretrained, img_size) -> nn.Module:
+def build_model(conf_model, task, num_classes, model_checkpoint, use_pretrained) -> nn.Module:
 
     if conf_model.single_task_model:
         model_name = str(conf_model.architecture.full.name).lower()
         return load_full_model(
             conf_model, model_name, num_classes,
             model_checkpoint=model_checkpoint,
             use_pretrained=use_pretrained
@@ -89,9 +86,8 @@
     head_name = str(conf_model.architecture.head.name).lower()
     freeze_backbone = conf_model.freeze_backbone
     return load_backbone_and_head_model(
         conf_model, task, backbone_name, head_name, num_classes,
         model_checkpoint=model_checkpoint,
         use_pretrained=use_pretrained,
         freeze_backbone=freeze_backbone,
-        img_size=img_size
     )
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/full/experimental/pidnet.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/full/experimental/pidnet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 
 class AllMLPDecoder(nn.Module):
     def __init__(
             self,
             num_classes: int,
             intermediate_features_dim: List[int],
-            label_size: Union[Tuple[int, int], int],
             params: DictConfig,
         ):
         super().__init__()
         intermediate_channels = params.intermediate_channels
         classifier_dropout_prob = params.classifier_dropout_prob
+        self.label_size = params.resize_output
 
         # linear layers which will unify the channel dimension of each of the encoder blocks to the same config.decoder_hidden_size
         mlps = []
         for feature_dim in intermediate_features_dim:
             mlp = ConvLayer(feature_dim, intermediate_channels, kernel_size=1,
                             use_norm=True, use_act=True, norm_type='batch_norm', act_type='relu')
             mlps.append(mlp)
@@ -34,16 +34,14 @@
         self.linear_fuse = ConvLayer(len(intermediate_features_dim) * intermediate_channels,
                                      intermediate_channels, kernel_size=1,
                                      use_norm=True, use_act=False)
 
         self.dropout = nn.Dropout(classifier_dropout_prob)
         self.classifier = nn.Conv2d(intermediate_channels, num_classes, kernel_size=1)
 
-        self.label_size = (label_size, label_size) if isinstance(label_size, int) else label_size
-
     def forward(self, encoder_hidden_states: FXTensorListType):
 
         all_hidden_states = ()
         for encoder_hidden_state, mlp in zip(encoder_hidden_states, self.linear_c):
 
             # unify channel dimension
             encoder_hidden_state = mlp(encoder_hidden_state)
@@ -65,12 +63,11 @@
             logits = F.interpolate(
                 logits, size=(H, W), mode="bilinear", align_corners=False
             )
 
         return ModelOutput(pred=logits)
 
 
-def all_mlp_decoder(num_classes, intermediate_features_dim, label_size, conf_model_head, **kwargs) -> AllMLPDecoder:
+def all_mlp_decoder(num_classes, intermediate_features_dim, conf_model_head, **kwargs) -> AllMLPDecoder:
     return AllMLPDecoder(num_classes,
                          intermediate_features_dim,
-                         label_size=label_size,
                          params=conf_model_head.params)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/experimental/fpn.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/fpn.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -142,8 +142,8 @@
     
     @property
     def intermediate_features_dim(self):
         return self._intermediate_features_dim
 
 
 def fpn(intermediate_features_dim, conf_model_neck, **kwargs):
-    return FPN(intermediate_features_dim=intermediate_features_dim, params=conf_model_neck.params)
+    return FPN(intermediate_features_dim=intermediate_features_dim, params=conf_model_neck.params)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/necks/experimental/yolopafpn.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/necks/experimental/yolopafpn.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,22 @@
             n=round(3 * depth),
             shortcut=False,
             act_type=act_type,
         )
 
         self._intermediate_features_dim = self.in_channels
 
+        # Initialize
+        def init_bn(M):
+            for m in M.modules():
+                if isinstance(m, nn.BatchNorm2d):
+                    m.eps = 1e-3
+                    m.momentum = 0.03
+        self.apply(init_bn)
+
     def forward(self, inputs):
         """
         Args:
             inputs: input images.
 
         Returns:
             Tuple[Tensor]: FPN feature.
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/base_metaformer.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/base_metaformer.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/custom.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/custom.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/depth.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/depth.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/op/pidnet.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/op/pidnet.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/registry.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from pathlib import Path
 from typing import Callable, Dict, List, Type
 
 import torch.nn as nn
 
 from .backbones import cspdarknet, efficientformer, mixnet, mixtransformer, mobilenetv3, mobilevit, resnet, vit
-from .base import ClassificationModel, DetectionModel, SegmentationModel, TaskModel
+from .base import ClassificationModel, DetectionModel, PoseEstimationModel, SegmentationModel, TaskModel
 from .full import pidnet
 from .heads.classification import fc
 from .heads.detection import anchor_decoupled_head, anchor_free_decoupled_head
+from .heads.pose_estimation import rtmcc
 from .heads.segmentation import all_mlp_decoder
 from .necks import fpn, yolopafpn
 
 MODEL_BACKBONE_DICT: Dict[str, Callable[..., nn.Module]] = {
     'resnet': resnet,
     'mobilenetv3': mobilenetv3,
     'mixtransformer': mixtransformer,
@@ -34,21 +35,25 @@
     'segmentation': {
         'all_mlp_decoder': all_mlp_decoder,
     },
     'detection': {
         'anchor_free_decoupled_head': anchor_free_decoupled_head,
         'anchor_decoupled_head': anchor_decoupled_head,
     },
+    'pose_estimation': {
+        'rtmcc': rtmcc,
+    }
 }
 
 MODEL_FULL_DICT = {
     'pidnet': pidnet
 }
 
 SUPPORTING_MODEL_LIST = list(MODEL_BACKBONE_DICT.keys()) + list(MODEL_FULL_DICT.keys())
-SUPPORTING_TASK_LIST: List[str] = ['classification', 'segmentation', 'detection']
+SUPPORTING_TASK_LIST: List[str] = ['classification', 'segmentation', 'detection', 'pose_estimation']
 
 TASK_MODEL_DICT: Dict[str, Type[TaskModel]] = {
     'classification': ClassificationModel,
     'segmentation': SegmentationModel,
-    'detection': DetectionModel
+    'detection': DetectionModel,
+    'pose_estimation': PoseEstimationModel,
 }
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/models/utils.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/models/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,51 +29,51 @@
     'mixnet_l': 'imagenet1k',
     'pidnet_s': 'cityscapes',
     'yolox_s': 'coco',
 }
 
 MODEL_CHECKPOINT_URL_DICT = {
     'resnet18': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/resnet/resnet18_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/resnet/resnet18_imagenet1k.safetensors?versionId=rI_BkIYyNFBtem180CSHA5QiGjuXgxMb",
     },
     'resnet34': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/resnet/resnet34_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/resnet/resnet34_imagenet1k.safetensors?versionId=YV687nYQc8tj5lq6ffqPpiJ8h2e0DW6L",
     },
     'resnet50': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/resnet/resnet50_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/resnet/resnet50_imagenet1k.safetensors?versionId=kDZZabJz8kK.HWDtvo7VJ.HYZ7A3GcxS",
     },
     'mobilenet_v3_small': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mobilenetv3/mobilenet_v3_small_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mobilenetv3/mobilenet_v3_small_imagenet1k.safetensors?versionId=NTpIJOERdx4efzBgY7Wcca7Xe1_Vwal9",
     },
     'segformer_b0': {
-        'undefined': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/segformer/segformer_b0.safetensors",
+        'undefined': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/segformer/segformer_b0.safetensors?versionId=aZsJLrZrAysdvqRz2WVfCrjM.0sTFs3H",
     },
     'mobilevit_s': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mobilevit/mobilevit_s_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mobilevit/mobilevit_s_imagenet1k.safetensors?versionId=Kg71H367_VeSJqfzJv54At1uFcMyIf9D",
     },
     'vit_tiny': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/vit/vit_tiny_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/vit/vit_tiny_imagenet1k.safetensors?versionId=1WC4OqtnA5gJFolvCMrOWAdmiMwpL8RO",
     },
     'efficientformer_l1': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/efficientformer/efficientformer_l1_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/efficientformer/efficientformer_l1_imagenet1k.safetensors?versionId=JIkKVaUF0fhkvLz2jfcY3MmbUg6MkUO6",
     },
     'mixnet_s': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mixnet/mixnet_s_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mixnet/mixnet_s_imagenet1k.safetensors?versionId=n0sHuieRyTWWzwBmSAE8oSP4BL53laDP",
     },
     'mixnet_m': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mixnet/mixnet_m_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mixnet/mixnet_m_imagenet1k.safetensors?versionId=cMkB57XAqu8Ro9OOWf9M6nLBPbrD2C7k",
     },
     'mixnet_l': {
-        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mixnet/mixnet_l_imagenet1k.safetensors",
+        'imagenet1k': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/mixnet/mixnet_l_imagenet1k.safetensors?versionId=UZFlpK8LO_SlYbu5GnUe9Qb3srikM6mk",
     },
     'pidnet_s': {
-        'cityscapes': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/pidnet/pidnet_s_cityscapes.safetensors",
+        'cityscapes': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/pidnet/pidnet_s_cityscapes.safetensors?versionId=lsgtDpiF1yqJpuCLYpruLdR6on0V53r8",
     },
     'yolox_s': {
-        'coco': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/yolox/yolox_s_coco.safetensors",
+        'coco': "https://netspresso-trainer-public.s3.ap-northeast-2.amazonaws.com/checkpoint/yolox/yolox_s_coco.safetensors?versionId=QRLqHKqhv8TSYBrmsQ3M8lCR8w7HEZyA",
     },
 }
 
 
 class BackboneOutput(TypedDict):
     intermediate_features: Optional[FXTensorListType]
     last_feature: Optional[FXTensorType]
@@ -117,19 +117,19 @@
     assert model_name in MODEL_CHECKPOINT_URL_DICT
 
     # TODO: User can select the specific weight version
     checkpoint_weight_version = DEFAULT_WEIGHT_VERSION_DICT[model_name]
 
     checkpoint_url = MODEL_CHECKPOINT_URL_DICT[model_name][checkpoint_weight_version]
 
-    checkpoint_filename = Path(checkpoint_url).name
+    checkpoint_filename = Path(checkpoint_url).name.split('?versionId')[0] # @illian01: Remove specified version id
     model_checkpoint: Path = DEFAULT_CACHE_DIR / model_name / checkpoint_filename
     model_checkpoint.parent.mkdir(parents=True, exist_ok=True)
     # Safer switch: only extension, user can use the custom name for checkpoint file
-    model_checkpoint = model_checkpoint.with_suffix(Path(checkpoint_url).suffix)
+    model_checkpoint = model_checkpoint.with_suffix(Path(checkpoint_filename).suffix)
     if not model_checkpoint.exists():
         torch.hub.download_url_to_file(checkpoint_url, model_checkpoint)
 
     return model_checkpoint
 
 
 def load_from_checkpoint(
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/optimizers/builder.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/builder.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/optimizers/custom.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/optimizers/custom.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/pipelines/base.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/pipelines/train.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,178 +1,132 @@
 import copy
 import json
-import os
-from abc import ABC, abstractmethod
+from ctypes import c_int
 from dataclasses import asdict
 from pathlib import Path
 from statistics import mean
-from typing import Dict, Literal, final
+from typing import Dict, List, Literal, Optional, final
 
 import torch
-import torch.distributed as dist
 import torch.nn as nn
 from loguru import logger
+from omegaconf import DictConfig
+from torch.optim.lr_scheduler import _LRScheduler
+from torch.optim.optimizer import Optimizer
+from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-from ..loggers import START_EPOCH_ZERO_OR_ONE, build_logger
-from ..losses import build_losses
-from ..metrics import build_metrics
-from ..optimizers import build_optimizer
-from ..postprocessors import build_postprocessor
-from ..schedulers import build_scheduler
+from ..loggers.base import TrainingLogger
+from ..losses.builder import LossFactory
+from ..metrics.builder import MetricFactory
 from ..utils.checkpoint import load_checkpoint, save_checkpoint
 from ..utils.fx import save_graphmodule
 from ..utils.logger import yaml_for_logging
+from ..utils.model_ema import ModelEMA
 from ..utils.onnx import save_onnx
 from ..utils.record import Timer, TrainingSummary
 from ..utils.stats import get_params_and_macs
+from .base import BasePipeline
+from .task_processors.base import BaseTaskProcessor
 
 NUM_SAMPLES = 16
 
 
-class BasePipeline(ABC):
-    def __init__(self, conf, task, model_name, model, devices,
-                 train_dataloader, eval_dataloader, class_map, logging_dir,
-                 is_graphmodule_training=False, profile=False):
-        super(BasePipeline, self).__init__()
-        self.conf = conf
-        self.task = task
-        self.model_name = model_name
-        self.save_dtype = next(model.parameters()).dtype
-        self.model = model.float()
-        self.devices = devices
+class TrainingPipeline(BasePipeline):
+    def __init__(
+        self,
+        conf: DictConfig,
+        task: str,
+        task_processor: BaseTaskProcessor,
+        model_name: str,
+        model: nn.Module,
+        logger: Optional[TrainingLogger],
+        timer: Timer,
+        optimizer: Optimizer,
+        scheduler: _LRScheduler,
+        loss_factory: LossFactory,
+        metric_factory: MetricFactory,
+        train_dataloader: DataLoader,
+        eval_dataloader: DataLoader,
+        single_gpu_or_rank_zero: bool,
+        is_graphmodule_training: bool,
+        model_ema: Optional[ModelEMA],
+        start_epoch: int,
+        cur_epoch: c_int,
+        profile: bool,
+    ):
+        super(TrainingPipeline, self).__init__(conf, task, task_processor, model_name, model, logger, timer)
+        self.optimizer = optimizer
+        self.scheduler = scheduler
+        self.loss_factory = loss_factory
+        self.metric_factory = metric_factory
         self.train_dataloader = train_dataloader
         self.eval_dataloader = eval_dataloader
-        self.train_step_per_epoch = len(train_dataloader)
+        self.single_gpu_or_rank_zero = single_gpu_or_rank_zero
+        self.is_graphmodule_training = is_graphmodule_training
+        self.model_ema = model_ema
+        self.start_epoch = start_epoch
+        self.cur_epoch = cur_epoch
+        self.profile = profile  # TODO: provide torch_tb_profiler for training
+
         self.training_history: Dict[int, Dict[
             Literal['train_losses', 'valid_losses', 'train_metrics', 'valid_metrics'], Dict[str, float]
         ]] = {}
 
-        self.timer = Timer()
-
-        self.loss_factory = None
-        self.metric_factory = None
-        self.optimizer = None
-        self.start_epoch_at_one = bool(START_EPOCH_ZERO_OR_ONE)
-        self.start_epoch = int(self.start_epoch_at_one)
-
-        self.ignore_index = None
-        self.num_classes = None
-
-        self.profile = profile  # TODO: provide torch_tb_profiler for training
-        self.is_graphmodule_training = is_graphmodule_training
-        self.save_optimizer_state = self.conf.logging.save_optimizer_state
-
-        self.single_gpu_or_rank_zero = (not self.conf.distributed) or (self.conf.distributed and dist.get_rank() == 0)
-
-        if self.single_gpu_or_rank_zero:
-            self.train_logger = build_logger(
-                self.conf, self.task, self.model_name,
-                step_per_epoch=self.train_step_per_epoch,
-                class_map=class_map,
-                num_sample_images=NUM_SAMPLES,
-                result_dir=logging_dir,
-            )
+        # TODO: These will be removed
+        self.save_optimizer_state = True
 
     @final
     def _is_ready(self):
         assert self.model is not None, "`self.model` is not defined!"
         assert self.optimizer is not None, "`self.optimizer` is not defined!"
         """Append here if you need more assertion checks!"""
         assert self.conf.logging.save_checkpoint_epoch % self.conf.logging.validation_epoch == 0, \
             "`save_checkpoint_epoch` should be the multiplier of `validation_epoch`."
         return True
 
-    def set_train(self):
-
-        assert self.model is not None
-        self.optimizer = build_optimizer(self.model,
-                                         optimizer_conf=self.conf.training.optimizer)
-        self.scheduler, _ = build_scheduler(self.optimizer, self.conf.training)
-        self.loss_factory = build_losses(self.conf.model, ignore_index=self.ignore_index)
-        self.metric_factory = build_metrics(self.task, self.conf.model, ignore_index=self.ignore_index, num_classes=self.num_classes)
-        self.postprocessor = build_postprocessor(self.task, self.conf.model)
-        resume_optimizer_checkpoint = self.conf.model.checkpoint.optimizer_path
-        if resume_optimizer_checkpoint is not None:
-            resume_optimizer_checkpoint = Path(resume_optimizer_checkpoint)
-            if not resume_optimizer_checkpoint.exists():
-                logger.warning(f"Traning summary checkpoint path {str(resume_optimizer_checkpoint)} is not found!"
-                               f"Skip loading the previous history and trainer will be started from the beginning")
-                return
-
-            optimizer_dict = torch.load(resume_optimizer_checkpoint, map_location='cpu')
-            optimizer_state_dict = optimizer_dict['optimizer']
-            start_epoch = optimizer_dict['last_epoch'] + 1  # Start from the next to the end of last training
-            start_epoch_at_one = optimizer_dict['start_epoch_at_one']
-
-            self.optimizer.load_state_dict(optimizer_state_dict)
-            self.scheduler.step(epoch=start_epoch)
-
-            self.start_epoch_at_one = start_epoch_at_one
-            self.start_epoch = start_epoch
-            logger.info(f"Resume training from {str(resume_optimizer_checkpoint)}. Start training at epoch: {self.start_epoch}")
-
     def epoch_with_valid_logging(self, epoch: int):
         validation_freq = self.conf.logging.validation_epoch
-        last_epoch = epoch == (self.conf.training.epochs + self.start_epoch_at_one - 1)
-        return (epoch % validation_freq == self.start_epoch_at_one % validation_freq) or last_epoch
+        last_epoch = epoch == self.conf.training.epochs
+        return (epoch % validation_freq == 1 % validation_freq) or last_epoch
 
     def epoch_with_checkpoint_saving(self, epoch: int):
         checkpoint_freq = self.conf.logging.save_checkpoint_epoch
-        last_epoch = epoch == (self.conf.training.epochs + self.start_epoch_at_one - 1)
-        return (epoch % checkpoint_freq == self.start_epoch_at_one % checkpoint_freq) or last_epoch
-
-    @abstractmethod
-    def train_step(self, batch):
-        raise NotImplementedError
-
-    @abstractmethod
-    def valid_step(self, batch):
-        raise NotImplementedError
-
-    @abstractmethod
-    def test_step(self, batch):
-        raise NotImplementedError
-
-    @abstractmethod
-    def get_metric_with_all_outputs(self, outputs, phase: Literal['train', 'valid']):
-        raise NotImplementedError
+        last_epoch = epoch == self.conf.training.epochs
+        return (epoch % checkpoint_freq == 1 % checkpoint_freq) or last_epoch
 
     @property
     def learning_rate(self):
         return mean([param_group['lr'] for param_group in self.optimizer.param_groups])
 
     @property
     def train_loss(self):
         return self.loss_factory.result('train').get('total').avg
 
     @property
     def valid_loss(self):
         return self.loss_factory.result('valid').get('total').avg
 
-    @property
-    def sample_input(self):
-        return torch.randn((1, 3, self.conf.augmentation.img_size, self.conf.augmentation.img_size))
-
     def train(self):
         if self.single_gpu_or_rank_zero:
             logger.debug(f"Training configuration:\n{yaml_for_logging(self.conf)}")
             logger.info("-" * 40)
 
         self.timer.start_record(name='train_all')
         self._is_ready()
 
         num_epoch = -1
         try:
-            for num_epoch in range(self.start_epoch, self.conf.training.epochs + self.start_epoch_at_one):
+            for num_epoch in range(self.start_epoch, self.conf.training.epochs + 1):
                 self.timer.start_record(name=f'train_epoch_{num_epoch}')
                 self.loss_factory.reset_values()
                 self.metric_factory.reset_values()
+                self.cur_epoch.value = num_epoch
 
-                self.train_one_epoch()
+                self.train_one_epoch(epoch=num_epoch)
 
                 with_valid_logging = self.epoch_with_valid_logging(num_epoch)
                 with_checkpoint_saving = self.epoch_with_checkpoint_saving(num_epoch)
                 # FIXME: multi-gpu sample counting & validation
                 valid_samples = self.validate() if with_valid_logging else None
 
                 self.timer.end_record(name=f'train_epoch_{num_epoch}')
@@ -192,135 +146,141 @@
                 self.scheduler.step()  # call after reporting the current `learning_rate`
 
             self.timer.end_record(name='train_all')
             total_train_time = self.timer.get(name='train_all', as_pop=False)
             logger.info(f"Total time: {total_train_time:.2f} s")
 
             if self.single_gpu_or_rank_zero:
-                self.train_logger.log_end_of_traning(final_metrics={'time_for_last_epoch': time_for_epoch})
+                self.logger.log_end_of_traning(final_metrics={'time_for_last_epoch': time_for_epoch})
+                self.save_best()
                 self.save_summary(end_training=True)
         except KeyboardInterrupt as e:
             # TODO: add independent procedure for KeyboardInterupt
             logger.error("Keyboard interrupt detected! Try saving the current checkpoint...")
             if self.single_gpu_or_rank_zero:
                 self.save_checkpoint(epoch=num_epoch)
+                self.save_best()
                 self.save_summary()
             raise e
         except Exception as e:
             logger.error(str(e))
             raise e
 
-    def train_one_epoch(self):
+    def train_one_epoch(self, epoch):
         outputs = []
         for _idx, batch in enumerate(tqdm(self.train_dataloader, leave=False)):
-            out = self.train_step(batch)
+            out = self.task_processor.train_step(self.model, batch, self.optimizer, self.loss_factory, self.metric_factory)
+            if self.model_ema:
+                self.model_ema.update(model=self.model.module if hasattr(self.model, 'module') else self.model)
             outputs.append(out)
-        self.get_metric_with_all_outputs(outputs, phase='train')
+        self.task_processor.get_metric_with_all_outputs(outputs, phase='train', metric_factory=self.metric_factory)
 
     @torch.no_grad()
     def validate(self, num_samples=NUM_SAMPLES):
         num_returning_samples = 0
         returning_samples = []
         outputs = []
+        eval_model = self.model_ema.ema_model if self.model_ema else self.model
         for _idx, batch in enumerate(tqdm(self.eval_dataloader, leave=False)):
-            out = self.valid_step(batch)
+            out = self.task_processor.valid_step(eval_model, batch, self.loss_factory, self.metric_factory)
             if out is not None:
                 outputs.append(out)
                 if num_returning_samples < num_samples:
                     returning_samples.append(out)
                     num_returning_samples += len(out['pred'])
-        self.get_metric_with_all_outputs(outputs, phase='valid')
+        self.task_processor.get_metric_with_all_outputs(outputs, phase='valid', metric_factory=self.metric_factory)
         return returning_samples
 
-    @torch.no_grad()
-    def inference(self, test_dataset):
-        returning_samples = []
-        for _idx, batch in enumerate(tqdm(test_dataset, leave=False)):
-            out = self.test_step(batch)
-            returning_samples.append(out)
-        return returning_samples
-
-    def log_end_epoch(self, epoch, time_for_epoch, valid_samples=None, valid_logging=False):
+    def log_end_epoch(
+        self,
+        epoch: int,
+        time_for_epoch: float,
+        valid_samples: Optional[List] = None,
+        valid_logging: bool = False,
+    ):
         train_losses = self.loss_factory.result('train')
         train_metrics = self.metric_factory.result('train')
+        self.log_results(prefix='training', epoch=epoch, losses=train_losses, metrics=train_metrics,
+                         learning_rate=self.learning_rate, elapsed_time=time_for_epoch)
 
-        valid_losses = self.loss_factory.result('valid') if valid_logging else None
-        valid_metrics = self.metric_factory.result('valid') if valid_logging else None
-
-        self.train_logger.update_epoch(epoch)
-        self.train_logger.log(
-            train_losses=train_losses,
-            train_metrics=train_metrics,
-            valid_losses=valid_losses,
-            valid_metrics=valid_metrics,
-            train_images=None,
-            valid_images=valid_samples,
-            learning_rate=self.learning_rate,
-            elapsed_time=time_for_epoch
-        )
+        if valid_logging:
+            valid_losses = self.loss_factory.result('valid') if valid_logging else None
+            valid_metrics = self.metric_factory.result('valid') if valid_logging else None
+            self.log_results(prefix='validation', epoch=epoch, samples=valid_samples, losses=valid_losses, metrics=valid_metrics)
 
         summary_record = {'train_losses': train_losses, 'train_metrics': train_metrics}
         if valid_logging:
             summary_record.update({'valid_losses': valid_losses, 'valid_metrics': valid_metrics})
         self.training_history.update({epoch: summary_record})
 
     def save_checkpoint(self, epoch: int):
-
-        # Check whether the valid loss is minimum at this epoch
-        valid_losses = {epoch: record['valid_losses'].get('total') for epoch, record in self.training_history.items()
-                        if 'valid_losses' in record}
-        best_epoch = min(valid_losses, key=valid_losses.get)
-        save_best_model = best_epoch == epoch
-
-        model = self.model.module if hasattr(self.model, 'module') else self.model
+        if self.model_ema:
+            model = self.model_ema.ema_model
+        else:
+            model = self.model.module if hasattr(self.model, 'module') else self.model
         if self.save_dtype == torch.float16:
             model = copy.deepcopy(model).type(self.save_dtype)
-        logging_dir = self.train_logger.result_dir
+        logging_dir = self.logger.result_dir
         model_path = Path(logging_dir) / f"{self.task}_{self.model_name}_epoch_{epoch}.ext"
-        best_model_path = Path(logging_dir) / f"{self.task}_{self.model_name}_best.ext"
         optimizer_path = Path(logging_dir) / f"{self.task}_{self.model_name}_epoch_{epoch}_optimzer.pth"
 
         if self.save_optimizer_state:
             optimizer = self.optimizer.module if hasattr(self.optimizer, 'module') else self.optimizer
-            save_dict = {'optimizer': optimizer.state_dict(), 'start_epoch_at_one': self.start_epoch_at_one, 'last_epoch': epoch}
+            save_dict = {'optimizer': optimizer.state_dict(), 'last_epoch': epoch}
             torch.save(save_dict, optimizer_path)
             logger.debug(f"Optimizer state saved at {str(optimizer_path)}")
 
         if self.is_graphmodule_training:
             # Just save graphmodule checkpoint
             torch.save(model, model_path.with_suffix(".pt"))
             logger.debug(f"PyTorch FX model saved at {str(model_path.with_suffix('.pt'))}")
-            if save_best_model:
-                save_onnx(model, best_model_path.with_suffix(".onnx"), sample_input=self.sample_input.type(self.save_dtype))
-                logger.info(f"ONNX model converting and saved at {str(best_model_path.with_suffix('.onnx'))}")
-                torch.save(model, best_model_path.with_suffix(".pt"))
-                logger.info(f"Best model saved at {str(best_model_path.with_suffix('.pt'))}")
             return
         pytorch_model_state_dict_path = model_path.with_suffix(".safetensors")
         save_checkpoint(model.state_dict(), pytorch_model_state_dict_path)
         logger.debug(f"PyTorch model saved at {str(pytorch_model_state_dict_path)}")
-        if save_best_model:
-            pytorch_best_model_state_dict_path = best_model_path.with_suffix(".safetensors")
-            save_checkpoint(model.state_dict(), pytorch_best_model_state_dict_path)
-            logger.info(f"Best model saved at {str(pytorch_best_model_state_dict_path)}")
-
-            try:
-                save_onnx(model, best_model_path.with_suffix(".onnx"), sample_input=self.sample_input.type(self.save_dtype))
-                logger.info(f"ONNX model converting and saved at {str(best_model_path.with_suffix('.onnx'))}")
-
-                save_graphmodule(model, (model_path.parent / f"{best_model_path.stem}_fx").with_suffix(".pt"))
-                logger.info(f"PyTorch FX model tracing and saved at {str(best_model_path.with_suffix('.pt'))}")
-            except Exception as e:
-                logger.error(e)
-                pass
+
+    def save_best(self):
+        valid_losses = {epoch: record['valid_losses'].get('total') for epoch, record in self.training_history.items()
+                if 'valid_losses' in record}
+        best_epoch = min(valid_losses, key=valid_losses.get)
+
+        logging_dir = self.logger.result_dir
+
+        best_checkpoint_path = Path(logging_dir) / f"{self.task}_{self.model_name}_epoch_{best_epoch}.ext"
+        best_model_save_path = Path(logging_dir) / f"{self.task}_{self.model_name}_best.ext"
+
+        model = self.model.module if hasattr(self.model, 'module') else self.model
+        best_model_to_save = copy.deepcopy(model)
+
+        if self.is_graphmodule_training:
+            best_model_to_save.load_state_dict(load_checkpoint(best_checkpoint_path.with_suffix('.pt')).state_dict())
+            save_onnx(best_model_to_save, best_model_save_path.with_suffix(".onnx"), sample_input=self.sample_input.type(self.save_dtype))
+            logger.info(f"ONNX model converting and saved at {str(best_model_save_path.with_suffix('.onnx'))}")
+            torch.save(best_model_to_save, best_model_save_path.with_suffix(".pt"))
+            logger.info(f"Best model saved at {str(best_model_save_path.with_suffix('.pt'))}")
+            return
+
+        best_model_to_save.load_state_dict(load_checkpoint(best_checkpoint_path.with_suffix('.safetensors')))
+        pytorch_best_model_state_dict_path = best_model_save_path.with_suffix(".safetensors")
+        save_checkpoint(best_model_to_save.state_dict(), pytorch_best_model_state_dict_path)
+        logger.info(f"Best model saved at {str(pytorch_best_model_state_dict_path)}")
+
+        try:
+            save_onnx(best_model_to_save, best_model_save_path.with_suffix(".onnx"), sample_input=self.sample_input.type(self.save_dtype))
+            logger.info(f"ONNX model converting and saved at {str(best_model_save_path.with_suffix('.onnx'))}")
+
+            save_graphmodule(best_model_to_save, (best_model_save_path.parent / f"{best_model_save_path.stem}_fx").with_suffix(".pt"))
+            logger.info(f"PyTorch FX model tracing and saved at {str(best_model_save_path.with_suffix('.pt'))}")
+        except Exception as e:
+            logger.error(e)
+            pass
 
     def save_summary(self, end_training=False):
         training_summary = TrainingSummary(
             total_epoch=self.conf.training.epochs,
-            start_epoch_at_one=self.start_epoch_at_one,
             train_losses={epoch: record['train_losses'].get('total') for epoch, record in self.training_history.items()},
             valid_losses={epoch: record['valid_losses'].get('total') for epoch, record in self.training_history.items()
                           if 'valid_losses' in record},
             train_metrics={epoch: record['train_metrics'] for epoch, record in self.training_history.items()},
             valid_metrics={epoch: record['valid_metrics'] for epoch, record in self.training_history.items()
                            if 'valid_metrics' in record},
             metrics_list=self.metric_factory.metric_names,
@@ -331,36 +291,36 @@
             macs, params = get_params_and_macs(self.model, self.sample_input.float())
             logger.info(f"[Model stats] Params: {(params/1e6):.2f}M | MACs: {(macs/1e9):.2f}G")
             training_summary.total_train_time = total_train_time
             training_summary.macs = macs
             training_summary.params = params
             training_summary.success = True
 
-        logging_dir = self.train_logger.result_dir
+        logging_dir = self.logger.result_dir
         summary_path = Path(logging_dir) / "training_summary.json"
 
         with open(summary_path, 'w') as f:
             json.dump(asdict(training_summary), f, indent=4)
         logger.info(f"Model training summary saved at {str(summary_path)}")
 
     def profile_one_epoch(self):
         PROFILE_WAIT = 1
         PROFILE_WARMUP = 1
         PROFILE_ACTIVE = 10
         PROFILE_REPEAT = 1
-        _ = torch.ones(1).to(self.devices)
+        #_ = torch.ones(1).to(self.devices)
         with torch.profiler.profile(
             schedule=torch.profiler.schedule(wait=PROFILE_WAIT,
                                              warmup=PROFILE_WARMUP,
                                              active=PROFILE_ACTIVE,
                                              repeat=PROFILE_REPEAT),
             on_trace_ready=torch.profiler.tensorboard_trace_handler('./log/test'),
             record_shapes=True,
             profile_memory=True,
             with_flops=True,
             with_modules=True
         ) as prof:
             for idx, batch in enumerate(self.train_dataloader):
                 if idx >= (PROFILE_WAIT + PROFILE_WARMUP + PROFILE_ACTIVE) * PROFILE_REPEAT:
                     break
-                self.train_step(batch)
+                self.task_processor.train_step(batch)
                 prof.step()
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/postprocessors/detection.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/postprocessors/detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         strides.append(torch.full((*shape, 1), stride))
 
     grids = torch.cat(grids, dim=1).type(dtype)
     strides = torch.cat(strides, dim=1).type(dtype)
 
     pred = torch.cat([
         (pred[..., 0:2] + grids) * strides,
-        torch.clamp(torch.exp(pred[..., 2:4]) * strides, min=torch.iinfo(torch.int32).min, max=torch.iinfo(torch.int32).max),
+        torch.exp(pred[..., 2:4]) * strides,
         pred[..., 4:]
     ], dim=-1)
 
     box_corner = pred.new(pred.shape)
     box_corner[:, :, 0] = pred[:, :, 0] - pred[:, :, 2] / 2
     box_corner[:, :, 1] = pred[:, :, 1] - pred[:, :, 3] / 2
     box_corner[:, :, 2] = pred[:, :, 0] + pred[:, :, 2] / 2
@@ -164,11 +164,11 @@
         pred = outputs
 
         if self.decode_outputs:
             pred = self.decode_outputs(pred, original_shape)
         if self.postprocess:
             pred = self.postprocess(pred)
 
-        pred = [(torch.cat([p[:, :4], p[:, 5:6]], dim=-1).detach().cpu().numpy(),
+        pred = [(torch.cat([p[:, :4], p[:, 4:5] * p[:, 5:6]], dim=-1).detach().cpu().numpy(),
                       p[:, 6].to(torch.int).detach().cpu().numpy())
                       for p in pred]
         return pred
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/base.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/base.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/cosine_lr.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_lr.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,16 +17,20 @@
         min_lr (float): Minimum learning rate. Originally named as `eta_min`.
     """
 
     def __init__(
         self,
         optimizer,
         scheduler_conf,
+        training_epochs,
     ):
-        self.T_max = scheduler_conf.total_iters
+        if scheduler_conf.end_epoch > training_epochs:
+            logger.warning('``training.scheduler.end_epoch`` is larger than ``training.epochs``. Automatically set scheduler end_epoch as training epochs.')
+            scheduler_conf.end_epoch = training_epochs
+        self.T_max = scheduler_conf.end_epoch
         self.eta_min = scheduler_conf.min_lr
         self.warmup_bias_lr = scheduler_conf.warmup_bias_lr
         self.warmup_iters = scheduler_conf.warmup_epochs
         super().__init__(optimizer)
 
     def get_lr(self):
         if not self._get_lr_called_within_step:
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/cosine_warm_restart.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/cosine_warm_restart.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,17 @@
         https://arxiv.org/abs/1608.03983
     """
 
     def __init__(
         self,
         optimizer,
         scheduler_conf,
+        training_epochs,
     ):
-        total_iters = scheduler_conf.total_iters
+        total_iters = training_epochs
         iters_per_phase = scheduler_conf.iters_per_phase
 
         if iters_per_phase <= 0 or not isinstance(iters_per_phase, int):
             T_0_maybe = total_iters // 10 if total_iters // 10 != 0 else total_iters
             assert T_0_maybe > 0 and isinstance(T_0_maybe, int)
             logger.info(f"Original T_0 is invalid {iters_per_phase}! Prefer to set T_0 as {T_0_maybe}.")
             iters_per_phase = T_0_maybe
@@ -61,15 +62,15 @@
 
         self.T_0 = iters_per_phase
         self.T_i = iters_per_phase
         self.T_mult = 1 # @illian01: fix as 1 for simplicity
         self.T_i, self.remain_iters = self.get_reassigned_t_i(self.T_0, self.T_i * self.T_mult, total_iters)
         self.total_iters = total_iters
         self.eta_min = scheduler_conf.min_lr
-        self.T_cur = -1 # @illian01: fix as -1 since last_epoch is set to default
+        self.T_cur = 0 # @illian01: fix as 0 since last_epoch is set to default
         self.warmup_bias_lr = scheduler_conf.warmup_bias_lr
         self.warmup_iters = scheduler_conf.warmup_epochs
         super().__init__(optimizer)
 
     def get_lr(self):
         if not self._get_lr_called_within_step:
             warnings.warn("To get the last learning rate computed by the scheduler, "
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/poly_lr.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/poly_lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
         total_iters (int): The number of steps that the scheduler decays the learning rate.
         power (int): The power of the polynomial.
     """
     def __init__(
         self,
         optimizer,
         scheduler_conf,
+        training_epochs,
     ):
         self.warmup_iters = scheduler_conf.warmup_epochs
-        self.total_iters = scheduler_conf.total_iters
+        self.total_iters = scheduler_conf.end_epoch
         self.warmup_bias_lr = scheduler_conf.warmup_bias_lr
         self.min_lr = scheduler_conf.min_lr
         self.power = scheduler_conf.power
         super().__init__(optimizer)
 
     def get_lr(self):
         if not self._get_lr_called_within_step:
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/registry.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/schedulers/step_lr.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/schedulers/step_lr.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,26 +34,28 @@
         >>>     scheduler.step()
     """
 
     def __init__(
         self,
         optimizer,
         scheduler_conf,
+        training_epochs,
     ):
         self.step_size = scheduler_conf.iters_per_phase
         self.gamma = scheduler_conf.gamma
+        self.end_epoch = scheduler_conf.end_epoch
 
         super().__init__(optimizer)
 
     def get_lr(self):
         if not self._get_lr_called_within_step:
             warnings.warn("To get the last learning rate computed by the scheduler, "
                           "please use `get_last_lr()`.", UserWarning, stacklevel=2)
 
-        if (self.last_epoch == 0) or (self.last_epoch % self.step_size != 0):
+        if (self.last_epoch > self.end_epoch) or (self.last_epoch == 0) or (self.last_epoch % self.step_size != 0):
             return [group['lr'] for group in self.optimizer.param_groups]
         return [group['lr'] * self.gamma
                 for group in self.optimizer.param_groups]
 
     def _get_closed_form_lr(self):
         return [base_lr * self.gamma ** (self.last_epoch // self.step_size)
                 for base_lr in self.base_lrs]
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/trainer_common.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/evaluator_common.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,75 +9,79 @@
 from .dataloaders import build_dataloader, build_dataset
 from .models import SUPPORTING_TASK_LIST, build_model, is_single_task_model
 from .pipelines import build_pipeline
 from .utils.environment import set_device
 from .utils.logger import add_file_handler, set_logger
 
 
-def train_common(
+def evaluation_common(
     conf: DictConfig,
     task: str,
     model_name: str,
-    is_graphmodule_training: bool,
     logging_dir: Path,
     log_level: Literal['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'] = 'INFO'
 ):
     distributed, world_size, rank, devices = set_device(conf.environment.seed)
     logger = set_logger(level=log_level, distributed=distributed)
 
     conf.distributed = distributed
     conf.world_size = world_size
     conf.rank = rank
 
     # Basic setup
     add_file_handler(logging_dir / "result.log", distributed=conf.distributed)
 
     if not distributed or dist.get_rank() == 0:
-        logger.info(f"Task: {task} | Model: {model_name} | Training with torch.fx model? {is_graphmodule_training}")
+        logger.info(f"Task: {task} | Model: {model_name}")
         logger.info(f"Result will be saved at {logging_dir}")
 
     if conf.distributed and conf.rank != 0:
         torch.distributed.barrier()  # wait for rank 0 to download dataset
 
     single_task_model = is_single_task_model(conf.model)
     conf.model.single_task_model = single_task_model
 
-    train_dataset, valid_dataset, test_dataset = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed)
+    # Build dataloader
+    _, _, test_dataset = build_dataset(conf.data, conf.augmentation, task, model_name, distributed=distributed)
+    assert test_dataset is not None, "For evaluation, valid split of dataset must be provided."
+    if not distributed or dist.get_rank() == 0:
+        logger.info(f"Summary | Dataset: <{conf.data.name}> (with {conf.data.format} format)")
+        logger.info(f"Summary | Validation dataset: {len(test_dataset)} sample(s)")
 
     if conf.distributed and conf.rank == 0:
         torch.distributed.barrier()
 
-    train_dataloader, eval_dataloader = \
-        build_dataloader(conf, task, model_name, train_dataset=train_dataset, eval_dataset=valid_dataset)
+    eval_dataloader = build_dataloader(conf, task, model_name, dataset=test_dataset, phase='val')
 
-    if is_graphmodule_training:
-        assert conf.model.checkpoint.fx_model_path is not None
-        assert Path(conf.model.checkpoint.fx_model_path).exists()
-        model = torch.load(conf.model.checkpoint.fx_model_path)
-    else:
-        model = build_model(
-            conf.model, task, train_dataset.num_classes,
-            model_checkpoint=conf.model.checkpoint.path,
-            use_pretrained=conf.model.checkpoint.use_pretrained,
-            img_size=conf.augmentation.img_size
-        )
+    # Build model
+    # TODO: Not implemented for various model types. Only support pytorch model now
+    model = build_model(
+        conf.model, task, test_dataset.num_classes,
+        model_checkpoint=conf.model.checkpoint.path,
+        use_pretrained=conf.model.checkpoint.use_pretrained,
+    )
 
     model = model.to(device=devices)
     if conf.distributed:
         model = DDP(model, device_ids=[devices], find_unused_parameters=True)  # TODO: find_unused_parameters should be false (for now, PIDNet has problem)
 
-    trainer = build_pipeline(conf, task, model_name, model,
-                             devices, train_dataloader, eval_dataloader,
-                             class_map=train_dataset.class_map,
-                             logging_dir=logging_dir,
-                             is_graphmodule_training=is_graphmodule_training)
+    # Build evaluation pipeline
+    pipeline_type = 'evaluation'
+    pipeline = build_pipeline(pipeline_type=pipeline_type,
+                              conf=conf,
+                              task=task,
+                              model_name=model_name,
+                              model=model,
+                              devices=devices,
+                              class_map=test_dataset.class_map,
+                              logging_dir=logging_dir,
+                              is_graphmodule_training=None, # TODO: Remove is_graphmodule_training ...
+                              dataloaders={'test': eval_dataloader})
 
-    trainer.set_train()
     try:
-        trainer.train()
+        # Start evaluation
+        pipeline.evaluation()
 
-        if test_dataset:
-            trainer.inference(test_dataset)
     except KeyboardInterrupt:
         pass
     except Exception as e:
         raise e
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/trainer_util.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/engine_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import argparse
 import json
 import os
 import subprocess
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import List, Literal, Optional, Tuple, Union
 
 import torch
 from omegaconf import DictConfig, OmegaConf
 
-from netspresso_trainer.cfg import TrainerConfig
-from netspresso_trainer.trainer_common import train_common
-
-from .models import SUPPORTING_TASK_LIST
+from ..models import SUPPORTING_TASK_LIST
 
 OUTPUT_ROOT_DIR = "./outputs"
-
 LOG_LEVEL = os.getenv('LOG_LEVEL', 'INFO')
 
+
 @dataclass
 class ConfigSummary:
     task: Optional[str] = None
     model_name: Optional[str] = None
     is_graphmodule_training: Optional[bool] = None
     logging_dir: Optional[Path] = None
 
+
 def str2bool(v):
     return v.lower() in ("yes", "true", "t", "1")
 
-def parse_args_netspresso(with_gpus=False):
+
+def parse_args_netspresso(with_gpus=False, isTrain=True):
 
     parser = argparse.ArgumentParser(description="Parser for NetsPresso configuration")
 
     # -------- User arguments ----------------------------------------
 
     if with_gpus:
         parser.add_argument(
@@ -51,18 +50,19 @@
         help="Config for data augmentation")
 
     parser.add_argument(
         '--model', type=str, required=True,
         dest='model',
         help="Config for the model architecture")
 
-    parser.add_argument(
-        '--training', type=str, required=True,
-        dest='training',
-        help="Config for training options")
+    if isTrain:
+        parser.add_argument(
+            '--training', type=str, required=True,
+            dest='training',
+            help="Config for training options")
 
     parser.add_argument(
         '--logging', type=str, default='config/logging.yaml',
         dest='logging',
         help="Config for logging options")
 
     parser.add_argument(
@@ -96,49 +96,14 @@
         help="")
 
     args_parsed, _ = parser.parse_known_args()
 
     return args_parsed
 
 
-def run_distributed_training_script(gpu_ids, data, augmentation, model, training, logging, environment, log_level,
-                                    task, model_name, is_graphmodule_training, logging_dir):
-
-    command = [
-        "--data", data,
-        "--augmentation", augmentation,
-        "--model", model,
-        "--training", training,
-        "--logging", logging,
-        "--environment", environment,
-        "--log-level", log_level,
-        "--task", task,
-        "--model-name", model_name,
-        "--is-graphmodule-training", is_graphmodule_training,
-        "--logging-dir", logging_dir,
-    ]
-
-    # Distributed training script
-    command = [
-        'python', '-m', 'torch.distributed.launch',
-        f'--nproc_per_node={len(gpu_ids)}',  # GPU #
-        f"{Path(__file__).absolute().parent / 'trainer_cli_multi_gpu.py'}", *map(str, command)
-    ]
-
-    # Run subprocess
-    process = subprocess.Popen(command)
-
-    try:
-        process.wait()
-    except KeyboardInterrupt:
-        print("Interrupted. Terminating the training process...")
-        process.terminate()
-        process.wait()
-
-
 def parse_gpu_ids(gpu_arg: str) -> Optional[Union[List, int]]:
     """Parse comma-separated GPU IDs and return as a list of integers."""
     if gpu_arg is None or str(gpu_arg) in ["", "None"]:
         return None
 
     try:
         gpu_ids = [int(id) for id in gpu_arg.split(',')]
@@ -148,149 +113,112 @@
 
         gpu_ids = sorted(gpu_ids)
         return gpu_ids
     except ValueError as e:
         raise argparse.ArgumentTypeError('Invalid GPU IDs. Please provide comma-separated integers.') from e
 
 
-def get_new_logging_dir(output_root_dir, project_id, initialize=True):
-    version_idx = 0
-    project_dir: Path = Path(output_root_dir) / project_id
-
-    while (project_dir / f"version_{version_idx}").exists():
-        version_idx += 1
-
-    new_logging_dir: Path = project_dir / f"version_{version_idx}"
-    new_logging_dir.mkdir(exist_ok=True, parents=True)
-
-    if initialize:
-        summary_path = new_logging_dir / "training_summary.json"
-        with open(summary_path, 'w') as f:
-            json.dump({"success": False}, f, indent=4)
-
-    return new_logging_dir
-
-
 def set_arguments(
     data: Union[Path, str],
     augmentation: Union[Path, str],
     model: Union[Path, str],
-    training: Union[Path, str],
     logging: Union[Path, str],
-    environment: Union[Path, str]
+    environment: Union[Path, str],
+    training: Optional[Union[Path, str]] = None,
 ) -> DictConfig:
 
     conf_data = OmegaConf.load(data)
     conf_augmentation = OmegaConf.load(augmentation)
     conf_model = OmegaConf.load(model)
-    conf_training = OmegaConf.load(training)
+    if training:
+        conf_training = OmegaConf.load(training)
     conf_logging = OmegaConf.load(logging)
     conf_environment = OmegaConf.load(environment)
 
     conf = OmegaConf.create()
     conf.merge_with(conf_data)
     conf.merge_with(conf_augmentation)
     conf.merge_with(conf_model)
-    conf.merge_with(conf_training)
+    if training:
+        conf.merge_with(conf_training)
     conf.merge_with(conf_logging)
     conf.merge_with(conf_environment)
 
     return conf
 
-def validate_config(conf: DictConfig) -> ConfigSummary:
+
+def get_gpu_from_config(conf_environment: DictConfig) -> Optional[Union[List, int]]:
+    conf_environment_gpus = str(conf_environment.gpus) if hasattr(conf_environment, 'gpus') else None
+    return parse_gpu_ids(conf_environment_gpus)
+
+
+def get_gpus_from_parser_and_config(
+    gpus: Optional[Union[List, int]],
+    conf_environment: DictConfig
+) -> Union[List, int]:
+    conf_environment_gpus = get_gpu_from_config(conf_environment)
+    if gpus is None:
+        if conf_environment_gpus is None:
+            return 0  # Try use the 'cuda:0'
+        return conf_environment_gpus
+    return gpus
+
+
+def get_new_logging_dir(output_root_dir, project_id, mode: Literal['training', 'evaluation', 'inference']):
+    version_idx = 0
+    project_dir: Path = Path(output_root_dir) / project_id
+
+    while (project_dir / f"version_{version_idx}").exists():
+        version_idx += 1
+
+    new_logging_dir: Path = project_dir / f"version_{version_idx}"
+    new_logging_dir.mkdir(exist_ok=True, parents=True)
+
+    summary_path = new_logging_dir / f"{mode}_summary.json"
+    with open(summary_path, 'w') as f:
+        json.dump({"success": False}, f, indent=4)
+
+    return new_logging_dir
+
+
+def validate_train_config(conf: DictConfig) -> ConfigSummary:
     # Get information from configuration
     is_graphmodule_training = bool(conf.model.checkpoint.fx_model_path)
 
     task = str(conf.model.task).lower()
     assert task in SUPPORTING_TASK_LIST
 
     model_name = str(conf.model.name).lower()
 
     if is_graphmodule_training:
         model_name += "_graphmodule"
 
     project_id = conf.logging.project_id if conf.logging.project_id is not None else f"{task}_{model_name}"
-    logging_dir: Path = get_new_logging_dir(output_root_dir="./outputs", project_id=project_id)
+    logging_dir: Path = get_new_logging_dir(output_root_dir=conf.logging.output_dir, project_id=project_id, mode='training')
 
     return ConfigSummary(task=task, model_name=model_name, is_graphmodule_training=is_graphmodule_training, logging_dir=logging_dir)
 
-def set_struct_recursive(conf: DictConfig, value: bool) -> None:
-    OmegaConf.set_struct(conf, value)
 
-    for _, conf_value in conf.items():
-        if isinstance(conf_value, DictConfig):
-            set_struct_recursive(conf_value, value)
+def validate_evaluation_config(conf: DictConfig) -> ConfigSummary:
 
-def get_gpu_from_config(conf_environment: DictConfig) -> Optional[Union[List, int]]:
-    conf_environment_gpus = str(conf_environment.gpus) if hasattr(conf_environment, 'gpus') else None
-    return parse_gpu_ids(conf_environment_gpus)
+    task = str(conf.model.task).lower()
+    assert task in SUPPORTING_TASK_LIST
 
+    model_name = str(conf.model.name).lower() + '_evaluation'
 
-def get_gpus_from_parser_and_config(
-    gpus: Optional[Union[List, int]],
-    conf_environment: DictConfig
-) -> Union[List, int]:
-    conf_environment_gpus = get_gpu_from_config(conf_environment)
-    if gpus is None:
-        if conf_environment_gpus is None:
-            return 0  # Try use the 'cuda:0'
-        return conf_environment_gpus
-    return gpus
+    project_id = conf.logging.project_id if conf.logging.project_id is not None else f"{task}_{model_name}"
+    logging_dir: Path = get_new_logging_dir(output_root_dir=conf.logging.output_dir, project_id=project_id, mode='evaluation')
 
+    return ConfigSummary(task=task, model_name=model_name, is_graphmodule_training=None, logging_dir=logging_dir)
 
-def train_with_yaml_impl(gpus: Optional[Union[List, int]], data: Union[Path, str], augmentation: Union[Path, str],
-                         model: Union[Path, str], training: Union[Path, str],
-                         logging: Union[Path, str], environment: Union[Path, str], log_level: str = LOG_LEVEL):
-    conf_environment = OmegaConf.load(environment).environment
-    gpus = get_gpus_from_parser_and_config(gpus, conf_environment)
-    assert isinstance(gpus, (list, int))
-
-    gpu_ids_str = ','.join(map(str, gpus)) if isinstance(gpus, list) else str(gpus)
-    os.environ['CUDA_VISIBLE_DEVICES'] = gpu_ids_str
-    torch.cuda.empty_cache()  # Reinitialize CUDA to apply the change
 
-    conf = set_arguments(data, augmentation, model, training, logging, environment)
-    config_summary = validate_config(conf)
+def validate_inference_config(conf: DictConfig) -> ConfigSummary:
 
-    try:
-        if isinstance(gpus, int):
-            train_common(
-                conf,
-                task=config_summary.task,
-                model_name=config_summary.model_name,
-                is_graphmodule_training=config_summary.is_graphmodule_training,
-                logging_dir=config_summary.logging_dir,
-                log_level=log_level
-            )
-        else:
-            run_distributed_training_script(
-                gpus, data, augmentation, model, training, logging, environment, log_level,
-                config_summary.task, config_summary.model_name, config_summary.is_graphmodule_training, config_summary.logging_dir
-            )
-        return config_summary.logging_dir
-    except Exception as e:
-        raise e
-
-def train_with_config_impl(gpus: int, config: TrainerConfig, log_level: str = LOG_LEVEL):
-
-    gpus = get_gpus_from_parser_and_config(gpus, config.environment)
-    assert isinstance(gpus, int), f"Currently, only single-GPU training is supported in this API. Your gpu(s): {gpus}"
-
-    os.environ['CUDA_VISIBLE_DEVICES'] = str(gpus)
-    torch.cuda.empty_cache()  # Reinitialize CUDA to apply the change
-
-    conf: DictConfig = OmegaConf.create(config)
-    set_struct_recursive(conf, False)
-    config_summary = validate_config(conf)
+    task = str(conf.model.task).lower()
+    assert task in SUPPORTING_TASK_LIST
 
-    try:
-        train_common(
-            conf,
-            task=config_summary.task,
-            model_name=config_summary.model_name,
-            is_graphmodule_training=config_summary.is_graphmodule_training,
-            logging_dir=config_summary.logging_dir,
-            log_level=log_level
-        )
-        return config_summary.logging_dir
-    except Exception as e:
-        raise e
+    model_name = str(conf.model.name).lower() + '_inference'
+
+    project_id = conf.logging.project_id if conf.logging.project_id is not None else f"{task}_{model_name}"
+    logging_dir: Path = get_new_logging_dir(output_root_dir=conf.logging.output_dir, project_id=project_id, mode='inference')
+
+    return ConfigSummary(task=task, model_name=model_name, is_graphmodule_training=None, logging_dir=logging_dir)
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/utils/checkpoint.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/utils/environment.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/environment.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/utils/fx.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/fx.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/utils/logger.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/logger.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/utils/onnx.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/utils/record.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/record.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,43 @@
         return fmtstr.format(**self.__dict__)
 
     @property
     def avg(self) -> float:
         return self._avg
 
 
+class MetricMeter(object):
+    """Computes and stores the average and current value"""
+
+    def __init__(self, name: str, fmt=':f'):
+        self.name = name
+        self.fmt = fmt
+        self.reset()
+
+    def reset(self):
+        self._val: float = 0.
+        self._avg: float = 0.
+        self._sum: float = 0.
+        self._count: int = 0
+
+    def update(self, val: Union[float, int], n: int = 1) -> None:
+        self._val = val
+        self._sum += val
+        self._count += n
+        self._avg = self._sum / self._count
+
+    def __str__(self):
+        fmtstr = '{name} {val' + self.fmt + '} ({avg' + self.fmt + '})'
+        return fmtstr.format(**self.__dict__)
+
+    @property
+    def avg(self) -> float:
+        return self._avg
+
+
 class TimeRecode:
     def __init__(self) -> None:
         self._start = time.time()
         self._end = None
 
     def end(self) -> None:
         self._end = time.time()
@@ -92,18 +121,37 @@
     total_epoch: int
     train_losses: TYPE_SUMMARY_RECORD
     valid_losses: TYPE_SUMMARY_RECORD
     train_metrics: TYPE_SUMMARY_RECORD
     valid_metrics: TYPE_SUMMARY_RECORD
     metrics_list: List[str]
     primary_metric: str
-    start_epoch_at_one: bool
     macs: Optional[int] = None
     params: Optional[int] = None
     total_train_time: Optional[float] = None
     best_epoch: int = field(init=False)
     last_epoch: int = field(init=False)
     success: bool = False
 
     def __post_init__(self):
         self.best_epoch = min(self.valid_losses, key=self.valid_losses.get)
         self.last_epoch = list(self.train_losses.keys())[-1]
+
+
+@dataclass
+class EvaluationSummary:
+    losses: float
+    metrics: float
+    metrics_list: List[str]
+    primary_metric: str
+    macs: Optional[int] = None
+    params: Optional[int] = None
+    total_evaluation_time: Optional[float] = None
+    success: bool = False
+
+
+@dataclass
+class InferenceSummary:
+    macs: Optional[int] = None
+    params: Optional[int] = None
+    total_inference_time: Optional[float] = None
+    success: bool = False
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer/utils/stats.py` & `netspresso_trainer-0.2.0/src/netspresso_trainer/utils/stats.py`

 * *Files identical despite different names*

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/PKG-INFO` & `netspresso_trainer-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: netspresso-trainer
-Version: 0.1.2
+Name: netspresso_trainer
+Version: 0.2.0
 Summary: NetsPresso Python Package
 Home-page: https://github.com/Nota-NetsPresso/netspresso-trainer
 Author: NetsPresso
 Author-email: netspresso@nota.ai
 License: UNKNOWN
 Description: <div align="center">
             <img src="./assets/netspresso_trainer_header_tmp.png" width="800"/>
@@ -24,24 +24,54 @@
           <a href="https://github.com/Nota-NetsPresso/netspresso-trainer/issues">Issues</a> •
           <a href="https://nota-netspresso.github.io/netspresso-trainer">Docs</a>
         </p>
         </div>
         
         _____
         
-        
         ## Table of contents
         
         <!-- toc -->
         
-        - [Getting started](#getting-started)
         - [Installation](#installation)
+        - [Getting started](#getting-started)
         
         <!-- tocstop -->
         
+        ## Installation (Stable)
+        
+        ### Prerequisites
+        
+        - Python `3.8` | `3.9` | `3.10`
+        - PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
+        
+        ### Install with pypi
+        
+        ```bash
+        pip install netspresso_trainer
+        ```
+        
+        ### Install with GitHub
+        
+        ```bash
+        pip install git+https://github.com/Nota-NetsPresso/netspresso-trainer.git@master
+        ```
+        
+        To install with editable mode,
+        
+        ```bash
+        git clone -b master https://github.com/Nota-NetsPresso/netspresso-trainer.git
+        pip install -e netspresso-trainer
+        ```
+        
+        ### Set-up with docker
+        
+        Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
+        For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
+        
         ## Getting started
         
         Write your training script in `train.py` like:
         
         ```python
         from netspresso_trainer import train_cli
         
@@ -74,45 +104,14 @@
           --environment config/environment.yaml
         ```
         
         Please refer to [`scripts/example_train.sh`](./scripts/example_train.sh).
         
         NetsPresso Trainer is compatible with [NetsPresso](https://netspresso.ai/) service. We provide NetsPresso Trainer tutorial that contains whole procedure from model train to model compression and benchmark. Please refer to our [colab tutorial](https://colab.research.google.com/drive/1RBKMCPEa4x-4X31zqzTS8WgQI9TQt3e-?usp=sharing).
         
-        ## Installation
-        
-        ### Prerequisites
-        
-        - Python `3.8` | `3.9` | `3.10`
-        - PyTorch `1.13.0` (recommended) (compatible with: `1.11.x` - `1.13.x`)
-        
-        ### Install with pypi (stable)
-        
-        ```bash
-        pip install netspresso_trainer
-        ```
-        
-        ### Install with GitHub
-        
-        ```bash
-        pip install git+https://github.com:Nota-NetsPresso/netspresso-trainer.git@stable
-        ```
-        
-        To install with editable mode,
-        
-        ```bash
-        git clone https://github.com:Nota-NetsPresso/netspresso-trainer.git .
-        pip install -e netspresso-trainer
-        ```
-        
-        ### Set-up with docker
-        
-        Please clone this repository and refer to [`Dockerfile`](./Dockerfile) and [`docker-compose-example.yml`](./docker-compose-example.yml).  
-        For docker users, we provide more detailed guide in our [Docs](https://nota-netspresso.github.io/netspresso-trainer).
-        
         ## Tensorboard
         
         We provide basic tensorboard to track your training status. Run the tensorboard with the following command: 
         
         ```bash
         tensorboard --logdir ./outputs --port 50001 --bind_all
         ```
```

### Comparing `netspresso_trainer-0.1.2/src/netspresso_trainer.egg-info/SOURCES.txt` & `netspresso_trainer-0.2.0/src/netspresso_trainer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,94 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/netspresso_trainer/VERSION
 src/netspresso_trainer/__init__.py
-src/netspresso_trainer/trainer_cli.py
-src/netspresso_trainer/trainer_cli_multi_gpu.py
+src/netspresso_trainer/evaluator_common.py
+src/netspresso_trainer/evaluator_main.py
+src/netspresso_trainer/inferencer_common.py
+src/netspresso_trainer/inferencer_main.py
 src/netspresso_trainer/trainer_common.py
-src/netspresso_trainer/trainer_inline.py
-src/netspresso_trainer/trainer_util.py
+src/netspresso_trainer/trainer_main.py
 src/netspresso_trainer.egg-info/PKG-INFO
 src/netspresso_trainer.egg-info/SOURCES.txt
 src/netspresso_trainer.egg-info/dependency_links.txt
 src/netspresso_trainer.egg-info/entry_points.txt
 src/netspresso_trainer.egg-info/requires.txt
 src/netspresso_trainer.egg-info/top_level.txt
-src/netspresso_trainer/cfg/__init__.py
-src/netspresso_trainer/cfg/augmentation.py
-src/netspresso_trainer/cfg/data.py
-src/netspresso_trainer/cfg/environment.py
-src/netspresso_trainer/cfg/logging.py
-src/netspresso_trainer/cfg/model.py
-src/netspresso_trainer/cfg/training.py
 src/netspresso_trainer/dataloaders/__init__.py
 src/netspresso_trainer/dataloaders/base.py
 src/netspresso_trainer/dataloaders/builder.py
 src/netspresso_trainer/dataloaders/registry.py
 src/netspresso_trainer/dataloaders/augmentation/__init__.py
-src/netspresso_trainer/dataloaders/augmentation/custom.py
 src/netspresso_trainer/dataloaders/augmentation/registry.py
 src/netspresso_trainer/dataloaders/augmentation/transforms.py
+src/netspresso_trainer/dataloaders/augmentation/custom/__init__.py
+src/netspresso_trainer/dataloaders/augmentation/custom/image_proc.py
+src/netspresso_trainer/dataloaders/augmentation/custom/mixing.py
+src/netspresso_trainer/dataloaders/augmentation/custom/mosaic.py
 src/netspresso_trainer/dataloaders/classification/__init__.py
 src/netspresso_trainer/dataloaders/classification/dataset.py
 src/netspresso_trainer/dataloaders/classification/huggingface.py
 src/netspresso_trainer/dataloaders/classification/local.py
 src/netspresso_trainer/dataloaders/detection/__init__.py
 src/netspresso_trainer/dataloaders/detection/dataset.py
 src/netspresso_trainer/dataloaders/detection/local.py
+src/netspresso_trainer/dataloaders/pose_estimation/__init__.py
+src/netspresso_trainer/dataloaders/pose_estimation/dataset.py
+src/netspresso_trainer/dataloaders/pose_estimation/local.py
 src/netspresso_trainer/dataloaders/segmentation/__init__.py
 src/netspresso_trainer/dataloaders/segmentation/dataset.py
 src/netspresso_trainer/dataloaders/segmentation/huggingface.py
 src/netspresso_trainer/dataloaders/segmentation/local.py
 src/netspresso_trainer/dataloaders/utils/__init__.py
 src/netspresso_trainer/dataloaders/utils/constants.py
 src/netspresso_trainer/dataloaders/utils/loader.py
 src/netspresso_trainer/dataloaders/utils/misc.py
+src/netspresso_trainer/dataloaders/utils/sampler.py
 src/netspresso_trainer/loggers/__init__.py
 src/netspresso_trainer/loggers/base.py
 src/netspresso_trainer/loggers/builder.py
-src/netspresso_trainer/loggers/csv.py
 src/netspresso_trainer/loggers/image.py
-src/netspresso_trainer/loggers/netspresso.py
 src/netspresso_trainer/loggers/registry.py
 src/netspresso_trainer/loggers/stdout.py
 src/netspresso_trainer/loggers/tensorboard.py
 src/netspresso_trainer/loggers/visualizer.py
 src/netspresso_trainer/losses/__init__.py
 src/netspresso_trainer/losses/builder.py
 src/netspresso_trainer/losses/common.py
 src/netspresso_trainer/losses/registry.py
 src/netspresso_trainer/losses/classification/__init__.py
 src/netspresso_trainer/losses/detection/__init__.py
 src/netspresso_trainer/losses/detection/retinanet.py
 src/netspresso_trainer/losses/detection/yolox.py
+src/netspresso_trainer/losses/pose_estimation/__init__.py
+src/netspresso_trainer/losses/pose_estimation/rtmcc.py
 src/netspresso_trainer/losses/segmentation/__init__.py
 src/netspresso_trainer/losses/segmentation/pidnet.py
 src/netspresso_trainer/metrics/__init__.py
 src/netspresso_trainer/metrics/base.py
 src/netspresso_trainer/metrics/builder.py
 src/netspresso_trainer/metrics/registry.py
 src/netspresso_trainer/metrics/classification/__init__.py
 src/netspresso_trainer/metrics/classification/metric.py
 src/netspresso_trainer/metrics/detection/__init__.py
 src/netspresso_trainer/metrics/detection/metric.py
+src/netspresso_trainer/metrics/pose_estimation/__init__.py
+src/netspresso_trainer/metrics/pose_estimation/metric.py
 src/netspresso_trainer/metrics/segmentation/__init__.py
 src/netspresso_trainer/metrics/segmentation/metric.py
 src/netspresso_trainer/models/__init__.py
 src/netspresso_trainer/models/base.py
 src/netspresso_trainer/models/builder.py
 src/netspresso_trainer/models/registry.py
 src/netspresso_trainer/models/utils.py
 src/netspresso_trainer/models/backbones/__init__.py
+src/netspresso_trainer/models/backbones/registry.py
 src/netspresso_trainer/models/backbones/core/__init__.py
 src/netspresso_trainer/models/backbones/core/resnet.py
 src/netspresso_trainer/models/backbones/experimental/__init__.py
 src/netspresso_trainer/models/backbones/experimental/darknet.py
 src/netspresso_trainer/models/backbones/experimental/efficientformer.py
 src/netspresso_trainer/models/backbones/experimental/mixnet.py
 src/netspresso_trainer/models/backbones/experimental/mixtransformer.py
@@ -103,14 +107,18 @@
 src/netspresso_trainer/models/heads/detection/__init__.py
 src/netspresso_trainer/models/heads/detection/core/__init__.py
 src/netspresso_trainer/models/heads/detection/experimental/__init__.py
 src/netspresso_trainer/models/heads/detection/experimental/anchor_decoupled_head.py
 src/netspresso_trainer/models/heads/detection/experimental/anchor_free_decoupled_head.py
 src/netspresso_trainer/models/heads/detection/experimental/detection/__init__.py
 src/netspresso_trainer/models/heads/detection/experimental/detection/anchor_generator.py
+src/netspresso_trainer/models/heads/pose_estimation/__init__.py
+src/netspresso_trainer/models/heads/pose_estimation/core/__init__.py
+src/netspresso_trainer/models/heads/pose_estimation/experimental/__init__.py
+src/netspresso_trainer/models/heads/pose_estimation/experimental/rtmcc.py
 src/netspresso_trainer/models/heads/segmentation/__init__.py
 src/netspresso_trainer/models/heads/segmentation/core/__init__.py
 src/netspresso_trainer/models/heads/segmentation/experimental/__init__.py
 src/netspresso_trainer/models/heads/segmentation/experimental/all_mlp_decoder.py
 src/netspresso_trainer/models/necks/__init__.py
 src/netspresso_trainer/models/necks/core/__init__.py
 src/netspresso_trainer/models/necks/experimental/__init__.py
@@ -125,33 +133,42 @@
 src/netspresso_trainer/optimizers/__init__.py
 src/netspresso_trainer/optimizers/builder.py
 src/netspresso_trainer/optimizers/custom.py
 src/netspresso_trainer/optimizers/registry.py
 src/netspresso_trainer/pipelines/__init__.py
 src/netspresso_trainer/pipelines/base.py
 src/netspresso_trainer/pipelines/builder.py
-src/netspresso_trainer/pipelines/classification.py
-src/netspresso_trainer/pipelines/detection.py
+src/netspresso_trainer/pipelines/evaluation.py
+src/netspresso_trainer/pipelines/inference.py
 src/netspresso_trainer/pipelines/registry.py
-src/netspresso_trainer/pipelines/segmentation.py
+src/netspresso_trainer/pipelines/train.py
+src/netspresso_trainer/pipelines/task_processors/__init__.py
+src/netspresso_trainer/pipelines/task_processors/base.py
+src/netspresso_trainer/pipelines/task_processors/classification.py
+src/netspresso_trainer/pipelines/task_processors/detection.py
+src/netspresso_trainer/pipelines/task_processors/pose_estimation.py
+src/netspresso_trainer/pipelines/task_processors/segmentation.py
 src/netspresso_trainer/postprocessors/__init__.py
 src/netspresso_trainer/postprocessors/builder.py
 src/netspresso_trainer/postprocessors/classification.py
 src/netspresso_trainer/postprocessors/detection.py
+src/netspresso_trainer/postprocessors/pose_estimation.py
 src/netspresso_trainer/postprocessors/register.py
 src/netspresso_trainer/postprocessors/segmentation.py
 src/netspresso_trainer/schedulers/__init__.py
 src/netspresso_trainer/schedulers/base.py
 src/netspresso_trainer/schedulers/builder.py
 src/netspresso_trainer/schedulers/cosine_lr.py
 src/netspresso_trainer/schedulers/cosine_warm_restart.py
 src/netspresso_trainer/schedulers/poly_lr.py
 src/netspresso_trainer/schedulers/registry.py
 src/netspresso_trainer/schedulers/step_lr.py
 src/netspresso_trainer/utils/__init__.py
 src/netspresso_trainer/utils/checkpoint.py
+src/netspresso_trainer/utils/engine_utils.py
 src/netspresso_trainer/utils/environment.py
 src/netspresso_trainer/utils/fx.py
 src/netspresso_trainer/utils/logger.py
+src/netspresso_trainer/utils/model_ema.py
 src/netspresso_trainer/utils/onnx.py
 src/netspresso_trainer/utils/record.py
 src/netspresso_trainer/utils/stats.py
```

