# Comparing `tmp/pwd_generator-1.1.0.tar.gz` & `tmp/pwd_generator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwd_generator-1.1.0.tar", max compression
+gzip compressed data, was "pwd_generator-2.0.0.tar", max compression
```

## Comparing `pwd_generator-1.1.0.tar` & `pwd_generator-2.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      358 2024-04-10 09:42:08.605159 pwd_generator-1.1.0/README.md
--rw-r--r--   0        0        0      990 2024-04-10 09:35:36.722962 pwd_generator-1.1.0/pwdgen.py
--rw-r--r--   0        0        0      409 2024-04-10 09:43:02.153873 pwd_generator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 pwd_generator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      357 2024-04-15 15:25:29.587959 pwd_generator-2.0.0/README.md
+-rw-r--r--   0        0        0     1003 2024-04-15 15:36:56.189973 pwd_generator-2.0.0/pwdgen.py
+-rw-r--r--   0        0        0      409 2024-04-15 15:44:01.713854 pwd_generator-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 pwd_generator-2.0.0/PKG-INFO
```

### Comparing `pwd_generator-1.1.0/pwdgen.py` & `pwd_generator-2.0.0/pwdgen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """
 A simple password generator
 """
 
 
-import random
+import secrets
 CONSONANTS = "bcdfghjklmnpqrstvwxz"
 VOWELS = "aeiouy"
 SPECIAL_CHARS=".:;-!&*_+#,=" # #!$%^&*
 
 def generate(syllables=6):
     pw = ""
     for _ in range(syllables):
-        pw += random.choice(CONSONANTS) + random.choice(VOWELS)
+        pw += secrets.choice(CONSONANTS) + secrets.choice(VOWELS)
         
-    idx_sep = random.randrange(1,syllables)*2
-    pw = pw[:idx_sep].capitalize() + random.choice(SPECIAL_CHARS) + pw[idx_sep:].capitalize()
+    idx_sep = (secrets.randbelow(syllables)+1)*2
+    pw = pw[:idx_sep].capitalize() + secrets.choice(SPECIAL_CHARS) + pw[idx_sep:].capitalize()
     
-    number=str(random.randrange(10))
-    if random.randrange(2):
+    number=str(secrets.randbelow(10))
+    if secrets.randbelow(2):
         pw+=number
     else:
         pw=number+pw
     return pw
 
 def main():
     import argparse
     parser = argparse.ArgumentParser(description="A simple password generator")
     parser.add_argument("-s","--syllables", type=int, default=6, help="Number of syllables in the password")
-    parser.add_argument("-n","--number", type=int, default=1, help="Number of passwords to generate")
+    parser.add_argument("number", type=int, default=1, nargs='?', help="Number of passwords to generate")
     args = parser.parse_args()
     for _ in range(args.number):
         print(generate(args.syllables))
```

### Comparing `pwd_generator-1.1.0/PKG-INFO` & `pwd_generator-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwd-generator
-Version: 1.1.0
+Version: 2.0.0
 Summary: A simple password generator
 License: MIT
 Author: RadoTheProgrammer
 Author-email: rado@arazakar.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 
 This is a generator of simple, strong, memorable and easy-to-type passwords.
 
 You can install it with `pip install pwd-generator` and use the cli version:
 
 ```
 
-pwd-gen
+pwdgen
 ```
 
 Then the output would be like:
 
 ```
 
 6Nixe#Becokace
```

