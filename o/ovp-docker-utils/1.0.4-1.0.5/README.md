# Comparing `tmp/ovp_docker_utils-1.0.4.tar.gz` & `tmp/ovp_docker_utils-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovp_docker_utils-1.0.4.tar", last modified: Tue Apr  2 03:28:56 2024, max compression
+gzip compressed data, was "ovp_docker_utils-1.0.5.tar", last modified: Mon Apr 15 20:16:57 2024, max compression
```

## Comparing `ovp_docker_utils-1.0.4.tar` & `ovp_docker_utils-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 03:28:56.261077 ovp_docker_utils-1.0.4/
--rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      380 2024-04-02 03:28:56.260078 ovp_docker_utils-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 03:28:56.219748 ovp_docker_utils-1.0.4/ovp_docker_utils/
--rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-02 03:16:28.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/__version__.py
--rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/defaults.py
--rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/docker_compose_instance.py
--rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/oem_logging.py
--rw-rw-rw-   0        0        0    33420 2024-04-02 03:28:03.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/ovp_docker_utils.py
--rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/ssh_file_utils.py
--rw-rw-rw-   0        0        0     3948 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/ssh_key_gen.py
-drwxrwxrwx   0        0        0        0 2024-04-02 03:28:56.259077 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 03:28:56.262080 ovp_docker_utils-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:16:57.819455 ovp_docker_utils-1.0.5/
+-rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      380 2024-04-15 20:16:57.818456 ovp_docker_utils-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 20:16:57.787455 ovp_docker_utils-1.0.5/ovp_docker_utils/
+-rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-15 20:16:15.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/__version__.py
+-rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/defaults.py
+-rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/docker_compose_instance.py
+-rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/oem_logging.py
+-rw-rw-rw-   0        0        0    33479 2024-04-15 20:14:29.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/ovp_docker_utils.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_file_utils.py
+-rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_key_gen.py
+drwxrwxrwx   0        0        0        0 2024-04-15 20:16:57.817456 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-15 20:16:57.000000 ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 20:16:57.819455 ovp_docker_utils-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.5/setup.py
```

### Comparing `ovp_docker_utils-1.0.4/LICENSE` & `ovp_docker_utils-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.4/README.md` & `ovp_docker_utils-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.4/ovp_docker_utils/docker_compose_instance.py` & `ovp_docker_utils-1.0.5/ovp_docker_utils/docker_compose_instance.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.4/ovp_docker_utils/oem_logging.py` & `ovp_docker_utils-1.0.5/ovp_docker_utils/oem_logging.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.4/ovp_docker_utils/ovp_docker_utils.py` & `ovp_docker_utils-1.0.5/ovp_docker_utils/ovp_docker_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,17 @@
     def vpu_name(self):
         return self.vpu_config["device"]["info"]["name"]
 
     def connect(self,) -> bool:
 
         if not USING_IFM3DPY:
             logger.info("ifm3dpy unavailable")
-        if USING_IFM3DPY and self.config.possible_initial_ip_addresses_to_try:
+        if USING_IFM3DPY:
+            if not possible_initial_ip_addresses:
+                possible_initial_ip_addresses = []
             possible_initial_ip_addresses = list(
                 set([self.config.IP] + self.config.possible_initial_ip_addresses_to_try))
             if len(possible_initial_ip_addresses) > 1:
                 logger.info(
                     f"Trying to connect to VPU at any of the following addresses: {possible_initial_ip_addresses}")
 
                 for temp_IP in possible_initial_ip_addresses:
@@ -372,15 +374,15 @@
             self._fw_version = ".".join(self.vpu_config["device"]["swVersion"]["firmware"].split(
                 "-")[0].split(".")[:3])  # get the first 3 parts of the version number
 
             logger.info(f"Device firmware version: {self._fw_version}")
 
             # Check for firmware compatibility
             if not any(
-                    [semver.compare(self._fw_version, range[0])*semver.compare(range[1], self._fw_version) == 1 for range in TESTED_COMPATIBLE_FIRMWARE_RANGES]):
+                    [(semver.compare(self._fw_version, range[0]) >= 0 and semver.compare(range[1], self._fw_version) >= 0) for range in TESTED_COMPATIBLE_FIRMWARE_RANGES]):
                 raise Exception(
                     f"Device firmware version {self._fw_version} is not compatible with version of the deployment manager (tested with the following ranges: {TESTED_COMPATIBLE_FIRMWARE_RANGES})")
 
             self.private_key_path = assign_key(
                 ip=self.config.IP, target_dir=self.config.ssh_key_dir, key_title=self.config.ssh_key_file_name)
 
             logger.info(f"private_key_path = {self.private_key_path}")
```

### Comparing `ovp_docker_utils-1.0.4/ovp_docker_utils/ssh_file_utils.py` & `ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_file_utils.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.4/ovp_docker_utils/ssh_key_gen.py` & `ovp_docker_utils-1.0.5/ovp_docker_utils/ssh_key_gen.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/SOURCES.txt` & `ovp_docker_utils-1.0.5/ovp_docker_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.4/setup.py` & `ovp_docker_utils-1.0.5/setup.py`

 * *Files identical despite different names*

