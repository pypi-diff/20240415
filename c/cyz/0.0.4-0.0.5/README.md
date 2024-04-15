# Comparing `tmp/cyz-0.0.4.tar.gz` & `tmp/cyz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyz-0.0.4.tar", last modified: Mon Apr  8 07:29:26 2024, max compression
+gzip compressed data, was "cyz-0.0.5.tar", last modified: Mon Apr 15 06:38:21 2024, max compression
```

## Comparing `cyz-0.0.4.tar` & `cyz-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 07:29:26.156764 cyz-0.0.4/
--rw-rw-rw-   0        0        0      390 2024-04-08 07:29:26.155341 cyz-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      143 2024-04-08 07:27:01.000000 cyz-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 07:29:26.125670 cyz-0.0.4/cyz/
--rw-rw-rw-   0        0        0       19 2024-04-08 07:21:05.000000 cyz-0.0.4/cyz/__init__.py
--rw-rw-rw-   0        0        0     3548 2024-04-08 07:20:39.000000 cyz-0.0.4/cyz/mail.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:29:26.152937 cyz-0.0.4/cyz.egg-info/
--rw-rw-rw-   0        0        0      390 2024-04-08 07:29:26.000000 cyz-0.0.4/cyz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      154 2024-04-08 07:29:26.000000 cyz-0.0.4/cyz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 07:29:26.000000 cyz-0.0.4/cyz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-08 07:29:26.000000 cyz-0.0.4/cyz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 07:29:26.156764 cyz-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1106 2024-04-08 07:28:09.000000 cyz-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:38:21.975962 cyz-0.0.5/
+-rw-rw-rw-   0        0        0      336 2024-04-15 06:38:21.975962 cyz-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-04-15 06:37:04.000000 cyz-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 06:38:21.958107 cyz-0.0.5/cyz/
+-rw-rw-rw-   0        0        0       19 2024-04-08 07:21:05.000000 cyz-0.0.5/cyz/__init__.py
+-rw-rw-rw-   0        0        0     3548 2024-04-08 07:20:39.000000 cyz-0.0.5/cyz/mail.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:38:21.974821 cyz-0.0.5/cyz.egg-info/
+-rw-rw-rw-   0        0        0      336 2024-04-15 06:38:21.000000 cyz-0.0.5/cyz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2024-04-15 06:38:21.000000 cyz-0.0.5/cyz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:38:21.000000 cyz-0.0.5/cyz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-15 06:38:21.000000 cyz-0.0.5/cyz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:38:21.975962 cyz-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2024-04-15 06:37:51.000000 cyz-0.0.5/setup.py
```

### Comparing `cyz-0.0.4/cyz/mail.py` & `cyz-0.0.5/cyz/mail.py`

 * *Files identical despite different names*

### Comparing `cyz-0.0.4/setup.py` & `cyz-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='cyz',  # 必填，项目的名字，用户根据这个名字安装，pip install SpiderKeeper-new
-    version='0.0.4',  # 必填，项目的版本，建议遵循语义化版本规范
+    version='0.0.5',  # 必填，项目的版本，建议遵循语义化版本规范
     author='cyz020403',  # 项目的作者
-    description='my utils',  # 项目的一个简短描述
+    description='Has been deprecated, please refer to `cyzutils`',  # 项目的一个简短描述
     long_description=long_description,  # 项目的详细说明，通常读取 README.md 文件的内容
     long_description_content_type='text/markdown',  # 描述的格式，可选的值： text/plain, text/x-rst, and text/markdown
     author_email='cyz020403@gmail.com',  # 作者的有效邮箱地址
     url='https://github.com/cyz020403',  # 项目的源码地址
     license='MIT',
     packages=['cyz'],  # 必填，指定打包的目录，默认是当前目录，如果是其他目录比如 src, 可以使用 find_packages(where='src')
     python_requires='>=3.6',
```

