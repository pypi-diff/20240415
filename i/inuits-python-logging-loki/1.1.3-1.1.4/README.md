# Comparing `tmp/inuits-python-logging-loki-1.1.3.tar.gz` & `tmp/inuits_python_logging_loki-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits-python-logging-loki-1.1.3.tar", last modified: Fri Apr 12 09:48:06 2024, max compression
+gzip compressed data, was "inuits_python_logging_loki-1.1.4.tar", last modified: Mon Apr 15 15:13:14 2024, max compression
```

## Comparing `inuits-python-logging-loki-1.1.3.tar` & `inuits_python_logging_loki-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:48:06.850619 inuits-python-logging-loki-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-12 09:48:06.850619 inuits-python-logging-loki-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:48:06.850619 inuits-python-logging-loki-1.1.3/inuits_python_logging_loki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-12 09:48:06.000000 inuits-python-logging-loki-1.1.3/inuits_python_logging_loki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 09:48:06.000000 inuits-python-logging-loki-1.1.3/inuits_python_logging_loki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:48:06.000000 inuits-python-logging-loki-1.1.3/inuits_python_logging_loki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 09:48:06.000000 inuits-python-logging-loki-1.1.3/inuits_python_logging_loki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 09:48:06.000000 inuits-python-logging-loki-1.1.3/inuits_python_logging_loki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:48:06.846619 inuits-python-logging-loki-1.1.3/logging_loki/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/logging_loki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/logging_loki/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/logging_loki/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/logging_loki/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:48:06.850619 inuits-python-logging-loki-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:48:06.846619 inuits-python-logging-loki-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-12 09:48:02.000000 inuits-python-logging-loki-1.1.3/tests/test_emitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 15:13:14.000000 inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/logging_loki/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/logging_loki/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:13:14.696499 inuits_python_logging_loki-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-15 15:13:07.000000 inuits_python_logging_loki-1.1.4/tests/test_emitter_v1.py
```

### Comparing `inuits-python-logging-loki-1.1.3/LICENSE` & `inuits_python_logging_loki-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits-python-logging-loki-1.1.3/PKG-INFO` & `inuits_python_logging_loki-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits-python-logging-loki-1.1.3/README.md` & `inuits_python_logging_loki-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `inuits-python-logging-loki-1.1.3/inuits_python_logging_loki.egg-info/PKG-INFO` & `inuits_python_logging_loki-1.1.4/inuits_python_logging_loki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-python-logging-loki
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python logging handler for Grafana Loki.
 Author-email: Inuits <developers@inuits.eu>, Andrey Maslov <greyzmeem@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Andrey Maslov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `inuits-python-logging-loki-1.1.3/logging_loki/const.py` & `inuits_python_logging_loki-1.1.4/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `inuits-python-logging-loki-1.1.3/logging_loki/emitter.py` & `inuits_python_logging_loki-1.1.4/logging_loki/emitter.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,35 +22,37 @@
         # Prevent "recursion" when e.g. urllib3 logs debug messages on POST
         if not self._lock.acquire(blocking=False):
             return
         try:
             return method(self, *method_args, **method_kwargs)
         finally:
             self._lock.release()
+
     return _impl
 
 
 class LokiEmitter:
     """Base Loki emitter class."""
 
     success_response_code = const.success_response_code
     label_allowed_chars = const.label_allowed_chars
     label_replace_with = const.label_replace_with
     session_class = requests.Session
 
-    def __init__(self, 
-        url: str, 
-        tags: Optional[dict] = None, 
-        headers: Optional[dict] = None, 
-        auth: BasicAuth = None, 
+    def __init__(
+        self,
+        url: str,
+        tags: Optional[dict] = None,
+        headers: Optional[dict] = None,
+        auth: BasicAuth = None,
         as_json: bool = False,
         props_to_labels: Optional[list[str] | dict] = None,
         level_tag: Optional[str] = const.level_tag,
         logger_tag: Optional[str] = const.logger_tag,
-        verify: Union[bool, str] = True
+        verify: Union[bool, str] = True,
     ):
         """
         Create new Loki emitter.
 
         Arguments:
             url: Endpoint used to send log entries to Loki (e.g. `https://my-loki-instance/loki/api/v1/push`).
             tags: Default tags added to every log record.
@@ -81,20 +83,36 @@
 
     @with_lock
     def __call__(self, record: logging.LogRecord, line: str):
         """Send log record to Loki."""
         payload = self.build_payload(record, line)
         self._post_to_loki(payload)
 
+    @staticmethod
+    def convert_stream_key_values_to_string(payload):
+        """To prevent error 400 when a label isn't a string for Loki 2.9.4"""
+        if "streams" in payload:
+            for stream_data in payload["streams"]:
+                if "stream" in stream_data:
+                    stream = stream_data["stream"]
+                    for key, value in stream.items():
+                        if value is None:
+                            stream[key] = "null"
+                        elif not isinstance(value, str):
+                            stream[key] = str(stream[key])
+        return payload
+
     def _post_to_loki(self, payload: dict):
+        payload = self.convert_stream_key_values_to_string(payload)
         resp = self.session.post(self.url, json=payload, headers=self.headers)
         # TODO: Enqueue logs instead of raising an error and losing the logs
         if resp.status_code != self.success_response_code:
-            raise ValueError("Unexpected Loki API response status code: {0}".format(resp.status_code))
-
+            raise ValueError(
+                "Unexpected Loki API response status code: {0}".format(resp.status_code)
+            )
 
     @property
     def session(self) -> requests.Session:
         """Create HTTP session."""
         if self._session is None:
             self._session = self.session_class()
             self._session.auth = self.auth or None
@@ -135,34 +153,39 @@
                     if isinstance(self.props_to_labels, list):
                         extra_tags.update({k: str(prop_value)})
                     else:
                         extra_tags.update({self.props_to_labels[k]: str(prop_value)})
         if isinstance(passed_tags := getattr(record, "tags", {}), dict):
             extra_tags = extra_tags | passed_tags
 
-        
         for tag_name, tag_value in extra_tags.items():
             cleared_name = self.format_label(tag_name)
             if cleared_name:
                 tags[cleared_name] = tag_value
 
         return tags
 
     def build_payload(self, record: logging.LogRecord, line: str) -> dict:
         """Build JSON payload with a log entry."""
         labels = self.build_tags(record, line)
         ns = 1e9
         ts = str(int(time.time() * ns))
 
-        line = json.dumps(record, default=lambda obj: obj.__dict__) if self.as_json else line
+        line = (
+            json.dumps(record, default=lambda obj: obj.__dict__)
+            if self.as_json
+            else line
+        )
 
         stream = {
             "stream": labels,
             "values": [[ts, line]],
         }
         return {"streams": [stream]}
-    
+
     @with_lock
     def emit_batch(self, records: list[Tuple[logging.LogRecord, str]]):
         """Send log records to Loki."""
-        streams = [self.build_payload(record[0], record[1])["streams"][0] for record in records]
+        streams = [
+            self.build_payload(record[0], record[1])["streams"][0] for record in records
+        ]
         self._post_to_loki({"streams": streams})
```

### Comparing `inuits-python-logging-loki-1.1.3/logging_loki/handlers.py` & `inuits_python_logging_loki-1.1.4/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `inuits-python-logging-loki-1.1.3/pyproject.toml` & `inuits_python_logging_loki-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inuits-python-logging-loki"
-version = "1.1.3"
+version = "1.1.4"
 description = "Python logging handler for Grafana Loki."
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }, {name="Andrey Maslov", email="greyzmeem@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `inuits-python-logging-loki-1.1.3/tests/test_emitter_v1.py` & `inuits_python_logging_loki-1.1.4/tests/test_emitter_v1.py`

 * *Files identical despite different names*

