# Comparing `tmp/wagtail_fedit-1.4.8b0.tar.gz` & `tmp/wagtail_fedit-1.4.8rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.8b0.tar", last modified: Mon Apr 15 18:07:39 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.8rc0.tar", last modified: Mon Apr 15 18:10:23 2024, max compression
```

## Comparing `wagtail_fedit-1.4.8b0.tar` & `wagtail_fedit-1.4.8rc0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.799148 wagtail_fedit-1.4.8b0/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/MANIFEST.in
--rw-rw-rw-   0        0        0    12405 2024-04-15 18:07:39.799148 wagtail_fedit-1.4.8b0/PKG-INFO
--rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.4.8b0/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/pyproject.toml
--rw-rw-rw-   0        0        0     1188 2024-04-15 18:07:39.801913 wagtail_fedit-1.4.8b0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.623913 wagtail_fedit-1.4.8b0/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.698553 wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     4180 2024-04-15 18:04:16.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     4227 2024-04-15 18:03:25.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     7523 2024-04-13 11:18:27.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.703113 wagtail_fedit-1.4.8b0/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.578135 wagtail_fedit-1.4.8b0/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.579137 wagtail_fedit-1.4.8b0/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.705115 wagtail_fedit-1.4.8b0/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.707113 wagtail_fedit-1.4.8b0/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.709115 wagtail_fedit-1.4.8b0/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.580042 wagtail_fedit-1.4.8b0/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.589211 wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.713385 wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.714398 wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    16161 2024-04-15 15:58:30.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.590656 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.593678 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.717044 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.720796 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      386 2024-04-13 11:13:58.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.727819 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.735456 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.737464 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.739453 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.752713 wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.755730 wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     9097 2024-04-14 13:32:19.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     6747 2024-04-15 18:06:17.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.757700 wagtail_fedit-1.4.8b0/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.761790 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.767819 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.777473 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4314 2024-04-14 13:07:00.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.783747 wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.787670 wagtail_fedit-1.4.8b0/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6271 2024-04-15 17:21:37.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.797671 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:07:39.652811 wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12405 2024-04-15 18:07:39.000000 wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4043 2024-04-15 18:07:39.000000 wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:07:39.000000 wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-15 18:07:39.000000 wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 18:07:39.000000 wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.048943 wagtail_fedit-1.4.8rc0/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12406 2024-04-15 18:10:23.048943 wagtail_fedit-1.4.8rc0/PKG-INFO
+-rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.4.8rc0/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/pyproject.toml
+-rw-rw-rw-   0        0        0     1188 2024-04-15 18:10:23.052090 wagtail_fedit-1.4.8rc0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.886956 wagtail_fedit-1.4.8rc0/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.920758 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     4180 2024-04-15 18:04:16.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     4232 2024-04-15 18:09:49.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     7523 2024-04-13 11:18:27.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.927819 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.849726 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.849726 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.931196 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.932230 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.934576 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.852563 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.853134 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.939423 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.940425 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    16161 2024-04-15 15:58:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.855148 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.858146 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.943204 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.949040 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      386 2024-04-13 11:13:58.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.956834 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.966800 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.970160 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.973407 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.977227 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.982182 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9097 2024-04-14 13:32:19.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6747 2024-04-15 18:06:17.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.983960 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.989005 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.998587 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.014930 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4314 2024-04-14 13:07:00.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.022632 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.029922 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6271 2024-04-15 17:21:37.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.046894 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.913412 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12406 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4043 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.8b0/LICENSE` & `wagtail_fedit-1.4.8rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/PKG-INFO` & `wagtail_fedit-1.4.8rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.8b0
+Version: 1.4.8rc0
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.8b0 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.8rc0 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.4.8b0/README.md` & `wagtail_fedit-1.4.8rc0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/setup.cfg` & `wagtail_fedit-1.4.8rc0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 3862 300d 0a64 6573 6372 6970 7469 6f6e  8b0..description
+00000030: 3863 300d 0a64 6573 6372 6970 7469 6f6e  8c0..description
 00000040: 203d 2046 726f 6e74 656e 6420 6564 6974   = Frontend edit
 00000050: 696e 6720 666f 7220 796f 7572 2057 6167  ing for your Wag
 00000060: 7461 696c 2073 6974 650d 0a6c 6f6e 675f  tail site..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
```

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                     "block_label": str(self.block.block.label),
                 },
                 content_changed=True,
                 **extra_log_kwargs,
             )
 
     @classmethod
-    def render_from_kwargs(context, **kwargs):
+    def render_from_kwargs(cls, context, **kwargs):
         if "block" not in kwargs:
             raise AdapterError("Block is required")
         
         block = kwargs.pop("block")
         if not hasattr(block, "render"):
             raise AdapterError("Invalid block type, missing render method")
```

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/models.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.4.8b0
+Version: 1.4.8rc0
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.8b0 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.8rc0 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.4.8b0/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

