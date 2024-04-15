# Comparing `tmp/zimo-web-screenshot-0.1.0.tar.gz` & `tmp/zimo_web_screenshot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimo-web-screenshot-0.1.0.tar", last modified: Mon Apr 15 10:41:10 2024, max compression
+gzip compressed data, was "zimo_web_screenshot-0.1.1.tar", last modified: Mon Apr 15 11:33:02 2024, max compression
```

## Comparing `zimo-web-screenshot-0.1.0.tar` & `zimo_web_screenshot-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:41:10.311441 zimo-web-screenshot-0.1.0/
--rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo-web-screenshot-0.1.0/LICENSE
--rw-r--r--   0 zimoluo    (501) staff       (20)     2195 2024-04-15 10:41:10.311507 zimo-web-screenshot-0.1.0/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)     1690 2024-04-15 05:55:10.000000 zimo-web-screenshot-0.1.0/README.md
--rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-04-15 10:41:10.311694 zimo-web-screenshot-0.1.0/setup.cfg
--rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-04-15 10:39:36.000000 zimo-web-screenshot-0.1.0/setup.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:41:10.310612 zimo-web-screenshot-0.1.0/zimo_web_screenshot/
--rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot/__init__.py
--rw-r--r--   0 zimoluo    (501) staff       (20)     2254 2024-04-15 05:05:14.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot/screenshot.py
-drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:41:10.311344 zimo-web-screenshot-0.1.0/zimo_web_screenshot.egg-info/
--rw-r--r--   0 zimoluo    (501) staff       (20)     2195 2024-04-15 10:41:10.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot.egg-info/PKG-INFO
--rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-04-15 10:41:10.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot.egg-info/SOURCES.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-04-15 10:41:10.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot.egg-info/dependency_links.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-04-15 10:41:10.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot.egg-info/entry_points.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-04-15 10:41:10.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot.egg-info/requires.txt
--rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-04-15 10:41:10.000000 zimo-web-screenshot-0.1.0/zimo_web_screenshot.egg-info/top_level.txt
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:33:02.637790 zimo_web_screenshot-0.1.1/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1057 2024-04-15 05:14:35.000000 zimo_web_screenshot-0.1.1/LICENSE
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2160 2024-04-15 11:33:02.637875 zimo_web_screenshot-0.1.1/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)     1655 2024-04-15 11:32:37.000000 zimo_web_screenshot-0.1.1/README.md
+-rw-r--r--   0 zimoluo    (501) staff       (20)       79 2024-04-15 11:33:02.638064 zimo_web_screenshot-0.1.1/setup.cfg
+-rw-r--r--   0 zimoluo    (501) staff       (20)      888 2024-04-15 11:30:24.000000 zimo_web_screenshot-0.1.1/setup.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:33:02.636613 zimo_web_screenshot-0.1.1/zimo_web_screenshot/
+-rw-r--r--   0 zimoluo    (501) staff       (20)        0 2024-04-15 10:38:36.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot/__init__.py
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2254 2024-04-15 05:05:14.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot/screenshot.py
+drwxr-xr-x   0 zimoluo    (501) staff       (20)        0 2024-04-15 11:33:02.637677 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/
+-rw-r--r--   0 zimoluo    (501) staff       (20)     2160 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/PKG-INFO
+-rw-r--r--   0 zimoluo    (501) staff       (20)      362 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/SOURCES.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        1 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/dependency_links.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       76 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/entry_points.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)        9 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/requires.txt
+-rw-r--r--   0 zimoluo    (501) staff       (20)       20 2024-04-15 11:33:02.000000 zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/top_level.txt
```

### Comparing `zimo-web-screenshot-0.1.0/LICENSE` & `zimo_web_screenshot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zimo-web-screenshot-0.1.0/PKG-INFO` & `zimo_web_screenshot-0.1.1/zimo_web_screenshot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimo-web-screenshot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple CLI tool to take screenshots of Zimo Web pages with Selenium.
 Home-page: https://github.com/zimoluo/zimo-web-screenshot-tool
 Author: Zimo Luo
 Author-email: abgkings0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,35 +22,30 @@
 - Set browser window dimensions.
 - Apply custom themes.
 - Configure delays for screenshots to wait for dynamic content to load.
 - Save screenshots locally in PNG format.
 
 ## Installation
 
-To run this tool, you'll need Python and Selenium. Here are the steps to set it up:
+To use this tool, you'll need Python installed on your system. The tool also requires Selenium, which will be automatically installed when you install the package from PyPI.
 
-1. **Clone the repository**:
+1. **Install the Package**:
+   You can install `zimo_web_screenshot` directly from PyPI using pip:
    ```bash
-   git clone https://github.com/zimoluo/zimo-web-screenshot-tool.git
-   cd zimo-web-screenshot-tool
+   pip install zimo_web_screenshot
    ```
-2. **Install dependencies**:
-   You will need Python and pip installed. Then, you can install Selenium:
-   ```bash
-   pip install selenium
-   ```
-3. **Web Driver**:
-   You need to have at least one recognizable web driver installed on your device. This is typically bundled within a Chrome browser.
+2. **Install a Web Driver**:
+   You need to have at least one recognizable Chrome web driver installed on your device. This is typically bundled within a Chrome browser.
 
 ## Usage
 
 To use the tool, navigate to the project directory and run the script with the required options. Example below:
 
 ```bash
-python screenshot.py --width 1600 --height 900 --theme plainDark --pathname about --delay 0
+zimo_web_screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
 - `-w`, `--width`: Width of the browser window (default: `1600`)
 - `-H`, `--height`: Height of the browser window (default: `900`)
 - `-t`, `--theme`: Theme name to apply (default: `pixelland`)
```

### Comparing `zimo-web-screenshot-0.1.0/README.md` & `zimo_web_screenshot-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,35 +7,30 @@
 - Set browser window dimensions.
 - Apply custom themes.
 - Configure delays for screenshots to wait for dynamic content to load.
 - Save screenshots locally in PNG format.
 
 ## Installation
 
-To run this tool, you'll need Python and Selenium. Here are the steps to set it up:
+To use this tool, you'll need Python installed on your system. The tool also requires Selenium, which will be automatically installed when you install the package from PyPI.
 
-1. **Clone the repository**:
+1. **Install the Package**:
+   You can install `zimo_web_screenshot` directly from PyPI using pip:
    ```bash
-   git clone https://github.com/zimoluo/zimo-web-screenshot-tool.git
-   cd zimo-web-screenshot-tool
+   pip install zimo_web_screenshot
    ```
-2. **Install dependencies**:
-   You will need Python and pip installed. Then, you can install Selenium:
-   ```bash
-   pip install selenium
-   ```
-3. **Web Driver**:
-   You need to have at least one recognizable web driver installed on your device. This is typically bundled within a Chrome browser.
+2. **Install a Web Driver**:
+   You need to have at least one recognizable Chrome web driver installed on your device. This is typically bundled within a Chrome browser.
 
 ## Usage
 
 To use the tool, navigate to the project directory and run the script with the required options. Example below:
 
 ```bash
-python screenshot.py --width 1600 --height 900 --theme plainDark --pathname about --delay 0
+zimo_web_screenshot --width 1600 --height 900 --theme plainDark --pathname about --delay 0
 ```
 
 **Command Line Arguments**
 
 - `-w`, `--width`: Width of the browser window (default: `1600`)
 - `-H`, `--height`: Height of the browser window (default: `900`)
 - `-t`, `--theme`: Theme name to apply (default: `pixelland`)
```

### Comparing `zimo-web-screenshot-0.1.0/setup.py` & `zimo_web_screenshot-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='zimo-web-screenshot',
-    version='0.1.0',
+    name='zimo_web_screenshot',
+    version='0.1.1',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'selenium',
     ],
     entry_points={
         'console_scripts': [
-            'zimo-web-screenshot=zimo_web_screenshot.screenshot:main',
+            'zimo_web_screenshot=zimo_web_screenshot.screenshot:main',
         ],
     },
     author='Zimo Luo',
     author_email='abgkings0920@gmail.com',
     description='A simple CLI tool to take screenshots of Zimo Web pages with Selenium.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `zimo-web-screenshot-0.1.0/zimo_web_screenshot/screenshot.py` & `zimo_web_screenshot-0.1.1/zimo_web_screenshot/screenshot.py`

 * *Files identical despite different names*

