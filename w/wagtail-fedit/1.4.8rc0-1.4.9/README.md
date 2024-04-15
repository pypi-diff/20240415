# Comparing `tmp/wagtail_fedit-1.4.8rc0.tar.gz` & `tmp/wagtail_fedit-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.8rc0.tar", last modified: Mon Apr 15 18:10:23 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.9.tar", last modified: Mon Apr 15 19:34:13 2024, max compression
```

## Comparing `wagtail_fedit-1.4.8rc0.tar` & `wagtail_fedit-1.4.9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.048943 wagtail_fedit-1.4.8rc0/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/MANIFEST.in
--rw-rw-rw-   0        0        0    12406 2024-04-15 18:10:23.048943 wagtail_fedit-1.4.8rc0/PKG-INFO
--rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.4.8rc0/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/pyproject.toml
--rw-rw-rw-   0        0        0     1188 2024-04-15 18:10:23.052090 wagtail_fedit-1.4.8rc0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.886956 wagtail_fedit-1.4.8rc0/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.920758 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     4180 2024-04-15 18:04:16.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     4232 2024-04-15 18:09:49.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     7523 2024-04-13 11:18:27.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.927819 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.849726 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.849726 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.931196 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.932230 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.934576 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.852563 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.853134 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.939423 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.940425 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    16161 2024-04-15 15:58:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.855148 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.858146 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.943204 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.949040 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      386 2024-04-13 11:13:58.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.956834 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.966800 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.970160 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.973407 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.977227 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.982182 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     9097 2024-04-14 13:32:19.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     6747 2024-04-15 18:06:17.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.983960 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.989005 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.998587 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.014930 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4314 2024-04-14 13:07:00.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.022632 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.029922 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     6271 2024-04-15 17:21:37.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:23.046894 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:10:22.913412 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    12406 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4043 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 18:10:22.000000 wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.444926 wagtail_fedit-1.4.9/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    12403 2024-04-15 19:34:13.444926 wagtail_fedit-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.4.9/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-04-15 19:34:13.458502 wagtail_fedit-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.289628 wagtail_fedit-1.4.9/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.9/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.333120 wagtail_fedit-1.4.9/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      313 2024-04-15 18:06:14.000000 wagtail_fedit-1.4.9/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     4259 2024-04-15 18:49:04.000000 wagtail_fedit-1.4.9/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     4335 2024-04-15 18:50:49.000000 wagtail_fedit-1.4.9/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     7692 2024-04-15 18:52:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.4.9/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.9/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.336123 wagtail_fedit-1.4.9/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.9/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.9/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.4.9/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.258024 wagtail_fedit-1.4.9/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.258024 wagtail_fedit-1.4.9/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.338111 wagtail_fedit-1.4.9/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.339618 wagtail_fedit-1.4.9/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.9/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.340626 wagtail_fedit-1.4.9/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.9/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.9/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.261574 wagtail_fedit-1.4.9/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.262573 wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.345008 wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4333 2024-04-15 18:17:44.000000 wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.372181 wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    16149 2024-04-15 19:27:25.000000 wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.263594 wagtail_fedit-1.4.9/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.267101 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.373138 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.378304 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      420 2024-04-15 18:48:24.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.384478 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.389488 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.393062 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.396550 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.399670 wagtail_fedit-1.4.9/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.9/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.403759 wagtail_fedit-1.4.9/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.9/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9291 2024-04-15 18:55:47.000000 wagtail_fedit-1.4.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6828 2024-04-15 18:36:41.000000 wagtail_fedit-1.4.9/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.404759 wagtail_fedit-1.4.9/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.408111 wagtail_fedit-1.4.9/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.414630 wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.424268 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     7837 2024-04-15 19:13:02.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.429436 wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.4.9/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.4.9/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.4.9/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.434574 wagtail_fedit-1.4.9/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.4.9/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6271 2024-04-15 17:21:37.000000 wagtail_fedit-1.4.9/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.9/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.9/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.443921 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:34:13.326545 wagtail_fedit-1.4.9/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12403 2024-04-15 19:34:13.000000 wagtail_fedit-1.4.9/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4043 2024-04-15 19:34:13.000000 wagtail_fedit-1.4.9/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 19:34:13.000000 wagtail_fedit-1.4.9/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-15 19:34:13.000000 wagtail_fedit-1.4.9/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 19:34:13.000000 wagtail_fedit-1.4.9/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.8rc0/LICENSE` & `wagtail_fedit-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/PKG-INFO` & `wagtail_fedit-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.8rc0
+Version: 1.4.9
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.8rc0 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.9 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.4.8rc0/README.md` & `wagtail_fedit-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/setup.cfg` & `wagtail_fedit-1.4.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 3863 300d 0a64 6573 6372 6970 7469 6f6e  8c0..description
-00000040: 203d 2046 726f 6e74 656e 6420 6564 6974   = Frontend edit
-00000050: 696e 6720 666f 7220 796f 7572 2057 6167  ing for your Wag
-00000060: 7461 696c 2073 6974 650d 0a6c 6f6e 675f  tail site..long_
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-000000b0: 6578 742f 6d61 726b 646f 776e 0d0a 6175  ext/markdown..au
-000000c0: 7468 6f72 203d 204e 6967 656c 0d0a 6175  thor = Nigel..au
-000000d0: 7468 6f72 5f65 6d61 696c 203d 206e 6967  thor_email = nig
-000000e0: 656c 4067 6f6f 6461 6476 6963 652e 6974  el@goodadvice.it
-000000f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000100: 6769 7468 7562 2e63 6f6d 2f4e 6967 656c  github.com/Nigel
-00000110: 3233 3932 2f77 6167 7461 696c 5f66 6564  2392/wagtail_fed
-00000120: 6974 0d0a 6c69 6365 6e73 6520 3d20 4750  it..license = GP
-00000130: 4c2d 322e 302d 6f6e 6c79 0d0a 636c 6173  L-2.0-only..clas
-00000140: 7369 6669 6572 7320 3d20 0d0a 0945 6e76  sifiers = ...Env
-00000150: 6972 6f6e 6d65 6e74 203a 3a20 5765 6220  ironment :: Web 
-00000160: 456e 7669 726f 6e6d 656e 740d 0a09 4672  Environment...Fr
-00000170: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
-00000180: 6f0d 0a09 4672 616d 6577 6f72 6b20 3a3a  o...Framework ::
-00000190: 2044 6a61 6e67 6f20 3a3a 2034 2e32 0d0a   Django :: 4.2..
-000001a0: 0946 7261 6d65 776f 726b 203a 3a20 5761  .Framework :: Wa
-000001b0: 6774 6169 6c0d 0a09 4672 616d 6577 6f72  gtail...Framewor
-000001c0: 6b20 3a3a 2057 6167 7461 696c 203a 3a20  k :: Wagtail :: 
-000001d0: 350d 0a09 4672 616d 6577 6f72 6b20 3a3a  5...Framework ::
-000001e0: 2057 6167 7461 696c 203a 3a20 360d 0a09   Wagtail :: 6...
-000001f0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-00000200: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
-00000210: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000220: 2041 7070 726f 7665 6420 3a3a 2047 4e55   Approved :: GNU
-00000230: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00000240: 4c69 6365 6e73 6520 7632 206f 7220 6c61  License v2 or la
-00000250: 7465 7220 2847 504c 7632 2b29 0d0a 094f  ter (GPLv2+)...O
-00000260: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000270: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000280: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
-00000290: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002a0: 6f6e 0d0a 0950 726f 6772 616d 6d69 6e67  on...Programming
-000002b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002c0: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
-000002d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
-000002f0: 3a20 4f6e 6c79 0d0a 0950 726f 6772 616d  : Only...Program
-00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000310: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
-00000320: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000330: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000340: 3a3a 2033 2e39 0d0a 0950 726f 6772 616d  :: 3.9...Program
-00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000360: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
-00000370: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000380: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000390: 203a 3a20 332e 3131 0d0a 0954 6f70 6963   :: 3.11...Topic
-000003a0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-000003b0: 5757 572f 4854 5450 0d0a 0954 6f70 6963  WWW/HTTP...Topic
-000003c0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
-000003d0: 5757 572f 4854 5450 203a 3a20 4479 6e61  WWW/HTTP :: Dyna
-000003e0: 6d69 6320 436f 6e74 656e 740d 0a0d 0a5b  mic Content....[
-000003f0: 6f70 7469 6f6e 735d 0d0a 696e 636c 7564  options]..includ
-00000400: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-00000410: 2074 7275 650d 0a70 6163 6b61 6765 7320   true..packages 
-00000420: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-00000430: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
-00000440: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000450: 6573 203d 200d 0a09 446a 616e 676f 203e  es = ...Django >
-00000460: 3d20 342e 320d 0a09 5761 6774 6169 6c20  = 4.2...Wagtail 
-00000470: 3e3d 2035 2e32 0d0a 0d0a 5b65 6767 5f69  >= 5.2....[egg_i
-00000480: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000490: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000004a0: 0d0a 0d0a                                ....
+00000030: 390d 0a64 6573 6372 6970 7469 6f6e 203d  9..description =
+00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
+00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
+00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
+00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+000000b0: 742f 6d61 726b 646f 776e 0d0a 6175 7468  t/markdown..auth
+000000c0: 6f72 203d 204e 6967 656c 0d0a 6175 7468  or = Nigel..auth
+000000d0: 6f72 5f65 6d61 696c 203d 206e 6967 656c  or_email = nigel
+000000e0: 4067 6f6f 6461 6476 6963 652e 6974 0d0a  @goodadvice.it..
+000000f0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
+00000100: 7468 7562 2e63 6f6d 2f4e 6967 656c 3233  thub.com/Nigel23
+00000110: 3932 2f77 6167 7461 696c 5f66 6564 6974  92/wagtail_fedit
+00000120: 0d0a 6c69 6365 6e73 6520 3d20 4750 4c2d  ..license = GPL-
+00000130: 322e 302d 6f6e 6c79 0d0a 636c 6173 7369  2.0-only..classi
+00000140: 6669 6572 7320 3d20 0d0a 0945 6e76 6972  fiers = ...Envir
+00000150: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
+00000160: 7669 726f 6e6d 656e 740d 0a09 4672 616d  vironment...Fram
+00000170: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f0d  ework :: Django.
+00000180: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
+00000190: 6a61 6e67 6f20 3a3a 2034 2e32 0d0a 0946  jango :: 4.2...F
+000001a0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
+000001b0: 6169 6c0d 0a09 4672 616d 6577 6f72 6b20  ail...Framework 
+000001c0: 3a3a 2057 6167 7461 696c 203a 3a20 350d  :: Wagtail :: 5.
+000001d0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2057  ..Framework :: W
+000001e0: 6167 7461 696c 203a 3a20 360d 0a09 496e  agtail :: 6...In
+000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000200: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
+00000210: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000220: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
+00000230: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
+00000240: 6365 6e73 6520 7632 206f 7220 6c61 7465  cense v2 or late
+00000250: 7220 2847 504c 7632 2b29 0d0a 094f 7065  r (GPLv2+)...Ope
+00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000280: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002c0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+000002f0: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000310: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
+00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000340: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000360: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000390: 3a20 332e 3131 0d0a 0954 6f70 6963 203a  : 3.11...Topic :
+000003a0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+000003b0: 572f 4854 5450 0d0a 0954 6f70 6963 203a  W/HTTP...Topic :
+000003c0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
+000003d0: 572f 4854 5450 203a 3a20 4479 6e61 6d69  W/HTTP :: Dynami
+000003e0: 6320 436f 6e74 656e 740d 0a0d 0a5b 6f70  c Content....[op
+000003f0: 7469 6f6e 735d 0d0a 696e 636c 7564 655f  tions]..include_
+00000400: 7061 636b 6167 655f 6461 7461 203d 2074  package_data = t
+00000410: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
+00000420: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000430: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
+00000440: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000450: 203d 200d 0a09 446a 616e 676f 203e 3d20   = ...Django >= 
+00000460: 342e 320d 0a09 5761 6774 6169 6c20 3e3d  4.2...Wagtail >=
+00000470: 2035 2e32 0d0a 0d0a 5b65 6767 5f69 6e66   5.2....[egg_inf
+00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+000004a0: 0d0a                                     ..
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.4.9/wagtail_fedit/adapters/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,17 @@
         return self.object.__class__
     
     def check_permissions(self):
         if not self.request.user.is_authenticated:
             return False
         return True
     
+    def get_element_id(self) -> str:
+        raise NotImplementedError
+    
     def get_form(self) -> "forms.Form":
         raise NotImplementedError
 
     def form_valid(self, form: "forms.Form"):
         pass
     
     def form_invalid(self, form: "forms.Form"):
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.4.9/wagtail_fedit/adapters/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
             model_string = getattr(self.object, "title", str(self.object))
 
         return _("Edit block %(block_label)s for %(model_name)s %(model_string)s") % {
             "block_label": self.block.block.label,
             "model_name": self.model._meta.verbose_name,
             "model_string": model_string,
         }
+    
+    def get_element_id(self) -> str:
+        return f"block-{self.kwargs['block_id']}-section"
 
     def get_form(self):
 
         self.form_class = block_forms.get_block_form_class(self.block.block)
 
         if self.request.method == "POST":
             form = self.form_class(self.request.POST, block=self.block, parent_instance=self.object, request=self.request)
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.4.9/wagtail_fedit/adapters/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,19 @@
                 "text": mark_safe(_("You must publish the related object of type %(type)s (%(model)s) to make any changes visible.") % {
                     "type": self.original_object._meta.verbose_name,
                     "model": get_model_string(self.original_object, publish_url=True, request=self.request),
                 })
             }
 
         return super().get_help_text()
-        
+          
+    def get_element_id(self) -> str:
+        m = self.model
+        return f"field-{self.field_name}-{m._meta.app_label}-{m._meta.model_name}-{self.object.pk}"
+  
     def get_form(self):
         if self.request.method == "POST":
             form = self.form_class(self.request.POST, request=self.request, instance=self.object)
         else:
             form = self.form_class(request=self.request, instance=self.object)
         return form
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.4.9/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.9/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.9/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.9/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.4.9/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.4.9/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/models.py` & `wagtail_fedit-1.4.9/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,31 @@
     padding: 0;
 }
 
 .wagtail-fedit-buttons {
     display: flex;
 }
 
-.wagtail-fedit-field-wrapper,
-.wagtail-fedit-block-wrapper {
+.wagtail-fedit-adapter-wrapper {
     position: relative;
 }
-.wagtail-fedit-field-wrapper:has(> .wagtail-fedit-buttons button:hover)::after,
-.wagtail-fedit-block-wrapper:has(> .wagtail-fedit-buttons button:hover)::after {
+.wagtail-fedit-adapter-wrapper:has(> .wagtail-fedit-buttons button:hover)::after {
     content: '';
     display: block;
     position: absolute;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     background-color: rgba(0, 0, 0, 0.05);
     outline: 2px solid #333333;
     pointer-events: none;
     z-index: 300;
 }
-.wagtail-fedit-field-wrapper:has(.wagtail-fedit-block-wrapper) > .wagtail-fedit-buttons {
+.wagtail-fedit-adapter-wrapper.wagtail-fedit-field:has(.wagtail-fedit-adapter) > .wagtail-fedit-buttons {
     right: 30px;
 }
 .wagtail-fedit-buttons {
     display: flex;
     gap: 0.5em;
     border-radius: 0.5em;
     position: absolute;
@@ -46,15 +44,15 @@
     left: unset;
     right: unset;
 }
 
 /* .wagtail-fedit-field-wrapper > .wagtail-fedit-buttons { */
     /* position: relative; */
 /* } */
-.wagtail-fedit-field-wrapper > .wagtail-fedit-buttons button {
+.wagtail-fedit-adapter-wrapper > .wagtail-fedit-buttons button {
     display: inline-block;
     vertical-align: middle;
 }
 .wagtail-fedit-buttons button {
     border: none;
     background-color: white;
     padding: 0.1em;
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.9/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -194,15 +194,14 @@
                             }
 
                             const cancelButton = this.iframe.document.querySelector(".wagtail-fedit-cancel-button");
                             cancelButton.addEventListener("click", this.closeModal.bind(this));
                             return;
                         }
                         this.setWrapperHtml(response.html);
-                        this.initNewEditors();
                         this.closeModal();
 
                         const event = new CustomEvent("wagtail-fedit:change", {
                             detail: {
                                 element: this.wrapperElement,
                             }
                         });
@@ -262,14 +261,15 @@
             newBlock.innerHTML = html;
             const blockWrapper = newBlock.firstElementChild;
             blockWrapper.classList.add("wagtail-fedit-initialized");
             this.wrapperElement.parentNode.insertBefore(blockWrapper, this.wrapperElement);
             this.wrapperElement.parentNode.removeChild(this.wrapperElement);
             blockWrapper.style.opacity = 0;
             this.wrapperElement = blockWrapper;
+            this.initNewEditors();
             this.init();
 
             const anim = blockWrapper.animate([{
                 opacity: 0
             }, {
                 opacity: 1
             }, ], {
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.9/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.9/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,315 +1,277 @@
 magic:    0xa70d0d0a
-moddate:  0xe1da1b66 (Sun Apr 14 13:32:17 2024 UTC)
-files sz: 6514
+moddate:  0xb9731d66 (Mon Apr 15 18:36:41 2024 UTC)
+files sz: 6828
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a056d065a060100640064036c076d085a080100640064046c096d0a5a
-      0a6d0b5a0b0100640064056c096d0c5a0c0100640064066c0d6d0e5a0e01
-      00640064076c0f6d105a100100640064086c116d125a120100640064096c
-      136d145a1401006400640a6c156d165a1601006400640b6c176d185a1801
-      006400640c6c196d1a5a1a01006400640d6c1b6d1c5a1c01006400640e6c
-      1d5a1d640f64106c1e6d1f5a1f6d205a200100640f64116c216d225a226d
-      235a236d245a240100640f64126c256d265a266d275a270100640f64136c
-      1a6d285a280100020065036a290000000000000000a6000000ab00000000
-      00000000005a2a64145a2b64155a2c020047006416840064176504a60300
-      00ab0300000000000000005a2d652aa02e00000000000000000000000000
-      000000000000006418ac19a6010000ab010000000000000000641a650a64
-      1b650b6604641c8404a6000000ab0000000000000000005a2f641d651064
-      1e6524641f6530642065316608642184045a326425641a650a6422653365
-      311900000000000000000064236533653119000000000000000000642065
-      306608642484055a34640e5300
+      055a050100640064036c066d075a070100640064046c086d095a096d0a5a
+      0a0100640064056c086d0b5a0b0100640064066c0c6d0d5a0d0100640064
+      076c0e6d0f5a0f0100640064086c106d115a110100640064096c126d135a
+      1301006400640a6c145a14640b640c6c156d165a160100640b640d6c176d
+      185a186d195a196d1a5a1a6d1b5a1b0100640b640e6c1c6d1d5a1d010064
+      0b640f6c136d1e5a1e0100020065036a1f0000000000000000a6000000ab
+      0000000000000000005a2064105a2164115a220200470064128400641365
+      04a6030000ab0300000000000000005a236520a024000000000000000000
+      00000000000000000000006414ac15a6010000ab01000000000000000064
+      1665096417650a660464188404a6000000ab0000000000000000005a2564
+      19650d641a651a641b6526641c65276608641d84045a2864216416650964
+      1e6529652719000000000000000000641f65296527190000000000000000
+      00641c65266608642084055a2a640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Type',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Type)
                 10 STORE_NAME               1 (Type)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('library', 'Node', 'NodeList', 'TemplateSyntaxError'))
+                16 LOAD_CONST               2 (('library', 'Node', 'TemplateSyntaxError'))
                 18 IMPORT_NAME              2 (django.template)
                 20 IMPORT_FROM              3 (library)
                 22 STORE_NAME               3 (library)
                 24 IMPORT_FROM              4 (Node)
                 26 STORE_NAME               4 (Node)
-                28 IMPORT_FROM              5 (NodeList)
-                30 STORE_NAME               5 (NodeList)
-                32 IMPORT_FROM              6 (TemplateSyntaxError)
-                34 STORE_NAME               6 (TemplateSyntaxError)
-                36 POP_TOP
-   
-     3          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('render_to_string',))
-                42 IMPORT_NAME              7 (django.template.loader)
-                44 IMPORT_FROM              8 (render_to_string)
-                46 STORE_NAME               8 (render_to_string)
-                48 POP_TOP
-   
-     4          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('Parser', 'Token'))
-                54 IMPORT_NAME              9 (django.template.base)
-                56 IMPORT_FROM             10 (Parser)
-                58 STORE_NAME              10 (Parser)
-                60 IMPORT_FROM             11 (Token)
-                62 STORE_NAME              11 (Token)
-                64 POP_TOP
-   
-     5          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('FilterExpression',))
-                70 IMPORT_NAME              9 (django.template.base)
-                72 IMPORT_FROM             12 (FilterExpression)
-                74 STORE_NAME              12 (FilterExpression)
-                76 POP_TOP
-   
-     6          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('mark_safe',))
-                82 IMPORT_NAME             13 (django.utils.safestring)
-                84 IMPORT_FROM             14 (mark_safe)
-                86 STORE_NAME              14 (mark_safe)
-                88 POP_TOP
-   
-     7          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('HttpRequest',))
-                94 IMPORT_NAME             15 (django.http)
-                96 IMPORT_FROM             16 (HttpRequest)
-                98 STORE_NAME              16 (HttpRequest)
-               100 POP_TOP
-   
-     8         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               8 (('reverse',))
-               106 IMPORT_NAME             17 (django.urls)
-               108 IMPORT_FROM             18 (reverse)
-               110 STORE_NAME              18 (reverse)
-               112 POP_TOP
-   
-     9         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST               9 (('signing',))
-               118 IMPORT_NAME             19 (django.core)
-               120 IMPORT_FROM             20 (signing)
-               122 STORE_NAME              20 (signing)
-               124 POP_TOP
-   
-    10         126 LOAD_CONST               0 (0)
-               128 LOAD_CONST              10 (('models',))
-               130 IMPORT_NAME             21 (django.db)
-               132 IMPORT_FROM             22 (models)
-               134 STORE_NAME              22 (models)
-               136 POP_TOP
-   
-    12         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST              11 (('BoundBlock',))
-               142 IMPORT_NAME             23 (wagtail.blocks)
-               144 IMPORT_FROM             24 (BoundBlock)
-               146 STORE_NAME              24 (BoundBlock)
-               148 POP_TOP
-   
-    13         150 LOAD_CONST               0 (0)
-               152 LOAD_CONST              12 (('hooks',))
-               154 IMPORT_NAME             25 (wagtail)
-               156 IMPORT_FROM             26 (hooks)
-               158 STORE_NAME              26 (hooks)
-               160 POP_TOP
-   
-    14         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST              13 (('urlencode',))
-               166 IMPORT_NAME             27 (urllib.parse)
-               168 IMPORT_FROM             28 (urlencode)
-               170 STORE_NAME              28 (urlencode)
-               172 POP_TOP
-   
-    16         174 LOAD_CONST               0 (0)
-               176 LOAD_CONST              14 (None)
-               178 IMPORT_NAME             29 (warnings)
-               180 STORE_NAME              29 (warnings)
-   
-    18         182 LOAD_CONST              15 (2)
-               184 LOAD_CONST              16 (('FeditBlockEditButton', 'FeditAdapterEditButton'))
-               186 IMPORT_NAME             30 (toolbar)
-               188 IMPORT_FROM             31 (FeditBlockEditButton)
-               190 STORE_NAME              31 (FeditBlockEditButton)
-               192 IMPORT_FROM             32 (FeditAdapterEditButton)
-               194 STORE_NAME              32 (FeditAdapterEditButton)
-               196 POP_TOP
-   
-    22         198 LOAD_CONST              15 (2)
-               200 LOAD_CONST              17 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter'))
-               202 IMPORT_NAME             33 (adapters)
-               204 IMPORT_FROM             34 (adapter_registry)
-               206 STORE_NAME              34 (adapter_registry)
-               208 IMPORT_FROM             35 (RegistryLookUpError)
-               210 STORE_NAME              35 (RegistryLookUpError)
-               212 IMPORT_FROM             36 (BaseAdapter)
-               214 STORE_NAME              36 (BaseAdapter)
-               216 POP_TOP
-   
-    27         218 LOAD_CONST              15 (2)
-               220 LOAD_CONST              18 (('_can_edit', 'edit_url'))
-               222 IMPORT_NAME             37 (utils)
-               224 IMPORT_FROM             38 (_can_edit)
-               226 STORE_NAME              38 (_can_edit)
-               228 IMPORT_FROM             39 (edit_url)
-               230 STORE_NAME              39 (edit_url)
-               232 POP_TOP
-   
-    31         234 LOAD_CONST              15 (2)
-               236 LOAD_CONST              19 (('CONSTRUCT_ADAPTER_TOOLBAR',))
-               238 IMPORT_NAME             26 (hooks)
-               240 IMPORT_FROM             40 (CONSTRUCT_ADAPTER_TOOLBAR)
-               242 STORE_NAME              40 (CONSTRUCT_ADAPTER_TOOLBAR)
-               244 POP_TOP
-   
-    36         246 PUSH_NULL
-               248 LOAD_NAME                3 (library)
-               250 LOAD_ATTR               41 (Library)
-               260 PRECALL                  0
-               264 CALL                     0
-               274 STORE_NAME              42 (register)
-   
-    39         276 LOAD_CONST              20 ('Field name is not available in the context for %(object)s.')
-               278 STORE_NAME              43 (WARNING_FIELD_NAME_NOT_AVAILABLE)
-   
-    40         280 LOAD_CONST              21 ('Model instance is not available in the context for %(object)s.')
-               282 STORE_NAME              44 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
-   
-    44         284 PUSH_NULL
-               286 LOAD_BUILD_CLASS
-               288 LOAD_CONST              22 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 44>)
-               290 MAKE_FUNCTION            0
-               292 LOAD_CONST              23 ('AdapterNode')
-               294 LOAD_NAME                4 (Node)
-               296 PRECALL                  3
-               300 CALL                     3
-               310 STORE_NAME              45 (AdapterNode)
-   
-   107         312 LOAD_NAME               42 (register)
-               314 LOAD_METHOD             46 (tag)
-               336 LOAD_CONST              24 ('fedit')
-               338 KW_NAMES                25
-               340 PRECALL                  1
-               344 CALL                     1
-   
-   108         354 LOAD_CONST              26 ('parser')
-               356 LOAD_NAME               10 (Parser)
-               358 LOAD_CONST              27 ('token')
-               360 LOAD_NAME               11 (Token)
-               362 BUILD_TUPLE              4
-               364 LOAD_CONST              28 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 107>)
-               366 MAKE_FUNCTION            4 (annotations)
-   
-   107         368 PRECALL                  0
-               372 CALL                     0
-   
-   108         382 STORE_NAME              47 (do_render_fedit)
-   
-   146         384 LOAD_CONST              29 ('request')
-               386 LOAD_NAME               16 (HttpRequest)
-               388 LOAD_CONST              30 ('adapter')
-               390 LOAD_NAME               36 (BaseAdapter)
-               392 LOAD_CONST              31 ('context')
-               394 LOAD_NAME               48 (dict)
-               396 LOAD_CONST              32 ('return')
-               398 LOAD_NAME               49 (str)
-               400 BUILD_TUPLE              8
-               402 LOAD_CONST              33 (<code object wrap_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 146>)
-               404 MAKE_FUNCTION            4 (annotations)
-               406 STORE_NAME              50 (wrap_adapter)
-   
-   192         408 LOAD_CONST              37 ((None,))
-               410 LOAD_CONST              26 ('parser')
-               412 LOAD_NAME               10 (Parser)
-               414 LOAD_CONST              34 ('tokens')
-               416 LOAD_NAME               51 (list)
-               418 LOAD_NAME               49 (str)
-               420 BINARY_SUBSCR
-               430 LOAD_CONST              35 ('kwarg_list')
-               432 LOAD_NAME               51 (list)
-               434 LOAD_NAME               49 (str)
-               436 BINARY_SUBSCR
-               446 LOAD_CONST              32 ('return')
-               448 LOAD_NAME               48 (dict)
-               450 BUILD_TUPLE              8
-               452 LOAD_CONST              36 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 192>)
-               454 MAKE_FUNCTION            5 (defaults, annotations)
-               456 STORE_NAME              52 (get_kwargs)
-               458 LOAD_CONST              14 (None)
-               460 RETURN_VALUE
+                28 IMPORT_FROM              5 (TemplateSyntaxError)
+                30 STORE_NAME               5 (TemplateSyntaxError)
+                32 POP_TOP
+   
+     3          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               3 (('render_to_string',))
+                38 IMPORT_NAME              6 (django.template.loader)
+                40 IMPORT_FROM              7 (render_to_string)
+                42 STORE_NAME               7 (render_to_string)
+                44 POP_TOP
+   
+     4          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('Parser', 'Token'))
+                50 IMPORT_NAME              8 (django.template.base)
+                52 IMPORT_FROM              9 (Parser)
+                54 STORE_NAME               9 (Parser)
+                56 IMPORT_FROM             10 (Token)
+                58 STORE_NAME              10 (Token)
+                60 POP_TOP
+   
+     5          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               5 (('FilterExpression',))
+                66 IMPORT_NAME              8 (django.template.base)
+                68 IMPORT_FROM             11 (FilterExpression)
+                70 STORE_NAME              11 (FilterExpression)
+                72 POP_TOP
+   
+     6          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               6 (('HttpRequest',))
+                78 IMPORT_NAME             12 (django.http)
+                80 IMPORT_FROM             13 (HttpRequest)
+                82 STORE_NAME              13 (HttpRequest)
+                84 POP_TOP
+   
+     7          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               7 (('reverse',))
+                90 IMPORT_NAME             14 (django.urls)
+                92 IMPORT_FROM             15 (reverse)
+                94 STORE_NAME              15 (reverse)
+                96 POP_TOP
+   
+     8          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               8 (('signing',))
+               102 IMPORT_NAME             16 (django.core)
+               104 IMPORT_FROM             17 (signing)
+               106 STORE_NAME              17 (signing)
+               108 POP_TOP
+   
+    10         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               9 (('hooks',))
+               114 IMPORT_NAME             18 (wagtail)
+               116 IMPORT_FROM             19 (hooks)
+               118 STORE_NAME              19 (hooks)
+               120 POP_TOP
+   
+    12         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST              10 (None)
+               126 IMPORT_NAME             20 (warnings)
+               128 STORE_NAME              20 (warnings)
+   
+    14         130 LOAD_CONST              11 (2)
+               132 LOAD_CONST              12 (('FeditAdapterEditButton',))
+               134 IMPORT_NAME             21 (toolbar)
+               136 IMPORT_FROM             22 (FeditAdapterEditButton)
+               138 STORE_NAME              22 (FeditAdapterEditButton)
+               140 POP_TOP
+   
+    17         142 LOAD_CONST              11 (2)
+               144 LOAD_CONST              13 (('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError'))
+               146 IMPORT_NAME             23 (adapters)
+               148 IMPORT_FROM             24 (adapter_registry)
+               150 STORE_NAME              24 (adapter_registry)
+               152 IMPORT_FROM             25 (RegistryLookUpError)
+               154 STORE_NAME              25 (RegistryLookUpError)
+               156 IMPORT_FROM             26 (BaseAdapter)
+               158 STORE_NAME              26 (BaseAdapter)
+               160 IMPORT_FROM             27 (AdapterError)
+               162 STORE_NAME              27 (AdapterError)
+               164 POP_TOP
+   
+    23         166 LOAD_CONST              11 (2)
+               168 LOAD_CONST              14 (('_can_edit',))
+               170 IMPORT_NAME             28 (utils)
+               172 IMPORT_FROM             29 (_can_edit)
+               174 STORE_NAME              29 (_can_edit)
+               176 POP_TOP
+   
+    26         178 LOAD_CONST              11 (2)
+               180 LOAD_CONST              15 (('CONSTRUCT_ADAPTER_TOOLBAR',))
+               182 IMPORT_NAME             19 (hooks)
+               184 IMPORT_FROM             30 (CONSTRUCT_ADAPTER_TOOLBAR)
+               186 STORE_NAME              30 (CONSTRUCT_ADAPTER_TOOLBAR)
+               188 POP_TOP
+   
+    31         190 PUSH_NULL
+               192 LOAD_NAME                3 (library)
+               194 LOAD_ATTR               31 (Library)
+               204 PRECALL                  0
+               208 CALL                     0
+               218 STORE_NAME              32 (register)
+   
+    34         220 LOAD_CONST              16 ('Field name is not available in the context for %(object)s.')
+               222 STORE_NAME              33 (WARNING_FIELD_NAME_NOT_AVAILABLE)
+   
+    35         224 LOAD_CONST              17 ('Model instance is not available in the context for %(object)s.')
+               226 STORE_NAME              34 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+   
+    39         228 PUSH_NULL
+               230 LOAD_BUILD_CLASS
+               232 LOAD_CONST              18 (<code object AdapterNode, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 39>)
+               234 MAKE_FUNCTION            0
+               236 LOAD_CONST              19 ('AdapterNode')
+               238 LOAD_NAME                4 (Node)
+               240 PRECALL                  3
+               244 CALL                     3
+               254 STORE_NAME              35 (AdapterNode)
+   
+   116         256 LOAD_NAME               32 (register)
+               258 LOAD_METHOD             36 (tag)
+               280 LOAD_CONST              20 ('fedit')
+               282 KW_NAMES                21
+               284 PRECALL                  1
+               288 CALL                     1
+   
+   117         298 LOAD_CONST              22 ('parser')
+               300 LOAD_NAME                9 (Parser)
+               302 LOAD_CONST              23 ('token')
+               304 LOAD_NAME               10 (Token)
+               306 BUILD_TUPLE              4
+               308 LOAD_CONST              24 (<code object do_render_fedit, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 116>)
+               310 MAKE_FUNCTION            4 (annotations)
+   
+   116         312 PRECALL                  0
+               316 CALL                     0
+   
+   117         326 STORE_NAME              37 (do_render_fedit)
+   
+   155         328 LOAD_CONST              25 ('request')
+               330 LOAD_NAME               13 (HttpRequest)
+               332 LOAD_CONST              26 ('adapter')
+               334 LOAD_NAME               26 (BaseAdapter)
+               336 LOAD_CONST              27 ('context')
+               338 LOAD_NAME               38 (dict)
+               340 LOAD_CONST              28 ('return')
+               342 LOAD_NAME               39 (str)
+               344 BUILD_TUPLE              8
+               346 LOAD_CONST              29 (<code object wrap_adapter, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 155>)
+               348 MAKE_FUNCTION            4 (annotations)
+               350 STORE_NAME              40 (wrap_adapter)
+   
+   202         352 LOAD_CONST              33 ((None,))
+               354 LOAD_CONST              22 ('parser')
+               356 LOAD_NAME                9 (Parser)
+               358 LOAD_CONST              30 ('tokens')
+               360 LOAD_NAME               41 (list)
+               362 LOAD_NAME               39 (str)
+               364 BINARY_SUBSCR
+               374 LOAD_CONST              31 ('kwarg_list')
+               376 LOAD_NAME               41 (list)
+               378 LOAD_NAME               39 (str)
+               380 BINARY_SUBSCR
+               390 LOAD_CONST              28 ('return')
+               392 LOAD_NAME               38 (dict)
+               394 BUILD_TUPLE              8
+               396 LOAD_CONST              32 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 202>)
+               398 MAKE_FUNCTION            5 (defaults, annotations)
+               400 STORE_NAME              42 (get_kwargs)
+               402 LOAD_CONST              10 (None)
+               404 RETURN_VALUE
    consts
       0
       ('Type',)
-      ('library', 'Node', 'NodeList', 'TemplateSyntaxError')
+      ('library', 'Node', 'TemplateSyntaxError')
       ('render_to_string',)
       ('Parser', 'Token')
       ('FilterExpression',)
-      ('mark_safe',)
       ('HttpRequest',)
       ('reverse',)
       ('signing',)
-      ('models',)
-      ('BoundBlock',)
       ('hooks',)
-      ('urlencode',)
       None
       2
-      ('FeditBlockEditButton', 'FeditAdapterEditButton')
-      ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter')
-      ('_can_edit', 'edit_url')
+      ('FeditAdapterEditButton',)
+      ('adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError')
+      ('_can_edit',)
       ('CONSTRUCT_ADAPTER_TOOLBAR',)
       'Field name is not available in the context for %(object)s.'
       'Model instance is not available in the context for %(object)s.'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02020065036a040000000000000000a6000000ab
             0000000000000000005a0564016506650719000000000000000000640265
             0864036509650a190000000000000000006606640484045a0b640584005a
             0c640684005a0d64075300
-          44           0 RESUME                   0
+          39           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdapterNode')
                        8 STORE_NAME               2 (__qualname__)
          
-          45          10 PUSH_NULL
+          40          10 PUSH_NULL
                       12 LOAD_NAME                3 (signing)
                       14 LOAD_ATTR                4 (TimestampSigner)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_NAME               5 (signer)
          
-          47          40 LOAD_CONST               1 ('adapter')
+          42          40 LOAD_CONST               1 ('adapter')
                       42 LOAD_NAME                6 (Type)
                       44 LOAD_NAME                7 (BaseAdapter)
                       46 BINARY_SUBSCR
                       56 LOAD_CONST               2 ('model')
                       58 LOAD_NAME                8 (FilterExpression)
                       60 LOAD_CONST               3 ('getters')
                       62 LOAD_NAME                9 (list)
                       64 LOAD_NAME               10 (str)
                       66 BINARY_SUBSCR
                       76 BUILD_TUPLE              6
-                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 47>)
+                      78 LOAD_CONST               4 (<code object __init__, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 42>)
                       80 MAKE_FUNCTION            4 (annotations)
                       82 STORE_NAME              11 (__init__)
          
-          53          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 53>)
+          48          84 LOAD_CONST               5 (<code object _resolve_expressions, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 48>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME              12 (_resolve_expressions)
          
-          63          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 63>)
+          58          90 LOAD_CONST               6 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 58>)
                       92 MAKE_FUNCTION            0
                       94 STORE_NAME              13 (render)
                       96 LOAD_CONST               7 (None)
                       98 RETURN_VALUE
          consts
             'AdapterNode'
             'adapter'
@@ -320,42 +282,42 @@
                nlocals   : 5
                stacksize : 2
                flags     : 11
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   007c037c005f0200000000000000007c047c005f03000000000000000064
                   005300
-                47           0 RESUME                   0
+                42           0 RESUME                   0
                
-                48           2 LOAD_FAST                1 (adapter)
+                43           2 LOAD_FAST                1 (adapter)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (adapter)
                
-                49          16 LOAD_FAST                2 (model)
+                44          16 LOAD_FAST                2 (model)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (model)
                
-                50          30 LOAD_FAST                3 (getters)
+                45          30 LOAD_FAST                3 (getters)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (getters)
                
-                51          44 LOAD_FAST                4 (kwargs)
+                46          44 LOAD_FAST                4 (kwargs)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (kwargs)
                             58 LOAD_CONST               0 (None)
                             60 RETURN_VALUE
                consts
                   None
                names      ('adapter', 'model', 'getters', 'kwargs')
                varnames   ('self', 'adapter', 'model', 'getters', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
-               firstlineno 47
+               firstlineno 42
                lnotab 0x02010e010e010e01
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
                flags     : 11
                code
@@ -363,316 +325,391 @@
                   00ab00000000000000000044005d325c0200007d047d0574030000000000
                   00000000007c05740400000000000000000000a6020000ab020000000000
                   00000072187c05a00300000000000000000000000000000000000000007c
                   01a6010000ab0100000000000000007c037c043c0000008c337403000000
                   000000000000007c02740400000000000000000000a6020000ab02000000
                   000000000072157c02a00300000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c027c0366025300
-                53           0 RESUME                   0
+                48           0 RESUME                   0
                
-                54           2 LOAD_FAST                3 (kwargs)
+                49           2 LOAD_FAST                3 (kwargs)
                              4 LOAD_METHOD              0 (items)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 GET_ITER
                        >>   42 FOR_ITER                50 (to 144)
                             44 UNPACK_SEQUENCE          2
                             48 STORE_FAST               4 (k)
                             50 STORE_FAST               5 (v)
                
-                55          52 LOAD_GLOBAL              3 (NULL + isinstance)
+                50          52 LOAD_GLOBAL              3 (NULL + isinstance)
                             64 LOAD_FAST                5 (v)
                             66 LOAD_GLOBAL              4 (FilterExpression)
                             78 PRECALL                  2
                             82 CALL                     2
                             92 POP_JUMP_FORWARD_IF_FALSE    24 (to 142)
                
-                56          94 LOAD_FAST                5 (v)
+                51          94 LOAD_FAST                5 (v)
                             96 LOAD_METHOD              3 (resolve)
                            118 LOAD_FAST                1 (context)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (kwargs)
                            136 LOAD_FAST                4 (k)
                            138 STORE_SUBSCR
                        >>  142 JUMP_BACKWARD           51 (to 42)
                
-                58     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
+                53     >>  144 LOAD_GLOBAL              3 (NULL + isinstance)
                            156 LOAD_FAST                2 (model)
                            158 LOAD_GLOBAL              4 (FilterExpression)
                            170 PRECALL                  2
                            174 CALL                     2
                            184 POP_JUMP_FORWARD_IF_FALSE    21 (to 228)
                
-                59         186 LOAD_FAST                2 (model)
+                54         186 LOAD_FAST                2 (model)
                            188 LOAD_METHOD              3 (resolve)
                            210 LOAD_FAST                1 (context)
                            212 PRECALL                  1
                            216 CALL                     1
                            226 STORE_FAST               2 (model)
                
-                61     >>  228 LOAD_FAST                2 (model)
+                56     >>  228 LOAD_FAST                2 (model)
                            230 LOAD_FAST                3 (kwargs)
                            232 BUILD_TUPLE              2
                            234 RETURN_VALUE
                consts
                   None
                names      ('items', 'isinstance', 'FilterExpression', 'resolve')
                varnames   ('self', 'context', 'model', 'kwargs', 'k', 'v')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '_resolve_expressions'
-               firstlineno 53
+               firstlineno 48
                lnotab 0x020132012a0132022a012a02
             code
                argcount  : 2
-               nlocals   : 11
+               nlocals   : 12
                stacksize : 8
                flags     : 3
                code
                   0x97007c006a0000000000000000007d027c006a0100000000000000007d
                   0302007c006a0200000000000000007c017c02660269007c006a03000000
-                  0000000000a4018e015c0200007d027d0464017c017600721764027c0176
-                  0072137c0273117c016401190000000000000000007d057c016402190000
-                  000000000000007d066e937c02730f7409000000000000000000006403a6
-                  010000ab01000000000000000082017c03740b000000000000000000007c
-                  03a6010000ab01000000000000000064047a0a0000190000000000000000
-                  007d057c027d06740d00000000000000000000740b000000000000000000
-                  007c03a6010000ab01000000000000000064047a0a0000a6010000ab0100
-                  0000000000000044005d487d077c037c07190000000000000000007d0809
-                  00740f000000000000000000007c067c08a6020000ab0200000000000000
-                  007d068c1c23007410000000000000000000002400722001007411000000
-                  0000000000000064057c026a0900000000000000006a0a00000000000000
-                  009b0064067c089b009d04a6010000ab0100000000000000008201770078
-                  03590077017c01a00b000000000000000000000000000000000000000064
-                  07a6010000ab0100000000000000007d0902007c006a0c00000000000000
-                  0064097c067c057c0964089c037c04a4018e017d0a7c0aa00d0000000000
-                  000000000000000000000000000000a6000000ab00000000000000000072
-                  10741d000000000000000000007c097c06a6020000ab0200000000000000
-                  0073157c0aa00f00000000000000000000000000000000000000007c01a6
-                  010000ab01000000000000000053007421000000000000000000007c097c
-                  0a7c01a6030000ab0300000000000000005300
-                63           0 RESUME                   0
+                  0000000000a4018e015c0200007d027d0464017c017600721864027c0176
+                  0072147c0273127c016401190000000000000000007d057c016402190000
+                  000000000000007d0690016e087c0273847409000000000000000000006a
+                  050000000000000000740c0000000000000000000064037c006a07000000
+                  00000000006a08000000000000000069017a060000741200000000000000
+                  000000a6020000ab02000000000000000001007c01a00a00000000000000
+                  00000000000000000000000000a6000000ab0000000000000000007d0109
+                  0002007c006a0700000000000000006a0b00000000000000007c01660169
+                  007c04a4018e0153002300741800000000000000000000240072217d0774
+                  1b00000000000000000000741d000000000000000000007c07a6010000ab
+                  010000000000000000a6010000ab010000000000000000820164007d077e
+                  07770177007803590077017c03741f000000000000000000007c03a60100
+                  00ab01000000000000000064047a0a0000190000000000000000007d057c
+                  027d06742100000000000000000000741f000000000000000000007c03a6
+                  010000ab01000000000000000064047a0a0000a6010000ab010000000000
+                  00000044005d487d087c037c08190000000000000000007d090900742300
+                  0000000000000000007c067c09a6020000ab0200000000000000007d068c
+                  1c2300742400000000000000000000240072200100742500000000000000
+                  00000064057c026a1300000000000000006a0800000000000000009b0064
+                  067c099b009d04a6010000ab010000000000000000820177007803590077
+                  017c01a01400000000000000000000000000000000000000006407a60100
+                  00ab0100000000000000007d0a02007c006a07000000000000000064097c
+                  067c057c0a64089c037c04a4018e017d0b7c0ba015000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000007210742d00
+                  0000000000000000007c0a7c06a6020000ab02000000000000000073157c
+                  0ba01700000000000000000000000000000000000000007c01a6010000ab
+                  01000000000000000053007431000000000000000000007c0a7c0b7c01a6
+                  030000ab0300000000000000005300
+                58           0 RESUME                   0
                
-                64           2 LOAD_FAST                0 (self)
+                59           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (model)
                             14 STORE_FAST               2 (model)
                
-                65          16 LOAD_FAST                0 (self)
+                60          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (getters)
                             28 STORE_FAST               3 (getters)
                
-                67          30 PUSH_NULL
+                62          30 PUSH_NULL
                             32 LOAD_FAST                0 (self)
                             34 LOAD_ATTR                2 (_resolve_expressions)
                
-                68          44 LOAD_FAST                1 (context)
+                63          44 LOAD_FAST                1 (context)
                             46 LOAD_FAST                2 (model)
                
-                67          48 BUILD_TUPLE              2
+                62          48 BUILD_TUPLE              2
                             50 BUILD_MAP                0
                
-                68          52 LOAD_FAST                0 (self)
+                63          52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (kwargs)
                
-                67          64 DICT_MERGE               1
+                62          64 DICT_MERGE               1
                             66 CALL_FUNCTION_EX         1
                             68 UNPACK_SEQUENCE          2
                             72 STORE_FAST               2 (model)
                             74 STORE_FAST               4 (kwargs)
                
-                71          76 LOAD_CONST               1 ('wagtail_fedit_field')
+                66          76 LOAD_CONST               1 ('wagtail_fedit_field')
                             78 LOAD_FAST                1 (context)
                             80 CONTAINS_OP              0
-                            82 POP_JUMP_FORWARD_IF_FALSE    23 (to 130)
+                            82 POP_JUMP_FORWARD_IF_FALSE    24 (to 132)
                
-                72          84 LOAD_CONST               2 ('wagtail_fedit_instance')
+                67          84 LOAD_CONST               2 ('wagtail_fedit_instance')
                             86 LOAD_FAST                1 (context)
                             88 CONTAINS_OP              0
-                            90 POP_JUMP_FORWARD_IF_FALSE    19 (to 130)
+                            90 POP_JUMP_FORWARD_IF_FALSE    20 (to 132)
                
-                73          92 LOAD_FAST                2 (model)
+                68          92 LOAD_FAST                2 (model)
                
-                72          94 POP_JUMP_FORWARD_IF_TRUE    17 (to 130)
+                67          94 POP_JUMP_FORWARD_IF_TRUE    18 (to 132)
                
-                75          96 LOAD_FAST                1 (context)
+                70          96 LOAD_FAST                1 (context)
                             98 LOAD_CONST               1 ('wagtail_fedit_field')
                            100 BINARY_SUBSCR
                            110 STORE_FAST               5 (field_name)
                
-                76         112 LOAD_FAST                1 (context)
+                71         112 LOAD_FAST                1 (context)
                            114 LOAD_CONST               2 ('wagtail_fedit_instance')
                            116 BINARY_SUBSCR
                            126 STORE_FAST               6 (obj)
-                           128 JUMP_FORWARD           147 (to 424)
+                           128 EXTENDED_ARG             1
+                           130 JUMP_FORWARD           264 (to 660)
                
-                80     >>  130 LOAD_FAST                2 (model)
-                           132 POP_JUMP_FORWARD_IF_TRUE    15 (to 164)
+                75     >>  132 LOAD_FAST                2 (model)
+                           134 POP_JUMP_FORWARD_IF_TRUE   132 (to 400)
                
-                81         134 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
-                           146 LOAD_CONST               3 ('Model is required')
-                           148 PRECALL                  1
-                           152 CALL                     1
-                           162 RAISE_VARARGS            1
-               
-                83     >>  164 LOAD_FAST                3 (getters)
-                           166 LOAD_GLOBAL             11 (NULL + len)
-                           178 LOAD_FAST                3 (getters)
-                           180 PRECALL                  1
-                           184 CALL                     1
-                           194 LOAD_CONST               4 (1)
-                           196 BINARY_OP               10 (-)
-                           200 BINARY_SUBSCR
-                           210 STORE_FAST               5 (field_name)
-               
-                84         212 LOAD_FAST                2 (model)
-                           214 STORE_FAST               6 (obj)
-               
-                85         216 LOAD_GLOBAL             13 (NULL + range)
-                           228 LOAD_GLOBAL             11 (NULL + len)
-                           240 LOAD_FAST                3 (getters)
-                           242 PRECALL                  1
-                           246 CALL                     1
-                           256 LOAD_CONST               4 (1)
-                           258 BINARY_OP               10 (-)
-                           262 PRECALL                  1
-                           266 CALL                     1
-                           276 GET_ITER
-                       >>  278 FOR_ITER                72 (to 424)
-                           280 STORE_FAST               7 (i)
-               
-                86         282 LOAD_FAST                3 (getters)
-                           284 LOAD_FAST                7 (i)
-                           286 BINARY_SUBSCR
-                           296 STORE_FAST               8 (getter)
-               
-                87         298 NOP
-               
-                88         300 LOAD_GLOBAL             15 (NULL + getattr)
-                           312 LOAD_FAST                6 (obj)
-                           314 LOAD_FAST                8 (getter)
-                           316 PRECALL                  2
-                           320 CALL                     2
-                           330 STORE_FAST               6 (obj)
-                           332 JUMP_BACKWARD           28 (to 278)
-                       >>  334 PUSH_EXC_INFO
-               
-                89         336 LOAD_GLOBAL             16 (AttributeError)
-                           348 CHECK_EXC_MATCH
-                           350 POP_JUMP_FORWARD_IF_FALSE    32 (to 416)
-                           352 POP_TOP
-               
-                90         354 LOAD_GLOBAL             17 (NULL + AttributeError)
-                           366 LOAD_CONST               5 ('Object ')
-                           368 LOAD_FAST                2 (model)
-                           370 LOAD_ATTR                9 (__class__)
-                           380 LOAD_ATTR               10 (__name__)
-                           390 FORMAT_VALUE             0
-                           392 LOAD_CONST               6 (' does not have attribute ')
-                           394 LOAD_FAST                8 (getter)
-                           396 FORMAT_VALUE             0
-                           398 BUILD_STRING             4
-                           400 PRECALL                  1
-                           404 CALL                     1
-                           414 RAISE_VARARGS            1
-               
-                89     >>  416 RERAISE                  0
-                       >>  418 COPY                     3
-                           420 POP_EXCEPT
-                           422 RERAISE                  1
-               
-                92     >>  424 LOAD_FAST                1 (context)
-                           426 LOAD_METHOD             11 (get)
-                           448 LOAD_CONST               7 ('request')
-                           450 PRECALL                  1
-                           454 CALL                     1
-                           464 STORE_FAST               9 (request)
-               
-                93         466 PUSH_NULL
-                           468 LOAD_FAST                0 (self)
-                           470 LOAD_ATTR               12 (adapter)
-                           480 LOAD_CONST               9 (())
-               
-                94         482 LOAD_FAST                6 (obj)
-               
-                95         484 LOAD_FAST                5 (field_name)
-               
-                96         486 LOAD_FAST                9 (request)
-               
-                93         488 LOAD_CONST               8 (('object', 'field_name', 'request'))
-                           490 BUILD_CONST_KEY_MAP      3
-               
-                97         492 LOAD_FAST                4 (kwargs)
-               
-                93         494 DICT_MERGE               1
-                           496 CALL_FUNCTION_EX         1
-                           498 STORE_FAST              10 (adapter)
-               
-               100         500 LOAD_FAST               10 (adapter)
-                           502 LOAD_METHOD             13 (check_permissions)
-                           524 PRECALL                  0
-                           528 CALL                     0
-                           538 POP_JUMP_FORWARD_IF_FALSE    16 (to 572)
-               
-               101         540 LOAD_GLOBAL             29 (NULL + _can_edit)
-                           552 LOAD_FAST                9 (request)
-                           554 LOAD_FAST                6 (obj)
-                           556 PRECALL                  2
-                           560 CALL                     2
-               
-               100         570 POP_JUMP_FORWARD_IF_TRUE    21 (to 614)
-               
-               102     >>  572 LOAD_FAST               10 (adapter)
-                           574 LOAD_METHOD             15 (render_content)
-                           596 LOAD_FAST                1 (context)
-                           598 PRECALL                  1
-                           602 CALL                     1
-                           612 RETURN_VALUE
-               
-               104     >>  614 LOAD_GLOBAL             33 (NULL + wrap_adapter)
-                           626 LOAD_FAST                9 (request)
-                           628 LOAD_FAST               10 (adapter)
-                           630 LOAD_FAST                1 (context)
-                           632 PRECALL                  3
-                           636 CALL                     3
-                           646 RETURN_VALUE
+                76         136 LOAD_GLOBAL              9 (NULL + warnings)
+                           148 LOAD_ATTR                5 (warn)
+               
+                77         158 LOAD_GLOBAL             12 (WARNING_MODEL_INSTANCE_NOT_AVAILABLE)
+               
+                78         170 LOAD_CONST               3 ('object')
+                           172 LOAD_FAST                0 (self)
+                           174 LOAD_ATTR                7 (adapter)
+                           184 LOAD_ATTR                8 (__name__)
+               
+                77         194 BUILD_MAP                1
+                           196 BINARY_OP                6 (%)
+               
+                80         200 LOAD_GLOBAL             18 (RuntimeWarning)
+               
+                76         212 PRECALL                  2
+                           216 CALL                     2
+                           226 POP_TOP
+               
+                83         228 LOAD_FAST                1 (context)
+                           230 LOAD_METHOD             10 (flatten)
+                           252 PRECALL                  0
+                           256 CALL                     0
+                           266 STORE_FAST               1 (context)
+               
+                85         268 NOP
+               
+                86         270 PUSH_NULL
+                           272 LOAD_FAST                0 (self)
+                           274 LOAD_ATTR                7 (adapter)
+                           284 LOAD_ATTR               11 (render_from_kwargs)
+               
+                87         294 LOAD_FAST                1 (context)
+               
+                86         296 BUILD_TUPLE              1
+                           298 BUILD_MAP                0
+               
+                87         300 LOAD_FAST                4 (kwargs)
+               
+                86         302 DICT_MERGE               1
+                           304 CALL_FUNCTION_EX         1
+                           306 RETURN_VALUE
+                       >>  308 PUSH_EXC_INFO
+               
+                89         310 LOAD_GLOBAL             24 (AdapterError)
+                           322 CHECK_EXC_MATCH
+                           324 POP_JUMP_FORWARD_IF_FALSE    33 (to 392)
+                           326 STORE_FAST               7 (e)
+               
+                90         328 LOAD_GLOBAL             27 (NULL + TemplateSyntaxError)
+                           340 LOAD_GLOBAL             29 (NULL + str)
+                           352 LOAD_FAST                7 (e)
+                           354 PRECALL                  1
+                           358 CALL                     1
+                           368 PRECALL                  1
+                           372 CALL                     1
+                           382 RAISE_VARARGS            1
+                       >>  384 LOAD_CONST               0 (None)
+                           386 STORE_FAST               7 (e)
+                           388 DELETE_FAST              7 (e)
+                           390 RERAISE                  1
+               
+                89     >>  392 RERAISE                  0
+                       >>  394 COPY                     3
+                           396 POP_EXCEPT
+                           398 RERAISE                  1
+               
+                92     >>  400 LOAD_FAST                3 (getters)
+                           402 LOAD_GLOBAL             31 (NULL + len)
+                           414 LOAD_FAST                3 (getters)
+                           416 PRECALL                  1
+                           420 CALL                     1
+                           430 LOAD_CONST               4 (1)
+                           432 BINARY_OP               10 (-)
+                           436 BINARY_SUBSCR
+                           446 STORE_FAST               5 (field_name)
+               
+                93         448 LOAD_FAST                2 (model)
+                           450 STORE_FAST               6 (obj)
+               
+                94         452 LOAD_GLOBAL             33 (NULL + range)
+                           464 LOAD_GLOBAL             31 (NULL + len)
+                           476 LOAD_FAST                3 (getters)
+                           478 PRECALL                  1
+                           482 CALL                     1
+                           492 LOAD_CONST               4 (1)
+                           494 BINARY_OP               10 (-)
+                           498 PRECALL                  1
+                           502 CALL                     1
+                           512 GET_ITER
+                       >>  514 FOR_ITER                72 (to 660)
+                           516 STORE_FAST               8 (i)
+               
+                95         518 LOAD_FAST                3 (getters)
+                           520 LOAD_FAST                8 (i)
+                           522 BINARY_SUBSCR
+                           532 STORE_FAST               9 (getter)
+               
+                96         534 NOP
+               
+                97         536 LOAD_GLOBAL             35 (NULL + getattr)
+                           548 LOAD_FAST                6 (obj)
+                           550 LOAD_FAST                9 (getter)
+                           552 PRECALL                  2
+                           556 CALL                     2
+                           566 STORE_FAST               6 (obj)
+                           568 JUMP_BACKWARD           28 (to 514)
+                       >>  570 PUSH_EXC_INFO
+               
+                98         572 LOAD_GLOBAL             36 (AttributeError)
+                           584 CHECK_EXC_MATCH
+                           586 POP_JUMP_FORWARD_IF_FALSE    32 (to 652)
+                           588 POP_TOP
+               
+                99         590 LOAD_GLOBAL             37 (NULL + AttributeError)
+                           602 LOAD_CONST               5 ('Object ')
+                           604 LOAD_FAST                2 (model)
+                           606 LOAD_ATTR               19 (__class__)
+                           616 LOAD_ATTR                8 (__name__)
+                           626 FORMAT_VALUE             0
+                           628 LOAD_CONST               6 (' does not have attribute ')
+                           630 LOAD_FAST                9 (getter)
+                           632 FORMAT_VALUE             0
+                           634 BUILD_STRING             4
+                           636 PRECALL                  1
+                           640 CALL                     1
+                           650 RAISE_VARARGS            1
+               
+                98     >>  652 RERAISE                  0
+                       >>  654 COPY                     3
+                           656 POP_EXCEPT
+                           658 RERAISE                  1
+               
+               101     >>  660 LOAD_FAST                1 (context)
+                           662 LOAD_METHOD             20 (get)
+                           684 LOAD_CONST               7 ('request')
+                           686 PRECALL                  1
+                           690 CALL                     1
+                           700 STORE_FAST              10 (request)
+               
+               102         702 PUSH_NULL
+                           704 LOAD_FAST                0 (self)
+                           706 LOAD_ATTR                7 (adapter)
+                           716 LOAD_CONST               9 (())
+               
+               103         718 LOAD_FAST                6 (obj)
+               
+               104         720 LOAD_FAST                5 (field_name)
+               
+               105         722 LOAD_FAST               10 (request)
+               
+               102         724 LOAD_CONST               8 (('object', 'field_name', 'request'))
+                           726 BUILD_CONST_KEY_MAP      3
+               
+               106         728 LOAD_FAST                4 (kwargs)
+               
+               102         730 DICT_MERGE               1
+                           732 CALL_FUNCTION_EX         1
+                           734 STORE_FAST              11 (adapter)
+               
+               109         736 LOAD_FAST               11 (adapter)
+                           738 LOAD_METHOD             21 (check_permissions)
+                           760 PRECALL                  0
+                           764 CALL                     0
+                           774 POP_JUMP_FORWARD_IF_FALSE    16 (to 808)
+               
+               110         776 LOAD_GLOBAL             45 (NULL + _can_edit)
+                           788 LOAD_FAST               10 (request)
+                           790 LOAD_FAST                6 (obj)
+                           792 PRECALL                  2
+                           796 CALL                     2
+               
+               109         806 POP_JUMP_FORWARD_IF_TRUE    21 (to 850)
+               
+               111     >>  808 LOAD_FAST               11 (adapter)
+                           810 LOAD_METHOD             23 (render_content)
+                           832 LOAD_FAST                1 (context)
+                           834 PRECALL                  1
+                           838 CALL                     1
+                           848 RETURN_VALUE
+               
+               113     >>  850 LOAD_GLOBAL             49 (NULL + wrap_adapter)
+                           862 LOAD_FAST               10 (request)
+                           864 LOAD_FAST               11 (adapter)
+                           866 LOAD_FAST                1 (context)
+                           868 PRECALL                  3
+                           872 CALL                     3
+                           882 RETURN_VALUE
                ExceptionTable:
-                 300 to 330 -> 334 [1]
-                 334 to 416 -> 418 [2] lasti
+                 270 to 304 -> 308 [0]
+                 308 to 326 -> 394 [1] lasti
+                 328 to 382 -> 384 [1] lasti
+                 384 to 392 -> 394 [1] lasti
+                 536 to 566 -> 570 [1]
+                 570 to 652 -> 654 [2] lasti
                consts
                   None
                   'wagtail_fedit_field'
                   'wagtail_fedit_instance'
-                  'Model is required'
+                  'object'
                   1
                   'Object '
                   ' does not have attribute '
                   'request'
                   ('object', 'field_name', 'request')
                   ()
-               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'TemplateSyntaxError', 'len', 'range', 'getattr', 'AttributeError', '__class__', '__name__', 'get', 'adapter', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
-               varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'i', 'getter', 'request', 'adapter')
+               names      ('model', 'getters', '_resolve_expressions', 'kwargs', 'warnings', 'warn', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'adapter', '__name__', 'RuntimeWarning', 'flatten', 'render_from_kwargs', 'AdapterError', 'TemplateSyntaxError', 'str', 'len', 'range', 'getattr', 'AttributeError', '__class__', 'get', 'check_permissions', '_can_edit', 'render_content', 'wrap_adapter')
+               varnames   ('self', 'context', 'model', 'getters', 'kwargs', 'field_name', 'obj', 'e', 'i', 'getter', 'request', 'adapter')
                freevars   ()
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
-               firstlineno 63
+               firstlineno 58
                lnotab
-                  0x02010e010e020e0104ff04010cff0c040801080102ff02031001120404
-                  011e0230010401420110010201240112013eff08032a0110010201020102
+                  0x02010e010e020e0104ff04010cff0c040801080102ff02031001140404
+                  0116010c0118ff06030cfc100728020201180102ff040102ff0803120140
+                  ff080330010401420110010201240112013eff08032a0110010201020102
                   fd040402fc060728011eff02022a02
             None
          names      ('__name__', '__module__', '__qualname__', 'signing', 'TimestampSigner', 'signer', 'Type', 'BaseAdapter', 'FilterExpression', 'list', 'str', '__init__', '_resolve_expressions', 'render')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'AdapterNode'
-         firstlineno 44
+         firstlineno 39
          lnotab 0x0a011e022c06060a
       'AdapterNode'
       'fedit'
       ('name',)
       'parser'
       'token'
       code
@@ -698,153 +735,153 @@
             00000000007c07a6010000ab01000000000000000064096b040000000072
             287c00a00700000000000000000000000000000000000000007c07a00100
             000000000000000000000000000000000000006401a6010000ab01000000
             0000000000a6010000ab0100000000000000007d06741100000000000000
             0000007c007c027c056a090000000000000000a6030000ab030000000000
             0000007d09741500000000000000000000640b7c057c067c07640a9c037c
             09a4018e015300
-         107           0 RESUME                   0
+         116           0 RESUME                   0
          
-         110           2 LOAD_FAST                1 (token)
+         119           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         112          42 LOAD_FAST                2 (tokens)
+         121          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         113          84 LOAD_FAST                2 (tokens)
+         122          84 LOAD_FAST                2 (tokens)
                       86 LOAD_METHOD              1 (pop)
                      108 LOAD_CONST               1 (0)
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               4 (adapter_id)
          
-         115         126 NOP
+         124         126 NOP
          
-         116         128 LOAD_GLOBAL              4 (adapter_registry)
+         125         128 LOAD_GLOBAL              4 (adapter_registry)
                      140 LOAD_FAST                4 (adapter_id)
                      142 BINARY_SUBSCR
                      152 STORE_FAST               5 (adapter)
                      154 JUMP_FORWARD            33 (to 222)
                  >>  156 PUSH_EXC_INFO
          
-         117         158 LOAD_GLOBAL              6 (RegistryLookUpError)
+         126         158 LOAD_GLOBAL              6 (RegistryLookUpError)
                      170 CHECK_EXC_MATCH
                      172 POP_JUMP_FORWARD_IF_FALSE    20 (to 214)
                      174 POP_TOP
          
-         118         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         127         176 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
                      188 LOAD_CONST               2 ("No adapter found with identifier '")
                      190 LOAD_FAST                4 (adapter_id)
                      192 FORMAT_VALUE             0
                      194 LOAD_CONST               3 ("'")
                      196 BUILD_STRING             3
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RAISE_VARARGS            1
          
-         117     >>  214 RERAISE                  0
+         126     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          
-         120     >>  222 LOAD_CONST               4 ((None, None))
+         129     >>  222 LOAD_CONST               4 ((None, None))
                      224 UNPACK_SEQUENCE          2
                      228 STORE_FAST               6 (model)
                      230 STORE_FAST               7 (model_tokens)
          
-         121         232 LOAD_FAST                2 (tokens)
+         130         232 LOAD_FAST                2 (tokens)
                      234 POP_JUMP_FORWARD_IF_FALSE   147 (to 530)
          
-         122         236 LOAD_FAST                2 (tokens)
+         131         236 LOAD_FAST                2 (tokens)
                      238 LOAD_METHOD              1 (pop)
                      260 LOAD_CONST               1 (0)
                      262 PRECALL                  1
                      266 CALL                     1
                      276 STORE_FAST               8 (model__field)
          
-         123         278 LOAD_FAST                8 (model__field)
+         132         278 LOAD_FAST                8 (model__field)
                      280 LOAD_METHOD              5 (split)
                      302 LOAD_CONST               5 ('.')
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               7 (model_tokens)
          
-         125         320 LOAD_GLOBAL             13 (NULL + len)
+         134         320 LOAD_GLOBAL             13 (NULL + len)
                      332 LOAD_FAST                7 (model_tokens)
                      334 PRECALL                  1
                      338 CALL                     1
                      348 LOAD_CONST               6 (2)
                      350 COMPARE_OP               0 (<)
                      356 POP_JUMP_FORWARD_IF_FALSE    27 (to 412)
          
-         126         358 LOAD_FAST                7 (model_tokens)
+         135         358 LOAD_FAST                7 (model_tokens)
                      360 LOAD_CONST               1 (0)
                      362 BINARY_SUBSCR
                      372 LOAD_CONST               7 ('from_context')
                      374 COMPARE_OP               3 (!=)
                      380 POP_JUMP_FORWARD_IF_FALSE    15 (to 412)
          
-         127         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
+         136         382 LOAD_GLOBAL              9 (NULL + TemplateSyntaxError)
          
-         128         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
+         137         394 LOAD_CONST               8 ("Model and field name are required: 'mymodel.myfield' or 'from_context'")
          
-         127         396 PRECALL                  1
+         136         396 PRECALL                  1
                      400 CALL                     1
                      410 RAISE_VARARGS            1
          
-         131     >>  412 LOAD_GLOBAL             13 (NULL + len)
+         140     >>  412 LOAD_GLOBAL             13 (NULL + len)
                      424 LOAD_FAST                7 (model_tokens)
                      426 PRECALL                  1
                      430 CALL                     1
                      440 LOAD_CONST               9 (1)
                      442 COMPARE_OP               4 (>)
                      448 POP_JUMP_FORWARD_IF_FALSE    40 (to 530)
          
-         134         450 LOAD_FAST                0 (parser)
+         143         450 LOAD_FAST                0 (parser)
                      452 LOAD_METHOD              7 (compile_filter)
                      474 LOAD_FAST                7 (model_tokens)
                      476 LOAD_METHOD              1 (pop)
                      498 LOAD_CONST               1 (0)
                      500 PRECALL                  1
                      504 CALL                     1
                      514 PRECALL                  1
                      518 CALL                     1
                      528 STORE_FAST               6 (model)
          
-         136     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
+         145     >>  530 LOAD_GLOBAL             17 (NULL + get_kwargs)
                      542 LOAD_FAST                0 (parser)
                      544 LOAD_FAST                2 (tokens)
                      546 LOAD_FAST                5 (adapter)
                      548 LOAD_ATTR                9 (required_kwargs)
                      558 PRECALL                  3
                      562 CALL                     3
                      572 STORE_FAST               9 (kwargs)
          
-         138         574 LOAD_GLOBAL             21 (NULL + AdapterNode)
+         147         574 LOAD_GLOBAL             21 (NULL + AdapterNode)
                      586 LOAD_CONST              11 (())
          
-         139         588 LOAD_FAST                5 (adapter)
+         148         588 LOAD_FAST                5 (adapter)
          
-         140         590 LOAD_FAST                6 (model)
+         149         590 LOAD_FAST                6 (model)
          
-         141         592 LOAD_FAST                7 (model_tokens)
+         150         592 LOAD_FAST                7 (model_tokens)
          
-         138         594 LOAD_CONST              10 (('adapter', 'model', 'getters'))
+         147         594 LOAD_CONST              10 (('adapter', 'model', 'getters'))
                      596 BUILD_CONST_KEY_MAP      3
          
-         142         598 LOAD_FAST                9 (kwargs)
+         151         598 LOAD_FAST                9 (kwargs)
          
-         138         600 DICT_MERGE               1
+         147         600 DICT_MERGE               1
                      602 CALL_FUNCTION_EX         1
                      604 RETURN_VALUE
          ExceptionTable:
            128 to 152 -> 156 [0]
            156 to 214 -> 216 [1] lasti
          consts
             None
@@ -859,207 +896,213 @@
             1
             ('adapter', 'model', 'getters')
             ()
          names      ('split_contents', 'pop', 'adapter_registry', 'RegistryLookUpError', 'TemplateSyntaxError', 'split', 'len', 'compile_filter', 'get_kwargs', 'required_kwargs', 'AdapterNode')
          varnames   ('parser', 'token', 'tokens', '_', 'adapter_id', 'adapter', 'model', 'model_tokens', 'model__field', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit'
-         firstlineno 107
+         firstlineno 116
          lnotab
             0x020328022a012a0202011e01120126ff08030a0104012a012a02260118
             010c0102ff1004260350022c020e010201020102fd040402fc
       'request'
       'adapter'
       'context'
       'return'
       code
          argcount  : 3
          nlocals   : 8
          stacksize : 13
          flags     : 3
          code
             0x870097007c02730269007d027c016a0000000000000000007c0264013c
-            0000007c016a0100000000000000007c0264023c0000007c01a002000000
-            00000000000000000000000000000000007c02a6010000ab010000000000
-            0000007d037c01a0030000000000000000000000000000000000000000a6
-            000000ab0000000000000000007d04740900000000000000000000a60000
-            00ab00000000000000000067017d05740b000000000000000000006a0600
-            00000000000000740e00000000000000000000a6010000ab010000000000
-            00000044005d0f7d0602007c067c057c01ac03a6020000ab020000000000
-            00000001008c1088006601640484087c054400a6000000ab000000000000
-            0000007d0574110000000000000000000074130000000000000000000064
-            007c05a6020000ab020000000000000000a6010000ab0100000000000000
-            007d057c016a0a00000000000000007c016a0000000000000000007c016a
-            0100000000000000006a0b00000000000000006a0c00000000000000007c
-            016a0100000000000000006a0b00000000000000006a0d00000000000000
-            007c016a0100000000000000006a0e000000000000000064059c057d0774
-            1f0000000000000000000064067c016a0a00000000000000007c037c017c
-            057c047c016a10000000000000000074230000000000000000000064077c
-            07ac08a6020000ab02000000000000000064099c078900ac0aa6030000ab
-            0300000000000000005300
+            0000007c016a0100000000000000007c0264023c00000089007c0264033c
+            0000007c01a00200000000000000000000000000000000000000007c02a6
+            010000ab0100000000000000007d037c01a0030000000000000000000000
+            000000000000000000a6000000ab0000000000000000007d047409000000
+            00000000000000a6000000ab00000000000000000067017d05740b000000
+            000000000000006a060000000000000000740e00000000000000000000a6
+            010000ab01000000000000000044005d0f7d0602007c067c057c01ac04a6
+            020000ab02000000000000000001008c1088006601640584087c054400a6
+            000000ab0000000000000000007d05741100000000000000000000741300
+            00000000000000000064007c05a6020000ab020000000000000000a60100
+            00ab0100000000000000007d057c016a0a00000000000000007c016a0000
+            000000000000007c016a0100000000000000006a0b00000000000000006a
+            0c00000000000000007c016a0100000000000000006a0b00000000000000
+            006a0d00000000000000007c016a0100000000000000006a0e0000000000
+            00000064069c057d07741f0000000000000000000064077c016a0a000000
+            00000000007c037c017c057c047c016a1000000000000000007423000000
+            0000000000000064087c07ac09a6020000ab020000000000000000640a9c
+            078900ac0ba6030000ab0300000000000000005300
                        0 MAKE_CELL                0 (request)
          
-         146           2 RESUME                   0
+         155           2 RESUME                   0
          
-         147           4 LOAD_FAST                2 (context)
+         156           4 LOAD_FAST                2 (context)
                        6 POP_JUMP_FORWARD_IF_TRUE     2 (to 12)
          
-         148           8 BUILD_MAP                0
+         157           8 BUILD_MAP                0
                       10 STORE_FAST               2 (context)
          
-         150     >>   12 LOAD_FAST                1 (adapter)
+         159     >>   12 LOAD_FAST                1 (adapter)
                       14 LOAD_ATTR                0 (field_name)
                       24 LOAD_FAST                2 (context)
                       26 LOAD_CONST               1 ('wagtail_fedit_field')
                       28 STORE_SUBSCR
          
-         151          32 LOAD_FAST                1 (adapter)
+         160          32 LOAD_FAST                1 (adapter)
                       34 LOAD_ATTR                1 (object)
                       44 LOAD_FAST                2 (context)
                       46 LOAD_CONST               2 ('wagtail_fedit_instance')
                       48 STORE_SUBSCR
          
-         153          52 LOAD_FAST                1 (adapter)
-                      54 LOAD_METHOD              2 (render_content)
-                      76 LOAD_FAST                2 (context)
-                      78 PRECALL                  1
-                      82 CALL                     1
-                      92 STORE_FAST               3 (content)
-         
-         154          94 LOAD_FAST                1 (adapter)
-                      96 LOAD_METHOD              3 (encode_shared_context)
-                     118 PRECALL                  0
-                     122 CALL                     0
-                     132 STORE_FAST               4 (shared)
-         
-         157         134 LOAD_GLOBAL              9 (NULL + FeditAdapterEditButton)
-                     146 PRECALL                  0
-                     150 CALL                     0
-         
-         156         160 BUILD_LIST               1
-                     162 STORE_FAST               5 (items)
-         
-         160         164 LOAD_GLOBAL             11 (NULL + hooks)
-                     176 LOAD_ATTR                6 (get_hooks)
-                     186 LOAD_GLOBAL             14 (CONSTRUCT_ADAPTER_TOOLBAR)
-                     198 PRECALL                  1
-                     202 CALL                     1
-                     212 GET_ITER
-                 >>  214 FOR_ITER                15 (to 246)
-                     216 STORE_FAST               6 (hook)
-         
-         161         218 PUSH_NULL
-                     220 LOAD_FAST                6 (hook)
-                     222 LOAD_FAST                5 (items)
-                     224 LOAD_FAST                1 (adapter)
-                     226 KW_NAMES                 3
-                     228 PRECALL                  2
-                     232 CALL                     2
-                     242 POP_TOP
-                     244 JUMP_BACKWARD           16 (to 214)
-         
-         163     >>  246 LOAD_CLOSURE             0 (request)
-                     248 BUILD_TUPLE              1
-                     250 LOAD_CONST               4 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 163>)
-                     252 MAKE_FUNCTION            8 (closure)
-                     254 LOAD_FAST                5 (items)
-                     256 GET_ITER
-                     258 PRECALL                  0
-                     262 CALL                     0
-                     272 STORE_FAST               5 (items)
-         
-         164         274 LOAD_GLOBAL             17 (NULL + list)
-                     286 LOAD_GLOBAL             19 (NULL + filter)
-                     298 LOAD_CONST               0 (None)
-                     300 LOAD_FAST                5 (items)
-                     302 PRECALL                  2
-                     306 CALL                     2
-                     316 PRECALL                  1
-                     320 CALL                     1
-                     330 STORE_FAST               5 (items)
+         161          52 LOAD_DEREF               0 (request)
+                      54 LOAD_FAST                2 (context)
+                      56 LOAD_CONST               3 ('request')
+                      58 STORE_SUBSCR
+         
+         163          62 LOAD_FAST                1 (adapter)
+                      64 LOAD_METHOD              2 (render_content)
+                      86 LOAD_FAST                2 (context)
+                      88 PRECALL                  1
+                      92 CALL                     1
+                     102 STORE_FAST               3 (content)
+         
+         164         104 LOAD_FAST                1 (adapter)
+                     106 LOAD_METHOD              3 (encode_shared_context)
+                     128 PRECALL                  0
+                     132 CALL                     0
+                     142 STORE_FAST               4 (shared)
+         
+         167         144 LOAD_GLOBAL              9 (NULL + FeditAdapterEditButton)
+                     156 PRECALL                  0
+                     160 CALL                     0
+         
+         166         170 BUILD_LIST               1
+                     172 STORE_FAST               5 (items)
+         
+         170         174 LOAD_GLOBAL             11 (NULL + hooks)
+                     186 LOAD_ATTR                6 (get_hooks)
+                     196 LOAD_GLOBAL             14 (CONSTRUCT_ADAPTER_TOOLBAR)
+                     208 PRECALL                  1
+                     212 CALL                     1
+                     222 GET_ITER
+                 >>  224 FOR_ITER                15 (to 256)
+                     226 STORE_FAST               6 (hook)
+         
+         171         228 PUSH_NULL
+                     230 LOAD_FAST                6 (hook)
+                     232 LOAD_FAST                5 (items)
+                     234 LOAD_FAST                1 (adapter)
+                     236 KW_NAMES                 4
+                     238 PRECALL                  2
+                     242 CALL                     2
+                     252 POP_TOP
+                     254 JUMP_BACKWARD           16 (to 224)
+         
+         173     >>  256 LOAD_CLOSURE             0 (request)
+                     258 BUILD_TUPLE              1
+                     260 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Packages\wagtail_fedit\wagtail_fedit\templatetags\fedit.py", line 173>)
+                     262 MAKE_FUNCTION            8 (closure)
+                     264 LOAD_FAST                5 (items)
+                     266 GET_ITER
+                     268 PRECALL                  0
+                     272 CALL                     0
+                     282 STORE_FAST               5 (items)
+         
+         174         284 LOAD_GLOBAL             17 (NULL + list)
+                     296 LOAD_GLOBAL             19 (NULL + filter)
+                     308 LOAD_CONST               0 (None)
+                     310 LOAD_FAST                5 (items)
+                     312 PRECALL                  2
+                     316 CALL                     2
+                     326 PRECALL                  1
+                     330 CALL                     1
+                     340 STORE_FAST               5 (items)
          
-         167         332 LOAD_FAST                1 (adapter)
-                     334 LOAD_ATTR               10 (identifier)
+         177         342 LOAD_FAST                1 (adapter)
+                     344 LOAD_ATTR               10 (identifier)
          
-         168         344 LOAD_FAST                1 (adapter)
-                     346 LOAD_ATTR                0 (field_name)
+         178         354 LOAD_FAST                1 (adapter)
+                     356 LOAD_ATTR                0 (field_name)
          
-         169         356 LOAD_FAST                1 (adapter)
-                     358 LOAD_ATTR                1 (object)
-                     368 LOAD_ATTR               11 (_meta)
-                     378 LOAD_ATTR               12 (app_label)
+         179         366 LOAD_FAST                1 (adapter)
+                     368 LOAD_ATTR                1 (object)
+                     378 LOAD_ATTR               11 (_meta)
+                     388 LOAD_ATTR               12 (app_label)
          
-         170         388 LOAD_FAST                1 (adapter)
-                     390 LOAD_ATTR                1 (object)
-                     400 LOAD_ATTR               11 (_meta)
-                     410 LOAD_ATTR               13 (model_name)
+         180         398 LOAD_FAST                1 (adapter)
+                     400 LOAD_ATTR                1 (object)
+                     410 LOAD_ATTR               11 (_meta)
+                     420 LOAD_ATTR               13 (model_name)
          
-         171         420 LOAD_FAST                1 (adapter)
-                     422 LOAD_ATTR                1 (object)
-                     432 LOAD_ATTR               14 (pk)
+         181         430 LOAD_FAST                1 (adapter)
+                     432 LOAD_ATTR                1 (object)
+                     442 LOAD_ATTR               14 (pk)
          
-         166         442 LOAD_CONST               5 (('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id'))
-                     444 BUILD_CONST_KEY_MAP      5
-                     446 STORE_FAST               7 (reverse_kwargs)
+         176         452 LOAD_CONST               6 (('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id'))
+                     454 BUILD_CONST_KEY_MAP      5
+                     456 STORE_FAST               7 (reverse_kwargs)
          
-         174         448 LOAD_GLOBAL             31 (NULL + render_to_string)
+         184         458 LOAD_GLOBAL             31 (NULL + render_to_string)
          
-         175         460 LOAD_CONST               6 ('wagtail_fedit/content/editable_adapter.html')
+         185         470 LOAD_CONST               7 ('wagtail_fedit/content/editable_adapter.html')
          
-         177         462 LOAD_FAST                1 (adapter)
-                     464 LOAD_ATTR               10 (identifier)
+         187         472 LOAD_FAST                1 (adapter)
+                     474 LOAD_ATTR               10 (identifier)
          
-         178         474 LOAD_FAST                3 (content)
+         188         484 LOAD_FAST                3 (content)
          
-         179         476 LOAD_FAST                1 (adapter)
+         189         486 LOAD_FAST                1 (adapter)
          
-         180         478 LOAD_FAST                5 (items)
+         190         488 LOAD_FAST                5 (items)
          
-         181         480 LOAD_FAST                4 (shared)
+         191         490 LOAD_FAST                4 (shared)
          
-         182         482 LOAD_FAST                1 (adapter)
-                     484 LOAD_ATTR               16 (kwargs)
+         192         492 LOAD_FAST                1 (adapter)
+                     494 LOAD_ATTR               16 (kwargs)
          
-         183         494 LOAD_GLOBAL             35 (NULL + reverse)
+         193         504 LOAD_GLOBAL             35 (NULL + reverse)
          
-         184         506 LOAD_CONST               7 ('wagtail_fedit:edit')
+         194         516 LOAD_CONST               8 ('wagtail_fedit:edit')
          
-         185         508 LOAD_FAST                7 (reverse_kwargs)
+         195         518 LOAD_FAST                7 (reverse_kwargs)
          
-         183         510 KW_NAMES                 8
-                     512 PRECALL                  2
-                     516 CALL                     2
+         193         520 KW_NAMES                 9
+                     522 PRECALL                  2
+                     526 CALL                     2
          
-         176         526 LOAD_CONST               9 (('identifier', 'content', 'adapter', 'buttons', 'shared', 'shared_context', 'edit_url'))
-                     528 BUILD_CONST_KEY_MAP      7
+         186         536 LOAD_CONST              10 (('identifier', 'content', 'adapter', 'buttons', 'shared', 'shared_context', 'edit_url'))
+                     538 BUILD_CONST_KEY_MAP      7
          
-         188         530 LOAD_DEREF               0 (request)
+         198         540 LOAD_DEREF               0 (request)
          
-         174         532 KW_NAMES                10
-                     534 PRECALL                  3
-                     538 CALL                     3
-                     548 RETURN_VALUE
+         184         542 KW_NAMES                11
+                     544 PRECALL                  3
+                     548 CALL                     3
+                     558 RETURN_VALUE
          consts
             None
             'wagtail_fedit_field'
             'wagtail_fedit_instance'
+            'request'
             ('items', 'adapter')
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               163           2 RESUME                   0
+               173           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -1069,35 +1112,35 @@
                             54 JUMP_BACKWARD           24 (to 8)
                        >>   56 RETURN_VALUE
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
-               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+               filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 163
+               firstlineno 173
                lnotab 0x
             ('adapter_id', 'field_name', 'app_label', 'model_name', 'model_id')
             'wagtail_fedit/content/editable_adapter.html'
             'wagtail_fedit:edit'
             ('kwargs',)
             ('identifier', 'content', 'adapter', 'buttons', 'shared', 'shared_context', 'edit_url')
             ('request',)
          names      ('field_name', 'object', 'render_content', 'encode_shared_context', 'FeditAdapterEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_ADAPTER_TOOLBAR', 'list', 'filter', 'identifier', '_meta', 'app_label', 'model_name', 'pk', 'render_to_string', 'kwargs', 'reverse')
          varnames   ('request', 'adapter', 'context', 'content', 'shared', 'items', 'hook', 'reverse_kwargs')
          freevars   ()
          cellvars   ('request',)
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'wrap_adapter'
-         firstlineno 146
+         firstlineno 155
          lnotab
-            0x040104010402140114022a0128031aff040436011c021c013a030c010c
-            012001200116fb06080c0102020c0102010201020102010c010c01020102
-            fe10f9040c02f2
+            0x040104010402140114010a022a0128031aff040436011c021c013a030c
+            010c012001200116fb06080c0102020c0102010201020102010c010c0102
+            0102fe10f9040c02f2
       'tokens'
       'kwarg_list'
       code
          argcount  : 3
          nlocals   : 10
          stacksize : 5
          flags     : 3
@@ -1112,147 +1155,147 @@
             017c00a00400000000000000000000000000000000000000007c06a60100
             00ab0100000000000000007c047c027c05190000000000000000003c0000
             008c707c076405190000000000000000007d087c00a00400000000000000
             000000000000000000000000007c07640319000000000000000000a60100
             00ab0100000000000000007c047c083c00000064067d038c997c0244005d
             187d097c097c0476017212740b0000000000000000000064077c099b009d
             02a6010000ab01000000000000000082018c197c045300
-         192           0 RESUME                   0
+         202           0 RESUME                   0
          
-         193           2 LOAD_CONST               1 (False)
+         203           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         194           6 BUILD_MAP                0
+         204           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         196          10 LOAD_FAST                2 (kwarg_list)
+         206          10 LOAD_FAST                2 (kwarg_list)
                       12 POP_JUMP_FORWARD_IF_TRUE     2 (to 18)
          
-         197          14 BUILD_LIST               0
+         207          14 BUILD_LIST               0
                       16 STORE_FAST               2 (kwarg_list)
          
-         199     >>   18 LOAD_GLOBAL              1 (NULL + enumerate)
+         209     >>   18 LOAD_GLOBAL              1 (NULL + enumerate)
                       30 LOAD_FAST                1 (tokens)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 GET_ITER
                  >>   48 FOR_ITER               152 (to 354)
                       50 UNPACK_SEQUENCE          2
                       54 STORE_FAST               5 (i)
                       56 STORE_FAST               6 (token)
          
-         200          58 LOAD_FAST                6 (token)
+         210          58 LOAD_FAST                6 (token)
                       60 LOAD_METHOD              1 (split)
                       82 LOAD_CONST               2 ('=')
                       84 PRECALL                  1
                       88 CALL                     1
                       98 STORE_FAST               7 (split)
          
-         201         100 LOAD_GLOBAL              5 (NULL + len)
+         211         100 LOAD_GLOBAL              5 (NULL + len)
                      112 LOAD_FAST                7 (split)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 LOAD_CONST               3 (1)
                      130 COMPARE_OP               2 (==)
                      136 POP_JUMP_FORWARD_IF_FALSE    67 (to 272)
                      138 LOAD_GLOBAL              5 (NULL + len)
                      150 LOAD_FAST                2 (kwarg_list)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 LOAD_FAST                5 (i)
                      168 COMPARE_OP               4 (>)
                      174 POP_JUMP_FORWARD_IF_FALSE    48 (to 272)
          
-         202         176 LOAD_FAST                3 (had_kwargs)
+         212         176 LOAD_FAST                3 (had_kwargs)
                      178 POP_JUMP_FORWARD_IF_FALSE    15 (to 210)
          
-         203         180 LOAD_GLOBAL              7 (NULL + ValueError)
+         213         180 LOAD_GLOBAL              7 (NULL + ValueError)
                      192 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RAISE_VARARGS            1
          
-         205     >>  210 LOAD_FAST                0 (parser)
+         215     >>  210 LOAD_FAST                0 (parser)
                      212 LOAD_METHOD              4 (compile_filter)
                      234 LOAD_FAST                6 (token)
                      236 PRECALL                  1
                      240 CALL                     1
                      250 LOAD_FAST                4 (kwargs)
                      252 LOAD_FAST                2 (kwarg_list)
                      254 LOAD_FAST                5 (i)
                      256 BINARY_SUBSCR
                      266 STORE_SUBSCR
                      270 JUMP_BACKWARD          112 (to 48)
          
-         207     >>  272 LOAD_FAST                7 (split)
+         217     >>  272 LOAD_FAST                7 (split)
                      274 LOAD_CONST               5 (0)
                      276 BINARY_SUBSCR
                      286 STORE_FAST               8 (key)
          
-         211         288 LOAD_FAST                0 (parser)
+         221         288 LOAD_FAST                0 (parser)
                      290 LOAD_METHOD              4 (compile_filter)
                      312 LOAD_FAST                7 (split)
                      314 LOAD_CONST               3 (1)
                      316 BINARY_SUBSCR
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST                4 (kwargs)
                      342 LOAD_FAST                8 (key)
                      344 STORE_SUBSCR
          
-         212         348 LOAD_CONST               6 (True)
+         222         348 LOAD_CONST               6 (True)
                      350 STORE_FAST               3 (had_kwargs)
                      352 JUMP_BACKWARD          153 (to 48)
          
-         214     >>  354 LOAD_FAST                2 (kwarg_list)
+         224     >>  354 LOAD_FAST                2 (kwarg_list)
                      356 GET_ITER
                  >>  358 FOR_ITER                24 (to 408)
                      360 STORE_FAST               9 (kwarg)
          
-         215         362 LOAD_FAST                9 (kwarg)
+         225         362 LOAD_FAST                9 (kwarg)
                      364 LOAD_FAST                4 (kwargs)
                      366 CONTAINS_OP              1
                      368 POP_JUMP_FORWARD_IF_FALSE    18 (to 406)
          
-         216         370 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
+         226         370 LOAD_GLOBAL             11 (NULL + TemplateSyntaxError)
                      382 LOAD_CONST               7 ('Missing required keyword argument ')
                      384 LOAD_FAST                9 (kwarg)
                      386 FORMAT_VALUE             0
                      388 BUILD_STRING             2
                      390 PRECALL                  1
                      394 CALL                     1
                      404 RAISE_VARARGS            1
          
-         215     >>  406 JUMP_BACKWARD           25 (to 358)
+         225     >>  406 JUMP_BACKWARD           25 (to 358)
          
-         218     >>  408 LOAD_FAST                4 (kwargs)
+         228     >>  408 LOAD_FAST                4 (kwargs)
                      410 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
             0
             True
             'Missing required keyword argument '
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter', 'TemplateSyntaxError')
          varnames   ('parser', 'tokens', 'kwarg_list', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key', 'kwarg')
          freevars   ()
          cellvars   ()
-         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+         filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 192
+         firstlineno 202
          lnotab
             0x0201040104020401040228012a014c0104011e023e0210043c01060208
             01080124ff0203
       (None,)
-   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'NodeList', 'TemplateSyntaxError', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditAdapterEditButton', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'utils', '_can_edit', 'edit_url', 'CONSTRUCT_ADAPTER_TOOLBAR', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'dict', 'str', 'wrap_adapter', 'list', 'get_kwargs')
+   names      ('typing', 'Type', 'django.template', 'library', 'Node', 'TemplateSyntaxError', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'FilterExpression', 'django.http', 'HttpRequest', 'django.urls', 'reverse', 'django.core', 'signing', 'wagtail', 'hooks', 'warnings', 'toolbar', 'FeditAdapterEditButton', 'adapters', 'adapter_registry', 'RegistryLookUpError', 'BaseAdapter', 'AdapterError', 'utils', '_can_edit', 'CONSTRUCT_ADAPTER_TOOLBAR', 'Library', 'register', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'AdapterNode', 'tag', 'do_render_fedit', 'dict', 'str', 'wrap_adapter', 'list', 'get_kwargs')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
+   filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Packages\\wagtail_fedit\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c0118010c0110010c010c010c010c010c010c020c010c010c
-      0208021004140510040c051e03040104041c3f2a010eff0e010226182e
+      0x00ff02010c0114010c0110010c010c010c010c020c0208020c0318060c
+      030c051e03040104041c4d2a010eff0e010226182f
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.9/wagtail_fedit/templatetags/fedit.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,16 @@
                 warnings.warn(
                     WARNING_MODEL_INSTANCE_NOT_AVAILABLE % {
                         "object": self.adapter.__name__,
                     },
                     RuntimeWarning,
                 )
 
+                context = context.flatten()
+
                 try:
                     return self.adapter.render_from_kwargs(
                         context, **kwargs,
                     )
                 except AdapterError as e:
                     raise TemplateSyntaxError(str(e))
 
@@ -152,14 +154,15 @@
 
 def wrap_adapter(request: HttpRequest, adapter: BaseAdapter, context: dict) -> str:
     if not context:
         context = {}
 
     context["wagtail_fedit_field"] = adapter.field_name
     context["wagtail_fedit_instance"] = adapter.object
+    context["request"] = request
 
     content = adapter.render_content(context)
     shared = adapter.encode_shared_context()
 
     items = [
         FeditAdapterEditButton(),
     ]
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,121 @@
-from django.db.models.base import Model as Model
-from django.http import HttpRequest
-from django.template import (
-    Context, Template,
-    TemplateSyntaxError,
-)
-from wagtail_fedit.adapters import (
-    BaseAdapter,
-    adapter_registry,
-    BlockAdapter,
-    FieldAdapter,
+from wagtail.models import (
+    RevisionMixin,
 )
 from wagtail_fedit.utils import (
-    FEDIT_PREVIEW_VAR,
-)
-from wagtail_fedit.templatetags.fedit import (
-    wrap_adapter,
+    find_block,
 )
 from .base import (
     BaseFEditTest,
 )
 
 import json
 
-adapters = {}
-
-class TestAdapter(BaseAdapter):
-    identifier = "test"
-    required_kwargs = ["test"]
-
-    def __init__(self, object: Model, field_name: str, request: HttpRequest, **kwargs):
-        super().__init__(object, field_name, request, **kwargs)
-        adapters[self.kwargs["id"]] = self
-
-    def render_content(self, parent_context: dict = None) -> str:
-        return f"TestAdapter: {self.field_value}"
-
-
-adapter_registry.register(TestAdapter)
-
-
-class TestBaseAdapter(BaseFEditTest):
-
-    def test_required_kwargs_ok(self):
-        self.assertEqual(TestAdapter.required_kwargs, ["test"])
+class TestBlockEdit(BaseFEditTest):
+    def test_block_edited(self):
 
-        template_ok = Template(
-            "{% load fedit %}"
-            "{% fedit test object.title test='test' id=1 %}"
-        )
-
-        request = self.request_factory.get(
-            self.get_editable_url(
-                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+        self.client.force_login(self.admin_user)
+        
+        for i, model in enumerate(self.models):
+            
+            if isinstance(model, RevisionMixin):
+                self.assertEqual(model.revisions.count(), 0)
+            else:
+                with self.assertRaises(AttributeError):
+                    model.revisions.count()
+
+            bound, _ = find_block(block_id=self.BLOCK_ID, field=model.content)
+            initial_content = bound.value["link"]["text"]
+
+            response = self.client.post(
+                self.get_block_url(
+                    self.BLOCK_ID,
+                    "content",
+                    model._meta.app_label,
+                    model._meta.model_name,
+                    model.pk,
+                ),
+                {
+                    "value-link-text": f"{initial_content} test case {i + 1}"
+                }
             )
-        )
-        request.user = self.admin_user
 
-        template_ok = template_ok.render(
-            Context({
-                "request": request,
-                "object": self.basic_model,
-            })
-        )
+            self.assertEqual(response.status_code, 200)
+            model.refresh_from_db()
 
-        self.assertHTMLEqual(
-            template_ok,
-            f'TestAdapter: {self.basic_model.title}'
-        )
-
-        self.assertDictEqual(
-            adapters[1].kwargs,
-            {"test": "test", "id": 1}
-        )
-
-    def test_required_kwargs_fail(self):
-        request = self.request_factory.get(
-            self.get_editable_url(
-                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            if isinstance(model, RevisionMixin):
+                self.assertEqual(model.revisions.count(), 1)
+                chk = model.latest_revision.as_object()
+            else:
+                with self.assertRaises(AttributeError):
+                    model.revisions.count()
+                chk = model
+
+            bound, contentpath = find_block(block_id=self.BLOCK_ID, field=chk.content)
+            self.assertEqual(bound.value["link"]["text"], f"{initial_content} test case {i + 1}",
+                msg=f"Block: {bound.block} does not contain the expected value: {initial_content} test case {i + 1}"
             )
-        )
-        request.user = self.admin_user
 
-        try:
-            template_fail = Template(
-                "{% load fedit %}"
-                "{% fedit test object.title id=2 %}"
-            )
-
-            # self.fail(f"Expected exception: {e}")
-            template_fail.render(Context({
-                "request": request,
-                "object": self.basic_model,
-            }))
-
-        except TemplateSyntaxError as e:
-            self.assertEqual(
-                str(e),
-                "Missing required keyword argument test"
+    def test_unauthorized_unchanged(self):
+        self.client.force_login(self.regular_user)
+        
+        for i, model in enumerate(self.models):
+            
+            initial_content = model.content
+            response = self.client.post(
+                self.get_field_url(
+                    "content",
+                    model._meta.app_label,
+                    model._meta.model_name,
+                    model.pk,
+                ),
+                {
+                    "content": f"{model.content} test case {i + 1}"
+                }
             )
 
-        except Exception as e:
-            self.fail(f"Unexpected exception: {e} ({type(e)})")
+            self.assertEqual(response.status_code, 403, msg=f"Expected 403, got {response.status_code} ({response.content})")
 
-        else:
-            self.fail("Expected exception not raised")
+            model.refresh_from_db()
 
-    def test_adapter_render_content(self):
-        adapter = TestAdapter(
-            self.basic_model,
-            "title",
-            self.request_factory.get(
-                self.get_editable_url(
-                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
-                )
+            if isinstance(model, RevisionMixin):
+                self.assertEqual(model.revisions.count(), 0)
+                chk = model
+
+            else:
+                with self.assertRaises(AttributeError):
+                    model.revisions.count()
+                chk = model
+
+            self.assertEqual(chk.content.get_prep_value(), initial_content.get_prep_value())
+
+    def test_lock_unchanged(self):
+        self.client.force_login(self.other_admin_user)
+        initial_content = self.lock_model.content
+        initial_bound, _ = find_block(block_id=self.BLOCK_ID, field=self.lock_model.content)
+
+        response = self.client.post(
+            self.get_block_url(
+                self.BLOCK_ID,
+                "content",
+                self.lock_model._meta.app_label,
+                self.lock_model._meta.model_name,
+                self.lock_model.pk,
             ),
-            id=3,
-        )
-
-        self.assertEqual(
-            adapter.render_content(),
-            f"TestAdapter: {self.basic_model.title}"
-        )
-
-    def test_adapter_editable(self):
-        self.assertEqual(TestAdapter.required_kwargs, ["test"])
-
-        tpl = Template(
-            "{% load fedit %}"
-            "{% fedit test object.title test='test' id=4 %}"
-        )
-
-        request = self.request_factory.get(
-            self.get_editable_url(
-                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
-            )
-        )
-        request.user = self.admin_user
-
-        setattr(
-            request,
-            FEDIT_PREVIEW_VAR,
-            True,
-        )
-
-        tpl = tpl.render(
-            Context({
-                "request": request,
-                "object": self.basic_model,
-            })
-        )
-
-        self.assertHTMLEqual(
-            tpl,
-            wrap_adapter(request, adapters[4], {})
+            {
+                "value-link-text": f"{initial_bound.value['link']['text']} test case"
+            }
         )
 
+        self.lock_model.refresh_from_db()
 
+        self.assertEqual(response.status_code, 423) # 423 Locked
+        self.assertEqual(self.lock_model.revisions.count(), 0)
+        
+        try:
+            response_content = (json.loads(response.content) or {})
+        except json.JSONDecodeError:
+            self.fail("Response content is not valid JSON")
+            
+        self.assertTrue(response_content.get("locked", False))
+        self.assertEqual(self.lock_model.locked_by, self.admin_user)
+        self.assertEqual(self.lock_model.content.get_prep_value(), initial_content.get_prep_value())
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,70 @@
 from wagtail.models import (
     RevisionMixin,
 )
-from wagtail_fedit.utils import (
-    find_block,
-)
 from .base import (
     BaseFEditTest,
 )
 
 import json
 
-class TestBlockEdit(BaseFEditTest):
-    def test_block_edited(self):
-
+class TestFieldEdit(BaseFEditTest):
+    def test_field_edited(self):
         self.client.force_login(self.admin_user)
         
         for i, model in enumerate(self.models):
             
             if isinstance(model, RevisionMixin):
                 self.assertEqual(model.revisions.count(), 0)
             else:
                 with self.assertRaises(AttributeError):
                     model.revisions.count()
 
-            bound, _ = find_block(block_id=self.BLOCK_ID, field=model.content)
-            initial_content = bound.value["link"]["text"]
+            initial_title = model.title
 
-            response = self.client.post(
-                self.get_block_url(
-                    self.BLOCK_ID,
-                    "content",
+            self.client.post(
+                self.get_field_url(
+                    "title",
                     model._meta.app_label,
                     model._meta.model_name,
                     model.pk,
                 ),
                 {
-                    "value-link-text": f"{initial_content} test case {i + 1}"
+                    "title": f"{model.title} test case {i + 1}"
                 }
             )
 
-            self.assertEqual(response.status_code, 200)
             model.refresh_from_db()
 
             if isinstance(model, RevisionMixin):
                 self.assertEqual(model.revisions.count(), 1)
+                self.assertEqual(model.title, initial_title)
                 chk = model.latest_revision.as_object()
             else:
                 with self.assertRaises(AttributeError):
                     model.revisions.count()
                 chk = model
 
-            bound, contentpath = find_block(block_id=self.BLOCK_ID, field=chk.content)
-            self.assertEqual(bound.value["link"]["text"], f"{initial_content} test case {i + 1}",
-                msg=f"Block: {bound.block} does not contain the expected value: {initial_content} test case {i + 1}"
-            )
+            self.assertEqual(chk.title, f"{initial_title} test case {i + 1}")
 
     def test_unauthorized_unchanged(self):
         self.client.force_login(self.regular_user)
         
         for i, model in enumerate(self.models):
             
-            initial_content = model.content
+            initial_title = model.title
             response = self.client.post(
                 self.get_field_url(
-                    "content",
+                    "title",
                     model._meta.app_label,
                     model._meta.model_name,
                     model.pk,
                 ),
                 {
-                    "content": f"{model.content} test case {i + 1}"
+                    "title": f"{model.title} test case {i + 1}"
                 }
             )
 
             self.assertEqual(response.status_code, 403, msg=f"Expected 403, got {response.status_code} ({response.content})")
 
             model.refresh_from_db()
 
@@ -82,31 +73,30 @@
                 chk = model
 
             else:
                 with self.assertRaises(AttributeError):
                     model.revisions.count()
                 chk = model
 
-            self.assertEqual(chk.content.get_prep_value(), initial_content.get_prep_value())
+            self.assertEqual(chk.title, initial_title)
+
 
     def test_lock_unchanged(self):
         self.client.force_login(self.other_admin_user)
-        initial_content = self.lock_model.content
-        initial_bound, _ = find_block(block_id=self.BLOCK_ID, field=self.lock_model.content)
+        initial_content = self.lock_model.title
 
         response = self.client.post(
-            self.get_block_url(
-                self.BLOCK_ID,
-                "content",
+            self.get_field_url(
+                "title",
                 self.lock_model._meta.app_label,
                 self.lock_model._meta.model_name,
                 self.lock_model.pk,
             ),
             {
-                "value-link-text": f"{initial_bound.value['link']['text']} test case"
+                "title": f"{self.lock_model.title} test case"
             }
         )
 
         self.lock_model.refresh_from_db()
 
         self.assertEqual(response.status_code, 423) # 423 Locked
         self.assertEqual(self.lock_model.revisions.count(), 0)
@@ -114,8 +104,10 @@
         try:
             response_content = (json.loads(response.content) or {})
         except json.JSONDecodeError:
             self.fail("Response content is not valid JSON")
             
         self.assertTrue(response_content.get("locked", False))
         self.assertEqual(self.lock_model.locked_by, self.admin_user)
-        self.assertEqual(self.lock_model.content.get_prep_value(), initial_content.get_prep_value())
+        self.assertEqual(self.lock_model.title, initial_content)
+        
+
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.9/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.9/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.9/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.9/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.4.9/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.9/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.9/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.9/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.9/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.4.8rc0
+Version: 1.4.9
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
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.8rc0 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.9 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
```

### Comparing `wagtail_fedit-1.4.8rc0/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.9/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

