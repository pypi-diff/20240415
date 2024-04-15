# Comparing `tmp/phasegen-0.0.6b0.tar.gz` & `tmp/phasegen-0.0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasegen-0.0.6b0.tar", max compression
+gzip compressed data, was "phasegen-0.0.7b0.tar", max compression
```

## Comparing `phasegen-0.0.6b0.tar` & `phasegen-0.0.7b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      725 2024-04-11 08:07:49.318896 phasegen-0.0.6b0/README.md
--rw-r--r--   0        0        0     4599 2024-04-11 08:07:49.330896 phasegen-0.0.6b0/phasegen/__init__.py
--rw-r--r--   0        0        0    15044 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/coalescent_models.py
--rw-r--r--   0        0        0    14462 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/comparison.py
--rw-r--r--   0        0        0    36975 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/demography.py
--rw-r--r--   0        0        0    80702 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/distributions.py
--rw-r--r--   0        0        0     1722 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/expm.py
--rw-r--r--   0        0        0    27043 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/inference.py
--rw-r--r--   0        0        0     2378 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/lineage.py
--rw-r--r--   0        0        0     2751 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/locus.py
--rw-r--r--   0        0        0     2653 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/norms.py
--rw-r--r--   0        0        0    16757 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/rewards.py
--rw-r--r--   0        0        0     1121 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/serialization.py
--rw-r--r--   0        0        0    11106 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/spectrum.py
--rw-r--r--   0        0        0    29433 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/state_space.py
--rw-r--r--   0        0        0    53110 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/state_space_old.py
--rw-r--r--   0        0        0     1230 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/utils.py
--rw-r--r--   0        0        0     4478 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/visualization.py
--rw-r--r--   0        0        0      931 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/pyproject.toml
--rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.6b0/PKG-INFO
+-rw-r--r--   0        0        0      725 2024-04-15 08:39:53.445649 phasegen-0.0.7b0/README.md
+-rw-r--r--   0        0        0     4814 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/__init__.py
+-rw-r--r--   0        0        0    15044 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/coalescent_models.py
+-rw-r--r--   0        0        0    14488 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/comparison.py
+-rw-r--r--   0        0        0    37050 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/demography.py
+-rw-r--r--   0        0        0    85927 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/distributions.py
+-rw-r--r--   0        0        0     3278 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/expm.py
+-rw-r--r--   0        0        0    27043 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/inference.py
+-rw-r--r--   0        0        0     2378 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/lineage.py
+-rw-r--r--   0        0        0     2751 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/locus.py
+-rw-r--r--   0        0        0     2653 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/norms.py
+-rw-r--r--   0        0        0    18837 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/rewards.py
+-rw-r--r--   0        0        0     1121 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/serialization.py
+-rw-r--r--   0        0        0    11106 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/spectrum.py
+-rw-r--r--   0        0        0    29578 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/state_space.py
+-rw-r--r--   0        0        0    53044 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/state_space_old.py
+-rw-r--r--   0        0        0     1229 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/utils.py
+-rw-r--r--   0        0        0     4478 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/phasegen/visualization.py
+-rw-r--r--   0        0        0      931 2024-04-15 08:39:53.461649 phasegen-0.0.7b0/pyproject.toml
+-rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.7b0/PKG-INFO
```

### Comparing `phasegen-0.0.6b0/README.md` & `phasegen-0.0.7b0/README.md`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/__init__.py` & `phasegen-0.0.7b0/phasegen/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PhaseGen package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-04-09"
 
-__version__ = '0.0.6-beta'
+__version__ = '0.0.7-beta'
 
 import logging
 import os
 import sys
 
 import jsonpickle.ext.numpy as jsonpickle_numpy
 from tqdm import tqdm
@@ -140,14 +140,15 @@
 from .rewards import (
     Reward,
     TreeHeightReward,
     TotalTreeHeightReward,
     TotalBranchLengthReward,
     UnfoldedSFSReward,
     FoldedSFSReward,
+    LineageReward,
     CustomReward,
     ProductReward,
     SumReward,
     CombinedReward,
     DemeReward
 )
 
@@ -169,15 +170,21 @@
     L2Norm,
     LInfNorm,
     PoissonLikelihood
 )
 
 from .state_space_old import StateSpace as OldStateSpace
 
-from .expm import Backend, SciPyExpm, TensorFlowExpm
+from .expm import (
+    ExpmBackend,
+    Backend,
+    SciPyExpmBackend,
+    TensorFlowExpmBackend,
+    JaxExpmBackend
+)
 
 __all__ = [
     'PhaseTypeDistribution',
     'Coalescent',
     'Demography',
     'Epoch',
     'PopSizeChanges',
@@ -205,19 +212,25 @@
     'PoissonLikelihood',
     'Reward',
     'TreeHeightReward',
     'TotalTreeHeightReward',
     'TotalBranchLengthReward',
     'UnfoldedSFSReward',
     'FoldedSFSReward',
+    'LineageReward',
     'CustomReward',
     'ProductReward',
     'SumReward',
     'DemeReward',
     'CombinedReward',
     'StateSpace',
     'DefaultStateSpace',
     'BlockCountingStateSpace',
     'CoalescentModel',
     'LineageConfig',
     'LocusConfig',
+    'Backend',
+    'ExpmBackend',
+    'SciPyExpmBackend',
+    'TensorFlowExpmBackend',
+    'JaxExpmBackend'
 ]
```

### Comparing `phasegen-0.0.6b0/phasegen/coalescent_models.py` & `phasegen-0.0.7b0/phasegen/coalescent_models.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/comparison.py` & `phasegen-0.0.7b0/phasegen/comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         :param do_assertion: Whether to assert that the distributions are the same.
         """
         title = f"{title}: {stat}"
 
         with mpl.rc_context({'axes.titlesize': 7}):
 
             if stat in ['m3', 'm4']:
-                ph_stat = ph.moment(int(stat[1]))
+                ph_stat = ph.moment(int(stat[1]), center=False)
                 ms_stat = getattr(ms, stat)
 
             else:
                 ph_stat = getattr(ph, stat)
                 ms_stat = getattr(ms, stat)
 
             if isinstance(ph_stat, float):
@@ -296,15 +296,15 @@
             else:
                 raise ValueError(f"Unknown type {type(ph_stat)}.")
 
         if not diff <= tol:
             self.logger.critical(f"{title}: {diff} > {tol}")
 
             if do_assertion:
-                raise AssertionError(f"Maximum relative difference {diff} exceeds threshold {tol}.")
+                raise AssertionError(f"Maximum relative difference {diff} exceeds threshold {tol} for {title}.")
         else:
             self.logger.info(f"{title}: {diff} <= {tol}")
 
         if do_assertion:
             self.n_assertions += 1
 
         plt.clf()
```

### Comparing `phasegen-0.0.6b0/phasegen/demography.py` & `phasegen-0.0.7b0/phasegen/demography.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,24 +216,21 @@
             prev = epoch
 
             if epoch.end_time == np.inf:
                 break
 
             i += 1
 
-    def get_epochs(self, t: float | Iterable[float]) -> Union['Epoch', Sequence['Epoch']]:
+    def get_epochs(self, t: Iterable[float]) -> Sequence['Epoch']:
         """
         Get the epoch at the given times.
 
-        :param t: Time or times.
-        :return: Epoch or array of epochs.
+        :param t: Times.
+        :return: Array of epochs.
         """
-        if not isinstance(t, Iterable):
-            return self.get_epochs([t])[0]
-
         t = list(t)
 
         # sort times in ascending order
         t_sorted: Sequence[float] = np.sort(t)
 
         # get epoch iterator
         iterator: Iterator[Epoch] = self.epochs
@@ -251,14 +248,23 @@
 
             # add epoch to array
             epochs[i] = epoch
 
         # sort back to original order
         return np.array(epochs[np.argsort(t)])
 
+    def get_epoch(self, t: float) -> 'Epoch':
+        """
+        Get the epoch at the given time.
+
+        :param t: Time.
+        :return: Epoch.
+        """
+        return self.get_epochs([t])[0]
+
     def add_events(self, events: List['DemographicEvent']):
         """
         Add demographic events.
 
         :param events: List of demographic events.
         """
         self.events += events
```

### Comparing `phasegen-0.0.6b0/phasegen/distributions.py` & `phasegen-0.0.7b0/phasegen/distributions.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 Probability distributions.
 """
 
 import copy
 import itertools
 import logging
 from abc import ABC, abstractmethod
+from collections import Counter
 from collections.abc import Mapping
 from functools import cached_property, cache
+from math import comb
 from math import factorial
 from typing import Generator, List, Callable, Tuple, Dict, Collection, Iterable, Iterator
 
 import numpy as np
 from scipy.ndimage import gaussian_filter1d
 
 from .coalescent_models import StandardCoalescent, CoalescentModel, BetaCoalescent, DiracCoalescent
@@ -193,20 +195,22 @@
         :param locus1: The first locus.
         :param locus2: The second locus.
         :return: The covariance.
         """
         if locus1 not in range(self.dist.locus_config.n) or locus2 not in range(self.dist.locus_config.n):
             raise ValueError(f"Locus {locus1} or {locus2} does not exist.")
 
-        xy = self.dist.moment(k=2, rewards=(
-            CombinedReward([self.dist.reward, LocusReward(locus1)]),
-            CombinedReward([self.dist.reward, LocusReward(locus2)])
-        ))
-
-        return xy - self.loci[locus1].mean * self.loci[locus2].mean
+        return self.dist.moment(
+            k=2,
+            rewards=(
+                CombinedReward([self.dist.reward, LocusReward(locus1)]),
+                CombinedReward([self.dist.reward, LocusReward(locus2)])
+            ),
+            center=True
+        )
 
     @cached_property
     def cov(self) -> np.ndarray:
         """
         Covariance matrix across loci.
         """
         n_loci = self.dist.locus_config.n
@@ -299,20 +303,22 @@
         :param pop1: The first deme.
         :param pop2: The second deme.
         :return: The covariance.
         """
         if pop1 not in self.dist.lineage_config.pop_names or pop2 not in self.dist.lineage_config.pop_names:
             raise ValueError(f"Population {pop1} or {pop2} does not exist.")
 
-        xy = self.dist.moment(k=2, rewards=(
-            CombinedReward([self.dist.reward, DemeReward(pop1)]),
-            CombinedReward([self.dist.reward, DemeReward(pop2)])
-        ))
-
-        return xy - self.demes[pop1].mean * self.demes[pop2].mean
+        return self.dist.moment(
+            k=2,
+            rewards=(
+                CombinedReward([self.dist.reward, DemeReward(pop1)]),
+                CombinedReward([self.dist.reward, DemeReward(pop2)])
+            ),
+            center=True
+        )
 
     @cached_property
     def cov(self) -> np.ndarray:
         """
         Covariance matrix across demes.
         """
         pops = self.dist.lineage_config.pop_names
@@ -523,29 +529,29 @@
         return self.moment(k=1)
 
     @cached_property
     def var(self) -> float | SFS:
         """
         Second central moment / variance.
         """
-        return self.moment(k=2) - self.moment(k=1) ** 2
+        return self.moment(k=2, center=True)
 
     @cached_property
     def std(self) -> float | SFS:
         """
         Standard deviation.
         """
         return self.var ** 0.5
 
     @cached_property
     def m2(self) -> float | SFS:
         """
         Second (non-central) moment.
         """
-        return self.moment(k=2)
+        return self.moment(k=2, center=False)
 
     @cached_property
     def demes(self) -> MarginalDemeDistributions:
         """
         Marginal distributions over each deme.
         """
         return MarginalDemeDistributions(self)
@@ -553,27 +559,102 @@
     @cached_property
     def loci(self) -> MarginalLocusDistributions:
         """
         Marginal distributions over each locus.
         """
         return MarginalLocusDistributions(self)
 
-    @cache
     def moment(
             self,
             k: int,
             rewards: Tuple[Reward, ...] = None,
             start_time: float = None,
+            end_time: float = None,
+            center: bool = True,
+            permute: bool = True
+    ) -> float:
+        """
+        Get the kth (non-central) (cross-)moment.
+
+        :param k: The order of the moment.
+        :param rewards: Iterable of k rewards. By default, the reward of the underlying distribution.
+        :param start_time: Time when to start accumulation of moments. By default, the start time specified when
+            initializing the distribution.
+        :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
+            initializing the distribution or the time until almost sure absorption.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
+        :return: The kth moment
+        """
+        if rewards is None:
+            rewards = [self.reward] * k
+
+        if k != len(rewards):
+            raise ValueError(f"Number of specified rewards for moment of order {k} must be {k}.")
+
+        if k == 0:
+            return 1
+
+        # center moments around the mean
+        if center and k > 1:
+
+            # center moment
+            if len(set(rewards)) == 1:
+
+                reward = list(rewards)[0]
+                components = []
+
+                for i in range(k + 1):
+                    mu_i = PhaseTypeDistribution.moment(self, i, (reward,) * i, start_time, end_time, False)
+                    mu1_k_i = PhaseTypeDistribution.moment(self, 1, (reward,), start_time, end_time, False) ** (k - i)
+
+                    components += [comb(k, i) * (-1) ** (k - i) * mu_i * mu1_k_i]
+
+                return sum(components)
+
+            # center cross-moment
+            else:
+
+                cross_components = []
+
+                # count number of different rewards
+                for reward, count in Counter(rewards).items():
+                    cross_components += [
+                        PhaseTypeDistribution.moment(self, count, (reward,) * count, start_time, end_time, True)
+                    ]
+
+                uncentered = PhaseTypeDistribution.moment(self, k, rewards, start_time, end_time, False)
+
+                return uncentered - np.prod(cross_components)
+
+        if permute:
+            # get all possible permutations of rewards
+            permutations = list(itertools.permutations(rewards))
+
+            # compute average over all permutations
+            return sum(self._raw_moment(k, r, start_time, end_time) for r in permutations) / len(permutations)
+
+        return self._raw_moment(k, rewards, start_time, end_time)
+
+    @cache
+    def _raw_moment(
+            self,
+            k: int,
+            rewards: Tuple[Reward, ...] = None,
+            start_time: float = None,
             end_time: float = None
     ) -> float:
         """
-        Get the kth (non-central) moment.
+        Get the raw kth-order (non-central) moment. Note that for cross-moments, we need average over all possible
+        reward permutations.
 
         :param k: The order of the moment.
-        :param rewards: Tuple of k rewards
+        :param rewards: Tuple of k rewards. By default, the reward of the underlying distribution.
         :param start_time: Time when to start accumulation of moments. By default, the start time specified when
             initializing the distribution.
         :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
             initializing the distribution or the time until almost sure absorption.
         :return: The kth moment
         """
         if start_time is None:
@@ -619,15 +700,15 @@
         :param S: (Regularized) intensity matrix.
         :param epoch: Epoch number.
         """
         rates = S[S > 0]
 
         if rates.min() / rates.max() < 1e-10:
             self._logger.warning(
-                f"Intensity matrix in epoch {epoch} contains rates that differ by more than 6 orders of magnitude: "
+                f"Intensity matrix in epoch {epoch} contains rates that differ by more than 10 orders of magnitude: "
                 f"min: {rates.min()}, max: {rates.max()}. "
                 f"This may potentially lead to numerical instability, despite matrix regularization."
             )
 
     def accumulate(
             self,
             k: int,
@@ -792,15 +873,15 @@
     Phase-type distribution for a piecewise time-homogeneous process that allows the computation of the
     density function. This is currently only possible with default rewards.
     """
     #: Maximum number of epochs to consider when determining time to almost sure absorption.
     max_epochs: int = 10000
 
     #: Maximum number of time we double the end time when determining time to almost sure absorption.
-    max_iter: int = 10
+    max_iter: int = 20
 
     #: Probability of almost sure absorption.
     p_absorption: float = 1 - 1e-15
 
     def __init__(
             self,
             state_space: DefaultStateSpace,
@@ -910,55 +991,115 @@
         if np.isnan(probs).any():
             self._logger.critical(
                 "NaN values in CDF. This is likely due to an ill-conditioned rate matrix."
             )
 
         return probs
 
+    def _update(
+            self,
+            u: float,
+            u_prev: float,
+            T: np.ndarray,
+            epoch: 'Epoch'
+    ) -> Tuple[float, np.ndarray, 'Epoch']:
+        """
+        Update transition matrix and time.
+
+        :param u: Time to update to.
+        :param u_prev: Previous time.
+        :param T: Transition matrix.
+        :param epoch: Current epoch.
+        :return: Updated time, transition matrix, and epoch.
+        """
+        self.state_space.update_epoch(epoch)
+
+        while u > epoch.end_time:
+
+            # update transition matrix with remaining time in current epoch
+            tau = epoch.end_time - u_prev
+            T = T @ expm(self.state_space.S * tau)
+            u_prev = epoch.end_time
+
+            # fetch and update for next epoch
+            epoch = self.demography.get_epoch(epoch.end_time)
+            self.state_space.update_epoch(epoch)
+        else:
+            # update transition matrix
+            T = T @ expm(self.state_space.S * (u - u_prev))
+
+        return u, T, epoch
+
+    @cached_property
+    def _e(self) -> np.ndarray:
+        """
+        Exit vector.
+        """
+        return self.reward._get(self.state_space)
+
+    def _cum(self, T: np.ndarray) -> float:
+        """
+        Get cumulative probability for given transition matrix.
+
+        :param T: Transition matrix.
+        :return: Cumulative probability.
+        """
+        return float(1 - self.state_space.alpha @ T @ self._e)
+
     @cache
     def quantile(
             self,
             q: float,
             expansion_factor: float = 2,
-            tol: float = 1e-5,
+            precision: float = 1e-5,
             max_iter: int = 1000
     ):
         """
         Find the specified quantile of a CDF using an adaptive bisection method.
 
-        TODO this can be optimized
-
         :param q: The desired quantile (between 0 and 1).
-        :param expansion_factor: Factor by which to expand the upper bound that does not yet contain the quantile.
-        :param tol: The tolerance for convergence.
-        :param max_iter: Maximum number of iterations for the bisection method.
-        :return: The approximate x value for the nth quantile.
+        :param expansion_factor: Factor by which to multiply the upper bound that does not yet contain the quantile.
+        :param precision: Precision for quantile, i.e. ``F(b) - F(a) < precision``.
+        :param max_iter: Maximum number of iterations.
+        :return: The quantile.
         """
         if q < 0 or q > 1:
             raise ValueError("Specified quantile must be between 0 and 1.")
 
+        if expansion_factor <= 1:
+            raise ValueError("Expansion factor must be greater than 1.")
+
         # initialize bounds
         a, b = 0, 1
 
-        # expand upper bound until it contains the quantile
-        while self.cdf(b) < q and max_iter > 0:
-            b *= expansion_factor
-            max_iter -= 1
+        T_a = np.eye(self.state_space.k)
+        epoch_a, epoch_b = self.demography.get_epoch(0), self.demography.get_epoch(0)
+        b, T_b, epoch_b = self._update(b, a, T_a, epoch_b)
+
+        i = 0
+
+        # expand lower bound until it contains the quantile
+        while self._cum(T_b) < q and i < max_iter:
+            b, T_b, epoch_b = self._update(b * expansion_factor, b, T_b, epoch_b)
+
+            i += 1
 
         # use bisection method within the determined bounds
-        while (b - a) > tol and max_iter > 0:
-            m = (a + b) / 2
-            if self.cdf(m) < q:
-                a = m
+        while self._cum(T_b) - self._cum(T_a) > precision and i < max_iter:
+            m, T_m, epoch_m = self._update((a + b) / 2, a, T_a, epoch_a)
+
+            if self._cum(T_m) < q:
+                a, T_a, epoch_a = m, T_m, epoch_m
             else:
-                b = m
-            max_iter -= 1
+                b, T_b, epoch_b = m, T_m, epoch_m
+
+            i += 1
 
         # warn if maximum number of iterations reached
-        if max_iter == 0:
+        if i - 1 == max_iter:
             raise RuntimeError("Maximum number of iterations reached when determining quantile.")
 
         return (a + b) / 2
 
     def pdf(self, t: float | np.ndarray, dx: float = 1e-10) -> float | np.ndarray:
         """
         Density function. We use numerical differentiation of the CDF to calculate the density. This provides good
@@ -997,120 +1138,47 @@
     def _get_absorption_time(self) -> float:
         """
         Get a time estimate for when we have reached absorption almost surely.
         We base this computation on the transition matrix rather than the moments, because here
         we have a good idea about how likely absorption, and can warn the user if necessary.
         Stopping the simulation when no more rewards are accumulated is not a good idea, as this
         can happen before almost sure absorption (exponential runaway growth, temporary isolation in different demes).
-
-        TODO clean up further?
         """
-        # initialize transition matrix
-        T_curr = np.eye(self.state_space.k)
-
-        # take reward vector as exit vector
-        e = self.reward._get(self.state_space)
-
-        # time and probability of absorption
-        t, p = 0, 0
-
-        epoch = None
-
-        # iterate over epochs and stop when almost sure absorption is reached
-        for i, epoch in enumerate(self.demography.epochs):
-            # update state space
-            self.state_space.update_epoch(epoch)
-
-            if i > self.max_epochs:
-                self._logger.warning(
-                    f"Reached maximum number of epochs ({self.max_epochs}) when determining "
-                    "time of almost sure absorption. This may be due to an ill-defined demography. "
-                    "You can also increase the maximum number of epochs (TreeHeightDistribution.max_epochs) or "
-                    "set the end time manually (Coalescent.end_time)."
-                )
-                return t
-
-            # make sure we are not in last epoch
-            if epoch.tau < np.inf:
-                # update transition matrix
-                T_curr = expm(self.state_space.S * epoch.tau) @ T_curr
-
-                # calculate probability of absorption
-                p = 1 - self.state_space.alpha @ T_curr @ e
-
-                if np.isnan(p):
-                    return self._warn_p_is_nan(t)
-
-                t += epoch.tau
-
-                if p >= self.p_absorption:
-                    return t
-            else:
-                # handle last epoch separately
-                break
-
-        # in the last epoch choose step size to be log-average population size
-        tau = 10 ** np.mean(np.log10(np.array(list(epoch.pop_sizes.values()))))
-        T_tau = expm(self.state_space.S * tau)
-
-        # in the last epoch, we increase tau exponentially
-        for i in range(self.max_iter):
-            # update transition matrix
-            T_curr = T_tau @ T_curr
-
-            # calculate probability of absorption
-            p_next = 1 - self.state_space.alpha @ T_curr @ e
-
-            if np.isnan(p_next):
-                return self._warn_p_is_nan(t)
-
-            # break if p_next is not increasing anymore
-            if p_next < p:
-                self._logger.warning(
-                    "Could not reliably find time of almost sure absorption as it decreased for increasing time. "
-                    f"Using time {t:.1f} with probability of absorption 1 - {1 - p:.1e}. "
-                    "This could be due to numerical imprecision, unreachable states or very large or small "
-                    "absorption times. You can also set the end time manually (see `Coalescent.end_time`)."
+        i = 0
+        T = np.eye(self.state_space.k)
+        epoch = self.demography.get_epoch(0)
+        t = 2 ** int(np.log2(np.mean(list(epoch.pop_sizes.values()))))
+        expansion_factor = 2
+
+        t, T, epoch = self._update(t, 0, T, epoch)
+        p = self._cum(T)
+
+        # multiple time by expansion_factor until we reach p_absorption
+        while p < self.p_absorption and i < self.max_iter:
+            t, T, epoch = self._update(t * expansion_factor, t, T, epoch)
+            p = self._cum(T)
+
+            if np.isnan(p):
+                self._logger.critical(
+                    "Could not reliably find time of almost sure absorption "
+                    "as probability of absorption is NaN. "
+                    "This is likely due to an ill-conditioned rate matrix. "
+                    f"Using time {t:.1f}. "
                 )
-                return t
-
-            # update time and probability
-            t += tau
-            p = p_next
-
-            # double tau, and update transition matrix accordingly
-            tau *= 2
-            T_tau @= T_tau
-
-            if p >= self.p_absorption:
-                return t
-
-        self._logger.warning(
-            "Could not reliably find time of almost sure absorption after maximum number of iterations. "
-            f"Using time {t:.1f} with probability of absorption 1 - {1 - p:.1e}. "
-            "This could be due to numerical imprecision, unreachable states or very large or small absorption times. "
-            "You can set the end time manually (see `Coalescent.end_time`) or increase the maximum "
-            "number of iterations (`TreeHeightDistribution.max_iter`)."
-        )
-
-        return t
 
-    def _warn_p_is_nan(self, t: float) -> float:
-        """
-        Warn if the probability of absorption is nan.
+            i += 1
 
-        :param t: The absorption time.
-        :return: The time.
-        """
-        self._logger.critical(
-            "Could not reliably find time of almost sure absorption "
-            "as probability of absorption is NaN. "
-            "This is likely due to an ill-conditioned rate matrix. "
-            f"Using time {t:.1f}. "
-        )
+        if i - 1 == self.max_iter:
+            self._logger.warning(
+                "Could not reliably find time of almost sure absorption after maximum number of iterations. "
+                f"Using time {t:.1f} with probability of absorption 1 - {1 - p:.1e}. "
+                "This could be due to numerical imprecision, unreachable states or very large or small "
+                "absorption times. You can set the end time manually (see `Coalescent.end_time`) or increase "
+                "the maximum number of iterations (`TreeHeightDistribution.max_iter`)."
+            )
 
         return t
 
 
 class SFSDistribution(PhaseTypeDistribution, ABC):
     """
     Base class for site-frequency spectrum distributions.
@@ -1173,66 +1241,81 @@
 
     @cache
     def moment(
             self,
             k: int,
             rewards: Tuple[SFSReward, ...] = None,
             start_time: float = None,
-            end_time: float = None
+            end_time: float = None,
+            center: bool = True,
+            permute: bool = True
     ) -> SFS:
         """
         Get the kth moments of the site-frequency spectrum.
 
         :param k: The order of the moment
         :param rewards: Tuple of k rewards
         :param start_time: Time when to start accumulation of moments. By default, the start time specified when
             initializing the distribution.
         :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
             initializing the distribution or the time until almost sure absorption.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :return: A site-frequency spectrum of kth order moments.
         """
         if rewards is None:
             rewards = (self.reward,) * k
 
         # optionally parallelize the moment computation of the SFS bins
         moments = parallelize(
             func=lambda x: self._moment(*x),
-            data=[[k, i, rewards, start_time, end_time] for i in self._get_indices()],
+            data=[[k, i, rewards, start_time, end_time, center, permute] for i in self._get_indices()],
             desc=f"Calculating {k}-moments",
             pbar=self.pbar,
             parallelize=self.parallelize
         )
 
         return SFS([0] + list(moments) + [0] * (self.lineage_config.n - len(moments)))
 
     def _moment(
             self,
             k: int,
             i: int,
             rewards: Tuple[SFSReward, ...] = None,
             start_time: float = None,
-            end_time: float = None
+            end_time: float = None,
+            center: bool = True,
+            permute: bool = True
     ) -> float:
         """
-        Get the kth moment for the ith site-frequency count.
+        Get the kth raw moment for the ith site-frequency count.
 
         :param k: The order of the moment
         :param i: The ith site-frequency count
         :param rewards: Tuple of k rewards
         :param start_time: Time when to start accumulation of moments. By default, the start time specified when
             initializing the distribution.
         :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
             initializing the distribution or the time until almost sure absorption.
+        :param center: Whether to center the moment around the mean.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :return: The kth SFS (cross)-moment at the ith site-frequency count
         """
-        return super().moment(
+        return PhaseTypeDistribution.moment(
+            self,
             k=k,
             rewards=tuple([CombinedReward([r, self._get_sfs_reward(i)]) for r in rewards]),
             start_time=start_time,
-            end_time=end_time
+            end_time=end_time,
+            center=center,
+            permute=permute
         )
 
     def accumulate(
             self,
             k: int,
             end_times: Iterable[float] | float,
             rewards: Tuple[Reward, ...] = None
@@ -1363,15 +1446,15 @@
         """
         # create list of arguments for each combination of i, j
         indices = [(i, j) for i in self._get_indices() for j in self._get_indices()]
 
         # get sfs using parallelized function
         sfs_results = parallelize(
             func=lambda x: (
-                PhaseTypeDistribution.moment(self, k=2, rewards=(
+                PhaseTypeDistribution.moment(self, k=2, permute=False, center=False, rewards=(
                     CombinedReward([self.reward, self._get_sfs_reward(x[0])]),
                     CombinedReward([self.reward, self._get_sfs_reward(x[1])])
                 ))
             ),
             data=indices,
             desc="Calculating covariance",
             pbar=self.pbar,
@@ -1398,24 +1481,22 @@
         :param i: The ith frequency count
         :param j: The jth frequency count
         :return: covariance
         """
         if i in (0, self.lineage_config.n) or j in (0, self.lineage_config.n):
             return 0
 
-        reward_i = CombinedReward([self.reward, self._get_sfs_reward(i)])
-        reward_j = CombinedReward([self.reward, self._get_sfs_reward(j)])
-
-        xy = super().moment(k=2, rewards=(reward_i, reward_j))
-        yx = super().moment(k=2, rewards=(reward_j, reward_i))
-
-        x = super().moment(k=1, rewards=(reward_i,))
-        y = super().moment(k=1, rewards=(reward_j,))
-
-        return (xy + yx) / 2 - x * y
+        return super().moment(
+            k=2,
+            rewards=(
+                CombinedReward([self.reward, self._get_sfs_reward(i)]),
+                CombinedReward([self.reward, self._get_sfs_reward(j)])
+            ),
+            center=True
+        )
 
     @cached_property
     def corr(self) -> SFS2:
         """
         Correlation matrix across site-frequency counts.
         """
         # get standard deviations
@@ -1892,24 +1973,24 @@
             time of almost sure absorption. Note that unnecessarily large end times can lead to numerical errors.
         """
         self._logger = logger.getChild(self.__class__.__name__)
 
         if model is None:
             model = StandardCoalescent()
 
-        if demography is None:
-            demography = Demography()
-
         if not isinstance(n, LineageConfig):
             #: Population configuration
             self.lineage_config: LineageConfig = LineageConfig(n)
         else:
             #: Population configuration
             self.lineage_config: LineageConfig = n
 
+        if demography is None:
+            demography = Demography(pop_sizes={p: 1 for p in self.lineage_config.pop_names})
+
         # set up locus configuration
         if isinstance(loci, int):
             #: Locus configuration
             self.locus_config: LocusConfig = LocusConfig(
                 n=loci,
                 recombination_rate=recombination_rate if recombination_rate is not None else 0
             )
@@ -2023,27 +2104,27 @@
         """
         The default state space.
         """
         return DefaultStateSpace(
             lineage_config=self.lineage_config,
             locus_config=self.locus_config,
             model=self.model,
-            epoch=self.demography.get_epochs(0)
+            epoch=self.demography.get_epoch(0)
         )
 
     @cached_property
     def block_counting_state_space(self) -> BlockCountingStateSpace:
         """
         The block counting state space.
         """
         return BlockCountingStateSpace(
             lineage_config=self.lineage_config,
             locus_config=self.locus_config,
             model=self.model,
-            epoch=self.demography.get_epochs(0)
+            epoch=self.demography.get_epoch(0)
         )
 
     @cached_property
     def tree_height(self) -> TreeHeightDistribution:
         """
         Tree height distribution.
         """
@@ -2084,46 +2165,92 @@
         """
         return FoldedSFSDistribution(
             state_space=self.block_counting_state_space,
             tree_height=self.tree_height,
             demography=self.demography
         )
 
-    @cache
+    def _get_dist(self, k: int, rewards: Iterable[Reward] = None) -> PhaseTypeDistribution:
+        """
+        Get the kth-order phase-type distribution with state space inferred from the rewards.
+        The returned phase-type distribution is configured with the unit reward.
+
+        :return: Distribution.
+        """
+        if rewards is None:
+            rewards = [TreeHeightReward()] * k
+
+        if Reward.support(DefaultStateSpace, rewards):
+            state_space = self.default_state_space
+        else:
+            state_space = self.block_counting_state_space
+
+        return PhaseTypeDistribution(
+            reward=UnitReward(),
+            tree_height=self.tree_height,
+            state_space=state_space,
+            demography=self.demography
+        )
+
     def moment(
             self,
             k: int = 1,
             rewards: Tuple[Reward, ...] = None,
             start_time: float = None,
-            end_time: float = None
+            end_time: float = None,
+            center: bool = True,
+            permute: bool = True
     ) -> float:
         """
         Get the kth (non-central) moment using the specified rewards and state space.
 
         :param k: The order of the moment
         :param rewards: Tuple of k rewards. By default, tree height rewards are used.
         :param start_time: Time when to start accumulation of moments. By default, the start time specified when
             initializing the distribution.
         :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
             initializing the distribution or the time until almost sure absorption.
+        :param center: Whether to center the moment.
+        :param permute: For cross-moments, whether to average over all permutations of rewards. Default is ``True``,
+            which will provide the correct cross-moment. If set to ``False``, the cross-moment will be conditioned on
+            the order of rewards.
         :return: The kth moment
         """
-        if Reward.support(DefaultStateSpace, rewards):
-            state_space = self.default_state_space
-        else:
-            state_space = self.block_counting_state_space
+        dist = self._get_dist(k, rewards)
 
-        dist = PhaseTypeDistribution(
-            reward=TreeHeightReward() if rewards is None else UnitReward(),
-            tree_height=self.tree_height,
-            state_space=state_space,
-            demography=self.demography
+        return dist.moment(
+            k=k,
+            rewards=rewards,
+            start_time=start_time,
+            end_time=end_time,
+            center=center,
+            permute=permute
         )
 
-        return dist.moment(k=k, rewards=rewards, start_time=start_time, end_time=end_time)
+    def _raw_moment(
+            self,
+            k: int,
+            rewards: Tuple[Reward, ...] = None,
+            start_time: float = None,
+            end_time: float = None
+    ) -> float:
+        """
+        Get the kth raw moment using the specified rewards and state space.
+
+        :param k: The order of the moment
+        :param rewards: Tuple of k rewards. By default, tree height rewards are used.
+        :param start_time: Time when to start accumulation of moments. By default, the start time specified when
+            initializing the distribution.
+        :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
+            initializing the distribution or the time until almost sure absorption.
+        :return: The kth raw moment
+        """
+        dist = self._get_dist(k, rewards)
+
+        return dist._raw_moment(k=k, rewards=rewards, start_time=start_time, end_time=end_time)
 
     def drop_cache(self):
         """
         Drop state space cache.
         """
         self.default_state_space.drop_cache()
         self.block_counting_state_space.drop_cache()
```

### Comparing `phasegen-0.0.6b0/phasegen/inference.py` & `phasegen-0.0.7b0/phasegen/inference.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/lineage.py` & `phasegen-0.0.7b0/phasegen/lineage.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/locus.py` & `phasegen-0.0.7b0/phasegen/locus.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/norms.py` & `phasegen-0.0.7b0/phasegen/norms.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/rewards.py` & `phasegen-0.0.7b0/phasegen/rewards.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,28 @@
         """
         pass
 
     def __hash__(self) -> int:
         """
         Get the hash for the reward.
         
-        :return: hash
+        :return: hash.
         """
         # hash the class name as this class is stateless.
         return hash(self.__class__.__name__)
 
+    def __eq__(self, other: 'Reward') -> bool:
+        """
+        Check if the rewards are equal.
+
+        :param other: other reward.
+        :return: True if the rewards are equal, False otherwise.
+        """
+        return self.__class__ == other.__class__ and hash(self) == hash(other)
+
     def prod(self, *rewards: 'Reward') -> 'ProductReward':
         """
         Product of this reward with other rewards.
 
         :param rewards: Rewards to take the product with.
         :return: Product of the rewards.
         """
@@ -247,14 +256,55 @@
             return state_space.states[:, :, :, blocks].sum(axis=(1, 2, 3))
 
         raise NotImplementedError(
             f'Unsupported state space type for reward {self.__class__.__name__}: {state_space.__class__.__name__}'
         )
 
 
+class LineageReward(LineageCountingReward):
+    """
+    Reward for a specific number of lineages present in across all demes and loci.
+    This reward can be used to, for example, track the individual coalescent times.
+    """
+
+    def __init__(self, n: int):
+        """
+        Initialize the reward.
+
+        :param n: The number of lineages to reward. Must be at least 2.
+        """
+        if n < 2:
+            raise ValueError('Number of lineages must be at least 2.')
+
+        self.n: int = n
+
+    def _get(self, state_space: StateSpace) -> np.ndarray:
+        """
+        Get the reward vector.
+
+        :param state_space: state space
+        :return: reward vector
+        :raises: NotImplementedError if the state space is not supported
+        """
+        if isinstance(state_space, (DefaultStateSpace, BlockCountingStateSpace)):
+            return (state_space.states.sum(axis=(1, 2, 3)) == self.n).astype(int)
+
+        raise NotImplementedError(
+            f'Unsupported state space type for reward {self.__class__.__name__}: {state_space.__class__.__name__}'
+        )
+
+    def __hash__(self) -> int:
+        """
+        Calculate the hash of the class name and the lineage index.
+
+        :return: hash
+        """
+        return hash(self.__class__.__name__ + str(self.n))
+
+
 class DemeReward(LineageCountingReward, BlockCountingReward):
     """
     Reward fraction of lineages in a specific deme. Taking the product of this reward with another reward
     will result in a reward that only considers the specified deme. Use :class:`SumReward` to marginalize over
     several demes.
     """
 
@@ -343,14 +393,30 @@
         """
         Get the reward vector.
 
         :param state_space: state space
         :return: reward vector
         """
         return np.ones(state_space.k)
+
+
+class BlockCountingUnitReward(BlockCountingReward):
+    """
+    Reward all states with 1 (including absorbing states), and only support block counting state spaces.
+    This reward can be used to force usage of the block counting state space.
+    """
+
+    def _get(self, state_space: BlockCountingStateSpace) -> np.ndarray:
+        """
+        Get the reward vector.
+
+        :param state_space: state space
+        :return: reward vector
+        """
+        return np.ones(state_space.k)
 
 
 class TotalBranchLengthLocusReward(LocusReward, LineageCountingReward):
     """
     Reward for total branch length per locus. This is needed as the taking the product of
     :class:`TotalBranchLengthReward` and :class:`LocusReward` will not work as expected (see
     :class:`CombinedReward`).
```

### Comparing `phasegen-0.0.6b0/phasegen/serialization.py` & `phasegen-0.0.7b0/phasegen/serialization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/spectrum.py` & `phasegen-0.0.7b0/phasegen/spectrum.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/phasegen/state_space.py` & `phasegen-0.0.7b0/phasegen/state_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,21 @@
         # cache rate matrix if specified
         if self.cache:
             self._cache[self.epoch] = (transitions, states)
 
         # indices of non-zero rates
         return np.array([s.lineages for s in states])
 
+    @property
+    def unlinked(self) -> np.ndarray:
+        """
+        Unlinked lineages.
+        """
+        return self.states - self.linked
+
     @cached_property
     def _states(self) -> List['State']:
         """
         Ordered list of states.
         """
         _ = self.states
         return self.__states
```

### Comparing `phasegen-0.0.6b0/phasegen/state_space_old.py` & `phasegen-0.0.7b0/phasegen/state_space_old.py`

 * *Files 1% similar despite different names*

```diff
@@ -736,16 +736,14 @@
 
         return k
 
 
 class Transition:
     """
     Class representing a transition between two states.
-
-    TODO reimplement by cycling through all possible transitions
     """
     #: Colors for different types of transitions
     _colors: Dict[str, str] = {
         'recombination': 'orange',
         'locus_coalescence': 'darkgreen',
         'linked_coalescence': 'darkgreen',
         'unlinked_coalescence': 'darkgreen',
```

### Comparing `phasegen-0.0.6b0/phasegen/utils.py` & `phasegen-0.0.7b0/phasegen/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     :param pbar: Whether to show a progress bar
     :param batch_size: Number of units to show in the pbar per function
     :param desc: Description for tqdm progress bar
     :param dtype: Data type of the results
     :param delay: Delay for tqdm progress bar
     :return: Array of results
     """
-
     if parallelize and len(data) > 1:
         # parallelize
         iterator = Pool().imap(func, data)
     else:
         # sequentialize
         iterator = map(func, data)
```

### Comparing `phasegen-0.0.6b0/phasegen/visualization.py` & `phasegen-0.0.7b0/phasegen/visualization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.6b0/pyproject.toml` & `phasegen-0.0.7b0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phasegen"
-version = "0.0.6-beta"
+version = "0.0.7-beta"
 description = "Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios."
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `phasegen-0.0.6b0/PKG-INFO` & `phasegen-0.0.7b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasegen
-Version: 0.0.6b0
+Version: 0.0.7b0
 Summary: Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios.
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

