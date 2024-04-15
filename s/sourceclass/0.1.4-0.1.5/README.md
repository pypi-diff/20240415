# Comparing `tmp/sourceclass-0.1.4.tar.gz` & `tmp/sourceclass-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourceclass-0.1.4.tar", last modified: Sun Dec 17 16:49:02 2023, max compression
+gzip compressed data, was "sourceclass-0.1.5.tar", last modified: Mon Apr 15 13:29:54 2024, max compression
```

## Comparing `sourceclass-0.1.4.tar` & `sourceclass-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lara       (501) staff       (20)        0 2023-12-17 16:49:02.096365 sourceclass-0.1.4/
--rw-r--r--   0 lara       (501) staff       (20)       55 2023-12-17 16:49:02.096143 sourceclass-0.1.4/PKG-INFO
--rw-r--r--   0 lara       (501) staff       (20)      617 2023-12-17 16:48:20.000000 sourceclass-0.1.4/README.md
--rw-r--r--   0 lara       (501) staff       (20)       38 2023-12-17 16:49:02.096410 sourceclass-0.1.4/setup.cfg
--rw-r--r--   0 lara       (501) staff       (20)      151 2023-12-17 16:48:13.000000 sourceclass-0.1.4/setup.py
-drwxr-xr-x   0 lara       (501) staff       (20)        0 2023-12-17 16:49:02.094368 sourceclass-0.1.4/sourceclass/
--rw-r--r--   0 lara       (501) staff       (20)       96 2023-12-16 18:34:08.000000 sourceclass-0.1.4/sourceclass/__init__.py
--rw-r--r--   0 lara       (501) staff       (20)     1931 2023-12-17 15:54:11.000000 sourceclass-0.1.4/sourceclass/gitCommit.py
--rw-r--r--   0 lara       (501) staff       (20)     4034 2023-12-17 14:00:35.000000 sourceclass-0.1.4/sourceclass/githubPr.py
--rw-r--r--   0 lara       (501) staff       (20)    10269 2023-12-17 16:47:16.000000 sourceclass-0.1.4/sourceclass/jiraIssue.py
-drwxr-xr-x   0 lara       (501) staff       (20)        0 2023-12-17 16:49:02.095923 sourceclass-0.1.4/sourceclass.egg-info/
--rw-r--r--   0 lara       (501) staff       (20)       55 2023-12-17 16:49:02.000000 sourceclass-0.1.4/sourceclass.egg-info/PKG-INFO
--rw-r--r--   0 lara       (501) staff       (20)      314 2023-12-17 16:49:02.000000 sourceclass-0.1.4/sourceclass.egg-info/SOURCES.txt
--rw-r--r--   0 lara       (501) staff       (20)        1 2023-12-17 16:49:02.000000 sourceclass-0.1.4/sourceclass.egg-info/dependency_links.txt
--rw-r--r--   0 lara       (501) staff       (20)       12 2023-12-17 16:49:02.000000 sourceclass-0.1.4/sourceclass.egg-info/top_level.txt
-drwxr-xr-x   0 lara       (501) staff       (20)        0 2023-12-17 16:49:02.095654 sourceclass-0.1.4/tests/
--rw-r--r--   0 lara       (501) staff       (20)     1934 2023-12-17 16:20:50.000000 sourceclass-0.1.4/tests/test_commit.py
--rw-r--r--   0 lara       (501) staff       (20)     5946 2023-12-17 16:47:58.000000 sourceclass-0.1.4/tests/test_issue.py
--rw-r--r--   0 lara       (501) staff       (20)     2574 2023-12-17 15:29:12.000000 sourceclass-0.1.4/tests/test_pr.py
+drwxr-xr-x   0 lara       (501) staff       (20)        0 2024-04-15 13:29:54.289790 sourceclass-0.1.5/
+-rw-r--r--   0 lara       (501) staff       (20)       55 2024-04-15 13:29:54.289661 sourceclass-0.1.5/PKG-INFO
+-rw-r--r--   0 lara       (501) staff       (20)      617 2023-12-17 16:48:20.000000 sourceclass-0.1.5/README.md
+-rw-r--r--   0 lara       (501) staff       (20)       38 2024-04-15 13:29:54.289828 sourceclass-0.1.5/setup.cfg
+-rw-r--r--   0 lara       (501) staff       (20)      151 2024-04-15 13:23:58.000000 sourceclass-0.1.5/setup.py
+drwxr-xr-x   0 lara       (501) staff       (20)        0 2024-04-15 13:29:54.288567 sourceclass-0.1.5/sourceclass/
+-rw-r--r--   0 lara       (501) staff       (20)       96 2023-12-16 18:34:08.000000 sourceclass-0.1.5/sourceclass/__init__.py
+-rw-r--r--   0 lara       (501) staff       (20)     1931 2023-12-17 15:54:11.000000 sourceclass-0.1.5/sourceclass/gitCommit.py
+-rw-r--r--   0 lara       (501) staff       (20)     4034 2023-12-17 14:00:35.000000 sourceclass-0.1.5/sourceclass/githubPr.py
+-rw-r--r--   0 lara       (501) staff       (20)    10359 2024-04-15 13:21:07.000000 sourceclass-0.1.5/sourceclass/jiraIssue.py
+drwxr-xr-x   0 lara       (501) staff       (20)        0 2024-04-15 13:29:54.289163 sourceclass-0.1.5/sourceclass.egg-info/
+-rw-r--r--   0 lara       (501) staff       (20)       55 2024-04-15 13:29:54.000000 sourceclass-0.1.5/sourceclass.egg-info/PKG-INFO
+-rw-r--r--   0 lara       (501) staff       (20)      314 2024-04-15 13:29:54.000000 sourceclass-0.1.5/sourceclass.egg-info/SOURCES.txt
+-rw-r--r--   0 lara       (501) staff       (20)        1 2024-04-15 13:29:54.000000 sourceclass-0.1.5/sourceclass.egg-info/dependency_links.txt
+-rw-r--r--   0 lara       (501) staff       (20)       12 2024-04-15 13:29:54.000000 sourceclass-0.1.5/sourceclass.egg-info/top_level.txt
+drwxr-xr-x   0 lara       (501) staff       (20)        0 2024-04-15 13:29:54.289501 sourceclass-0.1.5/tests/
+-rw-r--r--   0 lara       (501) staff       (20)     1934 2023-12-17 16:20:50.000000 sourceclass-0.1.5/tests/test_commit.py
+-rw-r--r--   0 lara       (501) staff       (20)     5946 2023-12-17 16:47:58.000000 sourceclass-0.1.5/tests/test_issue.py
+-rw-r--r--   0 lara       (501) staff       (20)     3670 2023-12-17 16:59:48.000000 sourceclass-0.1.5/tests/test_pr.py
```

### Comparing `sourceclass-0.1.4/README.md` & `sourceclass-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sourceclass-0.1.4/sourceclass/gitCommit.py` & `sourceclass-0.1.5/sourceclass/gitCommit.py`

 * *Files identical despite different names*

### Comparing `sourceclass-0.1.4/sourceclass/githubPr.py` & `sourceclass-0.1.5/sourceclass/githubPr.py`

 * *Files identical despite different names*

### Comparing `sourceclass-0.1.4/sourceclass/jiraIssue.py` & `sourceclass-0.1.5/sourceclass/jiraIssue.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             return None        
     
     def getAssigner(self):
         try:
             histories = self.data["changelog"]["histories"]
             for history in reversed(histories):
                 for item in history["items"]:
-                    if item["field"] == "assignee":
+                    if item["field"] == "assignee" and  history["author"]:
                         return history["author"]["displayName"] or history["author"]["name"]
             return None
         except (KeyError, TypeError):
             return None   
         
     def getCommentsData(self):
         try:
@@ -179,26 +179,26 @@
                         "date":assignee["created"]
                     })      
         return returnList
     
     def getResolver(self):
         for history in  self.data["changelog"]["histories"]:
             for item in history["items"]:
-                if item["field"] == "resolution" and item["toString"]:
+                if item["field"] == "resolution" and item["toString"] and history["author"]:
                     return history["author"]["displayName"] or history["author"]["name"]
-                if item["field"] == "status" and item["toString"].lower() == "resolved":
+                if item["field"] == "status" and item["toString"].lower() == "resolved" and history["author"]:
                     return history["author"]["displayName"] or history["author"]["name"]
         return None   
          
     def getCloser(self):
         history = self.data["changelog"]["histories"]
         if len(history)>0:
             lastItem = history[-1]
             for item in  lastItem["items"]:
-                if item["field"] == "status" and item["toString"]=="Closed":
+                if item["field"] == "status" and item["toString"]=="Closed" and lastItem["author"]:
                     return lastItem["author"]["displayName"] or lastItem["author"]["name"]
         return None
     
     def getCloseDate(self):
         history = self.data["changelog"]["histories"]
         if len(history)>0:
             lastItem = history[-1]
```

### Comparing `sourceclass-0.1.4/tests/test_commit.py` & `sourceclass-0.1.5/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `sourceclass-0.1.4/tests/test_issue.py` & `sourceclass-0.1.5/tests/test_issue.py`

 * *Files identical despite different names*

