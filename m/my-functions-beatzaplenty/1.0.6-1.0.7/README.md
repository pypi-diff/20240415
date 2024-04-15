# Comparing `tmp/my_functions_beatzaplenty-1.0.6.tar.gz` & `tmp/my_functions_beatzaplenty-1.0.7.tar.gz`

## Comparing `my_functions_beatzaplenty-1.0.6.tar` & `my_functions_beatzaplenty-1.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/.vscode/launch.json
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/.vscode/settings.json
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/.gitignore
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/check_command_exists.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/check_outgoing_ports.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/config.ini
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/create_config_file.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/create_ssh_connection.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/execute_ssh_command.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/install_required_modules.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/is_repo_up_to_date.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/parse_tuple.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/remote_update.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/requirements.txt
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/resize_linode_instance.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/run_command.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/run_updates.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/update-firewall.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/update_containers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/__init__.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_check_command_exists.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_check_outgoing_ports.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_create_config_file.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_create_ssh_connection.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_execute_ssh_command.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_install_required_modules.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_is_repo_up_to_date.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_parse_tuple.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_remote_update.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_resize_linode_instance.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_run_command.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_run_updates.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/tests/test_update_containers.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/LICENSE
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/.vscode/launch.json
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/.gitignore
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/check_command_exists.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/check_outgoing_ports.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/config.ini
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/create_config_file.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/create_ssh_connection.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/execute_ssh_command.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/install_required_modules.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/is_repo_up_to_date.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/parse_tuple.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/remote_update.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/requirements.txt
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/resize_linode_instance.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/run_command.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/run_updates.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/update-firewall.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/update_containers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_check_command_exists.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_check_outgoing_ports.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_create_config_file.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_create_ssh_connection.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_execute_ssh_command.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_install_required_modules.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_is_repo_up_to_date.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_parse_tuple.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_remote_update.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_resize_linode_instance.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_run_command.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_run_updates.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/tests/test_update_containers.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/LICENSE
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.7/PKG-INFO
```

### Comparing `my_functions_beatzaplenty-1.0.6/.vscode/launch.json` & `my_functions_beatzaplenty-1.0.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/.gitignore` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/.gitignore`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/README.md` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/README.md`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/check_command_exists.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/check_command_exists.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/check_outgoing_ports.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/check_outgoing_ports.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/config.ini` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/config.ini`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/create_config_file.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/create_config_file.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/create_ssh_connection.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/create_ssh_connection.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/execute_ssh_command.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/execute_ssh_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/install_required_modules.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/install_required_modules.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/is_repo_up_to_date.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/is_repo_up_to_date.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/remote_update.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/remote_update.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/resize_linode_instance.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/resize_linode_instance.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/run_command.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/run_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/run_updates.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/run_updates.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/update-firewall.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/update-firewall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os, subprocess, socket, configparser
 from datetime import datetime, timezone, timedelta
 
 # Get script parent dir
 parent_dir = os.path.dirname(os.path.abspath(__file__))
+
+# Timezone settings
 timezone_offset = +10.0  # Pacific Standard Time (UTC−08:00)
 tzinfo = timezone(timedelta(hours=timezone_offset))
+tz_string_format = "%a %b %d %H:%M"
 
 # Init configparser
 config = configparser.ConfigParser()
 config.read(f'{parent_dir}/config.ini')
 default_config = config['firewall']
 
 LOG_FILE = default_config.get("log_file")
@@ -29,25 +32,25 @@
 
 #Function to update config file with new values
 def update_config(config_file, ip_address, tzinfo):
     edit = configparser.ConfigParser()
     edit.read(config_file)
     config_items = edit["firewall"]
     config_items["last_ip"] = ip_address
-    config_items["last_change"] = datetime.now(tzinfo).strftime("%a %b %d %T")
+    config_items["last_change"] = datetime.now(tzinfo).strftime(tz_string_format)
     with open(config_file, "w") as config:
         edit.write(config)
 
 # Function to update firewall rules
 def update_firewall_rules(current_ip, last_ip):
     cmd_part_1 = default_config.get("cmd_part_1")
     cmd_part_2 = default_config.get("cmd_part_2")
 
     with open(LOG_FILE, "w") as log_file:
-        log_file.write("Run time: " + str(datetime.now(tzinfo).strftime("%a %b %d %T")) + "\n")
+        log_file.write("Run time: " + str(datetime.now(tzinfo).strftime(tz_string_format)) + "\n")
         log_file.write("Last Change: " + str(default_config.get("last_change")) + "\n")
 
         if current_ip != last_ip:
             del_cmd = f"sudo ufw delete {cmd_part_1} {last_ip} {cmd_part_2}"
             add_cmd = f"sudo ufw {cmd_part_1} {current_ip} {cmd_part_2}"
             log_file.write("Last IP address: " + str(last_ip) + "\n")
             log_file.write("Current IP address: " + str(current_ip) + "\n")
```

### Comparing `my_functions_beatzaplenty-1.0.6/src/my_functions_beatzaplenty/update_containers.py` & `my_functions_beatzaplenty-1.0.7/src/my_functions_beatzaplenty/update_containers.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_check_command_exists.py` & `my_functions_beatzaplenty-1.0.7/tests/test_check_command_exists.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_check_outgoing_ports.py` & `my_functions_beatzaplenty-1.0.7/tests/test_check_outgoing_ports.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_create_config_file.py` & `my_functions_beatzaplenty-1.0.7/tests/test_create_config_file.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_create_ssh_connection.py` & `my_functions_beatzaplenty-1.0.7/tests/test_create_ssh_connection.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_execute_ssh_command.py` & `my_functions_beatzaplenty-1.0.7/tests/test_execute_ssh_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_install_required_modules.py` & `my_functions_beatzaplenty-1.0.7/tests/test_install_required_modules.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_is_repo_up_to_date.py` & `my_functions_beatzaplenty-1.0.7/tests/test_is_repo_up_to_date.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_parse_tuple.py` & `my_functions_beatzaplenty-1.0.7/tests/test_parse_tuple.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_remote_update.py` & `my_functions_beatzaplenty-1.0.7/tests/test_remote_update.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_resize_linode_instance.py` & `my_functions_beatzaplenty-1.0.7/tests/test_resize_linode_instance.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_run_command.py` & `my_functions_beatzaplenty-1.0.7/tests/test_run_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_run_updates.py` & `my_functions_beatzaplenty-1.0.7/tests/test_run_updates.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/tests/test_update_containers.py` & `my_functions_beatzaplenty-1.0.7/tests/test_update_containers.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/.gitignore` & `my_functions_beatzaplenty-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/LICENSE` & `my_functions_beatzaplenty-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.6/pyproject.toml` & `my_functions_beatzaplenty-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "my_functions_beatzaplenty"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Wayne Bennett", email="wayne.bennett@live.com" },
 ]
 description = "My Custom functions that I use all the time"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `my_functions_beatzaplenty-1.0.6/PKG-INFO` & `my_functions_beatzaplenty-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: my_functions_beatzaplenty
-Version: 1.0.6
+Version: 1.0.7
 Summary: My Custom functions that I use all the time
 Project-URL: Homepage, https://github.com/WayneBennett666/common
 Project-URL: Issues, https://github.com/WayneBennett666/common/issues
 Author-email: Wayne Bennett <wayne.bennett@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

