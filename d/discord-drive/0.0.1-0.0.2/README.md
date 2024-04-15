# Comparing `tmp/discord_drive-0.0.1.tar.gz` & `tmp/discord_drive-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_drive-0.0.1.tar", last modified: Fri Apr 12 21:06:35 2024, max compression
+gzip compressed data, was "discord_drive-0.0.2.tar", last modified: Mon Apr 15 12:50:21 2024, max compression
```

## Comparing `discord_drive-0.0.1.tar` & `discord_drive-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-12 21:06:35.731766 discord_drive-0.0.1/
--rw-r--r--   0 ryankarch   (501) staff       (20)     1081 2024-01-26 22:14:00.000000 discord_drive-0.0.1/LICENSE.md
--rw-r--r--   0 ryankarch   (501) staff       (20)      511 2024-04-12 21:06:35.731101 discord_drive-0.0.1/PKG-INFO
--rw-r--r--   0 ryankarch   (501) staff       (20)     3473 2024-04-12 19:58:00.000000 discord_drive-0.0.1/README.md
-drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-12 21:06:35.727906 discord_drive-0.0.1/discord_drive/
--rw-r--r--   0 ryankarch   (501) staff       (20)       43 2024-04-12 20:04:59.000000 discord_drive-0.0.1/discord_drive/__init__.py
--rw-r--r--   0 ryankarch   (501) staff       (20)    27491 2024-04-12 20:18:29.000000 discord_drive-0.0.1/discord_drive/discord_drive.py
--rw-r--r--   0 ryankarch   (501) staff       (20)    13544 2024-04-12 19:58:00.000000 discord_drive-0.0.1/discord_drive/drive.py
--rw-r--r--   0 ryankarch   (501) staff       (20)      241 2024-02-23 21:48:33.000000 discord_drive-0.0.1/discord_drive/utils.py
-drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-12 21:06:35.730570 discord_drive-0.0.1/discord_drive.egg-info/
--rw-r--r--   0 ryankarch   (501) staff       (20)      511 2024-04-12 21:06:35.000000 discord_drive-0.0.1/discord_drive.egg-info/PKG-INFO
--rw-r--r--   0 ryankarch   (501) staff       (20)      316 2024-04-12 21:06:35.000000 discord_drive-0.0.1/discord_drive.egg-info/SOURCES.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)        1 2024-04-12 21:06:35.000000 discord_drive-0.0.1/discord_drive.egg-info/dependency_links.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)      120 2024-04-12 21:06:35.000000 discord_drive-0.0.1/discord_drive.egg-info/requires.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)       14 2024-04-12 21:06:35.000000 discord_drive-0.0.1/discord_drive.egg-info/top_level.txt
--rw-r--r--   0 ryankarch   (501) staff       (20)       38 2024-04-12 21:06:35.731921 discord_drive-0.0.1/setup.cfg
--rw-r--r--   0 ryankarch   (501) staff       (20)      710 2024-04-09 21:03:26.000000 discord_drive-0.0.1/setup.py
+drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-15 12:50:21.008006 discord_drive-0.0.2/
+-rw-r--r--   0 ryankarch   (501) staff       (20)     1081 2024-01-26 22:14:00.000000 discord_drive-0.0.2/LICENSE.md
+-rw-r--r--   0 ryankarch   (501) staff       (20)      511 2024-04-15 12:50:21.007284 discord_drive-0.0.2/PKG-INFO
+-rw-r--r--   0 ryankarch   (501) staff       (20)     3473 2024-04-12 19:58:00.000000 discord_drive-0.0.2/README.md
+drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-15 12:50:21.004298 discord_drive-0.0.2/discord_drive/
+-rw-r--r--   0 ryankarch   (501) staff       (20)       43 2024-04-12 20:04:59.000000 discord_drive-0.0.2/discord_drive/__init__.py
+-rw-r--r--   0 ryankarch   (501) staff       (20)    27158 2024-04-15 12:36:22.000000 discord_drive-0.0.2/discord_drive/discord_drive.py
+-rw-r--r--   0 ryankarch   (501) staff       (20)    13544 2024-04-12 19:58:00.000000 discord_drive-0.0.2/discord_drive/drive.py
+-rw-r--r--   0 ryankarch   (501) staff       (20)      241 2024-02-23 21:48:33.000000 discord_drive-0.0.2/discord_drive/utils.py
+drwxr-xr-x   0 ryankarch   (501) staff       (20)        0 2024-04-15 12:50:21.006698 discord_drive-0.0.2/discord_drive.egg-info/
+-rw-r--r--   0 ryankarch   (501) staff       (20)      511 2024-04-15 12:50:20.000000 discord_drive-0.0.2/discord_drive.egg-info/PKG-INFO
+-rw-r--r--   0 ryankarch   (501) staff       (20)      316 2024-04-15 12:50:20.000000 discord_drive-0.0.2/discord_drive.egg-info/SOURCES.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)        1 2024-04-15 12:50:20.000000 discord_drive-0.0.2/discord_drive.egg-info/dependency_links.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)      120 2024-04-15 12:50:20.000000 discord_drive-0.0.2/discord_drive.egg-info/requires.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)       14 2024-04-15 12:50:20.000000 discord_drive-0.0.2/discord_drive.egg-info/top_level.txt
+-rw-r--r--   0 ryankarch   (501) staff       (20)       38 2024-04-15 12:50:21.008139 discord_drive-0.0.2/setup.cfg
+-rw-r--r--   0 ryankarch   (501) staff       (20)      710 2024-04-15 12:49:05.000000 discord_drive-0.0.2/setup.py
```

### Comparing `discord_drive-0.0.1/LICENSE.md` & `discord_drive-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `discord_drive-0.0.1/README.md` & `discord_drive-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `discord_drive-0.0.1/discord_drive/discord_drive.py` & `discord_drive-0.0.2/discord_drive/discord_drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,15 @@
 
 class Command:
     def __init__(self, str_, params: dict):
         self._str = str_
         self._params = params
         self._timestamp = datetime.now()
 
-def get_guild_ids():
-    guild_id = os.getenv("DD_GUILD_ID")
-    if not guild_id:
-        raise Exception("Environment variable 'DD_GUILD_ID' not found, please ensure that the .env file contains this variable, and that 'load_dotenv()' is placed above the import of this cog.")
-    return [guild_id]
-
-class DriveAPICommands(discord.ext.commands.Cog, guild_ids=get_guild_ids()):
+class DriveAPICommands(discord.ext.commands.Cog):
     
     _drive_state = defaultdict(lambda: defaultdict(id=None, folders=[], files=[]))
     _wd_cache = None
     
 
     def __init__(self, bot: discord.ext.commands.Bot, root:str):
         """Initializes the API connection and cache
```

### Comparing `discord_drive-0.0.1/discord_drive/drive.py` & `discord_drive-0.0.2/discord_drive/drive.py`

 * *Files identical despite different names*

### Comparing `discord_drive-0.0.1/setup.py` & `discord_drive-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # print(os.curdir)
 # with open('./discord_drive/requirements.txt') as f:
 #     required = f.read().splitlines()
     
 setup(
     name='discord_drive',
-    version='0.0.1',
+    version='0.0.2',
     description='Use Google Drive via Discord!',
     license='MIT',
     packages=['discord_drive'],
     author='Ryan Karch, Dominic Beyer',
     author_email='',
     keywords=['Discord', 'Google Drive'],
     url='https://github.com/thedomino1313/DiscordDrive',
```

