# Comparing `tmp/2404-segmentation-pipeline-0.1.2.tar.gz` & `tmp/2404-segmentation-pipeline-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2404-segmentation-pipeline-0.1.2.tar", last modified: Tue Apr  9 18:13:23 2024, max compression
+gzip compressed data, was "2404-segmentation-pipeline-1.0.0.tar", last modified: Mon Apr 15 06:15:58 2024, max compression
```

## Comparing `2404-segmentation-pipeline-0.1.2.tar` & `2404-segmentation-pipeline-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jo         (501) staff       (20)        0 2024-04-09 18:13:23.042127 2404-segmentation-pipeline-0.1.2/
-drwxr-xr-x   0 jo         (501) staff       (20)        0 2024-04-09 18:13:23.040961 2404-segmentation-pipeline-0.1.2/2404_segmentation_pipeline.egg-info/
--rw-r--r--   0 jo         (501) staff       (20)     5084 2024-04-09 18:13:23.000000 2404-segmentation-pipeline-0.1.2/2404_segmentation_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 jo         (501) staff       (20)      309 2024-04-09 18:13:23.000000 2404-segmentation-pipeline-0.1.2/2404_segmentation_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 jo         (501) staff       (20)        1 2024-04-09 18:13:23.000000 2404-segmentation-pipeline-0.1.2/2404_segmentation_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 jo         (501) staff       (20)      142 2024-04-09 18:13:23.000000 2404-segmentation-pipeline-0.1.2/2404_segmentation_pipeline.egg-info/requires.txt
--rw-r--r--   0 jo         (501) staff       (20)        9 2024-04-09 18:13:23.000000 2404-segmentation-pipeline-0.1.2/2404_segmentation_pipeline.egg-info/top_level.txt
--rw-r--r--   0 jo         (501) staff       (20)     5084 2024-04-09 18:13:23.042015 2404-segmentation-pipeline-0.1.2/PKG-INFO
--rw-r--r--   0 jo         (501) staff       (20)     4777 2024-04-09 16:32:43.000000 2404-segmentation-pipeline-0.1.2/README.md
-drwxr-xr-x   0 jo         (501) staff       (20)        0 2024-04-09 18:13:23.041253 2404-segmentation-pipeline-0.1.2/pipeline/
--rw-r--r--   0 jo         (501) staff       (20)       55 2024-04-09 00:37:33.000000 2404-segmentation-pipeline-0.1.2/pipeline/__init__.py
--rw-r--r--   0 jo         (501) staff       (20)    20185 2024-04-09 16:32:44.000000 2404-segmentation-pipeline-0.1.2/pipeline/pipeline.py
--rw-r--r--   0 jo         (501) staff       (20)       38 2024-04-09 18:13:23.042165 2404-segmentation-pipeline-0.1.2/setup.cfg
--rw-r--r--   0 jo         (501) staff       (20)      710 2024-04-09 18:12:29.000000 2404-segmentation-pipeline-0.1.2/setup.py
+drwxr-xr-x   0 jo         (501) staff       (20)        0 2024-04-15 06:15:58.476046 2404-segmentation-pipeline-1.0.0/
+drwxr-xr-x   0 jo         (501) staff       (20)        0 2024-04-15 06:15:58.475144 2404-segmentation-pipeline-1.0.0/2404_segmentation_pipeline.egg-info/
+-rw-r--r--   0 jo         (501) staff       (20)     5084 2024-04-15 06:15:58.000000 2404-segmentation-pipeline-1.0.0/2404_segmentation_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 jo         (501) staff       (20)      309 2024-04-15 06:15:58.000000 2404-segmentation-pipeline-1.0.0/2404_segmentation_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 jo         (501) staff       (20)        1 2024-04-15 06:15:58.000000 2404-segmentation-pipeline-1.0.0/2404_segmentation_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 jo         (501) staff       (20)      142 2024-04-15 06:15:58.000000 2404-segmentation-pipeline-1.0.0/2404_segmentation_pipeline.egg-info/requires.txt
+-rw-r--r--   0 jo         (501) staff       (20)        9 2024-04-15 06:15:58.000000 2404-segmentation-pipeline-1.0.0/2404_segmentation_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 jo         (501) staff       (20)     5084 2024-04-15 06:15:58.475897 2404-segmentation-pipeline-1.0.0/PKG-INFO
+-rw-r--r--   0 jo         (501) staff       (20)     4777 2024-04-09 16:32:43.000000 2404-segmentation-pipeline-1.0.0/README.md
+drwxr-xr-x   0 jo         (501) staff       (20)        0 2024-04-15 06:15:58.475566 2404-segmentation-pipeline-1.0.0/pipeline/
+-rw-r--r--   0 jo         (501) staff       (20)       55 2024-04-09 00:37:33.000000 2404-segmentation-pipeline-1.0.0/pipeline/__init__.py
+-rw-r--r--   0 jo         (501) staff       (20)    20881 2024-04-15 06:13:26.000000 2404-segmentation-pipeline-1.0.0/pipeline/pipeline.py
+-rw-r--r--   0 jo         (501) staff       (20)       38 2024-04-15 06:15:58.476104 2404-segmentation-pipeline-1.0.0/setup.cfg
+-rw-r--r--   0 jo         (501) staff       (20)      710 2024-04-15 06:15:52.000000 2404-segmentation-pipeline-1.0.0/setup.py
```

### Comparing `2404-segmentation-pipeline-0.1.2/2404_segmentation_pipeline.egg-info/PKG-INFO` & `2404-segmentation-pipeline-1.0.0/2404_segmentation_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 2404-segmentation-pipeline
-Version: 0.1.2
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: https://github.com/2404-Organ-Segmentation/segmentation-pipeline
 Author: 2404 Organ Segmentation
 Author-email: joey.xiang426@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `2404-segmentation-pipeline-0.1.2/PKG-INFO` & `2404-segmentation-pipeline-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 2404-segmentation-pipeline
-Version: 0.1.2
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: https://github.com/2404-Organ-Segmentation/segmentation-pipeline
 Author: 2404 Organ Segmentation
 Author-email: joey.xiang426@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `2404-segmentation-pipeline-0.1.2/README.md` & `2404-segmentation-pipeline-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `2404-segmentation-pipeline-0.1.2/pipeline/pipeline.py` & `2404-segmentation-pipeline-1.0.0/pipeline/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     EnsureTyped,
     Activationsd,
     Invertd,
     AsDiscreted,
     SaveImaged,
     KeepLargestConnectedComponentd,
 )
-from monai.metrics import DiceMetric
+from monai.metrics import DiceMetric, MeanIoU, MAEMetric
 from monai.losses import DiceCELoss
 from monai.inferers import sliding_window_inference
 import torch
 import re
 import nibabel as nib
 import os
 from tqdm import tqdm
@@ -139,18 +139,18 @@
             data=datalist,
             transform=train_transforms,
             cache_num=cache_num_train,
             cache_rate=1.0,
             num_workers=workers,
         )
         train_loader = DataLoader(train_ds, batch_size=train_batch_size, shuffle=True, num_workers=workers,
-                                  pin_memory=True)
+                                  pin_memory=False)
         val_ds = CacheDataset(data=val_files, transform=val_transforms, cache_num=cache_num_val, cache_rate=1.0,
                               num_workers=workers)
-        val_loader = DataLoader(val_ds, batch_size=val_batch_size, shuffle=False, num_workers=workers, pin_memory=True)
+        val_loader = DataLoader(val_ds, batch_size=val_batch_size, shuffle=False, num_workers=workers, pin_memory=False)
 
         self.train_transforms = train_transforms
         self.val_transforms = val_transforms
 
         f = open(dataset_path)
         json_data = json.load(f)
 
@@ -184,15 +184,17 @@
 
         max_iterations = math.ceil(max_epoch * self.num_train_images / self.train_batch_size)
         eval_num = math.ceil(epoch_val * self.num_train_images / self.train_batch_size)
         post_label = AsDiscrete(to_onehot=self.num_of_labels)
         post_pred = AsDiscrete(argmax=True, to_onehot=self.num_of_labels)
 
         dice_metric = DiceMetric(include_background=True, reduction="mean", get_not_nans=False)
-
+        iou_metric = MeanIoU(include_background=True)
+        pixel_metric = MAEMetric()
+        
         save_folder = self.model_type + self.dataset_name + str(datetime.now().strftime("%Y_%m_%d_%H_%M_%S"))
         os.makedirs(save_folder)
         os.makedirs(save_folder + "/logs")
         writer = SummaryWriter(save_folder + '/logs/{}'.format(datetime.now().strftime("%Y_%m_%d")))
 
         global_step = 0
         dice_val_best = 0.0
@@ -210,22 +212,28 @@
                     val_labels_list = decollate_batch(val_labels)
                     val_labels_convert = [post_label(val_label_tensor) for val_label_tensor in val_labels_list]
                     val_outputs_list = decollate_batch(val_outputs)
                     val_output_convert = [post_pred(val_pred_tensor) for val_pred_tensor in val_outputs_list]
 
                     # Calculate metrics
                     dice_metric(y_pred=val_output_convert, y=val_labels_convert)
+                    iou_metric(y_pred=val_output_convert, y=val_labels_convert)
+                    pixel_metric(y_pred=val_output_convert, y=val_labels_convert)
 
                     epoch_iterator_val.set_description(
                         "Validate (%d / %d Steps)" % (global_step, max_iterations))  # noqa: B038
                 mean_dice_val = dice_metric.aggregate().item()
+                mean_iou = iou_metric.aggregate().item()
+                pixel_error = pixel_metric.aggregate().item()
 
                 dice_metric.reset()
+                iou_metric.reset()
+                pixel_metric.reset()
 
-            return mean_dice_val
+            return mean_dice_val, mean_iou, pixel_error
 
         def __train(global_step, train_loader, dice_val_best, global_step_best):
             self.model.train()
             epoch_loss = 0
             step = 0
             epoch_iterator = tqdm(train_loader, desc="Training (X / X Steps) (loss=X.X)", dynamic_ncols=True)
             for step, batch in enumerate(epoch_iterator):
@@ -243,15 +251,15 @@
                 epoch_iterator.set_description( 
                     f"Training ({global_step} / {max_iterations} Steps) (loss={loss:2.5f})"
                 )
 
                 if (global_step % eval_num == 0 and global_step != 0) or global_step == max_iterations:
                     epoch_iterator_val = tqdm(self.val_loader, desc="Validate (X / X Steps) (dice=X.X)",
                                               dynamic_ncols=True)
-                    dice_val = __validation(epoch_iterator_val)
+                    dice_val, iou_val, pixel_err_val = __validation(epoch_iterator_val)
                     epoch_loss /= step
                     epoch_loss_values.append(epoch_loss)
                     metric_values.append(dice_val)
                     if dice_val > dice_val_best:
                         dice_val_best = dice_val
                         global_step_best = global_step
 
@@ -260,14 +268,16 @@
                                             self.model_type + self.dataset_name + str(global_step) + ".pth"))
                     print(
                         "Model Was Saved ! Current Best Avg. Dice: {} Current Avg. Dice: {}".format(dice_val_best,
                                                                                                     dice_val)
                     )
                     # Record metric with tensorboard
                     writer.add_scalar("Dice Val", dice_val, global_step=global_step)
+                    writer.add_scalar("IoU Val", iou_val, global_step=global_step)
+                    writer.add_scalar("Pixel Error", pixel_err_val, global_step=global_step)
                     writer.add_scalar("Dice Cross Entropy Loss", epoch_loss, global_step=global_step)
                 global_step += 1
             return global_step, dice_val_best, global_step_best
 
         while global_step < max_iterations:
             global_step, dice_val_best, global_step_best = __train(global_step, self.train_loader, dice_val_best,
                                                                    global_step_best)
@@ -349,15 +359,15 @@
         self.__load_files_from_folder(data_folder)
         test_dataset = data.Dataset(data=self.file_dicts, transform=self.inference_transforms)
         self.val_loader_inference = data.DataLoader(
             test_dataset,
             batch_size=1,
             shuffle=False,
             num_workers=4,
-            pin_memory=True,
+            pin_memory=False,
         )
 
     def __load_files_from_folder(self, data_folder: str) -> None:
         """
         Loads the files into a list of dictionaries to be read by Monai's built in dataset. This needs to be
         formatted in this specific way so the transforms can be properly applied (the transforms are expecting specific
         keys). The files that are loaded are all the files in the folder specified by data_folder. This is a mock
```

### Comparing `2404-segmentation-pipeline-0.1.2/setup.py` & `2404-segmentation-pipeline-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='2404-segmentation-pipeline',
-    version='0.1.2',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=[
         'monai==1.3.0',
         'nibabel==5.2.0',
         'matplotlib==3.8.2',
         'tensorboard==2.15.1',
         'tqdm==4.66.1',
```

