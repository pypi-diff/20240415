# Comparing `tmp/mypcremote-0.5.1.tar.gz` & `tmp/mypcremote-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypcremote-0.5.1.tar", last modified: Mon Apr 15 09:44:39 2024, max compression
+gzip compressed data, was "mypcremote-0.5.2.tar", last modified: Mon Apr 15 11:19:14 2024, max compression
```

## Comparing `mypcremote-0.5.1.tar` & `mypcremote-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 09:44:39.964512 mypcremote-0.5.1/
--rw-rw-rw-   0        0        0     1092 2024-04-15 07:22:18.000000 mypcremote-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     3825 2024-04-15 09:44:39.963605 mypcremote-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2812 2024-04-15 08:04:42.000000 mypcremote-0.5.1/README.md
--rw-rw-rw-   0        0        0     1171 2024-04-15 09:44:27.000000 mypcremote-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 09:44:39.964512 mypcremote-0.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 09:44:39.920803 mypcremote-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 09:44:39.925101 mypcremote-0.5.1/src/mypcremote/
--rw-rw-rw-   0        0        0     1888 2024-04-15 08:46:46.000000 mypcremote-0.5.1/src/mypcremote/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:44:39.960639 mypcremote-0.5.1/src/mypcremote/commands/
--rw-rw-rw-   0        0        0        0 2023-11-10 12:39:58.000000 mypcremote-0.5.1/src/mypcremote/commands/__init__.py
--rw-rw-rw-   0        0        0      453 2023-11-12 15:27:05.000000 mypcremote-0.5.1/src/mypcremote/commands/beep.py
--rw-rw-rw-   0        0        0      671 2023-11-11 11:31:42.000000 mypcremote-0.5.1/src/mypcremote/commands/camera.py
--rw-rw-rw-   0        0        0      547 2023-11-11 11:30:48.000000 mypcremote-0.5.1/src/mypcremote/commands/clear.py
--rw-rw-rw-   0        0        0      628 2023-11-12 14:41:43.000000 mypcremote-0.5.1/src/mypcremote/commands/hybernate.py
--rw-rw-rw-   0        0        0     1588 2023-11-12 14:20:10.000000 mypcremote-0.5.1/src/mypcremote/commands/kill.py
--rw-rw-rw-   0        0        0      694 2023-11-24 17:15:03.000000 mypcremote-0.5.1/src/mypcremote/commands/location.py
--rw-rw-rw-   0        0        0      690 2023-11-11 11:30:21.000000 mypcremote-0.5.1/src/mypcremote/commands/lock.py
--rw-rw-rw-   0        0        0     1528 2023-11-13 05:53:39.000000 mypcremote-0.5.1/src/mypcremote/commands/notify.py
--rw-rw-rw-   0        0        0      518 2023-11-13 08:29:30.000000 mypcremote-0.5.1/src/mypcremote/commands/openurl.py
--rw-rw-rw-   0        0        0      145 2023-11-12 14:45:38.000000 mypcremote-0.5.1/src/mypcremote/commands/ping.py
--rw-rw-rw-   0        0        0      710 2023-11-11 11:30:01.000000 mypcremote-0.5.1/src/mypcremote/commands/reboot.py
--rw-rw-rw-   0        0        0      410 2023-11-11 11:29:27.000000 mypcremote-0.5.1/src/mypcremote/commands/screenshot.py
--rw-rw-rw-   0        0        0      763 2023-11-11 11:28:54.000000 mypcremote-0.5.1/src/mypcremote/commands/shutdown.py
--rw-rw-rw-   0        0        0      717 2023-11-11 11:28:24.000000 mypcremote-0.5.1/src/mypcremote/commands/sleep.py
--rw-rw-rw-   0        0        0      676 2023-11-11 14:09:49.000000 mypcremote-0.5.1/src/mypcremote/commands/speak.py
--rw-rw-rw-   0        0        0      692 2023-11-11 11:28:42.000000 mypcremote-0.5.1/src/mypcremote/commands/status.py
--rw-rw-rw-   0        0        0      440 2023-11-11 11:26:35.000000 mypcremote-0.5.1/src/mypcremote/commands/terminal.py
--rw-rw-rw-   0        0        0      210 2023-11-13 08:33:07.000000 mypcremote-0.5.1/src/mypcremote/commands/terminate.py
--rw-rw-rw-   0        0        0     1005 2023-11-12 14:31:11.000000 mypcremote-0.5.1/src/mypcremote/commands/upload.py
--rw-rw-rw-   0        0        0     1081 2023-11-11 11:27:07.000000 mypcremote-0.5.1/src/mypcremote/commands/voicecall.py
--rw-rw-rw-   0        0        0     1387 2023-11-12 13:56:04.000000 mypcremote-0.5.1/src/mypcremote/commands/volume.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:44:39.961644 mypcremote-0.5.1/src/mypcremote.egg-info/
--rw-rw-rw-   0        0        0     3825 2024-04-15 09:44:39.000000 mypcremote-0.5.1/src/mypcremote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2024-04-15 09:44:39.000000 mypcremote-0.5.1/src/mypcremote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 09:44:39.000000 mypcremote-0.5.1/src/mypcremote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-04-15 09:44:39.000000 mypcremote-0.5.1/src/mypcremote.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 09:44:39.000000 mypcremote-0.5.1/src/mypcremote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 11:19:14.034178 mypcremote-0.5.2/
+-rw-rw-rw-   0        0        0     1092 2024-04-15 07:22:18.000000 mypcremote-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0     3825 2024-04-15 11:19:14.033178 mypcremote-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2812 2024-04-15 08:04:42.000000 mypcremote-0.5.2/README.md
+-rw-rw-rw-   0        0        0     1233 2024-04-15 11:15:43.000000 mypcremote-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:19:14.034178 mypcremote-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 11:19:13.979840 mypcremote-0.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 11:19:13.993275 mypcremote-0.5.2/src/mypcremote/
+-rw-rw-rw-   0        0        0     2106 2024-04-15 11:06:09.000000 mypcremote-0.5.2/src/mypcremote/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:19:14.030138 mypcremote-0.5.2/src/mypcremote/commands/
+-rw-rw-rw-   0        0        0        0 2023-11-10 12:39:58.000000 mypcremote-0.5.2/src/mypcremote/commands/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-11-12 15:27:05.000000 mypcremote-0.5.2/src/mypcremote/commands/beep.py
+-rw-rw-rw-   0        0        0      671 2023-11-11 11:31:42.000000 mypcremote-0.5.2/src/mypcremote/commands/camera.py
+-rw-rw-rw-   0        0        0      547 2023-11-11 11:30:48.000000 mypcremote-0.5.2/src/mypcremote/commands/clear.py
+-rw-rw-rw-   0        0        0      628 2023-11-12 14:41:43.000000 mypcremote-0.5.2/src/mypcremote/commands/hybernate.py
+-rw-rw-rw-   0        0        0     1588 2023-11-12 14:20:10.000000 mypcremote-0.5.2/src/mypcremote/commands/kill.py
+-rw-rw-rw-   0        0        0      694 2023-11-24 17:15:03.000000 mypcremote-0.5.2/src/mypcremote/commands/location.py
+-rw-rw-rw-   0        0        0      690 2023-11-11 11:30:21.000000 mypcremote-0.5.2/src/mypcremote/commands/lock.py
+-rw-rw-rw-   0        0        0     1528 2023-11-13 05:53:39.000000 mypcremote-0.5.2/src/mypcremote/commands/notify.py
+-rw-rw-rw-   0        0        0      518 2023-11-13 08:29:30.000000 mypcremote-0.5.2/src/mypcremote/commands/openurl.py
+-rw-rw-rw-   0        0        0      145 2023-11-12 14:45:38.000000 mypcremote-0.5.2/src/mypcremote/commands/ping.py
+-rw-rw-rw-   0        0        0      710 2023-11-11 11:30:01.000000 mypcremote-0.5.2/src/mypcremote/commands/reboot.py
+-rw-rw-rw-   0        0        0      410 2023-11-11 11:29:27.000000 mypcremote-0.5.2/src/mypcremote/commands/screenshot.py
+-rw-rw-rw-   0        0        0      763 2023-11-11 11:28:54.000000 mypcremote-0.5.2/src/mypcremote/commands/shutdown.py
+-rw-rw-rw-   0        0        0      717 2023-11-11 11:28:24.000000 mypcremote-0.5.2/src/mypcremote/commands/sleep.py
+-rw-rw-rw-   0        0        0      676 2023-11-11 14:09:49.000000 mypcremote-0.5.2/src/mypcremote/commands/speak.py
+-rw-rw-rw-   0        0        0      692 2023-11-11 11:28:42.000000 mypcremote-0.5.2/src/mypcremote/commands/status.py
+-rw-rw-rw-   0        0        0      440 2023-11-11 11:26:35.000000 mypcremote-0.5.2/src/mypcremote/commands/terminal.py
+-rw-rw-rw-   0        0        0      210 2023-11-13 08:33:07.000000 mypcremote-0.5.2/src/mypcremote/commands/terminate.py
+-rw-rw-rw-   0        0        0     1005 2023-11-12 14:31:11.000000 mypcremote-0.5.2/src/mypcremote/commands/upload.py
+-rw-rw-rw-   0        0        0     1081 2023-11-11 11:27:07.000000 mypcremote-0.5.2/src/mypcremote/commands/voicecall.py
+-rw-rw-rw-   0        0        0     1387 2023-11-12 13:56:04.000000 mypcremote-0.5.2/src/mypcremote/commands/volume.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:19:14.032194 mypcremote-0.5.2/src/mypcremote.egg-info/
+-rw-rw-rw-   0        0        0     3825 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 11:19:13.000000 mypcremote-0.5.2/src/mypcremote.egg-info/top_level.txt
```

### Comparing `mypcremote-0.5.1/LICENSE` & `mypcremote-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/PKG-INFO` & `mypcremote-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypcremote
-Version: 0.5.1
+Version: 0.5.2
 Summary: A good package to let your computer remote controlled using Discord
 Author-email: Zain Ul Abidin <zain26134@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Zedstron/My-PC-Remote
 Project-URL: Issues, https://github.com/Zedstron/My-PC-Remote/issues
 Keywords: discord,remote,remote-pc,pccontrol,pc-remote,screen-sharing,remote-access,remote-control,pc-management,pc-administration,computer-access,computer-control
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mypcremote-0.5.1/README.md` & `mypcremote-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/__main__.py` & `mypcremote-0.5.2/src/mypcremote/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import sys
 import discord
-import importlib
+from pydoc import importfile
 from dotenv import load_dotenv
 from discord.ext.commands import Bot
 
-load_dotenv()
+load_dotenv(dotenv_path=os.path.join(os.path.dirname(__file__), ".env"))
 intents = discord.Intents.all()
 
 bot = Bot(description="A remote administration discord BOT to control your PC", command_prefix='#', intents=intents)
 
 def RegisterCommands():
-    scripts = [file[:-3] for file in os.listdir('commands') if file.endswith('.py') and file != '__init__.py']
+    commands = os.path.join(os.path.dirname(__file__), "commands")
+    scripts = [file for file in os.listdir(commands) if file.endswith('.py') and file != '__init__.py']
     for name in scripts:
-        script_module = importlib.import_module(f"commands.{name}")
+        script_module = importfile(os.path.join(commands, name))
         Instance = getattr(script_module, 'Run', None)
 
         if Instance and callable(Instance):
             desc = getattr(script_module, 'Desc', 'Not Available')
             bot.command(name=name.split(".")[0], help=desc())(Instance)
 
 def Init(token=os.environ.get('TOKEN')):
@@ -46,17 +47,18 @@
 @bot.event
 async def on_message(message):
     proceed = message.author != bot.user
     if proceed:
         await bot.process_commands(message)
 
 def main():
+    sys.path.append(os.path.dirname(__file__))
     if os.environ.get('TOKEN', None) is None:
         token = input("Enter Auth Token: ")
-        with open('.env', 'w') as f:
+        with open(os.path.join(os.path.dirname(__file__), ".env"), 'w') as f:
             f.write(f'TOKEN={token}')
         Init(token)
     else:
         Init()
 
 if __name__ == "__main__":
     main()
```

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/camera.py` & `mypcremote-0.5.2/src/mypcremote/commands/camera.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/clear.py` & `mypcremote-0.5.2/src/mypcremote/commands/clear.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/hybernate.py` & `mypcremote-0.5.2/src/mypcremote/commands/hybernate.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/kill.py` & `mypcremote-0.5.2/src/mypcremote/commands/kill.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/location.py` & `mypcremote-0.5.2/src/mypcremote/commands/location.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/lock.py` & `mypcremote-0.5.2/src/mypcremote/commands/lock.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/notify.py` & `mypcremote-0.5.2/src/mypcremote/commands/notify.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/openurl.py` & `mypcremote-0.5.2/src/mypcremote/commands/openurl.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/reboot.py` & `mypcremote-0.5.2/src/mypcremote/commands/reboot.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/shutdown.py` & `mypcremote-0.5.2/src/mypcremote/commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/sleep.py` & `mypcremote-0.5.2/src/mypcremote/commands/sleep.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/speak.py` & `mypcremote-0.5.2/src/mypcremote/commands/speak.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/status.py` & `mypcremote-0.5.2/src/mypcremote/commands/status.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/upload.py` & `mypcremote-0.5.2/src/mypcremote/commands/upload.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/voicecall.py` & `mypcremote-0.5.2/src/mypcremote/commands/voicecall.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote/commands/volume.py` & `mypcremote-0.5.2/src/mypcremote/commands/volume.py`

 * *Files identical despite different names*

### Comparing `mypcremote-0.5.1/src/mypcremote.egg-info/PKG-INFO` & `mypcremote-0.5.2/src/mypcremote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypcremote
-Version: 0.5.1
+Version: 0.5.2
 Summary: A good package to let your computer remote controlled using Discord
 Author-email: Zain Ul Abidin <zain26134@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Zedstron/My-PC-Remote
 Project-URL: Issues, https://github.com/Zedstron/My-PC-Remote/issues
 Keywords: discord,remote,remote-pc,pccontrol,pc-remote,screen-sharing,remote-access,remote-control,pc-management,pc-administration,computer-access,computer-control
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mypcremote-0.5.1/src/mypcremote.egg-info/SOURCES.txt` & `mypcremote-0.5.2/src/mypcremote.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 src/mypcremote/__main__.py
 src/mypcremote.egg-info/PKG-INFO
 src/mypcremote.egg-info/SOURCES.txt
 src/mypcremote.egg-info/dependency_links.txt
+src/mypcremote.egg-info/entry_points.txt
 src/mypcremote.egg-info/requires.txt
 src/mypcremote.egg-info/top_level.txt
 src/mypcremote/commands/__init__.py
 src/mypcremote/commands/beep.py
 src/mypcremote/commands/camera.py
 src/mypcremote/commands/clear.py
 src/mypcremote/commands/hybernate.py
```

