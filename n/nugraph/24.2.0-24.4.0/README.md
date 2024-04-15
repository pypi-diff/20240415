# Comparing `tmp/nugraph-24.2.0.tar.gz` & `tmp/nugraph-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nugraph-24.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nugraph-24.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nugraph-24.2.0.tar` & `nugraph-24.4.0.tar`

### file list

```diff
@@ -1,36 +1,50 @@
--rw-r--r--   0        0        0     1087 2023-06-16 18:33:40.021691 nugraph-24.2.0/LICENSE
--rw-r--r--   0        0        0     3249 2024-01-04 20:26:50.669885 nugraph-24.2.0/README.md
--rw-r--r--   0        0        0      163 2024-02-23 18:31:06.841162 nugraph-24.2.0/nugraph/__init__.py
--rw-r--r--   0        0        0     2100 2023-08-28 22:21:49.208721 nugraph-24.2.0/nugraph/data/.ipynb_checkpoints/BalanceSampler-checkpoint.py
--rw-r--r--   0        0        0     7541 2023-08-28 22:49:29.254574 nugraph-24.2.0/nugraph/data/.ipynb_checkpoints/H5DataModule-checkpoint.py
--rw-r--r--   0        0        0      803 2023-07-13 23:50:04.719437 nugraph-24.2.0/nugraph/data/.ipynb_checkpoints/H5Dataset-checkpoint.py
--rw-r--r--   0        0        0     2092 2023-10-14 14:54:54.807206 nugraph-24.2.0/nugraph/data/BalanceSampler.py
--rw-r--r--   0        0        0     7684 2024-01-04 20:26:50.670628 nugraph-24.2.0/nugraph/data/H5DataModule.py
--rw-r--r--   0        0        0      625 2023-08-31 15:14:34.358389 nugraph-24.2.0/nugraph/data/H5Dataset.py
--rw-r--r--   0        0        0       86 2023-06-16 18:33:40.022101 nugraph-24.2.0/nugraph/data/__init__.py
--rw-r--r--   0        0        0      892 2024-02-23 14:58:52.287445 nugraph-24.2.0/nugraph/meta.yaml
--rw-r--r--   0        0        0     9182 2023-07-13 23:30:50.658002 nugraph-24.2.0/nugraph/models/.ipynb_checkpoints/NuGraph2-checkpoint.py
--rw-r--r--   0        0        0     8983 2023-07-13 23:52:38.821448 nugraph-24.2.0/nugraph/models/.ipynb_checkpoints/decoders-checkpoint.py
--rw-r--r--   0        0        0    12120 2024-01-20 02:44:56.281267 nugraph-24.2.0/nugraph/models/NuGraph2.py
--rw-r--r--   0        0        0       45 2023-06-16 18:33:40.022344 nugraph-24.2.0/nugraph/models/__init__.py
--rw-r--r--   0        0        0    12007 2024-02-23 14:58:52.287601 nugraph-24.2.0/nugraph/models/decoders.py
--rw-r--r--   0        0        0      560 2024-01-20 02:44:56.282199 nugraph-24.2.0/nugraph/models/encoder.py
--rw-r--r--   0        0        0        0 2024-01-04 20:29:54.551406 nugraph-24.2.0/nugraph/models/event.py
--rw-r--r--   0        0        0     2779 2024-01-20 02:44:56.282716 nugraph-24.2.0/nugraph/models/nexus.py
--rw-r--r--   0        0        0     2085 2024-01-20 02:44:56.282827 nugraph-24.2.0/nugraph/models/plane.py
--rw-r--r--   0        0        0     1389 2023-06-26 17:27:21.928314 nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/FeatureNorm-checkpoint.py
--rw-r--r--   0        0        0      322 2023-07-13 23:28:07.254448 nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/LogCoshLoss-checkpoint.py
--rw-r--r--   0        0        0     6877 2023-07-11 16:14:18.458245 nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/ObjCondensationLoss-checkpoint.py
--rw-r--r--   0        0        0      455 2023-06-26 17:27:21.928380 nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/PositionFeatures-checkpoint.py
--rw-r--r--   0        0        0      782 2023-07-13 23:23:59.868518 nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/RecallLoss-checkpoint.py
--rw-r--r--   0        0        0      263 2023-07-13 23:28:47.941528 nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0        0 2023-07-11 17:51:58.774839 nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/untitled-checkpoint.py
--rw-r--r--   0        0        0     1389 2023-06-26 17:27:21.928314 nugraph-24.2.0/nugraph/util/FeatureNorm.py
--rw-r--r--   0        0        0      436 2023-10-14 14:54:54.808065 nugraph-24.2.0/nugraph/util/LogCoshLoss.py
--rw-r--r--   0        0        0     1650 2023-11-17 19:34:47.491485 nugraph-24.2.0/nugraph/util/ObjCondensationLoss.py
--rw-r--r--   0        0        0      455 2023-06-26 17:27:21.928380 nugraph-24.2.0/nugraph/util/PositionFeatures.py
--rw-r--r--   0        0        0      782 2023-10-14 14:54:54.808202 nugraph-24.2.0/nugraph/util/RecallLoss.py
--rw-r--r--   0        0        0      283 2023-11-17 19:34:47.491717 nugraph-24.2.0/nugraph/util/__init__.py
--rw-r--r--   0        0        0      711 2023-10-14 14:54:54.808430 nugraph-24.2.0/nugraph/util/scriptutils.py
--rw-r--r--   0        0        0      639 2023-11-17 19:34:49.861026 nugraph-24.2.0/pyproject.toml
--rw-r--r--   0        0        0     3876 1970-01-01 00:00:00.000000 nugraph-24.2.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-10-19 20:06:48.689173 nugraph-24.4.0/.gitattributes
+-rw-r--r--   0        0        0     3222 2024-03-23 02:17:42.863451 nugraph-24.4.0/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-23 17:30:38.617828 nugraph-24.4.0/LICENSE
+-rw-r--r--   0        0        0     3249 2024-03-13 13:40:00.109322 nugraph-24.4.0/README.md
+-rw-r--r--   0        0        0       37 2023-07-11 20:24:57.531451 nugraph-24.4.0/notebooks/.gitattributes
+-rw-r--r--   0        0        0    10374 2023-10-19 20:06:48.689173 nugraph-24.4.0/notebooks/evaluate.ipynb
+-rw-r--r--   0        0        0     5402 2024-03-13 13:40:00.109322 nugraph-24.4.0/notebooks/inference-time.ipynb
+-rw-r--r--   0        0        0    11736 2024-03-13 19:15:19.136256 nugraph-24.4.0/notebooks/plot.ipynb
+-rw-r--r--   0        0        0     5482 2024-03-13 19:15:19.136256 nugraph-24.4.0/notebooks/process.ipynb
+-rw-r--r--   0        0        0     1498 2023-10-19 20:06:48.689173 nugraph-24.4.0/notebooks/tensorboard.ipynb
+-rw-r--r--   0        0        0    11878 2024-03-13 19:15:19.136256 nugraph-24.4.0/notebooks/test.ipynb
+-rw-r--r--   0        0        0     5008 2024-04-15 14:45:48.838263 nugraph-24.4.0/notebooks/train.ipynb
+-rw-r--r--   0        0        0      163 2024-04-15 14:51:27.902753 nugraph-24.4.0/nugraph/__init__.py
+-rw-r--r--   0        0        0     2092 2023-10-19 20:06:48.689173 nugraph-24.4.0/nugraph/data/BalanceSampler.py
+-rw-r--r--   0        0        0     7684 2024-04-15 14:45:48.842263 nugraph-24.4.0/nugraph/data/H5DataModule.py
+-rw-r--r--   0        0        0      625 2023-08-29 18:49:39.299150 nugraph-24.4.0/nugraph/data/H5Dataset.py
+-rw-r--r--   0        0        0       86 2023-05-22 17:14:24.299289 nugraph-24.4.0/nugraph/data/__init__.py
+-rw-r--r--   0        0        0      892 2024-04-15 14:50:02.982616 nugraph-24.4.0/nugraph/meta.yaml
+-rw-r--r--   0        0        0       76 2024-03-23 02:17:42.863451 nugraph-24.4.0/nugraph/models/__init__.py
+-rw-r--r--   0        0        0    11093 2024-04-15 14:45:34.616900 nugraph-24.4.0/nugraph/models/nugraph2/NuGraph2.py
+-rw-r--r--   0        0        0       45 2024-03-23 02:17:42.863451 nugraph-24.4.0/nugraph/models/nugraph2/__init__.py
+-rw-r--r--   0        0        0     6386 2024-03-23 02:17:42.863451 nugraph-24.4.0/nugraph/models/nugraph2/decoders.py
+-rw-r--r--   0        0        0      752 2024-03-23 02:17:42.863451 nugraph-24.4.0/nugraph/models/nugraph2/encoder.py
+-rw-r--r--   0        0        0      658 2024-03-23 02:17:42.863451 nugraph-24.4.0/nugraph/models/nugraph2/linear.py
+-rw-r--r--   0        0        0     3228 2024-04-15 14:45:34.616900 nugraph-24.4.0/nugraph/models/nugraph2/nexus.py
+-rw-r--r--   0        0        0     2425 2024-03-23 02:17:42.863451 nugraph-24.4.0/nugraph/models/nugraph2/plane.py
+-rw-r--r--   0        0        0    12773 2024-04-15 14:45:56.394987 nugraph-24.4.0/nugraph/models/nugraph3/NuGraph3.py
+-rw-r--r--   0        0        0       45 2024-03-23 02:17:42.863451 nugraph-24.4.0/nugraph/models/nugraph3/__init__.py
+-rw-r--r--   0        0        0    12008 2024-04-15 14:45:56.394987 nugraph-24.4.0/nugraph/models/nugraph3/decoders.py
+-rw-r--r--   0        0        0      560 2024-04-11 03:58:51.215214 nugraph-24.4.0/nugraph/models/nugraph3/encoder.py
+-rw-r--r--   0        0        0     2779 2024-04-15 14:45:56.394987 nugraph-24.4.0/nugraph/models/nugraph3/nexus.py
+-rw-r--r--   0        0        0     2085 2024-04-15 14:45:56.394987 nugraph-24.4.0/nugraph/models/nugraph3/plane.py
+-rw-r--r--   0        0        0     1389 2023-11-09 17:49:26.829145 nugraph-24.4.0/nugraph/util/FeatureNorm.py
+-rw-r--r--   0        0        0      436 2024-03-23 02:12:13.549378 nugraph-24.4.0/nugraph/util/LogCoshLoss.py
+-rw-r--r--   0        0        0     1650 2024-04-15 14:45:48.842263 nugraph-24.4.0/nugraph/util/ObjCondensationLoss.py
+-rw-r--r--   0        0        0      455 2023-06-28 16:28:35.034179 nugraph-24.4.0/nugraph/util/PositionFeatures.py
+-rw-r--r--   0        0        0      782 2023-10-19 20:06:48.693173 nugraph-24.4.0/nugraph/util/RecallLoss.py
+-rw-r--r--   0        0        0      283 2024-03-13 13:40:00.109322 nugraph-24.4.0/nugraph/util/__init__.py
+-rw-r--r--   0        0        0      711 2023-10-19 20:06:48.693173 nugraph-24.4.0/nugraph/util/scriptutils.py
+-rw-r--r--   0        0        0      639 2023-11-17 17:55:45.653471 nugraph-24.4.0/pyproject.toml
+-rw-r--r--   0        0        0      492 2023-06-28 16:28:35.038180 nugraph-24.4.0/scripts/loss_landscape.py
+-rwxr-xr-x   0        0        0     1431 2023-09-20 20:39:53.571291 nugraph-24.4.0/scripts/merge.py
+-rwxr-xr-x   0        0        0     3440 2024-03-23 02:17:42.863451 nugraph-24.4.0/scripts/plot.py
+-rwxr-xr-x   0        0        0      637 2023-07-05 21:06:47.565903 nugraph-24.4.0/scripts/prepare.py
+-rwxr-xr-x   0        0        0     1040 2023-10-19 20:06:48.693173 nugraph-24.4.0/scripts/process.py
+-rw-r--r--   0        0        0      263 2024-03-13 13:40:00.109322 nugraph-24.4.0/scripts/process_batch.sh
+-rwxr-xr-x   0        0        0     1827 2024-03-23 02:17:42.863451 nugraph-24.4.0/scripts/test.py
+-rwxr-xr-x   0        0        0     3117 2024-04-15 14:33:24.630926 nugraph-24.4.0/scripts/train.py
+-rw-r--r--   0        0        0      215 2023-12-15 18:26:54.535461 nugraph-24.4.0/scripts/train_batch.sh
+-rw-r--r--   0        0        0     3876 1970-01-01 00:00:00.000000 nugraph-24.4.0/PKG-INFO
```

### Comparing `nugraph-24.2.0/LICENSE` & `nugraph-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/README.md` & `nugraph-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/nugraph/data/.ipynb_checkpoints/BalanceSampler-checkpoint.py` & `nugraph-24.4.0/nugraph/data/BalanceSampler.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self.batch_size = batch_size
         self.balance_frac = balance_frac
 
     def __iter__(self):
         # Retrieve dataset size
         dset_len = len(self.datasize)
         # Calculate number of batches in dataset
-        num_batches = np.floor(dset_len / self.batch_size)
+        num_batches = int(np.floor(dset_len / self.batch_size))
 
         # Assign N as a fraction of the dataset length
         num_outliers = int(np.floor(dset_len * self.balance_frac))
         if num_outliers > dset_len:
             print('Number of outliers is greater than dataset size')
             sys.exit()
 
@@ -30,33 +30,33 @@
         sample_indices = sample_indices[:dset_len-num_outliers]
 
         # Shuffle indices of n-largest values
         np.random.shuffle(n_largest_indices)
         np.random.shuffle(sample_indices)
 
         # Create as many bins as the number of batches
-        bins = []
-        for i in range(num_batches):
-            bins.append([])
+        bins = [ [] for i in range(num_batches) ]
 
         # Distribute the n-largest sample indices to each bin
         for i, sample_index in enumerate(n_largest_indices):
-            bin_index = i % self.batch_size
-            bins[bin_index].append(sample_index)
+            idx = i % num_batches
+            bins[idx].append(sample_index)
 
         # Distribute the remaining samples to each bin
-        #sample_indices = list(reversed(sample_indices))
+        offset = idx + 1
         for i, sample_index in enumerate(sample_indices):
-            bin_index = i % self.batch_size
-            bins[bin_index].append(sample_index)
+            idx = (i + offset) % num_batches
+            # drop last batch
+            if len(bins[idx]) == self.batch_size:
+                break
+            bins[idx].append(sample_index)
 
         # Shuffle each bin and append to indices array
         indices = []
         for bin in bins:
-            print(len(bins))
             np.random.shuffle(bin)
             indices += bin
 
         return iter(indices)
 
     def __len__(self):
         return len(self.datasize)
```

### Comparing `nugraph-24.2.0/nugraph/data/.ipynb_checkpoints/H5DataModule-checkpoint.py` & `nugraph-24.4.0/nugraph/data/H5DataModule.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from torch import tensor, cat
 from torch.utils.data import random_split
 from torch_geometric.loader import DataLoader
 from torch_geometric.transforms import Compose
 from pytorch_lightning import LightningDataModule
 
-from ..data import H5Dataset, BalanceSampler, SampleSizes
+from ..data import H5Dataset, BalanceSampler
 from ..util import PositionFeatures, FeatureNormMetric, FeatureNorm
 
 class H5DataModule(LightningDataModule):
     """PyTorch Lightning data module for neutrino graph data."""
     def __init__(self,
                  data_path: str,
                  batch_size: int,
@@ -26,14 +26,17 @@
 
         # for this HDF5 dataloader, worker processes slow things down
         # so we silence PyTorch Lightning's warnings
         warnings.filterwarnings("ignore", ".*does not have many workers.*")
 
         self.filename = data_path
         self.batch_size = batch_size
+        if shuffle != 'random' and shuffle != 'balance':
+            print('shuffle argument must be "random" or "balance".')
+            sys.exit()
         self.shuffle = shuffle
         self.balance_frac = balance_frac
 
         with h5py.File(self.filename) as f:
 
             # load metadata
             try:
@@ -54,15 +57,15 @@
                 train_samples = f['samples/train'].asstr()[()]
                 val_samples = f['samples/validation'].asstr()[()]
                 test_samples = f['samples/validation'].asstr()[()]
             except:
                 print('Sample splits not found in file! Call "generate_samples" to create them.')
                 sys.exit()
 
-            # load sample sizes
+            # load data sizes
             try:
                 self.train_datasize = f['datasize/train'][()]
             except:
                 print('Data size array not found in file! Call "generate_samples" to create it.')
                 sys.exit()
 
             # load feature normalisations
@@ -167,20 +170,20 @@
         return DataLoader(self.test_dataset,
                           batch_size=self.batch_size)
 
     @staticmethod
     def add_data_args(parser: ArgumentParser) -> ArgumentParser:
         data = parser.add_argument_group('data', 'Data module configuration')
         data.add_argument('--data-path', type=str,
-                          default='/data/CHEP2023/filtered.gnn.h5',
+                          default='/raid/uboone/NuGraph2/NG2-paper.gnn.h5',
                           help='Location of input data file')
         data.add_argument('--batch-size', type=int, default=64,
                           help='Size of each batch of graphs')
         data.add_argument('--limit_train_batches', type=int, default=None,
                           help='Max number of training batches to be used')
         data.add_argument('--limit_val_batches', type=int, default=None,
                           help='Max number of validation batches to be used')
-        data.add_argument('--shuffle', type=str, default='random',
+        data.add_argument('--shuffle', type=str, default='balance',
                           help='Dataset shuffling scheme to use')
         data.add_argument('--balance-frac', type=float, default=0.1,
                           help='Fraction of dataset to use for workload balancing')
         return parser
```

### Comparing `nugraph-24.2.0/nugraph/data/.ipynb_checkpoints/H5Dataset-checkpoint.py` & `nugraph-24.4.0/nugraph/data/H5Dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,13 @@
     def __init__(self,
                  filename: str,
                  samples: list[str],
                  transform: Optional[Callable] = None):
         super().__init__(transform=transform)
         self._interface = io.H5Interface(h5py.File(filename))
         self._samples = samples
-        print('WARNING: temporary hack fix for 3D vertex in DataLoader. this must be fixed in pynuml before merging')
 
     def len(self) -> int:
         return len(self._samples)
 
     def get(self, idx: int) -> 'pyg.data.HeteroData':
-        data = self._interface.load_heterodata(self._samples[idx])
-        data['evt'].y_vtx.unsqueeze_(0)
-        return data
+        return self._interface.load_heterodata(self._samples[idx])
```

### Comparing `nugraph-24.2.0/nugraph/meta.yaml` & `nugraph-24.4.0/nugraph/meta.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% set name = "nugraph" %}
-{% set version = "24.2.0" %}
+{% set version = "24.4.0" %}
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   url: https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/nugraph-{{ version }}.tar.gz
```

### Comparing `nugraph-24.2.0/nugraph/models/.ipynb_checkpoints/NuGraph2-checkpoint.py` & `nugraph-24.4.0/nugraph/models/nugraph3/NuGraph3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-from argparse import ArgumentParser
+import argparse
 import warnings
+import psutil
 
+import torch
 from torch import Tensor, cat, empty
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import OneCycleLR
 from pytorch_lightning import LightningModule
+from torch_geometric.data import Batch, HeteroData
+from torch_geometric.utils import unbatch
 
 from .encoder import Encoder
 from .plane import PlaneNet
 from .nexus import NexusNet
 from .decoders import SemanticDecoder, FilterDecoder, EventDecoder, VertexDecoder
 
-class NuGraph2(LightningModule):
+from ...data import H5DataModule
+
+class NuGraph3(LightningModule):
     """PyTorch Lightning module for model training.
 
     Wrap the base model in a LightningModule wrapper to handle training and
     inference, and compute training metrics."""
     def __init__(self,
                  in_features: int = 4,
-                 node_features: int = 8,
-                 edge_features: int = 8,
-                 sp_features: int = 8,
+                 planar_features: int = 128,
+                 nexus_features: int = 32,
+                 vertex_aggr: str = 'lstm',
+                 vertex_lstm_features: int = 64,
+                 vertex_mlp_features: list[int] = [ 64 ],
                  planes: list[str] = ['u','v','y'],
                  semantic_classes: list[str] = ['MIP','HIP','shower','michel','diffuse'],
                  event_classes: list[str] = ['numu','nue','nc'],
                  num_iters: int = 5,
-                 event_head: bool = True,
+                 event_head: bool = False,
                  semantic_head: bool = True,
-                 filter_head: bool = False,
+                 filter_head: bool = True,
                  vertex_head: bool = False,
                  checkpoint: bool = False,
                  lr: float = 0.001):
         super().__init__()
 
         warnings.filterwarnings("ignore", ".*NaN values found in confusion matrix.*")
 
@@ -40,59 +48,57 @@
         self.planes = planes
         self.semantic_classes = semantic_classes
         self.event_classes = event_classes
         self.num_iters = num_iters
         self.lr = lr
 
         self.encoder = Encoder(in_features,
-                               node_features,
+                               planar_features,
                                planes,
-                               semantic_classes)
+                              )
 
         self.plane_net = PlaneNet(in_features,
-                                  node_features,
-                                  edge_features,
-                                  len(semantic_classes),
+                                  planar_features,
                                   planes,
                                   checkpoint=checkpoint)
 
-        self.nexus_net = NexusNet(node_features,
-                                  edge_features,
-                                  sp_features,
-                                  len(semantic_classes),
+        self.nexus_net = NexusNet(planar_features,
+                                  nexus_features,
                                   planes,
                                   checkpoint=checkpoint)
 
         self.decoders = []
 
         if event_head:
             self.event_decoder = EventDecoder(
-                node_features,
+                planar_features,
                 planes,
-                semantic_classes,
                 event_classes)
             self.decoders.append(self.event_decoder)
 
         if semantic_head:
             self.semantic_decoder = SemanticDecoder(
-                node_features,
+                planar_features,
                 planes,
                 semantic_classes)
             self.decoders.append(self.semantic_decoder)
 
         if filter_head:
             self.filter_decoder = FilterDecoder(
-                node_features,
+                planar_features,
                 planes,
-                semantic_classes)
+            )
             self.decoders.append(self.filter_decoder)
             
         if vertex_head:
             self.vertex_decoder = VertexDecoder(
-                node_features,
+                planar_features,
+                vertex_aggr,
+                vertex_lstm_features,
+                vertex_mlp_features,
                 planes,
                 semantic_classes)
             self.decoders.append(self.vertex_decoder)
 
         if len(self.decoders) == 0:
             raise Exception('At least one decoder head must be enabled!')
 
@@ -102,34 +108,78 @@
                 edge_index_nexus: dict[str, Tensor],
                 nexus: Tensor,
                 batch: dict[str, Tensor]) -> dict[str, Tensor]:
         m = self.encoder(x)
         for _ in range(self.num_iters):
             # shortcut connect features
             for i, p in enumerate(self.planes):
-                m[p] = cat((m[p], x[p].detach().unsqueeze(1).expand(-1, m[p].size(1), -1)), dim=-1)
+                m[p] = torch.cat((m[p], x[p]), dim=-1)
             self.plane_net(m, edge_index_plane)
             self.nexus_net(m, edge_index_nexus, nexus)
         ret = {}
         for decoder in self.decoders:
             ret.update(decoder(m, batch))
         return ret
 
-    def step(self, batch):
+    def step(self, data: HeteroData | Batch,
+             stage: str = None,
+             confusion: bool = False):
+
+        # if it's a single data instance, convert to batch manually
+        if isinstance(data, Batch):
+            batch = data
+        else:
+            batch = Batch.from_data_list([data])
+
+        # unpack tensors to pass into forward function
         x = self(batch.collect('x'),
                  { p: batch[p, 'plane', p].edge_index for p in self.planes },
                  { p: batch[p, 'nexus', 'sp'].edge_index for p in self.planes },
-                 empty(batch['sp'].num_nodes, 0),
+                 torch.empty(batch['sp'].num_nodes, 0),
                  { p: batch[p].batch for p in self.planes })
-        for key, value in x.items():
-            batch.set_value_dict(key, value)
+
+        # append output tensors back onto input data object
+        if isinstance(data, Batch):
+            dlist = [ HeteroData() for i in range(data.num_graphs) ]
+            for attr, planes in x.items():
+                for p, t in planes.items():
+                    if t.size(0) == data[p].num_nodes:
+                        tlist = unbatch(t, data[p].batch)
+                    elif t.size(0) == data.num_graphs:
+                        tlist = unbatch(t, torch.arange(data.num_graphs))
+                    else:
+                        raise Exception(f'don\'t know how to unbatch attribute {attr}')
+                    for it_d, it_t in zip(dlist, tlist):
+                        it_d[p][attr] = it_t
+            tmp = Batch.from_data_list(dlist)
+            data.update(tmp)
+            for attr, planes in x.items():
+                for p in planes:
+                    data._slice_dict[p][attr] = tmp._slice_dict[p][attr]
+                    data._inc_dict[p][attr] = tmp._inc_dict[p][attr]
+
+        else:
+            for key, value in x.items():
+                data.set_value_dict(key, value)
+
+        total_loss = 0.
+        total_metrics = {}
+        for decoder in self.decoders:
+            loss, metrics = decoder.loss(data, stage, confusion)
+            total_loss += loss
+            total_metrics.update(metrics)
+            decoder.finalize(data)
+
+        return total_loss, total_metrics
 
     def on_train_start(self):
         hpmetrics = { 'max_lr': self.hparams.lr }
         self.logger.log_hyperparams(self.hparams, metrics=hpmetrics)
+        self.max_mem_cpu = 0.
+        self.max_mem_gpu = 0.
 
         scalars = {
             'loss': {'loss': [ 'Multiline', [ 'loss/train', 'loss/val' ]]},
             'acc': {}
         }
         for c in self.semantic_classes:
             scalars['acc'][c] = [ 'Multiline', [
@@ -137,89 +187,125 @@
                 f'semantic_accuracy_class_val/{c}'
             ]]
         self.logger.experiment.add_custom_scalars(scalars)
 
     def training_step(self,
                       batch,
                       batch_idx: int) -> float:
-        self.step(batch)
-        total_loss = 0.
-        for decoder in self.decoders:
-            loss, metrics = decoder.loss(batch, 'train')
-            total_loss += loss
-            self.log_dict(metrics, batch_size=batch.num_graphs)
-        self.log('loss/train', total_loss, batch_size=batch.num_graphs, prog_bar=True)
-        return total_loss
+        loss, metrics = self.step(batch, 'train')
+        self.log('loss/train', loss, batch_size=batch.num_graphs, prog_bar=True)
+        self.log_dict(metrics, batch_size=batch.num_graphs)
+        self.log_memory(batch, 'train')
+        return loss
 
     def validation_step(self,
                         batch,
                         batch_idx: int) -> None:
-        self.step(batch)
-        total_loss = 0.
-        for decoder in self.decoders:
-            loss, metrics = decoder.loss(batch, 'val', True)
-            total_loss += loss
-            self.log_dict(metrics, batch_size=batch.num_graphs)
-        self.log('loss/val', total_loss, batch_size=batch.num_graphs)
+        loss, metrics = self.step(batch, 'val', True)
+        self.log('loss/val', loss, batch_size=batch.num_graphs)
+        self.log_dict(metrics, batch_size=batch.num_graphs)
 
     def on_validation_epoch_end(self) -> None:
         epoch = self.trainer.current_epoch + 1
         for decoder in self.decoders:
             decoder.on_epoch_end(self.logger, 'val', epoch)
 
     def test_step(self,
                   batch,
                   batch_idx: int = 0) -> None:
-        self.step(batch)
-        total_loss = 0.
-        for decoder in self.decoders:
-            loss, metrics = decoder.loss(batch, 'test', True)
-            total_loss += loss
-            self.log_dict(metrics, batch_size=batch.num_graphs)
-        self.log('loss/test', total_loss, batch_size=batch.num_graphs)
+        loss, metrics = self.step(batch, 'test', True)
+        self.log('loss/test', loss, batch_size=batch.num_graphs)
+        self.log_dict(metrics, batch_size=batch.num_graphs)
+        self.log_memory(batch, 'test')
 
     def on_test_epoch_end(self) -> None:
         epoch = self.trainer.current_epoch + 1
         for decoder in self.decoders:
-            decoder.on_epoch_end(self.logger, 'val', epoch)
+            decoder.on_epoch_end(self.logger, 'test', epoch)
+
+    def predict_step(self,
+                     batch: Batch,
+                     batch_idx: int = 0) -> Batch:
+        self.step(batch)
+        return batch
 
     def configure_optimizers(self) -> tuple:
         optimizer = AdamW(self.parameters(),
                           lr=self.lr)
         onecycle = OneCycleLR(
                 optimizer,
                 max_lr=self.lr,
                 total_steps=self.trainer.estimated_stepping_batches)
         return [optimizer], {'scheduler': onecycle, 'interval': 'step'}
 
+    def log_memory(self, batch: Batch, stage: str) -> None:
+        # log CPU memory
+        if not hasattr(self, 'max_mem_cpu'):
+            self.max_mem_cpu = 0.
+        cpu_mem = psutil.Process().memory_info().rss / float(1073741824)
+        self.max_mem_cpu = max(self.max_mem_cpu, cpu_mem)
+        self.log(f'memory_cpu/{stage}', self.max_mem_cpu,
+                 batch_size=batch.num_graphs, reduce_fx=torch.max)
+
+        # log GPU memory
+        if not hasattr(self, 'max_mem_gpu'):
+            self.max_mem_gpu = 0.
+        if self.device != torch.device('cpu'):
+            gpu_mem = torch.cuda.memory_reserved(self.device)
+            gpu_mem = float(gpu_mem) / float(1073741824)
+            self.max_mem_gpu = max(self.max_mem_gpu, gpu_mem)
+            self.log(f'memory_gpu/{stage}', self.max_mem_gpu,
+                     batch_size=batch.num_graphs, reduce_fx=torch.max)
+
     @staticmethod
-    def add_model_args(parser: ArgumentParser) -> ArgumentParser:
+    def add_model_args(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
         '''Add argparse argpuments for model structure'''
-        model = parser.add_argument_group('model', 'NuGraph2 model configuration')
-        model.add_argument('--node-feats', type=int, default=64,
-                           help='Hidden dimensionality of 2D node convolutions')
-        model.add_argument('--edge-feats', type=int, default=16,
-                           help='Hidden dimensionality of edge convolutions')
-        model.add_argument('--sp-feats', type=int, default=16,
-                           help='Hidden dimensionality of spacepoint convolutions')
+        model = parser.add_argument_group('model', 'NuGraph3 model configuration')
+        model.add_argument('--num-iters', type=int, default=5,
+                           help='Number of message-passing iterations')
+        model.add_argument('--in-feats', type=int, default=4,
+                           help='Number of input node features')
+        model.add_argument('--planar-feats', type=int, default=128,
+                           help='Hidden dimensionality of planar convolutions')
+        model.add_argument('--nexus-feats', type=int, default=32,
+                           help='Hidden dimensionality of nexus convolutions')
+        model.add_argument('--vertex-aggr', type=str, default='lstm',
+                           help='Aggregation function for vertex decoder')
+        model.add_argument('--vertex-lstm-feats', type=int, default=32,
+                           help='Hidden dimensionality of vertex LSTM aggregation')
+        model.add_argument('--vertex-mlp-feats', type=int, nargs='*', default=[32],
+                           help='Hidden dimensionality of vertex decoder')
         model.add_argument('--event', action='store_true', default=False,
                            help='Enable event classification head')
         model.add_argument('--semantic', action='store_true', default=False,
                            help='Enable semantic segmentation head')
         model.add_argument('--filter', action='store_true', default=False,
                            help='Enable background filter head')
-        return parser
-
-    @staticmethod
-    def add_train_args(parser: ArgumentParser) -> ArgumentParser:
-        train = parser.add_argument_group('train', 'NuGraph2 training configuration')
-        train.add_argument('--no-checkpointing', action='store_true', default=False,
+        model.add_argument('--vertex', action='store_true', default=False,
+                           help='Enable vertex regression head')
+        model.add_argument('--no-checkpointing', action='store_true', default=False,
                            help='Disable checkpointing during training')
-        train.add_argument('--epochs', type=int, default=80,
+        model.add_argument('--epochs', type=int, default=80,
                            help='Maximum number of epochs to train for')
-        train.add_argument('--learning-rate', type=float, default=0.001,
+        model.add_argument('--learning-rate', type=float, default=0.001,
                            help='Max learning rate during training')
-        train.add_argument('--clip-gradients', type=float, default=None,
-                           help='Maximum value to clip gradient norm')
-        train.add_argument('--gamma', type=float, default=2,
-                           help='Focal loss gamma parameter')
         return parser
+
+    @classmethod
+    def from_args(cls, args: argparse.Namespace, nudata: H5DataModule) -> 'NuGraph3':
+        return cls(
+            in_features=args.in_feats,
+            planar_features=args.planar_feats,
+            nexus_features=args.nexus_feats,
+            vertex_aggr=args.vertex_aggr,
+            vertex_lstm_features=args.vertex_lstm_feats,
+            vertex_mlp_features=args.vertex_mlp_feats,
+            planes=nudata.planes,
+            semantic_classes=nudata.semantic_classes,
+            event_classes=nudata.event_classes,
+            num_iters=args.num_iters,
+            event_head=args.event,
+            semantic_head=args.semantic,
+            filter_head=args.filter,
+            vertex_head=args.vertex,
+            checkpoint=not args.no_checkpointing,
+            lr=args.learning_rate)
```

### Comparing `nugraph-24.2.0/nugraph/models/.ipynb_checkpoints/decoders-checkpoint.py` & `nugraph-24.4.0/nugraph/models/nugraph3/decoders.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 from typing import Any, Callable
 
 from abc import ABC
 
-from torch import Tensor, cat
+from torch import Tensor, tensor, cat
 import torch.nn as nn
 from torch_geometric.nn.aggr import SoftmaxAggregation, LSTMAggregation
+from torch_geometric.nn.resolver import aggregation_resolver as aggr_resolver
 
 import torchmetrics as tm
 
 import matplotlib.pyplot as plt
 import seaborn as sn
+import math
 
-from .linear import ClassLinear
-from ..util import FocalLoss, RecallLoss, LogCoshLoss
+from ...util import RecallLoss, LogCoshLoss, ObjCondensationLoss
 
 class DecoderBase(nn.Module, ABC):
     '''Base class for all NuGraph decoders'''
     def __init__(self,
                  name: str,
                  planes: list[str],
                  classes: list[str],
-                 loss_func: Callable):
+                 loss_func: Callable,
+                 weight: float,
+                 temperature: float = 0.):
         super().__init__()
         self.name = name
         self.planes = planes
         self.classes = classes
         self.loss_func = loss_func
+        self.weight = weight
+        self.temp = nn.Parameter(tensor(temperature))
         self.confusion = nn.ModuleDict()
 
     def arrange(self, batch) -> tuple[Tensor, Tensor]:
         raise NotImplementedError
 
     def metrics(self, x: Tensor, y: Tensor, stage: str) -> dict[str, Any]:
         raise NotImplementedError
 
     def loss(self,
              batch,
              stage: str,
              confusion: bool = False):
         x, y = self.arrange(batch)
-        metrics = self.metrics(x, y, stage)
-        loss = self.loss_func(x, y)
-        metrics[f'loss_{self.name}/{stage}'] = loss
-        for cm in self.confusion.values():
-            cm.update(x, y)
+        w = self.weight * (-1 * self.temp).exp()
+        loss = w * self.loss_func(x, y) + self.temp
+        metrics = {}
+        if stage:
+            metrics = self.metrics(x, y, stage)
+            metrics[f'loss_{self.name}/{stage}'] = loss
+            if stage == 'train':
+                metrics[f'temperature/{self.name}'] = self.temp
+            if confusion:
+                for cm in self.confusion.values():
+                    cm.update(x, y)
         return loss, metrics
 
+    def finalize(self, batch) -> None:
+        return
+
     def draw_confusion_matrix(self, cm: tm.ConfusionMatrix) -> plt.Figure:
         '''Produce confusion matrix at end of epoch'''
         confusion = cm.compute().cpu()
         fig = plt.figure(figsize=[8,6])
         sn.heatmap(confusion,
                    xticklabels=self.classes,
                    yticklabels=self.classes,
@@ -78,15 +92,19 @@
     Convolve down to a single node score per semantic class for each 2D graph,
     node, and remove intermediate node stores from data object.
     """
     def __init__(self,
                  node_features: int,
                  planes: list[str],
                  semantic_classes: list[str]):
-        super().__init__('semantic', planes, semantic_classes, RecallLoss())
+        super().__init__('semantic',
+                         planes,
+                         semantic_classes,
+                         RecallLoss(),
+                         weight=2.)
 
         # torchmetrics arguments
         metric_args = {
             'task': 'multiclass',
             'num_classes': len(semantic_classes),
             'ignore_index': -1
         }
@@ -96,65 +114,73 @@
         self.confusion['recall_semantic_matrix'] = tm.ConfusionMatrix(
             normalize='true', **metric_args)
         self.confusion['precision_semantic_matrix'] = tm.ConfusionMatrix(
             normalize='pred', **metric_args)
 
         self.net = nn.ModuleDict()
         for p in planes:
-            self.net[p] = ClassLinear(node_features, 1, len(semantic_classes))
+            self.net[p] = nn.Linear(node_features, len(semantic_classes))
 
     def forward(self, x: dict[str, Tensor],
                 batch: dict[str, Tensor]) -> dict[str, dict[str, Tensor]]:
-        return { 'x_semantic': { p: self.net[p](x[p]).squeeze(dim=-1) for p in self.planes } }
+        return { 'x_semantic': { p: self.net[p](x[p]) for p in self.planes } }
 
     def arrange(self, batch) -> tuple[Tensor, Tensor]:
         x = cat([batch[p].x_semantic for p in self.planes], dim=0)
         y = cat([batch[p].y_semantic for p in self.planes], dim=0)
         return x, y
 
     def metrics(self, x: Tensor, y: Tensor, stage: str) -> dict[str, Any]:
         return {
             f'recall_semantic/{stage}': self.recall(x, y),
             f'precision_semantic/{stage}': self.precision(x, y)
         }
 
+    def finalize(self, batch) -> None:
+        for p in self.planes:
+            batch[p].x_semantic = batch[p].x_semantic.softmax(dim=1)
+
 class FilterDecoder(DecoderBase):
     """NuGraph filter decoder module.
 
     Convolve down to a single node score, to identify and filter out
     graph nodes that are not part of the primary physics interaction
     """
     def __init__(self,
                  node_features: int,
                  planes: list[str],
-                 semantic_classes: list[str]):
-        super().__init__('filter', planes, ('noise', 'signal'), nn.BCELoss())
+                ):
+        super().__init__('filter',
+                         planes,
+                         ('noise', 'signal'),
+                         nn.BCELoss(),
+                         weight=2.)
 
         # torchmetrics arguments
         metric_args = {
             'task': 'binary'
         }
 
         self.recall = tm.Recall(**metric_args)
         self.precision = tm.Precision(**metric_args)
         self.confusion['recall_filter_matrix'] = tm.ConfusionMatrix(
             normalize='true', **metric_args)
         self.confusion['precision_filter_matrix'] = tm.ConfusionMatrix(
             normalize='pred', **metric_args)
 
-        num_features = len(semantic_classes) * node_features
         self.net = nn.ModuleDict()
         for p in planes:
             self.net[p] = nn.Sequential(
-                nn.Linear(num_features, 1),
-                nn.Sigmoid())
+                nn.Linear(node_features, 1),
+                nn.Sigmoid(),
+            )
 
     def forward(self, x: dict[str, Tensor],
                 batch: dict[str, Tensor]) -> dict[str, dict[str, Tensor]]:
-        return { 'x_filter': { p: self.net[p](x[p].flatten(start_dim=1)).squeeze(dim=-1) for p in self.planes }}
+        return { 'x_filter': { p: self.net[p](x[p]).squeeze(dim=-1) for p in self.planes }}
 
     def arrange(self, batch) -> tuple[Tensor, Tensor]:
         x = cat([batch[p].x_filter for p in self.planes], dim=0)
         y = cat([(batch[p].y_semantic!=-1).float() for p in self.planes], dim=0)
         return x, y
 
     def metrics(self, x: Tensor, y: Tensor, stage: str) -> dict[str, Any]:
@@ -168,20 +194,20 @@
 
     Convolve graph node features down to a single classification score
     for the entire event
     '''
     def __init__(self,
                  node_features: int,
                  planes: list[str],
-                 semantic_classes: list[str],
                  event_classes: list[str]):
         super().__init__('event',
                          planes,
                          event_classes,
-                         RecallLoss())
+                         RecallLoss(),
+                         weight=2.)
 
         # torchmetrics arguments
         metric_args = {
             'task': 'multiclass',
             'num_classes': len(event_classes)
         }
 
@@ -192,56 +218,119 @@
         self.confusion['precision_event_matrix'] = tm.ConfusionMatrix(
             normalize='pred', **metric_args)
 
         self.pool = nn.ModuleDict()
         for p in planes:
             self.pool[p] = SoftmaxAggregation(learn=True)
         self.net = nn.Sequential(
-            nn.Linear(in_features=len(planes) * len(semantic_classes) * node_features,
+            nn.Linear(in_features=len(planes) * node_features,
                       out_features=len(event_classes)))
 
     def forward(self, x: dict[str, Tensor],
                 batch: dict[str, Tensor]) -> dict[str, dict[str, Tensor]]:
-        x = [ pool(x[p].flatten(1), batch[p]) for p, pool in self.pool.items() ]
+        x = [ pool(x[p], batch[p]) for p, pool in self.pool.items() ]
         return { 'x': { 'evt': self.net(cat(x, dim=1)) }}
 
     def arrange(self, batch) -> tuple[Tensor, Tensor]:
         return batch['evt'].x, batch['evt'].y
 
     def metrics(self, x: Tensor, y: Tensor, stage: str) -> dict[str, Any]:
         return {
             f'recall_event/{stage}': self.recall(x, y),
             f'precision_event/{stage}': self.precision(x, y)
         }
 
+    def finalize(self, batch) -> None:
+        batch['evt'].x = batch['evt'].x.softmax(dim=1)
+
 class VertexDecoder(DecoderBase):
     """
     """
     def __init__(self,
                  node_features: int,
+                 aggr: str,
+                 lstm_features: int,
+                 mlp_features: list[int],
                  planes: list[str],
                  semantic_classes: list[str]):
         super().__init__('vertex',
                          planes,
                          semantic_classes,
-                         LogCoshLoss())
-        in_features = len(semantic_classes) * node_features
-        self.net = LSTMAggregation(in_channels=in_features,
-                                   out_channels=node_features)
+                         LogCoshLoss(),
+                         weight=1.,
+                         temperature=5.)
+
+        # initialise aggregation function
+        self.aggr = nn.ModuleDict()
+        aggr_kwargs = {}
+        in_features = node_features
+        if aggr == 'lstm':
+            aggr_kwargs = {
+                'in_channels': node_features,
+                'out_channels': lstm_features,
+            }
+            in_features = lstm_features
+        for p in self.planes:
+            self.aggr[p] = aggr_resolver(aggr, **(aggr_kwargs or {}))
+
+        # initialise MLP
+        net = []
+        feats = [ len(self.planes) * in_features ] + mlp_features + [ 3 ]
+        for f_in, f_out in zip(feats[:-1], feats[1:]):
+            net.append(nn.Linear(in_features=f_in, out_features=f_out))
+            net.append(nn.ReLU())
+        del net[-1] # remove last activation function
+        self.net = nn.Sequential(*net)
 
     def forward(self, x: dict[str, Tensor], batch: dict[str, Tensor]) -> dict[str,dict[str, Tensor]]:
-        merged_tensors = [x[p] for p in self.planes]
-        merged_tensor = cat(merged_tensors, dim = 0)
-        print(merged_tensor.shape)
-        flattened_tensor = merged_tensor.flatten(1)
-        res = self.net(flattened_tensor)
-        return { 'x_vtx': { 'evt': self.net(flattened_tensor) }}
+        x = [ net(x[p], index=batch[p]) for p, net in self.aggr.items() ]
+        x = cat(x, dim=1)
+        return { 'x_vtx': { 'evt': self.net(x) }}
 
     def arrange(self, batch) -> tuple[Tensor, Tensor]:
-        'dunno if x_vertex is correct name'
-        'also assuming one of them is our prediction and one is truth'
         x = batch['evt'].x_vtx
         y = batch['evt'].y_vtx
         return x, y
 
     def metrics(self, x: Tensor, y: Tensor, stage: str) -> dict[str, Any]:
-        return {}
+        xyz = (x-y).abs().mean(dim=0)
+        return {
+            f'vertex-resolution-x/{stage}': xyz[0],
+            f'vertex-resolution-y/{stage}': xyz[1],
+            f'vertex-resolution-z/{stage}': xyz[2],
+            f'vertex-resolution/{stage}': xyz.square().sum().sqrt()
+        }
+
+class InstanceDecoder(DecoderBase):
+    def __init__(self,
+                 node_features: int,
+                 planes: list[str],
+                 classes: list[str]):
+        super().__init__('Instance',
+                         planes,
+                         event_classes,
+                         ObjCondensationLoss(),
+                         'multiclass',
+                         confusion=False)
+
+        num_features = len(classes) * node_features
+
+        self.net = nn.ModuleDict()
+        for p in planes:
+            self.net[p] = nn.Sequential(
+                nn.Linear(num_features, 1),
+                nn.Sigmoid())
+
+    def forward(self, x: dict[str, Tensor], batch: dict[str, Tensor]) -> dict[str, dict[str, Tensor]]:
+        return {'x_instance': {p: self.net[p](x[p].flatten(start_dim=1)).squeeze(dim=-1) for p in self.net.keys()}}
+
+    def arrange(self, batch: dict[str, Tensor]) -> tuple[Tensor, Tensor]:
+        x = torch.cat([batch[p]['x_instance'] for p in self.planes], dim=0)
+        y = torch.cat([batch[p]['y_instance'] for p in self.planes], dim=0)
+        return x, y
+
+    def metrics(self, x: Tensor, y: Tensor, stage: str) -> dict[str, Any]:
+        metrics = {}
+        predictions = self.predict(x)
+        acc = self.acc_func(predictions, y)
+        metrics[f'{self.name}_accuracy/{stage}'] = accuracy
+        return metrics
```

### Comparing `nugraph-24.2.0/nugraph/models/encoder.py` & `nugraph-24.4.0/nugraph/models/nugraph3/encoder.py`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/nugraph/models/nexus.py` & `nugraph-24.4.0/nugraph/models/nugraph3/nexus.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             nn.Linear(feats, planar_features),
             nn.Tanh(),
             nn.Linear(planar_features, planar_features),
             nn.Tanh(),
         )
 
     def forward(self, x: Tensor, edge_index: Tensor, n: Tensor) -> Tensor:
-        return self.propagate(x=x, n=n, edge_index=edge_index)
+        return self.propagate(edge_index=edge_index, x=x, n=n)
 
     def message(self, x_i: Tensor, n_j: Tensor) -> Tensor:
         return self.edge_net(cat((x_i, n_j), dim=-1).detach()) * n_j
 
     def update(self, aggr_out: Tensor, x: Tensor) -> Tensor:
         return self.node_net(cat((x, aggr_out), dim=-1))
```

### Comparing `nugraph-24.2.0/nugraph/models/plane.py` & `nugraph-24.4.0/nugraph/models/nugraph3/plane.py`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/FeatureNorm-checkpoint.py` & `nugraph-24.4.0/nugraph/util/FeatureNorm.py`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/nugraph/util/.ipynb_checkpoints/RecallLoss-checkpoint.py` & `nugraph-24.4.0/nugraph/util/RecallLoss.py`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/nugraph/util/ObjCondensationLoss.py` & `nugraph-24.4.0/nugraph/util/ObjCondensationLoss.py`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/nugraph/util/scriptutils.py` & `nugraph-24.4.0/nugraph/util/scriptutils.py`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/pyproject.toml` & `nugraph-24.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nugraph-24.2.0/PKG-INFO` & `nugraph-24.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nugraph
-Version: 24.2.0
+Version: 24.4.0
 Summary: NuGraph2: A Graph Neural Network for neutrino physics event reconstruction
 Author-email: v hewes <vhewes@fnal.gov>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: matplotlib
```

