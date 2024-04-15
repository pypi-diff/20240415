# Comparing `tmp/mseedindex-3.0.4.tar.gz` & `tmp/mseedindex-3.0.5.tar.gz`

## Comparing `mseedindex-3.0.4.tar` & `mseedindex-3.0.5.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mseedindex-3.0.4/.clang-format
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 mseedindex-3.0.4/ChangeLog
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 mseedindex-3.0.4/Makefile
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 mseedindex-3.0.4/Makefile.win
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 mseedindex-3.0.4/doc/database-schema.txt
--rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 mseedindex-3.0.4/doc/mseedindex.1
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 mseedindex-3.0.4/doc/mseedindex.md
--rwxr-xr-x   0        0        0    25790 2020-02-02 00:00:00.000000 mseedindex-3.0.4/extra/fetchIndexInfo.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/.clang-format
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/.gitignore
--rw-r--r--   0        0        0    58778 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/ChangeLog
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/INSTALL.md
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/LICENSE
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/Makefile
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/Makefile.win
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/README.byteorder
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/README.md
--rw-r--r--   0        0        0    35946 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/crc32c.c
--rw-r--r--   0        0        0    39729 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/extraheaders.c
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/extraheaders.h
--rw-r--r--   0        0        0    34982 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/fileutils.c
--rw-r--r--   0        0        0    57240 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/genutils.c
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/gmtime64.c
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/gmtime64.h
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/libmseed.def
--rw-r--r--   0        0        0    63260 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/libmseed.h
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/libmseed.map
--rw-r--r--   0        0        0    20562 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/logging.c
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/lookup.c
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/mseed.pc.in
--rw-r--r--   0        0        0    32754 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/mseedformat.h
--rw-r--r--   0        0        0    22966 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/msio.c
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/msio.h
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/msrutils.c
--rw-r--r--   0        0        0    70965 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/pack.c
--rw-r--r--   0        0        0    22238 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/packdata.c
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/packdata.h
--rw-r--r--   0        0        0    55930 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/parseutils.c
--rw-r--r--   0        0        0    26348 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/selection.c
--rw-r--r--   0        0        0    76989 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/tracelist.c
--rw-r--r--   0        0        0    57962 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/unpack.c
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/unpack.h
--rw-r--r--   0        0        0    29345 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/unpackdata.c
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/unpackdata.h
--rw-r--r--   0        0        0   353726 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/yyjson.c
--rw-r--r--   0        0        0   306476 2020-02-02 00:00:00.000000 mseedindex-3.0.4/libmseed/yyjson.h
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mseedindex-3.0.4/python/README.md
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 mseedindex-3.0.4/python/__main__.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 mseedindex-3.0.4/python/hatch_build_mseedindex.py
--rw-r--r--   0        0        0  8847710 2020-02-02 00:00:00.000000 mseedindex-3.0.4/sqlite/sqlite3.c
--rw-r--r--   0        0        0   628463 2020-02-02 00:00:00.000000 mseedindex-3.0.4/sqlite/sqlite3.h
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/Makefile
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/Makefile.win
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/asprintf.c
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/asprintf.h
--rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/md5.c
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/md5.h
--rw-r--r--   0        0        0    81628 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/mseedindex.c
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/sha256.c
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 mseedindex-3.0.4/src/sha256.h
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 mseedindex-3.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedindex-3.0.4/LICENSE
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 mseedindex-3.0.4/README.md
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mseedindex-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 mseedindex-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mseedindex-3.0.5/.clang-format
+-rw-r--r--   0        0        0     8090 2020-02-02 00:00:00.000000 mseedindex-3.0.5/ChangeLog
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 mseedindex-3.0.5/Makefile
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 mseedindex-3.0.5/Makefile.win
+-rwxr-xr-x   0        0        0  1639464 2020-02-02 00:00:00.000000 mseedindex-3.0.5/mseedindex
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 mseedindex-3.0.5/doc/database-schema.txt
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 mseedindex-3.0.5/doc/mseedindex.1
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 mseedindex-3.0.5/doc/mseedindex.md
+-rwxr-xr-x   0        0        0    25790 2020-02-02 00:00:00.000000 mseedindex-3.0.5/extra/fetchIndexInfo.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/.clang-format
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/.gitignore
+-rw-r--r--   0        0        0    58778 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/ChangeLog
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/INSTALL.md
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/LICENSE
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/Makefile
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/Makefile.win
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/README.byteorder
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/README.md
+-rw-r--r--   0        0        0    35946 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/crc32c.c
+-rw-r--r--   0        0        0    39729 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/extraheaders.c
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/extraheaders.h
+-rw-r--r--   0        0        0    34982 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/fileutils.c
+-rw-r--r--   0        0        0    57240 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/genutils.c
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/gmtime64.c
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/gmtime64.h
+-rw-r--r--   0        0        0  2007080 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/libmseed.a
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/libmseed.def
+-rw-r--r--   0        0        0    63260 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/libmseed.h
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/libmseed.map
+-rw-r--r--   0        0        0    20562 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/logging.c
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/lookup.c
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/mseed.pc.in
+-rw-r--r--   0        0        0    32754 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/mseedformat.h
+-rw-r--r--   0        0        0    22966 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/msio.c
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/msio.h
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/msrutils.c
+-rw-r--r--   0        0        0    70965 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/pack.c
+-rw-r--r--   0        0        0    22238 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/packdata.c
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/packdata.h
+-rw-r--r--   0        0        0    55930 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/parseutils.c
+-rw-r--r--   0        0        0    26348 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/selection.c
+-rw-r--r--   0        0        0    76989 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/tracelist.c
+-rw-r--r--   0        0        0    57962 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/unpack.c
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/unpack.h
+-rw-r--r--   0        0        0    29345 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/unpackdata.c
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/unpackdata.h
+-rw-r--r--   0        0        0   353726 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/yyjson.c
+-rw-r--r--   0        0        0   306476 2020-02-02 00:00:00.000000 mseedindex-3.0.5/libmseed/yyjson.h
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mseedindex-3.0.5/python/README.md
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 mseedindex-3.0.5/python/__main__.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 mseedindex-3.0.5/python/hatch_build_mseedindex.py
+-rw-r--r--   0        0        0  8847710 2020-02-02 00:00:00.000000 mseedindex-3.0.5/sqlite/sqlite3.c
+-rw-r--r--   0        0        0   628463 2020-02-02 00:00:00.000000 mseedindex-3.0.5/sqlite/sqlite3.h
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/Makefile
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/Makefile.win
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/asprintf.c
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/asprintf.h
+-rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/md5.c
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/md5.h
+-rw-r--r--   0        0        0    81985 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/mseedindex.c
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/sha256.c
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 mseedindex-3.0.5/src/sha256.h
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 mseedindex-3.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 mseedindex-3.0.5/LICENSE
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 mseedindex-3.0.5/README.md
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 mseedindex-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 mseedindex-3.0.5/PKG-INFO
```

### Comparing `mseedindex-3.0.4/ChangeLog` & `mseedindex-3.0.5/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024.106: 3.0.5
+	- Change timestamps in JSON output to nanosecond epoch values to retain
+	nanosecond resolution.  Add formatted date-time strings for summary values.
+
 2024.032: 3.0.4
 	- Add WITHOUTURL build variable to disable building with URL support.
 	- Prefer /usr/bin/curl-config over any other curl-config.
 	- Replace setup.py with pyproject.toml for PyPI building hook.
 	- Update extra/fetchIndexInfo.py illustration example.
 	- Update libmseed to v3.1.1.
```

### Comparing `mseedindex-3.0.4/Makefile` & `mseedindex-3.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/doc/database-schema.txt` & `mseedindex-3.0.5/doc/database-schema.txt`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/doc/mseedindex.1` & `mseedindex-3.0.5/doc/mseedindex.1`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/doc/mseedindex.md` & `mseedindex-3.0.5/doc/mseedindex.md`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/extra/fetchIndexInfo.py` & `mseedindex-3.0.5/extra/fetchIndexInfo.py`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/ChangeLog` & `mseedindex-3.0.5/libmseed/ChangeLog`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/INSTALL.md` & `mseedindex-3.0.5/libmseed/INSTALL.md`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/LICENSE` & `mseedindex-3.0.5/libmseed/LICENSE`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/Makefile` & `mseedindex-3.0.5/libmseed/Makefile`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/Makefile.win` & `mseedindex-3.0.5/libmseed/Makefile.win`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/README.byteorder` & `mseedindex-3.0.5/libmseed/README.byteorder`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/README.md` & `mseedindex-3.0.5/libmseed/README.md`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/crc32c.c` & `mseedindex-3.0.5/libmseed/crc32c.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/extraheaders.c` & `mseedindex-3.0.5/libmseed/extraheaders.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/extraheaders.h` & `mseedindex-3.0.5/libmseed/extraheaders.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/fileutils.c` & `mseedindex-3.0.5/libmseed/fileutils.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/genutils.c` & `mseedindex-3.0.5/libmseed/genutils.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/gmtime64.c` & `mseedindex-3.0.5/libmseed/gmtime64.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/libmseed.def` & `mseedindex-3.0.5/libmseed/libmseed.def`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/libmseed.h` & `mseedindex-3.0.5/libmseed/libmseed.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/logging.c` & `mseedindex-3.0.5/libmseed/logging.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/lookup.c` & `mseedindex-3.0.5/libmseed/lookup.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/mseedformat.h` & `mseedindex-3.0.5/libmseed/mseedformat.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/msio.c` & `mseedindex-3.0.5/libmseed/msio.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/msio.h` & `mseedindex-3.0.5/libmseed/msio.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/msrutils.c` & `mseedindex-3.0.5/libmseed/msrutils.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/pack.c` & `mseedindex-3.0.5/libmseed/pack.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/packdata.c` & `mseedindex-3.0.5/libmseed/packdata.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/packdata.h` & `mseedindex-3.0.5/libmseed/packdata.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/parseutils.c` & `mseedindex-3.0.5/libmseed/parseutils.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/selection.c` & `mseedindex-3.0.5/libmseed/selection.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/tracelist.c` & `mseedindex-3.0.5/libmseed/tracelist.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/unpack.c` & `mseedindex-3.0.5/libmseed/unpack.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/unpack.h` & `mseedindex-3.0.5/libmseed/unpack.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/unpackdata.c` & `mseedindex-3.0.5/libmseed/unpackdata.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/unpackdata.h` & `mseedindex-3.0.5/libmseed/unpackdata.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/yyjson.c` & `mseedindex-3.0.5/libmseed/yyjson.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/libmseed/yyjson.h` & `mseedindex-3.0.5/libmseed/yyjson.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/python/hatch_build_mseedindex.py` & `mseedindex-3.0.5/python/hatch_build_mseedindex.py`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/sqlite/sqlite3.c` & `mseedindex-3.0.5/sqlite/sqlite3.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/sqlite/sqlite3.h` & `mseedindex-3.0.5/sqlite/sqlite3.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/src/Makefile` & `mseedindex-3.0.5/src/Makefile`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/src/asprintf.c` & `mseedindex-3.0.5/src/asprintf.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/src/asprintf.h` & `mseedindex-3.0.5/src/asprintf.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/src/md5.c` & `mseedindex-3.0.5/src/md5.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/src/md5.h` & `mseedindex-3.0.5/src/md5.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/src/mseedindex.c` & `mseedindex-3.0.5/src/mseedindex.c`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 #define asprintf internal_asprintf
 #define vasprintf internal_vasprintf
 #endif
 
 #include "md5.h"
 #include "sha256.h"
 
-#define VERSION "3.0.4"
+#define VERSION "3.0.5"
 #define PACKAGE "mseedindex"
 
 static flag verbose = 0;
 static flag skipnotdata = 0;      /* Used to control skipping of non-miniSEED data */
 static char keeppath = 0;         /* Use originally specified path, do not resolve absolute */
 static flag nosync = 0;           /* Control synchronization with database, 1 = no database */
 static flag noupdate = 0;         /* Control replacement of rows in database, 1 = no updating */
@@ -1821,16 +1821,16 @@
   struct filelink *flp = NULL;
 
   struct sectiondetails *sd;
   MS3TraceID *secid = NULL;
   int64_t bytecount;
   nstime_t earliest_ts = NSTUNSET;
   nstime_t latest_ts = NSTUNSET;
-  char earliest[64];
-  char latest[64];
+  char start_string[64];
+  char end_string[64];
   char pathmod[64];
   char updated[64];
   char scanned[64];
   char *formatstr;
   int format = -1;
 
   struct timeindex *tindex;
@@ -1911,21 +1911,23 @@
         latest_ts = sd->latest;
 
       /* Create and populate content array object entry */
       content = yyjson_mut_obj (rootdoc);
 
       yyjson_mut_ptr_add (content, "/source_id", yyjson_mut_strcpy (rootdoc, secid->sid), rootdoc);
 
-      /* Create earliest and latest and other time strings */
-      ms_nstime2timestr (sd->earliest, earliest, ISOMONTHDAY_Z, NANO_MICRO);
-      ms_nstime2timestr (sd->latest, latest, ISOMONTHDAY_Z, NANO_MICRO);
+      /* Create start and end and other time strings */
+      ms_nstime2timestr (sd->earliest, start_string, ISOMONTHDAY_Z, NANO_MICRO);
+      ms_nstime2timestr (sd->latest, end_string, ISOMONTHDAY_Z, NANO_MICRO);
       ms_nstime2timestr (MS_EPOCH2NSTIME(sd->updated), updated, ISOMONTHDAY_Z, NONE);
 
-      yyjson_mut_ptr_add (content, "/start", yyjson_mut_strcpy (rootdoc, earliest), rootdoc);
-      yyjson_mut_ptr_add (content, "/end", yyjson_mut_strcpy (rootdoc, latest), rootdoc);
+      yyjson_mut_ptr_add (content, "/start_string", yyjson_mut_strcpy (rootdoc, start_string), rootdoc);
+      yyjson_mut_ptr_add (content, "/end_string", yyjson_mut_strcpy (rootdoc, end_string), rootdoc);
+      yyjson_mut_ptr_add (content, "/start", yyjson_mut_sint (rootdoc, sd->earliest), rootdoc);
+      yyjson_mut_ptr_add (content, "/end", yyjson_mut_sint (rootdoc, sd->latest), rootdoc);
       yyjson_mut_ptr_add (content, "/updated", yyjson_mut_strcpy (rootdoc, updated), rootdoc);
 
       yyjson_mut_ptr_add (content, "/publication_version", yyjson_mut_int (rootdoc, secid->pubversion), rootdoc);
       yyjson_mut_ptr_add (content, "/byte_offset", yyjson_mut_sint (rootdoc, sd->startoffset), rootdoc);
       yyjson_mut_ptr_add (content, "/byte_count", yyjson_mut_sint (rootdoc, bytecount), rootdoc);
 
       yyjson_mut_ptr_add (content, "/md5", yyjson_mut_strcpy (rootdoc, sd->digeststr), rootdoc);
@@ -1941,15 +1943,15 @@
 
         yyjson_mut_ptr_add (content, "/ts_time_byteoffset", yyjson_mut_arr (rootdoc), rootdoc);
 
         while (tindex)
         {
           obj = yyjson_mut_obj (rootdoc);
 
-          yyjson_mut_ptr_add (obj, "/timestamp", yyjson_mut_real (rootdoc, (double)MS_NSTIME2EPOCH(tindex->time)), rootdoc);
+          yyjson_mut_ptr_add (obj, "/timestamp", yyjson_mut_sint (rootdoc, tindex->time), rootdoc);
           yyjson_mut_ptr_add (obj, "/offset", yyjson_mut_sint (rootdoc, tindex->byteoffset), rootdoc);
 
           yyjson_mut_ptr_add (content, "/ts_time_byteoffset/-", obj, rootdoc);
 
           tindex = tindex->next;
         }
       }
@@ -1968,16 +1970,16 @@
         while (id)
         {
           seg = id->first;
           while (seg)
           {
             obj = yyjson_mut_obj (rootdoc);
 
-            yyjson_mut_ptr_add (obj, "/start", yyjson_mut_real (rootdoc, (double)MS_NSTIME2EPOCH(seg->starttime)), rootdoc);
-            yyjson_mut_ptr_add (obj, "/end", yyjson_mut_real (rootdoc, (double)MS_NSTIME2EPOCH(seg->endtime)), rootdoc);
+            yyjson_mut_ptr_add (obj, "/start", yyjson_mut_sint (rootdoc, seg->starttime), rootdoc);
+            yyjson_mut_ptr_add (obj, "/end", yyjson_mut_sint (rootdoc, seg->endtime), rootdoc);
             yyjson_mut_ptr_add (obj, "/sample_rate", yyjson_mut_real (rootdoc, seg->samprate), rootdoc);
 
             yyjson_mut_ptr_add (content, "/ts_timespans/-", obj, rootdoc);
 
             seg = seg->next;
           }
 
@@ -2006,19 +2008,21 @@
       ms_nstime2timestr (MS_EPOCH2NSTIME (flp->filemodtime), pathmod, ISOMONTHDAY_Z, NONE);
       yyjson_mut_ptr_add (pathobj, "/path_modtime", yyjson_mut_strcpy (rootdoc, pathmod), rootdoc);
     }
 
     ms_nstime2timestr (MS_EPOCH2NSTIME (flp->scantime), scanned, ISOMONTHDAY_Z, NONE);
     yyjson_mut_ptr_add (pathobj, "/path_indextime", yyjson_mut_strcpy (rootdoc, scanned), rootdoc);
 
-    ms_nstime2timestr (earliest_ts, earliest, ISOMONTHDAY_Z, NANO_MICRO);
-    ms_nstime2timestr (latest_ts, latest, ISOMONTHDAY_Z, NANO_MICRO);
+    ms_nstime2timestr (earliest_ts, start_string, ISOMONTHDAY_Z, NANO_MICRO);
+    ms_nstime2timestr (latest_ts, end_string, ISOMONTHDAY_Z, NANO_MICRO);
 
-    yyjson_mut_ptr_add (pathobj, "/start", yyjson_mut_strcpy (rootdoc, earliest), rootdoc);
-    yyjson_mut_ptr_add (pathobj, "/end", yyjson_mut_strcpy (rootdoc, latest), rootdoc);
+    yyjson_mut_ptr_add (pathobj, "/start_string", yyjson_mut_strcpy (rootdoc, start_string), rootdoc);
+    yyjson_mut_ptr_add (pathobj, "/end_string", yyjson_mut_strcpy (rootdoc, end_string), rootdoc);
+    yyjson_mut_ptr_add (pathobj, "/start", yyjson_mut_sint (rootdoc, earliest_ts), rootdoc);
+    yyjson_mut_ptr_add (pathobj, "/end", yyjson_mut_sint (rootdoc, latest_ts), rootdoc);
 
     /* Add content object to content array */
     yyjson_mut_ptr_add (pathobj, "/content", content_arr, rootdoc);
 
     flp = flp->next;
   } /* End of looping over file list for synchronization */
```

### Comparing `mseedindex-3.0.4/src/sha256.c` & `mseedindex-3.0.5/src/sha256.c`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/src/sha256.h` & `mseedindex-3.0.5/src/sha256.h`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/LICENSE` & `mseedindex-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/README.md` & `mseedindex-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/pyproject.toml` & `mseedindex-3.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mseedindex-3.0.4/PKG-INFO` & `mseedindex-3.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mseedindex
-Version: 3.0.4
+Version: 3.0.5
 Summary: A Python package entry for building the C-based mseedindex program
 Project-URL: Homepage, https://github.com/EarthScope/mseedindex
 Project-URL: Issues, https://github.com/EarthScope/mseedindex/issues
 Author-email: EarthScope Data Services <software@earthscope.org>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: data,miniseed,mseed,seismic,seismology,waveform
```

