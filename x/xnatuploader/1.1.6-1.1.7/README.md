# Comparing `tmp/xnatuploader-1.1.6.tar.gz` & `tmp/xnatuploader-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnatuploader-1.1.6.tar", last modified: Tue Feb  6 22:27:45 2024, max compression
+gzip compressed data, was "xnatuploader-1.1.7.tar", last modified: Mon Apr 15 06:04:17 2024, max compression
```

## Comparing `xnatuploader-1.1.6.tar` & `xnatuploader-1.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-02-06 22:27:45.497318 xnatuploader-1.1.6/
--rw-r--r--   0 mike       (501) staff       (20)    14656 2024-02-06 22:27:45.497017 xnatuploader-1.1.6/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)    13805 2023-08-21 06:36:43.000000 xnatuploader-1.1.6/README.md
--rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.6/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)     1104 2024-02-06 22:27:45.498048 xnatuploader-1.1.6/setup.cfg
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-02-06 22:27:45.477726 xnatuploader-1.1.6/src/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-02-06 22:27:45.486353 xnatuploader-1.1.6/src/xnatuploader/
--rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.6/src/xnatuploader/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)      283 2023-05-25 02:08:09.000000 xnatuploader-1.1.6/src/xnatuploader/dataclass.py
--rw-r--r--   0 mike       (501) staff       (20)     3611 2023-12-20 05:46:20.000000 xnatuploader-1.1.6/src/xnatuploader/dicoms.py
--rw-r--r--   0 mike       (501) staff       (20)    15112 2024-02-06 22:21:42.000000 xnatuploader-1.1.6/src/xnatuploader/matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.6/src/xnatuploader/put.py
--rw-r--r--   0 mike       (501) staff       (20)     8601 2024-02-06 22:21:42.000000 xnatuploader-1.1.6/src/xnatuploader/upload.py
--rw-r--r--   0 mike       (501) staff       (20)      203 2023-04-05 06:48:06.000000 xnatuploader-1.1.6/src/xnatuploader/userdict.py
--rw-r--r--   0 mike       (501) staff       (20)     4131 2023-12-20 05:46:20.000000 xnatuploader-1.1.6/src/xnatuploader/workbook.py
--rwxr-xr-x   0 mike       (501) staff       (20)    18883 2023-12-20 05:46:20.000000 xnatuploader-1.1.6/src/xnatuploader/xnatuploader.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-02-06 22:27:45.495874 xnatuploader-1.1.6/src/xnatuploader.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)    14656 2024-02-06 22:27:45.000000 xnatuploader-1.1.6/src/xnatuploader.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      615 2024-02-06 22:27:45.000000 xnatuploader-1.1.6/src/xnatuploader.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2024-02-06 22:27:45.000000 xnatuploader-1.1.6/src/xnatuploader.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)       64 2024-02-06 22:27:45.000000 xnatuploader-1.1.6/src/xnatuploader.egg-info/entry_points.txt
--rw-r--r--   0 mike       (501) staff       (20)      123 2024-02-06 22:27:45.000000 xnatuploader-1.1.6/src/xnatuploader.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       13 2024-02-06 22:27:45.000000 xnatuploader-1.1.6/src/xnatuploader.egg-info/top_level.txt
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-02-06 22:27:45.495094 xnatuploader-1.1.6/tests/
--rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.6/tests/test_config.py
--rw-r--r--   0 mike       (501) staff       (20)     3117 2024-02-06 22:21:42.000000 xnatuploader-1.1.6/tests/test_matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     6032 2023-12-20 05:46:20.000000 xnatuploader-1.1.6/tests/test_scan.py
--rw-r--r--   0 mike       (501) staff       (20)     6014 2023-12-20 05:46:20.000000 xnatuploader-1.1.6/tests/test_upload.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.357443 xnatuploader-1.1.7/
+-rw-r--r--   0 mike       (501) staff       (20)    14656 2024-04-15 06:04:17.356798 xnatuploader-1.1.7/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)    13805 2023-08-21 06:36:43.000000 xnatuploader-1.1.7/README.md
+-rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.7/pyproject.toml
+-rw-r--r--   0 mike       (501) staff       (20)     1104 2024-04-15 06:04:17.358771 xnatuploader-1.1.7/setup.cfg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.332955 xnatuploader-1.1.7/src/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.344589 xnatuploader-1.1.7/src/xnatuploader/
+-rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.7/src/xnatuploader/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)      283 2023-05-25 02:08:09.000000 xnatuploader-1.1.7/src/xnatuploader/dataclass.py
+-rw-r--r--   0 mike       (501) staff       (20)     3420 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/dicoms.py
+-rw-r--r--   0 mike       (501) staff       (20)    14733 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.7/src/xnatuploader/put.py
+-rw-r--r--   0 mike       (501) staff       (20)     8483 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/upload.py
+-rw-r--r--   0 mike       (501) staff       (20)      203 2023-04-05 06:48:06.000000 xnatuploader-1.1.7/src/xnatuploader/userdict.py
+-rw-r--r--   0 mike       (501) staff       (20)     4131 2023-12-20 05:46:20.000000 xnatuploader-1.1.7/src/xnatuploader/workbook.py
+-rwxr-xr-x   0 mike       (501) staff       (20)    19103 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/src/xnatuploader/xnatuploader.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.354949 xnatuploader-1.1.7/src/xnatuploader.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)    14656 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)      615 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)       64 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/entry_points.txt
+-rw-r--r--   0 mike       (501) staff       (20)      123 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)       13 2024-04-15 06:04:17.000000 xnatuploader-1.1.7/src/xnatuploader.egg-info/top_level.txt
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-04-15 06:04:17.353873 xnatuploader-1.1.7/tests/
+-rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.7/tests/test_config.py
+-rw-r--r--   0 mike       (501) staff       (20)     3117 2024-02-06 22:21:42.000000 xnatuploader-1.1.7/tests/test_matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     5937 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/tests/test_scan.py
+-rw-r--r--   0 mike       (501) staff       (20)     5938 2024-04-15 05:45:59.000000 xnatuploader-1.1.7/tests/test_upload.py
```

### Comparing `xnatuploader-1.1.6/PKG-INFO` & `xnatuploader-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.6
+Version: 1.1.7
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.6/README.md` & `xnatuploader-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.6/setup.cfg` & `xnatuploader-1.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xnatuploader
-version = 1.1.6
+version = 1.1.7
 author = Mike Lynch
 author_email = m.lynch@sydney.edu.au
 description = CLI tool for uploading multiple files to XNAT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SydneyInformaticsHub/xnatuploader
 project_urls =
```

### Comparing `xnatuploader-1.1.6/src/xnatuploader/dicoms.py` & `xnatuploader-1.1.7/src/xnatuploader/dicoms.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,26 +23,25 @@
     "DICOM:StudyDate",
     "DICOM:StudyDescription",
 ]
 
 logger = logging.getLogger(__name__)
 
 
-def dicom_extractor(file, options):
+def dicom_extractor(file):
     """
     Try to extract DICOM metadata from a file, and check that it doesn't
     have an encapsulated document, or is of modality SR (which is a special
-    type reserved for reports).
+    type reserved for reports), or has image type DOSE_INFO (which makes
+    XNAT break on metadata extraction)
 
     Raises ExtractException if the file is not a DICOM, has an embedded
-    report or the wrong modality, or one of skip_image_types - this is passed
-    in so that it can be controlled by configuration rather than hard-coded
+    report or the wrong modality
     ---
     file: pathlib.Path
-    options: { str: [ str ]}
 
     returns: {str: str}
 
     raises: ExtractException
     """
     values = None
     dc_meta = None
@@ -54,33 +53,32 @@
         raise ExtractException("DICOM is an encapsulated report")
     values = {f"DICOM:{p}": dc_meta.get(p) for p in DICOM_PARAMS}
     if "DICOM:Modality" not in values:
         raise ExtractException("DICOM has no modality")
     if values["DICOM:Modality"] == "SR":
         raise ExtractException("DICOM is an SR (structured report)")
     image_type = dc_meta.get("ImageType")
-    if "skip_image_types" in options and image_type:
-        if image_type[2] in options["skip_image_types"]:
-            raise ExtractException(f"DICOM has banned image type '{image_type[2]}'")
+    if image_type[2] == "DOSE_INFO":
+        raise ExtractException("DICOM has ImageType DOSE_INFO")
     return values
 
 
 class XNATFileMatch(FileMatch):
     """
     Sublass of FileMatch which provides getters and setters for xnat-specific
     metadata.
     """
 
-    def load_dicom(self, options):
+    def load_dicom(self):
         """
         Utility method used to load the dicom metadata for an umatched file
         so that it can be written to the spreadsheet
         """
         try:
-            dicom_values = dicom_extractor(self.file, options)
+            dicom_values = dicom_extractor(self.file)
             if dicom_values is not None:
                 for key, value in dicom_values.items():
                     self[key] = value
         except ExtractException as e:
             logger.debug(f"DICOM extraction failed: {e}")
 
     # session_label gets constructed by the calling code in xnatuploader,
```

### Comparing `xnatuploader-1.1.6/src/xnatuploader/matcher.py` & `xnatuploader-1.1.7/src/xnatuploader/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,27 +85,22 @@
     A Matcher is a set of patterns for matching against filepaths and mappings
     which map the captured value to field values. It's used to perform
     the matching, returning FileMatch objects.
 
     file_extractor is a function which does application-specific metadata
     extraction: it's up to the calling code to make sure that the values it
     sets are coordinated with the values extracted by the patterns and mappings
-
-    extractor_options is application-specific config which is passed to
-    file_extractor along with the filepath, if there's a need to skip certain
-    files at this stage based on a config setting
     """
 
     def __init__(
         self,
         patterns,
         mappings,
         fields,
         file_extractor=None,
-        extractor_options=None,
         match_class=FileMatch,
         loglevel="WARNING",
     ):
         """
         patterns: OrderedDict(str: str) of path patterns
         mappings: OrderedDict(str: str) of metadata values to captured fields
         fields: list of extra fields to include in the spreadsheet
@@ -114,15 +109,14 @@
         """
         logger.setLevel(loglevel)
         logch = logging.StreamHandler()
         logch.setLevel(loglevel.upper())
         logger.addHandler(logch)
         self.mappings = mappings
         self.file_extractor = file_extractor
-        self.extractor_options = extractor_options
         self.match_class = match_class
         self.fields = fields
         self._headers = None
         self.path_values = []
         self.parse_recipes(patterns)
 
     @property
@@ -291,18 +285,15 @@
 
         returns: a FileMatch
         """
         label, values = self.match_path(filepath.relative_to(root))
         if label:
             if self.file_extractor is not None:
                 try:
-                    file_values = self.file_extractor(
-                        filepath,
-                        self.extractor_options,
-                    )
+                    file_values = self.file_extractor(filepath)
                 except ExtractException as e:
                     match = self.match_class(self, filepath)
                     match.status = "unmatched"
                     match.error = str(e)
                     return match
                 for field, value in file_values.items():
                     values[field] = value  # file metadata can overwrite path
```

### Comparing `xnatuploader-1.1.6/src/xnatuploader/put.py` & `xnatuploader-1.1.7/src/xnatuploader/put.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.6/src/xnatuploader/upload.py` & `xnatuploader-1.1.7/src/xnatuploader/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,23 +195,21 @@
 def trigger_pipelines(xnat_session, project, uploads):
     """
     Call the put API endpoints to trigger DICOM metadata extraction and
     snapshotting on the server
     """
     sessions = {upload.session_label: upload.subject for upload in uploads.values()}
     for session, subject in sessions.items():
-        try:
-            logger.debug(f"Pipelines for {project} / {subject} / {session}")
-            uri = f"/data/projects/{project}/subjects/{subject}/experiments/{session}"
-            xnat_session.put(f"{uri}?pullDataFromHeaders=true")
-            xnat_session.put(f"{uri}?fixScanTypes=true")
-            xnat_session.put(f"{uri}?triggerPipelines=true")
-        except Exception as e:
-            logger.info("Error while triggering metadata extraction / pipelines")
-            logger.info(str(e))
+        uri = f"/data/projects/{project}/subjects/{subject}/experiments/{session}"
+        for cmd in ["pullDataFromHeaders", "fixScanTypes", "triggerPipelines"]:
+            try:
+                xnat_session.put(f"{uri}?{cmd}=true")
+            except Exception as e:
+                logger.error(f"Error on trigger {cmd} for {subject} {session}")
+                logger.error(str(e))
 
 
 def parse_allow_fields(allow_fields):
     """Takes a list of fields which we don't want stripped from the DICOMs
     and tries to convert them to a custom ruleset for dicom-anonymiser. Raises
     a ValueError on any tags which aren't in the DICOM spec."""
```

### Comparing `xnatuploader-1.1.6/src/xnatuploader/workbook.py` & `xnatuploader-1.1.7/src/xnatuploader/workbook.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.6/src/xnatuploader/xnatuploader.py` & `xnatuploader-1.1.7/src/xnatuploader/xnatuploader.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from importlib.metadata import version
 
 __version__ = version("xnatuploader")
 
 from openpyxl import load_workbook
 
-from xnatuploader.matcher import Matcher
+from xnatuploader.matcher import Matcher, ExtractException
 from xnatuploader.dicoms import dicom_extractor, XNATFileMatch, SPREADSHEET_FIELDS
 from xnatuploader.workbook import new_workbook, add_filesheet, load_config
 from xnatuploader.upload import Upload, trigger_pipelines, parse_allow_fields
 
 from xnatutils.base import sanitize_re
 
 FILE_COLUMN_WIDTH = 50
@@ -77,15 +77,15 @@
             logger.debug(f"Scanning {filepath}")
             file = matcher.match(root, filepath)
             if file.success:
                 logger.debug(f"Matched {file.file}")
                 files.append(file)
             else:
                 if include_unmatched:
-                    file.load_dicom(matcher.extractor_options)
+                    file.load_dicom()
                     unmatched.append(file)
 
     skips, uploads = collate_uploads(files, strict_scan_ids)
 
     ns = len(uploads)
     nm = len(files)
     num = len(unmatched)
@@ -290,17 +290,20 @@
         if not file.selected:
             skip.append(file)
         else:
             if file.status == "success":
                 logger.debug(f"skipping file already uploaded {file.file}")
                 skip.append(file)
             else:
-                if file["Subject"] not in subjects:
-                    subjects[file["Subject"]] = []
-                subjects[file["Subject"]].append(file)
+                if not check_safe_dicom(file):
+                    skip.append(file)
+                else:
+                    if file["Subject"] not in subjects:
+                        subjects[file["Subject"]] = []
+                    subjects[file["Subject"]].append(file)
     uploads = {}
     for subject_id, files in subjects.items():
         dates = sorted(set([file.study_date for file in files]))
         visits = {dates[i]: i + 1 for i in range(len(dates))}
         clean_datasets = sanitise_dataset_names(files)
         for file in files:
             visit = visits[file.study_date]
@@ -352,14 +355,27 @@
                 i += 1
                 sanitised = base + str(i)
             clean[file.dataset] = sanitised
             used.append(sanitised)
     return clean
 
 
+def check_safe_dicom(file):
+    """Extra test to make sure that we don't try to upload a dicom with one
+    of the forbidden conditions, even though this is tested for at scan time"""
+    try:
+        dicom_extractor(file.file)
+        return True
+    except ExtractException as e:
+        logger.warning(f"Skipping bad file {file.file}: {e}")
+    except Exception as e:
+        logger.warning(f"Can't upload {file.file}: {e}")
+    return False
+
+
 def get_csv_filename(spreadsheet):
     csv = spreadsheet.with_suffix(".csv")
     n = 0
     while csv.is_file():
         n += 1
         csv = spreadsheet.parent / Path(f"{spreadsheet.stem}.{n}.csv")
     return csv
@@ -509,28 +525,20 @@
 
     if args.operation == "init":
         new_workbook(args.spreadsheet)
         logger.info(f"Initialised spreadsheet at {args.spreadsheet}")
         exit()
 
     config = load_config(args.spreadsheet)
-    skip_image_types = []
-    if "SkipImageTypes" in config["xnat"]:
-        skip_image_types = config["xnat"]["SkipImageTypes"]
-        if skip_image_types is None:
-            skip_image_types = []
-        else:
-            skip_image_types = skip_image_types.split(",")
 
     matcher = Matcher(
         patterns=config["paths"],
         mappings=config["mappings"],
         fields=SPREADSHEET_FIELDS,
         file_extractor=dicom_extractor,
-        extractor_options={"skip_image_types": skip_image_types},
         match_class=XNATFileMatch,
         loglevel=loglevel,
     )
 
     if args.operation == "scan":
         scan(
             matcher,
```

### Comparing `xnatuploader-1.1.6/src/xnatuploader.egg-info/PKG-INFO` & `xnatuploader-1.1.7/src/xnatuploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.6
+Version: 1.1.7
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.6/src/xnatuploader.egg-info/SOURCES.txt` & `xnatuploader-1.1.7/src/xnatuploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.6/tests/test_matcher.py` & `xnatuploader-1.1.7/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.6/tests/test_scan.py` & `xnatuploader-1.1.7/tests/test_scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     fileset = test_files["basic"]
     config = load_config(fileset["config_excel"])
     matcher = Matcher(
         config["paths"],
         config["mappings"],
         SPREADSHEET_FIELDS,
         dicom_extractor,
-        {"skip_image_types": []},
         XNATFileMatch,
     )
     scanned = tmp_path / "scanned.xlsx"
     new_workbook(scanned)
     scan(matcher, Path(fileset["dir"]), scanned, include_unmatched=True)
     expect_wb = load_workbook(fileset["scanned_excel"])
     got_wb = load_workbook(scanned)
@@ -46,15 +45,14 @@
     uploads_dict = fileset["uploads_dict"]
     config = load_config(fileset["config_excel"])
     matcher = Matcher(
         config["paths"],
         config["mappings"],
         SPREADSHEET_FIELDS,
         dicom_extractor,
-        {"skip_image_types": []},
         XNATFileMatch,
     )
     log = tmp_path / "log.xlsx"
     new_workbook(log)
     scan(matcher, Path(fileset["dir"]), log, strict_scan_ids=fileset["strict_scan_ids"])
     wb = load_workbook(log)
     ws = wb["Files"]
@@ -79,15 +77,14 @@
     with open(config_file, "r") as fh:
         config = json.load(fh)
     matcher = Matcher(
         config["paths"],
         config["mappings"],
         SPREADSHEET_FIELDS,
         dicom_extractor,
-        {"skip_image_types": []},
         XNATFileMatch,
     )
     logger.warning(f"Testing santisation in {fileset}")
     log = tmp_path / "log.xlsx"
     new_workbook(log)
     scan(matcher, Path(fileset["dir"]), log, strict_scan_ids=True)
     wb = load_workbook(log)
@@ -114,15 +111,14 @@
     uploads_dict = fileset["uploads_dict"]
     config = load_config(fileset["config_excel"])
     matcher = Matcher(
         config["paths"],
         config["mappings"],
         SPREADSHEET_FIELDS,
         dicom_extractor,
-        {"skip_image_types": []},
         XNATFileMatch,
     )
     log = tmp_path / "log.xlsx"
     new_workbook(log)
     scan(matcher, Path(fileset["dir"]), log, strict_scan_ids=fileset["strict_scan_ids"])
     wb = load_workbook(log)
     ws = wb["Files"]
@@ -152,23 +148,23 @@
         upload_files = [f for f in files if f not in skipstr]
         # don't add if the list of files is empty
         if upload_files:
             upload_skipped[subject_id] = upload_files
     assert uploads == upload_skipped
 
 
-def test_secret_pdfs(tmp_path, test_files):
-    fileset = test_files["secret_pdf"]
+@pytest.mark.parametrize("forbidden", ["secret_pdf", "dose_info"])
+def test_secret_pdfs(tmp_path, test_files, forbidden):
+    fileset = test_files[forbidden]
     config = load_config(fileset["config_excel"])
     matcher = Matcher(
         config["paths"],
         config["mappings"],
         SPREADSHEET_FIELDS,
         dicom_extractor,
-        {"skip_image_types": []},
         XNATFileMatch,
     )
     scanned = tmp_path / "scanned.xlsx"
     new_workbook(scanned)
     scan(
         matcher,
         Path(fileset["dir"]),
```

### Comparing `xnatuploader-1.1.6/tests/test_upload.py` & `xnatuploader-1.1.7/tests/test_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     with open(test_config, "r") as fh:
         config = json.load(fh)
         matcher = Matcher(
             config["paths"],
             config["mappings"],
             SPREADSHEET_FIELDS,
             dicom_extractor,
-            {"skip_image_types": []},
             XNATFileMatch,
         )
         anon_rules = parse_allow_fields(config["xnat"]["AllowFields"])
     project = xnat_connection.classes.ProjectData(
         parent=xnat_connection,
         name="Test_" + source_dir,
     )
@@ -120,15 +119,14 @@
     with open(basic["config"], "r") as fh:
         config = json.load(fh)
         matcher = Matcher(
             config["paths"],
             config["mappings"],
             SPREADSHEET_FIELDS,
             dicom_extractor,
-            {"skip_image_types": []},
             XNATFileMatch,
         )
         anon_rules = parse_allow_fields(config["xnat"]["AllowFields"])
     log_scanned = tmp_path / "log_scanned.xlsx"
     log_uploaded = tmp_path / "log_uploaded.xlsx"
     new_workbook(log_scanned)
     scan(matcher, Path(basic["dir"]), log_scanned)
```

