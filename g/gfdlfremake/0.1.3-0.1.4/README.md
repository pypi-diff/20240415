# Comparing `tmp/gfdlfremake-0.1.3.tar.gz` & `tmp/gfdlfremake-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfdlfremake-0.1.3.tar", last modified: Mon Apr 15 15:32:19 2024, max compression
+gzip compressed data, was "gfdlfremake-0.1.4.tar", last modified: Mon Apr 15 15:46:38 2024, max compression
```

## Comparing `gfdlfremake-0.1.3.tar` & `gfdlfremake-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:32:19.063903 gfdlfremake-0.1.3/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7642 2024-04-10 13:57:11.000000 gfdlfremake-0.1.3/LICENSE.md
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       69 2024-04-15 15:25:43.000000 gfdlfremake-0.1.3/MANIFEST.in
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      269 2024-04-15 15:32:19.061904 gfdlfremake-0.1.3/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2382 2023-11-01 18:23:29.000000 gfdlfremake-0.1.3/README.md
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:32:19.036911 gfdlfremake-0.1.3/gfdlfremake/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/__init__.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4487 2024-04-15 15:26:01.000000 gfdlfremake-0.1.3/gfdlfremake/buildBaremetal.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7980 2024-04-15 15:26:16.000000 gfdlfremake-0.1.3/gfdlfremake/buildDocker.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     5780 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/checkout.py
--rwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)    12006 2024-04-12 18:17:54.000000 gfdlfremake-0.1.3/gfdlfremake/fremake
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7576 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/makefilefre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4381 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/platformfre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/schema.json
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2367 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/targetfre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2493 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/varsfre.py
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6055 2024-04-15 15:29:22.000000 gfdlfremake-0.1.3/gfdlfremake/yamlfre.py
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:32:19.058910 gfdlfremake-0.1.3/gfdlfremake/yamls/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      231 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/yamls/am5.yaml
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     3046 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/yamls/compile.yaml
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     1131 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/yamls/platforms.yaml
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-12 18:07:18.000000 gfdlfremake-0.1.3/gfdlfremake/yamls/schema.json
-drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:32:19.049923 gfdlfremake-0.1.3/gfdlfremake.egg-info/
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      269 2024-04-15 15:32:18.000000 gfdlfremake-0.1.3/gfdlfremake.egg-info/PKG-INFO
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      610 2024-04-15 15:32:18.000000 gfdlfremake-0.1.3/gfdlfremake.egg-info/SOURCES.txt
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        1 2024-04-15 15:32:18.000000 gfdlfremake-0.1.3/gfdlfremake.egg-info/dependency_links.txt
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       27 2024-04-15 15:32:18.000000 gfdlfremake-0.1.3/gfdlfremake.egg-info/requires.txt
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       12 2024-04-15 15:32:18.000000 gfdlfremake-0.1.3/gfdlfremake.egg-info/top_level.txt
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       38 2024-04-15 15:32:19.063910 gfdlfremake-0.1.3/setup.cfg
--rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      409 2024-04-15 15:32:15.000000 gfdlfremake-0.1.3/setup.py
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:46:38.369897 gfdlfremake-0.1.4/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7642 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/LICENSE.md
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       69 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/MANIFEST.in
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      269 2024-04-15 15:46:38.367894 gfdlfremake-0.1.4/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2382 2023-11-01 18:23:29.000000 gfdlfremake-0.1.4/README.md
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:46:38.338884 gfdlfremake-0.1.4/gfdlfremake/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/__init__.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4487 2024-04-15 15:46:12.000000 gfdlfremake-0.1.4/gfdlfremake/buildBaremetal.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7980 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/buildDocker.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     5780 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/checkout.py
+-rwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)    12006 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/fremake
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     7576 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/makefilefre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     4381 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/platformfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/schema.json
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2367 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/targetfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     2493 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/varsfre.py
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6054 2024-04-15 15:45:25.000000 gfdlfremake-0.1.4/gfdlfremake/yamlfre.py
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:46:38.364887 gfdlfremake-0.1.4/gfdlfremake/yamls/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      231 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/yamls/am5.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     3046 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/yamls/compile.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     1131 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/yamls/platforms.yaml
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)     6593 2024-04-15 15:42:01.000000 gfdlfremake-0.1.4/gfdlfremake/yamls/schema.json
+drwxr-xr-x   0 Bennett.Chang (21243) gfdl       (500)        0 2024-04-15 15:46:38.353888 gfdlfremake-0.1.4/gfdlfremake.egg-info/
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      269 2024-04-15 15:46:38.000000 gfdlfremake-0.1.4/gfdlfremake.egg-info/PKG-INFO
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      610 2024-04-15 15:46:38.000000 gfdlfremake-0.1.4/gfdlfremake.egg-info/SOURCES.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)        1 2024-04-15 15:46:38.000000 gfdlfremake-0.1.4/gfdlfremake.egg-info/dependency_links.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       27 2024-04-15 15:46:38.000000 gfdlfremake-0.1.4/gfdlfremake.egg-info/requires.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       12 2024-04-15 15:46:38.000000 gfdlfremake-0.1.4/gfdlfremake.egg-info/top_level.txt
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)       38 2024-04-15 15:46:38.370889 gfdlfremake-0.1.4/setup.cfg
+-rw-r--r--   0 Bennett.Chang (21243) gfdl       (500)      409 2024-04-15 15:46:23.000000 gfdlfremake-0.1.4/setup.py
```

### Comparing `gfdlfremake-0.1.3/LICENSE.md` & `gfdlfremake-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/README.md` & `gfdlfremake-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/buildBaremetal.py` & `gfdlfremake-0.1.4/gfdlfremake/buildBaremetal.py`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/buildDocker.py` & `gfdlfremake-0.1.4/gfdlfremake/buildDocker.py`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/checkout.py` & `gfdlfremake-0.1.4/gfdlfremake/checkout.py`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/fremake` & `gfdlfremake-0.1.4/gfdlfremake/fremake`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/makefilefre.py` & `gfdlfremake-0.1.4/gfdlfremake/makefilefre.py`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/platformfre.py` & `gfdlfremake-0.1.4/gfdlfremake/platformfre.py`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/schema.json` & `gfdlfremake-0.1.4/gfdlfremake/schema.json`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/targetfre.py` & `gfdlfremake-0.1.4/gfdlfremake/targetfre.py`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/varsfre.py` & `gfdlfremake-0.1.4/gfdlfremake/varsfre.py`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/yamlfre.py` & `gfdlfremake-0.1.4/gfdlfremake/yamlfre.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
           self.modelyaml = yaml.safe_load(v.freVarSub(file.read()))
      self.freyaml.update(self.modelyaml)
      self.compilefile = self.modelyaml["compileYaml"]
      self.compile = compileYaml(self.compilefile,v)
      self.compileyaml = self.compile.getCompileYaml()
      self.freyaml.update(self.compileyaml)
      self.platformsfile = self.modelyaml["platformYaml"]
-     self.platforms = gfdl_fremake.platformfre.platforms(self.platformsfile,v)
+     self.platforms = gfdlfremake.platformfre.platforms(self.platformsfile,v)
      self.platformsyaml = self.platforms.getPlatformsYaml()
      self.freyaml.update(self.platformsyaml)
 ## Validate the YAML
      with open("schema.json", 'r') as f:
          s = f.read()
      schema = json.loads(s)
      validate(instance=self.freyaml, schema=schema)
```

### Comparing `gfdlfremake-0.1.3/gfdlfremake/yamls/compile.yaml` & `gfdlfremake-0.1.4/gfdlfremake/yamls/compile.yaml`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/yamls/platforms.yaml` & `gfdlfremake-0.1.4/gfdlfremake/yamls/platforms.yaml`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake/yamls/schema.json` & `gfdlfremake-0.1.4/gfdlfremake/yamls/schema.json`

 * *Files identical despite different names*

### Comparing `gfdlfremake-0.1.3/gfdlfremake.egg-info/SOURCES.txt` & `gfdlfremake-0.1.4/gfdlfremake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

