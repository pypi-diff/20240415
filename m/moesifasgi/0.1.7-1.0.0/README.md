# Comparing `tmp/moesifasgi-0.1.7.tar.gz` & `tmp/moesifasgi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moesifasgi-0.1.7.tar", last modified: Fri Jan 12 02:39:26 2024, max compression
+gzip compressed data, was "moesifasgi-1.0.0.tar", last modified: Mon Apr 15 17:34:30 2024, max compression
```

## Comparing `moesifasgi-0.1.7.tar` & `moesifasgi-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,21 @@
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/
--rw-rw-r--   0 praveen    (501) staff       (20)    11908 2021-12-23 21:51:46.000000 moesifasgi-0.1.7/LICENSE
--rw-rw-r--   0 praveen    (501) staff       (20)       61 2021-12-23 21:51:46.000000 moesifasgi-0.1.7/MANIFEST.in
--rw-r--r--   0 praveen    (501) staff       (20)    13732 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/PKG-INFO
--rw-r--r--   0 praveen    (501) staff       (20)    12564 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/README.md
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/moesifasgi/
--rw-rw-r--   0 praveen    (501) staff       (20)       26 2021-12-23 21:51:46.000000 moesifasgi-0.1.7/moesifasgi/__init__.py
--rw-r--r--   0 praveen    (501) staff       (20)     2320 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/app_config.py
--rw-rw-r--   0 praveen    (501) staff       (20)      301 2021-12-23 21:51:46.000000 moesifasgi-0.1.7/moesifasgi/async_iterator_wrapper.py
--rw-r--r--   0 praveen    (501) staff       (20)     4843 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/client_ip.py
--rw-r--r--   0 praveen    (501) staff       (20)     3848 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/event_mapper.py
--rw-r--r--   0 praveen    (501) staff       (20)     8813 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/logger_helper.py
--rw-r--r--   0 praveen    (501) staff       (20)    11991 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/middleware.py
--rw-rw-r--   0 praveen    (501) staff       (20)     1159 2021-12-23 21:51:46.000000 moesifasgi-0.1.7/moesifasgi/parse_body.py
--rw-r--r--   0 praveen    (501) staff       (20)     2218 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/send_batch_events.py
--rw-r--r--   0 praveen    (501) staff       (20)     6835 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/update_companies.py
--rw-r--r--   0 praveen    (501) staff       (20)     6498 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/moesifasgi/update_users.py
-drwxr-xr-x   0 praveen    (501) staff       (20)        0 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/moesifasgi.egg-info/
--rw-r--r--   0 praveen    (501) staff       (20)    13732 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/moesifasgi.egg-info/PKG-INFO
--rw-rw-r--   0 praveen    (501) staff       (20)      521 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/moesifasgi.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen    (501) staff       (20)        1 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/moesifasgi.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen    (501) staff       (20)       86 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/moesifasgi.egg-info/requires.txt
--rw-rw-r--   0 praveen    (501) staff       (20)       11 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/moesifasgi.egg-info/top_level.txt
--rw-rw-r--   0 praveen    (501) staff       (20)       67 2024-01-12 02:39:26.000000 moesifasgi-0.1.7/setup.cfg
--rw-r--r--   0 praveen    (501) staff       (20)     3339 2024-01-12 01:35:11.000000 moesifasgi-0.1.7/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-15 17:34:30.564603 moesifasgi-1.0.0/
+-rw-r--r--   0 keyur      (501) staff       (20)    11908 2021-08-28 00:36:27.000000 moesifasgi-1.0.0/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2021-08-28 00:36:31.000000 moesifasgi-1.0.0/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-04-15 17:34:30.564771 moesifasgi-1.0.0/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)    12564 2024-01-10 01:16:32.000000 moesifasgi-1.0.0/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-15 17:34:30.562479 moesifasgi-1.0.0/moesifasgi/
+-rw-r--r--   0 keyur      (501) staff       (20)       26 2024-04-15 15:48:48.000000 moesifasgi-1.0.0/moesifasgi/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)      301 2021-08-28 00:35:10.000000 moesifasgi-1.0.0/moesifasgi/async_iterator_wrapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4843 2024-03-29 23:20:02.000000 moesifasgi-1.0.0/moesifasgi/client_ip.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3592 2024-04-15 17:25:00.000000 moesifasgi-1.0.0/moesifasgi/event_mapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     9087 2024-04-15 17:25:00.000000 moesifasgi-1.0.0/moesifasgi/logger_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)    11096 2024-04-15 17:25:00.000000 moesifasgi-1.0.0/moesifasgi/middleware.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2218 2024-03-29 23:20:02.000000 moesifasgi-1.0.0/moesifasgi/send_batch_events.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-15 17:34:30.564367 moesifasgi-1.0.0/moesifasgi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-04-15 17:34:30.000000 moesifasgi-1.0.0/moesifasgi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)      413 2024-04-15 17:34:30.000000 moesifasgi-1.0.0/moesifasgi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2024-04-15 17:34:30.000000 moesifasgi-1.0.0/moesifasgi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       82 2024-04-15 17:34:30.000000 moesifasgi-1.0.0/moesifasgi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       11 2024-04-15 17:34:30.000000 moesifasgi-1.0.0/moesifasgi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2024-04-15 17:34:30.565501 moesifasgi-1.0.0/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3269 2024-04-15 17:25:00.000000 moesifasgi-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `moesifasgi-0.1.7/LICENSE` & `moesifasgi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifasgi-0.1.7/PKG-INFO` & `moesifasgi-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: moesifasgi
-Version: 0.1.7
+Version: 1.0.0
 Summary: Moesif Middleware for Python ASGI based platforms (FastAPI & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-asgi/
 Author: Moesif, Inc
 Author-email: keyur@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug asgi fastapi http middleware
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Moesif Middleware for Python ASGI based Frameworks
```

### Comparing `moesifasgi-0.1.7/README.md` & `moesifasgi-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `moesifasgi-0.1.7/moesifasgi/client_ip.py` & `moesifasgi-1.0.0/moesifasgi/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-0.1.7/moesifasgi/event_mapper.py` & `moesifasgi-1.0.0/moesifasgi/event_mapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from moesifapi.models import *
-from .parse_body import ParseBody
+from moesifapi.parse_body import ParseBody
 from .logger_helper import LoggerHelper
 from .client_ip import ClientIp
-from datetime import datetime
 import uuid
 
 
 class EventMapper:
     def __init__(self):
         self.parse_body = ParseBody()
         self.logger_helper = LoggerHelper()
         self.client_ip = ClientIp()
         self.transaction_id = None
 
-    async def to_event(self, request, response, event_req, event_rsp, moesif_settings, debug):
+    async def to_event(self, event_req, event_rsp, user_id, company_id, session_token, metadata, blocked_by):
         return EventModel(request=event_req,
                           response=event_rsp,
-                          user_id=await self.logger_helper.get_user_id(moesif_settings, request, response, dict(request.headers), debug),
-                          company_id=await self.logger_helper.get_company_id(moesif_settings, request, response, debug),
-                          session_token=await self.logger_helper.get_session_token(moesif_settings, request, response, debug),
-                          metadata=await self.logger_helper.get_metadata(moesif_settings, request, response, debug),
-                          direction="Incoming")
+                          user_id=user_id,
+                          company_id=company_id,
+                          session_token=session_token,
+                          metadata=metadata,
+                          direction="Incoming",
+                          blocked_by=blocked_by)
 
     def to_request(self, request, request_time, request_body, api_version, disable_capture_transaction_id, debug=False):
         # Request URI
         request_uri = request.url._url
         # Request Verb
         request_verb = request.method
         # Request Headers
@@ -42,15 +42,15 @@
                 request_headers["X-Moesif-Transaction-Id"] = self.transaction_id
         # Request Ip address
         request_ip_address = self.client_ip.get_client_address(request_headers, request.client.host, debug)
         # Request Body
         req_body = None
         req_transfer_encoding = None
         if request_body:
-            req_body, req_transfer_encoding = self.parse_body.parse_bytes_body(request_body, request_headers)
+            req_body, req_transfer_encoding = self.parse_body.parse_bytes_body(request_body, None, request_headers)
 
         return EventRequestModel(time=request_time,
                                  uri=request_uri,
                                  verb=request_verb,
                                  api_version=api_version,
                                  ip_address=request_ip_address,
                                  headers=request_headers,
@@ -70,14 +70,14 @@
         rsp_transfer_encoding = None
         if response_body:
             try:
                 rsp_body = response_body[0]
             except Exception as e:
                 rsp_body = str(response_body)
 
-            rsp_body, rsp_transfer_encoding = self.parse_body.parse_bytes_body(rsp_body, response_headers)
+            rsp_body, rsp_transfer_encoding = self.parse_body.parse_bytes_body(rsp_body, None, response_headers)
 
         return EventResponseModel(time=response_time,
                                   status=response_status,
                                   headers=response_headers,
                                   body=rsp_body,
                                   transfer_encoding=rsp_transfer_encoding)
```

### Comparing `moesifasgi-0.1.7/moesifasgi/logger_helper.py` & `moesifasgi-1.0.0/moesifasgi/logger_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import inspect
 import json
 import base64
 import logging
+import re
 
 logger = logging.getLogger(__name__)
 
 
 class LoggerHelper:
 
     def __init__(self):
         pass
+    @classmethod
+    def sanitize_header_value(cls, value):
+        # Remove any non-printable characters
+        value = re.sub(r'[^\x20-\x7E]', '', value)
+        # Replace any spaces with underscores
+        value = value.replace(' ', '_')
+        return value
 
     @classmethod
     def transform_token(cls, token):
         if not isinstance(token, str):
             token = token.decode('utf-8')
         return token
```

### Comparing `moesifasgi-0.1.7/moesifasgi/middleware.py` & `moesifasgi-1.0.0/moesifasgi/middleware.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,111 @@
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.requests import Request
-from datetime import datetime, timedelta
+from datetime import datetime
 from moesifapi.moesif_api_client import *
-from .send_batch_events import SendEventAsync
-from .app_config import AppConfig
+from moesifapi.app_config import AppConfig
 from .async_iterator_wrapper import async_iterator_wrapper
 from .logger_helper import LoggerHelper
-from .parse_body import ParseBody
 from .event_mapper import EventMapper
-from .update_companies import Company
-from .update_users import User
-from apscheduler.schedulers.background import BackgroundScheduler
-from apscheduler.triggers.interval import IntervalTrigger
-from apscheduler.events import EVENT_JOB_ERROR, EVENT_JOB_EXECUTED
+from moesifapi.update_companies import Company
+from moesifapi.update_users import User
+from starlette.middleware.base import _StreamingResponse
 from moesifpythonrequest.start_capture.start_capture import StartCapture
+from moesifapi.config_manager import ConfigUpdateManager
+from moesifapi.workers import BatchedWorkerPool, ConfigJobScheduler
 from starlette.types import Message
 from importlib.metadata import version
 from distutils.version import LooseVersion
-import logging
 import math
 import random
-import queue
-import atexit
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class MoesifMiddleware(BaseHTTPMiddleware):
     """ASGI Middleware for recording of request-response"""
     def __init__(self, settings=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
        
         if settings is None:
             raise Exception('Moesif Application ID is required in settings')
-        self.moesif_settings = settings
-       
-        if self.moesif_settings.get('APPLICATION_ID', None):
-            self.client = MoesifAPIClient(self.moesif_settings.get('APPLICATION_ID'))
-        else:
-            raise Exception('Moesif Application ID is required in settings')
-        self.DEBUG = self.moesif_settings.get('DEBUG', False)
-        if self.DEBUG:
-            Configuration.BASE_URI = self.moesif_settings.get('BASE_URI', 'https://api.moesif.net')
-        Configuration.version = 'moesifasgi-python/0.1.5'
-        if self.moesif_settings.get('CAPTURE_OUTGOING_REQUESTS', False):
+        self.settings = settings
+        self.DEBUG = self.settings.get('DEBUG', False)
+
+        self.initialize_logger()
+        self.validate_settings()
+
+        self.initialize_counter()
+        self.initialize_client()
+        self.initialize_config()
+        self.initialize_worker_pool()
+
+        if self.settings.get('CAPTURE_OUTGOING_REQUESTS', False):
             try:
                 if self.DEBUG:
                     logger.info('Start capturing outgoing requests')
                 # Start capturing outgoing requests
-                StartCapture().start_capture_outgoing(self.moesif_settings)
+                StartCapture().start_capture_outgoing(self.settings)
             except:
                 logger.warning('Error while starting to capture the outgoing events')
-        self.api_client = self.client.api
-        self.app_config = AppConfig()
-        self.send_async_events = SendEventAsync()
+
+        self.disable_transaction_id = self.settings.get('DISABLED_TRANSACTION_ID', False)
+        self.starlette_version = version('starlette')
+
+    def initialize_logger(self):
+        """Initialize logger mirroring the debug and stdout behavior of previous print statements for compatibility"""
+        logging.basicConfig(
+            level=logging.DEBUG if self.DEBUG else logging.INFO,
+            format='%(asctime)s\t%(levelname)s\tPID: %(process)d\tThread: %(thread)d\t%(funcName)s\t%(message)s',
+            handlers=[logging.StreamHandler()]
+        )
+
+    def validate_settings(self):
+        if self.settings is None or not self.settings.get("APPLICATION_ID", None):
+            raise Exception("Moesif Application ID is required in settings")
+    def initialize_counter(self):
+        self.dropped_events = 0
         self.logger_helper = LoggerHelper()
-        self.parse_body = ParseBody()
         self.event_mapper = EventMapper()
-        self.sampling_percentage = 100
-        self.last_updated_time = datetime.utcnow()
-        self.disable_transaction_id = self.moesif_settings.get('DISABLED_TRANSACTION_ID', False)
-        self.event_queue_size = self.moesif_settings.get('EVENT_QUEUE_SIZE', 1000000)
-        self.moesif_events_queue = queue.Queue(maxsize=self.event_queue_size)
-        self.BATCH_SIZE = self.moesif_settings.get('BATCH_SIZE', 25)
-        self.last_event_job_run_time = datetime(1970, 1, 1, 0, 0)  # Assuming job never ran, set it to epoch start time
-        self.scheduler = None
-        self.config_etag = None
-        self.config = self.app_config.get_config(self.api_client, self.DEBUG)
-        self.is_event_job_scheduled = False
-        self.api_version = self.moesif_settings.get('API_VERSION')
-        self.LOG_BODY = self.moesif_settings.get('LOG_BODY', True)
-        self.starlette_version = version('starlette')
+
+    def initialize_client(self):
+        self.api_version = self.settings.get("API_VERSION")
+        self.client = MoesifAPIClient(self.settings.get("APPLICATION_ID"))
+        self.api_client = self.client.api
+
+    def schedule_config_job(self):
         try:
-            if self.config:
-                self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
-                    self.config, self.DEBUG)
+            ConfigJobScheduler(self.DEBUG, self.config).schedule_background_job()
+            self.is_config_job_scheduled = True
         except Exception as ex:
+            self.is_config_job_scheduled = False
             if self.DEBUG:
-                logger.info(f'Error while parsing application configuration on initialization:{str(ex)}')
+                logger.info(f'Error while starting the config scheduler job in background: {str(ex)}')
 
-    # Function to listen to the send event job response
-    def moesif_event_listener(self, event):
-        if event.exception:
-            if self.DEBUG:
-                logger.info('Error reading response from the scheduled job')
-        else:
-            if event.retval:
-                response_etag, self.last_event_job_run_time = event.retval
-                if response_etag is not None \
-                    and self.config_etag is not None \
-                    and self.config_etag != response_etag \
-                        and datetime.utcnow() > self.last_updated_time + timedelta(minutes=5):
-                    try:
-                        self.config = self.app_config.get_config(self.api_client, self.DEBUG)
-                        self.config_etag, self.sampling_percentage, self.last_updated_time = self.app_config.parse_configuration(
-                            self.config, self.DEBUG)
-                    except Exception as ex:
-                        if self.DEBUG:
-                            logger.info(f'Error while updating the application configuration: {str(ex)}')
+    def initialize_config(self):
+        Configuration.BASE_URI = self.settings.get("BASE_URI", "https://api.moesif.net")
+        Configuration.version = 'moesifasgi-python/1.0.0'
+        self.LOG_BODY = self.settings.get("LOG_BODY", True)
 
-    def schedule_background_job(self):
-        try:
-            if not self.scheduler:
-                self.scheduler = BackgroundScheduler(daemon=True)
-            if not self.scheduler.get_jobs():
-                self.scheduler.add_listener(self.moesif_event_listener, EVENT_JOB_EXECUTED | EVENT_JOB_ERROR)
-                self.scheduler.start()
-                self.scheduler.add_job(
-                    func=lambda: self.send_async_events.batch_events(self.api_client, self.moesif_events_queue,
-                                                                     self.DEBUG, self.BATCH_SIZE),
-                    trigger=IntervalTrigger(seconds=2),
-                    id='moesif_events_batch_job',
-                    name='Schedule events batch job every 2 second',
-                    replace_existing=True)
-
-                # Avoid passing logging message to the ancestor loggers
-                logging.getLogger('apscheduler.executors.default').setLevel(logging.WARNING)
-                logging.getLogger('apscheduler.executors.default').propagate = False
+        self.app_config = AppConfig()
+        self.config = ConfigUpdateManager(self.api_client, self.app_config, self.DEBUG)
+        self.schedule_config_job()
 
-                # Exit handler when exiting the app
-                atexit.register(lambda: self.send_async_events.exit_handler(self.scheduler, self.DEBUG))
-        except Exception as ex:
-            if self.DEBUG:
-                logger.info(f"Error when scheduling the job: {str(ex)}")
+    def initialize_worker_pool(self):
+        # Create queues and threads which will batch and send events in the background
+        self.worker_pool = BatchedWorkerPool(
+            worker_count=self.settings.get("EVENT_WORKER_COUNT", 2),
+            api_client=self.api_client,
+            config=self.config,
+            debug=self.DEBUG,
+            max_queue_size=self.settings.get("EVENT_QUEUE_SIZE", 1000000),
+            batch_size=self.settings.get("BATCH_SIZE", 100),
+            timeout=self.settings.get("EVENT_BATCH_TIMEOUT", 1),
+        )
 
     def update_user(self, user_profile):
         User().update_user(user_profile, self.api_client, self.DEBUG)
 
     def update_users_batch(self, user_profiles):
         User().update_users_batch(user_profiles, self.api_client, self.DEBUG)
 
@@ -151,90 +129,118 @@
             self.set_body(request, body)
         return body
 
     @classmethod
     def get_time(cls):
         return datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3]
 
+    # Prepare response for the governance rule
+    def prepare_response_content(self, body):
+        response_content = None
+        try:
+            response_content = body[0]
+        except Exception as ex:
+            if self.DEBUG:
+                logger.info(f"Error while preparing the response content: {str(ex)}")
+        return response_content
+
     async def dispatch(self, request, call_next):
         # request time
         request_time = self.get_time()
         if self.DEBUG:
             logger.info(f"event request time: {str(request_time)}")
 
         # Read Request Body
         request_body = None
         if self.LOG_BODY:
             request_body = await self.get_body(request)
 
-        # Call the next middleware
-        response = await call_next(request)
+        # Prepare Event Request Model
+        event_req = self.event_mapper.to_request(request, request_time, request_body, self.api_version,
+                                                 self.disable_transaction_id, self.DEBUG)
+
+        governed_response = {}
+        if self.config.have_governance_rules():
+            # we must fire these hooks early.
+            user_id = await self.logger_helper.get_user_id(self.settings, request, None, dict(request.headers), self.DEBUG)
+            company_id = await self.logger_helper.get_company_id(self.settings, request, None, self.DEBUG)
+            governed_response = self.config.govern_request(event_req, user_id, company_id, event_req.body)
+
+        blocked_by = None
+        if 'blocked_by' in governed_response:
+            # start response immediately, skip next step
+            response_content = self.prepare_response_content(governed_response['body'])
+            blocked_by = governed_response['blocked_by']
+            async def generate_data():
+                yield response_content
+            headers = {k: self.logger_helper.sanitize_header_value(v) for k, v in governed_response['headers'].items() }
+            response = _StreamingResponse(content=generate_data(), status_code=governed_response['status'], headers=headers)
+        else:
+            # Call the next middleware
+            response = await call_next(request)
 
         # response time
         response_time = self.get_time()
         if self.DEBUG:
             logger.info(f"event response time: {str(response_time)}")
 
-        skip = await self.logger_helper.should_skip(self.moesif_settings, request, response, self.DEBUG)
-        if not skip:
-            random_percentage = random.random() * 100
-
-            self.sampling_percentage = self.app_config.get_sampling_percentage(self.config,
-                                                                               await self.logger_helper.get_user_id(self.moesif_settings, request, response, request.headers, self.DEBUG),
-                                                                               await self.logger_helper.get_company_id(self.moesif_settings, request, response, self.DEBUG))
-
-            if self.sampling_percentage >= random_percentage:
-                # Prepare Event Request Model
-                event_req = self.event_mapper.to_request(request, request_time, request_body, self.api_version, self.disable_transaction_id, self.DEBUG)
-
-                # Read Response Body
-                resp_body = None
-                if self.LOG_BODY:
-                    # Consuming FastAPI response and grabbing body here
-                    resp_body = [section async for section in response.__dict__['body_iterator']]
-                    # Preparing FastAPI response
-                    response.__setattr__('body_iterator', async_iterator_wrapper(resp_body))
-
-                # Prepare Event Response Model
-                event_rsp = self.event_mapper.to_response(response, response_time, resp_body)
-                # Prepare Event Model
-                event_data = await self.event_mapper.to_event(request, response, event_req, event_rsp, self.moesif_settings,
-                                                         self.DEBUG)
-
-                # Mask Event Model
-                if self.logger_helper.is_coroutine_function(self.logger_helper.mask_event):
-                    event_data = await self.logger_helper.mask_event(event_data, self.moesif_settings, self.DEBUG)
-                else:
-                    event_data = self.logger_helper.mask_event(event_data, self.moesif_settings, self.DEBUG)
-
-                if event_data:
-                    # Add Weight to the event
-                    event_data.weight = 1 if self.sampling_percentage == 0 else math.floor(100 / self.sampling_percentage)
-                    try:
-                        if not self.is_event_job_scheduled and datetime.utcnow() > self.last_event_job_run_time + timedelta(
-                                minutes=5):
-                            try:
-                                self.schedule_background_job()
-                                self.is_event_job_scheduled = True
-                                self.last_event_job_run_time = datetime.utcnow()
-                            except Exception as ex:
-                                self.is_event_job_scheduled = False
-                                if self.DEBUG:
-                                    logger.info(f'Error while starting the event scheduler job in background: {str(ex)}')
-                        # Add Event to the queue
-                        if self.DEBUG:
-                            logger.info('Add Event to the queue')
-                        self.moesif_events_queue.put(event_data)
-                    except Exception as ex:
-                        if self.DEBUG:
-                            logger.info(f"Error while adding event to the queue: {str(ex)}")
-                else:
-                    if self.DEBUG:
-                        logger.info('Skipped Event as the moesif event model is None')
+        # Check if needs to skip the event
+        skip = await self.logger_helper.should_skip(self.settings, request, response, self.DEBUG)
+        if skip:
+            if self.DEBUG:
+                logger.info("Skipped Event using should_skip configuration option")
+            return response
+
+        # Read Response Body
+        resp_body = None
+        if self.LOG_BODY:
+            # Consuming FastAPI response and grabbing body here
+            resp_body = [section async for section in response.__dict__['body_iterator']]
+            # Preparing FastAPI response
+            response.__setattr__('body_iterator', async_iterator_wrapper(resp_body))
+
+        # Prepare Event Response Model
+        event_rsp = self.event_mapper.to_response(response, response_time, resp_body)
+
+        # Add user, company, session_token, and metadata
+        user_id = await self.logger_helper.get_user_id(self.settings, request, response, dict(request.headers), self.DEBUG)
+        company_id = await self.logger_helper.get_company_id(self.settings, request, response, self.DEBUG)
+        session_token = await self.logger_helper.get_session_token(self.settings, request, response, self.DEBUG)
+        metadata = await self.logger_helper.get_metadata(self.settings, request, response, self.DEBUG)
+
+        # Prepare Event Model
+        event_data = await self.event_mapper.to_event(event_req, event_rsp, user_id, company_id, session_token, metadata, blocked_by)
+
+        # Mask Event Model
+        if self.logger_helper.is_coroutine_function(self.logger_helper.mask_event):
+            event_data = await self.logger_helper.mask_event(event_data, self.settings, self.DEBUG)
+        else:
+            event_data = self.logger_helper.mask_event(event_data, self.settings, self.DEBUG)
+
+        # Sampling percentage
+        random_percentage = random.random() * 100
+        self.sampling_percentage = self.config.get_sampling_percentage(event_data, user_id, company_id)
+
+        # Add Weight to the event
+        event_data.weight = 1 if self.sampling_percentage == 0 else math.floor(100 / self.sampling_percentage)
+
+        if random_percentage >= self.sampling_percentage:
+            logger.info(f"Skipped Event due to sampling percentage: {str(self.sampling_percentage)}"
+                         f" and random percentage: {str(random_percentage)}")
+            return response
+
+        try:
+            # Add Event to the queue if able and count the dropped event if at capacity
+            if self.worker_pool.add_event(event_data):
+                logger.debug("Add Event to the queue")
+                if self.DEBUG:
+                    logger.info(f"Event added to the queue: {APIHelper.json_serialize(event_data)}")
             else:
+                self.dropped_events += 1
+                logger.info(f"Dropped Event due to queue capacity drop_count: {str(self.dropped_events)}")
                 if self.DEBUG:
-                    logger.info(f"Skipped Event due to sampling percentage: {str(self.sampling_percentage)} and random percentage: {str(random_percentage)}")
-        else:
-            if self.DEBUG:
-                logger.info('Skipped Event using should_skip configuration option')
+                    logger.info(f"Event dropped: {APIHelper.json_serialize(event_data)}")
+        # add_event does not throw exceptions so this is unexepected
+        except Exception as ex:
+            logger.exception(f"Error while adding event to the queue: {str(ex)}")
 
         return response
```

### Comparing `moesifasgi-0.1.7/moesifasgi/send_batch_events.py` & `moesifasgi-1.0.0/moesifasgi/send_batch_events.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-0.1.7/moesifasgi.egg-info/PKG-INFO` & `moesifasgi-1.0.0/moesifasgi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: moesifasgi
-Version: 0.1.7
+Version: 1.0.0
 Summary: Moesif Middleware for Python ASGI based platforms (FastAPI & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-asgi/
 Author: Moesif, Inc
 Author-email: keyur@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug asgi fastapi http middleware
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Moesif Middleware for Python ASGI based Frameworks
```

### Comparing `moesifasgi-0.1.7/setup.py` & `moesifasgi-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifasgi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.7',
+    version='1.0.0',
 
     description='Moesif Middleware for Python ASGI based platforms (FastAPI & Others)',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-asgi/',
@@ -58,35 +58,34 @@
         'Topic :: Software Development :: Libraries',
         'Topic :: Internet :: WWW/HTTP',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: Apache Software License',
 
         # Specify the Python versions you support here. In particular, ensure
-        # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        # Specify the Python versions you support here.
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     keywords='log analysis restful api development debug asgi fastapi http middleware',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['starlette', 'moesifapi>=1.4.2', 'moesifpythonrequest>=0.3.3', 'apscheduler'],
+    install_requires=['starlette>=0.16.0', 'moesifapi>=1.4.5', 'moesifpythonrequest>=0.3.3'],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={
         'dev': [],
```

