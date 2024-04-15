# Comparing `tmp/ohbot-4.0.8.tar.gz` & `tmp/ohbot-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ohbot-python/ohbot-python/dist/tmp4p679qqy/ohbot-4.0.8.tar", last modified: Wed Apr 14 13:38:35 2021, max compression
+gzip compressed data, was "ohbot-4.0.9.tar", last modified: Fri Mar  8 16:24:35 2024, max compression
```

## Comparing `ohbot-4.0.8.tar` & `ohbot-4.0.9.tar`

### file list

```diff
@@ -1,14 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-14 13:38:35.000000 ohbot-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)      355 2021-04-14 13:38:35.000000 ohbot-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     9675 2021-04-14 13:38:25.000000 ohbot-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-14 13:38:35.000000 ohbot-4.0.8/ohbot/
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-04-14 13:38:25.000000 ohbot-4.0.8/ohbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39357 2021-04-14 13:38:25.000000 ohbot-4.0.8/ohbot/ohbot.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-14 13:38:35.000000 ohbot-4.0.8/ohbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      355 2021-04-14 13:38:35.000000 ohbot-4.0.8/ohbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      205 2021-04-14 13:38:35.000000 ohbot-4.0.8/ohbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-04-14 13:38:35.000000 ohbot-4.0.8/ohbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2021-04-14 13:38:35.000000 ohbot-4.0.8/ohbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-04-14 13:38:35.000000 ohbot-4.0.8/ohbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2021-04-14 13:38:35.000000 ohbot-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1478 2021-04-14 13:38:25.000000 ohbot-4.0.8/setup.py
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-03-08 16:24:35.191040 ohbot-4.0.9/
+-rw-r--r--   0 georgewalker   (501) staff       (20)      459 2024-03-08 16:24:35.190893 ohbot-4.0.9/PKG-INFO
+-rw-r--r--   0 georgewalker   (501) staff       (20)     9675 2024-03-08 15:53:56.000000 ohbot-4.0.9/README.md
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-03-08 16:24:35.135170 ohbot-4.0.9/ohbot/
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-03-08 16:24:35.172417 ohbot-4.0.9/ohbot/Images/
+-rw-r--r--   0 georgewalker   (501) staff       (20)    53536 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/calibrate400.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      856 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/logoPT.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)     1467 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/logoPTOH.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      874 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/movedown.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      877 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/moveright.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)       90 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/off.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)       74 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/offsmaller.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      855 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/ohbotlogoSmall.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)       90 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/on.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)       74 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/onsmaller.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)     2002 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/picohlogo.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)     2002 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/picohlogoOn.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)     1314 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/picohlogoSmall.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      807 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/pixel.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      875 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/plus.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      633 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/resetIcon.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)     2486 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Images/savebutton.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)     1050 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/MotorDefinitionsv21.omd
+-rw-r--r--   0 georgewalker   (501) staff       (20)      456 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/OhbotSettings.xml
+-rw-r--r--   0 georgewalker   (501) staff       (20)      221 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/OhbotSpeech.csv
+-rw-r--r--   0 georgewalker   (501) staff       (20)    88134 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Silence1.wav
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-03-08 16:24:35.189826 ohbot-4.0.9/ohbot/Sounds/
+-rw-r--r--   0 georgewalker   (501) staff       (20)  1206224 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Sounds/fanfare.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)  1619014 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Sounds/loop.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)   234489 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Sounds/ohbot.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)   103760 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Sounds/smash.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)   287760 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/Sounds/spring.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)        7 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/__init__.py
+-rw-r--r--   0 georgewalker   (501) staff       (20)     4998 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/ohbot.obe
+-rw-r--r--   0 georgewalker   (501) staff       (20)    39484 2024-03-08 15:53:57.000000 ohbot-4.0.9/ohbot/ohbot.py
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-03-08 16:24:35.190479 ohbot-4.0.9/ohbot.egg-info/
+-rw-r--r--   0 georgewalker   (501) staff       (20)      459 2024-03-08 16:24:35.000000 ohbot-4.0.9/ohbot.egg-info/PKG-INFO
+-rw-r--r--   0 georgewalker   (501) staff       (20)      882 2024-03-08 16:24:35.000000 ohbot-4.0.9/ohbot.egg-info/SOURCES.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)        1 2024-03-08 16:24:35.000000 ohbot-4.0.9/ohbot.egg-info/dependency_links.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)       55 2024-03-08 16:24:35.000000 ohbot-4.0.9/ohbot.egg-info/requires.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)        6 2024-03-08 16:24:35.000000 ohbot-4.0.9/ohbot.egg-info/top_level.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)       79 2024-03-08 16:24:35.191340 ohbot-4.0.9/setup.cfg
+-rw-r--r--   0 georgewalker   (501) staff       (20)     1583 2024-03-08 16:23:18.000000 ohbot-4.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ohbot-4.0.8/README.md` & `ohbot-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ohbot-4.0.8/ohbot/ohbot.py` & `ohbot-4.0.9/ohbot/ohbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 HEADNOD = 0
 HEADTURN = 1
 EYETURN = 2
 LIDBLINK = 3
 TOPLIP = 4
 BOTTOMLIP = 5
 EYETILT = 6
+HEADROLL = 7
 
 # array to hold sensor values.
 sensors = [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
 
 # Put motor ranges into lists
 motorPos = [11, 11, 11, 11, 11, 11, 11, 11]
 motorMins = [0, 0, 0, 0, 0, 0, 0, 0]
@@ -80,15 +81,15 @@
 shapeList = []
 phraseList = []
 
 # define a module level variable for the serial port
 port = ""
 
 # define library version
-version = "4.0.8"
+version = "4.0.9"
 
 # flag to stop writing when writing for threading
 writing = False
 
 # flag to allow the library to run when not connected
 connected = False
 
@@ -458,14 +459,19 @@
         line = ser.readline()
         ser.close()
 
         subString = "v1".encode('latin-1')
 
         if line.find(subString) != -1:
             return True
+
+        subString = "v2".encode('latin-1')
+
+        if line.find(subString) != -1:
+            return True
         else:
             return False
     except:
         return False
 
 def init(portName = None):
     # pickup global instances of port, ser and sapi variables
```

### Comparing `ohbot-4.0.8/setup.py` & `ohbot-4.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from distutils.core import setup
-
+from setuptools import setup, find_packages
 import platform
 
-if platform.system() == "Darwin":
-    includes =['pyserial','lxml','playsound','pyobjc','numpy','comtypes','requests']
-
-if platform.system() == "Windows":
-    includes =['pyserial','lxml','playsound','numpy','comtypes','requests']
-
-if platform.system() == "Linux":
-    includes =['pyserial','playsound','gTTS','pydub','requests']
+# Define your includes per platform
+includes = {
+    "Darwin": ['pyserial', 'lxml', 'playsound', 'pyobjc', 'numpy', 'comtypes', 'requests'],
+    "Windows": ['pyserial', 'lxml', 'playsound', 'numpy', 'comtypes', 'requests'],
+    "Linux": ['pyserial', 'playsound', 'gTTS', 'pydub', 'requests']
+}
 
 setup(
-    name = 'ohbot',
-    packages = ['ohbot'],
-      package_data={'': ['OhbotSettings.xml','Silence1.wav','ohbotspeech.wav','OhbotSpeech.csv','ohbot.obe','phonemes.txt','Images/movedown.gif','Images/moveright.gif','Images/off.gif','Images/offsmaller.gif','Images/on.gif','Images/onsmaller.gif','Images/picohlogo.gif','Images/picohlogoOn.gif','Images/picohlogoSmall.gif','Images/ohbotlogoSmall.gif','Images/logoPTOH.gif','Images/calibrate400.gif','Images/plus.gif','Images/resetIcon.gif','Images/savebutton.gif','Images/logoPT.gif','MotorDefinitionsv21.omd','Images/pixel.gif','Sounds/fanfare.wav','Sounds/loop.wav','Sounds/ohbot.wav','Sounds/smash.wav','Sounds/spring.wav']},
+    name='ohbot',
+    packages=find_packages(),
+    package_data={
+        '': ['OhbotSettings.xml', 'Silence1.wav', 'ohbotspeech.wav', 'OhbotSpeech.csv', 'ohbot.obe',
+             'phonemes.txt', 'Images/movedown.gif', 'Images/moveright.gif', 'Images/off.gif',
+             'Images/offsmaller.gif', 'Images/on.gif', 'Images/onsmaller.gif', 'Images/picohlogo.gif',
+             'Images/picohlogoOn.gif', 'Images/picohlogoSmall.gif', 'Images/ohbotlogoSmall.gif',
+             'Images/logoPTOH.gif', 'Images/calibrate400.gif', 'Images/plus.gif', 'Images/resetIcon.gif',
+             'Images/savebutton.gif', 'Images/logoPT.gif', 'MotorDefinitionsv21.omd', 'Images/pixel.gif',
+             'Sounds/fanfare.wav', 'Sounds/loop.wav', 'Sounds/ohbot.wav', 'Sounds/smash.wav', 'Sounds/spring.wav']
+    },
     include_package_data=True,
-    version = '4.0.8',
-    description = 'Python library for controlling an Ohbot Robot',
-    author = 'ohbot',
-    author_email = 'info@ohbot.co.uk',
-    url = 'https://github.com/ohbot/ohbot-python',
-    download_url = 'https://github.com/ohbot/ohbot-python/archive/4.0.2.tar.gz',
-    keywords = ['ohbot', 'robot','picoh'],
-    classifiers = [],
-    install_requires= includes,
+    version='4.0.9',
+    description='Python library for controlling an Ohbot Robot',
+    author='ohbot',
+    author_email='info@ohbot.co.uk',
+    url='https://github.com/ohbot/ohbot-python',
+    download_url='https://github.com/ohbot/ohbot-python/archive/4.0.2.tar.gz',
+    keywords=['ohbot', 'robot', 'picoh'],
+    classifiers=[],
+    install_requires=includes.get(platform.system(), []),
 )
```

