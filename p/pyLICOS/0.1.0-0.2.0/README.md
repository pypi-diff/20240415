# Comparing `tmp/pyLICOS-0.1.0.tar.gz` & `tmp/pylicos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLICOS-0.1.0.tar", last modified: Tue Aug 22 18:52:59 2023, max compression
+gzip compressed data, was "pylicos-0.2.0.tar", last modified: Mon Apr 15 15:05:15 2024, max compression
```

## Comparing `pyLICOS-0.1.0.tar` & `pylicos-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-22 18:52:59.889054 pyLICOS-0.1.0/
--rw-rw-rw-   0        0        0      303 2023-08-22 18:52:59.889054 pyLICOS-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-08-22 13:35:23.000000 pyLICOS-0.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-08-22 13:34:16.000000 pyLICOS-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      362 2023-08-22 18:52:59.894043 pyLICOS-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-22 18:52:59.862188 pyLICOS-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-22 18:52:59.868165 pyLICOS-0.1.0/src/pyLICOS/
--rw-rw-rw-   0        0        0        0 2023-08-21 18:42:37.000000 pyLICOS-0.1.0/src/pyLICOS/__init__.py
--rw-rw-rw-   0        0        0    19145 2023-08-22 18:22:19.000000 pyLICOS-0.1.0/src/pyLICOS/client.py
--rw-rw-rw-   0        0        0     2103 2023-08-22 17:53:09.000000 pyLICOS-0.1.0/src/pyLICOS/communication.py
-drwxrwxrwx   0        0        0        0 2023-08-22 18:52:59.888110 pyLICOS-0.1.0/src/pyLICOS.egg-info/
--rw-rw-rw-   0        0        0      303 2023-08-22 18:52:59.000000 pyLICOS-0.1.0/src/pyLICOS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-08-22 18:52:59.000000 pyLICOS-0.1.0/src/pyLICOS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-22 18:52:59.000000 pyLICOS-0.1.0/src/pyLICOS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-22 18:52:59.000000 pyLICOS-0.1.0/src/pyLICOS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-22 18:52:59.000000 pyLICOS-0.1.0/src/pyLICOS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 15:05:15.142311 pylicos-0.2.0/
+-rw-rw-rw-   0        0        0      328 2024-04-15 15:05:15.142311 pylicos-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-08-22 13:35:23.000000 pylicos-0.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-22 13:34:16.000000 pylicos-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      362 2024-04-15 15:05:15.147327 pylicos-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 15:05:15.119372 pylicos-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 15:05:15.123361 pylicos-0.2.0/src/pyLICOS/
+-rw-rw-rw-   0        0        0        0 2023-08-21 18:42:37.000000 pylicos-0.2.0/src/pyLICOS/__init__.py
+-rw-rw-rw-   0        0        0    21569 2024-04-15 14:59:30.000000 pylicos-0.2.0/src/pyLICOS/client.py
+-rw-rw-rw-   0        0        0     2103 2023-08-22 17:53:09.000000 pylicos-0.2.0/src/pyLICOS/communication.py
+drwxrwxrwx   0        0        0        0 2024-04-15 15:05:15.141312 pylicos-0.2.0/src/pyLICOS.egg-info/
+-rw-rw-rw-   0        0        0      328 2024-04-15 15:05:15.000000 pylicos-0.2.0/src/pyLICOS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-15 15:05:15.000000 pylicos-0.2.0/src/pyLICOS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 15:05:15.000000 pylicos-0.2.0/src/pyLICOS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 15:05:15.000000 pylicos-0.2.0/src/pyLICOS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 15:05:15.000000 pylicos-0.2.0/src/pyLICOS.egg-info/top_level.txt
```

### Comparing `pyLICOS-0.1.0/src/pyLICOS/client.py` & `pylicos-0.2.0/src/pyLICOS/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import requests
 import time
 
 from math import ceil
 from http import HTTPStatus
 
-from . import communication
+from pyLICOS.src.pyLICOS import communication
 
 
 class Client:
     MAXIMUM_ATTEMPTS_SUBMISSION = 30
     SERVER_TIMEOUT = 30
     FILE_SIZE = 4
 
@@ -63,35 +63,35 @@
         :return: Enum of the current status
         """
         current_status = self._get_status(server_address, process_id, username, password)
         if (current_status is None) or (current_status == 'null'):
             return communication.Status.UNKOWN
         else:
             match current_status:
-                case '\"S\"':
+                case 'S':
                     pass
-                case '\"I\"':
+                case 'I':
                     pass
-                case '\"D\"':
+                case 'D':
                     pass
-                case '\"U\"':
+                case 'U':
                     pass
-                case '\"Q\"':
+                case 'Q':
                     pass
-                case '\"A\"':
+                case 'A':
                     pass
-                case '\"E\"':
+                case 'E':
                     pass
-                case '\"T\"':
+                case 'T':
                     return communication.Status.QUEUE
-                case '\"C\"':
+                case 'C':
                     return communication.Status.CANCELED
-                case '\"#\"':
+                case '#':
                     return communication.Status.ERROR
-                case '\"F\"':
+                case 'F':
                     return communication.Status.DONE
                 case default:
                     return communication.Status.RUNNING
 
     # TODO testar
     def cancel(self, server_address: str, username: str, password: str, process_id: int) -> bool:
         """
@@ -116,14 +116,53 @@
         """
         file = self._download_file(server_address, process_id, username, password, "output.zip")
 
         out_file = open(file_path, mode='wb')
         out_file.write(file)
         out_file.close()
 
+    def run(self, server_adress: str, zip_path: str, output_path: str, maximization: bool = True,
+            miprelstop: float = None, time_limit: float = None, username: str = '', password: str = ''):
+        """
+        Executes the full processing of LICOs, and saves the optmization result on a specified path.
+        :param server_adress: Full URL of LICOS server
+        :param zip_path: Full path of the zip file. It should contain the .MPS file
+        :param output_path: Full disk path (including file name and extension) where the output file will be saved.
+        :param maximization: If true (default), the sense of the optimization will be maximization.
+        :param miprelstop: Branch and Bound: This determines when the branch and bound tree search will terminate.
+            Branch and bound tree search will stop if:
+                |MIPOBJVAL - BESTBOUND| ≤ MIPRELSTOP x max(|BESTBOUND|,|MIPOBJVAL|)
+            where MIPOBJVAL is the value of the best solution’s objective function and BESTBOUND is the current best
+            solution bound.
+        :param time_limit: The maximum time in seconds that the Optimizer will run before it terminates,
+            including the problem setup time and solution time. For MIP problems, this is the total time taken to solve
+            all nodes.
+        :param username: Username for authentication
+        :param password: Password for authentication
+        :return:
+        """
+        process_id = self.queue_processing(server_adress, username, password, zip_path, maximization, miprelstop,
+                                           time_limit)
+        status = communication.Status.UNKOWN
+
+        while (status != communication.Status.CANCELED and status != communication.Status.ERROR and
+               status != communication.Status.DONE):
+            status = self.status(server_adress, username, password, process_id)
+            time.sleep(4)
+
+        if status == communication.Status.DONE:
+            self.download(server_adress, username, password, process_id, output_path)
+        else:
+            if status == communication.Status.ERROR:
+                raise Exception('Error during processing for ID {0}'.format(process_id))
+            else:
+                raise Exception('Processing for ID {0} was canceled!'.format(process_id))
+
+        return True
+
     def _get_process_id(self, queue_service_address: str, username: str, password: str) -> int:
         """
         Get the process ID of the user's current process
         :param queue_service_address: server address
         :param username: Username for authentication
         :param password: Password for authentication
         :return: ID of the running process
@@ -341,37 +380,38 @@
         request_header['Content-type'] = "application/json; charset=utf-8"
 
         json_dict = {'IDProcessamento': str(process_id)}
         json_content = json.dumps(json_dict)
 
         str_time = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
         link = communication.build_link(queue_service_address,
-                                        "QueueService/StatusAtual?datahora=" + str_time)
+                                        "QueueService/StatusGenerico?datahora=" + str_time)
         success = False
         tries = 0
         while (not success) and (tries < self.MAXIMUM_ATTEMPTS_SUBMISSION):
             try:
                 response = requests.post(link, data=json_content, timeout=self.SERVER_TIMEOUT, headers=request_header)
                 if response.status_code == HTTPStatus.OK:
-                    str_return = response.content.decode('utf8')
+                    response_json = response.content.decode('utf8')
+                    str_return = json.loads(response_json)['Status']
+
                     success = True
                 else:
                     time.sleep(3)
                     tries += 1
 
             except Exception:
                 time.sleep(3)
                 tries += 1
 
         if not success:
             raise Exception('It was not possible to get the process status.')
         else:
             return str_return
 
-    # TODO testar
     def _download_file(self, queue_service_address: str, process_id: int, username: str, password: str,
                        filename_on_server: str) -> bytes:
 
         file_content = []
         file_size_bytes = int(round(self.FILE_SIZE * 1024 * 1024))
 
         total_received = 0
```

### Comparing `pyLICOS-0.1.0/src/pyLICOS/communication.py` & `pylicos-0.2.0/src/pyLICOS/communication.py`

 * *Files identical despite different names*

