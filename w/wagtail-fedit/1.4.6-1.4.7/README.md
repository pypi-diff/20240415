# Comparing `tmp/wagtail_fedit-1.4.6.tar.gz` & `tmp/wagtail_fedit-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.6.tar", last modified: Thu Apr 11 11:04:47 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.7.tar", last modified: Mon Apr 15 16:22:54 2024, max compression
```

## Comparing `wagtail_fedit-1.4.6.tar` & `wagtail_fedit-1.4.7.tar`

### file list

```diff
@@ -1,121 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.372470 wagtail_fedit-1.4.6/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0    13152 2024-04-11 11:04:47.373471 wagtail_fedit-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    11954 2024-04-08 20:13:14.000000 wagtail_fedit-1.4.6/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-04-11 11:04:47.382724 wagtail_fedit-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.987100 wagtail_fedit-1.4.6/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.6/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.6/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.036675 wagtail_fedit-1.4.6/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-05 10:46:54.000000 wagtail_fedit-1.4.6/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.6/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     3358 2024-04-10 10:24:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.936096 wagtail_fedit-1.4.6/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.936096 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.060165 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.061303 wagtail_fedit-1.4.6/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.6/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.063316 wagtail_fedit-1.4.6/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.6/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.938096 wagtail_fedit-1.4.6/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.938096 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.072314 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.096592 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    15915 2024-04-06 00:14:04.000000 wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.940097 wagtail_fedit-1.4.6/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:46.941100 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.098590 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.100591 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.109359 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      789 2024-04-07 05:29:57.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.116296 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.121759 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.126389 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.144202 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.148470 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    17687 2024-04-10 19:17:23.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    14619 2024-04-10 19:17:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.151871 wagtail_fedit-1.4.6/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.186778 wagtail_fedit-1.4.6/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.199780 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.262390 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7106 2024-04-10 12:43:12.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     2996 2024-04-10 10:50:37.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_block_templatetag.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3994 2024-04-10 11:08:06.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_templatetag.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.287401 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.4.6/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      951 2024-04-11 08:07:43.000000 wagtail_fedit-1.4.6/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15352 2024-04-10 13:08:18.000000 wagtail_fedit-1.4.6/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.340531 wagtail_fedit-1.4.6/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      188 2024-04-05 18:53:00.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9321 2024-04-11 07:42:21.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0    12413 2024-04-11 07:51:29.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/fields.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.6/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.371464 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      182 2024-04-11 08:26:05.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7068 2024-04-11 11:04:16.000000 wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-11 11:04:47.014620 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    13152 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3976 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 11:04:46.000000 wagtail_fedit-1.4.6/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.307673 wagtail_fedit-1.4.7/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    13123 2024-04-15 16:22:54.307673 wagtail_fedit-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11925 2024-04-15 16:22:37.000000 wagtail_fedit-1.4.7/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2024-04-15 16:22:54.319259 wagtail_fedit-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.026410 wagtail_fedit-1.4.7/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.7/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.078014 wagtail_fedit-1.4.7/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      294 2024-04-13 11:18:53.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     3762 2024-04-13 19:50:56.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     3857 2024-04-15 16:08:58.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     7523 2024-04-13 11:18:27.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.7/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.081415 wagtail_fedit-1.4.7/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.7/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.7/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     3588 2024-04-13 07:17:52.000000 wagtail_fedit-1.4.7/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.982963 wagtail_fedit-1.4.7/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.983961 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.104776 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.105785 wagtail_fedit-1.4.7/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.7/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.107883 wagtail_fedit-1.4.7/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.7/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.987043 wagtail_fedit-1.4.7/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.988042 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.143397 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.168557 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    16161 2024-04-15 15:58:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.989043 wagtail_fedit-1.4.7/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.993231 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.191937 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.203892 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      386 2024-04-13 11:13:58.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+-rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.220775 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.227410 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.245121 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.256895 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.259941 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.262957 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9097 2024-04-14 13:32:19.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6514 2024-04-14 13:32:17.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.264906 wagtail_fedit-1.4.7/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.268274 wagtail_fedit-1.4.7/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.275937 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.283966 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4314 2024-04-14 13:07:00.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.291309 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.4.7/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.4.7/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.4.7/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.294776 wagtail_fedit-1.4.7/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     5960 2024-04-13 19:04:24.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.306664 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.070950 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    13123 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4175 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.6/LICENSE` & `wagtail_fedit-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/PKG-INFO` & `wagtail_fedit-1.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.6
+Version: 1.4.7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -88,19 +88,18 @@
        <title>Document</title>
        <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
    </head>
    <body>
        {# Adress the model.field or model.my.related.field you wish to edit. #}
        {# Editable fields get a special `inline` argument. #}
        {# if True the button is not placed with an absolute CSS position. #}
-       <h1>{% fedit_field self.title inline=True or False %}</h1>
+       <h1>{% fedit field self.title inline=True or False %}</h1>
 
-       {# Pass in the field_name and the model instance on which that field resides if you are using `wagtail_fedit <= 1.3.8` #}
        <main class="my-streamfield-content">
-           {% fedit_field "content" self %}
+           {% fedit field self.content %}
        </main>
 
        {% wagtailuserbar %}
 
        <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
    </body>
    </html>
@@ -116,15 +115,15 @@
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
        {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
        {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
-       {% fedit_block block=block block_id=block.id field_name="content" model=self %}
+       {% fedit block self.content block=block block_id=block.id %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
    ...
@@ -132,17 +131,24 @@
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
-   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
+   Your content will then automatically be rendered with that method when need be by using
+   `{% fedit field self.content %} `
 4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
+**Note:** If the parent block is wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance variable and field name should be omitted and replaced with `from_context`.
+Example: `{% fedit block from_context block=item block_id=item.id %}`
+The parent- blocktag will share these variables through context.
+This makes it possibly to easily use editable sub-blocks across multiple different model types.
+If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
+
 ## Permissions
 
 **Note: This is not required for pages.**
 
 **The `Page` model already provides this interface.**
 
 We have the following basic permission requirements:
@@ -214,23 +220,18 @@
 This is done by accessing the `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for the toplevel block!)*
 
 Our new loop would then be:
 
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
-    {% fedit_block block=item block_id=item.id field_name="content" model=my_model_instance_var %}
+    {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
-**Note:** If the parent block is wrapped with `fedit_block` or `fedit_field` the field_name and model argument can be omitted.
-The parent- blocktag will share these variables through context.
-This makes it possibly to easily use editable sub-blocks across multiple different model types.
-If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
-
 ## Hooks
 
 ### wagtail_fedit.construct_block_toolbar
 
 Construct the toolbar for the given block.
 This is used to display the edit icon in the block.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.6 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.7 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -34,94 +34,92 @@
 Editing! 1. Make sure the models you wish to edit inherit from
 PreviewableMixin. **This is a requirement.** 2. Define a template for your
 model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
 the required template tag libraries #}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {#
 Editable fields get a special `inline` argument. #} {# if True the button is
 not placed with an absolute CSS position. #}
-************ {{%% ffeeddiitt__ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
-{# Pass in the field_name and the model instance on which that field resides if
-you are using `wagtail_fedit <= 1.3.8` #} {% fedit_field "content" self %} {%
-wagtailuserbar %}
+************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
+{% fedit field self.content %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
 do not require the field_name or model argument. #} {# This is taken from the
 parent (also wrapped by `fedit_block`); the model and field name are shared
-through context. #} {% fedit_block block=block block_id=block.id
-field_name="content" model=self %} {% endfor %} ``` ```python from
-django.template.loader import render_to_string ... class MyPage(...): # Can be
-any type of model. content = StreamField(...) def render_fedit_content(self,
-request): return render_to_string("myapp/render_my_field.html",
-self.get_context(request)) ``` Your content will then automatically be rendered
-with that method when need be by using `{% fedit_field "content" self %} ` 4.
-**But wait?! I go to my template and I do not see a way to edit!**That is true!
-We try to protect any styling on your actual page; we do not want to
-interfere.Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
-on that userbar! It is also used for publishing if your model inherits from
-`DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
-**The `Page` model already provides this interface.** We have the following
-basic permission requirements: * You must have `wagtailadmin.access_admin` to
-edit a block/field. * You must have the appropriate `app_label.change_*`
-permission for the model. This however only applies to editing. We use separate
-permissions for publishing and submitting workflows, etc. Models which you want
-to allow the publish view for should also implement a `PermissionTester`- like
-object. Example of how you should implement the `Tester` object and all
-required permissions. (More details in `models.py`) ```python class MyModel
-(...): def permissions_for_user(self, user): return MyModelPermissionTester
-(self, user) class MyModelPermissionTester(...): def can_unpublish(self): """
-Can the user unpublish this object? (Required for un-publishing""" def
-can_publish(self): """ Can the user publish this object? (Required for
-publishing)""" def can_submit_for_moderation(self): """ Can the user submit
-this object for moderation? (Optional) """ ``` ## Revisions Revision support is
-included out of the box. If your model inherits from a `RevisionMixin`, we will
-automatically create drafts for you. These will not be published (If the model
-inherits from `DraftStateMixin`) until you choose to do so. ## Workflows We
-include a `WorkFlow` to submit this object for moderation. More workflow
-support will be included in the future. ## Logs Logs are also included out of
-the box. We will automatically update your model's history; including possible
-revisions. This will allow you to backtrack each change made on the frontend.
-This however does mean that a possibly large amount of data will be stored in
-your database. ## Caveats Wagtail does not always make it's `id` attribute
-available. This is only available to instances of `StreamChild` and
-`ListChild`. Consider the following regular wagtail list loop where `items` is
-a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
-item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
-editable block instead; we would slightly change the loop to make the block's
-`id` available. This is done by accessing the `bound_blocks` of that ListBlock
-*(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
-would then be: ```django-html {% for item in self.items.bound_blocks %} {#
-Field name and model are the same arguments as in the first example! #} {%
-fedit_block block=item block_id=item.id field_name="content"
-model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
-is wrapped with `fedit_block` or `fedit_field` the field_name and model
-argument can be omitted. The parent- blocktag will share these variables
-through context. This makes it possibly to easily use editable sub-blocks
-across multiple different model types. If your model **ISN'T** capable of
-editing; or these variables aren't shared - your block will be rendered as
-normal. ## Hooks ### wagtail_fedit.construct_block_toolbar Construct the
-toolbar for the given block. This is used to display the edit icon in the
-block. How it is called: ```python for hook in hooks.get_hooks
-(CONSTRUCT_BLOCK_TOOLBAR): hook(request=request, items=items, model=model,
-block_id=block_id, field_name=field_name) ``` ###
-wagtail_fedit.construct_field_toolbar Construct the toolbar for the given
-field. This is used to display the edit icon in the field. How it is called:
-```python for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR): hook
-(request=request, items=items, model=model, field_name=field_name) ``` ###
-wagtail_fedit.register_type_renderer Register a custom renderer for a type.
-Example of how this type of renderer can be used: ```python @hooks.register
-(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
-custom renderer for the Page model. # It will render the Page model as a simple
-h2 tag. renderer_map[Page] = lambda request, context, instance, value:
-format_html( '
+through context. #} {% fedit block self.content block=block block_id=block.id
+%} {% endfor %} ``` ```python from django.template.loader import
+render_to_string ... class MyPage(...): # Can be any type of model. content =
+StreamField(...) def render_fedit_content(self, request): return
+render_to_string("myapp/render_my_field.html", self.get_context(request)) ```
+Your content will then automatically be rendered with that method when need be
+by using `{% fedit field self.content %} ` 4. **But wait?! I go to my template
+and I do not see a way to edit!**That is true! We try to protect any styling on
+your actual page; we do not want to interfere.Instead; we serve the editing
+interface on a different URL, accessible by clicking `Frontend Editing` in the
+Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if
+your model inherits from `DraftStateMixin`. **Note:** If the parent block is
+wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance
+variable and field name should be omitted and replaced with `from_context`.
+Example: `{% fedit block from_context block=item block_id=item.id %}` The
+parent- blocktag will share these variables through context. This makes it
+possibly to easily use editable sub-blocks across multiple different model
+types. If your model **ISN'T** capable of editing; or these variables aren't
+shared - your block will be rendered as normal. ## Permissions **Note: This is
+not required for pages.** **The `Page` model already provides this interface.**
+We have the following basic permission requirements: * You must have
+`wagtailadmin.access_admin` to edit a block/field. * You must have the
+appropriate `app_label.change_*` permission for the model. This however only
+applies to editing. We use separate permissions for publishing and submitting
+workflows, etc. Models which you want to allow the publish view for should also
+implement a `PermissionTester`- like object. Example of how you should
+implement the `Tester` object and all required permissions. (More details in
+`models.py`) ```python class MyModel(...): def permissions_for_user(self,
+user): return MyModelPermissionTester(self, user) class MyModelPermissionTester
+(...): def can_unpublish(self): """ Can the user unpublish this object?
+(Required for un-publishing""" def can_publish(self): """ Can the user publish
+this object? (Required for publishing)""" def can_submit_for_moderation(self):
+""" Can the user submit this object for moderation? (Optional) """ ``` ##
+Revisions Revision support is included out of the box. If your model inherits
+from a `RevisionMixin`, we will automatically create drafts for you. These will
+not be published (If the model inherits from `DraftStateMixin`) until you
+choose to do so. ## Workflows We include a `WorkFlow` to submit this object for
+moderation. More workflow support will be included in the future. ## Logs Logs
+are also included out of the box. We will automatically update your model's
+history; including possible revisions. This will allow you to backtrack each
+change made on the frontend. This however does mean that a possibly large
+amount of data will be stored in your database. ## Caveats Wagtail does not
+always make it's `id` attribute available. This is only available to instances
+of `StreamChild` and `ListChild`. Consider the following regular wagtail list
+loop where `items` is a `ListBlock`. ```django-html {% for item in self.items
+%} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
+``` To make this an editable block instead; we would slightly change the loop
+to make the block's `id` available. This is done by accessing the
+`bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
+the toplevel block!)* Our new loop would then be: ```django-html {% for item in
+self.items.bound_blocks %} {# Field name and model are the same arguments as in
+the first example! #} {% fedit block my_model_instance_var.content_field
+block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
+wagtail_fedit.construct_block_toolbar Construct the toolbar for the given
+block. This is used to display the edit icon in the block. How it is called:
+```python for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR): hook
+(request=request, items=items, model=model, block_id=block_id,
+field_name=field_name) ``` ### wagtail_fedit.construct_field_toolbar Construct
+the toolbar for the given field. This is used to display the edit icon in the
+field. How it is called: ```python for hook in hooks.get_hooks
+(CONSTRUCT_FIELD_TOOLBAR): hook(request=request, items=items, model=model,
+field_name=field_name) ``` ### wagtail_fedit.register_type_renderer Register a
+custom renderer for a type. Example of how this type of renderer can be used:
+```python @hooks.register(REGISTER_TYPE_RENDERER) def register_renderers
+(renderer_map): # This is a custom renderer for the Page model. # It will
+render the Page model as a simple h2 tag. renderer_map[Page] = lambda request,
+context, instance, value: format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
```

### Comparing `wagtail_fedit-1.4.6/README.md` & `wagtail_fedit-1.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,19 +58,18 @@
        <title>Document</title>
        <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
    </head>
    <body>
        {# Adress the model.field or model.my.related.field you wish to edit. #}
        {# Editable fields get a special `inline` argument. #}
        {# if True the button is not placed with an absolute CSS position. #}
-       <h1>{% fedit_field self.title inline=True or False %}</h1>
+       <h1>{% fedit field self.title inline=True or False %}</h1>
 
-       {# Pass in the field_name and the model instance on which that field resides if you are using `wagtail_fedit <= 1.3.8` #}
        <main class="my-streamfield-content">
-           {% fedit_field "content" self %}
+           {% fedit field self.content %}
        </main>
 
        {% wagtailuserbar %}
 
        <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
    </body>
    </html>
@@ -86,15 +85,15 @@
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
        {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
        {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
-       {% fedit_block block=block block_id=block.id field_name="content" model=self %}
+       {% fedit block self.content block=block block_id=block.id %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
    ...
@@ -102,17 +101,24 @@
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
-   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
+   Your content will then automatically be rendered with that method when need be by using
+   `{% fedit field self.content %} `
 4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
+**Note:** If the parent block is wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance variable and field name should be omitted and replaced with `from_context`.
+Example: `{% fedit block from_context block=item block_id=item.id %}`
+The parent- blocktag will share these variables through context.
+This makes it possibly to easily use editable sub-blocks across multiple different model types.
+If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
+
 ## Permissions
 
 **Note: This is not required for pages.**
 
 **The `Page` model already provides this interface.**
 
 We have the following basic permission requirements:
@@ -184,23 +190,18 @@
 This is done by accessing the `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for the toplevel block!)*
 
 Our new loop would then be:
 
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
-    {% fedit_block block=item block_id=item.id field_name="content" model=my_model_instance_var %}
+    {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
-**Note:** If the parent block is wrapped with `fedit_block` or `fedit_field` the field_name and model argument can be omitted.
-The parent- blocktag will share these variables through context.
-This makes it possibly to easily use editable sub-blocks across multiple different model types.
-If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
-
 ## Hooks
 
 ### wagtail_fedit.construct_block_toolbar
 
 Construct the toolbar for the given block.
 This is used to display the edit icon in the block.
```

#### html2text {}

```diff
@@ -19,94 +19,92 @@
 Editing! 1. Make sure the models you wish to edit inherit from
 PreviewableMixin. **This is a requirement.** 2. Define a template for your
 model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
 the required template tag libraries #}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {#
 Editable fields get a special `inline` argument. #} {# if True the button is
 not placed with an absolute CSS position. #}
-************ {{%% ffeeddiitt__ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
-{# Pass in the field_name and the model instance on which that field resides if
-you are using `wagtail_fedit <= 1.3.8` #} {% fedit_field "content" self %} {%
-wagtailuserbar %}
+************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
+{% fedit field self.content %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
 do not require the field_name or model argument. #} {# This is taken from the
 parent (also wrapped by `fedit_block`); the model and field name are shared
-through context. #} {% fedit_block block=block block_id=block.id
-field_name="content" model=self %} {% endfor %} ``` ```python from
-django.template.loader import render_to_string ... class MyPage(...): # Can be
-any type of model. content = StreamField(...) def render_fedit_content(self,
-request): return render_to_string("myapp/render_my_field.html",
-self.get_context(request)) ``` Your content will then automatically be rendered
-with that method when need be by using `{% fedit_field "content" self %} ` 4.
-**But wait?! I go to my template and I do not see a way to edit!**That is true!
-We try to protect any styling on your actual page; we do not want to
-interfere.Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
-on that userbar! It is also used for publishing if your model inherits from
-`DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
-**The `Page` model already provides this interface.** We have the following
-basic permission requirements: * You must have `wagtailadmin.access_admin` to
-edit a block/field. * You must have the appropriate `app_label.change_*`
-permission for the model. This however only applies to editing. We use separate
-permissions for publishing and submitting workflows, etc. Models which you want
-to allow the publish view for should also implement a `PermissionTester`- like
-object. Example of how you should implement the `Tester` object and all
-required permissions. (More details in `models.py`) ```python class MyModel
-(...): def permissions_for_user(self, user): return MyModelPermissionTester
-(self, user) class MyModelPermissionTester(...): def can_unpublish(self): """
-Can the user unpublish this object? (Required for un-publishing""" def
-can_publish(self): """ Can the user publish this object? (Required for
-publishing)""" def can_submit_for_moderation(self): """ Can the user submit
-this object for moderation? (Optional) """ ``` ## Revisions Revision support is
-included out of the box. If your model inherits from a `RevisionMixin`, we will
-automatically create drafts for you. These will not be published (If the model
-inherits from `DraftStateMixin`) until you choose to do so. ## Workflows We
-include a `WorkFlow` to submit this object for moderation. More workflow
-support will be included in the future. ## Logs Logs are also included out of
-the box. We will automatically update your model's history; including possible
-revisions. This will allow you to backtrack each change made on the frontend.
-This however does mean that a possibly large amount of data will be stored in
-your database. ## Caveats Wagtail does not always make it's `id` attribute
-available. This is only available to instances of `StreamChild` and
-`ListChild`. Consider the following regular wagtail list loop where `items` is
-a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
-item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
-editable block instead; we would slightly change the loop to make the block's
-`id` available. This is done by accessing the `bound_blocks` of that ListBlock
-*(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
-would then be: ```django-html {% for item in self.items.bound_blocks %} {#
-Field name and model are the same arguments as in the first example! #} {%
-fedit_block block=item block_id=item.id field_name="content"
-model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
-is wrapped with `fedit_block` or `fedit_field` the field_name and model
-argument can be omitted. The parent- blocktag will share these variables
-through context. This makes it possibly to easily use editable sub-blocks
-across multiple different model types. If your model **ISN'T** capable of
-editing; or these variables aren't shared - your block will be rendered as
-normal. ## Hooks ### wagtail_fedit.construct_block_toolbar Construct the
-toolbar for the given block. This is used to display the edit icon in the
-block. How it is called: ```python for hook in hooks.get_hooks
-(CONSTRUCT_BLOCK_TOOLBAR): hook(request=request, items=items, model=model,
-block_id=block_id, field_name=field_name) ``` ###
-wagtail_fedit.construct_field_toolbar Construct the toolbar for the given
-field. This is used to display the edit icon in the field. How it is called:
-```python for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR): hook
-(request=request, items=items, model=model, field_name=field_name) ``` ###
-wagtail_fedit.register_type_renderer Register a custom renderer for a type.
-Example of how this type of renderer can be used: ```python @hooks.register
-(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
-custom renderer for the Page model. # It will render the Page model as a simple
-h2 tag. renderer_map[Page] = lambda request, context, instance, value:
-format_html( '
+through context. #} {% fedit block self.content block=block block_id=block.id
+%} {% endfor %} ``` ```python from django.template.loader import
+render_to_string ... class MyPage(...): # Can be any type of model. content =
+StreamField(...) def render_fedit_content(self, request): return
+render_to_string("myapp/render_my_field.html", self.get_context(request)) ```
+Your content will then automatically be rendered with that method when need be
+by using `{% fedit field self.content %} ` 4. **But wait?! I go to my template
+and I do not see a way to edit!**That is true! We try to protect any styling on
+your actual page; we do not want to interfere.Instead; we serve the editing
+interface on a different URL, accessible by clicking `Frontend Editing` in the
+Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if
+your model inherits from `DraftStateMixin`. **Note:** If the parent block is
+wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance
+variable and field name should be omitted and replaced with `from_context`.
+Example: `{% fedit block from_context block=item block_id=item.id %}` The
+parent- blocktag will share these variables through context. This makes it
+possibly to easily use editable sub-blocks across multiple different model
+types. If your model **ISN'T** capable of editing; or these variables aren't
+shared - your block will be rendered as normal. ## Permissions **Note: This is
+not required for pages.** **The `Page` model already provides this interface.**
+We have the following basic permission requirements: * You must have
+`wagtailadmin.access_admin` to edit a block/field. * You must have the
+appropriate `app_label.change_*` permission for the model. This however only
+applies to editing. We use separate permissions for publishing and submitting
+workflows, etc. Models which you want to allow the publish view for should also
+implement a `PermissionTester`- like object. Example of how you should
+implement the `Tester` object and all required permissions. (More details in
+`models.py`) ```python class MyModel(...): def permissions_for_user(self,
+user): return MyModelPermissionTester(self, user) class MyModelPermissionTester
+(...): def can_unpublish(self): """ Can the user unpublish this object?
+(Required for un-publishing""" def can_publish(self): """ Can the user publish
+this object? (Required for publishing)""" def can_submit_for_moderation(self):
+""" Can the user submit this object for moderation? (Optional) """ ``` ##
+Revisions Revision support is included out of the box. If your model inherits
+from a `RevisionMixin`, we will automatically create drafts for you. These will
+not be published (If the model inherits from `DraftStateMixin`) until you
+choose to do so. ## Workflows We include a `WorkFlow` to submit this object for
+moderation. More workflow support will be included in the future. ## Logs Logs
+are also included out of the box. We will automatically update your model's
+history; including possible revisions. This will allow you to backtrack each
+change made on the frontend. This however does mean that a possibly large
+amount of data will be stored in your database. ## Caveats Wagtail does not
+always make it's `id` attribute available. This is only available to instances
+of `StreamChild` and `ListChild`. Consider the following regular wagtail list
+loop where `items` is a `ListBlock`. ```django-html {% for item in self.items
+%} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
+``` To make this an editable block instead; we would slightly change the loop
+to make the block's `id` available. This is done by accessing the
+`bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
+the toplevel block!)* Our new loop would then be: ```django-html {% for item in
+self.items.bound_blocks %} {# Field name and model are the same arguments as in
+the first example! #} {% fedit block my_model_instance_var.content_field
+block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
+wagtail_fedit.construct_block_toolbar Construct the toolbar for the given
+block. This is used to display the edit icon in the block. How it is called:
+```python for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR): hook
+(request=request, items=items, model=model, block_id=block_id,
+field_name=field_name) ``` ### wagtail_fedit.construct_field_toolbar Construct
+the toolbar for the given field. This is used to display the edit icon in the
+field. How it is called: ```python for hook in hooks.get_hooks
+(CONSTRUCT_FIELD_TOOLBAR): hook(request=request, items=items, model=model,
+field_name=field_name) ``` ### wagtail_fedit.register_type_renderer Register a
+custom renderer for a type. Example of how this type of renderer can be used:
+```python @hooks.register(REGISTER_TYPE_RENDERER) def register_renderers
+(renderer_map): # This is a custom renderer for the Page model. # It will
+render the Page model as a simple h2 tag. renderer_map[Page] = lambda request,
+context, instance, value: format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
```

### Comparing `wagtail_fedit-1.4.6/setup.cfg` & `wagtail_fedit-1.4.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
+00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
 00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
 00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
 00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
 00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.7/wagtail_fedit/forms/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,28 @@
 class BlockEditForm(forms.Form):
     def __init__(self, *args, block: BoundBlock, parent_instance: models.Model, request = None, **kwargs):
         self.block = block
         self.request = request
         self.parent_instance = parent_instance
 
         if "initial" not in kwargs:
-            # print(block.block.get_form_state(block.value))
             kwargs["initial"] = {
                 "value": block.value,
             }
 
         super().__init__(*args, **kwargs)
 
     def full_clean(self):
         super().full_clean()
         if self.errors:
             self.fields["value"].widget.form_errors = self.errors["value"]
 
     def save(self):
         block = self.cleaned_data["value"]
-        self.block.value = block
+        self.block.value.update(block)
         self.parent_instance.full_clean()
 
         if isinstance(self.parent_instance, RevisionMixin) and self.request:
             self.parent_instance = self.parent_instance.save_revision(
                 user=self.request.user,
                 log_action=False,
             )
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.7/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.7/wagtail_fedit/hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 
 ```python
 for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR):
     hook(request=request, items=items, model=model, field_name=field_name)
 ```
 """
 
+CONSTRUCT_ADAPTER_TOOLBAR = prefix("construct_adapter_toolbar")
+"""
+### wagtail_fedit.construct_adapter_toolbar
+Construct the toolbar for the given adapter.
+This is used to display the edit icon for the given adapter.
+"""
+
 
 REGISTER_TYPE_RENDERER   = prefix("register_type_renderer")
 """
 ### wagtail_fedit.register_type_renderer
 Register a custom renderer for a type.
 
 Example of how this type of renderer can be used:
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/models.py` & `wagtail_fedit-1.4.7/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,34 @@
 class iFrame {
     constructor(options) {
         const {
-            url,
             id,
             className,
+            srcdoc = null,
+            url = null,
             onLoad = () => {},
             onError = () => {},
             onCancel = () => {},
         } = options;
 
 
         this.url = url;
+        this.srcdoc = srcdoc;
+        this.iframe = null;
         this.id = id;
         this.className = className;
         this.onLoad = onLoad;
         this.onError = onError;
         this.onCancel = onCancel;
         this.render();
     }
 
     get element() {
         if (!this.iframe) {
-            this.iframe = this._renderFrame(this.url, this.onLoad);
+            this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad);
         }
         return this.iframe;
     }
 
     get document() {
         return this.element.contentWindow.document;
     }
@@ -42,38 +45,43 @@
         return this.document.querySelector("#wagtail-fedit-form");
     }
 
     get formWrapper() {
         return this.document.querySelector(".wagtail-fedit-form-wrapper");
     }
 
-    update(url) {
+    update(url = null, srcdoc = null) {
+        this.srcdoc = srcdoc;
         this.url = url;
-        this._renderFrame(this.url, ({
+        this._renderFrame(this.url, this.srcdoc, ({
             newFrame
         }) => {
             this.iframe.remove();
             this.iframe = newFrame;
             this.onLoad({
                 newFrame
             });
         }, this.onError);
     }
 
     render() {
         if (this.iframe) {
             return this.iframe;
         }
-        this.iframe = this._renderFrame(this.url, this.onLoad);
+        this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad);
         return this.iframe;
     }
 
-    _renderFrame(url, onLoad, onError) {
+    _renderFrame(url, srcDoc, onLoad, onError) {
         const iframe = document.createElement('iframe');
-        iframe.src = url;
+        if (srcDoc) {
+            iframe.srcdoc = srcDoc;
+        } else {
+            iframe.src = url;
+        }
         iframe.id = this.id;
         iframe.className = this.className;
         iframe.onload = () => {
             const cancelButton = this.document.querySelector(".wagtail-fedit-cancel-button");
             if (cancelButton) {
                 cancelButton.addEventListener("click", this.onCancel);
             }
@@ -113,64 +121,64 @@
 }
 
 
 class WagtailFeditEditor {
     constructor(options) {
         const {
             element = null,
-                wrapperQuerySelector = ".wagtail-fedit-block-wrapper",
-                type = "block",
         } = options;
 
-        this.type = type;
         this.initialTitle = document.title;
 
         if (!element) {
             this.wrapperQuerySelector = wrapperQuerySelector;
             this.wrapperElement = document.querySelector(this.wrapperQuerySelector);
         } else {
             /**@type {HTMLElement} */
             this.wrapperElement = element;
         }
-        this.editUrl = null;
+        this.sharedContext = null;
         this.modalHtml = null;
         this.editBtn = null;
         this.init();
         this.iframe = null;
 
         if (window.location.hash === `#${this.wrapperElement.id}`) {
             this.makeModal();
             this.focus();
         }
     }
 
-    get wrapperElementContent() {
-        return this.wrapperElement.querySelector(`.wagtail-fedit-${this.type}-content`);
+    focus() {
+        this.wrapperElement.focus();
     }
 
-    focus() {
-        const content = this.wrapperElementContent;
-        if (content) {
-            content.focus();
-            return;
+    getEditUrl() {
+        // build the edit url from relative edit url
+        const url = new URL(window.location.href);
+        url.pathname = this.editUrl;
+        if (this.sharedContext) {
+            url.searchParams.set("shared_context", this.sharedContext);
         }
+        return url.toString();
     }
 
-    makeModal() {
+    async makeModal() {
         this.modalWrapper.innerHTML = this.modalHtml;
         this.modal = this.modalWrapper.querySelector(".wagtail-fedit-modal");
+
         this.iframe = new iFrame({
-            url: this.editUrl,
-            id: null,
+            url: this.getEditUrl(),
+            id: "wagtail-fedit-iframe",
             className: null,
             onLoad: () => {
                 const onSubmit = (e) => {
                     e.preventDefault();
                     const formData = new FormData(this.iframe.formElement);
-                    fetch(this.editUrl, {
+                    fetch(this.getEditUrl(), {
                         method: "POST",
                         body: formData,
                     }).then((response) => {
                         response = response.json();
                         return response;
                     }).then((response) => {
                         if (!response.success) {
@@ -224,36 +232,40 @@
             onError: () => {
                 this.closeModal();
             },
             onCancel: () => {
                 this.closeModal();
             },
         });
+
         this.modal.appendChild(this.iframe.element);
 
         const closeBtn = document.createElement("button");
         closeBtn.innerHTML = "&times;";
         closeBtn.classList.add("wagtail-fedit-close-button");
         closeBtn.addEventListener("click", this.closeModal.bind(this));
         this.modal.appendChild(closeBtn);
     }
 
     setWrapperHtml(html) {
+
         const anim = this.wrapperElement.animate([{
             opacity: 1
         }, {
             opacity: 0
         }, ], {
             duration: 350,
             easing: "ease-in-out",
         });
+
         anim.onfinish = () => {
             const newBlock = document.createElement("div");
             newBlock.innerHTML = html;
             const blockWrapper = newBlock.firstElementChild;
+            blockWrapper.classList.add("wagtail-fedit-initialized");
             this.wrapperElement.parentNode.insertBefore(blockWrapper, this.wrapperElement);
             this.wrapperElement.parentNode.removeChild(this.wrapperElement);
             blockWrapper.style.opacity = 0;
             this.wrapperElement = blockWrapper;
             this.init();
 
             const anim = blockWrapper.animate([{
@@ -284,41 +296,47 @@
         const wrapper = document.createElement("div");
         wrapper.id = "wagtail-fedit-modal-wrapper";
         wrapper.classList.add("wagtail-fedit-modal-wrapper");
         document.body.appendChild(wrapper);
         return wrapper;
     }
 
+    get editUrl() {
+        return this.wrapperElement.dataset.editUrl;
+    }
+
     init() {
-        this.editUrl = this.wrapperElement.dataset.editUrl;
+        console.log("before", this.sharedContext);
+        this.sharedContext = this.wrapperElement.dataset.sharedContext;
         this.modalHtml = modalHtml.replace("__ID__", this.wrapperElement.dataset.id);
         this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button");
 
+        console.log("after", this.sharedContext);
+
         const api = new WagtailFeditorAPI(this);
         const content = this.wrapperElementContent;
         this.wrapperElement.editorAPI = api;
         if (content) {
             content.editorAPI = api;
         }
 
-        this.editBtn.addEventListener("click", (e) => {
+        this.editBtn.addEventListener("click", async (e) => {
             e.preventDefault();
             e.stopPropagation();
-            this.makeModal();
+            await this.makeModal();
         });
     }
 
     initNewEditors() {
-        const wagtailFeditBlockEditors = this.wrapperElement.querySelectorAll(".wagtail-fedit-block-wrapper");
+        const wagtailFeditBlockEditors = this.wrapperElement.querySelectorAll(".wagtail-fedit-adapter-wrapper");
         for (const editor of wagtailFeditBlockEditors) {
             if (!editor.classList.contains("wagtail-fedit-initialized")) {
                 editor.classList.add("wagtail-fedit-initialized");
                 new WagtailFeditEditor({
-                    element: editor,
-                    type: this.type
+                    element: editor
                 });
             }
         }
     }
 }
 
 class WagtailFeditPublishMenu {
@@ -381,39 +399,30 @@
                 this.publishButtonsWrapper.classList.add("open");
             };
         });
     }
 }
 
 function initFEditors() {
-    const wagtailFeditBlockEditors = document.querySelectorAll(".wagtail-fedit-block-wrapper");
-    const wagtailFeditFieldEditors = document.querySelectorAll(".wagtail-fedit-field-wrapper");
-    for (const editor of wagtailFeditBlockEditors) {
-        if (!editor.classList.contains("wagtail-fedit-initialized")) {
-            editor.classList.add("wagtail-fedit-initialized");
-            new WagtailFeditEditor({
-                element: editor,
-                type: "block"
-            });
-        }
-    }
-    for (const editor of wagtailFeditFieldEditors) {
+    const editors = document.querySelectorAll(".wagtail-fedit-adapter-wrapper");
+    for (const editor of editors) {
         if (!editor.classList.contains("wagtail-fedit-initialized")) {
             editor.classList.add("wagtail-fedit-initialized");
             new WagtailFeditEditor({
                 element: editor,
-                type: "field"
+                type: "adapter"
             });
         }
     }
     const observer = new MutationObserver((mutations) => {
         for (const mutation of mutations) {
             for (const node of mutation.addedNodes) {
                 if (node.nodeType === 1) {
-                    if (node.classList.contains("wagtail-fedit-block-wrapper") && !node.classList.contains("wagtail-fedit-initialized")) {
+                    if (node.classList.contains("wagtail-fedit-adapter-wrapper") && !node.classList.contains("wagtail-fedit-initialized")) {
+                        node.classList.add("wagtail-fedit-initialized");
                         new WagtailFeditEditor({
                             element: node
                         });
                     }
                 }
             }
         }
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 {% extends "./base_iframe.html" %}
 
 {% load i18n wagtailadmin_tags %}
 
 {% block content %}
     <div class="wagtail-fedit-form-wrapper{% if form.block.block.meta.fedit_full %} fedit-full{% endif %}">
-        
+
         {{ block.super }}
 
         <form id="wagtail-fedit-form" action="{{ edit_url }}" method="post" {% for k, v in form_attrs.items %}{{ k }}="{{ v|safe }}" {% endfor %}>
             {% csrf_token %}
             {% block form %}
-                {% panel id="wagtail-fedit-editor" icon="draft" heading=label %}
+                {% panel id="wagtail-fedit-editor" icon="draft" heading=meta_field.verbose_name %}
                     <div class="wagtail-fedit-form">
-                        
-                        {{ form.value }}
-
+                        {% for field in form %}
+                            {% include "./field.html" %}
+                        {% endfor %}
                     </div>
                 {% endpanel %}
             {% endblock %}
         </form>
     </div>
 {% endblock %}
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.7/wagtail_fedit/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,458 +1,457 @@
-from django.template import library, Node, NodeList
-from django.template.loader import render_to_string
-from django.template.base import Parser, Token
-from django.template.base import FilterExpression
+from typing import Any
+from collections import namedtuple
+from urllib.parse import urlencode
+from django.db import models
+from django.http import HttpRequest
 from django.utils.safestring import mark_safe
+from django.utils.translation import gettext_lazy as _
+from django.template.base import FilterExpression
+from django.conf import settings
 from django.urls import reverse
-from django.core import signing
-from django.db import models
 
-from wagtail.blocks import BoundBlock
 from wagtail import hooks
-from urllib.parse import urlencode
-
-import warnings
-
-from ..toolbar import (
-    FeditBlockEditButton,
-    FeditFieldEditButton,
+from wagtail.models import (
+    DraftStateMixin,
+    WorkflowMixin,
+    LockableMixin,
+    PreviewableMixin
 )
-from ..utils import (
-    _can_edit,
-    edit_url,
-    get_field_content,
-    _resolve_expressions,
-)
-from ..hooks import (
-    CONSTRUCT_BLOCK_TOOLBAR,
-    CONSTRUCT_FIELD_TOOLBAR,
+from wagtail.admin.admin_url_finder import AdminURLFinder
+from wagtail.blocks.stream_block import StreamValue
+from wagtail.blocks.list_block import ListValue
+from wagtail import blocks
+
+from .hooks import (
+    EXCLUDE_FROM_RELATED_FORMS,
+    REGISTER_TYPE_RENDERER,
+    REGISTER_FIELD_RENDERER,
 )
 
 
-register = library.Library()
-url_value_signer = signing.TimestampSigner()
+FEDIT_PREVIEW_VAR = "_wagtail_fedit_preview"
+USERBAR_MODEL_VAR = "_wagtail_fedit_userbar_model"
 
 
-WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for %(object)s."
-WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for %(object)s."
+class FeditPermissionCheck:
+    @staticmethod
+    def has_perms(request: HttpRequest, model: Any) -> bool:
 
+        user = request
+        if isinstance(request, HttpRequest):
+            user = request.user
+        
+        if (
+            not user.is_authenticated\
+            or not user.has_perm("wagtailadmin.access_admin")\
+            or not user.has_perm(f"{model._meta.app_label}.change_{model._meta.model_name}")    
+        ):
+            return False
+        
+        return True
 
-class BlockEditNode(Node):
-    class UnpackError(Exception):
-        pass
 
-    def __init__(self,
-            nodelist: NodeList = None,
-            block: BoundBlock = None,
-            block_id: str = None,
-            field_name: str = None,
-            model: models.Model = None,
-            **extra,
-        ):
+class FeditIFrameMixin:
+    ERROR_TITLE = _("Validation Errors")
 
-        self.nl = nodelist
-        self.block = block
-        self.block_id = block_id
-        self.field_name = field_name
-        self.model = model
-        self.extra = extra
-
-    def render(self, context):
-        block = self.block
-        block_id = self.block_id
-        field_name = self.field_name
-        model = self.model
-        extra = self.extra
-
-        # Conversions for filterexpressions
-        for k, e in extra.items():
-            if isinstance(e, FilterExpression):
-                extra[k] = e.resolve(context)
+    HEADING_SUPPORTS_DRAFTS = _("Publishing Required")
+    TITLE_SUPPORTS_DRAFTS = _("The object you are editing supports drafts.")
+    TEXT_PUBLISH_DRAFTS = _("You must publish %(model)s to make any changes visible.")
 
-        if not field_name and "wagtail_fedit_field_name" in context:
-            field_name = context["wagtail_fedit_field_name"]
+    HEADING_NO_DRAFTS = _("No Publishing Required")
+    TITLE_NO_DRAFTS = _("The object you are editing does not support drafts.")
+    TEXT_NO_DRAFTS = _("You are not required to publish this object to make this change visible.")
 
-        block, block_id, field_name, model =\
-            _resolve_expressions(context, block, block_id, field_name, model)
-        
-        # if not block_id and "block_id" not in context and not block:
-        #     raise ValueError("Block ID is required")
-        
-        # `wagtail_fedit_instance` is provided after the form is saved.
-        # This allows us to easily use the same instance across multiple views.
-        # Model will only be provided initially when the block is rendered.
-        model = model or context.get("wagtail_fedit_instance")
-        context["wagtail_fedit_field_name"] = field_name
-        context["wagtail_fedit_instance"] = model
-        
-        # Render the block or nodelist
-        # This allows us to use the block as a block tag or as a simple tag.
-        if block:
-            try:
-                block_context = context.flatten()
-            except AttributeError:
-                block_context = context
-            block_context.update(extra)
-            rendered = block.render_as_block(block_context)
-            self.has_block = True
-        elif self.nl:
-            rendered = self.nl.render(context)
-            self.has_block = False
-        else:
-            raise ValueError("Block or nodelist is required")
-        
-        if not field_name:
-            warnings.warn(
-                WARNING_FIELD_NAME_NOT_AVAILABLE
-                % {"object": context.template_name}
-            )
-            return rendered
+
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data(**kwargs)
+        context["help_text"] = self.get_help_text()
+        context["error_title"] = self.get_error_title()
+        return context
+    
+    def get_error_title(self) -> str:
+        return self.ERROR_TITLE
+
+    def get_help_text(self) -> str:
+        # No relations. Maybe draft support.
+        if is_draft_capable(getattr(self, "absolute_instance", self.object)):
+            return {
+                "status": "warning",
+                "heading": self.HEADING_SUPPORTS_DRAFTS,
+                "title": self.TITLE_SUPPORTS_DRAFTS,
+                "text": mark_safe(self.TEXT_PUBLISH_DRAFTS % {
+                    "model": get_model_string(getattr(self, "absolute_instance", self.object), publish_url=True, request=self.request),
+                })
+            }
         
-        if not model:
-            warnings.warn(
-                WARNING_MODEL_INSTANCE_NOT_AVAILABLE
-                % {"object": block.block.__class__.__name__}
-            )
-            return rendered
+        return {
+            "status": "info",
+            "heading": self.HEADING_NO_DRAFTS,
+            "title": self.TITLE_NO_DRAFTS,
+            "text": mark_safe(self.TEXT_NO_DRAFTS)
+        }
+
+
+def use_related_form(field: models.Field) -> bool:
+    """
+    Check if a field should be included in the related forms.
+    Internally used to make sure we use widgets instead
+    of rendering a form for a Page, Image or Document model.
+    """
+    for hook in hooks.get_hooks(EXCLUDE_FROM_RELATED_FORMS):
+        if hook(field):
+            return False
+    return True
+
+
+def access_userbar_model(request: HttpRequest) -> models.Model:
+    """
+    Retrieve the model set for the userbar in the request.
+    """
+    if not hasattr(request, USERBAR_MODEL_VAR):
+        return None
+    
+    return getattr(request, USERBAR_MODEL_VAR)
+
+def with_userbar_model(request: HttpRequest, model: models.Model) -> HttpRequest:
+    """
+    Set the model to be available in the userbar.
+    The request is shared easily between these contexts - might as well use it.
+    """
+    setattr(request, USERBAR_MODEL_VAR, model)
+    return request
+
+def get_block_name(block):
+    """
+    Return the block's type name for a block in a StreamField or ListBlock.
+    eg. "heading", "paragraph", "image", "item", "column", etc.
+    """
+    if isinstance(block, StreamValue.StreamChild):
+        return block.block_type
+    elif isinstance(block, ListValue.ListChild):
+        return "item"
+    elif isinstance(block, ListValue):
+        return block.block.name
+    elif isinstance(block, (blocks.StructValue, blocks.BoundBlock)):
+        return block.block.name
+    else:
+        raise ValueError("Unknown block type: %s" % type(block))
+    
+def get_block_path(block):
+    """
+    Get the current path part of a block in a StreamField or ListBlock.
+    """
+    if isinstance(block, StreamValue.StreamChild):
+        return block.id
+    elif isinstance(block, ListValue.ListChild):
+        return block.id
+    elif isinstance(block, ListValue):
+        return block.block.name
+    elif isinstance(block, (blocks.StructValue, blocks.BoundBlock)):
+        return block.block.name
+    else:
+        raise ValueError("Unknown block type: %s" % type(block))
+
+def find_block(block_id, field, contentpath=None):
+    """
+    Find a block in a StreamField or ListBlock by its ID.
+    """
+    if contentpath is None:
+        contentpath = []
+
+    # Check and cast field to iterable if necessary, but do not append non-StreamValue names to contentpath here.
+    if not isinstance(field, StreamValue) and not hasattr(field, "__iter__"):
+        field = [field]
+
+    # Adjust for ListValue to get the iterable bound_blocks.
+    if isinstance(field, ListValue):
+        field = field.bound_blocks
+
+    for block in field:
+        # Determine the block's name only if needed to avoid premature addition to contentpath.
+        block_name = get_block_path(block)
         
-        # Get block id from block if bound or context.
-        if not block_id and "block_id" in context:
-            block_id = context["block_id"]
-        elif not block_id and block and hasattr(block, "id"):
-            block_id = block.id
-        # elif not block_id: # Commented out; just return rendered if block_id is not available.
-        #     raise ValueError("Block ID is required")
+        if getattr(block, "id", None) == block_id:
+            # Append the block name here as it directly leads to the target.
+            return block, contentpath + [block_name]
         
-        if not rendered:
-            rendered = mark_safe("")
+        # Prepare to check children without altering the current path yet.
+        if isinstance(block.value, blocks.StructValue):
+            for _, value in block.value.bound_blocks.items():
+                found, found_path = find_block(block_id, value, contentpath + [block_name])
+                if found:
+                    return found, found_path
 
-        # Check if the user has permission to edit the block.
-        request = context.get("request")
-        if not _can_edit(request, model) or not block_id:
-            return rendered
-
-        if self.has_block:
-            extra["has_block"] = self.has_block
-
-        return render_editable_block(
-            request=request,
-            content=rendered,
-            block_id=block_id,
-            field_name=field_name,
-            model=model,
-            context=context,
-            **extra,
-        )
+        elif isinstance(block.value, (StreamValue, StreamValue.StreamChild, ListValue)):
+            found, found_path = find_block(block_id, block.value, contentpath + [block_name])
+            if found:
+                return found, found_path
 
-    @staticmethod
-    def pack(**kwargs) -> dict:
+    # Return None and the current path if no block is found at this level.
+    return None, contentpath
 
-        packed = {}
-        for k, v in kwargs.items():
-            packed[k] = url_value_signer.sign(str(v))
-
-        return packed
-    
-    @classmethod
-    def unpack(cls, *expected: str, request = None) -> dict:
-        if not request:
-            raise ValueError("Request is required")
-        
-        unpacked = {}
-        for key in expected:
-            try:
-                unpacked[key] = url_value_signer.unsign(
-                    request.GET.get(key)
-                )
-            except signing.SignatureExpired:
-                raise cls.UnpackError(f"Value for {key} has expired")
-            except signing.BadSignature:
-                raise cls.UnpackError(f"Invalid value for {key}")
-            except TypeError:
-                raise cls.UnpackError(f"Missing value for {key}")
 
-        if not all([unpacked.get(key) for key in expected]):
-            raise cls.UnpackError(f"Missing value for {key}")
-        
-        return unpacked
 
-    @staticmethod
-    def get_edit_url(block_id: str, field_name: str, instance: models.Model, **kwargs) -> str:
-        base_url = reverse(
-            "wagtail_fedit:edit_block",
-            args=[block_id, field_name, instance._meta.app_label, instance._meta.model_name, instance.pk]
-        )
+_renderer_map = {}
+_field_renderer_map = {}
+_looked_for_renderers = False
 
-        if not kwargs:
-            return base_url
 
-        packed = urlencode(
-            BlockEditNode.pack(**kwargs),
-        )
-        return f"{base_url}?{packed}"
+def _look_for_renderers():
+    global _looked_for_renderers
+    if not _looked_for_renderers:
+        for hook in hooks.get_hooks(REGISTER_TYPE_RENDERER):
+            hook(_renderer_map)
 
+        for hook in hooks.get_hooks(REGISTER_FIELD_RENDERER):
+            hook(_field_renderer_map)
 
+        _looked_for_renderers = True
 
-@register.tag(name="fedit_block")
-def do_render_fedit_block(parser: Parser, token: Token):
+
+def get_field_content(request, instance, meta_field: models.Field, context, content=None):
+    """
+    Return the content for a field on a model.
+    Also checks the model for a rendering method.
+    The method should be named `render_fedit_{field_name}`.
+    We wil also check for any hooks which may convert the content.
     """
-    This tag is used to render an editable block.
+    _look_for_renderers()
 
-    This block will be wrapped and is able to be edited by the user on the frontend.
+    if isinstance(meta_field, str):
+        meta_field = instance._meta.get_field(meta_field)
 
-    We will require the block_id and field_name of the streamfield this block belongs to.
+    if hasattr(context, "flatten"):
+        context = context.flatten()
 
-    You could omit needing to pass a block ID by passing in the StreamChild instance as opposed to the StructValue instance.
-    
-    Usage example 1:
-        ```python
-        {% fedit_block my_structvalue_instance block_id my_streamfield_attribute_name page_instance %}
-        ```
+    if not content:
+        # Check for a rendering method if it exists
+        if hasattr(instance, f"render_fedit_{meta_field.name}"):
+            content = getattr(instance, f"render_fedit_{meta_field.name}")(request, context=context)
+        else:
+            content = getattr(instance, meta_field.name)
 
-    Optionally you can omit the block and pass in the block_id and field_name as keyword arguments.
+    for k, v in _field_renderer_map.items():
+        if isinstance(meta_field, k):
+            content = v(request, context, instance, content)
+            break
+
+    for k, v in _renderer_map.items():
+        if isinstance(content, k):
+            content = v(request, context, instance, content)
+            break
+
+    # The content might be a streamblock etc, we can render it as a block
+    # if isinstance(content, (blocks.BoundBlock, blocks.StructValue)):
+    if hasattr(content, "render_as_block"):
+        content = content.render_as_block(context)
 
-    This will allow you to use the block as a block tag.
+    return content
 
-    Usage example 2:
-        ```python
-        {% fedit_block block_id=my_structvalue_instance field_name=my_streamfield_attribute_name model=page_instance %}
-            <p>Some content before block</p>
-            {% include_block my_block %}
-            <p>Some content after block</p>
-        {% unfedit_block %}
-        ```
+def is_draft_capable(model):
+    """
+    Check if a model is capable of drafts.
     """
+    return isinstance(model, DraftStateMixin)\
+        or type(model) == type\
+        and issubclass(model, DraftStateMixin)
 
-    tokens = token.split_contents()
-    _ = tokens.pop(0)
-    kwargs_names = [
-        "block", "block_id",
-        "field_name", "model",
-    ]
+def model_diff(m1, m2):
+    """
+    Check if two model instances are different based on their type and primary key.
+    Does not check for differences in the model's fields.
+    This is used to determine if a relation is being saved.
+    """
+    return not (
+        m1._meta.app_label == m2._meta.app_label
+        and m1._meta.model_name == m2._meta.model_name\
+        and m1.pk == m2.pk
+    )
 
-    kwargs = get_kwargs(parser, kwargs_names, tokens)
-    
-    if "block" not in kwargs:
-        nodelist = parser.parse(("unfedit_block",))
-        parser.delete_first_token()
-    else:
-        nodelist = None
 
-    extra = {}
-    for key, value in kwargs.items():
-        if key not in kwargs_names:
-            extra[key] = value
-
-    return BlockEditNode(
-        nodelist=nodelist,
-        block=kwargs.get("block"),
-        block_id=kwargs.get("block_id"),
-        field_name=kwargs.get("field_name"),
-        model=kwargs.get("model"),
-        **extra,
-    )
+def edit_url(instance: models.Model, request: HttpRequest, hash = None, **params) -> str:
+    """
+        Return the edit URL for a given object and user (or request instead of user.)
+        If none exists and the model is an instance of PreviewableMixin;
+        return the wagtail_fedit:editable url; else an empty string.
+    """
 
+    user = request.user
+    finder = AdminURLFinder(user)
+    admin_url = finder.get_edit_url(instance)
+
+    if not admin_url:
+
+        # Check if the instance is a PreviewableMixin
+        # and the user has permission to edit it.
+        if isinstance(instance, PreviewableMixin)\
+                and _can_edit(request, instance):
+            
+            admin_url = reverse(
+                "wagtail_fedit:editable",
+                args=[
+                    instance.pk,
+                    instance._meta.app_label,
+                    instance._meta.model_name
+                ],
+            )
+        else:
+            return ""
 
-class FieldEditNode(Node):
-    def __init__(self, model: models.Model, getters: list[str], inline: bool = False, **kwargs):
-        self.model = model
-        self.field = getters[len(getters)-1]
-        self.getters = getters
-        self.inline = inline
-        self.kwargs = kwargs
-
-    def render(self, context):
-        getters = self.getters
-        model = self.model
-        inline = self.inline
-
-        model, inline =\
-            _resolve_expressions(context, model, inline)
-
-        obj = model
-        for i in range(len(getters) - 1):
-            getter = getters[i]
-            try:
-                obj = getattr(obj, getter)
-            except AttributeError:
-                raise AttributeError(f"Object {model.__class__.__name__} does not have attribute {getter}")
-
-        request = context.get("request")
-        content = get_field_content(
-            request,
-            obj,
-            obj._meta.get_field(self.field),
-            context,
-        )
+    data = urlencode(params)
+    if params:
+        admin_url = f"{admin_url}?{data}"
 
-        if not content:
-            content = mark_safe("")
-            # Force inline editing if no content is available.
-            # This will make sure the height of the field to edit is not 0.
-            inline = True
-
-        if not _can_edit(request, obj):
-            return content
-
-        for k, v in self.kwargs.items():
-            if isinstance(v, FilterExpression):
-                self.kwargs[k] = v.resolve(context)
-                  
-        if inline:
-            self.kwargs["inline"] = True
-  
-        return render_editable_field(
-            request=request, 
-            content=content,
-            field_name=self.field, 
-            model=obj,
-            context=context,
-            **self.kwargs,
-        )
+    if hash:
+        admin_url = f"{admin_url}#{hash}"
     
+    return admin_url
 
 
-@register.tag(name="fedit_field")
-def do_render_fedit_field(parser: Parser, token: Token):
+def get_model_string(instance: models.Model, publish_url: bool = False, request: HttpRequest = None, target = "_blank", **params) -> str:
     """
-    This tag is used to render an editable field.
+    Get a string representation of a model instance. If the instance has a
+    `get_admin_display_title` method, it will be used to get the string
+    representation.
+    If that method does not exist, the `title` attribute will be used.
+    If the `title` attribute does not exist, the string representation of the
+    instance will be used.
+    If `publish_url` is True, the string will be wrapped in an anchor tag
+    linking to the publish view for the instance.
+    Permissions will not be checked. This is the responsibility of the caller.
+    """
+    model_string = getattr(instance, "get_admin_display_title", None)
+    if model_string:
+        model_string = model_string()
+    else:
+        model_string = getattr(instance, "title", str(instance))
 
-    This field will be wrapped and is able to be edited by the user on the frontend.
+    if publish_url:
 
-    Usage example:
-        ```python
-        {% fedit_field mymodel.myfield inline=(default: False) key1=value1 key2=value2 %}
-        ```
+        if is_draft_capable(instance):
+            admin_url = reverse(
+                "wagtail_fedit:publish",
+                args=[
+                    instance.pk,
+                    instance._meta.app_label,
+                    instance._meta.model_name
+                ],
+            )
 
-    Optionally your model can define a `render_fedit_{field_name}` method that will be used to render the field.
-    This will allow you to use custom rendering logic if need be.
-    """
-    tokens = token.split_contents()
-    _ = tokens.pop(0)
-    model__field = tokens.pop(0)
-    model_tokens = model__field.split(".")
+            data = urlencode(params)
+            if params:
+                admin_url = f"{admin_url}?{data}"
 
-    if len(model_tokens) < 2:
-        raise ValueError("Model and field name are required")
-    
-    # mymodel.myfield
-    # mymodel.related_field.myfield
-    model = parser.compile_filter(model_tokens.pop(0))
+        else:
+            admin_url = edit_url(instance, request, **params)
 
-    if tokens:
-        kwargs_names = [
-            "inline",
-        ]
+        if admin_url:
+            model_string = mark_safe(
+                f'<a href="{admin_url}" target="{target}">{model_string}</a>'
+            )
 
-        kwargs = get_kwargs(parser, kwargs_names, tokens)
-    else:
-        kwargs = {}
+    return model_string
 
-    return FieldEditNode(
-        model=model,
-        getters=model_tokens,
-        **kwargs,
+def _can_edit(request, obj: models.Model):
+    """
+    Check if the user has appropriate permissions to edit an object.
+    Also requires the current request be on the `wagtail_fedit:editable` url
+    (Or the preview variable to be True)
+    """
+    if not request or not obj:
+        return False
+    
+    return (
+        FeditPermissionCheck.has_perms(request, obj)\
+        and getattr(request, FEDIT_PREVIEW_VAR, False)
     )
 
+def user_can_publish(instance, user, check_for_changes: bool = True):
+    """
+    Check if a user can publish an object.
+    Mostly comes from PagePermissionTester.can_publish
+    """
+    if not isinstance(instance, DraftStateMixin):
+        return False
+    
+    if not instance.has_unpublished_changes\
+        and check_for_changes:
+        return False
+
+    if hasattr(instance, "permission_policy"):
+        return instance.permission_policy.user_has_permission(user, "publish")
+    
+    if not hasattr(instance, "permissions_for_user"):
+        return False
 
-def render_editable_field(request, content, field_name, model, context, **kwargs):
-    edit_url = reverse(
-        "wagtail_fedit:edit_field",
-        args=[field_name, model._meta.app_label, model._meta.model_name, model.pk]
-    )
+    return instance.permissions_for_user(user).can_publish()
 
-    if kwargs:
-        packed = urlencode(
-            BlockEditNode.pack(**kwargs),
-        )
-        edit_url = f"{edit_url}?{packed}"
+def user_can_unpublish(instance, user):
+    """
+    Check if a user can unpublish an object.
+    Mostly comes from PagePermissionTester.can_unpublish
+    """
+    if not isinstance(instance, DraftStateMixin):
+        return False
+    
+    if not hasattr(instance, "permissions_for_user"):
+        return False
+    
+    return instance.permissions_for_user(user).can_unpublish()
 
-    items = [
-        FeditFieldEditButton(),
-    ]
-
-    for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR):
-        hook(request=request, items=items, model=model, field_name=field_name)
-
-    items = [item.render(request) for item in items]
-    items = list(filter(None, items))
-
-    kwargs["wagtail_fedit_field_name"] = field_name
-    kwargs["wagtail_fedit_instance"] = model
-    kwargs["inline"] = str(kwargs.get("inline", False)).lower() == "true"
-    return render_to_string(
-        "wagtail_fedit/content/editable_field.html",
-        {
-            "edit_url": edit_url,
-            "field_name": field_name,
-            "model": model,
-            "content": content,
-            "parent_context": context,
-            "toolbar_items": items,
-            **kwargs,
-        },
-        request=request,
-    )
+def user_can_submit_for_moderation(instance, user, check_for_changes: bool = True):
+    """
+    Check if a user can submit an object for moderation.
+    Mostly comes from PagePermissionTester.can_submit_for_moderation
+    """
+    if not getattr(settings, "WAGTAIL_WORKFLOW_ENABLED", True):
+        return False
 
-def render_editable_block(request, content, block_id, field_name, model, context, **kwargs):
-        admin_edit_url = edit_url(
-            model,
-            request,
-            hash=f"block-{block_id}-section",
-        )
+    if not instance.has_unpublished_changes\
+        and check_for_changes:
+        return False
 
-        items = [
-            FeditBlockEditButton(),
-        ]
+    if not isinstance(instance, WorkflowMixin):
+        return False
+    
+    if not hasattr(instance, "permissions_for_user"):
+        return False
+    
+    return instance.permissions_for_user(user).can_submit_for_moderation()
 
-        for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
-            hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
 
-        items = [item.render(request) for item in items]
-        items = list(filter(None, items))
-        
-        return render_to_string(
-            "wagtail_fedit/content/editable_block.html",
-            {
-                "edit_url": BlockEditNode.get_edit_url(
-                    block_id, field_name,
-                    instance=model,
-                    **kwargs,
-                ),
-                "admin_edit_url": admin_edit_url,
-                "block_id": block_id,
-                "model": model,
-                "content": content,
-                "field_name": field_name,
-                "parent_context": context,
-                "wagtail_fedit_field_name": field_name,
-                "wagtail_fedit_instance": model,
-                "toolbar_items": items,
-            }
+_lock_info = namedtuple("lock_info", ["lock", "locked_for_user"])
+
+def lock_info(object, user) -> _lock_info:
+    """
+        Returns the Lock instance (if any) and whether it is locked for the given user.
+    """
+    if isinstance(object, LockableMixin):
+        lock = object.get_lock()
+        locked_for_user = lock is not None and lock.for_user(
+            user
         )
+    else:
+        lock = None
+        locked_for_user = False
 
+    return _lock_info(lock, locked_for_user)
 
-def get_kwargs(parser: Parser, kwarg_list: list[str], tokens: list[str]) -> dict:
-    had_kwargs = False
-    kwargs = {}
-
-    # if len(tokens) > len(kwargs_names):
-    #     raise ValueError("Invalid number of arguments provided, expected at most %d" % len(kwargs_names))
-
-    for i, token in enumerate(tokens):
-        split = token.split("=")
-        if len(split) == 1:
-            if had_kwargs:
-                raise ValueError("Unexpected positional argument after keyword argument")
-            
-            kwargs[kwarg_list[i]] = parser.compile_filter(token)
-        else:
-            key = split[0]
-            # if key not in kwargs_names:
-            #     raise ValueError(f"Unexpected keyword argument {key}")
-            
-            kwargs[key] = parser.compile_filter(split[1])
-            had_kwargs = True
 
-    return kwargs
+def get_hooks(hook_name):
+    """
+        Return the hooks for a given hook name in the wagtail_fedit namespace.
+    """
+    for hook in hooks.get_hooks(f"wagtail_fedit.{hook_name}"):
+        yield hook
 
+    
+def _resolve_expressions(context, *expressions):
+    """
+        Resolve a list of possible templatetag filterexpressions.
+    """
+    def _map(expression):
+        if isinstance(expression, FilterExpression):
+            return expression.resolve(context)
+        return expression
+    
+    return tuple(map(_map, expressions))
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     EditableFullModel,
     EditableDraftModel,
     EditableRevisionModel,
     EditablePreviewModel,
     EditableLockModel,
 )
 
+import urllib.parse
+
+from wagtail_fedit.adapters import BaseAdapter
+
 TEST_BLOCK_DATA = [
     {
         "type": "heading_component",
         "value": {
             "heading": "This is pretty cool!!!",
             "subheading": "RIGHT?! FUCK YES!"
         },
@@ -200,33 +204,40 @@
                 "object_id": model_id,
                 "app_label": app_label,
                 "model_name": model_name,
             }
         )
 
     def get_field_url(self, field_name, app_label, model_name, model_id):
-        url_name = "edit_field"
+        url_name = "edit"
         return reverse(
             f"wagtail_fedit:{url_name}",
             kwargs={
+                "adapter_id": "field",
                 "field_name": field_name,
                 "app_label": app_label,
                 "model_name": model_name,
                 "model_id": model_id
             }
         )
 
 
     def get_block_url(self, block_id, field_name, app_label, model_name, model_id):
-        url_name = "edit_block"
-        return reverse(
+        url_name = "edit"
+        url = reverse(
             f"wagtail_fedit:{url_name}",
             kwargs={
-                "block_id": block_id,
+                "adapter_id": "block",
                 "field_name": field_name,
                 "app_label": app_label,
                 "model_name": model_name,
                 "model_id": model_id
             }
         )
+        adapter = BaseAdapter(
+            BasicModel(), "title", None, block_id=block_id,
+        )
+        encoded = adapter.encode_shared_context()
+        encoded = urllib.parse.urlencode({"shared_context": encoded})
+        return f"{url}?{encoded}"
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_field_templatetag.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,158 @@
-from django.db import models
-from wagtail import hooks
-from wagtail_fedit.templatetags import (
-    fedit as templatetags,
+from django.db.models.base import Model as Model
+from django.http import HttpRequest
+from django.template import (
+    Context, Template,
+    TemplateSyntaxError,
 )
-from wagtail_fedit import (
-    utils,
-    hooks as fedit_hooks,
+from wagtail_fedit.adapters import (
+    BaseAdapter,
+    adapter_registry,
+    BlockAdapter,
+    FieldAdapter,
+)
+from wagtail_fedit.utils import (
+    FEDIT_PREVIEW_VAR,
+)
+from wagtail_fedit.templatetags.fedit import (
+    wrap_adapter,
 )
 from .base import (
     BaseFEditTest,
 )
 
+import json
+
+adapters = {}
+
+class TestAdapter(BaseAdapter):
+    identifier = "test"
+    required_kwargs = ["test"]
 
-class TestFieldTemplateTag(BaseFEditTest):
+    def __init__(self, object: Model, field_name: str, request: HttpRequest, **kwargs):
+        super().__init__(object, field_name, request, **kwargs)
+        adapters[self.kwargs["id"]] = self
 
-    def setUp(self):
-        super().setUp()
+    def render_content(self, parent_context: dict = None) -> str:
+        return f"TestAdapter: {self.field_value}"
 
-        # # This might make tests fail runnning in parallel.
-        # @hooks.register(fedit_hooks.REGISTER_FIELD_RENDERER)
-        # def register_type_renderer(mapping):
-        #     mapping[models.TextField] =\
-        #         lambda request, context, instance, value: f"<p class=\"text-field\">{value}</p>"
 
-        # This is ok.
-        utils._field_renderer_map[models.TextField] =\
-            lambda request, context, instance, value: f"<p class=\"text-field\">{value}</p>"
+adapter_registry.register(TestAdapter)
 
-    def test_render_regular_no_custom_type_renderer(self):
 
-        # Setup user attribute for request.
-        request = self.request_factory.get("/")
+class TestBaseAdapter(BaseFEditTest):
+
+    def test_required_kwargs_ok(self):
+        self.assertEqual(TestAdapter.required_kwargs, ["test"])
+
+        template_ok = Template(
+            "{% load fedit %}"
+            "{% fedit test object.title test='test' id=1 %}"
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
         request.user = self.admin_user
 
-        context = {
-            "request": request,
-            "model": self.basic_model,
-            "field_name": "title",
-        }
-
-        title_node = templatetags.FieldEditNode(
-            model=self.basic_model,
-            getters=["title"],
+        template_ok = template_ok.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
         )
 
         self.assertHTMLEqual(
-            title_node.render(context),
-            self.basic_model.title
+            template_ok,
+            f'TestAdapter: {self.basic_model.title}'
+        )
+
+        self.assertDictEqual(
+            adapters[1].kwargs,
+            {"test": "test", "id": 1}
         )
 
-    def test_render_editable_no_custom_type_renderer(self):
-        # Setup user attribute for request.
-        request = self.request_factory.get("/")
+    def test_required_kwargs_fail(self):
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
         request.user = self.admin_user
 
-        context = {
-            "request": request,
-            "model": self.basic_model,
-            "field_name": "title",
-        }
+        try:
+            template_fail = Template(
+                "{% load fedit %}"
+                "{% fedit test object.title id=2 %}"
+            )
+
+            # self.fail(f"Expected exception: {e}")
+            template_fail.render(Context({
+                "request": request,
+                "object": self.basic_model,
+            }))
+
+        except TemplateSyntaxError as e:
+            self.assertEqual(
+                str(e),
+                "Missing required keyword argument test"
+            )
 
-        # Mark as editable.
-        setattr(
-            request,
-            utils.FEDIT_PREVIEW_VAR,
-            True,
-        )
+        except Exception as e:
+            self.fail(f"Unexpected exception: {e} ({type(e)})")
 
-        title_node = templatetags.FieldEditNode(
-            model=self.basic_model,
-            getters=["title"],
-        )
+        else:
+            self.fail("Expected exception not raised")
 
-        rendered_title = templatetags.render_editable_field(
-            request,
-            self.basic_model.title,
-            "title",
+    def test_adapter_render_content(self):
+        adapter = TestAdapter(
             self.basic_model,
-            context,
+            "title",
+            self.request_factory.get(
+                self.get_editable_url(
+                    self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+                )
+            ),
+            id=3,
         )
 
-        self.assertHTMLEqual(
-            title_node.render(context),
-            rendered_title
+        self.assertEqual(
+            adapter.render_content(),
+            f"TestAdapter: {self.basic_model.title}"
         )
 
-    def test_render_regular_custom_type_renderer(self):
-        # Setup user attribute for request.
-        request = self.request_factory.get("/")
-        request.user = self.admin_user
+    def test_adapter_editable(self):
+        self.assertEqual(TestAdapter.required_kwargs, ["test"])
 
-        context = {
-            "request": request,
-            "model": self.basic_model,
-            "field_name": "title",
-        }
-
-        body_node = templatetags.FieldEditNode(
-            model=self.basic_model,
-            getters=["body"],
+        tpl = Template(
+            "{% load fedit %}"
+            "{% fedit test object.title test='test' id=4 %}"
         )
 
-        self.assertHTMLEqual(
-            body_node.render(context),
-            f"<p class=\"text-field\">{self.basic_model.body}</p>"
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
         )
-
-    def test_render_editable_custom_type_renderer(self):
-        # Setup user attribute for request.
-        request = self.request_factory.get("/")
         request.user = self.admin_user
 
-        context = {
-            "request": request,
-            "model": self.basic_model,
-            "field_name": "title",
-        }
-
-        # Mark as editable.
         setattr(
             request,
-            utils.FEDIT_PREVIEW_VAR,
+            FEDIT_PREVIEW_VAR,
             True,
         )
 
-        body_node = templatetags.FieldEditNode(
-            model=self.basic_model,
-            getters=["body"],
-            inline=True,
-        )
-
-        rendered_body = templatetags.render_editable_field(
-            request,
-            f"<p class=\"text-field\">{self.basic_model.body}</p>",
-            "body",
-            self.basic_model,
-            context,
-            inline=True,
+        tpl = tpl.render(
+            Context({
+                "request": request,
+                "object": self.basic_model,
+            })
         )
 
         self.assertHTMLEqual(
-            body_node.render(context),
-            rendered_body
+            tpl,
+            wrap_adapter(request, adapters[4], {})
         )
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.7/wagtail_fedit/toolbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,7 +49,17 @@
         Required button class for the edit modal to function.
         This button is handled by the script in `wagtail_fedit/js/frontend.js`
     """
     template_name = "wagtail_fedit/content/buttons/edit_field.html"
     permissions = [
         "wagtailadmin.access_admin",
     ]
+
+class FeditAdapterEditButton(FeditToolbarComponent):
+    """
+        Required button class for the edit modal to function.
+        This button is handled by the script in `wagtail_fedit/js/frontend.js`
+    """
+    template_name = "wagtail_fedit/content/buttons/edit_adapter.html"
+    permissions = [
+        "wagtailadmin.access_admin",
+    ]
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.7/wagtail_fedit/views/editable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,457 +1,452 @@
 from typing import Any
-from collections import namedtuple
-from urllib.parse import urlencode
 from django.db import models
-from django.http import HttpRequest
-from django.utils.safestring import mark_safe
-from django.utils.translation import gettext_lazy as _
-from django.template.base import FilterExpression
 from django.conf import settings
+from django.utils.translation import gettext_lazy as _
+from django.views.generic import TemplateView
+from django.shortcuts import redirect
 from django.urls import reverse
-
-from wagtail import hooks
+from django.http import (
+    HttpRequest,
+    HttpResponseBadRequest,
+    HttpResponseForbidden,
+    HttpResponse,
+)
+from wagtail.admin import messages
+from wagtail.log_actions import (
+    registry,
+)
+from wagtail.admin.admin_url_finder import AdminURLFinder
+from wagtail.actions.publish_page_revision import PublishPageRevisionAction
+from wagtail.actions.publish_revision import PublishRevisionAction
+from wagtail.actions.unpublish_page import UnpublishPageAction
+from wagtail.actions.unpublish import UnpublishAction
 from wagtail.models import (
+    RevisionMixin,
+    PreviewableMixin,
     DraftStateMixin,
     WorkflowMixin,
-    LockableMixin,
-    PreviewableMixin
+    WorkflowState,
+    PageLogEntry,
+    ModelLogEntry,
+    Page,
 )
-from wagtail.admin.admin_url_finder import AdminURLFinder
-from wagtail.blocks.stream_block import StreamValue
-from wagtail.blocks.list_block import ListValue
-from wagtail import blocks
-
-from .hooks import (
-    EXCLUDE_FROM_RELATED_FORMS,
-    REGISTER_TYPE_RENDERER,
-    REGISTER_FIELD_RENDERER,
+from .. import forms as block_forms
+from ..utils import (
+    FEDIT_PREVIEW_VAR,
+    USERBAR_MODEL_VAR,
+    FeditPermissionCheck,
+    with_userbar_model,
+    # user_can_publish,
+    # user_can_unpublish,
+    # user_can_submit_for_moderation,
+    # lock_info,
 )
 
+from .mixins import (
+    ObjectViewMixin,
+    LockViewMixin,
+)
 
-FEDIT_PREVIEW_VAR = "_wagtail_fedit_preview"
-USERBAR_MODEL_VAR = "_wagtail_fedit_userbar_model"
 
+MAX_LOG_ENTRIES_DISPLAYED = 5
 
-class FeditPermissionCheck:
-    @staticmethod
-    def has_perms(request: HttpRequest, model: Any) -> bool:
 
-        user = request
-        if isinstance(request, HttpRequest):
-            user = request.user
-        
-        if (
-            not user.is_authenticated\
-            or not user.has_perm("wagtailadmin.access_admin")\
-            or not user.has_perm(f"{model._meta.app_label}.change_{model._meta.model_name}")    
-        ):
-            return False
-        
-        return True
+def get_unpublish_action(object):
+    if isinstance(object, Page):
+        return UnpublishPageAction
+    return UnpublishAction
 
 
-class FeditIFrameMixin:
-    ERROR_TITLE = _("Validation Errors")
+def get_publish_action(object):
+    if isinstance(object, Page):
+        return PublishPageRevisionAction
+    return PublishRevisionAction
 
-    HEADING_SUPPORTS_DRAFTS = _("Publishing Required")
-    TITLE_SUPPORTS_DRAFTS = _("The object you are editing supports drafts.")
-    TEXT_PUBLISH_DRAFTS = _("You must publish %(model)s to make any changes visible.")
 
-    HEADING_NO_DRAFTS = _("No Publishing Required")
-    TITLE_NO_DRAFTS = _("The object you are editing does not support drafts.")
-    TEXT_NO_DRAFTS = _("You are not required to publish this object to make this change visible.")
+class BaseFeditView(ObjectViewMixin, FeditPermissionCheck, TemplateView):
+    def dispatch(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
+        if self.error_response:
+            return self.error_response
 
+        if not self.has_perms(request, self.object):
+            return HttpResponseForbidden("You do not have permission to view this page")
 
-    def get_context_data(self, **kwargs):
-        context = super().get_context_data(**kwargs)
-        context["help_text"] = self.get_help_text()
-        context["error_title"] = self.get_error_title()
-        return context
-    
-    def get_error_title(self) -> str:
-        return self.ERROR_TITLE
+        if issubclass(self.model, RevisionMixin) and self.object.latest_revision_id:
+            instance: RevisionMixin  = self.object
+            revision: RevisionMixin = instance.latest_revision
+            self.object = revision.as_object()
+            self.is_preview = True
+        else:
+            self.is_preview = False
 
-    def get_help_text(self) -> str:
-        # No relations. Maybe draft support.
-        if is_draft_capable(getattr(self, "absolute_instance", self.instance)):
-            return {
-                "status": "warning",
-                "heading": self.HEADING_SUPPORTS_DRAFTS,
-                "title": self.TITLE_SUPPORTS_DRAFTS,
-                "text": mark_safe(self.TEXT_PUBLISH_DRAFTS % {
-                    "model": get_model_string(getattr(self, "absolute_instance", self.instance), publish_url=True, request=self.request),
-                })
-            }
-        
-        return {
-            "status": "info",
-            "heading": self.HEADING_NO_DRAFTS,
-            "title": self.TITLE_NO_DRAFTS,
-            "text": mark_safe(self.TEXT_NO_DRAFTS)
+        try:
+            self.checks(request, self.object)
+        except ValueError as e:
+            return HttpResponseForbidden(str(e))
+
+        return super().dispatch(request, object_id, app_label, model_name)
+    
+    def checks(self, request: HttpRequest, object: Any) -> None:
+        pass
+
+    def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
+        return super().get_context_data(**kwargs) | {
+            "object": self.object,
+            "model": self.model,
         }
 
 
-def use_related_form(field: models.Field) -> bool:
-    """
-    Check if a field should be included in the related forms.
-    Internally used to make sure we use widgets instead
-    of rendering a form for a Page, Image or Document model.
-    """
-    for hook in hooks.get_hooks(EXCLUDE_FROM_RELATED_FORMS):
-        if hook(field):
-            return False
-    return True
-
-
-def access_userbar_model(request: HttpRequest) -> models.Model:
-    """
-    Retrieve the model set for the userbar in the request.
-    """
-    if not hasattr(request, USERBAR_MODEL_VAR):
-        return None
-    
-    return getattr(request, USERBAR_MODEL_VAR)
+class FEditableView(BaseFeditView):
 
-def with_userbar_model(request: HttpRequest, model: models.Model) -> HttpRequest:
-    """
-    Set the model to be available in the userbar.
-    The request is shared easily between these contexts - might as well use it.
-    """
-    setattr(request, USERBAR_MODEL_VAR, model)
-    return request
-
-def get_block_name(block):
-    """
-    Return the block's type name for a block in a StreamField or ListBlock.
-    eg. "heading", "paragraph", "image", "item", "column", etc.
-    """
-    if isinstance(block, StreamValue.StreamChild):
-        return block.block_type
-    elif isinstance(block, ListValue.ListChild):
-        return "item"
-    elif isinstance(block, ListValue):
-        return block.block.name
-    elif isinstance(block, (blocks.StructValue, blocks.BoundBlock)):
-        return block.block.name
-    else:
-        raise ValueError("Unknown block type: %s" % type(block))
-    
-def get_block_path(block):
-    """
-    Get the current path part of a block in a StreamField or ListBlock.
-    """
-    if isinstance(block, StreamValue.StreamChild):
-        return block.id
-    elif isinstance(block, ListValue.ListChild):
-        return block.id
-    elif isinstance(block, ListValue):
-        return block.block.name
-    elif isinstance(block, (blocks.StructValue, blocks.BoundBlock)):
-        return block.block.name
-    else:
-        raise ValueError("Unknown block type: %s" % type(block))
-
-def find_block(block_id, field, contentpath=None):
-    """
-    Find a block in a StreamField or ListBlock by its ID.
-    """
-    if contentpath is None:
-        contentpath = []
-
-    # Check and cast field to iterable if necessary, but do not append non-StreamValue names to contentpath here.
-    if not isinstance(field, StreamValue) and not hasattr(field, "__iter__"):
-        field = [field]
-
-    # Adjust for ListValue to get the iterable bound_blocks.
-    if isinstance(field, ListValue):
-        field = field.bound_blocks
-
-    for block in field:
-        # Determine the block's name only if needed to avoid premature addition to contentpath.
-        block_name = get_block_path(block)
-        
-        if getattr(block, "id", None) == block_id:
-            # Append the block name here as it directly leads to the target.
-            return block, contentpath + [block_name]
-        
-        # Prepare to check children without altering the current path yet.
-        if isinstance(block.value, blocks.StructValue):
-            for _, value in block.value.bound_blocks.items():
-                found, found_path = find_block(block_id, value, contentpath + [block_name])
-                if found:
-                    return found, found_path
-
-        elif isinstance(block.value, (StreamValue, StreamValue.StreamChild, ListValue)):
-            found, found_path = find_block(block_id, block.value, contentpath + [block_name])
-            if found:
-                return found, found_path
-
-    # Return None and the current path if no block is found at this level.
-    return None, contentpath
-
-
-
-_renderer_map = {}
-_field_renderer_map = {}
-_looked_for_renderers = False
-
-
-def _look_for_renderers():
-    global _looked_for_renderers
-    if not _looked_for_renderers:
-        for hook in hooks.get_hooks(REGISTER_TYPE_RENDERER):
-            hook(_renderer_map)
-
-        for hook in hooks.get_hooks(REGISTER_FIELD_RENDERER):
-            hook(_field_renderer_map)
-
-        _looked_for_renderers = True
-
-
-def get_field_content(request, instance, meta_field: models.Field, context, content=None):
-    """
-    Return the content for a field on a model.
-    Also checks the model for a rendering method.
-    The method should be named `render_fedit_{field_name}`.
-    We wil also check for any hooks which may convert the content.
-    """
-    _look_for_renderers()
-
-    if isinstance(meta_field, str):
-        meta_field = instance._meta.get_field(meta_field)
-
-    if hasattr(context, "flatten"):
-        context = context.flatten()
-
-    if not content:
-        # Check for a rendering method if it exists
-        if hasattr(instance, f"render_fedit_{meta_field.name}"):
-            content = getattr(instance, f"render_fedit_{meta_field.name}")(request, context=context)
-        else:
-            content = getattr(instance, meta_field.name)
+    def checks(self, request: HttpRequest, object: Any) -> None:
+        super().checks(request, object)
+        if not isinstance(self.object, PreviewableMixin):
+            raise ValueError("Model {} does not inherit from PreviewableMixin, cannot edit.".format(self.model))
+
+    def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
+        # # Check if lock applies to this user
+        # if not self.locked_for_user:
+        self.request = with_userbar_model(self.request, self.object)
+
+        object: PreviewableMixin = self.object
+        return object.make_preview_request(original_request=self.request, extra_request_attrs={
+            FEDIT_PREVIEW_VAR: True,
+            USERBAR_MODEL_VAR: self.object,
+        })
+    
+
+class BaseActionView(LockViewMixin, BaseFeditView):
+    template_name         = "wagtail_fedit/editor/action_confirm.html"
+    required_superclasses = [DraftStateMixin]
+    action_icon            = None
+    action_text            = None
+    title_format           = None
+    action_help_text_title = None
+    action_help_text       = None
+
+    def get_action(self) -> str:
+        return self.action_text
+    
+    def get_action_value(self) -> str:
+        return f"{self.__class__.__name__.lower()}"
+
+    def get_action_title(self) -> str:
+        return self.title_format.format(self.object)
+    
+    def get_action_help_text_title(self) -> str:
+        return self.action_help_text_title
+    
+    def get_action_help_text(self) -> str:
+        return self.action_help_text
+    
+    def get_action_icon(self) -> str:
+        return self.action_icon
+    
+    def setup(self, request: HttpRequest, object_id: Any, app_label: str, model_name: str) -> HttpResponse:
+        super().setup(request, object_id, app_label, model_name)
+        self.policy = self.object.permissions_for_user(request.user)
+
+        if not isinstance(self.object, tuple(self.required_superclasses)):
+            self.error_response = HttpResponseBadRequest(
+                "Model {} does not inherit from {}".format(
+                    self.model.__name__, ", ".join([cls.__name__ for cls in self.required_superclasses])
+                )
+            )
 
-    for k, v in _field_renderer_map.items():
-        if isinstance(meta_field, k):
-            content = v(request, context, instance, content)
-            break
-
-    for k, v in _renderer_map.items():
-        if isinstance(content, k):
-            content = v(request, context, instance, content)
-            break
-
-    # The content might be a streamblock etc, we can render it as a block
-    # if isinstance(content, (blocks.BoundBlock, blocks.StructValue)):
-    if hasattr(content, "render_as_block"):
-        content = content.render_as_block(context)
-
-    return content
-
-def is_draft_capable(model):
-    """
-    Check if a model is capable of drafts.
-    """
-    return isinstance(model, DraftStateMixin)\
-        or type(model) == type\
-        and issubclass(model, DraftStateMixin)
-
-def model_diff(m1, m2):
-    """
-    Check if two model instances are different based on their type and primary key.
-    Does not check for differences in the model's fields.
-    This is used to determine if a relation is being saved.
-    """
-    return not (
-        m1._meta.app_label == m2._meta.app_label
-        and m1._meta.model_name == m2._meta.model_name\
-        and m1.pk == m2.pk
-    )
-
-
-def edit_url(instance: models.Model, request: HttpRequest, hash = None, **params) -> str:
-    """
-        Return the edit URL for a given object and user (or request instead of user.)
-        If none exists and the model is an instance of PreviewableMixin;
-        return the wagtail_fedit:editable url; else an empty string.
-    """
-
-    user = request.user
-    finder = AdminURLFinder(user)
-    admin_url = finder.get_edit_url(instance)
-
-    if not admin_url:
-
-        # Check if the instance is a PreviewableMixin
-        # and the user has permission to edit it.
-        if isinstance(instance, PreviewableMixin)\
-                and _can_edit(request, instance):
-            
-            admin_url = reverse(
+    def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
+        return super().get_context_data(**kwargs) | {
+            "action": self.get_action_value(),  # e.g. "publishview"
+            "action_text": self.get_action(),
+            "action_title": self.get_action_title(),
+            "action_help_text_title": self.get_action_help_text_title(),
+            "action_help_text": self.get_action_help_text(),
+            "action_icon": self.get_action_icon(),
+            "cancel_url": reverse(
                 "wagtail_fedit:editable",
-                args=[
-                    instance.pk,
-                    instance._meta.app_label,
-                    instance._meta.model_name
-                ],
+                args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
+            ),
+        }
+
+    def redirect_to_success_url(self, request: HttpRequest) -> HttpResponse:
+        if hasattr(self.object, "get_url"):
+            return redirect(self.object.get_url(request))
+        
+        elif hasattr(self.object, "get_absolute_url"):
+            return redirect(self.object.get_absolute_url())
+        
+        return redirect(reverse(
+            "wagtail_fedit:editable",
+            args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
+        ))
+
+    def redirect_to_failsafe_url(self, request: HttpRequest) -> HttpResponse:
+        try:
+            finder = AdminURLFinder(request.user)
+            edit_url = finder.get_edit_url(self.object)
+            return redirect(edit_url)
+        except Exception:
+            return redirect(reverse(
+                "wagtail_fedit:editable",
+                args=[self.object.pk, self.model._meta.app_label, self.model._meta.model_name],
+            ))
+        
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        pass
+
+    def action(self, request: HttpRequest) -> HttpResponse:
+        raise NotImplementedError("Subclasses must implement this method")
+    
+    def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
+        
+        if getattr(settings, "WAGTAIL_WORKFLOW_ENABLED", True) and issubclass(self.model, WorkflowMixin):
+            # Retrieve current workflow state if set, default to last workflow state
+            self.workflow_state = (
+                self.object.current_workflow_state
+                or self.object.workflow_states.order_by("created_at").last()
             )
         else:
-            return ""
+            self.workflow_state = None
 
-    data = urlencode(params)
-    if params:
-        admin_url = f"{admin_url}?{data}"
+        try:
+            self.check_policy(request, self.policy)
+        except ValueError as e:
+            messages.error(request, str(e))
+            return self.get(request, *args, **kwargs)
+
+        # Check if lock applies to this user
+        if self.locked_for_user:
+            messages.error(request, _("This object is locked. It cannot be acted upon."))
+            return self.redirect_to_failsafe_url(request)
+        
+        if "action" not in request.POST:
+            messages.error(request, _("No action specified"))
+            return self.get(request, *args, **kwargs)
+        
+        if request.POST["action"] != self.get_action_value():
+            messages.error(request, _("Invalid action specified: {}").format(request.POST["action"]))
+            return self.get(request, *args, **kwargs)
+        
+        return self.action(request)
 
-    if hash:
-        admin_url = f"{admin_url}#{hash}"
-    
-    return admin_url
 
+class PublishView(BaseActionView):
+    template_name = "wagtail_fedit/editor/action_publish_confirm.html"
+    required_superclasses = [DraftStateMixin, RevisionMixin]
+    action_text = _("Publish")
+    action_icon = "fedit-eye-open"
 
-def get_model_string(instance: models.Model, publish_url: bool = False, request: HttpRequest = None, target = "_blank", **params) -> str:
-    """
-    Get a string representation of a model instance. If the instance has a
-    `get_admin_display_title` method, it will be used to get the string
-    representation.
-    If that method does not exist, the `title` attribute will be used.
-    If the `title` attribute does not exist, the string representation of the
-    instance will be used.
-    If `publish_url` is True, the string will be wrapped in an anchor tag
-    linking to the publish view for the instance.
-    Permissions will not be checked. This is the responsibility of the caller.
-    """
-    model_string = getattr(instance, "get_admin_display_title", None)
-    if model_string:
-        model_string = model_string()
-    else:
-        model_string = getattr(instance, "title", str(instance))
-
-    if publish_url:
-
-        if is_draft_capable(instance):
-            admin_url = reverse(
-                "wagtail_fedit:publish",
-                args=[
-                    instance.pk,
-                    instance._meta.app_label,
-                    instance._meta.model_name
-                ],
-            )
+    def get_action_title(self):
+        return _("Publishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
+
+    def get_action_help_text_title(self):
+        return _("About publishing")
+
+    def get_action_help_text(self):
+        s = [
+            _("Publishing this object will make it visible to users on the site."),
+            _("That means that any changes you make will be immediately visible to everyone."),
+        ]
 
-            data = urlencode(params)
-            if params:
-                admin_url = f"{admin_url}?{data}"
+        if self.policy.can_unpublish():
+            s.append(_("You can always choose to unpublish it."))
 
+        return s
+    
+    def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
+        context = super().get_context_data(**kwargs)
+
+        log_entry_count = 0
+        log_entry_model = registry.get_log_model_for_model(self.object.__class__)
+        if issubclass(log_entry_model, PageLogEntry):
+            log_entries = log_entry_model.objects\
+                .filter(page=self.object)\
+                .order_by("-timestamp")
+            
+            context["view_more_url"] = reverse(
+                "wagtailadmin_pages:history",
+                args=[self.object.pk],
+            )
+                
+        elif issubclass(log_entry_model, ModelLogEntry):
+            log_entries = log_entry_model.objects\
+                .filter(object_id=self.object.pk)\
+                .order_by("-timestamp")
+                
         else:
-            admin_url = edit_url(instance, request, **params)
+            log_entries = None
 
-        if admin_url:
-            model_string = mark_safe(
-                f'<a href="{admin_url}" target="{target}">{model_string}</a>'
+        if log_entries:
+            log_entries = log_entries.filter(
+                timestamp__gt=models.Subquery(
+                    log_entries.filter(action="wagtail.publish")\
+                               .values("timestamp")\
+                               .order_by("-timestamp")[:1]
+                )
             )
 
-    return model_string
+            log_entries = log_entries.select_related(
+                "revision", "user", "user__wagtail_userprofile",
+            )
 
-def _can_edit(request, obj: models.Model):
-    """
-    Check if the user has appropriate permissions to edit an object.
-    Also requires the current request be on the `wagtail_fedit:editable` url
-    (Or the preview variable to be True)
-    """
-    if not request or not obj:
-        return False
-    
-    return (
-        FeditPermissionCheck.has_perms(request, obj)\
-        and getattr(request, FEDIT_PREVIEW_VAR, False)
-    )
-
-def user_can_publish(instance, user, check_for_changes: bool = True):
-    """
-    Check if a user can publish an object.
-    Mostly comes from PagePermissionTester.can_publish
-    """
-    if not isinstance(instance, DraftStateMixin):
-        return False
-    
-    if not instance.has_unpublished_changes\
-        and check_for_changes:
-        return False
+            # if not self.request.user.is_superuser or\
+            #    not self.request.user.is_staff:
+            #     log_entries = log_entries.filter(user=self.request.user)
+
+            if isinstance(self.object, Page):
+                log_entries = log_entries.select_related("page")
+            else:
+                log_entries = log_entries.select_related("content_type")
+
+            log_entry_count = log_entries.count()
+            log_entries = log_entries[:MAX_LOG_ENTRIES_DISPLAYED]
+
+        context.update({
+            "log_entries": log_entries,
+            "has_more_entries": log_entry_count > MAX_LOG_ENTRIES_DISPLAYED,
+            "log_entry_count": log_entry_count,
+            "last_published_at": self.object.last_published_at,
+            "is_page": isinstance(self.object, Page),
+        })
 
-    if hasattr(instance, "permission_policy"):
-        return instance.permission_policy.user_has_permission(user, "publish")
-    
-    if not hasattr(instance, "permissions_for_user"):
-        return False
+        return context
 
-    return instance.permissions_for_user(user).can_publish()
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not policy.can_publish():
+            raise ValueError("User does not have permission to publish")
+        
+        if self.locked_for_user:
+            raise ValueError("Object is locked")
+        
+        if not self.object.has_unpublished_changes:
+            raise ValueError("Object has no unpublished changes")
 
-def user_can_unpublish(instance, user):
-    """
-    Check if a user can unpublish an object.
-    Mostly comes from PagePermissionTester.can_unpublish
-    """
-    if not isinstance(instance, DraftStateMixin):
-        return False
-    
-    if not hasattr(instance, "permissions_for_user"):
-        return False
-    
-    return instance.permissions_for_user(user).can_unpublish()
+    def action(self, request: HttpRequest) -> HttpResponse:
+        latest_revision = self.object.latest_revision
 
-def user_can_submit_for_moderation(instance, user, check_for_changes: bool = True):
-    """
-    Check if a user can submit an object for moderation.
-    Mostly comes from PagePermissionTester.can_submit_for_moderation
-    """
-    if not getattr(settings, "WAGTAIL_WORKFLOW_ENABLED", True):
-        return False
-
-    if not instance.has_unpublished_changes\
-        and check_for_changes:
-        return False
+        if not latest_revision:
+            latest_revision = self.object.save_revision(
+                user=request.user,
+            )
 
-    if not isinstance(instance, WorkflowMixin):
-        return False
-    
-    if not hasattr(instance, "permissions_for_user"):
-        return False
-    
-    return instance.permissions_for_user(user).can_submit_for_moderation()
+        action = get_publish_action(self.object)(
+            revision=latest_revision,
+            user=request.user,
+        )
 
+        action.execute()
 
-_lock_info = namedtuple("lock_info", ["lock", "locked_for_user"])
+        if latest_revision:
+            self.object = latest_revision.as_object()
 
-def lock_info(object, user) -> _lock_info:
-    """
-        Returns the Lock instance (if any) and whether it is locked for the given user.
-    """
-    if isinstance(object, LockableMixin):
-        lock = object.get_lock()
-        locked_for_user = lock is not None and lock.for_user(
-            user
+        return self.redirect_to_success_url(request)
+
+
+class UnpublishView(BaseActionView):
+    required_superclasses = [DraftStateMixin]
+    action_icon = "fedit-eye-closed"
+    action_text = _("Unpublish")
+    action_help_text_title = _("About unpublishing")
+    action_help_text = [
+        _("Unpublishing this object will make it invisible to users on the site."),
+        _("That means that it will no longer be visible to anyone."),
+        _("You can always choose to publish it again."),
+    ]
+
+    def get_action_title(self):
+        return _("Unpublishing {} \"{}\"").format(self.object._meta.verbose_name, self.object)
+    
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not policy.can_unpublish():
+            raise ValueError("User does not have permission to unpublish")
+        
+        if self.locked_for_user:
+            raise ValueError("Object is locked")
+        
+        if not self.object.live:
+            raise ValueError("Object is not live")
+ 
+    def action(self, request: HttpRequest) -> HttpResponse:
+        if not self.object.live:
+            messages.error(request, _("This object is not live"))
+            return self.get(request)
+        
+        action = get_unpublish_action(self.object)(
+            self.object,
+            user=request.user,
         )
-    else:
-        lock = None
-        locked_for_user = False
-
-    return _lock_info(lock, locked_for_user)
 
+        action.execute()
 
-def get_hooks(hook_name):
-    """
-        Return the hooks for a given hook name in the wagtail_fedit namespace.
-    """
-    for hook in hooks.get_hooks(f"wagtail_fedit.{hook_name}"):
-        yield hook
+        return self.redirect_to_failsafe_url(request)
 
-    
-def _resolve_expressions(context, *expressions):
-    """
-        Resolve a list of possible templatetag filterexpressions.
-    """
-    def _map(expression):
-        if isinstance(expression, FilterExpression):
-            return expression.resolve(context)
-        return expression
-    
-    return tuple(map(_map, expressions))
+
+class SubmitView(BaseActionView):
+    required_superclasses = [DraftStateMixin, WorkflowMixin, RevisionMixin]
+    action_icon = "fedit-check-list"
+    action_text = _("Submit for moderation")
+    action_help_text_title = _("About submitting for moderation")
+    action_help_text = [
+        _("Submitting this object for moderation will make it invisible to users on the site."),
+        _("That means that it will no longer be visible to anyone."),
+        _("You can always choose to publish it again."),
+    ]
+
+    def get_action_title(self):
+        return _("Submitting {} \"{}\" for moderation").format(self.object._meta.verbose_name, self.object)
+
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not policy.can_submit_for_moderation():
+            raise ValueError("User does not have permission to submit for moderation")
+        
+        if not self.object.has_unpublished_changes:
+            raise ValueError("Object has no unpublished changes")
+   
+    def action(self, request: HttpRequest) -> HttpResponse:
+        
+        latest_revision = getattr(self.object, "latest_revision", None)
+        if not latest_revision:
+            latest_revision = self.object.save_revision(
+                user=request.user,
+            )
+
+        if (
+            self.workflow_state
+            and self.workflow_state.status == WorkflowState.STATUS_NEEDS_CHANGES
+        ):
+            # If the workflow was in the needs changes state, resume the existing workflow on submission
+            self.workflow_state.resume(self.request.user)
+        else:
+            # Otherwise start a new workflow
+            workflow = self.object.get_workflow()
+            workflow.start(self.object, self.request.user)
+
+        return self.redirect_to_success_url(request)
+
+
+class CancelView(BaseActionView):
+    required_superclasses = [DraftStateMixin, WorkflowMixin]
+    action_icon = "fedit-stop-sign"
+    action_text = _("Cancel Workflow")
+    action_help_text_title = _("About cancelling workflows")
+    action_help_text = [
+        _("Cancelling the workflow for this object will remove it from the moderation process."),
+        _("That means that it will no longer be visible to anyone."),
+        _("You can always choose to submit it for moderation again."),
+    ]
+
+    def get_action_title(self):
+        return _("Cancelling workflow for {} \"{}\"").format(self.object._meta.verbose_name, self.object)
+
+    def check_policy(self, request: HttpRequest, policy: FeditPermissionCheck) -> None:
+        if not self.workflow_state:
+            raise ValueError("No workflow state found")
+        
+        if not self.workflow_state.user_can_cancel(request.user):
+            raise ValueError("User does not have permission to cancel this workflow")
+
+    def action(self, request: HttpRequest) -> HttpResponse:
+        if self.workflow_state:
+            self.workflow_state.cancel(user=self.request.user)
+            return self.redirect_to_success_url(request)
+        
+        return self.get(request)
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.7/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from django.urls import reverse
+from django.conf import settings
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.templatetags.static import static
 from django.utils.translation import gettext_lazy as _
-from wagtail.models import WorkflowMixin
+from wagtail.models import (
+    WorkflowMixin,
+)
 from wagtail.admin.userbar import (
     BaseItem,
     AddPageItem,
     ExplorePageItem,
     EditPageItem,
 )
 from wagtail import hooks
@@ -48,15 +51,16 @@
     action_icon = "fedit-eye-open"
     action_text = _("Publish")
     
     def is_shown(self, request):
         if not super().is_shown(request):
             return False
         
-        return user_can_publish(self.instance, request.user, check_for_changes=False)
+        return user_can_publish(self.instance, request.user, check_for_changes=False)\
+               and self.instance.has_unpublished_changes
 
 class UserBarActionUnpublishComponent(FeditableModelComponent):
     action_url = "wagtail_fedit:unpublish"
     action_icon = "fedit-eye-closed"
     action_text = _("Unpublish")
         
     def is_shown(self, request):
@@ -70,15 +74,16 @@
     action_icon = "fedit-check-list"
     action_text = _("Submit for moderation")
 
     def is_shown(self, request):
         if not super().is_shown(request):
             return False
         
-        return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=False)
+        return user_can_submit_for_moderation(self.instance, request.user, check_for_changes=False)\
+               and self.instance.has_unpublished_changes
 
 class UserBarActionCancelComponent(FeditableModelComponent):
     action_url = "wagtail_fedit:cancel"
     action_icon = "fedit-stop-sign"
     action_text = _("Cancel Workflow")
 
     def is_shown(self, request):
@@ -87,19 +92,29 @@
         
         if not is_draft_capable(self.instance):
             return False
         
         if not isinstance(self.instance, WorkflowMixin):
             return False
         
-        workflow_state = self.instance.current_workflow_state
-        return workflow_state and (
-            workflow_state.status == workflow_state.STATUS_IN_PROGRESS or\
-            workflow_state.status == workflow_state.STATUS_NEEDS_CHANGES
-        )
+        if not getattr(settings, "WAGTAIL_WORKFLOW_ENABLED", True):
+            return False
+        
+        wf_state = self.instance.current_workflow_state or\
+            self.instance.workflow_states.order_by("created_at").last()
+
+        return wf_state and\
+            wf_state.status in\
+                (wf_state.STATUS_IN_PROGRESS, wf_state.STATUS_NEEDS_CHANGES)
+
+        # workflow_state = self.instance.current_workflow_state
+        # return workflow_state and (
+        #     workflow_state.status == workflow_state.STATUS_IN_PROGRESS or\
+        #     workflow_state.status == workflow_state.STATUS_NEEDS_CHANGES
+        # )
 
 class BaseWagtailFeditItem(BaseItem, FeditPermissionCheck):
     def __init__(self, model):
         self.model = model
 
     def get_context_data(self, request):
         context = super().get_context_data(request)
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.7/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.4.6
+Version: 1.4.7
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -88,19 +88,18 @@
        <title>Document</title>
        <link rel="stylesheet" href="{% static 'wagtail_fedit/css/frontend.css' %}">
    </head>
    <body>
        {# Adress the model.field or model.my.related.field you wish to edit. #}
        {# Editable fields get a special `inline` argument. #}
        {# if True the button is not placed with an absolute CSS position. #}
-       <h1>{% fedit_field self.title inline=True or False %}</h1>
+       <h1>{% fedit field self.title inline=True or False %}</h1>
 
-       {# Pass in the field_name and the model instance on which that field resides if you are using `wagtail_fedit <= 1.3.8` #}
        <main class="my-streamfield-content">
-           {% fedit_field "content" self %}
+           {% fedit field self.content %}
        </main>
 
        {% wagtailuserbar %}
 
        <script src="{% static 'wagtail_fedit/js/frontend.js' %}"></script>
    </body>
    </html>
@@ -116,15 +115,15 @@
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
        {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
        {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
-       {% fedit_block block=block block_id=block.id field_name="content" model=self %}
+       {% fedit block self.content block=block block_id=block.id %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
    ...
@@ -132,17 +131,24 @@
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
        def render_fedit_content(self, request):
            return render_to_string("myapp/render_my_field.html", self.get_context(request))
    ```
 
-   Your content will then automatically be rendered with that method when need be by using `{% fedit_field "content" self %} `
+   Your content will then automatically be rendered with that method when need be by using
+   `{% fedit field self.content %} `
 4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
+**Note:** If the parent block is wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance variable and field name should be omitted and replaced with `from_context`.
+Example: `{% fedit block from_context block=item block_id=item.id %}`
+The parent- blocktag will share these variables through context.
+This makes it possibly to easily use editable sub-blocks across multiple different model types.
+If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
+
 ## Permissions
 
 **Note: This is not required for pages.**
 
 **The `Page` model already provides this interface.**
 
 We have the following basic permission requirements:
@@ -214,23 +220,18 @@
 This is done by accessing the `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for the toplevel block!)*
 
 Our new loop would then be:
 
 ```django-html
 {% for item in self.items.bound_blocks %}
     {# Field name and model are the same arguments as in the first example! #}
-    {% fedit_block block=item block_id=item.id field_name="content" model=my_model_instance_var %}
+    {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
-**Note:** If the parent block is wrapped with `fedit_block` or `fedit_field` the field_name and model argument can be omitted.
-The parent- blocktag will share these variables through context.
-This makes it possibly to easily use editable sub-blocks across multiple different model types.
-If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
-
 ## Hooks
 
 ### wagtail_fedit.construct_block_toolbar
 
 Construct the toolbar for the given block.
 This is used to display the edit icon in the block.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.6 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.7 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -34,94 +34,92 @@
 Editing! 1. Make sure the models you wish to edit inherit from
 PreviewableMixin. **This is a requirement.** 2. Define a template for your
 model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
 the required template tag libraries #}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {#
 Editable fields get a special `inline` argument. #} {# if True the button is
 not placed with an absolute CSS position. #}
-************ {{%% ffeeddiitt__ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
-{# Pass in the field_name and the model instance on which that field resides if
-you are using `wagtail_fedit <= 1.3.8` #} {% fedit_field "content" self %} {%
-wagtailuserbar %}
+************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
+{% fedit field self.content %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
 fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
 do not require the field_name or model argument. #} {# This is taken from the
 parent (also wrapped by `fedit_block`); the model and field name are shared
-through context. #} {% fedit_block block=block block_id=block.id
-field_name="content" model=self %} {% endfor %} ``` ```python from
-django.template.loader import render_to_string ... class MyPage(...): # Can be
-any type of model. content = StreamField(...) def render_fedit_content(self,
-request): return render_to_string("myapp/render_my_field.html",
-self.get_context(request)) ``` Your content will then automatically be rendered
-with that method when need be by using `{% fedit_field "content" self %} ` 4.
-**But wait?! I go to my template and I do not see a way to edit!**That is true!
-We try to protect any styling on your actual page; we do not want to
-interfere.Instead; we serve the editing interface on a different URL,
-accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye
-on that userbar! It is also used for publishing if your model inherits from
-`DraftStateMixin`. ## Permissions **Note: This is not required for pages.**
-**The `Page` model already provides this interface.** We have the following
-basic permission requirements: * You must have `wagtailadmin.access_admin` to
-edit a block/field. * You must have the appropriate `app_label.change_*`
-permission for the model. This however only applies to editing. We use separate
-permissions for publishing and submitting workflows, etc. Models which you want
-to allow the publish view for should also implement a `PermissionTester`- like
-object. Example of how you should implement the `Tester` object and all
-required permissions. (More details in `models.py`) ```python class MyModel
-(...): def permissions_for_user(self, user): return MyModelPermissionTester
-(self, user) class MyModelPermissionTester(...): def can_unpublish(self): """
-Can the user unpublish this object? (Required for un-publishing""" def
-can_publish(self): """ Can the user publish this object? (Required for
-publishing)""" def can_submit_for_moderation(self): """ Can the user submit
-this object for moderation? (Optional) """ ``` ## Revisions Revision support is
-included out of the box. If your model inherits from a `RevisionMixin`, we will
-automatically create drafts for you. These will not be published (If the model
-inherits from `DraftStateMixin`) until you choose to do so. ## Workflows We
-include a `WorkFlow` to submit this object for moderation. More workflow
-support will be included in the future. ## Logs Logs are also included out of
-the box. We will automatically update your model's history; including possible
-revisions. This will allow you to backtrack each change made on the frontend.
-This however does mean that a possibly large amount of data will be stored in
-your database. ## Caveats Wagtail does not always make it's `id` attribute
-available. This is only available to instances of `StreamChild` and
-`ListChild`. Consider the following regular wagtail list loop where `items` is
-a `ListBlock`. ```django-html {% for item in self.items %} {% include_block
-item %} {# No access to ID! Cannot edit! #} {% endfor %} ``` To make this an
-editable block instead; we would slightly change the loop to make the block's
-`id` available. This is done by accessing the `bound_blocks` of that ListBlock
-*(`StreamBlock` does this automatically for the toplevel block!)* Our new loop
-would then be: ```django-html {% for item in self.items.bound_blocks %} {#
-Field name and model are the same arguments as in the first example! #} {%
-fedit_block block=item block_id=item.id field_name="content"
-model=my_model_instance_var %} {% endfor %} ``` **Note:** If the parent block
-is wrapped with `fedit_block` or `fedit_field` the field_name and model
-argument can be omitted. The parent- blocktag will share these variables
-through context. This makes it possibly to easily use editable sub-blocks
-across multiple different model types. If your model **ISN'T** capable of
-editing; or these variables aren't shared - your block will be rendered as
-normal. ## Hooks ### wagtail_fedit.construct_block_toolbar Construct the
-toolbar for the given block. This is used to display the edit icon in the
-block. How it is called: ```python for hook in hooks.get_hooks
-(CONSTRUCT_BLOCK_TOOLBAR): hook(request=request, items=items, model=model,
-block_id=block_id, field_name=field_name) ``` ###
-wagtail_fedit.construct_field_toolbar Construct the toolbar for the given
-field. This is used to display the edit icon in the field. How it is called:
-```python for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR): hook
-(request=request, items=items, model=model, field_name=field_name) ``` ###
-wagtail_fedit.register_type_renderer Register a custom renderer for a type.
-Example of how this type of renderer can be used: ```python @hooks.register
-(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): # This is a
-custom renderer for the Page model. # It will render the Page model as a simple
-h2 tag. renderer_map[Page] = lambda request, context, instance, value:
-format_html( '
+through context. #} {% fedit block self.content block=block block_id=block.id
+%} {% endfor %} ``` ```python from django.template.loader import
+render_to_string ... class MyPage(...): # Can be any type of model. content =
+StreamField(...) def render_fedit_content(self, request): return
+render_to_string("myapp/render_my_field.html", self.get_context(request)) ```
+Your content will then automatically be rendered with that method when need be
+by using `{% fedit field self.content %} ` 4. **But wait?! I go to my template
+and I do not see a way to edit!**That is true! We try to protect any styling on
+your actual page; we do not want to interfere.Instead; we serve the editing
+interface on a different URL, accessible by clicking `Frontend Editing` in the
+Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if
+your model inherits from `DraftStateMixin`. **Note:** If the parent block is
+wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance
+variable and field name should be omitted and replaced with `from_context`.
+Example: `{% fedit block from_context block=item block_id=item.id %}` The
+parent- blocktag will share these variables through context. This makes it
+possibly to easily use editable sub-blocks across multiple different model
+types. If your model **ISN'T** capable of editing; or these variables aren't
+shared - your block will be rendered as normal. ## Permissions **Note: This is
+not required for pages.** **The `Page` model already provides this interface.**
+We have the following basic permission requirements: * You must have
+`wagtailadmin.access_admin` to edit a block/field. * You must have the
+appropriate `app_label.change_*` permission for the model. This however only
+applies to editing. We use separate permissions for publishing and submitting
+workflows, etc. Models which you want to allow the publish view for should also
+implement a `PermissionTester`- like object. Example of how you should
+implement the `Tester` object and all required permissions. (More details in
+`models.py`) ```python class MyModel(...): def permissions_for_user(self,
+user): return MyModelPermissionTester(self, user) class MyModelPermissionTester
+(...): def can_unpublish(self): """ Can the user unpublish this object?
+(Required for un-publishing""" def can_publish(self): """ Can the user publish
+this object? (Required for publishing)""" def can_submit_for_moderation(self):
+""" Can the user submit this object for moderation? (Optional) """ ``` ##
+Revisions Revision support is included out of the box. If your model inherits
+from a `RevisionMixin`, we will automatically create drafts for you. These will
+not be published (If the model inherits from `DraftStateMixin`) until you
+choose to do so. ## Workflows We include a `WorkFlow` to submit this object for
+moderation. More workflow support will be included in the future. ## Logs Logs
+are also included out of the box. We will automatically update your model's
+history; including possible revisions. This will allow you to backtrack each
+change made on the frontend. This however does mean that a possibly large
+amount of data will be stored in your database. ## Caveats Wagtail does not
+always make it's `id` attribute available. This is only available to instances
+of `StreamChild` and `ListChild`. Consider the following regular wagtail list
+loop where `items` is a `ListBlock`. ```django-html {% for item in self.items
+%} {% include_block item %} {# No access to ID! Cannot edit! #} {% endfor %}
+``` To make this an editable block instead; we would slightly change the loop
+to make the block's `id` available. This is done by accessing the
+`bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
+the toplevel block!)* Our new loop would then be: ```django-html {% for item in
+self.items.bound_blocks %} {# Field name and model are the same arguments as in
+the first example! #} {% fedit block my_model_instance_var.content_field
+block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
+wagtail_fedit.construct_block_toolbar Construct the toolbar for the given
+block. This is used to display the edit icon in the block. How it is called:
+```python for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR): hook
+(request=request, items=items, model=model, block_id=block_id,
+field_name=field_name) ``` ### wagtail_fedit.construct_field_toolbar Construct
+the toolbar for the given field. This is used to display the edit icon in the
+field. How it is called: ```python for hook in hooks.get_hooks
+(CONSTRUCT_FIELD_TOOLBAR): hook(request=request, items=items, model=model,
+field_name=field_name) ``` ### wagtail_fedit.register_type_renderer Register a
+custom renderer for a type. Example of how this type of renderer can be used:
+```python @hooks.register(REGISTER_TYPE_RENDERER) def register_renderers
+(renderer_map): # This is a custom renderer for the Page model. # It will
+render the Page model as a simple h2 tag. renderer_map[Page] = lambda request,
+context, instance, value: format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
```

### Comparing `wagtail_fedit-1.4.6/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.7/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,35 +12,41 @@
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
 wagtail_fedit.egg-info/top_level.txt
+wagtail_fedit/adapters/__init__.py
+wagtail_fedit/adapters/base.py
+wagtail_fedit/adapters/block.py
+wagtail_fedit/adapters/field.py
+wagtail_fedit/adapters/registry.py
 wagtail_fedit/forms/__init__.py
 wagtail_fedit/forms/blocks.py
 wagtail_fedit/forms/fields.py
 wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
+wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
-wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
-wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
@@ -58,33 +64,32 @@
 wagtail_fedit/test/core/migrations/0001_initial.py
 wagtail_fedit/test/core/migrations/0002_basicmodel.py
 wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
 wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
 wagtail_fedit/test/core/migrations/__init__.py
 wagtail_fedit/test/core/tests/__init__.py
 wagtail_fedit/test/core/tests/base.py
+wagtail_fedit/test/core/tests/test_adapters.py
 wagtail_fedit/test/core/tests/test_block_edit.py
-wagtail_fedit/test/core/tests/test_block_templatetag.py
 wagtail_fedit/test/core/tests/test_blocks.py
 wagtail_fedit/test/core/tests/test_field_edit.py
-wagtail_fedit/test/core/tests/test_field_templatetag.py
 wagtail_fedit/test/core/tests/test_generic.py
 wagtail_fedit/test/core/tests/test_revision.py
 wagtail_fedit/test/core/tests/test_submit.py
 wagtail_fedit/test/testapp/__init__.py
 wagtail_fedit/test/testapp/asgi.py
 wagtail_fedit/test/testapp/settings.py
 wagtail_fedit/test/testapp/urls.py
 wagtail_fedit/test/testapp/wsgi.py
 wagtail_fedit/views/__init__.py
-wagtail_fedit/views/blocks.py
+wagtail_fedit/views/adapters.py
 wagtail_fedit/views/editable.py
-wagtail_fedit/views/fields.py
 wagtail_fedit/views/mixins.py
 wagtail_fedit/wagtail_hooks/__init__.py
 wagtail_fedit/wagtail_hooks/action_menu.py
+wagtail_fedit/wagtail_hooks/adapter_registry.py
 wagtail_fedit/wagtail_hooks/excluded_relations.py
 wagtail_fedit/wagtail_hooks/icons.py
 wagtail_fedit/wagtail_hooks/log_actions.py
 wagtail_fedit/wagtail_hooks/renderers.py
 wagtail_fedit/wagtail_hooks/urls.py
 wagtail_fedit/wagtail_hooks/userbar.py
```

