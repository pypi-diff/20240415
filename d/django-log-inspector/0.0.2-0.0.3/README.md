# Comparing `tmp/django-log-inspector-0.0.2.tar.gz` & `tmp/django_log_inspector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-log-inspector-0.0.2.tar", last modified: Tue Jan 23 12:18:43 2024, max compression
+gzip compressed data, was "django_log_inspector-0.0.3.tar", last modified: Mon Apr 15 09:19:57 2024, max compression
```

## Comparing `django-log-inspector-0.0.2.tar` & `django_log_inspector-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.193756 django-log-inspector-0.0.2/
--rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django-log-inspector-0.0.2/LICENSE
--rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django-log-inspector-0.0.2/MANIFEST.in
--rw-r--r--   0 peyman627   (501) staff       (20)      286 2024-01-23 12:18:43.193517 django-log-inspector-0.0.2/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)      165 2024-01-23 11:21:18.000000 django-log-inspector-0.0.2/README.rst
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.193287 django-log-inspector-0.0.2/django_log_inspector.egg-info/
--rw-r--r--   0 peyman627   (501) staff       (20)      286 2024-01-23 12:18:43.000000 django-log-inspector-0.0.2/django_log_inspector.egg-info/PKG-INFO
--rw-r--r--   0 peyman627   (501) staff       (20)     1002 2024-01-23 12:18:43.000000 django-log-inspector-0.0.2/django_log_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-01-23 12:18:43.000000 django-log-inspector-0.0.2/django_log_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-01-23 12:18:43.000000 django-log-inspector-0.0.2/django_log_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.188381 django-log-inspector-0.0.2/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django-log-inspector-0.0.2/log_inspector/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django-log-inspector-0.0.2/log_inspector/admin.py
--rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django-log-inspector-0.0.2/log_inspector/apps.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.188636 django-log-inspector-0.0.2/log_inspector/migrations/
--rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django-log-inspector-0.0.2/log_inspector/migrations/__init__.py
--rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django-log-inspector-0.0.2/log_inspector/models.py
--rw-r--r--   0 peyman627   (501) staff       (20)      985 2024-01-23 10:07:05.000000 django-log-inspector-0.0.2/log_inspector/settings.py
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.184780 django-log-inspector-0.0.2/log_inspector/static/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.184897 django-log-inspector-0.0.2/log_inspector/static/log_inspector/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.189066 django-log-inspector-0.0.2/log_inspector/static/log_inspector/css/
--rw-r--r--   0 peyman627   (501) staff       (20)      103 2024-01-16 11:12:40.000000 django-log-inspector-0.0.2/log_inspector/static/log_inspector/css/input.css
--rw-r--r--   0 peyman627   (501) staff       (20)    14496 2024-01-21 07:03:38.000000 django-log-inspector-0.0.2/log_inspector/static/log_inspector/css/output.css
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.190204 django-log-inspector-0.0.2/log_inspector/static/log_inspector/js/
--rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django-log-inspector-0.0.2/log_inspector/static/log_inspector/js/alpinejs.min.js
--rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django-log-inspector-0.0.2/log_inspector/static/log_inspector/js/htmx.min.js
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.185010 django-log-inspector-0.0.2/log_inspector/templates/
-drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-01-23 12:18:43.192977 django-log-inspector-0.0.2/log_inspector/templates/log_inspector/
--rw-r--r--   0 peyman627   (501) staff       (20)     1569 2024-01-23 10:10:12.000000 django-log-inspector-0.0.2/log_inspector/templates/log_inspector/file_log_entry_list.html
--rw-r--r--   0 peyman627   (501) staff       (20)     6077 2024-01-23 10:07:05.000000 django-log-inspector-0.0.2/log_inspector/templates/log_inspector/home.html
--rw-r--r--   0 peyman627   (501) staff       (20)      720 2024-01-23 09:54:07.000000 django-log-inspector-0.0.2/log_inspector/templates/log_inspector/log_file_list.html
--rw-r--r--   0 peyman627   (501) staff       (20)     2582 2024-01-23 09:54:07.000000 django-log-inspector-0.0.2/log_inspector/templates/log_inspector/pagination.html
--rw-r--r--   0 peyman627   (501) staff       (20)      568 2024-01-23 09:54:07.000000 django-log-inspector-0.0.2/log_inspector/templates/log_inspector/start_live.html
--rw-r--r--   0 peyman627   (501) staff       (20)      609 2024-01-23 09:54:07.000000 django-log-inspector-0.0.2/log_inspector/templates/log_inspector/stop_live.html
--rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django-log-inspector-0.0.2/log_inspector/tests.py
--rw-r--r--   0 peyman627   (501) staff       (20)      837 2024-01-23 09:54:07.000000 django-log-inspector-0.0.2/log_inspector/urls.py
--rw-r--r--   0 peyman627   (501) staff       (20)     1534 2024-01-23 09:58:26.000000 django-log-inspector-0.0.2/log_inspector/utils.py
--rw-r--r--   0 peyman627   (501) staff       (20)     3508 2024-01-23 10:07:05.000000 django-log-inspector-0.0.2/log_inspector/views.py
--rw-r--r--   0 peyman627   (501) staff       (20)      323 2024-01-23 12:18:13.000000 django-log-inspector-0.0.2/pyproject.toml
--rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-01-23 12:18:43.193859 django-log-inspector-0.0.2/setup.cfg
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.580671 django_log_inspector-0.0.3/
+-rw-r--r--   0 peyman627   (501) staff       (20)     1071 2024-01-23 09:55:45.000000 django_log_inspector-0.0.3/LICENSE
+-rw-r--r--   0 peyman627   (501) staff       (20)      100 2024-01-23 12:18:13.000000 django_log_inspector-0.0.3/MANIFEST.in
+-rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-15 09:19:57.580489 django_log_inspector-0.0.3/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     1838 2024-04-15 09:19:35.000000 django_log_inspector-0.0.3/README.md
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.580310 django_log_inspector-0.0.3/django_log_inspector.egg-info/
+-rw-r--r--   0 peyman627   (501) staff       (20)     3430 2024-04-15 09:19:57.000000 django_log_inspector-0.0.3/django_log_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 peyman627   (501) staff       (20)     1050 2024-04-15 09:19:57.000000 django_log_inspector-0.0.3/django_log_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)        1 2024-04-15 09:19:57.000000 django_log_inspector-0.0.3/django_log_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 peyman627   (501) staff       (20)       14 2024-04-15 09:19:57.000000 django_log_inspector-0.0.3/django_log_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.575648 django_log_inspector-0.0.3/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.3/log_inspector/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       63 2024-01-23 09:38:31.000000 django_log_inspector-0.0.3/log_inspector/admin.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      163 2024-01-23 10:07:05.000000 django_log_inspector-0.0.3/log_inspector/apps.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.576017 django_log_inspector-0.0.3/log_inspector/migrations/
+-rw-r--r--   0 peyman627   (501) staff       (20)        0 2024-01-23 09:38:31.000000 django_log_inspector-0.0.3/log_inspector/migrations/__init__.py
+-rw-r--r--   0 peyman627   (501) staff       (20)       57 2024-01-23 09:38:31.000000 django_log_inspector-0.0.3/log_inspector/models.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      985 2024-01-23 10:07:05.000000 django_log_inspector-0.0.3/log_inspector/settings.py
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.572297 django_log_inspector-0.0.3/log_inspector/static/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.572421 django_log_inspector-0.0.3/log_inspector/static/log_inspector/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.576516 django_log_inspector-0.0.3/log_inspector/static/log_inspector/css/
+-rw-r--r--   0 peyman627   (501) staff       (20)     2023 2024-03-17 11:00:14.000000 django_log_inspector-0.0.3/log_inspector/static/log_inspector/css/input.css
+-rw-r--r--   0 peyman627   (501) staff       (20)     8404 2024-04-15 06:33:34.000000 django_log_inspector-0.0.3/log_inspector/static/log_inspector/css/output.css
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.577327 django_log_inspector-0.0.3/log_inspector/static/log_inspector/js/
+-rw-r--r--   0 peyman627   (501) staff       (20)    43440 2024-01-05 17:19:20.000000 django_log_inspector-0.0.3/log_inspector/static/log_inspector/js/alpinejs.min.js
+-rw-r--r--   0 peyman627   (501) staff       (20)    47755 2024-01-05 17:17:16.000000 django_log_inspector-0.0.3/log_inspector/static/log_inspector/js/htmx.min.js
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.572544 django_log_inspector-0.0.3/log_inspector/templates/
+drwxr-xr-x   0 peyman627   (501) staff       (20)        0 2024-04-15 09:19:57.580090 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/
+-rw-r--r--   0 peyman627   (501) staff       (20)     9809 2024-03-17 10:44:38.000000 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/home.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     2000 2024-03-17 11:00:05.000000 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/log_entries.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     2646 2024-03-17 11:00:05.000000 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/log_entries_table.html
+-rw-r--r--   0 peyman627   (501) staff       (20)      978 2024-02-15 09:07:48.000000 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/log_files.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     2645 2024-02-05 11:01:20.000000 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/pagination.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1016 2024-02-15 09:07:48.000000 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/start_live.html
+-rw-r--r--   0 peyman627   (501) staff       (20)     1056 2024-02-15 09:07:48.000000 django_log_inspector-0.0.3/log_inspector/templates/log_inspector/stop_live.html
+-rw-r--r--   0 peyman627   (501) staff       (20)       60 2024-01-23 09:38:31.000000 django_log_inspector-0.0.3/log_inspector/tests.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      809 2024-01-24 12:07:02.000000 django_log_inspector-0.0.3/log_inspector/urls.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     2664 2024-03-17 09:58:30.000000 django_log_inspector-0.0.3/log_inspector/utils.py
+-rw-r--r--   0 peyman627   (501) staff       (20)     3934 2024-02-15 09:02:47.000000 django_log_inspector-0.0.3/log_inspector/views.py
+-rw-r--r--   0 peyman627   (501) staff       (20)      388 2024-04-15 09:19:53.000000 django_log_inspector-0.0.3/pyproject.toml
+-rw-r--r--   0 peyman627   (501) staff       (20)       38 2024-04-15 09:19:57.580711 django_log_inspector-0.0.3/setup.cfg
```

### Comparing `django-log-inspector-0.0.2/LICENSE` & `django_log_inspector-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-log-inspector-0.0.2/django_log_inspector.egg-info/SOURCES.txt` & `django_log_inspector-0.0.3/django_log_inspector.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 django_log_inspector.egg-info/PKG-INFO
 django_log_inspector.egg-info/SOURCES.txt
 django_log_inspector.egg-info/dependency_links.txt
 django_log_inspector.egg-info/top_level.txt
 log_inspector/__init__.py
 log_inspector/admin.py
@@ -16,13 +16,14 @@
 log_inspector/utils.py
 log_inspector/views.py
 log_inspector/migrations/__init__.py
 log_inspector/static/log_inspector/css/input.css
 log_inspector/static/log_inspector/css/output.css
 log_inspector/static/log_inspector/js/alpinejs.min.js
 log_inspector/static/log_inspector/js/htmx.min.js
-log_inspector/templates/log_inspector/file_log_entry_list.html
 log_inspector/templates/log_inspector/home.html
-log_inspector/templates/log_inspector/log_file_list.html
+log_inspector/templates/log_inspector/log_entries.html
+log_inspector/templates/log_inspector/log_entries_table.html
+log_inspector/templates/log_inspector/log_files.html
 log_inspector/templates/log_inspector/pagination.html
 log_inspector/templates/log_inspector/start_live.html
 log_inspector/templates/log_inspector/stop_live.html
```

### Comparing `django-log-inspector-0.0.2/log_inspector/settings.py` & `django_log_inspector-0.0.3/log_inspector/settings.py`

 * *Files identical despite different names*

### Comparing `django-log-inspector-0.0.2/log_inspector/static/log_inspector/js/alpinejs.min.js` & `django_log_inspector-0.0.3/log_inspector/static/log_inspector/js/alpinejs.min.js`

 * *Files identical despite different names*

### Comparing `django-log-inspector-0.0.2/log_inspector/static/log_inspector/js/htmx.min.js` & `django_log_inspector-0.0.3/log_inspector/static/log_inspector/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-log-inspector-0.0.2/log_inspector/templates/log_inspector/pagination.html` & `django_log_inspector-0.0.3/log_inspector/templates/log_inspector/pagination.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 {% load static i18n %}
 
-<tfoot id="log-entries-footer" hx-swap-oob="true">
 <tr>
-    <td colspan="2">
-        <div class="flex items-center justify-center mt-4">
+    <td colspan="2" class="dark:bg-slate-800 dark:border-gray-700 dark:text-white">
+        <div class="flex items-center justify-center mt-4 dark:bg-slate-800">
             {% if log_entries.has_previous %}
-                <span class="px-4 py-2 border border-gray-300 rounded-l cursor-pointer"
-                      hx-get="{% url 'log_inspector:file_log_entries' filename=filename %}?page={{ log_entries.previous_page_number }}"
-                      hx-target="#log-entries-data"
+                <span class="px-4 py-2 border border-gray-300 rounded-l cursor-pointer dark:border-gray-700"
+                      hx-get="{% url 'log_inspector:log_entries' filename=filename %}?page={{ log_entries.previous_page_number }}"
+                      hx-target="#log-entries-table"
                       hx-swap="outerHTML">
-                        {% trans 'Previous' %}
-                    </span>
+                {% trans 'Previous' %}
+            </span>
             {% endif %}
-
             {% for page_num in log_entries.paginator.page_range %}
                 {% if page_num == log_entries.number %}
-                    <span class="px-4 py-2 bg-blue-500 text-white rounded-md">
-                            {{ page_num }}
-                        </span>
+                    <span class="px-4 py-2 bg-blue-500 text-white rounded-md dark:bg-slate-600 dark:text-white">
+                    {{ page_num }}
+                </span>
                 {% elif page_num == 1 or page_num == log_entries.paginator.num_pages %}
-                    <span class="px-4 py-2 border border-gray-300 rounded-md cursor-pointer"
-                          hx-get="{% url 'log_inspector:file_log_entries' filename=filename %}?page={{ page_num }}"
-                          hx-target="#log-entries-data"
+                    <span class="px-4 py-2 border border-gray-300 rounded-md cursor-pointer dark:border-gray-700"
+                          hx-get="{% url 'log_inspector:log_entries' filename=filename %}?page={{ page_num }}"
+                          hx-target="#log-entries-table"
                           hx-swap="outerHTML">
-                            {{ page_num }}
-                        </span>
+                    {{ page_num }}
+                </span>
                 {% elif page_num > log_entries.number|add:'-3' and page_num < log_entries.number|add:'3' %}
-                    <span class="px-4 py-2 border border-gray-300 rounded-md cursor-pointer"
-                          hx-get="{% url 'log_inspector:file_log_entries' filename=filename %}?page={{ page_num }}"
-                          hx-target="#log-entries-data"
+                    <span class="px-4 py-2 border border-gray-300 rounded-md cursor-pointer dark:border-gray-700"
+                          hx-get="{% url 'log_inspector:log_entries' filename=filename %}?page={{ page_num }}"
+                          hx-target="#log-entries-table"
                           hx-swap="outerHTML">
-                            {{ page_num }}
-                        </span>
+                    {{ page_num }}
+                </span>
                 {% elif page_num == log_entries.number|add:'-3' or page_num == log_entries.number|add:'3' %}
-                    <span class="px-4 py-2">...</span>
+                    <span class="px-4 py-2 dark:border-gray-700">...</span>
                 {% endif %}
             {% endfor %}
 
             {% if log_entries.has_next %}
-                <span class="px-4 py-2 border border-gray-300 rounded-r cursor-pointer"
-                      hx-get="{% url 'log_inspector:file_log_entries' filename=filename %}?page={{ log_entries.next_page_number }}"
-                      hx-target="#log-entries-data"
+                <span class="px-4 py-2 border border-gray-300 rounded-r cursor-pointer dark:border-gray-700"
+                      hx-get="{% url 'log_inspector:log_entries' filename=filename %}?page={{ log_entries.next_page_number }}"
+                      hx-target="#log-entries-table"
                       hx-swap="outerHTML">
-                        {% trans 'Next' %}
-                    </span>
+                {% trans 'Next' %}
+            </span>
             {% endif %}
         </div>
     </td>
-</tr>
-</tfoot>
+</tr>
```

### Comparing `django-log-inspector-0.0.2/log_inspector/urls.py` & `django_log_inspector-0.0.3/log_inspector/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import django
 
 if django.VERSION >= (2, 0):
     from django.urls import re_path
 else:
     from django.conf.urls import url as re_path
 
-from .views import FileLogEntryListView, LogFileListView, HomeView, StartLiveView, StopLiveView, DownloadLogFileView
+from .views import LogEntriesView, LogFilesView, HomeView, StartLiveView, StopLiveView, DownloadLogFileView
 
 app_name = "log_inspector"
 
 urlpatterns = [
     re_path(r"^$", HomeView.as_view(), name='home'),
-    re_path(r'^log-files/$', LogFileListView.as_view(), name='log_files'),
-    re_path(r'^file-log-entries/(?P<filename>[\w\.-]+)/$', FileLogEntryListView.as_view(), name='file_log_entries'),
+    re_path(r'^log-files/$', LogFilesView.as_view(), name='log_files'),
+    re_path(r'^log-entries/(?P<filename>[\w\.-]+)/$', LogEntriesView.as_view(), name='log_entries'),
     re_path(r'^start-live/(?P<filename>[\w\.-]+)/$', StartLiveView.as_view(), name='start_live'),
     re_path(r'^stop-live/(?P<filename>[\w\.-]+)/$', StopLiveView.as_view(), name='stop_live'),
     re_path(r'^download/(?P<filename>[\w\.-]+)/$', DownloadLogFileView.as_view(), name='download'),
 ]
```

### Comparing `django-log-inspector-0.0.2/log_inspector/views.py` & `django_log_inspector-0.0.3/log_inspector/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from django.core.paginator import Paginator, EmptyPage, PageNotAnInteger
 from django.http import Http404, HttpResponse
 from django.shortcuts import render
 from django.utils.decorators import method_decorator
 from django.views.generic import TemplateView as _TemplateView
 
 from . import settings
-from .utils import get_log_entries, get_log_file_names
+from .utils import get_log_entries, get_log_file_names, filter_log_entries, is_valid_filename
+
+HTMX_STOP_POLLING = 286
 
 
 class TemplateView(_TemplateView):
     @method_decorator(login_required)
     @method_decorator(user_passes_test(lambda u: u.is_superuser))
     def dispatch(self, *args, **kwargs):
         return super(TemplateView, self).dispatch(*args, **kwargs)
@@ -25,70 +27,72 @@
     def get(self, request, *args, **kwargs):
         context = self.get_context_data(**kwargs)
         context['custom_title'] = settings.LOG_INSPECTOR_FILE_LIST_TITLE
         context['custom_style_file'] = settings.LOG_INSPECTOR_FILE_LIST_STYLES
         return render(request, 'log_inspector/home.html', context=context)
 
 
-class LogFileListView(TemplateView):
+class LogFilesView(TemplateView):
     def get(self, request, *args, **kwargs):
         search = request.GET.get('search', '')
 
-        log_filenames = get_log_file_names(settings.LOG_INSPECTOR_FILES_DIR)
-
-        filenames = []
-        for fn in log_filenames:
-            if search and search.lower() not in fn:
-                continue
-
-            filenames.append(fn)
+        filenames = get_log_file_names(settings.LOG_INSPECTOR_FILES_DIR, search)
+        filenames.sort()
 
         context = {'filenames': filenames}
-        return render(request, 'log_inspector/log_file_list.html', context=context)
+        return render(request, 'log_inspector/log_files.html', context=context)
 
 
-class FileLogEntryListView(TemplateView):
+class LogEntriesView(TemplateView):
     def get(self, request, filename, *args, **kwargs):
-        if filename not in get_log_file_names(settings.LOG_INSPECTOR_FILES_DIR):
+        if not is_valid_filename(filename):
             raise Http404
 
-        log_entries = get_log_entries(filename)
+        search = request.GET.get('search', '')
+        page = request.GET.get('page', 1)
+        live_action = request.META.get('HTTP_X_LIVE_ACTION')
+        is_start_live = live_action == 'START'
+        is_stop_live = live_action == 'STOP'
 
-        max_lines = 1000
-        paginator = Paginator(list(islice(log_entries, max_lines)), 20)
+        log_entries = get_log_entries(filename)
+        log_entries = filter_log_entries(log_entries, search)
 
-        page = request.GET.get('page', 1)
+        max_lines = settings.LOG_INSPECTOR_MAX_READ_LINES if not is_start_live else settings.LOG_INSPECTOR_PAGE_LENGTH
+        paginator = Paginator(list(islice(log_entries, max_lines)), settings.LOG_INSPECTOR_PAGE_LENGTH)
+        start_index = (int(page) - 1) * paginator.per_page
 
         try:
             log_entries = paginator.page(page)
         except PageNotAnInteger:
             log_entries = paginator.page(1)
         except EmptyPage:
             log_entries = paginator.page(paginator.num_pages)
 
-        context = {'log_entries': log_entries, 'filename': filename}
-        return render(request, 'log_inspector/file_log_entry_list.html', context)
+        context = {'log_entries': log_entries, 'filename': filename, 'start_index': start_index}
+        if is_start_live or is_stop_live:
+            return render(request, 'log_inspector/log_entries.html', context)
+
+        return render(request, 'log_inspector/log_entries_table.html', context, status=HTMX_STOP_POLLING)
 
 
 class StartLiveView(TemplateView):
     def get(self, request, filename, *args, **kwargs):
         context = {'filename': filename}
         return render(request, 'log_inspector/start_live.html', context=context)
 
 
 class StopLiveView(TemplateView):
     def get(self, request, filename, *args, **kwargs):
-        htmx_stop_polling = 286
         context = {'filename': filename}
-        return render(request, 'log_inspector/stop_live.html', context=context, status=htmx_stop_polling)
+        return render(request, 'log_inspector/stop_live.html', context=context, status=HTMX_STOP_POLLING)
 
 
 class DownloadLogFileView(TemplateView):
     def get(self, request, filename, *args, **kwargs):
-        if filename not in get_log_file_names(settings.LOG_INSPECTOR_FILES_DIR):
+        if not is_valid_filename(filename):
             raise Http404
 
         zip_buffer = io.BytesIO()
         with zipfile.ZipFile(zip_buffer, 'w') as zip_file:
             zip_file.write(os.path.join(settings.LOG_INSPECTOR_FILES_DIR, filename))
 
         basename, _ = os.path.splitext(filename)
```

