# Comparing `tmp/pyweatherfr-5.2.0.tar.gz` & `tmp/pyweatherfr-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.2.0.tar", last modified: Sun Apr 14 19:50:18 2024, max compression
+gzip compressed data, was "pyweatherfr-5.2.1.tar", last modified: Mon Apr 15 18:28:21 2024, max compression
```

## Comparing `pyweatherfr-5.2.0.tar` & `pyweatherfr-5.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    41939 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:49:43.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.285866 pyweatherfr-5.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 18:28:21.281866 pyweatherfr-5.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.281866 pyweatherfr-5.2.1/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43111 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:28:21.281866 pyweatherfr-5.2.1/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:27:43.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 18:28:21.000000 pyweatherfr-5.2.1/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:28:21.285866 pyweatherfr-5.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-15 18:27:38.000000 pyweatherfr-5.2.1/setup.py
```

### Comparing `pyweatherfr-5.2.0/LICENSE.txt` & `pyweatherfr-5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.0/PKG-INFO` & `pyweatherfr-5.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.0
+Version: 5.2.1
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.0/README.md` & `pyweatherfr-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.0/pyweatherfr/args.py` & `pyweatherfr-5.2.1/pyweatherfr/args.py`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.2.0/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.2.1/pyweatherfr/pyweatherfr.py`

 * *Files 2% similar despite different names*

```diff
@@ -778,48 +778,66 @@
     print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
 
 
     return ville, dpt, lat, long, country
 
 
 def obtain_city_data():
-
-    town = compute_args().town
+    parties = compute_args().town.split(',')
+    if len(parties)>2:
+        print(my_colored("erreur : format incorrect : attendu 'ville, pays' ou 'ville'","red"))
+        exit(1)
+    if len(parties)==1 and compute_args().world==True:
+        print(my_colored("warning : si la ville souhaitée ne s'affiche pas vous pouvez utiliser le format 'ville, pays' pour la recherche","yellow"))       
+    town = parties[0]
+    others = ','.join(parties[1:])
+    print_debug(town)
+    print_debug(others)
     ctx = ssl.create_default_context(cafile=certifi.where())
     geopy.geocoders.options.default_ssl_context = ctx
     geolocator = geopy.geocoders.Nominatim(user_agent="my_geocoder")
     if compute_args().lang:
-        locations = geolocator.geocode(town,exactly_one=False,addressdetails=True)
+        locations = geolocator.geocode(town+","+others,exactly_one=False,addressdetails=True,limit=9999)
     else:
-        locations = geolocator.geocode(town,exactly_one=False,addressdetails=True,language="fr")    
+        locations = geolocator.geocode(town+","+others,exactly_one=False,addressdetails=True,language="fr",limit=9999)    
     choix = []
     if locations is None:
         print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)  
-    world=False    
+    world=False
+    print_debug(str(len(locations)) +" villes trouvées")    
     for location in locations:
-        print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
-        if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village"):
+        #print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
+        if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or location.raw.get("addresstype")=="hamlet" or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village"):
+            
             
             ville = None
+            if ville is None or (location.raw.get("address").get("hamlet") is not None and (clean_string(location.raw.get("address").get("hamlet").lower())==clean_string(town.lower()))):
+                ville = location.raw.get("address").get("hamlet")
             if ville is None or (location.raw.get("address").get("village") is not None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("village")
             if ville is None or (location.raw.get("address").get("municipality") is not None and (clean_string(location.raw.get("address").get("municipality").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("municipality")
             if ville is None or (location.raw.get("address").get("town") is not None and (clean_string(location.raw.get("address").get("town").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("town")               
             if ville is None or (location.raw.get("address").get("city") is not None and (clean_string(location.raw.get("address").get("city").lower())==clean_string(town.lower()))):
-                ville = location.raw.get("address").get("city")        
-            dpt = location.raw.get("address").get("county")
-            if dpt is None:
-                dpt=location.raw.get("address").get("state")
-            if dpt is None:
-                dpt= location.raw.get("address").get("postcode") 
-            if dpt is None or location.raw.get("address").get("country")!="France":
-                dpt= location.raw.get("address").get("country")
+                ville = location.raw.get("address").get("city") 
+            dpt = ""
+            if location.raw.get("address").get("county") is not None:        
+                dpt = location.raw.get("address").get("county")
+            if location.raw.get("address").get("state") is not None:
+                if dpt =="":
+                    dpt = location.raw.get("address").get("state")  
+                else:
+                    dpt = dpt + ", "+ location.raw.get("address").get("state") 
+            if compute_args().world:
+                if dpt =="":                       
+                    dpt= location.raw.get("address").get("country")
+                else:
+                    dpt= dpt + ", "+location.raw.get("address").get("country")
 
             country = location.raw.get("address").get("country")
             if country == "France":
                 cp = location.raw.get("address").get("postcode")
             else:
                 cp = ""
             lat = location.raw.get("lat")
@@ -1092,10 +1110,10 @@
 def clean_string(mystring):
     if mystring is None:
         return None
     retour =""
     nfkd_form = unicodedata.normalize('NFKD', mystring)
     retour = ''.join([c for c in nfkd_form if not unicodedata.combining(c)])
     retour = retour.replace(' ', '-').replace("'", '-').replace('"', '-')
-    if mystring!=retour:
-        print_debug(mystring + " modifié en " + retour)
+    #if mystring!=retour:
+    #    print_debug(mystring + " modifié en " + retour)
     return retour
```

### Comparing `pyweatherfr-5.2.0/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.2.1/pyweatherfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.2.0
+Version: 5.2.1
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.2.0/setup.py` & `pyweatherfr-5.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.2.0",
+    version="5.2.1",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

