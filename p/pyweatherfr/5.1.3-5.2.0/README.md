# Comparing `tmp/pyweatherfr-5.1.3.tar.gz` & `tmp/pyweatherfr-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweatherfr-5.1.3.tar", last modified: Sun Apr 14 11:44:36 2024, max compression
+gzip compressed data, was "pyweatherfr-5.2.0.tar", last modified: Sun Apr 14 19:50:18 2024, max compression
```

## Comparing `pyweatherfr-5.1.3.tar` & `pyweatherfr-5.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/pyweatherfr/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    41381 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/pyweatherfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/pyweatherfr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/pyweatherfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:44:03.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 11:44:36.000000 pyweatherfr-5.1.3/pyweatherfr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:44:36.887249 pyweatherfr-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 11:43:59.000000 pyweatherfr-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/pyweatherfr/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41939 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/pyweatherfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/pyweatherfr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/pyweatherfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:49:43.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 19:50:18.000000 pyweatherfr-5.2.0/pyweatherfr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 19:50:18.329892 pyweatherfr-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-14 19:49:38.000000 pyweatherfr-5.2.0/setup.py
```

### Comparing `pyweatherfr-5.1.3/LICENSE.txt` & `pyweatherfr-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyweatherfr-5.1.3/PKG-INFO` & `pyweatherfr-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.3
+Version: 5.2.0
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.3/README.md` & `pyweatherfr-5.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 pyweatherfr \[TOWN\] -d [STR]
 
 exemple : ``pyweatherfr Grenoble -d 2024-03-30`` affiche les données météo détaillées pour Grenoble au 30/03/2024
 
 
 ## Autres options
 
+  - ``-w/--world``  recherche la ville en pramètre dans le monde et non seulement en France
   - ``-h/--help``    montrer l'aide
   - ``-u/--update``  update pyweatherfr
   - ``-c/--condensate``  condense la sortie
   - ``--nocolor``  désactive les couleurs et les emojis en sortie
   - ``-v/--verbose``  mode verbeux
   - ``--nocache``  supprime le cache de l'api meteo france avant l'appel
   - ``--utc``    utilise l'heure utc dans les previsions au lieu de l'heure locale de la ville
```

### Comparing `pyweatherfr-5.1.3/pyweatherfr/args.py` & `pyweatherfr-5.2.0/pyweatherfr/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,19 +98,20 @@
         help="utilisation des coordonnées GPS à la place d'un nom de ville",
     )      
     my_parser.add_argument(
         "--nocolor",
         action="store_true",
         help="désactiver couleur et emojis en sortie -à utiliser en cas de problème d'affichage-",
     )
-    #my_parser.add_argument(
-    #    "--world",
-    #    action="store_true",
-    #    help="activer la recherche hors France",
-    #)
+    my_parser.add_argument(
+        "-w",
+        "--world",
+        action="store_true",
+        help="activer la recherche hors France",
+    )
     my_parser.add_argument(
         "--lang",
         action="store_true",
         help="recherche (puis affiche) les villes avec leurs noms locaux",
     )     
     group = my_parser.add_mutually_exclusive_group()
     group.add_argument(
```

### Comparing `pyweatherfr-5.1.3/pyweatherfr/pyweatherfr.py` & `pyweatherfr-5.2.0/pyweatherfr/pyweatherfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,24 +598,14 @@
                         pluie,
                         vent,
                         direction,
                         duree_pluie,
                         duree_soleil
                     ]
                 )
-                headers = [
-                    "date",
-                    "temps",
-                    "température (ressentie)",
-                    "précipitations",
-                    "vent (rafales)",
-                    "direction",
-                    "durée pluie",
-                    "durée soleil"
-                ]
             else:
                 data.append(
                     [
                         datetime.datetime.strftime(
                             datetime.datetime.now(tz=pytz.timezone(tz)).replace(
                                 hour=0, minute=0, second=0, microsecond=0
                             )
@@ -629,28 +619,41 @@
                         vent,
                         direction,
                         duree_pluie,
                         duree_soleil,
                         warning,
                     ]
                 )
-                headers = [
-                    "date",
-                    "temps",
-                    "température (ressentie)",
-                    "précipitations",
-                    "vent (rafales)",
-                    "direction vent",
-                    "durée pluie",
-                    "durée soleil",
-                    "warning",
-                ]
         else:
             tronque=True
     if data != []:
+        if compute_args().nocolor:
+            headers = [
+                "date",
+                "temps",
+                "température (ressentie)",
+                "précipitations",
+                "vent (rafales)",
+                "direction",
+                "durée pluie",
+                "durée soleil"
+            ]
+        else:
+            headers = [
+                "date",
+                "temps",
+                "température (ressentie)",
+                "précipitations",
+                "vent (rafales)",
+                "direction vent",
+                "durée pluie",
+                "durée soleil",
+                "warning",
+            ]
+
         if compute_args().condensate:
             table = columnar.columnar(data, headers, no_borders=True, wrap_max=0)
         else:
             print("")
             table = columnar.columnar(data, headers, no_borders=False, wrap_max=0)
         print(table)
     if tronque:
@@ -788,14 +791,15 @@
         locations = geolocator.geocode(town,exactly_one=False,addressdetails=True)
     else:
         locations = geolocator.geocode(town,exactly_one=False,addressdetails=True,language="fr")    
     choix = []
     if locations is None:
         print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)  
+    world=False    
     for location in locations:
         print_debug(json.dumps(location.raw, indent=4,ensure_ascii=False))
         if ((location.raw.get("addresstype")=="postcode" and location.raw.get("address").get("country")=="France") or location.raw.get("addresstype")=="town" or location.raw.get("addresstype")=="city" or location.raw.get("addresstype")=="municipality" or location.raw.get("addresstype")=="village"):
             
             ville = None
             if ville is None or (location.raw.get("address").get("village") is not None and (clean_string(location.raw.get("address").get("village").lower())==clean_string(town.lower()))):
                 ville = location.raw.get("address").get("village")
@@ -819,41 +823,51 @@
             else:
                 cp = ""
             lat = location.raw.get("lat")
             long = location.raw.get("lon")
             print_debug(ville+"-"+dpt+"-"+lat+"-"+long+"-"+country)
             if (clean_string(ville.lower()) == clean_string(town.lower()) or cp.lower() == town.lower()):
                 if ville+"-"+dpt not in [item[0] for item in choix]:  
-                    choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
+                    if country=="France":
+                        choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
+                    else:
+                        if compute_args().world:
+                            choix.append([ville+"-"+dpt, ville, dpt, country,lat, long])
+                        else:
+                            world=True    
+    if not compute_args().world and world:
+        print("")
+        print(my_colored("warning : il existe des villes hors France disponibles pour wotre recherche. Relancez la avec --world pour y acceder", "yellow"))
     if len(choix)==1:
         choice = choix[0]
         ville = choice[1]
         dpt = choice[2]
         country = choice[3]
         lat = choice[4]
         long = choice[5]
         return ville, dpt, lat, long, country    
-    if len(choix)==0:
+    elif len(choix)==0:
         print(my_colored("erreur : aucune ville trouvée", "red"))
         exit(1)
-    while True:    
-        i=0    
-        for choice in choix:
-            i=i+1
-            print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
-        toto = input("Quelle ville? ")
-        if toto.isnumeric() and 1 <= int(toto) <= len(choix):
-            break
-        print(my_colored("erreur : choix incorrect", "red"))       
-    choice = choix[int(toto)-1]
-    ville = choice[1]
-    dpt = choice[2]
-    country = choice[3]
-    lat = choice[4]
-    long = choice[5]
+    else:
+        while True:    
+            i=0    
+            for choice in choix:
+                i=i+1
+                print("["+str(i)+"] " + choice[1] + " (" + choice[2]+ ")")
+            toto = input("Quelle ville? ")
+            if toto.isnumeric() and 1 <= int(toto) <= len(choix):
+                break
+            print(my_colored("erreur : choix incorrect", "red"))       
+        choice = choix[int(toto)-1]
+        ville = choice[1]
+        dpt = choice[2]
+        country = choice[3]
+        lat = choice[4]
+        long = choice[5]
     return ville, dpt, lat, long, country
 
 
 def my_colored(message, color):
     if compute_args().nocolor:
         return message
     return termcolor.colored(message, color)
```

### Comparing `pyweatherfr-5.1.3/pyweatherfr.egg-info/PKG-INFO` & `pyweatherfr-5.2.0/pyweatherfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweatherfr
-Version: 5.1.3
+Version: 5.2.0
 Summary: pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)
 Home-page: https://github.com/thib1984/pyweatherfr
 Author: thib1984
 Author-email: thibault.garcon@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pyweatherfr-5.1.3/setup.py` & `pyweatherfr-5.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="pyweatherfr",
-    version="5.1.3",
+    version="5.2.0",
     description="pyweatherfr displays weather forecast for a given town in world (with high accuracy for France)",
     long_description="The complete description/installation/use/FAQ is available at : https://github.com/thib1984/pyweatherfr#readme",
     url="https://github.com/thib1984/pyweatherfr",
     author="thib1984",
     author_email="thibault.garcon@gmail.com",
     license="MIT",
     packages=["pyweatherfr"],
```

