# Comparing `tmp/zodchy_security-0.1.0.tar.gz` & `tmp/zodchy_security-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_security-0.1.0.tar", max compression
+gzip compressed data, was "zodchy_security-0.1.1.tar", max compression
```

## Comparing `zodchy_security-0.1.0.tar` & `zodchy_security-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       17 2024-04-13 13:40:05.904405 zodchy_security-0.1.0/README.md
--rw-r--r--   0        0        0      411 2024-04-13 13:40:40.836894 zodchy_security-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       90 2024-04-11 13:37:07.017037 zodchy_security-0.1.0/zodchy_security/__init__.py
--rw-r--r--   0        0        0       36 2024-04-11 13:29:06.723696 zodchy_security-0.1.0/zodchy_security/credentials/__init__.py
--rw-r--r--   0        0        0       87 2024-04-11 13:29:06.729526 zodchy_security-0.1.0/zodchy_security/credentials/otp.py
--rw-r--r--   0        0        0        0 2024-04-11 13:14:21.400474 zodchy_security-0.1.0/zodchy_security/tokens/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-11 13:23:33.081141 zodchy_security-0.1.0/zodchy_security/tokens/jwts.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 zodchy_security-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-13 13:40:05.904405 zodchy_security-0.1.1/README.md
+-rw-r--r--   0        0        0      468 2024-04-15 11:05:19.578042 zodchy_security-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       90 2024-04-11 13:37:07.017037 zodchy_security-0.1.1/zodchy_security/__init__.py
+-rw-r--r--   0        0        0       36 2024-04-11 13:29:06.723696 zodchy_security-0.1.1/zodchy_security/credentials/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-11 13:29:06.729526 zodchy_security-0.1.1/zodchy_security/credentials/otp.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:14:21.400474 zodchy_security-0.1.1/zodchy_security/tokens/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-11 13:23:33.081141 zodchy_security-0.1.1/zodchy_security/tokens/jwts.py
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 zodchy_security-0.1.1/PKG-INFO
```

### Comparing `zodchy_security-0.1.0/zodchy_security/tokens/jwts.py` & `zodchy_security-0.1.1/zodchy_security/tokens/jwts.py`

 * *Files identical despite different names*

