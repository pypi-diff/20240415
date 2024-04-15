# Comparing `tmp/caustic.lexer-1.2.0.post1.tar.gz` & `tmp/caustic.lexer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.lexer-1.2.0.post1.tar", last modified: Sat Apr 13 00:12:55 2024, max compression
+gzip compressed data, was "caustic.lexer-1.2.1.tar", last modified: Mon Apr 15 01:43:31 2024, max compression
```

## Comparing `caustic.lexer-1.2.0.post1.tar` & `caustic.lexer-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:12:55.883534 caustic.lexer-1.2.0.post1/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.2.0.post1/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     7446 2024-04-13 00:12:55.883534 caustic.lexer-1.2.0.post1/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     6508 2024-04-13 00:12:27.000000 caustic.lexer-1.2.0.post1/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1091 2024-04-13 00:12:38.000000 caustic.lexer-1.2.0.post1/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-13 00:12:55.883534 caustic.lexer-1.2.0.post1/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:12:55.873534 caustic.lexer-1.2.0.post1/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:12:55.873534 caustic.lexer-1.2.0.post1/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:12:55.880201 caustic.lexer-1.2.0.post1/src/caustic/lexer/
--rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/basic_compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     7685 2024-04-12 22:41:29.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1377 2024-04-12 23:40:42.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/grammar.cag
--rw-r--r--   0 shae      (1000) shae      (1000)    14142 2024-04-12 23:45:20.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/nodes.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3260 2024-04-13 00:12:52.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/precompiled_nodes.pkl
--rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/serialize.py
--rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.2.0.post1/src/caustic/lexer/util.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-13 00:12:55.880201 caustic.lexer-1.2.0.post1/src/caustic.lexer.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     7446 2024-04-13 00:12:55.000000 caustic.lexer-1.2.0.post1/src/caustic.lexer.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      486 2024-04-13 00:12:55.000000 caustic.lexer-1.2.0.post1/src/caustic.lexer.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-13 00:12:55.000000 caustic.lexer-1.2.0.post1/src/caustic.lexer.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-13 00:12:55.000000 caustic.lexer-1.2.0.post1/src/caustic.lexer.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-13 00:12:55.000000 caustic.lexer-1.2.0.post1/src/caustic.lexer.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.840969 caustic.lexer-1.2.1/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.2.1/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     7504 2024-04-15 01:43:31.837636 caustic.lexer-1.2.1/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     6572 2024-04-15 01:36:25.000000 caustic.lexer-1.2.1/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1089 2024-04-15 01:43:15.000000 caustic.lexer-1.2.1/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-15 01:43:31.840969 caustic.lexer-1.2.1/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.830969 caustic.lexer-1.2.1/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.830969 caustic.lexer-1.2.1/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.837636 caustic.lexer-1.2.1/src/caustic/lexer/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.2.1/src/caustic/lexer/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.2.1/src/caustic/lexer/basic_compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     7685 2024-04-12 22:41:29.000000 caustic.lexer-1.2.1/src/caustic/lexer/compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1382 2024-04-15 01:40:52.000000 caustic.lexer-1.2.1/src/caustic/lexer/grammar.cag
+-rw-r--r--   0 shae      (1000) shae      (1000)    14142 2024-04-12 23:45:20.000000 caustic.lexer-1.2.1/src/caustic/lexer/nodes.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3281 2024-04-15 01:43:29.000000 caustic.lexer-1.2.1/src/caustic/lexer/precompiled_nodes.pkl
+-rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.2.1/src/caustic/lexer/serialize.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.2.1/src/caustic/lexer/util.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-15 01:43:31.837636 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     7504 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      486 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-15 01:43:31.000000 caustic.lexer-1.2.1/src/caustic.lexer.egg-info/top_level.txt
```

### Comparing `caustic.lexer-1.2.0.post1/LICENSE` & `caustic.lexer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.0.post1/PKG-INFO` & `caustic.lexer-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.2.0.post1
+Version: 1.2.1
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -215,7 +215,10 @@
 
 ## 1.1.0
 - Added support for periods in node names
 - Fixed `Compiler.post_process_compile()` not actually doing anything
 
 ## 1.2.0
 - Implemented [unpacking](#unpack) nodes
+
+## 1.2.1
+- Fixed several nodes improperly stripping whitespace
```

### Comparing `caustic.lexer-1.2.0.post1/README.md` & `caustic.lexer-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -191,7 +191,10 @@
 
 ## 1.1.0
 - Added support for periods in node names
 - Fixed `Compiler.post_process_compile()` not actually doing anything
 
 ## 1.2.0
 - Implemented [unpacking](#unpack) nodes
+
+## 1.2.1
+- Fixed several nodes improperly stripping whitespace
```

### Comparing `caustic.lexer-1.2.0.post1/pyproject.toml` & `caustic.lexer-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.lexer"
-version = "1.2.0-1"
+version = "1.2.1"
 dependencies = [
     "buffer-matcher >= 0.1.1",
 ]
 requires-python = ">=3.12"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Grammar compilation for Caustic"
```

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/__init__.py` & `caustic.lexer-1.2.1/src/caustic/lexer/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/basic_compiler.py` & `caustic.lexer-1.2.1/src/caustic/lexer/basic_compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/compiler.py` & `caustic.lexer-1.2.1/src/caustic/lexer/compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/grammar.cag` & `caustic.lexer-1.2.1/src/caustic/lexer/grammar.cag`

 * *Files 9% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 ## NodeRange
 NODE_RANGE = min:0/\d*/ "-" ! max:1/(\d+)?/ ! node:@EXPRESSION ;
 NODE_RANGE_WS_SENSITIVE = min:0/\d*/ "~" ! max:1/(\d+)?/ node:@EXPRESSION ;
 
 # Real nodes
 ## StringNode
 STRING_NODE = :[
-    ( "\"" ! :0/(?:[^"\\]|(?:\\.))*/ "\"" )
-    ( "'" ! :0/(?:[^'\\]|(?:\\.))*/ "'" )
+    { "\"" ! :0/(?:[^"\\]|(?:\\.))*/ "\"" }
+    { "'" ! :0/(?:[^'\\]|(?:\\.))*/ "'" }
 ];
 ## PatternNode
-PATTERN_NODE = group:1/(\d*)?/ "/" ! pattern:0/(?:[^\/\\]|(?:\\.))*/ ! "/" ! flags:0/[ims]*/ ;
+PATTERN_NODE = :{ group:1/(\d*)?/ "/" ! pattern:0/(?:[^\/\\]|(?:\\.))*/ ! "/" ! flags:0/[ims]*/ } ;
 
 # Meta nodes
 STEALER = "!" ;
 CONTEXT = "<" ! :[ ( str:@STRING_NODE ) ( raw:0/\w*/ ) ] ! ">" ;
 NODEREF = "@" ! :0/[\w\.]+/ ;
```

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/nodes.py` & `caustic.lexer-1.2.1/src/caustic/lexer/nodes.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/precompiled_nodes.pkl` & `caustic.lexer-1.2.1/src/caustic/lexer/precompiled_nodes.pkl`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95b1 0c00 0000 0000 0028 4307 434f  ...........(C.CO
+00000000: 8004 95c6 0c00 0000 0000 0028 4307 434f  ...........(C.CO
 00000010: 4d4d 454e 544b 0251 2981 4e7d 288c 056e  MMENTK.Q).N}(..n
 00000020: 6f64 6573 944b 0551 2981 4e7d 288c 0673  odes.K.Q).N}(..s
 00000030: 7472 696e 6794 4301 238c 046e 616d 6594  tring.C.#..name.
 00000040: 4e75 8662 4b07 5129 814e 7d68 024e 7386  Nu.bK.Q).N}h.Ns.
 00000050: 624b 0651 2981 4e7d 288c 0770 6174 7465  bK.Q).N}(..patte
 00000060: 726e 948c 0272 658c 085f 636f 6d70 696c  rn...re.._compil
 00000070: 6593 9443 042e 2a3f 244b 0886 528c 0567  e..C..*?$K..R..g
@@ -149,56 +149,58 @@
 00000940: 004b 0351 2981 4e7d 2868 004b 0251 2981  .K.Q).N}(h.K.Q).
 00000950: 4e7d 2868 0028 4b05 5129 814e 7d28 6801  N}(h.(K.Q).N}(h.
 00000960: 4301 2294 6802 4e75 8662 4b07 5129 814e  C.".h.Nu.bK.Q).N
 00000970: 7d68 024e 7386 624b 0651 2981 4e7d 2868  }h.Ns.bK.Q).N}(h
 00000980: 0368 0443 1328 3f3a 5b5e 225c 5c5d 7c28  .h.C.(?:[^"\\]|(
 00000990: 3f3a 5c5c 2e29 292a 4b00 8652 6805 4b00  ?:\\.))*K..Rh.K.
 000009a0: 6802 680e 7586 624b 0551 2981 4e7d 2868  h.h.u.bK.Q).N}(h
-000009b0: 0168 1168 024e 7586 6274 6806 8968 024e  .h.h.Nu.bth..h.N
+000009b0: 0168 1168 024e 7586 6274 6806 8868 024e  .h.h.Nu.bth..h.N
 000009c0: 7586 624b 0251 2981 4e7d 2868 0028 4b05  u.bK.Q).N}(h.(K.
 000009d0: 5129 814e 7d28 6801 4301 2794 6802 4e75  Q).N}(h.C.'.h.Nu
 000009e0: 8662 4b07 5129 814e 7d68 024e 7386 624b  .bK.Q).N}h.Ns.bK
 000009f0: 0651 2981 4e7d 2868 0368 0443 1328 3f3a  .Q).N}(h.h.C.(?:
 00000a00: 5b5e 275c 5c5d 7c28 3f3a 5c5c 2e29 292a  [^'\\]|(?:\\.))*
 00000a10: 4b00 8652 6805 4b00 6802 680e 7586 624b  K..Rh.K.h.h.u.bK
 00000a20: 0551 2981 4e7d 2868 0168 1268 024e 7586  .Q).N}(h.h.h.Nu.
-00000a30: 6274 6806 8968 024e 7586 6286 6802 680e  bth..h.Nu.b.h.h.
+00000a30: 6274 6806 8868 024e 7586 6286 6802 680e  bth..h.Nu.b.h.h.
 00000a40: 7586 6285 6806 8968 024e 7586 6286 430c  u.b.h..h.Nu.b.C.
 00000a50: 5041 5454 4552 4e5f 4e4f 4445 4b02 5129  PATTERN_NODEK.Q)
-00000a60: 814e 7d28 6800 284b 0651 2981 4e7d 2868  .N}(h.(K.Q).N}(h
-00000a70: 0368 0443 0628 5c64 2a29 3f4b 0086 5268  .h.C.(\d*)?K..Rh
-00000a80: 054b 0168 028c 0567 726f 7570 7586 624b  .K.h...groupu.bK
-00000a90: 0551 2981 4e7d 2868 0143 012f 9468 024e  .Q).N}(h.C./.h.N
-00000aa0: 7586 624b 0751 2981 4e7d 6802 4e73 8662  u.bK.Q).N}h.Ns.b
-00000ab0: 4b06 5129 814e 7d28 6803 6804 4314 283f  K.Q).N}(h.h.C.(?
-00000ac0: 3a5b 5e5c 2f5c 5c5d 7c28 3f3a 5c5c 2e29  :[^\/\\]|(?:\\.)
-00000ad0: 292a 4b00 8652 6805 4b00 6802 8c07 7061  )*K..Rh.K.h...pa
-00000ae0: 7474 6572 6e75 8662 4b07 5129 814e 7d68  tternu.bK.Q).N}h
-00000af0: 024e 7386 624b 0551 2981 4e7d 2868 0168  .Ns.bK.Q).N}(h.h
-00000b00: 1368 024e 7586 624b 0751 2981 4e7d 6802  .h.Nu.bK.Q).N}h.
-00000b10: 4e73 8662 4b06 5129 814e 7d28 6803 6804  Ns.bK.Q).N}(h.h.
-00000b20: 4306 5b69 6d73 5d2a 4b00 8652 6805 4b00  C.[ims]*K..Rh.K.
-00000b30: 6802 8c05 666c 6167 7375 8662 7468 0689  h...flagsu.bth..
-00000b40: 6802 4e75 8662 8643 0753 5445 414c 4552  h.Nu.b.C.STEALER
-00000b50: 4b02 5129 814e 7d28 6800 4b05 5129 814e  K.Q).N}(h.K.Q).N
-00000b60: 7d28 6801 4301 2168 024e 7586 6285 6806  }(h.C.!h.Nu.b.h.
-00000b70: 8968 024e 7586 6286 4307 434f 4e54 4558  .h.Nu.b.C.CONTEX
-00000b80: 544b 0251 2981 4e7d 2868 0028 4b05 5129  TK.Q).N}(h.(K.Q)
-00000b90: 814e 7d28 6801 4301 3c68 024e 7586 624b  .N}(h.C.<h.Nu.bK
-00000ba0: 0751 2981 4e7d 6802 4e73 8662 4b03 5129  .Q).N}h.Ns.bK.Q)
-00000bb0: 814e 7d28 6800 4b02 5129 814e 7d28 6800  .N}(h.K.Q).N}(h.
-00000bc0: 4b09 5129 814e 7d28 680a 430b 5354 5249  K.Q).N}(h.C.STRI
-00000bd0: 4e47 5f4e 4f44 4568 0b4e 6802 8c03 7374  NG_NODEh.Nh...st
-00000be0: 7275 8662 8568 0689 6802 4e75 8662 4b02  ru.b.h..h.Nu.bK.
-00000bf0: 5129 814e 7d28 6800 4b06 5129 814e 7d28  Q).N}(h.K.Q).N}(
-00000c00: 6803 6804 4303 5c77 2a4b 0086 5268 054b  h.h.C.\w*K..Rh.K
-00000c10: 0068 028c 0372 6177 7586 6285 6806 8968  .h...rawu.b.h..h
-00000c20: 024e 7586 6286 6802 680e 7586 624b 0751  .Nu.b.h.h.u.bK.Q
-00000c30: 2981 4e7d 6802 4e73 8662 4b05 5129 814e  ).N}h.Ns.bK.Q).N
-00000c40: 7d28 6801 4301 3e68 024e 7586 6274 6806  }(h.C.>h.Nu.bth.
-00000c50: 8968 024e 7586 6286 4307 4e4f 4445 5245  .h.Nu.b.C.NODERE
-00000c60: 464b 0251 2981 4e7d 2868 004b 0551 2981  FK.Q).N}(h.K.Q).
-00000c70: 4e7d 2868 0143 0140 6802 4e75 8662 4b07  N}(h.C.@h.Nu.bK.
-00000c80: 5129 814e 7d68 024e 7386 624b 0651 2981  Q).N}h.Ns.bK.Q).
-00000c90: 4e7d 2868 0368 0443 075b 5c77 5c2e 5d2b  N}(h.h.C.[\w\.]+
-00000ca0: 4b00 8652 6805 4b00 6802 680e 7586 6287  K..Rh.K.h.h.u.b.
-00000cb0: 6806 8968 024e 7586 6286 742e            h..h.Nu.b.t.
+00000a60: 814e 7d28 6800 4b02 5129 814e 7d28 6800  .N}(h.K.Q).N}(h.
+00000a70: 284b 0651 2981 4e7d 2868 0368 0443 0628  (K.Q).N}(h.h.C.(
+00000a80: 5c64 2a29 3f4b 0086 5268 054b 0168 028c  \d*)?K..Rh.K.h..
+00000a90: 0567 726f 7570 7586 624b 0551 2981 4e7d  .groupu.bK.Q).N}
+00000aa0: 2868 0143 012f 9468 024e 7586 624b 0751  (h.C./.h.Nu.bK.Q
+00000ab0: 2981 4e7d 6802 4e73 8662 4b06 5129 814e  ).N}h.Ns.bK.Q).N
+00000ac0: 7d28 6803 6804 4314 283f 3a5b 5e5c 2f5c  }(h.h.C.(?:[^\/\
+00000ad0: 5c5d 7c28 3f3a 5c5c 2e29 292a 4b00 8652  \]|(?:\\.))*K..R
+00000ae0: 6805 4b00 6802 8c07 7061 7474 6572 6e75  h.K.h...patternu
+00000af0: 8662 4b07 5129 814e 7d68 024e 7386 624b  .bK.Q).N}h.Ns.bK
+00000b00: 0551 2981 4e7d 2868 0168 1368 024e 7586  .Q).N}(h.h.h.Nu.
+00000b10: 624b 0751 2981 4e7d 6802 4e73 8662 4b06  bK.Q).N}h.Ns.bK.
+00000b20: 5129 814e 7d28 6803 6804 4306 5b69 6d73  Q).N}(h.h.C.[ims
+00000b30: 5d2a 4b00 8652 6805 4b00 6802 8c05 666c  ]*K..Rh.K.h...fl
+00000b40: 6167 7375 8662 7468 0688 6802 680e 7586  agsu.bth..h.h.u.
+00000b50: 6285 6806 8968 024e 7586 6286 4307 5354  b.h..h.Nu.b.C.ST
+00000b60: 4541 4c45 524b 0251 2981 4e7d 2868 004b  EALERK.Q).N}(h.K
+00000b70: 0551 2981 4e7d 2868 0143 0121 6802 4e75  .Q).N}(h.C.!h.Nu
+00000b80: 8662 8568 0689 6802 4e75 8662 8643 0743  .b.h..h.Nu.b.C.C
+00000b90: 4f4e 5445 5854 4b02 5129 814e 7d28 6800  ONTEXTK.Q).N}(h.
+00000ba0: 284b 0551 2981 4e7d 2868 0143 013c 6802  (K.Q).N}(h.C.<h.
+00000bb0: 4e75 8662 4b07 5129 814e 7d68 024e 7386  Nu.bK.Q).N}h.Ns.
+00000bc0: 624b 0351 2981 4e7d 2868 004b 0251 2981  bK.Q).N}(h.K.Q).
+00000bd0: 4e7d 2868 004b 0951 2981 4e7d 2868 0a43  N}(h.K.Q).N}(h.C
+00000be0: 0b53 5452 494e 475f 4e4f 4445 680b 4e68  .STRING_NODEh.Nh
+00000bf0: 028c 0373 7472 7586 6285 6806 8968 024e  ...stru.b.h..h.N
+00000c00: 7586 624b 0251 2981 4e7d 2868 004b 0651  u.bK.Q).N}(h.K.Q
+00000c10: 2981 4e7d 2868 0368 0443 035c 772a 4b00  ).N}(h.h.C.\w*K.
+00000c20: 8652 6805 4b00 6802 8c03 7261 7775 8662  .Rh.K.h...rawu.b
+00000c30: 8568 0689 6802 4e75 8662 8668 0268 0e75  .h..h.Nu.b.h.h.u
+00000c40: 8662 4b07 5129 814e 7d68 024e 7386 624b  .bK.Q).N}h.Ns.bK
+00000c50: 0551 2981 4e7d 2868 0143 013e 6802 4e75  .Q).N}(h.C.>h.Nu
+00000c60: 8662 7468 0689 6802 4e75 8662 8643 074e  .bth..h.Nu.b.C.N
+00000c70: 4f44 4552 4546 4b02 5129 814e 7d28 6800  ODEREFK.Q).N}(h.
+00000c80: 4b05 5129 814e 7d28 6801 4301 4068 024e  K.Q).N}(h.C.@h.N
+00000c90: 7586 624b 0751 2981 4e7d 6802 4e73 8662  u.bK.Q).N}h.Ns.b
+00000ca0: 4b06 5129 814e 7d28 6803 6804 4307 5b5c  K.Q).N}(h.h.C.[\
+00000cb0: 775c 2e5d 2b4b 0086 5268 054b 0068 0268  w\.]+K..Rh.K.h.h
+00000cc0: 0e75 8662 8768 0689 6802 4e75 8662 8674  .u.b.h..h.Nu.b.t
+00000cd0: 2e                                       .
```

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/serialize.py` & `caustic.lexer-1.2.1/src/caustic/lexer/serialize.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.0.post1/src/caustic/lexer/util.py` & `caustic.lexer-1.2.1/src/caustic/lexer/util.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.2.0.post1/src/caustic.lexer.egg-info/PKG-INFO` & `caustic.lexer-1.2.1/src/caustic.lexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.2.0.post1
+Version: 1.2.1
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -215,7 +215,10 @@
 
 ## 1.1.0
 - Added support for periods in node names
 - Fixed `Compiler.post_process_compile()` not actually doing anything
 
 ## 1.2.0
 - Implemented [unpacking](#unpack) nodes
+
+## 1.2.1
+- Fixed several nodes improperly stripping whitespace
```

