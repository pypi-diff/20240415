# Comparing `tmp/pih-plb_rw_ntf-0.13.tar.gz` & `tmp/pih-plb_rw_ntf-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_rw_ntf-0.13.tar", last modified: Wed Apr 10 02:24:23 2024, max compression
+gzip compressed data, was "pih-plb_rw_ntf-0.14.tar", last modified: Mon Apr 15 00:29:18 2024, max compression
```

## Comparing `pih-plb_rw_ntf-0.13.tar` & `pih-plb_rw_ntf-0.14.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 02:24:23.785639 pih-plb_rw_ntf-0.13/
--rw-rw-rw-   0        0        0      302 2024-04-10 02:24:23.753311 pih-plb_rw_ntf-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 02:24:23.358940 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/__init__.py
--rw-rw-rw-   0        0        0      174 2024-02-15 00:20:05.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/__main__.py
--rw-rw-rw-   0        0        0     2508 2024-03-13 12:29:09.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/api.py
--rw-rw-rw-   0        0        0      579 2024-04-10 02:23:34.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/const.py
--rw-rw-rw-   0        0        0     8481 2024-04-10 00:36:48.000000 pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-10 02:24:23.722058 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/
--rw-rw-rw-   0        0        0      302 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2024-04-10 02:24:23.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       40 2024-04-10 02:24:22.000000 pih-plb_rw_ntf-0.13/pih_plb_rw_ntf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 02:24:23.801262 pih-plb_rw_ntf-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 00:29:18.444122 pih-plb_rw_ntf-0.14/
+-rw-rw-rw-   0        0        0      302 2024-04-15 00:29:18.365993 pih-plb_rw_ntf-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 00:29:17.918960 pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-02-15 00:20:05.000000 pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/__main__.py
+-rw-rw-rw-   0        0        0     2508 2024-03-13 12:29:09.000000 pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/api.py
+-rw-rw-rw-   0        0        0      579 2024-04-15 00:03:20.000000 pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/const.py
+-rw-rw-rw-   0        0        0     8488 2024-04-15 00:03:15.000000 pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:29:18.319121 pih-plb_rw_ntf-0.14/pih_plb_rw_ntf.egg-info/
+-rw-rw-rw-   0        0        0      302 2024-04-15 00:29:17.000000 pih-plb_rw_ntf-0.14/pih_plb_rw_ntf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      480 2024-04-15 00:29:17.000000 pih-plb_rw_ntf-0.14/pih_plb_rw_ntf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:29:17.000000 pih-plb_rw_ntf-0.14/pih_plb_rw_ntf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-15 00:29:17.000000 pih-plb_rw_ntf-0.14/pih_plb_rw_ntf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-15 00:29:17.000000 pih-plb_rw_ntf-0.14/pih_plb_rw_ntf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       40 2024-04-15 00:29:17.000000 pih-plb_rw_ntf-0.14/pih_plb_rw_ntf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:29:18.444122 pih-plb_rw_ntf-0.14/setup.cfg
```

### Comparing `pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/api.py` & `pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/api.py`

 * *Files identical despite different names*

### Comparing `pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/const.py` & `pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibasePersonReviewNotification"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 SD: ServiceDescription = ServiceDescription(
        name=NAME,
        description="Polibase Person Review Notification service",
        host=HOST.NAME,
        use_standalone=True,
        version=VERSION,
```

### Comparing `pih-plb_rw_ntf-0.13/PolibasePersonReviewNotificationService/service.py` & `pih-plb_rw_ntf-0.14/PolibasePersonReviewNotificationService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import ipih
 
 from pih import A, PIHThread
-from pih.collections import EventDS
-from PolibasePersonReviewNotificationService.api import (
-    PolibasePersonReviewNotificationApi as Api,
-)
 from PolibasePersonReviewNotificationService.const import SD
-from pih.tools import j, nn, ne, one, FullNameTool, ParameterList
-
 
 SC = A.CT_SC
 
 ISOLATED: bool = False
 
+
 def start(as_standalone: bool = False) -> None:
     from datetime import datetime
     from pih.consts.errors import NotFound
     from pih.collections import (
+        EventDS,
         Message,
         PolibasePerson,
         WhatsAppMessage,
         PolibasePersonNotificationConfirmation as PPNC,
     )
+    from PolibasePersonReviewNotificationService.api import (
+        PolibasePersonReviewNotificationApi as Api,
+    )
+    from pih.tools import j, nn, ne, one, esc, FullNameTool, ParameterList
 
     SENDER: str = A.D.get(A.CT_ME_WH_W.Profiles.MARKETER)
 
     def service_call_handler(sc: SC, pl: ParameterList) -> bool | None:
         if sc == SC.heart_beat:
             heat_beat_handler(A.D_Ex.parameter_list(pl).get())
             return True
@@ -125,15 +125,15 @@
                                                     )
                                                 )
 
                                             A.E.send(
                                                 A.CT_E.POLIBASE_PERSON_REVIEW_NOTIFICATION_WAS_ANSWERED,
                                                 (
                                                     person.pin,
-                                                    message_text,
+                                                    esc(message_text),
                                                     int(answer_yes),
                                                 ),
                                             )
                             except NotFound as error:
                                 A.L.debug_bot(
                                     j((SD.standalone_name, ": ", error.get_details()))
                                 )
```

