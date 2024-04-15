# Comparing `tmp/t_bug_catcher-0.4.2.tar.gz` & `tmp/t_bug_catcher-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-956qxe83/t_bug_catcher-0.4.2.tar", last modified: Wed Apr 10 13:16:11 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-5govxv9y/t_bug_catcher-0.4.3.tar", last modified: Mon Apr 15 11:02:43 2024, max compression
```

## Comparing `t_bug_catcher-0.4.2.tar` & `t_bug_catcher-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-10 13:16:11.299898 t_bug_catcher-0.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.291898 t_bug_catcher-0.4.2/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    44739 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/t_bug_catcher/resources/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/resources/whispers_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    45412 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-15 11:02:43.000000 t_bug_catcher-0.4.3/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 11:02:43.737404 t_bug_catcher-0.4.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-15 11:02:18.000000 t_bug_catcher-0.4.3/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.2/PKG-INFO` & `t_bug_catcher-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.2
+Version: 0.4.3
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.2/README.rst` & `t_bug_catcher-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.2/setup.py` & `t_bug_catcher-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.4.2",
+    version="0.4.3",
     zip_safe=False,
     install_requires=install_requirements,
     include_package_data=True,
     package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.3/t_bug_catcher/bug_catcher.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.3/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/config.py` & `t_bug_catcher-0.4.3/t_bug_catcher/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 
         MAX_ATTACHMENTS: int = 5
         MAX_ISSUE_ATTACHMENTS: int = 100
         MAX_DESCRIPTION_LENGTH: int = 250
         SUMMARY_LENGTH: int = 120
         STACK_SCOPE: int = 3
 
+    class TICKET_PRIORITIES:
+        """Priorities class for configuring the application."""
+
+        HIGHEST: str = "1"
+        HIGH: str = "2"
+        MEDIUM: str = "3"
+        LOW: str = "4"
+        LOWEST: str = "5"
+
     SUPPORT_BOARD = "AB"
 
     KEYS_TO_REMOVE = ["credential", "password"]
 
     RC_RUN_LINK = (
         f"https://cloud.robocorp.com/organizations/{os.environ.get('RC_ORGANIZATION_ID')}"
         f"/workspaces/{os.environ.get('RC_WORKSPACE_ID')}/processes"
```

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.3/t_bug_catcher/jira.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,23 +205,25 @@
     def __generate_issue_body(
         self,
         summary: str,
         description: dict,
         issue_type: str,
         assignee: Optional[str] = None,
         labels: Optional[list] = None,
+        priority: Optional[str] = None,
     ) -> str:
         """Generates the issue body payload for creating a new issue.
 
         Args:
             summary (str): The summary of the issue.
             description (dict): The description of the issue.
             assignee (str): The assignee of the issue.
             issue_type (str): The type of the issue.
             labels (list, optional): The labels of the issue. Defaults to None.
+            priority (str, optional): The priority of the issue. Defaults to None.
 
         Returns:
             The JSON payload for creating a new issue.
         """
         fields = {
             "fields": {
                 "assignee": {"id": assignee if assignee else "-1"},
@@ -231,14 +233,16 @@
                 "summary": summary,
             },
         }
         if labels:
             fields["fields"]["labels"] = labels
         if self._project_key == CONFIG.SUPPORT_BOARD and CONFIG.ADMIN_CODE:
             fields["fields"]["customfield_10077"] = [CONFIG.ADMIN_CODE]
+        if priority:
+            fields["fields"]["priority"] = {"id": priority}
         payload = json.dumps(fields)
         return payload
 
     def move_ticket_to_board(self, ticket_id: str) -> None:
         """Move a ticket to a board using its ID.
 
         Args:
@@ -886,23 +890,25 @@
     def __create_new_ticket(
         self,
         summary: str,
         description: dict,
         assignee_id: Optional[str] = None,
         attachments: Optional[List] = None,
         labels: Optional[list] = None,
+        priority: Optional[str] = None,
     ) -> requests.Response:
         """Create a new ticket.
 
         Args:
             summary (str): The summary of the ticket.
             description (dict): The description of the ticket.
             assignee_id (str, optional): The assignee of the ticket. Defaults to None.
             attachments (List, optional): The list of attachments. Defaults to None.
             labels (List, optional): The list of labels. Defaults to None.
+            priority (str, optional): The priority of the ticket. Defaults to None.
 
         Returns:
             The response from creating the ticket.
         """
         if CONFIG.STAGE.lower() == "hypercare":
             issue_type = self._issue_types.get("hypercare") or self._issue_types.get("epic")
         elif CONFIG.STAGE.lower() == "support":
@@ -919,23 +925,25 @@
 
         issue = self.__generate_issue_body(
             summary=summary[:255].split("\n")[0],
             description=description,
             assignee=assignee_id,
             issue_type=issue_type,
             labels=labels,
+            priority=priority,
         )
         response = self.post_ticket(issue=issue)
 
         if response.json().get("errors", {}).get("labels"):
             issue = self.__generate_issue_body(
                 summary=summary[:255].split("\n")[0],
                 description=description,
                 assignee=assignee_id,
                 issue_type=issue_type,
+                priority=priority,
             )
             response = self.post_ticket(issue=issue)
 
         if response.status_code != 201:
             logger.warning(
                 f"Failed to create Jira issue. Status code: {response.status_code}"
                 f" Error messages: {', '.join(response.json()['errorMessages'])}"
@@ -1030,20 +1038,23 @@
                 exc_value=exception,
                 exc_traceback=exception.__traceback__,
                 error_id=error_id,
                 additional_info=additional_info,
                 metadata=metadata,
             )
 
+            priority = CONFIG.TICKET_PRIORITIES.HIGH if CONFIG.STAGE.lower() == "hypercare" else None
+
             response = self.__create_new_ticket(
                 summary=summary,
                 description=description,
                 assignee_id=assignee_id,
                 attachments=attachments,
                 labels=["bug_catcher"],
+                priority=priority,
             )
             if os.path.exists(stack_trace):
                 os.remove(stack_trace)
             return response
         except Exception as ex:
             logger.warning(f"Failed to create Jira issue due to: {ex.__class__.__name__}: {ex}")
             return False
@@ -1087,20 +1098,23 @@
             description = self.__create_description_markup(
                 exc_type=exc_type,
                 exc_value=exc_value,
                 exc_traceback=exc_traceback,
                 error_id=error_id,
             )
 
+            priority = CONFIG.TICKET_PRIORITIES.HIGHEST if CONFIG.STAGE.lower() == "hypercare" else None
+
             response = self.__create_new_ticket(
                 summary=summary,
                 description=description,
                 assignee_id=assignee_id,
                 attachments=[stack_trace] if stack_trace else None,
                 labels=["bug_catcher", "fatal_error"],
+                priority=priority,
             )
             if os.path.exists(stack_trace):
                 os.remove(stack_trace)
             return response
         except Exception as ex:
             logger.warning(f"Failed to create Jira issue due to: {ex.__class__.__name__}: {ex}")
             return False
```

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/resources/whispers_config.yml` & `t_bug_catcher-0.4.3/t_bug_catcher/resources/whispers_config.yml`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.4.3/t_bug_catcher/stack_saver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import json
+import linecache
 import os
 import re
 import sys
 from datetime import datetime
 from pathlib import Path
 from types import FunctionType, ModuleType
 from typing import Optional
@@ -44,14 +45,16 @@
             dict: The serialized frame info.
         """
         run_locals = convert_keys_to_primitives(frame_info["locals"]) if frame_info["locals"] else {}
         run_args = convert_keys_to_primitives(frame_info["args"]) if frame_info["args"] else {}
         serializable_frame_info = {
             "filename": frame_info["filename"],
             "function_name": frame_info["function_name"],
+            "line_number": frame_info["line_number"],
+            "line": frame_info["line"],
             "locals": run_locals,
             "args": run_args,
         }
         return serializable_frame_info
 
     @staticmethod
     def filter_variables(variables: dict) -> dict:
@@ -122,28 +125,35 @@
 
         Returns:
             Optional[str]: The path of the saved stack trace.
         """
         try:
             frames = []
             stack_details_json = []
+            seen_frames = set()
             tb = exception.__traceback__ if exception else sys.exc_info()[2]
             while tb is not None:
                 frame = tb.tb_frame
+                if frame.f_code.co_name in seen_frames:
+                    tb = tb.tb_next
+                    continue
+                seen_frames.add(frame.f_code.co_name)
                 if "site-packages" in frame.f_code.co_filename:
                     tb = tb.tb_next
                     continue
                 frames.append(frame)
                 tb = tb.tb_next
             frames = frames[-CONFIG.LIMITS.STACK_SCOPE :]
 
             for frame in frames:
                 frame_info = {
                     "filename": self.strip_path(frame.f_code.co_filename),
                     "function_name": frame.f_code.co_name,
+                    "line_number": frame.f_lineno,
+                    "line": linecache.getline(frame.f_code.co_filename, frame.f_lineno).strip(),
                     "locals": self.filter_variables(frame.f_locals),
                     "args": self.filter_variables(inspect.getargvalues(frame)[3]),
                 }
                 stack_details_json.append(self.serialize_frame_info(frame_info))
 
             file_path = f"stack_details_{datetime.now().strftime('%Y%m%d%H%M%S')}.json"
```

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/utils/common.py` & `t_bug_catcher-0.4.3/t_bug_catcher/utils/common.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.3/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.3/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.2
+Version: 0.4.3
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.2/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.3/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.2/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.3/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

