# Comparing `tmp/torchenhanced-0.2.9.tar.gz` & `tmp/torchenhanced-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchenhanced-0.2.9.tar", last modified: Fri Nov 24 16:38:16 2023, max compression
+gzip compressed data, was "torchenhanced-0.3.0b1.tar", last modified: Mon Apr 15 10:03:47 2024, max compression
```

## Comparing `torchenhanced-0.2.9.tar` & `torchenhanced-0.3.0b1.tar`

### file list

```diff
@@ -1,29 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-11-24 16:38:16.257061 torchenhanced-0.2.9/
--rw-rw-rw-   0        0        0      132 2023-11-20 16:38:31.000000 torchenhanced-0.2.9/.gitignore
--rw-rw-rw-   0        0        0      785 2023-11-24 16:38:16.252068 torchenhanced-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-06-14 09:27:16.000000 torchenhanced-0.2.9/README.md
--rw-rw-rw-   0        0        0      862 2023-08-07 10:56:17.000000 torchenhanced-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-24 16:38:16.258073 torchenhanced-0.2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-24 16:38:16.192459 torchenhanced-0.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-11-24 16:38:16.213065 torchenhanced-0.2.9/src/torchenhanced/
--rw-rw-rw-   0        0        0     3977 2023-09-21 19:27:17.000000 torchenhanced-0.2.9/src/torchenhanced/CosineWarmup.py
--rw-rw-rw-   0        0        0    34256 2023-11-24 16:20:41.000000 torchenhanced-0.2.9/src/torchenhanced/Trainer.py
--rw-rw-rw-   0        0        0      112 2023-08-07 11:01:49.000000 torchenhanced-0.2.9/src/torchenhanced/__init__.py
--rw-rw-rw-   0        0        0     1796 2023-11-20 11:26:40.000000 torchenhanced-0.2.9/src/torchenhanced/modules.py
-drwxrwxrwx   0        0        0        0 2023-11-24 16:38:16.243062 torchenhanced-0.2.9/src/torchenhanced/util/
--rw-rw-rw-   0        0        0      103 2023-06-14 09:27:16.000000 torchenhanced-0.2.9/src/torchenhanced/util/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-06-14 09:27:16.000000 torchenhanced-0.2.9/src/torchenhanced/util/color_compression.py
--rw-rw-rw-   0        0        0      721 2023-08-07 10:56:17.000000 torchenhanced-0.2.9/src/torchenhanced/util/files.py
--rw-rw-rw-   0        0        0     1335 2023-06-14 09:27:16.000000 torchenhanced-0.2.9/src/torchenhanced/util/misc.py
--rw-rw-rw-   0        0        0     2958 2023-11-20 11:29:18.000000 torchenhanced-0.2.9/src/torchenhanced/util/visualize.py
-drwxrwxrwx   0        0        0        0 2023-11-24 16:38:16.250062 torchenhanced-0.2.9/src/torchenhanced.egg-info/
--rw-rw-rw-   0        0        0      785 2023-11-24 16:38:16.000000 torchenhanced-0.2.9/src/torchenhanced.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-11-24 16:38:16.000000 torchenhanced-0.2.9/src/torchenhanced.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-24 16:38:16.000000 torchenhanced-0.2.9/src/torchenhanced.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-11-24 16:38:16.000000 torchenhanced-0.2.9/src/torchenhanced.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-11-24 16:38:16.000000 torchenhanced-0.2.9/src/torchenhanced.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-24 16:38:16.248066 torchenhanced-0.2.9/tests/
--rw-rw-rw-   0        0        0     6792 2023-11-24 15:21:15.000000 torchenhanced-0.2.9/tests/test_Trainer.py
--rw-rw-rw-   0        0        0     4717 2023-11-24 16:19:11.000000 torchenhanced-0.2.9/tests/test_Trainer_mini.py
--rw-rw-rw-   0        0        0      823 2023-09-26 17:42:22.000000 torchenhanced-0.2.9/tests/test_cosine.py
--rw-rw-rw-   0        0        0     2217 2023-08-07 10:56:17.000000 torchenhanced-0.2.9/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.923660 torchenhanced-0.3.0b1/
+-rw-rw-rw-   0        0        0       95 2024-04-11 10:37:32.000000 torchenhanced-0.3.0b1/.gitignore
+-rw-rw-rw-   0        0        0     1118 2024-04-15 10:03:47.920653 torchenhanced-0.3.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-11 14:27:41.000000 torchenhanced-0.3.0b1/README.md
+-rw-rw-rw-   0        0        0      901 2024-02-28 18:27:27.000000 torchenhanced-0.3.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0       66 2024-04-11 10:34:25.000000 torchenhanced-0.3.0b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 10:03:47.923660 torchenhanced-0.3.0b1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.684312 torchenhanced-0.3.0b1/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.740381 torchenhanced-0.3.0b1/src/torchenhanced/
+-rw-rw-rw-   0        0        0      169 2024-04-11 10:38:23.000000 torchenhanced-0.3.0b1/src/torchenhanced/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.779282 torchenhanced-0.3.0b1/src/torchenhanced/ml/
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.799285 torchenhanced-0.3.0b1/src/torchenhanced/ml/functional/
+-rw-rw-rw-   0        0        0       34 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/functional/__init__.py
+-rw-rw-rw-   0        0        0      959 2024-04-11 10:24:19.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/functional/batch_roll.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.821212 torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/
+-rw-rw-rw-   0        0        0       39 2024-04-11 10:33:33.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/__init__.py
+-rw-rw-rw-   0        0        0     3975 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/cosine_warmup.py
+-rw-rw-rw-   0        0        0     2408 2024-04-11 17:04:26.000000 torchenhanced-0.3.0b1/src/torchenhanced/modules.py
+-rw-rw-rw-   0        0        0    35707 2024-04-11 17:50:34.000000 torchenhanced-0.3.0b1/src/torchenhanced/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.866825 torchenhanced-0.3.0b1/src/torchenhanced/util/
+-rw-rw-rw-   0        0        0      105 2024-04-11 10:40:11.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-06-14 09:27:16.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/color_compression.py
+-rw-rw-rw-   0        0        0      723 2024-04-11 10:24:44.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/files.py
+-rw-rw-rw-   0        0        0     1335 2023-06-14 09:27:16.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/misc.py
+-rw-rw-rw-   0        0        0     8707 2024-04-11 10:35:08.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/visualize.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.919176 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/
+-rw-rw-rw-   0        0        0     1118 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.916571 torchenhanced-0.3.0b1/tests/
+-rw-rw-rw-   0        0        0      836 2024-04-11 17:12:42.000000 torchenhanced-0.3.0b1/tests/test_cosine.py
+-rw-rw-rw-   0        0        0     4309 2024-04-11 17:32:43.000000 torchenhanced-0.3.0b1/tests/test_custom_dataset.py
+-rw-rw-rw-   0        0        0     1855 2024-04-11 16:17:07.000000 torchenhanced-0.3.0b1/tests/test_modules.py
+-rw-rw-rw-   0        0        0     7908 2024-04-11 17:43:48.000000 torchenhanced-0.3.0b1/tests/test_trainer.py
+-rw-rw-rw-   0        0        0     2270 2024-04-11 16:19:01.000000 torchenhanced-0.3.0b1/tests/test_util.py
```

### Comparing `torchenhanced-0.2.9/PKG-INFO` & `torchenhanced-0.3.0b1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchenhanced
-Version: 0.2.9
+Version: 0.3.0b1
 Summary: Wrappers for pytorch stuff I use on the daily
 Author-email: Vassilis Papadopoulos <frotaur@hotmail.co.uk>
 License: MIT License
 Project-URL: Homepage, https://github.com/frotaur/torchenhanced
 Project-URL: Bug Tracker, https://github.com/frotaur/torchenhanced/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,10 +13,20 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: wandb
+Requires-Dist: opencv_python
+Requires-Dist: numpy
+Requires-Dist: Pillow
+Requires-Dist: tqdm
+
+# TorchEnhanced
+Wrappers for pytorch stuff I use on the daily. Basically a minimal 'pytorch lightning', I was just not aware it existed at the time of creation.
+
+
+## Coming soon : Readme and documentation
+In the meantime, everything is copiously doc-stringed, so you can take a look there.
+
 
-# torchEnhanced
-Wrappers for pytorch stuff I use on the daily.
```

### Comparing `torchenhanced-0.2.9/pyproject.toml` & `torchenhanced-0.3.0b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     'Development Status :: 3 - Alpha'
 ]
 dynamic = ["version"]
-dependencies = ["torch","torchvision","matplotlib","tqdm", "wandb",]
+dependencies = ["torch","torchvision","matplotlib","tqdm", "wandb","opencv_python","numpy","Pillow","tqdm"]
 
 
 [project.urls]
 "Homepage" = "https://github.com/frotaur/torchenhanced"
 "Bug Tracker" = "https://github.com/frotaur/torchenhanced/issues"
 
 [tool.setuptools_scm]
```

### Comparing `torchenhanced-0.2.9/src/torchenhanced/CosineWarmup.py` & `torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/cosine_warmup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import torch.optim.lr_scheduler as lrsched
 from torch.optim.optimizer import Optimizer
 import math
 
 class _enable_get_lr_call:
-
     def __init__(self, o):
         self.o = o
 
     def __enter__(self):
         self.o._get_lr_called_within_step = True
         return self
```

### Comparing `torchenhanced-0.2.9/src/torchenhanced/Trainer.py` & `torchenhanced-0.3.0b1/src/torchenhanced/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import torch.nn as nn, math
 import torch, wandb, os
 import torch.optim.lr_scheduler as lrsched
 from torch.optim import Optimizer
 from datetime import datetime
 from tqdm import tqdm
-from .modules import DevModule, ConfigModule
 
 
-class Trainer(DevModule):
+class Trainer:
     """
         Mother class used to train models, exposing a host of useful functions.
         Should be subclassed to be used, and the following methods should be redefined :
             - process_batch, mandatory
             - get_loaders, mandatory
             - epoch_log, optional
             - valid_log, optional
@@ -25,40 +24,43 @@
         Parameters :
         model : Model to be trained
         optim : Optimizer to be used. ! Must be initialized
         with the model parameters ! Default : AdamW with 1e-3 lr.
         scheduler : Scheduler to be used. Can be provided only if using
         non-default optimizer. Must be initialized with aforementioned 
         optimizer. Default : warmup for 4 epochs from 1e-6.
-        state_save_loc : str or None(default), folder in which to store data 
+        save_loc : str or None(default), folder in which to store data 
         pertaining to training, such as the training state, wandb folder and model weights.
         device : torch.device, device on which to train the model
+        parallel : None or list[int,str], if None, no parallelization, if list, list of devices (int or torch.device) to parallelize on
         run_name : str, for wandb and saves, name of the training session
         project_name : str, name of the project in which the run belongs
         run_config : dict, dictionary of hyperparameters (any). Will be viewable in wandb.
     """
 
     def __init__(self, model : nn.Module, optim :Optimizer =None, scheduler : lrsched._LRScheduler =None,*, 
-                 state_save_loc=None,device:str ='cpu', run_name :str = None,project_name :str = None,
+                 save_loc=None,device:str ='cpu',parallel:list[int]=None, run_name :str = None,project_name :str = None,
                  run_config : dict = {}):
         super().__init__()
         
-        self.to(device)
+        self.parallel_train = parallel is not None
+        self.parallel_devices = parallel
+        if(self.parallel_train):
+            # Go to GPU if parallel training
+            device = self.parallel_devices[0]
+
         self.model = model.to(device)
 
-        
-        if(state_save_loc is None) :
+        if(save_loc is None) :
             self.data_fold = os.path.join('.',project_name)
-            self.state_save_loc = os.path.join(self.data_fold,"state")
-            self.model_save_loc = os.path.join(self.data_fold,"weights")
+            self.save_loc = os.path.join(self.data_fold,"state")
         else :
-            self.data_fold = os.path.join(state_save_loc,project_name)#
-            
-            self.state_save_loc = os.path.join(state_save_loc,project_name,"state")
-            self.model_save_loc = os.path.join(state_save_loc,project_name,"weights")
+            self.data_fold = os.path.join(save_loc,project_name)#
+            self.save_loc = os.path.join(save_loc,project_name,"state")
+
         
         os.makedirs(self.data_fold,exist_ok=True)
         if(optim is None):
             self.optim = torch.optim.AdamW(self.model.parameters(),lr=1e-3)
         else :
             self.optim = optim
 
@@ -72,61 +74,68 @@
         self.session_hash = datetime.now().strftime('%H-%M_%d_%m')
         if(run_name is None):
             self.run_name = self.session_hash
             run_name= os.path.join('.','runs',self.session_hash)
         else :
             self.run_name=run_name
             run_name = os.path.join('.','runs',run_name)
-        
+ 
         self.run_config = dict(model=self.model.__class__.__name__,
-                               **run_config)
-        
+                            **run_config)
+
         self.run_id = wandb.util.generate_id() # For restoring the run
         self.project_name = project_name
         
+        self.device=device
         # Universal attributes for logging purposes
-        self.stepnum = 0 # number of steps in current training instance
-        self.batchnum = None # same as stepnum, DEPRECATED
+        self.stepnum = 0 # number of steps in current training instance (+1 each optimizer step)
+        self.batchnum = 0 # (+1 each batch. Equal to stepnum if no aggregation)
 
-        self.batches = 0 # number of total batches ever
-        self.steps_done = 0 # number of total steps ever TODO (now its same as batches, will become optimizer steps later)
+        self.batches = 0 # number of total batches ever (+1 each batch. Same a steps_done if no aggregation)
+        self.steps_done = 0 # number of total steps ever (+1 each optimizer step)
         self.epochs = 0 # number of total epochs ever
         self.samples = 0 # number of total samples ever
 
         self.step_log = None # number of steps between each log
         self.totbatch = None # total number of batches in one epoch for this training instance
-        self.do_batch_log = False 
+        self.do_step_log = False 
 
         # Used for logging instead of wandb.log, useful if wandb not imported
         self.logger = None
-    
+
     def change_lr(self, new_lr):
         """
             Changes the learning rate of the optimizer.
             Might clash with scheduler ?
         """
-
         for g in self.optim.param_groups:
             g['lr'] = new_lr
         
 
     def load_state(self,state_path : str, strict: bool=True):
         """
-            Loads trainer minimal trainer state (model,session_hash,optim,scheduler).
+            Loads Trainer state, for restoring a run.
 
             params : 
-            state_path : str, location of the sought-out state_dict
-
+            state_path : location of the sought-out state_dict
+            strict: whether to load the state_dict in strict mode or not
         """
+
+        if(isinstance(self.model, nn.DataParallel)):
+            # Unwrap the model, since we saved the state_dict of the model, not the DataParallel
+            self.model = self.model.module.to(self.device)
+        
         if(not os.path.exists(state_path)):
             raise ValueError(f'Path {state_path} not found, can\'t load state')
+
         state_dict = torch.load(state_path,map_location=self.device)
         if(self.model.config != state_dict['model_config']):
             print('WARNING ! Loaded model configuration and state model_config\
                   do not match. This may generate errors.')
+            
         assert self.model.class_name == state_dict['model_name'], f'Loaded model {state_dict["model_name"]} mismatch with current: {self.model.class_name}!'
         assert self.optim.__class__.__name__ == state_dict['optim_name'], f'Loaded optimizer : {state_dict["optim_name"]} mismatch with current: {self.optim.__class__.__name__} !'
         assert self.scheduler.__class__.__name__ == state_dict['scheduler_name'], f'Loaded scheduler : {state_dict["scheduler_name"]} mismatch with current: {self.optim.__class__.__name__} !'
 
         self.model.load_state_dict(state_dict['model_state'],strict=strict)
         self.session_hash = state_dict['session']
         self.optim.load_state_dict(state_dict['optim_state'])
@@ -135,17 +144,48 @@
         self.steps_done = state_dict.get('steps_done',0)
         self.batches = state_dict.get('batches',0)
 
         self.epochs = state_dict.get('epochs',0)
         self.samples = state_dict.get('samples',0)
         self.run_config = state_dict.get('run_config',{'model':self.model.__class__.__name__})
         # Maybe I need to load also the run_name, we'll see
+        
+        # Reset the default step_loss, although shouldn't load stuff after a bit of training.
+        self.step_loss = []
 
-        print('LOAD OF SUCCESSFUL !')
-        print('loaded dict : ', state_dict['batches'])
+        print('Training state load successful !')
+        print(f'Loaded state had {state_dict["epochs"]} epochs trained.')
+
+    def load_model_from_state(self,state_path : str, strict: bool=True, force_config_match:bool=False):
+        """
+            Loads only model weights from state. Useful if you just want to load a 
+            pretrained model to train it on a different dataset.
+        """
+        if(isinstance(self.model, nn.DataParallel)):
+            # Unwrap the model, since we saved the state_dict of the model, not the DataParallel
+            self.model = self.model.module.to(self.device)
+        
+        if(not os.path.exists(state_path)):
+            raise ValueError(f'Path {state_path} not found, can\'t load state')
+
+        state_dict = torch.load(state_path,map_location=self.device)
+        if(self.model.config != state_dict['model_config']):
+            if(force_config_match):
+                raise ValueError(f'Loaded model configuration and state model_config\
+                                 do not match. \n Model : {self.model.config} \n State : {state_dict["model_config"]}')
+            else:
+                print('WARNING ! Loaded model configuration and state model_config\
+                    do not match. This may generate errors.')
+            
+        assert self.model.class_name == state_dict['model_name'], f'Loaded model {state_dict["model_name"]} mismatch with current: {self.model.class_name}!'
+
+        self.model.load_state_dict(state_dict['model_state'],strict=strict)
+
+        print('Model load successful !')
+        print(f'Loaded model had {state_dict["epochs"]} epochs trained.')
 
     def save_state(self,epoch:int = None):
         """
             Saves trainer state. Describe by the following dictionary :
 
             state_dict : dict, contains at least the following key-values:
                 - 'model' : contains model.state_dict
@@ -157,43 +197,44 @@
                 - 'steps_done' : only applicable in case of step training, number of steps done
                 - 'samples' : number of samples seen
             If you want a more complicated state, training_epoch should be overriden.
 
             Args :
             epoch : int, if not None, will append the epoch number to the state name.
         """
-        os.makedirs(self.state_save_loc,exist_ok=True)
-
+        os.makedirs(self.save_loc,exist_ok=True)
+        
+        # Avoid saving the DataParallel
+        saving_model = self.model.module if self.parallel_train else self.model
+    
         # Create the state
         try :
-            model_config = self.model.config
+            model_config = saving_model.config
         except AttributeError as e:
-            print(f'''Error while fetching model config ! 
-                    Make sure model.config is defined. (see ConfigModule doc).
-                    Continuing, but might generate errors while loading/save models)''')
-            model_config = None
+            raise AttributeError(f"Error while fetching model config ! Make sure model.config is defined. (see ConfigModule doc).")
 
         state = dict(
-        optim_state=self.optim.state_dict(),scheduler_state=self.scheduler.state_dict(),model_state=self.model.state_dict(),
-        model_name=self.model.class_name,optim_name=self.optim.__class__.__name__,scheduler_name=self.scheduler.__class__.__name__,
+        optim_state=self.optim.state_dict(),scheduler_state=self.scheduler.state_dict(),model_state=saving_model.state_dict(),
+        model_name=saving_model.class_name,optim_name=self.optim.__class__.__name__,scheduler_name=self.scheduler.__class__.__name__,
         model_config=model_config,session=self.session_hash,run_id=self.run_id, steps_done=self.steps_done,epochs=self.epochs,
         samples=self.samples, batches=self.batches,run_config=self.run_config
         )
 
         name = self.run_name
         if (epoch is not None):
-            os.makedirs(os.path.join(self.state_save_loc,'backups'),exist_ok=True)
+            os.makedirs(os.path.join(self.save_loc,'backups'),exist_ok=True)
             name=os.path.join('backups',name+'_'+f'{epoch:.2f}')
 
         name = name + '.state'
-        saveloc = os.path.join(self.state_save_loc,name)
+        saveloc = os.path.join(self.save_loc,name)
         torch.save(state,saveloc)
 
         print(f'Saved training state at {datetime.now().strftime("%H-%M_%d_%m")}')
-        print(f'At save : ', self.batches)
+        print(f'At save, {self.epochs} epochs are done.')
+
 
     @staticmethod
     def save_model_from_state(state_path:str,save_dir:str='.',name:str=None):
         """
             Extract model weights and configuration, and saves two files in the specified directory,
             the weights (.pt) and a .config file containing the model configuration, which can be loaded
             as a dictionary with torch.load.
@@ -246,56 +287,23 @@
         opti_state = state_dict['optim_state']
         sched_name = state_dict['sched_name']
         sched_state = state_dict['sched_state']
 
         return (opti_name,opti_state),(sched_name,sched_state)
 
     @staticmethod
-    def config_from_state(state_path: str,device: str=None):
-        """
-            Given the path to a trainer state, returns a tuple (config, weights)
-            for the saved model. The model can then be initialized by using config 
-            as its __init__ arguments, and load the state_dict from weights.
-
-            Args :
-            state_path : path of the saved trainer state
-            device : device on which to load. Default one if None specified
-
-            returns: 3-uple
-            model_name : str, the saved model class name
-            config : dict, the saved model config (instanciate with element_name(**config))
-            state_dict : torch.state_dict, the model's state_dict (load with .load_state_dict(weights))
-
-        """
-        print('WARNING : Deprecated, will be removed in next version')
-        print('For model config, use model_config_from_state instead')
-        if(not os.path.exists(state_path)):
-            raise ValueError(f'Path {state_path} not found, can\'t load config from it')
-        
-        if(device is None):
-            state_dict = torch.load(state_path)
-        else :
-            state_dict = torch.load(state_path,map_location=device)
-
-        config = state_dict['model_config']
-        model_name = state_dict['model_name']
-        weights = state_dict['model_state']
-
-        return model_name,config,weights
-
-    @staticmethod
     def model_config_from_state(state_path: str,device: str=None):
         """
-            Given the path to a trainer state, returns a tuple (config, weights)
+            Given the path to a trainer state, returns a 3-uple (model_name,config, weights)
             for the saved model. The model can then be initialized by using config 
             as its __init__ arguments, and load the state_dict from weights.
 
             Args :
             state_path : path of the saved trainer state
-            device : device on which to load. Default one if None specified
+            device : device on which to load. Previous one if None specified
 
             returns: 3-uple
             model_name : str, the saved model class name
             config : dict, the saved model config (instanciate with element_name(**config))
             state_dict : torch.state_dict, the model's state_dict (load with .load_state_dict(weights))
 
         """
@@ -330,51 +338,52 @@
         if(device is None):
             state_dict = torch.load(state_path)
         else :
             state_dict = torch.load(state_path,map_location=device)
 
         return state_dict['run_config']
 
-    def process_batch(self,batch_data,**kwargs):
+    def process_batch(self,batch_data):
         """
-            Redefine this in sub-classes. Should return the loss, as well as 
-            the data_dict (potentially updated). Can do logging and other things 
+            Redefine this in sub-classes. Should return the loss. Batch_data will be on 'cpu' most of the
+            time, except if you dataset sets a specific device. Can do logging and other things 
             optionally. Loss is automatically logged, so no need to worry about it. 
+            Use self.model to access the model.
 
             Args :
             batch_data : whatever is returned by the dataloader
             Default class attributes, automatically maintained by the trainer, are :
-                - self.batchnum : current validation mini-batch number
-                - self.step_log : number of steps (minibatches) interval in 
-                        which we should log. (PREFER USING do_batch_log instead)
-                - self.do_batch_log : whether we should log this batch or not
-                - self.totbatch : total number of validation minibatches.
-                - self.epoch : current epoch
+                - self.device : current model device
+                - self.stepnum : current step number since last training/epoch start
+                - self.do_step_log : whether we should log this batch or not
+                - self.totbatch : total number of minibatches in one epoch.
+                - self.epochs: current epoch
                 - self.samples : number of samples seen
+                - self.steps_done : number of steps done since the beginning of training
             Returns : 2-uple, (loss, data_dict)
         """
         raise NotImplementedError('process_batch should be implemented in Trainer sub-class')
 
-    def process_batch_valid(self,batch_data, **kwargs):
+    def process_batch_valid(self,batch_data):
         """
             Redefine this in sub-classes. Should return the loss, as well as 
-            the data_dict (potentially updated). There should be NO logging done
-            inside this function, only in valid_log. Proper use should be to collect the data
-            to be logged in a class attribute, and then log it in valid_log (to log once per epoch)
-            Loss is automatically logged, so no need to worry about it. 
+            the data_dict (potentially updated). Use self.model to access the model (it is already in eval mode).
+            Batch_data will be on 'cpu' most of the time, except if you dataset sets a specific device. 
+            There should be NO logging done inside this function, only in valid_log.
+            Proper use should be to collect the data to be logged in a class attribute,
+            and then log it in valid_log (to log once per epoch). Loss is automatically 
+            logged, so no need to worry about it. 
 
             Args :
             batch_data : whatever is returned by the dataloader
-            data_dict : DEPRECATED ! Avoid using it. Use class attributes instead. 
             Default class attributes, automatically maintained by the trainer, are :
+                - self.device : current model device
                 - self.batchnum : current validation mini-batch number
-                - self.step_log : number of steps (minibatches) interval in which we should log 
-                    Minibatch logging in valid is not recommended, since it is not synchronized with the epoch x-axis.
                 - self.totbatch : total number of validation minibatches.
-                - self.epoch : current epoch
+                - self.epochs: current epoch
                 - self.samples : number of samples seen
 
             Returns : 2-uple, (loss, data_dict)
         """
         raise NotImplementedError('process_batch_valid should be implemented in Trainer sub-class')
 
     def get_loaders(self,batch_size, num_workers=0):
@@ -393,50 +402,48 @@
     def epoch_log(self):
         """
             To be (optionally) implemented in sub-class. Does the logging 
             at the epoch level, is called every epoch. Only log using commit=False,
             because of sync issues with the epoch x-axis.
 
             Args :
-            data_dict : DEPRECATED ! Avoid using it. Use class attributes instead. 
             Default class attributes, automatically maintained by the trainer, are :
-                - self.batchnum : current validation mini-batch number
-                - self.step_log : number of steps (minibatches) interval in which we should log 
-                - self.totbatch : total number of validation minibatches.
-                - self.epoch : current epoch
+                - self.device : current model device
+                - self.stepnum : current step number since last training/epoch start
+                - self.do_step_log : whether we should log this batch or not
+                - self.totbatch : total number of minibatches in one epoch.
+                - self.epochs: current epoch
                 - self.samples : number of samples seen
+                - self.steps_done : number of steps done since the beginning of training
         """
         pass
 
     def valid_log(self):
         """
             To be (optionally) implemented in sub-class. Does the logging 
             at the epoch level, is called every epoch. Only log using commit=False,
             because of sync issues with the epoch x-axis.
 
 
             Args :
-            data_dict : DEPRECATED ! Avoid using it. Use class attributes instead. 
-                Default class attributes, automatically maintained by the trainer, are :
-                    - self.batchnum : current validation mini-batch number
-                    - self.step_log : number of steps (minibatches) interval in which we should log 
-                    - self.totbatch : total number of validation minibatches.
-                    - self.epoch : current epoch
-                    
-                    - self.samples : number of samples seen
-
+            Default class attributes, automatically maintained by the trainer, are :
+                - self.batchnum : current validation mini-batch number
+                - self.totbatch : total number of validation minibatches.
+                - self.epochs: current epoch
+                - self.samples : number of samples seen
+                - self.steps_done : number of steps done since the beginning of training
         """
         pass
     
     def train_init(self,**kwargs):
         """
             Can be redefined for doing stuff just at the beginning of the training,
             for example, freezing weights, preparing some extra variables, or anything really.
             Not mandatory, it is called at the very beginnig of train_epochs/train_steps. The
-            dictionary 'train_init_params' is passed as parameter. As such, it can take
+            dictionary 'train_init_params' is passed as parameter list. As such, it can take
             any combination of parameters.
         """
         pass
 
     def train_epochs(self,epochs : int,batch_size:int,*,batch_sched:bool=False,save_every:int=50,
                      backup_every: int=None,step_log:int=None,
                      num_workers:int=0,aggregate:int=1,
@@ -448,113 +455,111 @@
 
             data_dict can be used to carry info from one batch to another inside the same epoch,
             and can be used by process_batch* functions for logging of advanced quantities.
             Params :
             epochs : number of epochs to train for
             batch_size : batch size
             batch_sched : if True, scheduler steps (by a lower amount) between each batch.
-            Not that this use is deprecated, so it is recommended to keep False. For now, 
+            Note that this use is deprecated, so it is recommended to keep False. For now, 
             necessary for some Pytorch schedulers (cosine annealing).
-            save_every : saves trainer state every 'save_every' epochs
-            step_log : If not none, will also log every step_log minibatches, in addition to each epoch
-            batch_log : same as step_log, DEPRECATED
+            save_every : saves trainer state every 'save_every' EPOCHS
+            backup_every : saves trainer state without overwrite every 'backup_every' EPOCHS
+            step_log : If not none, will also log every step_log optim steps, in addition to each epoch
             num_workers : number of workers in dataloader
             aggregate : how many batches to aggregate (effective batch_size is aggreg*batch_size)
-            load_from : path to a trainer state_dict. Loads the state
-                of the trainer from file, then continues training the specified
-                number of epochs.
+            batch_tqdm : if True, will use tqdm for the batch loop, if False, will not use tqdm
             train_init_params : Parameter dictionary passed as argument to train_init
         """
         
         # Initiate logging
-        self.logger = wandb.init(name=self.run_name,project=self.project_name,config=self.run_config,
-                   id = self.run_id,resume='allow',dir=self.data_fold)
-        
-        # Define the custom x axis metric, epochs
-        self.logger.define_metric("batches",hidden=True)
-        self.logger.define_metric("epochs",hidden=True)
-        self.logger.define_metric("ksamples",hidden=True)
+        self._init_logger()
         # For all plots, we plot against the epoch by default
         self.logger.define_metric("*", step_metric='epochs')
 
         self.train_init(**train_init_params)
         
         train_loader,valid_loader = self.get_loaders(batch_size,num_workers=num_workers)
         validate = valid_loader is not None
-
+        
+        self.totbatch = len(train_loader)
+        assert self.totbatch > aggregate, f'Aggregate ({aggregate}) should be smaller than number of batches \
+                                            in one epoch ({self.totbatch}), otherwise we never step !'
         self.model.train()
+        if(self.parallel_train):
+            print('Parallel training on devices : ',self.parallel_devices)
+            self.model = nn.DataParallel(self.model,device_ids=self.parallel_devices)
+        
         if(batch_sched):
             assert self.epochs-self.scheduler.last_epoch<1e-5, f'Epoch mismatch {self.epochs} vs {self.scheduler.last_epoch}'
         else:
             assert int(self.epochs)==self.scheduler.last_epoch, f'Epoch mismatch {self.epochs} vs {self.scheduler.last_epoch}'
+        
         #Floor frac epochs, since we start at start of epoch, and also for the scheduler :
         self.epochs = int(self.epochs)
         print('Number of batches/epoch : ',len(train_loader))
         self.stepnum = 0 # This is the current instance number of steps, using for when to log save etc
 
         self.step_log = step_log
-        step_loss=[]
-
+        self.step_loss=[]
+        
         
         for ep_incr in tqdm(range(epochs)):
-            epoch_loss,n_aggreg=[[],0]
-            
-            self.totbatch = len(train_loader)
+            self.epoch_loss=[]
+            n_aggreg = 0
 
             # Iterate with or without tqdm
             if(batch_tqdm):
                 iter_on=tqdm(enumerate(train_loader),total=self.totbatch)
             else :
                 iter_on=enumerate(train_loader)
 
             # Epoch of Training
             for batchnum,batch_data in iter_on :
                 # Process the batch
                 self.batchnum=batchnum
-                epoch_loss, step_loss, n_aggreg = self._step_batch(batch_data,True,epoch_loss,step_loss,n_aggreg, aggregate, step_sched=False)
-    
+                n_aggreg = self._step_batch(batch_data,n_aggreg, aggregate, step_sched=False)
+
+
                 if(batch_sched):
                     self.scheduler.step(self.epochs)
 
-                self.stepnum+=1
-                self.steps_done+=1
-                self.batches+=1
                 self.samples+=batch_size
                 self.epochs+=1/self.totbatch
+                # NOTE: Not great, but batches and steps update in _step_batch by necessity
 
             self.epochs = round(self.epochs) # round to integer, should already be, but to remove floating point stuff
             
             if(not batch_sched):
                 self.scheduler.step()
             else :
+                # Is useless in principle, just to synchronize with the rounding of epochs
                 self.scheduler.step(self.epochs)
             
             # Epoch of validation
             if(validate):
-                self._validate(valid_loader,batch_tqdm)
-                self.model.train()
+                self._validate(valid_loader)
                 self.valid_log()
+                self.model.train()
     
 
-            # Log training at epoch level
-            self.logger.log({'loss/train_epoch':sum(epoch_loss)/len(epoch_loss)},commit=False)
+            # Log training loss at epoch level
+            self.logger.log({'loss/train_epoch':sum(self.epoch_loss)/len(self.epoch_loss)},commit=False)
             self.epoch_log()
                 
-            self._update_x_axis(epoch_mode=True)
+            self._update_x_axis()
             
             # Save and backup when applicable
             self._save_and_backup(curstep=ep_incr,save_every=save_every,backup_every=backup_every)
 
         self.logger.finish()
 
-
     def train_steps(self,steps : int,batch_size:int,*,save_every:int=50,
                     backup_every: int=None, valid_every:int=1000,step_log:int=None,
-                    num_workers:int=0,aggregate:int=1,resume_batches:bool=False,
-                    batch_tqdm:bool=True, train_init_params:dict={}):
+                    num_workers:int=0,aggregate:int=1,pickup:bool=True,resume_batches:bool=False, 
+                    train_init_params:dict={}):
         """
             Trains for specified number of steps(batches). This method trains the model in a basic way,
             and does very basic logging. At the minimum, it requires process_batch and 
             process_batch_valid to be overriden, and other logging methods are optionals. Epoch_log is not
             used in step level training.
             Note that the scheduler will be called AFTER EVERY MINIBATCH, i.e. after every step. Everything
             is logged by default against the number of steps, but the 'epochs' metric is also defined, and
@@ -562,179 +567,195 @@
 
             Params :
             batch_size : batch size
             steps : number of steps (batches) to train for
             save_every : saves trainer state every 'save_every' epochs
             backup_every : saves trainer state without overwrite every 'backup_every' steps
             valid_every : validates the model every 'valid_every' steps
-            step_log : If not none, used for logging every step_log steps. In process_batch,
-            use self.do_step_log to know when to log. NOTE : if using aggregating, for step logging,
-            we consider a step to be aggregate batches, not 'true' batches.
+            step_log : If not none, used for logging every step_log optim steps. In process_batch,
+            use self.do_step_log to know when to log. 
             num_workers : number of workers in dataloader
             aggregate : how many batches to aggregate (effective batch_size is aggreg*batch_size)
+            pickup : if False, will train for exactly 'steps' steps. If True, will restart at the previous
+            number of steps, and train until total number of steps is 'steps'. Useful for resuming training,
+            if you want to train for a certain specific number of steps. In both cases, the training resumes
+            where it left off, only difference is how many MORE steps it will do.
             resume_batches : if True, will resume training assuming the first self.batches on the dataloader
             are already done. Usually, use ONLY if dataloader does NOT shuffle.
-            batch_tqdm : whether to use tqdm for the batch loop or not
             train_init_params : Parameter dictionary passed as argument to train_init
         """
     
         # Initiate logging
-        self.logger = wandb.init(name=self.run_name,project=self.project_name,config=self.run_config,
-                   id = self.run_id,resume='allow',dir=self.data_fold)
-        
-        # Define the custom x axis metrics
-        self.logger.define_metric("epochs",hidden=True)
-        self.logger.define_metric("batches",hidden=True)
+        self._init_logger()
         # For all plots, we plot against the batches by default, since we do step training
-        self.logger.define_metric("*", step_metric='batches')
+        self.logger.define_metric("*", step_metric='steps')
 
         self.train_init(**train_init_params)
         
         train_loader,valid_loader = self.get_loaders(batch_size,num_workers=num_workers)
         validate = valid_loader is not None
 
         self.totbatch = len(train_loader) # Number of batches in one epoch
 
+        assert self.totbatch >= aggregate, f'Aggregate ({aggregate}) should be smaller than number of batches \
+                                            in one epoch ({self.totbatch}), otherwise we never step !'
         self.model.train()
-        # _=self.scheduler.last_epoch # this is equal to self.steps_done
-    
 
-        print('Number of batches/epoch : ',len(train_loader))
+        if(self.parallel_train):
+            print('Parallel training on devices : ',self.parallel_devices)
+            self.model = nn.DataParallel(self.model,device_ids=self.parallel_devices)
+        
+        print('Number of batches/epoch : ',len(train_loader)/1000 ,'k')
 
         self.step_log = step_log
-        step_loss=[]
+        self.step_loss=[]
+        self.epoch_loss = None
 
         steps_completed = False
-        self.stepnum = 0 # This is the current instance number of steps, using for when to log save etc
+        if(pickup):
+            self.stepnum = self.batches
+        else:
+            self.stepnum = 0 #Current instance stepnumber, used for when to log and stop training.
 
         while not steps_completed:
-            # Iterate with or without tqdm
-
-            if(batch_tqdm):
-                iter_on=tqdm(enumerate(train_loader),total=self.totbatch)
-            else :
-                iter_on=enumerate(train_loader)
+            iter_on=enumerate(train_loader)
 
             if(resume_batches):
                 resume_batches=False # Only resume for the first epoch, not if we reach and and restart.
-                print('Resuming from batch :', self.batches)
-                print(f'Fast forwarding {self.batches}%{self.totbatch}={self.batches%self.totbatch} batches')
-                for _ in tqdm(range((self.batches)%self.totbatch)):
+                tofastforward = (self.batches)%self.totbatch
+                print(f'Fast forwarding {self.batches}%{self.totbatch}={tofastforward} batches')
+                for _ in tqdm(range(tofastforward)):
                     # skip batches already done
                     next(iter_on)
-                # Now train_loader is synchronized with self.batches
-
+                iter_on=tqdm(iter_on,total=self.totbatch-tofastforward)
+            else :
+                iter_on=tqdm(iter_on,total=self.totbatch)
+    
             n_aggreg=0
             # Epoch of Training
             for batchnum,batch_data in iter_on :
                 # Process the batch according to the model.
                 self.batchnum=batchnum
-                _, step_loss, n_aggreg = self._step_batch(batch_data,False,[],step_loss,n_aggreg, aggregate,step_sched=True)
+                n_aggreg = self._step_batch(batch_data,n_aggreg, aggregate,step_sched=True)
 
                 # Validation if applicable
-                if(validate and self.stepnum%valid_every==valid_every-1):
-                    self._validate(valid_loader,batch_tqdm)
+                if(validate and self.batches%valid_every==valid_every-1):
+                    self._validate(valid_loader)
                     self.valid_log()
-                    self._update_x_axis(epoch_mode=False)
+                    self._update_x_axis()
                     self.model.train()
 
-                self.stepnum+=1
-                self.steps_done+=1 # TO BE MODIFIED TO BE OPTIMIZER STEPS
-                self.batches+=1
+
                 self.samples+=batch_size
-                self.epochs +=1/self.totbatch
+                self.epochs +=1/self.totbatch  # NOTE: Not great, but batches and steps update in _step_batch by necessity
+
+
+                # TODO minor bug, when we resume we shift by one minibatch the saving schedule
+                # Comes because the first save location is at %valid_every-1, so it last one less step since we start stepnum at 0
+                self._save_and_backup(self.steps_done,save_every,backup_every)
 
-    	        # Save and backup
-                self._save_and_backup(self.stepnum,save_every,backup_every)
-            
                 if(self.stepnum>=steps):
                     steps_completed=True
+                    self._save_and_backup(1,save_every,backup_every)
                     break
             
-            
-
         wandb.finish()
 
-    def _update_x_axis(self,epoch_mode):
+    def _update_x_axis(self):
         """
             Adds and commits pending wandb.log calls, and adds the x-axis metrics,
             to use the correct defaults.
 
             Args:   
             epoch_mode : bool, whether default x-axis is epoch or not
         """
-        # TODO remove the epoch_mode, and just use epochs as last one, it doesn't make a difference anyway
-        # TODO make so that batches area actually batches, and steps_done are optimizer steps
+
         self.logger.log({'ksamples' : self.samples//1000},commit=False)
+        self.logger.log({'epochs': self.epochs},commit=False)
+        self.logger.log({'steps': self.steps_done},commit=True)
 
-        if(epoch_mode):
-            self.logger.log({'batches': self.steps_done},commit=False) # TO BE MODIFIED TO BE OPTIMIZER STEPS
-            self.logger.log({'epochs': self.epochs},commit=True)
-        else :
-            self.logger.log({'epochs': self.epochs},commit=False)
-            self.logger.log({'batches': self.steps_done},commit=True)
 
-    def _step_batch(self, batch_data, epoch_mode, epoch_loss, step_loss, n_aggreg, aggregate, step_sched):
+    def _step_batch(self, batch_data, n_aggreg, aggregate, step_sched):
         """
             Internal function, makes one step of training given minibatch
         """
-        n_aggreg+=1
-        self.do_batch_log = self.stepnum%(self.step_log*aggregate)==0 #if aggregating, one 'batch' is actually aggregate batches
-
+        # Compute loss, and custom batch logging
         loss = self.process_batch(batch_data)
         
-        epoch_loss.append(loss.item())
-        step_loss.append(loss.item())
-
+        # Update default logging (NOTE :maybe I shouldn't do this, to avoid synchronization of CUDA ?)
+        # TODO : benchmark with and without the loss.item() to see if it changes significantly
+        self.step_loss.append(loss.item())
+        if(self.epoch_loss is not None):
+            self.epoch_loss.append(loss.item())
+        
+        # Do default logging
+        if(self.do_step_log):
+            self.logger.log({'loss/train_step':sum(self.step_loss)/len(self.step_loss)},commit=False)
+            self._update_x_axis()
+            self.step_loss=[]
+    
         loss=loss/aggregate # Rescale loss if aggregating.
         loss.backward() # Accumulate gradients
         
-        if(self.do_batch_log):
-            self.logger.log({'loss/train_step':sum(step_loss)/len(step_loss)},commit=False)
-            self._update_x_axis(epoch_mode=epoch_mode)
-            step_loss=[]
-            self.do_batch_log=False
+        self.batches+=1
+        n_aggreg+=1
 
-        if(n_aggreg%aggregate==aggregate-1):
+        if(n_aggreg%aggregate==0):
             n_aggreg=0
             torch.nn.utils.clip_grad_norm_(self.model.parameters(), 1.)
 
             self.optim.step()
             self.optim.zero_grad()
+
             if(step_sched):
                 self.scheduler.step()
-        
-        return epoch_loss,step_loss,n_aggreg
+
+            ## Update the step number
+            self.stepnum+=1
+            self.steps_done+=1
+
+        self.do_step_log = (self.stepnum%self.step_log)==0 if self.step_log else False
+
+        return n_aggreg
 
     @torch.no_grad()
-    def _validate(self,valid_loader, batch_tqdm)->None:
+    def _validate(self,valid_loader)->None:
         self.model.eval()
         val_loss=[]
         t_totbatch = self.totbatch
         t_batchnum = self.batchnum
 
         self.totbatch = len(valid_loader) # For now we use same totbatch for train and valid, might wanna change that in the future
-        if(batch_tqdm):
-            print('------ Validation ------')
-            iter_on=tqdm(enumerate(valid_loader),total=self.totbatch)
-        else:
-            iter_on=enumerate(valid_loader)
+        print('------ Validation ------')
+        iter_on=tqdm(enumerate(valid_loader),total=self.totbatch)
 
         for (v_batchnum,v_batch_data) in iter_on:
             self.batchnum=v_batchnum
             
             loss = self.process_batch_valid(v_batch_data)
             val_loss.append(loss.item())
         
         self.totbatch=t_totbatch
         self.batchnum=t_batchnum
-
+        
         # Log validation data
         self.logger.log({'loss/valid':sum(val_loss)/len(val_loss)},commit=False)
     
+    
+    def _init_logger(self):
+        """ Initiate the logger, and define the custom x axis metrics """
+        self.logger = wandb.init(name=self.run_name,project=self.project_name,config=self.run_config,
+                   id = self.run_id,resume='allow',dir=self.data_fold)
+        
+        self.logger.define_metric("epochs",hidden=True)
+        self.logger.define_metric("steps",hidden=True)
+        self.logger.define_metric("ksamples",hidden=True)
+
     def _save_and_backup(self,curstep,save_every,backup_every):
-        if curstep%save_every==save_every-1 :
+        # We use curstep-1, to save at a moment consistent with the valid
+        # And valid looks at curstep-1. (we updated curstep in between)
+        if (curstep-1)%save_every==0 :
             self.save_state()
         
         if backup_every is not None:
-            if curstep%backup_every==backup_every-1 :
+            if (curstep-1)%backup_every==backup_every-1 :
                 self.save_state(epoch=self.epochs)
```

### Comparing `torchenhanced-0.2.9/src/torchenhanced/modules.py` & `torchenhanced-0.3.0b1/src/torchenhanced/modules.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,28 +28,46 @@
 
 class ConfigModule(DevModule):
     """
         Same as DevModule, but with a config property that
         stores the necessary data to reconstruct the model.
         Use preferably over DevModule, especially with use with Trainer.
 
-        args :
+        Args :
         config : Dictionary that contains the key:value pairs needed to 
         instantiate the model (i.e. the argument values of the __init__ method)
     """
     def __init__(self, config:dict, device:str='cpu'):
         super().__init__(device=device)
 
         self._config = config
 
         self.class_name = self.__class__.__name__ # Use this instead if, at time of saving, you need the name.
-        # self._config['name'] = self.__class__.__name__ # Decided against using name in config, it defeats the purpose.
 
     @property
     def config(self):
         """
             Returns a json-serializable dict containing the config of the model.
             Essentially a key-value dictionary of the init arguments of the model.
             Should be redefined in sub-classes.
         """
         return self._config
 
+    def load_weights(self, weights_loc:str, strict:bool=True):
+        """
+            Loads weights from a file into the model, mapping them to current device.
+
+            Args:
+            weights_loc :  Path to the file containing the weights.
+            strict : If True, loads only if the model has exactly the same keys as the weights.
+        """
+
+        self.load_state_dict(torch.load(weights_loc,map_location=self.device),strict=strict)
+    
+    def save_weights(self, weights_loc:str):
+        """
+            Saves the weights of the model to a file.
+
+            Args:
+            weights_loc :  Path to the file to save the weights to.
+        """
+        torch.save(self.state_dict(),weights_loc)
```

### Comparing `torchenhanced-0.2.9/src/torchenhanced/util/color_compression.py` & `torchenhanced-0.3.0b1/src/torchenhanced/util/color_compression.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.2.9/src/torchenhanced/util/files.py` & `torchenhanced-0.3.0b1/src/torchenhanced/util/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     except: return ''
 
 def save_string(string, file_name):
     try: Path(file_name).write_text(string)
     except: return print(f"Error writing to {file_name=}")
 
 def load_json(file_name): return json.loads(load_string(file_name))
+
 def save_json(obj, file_name): save_string(json.dumps(obj), file_name)
 
 
 def save_torch(obj, file_path, *, replace=True, **params): 
     if not os.path.isfile(file_path) or replace: return torch.save(obj, file_path, **params) # wrapper to unify notation
     else:
         print(f"File {file_path} already exists ! Use replace=True to overwrite it.")
```

### Comparing `torchenhanced-0.2.9/src/torchenhanced/util/misc.py` & `torchenhanced-0.3.0b1/src/torchenhanced/util/misc.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.2.9/src/torchenhanced.egg-info/PKG-INFO` & `torchenhanced-0.3.0b1/src/torchenhanced.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchenhanced
-Version: 0.2.9
+Version: 0.3.0b1
 Summary: Wrappers for pytorch stuff I use on the daily
 Author-email: Vassilis Papadopoulos <frotaur@hotmail.co.uk>
 License: MIT License
 Project-URL: Homepage, https://github.com/frotaur/torchenhanced
 Project-URL: Bug Tracker, https://github.com/frotaur/torchenhanced/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,10 +13,20 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: wandb
+Requires-Dist: opencv_python
+Requires-Dist: numpy
+Requires-Dist: Pillow
+Requires-Dist: tqdm
+
+# TorchEnhanced
+Wrappers for pytorch stuff I use on the daily. Basically a minimal 'pytorch lightning', I was just not aware it existed at the time of creation.
+
+
+## Coming soon : Readme and documentation
+In the meantime, everything is copiously doc-stringed, so you can take a look there.
+
 
-# torchEnhanced
-Wrappers for pytorch stuff I use on the daily.
```

### Comparing `torchenhanced-0.2.9/src/torchenhanced.egg-info/SOURCES.txt` & `torchenhanced-0.3.0b1/src/torchenhanced.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 .gitignore
 README.md
 pyproject.toml
-src/torchenhanced/CosineWarmup.py
-src/torchenhanced/Trainer.py
+requirements.txt
 src/torchenhanced/__init__.py
 src/torchenhanced/modules.py
+src/torchenhanced/trainer.py
 src/torchenhanced.egg-info/PKG-INFO
 src/torchenhanced.egg-info/SOURCES.txt
 src/torchenhanced.egg-info/dependency_links.txt
 src/torchenhanced.egg-info/requires.txt
 src/torchenhanced.egg-info/top_level.txt
+src/torchenhanced/ml/__init__.py
+src/torchenhanced/ml/functional/__init__.py
+src/torchenhanced/ml/functional/batch_roll.py
+src/torchenhanced/ml/optim/__init__.py
+src/torchenhanced/ml/optim/cosine_warmup.py
 src/torchenhanced/util/__init__.py
 src/torchenhanced/util/color_compression.py
 src/torchenhanced/util/files.py
 src/torchenhanced/util/misc.py
 src/torchenhanced/util/visualize.py
-tests/test_Trainer.py
-tests/test_Trainer_mini.py
 tests/test_cosine.py
+tests/test_custom_dataset.py
+tests/test_modules.py
+tests/test_trainer.py
 tests/test_util.py
```

### Comparing `torchenhanced-0.2.9/tests/test_Trainer.py` & `torchenhanced-0.3.0b1/tests/test_trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,120 +23,146 @@
 
         self.layer = nn.Linear(hidden, out)
     
     def forward(self, x):
         return self.layer(x)
     
 class LinearTrainer(Trainer):
-    def __init__(self, run_name: str = None, project_name: str = None, state_save_loc=None,reach_plateau=100,run_config={}):
+    def __init__(self, run_name: str = None, project_name: str = None, save_loc=None,reach_plateau=100,run_config={},parallel=None,device='cpu'):
         model = LinSimple()
         opti = torch.optim.Adam(model.parameters(),lr=1e-3)
         schedo = lrsched.LinearLR(opti,start_factor=0.01,end_factor=1,total_iters=reach_plateau)
 
         super().__init__(model,optim=opti,scheduler=schedo, run_name=run_name, 
-                         project_name=project_name,state_save_loc=state_save_loc,run_config=run_config)
+                         project_name=project_name,save_loc=save_loc,
+                         run_config=run_config,parallel=parallel,device=device)
 
         self.dataset =Subset(MNIST(os.path.join(curfold,'data'),download=True,transform=t.ToTensor()),range(100))
     
     def get_loaders(self, batch_size, num_workers=0):
         self.loss_val = []
         return DataLoader(self.dataset, batch_size=batch_size, shuffle=False), DataLoader(self.dataset, batch_size=batch_size, shuffle=True)
     
     def process_batch(self, batch_data,**kwargs):
         x, y = batch_data
+        x = x.to(self.device)
+        y = y.to(self.device)
+
         x = x.reshape((x.shape[0],-1))
         
         pred = self.model(x) # (B,10)
         loss = F.cross_entropy(pred,y,reduction='mean') 
 
         # assert self.stepnum==data_dict['stepnum'], f"Stepnum mismatch {self.stepnum} vs {data_dict['stepnum']}"
         # assert self.step_log==data_dict['step_log'], f"Step_log mismatch {self.step_log} vs {data_dict['step_log']}"
         # assert self.epoch == data_dict['epoch'], f"Epoch mismatch {self.epoch} vs {data_dict['epoch']}"
         # assert self.batchnum == data_dict['batchnum'], f"Batchnum mismatch {self.batchnum} vs {data_dict['batchnum']}"
 
-        if(self.do_batch_log):
+        if(self.do_step_log):
             self.logger.log({'lossme/train':loss.item()},commit=False)
             self.logger.log({'other/lr':self.scheduler.get_last_lr()[0]},commit=False)
         
         return loss
     
     def process_batch_valid(self, batch_data):
         x, y = batch_data
+        x = x.to(self.device)
+        y = y.to(self.device)
         x = x.reshape((x.shape[0],-1))
         
         pred = self.model(x) # (B,10)
         loss = F.cross_entropy(pred,y,reduction='mean') 
 
         self.loss_val.append(loss.item())
 
         return loss
     
     def valid_log(self):
         self.logger.log({'lossme/valid':sum(self.loss_val)/len(self.loss_val)},commit=False)
         self.loss_val = []
         
 
-# FOR MANUAL TESTING, COULDN'T FIGURE OUT HOW TO AUTOMATE IT
-#EPOCHS :
-# trainer = LinearTrainer(run_name='test_epochs', project_name='test_torchenhanced', 
-#                         state_save_loc=os.path.join(curfold),reach_plateau=200, run_config={'manamajeff':True})
-# trainer.change_lr(1e-4)
-# if(os.path.exists(os.path.join(curfold,'test_torchenhanced','state','test_epochs.state'))):
-#     trainer.load_state(os.path.join(curfold,'test_torchenhanced','state','test_epochs.state'))
-# time.sleep(2)
-
-# trainer.train_epochs(epochs=100, batch_size=10, step_log=30, save_every=60,aggregate=2,batch_sched=True)
-
-# #STEPS :
-# trainer = LinearTrainer(run_name='test_steps', project_name='test_torchenhanced', state_save_loc=os.path.join(curfold),reach_plateau=1500)
-
-# trainer.change_lr(1e-4)
-# if(os.path.exists(os.path.join(curfold,'test_torchenhanced','state','test_steps.state'))):
-#     trainer.load_state(os.path.join(curfold,'test_torchenhanced','state','test_steps.state'))
+def test_parallel():
+    # Not much happening here, just test that we have no errors
+    # EPOCHS :
+    trainer = LinearTrainer(run_name='test_ep_paral', project_name='test_torchenhanced', 
+                            save_loc=os.path.join(curfold),reach_plateau=200, 
+                            run_config={'manamajeff':True},parallel=['cuda:0'],device='cpu')
+    trainer.change_lr(1e-4)
+
+    assert trainer.parallel_train, 'Trainer not parallelized'
+
+    if(os.path.exists(os.path.join(curfold,'test_torchenhanced','state','test_ep_paral.state'))):
+        trainer.load_state(os.path.join(curfold,'test_torchenhanced','state','test_ep_paral.state'))
+    time.sleep(2)
+
+    trainer.train_epochs(epochs=20, batch_size=10, step_log=50, save_every=10,aggregate=2,batch_sched=True)
+
+    #STEPS :
+    trainer = LinearTrainer(run_name='test_steps_paral', project_name='test_torchenhanced', save_loc=os.path.join(curfold),
+                            reach_plateau=1500,parallel=['cuda:0'],device='cpu')
+
+    trainer.change_lr(1e-4)
+    if(os.path.exists(os.path.join(curfold,'test_torchenhanced','state','test_steps_paral.state'))):
+        trainer.load_state(os.path.join(curfold,'test_torchenhanced','state','test_steps_paral.state'))
+
+    time.sleep(2)
+    trainer.train_steps(steps=200, batch_size=10, step_log=50, save_every=50,aggregate=2, valid_every=100)
+
+def test_aggregate():
+    trainer = LinearTrainer(run_name='test_aggregate', project_name='test_torchenhanced', 
+                            save_loc=os.path.join(curfold),reach_plateau=200)
+    
+    trainer.train_steps(steps=200, batch_size=10, step_log=30, save_every=60,aggregate=2, valid_every=100)
+
+    assert trainer.batches == 400, f"Batch mismatch : {trainer.batches} vs expected 400"
+    assert trainer.steps_done == 200, f"Step mismatch : {trainer.steps_done} vs expected 200"
 
-# time.sleep(2)
-# trainer.train_steps(steps=1000, batch_size=10, step_log=30, save_every=60,aggregate=2, valid_every=100)
 
 
 def test_resume_train():
-    trainer = LinearTrainer(run_name='test_resume_train', project_name='test_torchenhanced', state_save_loc=os.path.join(curfold),reach_plateau=1500)
+    trainer = LinearTrainer(run_name='test_resume_train', project_name='test_torchenhanced', save_loc=os.path.join(curfold),
+                            reach_plateau=1500)
     trainer.change_lr(1e-4)
-    trainer.train_steps(steps=1000, batch_size=200, step_log=30, save_every=60,aggregate=2, valid_every=100)
+    trainer.train_steps(steps=200, batch_size=10, step_log=5, save_every=60,aggregate=2, valid_every=100)
     trainer.save_state()
     print(f'Finished at batches : {trainer.batches}, epochs : {trainer.epochs}, steps : {trainer.steps_done}')
     
     # Test with resuming
-    trainer2 = LinearTrainer(run_name='test_with_resume', project_name='test_torchenhanced', state_save_loc=os.path.join(curfold),reach_plateau=1500)
+    trainer2 = LinearTrainer(run_name='test_with_resume', project_name='test_torchenhanced', save_loc=os.path.join(curfold),reach_plateau=1500)
     trainer2.change_lr(1e-4)
     trainer2.load_state(os.path.join(curfold,'test_torchenhanced','state','test_resume_train.state')) # Load the state
-    trainer2.train_steps(steps=200, batch_size=10, step_log=30, save_every=3000,aggregate=2, valid_every=100, resume_batches=True)
+    trainer2.train_steps(steps=150, batch_size=10, step_log=5, save_every=3000,aggregate=2, valid_every=100, resume_batches=True)
 
     # Test without resuming
-    trainer3 = LinearTrainer(run_name='test_without_resume', project_name='test_torchenhanced', state_save_loc=os.path.join(curfold),reach_plateau=1500)
+    trainer3 = LinearTrainer(run_name='test_without_resume', project_name='test_torchenhanced', save_loc=os.path.join(curfold),reach_plateau=1500)
     trainer3.change_lr(1e-4)
     trainer3.load_state(os.path.join(curfold,'test_torchenhanced','state','test_resume_train.state')) # Load the state
-    trainer3.train_steps(steps=200, batch_size=10, step_log=30, save_every=3000,aggregate=2, valid_every=100)
+    trainer3.train_steps(steps=150, batch_size=10, step_log=5, save_every=3000,aggregate=2, valid_every=100, resume_batches=False)
 
     assert trainer2.batches == trainer3.batches, f"Batch mismatch : {trainer2.batches} vs {trainer.batches}"
     assert trainer2.epochs == trainer3.epochs, f"Epoch mismatch : {trainer2.epochs} vs {trainer.epochs}"
     assert trainer2.steps_done == trainer3.steps_done, f"Step mismatch : {trainer2.steps_done} vs {trainer.steps_done}"
 
     # Look on wandb to see if they are the same
 
-
-def test_Save_Weights():
-    lintra = LinearTrainer(run_name='test_save_weights', project_name='AnewDawn', state_save_loc=os.path.join(curfold))
+def test_save_weights():
+    lintra = LinearTrainer(run_name='test_save_weights', project_name='test_torchenhanced', save_loc=os.path.join(curfold))
     lintra.save_state()
 
-    Trainer.save_model_from_state(state_path=os.path.join(curfold,'AnewDawn','state','test_save_weights.state'),
-                                 save_dir=os.path.join(curfold,'AnewDawn'),name='testJEFF')
+    Trainer.save_model_from_state(state_path=os.path.join(curfold,'test_torchenhanced','state','test_save_weights.state'),
+                                 save_dir=os.path.join(curfold,'test_torchenhanced'),name='testJEFF')
 
-    assert os.path.isfile(os.path.join(curfold,'AnewDawn','testJEFF.pt')), "Weights not found"
-    assert os.path.isfile(os.path.join(curfold,'AnewDawn','testJEFF.config')), "Config not found"
+    assert os.path.isfile(os.path.join(curfold,'test_torchenhanced','testJEFF.pt')), "Weights not found"
+    assert os.path.isfile(os.path.join(curfold,'test_torchenhanced','testJEFF.config')), "Config not found"
 
 def test_Trainer_config():
     ma = LinSimple(hidden=32,out=15)
     config = ma.config
-    assert config == {'hidden':32, 'out':15, 'name':'LinSimple'}, f"Invalid config : {config}"
+    assert config == {'hidden':32, 'out':15}, f"Invalid config : {config}, should be {{'hidden':32, 'out':15}}"
 
 
 # Probably need to add more unit_tests...
+test_save_weights()
+test_parallel()
+test_aggregate()
+test_resume_train()
```

### Comparing `torchenhanced-0.2.9/tests/test_Trainer_mini.py` & `torchenhanced-0.3.0b1/tests/test_custom_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,35 +28,35 @@
         # print('Dispensing item nb: ',index)
         return self.data[index],self.targets[index] # (1,1), (1,1)
     
     def __len__(self):
         return len(self.data)
 
 class LinearTrainer(Trainer):
-    def __init__(self, run_name: str = None, project_name: str = None, state_save_loc=None,reach_plateau=100,run_config={}):
+    def __init__(self, run_name: str = None, project_name: str = None, save_loc=None,reach_plateau=100,run_config={}):
         model = LinSimple()
         opti = torch.optim.Adam(model.parameters(),lr=1e-3)
         schedo = lrsched.LinearLR(opti,start_factor=0.01,end_factor=1,total_iters=reach_plateau)
 
         super().__init__(model,optim=opti,scheduler=schedo, run_name=run_name, 
-                         project_name=project_name,state_save_loc=state_save_loc,run_config=run_config)
+                         project_name=project_name,save_loc=save_loc,run_config=run_config)
 
         self.dataset =SimpleDataset() # Numbers from 0 to 99
         self.loss_val = []
         
     def get_loaders(self, batch_size, num_workers=0):
         return DataLoader(self.dataset, batch_size=batch_size, shuffle=False),None
     
     def process_batch(self, batch_data,**kwargs):
         x, y = batch_data # (B,1), (B,1)
         print(f'Processing batch {self.batches} : {x}')
         pred = self.model(x) # (B,1)
         loss = ((pred-y)**2).mean() # MSE
 
-        if(self.do_batch_log):
+        if(self.do_step_log):
             self.logger.log({'lossme/train':loss.item()},commit=False)
             self.logger.log({'other/lr':self.scheduler.get_last_lr()[0]},commit=False)
         
         return loss
     
     def process_batch_valid(self, batch_data):
         x, y = batch_data # (B,1), (B,1)
@@ -73,31 +73,27 @@
         self.loss_val = []
         
 
 def test_resume_train():
     """
         Testing is not automatic... Gotta look at the output, whether it does resume at the correct batch
     """
-    trainer = LinearTrainer(run_name='test_saveforresume', project_name='test_torchenhanced', state_save_loc=os.path.join(curfold),reach_plateau=7)
+    trainer = LinearTrainer(run_name='test_saveforresume', project_name='test_torchenhanced', save_loc=os.path.join(curfold),reach_plateau=7)
     print('-----------------INITIAL TRAINING-----------------')
-    trainer.train_steps(steps=115, batch_size=1, step_log=1,batch_tqdm=False, save_every=5,aggregate=2, valid_every=1)
+    trainer.train_steps(steps=29, batch_size=1, step_log=1, save_every=5,aggregate=2, valid_every=1)
     # print(f'Finished at batches : {trainer.batches}, epochs : {trainer.epochs}, steps : {trainer.steps_done}')
     
     # Test without resuming
-    trainer3 = LinearTrainer(run_name='test_without_resume', project_name='test_torchenhanced', state_save_loc=os.path.join(curfold),reach_plateau=7)
+    trainer3 = LinearTrainer(run_name='test_without_resume', project_name='test_torchenhanced', save_loc=os.path.join(curfold),reach_plateau=7)
     print('-----------------WITHOUT RESUMING TRAINING-----------------')
     trainer3.load_state(os.path.join(curfold,'test_torchenhanced','state','test_saveforresume.state')) # Load the state
-    trainer3.train_steps(steps=5, batch_size=1, step_log=1, batch_tqdm=False,save_every=3000,aggregate=2, valid_every=1,resume_batches=False)
+    trainer3.train_steps(steps=5, batch_size=1, step_log=1, save_every=5,aggregate=2, valid_every=1,resume_batches=False,pickup=False)
 
     # Test with resuming
-    trainer2 = LinearTrainer(run_name='test_with_resume', project_name='test_torchenhanced', state_save_loc=os.path.join(curfold),reach_plateau=7)
+    trainer2 = LinearTrainer(run_name='test_with_resume', project_name='test_torchenhanced', save_loc=os.path.join(curfold),reach_plateau=7)
     print('-----------------RESUMING TRAINING-----------------')
     trainer2.load_state(os.path.join(curfold,'test_torchenhanced','state','test_saveforresume.state')) # Load the state
-    trainer2.train_steps(steps=5, batch_size=1, step_log=1, batch_tqdm=False,save_every=3000,aggregate=2, valid_every=1,resume_batches=True)
+    trainer2.train_steps(steps=29, batch_size=1, step_log=1, save_every=5,aggregate=2, valid_every=1,resume_batches=True,pickup=True)
 
 
-    assert trainer2.batches == trainer3.batches, f"Batch mismatch : {trainer2.batches} vs {trainer.batches}"
-    assert trainer2.epochs == trainer3.epochs, f"Epoch mismatch : {trainer2.epochs} vs {trainer.epochs}"
-    assert trainer2.steps_done == trainer3.steps_done, f"Step mismatch : {trainer2.steps_done} vs {trainer.steps_done}"
-
 if __name__ == "__main__":
     test_resume_train()
```

### Comparing `torchenhanced-0.2.9/tests/test_cosine.py` & `torchenhanced-0.3.0b1/tests/test_cosine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch,sys,pathlib
 sys.path.append(pathlib.Path(__file__).parent.parent.as_posix())
-from torchenhanced import CosineWarmup
+from src.torchenhanced.ml.optim import CosineWarmup
 import matplotlib.pyplot as plt
 
 def test_cosine():
     pass #(for manual thingy only)
     # opti = torch.optim.SGD([torch.zeros(1)],lr=0.1)
     # sched = CosineWarmup(optimizer=opti, warmup_steps=10, T_0=100,
     #                      lr_shrink=0.8,lr_init=1e-3,T_mult=1,eta_min=1e-3)
```

### Comparing `torchenhanced-0.2.9/tests/test_util.py` & `torchenhanced-0.3.0b1/tests/test_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch,sys,pathlib
 sys.path.append(pathlib.Path(__file__).parent.parent.as_posix())
 
 from src.torchenhanced.util import *
-
+from src.torchenhanced.util.misc import coord_to_flat
 
 def test_coord_to_flat_batch():
     unfolded = torch.randint(0,100,(3,4,5,6)) #4-dim coord tensor
     folded = unfolded.reshape((-1))
 
     dimensions = unfolded.shape
     testcoord = torch.tensor([[1,2,3,4],[0,2,3,2]]) # Set of coordinate points
```

