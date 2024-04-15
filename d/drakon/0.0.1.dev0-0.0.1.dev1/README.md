# Comparing `tmp/drakon-0.0.1.dev0-py3-none-any.whl.zip` & `tmp/drakon-0.0.1.dev1-py3-none-any.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,170 +1,162 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      5971 (0000000000001753h)
-  Actual end-cent-dir record offset:          5949 (000000000000173Dh)
-  Expected end-cent-dir record offset:        5949 (000000000000173Dh)
+  Zip archive file size:                      5921 (0000000000001721h)
+  Actual end-cent-dir record offset:          5899 (000000000000170Bh)
+  Expected end-cent-dir record offset:        5899 (000000000000170Bh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 5 entries.
-  The central directory is 433 (00000000000001B1h) bytes long,
+  The central directory is 409 (0000000000000199h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 5516 (000000000000158Ch).
+  is 5490 (0000000000001572h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  drakon-0.0.1.dev0.dist-info/LICENSE
+  drakon-0.0.1.dev1.dist-info/LICENSE
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2019 Oct 17 22:30:32
+  file last modified on (DOS date/time):          2024 Apr 15 00:05:56
   32-bit CRC value (hex):                         095fec5b
   compressed size:                                3955 bytes
   uncompressed size:                              11361 bytes
   length of filename:                             35 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  drakon-0.0.1.dev0.dist-info/METADATA
+  drakon-0.0.1.dev1.dist-info/METADATA
 
   offset of local header from start of archive:   4020
                                                   (0000000000000FB4h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2019 Oct 17 18:31:02
-  file last modified on (UT extra field modtime): 2019 Oct 17 22:31:01 local
-  file last modified on (UT extra field modtime): 2019 Oct 17 22:31:01 UTC
-  32-bit CRC value (hex):                         e055f7dd
-  compressed size:                                855 bytes
-  uncompressed size:                              2347 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 00:05:56
+  32-bit CRC value (hex):                         878c98da
+  compressed size:                                856 bytes
+  uncompressed size:                              2465 bytes
   length of filename:                             36 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100600 octal):            -rw-------
+  apparent file type:                             binary
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 e8 03 00 00 04 e8 03 00 00.
-
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  drakon-0.0.1.dev0.dist-info/WHEEL
+  drakon-0.0.1.dev1.dist-info/WHEEL
 
-  offset of local header from start of archive:   4969
-                                                  (0000000000001369h) bytes
+  offset of local header from start of archive:   4942
+                                                  (000000000000134Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2019 Oct 17 22:30:32
-  32-bit CRC value (hex):                         7295a9ca
+  file last modified on (DOS date/time):          2024 Apr 15 00:05:56
+  32-bit CRC value (hex):                         4b7b0efc
   compressed size:                                92 bytes
   uncompressed size:                              92 bytes
   length of filename:                             33 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  drakon-0.0.1.dev0.dist-info/top_level.txt
+  drakon-0.0.1.dev1.dist-info/top_level.txt
 
-  offset of local header from start of archive:   5124
-                                                  (0000000000001404h) bytes
+  offset of local header from start of archive:   5097
+                                                  (00000000000013E9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2019 Oct 17 22:30:32
+  file last modified on (DOS date/time):          2024 Apr 15 00:05:56
   32-bit CRC value (hex):                         32d70693
   compressed size:                                3 bytes
   uncompressed size:                              1 bytes
   length of filename:                             41 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  drakon-0.0.1.dev0.dist-info/RECORD
+  drakon-0.0.1.dev1.dist-info/RECORD
 
-  offset of local header from start of archive:   5198
-                                                  (000000000000144Eh) bytes
+  offset of local header from start of archive:   5171
+                                                  (0000000000001433h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2019 Oct 17 22:30:32
-  32-bit CRC value (hex):                         7d712364
-  compressed size:                                254 bytes
+  file last modified on (DOS date/time):          2024 Apr 15 00:05:56
+  32-bit CRC value (hex):                         ece74980
+  compressed size:                                255 bytes
   uncompressed size:                              406 bytes
   length of filename:                             34 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (000664 octal):            ?rw-rw-r--
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: drakon-0.0.1.dev0.dist-info/LICENSE
+Filename: drakon-0.0.1.dev1.dist-info/LICENSE
 Comment: 
 
-Filename: drakon-0.0.1.dev0.dist-info/METADATA
+Filename: drakon-0.0.1.dev1.dist-info/METADATA
 Comment: 
 
-Filename: drakon-0.0.1.dev0.dist-info/WHEEL
+Filename: drakon-0.0.1.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: drakon-0.0.1.dev0.dist-info/top_level.txt
+Filename: drakon-0.0.1.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: drakon-0.0.1.dev0.dist-info/RECORD
+Filename: drakon-0.0.1.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `drakon-0.0.1.dev0.dist-info/LICENSE` & `drakon-0.0.1.dev1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `drakon-0.0.1.dev0.dist-info/METADATA` & `drakon-0.0.1.dev1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: drakon
-Version: 0.0.1.dev0
-Summary: Drakon is LLVM-based HotSpot-style Optimizing JIT Compiler for CPython
-Home-page: https://www.drakon.cc
+Version: 0.0.1.dev1
+Summary: Drakon is an LLVM-based Optimizing JIT Compiler for CPython
+Home-page: https://www.drakon.dev
+Download-URL: https://pypi.com/project/drakon
 Author: Karellen, Inc.
 Author-email: supervisor@karellen.co
 Maintainer: Arcadiy Ivanov
-Maintainer-email: arcadiy@ivanov.biz
+Maintainer-email: arcadiy@karellen.co
 License: Apache License, Version 2.0
-Download-URL: https://pypi.com/project/drakon
 Project-URL: Bug Tracker, https://github.com/karellen/drakon/issues
 Project-URL: Source Code, https://github.com/karellen/drakon/
-Project-URL: Documentation, https://www.drakon.cc
-Project-URL: Website, https://www.drakon.cc
+Project-URL: Documentation, https://www.drakon.dev
+Project-URL: Website, https://www.drakon.dev
 Keywords: cpython python jit llvm compiler
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Assemblers
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: <3.9,>=3.6
+Requires-Python: <3.13,>=3.6
 Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE
 
-========================================================================
- Drakon is LLVM-based HotSpot-style Optimizing JIT Compiler for CPython
-========================================================================
+=============================================================
+ Drakon is an LLVM-based Optimizing JIT Compiler for CPython
+=============================================================
 
 .. warning::
     HIC SUNT DRACONES!!! (pun intended)
 
     There is nothing to see here for now. Stay away.
 
 Problem
```

