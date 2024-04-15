# Comparing `tmp/zimo_web_screenshot-0.1.1.tar.gz` & `tmp/zimo-web-screenshot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimo_web_screenshot-0.1.1.tar", last modified: Mon Apr 15 11:33:02 2024, max compression
+gzip compressed data, was "zimo-web-screenshot-0.1.2.tar", last modified: Mon Apr 15 11:37:39 2024, max compression
```

## Comparing `zimo_web_screenshot-0.1.1.tar` & `zimo-web-screenshot-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:33:02.637790 zimo_web_screenshot-0.1.1/
--rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo_web_screenshot-0.1.1/LICENSE
--rw-r--r--   0 zimoluo    (501) staff       (20)     2160 2024-04-15 11:33:02.637875 zimo_web_screenshot-0.1.1/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)     1655 2024-04-15 11:32:37.000000 zimo_web_screenshot-0.1.1/README.md
--rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-04-15 11:33:02.638064 zimo_web_screenshot-0.1.1/setup.cfg
--rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-04-15 11:30:24.000000 zimo_web_screenshot-0.1.1/setup.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:33:02.636613 zimo_web_screenshot-0.1.1/zimo_web_screenshot/
--rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot/__init__.py
--rw-r--r--   0 zimoluo    (501) staff       (20)     2254 2024-04-15 05:05:14.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot/screenshot.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:33:02.637677 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/
--rw-r--r--   0 zimoluo    (501) staff       (20)     2160 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/requires.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:37:39.199027 zimo-web-screenshot-0.1.2/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo-web-screenshot-0.1.2/LICENSE
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2160 2024-04-15 11:37:39.199118 zimo-web-screenshot-0.1.2/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1655 2024-04-15 11:37:00.000000 zimo-web-screenshot-0.1.2/README.md
+-rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-04-15 11:37:39.199294 zimo-web-screenshot-0.1.2/setup.cfg
+-rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-04-15 11:37:26.000000 zimo-web-screenshot-0.1.2/setup.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:37:39.198108 zimo-web-screenshot-0.1.2/zimo_web_screenshot/
+-rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot/__init__.py
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2254 2024-04-15 05:05:14.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot/screenshot.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:37:39.198905 zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2160 2024-04-15 11:37:39.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-04-15 11:37:39.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-04-15 11:37:39.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-04-15 11:37:39.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-04-15 11:37:39.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/requires.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-04-15 11:37:39.000000 zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/top_level.txt
```

### Comparing `zimo_web_screenshot-0.1.1/LICENSE` & `zimo-web-screenshot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zimo_web_screenshot-0.1.1/PKG-INFO` & `zimo-web-screenshot-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zimo_web_screenshot
-Version: 0.1.1
+Name: zimo-web-screenshot
+Version: 0.1.2
 Summary: A simple CLI tool to take screenshots of Zimo Web pages with Selenium.
 Home-page: https://github.com/zimoluo/zimo-web-screenshot-tool
 Author: Zimo Luo
 Author-email: abgkings0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,27 +25,27 @@
 - Save screenshots locally in PNG format.
 
 ## Installation
 
 To use this tool, you'll need Python installed on your system. The tool also requires Selenium, which will be automatically installed when you install the package from PyPI.
 
 1. **Install the Package**:
-   You can install `zimo_web_screenshot` directly from PyPI using pip:
+   You can install `zimo-web-screenshot` directly from PyPI using pip:
    ```bash
-   pip install zimo_web_screenshot
+   pip install zimo-web-screenshot
    ```
 2. **Install a Web Driver**:
    You need to have at least one recognizable Chrome web driver installed on your device. This is typically bundled within a Chrome browser.
 
 ## Usage
 
 To use the tool, navigate to the project directory and run the script with the required options. Example below:
 
 ```bash
-zimo_web_screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
+zimo-web-screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
 - `-w`, `--width`: Width of the browser window (default: `1600`)
 - `-H`, `--height`: Height of the browser window (default: `900`)
 - `-t`, `--theme`: Theme name to apply (default: `pixelland`)
```

### Comparing `zimo_web_screenshot-0.1.1/README.md` & `zimo-web-screenshot-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 - Save screenshots locally in PNG format.
 
 ## Installation
 
 To use this tool, you'll need Python installed on your system. The tool also requires Selenium, which will be automatically installed when you install the package from PyPI.
 
 1. **Install the Package**:
-   You can install `zimo_web_screenshot` directly from PyPI using pip:
+   You can install `zimo-web-screenshot` directly from PyPI using pip:
    ```bash
-   pip install zimo_web_screenshot
+   pip install zimo-web-screenshot
    ```
 2. **Install a Web Driver**:
    You need to have at least one recognizable Chrome web driver installed on your device. This is typically bundled within a Chrome browser.
 
 ## Usage
 
 To use the tool, navigate to the project directory and run the script with the required options. Example below:
 
 ```bash
-zimo_web_screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
+zimo-web-screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
 - `-w`, `--width`: Width of the browser window (default: `1600`)
 - `-H`, `--height`: Height of the browser window (default: `900`)
 - `-t`, `--theme`: Theme name to apply (default: `pixelland`)
```

### Comparing `zimo_web_screenshot-0.1.1/setup.py` & `zimo-web-screenshot-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='zimo_web_screenshot',
-    version='0.1.1',
+    name='zimo-web-screenshot',
+    version='0.1.2',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'selenium',
     ],
     entry_points={
         'console_scripts': [
-            'zimo_web_screenshot=zimo_web_screenshot.screenshot:main',
+            'zimo-web-screenshot=zimo_web_screenshot.screenshot:main',
         ],
     },
     author='Zimo Luo',
     author_email='abgkings0920@gmail.com',
     description='A simple CLI tool to take screenshots of Zimo Web pages with Selenium.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `zimo_web_screenshot-0.1.1/zimo_web_screenshot/screenshot.py` & `zimo-web-screenshot-0.1.2/zimo_web_screenshot/screenshot.py`

 * *Files identical despite different names*

### Comparing `zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/PKG-INFO` & `zimo-web-screenshot-0.1.2/zimo_web_screenshot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimo-web-screenshot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple CLI tool to take screenshots of Zimo Web pages with Selenium.
 Home-page: https://github.com/zimoluo/zimo-web-screenshot-tool
 Author: Zimo Luo
 Author-email: abgkings0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,27 +25,27 @@
 - Save screenshots locally in PNG format.
 
 ## Installation
 
 To use this tool, you'll need Python installed on your system. The tool also requires Selenium, which will be automatically installed when you install the package from PyPI.
 
 1. **Install the Package**:
-   You can install `zimo_web_screenshot` directly from PyPI using pip:
+   You can install `zimo-web-screenshot` directly from PyPI using pip:
    ```bash
-   pip install zimo_web_screenshot
+   pip install zimo-web-screenshot
    ```
 2. **Install a Web Driver**:
    You need to have at least one recognizable Chrome web driver installed on your device. This is typically bundled within a Chrome browser.
 
 ## Usage
 
 To use the tool, navigate to the project directory and run the script with the required options. Example below:
 
 ```bash
-zimo_web_screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
+zimo-web-screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
 - `-w`, `--width`: Width of the browser window (default: `1600`)
 - `-H`, `--height`: Height of the browser window (default: `900`)
 - `-t`, `--theme`: Theme name to apply (default: `pixelland`)
```

