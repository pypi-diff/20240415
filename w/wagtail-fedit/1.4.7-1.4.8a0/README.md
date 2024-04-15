# Comparing `tmp/wagtail_fedit-1.4.7.tar.gz` & `tmp/wagtail_fedit-1.4.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.4.7.tar", last modified: Mon Apr 15 16:22:54 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.4.8a0.tar", last modified: Mon Apr 15 17:39:07 2024, max compression
```

## Comparing `wagtail_fedit-1.4.7.tar` & `wagtail_fedit-1.4.8a0.tar`

### file list

```diff
@@ -1,127 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.307673 wagtail_fedit-1.4.7/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0    13123 2024-04-15 16:22:54.307673 wagtail_fedit-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0    11925 2024-04-15 16:22:37.000000 wagtail_fedit-1.4.7/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-04-15 16:22:54.319259 wagtail_fedit-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.026410 wagtail_fedit-1.4.7/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.7/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.078014 wagtail_fedit-1.4.7/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      294 2024-04-13 11:18:53.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0     3762 2024-04-13 19:50:56.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0     3857 2024-04-15 16:08:58.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     7523 2024-04-13 11:18:27.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.4.7/wagtail_fedit/adapters/registry.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.7/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.081415 wagtail_fedit-1.4.7/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.7/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.7/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     3588 2024-04-13 07:17:52.000000 wagtail_fedit-1.4.7/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.982963 wagtail_fedit-1.4.7/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.983961 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.104776 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.105785 wagtail_fedit-1.4.7/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.7/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.107883 wagtail_fedit-1.4.7/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.7/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.987043 wagtail_fedit-1.4.7/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.988042 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.143397 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.168557 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    16161 2024-04-15 15:58:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.989043 wagtail_fedit-1.4.7/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:53.993231 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.191937 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.203892 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      386 2024-04-13 11:13:58.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
--rw-rw-rw-   0        0        0      302 2024-04-06 22:07:59.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      335 2024-04-06 22:08:01.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.220775 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.227410 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.245121 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.256895 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.259941 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.262957 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     9097 2024-04-14 13:32:19.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0     6514 2024-04-14 13:32:17.000000 wagtail_fedit-1.4.7/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.264906 wagtail_fedit-1.4.7/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.268274 wagtail_fedit-1.4.7/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.275937 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0002_basicmodel.py
--rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
--rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.283966 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0     4314 2024-04-14 13:07:00.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.291309 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.4.7/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.4.7/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.4.7/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.294776 wagtail_fedit-1.4.7/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     5960 2024-04-13 19:04:24.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.7/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.306664 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/adapter_registry.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:22:54.070950 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0    13123 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4175 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 16:22:53.000000 wagtail_fedit-1.4.7/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:07.312499 wagtail_fedit-1.4.8a0/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12405 2024-04-15 17:39:07.312499 wagtail_fedit-1.4.8a0/PKG-INFO
+-rw-rw-rw-   0        0        0    11205 2024-04-15 17:16:09.000000 wagtail_fedit-1.4.8a0/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1188 2024-04-15 17:39:07.327511 wagtail_fedit-1.4.8a0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.529685 wagtail_fedit-1.4.8a0/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.618627 wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      294 2024-04-13 11:18:53.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0     3776 2024-04-15 16:51:47.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/base.py
+-rw-rw-rw-   0        0        0     3857 2024-04-15 16:08:58.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/block.py
+-rw-rw-rw-   0        0        0     7523 2024-04-13 11:18:27.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     1321 2024-04-13 06:52:42.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/registry.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.662809 wagtail_fedit-1.4.8a0/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-04-15 16:05:40.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 13:08:11.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     2799 2024-04-15 17:01:35.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.434036 wagtail_fedit-1.4.8a0/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.434036 wagtail_fedit-1.4.8a0/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.690383 wagtail_fedit-1.4.8a0/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     7129 2024-04-11 09:05:50.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    12687 2024-04-11 09:05:42.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.690383 wagtail_fedit-1.4.8a0/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.690383 wagtail_fedit-1.4.8a0/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.438217 wagtail_fedit-1.4.8a0/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.439181 wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.702574 wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     4423 2024-04-04 16:40:10.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4991 2024-04-06 19:53:07.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1266 2024-04-05 19:37:44.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.723084 wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    16161 2024-04-15 15:58:30.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.440579 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.440579 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.730194 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.746015 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      386 2024-04-13 11:13:58.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.802713 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3813 2024-04-11 05:43:27.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      874 2024-04-04 16:25:30.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0     5899 2024-04-06 19:53:56.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.851727 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.872207 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.890005 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.906544 wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.912631 wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9097 2024-04-14 13:32:19.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6676 2024-04-15 16:54:43.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.923409 wagtail_fedit-1.4.8a0/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.962534 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:07.012310 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0     5194 2024-04-05 08:42:35.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      575 2024-04-05 09:29:36.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0002_basicmodel.py
+-rw-rw-rw-   0        0        0     3719 2024-04-05 10:34:38.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py
+-rw-rw-rw-   0        0        0     3314 2024-04-05 12:32:41.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     5003 2024-04-09 21:31:16.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:07.112478 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     7468 2024-04-13 19:54:41.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     4314 2024-04-14 13:07:00.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4320 2024-04-06 22:44:26.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     5664 2024-04-05 10:31:29.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1574 2024-04-05 10:54:34.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     5803 2024-04-11 11:03:32.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:07.172404 wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3540 2024-04-05 17:54:22.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     1923 2024-04-13 07:17:03.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      777 2024-04-13 10:38:39.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    15348 2024-04-13 11:03:39.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:07.217828 wagtail_fedit-1.4.8a0/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      190 2024-04-13 19:36:44.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     6271 2024-04-15 17:21:37.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17100 2024-04-11 09:23:35.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     1458 2024-04-05 20:53:30.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:07.312499 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      215 2024-04-13 09:10:53.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1748 2024-04-06 18:37:13.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0      178 2024-04-13 11:31:54.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/adapter_registry.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     2573 2024-04-11 07:39:50.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     7625 2024-04-11 13:24:34.000000 wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:39:06.570024 wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0    12405 2024-04-15 17:39:06.000000 wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4043 2024-04-15 17:39:06.000000 wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:39:06.000000 wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-15 17:39:06.000000 wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-15 17:39:06.000000 wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.4.7/LICENSE` & `wagtail_fedit-1.4.8a0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/PKG-INFO` & `wagtail_fedit-1.4.8a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.4.7
+Version: 1.4.8a0
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -41,23 +41,21 @@
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
 - [Hooks](#hooks)
-  - [Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar)
-  - [Construct Field Toolbar](#wagtail_feditconstruct_field_toolbar)
+  - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
-- [How your field/block is rendered](#how-your-fieldblock-is-rendered)
-  - [Rendered block output HTML](#rendered-block-output-html)
-  - [Rendered field output HTML](#rendered-field-output-html)
+- [How your content is rendered](#how-your-content-is-rendered)
+  - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this:
 
@@ -113,35 +111,37 @@
 
    Example:
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
-       {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
-       {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
+       {# Sub-Blocks wrapped by {# fedit block #} do not require the field_name or model argument. #}
+       {# This can (and probably should be) replaced with the `from_context` argument. #}
+       {# The variables are then taken from the parent {% fedit %} tag. The model and field name are shared through context. #}
+       {# This keeps everything extensible; but in this case it does not matter since what we are doing is instance- specific. #}
        {% fedit block self.content block=block block_id=block.id %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
    ...
 
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
-       def render_fedit_content(self, request):
-           return render_to_string("myapp/render_my_field.html", self.get_context(request))
+       def render_fedit_content(self, request, context):
+           return render_to_string("myapp/render_my_field.html", self.get_context(request) | context)
    ```
 
    Your content will then automatically be rendered with that method when need be by using
    `{% fedit field self.content %} `
-4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+4. **But wait?! I go to my template and I do not see a way to edit!** That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
 **Note:** If the parent block is wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance variable and field name should be omitted and replaced with `from_context`.
 Example: `{% fedit block from_context block=item block_id=item.id %}`
 The parent- blocktag will share these variables through context.
 This makes it possibly to easily use editable sub-blocks across multiple different model types.
 If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
 
@@ -226,36 +226,27 @@
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
 ## Hooks
 
-### wagtail_fedit.construct_block_toolbar
+### wagtail_fedit.construct_adapter_toolbar
 
-Construct the toolbar for the given block.
-This is used to display the edit icon in the block.
+Construct the toolbar for the given adapter.
+This is used to display the edit icon for the given adapter.
 
 How it is called:
 
 ```python
-for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
-    hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
-```
-
-### wagtail_fedit.construct_field_toolbar
-
-Construct the toolbar for the given field.
-This is used to display the edit icon in the field.
-
-How it is called:
-
-```python
-for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR):
-    hook(request=request, items=items, model=model, field_name=field_name)
+items = [
+    FeditAdapterEditButton(),
+]
+for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
+    hook(items=items, adapter=adapter)
 ```
 
 ### wagtail_fedit.register_type_renderer
 
 Register a custom renderer for a type.
 
 Example of how this type of renderer can be used:
@@ -322,41 +313,29 @@
 ```python
 for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
     result = hook(context, instance)
     if result is not None:
         return result # <- bool
 ```
 
-## How your field/block is rendered
+## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
-### Rendered block output HTML
-
-```html
-<div class="wagtail-fedit-block-wrapper" id="wagtail-fedit-{{ block_id }}" data-block-id="{{block_id}}" data-edit-url="{{ edit_url }}"> 
-    <div class="wagtail-fedit-buttons">
-        {% for item in toolbar_items %}
-            {{ item }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
-        {% endfor %}
-    </div>{{ content|safe }}{# Your block's rendered content. The same as {% include_block block %} #}
-</div>
-```
-
-### Rendered field output HTML
+### Rendered editable output HTML
 
 ```html
-<div class="wagtail-fedit-field-wrapper {% if inline %}wagtail-fedit-inline{% endif %}" id="wagtail-fedit-{{ field_name }}-{{model.pk}}" data-edit-url="{{ edit_url }}"> 
+<div class="wagtail-fedit-adapter-wrapper{%if shared_context.inline%} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}"{% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
     <div class="wagtail-fedit-buttons">
-        {% for item in toolbar_items %}
-            {{ item }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
+        {% for button in buttons %}
+            {{ button }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
         {% endfor %}
-    </div>{{ content|safe }}{# Your field's rendered content. Rendering may vary on your setup. #}
+    </div>{{ content|safe }}
 </div>
 ```
 
 ## Implemented
 
 * Revision Support
 * Locked Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.7 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.4.8a0 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -16,56 +16,57 @@
 License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
 (https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
-[Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
-Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
-Renderer](#wagtail_feditregister_type_renderer) - [Register Field Renderer]
-(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
-(#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
-(#wagtail_feditaction_menu_item_is_shown) - [How your field/block is rendered]
-(#how-your-fieldblock-is-rendered) - [Rendered block output HTML](#rendered-
-block-output-html) - [Rendered field output HTML](#rendered-field-output-html)
-- [Implemented](#implemented) Getting Started --------------- 1. Add
-'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
-[ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. ## Getting
-Editing! 1. Make sure the models you wish to edit inherit from
-PreviewableMixin. **This is a requirement.** 2. Define a template for your
-model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
-the required template tag libraries #}
+[Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar) -
+[Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
+Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
+Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
+(#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
+(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
+output-html) - [Implemented](#implemented) Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
+collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
+inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
+for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
+{# Load the required template tag libraries #}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {#
 Editable fields get a special `inline` argument. #} {# if True the button is
 not placed with an absolute CSS position. #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
-fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
-do not require the field_name or model argument. #} {# This is taken from the
-parent (also wrapped by `fedit_block`); the model and field name are shared
-through context. #} {% fedit block self.content block=block block_id=block.id
-%} {% endfor %} ``` ```python from django.template.loader import
-render_to_string ... class MyPage(...): # Can be any type of model. content =
-StreamField(...) def render_fedit_content(self, request): return
-render_to_string("myapp/render_my_field.html", self.get_context(request)) ```
-Your content will then automatically be rendered with that method when need be
-by using `{% fedit field self.content %} ` 4. **But wait?! I go to my template
-and I do not see a way to edit!**That is true! We try to protect any styling on
-your actual page; we do not want to interfere.Instead; we serve the editing
-interface on a different URL, accessible by clicking `Frontend Editing` in the
-Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if
-your model inherits from `DraftStateMixin`. **Note:** If the parent block is
-wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance
+fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by {# fedit
+block #} do not require the field_name or model argument. #} {# This can (and
+probably should be) replaced with the `from_context` argument. #} {# The
+variables are then taken from the parent {% fedit %} tag. The model and field
+name are shared through context. #} {# This keeps everything extensible; but in
+this case it does not matter since what we are doing is instance- specific. #}
+{% fedit block self.content block=block block_id=block.id %} {% endfor %} ```
+```python from django.template.loader import render_to_string ... class MyPage
+(...): # Can be any type of model. content = StreamField(...) def
+render_fedit_content(self, request, context): return render_to_string("myapp/
+render_my_field.html", self.get_context(request) | context) ``` Your content
+will then automatically be rendered with that method when need be by using `{%
+fedit field self.content %} ` 4. **But wait?! I go to my template and I do not
+see a way to edit!** That is true! We try to protect any styling on your actual
+page; we do not want to interfere.Instead; we serve the editing interface on a
+different URL, accessible by clicking `Frontend Editing` in the Wagtail
+userbar. Keep an eye on that userbar! It is also used for publishing if your
+model inherits from `DraftStateMixin`. **Note:** If the parent block is wrapped
+with `{% fedit block %}` or `{% fedit field %}` passing in the instance
 variable and field name should be omitted and replaced with `from_context`.
 Example: `{% fedit block from_context block=item block_id=item.id %}` The
 parent- blocktag will share these variables through context. This makes it
 possibly to easily use editable sub-blocks across multiple different model
 types. If your model **ISN'T** capable of editing; or these variables aren't
 shared - your block will be rendered as normal. ## Permissions **Note: This is
 not required for pages.** **The `Page` model already provides this interface.**
@@ -98,28 +99,24 @@
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
 block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
-wagtail_fedit.construct_block_toolbar Construct the toolbar for the given
-block. This is used to display the edit icon in the block. How it is called:
-```python for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR): hook
-(request=request, items=items, model=model, block_id=block_id,
-field_name=field_name) ``` ### wagtail_fedit.construct_field_toolbar Construct
-the toolbar for the given field. This is used to display the edit icon in the
-field. How it is called: ```python for hook in hooks.get_hooks
-(CONSTRUCT_FIELD_TOOLBAR): hook(request=request, items=items, model=model,
-field_name=field_name) ``` ### wagtail_fedit.register_type_renderer Register a
-custom renderer for a type. Example of how this type of renderer can be used:
-```python @hooks.register(REGISTER_TYPE_RENDERER) def register_renderers
-(renderer_map): # This is a custom renderer for the Page model. # It will
-render the Page model as a simple h2 tag. renderer_map[Page] = lambda request,
-context, instance, value: format_html( '
+wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
+adapter. This is used to display the edit icon for the given adapter. How it is
+called: ```python items = [ FeditAdapterEditButton(), ] for hook in
+hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
+``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
+type. Example of how this type of renderer can be used: ```python
+@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
+This is a custom renderer for the Page model. # It will render the Page model
+as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
+value: format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
@@ -133,25 +130,21 @@
 (EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field): if
 field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
-None: return result # <- bool ``` ## How your field/block is rendered
+None: return result # <- bool ``` ## How your content is rendered
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
 or even at all for most content - **if** you don't get hyperspecific with your
 CSS selectors and structure your templates well.) Your block and field are
 wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered block output HTML ```html
-{% for item in toolbar_items %} {{ item }} {# Edit button; more buttons MIGHT
+Rendered editable output HTML ```html
+% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
+{ edit_url }}">
+{% for button in buttons %} {{ button }} {# Edit button; more buttons MIGHT
 possibly be added in the future. #} {% endfor %}
-{{ content|safe }}{# Your block's rendered content. The same as {%
-include_block block %} #}
-``` ### Rendered field output HTML ```html
-{% for item in toolbar_items %} {{ item }} {# Edit button; more buttons MIGHT
-possibly be added in the future. #} {% endfor %}
-{{ content|safe }}{# Your field's rendered content. Rendering may vary on your
-setup. #}
+{{ content|safe }}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.4.7/README.md` & `wagtail_fedit-1.4.8a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
 - [Hooks](#hooks)
-  - [Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar)
-  - [Construct Field Toolbar](#wagtail_feditconstruct_field_toolbar)
+  - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
-- [How your field/block is rendered](#how-your-fieldblock-is-rendered)
-  - [Rendered block output HTML](#rendered-block-output-html)
-  - [Rendered field output HTML](#rendered-field-output-html)
+- [How your content is rendered](#how-your-content-is-rendered)
+  - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this:
 
@@ -83,35 +81,37 @@
 
    Example:
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
-       {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
-       {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
+       {# Sub-Blocks wrapped by {# fedit block #} do not require the field_name or model argument. #}
+       {# This can (and probably should be) replaced with the `from_context` argument. #}
+       {# The variables are then taken from the parent {% fedit %} tag. The model and field name are shared through context. #}
+       {# This keeps everything extensible; but in this case it does not matter since what we are doing is instance- specific. #}
        {% fedit block self.content block=block block_id=block.id %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
    ...
 
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
-       def render_fedit_content(self, request):
-           return render_to_string("myapp/render_my_field.html", self.get_context(request))
+       def render_fedit_content(self, request, context):
+           return render_to_string("myapp/render_my_field.html", self.get_context(request) | context)
    ```
 
    Your content will then automatically be rendered with that method when need be by using
    `{% fedit field self.content %} `
-4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+4. **But wait?! I go to my template and I do not see a way to edit!** That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
 **Note:** If the parent block is wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance variable and field name should be omitted and replaced with `from_context`.
 Example: `{% fedit block from_context block=item block_id=item.id %}`
 The parent- blocktag will share these variables through context.
 This makes it possibly to easily use editable sub-blocks across multiple different model types.
 If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
 
@@ -196,36 +196,27 @@
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
 ## Hooks
 
-### wagtail_fedit.construct_block_toolbar
+### wagtail_fedit.construct_adapter_toolbar
 
-Construct the toolbar for the given block.
-This is used to display the edit icon in the block.
+Construct the toolbar for the given adapter.
+This is used to display the edit icon for the given adapter.
 
 How it is called:
 
 ```python
-for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
-    hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
-```
-
-### wagtail_fedit.construct_field_toolbar
-
-Construct the toolbar for the given field.
-This is used to display the edit icon in the field.
-
-How it is called:
-
-```python
-for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR):
-    hook(request=request, items=items, model=model, field_name=field_name)
+items = [
+    FeditAdapterEditButton(),
+]
+for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
+    hook(items=items, adapter=adapter)
 ```
 
 ### wagtail_fedit.register_type_renderer
 
 Register a custom renderer for a type.
 
 Example of how this type of renderer can be used:
@@ -292,41 +283,29 @@
 ```python
 for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
     result = hook(context, instance)
     if result is not None:
         return result # <- bool
 ```
 
-## How your field/block is rendered
+## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
-### Rendered block output HTML
-
-```html
-<div class="wagtail-fedit-block-wrapper" id="wagtail-fedit-{{ block_id }}" data-block-id="{{block_id}}" data-edit-url="{{ edit_url }}"> 
-    <div class="wagtail-fedit-buttons">
-        {% for item in toolbar_items %}
-            {{ item }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
-        {% endfor %}
-    </div>{{ content|safe }}{# Your block's rendered content. The same as {% include_block block %} #}
-</div>
-```
-
-### Rendered field output HTML
+### Rendered editable output HTML
 
 ```html
-<div class="wagtail-fedit-field-wrapper {% if inline %}wagtail-fedit-inline{% endif %}" id="wagtail-fedit-{{ field_name }}-{{model.pk}}" data-edit-url="{{ edit_url }}"> 
+<div class="wagtail-fedit-adapter-wrapper{%if shared_context.inline%} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}"{% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
     <div class="wagtail-fedit-buttons">
-        {% for item in toolbar_items %}
-            {{ item }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
+        {% for button in buttons %}
+            {{ button }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
         {% endfor %}
-    </div>{{ content|safe }}{# Your field's rendered content. Rendering may vary on your setup. #}
+    </div>{{ content|safe }}
 </div>
 ```
 
 ## Implemented
 
 * Revision Support
 * Locked Support
```

#### html2text {}

```diff
@@ -1,56 +1,57 @@
 wagtail_fedit ============= ![Wagtail FEdit Example](https://github.com/
 Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
-[Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
-Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
-Renderer](#wagtail_feditregister_type_renderer) - [Register Field Renderer]
-(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
-(#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
-(#wagtail_feditaction_menu_item_is_shown) - [How your field/block is rendered]
-(#how-your-fieldblock-is-rendered) - [Rendered block output HTML](#rendered-
-block-output-html) - [Rendered field output HTML](#rendered-field-output-html)
-- [Implemented](#implemented) Getting Started --------------- 1. Add
-'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
-[ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. ## Getting
-Editing! 1. Make sure the models you wish to edit inherit from
-PreviewableMixin. **This is a requirement.** 2. Define a template for your
-model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
-the required template tag libraries #}
+[Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar) -
+[Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
+Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
+Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
+(#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
+(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
+output-html) - [Implemented](#implemented) Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
+collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
+inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
+for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
+{# Load the required template tag libraries #}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {#
 Editable fields get a special `inline` argument. #} {# if True the button is
 not placed with an absolute CSS position. #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
-fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
-do not require the field_name or model argument. #} {# This is taken from the
-parent (also wrapped by `fedit_block`); the model and field name are shared
-through context. #} {% fedit block self.content block=block block_id=block.id
-%} {% endfor %} ``` ```python from django.template.loader import
-render_to_string ... class MyPage(...): # Can be any type of model. content =
-StreamField(...) def render_fedit_content(self, request): return
-render_to_string("myapp/render_my_field.html", self.get_context(request)) ```
-Your content will then automatically be rendered with that method when need be
-by using `{% fedit field self.content %} ` 4. **But wait?! I go to my template
-and I do not see a way to edit!**That is true! We try to protect any styling on
-your actual page; we do not want to interfere.Instead; we serve the editing
-interface on a different URL, accessible by clicking `Frontend Editing` in the
-Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if
-your model inherits from `DraftStateMixin`. **Note:** If the parent block is
-wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance
+fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by {# fedit
+block #} do not require the field_name or model argument. #} {# This can (and
+probably should be) replaced with the `from_context` argument. #} {# The
+variables are then taken from the parent {% fedit %} tag. The model and field
+name are shared through context. #} {# This keeps everything extensible; but in
+this case it does not matter since what we are doing is instance- specific. #}
+{% fedit block self.content block=block block_id=block.id %} {% endfor %} ```
+```python from django.template.loader import render_to_string ... class MyPage
+(...): # Can be any type of model. content = StreamField(...) def
+render_fedit_content(self, request, context): return render_to_string("myapp/
+render_my_field.html", self.get_context(request) | context) ``` Your content
+will then automatically be rendered with that method when need be by using `{%
+fedit field self.content %} ` 4. **But wait?! I go to my template and I do not
+see a way to edit!** That is true! We try to protect any styling on your actual
+page; we do not want to interfere.Instead; we serve the editing interface on a
+different URL, accessible by clicking `Frontend Editing` in the Wagtail
+userbar. Keep an eye on that userbar! It is also used for publishing if your
+model inherits from `DraftStateMixin`. **Note:** If the parent block is wrapped
+with `{% fedit block %}` or `{% fedit field %}` passing in the instance
 variable and field name should be omitted and replaced with `from_context`.
 Example: `{% fedit block from_context block=item block_id=item.id %}` The
 parent- blocktag will share these variables through context. This makes it
 possibly to easily use editable sub-blocks across multiple different model
 types. If your model **ISN'T** capable of editing; or these variables aren't
 shared - your block will be rendered as normal. ## Permissions **Note: This is
 not required for pages.** **The `Page` model already provides this interface.**
@@ -83,28 +84,24 @@
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
 block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
-wagtail_fedit.construct_block_toolbar Construct the toolbar for the given
-block. This is used to display the edit icon in the block. How it is called:
-```python for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR): hook
-(request=request, items=items, model=model, block_id=block_id,
-field_name=field_name) ``` ### wagtail_fedit.construct_field_toolbar Construct
-the toolbar for the given field. This is used to display the edit icon in the
-field. How it is called: ```python for hook in hooks.get_hooks
-(CONSTRUCT_FIELD_TOOLBAR): hook(request=request, items=items, model=model,
-field_name=field_name) ``` ### wagtail_fedit.register_type_renderer Register a
-custom renderer for a type. Example of how this type of renderer can be used:
-```python @hooks.register(REGISTER_TYPE_RENDERER) def register_renderers
-(renderer_map): # This is a custom renderer for the Page model. # It will
-render the Page model as a simple h2 tag. renderer_map[Page] = lambda request,
-context, instance, value: format_html( '
+wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
+adapter. This is used to display the edit icon for the given adapter. How it is
+called: ```python items = [ FeditAdapterEditButton(), ] for hook in
+hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
+``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
+type. Example of how this type of renderer can be used: ```python
+@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
+This is a custom renderer for the Page model. # It will render the Page model
+as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
+value: format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
@@ -118,25 +115,21 @@
 (EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field): if
 field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
-None: return result # <- bool ``` ## How your field/block is rendered
+None: return result # <- bool ``` ## How your content is rendered
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
 or even at all for most content - **if** you don't get hyperspecific with your
 CSS selectors and structure your templates well.) Your block and field are
 wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered block output HTML ```html
-{% for item in toolbar_items %} {{ item }} {# Edit button; more buttons MIGHT
+Rendered editable output HTML ```html
+% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
+{ edit_url }}">
+{% for button in buttons %} {{ button }} {# Edit button; more buttons MIGHT
 possibly be added in the future. #} {% endfor %}
-{{ content|safe }}{# Your block's rendered content. The same as {%
-include_block block %} #}
-``` ### Rendered field output HTML ```html
-{% for item in toolbar_items %} {{ item }} {# Edit button; more buttons MIGHT
-possibly be added in the future. #} {% endfor %}
-{{ content|safe }}{# Your field's rendered content. Rendering may vary on your
-setup. #}
+{{ content|safe }}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.4.7/setup.cfg` & `wagtail_fedit-1.4.8a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 342e  ..version = 1.4.
-00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
-00000040: 2046 726f 6e74 656e 6420 6564 6974 696e   Frontend editin
-00000050: 6720 666f 7220 796f 7572 2057 6167 7461  g for your Wagta
-00000060: 696c 2073 6974 650d 0a6c 6f6e 675f 6465  il site..long_de
-00000070: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-00000080: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-00000090: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-000000a0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-000000b0: 742f 6d61 726b 646f 776e 0d0a 6175 7468  t/markdown..auth
-000000c0: 6f72 203d 204e 6967 656c 0d0a 6175 7468  or = Nigel..auth
-000000d0: 6f72 5f65 6d61 696c 203d 206e 6967 656c  or_email = nigel
-000000e0: 4067 6f6f 6461 6476 6963 652e 6974 0d0a  @goodadvice.it..
-000000f0: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-00000100: 7468 7562 2e63 6f6d 2f4e 6967 656c 3233  thub.com/Nigel23
-00000110: 3932 2f77 6167 7461 696c 5f66 6564 6974  92/wagtail_fedit
-00000120: 0d0a 6c69 6365 6e73 6520 3d20 4750 4c2d  ..license = GPL-
-00000130: 322e 302d 6f6e 6c79 0d0a 636c 6173 7369  2.0-only..classi
-00000140: 6669 6572 7320 3d20 0d0a 0945 6e76 6972  fiers = ...Envir
-00000150: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
-00000160: 7669 726f 6e6d 656e 740d 0a09 4672 616d  vironment...Fram
-00000170: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f0d  ework :: Django.
-00000180: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000190: 6a61 6e67 6f20 3a3a 2034 2e32 0d0a 0946  jango :: 4.2...F
-000001a0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
-000001b0: 6169 6c0d 0a09 4672 616d 6577 6f72 6b20  ail...Framework 
-000001c0: 3a3a 2057 6167 7461 696c 203a 3a20 350d  :: Wagtail :: 5.
-000001d0: 0a09 4672 616d 6577 6f72 6b20 3a3a 2057  ..Framework :: W
-000001e0: 6167 7461 696c 203a 3a20 360d 0a09 496e  agtail :: 6...In
-000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000200: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
-00000210: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000220: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
-00000230: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-00000240: 6365 6e73 6520 7632 206f 7220 6c61 7465  cense v2 or late
-00000250: 7220 2847 504c 7632 2b29 0d0a 094f 7065  r (GPLv2+)...Ope
-00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-00000280: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000290: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002a0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002c0: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
-000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002e0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
-000002f0: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
-00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000310: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
-00000320: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000330: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000340: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-00000350: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000360: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
-00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000390: 3a20 332e 3131 0d0a 0954 6f70 6963 203a  : 3.11...Topic :
-000003a0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
-000003b0: 572f 4854 5450 0d0a 0954 6f70 6963 203a  W/HTTP...Topic :
-000003c0: 3a20 496e 7465 726e 6574 203a 3a20 5757  : Internet :: WW
-000003d0: 572f 4854 5450 203a 3a20 4479 6e61 6d69  W/HTTP :: Dynami
-000003e0: 6320 436f 6e74 656e 740d 0a0d 0a5b 6f70  c Content....[op
-000003f0: 7469 6f6e 735d 0d0a 696e 636c 7564 655f  tions]..include_
-00000400: 7061 636b 6167 655f 6461 7461 203d 2074  package_data = t
-00000410: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
-00000420: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000430: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
-00000440: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000450: 203d 200d 0a09 446a 616e 676f 203e 3d20   = ...Django >= 
-00000460: 342e 320d 0a09 5761 6774 6169 6c20 3e3d  4.2...Wagtail >=
-00000470: 2035 2e32 0d0a 0d0a 5b65 6767 5f69 6e66   5.2....[egg_inf
-00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000004a0: 0d0a                                     ..
+00000030: 3861 300d 0a64 6573 6372 6970 7469 6f6e  8a0..description
+00000040: 203d 2046 726f 6e74 656e 6420 6564 6974   = Frontend edit
+00000050: 696e 6720 666f 7220 796f 7572 2057 6167  ing for your Wag
+00000060: 7461 696c 2073 6974 650d 0a6c 6f6e 675f  tail site..long_
+00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+000000b0: 6578 742f 6d61 726b 646f 776e 0d0a 6175  ext/markdown..au
+000000c0: 7468 6f72 203d 204e 6967 656c 0d0a 6175  thor = Nigel..au
+000000d0: 7468 6f72 5f65 6d61 696c 203d 206e 6967  thor_email = nig
+000000e0: 656c 4067 6f6f 6461 6476 6963 652e 6974  el@goodadvice.it
+000000f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
+00000100: 6769 7468 7562 2e63 6f6d 2f4e 6967 656c  github.com/Nigel
+00000110: 3233 3932 2f77 6167 7461 696c 5f66 6564  2392/wagtail_fed
+00000120: 6974 0d0a 6c69 6365 6e73 6520 3d20 4750  it..license = GP
+00000130: 4c2d 322e 302d 6f6e 6c79 0d0a 636c 6173  L-2.0-only..clas
+00000140: 7369 6669 6572 7320 3d20 0d0a 0945 6e76  sifiers = ...Env
+00000150: 6972 6f6e 6d65 6e74 203a 3a20 5765 6220  ironment :: Web 
+00000160: 456e 7669 726f 6e6d 656e 740d 0a09 4672  Environment...Fr
+00000170: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
+00000180: 6f0d 0a09 4672 616d 6577 6f72 6b20 3a3a  o...Framework ::
+00000190: 2044 6a61 6e67 6f20 3a3a 2034 2e32 0d0a   Django :: 4.2..
+000001a0: 0946 7261 6d65 776f 726b 203a 3a20 5761  .Framework :: Wa
+000001b0: 6774 6169 6c0d 0a09 4672 616d 6577 6f72  gtail...Framewor
+000001c0: 6b20 3a3a 2057 6167 7461 696c 203a 3a20  k :: Wagtail :: 
+000001d0: 350d 0a09 4672 616d 6577 6f72 6b20 3a3a  5...Framework ::
+000001e0: 2057 6167 7461 696c 203a 3a20 360d 0a09   Wagtail :: 6...
+000001f0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000200: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
+00000210: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+00000220: 2041 7070 726f 7665 6420 3a3a 2047 4e55   Approved :: GNU
+00000230: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+00000240: 4c69 6365 6e73 6520 7632 206f 7220 6c61  License v2 or la
+00000250: 7465 7220 2847 504c 7632 2b29 0d0a 094f  ter (GPLv2+)...O
+00000260: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000270: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000280: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
+00000290: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002a0: 6f6e 0d0a 0950 726f 6772 616d 6d69 6e67  on...Programming
+000002b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002c0: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
+000002d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
+000002f0: 3a20 4f6e 6c79 0d0a 0950 726f 6772 616d  : Only...Program
+00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000310: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
+00000320: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000330: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000340: 3a3a 2033 2e39 0d0a 0950 726f 6772 616d  :: 3.9...Program
+00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000360: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
+00000370: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000380: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000390: 203a 3a20 332e 3131 0d0a 0954 6f70 6963   :: 3.11...Topic
+000003a0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
+000003b0: 5757 572f 4854 5450 0d0a 0954 6f70 6963  WWW/HTTP...Topic
+000003c0: 203a 3a20 496e 7465 726e 6574 203a 3a20   :: Internet :: 
+000003d0: 5757 572f 4854 5450 203a 3a20 4479 6e61  WWW/HTTP :: Dyna
+000003e0: 6d69 6320 436f 6e74 656e 740d 0a0d 0a5b  mic Content....[
+000003f0: 6f70 7469 6f6e 735d 0d0a 696e 636c 7564  options]..includ
+00000400: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+00000410: 2074 7275 650d 0a70 6163 6b61 6765 7320   true..packages 
+00000420: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+00000430: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+00000440: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000450: 6573 203d 200d 0a09 446a 616e 676f 203e  es = ...Django >
+00000460: 3d20 342e 320d 0a09 5761 6774 6169 6c20  = 4.2...Wagtail 
+00000470: 3e3d 2035 2e32 0d0a 0d0a 5b65 6767 5f69  >= 5.2....[egg_i
+00000480: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000490: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000004a0: 0d0a 0d0a                                ....
```

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         raise NotImplementedError
 
     def form_valid(self, form: "forms.Form"):
         pass
     
     def form_invalid(self, form: "forms.Form"):
         pass
-    
+
+    @classmethod
     def render_content(self, parent_context: dict = None) -> str:
         """
         Render the content for the field.
         This should NOT include the wagtail-fedit wrapper.
         """
         raise NotImplementedError
```

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/block.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/adapters/registry.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/hooks.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/hooks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,14 @@
 def prefix(name):
     """
         Default prefix for wagtail_fedit hooks.
     """
     return f"wagtail_fedit.{name}"
 
 
-CONSTRUCT_BLOCK_TOOLBAR  = prefix("construct_block_toolbar")
-"""
-### wagtail_fedit.construct_block_toolbar
-Construct the toolbar for the given block.
-This is used to display the edit icon in the block.
-
-How it is called:
-
-```python
-for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
-    hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
-```
-"""
-
-
-CONSTRUCT_FIELD_TOOLBAR  = prefix("construct_field_toolbar")
-"""
-### wagtail_fedit.construct_field_toolbar
-Construct the toolbar for the given field.
-This is used to display the edit icon in the field.
-
-How it is called:
-
-```python
-for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR):
-    hook(request=request, items=items, model=model, field_name=field_name)
-```
-"""
-
 CONSTRUCT_ADAPTER_TOOLBAR = prefix("construct_adapter_toolbar")
 """
 ### wagtail_fedit.construct_adapter_toolbar
 Construct the toolbar for the given adapter.
 This is used to display the edit icon for the given adapter.
 """
```

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.4.8a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.4.8a0/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/models.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.4.8a0/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/templatetags/fedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,18 @@
 
             field_name = context["wagtail_fedit_field"]
             obj = context["wagtail_fedit_instance"]
 
         else:
 
             if not model:
-                raise TemplateSyntaxError("Model is required")
+                raise TemplateSyntaxError(
+                    "`instance.field` is required; use `from_context` if "
+                    "this is wrapped by a fedit templatetag or adress a model field."
+                )
 
             field_name = getters[len(getters)-1]
             obj = model
             for i in range(len(getters) - 1):
                 getter = getters[i]
                 try:
                     obj = getattr(obj, getter)
```

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0002_basicmodel.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0002_basicmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0003_basicmodel_content_editabledraftmodel_content_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/migrations/0004_editablelockmodel.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/urls.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/utils.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/views/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     HttpResponseBadRequest,
     HttpResponseForbidden,
     JsonResponse,
     HttpResponse,
 )
 from django.apps import apps
 from wagtail.models import (
-    RevisionMixin, 
+    RevisionMixin,
+    PAGE_TEMPLATE_VAR,
+    Page,
 )
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 
 from ..adapters import (
     adapter_registry,
     BaseAdapter,
     RegistryLookUpError,
@@ -170,19 +172,25 @@
                     request=request,
                 )
             }, status=423 if self.locked_for_user else 400)
 
         
         self.adapter.form_valid(form)
 
+        context = self.get_context_data()
+        if isinstance(self.instance, Page):
+            # Add the page template variable to the context.
+            # Wagtail uses this internally; for example in `{% wagtailpagecache %}`
+            context[PAGE_TEMPLATE_VAR] = self.instance
+
         # Render the frame HTML
         html = wrap_adapter(
             request=request,
             adapter=self.adapter,
-            context=self.get_context_data(),
+            context=context,
         )
 
         return JsonResponse({
             "success": True,
             "html": html,
         })
```

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.4.8a0/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.4.7
+Version: 1.4.8a0
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -41,23 +41,21 @@
 - [Getting Editing!](#getting-editing)
 - [Permissions](#permissions)
 - [Revisions](#revisions)
 - [Workflows](#workflows)
 - [Logs](#logs)
 - [Caveats](#caveats)
 - [Hooks](#hooks)
-  - [Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar)
-  - [Construct Field Toolbar](#wagtail_feditconstruct_field_toolbar)
+  - [Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar)
   - [Register Type Renderer](#wagtail_feditregister_type_renderer)
   - [Register Field Renderer](#wagtail_feditregister_field_renderer)
   - [Exclude Related Forms](#wagtail_feditexclude_related_forms)
   - [Action Menu Item Is Shown](#wagtail_feditaction_menu_item_is_shown)
-- [How your field/block is rendered](#how-your-fieldblock-is-rendered)
-  - [Rendered block output HTML](#rendered-block-output-html)
-  - [Rendered field output HTML](#rendered-field-output-html)
+- [How your content is rendered](#how-your-content-is-rendered)
+  - [Rendered output HTML](#rendered-editable-output-html)
 - [Implemented](#implemented)
 
 Getting Started
 ---------------
 
 1. Add 'wagtail_fedit' to your INSTALLED_APPS setting like this:
 
@@ -113,35 +111,37 @@
 
    Example:
 
    ```django-html
    {# myapp/render_my_field.html #}
    {% load fedit %}
    {% for block in self.content %}
-       {# Sub-Blocks wrapped by fedit_block do not require the field_name or model argument. #}
-       {# This is taken from the parent (also wrapped by `fedit_block`); the model and field name are shared through context. #}
+       {# Sub-Blocks wrapped by {# fedit block #} do not require the field_name or model argument. #}
+       {# This can (and probably should be) replaced with the `from_context` argument. #}
+       {# The variables are then taken from the parent {% fedit %} tag. The model and field name are shared through context. #}
+       {# This keeps everything extensible; but in this case it does not matter since what we are doing is instance- specific. #}
        {% fedit block self.content block=block block_id=block.id %}
    {% endfor %}
 
    ```
 
    ```python
    from django.template.loader import render_to_string
    ...
 
    class MyPage(...): # Can be any type of model.
        content = StreamField(...)
 
-       def render_fedit_content(self, request):
-           return render_to_string("myapp/render_my_field.html", self.get_context(request))
+       def render_fedit_content(self, request, context):
+           return render_to_string("myapp/render_my_field.html", self.get_context(request) | context)
    ```
 
    Your content will then automatically be rendered with that method when need be by using
    `{% fedit field self.content %} `
-4. **But wait?! I go to my template and I do not see a way to edit!**That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
+4. **But wait?! I go to my template and I do not see a way to edit!** That is true! We try to protect any styling on your actual page; we do not want to interfere.Instead; we serve the editing interface on a different URL, accessible by clicking `Frontend Editing` in the Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if your model inherits from `DraftStateMixin`.
 
 **Note:** If the parent block is wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance variable and field name should be omitted and replaced with `from_context`.
 Example: `{% fedit block from_context block=item block_id=item.id %}`
 The parent- blocktag will share these variables through context.
 This makes it possibly to easily use editable sub-blocks across multiple different model types.
 If your model **ISN'T** capable of editing; or these variables aren't shared - your block will be rendered as normal.
 
@@ -226,36 +226,27 @@
     {# Field name and model are the same arguments as in the first example! #}
     {% fedit block my_model_instance_var.content_field block=item block_id=item.id %}
 {% endfor %}
 ```
 
 ## Hooks
 
-### wagtail_fedit.construct_block_toolbar
+### wagtail_fedit.construct_adapter_toolbar
 
-Construct the toolbar for the given block.
-This is used to display the edit icon in the block.
+Construct the toolbar for the given adapter.
+This is used to display the edit icon for the given adapter.
 
 How it is called:
 
 ```python
-for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR):
-    hook(request=request, items=items, model=model, block_id=block_id, field_name=field_name)
-```
-
-### wagtail_fedit.construct_field_toolbar
-
-Construct the toolbar for the given field.
-This is used to display the edit icon in the field.
-
-How it is called:
-
-```python
-for hook in hooks.get_hooks(CONSTRUCT_FIELD_TOOLBAR):
-    hook(request=request, items=items, model=model, field_name=field_name)
+items = [
+    FeditAdapterEditButton(),
+]
+for hook in hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR):
+    hook(items=items, adapter=adapter)
 ```
 
 ### wagtail_fedit.register_type_renderer
 
 Register a custom renderer for a type.
 
 Example of how this type of renderer can be used:
@@ -322,41 +313,29 @@
 ```python
 for hook in hooks.get_hooks(ACTION_MENU_ITEM_IS_SHOWN):
     result = hook(context, instance)
     if result is not None:
         return result # <- bool
 ```
 
-## How your field/block is rendered
+## How your content is rendered
 
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much, or even at all for most content - **if** you don't get hyperspecific with your CSS selectors and structure your templates well.)
 
 Your block and field are wrapped in a `div`, any CSS for your templates should keep this in mind.
 
-### Rendered block output HTML
-
-```html
-<div class="wagtail-fedit-block-wrapper" id="wagtail-fedit-{{ block_id }}" data-block-id="{{block_id}}" data-edit-url="{{ edit_url }}"> 
-    <div class="wagtail-fedit-buttons">
-        {% for item in toolbar_items %}
-            {{ item }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
-        {% endfor %}
-    </div>{{ content|safe }}{# Your block's rendered content. The same as {% include_block block %} #}
-</div>
-```
-
-### Rendered field output HTML
+### Rendered editable output HTML
 
 ```html
-<div class="wagtail-fedit-field-wrapper {% if inline %}wagtail-fedit-inline{% endif %}" id="wagtail-fedit-{{ field_name }}-{{model.pk}}" data-edit-url="{{ edit_url }}"> 
+<div class="wagtail-fedit-adapter-wrapper{%if shared_context.inline%} wagtail-fedit-inline{%endif%} wagtail-fedit-{{ identifier }}"{% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{{ edit_url }}">
     <div class="wagtail-fedit-buttons">
-        {% for item in toolbar_items %}
-            {{ item }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
+        {% for button in buttons %}
+            {{ button }} {# Edit button; more buttons MIGHT possibly be added in the future. #}
         {% endfor %}
-    </div>{{ content|safe }}{# Your field's rendered content. Rendering may vary on your setup. #}
+    </div>{{ content|safe }}
 </div>
 ```
 
 ## Implemented
 
 * Revision Support
 * Locked Support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.7 Summary: Frontend
+Metadata-Version: 2.1 Name: wagtail-fedit Version: 1.4.8a0 Summary: Frontend
 editing for your Wagtail site Home-page: https://github.com/Nigel2392/
 wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it License: GPL-2.0-
 only Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Wagtail :: 6
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 or later (GPLv2+) Classifier: Operating System
@@ -16,56 +16,57 @@
 License-File: LICENSE wagtail_fedit ============= ![Wagtail FEdit Example]
 (https://github.com/Nigel2392/wagtail_fedit/blob/main/.github/images/
 wagtail_fedit_example.png?raw=true) Wagtail FEdit is a library to allow your
 Wagtail pages and content-blocks to be edited on the frontend. # Table of
 Contents - [Getting Started](#getting-started) - [Getting Editing!](#getting-
 editing) - [Permissions](#permissions) - [Revisions](#revisions) - [Workflows]
 (#workflows) - [Logs](#logs) - [Caveats](#caveats) - [Hooks](#hooks) -
-[Construct Block Toolbar](#wagtail_feditconstruct_block_toolbar) - [Construct
-Field Toolbar](#wagtail_feditconstruct_field_toolbar) - [Register Type
-Renderer](#wagtail_feditregister_type_renderer) - [Register Field Renderer]
-(#wagtail_feditregister_field_renderer) - [Exclude Related Forms]
-(#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
-(#wagtail_feditaction_menu_item_is_shown) - [How your field/block is rendered]
-(#how-your-fieldblock-is-rendered) - [Rendered block output HTML](#rendered-
-block-output-html) - [Rendered field output HTML](#rendered-field-output-html)
-- [Implemented](#implemented) Getting Started --------------- 1. Add
-'wagtail_fedit' to your INSTALLED_APPS setting like this: ``` INSTALLED_APPS =
-[ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py collectstatic`. ## Getting
-Editing! 1. Make sure the models you wish to edit inherit from
-PreviewableMixin. **This is a requirement.** 2. Define a template for your
-model. Example: ```django-html {% load fedit static wagtailuserbar %} {# Load
-the required template tag libraries #}
+[Construct Adapter Toolbar](#wagtail_feditconstruct_adapter_toolbar) -
+[Register Type Renderer](#wagtail_feditregister_type_renderer) - [Register
+Field Renderer](#wagtail_feditregister_field_renderer) - [Exclude Related
+Forms](#wagtail_feditexclude_related_forms) - [Action Menu Item Is Shown]
+(#wagtail_feditaction_menu_item_is_shown) - [How your content is rendered]
+(#how-your-content-is-rendered) - [Rendered output HTML](#rendered-editable-
+output-html) - [Implemented](#implemented) Getting Started --------------- 1.
+Add 'wagtail_fedit' to your INSTALLED_APPS setting like this: ```
+INSTALLED_APPS = [ ..., 'wagtail_fedit', ] ``` 2. Run `py ./manage.py
+collectstatic`. ## Getting Editing! 1. Make sure the models you wish to edit
+inherit from PreviewableMixin. **This is a requirement.** 2. Define a template
+for your model. Example: ```django-html {% load fedit static wagtailuserbar %}
+{# Load the required template tag libraries #}
 {# Adress the model.field or model.my.related.field you wish to edit. #} {#
 Editable fields get a special `inline` argument. #} {# if True the button is
 not placed with an absolute CSS position. #}
 ************ {{%% ffeeddiitt ffiieelldd sseellff..ttiittllee iinnlliinnee==TTrruuee oorr FFaallssee %%}} ************
 {% fedit field self.content %} {% wagtailuserbar %}
 ``` 3. If your needs some special form of rendering; we allow your model to
 define a custom render method. The format of the method name should be
 `render_fedit_{fieldname}`. Say we want all sub-blocks of our streamfield to
 automatically be made editable. This wouldn't be possible in the above
 configuration. To fix this; we should first create a custom template to render
 our content. Example: ```django-html {# myapp/render_my_field.html #} {% load
-fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by fedit_block
-do not require the field_name or model argument. #} {# This is taken from the
-parent (also wrapped by `fedit_block`); the model and field name are shared
-through context. #} {% fedit block self.content block=block block_id=block.id
-%} {% endfor %} ``` ```python from django.template.loader import
-render_to_string ... class MyPage(...): # Can be any type of model. content =
-StreamField(...) def render_fedit_content(self, request): return
-render_to_string("myapp/render_my_field.html", self.get_context(request)) ```
-Your content will then automatically be rendered with that method when need be
-by using `{% fedit field self.content %} ` 4. **But wait?! I go to my template
-and I do not see a way to edit!**That is true! We try to protect any styling on
-your actual page; we do not want to interfere.Instead; we serve the editing
-interface on a different URL, accessible by clicking `Frontend Editing` in the
-Wagtail userbar. Keep an eye on that userbar! It is also used for publishing if
-your model inherits from `DraftStateMixin`. **Note:** If the parent block is
-wrapped with `{% fedit block %}` or `{% fedit field %}` passing in the instance
+fedit %} {% for block in self.content %} {# Sub-Blocks wrapped by {# fedit
+block #} do not require the field_name or model argument. #} {# This can (and
+probably should be) replaced with the `from_context` argument. #} {# The
+variables are then taken from the parent {% fedit %} tag. The model and field
+name are shared through context. #} {# This keeps everything extensible; but in
+this case it does not matter since what we are doing is instance- specific. #}
+{% fedit block self.content block=block block_id=block.id %} {% endfor %} ```
+```python from django.template.loader import render_to_string ... class MyPage
+(...): # Can be any type of model. content = StreamField(...) def
+render_fedit_content(self, request, context): return render_to_string("myapp/
+render_my_field.html", self.get_context(request) | context) ``` Your content
+will then automatically be rendered with that method when need be by using `{%
+fedit field self.content %} ` 4. **But wait?! I go to my template and I do not
+see a way to edit!** That is true! We try to protect any styling on your actual
+page; we do not want to interfere.Instead; we serve the editing interface on a
+different URL, accessible by clicking `Frontend Editing` in the Wagtail
+userbar. Keep an eye on that userbar! It is also used for publishing if your
+model inherits from `DraftStateMixin`. **Note:** If the parent block is wrapped
+with `{% fedit block %}` or `{% fedit field %}` passing in the instance
 variable and field name should be omitted and replaced with `from_context`.
 Example: `{% fedit block from_context block=item block_id=item.id %}` The
 parent- blocktag will share these variables through context. This makes it
 possibly to easily use editable sub-blocks across multiple different model
 types. If your model **ISN'T** capable of editing; or these variables aren't
 shared - your block will be rendered as normal. ## Permissions **Note: This is
 not required for pages.** **The `Page` model already provides this interface.**
@@ -98,28 +99,24 @@
 ``` To make this an editable block instead; we would slightly change the loop
 to make the block's `id` available. This is done by accessing the
 `bound_blocks` of that ListBlock *(`StreamBlock` does this automatically for
 the toplevel block!)* Our new loop would then be: ```django-html {% for item in
 self.items.bound_blocks %} {# Field name and model are the same arguments as in
 the first example! #} {% fedit block my_model_instance_var.content_field
 block=item block_id=item.id %} {% endfor %} ``` ## Hooks ###
-wagtail_fedit.construct_block_toolbar Construct the toolbar for the given
-block. This is used to display the edit icon in the block. How it is called:
-```python for hook in hooks.get_hooks(CONSTRUCT_BLOCK_TOOLBAR): hook
-(request=request, items=items, model=model, block_id=block_id,
-field_name=field_name) ``` ### wagtail_fedit.construct_field_toolbar Construct
-the toolbar for the given field. This is used to display the edit icon in the
-field. How it is called: ```python for hook in hooks.get_hooks
-(CONSTRUCT_FIELD_TOOLBAR): hook(request=request, items=items, model=model,
-field_name=field_name) ``` ### wagtail_fedit.register_type_renderer Register a
-custom renderer for a type. Example of how this type of renderer can be used:
-```python @hooks.register(REGISTER_TYPE_RENDERER) def register_renderers
-(renderer_map): # This is a custom renderer for the Page model. # It will
-render the Page model as a simple h2 tag. renderer_map[Page] = lambda request,
-context, instance, value: format_html( '
+wagtail_fedit.construct_adapter_toolbar Construct the toolbar for the given
+adapter. This is used to display the edit icon for the given adapter. How it is
+called: ```python items = [ FeditAdapterEditButton(), ] for hook in
+hooks.get_hooks(CONSTRUCT_ADAPTER_TOOLBAR): hook(items=items, adapter=adapter)
+``` ### wagtail_fedit.register_type_renderer Register a custom renderer for a
+type. Example of how this type of renderer can be used: ```python
+@hooks.register(REGISTER_TYPE_RENDERER) def register_renderers(renderer_map): #
+This is a custom renderer for the Page model. # It will render the Page model
+as a simple h2 tag. renderer_map[Page] = lambda request, context, instance,
+value: format_html( '
 ********** {{00}} **********
 ', value.title ) ``` ### wagtail_fedit.register_field_renderer Register a
 custom renderer for a field. Example of how this type of renderer is used in
 wagtail_hooks/renderers.py: ```python @hooks.register(REGISTER_FIELD_RENDERER)
 def register_renderers(renderer_map): # This is a custom renderer for RichText
 fields. # It will render the RichText field as a RichText block. renderer_map
 [RichTextField] =\ lambda request, context, instance, value: richtext(value)
@@ -133,25 +130,21 @@
 (EXCLUDE_FROM_RELATED_FORMS) def exclude_related_forms(field): if
 field.related_model in [Page, Image, Document]: return True return False ```
 ### wagtail_fedit.action_menu_item_is_shown Decide if the action menu item
 should be shown for the given instance. Return None if you cannot decide, False
 if you want to hide the item, and True if you want to show the item. Example of
 how this hook is called: ```python for hook in hooks.get_hooks
 (ACTION_MENU_ITEM_IS_SHOWN): result = hook(context, instance) if result is not
-None: return result # <- bool ``` ## How your field/block is rendered
+None: return result # <- bool ``` ## How your content is rendered
 (**Maintainer's note:** In my experience this doesn't mess the CSS up too much,
 or even at all for most content - **if** you don't get hyperspecific with your
 CSS selectors and structure your templates well.) Your block and field are
 wrapped in a `div`, any CSS for your templates should keep this in mind. ###
-Rendered block output HTML ```html
-{% for item in toolbar_items %} {{ item }} {# Edit button; more buttons MIGHT
+Rendered editable output HTML ```html
+% if shared %} data-shared-context="{{ shared }}"{%endif%} data-edit-url="{
+{ edit_url }}">
+{% for button in buttons %} {{ button }} {# Edit button; more buttons MIGHT
 possibly be added in the future. #} {% endfor %}
-{{ content|safe }}{# Your block's rendered content. The same as {%
-include_block block %} #}
-``` ### Rendered field output HTML ```html
-{% for item in toolbar_items %} {{ item }} {# Edit button; more buttons MIGHT
-possibly be added in the future. #} {% endfor %}
-{{ content|safe }}{# Your field's rendered content. Rendering may vary on your
-setup. #}
+{{ content|safe }}
 ``` ## Implemented * Revision Support * Locked Support * Draft Support *
 Preview Support * Workflow Support * Permissions * Audit Logs * Full block
 capabilities on Frontend Editing
```

### Comparing `wagtail_fedit-1.4.7/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.4.8a0/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
 wagtail_fedit/static/wagtail_fedit/css/frontend.css
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/frontend.js
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
-wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
-wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
```

