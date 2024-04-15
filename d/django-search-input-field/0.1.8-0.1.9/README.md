# Comparing `tmp/django-search-input-field-0.1.8.tar.gz` & `tmp/django-search-input-field-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-search-input-field-0.1.8.tar", last modified: Wed Feb 14 16:43:08 2024, max compression
+gzip compressed data, was "django-search-input-field-0.1.9.tar", last modified: Mon Apr 15 09:38:10 2024, max compression
```

## Comparing `django-search-input-field-0.1.8.tar` & `django-search-input-field-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-02-14 16:43:08.802635 django-search-input-field-0.1.8/
--rwxr-xr-x   0 minaatef   (501) staff       (20)     1056 2023-12-29 21:55:49.000000 django-search-input-field-0.1.8/LICENSE
--rwxr-xr-x   0 minaatef   (501) staff       (20)      127 2024-02-14 16:42:05.000000 django-search-input-field-0.1.8/MANIFEST.in
--rw-r--r--   0 minaatef   (501) staff       (20)      227 2024-02-14 16:43:08.802357 django-search-input-field-0.1.8/PKG-INFO
-drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-02-14 16:43:08.800451 django-search-input-field-0.1.8/django_search_input_field/
--rw-r--r--   0 minaatef   (501) staff       (20)        0 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/__init__.py
--rw-r--r--   0 minaatef   (501) staff       (20)     1969 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/apis.py
--rw-r--r--   0 minaatef   (501) staff       (20)     3136 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/field.py
--rw-r--r--   0 minaatef   (501) staff       (20)     2211 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/form.py
--rw-r--r--   0 minaatef   (501) staff       (20)     2438 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/options.py
--rw-r--r--   0 minaatef   (501) staff       (20)     1128 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/query_function_register.py
-drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-02-14 16:43:08.801459 django-search-input-field-0.1.8/django_search_input_field/static/
--rw-r--r--   0 minaatef   (501) staff       (20)     3499 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/static/django_search_input_field.js
-drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-02-14 16:43:08.801738 django-search-input-field-0.1.8/django_search_input_field/templates/
--rw-r--r--   0 minaatef   (501) staff       (20)      774 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/templates/select_search_text_input.html
-drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-02-14 16:43:08.802095 django-search-input-field-0.1.8/django_search_input_field/templatetags/
--rw-r--r--   0 minaatef   (501) staff       (20)        0 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/templatetags/__init__.py
--rw-r--r--   0 minaatef   (501) staff       (20)      383 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/templatetags/django_search_input_field.py
--rw-r--r--   0 minaatef   (501) staff       (20)      254 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/urls.py
--rw-r--r--   0 minaatef   (501) staff       (20)      138 2024-02-08 12:35:24.000000 django-search-input-field-0.1.8/django_search_input_field/widgets.py
-drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-02-14 16:43:08.801303 django-search-input-field-0.1.8/django_search_input_field.egg-info/
--rw-r--r--   0 minaatef   (501) staff       (20)      227 2024-02-14 16:43:08.000000 django-search-input-field-0.1.8/django_search_input_field.egg-info/PKG-INFO
--rw-r--r--   0 minaatef   (501) staff       (20)      783 2024-02-14 16:43:08.000000 django-search-input-field-0.1.8/django_search_input_field.egg-info/SOURCES.txt
--rw-r--r--   0 minaatef   (501) staff       (20)        1 2024-02-14 16:43:08.000000 django-search-input-field-0.1.8/django_search_input_field.egg-info/dependency_links.txt
--rw-r--r--   0 minaatef   (501) staff       (20)       26 2024-02-14 16:43:08.000000 django-search-input-field-0.1.8/django_search_input_field.egg-info/top_level.txt
--rw-r--r--   0 minaatef   (501) staff       (20)       38 2024-02-14 16:43:08.802683 django-search-input-field-0.1.8/setup.cfg
--rwxr-xr-x   0 minaatef   (501) staff       (20)      779 2024-02-14 16:42:08.000000 django-search-input-field-0.1.8/setup.py
+drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-04-15 09:38:10.653545 django-search-input-field-0.1.9/
+-rwxr-xr-x   0 minaatef   (501) staff       (20)     1056 2023-12-29 21:55:49.000000 django-search-input-field-0.1.9/LICENSE
+-rwxr-xr-x   0 minaatef   (501) staff       (20)      127 2024-02-14 16:42:05.000000 django-search-input-field-0.1.9/MANIFEST.in
+-rw-r--r--   0 minaatef   (501) staff       (20)      227 2024-04-15 09:38:10.653231 django-search-input-field-0.1.9/PKG-INFO
+drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-04-15 09:38:10.650972 django-search-input-field-0.1.9/django_search_input_field/
+-rw-r--r--   0 minaatef   (501) staff       (20)        0 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/__init__.py
+-rw-r--r--   0 minaatef   (501) staff       (20)     1969 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/apis.py
+-rw-r--r--   0 minaatef   (501) staff       (20)     3344 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/field.py
+-rw-r--r--   0 minaatef   (501) staff       (20)     2211 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/form.py
+-rw-r--r--   0 minaatef   (501) staff       (20)     3561 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/options.py
+-rw-r--r--   0 minaatef   (501) staff       (20)     1128 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/query_function_register.py
+drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-04-15 09:38:10.652024 django-search-input-field-0.1.9/django_search_input_field/static/
+-rw-r--r--   0 minaatef   (501) staff       (20)     3499 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/static/django_search_input_field.js
+drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-04-15 09:38:10.652233 django-search-input-field-0.1.9/django_search_input_field/templates/
+-rw-r--r--   0 minaatef   (501) staff       (20)      839 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/templates/select_search_text_input.html
+drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-04-15 09:38:10.652622 django-search-input-field-0.1.9/django_search_input_field/templatetags/
+-rw-r--r--   0 minaatef   (501) staff       (20)        0 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/templatetags/__init__.py
+-rw-r--r--   0 minaatef   (501) staff       (20)      471 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/templatetags/django_search_input_field.py
+-rw-r--r--   0 minaatef   (501) staff       (20)      254 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/urls.py
+-rw-r--r--   0 minaatef   (501) staff       (20)      138 2024-04-08 23:10:55.000000 django-search-input-field-0.1.9/django_search_input_field/widgets.py
+drwxr-xr-x   0 minaatef   (501) staff       (20)        0 2024-04-15 09:38:10.651866 django-search-input-field-0.1.9/django_search_input_field.egg-info/
+-rw-r--r--   0 minaatef   (501) staff       (20)      227 2024-04-15 09:38:10.000000 django-search-input-field-0.1.9/django_search_input_field.egg-info/PKG-INFO
+-rw-r--r--   0 minaatef   (501) staff       (20)      783 2024-04-15 09:38:10.000000 django-search-input-field-0.1.9/django_search_input_field.egg-info/SOURCES.txt
+-rw-r--r--   0 minaatef   (501) staff       (20)        1 2024-04-15 09:38:10.000000 django-search-input-field-0.1.9/django_search_input_field.egg-info/dependency_links.txt
+-rw-r--r--   0 minaatef   (501) staff       (20)       26 2024-04-15 09:38:10.000000 django-search-input-field-0.1.9/django_search_input_field.egg-info/top_level.txt
+-rw-r--r--   0 minaatef   (501) staff       (20)       38 2024-04-15 09:38:10.653604 django-search-input-field-0.1.9/setup.cfg
+-rwxr-xr-x   0 minaatef   (501) staff       (20)      779 2024-03-12 12:22:57.000000 django-search-input-field-0.1.9/setup.py
```

### Comparing `django-search-input-field-0.1.8/LICENSE` & `django-search-input-field-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-search-input-field-0.1.8/django_search_input_field/apis.py` & `django-search-input-field-0.1.9/django_search_input_field/apis.py`

 * *Files identical despite different names*

### Comparing `django-search-input-field-0.1.8/django_search_input_field/field.py` & `django-search-input-field-0.1.9/django_search_input_field/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 import random
 
 
 
 class SelectSearchCharField(forms.CharField):
     widget = SelectSearchTextInput
 
-    def __init__(self, query_function_name='', min_search_length=1,*args, **kwargs):
+    def __init__(self, query_function_name='',field=None, min_search_length=1,*args, **kwargs):
         assert query_function_name is not None, f"The query function name cannot be None."
         self.query_function_name = query_function_name
         self.min_search_length = min_search_length
+        self.field = field
         super().__init__(*args, **kwargs)
 
     def widget_attrs(self, widget: Widget) -> Any:
         attrs = super().widget_attrs(widget)            
         attrs.update({'query_function_name': self.query_function_name,
                       'min_search_length': self.min_search_length,
+                      "search_field" : self.field,
+                      "id": f"search-input-{random.randint(0, 1000000000)}",
                       })
         return attrs
 
 
 class SearchModelField(forms.CharField):
     widget = SelectSearchTextInput
 
@@ -37,14 +40,15 @@
 
     def widget_attrs(self, widget: Widget) -> Any:
         attrs = super().widget_attrs(widget)        
         attrs.update({'query_function_name': self.query_function_name,
                       'min_search_length': self.min_search_length,
                       'id': f"search-input-{random.randint(0, 1000000000)}",
                       "search_field" : self.search_field,
+                      "model_field": True
                       })
         return attrs
     
     def to_python(self, value):
         if not value :
             return None
         return self.model.objects.get(id=value)
```

### Comparing `django-search-input-field-0.1.8/django_search_input_field/form.py` & `django-search-input-field-0.1.9/django_search_input_field/form.py`

 * *Files identical despite different names*

### Comparing `django-search-input-field-0.1.8/django_search_input_field/options.py` & `django-search-input-field-0.1.9/django_search_input_field/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     serializer = None
     
     def object_str(self, obj):
         return str(obj)
     
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
-        API_REGISTER().register(cls, cls.query_function_name)
+        API_REGISTER().register(cls, cls.query_function_name) 
     
     
     def get_permissions(self, request):
         return request.user.is_authenticated
     
     def get_queryset(self)->QuerySet:
         return self.model.objects.all()
@@ -71,8 +71,40 @@
                 key = key + '__icontains'
             function_filters[key] = value
         
         return self.get_queryset().filter(**function_filters)
         
     def get_filtered_options(self, function_filters, search_key):
         options = self.get_filtered_queryset(function_filters, search_key)
-        return [ModelOption(option, self.serializer, self.object_str) for option in options]
+        return [ModelOption(option, self.serializer, self.object_str) for option in options]
+    
+    
+class SearchFieldOptions():
+    model = None
+    query_function_name = None
+            
+    def object_str(self, obj):
+        return str(obj)
+    
+    def __init_subclass__(cls, **kwargs):
+        super().__init_subclass__(**kwargs)
+        API_REGISTER().register(cls, cls.query_function_name) 
+    
+    
+    def get_permissions(self, request):
+        return request.user.is_authenticated
+    
+    def get_queryset(self)->QuerySet:
+        return self.model.objects.all()
+    
+    def get_filtered_queryset(self, function_filters:dict, search_key)->QuerySet:
+        for key, value in function_filters.copy().items():
+            del function_filters[key]
+            if search_key == key:
+                key = key + '__icontains'
+            function_filters[key] = value
+        
+        return self.get_queryset().filter(**function_filters).values_list(search_key, flat=True).distinct()
+        
+    def get_filtered_options(self, function_filters, search_key):
+        options = self.get_filtered_queryset(function_filters, search_key)
+        return [InputOption(option, option) for option in options]
```

### Comparing `django-search-input-field-0.1.8/django_search_input_field/query_function_register.py` & `django-search-input-field-0.1.9/django_search_input_field/query_function_register.py`

 * *Files identical despite different names*

### Comparing `django-search-input-field-0.1.8/django_search_input_field/static/django_search_input_field.js` & `django-search-input-field-0.1.9/django_search_input_field/static/django_search_input_field.js`

 * *Files identical despite different names*

### Comparing `django-search-input-field-0.1.8/django_search_input_field/templates/select_search_text_input.html` & `django-search-input-field-0.1.9/django_search_input_field/templates/select_search_text_input.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 <style>
     .select2-results__option {
         color: black !important;
     }
     .select2-rendered__match {
         background-color: yellow;
       }
+  
 </style>  
 {% load django_search_input_field static %}
-{% search_field_get_init_value widget.attrs.query_function_name widget.value as inital_value %}
+{% search_field_get_init_value widget.attrs.query_function_name widget.attrs.model_field widget.value  as inital_value %}
+
+
 <div id="django-search-url" url="{% url 'get_search_input_query_result' %}" style='display: none;'></div>
 
 <select class="select2-search-query" query_function="{{ widget.attrs.query_function_name }}" 
-style="width: 100%;"
- name="{{ widget.name }}" 
+style="width: auto;min-width: 200px; max-width: 100%;" 
+name="{{ widget.name }}" 
  id="{{ widget.attrs.id }}"
  {% include "django/forms/widgets/attrs.html" %}
  >
 {% if inital_value %}
     <option value="{{ inital_value.id }}" selected="selected">{{ inital_value.string }}</option>
 {% endif %}
 </select>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 {% load django_search_input_field static %} {% search_field_get_init_value
-widget.attrs.query_function_name widget.value as inital_value %}
+widget.attrs.query_function_name widget.attrs.model_field widget.value as
+inital_value %}
 % include "django/forms/widgets/attrs.html" %} > {% if inital_value %}
 {{ inital_value.string }}
 {% endif %}
```

### Comparing `django-search-input-field-0.1.8/django_search_input_field.egg-info/SOURCES.txt` & `django-search-input-field-0.1.9/django_search_input_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-search-input-field-0.1.8/setup.py` & `django-search-input-field-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Remove the unused import statement for glob
 # Add the templates folder to the build configuration
 from setuptools import setup, find_packages
 
 
 setup(
     name='django-search-input-field',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     author="Treyd Services AB",
     author_email='support@treyd.io',
     packages=find_packages(include=['django_search_input_field', 'django_search_input_field.*',
                                     'django_search_input_field.templates', 'django_search_input_field.templates.*']),
     include_package_data=True,
     package_data={'django_search_input_field': ['django_search_input_field/templates/*']},
```

