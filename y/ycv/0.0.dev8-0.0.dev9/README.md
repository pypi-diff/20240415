# Comparing `tmp/ycv-0.0.dev8.tar.gz` & `tmp/ycv-0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ycv-0.0.dev8.tar", last modified: Tue Aug 29 07:32:35 2023, max compression
+gzip compressed data, was "ycv-0.0.dev9.tar", last modified: Tue Oct 24 12:22:46 2023, max compression
```

## Comparing `ycv-0.0.dev8.tar` & `ycv-0.0.dev9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-29 07:32:35.547357 ycv-0.0.dev8/
--rw-r--r--   0 arif      (1000) arif      (1000)     1071 2023-06-19 13:59:34.000000 ycv-0.0.dev8/LICENSE
--rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-08-29 07:32:35.547357 ycv-0.0.dev8/PKG-INFO
--rw-r--r--   0 arif      (1000) arif      (1000)     2697 2023-06-19 13:59:34.000000 ycv-0.0.dev8/README.md
--rw-r--r--   0 arif      (1000) arif      (1000)       84 2023-06-19 13:59:34.000000 ycv-0.0.dev8/pyproject.toml
--rw-r--r--   0 arif      (1000) arif      (1000)      686 2023-08-29 07:32:35.548357 ycv-0.0.dev8/setup.cfg
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-29 07:32:35.545357 ycv-0.0.dev8/test/
--rw-r--r--   0 arif      (1000) arif      (1000)      204 2023-06-19 13:59:34.000000 ycv-0.0.dev8/test/test_interface.py
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-29 07:32:35.545357 ycv-0.0.dev8/ycv/
--rw-r--r--   0 arif      (1000) arif      (1000)       88 2023-06-19 13:59:34.000000 ycv-0.0.dev8/ycv/__init__.py
--rw-r--r--   0 arif      (1000) arif      (1000)     2311 2023-06-19 13:59:34.000000 ycv-0.0.dev8/ycv/publications.py
--rw-r--r--   0 arif      (1000) arif      (1000)    25527 2023-08-29 07:27:51.000000 ycv-0.0.dev8/ycv/yamlToTex.py
--rw-r--r--   0 arif      (1000) arif      (1000)     1503 2023-06-19 13:59:34.000000 ycv-0.0.dev8/ycv/ycv.py
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-29 07:32:35.547357 ycv-0.0.dev8/ycv.egg-info/
--rw-r--r--   0 arif      (1000) arif      (1000)     3204 2023-08-29 07:32:35.000000 ycv-0.0.dev8/ycv.egg-info/PKG-INFO
--rw-r--r--   0 arif      (1000) arif      (1000)      293 2023-08-29 07:32:35.000000 ycv-0.0.dev8/ycv.egg-info/SOURCES.txt
--rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-08-29 07:32:35.000000 ycv-0.0.dev8/ycv.egg-info/dependency_links.txt
--rw-r--r--   0 arif      (1000) arif      (1000)       48 2023-08-29 07:32:35.000000 ycv-0.0.dev8/ycv.egg-info/entry_points.txt
--rw-r--r--   0 arif      (1000) arif      (1000)       20 2023-08-29 07:32:35.000000 ycv-0.0.dev8/ycv.egg-info/requires.txt
--rw-r--r--   0 arif      (1000) arif      (1000)        4 2023-08-29 07:32:35.000000 ycv-0.0.dev8/ycv.egg-info/top_level.txt
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-10-24 12:22:46.886083 ycv-0.0.dev9/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1071 2023-06-19 13:59:34.000000 ycv-0.0.dev9/LICENSE
+-rw-r--r--   0 arif      (1000) arif      (1000)     3254 2023-10-24 12:22:46.886083 ycv-0.0.dev9/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)     2697 2023-06-19 13:59:34.000000 ycv-0.0.dev9/README.md
+-rw-r--r--   0 arif      (1000) arif      (1000)       84 2023-06-19 13:59:34.000000 ycv-0.0.dev9/pyproject.toml
+-rw-r--r--   0 arif      (1000) arif      (1000)      686 2023-10-24 12:22:46.887082 ycv-0.0.dev9/setup.cfg
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-10-24 12:22:46.884082 ycv-0.0.dev9/test/
+-rw-r--r--   0 arif      (1000) arif      (1000)      204 2023-06-19 13:59:34.000000 ycv-0.0.dev9/test/test_interface.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-10-24 12:22:46.885083 ycv-0.0.dev9/ycv/
+-rw-r--r--   0 arif      (1000) arif      (1000)       88 2023-06-19 13:59:34.000000 ycv-0.0.dev9/ycv/__init__.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2311 2023-06-19 13:59:34.000000 ycv-0.0.dev9/ycv/publications.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    27371 2023-10-24 12:10:18.000000 ycv-0.0.dev9/ycv/yamlToTex.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1503 2023-06-19 13:59:34.000000 ycv-0.0.dev9/ycv/ycv.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-10-24 12:22:46.886083 ycv-0.0.dev9/ycv.egg-info/
+-rw-r--r--   0 arif      (1000) arif      (1000)     3254 2023-10-24 12:22:46.000000 ycv-0.0.dev9/ycv.egg-info/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)      293 2023-10-24 12:22:46.000000 ycv-0.0.dev9/ycv.egg-info/SOURCES.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-10-24 12:22:46.000000 ycv-0.0.dev9/ycv.egg-info/dependency_links.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       48 2023-10-24 12:22:46.000000 ycv-0.0.dev9/ycv.egg-info/entry_points.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       20 2023-10-24 12:22:46.000000 ycv-0.0.dev9/ycv.egg-info/requires.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        4 2023-10-24 12:22:46.000000 ycv-0.0.dev9/ycv.egg-info/top_level.txt
```

### Comparing `ycv-0.0.dev8/LICENSE` & `ycv-0.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev8/PKG-INFO` & `ycv-0.0.dev9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: ycv
-Version: 0.0.dev8
+Version: 0.0.dev9
 Summary: Build CV and job application materials from yaml files
 Home-page: https://github.com/md-arif-shaikh/ycv
 Author: Md Arif Shaikh
 Author-email: arifshaikh.astro@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-arif-shaikh/ycv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
+Requires-Dist: bibtexparser
 
 [![github](https://img.shields.io/badge/GitHub-ycv-blue.svg)](https://github.com/md-arif-shaikh/ycv)
 [![PyPI version](https://badge.fury.io/py/ycv.svg)](https://pypi.org/project/ycv)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/md-arif-shaikh/ycv/blob/main/LICENSE)
 [![Build Status](https://github.com/md-arif-shaikh/ycv/actions/workflows/test.yaml/badge.svg)](https://github.com/md-arif-shaikh/ycv/actions/workflows/test.yaml)
 
 # ycv
```

### Comparing `ycv-0.0.dev8/README.md` & `ycv-0.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev8/setup.cfg` & `ycv-0.0.dev9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ycv
-version = 0.0.dev8
+version = 0.0.dev9
 author = Md Arif Shaikh
 author_email = arifshaikh.astro@gmail.com
 description = Build CV and job application materials from yaml files
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/md-arif-shaikh/ycv
 project_urls =
```

### Comparing `ycv-0.0.dev8/ycv/publications.py` & `ycv-0.0.dev9/ycv/publications.py`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev8/ycv/yamlToTex.py` & `ycv-0.0.dev9/ycv/yamlToTex.py`

 * *Files 5% similar despite different names*

```diff
@@ -257,15 +257,16 @@
                                       "education": self.create_education_for_cv,
                                       "publications": self.create_list_of_publications_for_cv,
                                       "presentations": self.create_presentations_for_cv,
                                       "references": self.create_list_of_references_for_cv,
                                       "achievements": self.create_achievements_for_cv,
                                       "visits": self.create_visits_for_cv,
                                       "teaching": self.create_teaching_for_cv,
-                                      "refereeing": self.create_refereeing_for_cv}
+                                      "refereeing": self.create_refereeing_for_cv,
+                                      "meetings": self.create_meetings_for_cv}
         return cv_section_generators_dict[sec]
 
     def create_positions_for_cv(self):
         positions = self.cv["positions"]
         pos_text = "\\" + self.cv_section + self.cv_section_number + "{Positions}\n"
         pos_text += "\\begin{itemize}\n"
         for idx, pos in enumerate(positions):
@@ -424,21 +425,63 @@
                 references_text += rf", Phone: {ref['phone']}" + "\n\n"
             else:
                 references_text += "\n\n"
         references_text += "\\end{itemize}\n"
         return references_text
 
     def create_presentations_for_cv(self):
-        tex = "\\" + self.cv_section + self.cv_section_number + "{Conferences, seminars \& workshops}\n"
+        tex = "\\" + self.cv_section + self.cv_section_number + "{Presentations}\n"
         for presentation in self.cv["presentations"]:
             title = self.cv["presentations"][presentation]["title"]
             tex += f"\\sub{self.cv_section}" + self.cv_section_number + f"{{{title}}}\n"
             tex += self.create_list_of_talks_body(self.cv["presentations"][presentation]["file"])
         return tex
 
+    def create_meetings_for_cv(self):
+        tex = "\\" + self.cv_section + self.cv_section_number + "{" + self.cv['meetings']['title'] + "}\n"
+        tex += self.create_list_of_meetings(self.cv["meetings"]["file"])
+        return tex
+
+    def create_list_of_meetings(self, list_of_files):
+        meetins_dict = {}
+        for filename in list_of_files:
+            meetins_dict.update(self.get_data_from_yaml_file(filename))
+        sorted_meetings_dict_by_date = sorted(
+            meetins_dict.items(),
+            key=lambda x: datetime.datetime.strptime(
+                f"{x[1]['from-year']}-{x[1]['from-month']}-{x[1]['from-date']:2d}",
+                "%Y-%B-%d"),
+            reverse=True)
+        converted_dict = dict(sorted_meetings_dict_by_date)
+        tex = "\\begin{enumerate}\n"
+        for talk in converted_dict:
+            t = converted_dict[talk]
+            if "date" in t:
+                d = datetime.date.fromisoformat(f"{t['date']}")
+                day = d.strftime("%d")
+                month = d.strftime("%B")
+                year = d.strftime("%Y")
+                t.update({
+                    "from-date": day,
+                    "to-date": day,
+                    "from-month": month,
+                    "to-month": month,
+                    "to-year": year,
+                    "from-year": year})
+            date = self.get_duration_from_dict(t)
+            tex += r"\item "
+            if "conference" in t:
+                tex += self.create_link(t['conference-url'], t['conference'])
+            if "institute" in t:
+                tex += self.create_link(t['institute-url'], t['institute'])
+            tex += f"{t['city']}, {t['country']}, " + "\n"
+            tex += date
+        tex += "\\end{enumerate}\n"
+        return tex
+    
     def create_list_of_talks_body(self, talks_file):
         self.talks_file = talks_file
         self.talks = self.get_data_from_yaml_file(talks_file)
         tex = "\\begin{enumerate}\n"
         for talk in self.talks:
             t = self.talks[talk]
             if "date" in t:
```

### Comparing `ycv-0.0.dev8/ycv/ycv.py` & `ycv-0.0.dev9/ycv/ycv.py`

 * *Files identical despite different names*

### Comparing `ycv-0.0.dev8/ycv.egg-info/PKG-INFO` & `ycv-0.0.dev9/ycv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: ycv
-Version: 0.0.dev8
+Version: 0.0.dev9
 Summary: Build CV and job application materials from yaml files
 Home-page: https://github.com/md-arif-shaikh/ycv
 Author: Md Arif Shaikh
 Author-email: arifshaikh.astro@gmail.com
 Project-URL: Bug Tracker, https://github.com/md-arif-shaikh/ycv/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
+Requires-Dist: bibtexparser
 
 [![github](https://img.shields.io/badge/GitHub-ycv-blue.svg)](https://github.com/md-arif-shaikh/ycv)
 [![PyPI version](https://badge.fury.io/py/ycv.svg)](https://pypi.org/project/ycv)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/md-arif-shaikh/ycv/blob/main/LICENSE)
 [![Build Status](https://github.com/md-arif-shaikh/ycv/actions/workflows/test.yaml/badge.svg)](https://github.com/md-arif-shaikh/ycv/actions/workflows/test.yaml)
 
 # ycv
```

