# Comparing `tmp/iommi-6.8.0.tar.gz` & `tmp/iommi-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iommi-6.8.0.tar", last modified: Wed Mar 27 10:00:42 2024, max compression
+gzip compressed data, was "iommi-7.0.0.tar", last modified: Mon Apr 15 10:45:20 2024, max compression
```

## Comparing `iommi-6.8.0.tar` & `iommi-7.0.0.tar`

### file list

```diff
@@ -1,155 +1,157 @@
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.610711 iommi-6.8.0/
--rw-r--r--   0 boxed      (501) staff       (20)     1102 2024-02-18 13:30:36.000000 iommi-6.8.0/AUTHORS.rst
--rw-r--r--   0 boxed      (501) staff       (20)      212 2021-01-28 10:44:48.000000 iommi-6.8.0/CONTRIBUTING.rst
--rw-r--r--   0 boxed      (501) staff       (20)    42067 2024-03-27 09:57:49.000000 iommi-6.8.0/HISTORY.rst
--rw-r--r--   0 boxed      (501) staff       (20)     1485 2021-01-28 10:44:48.000000 iommi-6.8.0/LICENSE
--rw-r--r--   0 boxed      (501) staff       (20)      332 2022-01-21 14:21:52.000000 iommi-6.8.0/MANIFEST.in
--rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-03-27 10:00:42.610634 iommi-6.8.0/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)     2781 2023-04-05 18:05:05.000000 iommi-6.8.0/README.rst
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.594559 iommi-6.8.0/iommi/
--rw-r--r--   0 boxed      (501) staff       (20)     8196 2024-03-17 14:25:56.000000 iommi-6.8.0/iommi/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)     3606 2024-03-27 09:59:35.000000 iommi-6.8.0/iommi/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)     6391 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/_db_compat.py
--rw-r--r--   0 boxed      (501) staff       (20)     6578 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/_web_compat.py
--rw-r--r--   0 boxed      (501) staff       (20)      532 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/_web_compat_flask.py
--rw-r--r--   0 boxed      (501) staff       (20)     5757 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/action.py
--rw-r--r--   0 boxed      (501) staff       (20)    21315 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/admin.py
--rw-r--r--   0 boxed      (501) staff       (20)     1892 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/apps.py
--rw-r--r--   0 boxed      (501) staff       (20)     1950 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/asset.py
--rw-r--r--   0 boxed      (501) staff       (20)     5010 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/attrs.py
--rw-r--r--   0 boxed      (501) staff       (20)     2591 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/base.py
--rw-r--r--   0 boxed      (501) staff       (20)     4902 2022-01-19 10:19:49.000000 iommi-6.8.0/iommi/datetime_parsing.py
--rw-r--r--   0 boxed      (501) staff       (20)    11898 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/debug.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.596724 iommi-6.8.0/iommi/declarative/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-6.8.0/iommi/declarative/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)     5461 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/declarative/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)      571 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/declarative/dispatch.py
--rw-r--r--   0 boxed      (501) staff       (20)     7994 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/declarative/namespace.py
--rw-r--r--   0 boxed      (501) staff       (20)     1938 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/declarative/util.py
--rw-r--r--   0 boxed      (501) staff       (20)     1501 2023-09-06 07:14:35.000000 iommi-6.8.0/iommi/declarative/with_meta.py
--rw-r--r--   0 boxed      (501) staff       (20)    12419 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/docs.py
--rw-r--r--   0 boxed      (501) staff       (20)    16853 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/edit_table.py
--rw-r--r--   0 boxed      (501) staff       (20)     3769 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/endpoint.py
--rw-r--r--   0 boxed      (501) staff       (20)     1477 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/error.py
--rw-r--r--   0 boxed      (501) staff       (20)     5018 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/evaluate.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.597289 iommi-6.8.0/iommi/experimental/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-6.8.0/iommi/experimental/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-6.8.0/iommi/experimental/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)      133 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/experimental/edit_table.py
--rw-r--r--   0 boxed      (501) staff       (20)    71768 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/form.py
--rw-r--r--   0 boxed      (501) staff       (20)     8184 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/fragment.py
--rw-r--r--   0 boxed      (501) staff       (20)    10165 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/from_model.py
--rw-r--r--   0 boxed      (501) staff       (20)    19710 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/live_edit.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.597503 iommi-6.8.0/iommi/locale/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-6.8.0/iommi/locale/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.574169 iommi-6.8.0/iommi/locale/cs/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.598113 iommi-6.8.0/iommi/locale/cs/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     4410 2023-12-13 09:01:15.000000 iommi-6.8.0/iommi/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7115 2023-11-22 17:28:48.000000 iommi-6.8.0/iommi/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.598413 iommi-6.8.0/iommi/locale/de/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-6.8.0/iommi/locale/de/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.598952 iommi-6.8.0/iommi/locale/de/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     4442 2023-12-13 09:01:15.000000 iommi-6.8.0/iommi/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7751 2023-11-22 17:28:48.000000 iommi-6.8.0/iommi/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.599236 iommi-6.8.0/iommi/locale/sv/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-6.8.0/iommi/locale/sv/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.599648 iommi-6.8.0/iommi/locale/sv/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     5588 2023-12-13 09:01:15.000000 iommi-6.8.0/iommi/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7390 2023-11-22 17:28:48.000000 iommi-6.8.0/iommi/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.574504 iommi-6.8.0/iommi/locale/uk/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.600231 iommi-6.8.0/iommi/locale/uk/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     5610 2023-12-13 09:01:15.000000 iommi-6.8.0/iommi/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     8431 2023-11-22 17:28:48.000000 iommi-6.8.0/iommi/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.574608 iommi-6.8.0/iommi/locale/zh_Hans/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.600807 iommi-6.8.0/iommi/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 boxed      (501) staff       (20)     3975 2023-12-13 09:01:15.000000 iommi-6.8.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 boxed      (501) staff       (20)     7182 2023-11-22 17:28:48.000000 iommi-6.8.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 boxed      (501) staff       (20)    10204 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/member.py
--rw-r--r--   0 boxed      (501) staff       (20)    11141 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/menu.py
--rw-r--r--   0 boxed      (501) staff       (20)     3761 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/page.py
--rw-r--r--   0 boxed      (501) staff       (20)     8450 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/part.py
--rw-r--r--   0 boxed      (501) staff       (20)     4729 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/path.py
--rw-r--r--   0 boxed      (501) staff       (20)    10196 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/profiling.py
--rw-r--r--   0 boxed      (501) staff       (20)    36691 2024-03-27 09:47:35.000000 iommi-6.8.0/iommi/query.py
--rw-r--r--   0 boxed      (501) staff       (20)     8657 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/refinable.py
--rw-r--r--   0 boxed      (501) staff       (20)     2717 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/shortcut.py
--rw-r--r--   0 boxed      (501) staff       (20)     2540 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/sort_after.py
--rw-r--r--   0 boxed      (501) staff       (20)    17399 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/sql_trace.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.601072 iommi-6.8.0/iommi/static/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-6.8.0/iommi/static/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.601379 iommi-6.8.0/iommi/static/js/
--rw-r--r--   0 boxed      (501) staff       (20)    22012 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/static/js/iommi.js
--rw-r--r--   0 boxed      (501) staff       (20)     3716 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/struct.py
--rw-r--r--   0 boxed      (501) staff       (20)    10219 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/style.py
--rw-r--r--   0 boxed      (501) staff       (20)     5437 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/style_base.py
--rw-r--r--   0 boxed      (501) staff       (20)     6372 2023-10-23 18:24:08.000000 iommi-6.8.0/iommi/style_bootstrap.py
--rw-r--r--   0 boxed      (501) staff       (20)     6001 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/style_bootstrap5.py
--rw-r--r--   0 boxed      (501) staff       (20)      627 2023-11-23 15:03:08.000000 iommi-6.8.0/iommi/style_bootstrap_docs.py
--rw-r--r--   0 boxed      (501) staff       (20)      783 2024-01-31 10:54:17.000000 iommi-6.8.0/iommi/style_bootstrap_icons.py
--rw-r--r--   0 boxed      (501) staff       (20)     4529 2024-01-22 08:06:57.000000 iommi-6.8.0/iommi/style_bulma.py
--rw-r--r--   0 boxed      (501) staff       (20)     1856 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/style_django_admin.py
--rw-r--r--   0 boxed      (501) staff       (20)      793 2024-01-31 10:54:17.000000 iommi-6.8.0/iommi/style_font_awesome_4.py
--rw-r--r--   0 boxed      (501) staff       (20)     2551 2022-01-19 10:19:49.000000 iommi-6.8.0/iommi/style_foundation.py
--rw-r--r--   0 boxed      (501) staff       (20)     3817 2023-09-06 07:14:35.000000 iommi-6.8.0/iommi/style_semantic_ui.py
--rw-r--r--   0 boxed      (501) staff       (20)      934 2024-02-26 08:28:08.000000 iommi-6.8.0/iommi/style_test_base.py
--rw-r--r--   0 boxed      (501) staff       (20)     1775 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/style_uikit.py
--rw-r--r--   0 boxed      (501) staff       (20)      309 2023-02-14 18:44:36.000000 iommi-6.8.0/iommi/style_water.py
--rw-r--r--   0 boxed      (501) staff       (20)     1887 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/synthetic_traceback.py
--rw-r--r--   0 boxed      (501) staff       (20)    82936 2024-03-27 09:47:35.000000 iommi-6.8.0/iommi/table.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.601733 iommi-6.8.0/iommi/templates/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-09-30 13:08:45.000000 iommi-6.8.0/iommi/templates/.DS_Store
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.602471 iommi-6.8.0/iommi/templates/iommi/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 08:59:39.000000 iommi-6.8.0/iommi/templates/iommi/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)      623 2023-09-26 07:33:27.000000 iommi-6.8.0/iommi/templates/iommi/base.html
--rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-6.8.0/iommi/templates/iommi/blank.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.604383 iommi-6.8.0/iommi/templates/iommi/form/
--rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 19:05:37.000000 iommi-6.8.0/iommi/templates/iommi/form/.DS_Store
--rw-r--r--   0 boxed      (501) staff       (20)      873 2021-01-28 10:44:48.000000 iommi-6.8.0/iommi/templates/iommi/form/actions.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.604517 iommi-6.8.0/iommi/templates/iommi/form/bulma/
--rw-r--r--   0 boxed      (501) staff       (20)      255 2023-02-14 18:44:36.000000 iommi-6.8.0/iommi/templates/iommi/form/bulma/field.html
--rw-r--r--   0 boxed      (501) staff       (20)      418 2023-09-06 07:14:35.000000 iommi-6.8.0/iommi/templates/iommi/form/checkboxes.html
--rw-r--r--   0 boxed      (501) staff       (20)      495 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/templates/iommi/form/choice.html
--rw-r--r--   0 boxed      (501) staff       (20)      709 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/templates/iommi/form/choice_select2.html
--rw-r--r--   0 boxed      (501) staff       (20)      353 2022-01-19 10:19:49.000000 iommi-6.8.0/iommi/templates/iommi/form/form.html
--rw-r--r--   0 boxed      (501) staff       (20)       78 2022-01-19 10:19:49.000000 iommi-6.8.0/iommi/templates/iommi/form/heading.html
--rw-r--r--   0 boxed      (501) staff       (20)      187 2022-02-09 12:13:49.000000 iommi-6.8.0/iommi/templates/iommi/form/image_row.html
--rw-r--r--   0 boxed      (501) staff       (20)      415 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/templates/iommi/form/radio.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.605180 iommi-6.8.0/iommi/templates/iommi/form/semantic_ui/
--rw-r--r--   0 boxed      (501) staff       (20)      499 2023-09-06 07:14:35.000000 iommi-6.8.0/iommi/templates/iommi/form/semantic_ui/checkboxes.html
--rw-r--r--   0 boxed      (501) staff       (20)      496 2021-01-28 10:44:48.000000 iommi-6.8.0/iommi/templates/iommi/form/semantic_ui/radio.html
--rw-r--r--   0 boxed      (501) staff       (20)      166 2022-03-31 08:29:44.000000 iommi-6.8.0/iommi/templates/iommi/form/semantic_ui/row_checkbox.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.605405 iommi-6.8.0/iommi/templates/iommi/form/uikit/
--rw-r--r--   0 boxed      (501) staff       (20)      379 2023-02-14 18:44:36.000000 iommi-6.8.0/iommi/templates/iommi/form/uikit/row_checkbox.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.605999 iommi-6.8.0/iommi/templates/iommi/query/
--rw-r--r--   0 boxed      (501) staff       (20)     2622 2022-01-19 10:19:49.000000 iommi-6.8.0/iommi/templates/iommi/query/advanced.html
--rw-r--r--   0 boxed      (501) staff       (20)     1498 2021-04-15 06:01:07.000000 iommi-6.8.0/iommi/templates/iommi/query/form.html
--rw-r--r--   0 boxed      (501) staff       (20)     2808 2021-01-28 10:44:48.000000 iommi-6.8.0/iommi/templates/iommi/query/form_toggle_script.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.607740 iommi-6.8.0/iommi/templates/iommi/table/
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.607981 iommi-6.8.0/iommi/templates/iommi/table/bootstrap/
--rw-r--r--   0 boxed      (501) staff       (20)     1526 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/templates/iommi/table/bootstrap/paginator.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.608173 iommi-6.8.0/iommi/templates/iommi/table/bulma/
--rw-r--r--   0 boxed      (501) staff       (20)     1555 2024-01-22 08:06:57.000000 iommi-6.8.0/iommi/templates/iommi/table/bulma/paginator.html
--rw-r--r--   0 boxed      (501) staff       (20)      188 2023-09-21 07:03:11.000000 iommi-6.8.0/iommi/templates/iommi/table/header.html
--rw-r--r--   0 boxed      (501) staff       (20)     2303 2021-01-28 10:44:48.000000 iommi-6.8.0/iommi/templates/iommi/table/js_select_all.html
--rw-r--r--   0 boxed      (501) staff       (20)     1814 2023-02-14 18:44:36.000000 iommi-6.8.0/iommi/templates/iommi/table/paginator.html
--rw-r--r--   0 boxed      (501) staff       (20)      102 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/templates/iommi/table/row_group.html
--rw-r--r--   0 boxed      (501) staff       (20)      196 2022-10-31 14:55:23.000000 iommi-6.8.0/iommi/templates/iommi/table/select_column_header.html
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.608430 iommi-6.8.0/iommi/templates/iommi/table/semantic_ui/
--rw-r--r--   0 boxed      (501) staff       (20)     1091 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/templates/iommi/table/semantic_ui/paginator.html
--rw-r--r--   0 boxed      (501) staff       (20)       18 2023-02-13 19:03:15.000000 iommi-6.8.0/iommi/templates/iommi/table/table.html
--rw-r--r--   0 boxed      (501) staff       (20)      508 2021-04-15 06:01:07.000000 iommi-6.8.0/iommi/templates/iommi/table/table_container.html
--rw-r--r--   0 boxed      (501) staff       (20)      209 2021-01-28 10:44:48.000000 iommi-6.8.0/iommi/templates/iommi/table/table_header_rows.html
--rw-r--r--   0 boxed      (501) staff       (20)      560 2023-04-26 11:31:39.000000 iommi-6.8.0/iommi/templates/iommi/table/table_tag.html
--rw-r--r--   0 boxed      (501) staff       (20)      207 2022-01-13 18:46:04.000000 iommi-6.8.0/iommi/thread_locals.py
--rw-r--r--   0 boxed      (501) staff       (20)    11874 2024-03-07 08:19:20.000000 iommi-6.8.0/iommi/traversable.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-03-27 10:00:42.595504 iommi-6.8.0/iommi.egg-info/
--rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-03-27 10:00:42.000000 iommi-6.8.0/iommi.egg-info/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)     3537 2024-03-27 10:00:42.000000 iommi-6.8.0/iommi.egg-info/SOURCES.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2024-03-27 10:00:42.000000 iommi-6.8.0/iommi.egg-info/dependency_links.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2021-01-28 11:41:36.000000 iommi-6.8.0/iommi.egg-info/not-zip-safe
--rw-r--r--   0 boxed      (501) staff       (20)       22 2024-03-27 10:00:42.000000 iommi-6.8.0/iommi.egg-info/requires.txt
--rw-r--r--   0 boxed      (501) staff       (20)        6 2024-03-27 10:00:42.000000 iommi-6.8.0/iommi.egg-info/top_level.txt
--rw-r--r--   0 boxed      (501) staff       (20)      534 2024-03-07 08:19:20.000000 iommi-6.8.0/pyproject.toml
--rw-r--r--   0 boxed      (501) staff       (20)       10 2023-02-13 19:03:15.000000 iommi-6.8.0/requirements.txt
--rw-r--r--   0 boxed      (501) staff       (20)     1158 2024-03-27 10:00:42.611163 iommi-6.8.0/setup.cfg
--rwxr-xr-x   0 boxed      (501) staff       (20)     2893 2024-03-07 08:19:20.000000 iommi-6.8.0/setup.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.745983 iommi-7.0.0/
+-rw-r--r--   0 boxed      (501) staff       (20)     1102 2024-02-18 13:30:36.000000 iommi-7.0.0/AUTHORS.rst
+-rw-r--r--   0 boxed      (501) staff       (20)      212 2021-01-28 10:44:48.000000 iommi-7.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 boxed      (501) staff       (20)    42689 2024-04-15 10:35:27.000000 iommi-7.0.0/HISTORY.rst
+-rw-r--r--   0 boxed      (501) staff       (20)     1485 2021-01-28 10:44:48.000000 iommi-7.0.0/LICENSE
+-rw-r--r--   0 boxed      (501) staff       (20)      332 2022-01-21 14:21:52.000000 iommi-7.0.0/MANIFEST.in
+-rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-04-15 10:45:20.745852 iommi-7.0.0/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)     2781 2023-04-05 18:05:05.000000 iommi-7.0.0/README.rst
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.724551 iommi-7.0.0/iommi/
+-rw-r--r--   0 boxed      (501) staff       (20)     8196 2024-04-06 11:17:02.000000 iommi-7.0.0/iommi/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)     3606 2024-04-15 10:38:38.000000 iommi-7.0.0/iommi/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6391 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/_db_compat.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6578 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/_web_compat.py
+-rw-r--r--   0 boxed      (501) staff       (20)      532 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/_web_compat_flask.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5757 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/action.py
+-rw-r--r--   0 boxed      (501) staff       (20)    21492 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/admin.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1892 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/apps.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1950 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/asset.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5010 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/attrs.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2591 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4902 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/datetime_parsing.py
+-rw-r--r--   0 boxed      (501) staff       (20)    11898 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/debug.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.727993 iommi-7.0.0/iommi/declarative/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-7.0.0/iommi/declarative/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)     5461 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/declarative/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)      571 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/declarative/dispatch.py
+-rw-r--r--   0 boxed      (501) staff       (20)     7994 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/declarative/namespace.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1938 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/declarative/util.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1501 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/declarative/with_meta.py
+-rw-r--r--   0 boxed      (501) staff       (20)    12419 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/docs.py
+-rw-r--r--   0 boxed      (501) staff       (20)    17950 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/edit_table.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3769 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/endpoint.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1477 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/error.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5018 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/evaluate.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.728917 iommi-7.0.0/iommi/experimental/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-12-11 09:30:40.000000 iommi-7.0.0/iommi/experimental/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/experimental/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)      133 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/experimental/edit_table.py
+-rw-r--r--   0 boxed      (501) staff       (20)    71882 2024-04-15 10:35:20.000000 iommi-7.0.0/iommi/form.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8184 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/fragment.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10165 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/from_model.py
+-rw-r--r--   0 boxed      (501) staff       (20)    19710 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/live_edit.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.729234 iommi-7.0.0/iommi/locale/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-7.0.0/iommi/locale/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.699282 iommi-7.0.0/iommi/locale/cs/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.729828 iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     4410 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7115 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.730226 iommi-7.0.0/iommi/locale/de/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-7.0.0/iommi/locale/de/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.730827 iommi-7.0.0/iommi/locale/de/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     4442 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7751 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.731134 iommi-7.0.0/iommi/locale/sv/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-01-02 19:23:31.000000 iommi-7.0.0/iommi/locale/sv/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.731590 iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     5588 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7390 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.699837 iommi-7.0.0/iommi/locale/uk/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.732145 iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     5610 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     8431 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.699998 iommi-7.0.0/iommi/locale/zh_Hans/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.732768 iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 boxed      (501) staff       (20)     3975 2023-12-13 09:01:15.000000 iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 boxed      (501) staff       (20)     7182 2023-11-22 17:28:48.000000 iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 boxed      (501) staff       (20)    10204 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/member.py
+-rw-r--r--   0 boxed      (501) staff       (20)    11141 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/menu.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3761 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/page.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8450 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/part.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4729 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/path.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10196 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/profiling.py
+-rw-r--r--   0 boxed      (501) staff       (20)    36786 2024-04-15 07:51:09.000000 iommi-7.0.0/iommi/query.py
+-rw-r--r--   0 boxed      (501) staff       (20)     8657 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/refinable.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2717 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/shortcut.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2540 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/sort_after.py
+-rw-r--r--   0 boxed      (501) staff       (20)    17400 2024-04-15 10:17:16.000000 iommi-7.0.0/iommi/sql_trace.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.733190 iommi-7.0.0/iommi/static/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2024-01-05 19:32:48.000000 iommi-7.0.0/iommi/static/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.733529 iommi-7.0.0/iommi/static/js/
+-rw-r--r--   0 boxed      (501) staff       (20)    19226 2024-04-15 07:51:09.000000 iommi-7.0.0/iommi/static/js/iommi.js
+-rw-r--r--   0 boxed      (501) staff       (20)     3716 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/struct.py
+-rw-r--r--   0 boxed      (501) staff       (20)    10314 2024-04-15 08:37:40.000000 iommi-7.0.0/iommi/style.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5437 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/style_base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6372 2023-10-23 18:24:08.000000 iommi-7.0.0/iommi/style_bootstrap.py
+-rw-r--r--   0 boxed      (501) staff       (20)     6001 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/style_bootstrap5.py
+-rw-r--r--   0 boxed      (501) staff       (20)      630 2024-04-15 08:39:12.000000 iommi-7.0.0/iommi/style_bootstrap_docs.py
+-rw-r--r--   0 boxed      (501) staff       (20)      783 2024-01-31 10:54:17.000000 iommi-7.0.0/iommi/style_bootstrap_icons.py
+-rw-r--r--   0 boxed      (501) staff       (20)     4529 2024-01-22 08:06:57.000000 iommi-7.0.0/iommi/style_bulma.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1856 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/style_django_admin.py
+-rw-r--r--   0 boxed      (501) staff       (20)      793 2024-01-31 10:54:17.000000 iommi-7.0.0/iommi/style_font_awesome_4.py
+-rw-r--r--   0 boxed      (501) staff       (20)      785 2024-04-15 08:36:19.000000 iommi-7.0.0/iommi/style_font_awesome_6.py
+-rw-r--r--   0 boxed      (501) staff       (20)     2551 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/style_foundation.py
+-rw-r--r--   0 boxed      (501) staff       (20)     3817 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/style_semantic_ui.py
+-rw-r--r--   0 boxed      (501) staff       (20)      934 2024-02-26 08:28:08.000000 iommi-7.0.0/iommi/style_test_base.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1775 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/style_uikit.py
+-rw-r--r--   0 boxed      (501) staff       (20)      309 2023-02-14 18:44:36.000000 iommi-7.0.0/iommi/style_water.py
+-rw-r--r--   0 boxed      (501) staff       (20)     1887 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/synthetic_traceback.py
+-rw-r--r--   0 boxed      (501) staff       (20)    83012 2024-04-15 07:51:09.000000 iommi-7.0.0/iommi/table.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.734191 iommi-7.0.0/iommi/templates/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2023-09-30 13:08:45.000000 iommi-7.0.0/iommi/templates/.DS_Store
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.735117 iommi-7.0.0/iommi/templates/iommi/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 08:59:39.000000 iommi-7.0.0/iommi/templates/iommi/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)      623 2023-09-26 07:33:27.000000 iommi-7.0.0/iommi/templates/iommi/base.html
+-rw-r--r--   0 boxed      (501) staff       (20)        0 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/templates/iommi/blank.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.737651 iommi-7.0.0/iommi/templates/iommi/form/
+-rw-r--r--   0 boxed      (501) staff       (20)     6148 2022-12-11 19:05:37.000000 iommi-7.0.0/iommi/templates/iommi/form/.DS_Store
+-rw-r--r--   0 boxed      (501) staff       (20)      873 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/form/actions.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.737957 iommi-7.0.0/iommi/templates/iommi/form/bulma/
+-rw-r--r--   0 boxed      (501) staff       (20)      255 2023-02-14 18:44:36.000000 iommi-7.0.0/iommi/templates/iommi/form/bulma/field.html
+-rw-r--r--   0 boxed      (501) staff       (20)      418 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/templates/iommi/form/checkboxes.html
+-rw-r--r--   0 boxed      (501) staff       (20)      495 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/form/choice.html
+-rw-r--r--   0 boxed      (501) staff       (20)      709 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/form/choice_select2.html
+-rw-r--r--   0 boxed      (501) staff       (20)      440 2024-04-15 07:32:29.000000 iommi-7.0.0/iommi/templates/iommi/form/form.html
+-rw-r--r--   0 boxed      (501) staff       (20)       78 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/templates/iommi/form/heading.html
+-rw-r--r--   0 boxed      (501) staff       (20)      187 2022-02-09 12:13:49.000000 iommi-7.0.0/iommi/templates/iommi/form/image_row.html
+-rw-r--r--   0 boxed      (501) staff       (20)      415 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/form/radio.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.738919 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/
+-rw-r--r--   0 boxed      (501) staff       (20)      499 2023-09-06 07:14:35.000000 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/checkboxes.html
+-rw-r--r--   0 boxed      (501) staff       (20)      496 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/radio.html
+-rw-r--r--   0 boxed      (501) staff       (20)      166 2022-03-31 08:29:44.000000 iommi-7.0.0/iommi/templates/iommi/form/semantic_ui/row_checkbox.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.739204 iommi-7.0.0/iommi/templates/iommi/form/uikit/
+-rw-r--r--   0 boxed      (501) staff       (20)      379 2023-02-14 18:44:36.000000 iommi-7.0.0/iommi/templates/iommi/form/uikit/row_checkbox.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.740170 iommi-7.0.0/iommi/templates/iommi/query/
+-rw-r--r--   0 boxed      (501) staff       (20)     2622 2022-01-19 10:19:49.000000 iommi-7.0.0/iommi/templates/iommi/query/advanced.html
+-rw-r--r--   0 boxed      (501) staff       (20)     1498 2021-04-15 06:01:07.000000 iommi-7.0.0/iommi/templates/iommi/query/form.html
+-rw-r--r--   0 boxed      (501) staff       (20)     2808 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/query/form_toggle_script.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.743188 iommi-7.0.0/iommi/templates/iommi/table/
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.743515 iommi-7.0.0/iommi/templates/iommi/table/bootstrap/
+-rw-r--r--   0 boxed      (501) staff       (20)     1526 2024-04-15 07:16:46.000000 iommi-7.0.0/iommi/templates/iommi/table/bootstrap/paginator.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.743829 iommi-7.0.0/iommi/templates/iommi/table/bulma/
+-rw-r--r--   0 boxed      (501) staff       (20)     1555 2024-01-22 08:06:57.000000 iommi-7.0.0/iommi/templates/iommi/table/bulma/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)      125 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/templates/iommi/table/edit_table_container.html
+-rw-r--r--   0 boxed      (501) staff       (20)      188 2023-09-21 07:03:11.000000 iommi-7.0.0/iommi/templates/iommi/table/header.html
+-rw-r--r--   0 boxed      (501) staff       (20)     2303 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/table/js_select_all.html
+-rw-r--r--   0 boxed      (501) staff       (20)     1814 2024-04-15 07:16:49.000000 iommi-7.0.0/iommi/templates/iommi/table/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)      102 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/table/row_group.html
+-rw-r--r--   0 boxed      (501) staff       (20)      196 2022-10-31 14:55:23.000000 iommi-7.0.0/iommi/templates/iommi/table/select_column_header.html
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.744138 iommi-7.0.0/iommi/templates/iommi/table/semantic_ui/
+-rw-r--r--   0 boxed      (501) staff       (20)     1091 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/table/semantic_ui/paginator.html
+-rw-r--r--   0 boxed      (501) staff       (20)       18 2023-02-13 19:03:15.000000 iommi-7.0.0/iommi/templates/iommi/table/table.html
+-rw-r--r--   0 boxed      (501) staff       (20)      669 2024-04-15 07:14:49.000000 iommi-7.0.0/iommi/templates/iommi/table/table_container.html
+-rw-r--r--   0 boxed      (501) staff       (20)      209 2021-01-28 10:44:48.000000 iommi-7.0.0/iommi/templates/iommi/table/table_header_rows.html
+-rw-r--r--   0 boxed      (501) staff       (20)      560 2023-04-26 11:31:39.000000 iommi-7.0.0/iommi/templates/iommi/table/table_tag.html
+-rw-r--r--   0 boxed      (501) staff       (20)      207 2022-01-13 18:46:04.000000 iommi-7.0.0/iommi/thread_locals.py
+-rw-r--r--   0 boxed      (501) staff       (20)    11874 2024-03-07 08:19:20.000000 iommi-7.0.0/iommi/traversable.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-15 10:45:20.725965 iommi-7.0.0/iommi.egg-info/
+-rw-r--r--   0 boxed      (501) staff       (20)     3079 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)     3621 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/SOURCES.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/dependency_links.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2021-01-28 11:41:36.000000 iommi-7.0.0/iommi.egg-info/not-zip-safe
+-rw-r--r--   0 boxed      (501) staff       (20)       22 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/requires.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        6 2024-04-15 10:45:20.000000 iommi-7.0.0/iommi.egg-info/top_level.txt
+-rw-r--r--   0 boxed      (501) staff       (20)      534 2024-03-07 08:19:20.000000 iommi-7.0.0/pyproject.toml
+-rw-r--r--   0 boxed      (501) staff       (20)       10 2023-02-13 19:03:15.000000 iommi-7.0.0/requirements.txt
+-rw-r--r--   0 boxed      (501) staff       (20)     1158 2024-04-15 10:45:20.746782 iommi-7.0.0/setup.cfg
+-rwxr-xr-x   0 boxed      (501) staff       (20)     2893 2024-03-07 08:19:20.000000 iommi-7.0.0/setup.py
```

### Comparing `iommi-6.8.0/AUTHORS.rst` & `iommi-7.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/HISTORY.rst` & `iommi-7.0.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 Changelog
 ---------
 
-6.7.1 (2024-03-27)
+7.0.0 (2024-04-15)
+~~~~~~~~~~~~~~~~~~
+
+* `EditTable`s `EditColumn.edit` namespace is now called `field`. This is a breaking change. There was a namespace conflict between `Column.edit` and `EditColumn.edit`.
+
+* `EditTable` and bulk editing and filtering now compose cleanly
+
+* Changed default style to Bootstrap 5
+
+* Allow styling of `EditTable`/`EditColumn`
+
+* Nested forms respect if the parent form is non-editable
+
+* SQL trace for N+1 problems will now print the last found query+traceback instead of the first. This should increase the odds of it showing something useful.
+
+* Removed deprecated JavaScript functions
+
+6.8.0 (2024-03-27)
 ~~~~~~~~~~~~~~~~~~
 
 * `table.Column.boolean` changed from fontawesome icon to unicode check mark
 
 * `<meta>` viewport by default
 
 * `SearchVectorField` default None factory
```

### Comparing `iommi-6.8.0/LICENSE` & `iommi-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/PKG-INFO` & `iommi-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iommi
-Version: 6.8.0
+Version: 7.0.0
 Summary: iommi is a high level framework built on django
 Home-page: https://github.com/iommirocks/iommi
 Author: Anders Hovmöller
 Author-email: boxed@killingar.net
 License: BSD
 Keywords: iommi
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iommi-6.8.0/README.rst` & `iommi-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/.DS_Store` & `iommi-7.0.0/iommi/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -253,26 +253,26 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 001e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 007a 63d9 0000 000b 005f 005f 0070  ...zc......_._.p
+00001030: 0000 007a 4c87 0000 000b 005f 005f 0070  ...zL......_._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 4a12 1bc0  moDDblob....J...
-00001060: e6cc c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 0cb6 dc6a  moDDblob.......j
+00001060: b4de c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 4a12 1bc0 e6cc  dDblob....J.....
+00001080: 6444 626c 6f62 0000 0008 0cb6 dc6a b4de  dDblob.......j..
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0084 0000 0000 000b  comp............
+000010b0: 636f 6d70 0000 0000 0083 f000 0000 000b  comp............
 000010c0: 0064 0065 0063 006c 0061 0072 0061 0074  .d.e.c.l.a.r.a.t
 000010d0: 0069 0076 0065 6c67 3153 636f 6d70 0000  .i.v.elg1Scomp..
-000010e0: 0000 000c 11d3 0000 000b 0064 0065 0063  ...........d.e.c
+000010e0: 0000 000c 11d5 0000 000b 0064 0065 0063  ...........d.e.c
 000010f0: 006c 0061 0072 0061 0074 0069 0076 0065  .l.a.r.a.t.i.v.e
 00001100: 6d6f 4444 626c 6f62 0000 0008 c304 0304  moDDblob........
 00001110: d8cc c541 0000 000b 0064 0065 0063 006c  ...A.....d.e.c.l
 00001120: 0061 0072 0061 0074 0069 0076 0065 6d6f  .a.r.a.t.i.v.emo
 00001130: 6444 626c 6f62 0000 0008 c304 0304 d8cc  dDblob..........
 00001140: c541 0000 000b 0064 0065 0063 006c 0061  .A.....d.e.c.l.a
 00001150: 0072 0061 0074 0069 0076 0065 7068 3153  .r.a.t.i.v.eph1S
@@ -328,15 +328,15 @@
 00001470: 4444 626c 6f62 0000 0008 c31c 49cb 3149  DDblob......I.1I
 00001480: c541 0000 0006 0073 0074 0061 0074 0069  .A.....s.t.a.t.i
 00001490: 0063 6d6f 6444 626c 6f62 0000 0008 c31c  .cmodDblob......
 000014a0: 49cb 3149 c541 0000 0006 0073 0074 0061  I.1I.A.....s.t.a
 000014b0: 0074 0069 0063 7068 3153 636f 6d70 0000  .t.i.cph1Scomp..
 000014c0: 0000 0000 8000 0000 0009 0074 0065 006d  ...........t.e.m
 000014d0: 0070 006c 0061 0074 0065 0073 6c67 3153  .p.l.a.t.e.slg1S
-000014e0: 636f 6d70 0000 0000 0000 a1ac 0000 0009  comp............
+000014e0: 636f 6d70 0000 0000 0000 a1aa 0000 0009  comp............
 000014f0: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
 00001500: 0073 6d6f 4444 626c 6f62 0000 0008 fda2  .smoDDblob......
 00001510: b6ff 0614 c341 0000 0009 0074 0065 006d  .....A.....t.e.m
 00001520: 0070 006c 0061 0074 0065 0073 6d6f 6444  .p.l.a.t.e.smodD
 00001530: 626c 6f62 0000 0008 fda2 b6ff 0614 c341  blob...........A
 00001540: 0000 0009 0074 0065 006d 0070 006c 0061  .....t.e.m.p.l.a
 00001550: 0074 0065 0073 7068 3153 636f 6d70 0000  .t.e.sph1Scomp..
```

### Comparing `iommi-6.8.0/iommi/__init__.py` & `iommi-7.0.0/iommi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '6.8.0'
+__version__ = '7.0.0'
 
 from functools import wraps
 
 import django
 from django.core.exceptions import ImproperlyConfigured
 
 from iommi._db_compat import (
```

### Comparing `iommi-6.8.0/iommi/_db_compat.py` & `iommi-7.0.0/iommi/_db_compat.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/_web_compat.py` & `iommi-7.0.0/iommi/_web_compat.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/_web_compat_flask.py` & `iommi-7.0.0/iommi/_web_compat_flask.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/action.py` & `iommi-7.0.0/iommi/action.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/admin.py` & `iommi-7.0.0/iommi/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     path,
     reverse,
 )
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext
 
 from iommi import (
+    EditTable,
     LAST,
     Field,
     Form,
     Fragment,
     Menu,
     MenuItem,
     Page,
@@ -116,15 +117,15 @@
     return read_config_wrapper
 
 
 @with_meta  # we need @with_meta again here to make sure this constructor gets all the meta arguments first
 class Admin(Page):
     class Meta:
         iommi_style = 'bootstrap'
-        table_class = Table
+        table_class = EditTable
         form_class = Form
         apps = EMPTY
         parts = EMPTY
 
     model: Type[Model] = Refinable()
     instance: Model = Refinable()
     app_name: str = Refinable()
@@ -351,17 +352,17 @@
             title=gettext('All models'),
             call_target__cls=cls.get_meta().table_class,
             call_target__attribute='div',
             sortable=False,
             rows=rows,
             page_size=None,
             columns__name=dict(
-                cell__url=lambda row, **_: row.url,
+                cell__url=lambda row, **_: row.url if getattr(row, 'pk', None) != '#sentinel#' else None,
                 display_name='',
-                cell__format=lambda row, **format_kwargs: row.format(row=row, **format_kwargs),
+                cell__format=lambda row, **format_kwargs: row.format(row=row, **format_kwargs) if getattr(row, 'pk', None) != '#sentinel#' else '',
             ),
         )
 
         add_models = setdefaults_path(
             Namespace(),
             include=settings.DEBUG,
             call_target__cls=cls.get_meta().table_class,
@@ -389,15 +390,15 @@
                     ),
                     # cell__url=lambda row, **_: f'{row.url}add_model/' if row.key else None,
                     after=LAST,
                 )
             ),
             columns__name=dict(
                 display_name='',
-                cell__format=lambda row, **format_kwargs: row.format(row=row, **format_kwargs),
+                cell__format=lambda row, **format_kwargs: row.format(row=row, **format_kwargs) if getattr(row, 'pk', None) != '#sentinel#' else '',
             ),
         )
 
         return cls(
             parts=dict(
                 all_models=table,
                 add_models_title=html.h1(gettext('Add models to admin'), include=settings.DEBUG),
```

### Comparing `iommi-6.8.0/iommi/apps.py` & `iommi-7.0.0/iommi/apps.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/asset.py` & `iommi-7.0.0/iommi/asset.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/attrs.py` & `iommi-7.0.0/iommi/attrs.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/base.py` & `iommi-7.0.0/iommi/base.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/datetime_parsing.py` & `iommi-7.0.0/iommi/datetime_parsing.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/debug.py` & `iommi-7.0.0/iommi/debug.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/declarative/.DS_Store` & `iommi-7.0.0/iommi/declarative/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/declarative/__init__.py` & `iommi-7.0.0/iommi/declarative/__init__.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/declarative/dispatch.py` & `iommi-7.0.0/iommi/declarative/dispatch.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/declarative/namespace.py` & `iommi-7.0.0/iommi/declarative/namespace.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/declarative/util.py` & `iommi-7.0.0/iommi/declarative/util.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/declarative/with_meta.py` & `iommi-7.0.0/iommi/declarative/with_meta.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/docs.py` & `iommi-7.0.0/iommi/docs.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/edit_table.py` & `iommi-7.0.0/iommi/edit_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from collections import defaultdict
 from typing import (
+    Dict,
     Optional,
     Type,
 )
 
 from django.db.models import QuerySet
 from django.http import HttpResponseRedirect
 from django.template import (
     Context,
     Template,
 )
 from django.utils.safestring import mark_safe
 from django.utils.translation import gettext_lazy
 
-from iommi.action import Action
+from iommi._web_compat import render_template
+from iommi.action import (
+    Action,
+    Actions,
+    group_actions,
+)
 from iommi.asset import Asset
 from iommi.base import (
     MISSING,
     NOT_BOUND_MESSAGE,
     items,
     keys,
     values,
@@ -36,18 +42,23 @@
     FULL_FORM_FROM_REQUEST,
     Field,
     Form,
 )
 from iommi.fragment import (
     Fragment,
 )
-from iommi.member import bind_member
+from iommi.member import (
+    bind_member,
+    bind_members,
+    refine_done_members,
+)
 from iommi.refinable import (
     Refinable,
     refinable,
+    RefinableMembers,
 )
 from iommi.shortcut import with_defaults
 from iommi.struct import Struct
 from iommi.table import (
     Cell,
     Cells,
     Column,
@@ -125,19 +136,19 @@
 
 class EditColumn(Column):
     # language=rst
     """
     The column class for `EditTable`.
     """
 
-    edit: Field = Refinable()
+    field: Field = Refinable()
 
     def on_refine_done(self):
         super(EditColumn, self).on_refine_done()
-        self.edit = None
+        self.field = None
 
     @classmethod
     @with_defaults(
         header__template='iommi/table/header.html',
         sortable=False,
         filter__is_valid_filter=lambda **_: (True, ''),
         filter__field__include=False,
@@ -175,20 +186,20 @@
             return mark_safe(f'{button.__html__()}<input style="display: none" type="checkbox" name="{path}" />')
 
         setdefaults_path(kwargs, dict(cell__value=cell__value))
         return cls(**kwargs)
 
     @classmethod
     @dispatch(
-        edit=EMPTY,
+        field=EMPTY,
     )
     def hardcoded(cls, **kwargs):
         assert (
-            'parsed_data' in kwargs['edit']
-        ), 'Specify a hardcoded value by specifying `edit__parsed_data` as a callable'
+            'parsed_data' in kwargs['field']
+        ), 'Specify a hardcoded value by specifying `field__parsed_data` as a callable'
         return cls(**kwargs)
 
 
 def edit_table__post_handler(table, request, **_):
     # 1. Validate all the fields
     table.edit_errors = defaultdict(set)
     table.create_errors = defaultdict(set)
@@ -271,56 +282,50 @@
     """
     Describe an editable table. Example:
 
     .. code-block:: python
 
         table = EditTable(
             auto__model=Album,
-            columns__name__edit__include=True,
+            columns__name__field__include=True,
         )
 
         # @test
         show_output(table)
         # @end
     """
 
     edit_errors = None
     create_errors = None
     edit_form: Form = Refinable()
     create_form: Form = Refinable()
     form_class: Type[Form] = Refinable()
     parent_form: Optional[Form] = Refinable()
+    edit_actions: Dict[str, Action] = RefinableMembers()
 
     class Meta:
         form_class = Form
         member_class = EditColumn
-        outer__tag = 'form'
-        outer__attrs__enctype = 'multipart/form-data'
-        outer__attrs__method = 'post'
         cells_class = EditCells
-        actions__submit = dict(
+        edit_actions = EMPTY
+        edit_actions__save = dict(
             call_target__attribute='primary',
             display_name=gettext_lazy('Save'),
             post_handler=edit_table__post_handler,
             template=lambda table, **_: 'iommi/blank.html' if table.parent_form is not None else None,
         )
-        actions__csrf = Action(
-            tag='div',
-            children__csrf=Fragment(
-                template=lambda **_: Template('{% csrf_token %}'),
-            ),
-            attrs__style__display='none',
-        )
-        actions__add_row = Action.button(
+        edit_actions__add_row = Action.button(
             display_name=gettext_lazy('Add row'),
             attrs__onclick='iommi_add_row(this); return false',
         )
-        actions_below = True
         edit_form = EMPTY
         create_form = EMPTY
+        container__children__text__template = 'iommi/table/edit_table_container.html'
+
+        bulk__include = True
 
         attrs = {
             'data-next-virtual-pk': '-1',
         }
 
         # language=js
         assets__edit_table_js = Asset.js(
@@ -369,39 +374,43 @@
                 '''
             )
         )
 
     def on_refine_done(self):
         super(EditTable, self).on_refine_done()
 
+        if self.bulk is None:
+            form_class = self.get_meta().form_class
+            self.bulk = form_class(_name='bulk', attrs__method='post').refine_done(parent=self)
+
         fields = Struct()
 
         for name, column in items(self.iommi_namespace.columns):
             if not isinstance(column, EditColumn):
                 continue
             if getattr(column, 'include', None) is False:
                 continue
 
-            edit_conf = column.iommi_namespace.get('edit', None)
+            edit_conf = column.iommi_namespace.get('field', None)
 
             if not edit_conf:
                 continue
-            if getattr(column.edit, 'include', None) is False:
+            if getattr(column.field, 'include', None) is False:
                 continue
 
             if isinstance(edit_conf, dict):
                 field = setdefaults_path(
                     Namespace(),
                     edit_conf,
                     model=self.model,
                     model_field_name=column.model_field_name,
                     attr=name if column.attr is MISSING else column.attr,
                 )
             else:
-                field = column.iommi_namespace.edit
+                field = column.iommi_namespace.field
 
             fields[name] = field
 
         auto = Namespace(self.auto)
 
         auto.pop('rows', None)
         if 'model' not in auto and 'rows' in auto:
@@ -426,25 +435,35 @@
                 self.edit_form,
                 fields=fields,
                 _name='edit_form',
                 auto=auto,
             )
         )
 
+        refine_done_members(
+            self,
+            name='edit_actions',
+            members_from_namespace=self.edit_actions,
+            cls=self.get_meta().action_class,
+            members_cls=Actions,
+        )
+
         declared_fields = self.edit_form.iommi_namespace.fields
         self.edit_form = self.edit_form.refine_defaults(fields=declared_fields).refine_done()
         self.create_form = self.create_form.refine_defaults(fields=declared_fields).refine_done()
 
     def on_bind(self) -> None:
         super(EditTable, self).on_bind()
+        bind_members(self, name='edit_actions')
         bind_member(self, name='edit_form')
         bind_member(self, name='create_form')
 
         # If this is a nested form register it with the parent, need
         # to do this early because is_target needs self.parent_form
+        self.parent_form = None
         if self.iommi_parent() is not None:
             self.parent_form = self.iommi_parent().iommi_evaluate_parameters().get('form', None)
             if self.parent_form is not None:
                 self.parent_form.nested_forms[self._name] = self
                 self.outer.tag = None
 
         if self.model is not None:
@@ -500,7 +519,25 @@
     def get_errors(self):
         return set()
 
     @staticmethod
     @refinable
     def preprocess_row_for_create(row, **_):
         return row
+
+    @property
+    def render_edit_actions(self):
+        assert self._is_bound, NOT_BOUND_MESSAGE
+        non_grouped_actions, grouped_actions = group_actions(self.edit_actions)
+        return render_template(
+            self.get_request(),
+            self.actions_template,
+            dict(
+                actions=self.iommi_bound_members().edit_actions,
+                non_grouped_actions=non_grouped_actions,
+                grouped_actions=grouped_actions,
+                table=self,
+            ),
+        )
+
+    def should_render_form_tag(self):
+        return self.parent_form is None
```

### Comparing `iommi-6.8.0/iommi/endpoint.py` & `iommi-7.0.0/iommi/endpoint.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/error.py` & `iommi-7.0.0/iommi/error.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/evaluate.py` & `iommi-7.0.0/iommi/evaluate.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/experimental/.DS_Store` & `iommi-7.0.0/iommi/experimental/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/form.py` & `iommi-7.0.0/iommi/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -1573,15 +1573,15 @@
 
     def own_evaluate_parameters(self):
         return dict(group=self.group, **super().own_evaluate_parameters())
 
 
 @declarative(Part, '_fields_dict', add_init_kwargs=False)
 @with_meta
-class Form(Part):
+class Form(Part, Tag):
     # language=rst
     """
     Describe a Form. Example:
 
     .. code-block:: python
 
         class MyForm(Form):
@@ -1786,14 +1786,16 @@
                 self.read_nested_form_from_instance,
                 form=self,
                 instance=self.parent_form.instance,
             )
 
         self._evaluate_parameters['instance'] = self.instance
         self.editable = evaluate_strict(self.editable, **self.iommi_evaluate_parameters())
+        if self.parent_form is not None and self.parent_form.editable is False:
+            self.editable = False
 
         self.title = evaluate_strict(self.title, **self.iommi_evaluate_parameters())
         build_and_bind_h_tag(self)
 
         # Actions have to be bound first because is_target() needs it
         bind_members(self, name='actions')
 
@@ -1817,15 +1819,15 @@
 
     @property
     def is_nested_form(self) -> bool:
         """Is this form nested in a parent form?"""
         return self.parent_form is not None
 
     @property
-    def form_tag(self) -> str:
+    def tag(self) -> str:
         if self.is_nested_form:
             return "div"
         else:
             return "form"
 
     # property for jinja2 compatibility
     @property
```

### Comparing `iommi-6.8.0/iommi/fragment.py` & `iommi-7.0.0/iommi/fragment.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/from_model.py` & `iommi-7.0.0/iommi/from_model.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/live_edit.py` & `iommi-7.0.0/iommi/live_edit.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/.DS_Store` & `iommi-7.0.0/iommi/locale/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/cs/LC_MESSAGES/django.mo` & `iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/cs/LC_MESSAGES/django.po` & `iommi-7.0.0/iommi/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/de/.DS_Store` & `iommi-7.0.0/iommi/locale/de/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/de/LC_MESSAGES/django.mo` & `iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/de/LC_MESSAGES/django.po` & `iommi-7.0.0/iommi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/sv/.DS_Store` & `iommi-7.0.0/iommi/locale/sv/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/sv/LC_MESSAGES/django.mo` & `iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/sv/LC_MESSAGES/django.po` & `iommi-7.0.0/iommi/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/uk/LC_MESSAGES/django.mo` & `iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/uk/LC_MESSAGES/django.po` & `iommi-7.0.0/iommi/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo` & `iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po` & `iommi-7.0.0/iommi/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/member.py` & `iommi-7.0.0/iommi/member.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/menu.py` & `iommi-7.0.0/iommi/menu.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/page.py` & `iommi-7.0.0/iommi/page.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/part.py` & `iommi-7.0.0/iommi/part.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/path.py` & `iommi-7.0.0/iommi/path.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/profiling.py` & `iommi-7.0.0/iommi/profiling.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/query.py` & `iommi-7.0.0/iommi/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,18 @@
         instance = instance.refine(
             Prio.shortcut,
             field__choices=kwargs.get('choices'),
         )
         return instance
 
     @classmethod
+    def checkboxes(cls, **kwargs):
+        return cls.multi_choice(**kwargs)
+
+    @classmethod
     @with_defaults(
         field__call_target__attribute='choice_queryset',
         query_operator_to_q_operator=lambda op: 'exact',
         value_to_q=choice_queryset_value_to_q,
         is_valid_filter=choice_queryset__is_valid_filter,
     )
     def choice_queryset(cls, choices: QuerySet = None, **kwargs):
```

### Comparing `iommi-6.8.0/iommi/refinable.py` & `iommi-7.0.0/iommi/refinable.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/shortcut.py` & `iommi-7.0.0/iommi/shortcut.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/sort_after.py` & `iommi-7.0.0/iommi/sort_after.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/sql_trace.py` & `iommi-7.0.0/iommi/sql_trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,15 @@
 
                     filename, lineno = filename_and_line_num_from_part(response.iommi_part)
                     sql_debug('From source:')
                     sql_debug(
                         format_clickable_filename(filename, lineno, str(response.iommi_part._name)), sql_trace=True
                     )
                     sql_debug('With Stack:')
-                sql_debug(logs[0]['stack'], sql_trace=True)
+                sql_debug(logs[-1]['stack'], sql_trace=True)
                 for x in logs[:query_cutoff]:
                     sql_debug_trace_sql(**x)
                 if len(logs) > query_cutoff:
                     sql_debug(f'... and {len(logs) - query_cutoff:d} more unique statements\n')
         queries_per_using = defaultdict(int)
         for x in request.iommi_sql_debug_log:
             queries_per_using[x['using']] += 1
```

### Comparing `iommi-6.8.0/iommi/static/.DS_Store` & `iommi-7.0.0/iommi/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/static/js/iommi.js` & `iommi-7.0.0/iommi/static/js/iommi.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -53,25 +53,14 @@
                 window.location.reload();
             } else {
                 this.historyStatePushedByUser = true; // reset to default
             }
         }
     }
 
-    warnDeprecated(text) {
-        if (this.debug) {
-            console.warn(text);
-        }
-    }
-
-    updateURL(params) {
-        this.warnDeprecated('iommi.updateURL is deprecated');
-        window.history.replaceState(null, null, `${window.location.pathname}?${params.toString()}`);
-    }
-
     /**
      * returns iommi table container or null if none found
      * @param  {Element} element filter form or any other element with data-iommi-id-of-table attribute or any element inside container
      * @return {(Element|null)} container element or null
      */
     getContainer(element) {
         if (element.hasAttribute('data-iommi-id-of-table')) {
@@ -208,16 +197,14 @@
             }
         }
     }
 
     async updateTableContainer(container, params, extra) {
         const tbodyPath = container.getAttribute('data-endpoint');
 
-        this.callDeprecatedSpinner(true, container); // deprecated, use event "iommi.loading.start" instead
-
         container.dispatchEvent(
             new CustomEvent('iommi.loading.start', {
                 bubbles: true,
                 detail: {
                     ...extra,
                     urlSearchParams: params,
                     endpoint: tbodyPath
@@ -278,15 +265,14 @@
                             urlSearchParams: params,
                             endpoint: tbodyPath
                         },
                     })
                 );
             }
         } finally {
-            this.callDeprecatedSpinner(false, container); // deprecated, use event "iommi.loading.end" instead
             container.dispatchEvent(
                 new CustomEvent('iommi.loading.end', {
                     bubbles: true,
                     detail: {
                         ...extra,
                         urlSearchParams: params,
                         endpoint: tbodyPath
@@ -371,15 +357,14 @@
                 // if you really need a file-input in the filter form, you have to add your own listener on change
             } else if (fieldType === 'text') {
                 if (e.type === 'change') {
                     // change event fire when the input loses focus. We have already
                     // populated the form on the input event so ignore it
                     return;
                 }
-                SELF.callDeprecatedSpinner(true, container); // deprecated, also it doesn't make sense to start spinner here imo
                 // delay ajax request for free text
                 debouncedPopulate(form, e.target);
             } else {
                 // select2 elements have hidden inputs when they update GUI should respond immediately
                 // same goes for checkboxes
                 SELF.queryPopulate(form);
             }
@@ -420,14 +405,15 @@
             },
 
             getAjaxTbodyUrl: function(params, endpoint) {
                 return window.iommi.getDefaultAjaxUrl(params, endpoint);
             }
         };
     }
+
     getDefaultAjaxUrl(params, endpoint) {
         return `?${params.toString()}&${endpoint}`;
     }
 
     /**
      * simple live event listener (similar to jquery.on)
      */
@@ -485,25 +471,16 @@
                 let url = new URL(window.location.href);
                 return window.iommi.updateTableContainer(container, url.searchParams, {
                     isReload: true
                 });
             },
         };
     }
-
-    // in case someone has overridden iommi_show_spinner
-    callDeprecatedSpinner(isLoading, container) {
-        if (!iommi_show_spinner.iommiOriginal) {
-            this.warnDeprecated('iommi_show_spinner is deprecated, use events "iommi.loading.start" and "iommi.loading.end" instead');
-            iommi_show_spinner(isLoading, container);
-        }
-    }
 }
 
-
 class IommiSelect2 {
     constructor() {
         const SELF = this;
         document.addEventListener('iommi.element.populated', (event) => {
             SELF.initAll(event.target);
         });
     }
@@ -603,56 +580,8 @@
     window.iommi.onPopState(event);
 });
 
 document.addEventListener('readystatechange', () => {
     if (document.readyState === 'complete') {
         window.iommi.select2.onCompleteReadyState();
     }
-});
-
-
-// deprecated functions - for backward compatibility only
-
-function iommi_update_URL(params) {
-    window.iommi.warnDeprecated('iommi_update_URL is deprecated');
-    window.history.replaceState(null, null, `${window.location.pathname}?${params.toString()}`);
-}
-
-function iommi_debounce(func, wait) {
-    window.iommi.warnDeprecated('iommi_debounce is deprecated, use iommi.debounce instead');
-    return window.iommi.debounce(func, wait);
-}
-
-async function iommi_validate_form(params, form) {
-    window.iommi.warnDeprecated('iommi_validate_form is deprecated, use iommi.validateForm instead');
-    return window.iommi.validateForm(params, form);
-}
-
-async function iommi_query_populate(form) {
-    window.iommi.warnDeprecated('iommi_query_populate is deprecated, use iommi.queryPopulate instead');
-    return window.iommi.queryPopulate(form);
-}
-
-function iommi_has_same_data(prevData, newData) {
-    window.iommi.warnDeprecated('iommi_has_same_data is deprecated, use iommi.hasSameData instead');
-    return window.iommi.hasSameData(prevData, newData);
-}
-
-function iommi_enhance_form(form) {
-    window.iommi.warnDeprecated('iommi_enhance_form is deprecated, use iommi.enhanceFilterForm instead');
-    return window.iommi.enhanceFilterForm(form);
-}
-
-function iommi_show_spinner(isLoading, container) {
-    window.iommi.warnDeprecated('iommi_show_spinner is deprecated, use events "iommi.loading.start" and "iommi.loading.end" instead');
-}
-iommi_show_spinner.iommiOriginal = true;
-
-function iommi_init_all_select2() {
-    window.iommi.warnDeprecated('iommi_init_all_select2 is deprecated, use iommi.select2.initAll instead');
-    return window.iommi.select2.initAll();
-}
-
-function iommi_init_select2(elem) {
-    window.iommi.warnDeprecated('iommi_init_select2 is deprecated, use iommi.select2.initOne instead');
-    return window.iommi.select2.initOne(elem);
-}
+});
```

### Comparing `iommi-6.8.0/iommi/struct.py` & `iommi-7.0.0/iommi/struct.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style.py` & `iommi-7.0.0/iommi/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from iommi.declarative.namespace import (
     EMPTY,
     Namespace,
 )
 from iommi.refinable import RefinableObject
 from iommi.shortcut import get_shortcuts_by_name
 
-DEFAULT_STYLE = 'bootstrap'
+DEFAULT_STYLE = 'bootstrap5'
 
 
 def get_style_object(obj: Any) -> 'Style':
     return get_global_style(obj.iommi_style)
 
 
 def _style_name_for_class(cls):
@@ -208,14 +208,16 @@
     validate. By default it will validate all registered styles. This
     parameter is primarily used by tests.
     """
     if default_classes is None:
         from iommi import (
             Action,
             Column,
+            EditColumn,
+            EditTable,
             Field,
             Filter,
             Form,
             Menu,
             MenuItem,
             Query,
             Table,
@@ -231,31 +233,33 @@
             get_debug_menu,
         )
         from iommi.table import Paginator
 
         default_classes = [
             Action,
             Actions,
+            Admin,
             Column,
-            get_debug_menu().__class__,
+            Container,
+            EditColumn,
+            EditTable,
             Errors,
             Field,
+            FieldGroup,
+            Filter,
             Form,
+            Header,
+            LiveEditPage,
             Menu,
             MenuBase,
             MenuItem,
             Paginator,
             Query,
             Table,
-            Filter,
-            Admin,
-            Container,
-            Header,
-            LiveEditPage,
-            FieldGroup,
+            get_debug_menu().__class__,
         ]
     if additional_classes is None:
         additional_classes = []
 
     classes = default_classes + additional_classes
 
     if styles is None:
```

### Comparing `iommi-6.8.0/iommi/style_base.py` & `iommi-7.0.0/iommi/style_base.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_bootstrap.py` & `iommi-7.0.0/iommi/style_bootstrap.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_bootstrap5.py` & `iommi-7.0.0/iommi/style_bootstrap5.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_bootstrap_docs.py` & `iommi-7.0.0/iommi/style_bootstrap_docs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from iommi import (
     Asset,
     Style,
 )
-from iommi.style_bootstrap import bootstrap
+from iommi.style_bootstrap5 import bootstrap5
 
 bootstrap_docs = Style(
-    bootstrap,
+    bootstrap5,
     root__assets__doc_style=Asset.css(attrs__href='https://docs.iommi.rocks/en/latest/_static/iframe_custom.css'),
     root__assets__iommi_js=Asset.js(attrs=dict(src='https://docs.iommi.rocks//en/latest/_static/iommi.js')),
     internal=True,
     Container=dict(
         attrs__class={
             'container': False,
             'mt-5': False,
```

### Comparing `iommi-6.8.0/iommi/style_bootstrap_icons.py` & `iommi-7.0.0/iommi/style_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_bulma.py` & `iommi-7.0.0/iommi/style_bulma.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_django_admin.py` & `iommi-7.0.0/iommi/style_django_admin.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_font_awesome_4.py` & `iommi-7.0.0/iommi/style_font_awesome_4.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_foundation.py` & `iommi-7.0.0/iommi/style_foundation.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_semantic_ui.py` & `iommi-7.0.0/iommi/style_semantic_ui.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_test_base.py` & `iommi-7.0.0/iommi/style_test_base.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/style_uikit.py` & `iommi-7.0.0/iommi/style_uikit.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/synthetic_traceback.py` & `iommi-7.0.0/iommi/synthetic_traceback.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/table.py` & `iommi-7.0.0/iommi/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,14 +828,18 @@
                 bulk__model=kwargs.get('model'),
                 filter__model=kwargs.get('model'),
             ),
         )
         return cls.choice(**kwargs)
 
     @classmethod
+    def checkboxes(cls, **kwargs):
+        return cls.multi_choice(**kwargs)
+
+    @classmethod
     @with_defaults(
         bulk__call_target__attribute='text',
         filter__call_target__attribute='text',
     )
     def text(cls, **kwargs):
         # language=rst
         """
@@ -2160,18 +2164,15 @@
 
     def _bind_bulk_form(self):
         if self.bulk is None:
             return
 
         bind_member(self, name='bulk')
         if self.bulk is not None:
-            if self.bulk.actions:
-                self._bound_members.bulk = self.bulk
-            else:
-                self.bulk = None
+            self._bound_members.bulk = self.bulk
 
     # property for jinja2 compatibility
     @property
     def render_actions(self):
         assert self._is_bound, NOT_BOUND_MESSAGE
         non_grouped_actions, grouped_actions = group_actions(self.actions)
         return render_template(
@@ -2395,14 +2396,17 @@
 
         For use in post_handlers. Only valid when rows was a queryset.
         """
         assert isinstance(self.initial_rows, QuerySet), "bulk_queryset can only be used on querysets"
 
         return self.selection(prefix=prefix).filter(**self.bulk_filter).exclude(**self.bulk_exclude)
 
+    def should_render_form_tag(self):
+        return bool(self.bulk)
+
     @dispatch(
         render=render_template,
     )
     def __html__(self, *, template=None, render=None):
         assert self._is_bound, NOT_BOUND_MESSAGE
 
         request = self.get_request()
```

### Comparing `iommi-6.8.0/iommi/templates/.DS_Store` & `iommi-7.0.0/iommi/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/.DS_Store` & `iommi-7.0.0/iommi/templates/iommi/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/base.html` & `iommi-7.0.0/iommi/templates/iommi/base.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/form/.DS_Store` & `iommi-7.0.0/iommi/templates/iommi/form/.DS_Store`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/form/actions.html` & `iommi-7.0.0/iommi/templates/iommi/form/actions.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/form/choice_select2.html` & `iommi-7.0.0/iommi/templates/iommi/form/choice_select2.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/query/advanced.html` & `iommi-7.0.0/iommi/templates/iommi/query/advanced.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/query/form.html` & `iommi-7.0.0/iommi/templates/iommi/query/form.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/query/form_toggle_script.html` & `iommi-7.0.0/iommi/templates/iommi/query/form_toggle_script.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/table/bootstrap/paginator.html` & `iommi-7.0.0/iommi/templates/iommi/table/bootstrap/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/table/bulma/paginator.html` & `iommi-7.0.0/iommi/templates/iommi/table/bulma/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/table/js_select_all.html` & `iommi-7.0.0/iommi/templates/iommi/table/js_select_all.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/table/paginator.html` & `iommi-7.0.0/iommi/templates/iommi/table/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/table/semantic_ui/paginator.html` & `iommi-7.0.0/iommi/templates/iommi/table/semantic_ui/paginator.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/templates/iommi/table/table_tag.html` & `iommi-7.0.0/iommi/templates/iommi/table/table_tag.html`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi/traversable.py` & `iommi-7.0.0/iommi/traversable.py`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/iommi.egg-info/PKG-INFO` & `iommi-7.0.0/iommi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iommi
-Version: 6.8.0
+Version: 7.0.0
 Summary: iommi is a high level framework built on django
 Home-page: https://github.com/iommirocks/iommi
 Author: Anders Hovmöller
 Author-email: boxed@killingar.net
 License: BSD
 Keywords: iommi
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iommi-6.8.0/iommi.egg-info/SOURCES.txt` & `iommi-7.0.0/iommi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 iommi/style_bootstrap.py
 iommi/style_bootstrap5.py
 iommi/style_bootstrap_docs.py
 iommi/style_bootstrap_icons.py
 iommi/style_bulma.py
 iommi/style_django_admin.py
 iommi/style_font_awesome_4.py
+iommi/style_font_awesome_6.py
 iommi/style_foundation.py
 iommi/style_semantic_ui.py
 iommi/style_test_base.py
 iommi/style_uikit.py
 iommi/style_water.py
 iommi/synthetic_traceback.py
 iommi/table.py
@@ -107,14 +108,15 @@
 iommi/templates/iommi/form/semantic_ui/checkboxes.html
 iommi/templates/iommi/form/semantic_ui/radio.html
 iommi/templates/iommi/form/semantic_ui/row_checkbox.html
 iommi/templates/iommi/form/uikit/row_checkbox.html
 iommi/templates/iommi/query/advanced.html
 iommi/templates/iommi/query/form.html
 iommi/templates/iommi/query/form_toggle_script.html
+iommi/templates/iommi/table/edit_table_container.html
 iommi/templates/iommi/table/header.html
 iommi/templates/iommi/table/js_select_all.html
 iommi/templates/iommi/table/paginator.html
 iommi/templates/iommi/table/row_group.html
 iommi/templates/iommi/table/select_column_header.html
 iommi/templates/iommi/table/table.html
 iommi/templates/iommi/table/table_container.html
```

### Comparing `iommi-6.8.0/pyproject.toml` & `iommi-7.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/setup.cfg` & `iommi-7.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `iommi-6.8.0/setup.py` & `iommi-7.0.0/setup.py`

 * *Files identical despite different names*

