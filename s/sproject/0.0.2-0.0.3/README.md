# Comparing `tmp/sproject-0.0.2.tar.gz` & `tmp/sproject-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sproject-0.0.2.tar", last modified: Fri Apr  5 04:25:28 2024, max compression
+gzip compressed data, was "sproject-0.0.3.tar", last modified: Mon Apr 15 03:38:29 2024, max compression
```

## Comparing `sproject-0.0.2.tar` & `sproject-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 04:25:28.422887 sproject-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-03-22 06:19:00.000000 sproject-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      156 2024-04-05 04:25:28.422887 sproject-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2024-03-22 06:19:00.000000 sproject-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 04:25:28.422887 sproject-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      423 2024-04-05 04:25:23.000000 sproject-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:25:28.379498 sproject-0.0.2/sproject/
--rw-rw-rw-   0        0        0        0 2024-03-22 05:32:47.000000 sproject-0.0.2/sproject/__init__.py
--rw-rw-rw-   0        0        0     3360 2024-04-04 15:49:55.000000 sproject-0.0.2/sproject/file_organizer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:25:28.422887 sproject-0.0.2/sproject.egg-info/
--rw-rw-rw-   0        0        0      156 2024-04-05 04:25:28.000000 sproject-0.0.2/sproject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-04-05 04:25:28.000000 sproject-0.0.2/sproject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:25:28.000000 sproject-0.0.2/sproject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 04:25:28.000000 sproject-0.0.2/sproject.egg-info/top_level.txt
+drwx------   0 root         (0) root         (0)        0 2024-04-15 03:38:29.000000 sproject-0.0.3/
+-rw-------   0 root         (0) root         (0)     1070 2024-04-07 05:12:27.000000 sproject-0.0.3/LICENSE.txt
+-rw-------   0 root         (0) root         (0)      150 2024-04-15 03:38:29.000000 sproject-0.0.3/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1425 2024-04-07 05:12:27.000000 sproject-0.0.3/README.md
+-rw-------   0 root         (0) root         (0)       38 2024-04-15 03:38:29.000000 sproject-0.0.3/setup.cfg
+-rw-------   0 root         (0) root         (0)      423 2024-04-15 03:37:10.000000 sproject-0.0.3/setup.py
+drwx------   0 root         (0) root         (0)        0 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject/
+-rw-------   0 root         (0) root         (0)        0 2024-04-07 05:12:28.000000 sproject-0.0.3/sproject/__init__.py
+-rw-------   0 root         (0) root         (0)     6634 2024-04-15 03:23:29.000000 sproject-0.0.3/sproject/file_organizer.py
+drwx------   0 root         (0) root         (0)        0 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/
+-rw-------   0 root         (0) root         (0)      150 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      206 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        9 2024-04-15 03:38:29.000000 sproject-0.0.3/sproject.egg-info/top_level.txt
```

### Comparing `sproject-0.0.2/LICENSE.txt` & `sproject-0.0.3/LICENSE.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Ram Nikhilesh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Ram Nikhilesh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sproject-0.0.2/README.md` & `sproject-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# API for finding same type of files and copy in a specific path
-
-[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)   
-
-[Follow Doveloper](https://www.instagram.com/nicky_connects/?next=%2F)
-## Functionality of the Music Player
-
-- Better Optimization
-- Pause/Play Supported
-- Add/Delete songs from Playlist
-- Previous/Next song function
-- Time duration of song / next song displays
-- List of all the songs.
-- Adjust Volume
-- Automatically Playing in Queue
-- Play Selected song from Playlist
-
-## Usage
-
-- Make sure you have Python installed in your system.
-- Run Following command in the CMD.
- ```
-  pip install NTools
-  ```
-## Example
-
- ```
- #test.py
-from NTools import copy_files
-
-#Make sure you entered the correct file extension.
-extension = '.pdf'
-
-# enter the source and destination path as follows
-s_path = "your source directory"
-d_path = "your destination directory"
-
-# Now the Function call should be like this
-copy_files(s_path,d_path,extension)
-  ```
-
-## Run the following Script.
- ```
-  python test.py
- ```
-
-## Output 
-- x files copied
-- No files found with the extension
-
-## Note 
-- I have tried to implement all the functionality, it might have some bugs also. Ignore that or please try to solve that bug.
+# API for finding same type of files and copy in a specific path
+
+[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
+[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)   
+
+[Follow Doveloper](https://www.instagram.com/nicky_connects/?next=%2F)
+## Functionality of the Music Player
+
+- Better Optimization
+- Pause/Play Supported
+- Add/Delete songs from Playlist
+- Previous/Next song function
+- Time duration of song / next song displays
+- List of all the songs.
+- Adjust Volume
+- Automatically Playing in Queue
+- Play Selected song from Playlist
+
+## Usage
+
+- Make sure you have Python installed in your system.
+- Run Following command in the CMD.
+ ```
+  pip install NTools
+  ```
+## Example
+
+ ```
+ #test.py
+from NTools import copy_files
+
+#Make sure you entered the correct file extension.
+extension = '.pdf'
+
+# enter the source and destination path as follows
+s_path = "your source directory"
+d_path = "your destination directory"
+
+# Now the Function call should be like this
+copy_files(s_path,d_path,extension)
+  ```
+
+## Run the following Script.
+ ```
+  python test.py
+ ```
+
+## Output 
+- x files copied
+- No files found with the extension
+
+## Note 
+- I have tried to implement all the functionality, it might have some bugs also. Ignore that or please try to solve that bug.
```

