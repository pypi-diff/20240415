# Comparing `tmp/pybts-1.7.0.tar.gz` & `tmp/pybts-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.7.0.tar", max compression
+gzip compressed data, was "pybts-1.7.1.tar", max compression
```

## Comparing `pybts-1.7.0.tar` & `pybts-1.7.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0   157658 2024-04-14 11:05:23.381420 pybts-1.7.0/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-14 11:05:23.381420 pybts-1.7.0/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-14 11:05:23.385420 pybts-1.7.0/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-14 11:05:23.385420 pybts-1.7.0/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-14 11:05:23.385420 pybts-1.7.0/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5960 2024-04-14 11:05:23.385420 pybts-1.7.0/README.md
--rw-r--r--   0        0        0      385 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/__init__.py
--rw-r--r--   0        0        0       52 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/board/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/board/board.py
--rw-r--r--   0        0        0    11048 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/board/server.py
--rw-r--r--   0        0        0     8197 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/builder.py
--rw-r--r--   0        0        0      596 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/__init__.py
--rw-r--r--   0        0        0     9344 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/composite.py
--rw-r--r--   0        0        0     2175 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5460 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/parallel.py
--rw-r--r--   0        0        0      945 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/ppa.py
--rw-r--r--   0        0        0     2235 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/selector.py
--rw-r--r--   0        0        0     2460 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/sequence.py
--rw-r--r--   0        0        0     1510 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/switcher.py
--rw-r--r--   0        0        0      182 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/composites/template.py
--rw-r--r--   0        0        0     3243 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/constants.py
--rw-r--r--   0        0        0     4943 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/converter.py
--rw-r--r--   0        0        0      121 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    22898 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1073 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/display.py
--rw-r--r--   0        0        0     1521 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/main.py
--rw-r--r--   0        0        0    17521 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/nodes.py
--rw-r--r--   0        0        0       63 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/__init__.py
--rw-r--r--   0        0        0     8856 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/base_class.py
--rw-r--r--   0        0        0      268 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/builder.py
--rw-r--r--   0        0        0      460 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/common.py
--rw-r--r--   0        0        0    15167 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/nodes.py
--rw-r--r--   0        0        0     5687 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/off_policy.py
--rw-r--r--   0        0        0     8586 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/on_policy.py
--rw-r--r--   0        0        0     1172 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/rl/tree.py
--rw-r--r--   0        0        0    16958 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-14 11:05:23.389420 pybts-1.7.0/pybts/templates/index.html
--rw-r--r--   0        0        0  1967920 2024-04-14 11:05:23.401420 pybts-1.7.0/pybts/templates/static/index-BlldS3Jx.js
--rw-r--r--   0        0        0   320362 2024-04-14 11:05:23.401420 pybts-1.7.0/pybts/templates/static/index-DN1S--qx.css
--rw-r--r--   0        0        0     5267 2024-04-14 11:05:23.401420 pybts-1.7.0/pybts/templates/static/info-lb9hZOuB.png
--rw-r--r--   0        0        0     2140 2024-04-14 11:05:23.401420 pybts-1.7.0/pybts/tree.py
--rw-r--r--   0        0        0    10045 2024-04-14 11:05:23.401420 pybts-1.7.0/pybts/utility.py
--rw-r--r--   0        0        0      844 2024-04-14 11:05:23.401420 pybts-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-15 10:19:50.544755 pybts-1.7.1/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-15 10:19:50.548755 pybts-1.7.1/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5960 2024-04-15 10:19:50.548755 pybts-1.7.1/README.md
+-rw-r--r--   0        0        0      385 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2258 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/board/board.py
+-rw-r--r--   0        0        0    11048 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/board/server.py
+-rw-r--r--   0        0        0     8197 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/builder.py
+-rw-r--r--   0        0        0      596 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     9344 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2175 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5460 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/parallel.py
+-rw-r--r--   0        0        0      945 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/ppa.py
+-rw-r--r--   0        0        0     2235 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2460 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/sequence.py
+-rw-r--r--   0        0        0     1510 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/switcher.py
+-rw-r--r--   0        0        0      182 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/composites/template.py
+-rw-r--r--   0        0        0     3243 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/constants.py
+-rw-r--r--   0        0        0     4943 2024-04-15 10:19:50.548755 pybts-1.7.1/pybts/converter.py
+-rw-r--r--   0        0        0      121 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    22898 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1073 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/display.py
+-rw-r--r--   0        0        0     1521 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/main.py
+-rw-r--r--   0        0        0    17662 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/nodes.py
+-rw-r--r--   0        0        0       63 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/__init__.py
+-rw-r--r--   0        0        0     8803 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/base_class.py
+-rw-r--r--   0        0        0      268 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/builder.py
+-rw-r--r--   0        0        0      460 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/common.py
+-rw-r--r--   0        0        0    15167 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/nodes.py
+-rw-r--r--   0        0        0     5687 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/off_policy.py
+-rw-r--r--   0        0        0     8587 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0     1218 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/rl/tree.py
+-rw-r--r--   0        0        0    16958 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-15 10:19:50.552755 pybts-1.7.1/pybts/templates/index.html
+-rw-r--r--   0        0        0  1967920 2024-04-15 10:19:50.560755 pybts-1.7.1/pybts/templates/static/index-BlldS3Jx.js
+-rw-r--r--   0        0        0   320362 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/templates/static/index-DN1S--qx.css
+-rw-r--r--   0        0        0     5267 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/templates/static/info-lb9hZOuB.png
+-rw-r--r--   0        0        0     2140 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/tree.py
+-rw-r--r--   0        0        0    10045 2024-04-15 10:19:50.564755 pybts-1.7.1/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-15 10:19:50.564755 pybts-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6879 1970-01-01 00:00:00.000000 pybts-1.7.1/PKG-INFO
```

### Comparing `pybts-1.7.0/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.7.1/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/README.assets/image-20240329031220580.png` & `pybts-1.7.1/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/README.assets/image-20240329031233459.png` & `pybts-1.7.1/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/README.assets/image-20240401211552611.png` & `pybts-1.7.1/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/README.assets/image-20240401211609525.png` & `pybts-1.7.1/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/README.md` & `pybts-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/board/board.py` & `pybts-1.7.1/pybts/board/board.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/board/server.py` & `pybts-1.7.1/pybts/board/server.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/builder.py` & `pybts-1.7.1/pybts/builder.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/__init__.py` & `pybts-1.7.1/pybts/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/composite.py` & `pybts-1.7.1/pybts/composites/composite.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/condition_branch.py` & `pybts-1.7.1/pybts/composites/condition_branch.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/parallel.py` & `pybts-1.7.1/pybts/composites/parallel.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/ppa.py` & `pybts-1.7.1/pybts/composites/ppa.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/selector.py` & `pybts-1.7.1/pybts/composites/selector.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/sequence.py` & `pybts-1.7.1/pybts/composites/sequence.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/composites/switcher.py` & `pybts-1.7.1/pybts/composites/switcher.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/constants.py` & `pybts-1.7.1/pybts/constants.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/converter.py` & `pybts-1.7.1/pybts/converter.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/decorators/nodes.py` & `pybts-1.7.1/pybts/decorators/nodes.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/display.py` & `pybts-1.7.1/pybts/display.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/main.py` & `pybts-1.7.1/pybts/main.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/nodes.py` & `pybts-1.7.1/pybts/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,18 @@
         self.attrs: typing.Dict[str, typing.AnyStr] = kwargs  # 在builder和xml中传递的参数，会在__init__之后提供一个更完整的
         self.context: typing.Optional[dict] = None  # 共享的字典，在tree.setup的时候提供
         if children is not None:
             self.children = children
             for child in children:
                 child.parent = self
 
+    def setup(self, **kwargs: typing.Any) -> None:
+        super().setup(**kwargs)
+        self.name = self.converter.render(self.name)
+    
     def reset(self):
         self.debug_info['reset_count'] += 1
         self._updater_iter = None
         if self.status != Status.INVALID:
             self.stop(Status.INVALID)
 
     @property
```

### Comparing `pybts-1.7.0/pybts/rl/base_class.py` & `pybts-1.7.1/pybts/rl/base_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,242 +1,229 @@
-from pybts.nodes import Node
-from stable_baselines3.common.policies import ActorCriticPolicy
-from pybts.rl.off_policy import *
-from pybts.rl.on_policy import *
-from abc import ABC, abstractmethod
-import gymnasium as gym
-from typing import Union
-
-
-class RLPolicyNode(ABC):
-    """强化学习在线策略节点，拿来跟其他的Node多继承用"""
-
-    def __init__(self):
-        self.rl_collector = None
-        self.rl_accum_reward = 0  # 当前累积奖励
-        self.rl_info = None
-        self.rl_reward = 0  # 当前奖励
-        self.rl_obs = None
-        self.rl_iteration = 0
-        self.rl_done = False
-        self.rl_action = None
-        self.rl_model = None
-
-    def reset(self):
-        self.rl_accum_reward = 0
-
-    def to_data(self):
-        return {
-            'rl_iteration'   : self.rl_iteration,
-            'rl_policy'      : str(self.rl_policy()),
-            'rl_info'        : self.rl_info,
-            'rl_reward'      : self.rl_reward,
-            'rl_obs'         : self.rl_obs,
-            'rl_accum_reward': self.rl_accum_reward,
-            'rl_action'      : self.rl_action,
-            'rl_reward_scope': self.rl_reward_scope(),
-        }
-
-    @abstractmethod
-    def rl_env(self) -> gym.Env:
-        raise NotImplemented
-
-    @abstractmethod
-    def rl_action_space(self) -> gym.spaces.Space:
-        raise NotImplemented
-
-    @abstractmethod
-    def rl_observation_space(self) -> gym.spaces.Space:
-        raise NotImplemented
-
-    @abstractmethod
-    def rl_gen_obs(self):
-        raise NotImplemented
-
-    @abstractmethod
-    def rl_gen_info(self) -> dict:
-        raise NotImplemented
-
-    def rl_reward_scope(self) -> str:
-        """
-        奖励域
-
-        例如：default
-        多个奖励域用,分隔
-        如果设置了奖励域，则生成本轮奖励时会从self.context.rl_reward[scope]里获取
-        """
-        return ''
-
-    @abstractmethod
-    def rl_gen_reward(self) -> float:
-        reward_scope = self.rl_reward_scope()
-        if reward_scope != '':
-            assert isinstance(self, Node), 'RLOnPolicyNode 必须得继承Node节点'
-            assert self.context is not None, 'context必须得设置好'
-            assert 'reward' in self.context, 'context必须得含有rl_reward键'
-            scopes = reward_scope.split(',')
-            curr_reward = 0
-            for scope in scopes:
-                curr_reward += self.context['reward'].get(scope, 0)
-            return curr_reward - self.rl_accum_reward
-        raise NotImplemented
-
-    @abstractmethod
-    def rl_gen_done(self) -> bool:
-        # 返回当前环境是否结束
-        raise NotImplemented
-
-    def rl_device(self) -> str:
-        return 'cpu'
-
-    def rl_policy(self) -> Union[str, typing.Type[ActorCriticPolicy]]:
-        return 'MlpPolicy'
-
-    @abstractmethod
-    def rl_take_action(
-            self,
-            train: bool,
-            log_interval: int = 1,
-            save_interval: int = 5,
-            save_path: str = ''
-    ):
-        if isinstance(self.rl_model, OnPolicyAlgorithm):
-            return self._rl_on_policy_take_action(
-                    train=train,
-                    log_interval=log_interval,
-                    save_interval=save_interval,
-                    save_path=save_path)
-        else:
-            return self._rl_off_policy_take_action(
-                    train=train,
-                    log_interval=log_interval,
-                    save_interval=save_interval,
-                    save_path=save_path
-            )
-
-    def _rl_off_policy_take_action(
-            self,
-            train: bool,
-            log_interval: int = 1,
-            save_interval: int = 5,
-            save_path: str = ''
-    ):
-        assert self.rl_model is not None, 'RL model not initialized'
-        assert isinstance(self.rl_model, OffPolicyAlgorithm), 'RL model must be initialized with OffPolicyAlgorithm'
-        model: OffPolicyAlgorithm = self.rl_model
-        info = self.rl_gen_info()
-        reward = self.rl_gen_reward()
-        obs = self.rl_gen_obs()
-        done = self.rl_gen_done()
-
-        if train:
-            try:
-                if self.rl_collector is None:
-                    self.rl_collector = bt_off_policy_collect_rollouts(
-                            model,
-                            train_freq=model.train_freq,
-                            action_noise=model.action_noise,
-                            learning_starts=model.learning_starts,
-                            replay_buffer=model.replay_buffer,
-                            log_interval=log_interval,
-                    )
-                    action = self.rl_collector.send(None)
-                else:
-                    info = info
-                    action = self.rl_collector.send((obs, reward, done, info))
-
-                if isinstance(action, RolloutReturn):
-                    # 结束了
-                    rollout: RolloutReturn = action
-                    if model.num_timesteps > 0 and model.num_timesteps > model.learning_starts:
-                        # If no `gradient_steps` is specified,
-                        # do as many gradients steps as steps performed during the rollout
-                        gradient_steps = model.gradient_steps if model.gradient_steps >= 0 else rollout.episode_timesteps
-                        # Special case when the user passes `gradient_steps=0`
-                        if gradient_steps > 0:
-                            model.train(batch_size=model.batch_size, gradient_steps=gradient_steps)
-
-                    self.rl_collector = bt_off_policy_collect_rollouts(
-                            model,
-                            train_freq=model.train_freq,
-                            action_noise=model.action_noise,
-                            learning_starts=model.learning_starts,
-                            replay_buffer=model.replay_buffer,
-                            log_interval=log_interval,
-                    )
-                    action = self.rl_collector.send(None)
-            except StopIteration:
-                self.rl_collector = None
-                self.rl_iteration += 1
-                # Display training infos
-
-                if self.rl_iteration % save_interval == 0:
-                    model.save(save_path)
-
-                self.rl_collector = bt_off_policy_collect_rollouts(
-                        model,
-                        train_freq=model.train_freq,
-                        action_noise=model.action_noise,
-                        learning_starts=model.learning_starts,
-                        replay_buffer=model.replay_buffer,
-                        log_interval=log_interval,
-                )
-                action = self.rl_collector.send(None)
-        else:
-            # 预测模式
-            action, state = model.predict(obs)
-
-        self.rl_obs = obs
-        self.rl_reward = reward
-        self.rl_info = info
-        self.rl_accum_reward += reward
-        self.rl_action = action
-        self.rl_done = done
-        return action
-
-    def _rl_on_policy_take_action(
-            self,
-            train: bool,
-            log_interval: int = 1,
-            save_interval: int = 5,
-            save_path: str = ''
-    ):
-        assert self.rl_model is not None, 'RL model not initialized'
-        assert isinstance(self.rl_model, OnPolicyAlgorithm), 'RL model must be an instance of OnPolicyAlgorithm'
-        model: OnPolicyAlgorithm = self.rl_model
-        info = self.rl_gen_info()
-        reward = self.rl_gen_reward()
-        obs = self.rl_gen_obs()
-        done = self.rl_gen_done()
-        if train:
-            try:
-                if self.rl_collector is None:
-                    self.rl_collector = bt_on_policy_collect_rollouts(
-                            model,
-                            last_obs=obs)
-                    action = self.rl_collector.send(None)
-                else:
-                    info = info
-                    action = self.rl_collector.send((obs, reward, done, info))
-            except StopIteration:
-                self.rl_collector = None
-                self.rl_iteration += 1
-                # Display training infos
-                bt_on_policy_train(model, iteration=self.rl_iteration, log_interval=log_interval)
-                if self.rl_iteration % save_interval == 0:
-                    model.save(save_path)
-
-                self.rl_collector = bt_on_policy_collect_rollouts(
-                        model,
-                        last_obs=obs)
-                action = self.rl_collector.send(None)
-        else:
-            # 预测模式
-            action, state = model.predict(obs)
-
-        self.rl_obs = obs
-        self.rl_reward = reward
-        self.rl_info = info
-        self.rl_accum_reward += reward
-        self.rl_action = action
-        self.rl_done = done
-        return action
+# from pybts.nodes import Node
+# from stable_baselines3.common.policies import ActorCriticPolicy
+# from pybts.rl.off_policy import *
+# from pybts.rl.on_policy import *
+# from abc import ABC, abstractmethod
+# import gymnasium as gym
+# from typing import Union
+#
+#
+# class RLPolicyNode(ABC):
+#     """强化学习在线策略节点，拿来跟其他的Node多继承用"""
+#
+#     def __init__(self):
+#         self.rl_collector = None
+#         self.rl_accum_reward = 0  # 当前累积奖励
+#         self.rl_info = None
+#         self.rl_reward = 0  # 当前奖励
+#         self.rl_obs = None
+#         self.rl_iteration = 0
+#         self.rl_done = False
+#         self.rl_action = None
+#         self.rl_model = None
+#
+#     def reset(self):
+#         self.rl_accum_reward = 0
+#
+#     def to_data(self):
+#         return {
+#             'rl_iteration'   : self.rl_iteration,
+#             'rl_policy'      : str(self.rl_policy()),
+#             'rl_info'        : self.rl_info,
+#             'rl_reward'      : self.rl_reward,
+#             'rl_obs'         : self.rl_obs,
+#             'rl_accum_reward': self.rl_accum_reward,
+#             'rl_action'      : self.rl_action,
+#             'rl_reward_scope': self.rl_reward_scope(),
+#         }
+#
+#     @abstractmethod
+#     def rl_env(self) -> gym.Env:
+#         raise NotImplemented
+#
+#     @abstractmethod
+#     def rl_action_space(self) -> gym.spaces.Space:
+#         raise NotImplemented
+#
+#     @abstractmethod
+#     def rl_observation_space(self) -> gym.spaces.Space:
+#         raise NotImplemented
+#
+#     @abstractmethod
+#     def rl_gen_obs(self):
+#         raise NotImplemented
+#
+#     @abstractmethod
+#     def rl_gen_info(self) -> dict:
+#         raise NotImplemented
+#
+#     def rl_reward_scope(self) -> str:
+#         """
+#         奖励域
+#
+#         例如：default
+#         多个奖励域用,分隔
+#         如果设置了奖励域，则生成本轮奖励时会从self.context.rl_reward[scope]里获取
+#         """
+#         return ''
+#
+#     @abstractmethod
+#     def rl_gen_reward(self) -> float:
+#         reward_scope = self.rl_reward_scope()
+#         if reward_scope != '':
+#             assert isinstance(self, Node), 'RLOnPolicyNode 必须得继承Node节点'
+#             assert self.context is not None, 'context必须得设置好'
+#             assert 'reward' in self.context, 'context必须得含有rl_reward键'
+#             scopes = reward_scope.split(',')
+#             curr_reward = 0
+#             for scope in scopes:
+#                 curr_reward += self.context['reward'].get(scope, 0)
+#             return curr_reward - self.rl_accum_reward
+#         raise NotImplemented
+#
+#     @abstractmethod
+#     def rl_gen_done(self) -> bool:
+#         # 返回当前环境是否结束
+#         raise NotImplemented
+#
+#     def rl_device(self) -> str:
+#         return 'cpu'
+#
+#     def rl_policy(self) -> Union[str, typing.Type[ActorCriticPolicy]]:
+#         return 'MlpPolicy'
+#
+#     @abstractmethod
+#     def rl_take_action(
+#             self,
+#             train: bool,
+#             log_interval: int = 1,
+#     ):
+#         if isinstance(self.rl_model, OnPolicyAlgorithm):
+#             return self._rl_on_policy_take_action(
+#                     train=train,
+#                     log_interval=log_interval)
+#         else:
+#             return self._rl_off_policy_take_action(
+#                     train=train,
+#                     log_interval=log_interval,
+#             )
+#
+#     def _rl_off_policy_take_action(
+#             self,
+#             train: bool,
+#             log_interval: int = 1,
+#     ):
+#         print('_rl_off_policy_take_action', train)
+#         assert self.rl_model is not None, 'RL model not initialized'
+#         assert isinstance(self.rl_model, OffPolicyAlgorithm), 'RL model must be initialized with OffPolicyAlgorithm'
+#         model: OffPolicyAlgorithm = self.rl_model
+#         info = self.rl_gen_info()
+#         reward = self.rl_gen_reward()
+#         obs = self.rl_gen_obs()
+#         done = self.rl_gen_done()
+#
+#         if train:
+#             try:
+#                 if self.rl_collector is None:
+#                     self.rl_collector = bt_off_policy_collect_rollouts(
+#                             model,
+#                             train_freq=model.train_freq,
+#                             action_noise=model.action_noise,
+#                             learning_starts=model.learning_starts,
+#                             replay_buffer=model.replay_buffer,
+#                             log_interval=log_interval,
+#                     )
+#                     action = self.rl_collector.send(None)
+#                 else:
+#                     info = info
+#                     action = self.rl_collector.send((obs, reward, done, info))
+#
+#                 if isinstance(action, RolloutReturn):
+#                     # 结束了
+#                     rollout: RolloutReturn = action
+#                     if model.num_timesteps > 0 and model.num_timesteps > model.learning_starts:
+#                         # If no `gradient_steps` is specified,
+#                         # do as many gradients steps as steps performed during the rollout
+#                         gradient_steps = model.gradient_steps if model.gradient_steps >= 0 else rollout.episode_timesteps
+#                         # Special case when the user passes `gradient_steps=0`
+#                         if gradient_steps > 0:
+#                             model.train(batch_size=model.batch_size, gradient_steps=gradient_steps)
+#
+#                     self.rl_collector = bt_off_policy_collect_rollouts(
+#                             model,
+#                             train_freq=model.train_freq,
+#                             action_noise=model.action_noise,
+#                             learning_starts=model.learning_starts,
+#                             replay_buffer=model.replay_buffer,
+#                             log_interval=log_interval,
+#                     )
+#                     action = self.rl_collector.send(None)
+#             except StopIteration:
+#                 self.rl_collector = None
+#                 self.rl_iteration += 1
+#                 # Display training infos
+#
+#                 self.rl_collector = bt_off_policy_collect_rollouts(
+#                         model,
+#                         train_freq=model.train_freq,
+#                         action_noise=model.action_noise,
+#                         learning_starts=model.learning_starts,
+#                         replay_buffer=model.replay_buffer,
+#                         log_interval=log_interval,
+#                 )
+#                 action = self.rl_collector.send(None)
+#         else:
+#             # 预测模式
+#             action, state = model.predict(obs)
+#
+#         self.rl_obs = obs
+#         self.rl_reward = reward
+#         self.rl_info = info
+#         self.rl_accum_reward += reward
+#         self.rl_action = action
+#         self.rl_done = done
+#         return action
+#
+#     def _rl_on_policy_take_action(
+#             self,
+#             train: bool,
+#             log_interval: int = 1,
+#     ):
+#         print('_rl_on_policy_take_action', train)
+#         assert self.rl_model is not None, 'RL model not initialized'
+#         assert isinstance(self.rl_model, OnPolicyAlgorithm), 'RL model must be an instance of OnPolicyAlgorithm'
+#         model: OnPolicyAlgorithm = self.rl_model
+#         info = self.rl_gen_info()
+#         reward = self.rl_gen_reward()
+#         obs = self.rl_gen_obs()
+#         done = self.rl_gen_done()
+#         if train:
+#             try:
+#                 if self.rl_collector is None:
+#                     self.rl_collector = bt_on_policy_collect_rollouts(
+#                             model,
+#                             last_obs=obs)
+#                     action = self.rl_collector.send(None)
+#                 else:
+#                     info = info
+#                     action = self.rl_collector.send((obs, reward, done, info))
+#             except StopIteration:
+#                 self.rl_collector = None
+#                 self.rl_iteration += 1
+#                 # Display training infos
+#                 bt_on_policy_train(model, iteration=self.rl_iteration, log_interval=log_interval)
+#
+#                 self.rl_collector = bt_on_policy_collect_rollouts(
+#                         model,
+#                         last_obs=obs)
+#                 action = self.rl_collector.send(None)
+#         else:
+#             # 预测模式
+#             action, state = model.predict(obs)
+#
+#         self.rl_obs = obs
+#         self.rl_reward = reward
+#         self.rl_info = info
+#         self.rl_accum_reward += reward
+#         self.rl_action = action
+#         self.rl_done = done
+#         return action
```

### Comparing `pybts-1.7.0/pybts/rl/nodes.py` & `pybts-1.7.1/pybts/rl/nodes.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/rl/off_policy.py` & `pybts-1.7.1/pybts/rl/off_policy.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/rl/on_policy.py` & `pybts-1.7.1/pybts/rl/on_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
                 clipped_actions = self.policy.unscale_action(clipped_actions)
             else:
                 # Otherwise, clip the actions to avoid out of bound error
                 # as we are sampling from an unbounded Gaussian distribution
                 clipped_actions = np.clip(actions, self.action_space.low, self.action_space.high)
 
         new_obs, rewards, dones, infos = yield clipped_actions[0]
+
         # 数据都从单个处理成批量的
         new_obs = np.expand_dims(new_obs, axis=0)
         rewards = np.array([rewards])
         dones = np.array([dones])
         infos = [infos]
 
         self.num_timesteps += 1
```

### Comparing `pybts-1.7.0/pybts/rl/tree.py` & `pybts-1.7.1/pybts/rl/tree.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     def __init__(self, root: Node, name: str = '', context: dict = None):
         super().__init__(root=root, name=name, context=context)
         self.context['reward'] = defaultdict(int)  # 本轮的奖励，默认scope是default
 
     def reset(self):
         super().reset()
+        # 先reset所有节点再清空奖励
         # 清空奖励
         self.context['reward'] = defaultdict(int)
 
     def tick(
             self: RLTree,
             pre_tick_handler: typing.Optional[
                 typing.Callable[[RLTree], None]
```

### Comparing `pybts-1.7.0/pybts/templates/favicon.ico` & `pybts-1.7.1/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/templates/static/index-BlldS3Jx.js` & `pybts-1.7.1/pybts/templates/static/index-BlldS3Jx.js`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/templates/static/index-DN1S--qx.css` & `pybts-1.7.1/pybts/templates/static/index-DN1S--qx.css`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/templates/static/info-lb9hZOuB.png` & `pybts-1.7.1/pybts/templates/static/info-lb9hZOuB.png`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/tree.py` & `pybts-1.7.1/pybts/tree.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pybts/utility.py` & `pybts-1.7.1/pybts/utility.py`

 * *Files identical despite different names*

### Comparing `pybts-1.7.0/pyproject.toml` & `pybts-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybts"
-version = "1.7.0"
+version = "1.7.1"
 description = ""
 authors = ["王童 <785271992@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/wangtong2015/pybts"
 repository = "https://github.com/wangtong2015/pybts"
 keywords = ["BehaviorTree", "AI"]
 include = ["README.md", "pybts/templates/static/*", 'pybts/templates/*', 'README.assets']
```

### Comparing `pybts-1.7.0/PKG-INFO` & `pybts-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.7.0
+Version: 1.7.1
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

