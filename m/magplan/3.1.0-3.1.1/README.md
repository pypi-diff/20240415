# Comparing `tmp/magplan-3.1.0.tar.gz` & `tmp/magplan-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magplan-3.1.0.tar", max compression
+gzip compressed data, was "magplan-3.1.1.tar", max compression
```

## Comparing `magplan-3.1.0.tar` & `magplan-3.1.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0     6010 2023-12-13 19:44:22.572842 magplan-3.1.0/README.md
--rw-r--r--   0        0        0      729 2023-12-13 22:01:14.723860 magplan-3.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.574842 magplan-3.1.0/src/magplan/__init__.py
--rw-r--r--   0        0        0     2014 2023-12-13 19:44:22.574842 magplan-3.1.0/src/magplan/admin.py
--rw-r--r--   0        0        0       86 2023-12-13 19:44:22.574842 magplan-3.1.0/src/magplan/apps.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.574842 magplan-3.1.0/src/magplan/conf/__init__.py
--rw-r--r--   0        0        0     1702 2023-12-13 19:44:22.574842 magplan-3.1.0/src/magplan/conf/settings.py
--rw-r--r--   0        0        0      556 2023-12-13 19:44:22.574842 magplan-3.1.0/src/magplan/context_processors.py
--rw-r--r--   0        0        0     2949 2023-12-13 19:44:22.574842 magplan-3.1.0/src/magplan/dynamic_preferences_registry.py
--rw-r--r--   0        0        0  3415905 2023-12-13 19:44:22.642844 magplan-3.1.0/src/magplan/fixtures/db_test.json
--rw-r--r--   0        0        0     8363 2023-12-13 19:44:22.655844 magplan-3.1.0/src/magplan/forms.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.655844 magplan-3.1.0/src/magplan/integrations/__init__.py
--rw-r--r--   0        0        0      732 2023-12-13 19:44:22.655844 magplan-3.1.0/src/magplan/integrations/images.py
--rw-r--r--   0        0        0     4716 2023-12-13 19:44:22.655844 magplan-3.1.0/src/magplan/integrations/posts.py
--rw-r--r--   0        0        0     1823 2023-12-13 19:44:22.656844 magplan-3.1.0/src/magplan/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39873 2023-12-13 19:44:22.656844 magplan-3.1.0/src/magplan/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2456 2023-12-13 19:44:22.656844 magplan-3.1.0/src/magplan/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40385 2023-12-13 19:44:22.656844 magplan-3.1.0/src/magplan/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/management/__init__.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/management/commands/__init__.py
--rw-r--r--   0        0        0      350 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/management/commands/render.py
--rw-r--r--   0        0        0      718 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/middleware.py
--rw-r--r--   0        0        0    10914 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/migrations/0001_initial.py
--rw-r--r--   0        0        0     7877 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/migrations/0002_auto_20201115_1140.py
--rw-r--r--   0        0        0      541 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/migrations/0003_auto_20201121_1750.py
--rw-r--r--   0        0        0      465 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/migrations/0004_post_features.py
--rw-r--r--   0        0        0      947 2023-12-13 19:44:22.657844 magplan-3.1.0/src/magplan/migrations/0005_auto_20210213_1556.py
--rw-r--r--   0        0        0      883 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/migrations/0006_auto_20210316_1840.py
--rw-r--r--   0        0        0      561 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/migrations/0007_auto_20210316_1900.py
--rw-r--r--   0        0        0     1408 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/migrations/0008_auto_20210318_0108.py
--rw-r--r--   0        0        0      464 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/migrations/0009_auto_20210523_1641.py
--rw-r--r--   0        0        0     2334 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/migrations/0010_auto_20210624_1041.py
--rw-r--r--   0        0        0     1086 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/migrations/0011_auto_20210624_1817.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/migrations/__init__.py
--rw-r--r--   0        0        0    27751 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/models.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.658844 magplan-3.1.0/src/magplan/tasks/__init__.py
--rw-r--r--   0        0        0     3748 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/tasks/send_idea_comment_notification.py
--rw-r--r--   0        0        0      468 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/tasks/send_idea_notification.py
--rw-r--r--   0        0        0     4102 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/tasks/send_post_comment_notification.py
--rw-r--r--   0        0        0      542 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/tasks/upload_post_to_wp.py
--rw-r--r--   0        0        0     1762 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/tasks/utils.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/templates/__init__.py
--rw-r--r--   0        0        0     1400 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/templates/_test_issues.py
--rw-r--r--   0        0        0      758 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/templates/email/_vote_from_email.html
--rw-r--r--   0        0        0      416 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/templates/email/assigned_to_you.html
--rw-r--r--   0        0        0      701 2023-12-13 19:44:22.659844 magplan-3.1.0/src/magplan/templates/email/idea_approved.html
--rw-r--r--   0        0        0      634 2023-12-13 19:44:22.673844 magplan-3.1.0/src/magplan/templates/email/new_comment.html
--rw-r--r--   0        0        0      370 2023-12-13 19:44:22.673844 magplan-3.1.0/src/magplan/templates/email/new_idea.html
--rw-r--r--   0        0        0     8503 2023-12-13 19:44:22.673844 magplan-3.1.0/src/magplan/templates/layout_plan.html
--rw-r--r--   0        0        0      893 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/articles/advert.html
--rw-r--r--   0        0        0      860 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/articles/archived.html
--rw-r--r--   0        0        0      855 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/articles/default.html
--rw-r--r--   0        0        0     3053 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/articles/index.html
--rw-r--r--   0        0        0      911 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/articles/whitelisted.html
--rw-r--r--   0        0        0     4121 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/authors/_form.html
--rw-r--r--   0        0        0      541 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/authors/edit.html
--rw-r--r--   0        0        0      869 2023-12-13 19:44:22.674844 magplan-3.1.0/src/magplan/templates/magplan/authors/index.html
--rw-r--r--   0        0        0      480 2023-12-13 19:44:22.676844 magplan-3.1.0/src/magplan/templates/magplan/authors/new.html
--rw-r--r--   0        0        0     1077 2023-12-13 19:44:22.676844 magplan-3.1.0/src/magplan/templates/magplan/authors/show.html
--rw-r--r--   0        0        0      595 2023-12-13 19:44:22.676844 magplan-3.1.0/src/magplan/templates/magplan/ideas/_approve_ideas.html
--rw-r--r--   0        0        0      786 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/ideas/_authors_list.html
--rw-r--r--   0        0        0     2332 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/ideas/_form_base.html
--rw-r--r--   0        0        0     1088 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/ideas/_vote.html
--rw-r--r--   0        0        0     1521 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/ideas/_voting_results.html
--rw-r--r--   0        0        0     3959 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/ideas/index.html
--rw-r--r--   0        0        0     3149 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/ideas/show.html
--rw-r--r--   0        0        0     4404 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/index/index.html
--rw-r--r--   0        0        0     1786 2023-12-13 19:44:22.677844 magplan-3.1.0/src/magplan/templates/magplan/issues/_form.html
--rw-r--r--   0        0        0     1202 2023-12-13 19:44:22.678844 magplan-3.1.0/src/magplan/templates/magplan/issues/index.html
--rw-r--r--   0        0        0      477 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/issues/new.html
--rw-r--r--   0        0        0      837 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/issues/show.html
--rw-r--r--   0        0        0      573 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/partials/_navbar.sites.html
--rw-r--r--   0        0        0     1395 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/partials/_navbar_header_links.html
--rw-r--r--   0        0        0     2797 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/partials/comments.html
--rw-r--r--   0        0        0     2252 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/partials/navbar.html
--rw-r--r--   0        0        0     3180 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/partials/posts_table.html
--rw-r--r--   0        0        0      956 2023-12-13 19:44:22.683844 magplan-3.1.0/src/magplan/templates/magplan/posts/_admin_set_stage.html
--rw-r--r--   0        0        0     6970 2023-12-13 19:44:22.686844 magplan-3.1.0/src/magplan/templates/magplan/posts/_attachments.html
--rw-r--r--   0        0        0      768 2023-12-13 19:44:22.687845 magplan-3.1.0/src/magplan/templates/magplan/posts/_field_col.html
--rw-r--r--   0        0        0     3389 2023-12-13 19:44:22.687845 magplan-3.1.0/src/magplan/templates/magplan/posts/_form_base.html
--rw-r--r--   0        0        0     3359 2023-12-13 19:44:22.687845 magplan-3.1.0/src/magplan/templates/magplan/posts/_form_meta.html
--rw-r--r--   0        0        0      286 2023-12-13 19:44:22.687845 magplan-3.1.0/src/magplan/templates/magplan/posts/_paywall_alert.html
--rw-r--r--   0        0        0     1063 2023-12-13 19:44:22.687845 magplan-3.1.0/src/magplan/templates/magplan/posts/_progress.html
--rw-r--r--   0        0        0      882 2023-12-13 19:44:22.689845 magplan-3.1.0/src/magplan/templates/magplan/posts/_schedule.html
--rw-r--r--   0        0        0     2437 2023-12-13 19:44:22.689845 magplan-3.1.0/src/magplan/templates/magplan/posts/_stages.html
--rw-r--r--   0        0        0     8559 2023-12-13 19:44:22.691845 magplan-3.1.0/src/magplan/templates/magplan/posts/edit.html
--rw-r--r--   0        0        0     9102 2023-12-13 19:44:22.691845 magplan-3.1.0/src/magplan/templates/magplan/posts/show.html
--rw-r--r--   0        0        0      345 2023-12-13 19:44:22.691845 magplan-3.1.0/src/magplan/templates/magplan/preferences/index.html
--rw-r--r--   0        0        0      804 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/templates/magplan/sections/index.html
--rw-r--r--   0        0        0     1607 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/templates/magplan/stages/index.html
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/templatetags/__init__.py
--rw-r--r--   0        0        0     5963 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/templatetags/filters.py
--rw-r--r--   0        0        0     2611 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/urls.py
--rw-r--r--   0        0        0     1247 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/utils.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/views/__init__.py
--rw-r--r--   0        0        0      897 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/views/api.py
--rw-r--r--   0        0        0     6087 2023-12-13 19:44:22.696845 magplan-3.1.0/src/magplan/views/articles.py
--rw-r--r--   0        0        0     2838 2023-12-13 19:44:22.697845 magplan-3.1.0/src/magplan/views/authors.py
--rw-r--r--   0        0        0     7771 2023-12-13 19:44:22.697845 magplan-3.1.0/src/magplan/views/ideas.py
--rw-r--r--   0        0        0     3291 2023-12-13 19:44:22.697845 magplan-3.1.0/src/magplan/views/index.py
--rw-r--r--   0        0        0     1747 2023-12-13 19:44:22.697845 magplan-3.1.0/src/magplan/views/issues.py
--rw-r--r--   0        0        0    16403 2023-12-13 19:44:22.697845 magplan-3.1.0/src/magplan/views/posts.py
--rw-r--r--   0        0        0     1094 2023-12-13 19:44:22.697845 magplan-3.1.0/src/magplan/views/preferences.py
--rw-r--r--   0        0        0      319 2023-12-13 19:44:22.697845 magplan-3.1.0/src/magplan/views/sections.py
--rw-r--r--   0        0        0      390 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/views/stages.py
--rw-r--r--   0        0        0      390 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/README.md
--rw-r--r--   0        0        0       27 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/__init__.py
--rw-r--r--   0        0        0     3379 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/lexers.py
--rw-r--r--   0        0        0      880 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/mappers.py
--rw-r--r--   0        0        0     1421 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/markdown.py
--rw-r--r--   0        0        0     2587 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/renderer.py
--rw-r--r--   0        0        0      313 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/templates.py
--rw-r--r--   0        0        0        0 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/tests/__init__.py
--rw-r--r--   0        0        0       72 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/tests/conftest.py
--rw-r--r--   0        0        0     5958 2023-12-13 19:44:22.698845 magplan-3.1.0/src/magplan/xmd/tests/test_lexer.py
--rw-r--r--   0        0        0     1412 2023-12-13 19:44:22.709845 magplan-3.1.0/src/magplan/xmd/tests/test_renderer.py
--rw-r--r--   0        0        0     1226 2023-12-13 19:44:22.709845 magplan-3.1.0/src/magplan/xmd/tests/test_utils.py
--rw-r--r--   0        0        0      478 2023-12-13 19:44:22.709845 magplan-3.1.0/src/magplan/xmd/utils.py
--rw-r--r--   0        0        0      973 2023-12-13 19:44:22.709845 magplan-3.1.0/src/magplan/xmd/xmd.py
--rw-r--r--   0        0        0     7236 1970-01-01 00:00:00.000000 magplan-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6010 2023-12-13 19:44:22.000000 magplan-3.1.1/README.md
+-rw-r--r--   0        0        0      819 2024-04-15 14:14:16.217803 magplan-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/__init__.py
+-rw-r--r--   0        0        0     2211 2024-04-15 10:08:49.788255 magplan-3.1.1/src/magplan/admin.py
+-rw-r--r--   0        0        0       86 2024-04-15 10:08:49.747321 magplan-3.1.1/src/magplan/apps.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/conf/__init__.py
+-rw-r--r--   0        0        0     1720 2024-04-15 10:12:07.553740 magplan-3.1.1/src/magplan/conf/settings.py
+-rw-r--r--   0        0        0      556 2024-04-15 10:08:49.770398 magplan-3.1.1/src/magplan/context_processors.py
+-rw-r--r--   0        0        0     2908 2024-04-15 10:08:49.819748 magplan-3.1.1/src/magplan/dynamic_preferences_registry.py
+-rw-r--r--   0        0        0  3415905 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/fixtures/db_test.json
+-rw-r--r--   0        0        0    11011 2024-04-15 10:12:07.758358 magplan-3.1.1/src/magplan/forms.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/integrations/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-15 10:08:49.769775 magplan-3.1.1/src/magplan/integrations/images.py
+-rw-r--r--   0        0        0     4936 2024-04-15 14:14:42.235067 magplan-3.1.1/src/magplan/integrations/posts.py
+-rw-r--r--   0        0        0     1823 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39873 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2456 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40385 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/management/commands/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-15 10:08:49.771456 magplan-3.1.1/src/magplan/management/commands/render.py
+-rw-r--r--   0        0        0      748 2024-04-15 10:12:07.526323 magplan-3.1.1/src/magplan/middleware.py
+-rw-r--r--   0        0        0    17533 2024-04-15 10:12:07.987087 magplan-3.1.1/src/magplan/migrations/0001_initial.py
+-rw-r--r--   0        0        0    10857 2024-04-15 10:12:07.853222 magplan-3.1.1/src/magplan/migrations/0002_auto_20201115_1140.py
+-rw-r--r--   0        0        0      541 2024-04-15 10:08:49.809744 magplan-3.1.1/src/magplan/migrations/0003_auto_20201121_1750.py
+-rw-r--r--   0        0        0      611 2024-04-15 10:08:49.820296 magplan-3.1.1/src/magplan/migrations/0004_post_features.py
+-rw-r--r--   0        0        0     1424 2024-04-15 10:12:07.568938 magplan-3.1.1/src/magplan/migrations/0005_auto_20210213_1556.py
+-rw-r--r--   0        0        0     1005 2024-04-15 10:12:07.568958 magplan-3.1.1/src/magplan/migrations/0006_auto_20210316_1840.py
+-rw-r--r--   0        0        0      620 2024-04-15 10:12:07.553793 magplan-3.1.1/src/magplan/migrations/0007_auto_20210316_1900.py
+-rw-r--r--   0        0        0     1652 2024-04-15 10:12:07.607046 magplan-3.1.1/src/magplan/migrations/0008_auto_20210318_0108.py
+-rw-r--r--   0        0        0      610 2024-04-15 10:12:07.588161 magplan-3.1.1/src/magplan/migrations/0009_auto_20210523_1641.py
+-rw-r--r--   0        0        0     2846 2024-04-15 10:12:07.654210 magplan-3.1.1/src/magplan/migrations/0010_auto_20210624_1041.py
+-rw-r--r--   0        0        0     1274 2024-04-15 10:12:07.610111 magplan-3.1.1/src/magplan/migrations/0011_auto_20210624_1817.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/migrations/__init__.py
+-rw-r--r--   0        0        0    28279 2024-04-15 10:12:08.292154 magplan-3.1.1/src/magplan/models.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/tasks/__init__.py
+-rw-r--r--   0        0        0     3873 2024-04-15 10:12:07.677598 magplan-3.1.1/src/magplan/tasks/send_idea_comment_notification.py
+-rw-r--r--   0        0        0      468 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/tasks/send_idea_notification.py
+-rw-r--r--   0        0        0     4260 2024-04-15 10:12:07.684118 magplan-3.1.1/src/magplan/tasks/send_post_comment_notification.py
+-rw-r--r--   0        0        0      543 2024-04-15 10:08:49.906811 magplan-3.1.1/src/magplan/tasks/upload_post_to_wp.py
+-rw-r--r--   0        0        0     1790 2024-04-15 10:12:07.676796 magplan-3.1.1/src/magplan/tasks/utils.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/__init__.py
+-rw-r--r--   0        0        0     1510 2024-04-15 10:12:07.706967 magplan-3.1.1/src/magplan/templates/_test_issues.py
+-rw-r--r--   0        0        0      758 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/email/_vote_from_email.html
+-rw-r--r--   0        0        0      416 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/email/assigned_to_you.html
+-rw-r--r--   0        0        0      701 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/email/idea_approved.html
+-rw-r--r--   0        0        0      634 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/email/new_comment.html
+-rw-r--r--   0        0        0      370 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/email/new_idea.html
+-rw-r--r--   0        0        0     8503 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/layout_plan.html
+-rw-r--r--   0        0        0      893 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/articles/advert.html
+-rw-r--r--   0        0        0      860 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/articles/archived.html
+-rw-r--r--   0        0        0      855 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/articles/default.html
+-rw-r--r--   0        0        0     3053 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/articles/index.html
+-rw-r--r--   0        0        0      911 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/articles/whitelisted.html
+-rw-r--r--   0        0        0     4121 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/authors/_form.html
+-rw-r--r--   0        0        0      541 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/authors/edit.html
+-rw-r--r--   0        0        0      869 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/authors/index.html
+-rw-r--r--   0        0        0      480 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/authors/new.html
+-rw-r--r--   0        0        0     1077 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/authors/show.html
+-rw-r--r--   0        0        0      595 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/ideas/_approve_ideas.html
+-rw-r--r--   0        0        0      786 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/ideas/_authors_list.html
+-rw-r--r--   0        0        0     2332 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/ideas/_form_base.html
+-rw-r--r--   0        0        0     1088 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/ideas/_vote.html
+-rw-r--r--   0        0        0     1521 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/ideas/_voting_results.html
+-rw-r--r--   0        0        0     3959 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/ideas/index.html
+-rw-r--r--   0        0        0     3149 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/ideas/show.html
+-rw-r--r--   0        0        0     4404 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/index/index.html
+-rw-r--r--   0        0        0     1786 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/issues/_form.html
+-rw-r--r--   0        0        0     1202 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/issues/index.html
+-rw-r--r--   0        0        0      477 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/issues/new.html
+-rw-r--r--   0        0        0      837 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/issues/show.html
+-rw-r--r--   0        0        0      573 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/partials/_navbar.sites.html
+-rw-r--r--   0        0        0     1395 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/partials/_navbar_header_links.html
+-rw-r--r--   0        0        0     2797 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/partials/comments.html
+-rw-r--r--   0        0        0     2252 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/partials/navbar.html
+-rw-r--r--   0        0        0     3180 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/partials/posts_table.html
+-rw-r--r--   0        0        0      956 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_admin_set_stage.html
+-rw-r--r--   0        0        0     6970 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_attachments.html
+-rw-r--r--   0        0        0      768 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_field_col.html
+-rw-r--r--   0        0        0     3389 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_form_base.html
+-rw-r--r--   0        0        0     3359 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_form_meta.html
+-rw-r--r--   0        0        0      286 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_paywall_alert.html
+-rw-r--r--   0        0        0     1063 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_progress.html
+-rw-r--r--   0        0        0      882 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_schedule.html
+-rw-r--r--   0        0        0     2437 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/_stages.html
+-rw-r--r--   0        0        0     8559 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/edit.html
+-rw-r--r--   0        0        0     9102 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/posts/show.html
+-rw-r--r--   0        0        0      345 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/preferences/index.html
+-rw-r--r--   0        0        0      804 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/sections/index.html
+-rw-r--r--   0        0        0     1607 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templates/magplan/stages/index.html
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/templatetags/__init__.py
+-rw-r--r--   0        0        0     6000 2024-04-15 10:08:50.138892 magplan-3.1.1/src/magplan/templatetags/filters.py
+-rw-r--r--   0        0        0     2814 2024-04-15 10:12:07.760751 magplan-3.1.1/src/magplan/urls.py
+-rw-r--r--   0        0        0     1248 2024-04-15 10:08:49.983874 magplan-3.1.1/src/magplan/utils.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/views/__init__.py
+-rw-r--r--   0        0        0      898 2024-04-15 10:12:07.737198 magplan-3.1.1/src/magplan/views/api.py
+-rw-r--r--   0        0        0     6435 2024-04-15 10:08:50.142325 magplan-3.1.1/src/magplan/views/articles.py
+-rw-r--r--   0        0        0     3113 2024-04-15 10:12:07.834135 magplan-3.1.1/src/magplan/views/authors.py
+-rw-r--r--   0        0        0     7975 2024-04-15 10:12:07.938557 magplan-3.1.1/src/magplan/views/ideas.py
+-rw-r--r--   0        0        0     3321 2024-04-15 10:12:07.842747 magplan-3.1.1/src/magplan/views/index.py
+-rw-r--r--   0        0        0     1894 2024-04-15 10:12:07.826409 magplan-3.1.1/src/magplan/views/issues.py
+-rw-r--r--   0        0        0    16832 2024-04-15 10:12:08.117594 magplan-3.1.1/src/magplan/views/posts.py
+-rw-r--r--   0        0        0     1134 2024-04-15 10:12:07.855150 magplan-3.1.1/src/magplan/views/preferences.py
+-rw-r--r--   0        0        0      336 2024-04-15 10:08:50.139487 magplan-3.1.1/src/magplan/views/sections.py
+-rw-r--r--   0        0        0      473 2024-04-15 10:08:50.139462 magplan-3.1.1/src/magplan/views/stages.py
+-rw-r--r--   0        0        0      390 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/xmd/README.md
+-rw-r--r--   0        0        0       27 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/xmd/__init__.py
+-rw-r--r--   0        0        0     2909 2024-04-15 10:12:07.925445 magplan-3.1.1/src/magplan/xmd/lexers.py
+-rw-r--r--   0        0        0      874 2024-04-15 10:08:50.159967 magplan-3.1.1/src/magplan/xmd/mappers.py
+-rw-r--r--   0        0        0     1397 2024-04-15 10:08:50.169892 magplan-3.1.1/src/magplan/xmd/markdown.py
+-rw-r--r--   0        0        0     2561 2024-04-15 10:12:07.910598 magplan-3.1.1/src/magplan/xmd/renderer.py
+-rw-r--r--   0        0        0      313 2024-04-15 10:08:50.175035 magplan-3.1.1/src/magplan/xmd/templates.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/xmd/tests/__init__.py
+-rw-r--r--   0        0        0       72 2023-12-15 21:31:27.000000 magplan-3.1.1/src/magplan/xmd/tests/conftest.py
+-rw-r--r--   0        0        0     5167 2024-04-15 10:12:08.002177 magplan-3.1.1/src/magplan/xmd/tests/test_lexer.py
+-rw-r--r--   0        0        0     1526 2024-04-15 10:12:07.944020 magplan-3.1.1/src/magplan/xmd/tests/test_renderer.py
+-rw-r--r--   0        0        0     1296 2024-04-15 10:12:07.954891 magplan-3.1.1/src/magplan/xmd/tests/test_utils.py
+-rw-r--r--   0        0        0      478 2024-04-15 10:08:50.208773 magplan-3.1.1/src/magplan/xmd/utils.py
+-rw-r--r--   0        0        0      957 2024-04-15 10:08:50.224860 magplan-3.1.1/src/magplan/xmd/xmd.py
+-rw-r--r--   0        0        0     7236 1970-01-01 00:00:00.000000 magplan-3.1.1/PKG-INFO
```

### Comparing `magplan-3.1.0/README.md` & `magplan-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/pyproject.toml` & `magplan-3.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magplan"
-version = "3.1.0"
+version = "3.1.1"
 description = ""
 authors = ["Ilya Rusanen <ilya@rusanen.co.uk>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.34.0"
@@ -22,10 +22,15 @@
 pymysql = "^1.1.0"
 python-slugify = "^8.0.1"
 requests = "^2.31.0"
 sshtunnel = "^0.4.0"
 psycopg2-binary = "^2.9.9"
 
 
+[tool.poetry.group.dev.dependencies]
+black = "^24.4.0"
+mypy = "^1.9.0"
+flake8 = "^7.0.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `magplan-3.1.0/src/magplan/conf/settings.py` & `magplan-3.1.1/src/magplan/conf/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from django.conf import settings as django_settings
 
-SYSTEM_USER_ID = getattr(django_settings, 'SYSTEM_USER_ID', 'foo@bar.baz')
-PLAN_EMAIL_FROM = getattr(django_settings, 'PLAN_EMAIL_FROM', 'foo@bar.baz')
-EXTERNAL_PARSER_URL = getattr(django_settings, 'EXTERNAL_PARSER_URL', None)
-EXTERNAL_PARSER_TOKEN = getattr(django_settings, 'EXTERNAL_PARSER_TOKEN', None)
-PLAN_POSTS_INSTANCE_CHUNK = getattr(django_settings, 'PLAN_POSTS_INSTANCE_CHUNK', None)
-PLAN_EMAIL_SUBJECT_PREFIX = getattr(django_settings, 'PLAN_EMAIL_SUBJECT_PREFIX', '[magplan]')
+SYSTEM_USER_ID = getattr(django_settings, "SYSTEM_USER_ID", "foo@bar.baz")
+PLAN_EMAIL_FROM = getattr(django_settings, "PLAN_EMAIL_FROM", "foo@bar.baz")
+EXTERNAL_PARSER_URL = getattr(django_settings, "EXTERNAL_PARSER_URL", None)
+EXTERNAL_PARSER_TOKEN = getattr(django_settings, "EXTERNAL_PARSER_TOKEN", None)
+PLAN_POSTS_INSTANCE_CHUNK = getattr(
+    django_settings, "PLAN_POSTS_INSTANCE_CHUNK", None
+)
+PLAN_EMAIL_SUBJECT_PREFIX = getattr(
+    django_settings, "PLAN_EMAIL_SUBJECT_PREFIX", "[magplan]"
+)
 
-APP_HOST = getattr(django_settings, 'APP_HOST', 'magpplan.example.com')
-APP_URL = getattr(django_settings, 'APP_URL', 'https://magpplan.example.com')
-APP_ENV = getattr(django_settings, 'APP_ENV', 'PRODUCTION')
+APP_HOST = getattr(django_settings, "APP_HOST", "magpplan.example.com")
+APP_URL = getattr(django_settings, "APP_URL", "https://magpplan.example.com")
+APP_ENV = getattr(django_settings, "APP_ENV", "PRODUCTION")
 
-SSH_HOST = getattr(django_settings, 'SSH_HOST', '127.0.0.1')
-SSH_PORT = getattr(django_settings, 'SSH_PORT', 22)
-SSH_USER = getattr(django_settings, 'SSH_USER', 'user')
-SSH_PASS = getattr(django_settings, 'SSH_PASS', 'password')
+SSH_HOST = getattr(django_settings, "SSH_HOST", "127.0.0.1")
+SSH_PORT = getattr(django_settings, "SSH_PORT", 22)
+SSH_USER = getattr(django_settings, "SSH_USER", "user")
+SSH_PASS = getattr(django_settings, "SSH_PASS", "password")
 
-EXT_DB_HOST = getattr(django_settings, 'EXT_DB_HOST', '127.0.0.1')
-EXT_DB_PORT = getattr(django_settings, 'EXT_DB_PORT', '5432')
-EXT_DB_NAME = getattr(django_settings, 'EXT_DB_NAME', 'database')
-EXT_DB_USER = getattr(django_settings, 'EXT_DB_USER', 'db_user')
-EXT_DB_PASS = getattr(django_settings, 'EXT_DB_PASS', 'db_pass')
+EXT_DB_HOST = getattr(django_settings, "EXT_DB_HOST", "127.0.0.1")
+EXT_DB_PORT = getattr(django_settings, "EXT_DB_PORT", "5432")
+EXT_DB_NAME = getattr(django_settings, "EXT_DB_NAME", "database")
+EXT_DB_USER = getattr(django_settings, "EXT_DB_USER", "db_user")
+EXT_DB_PASS = getattr(django_settings, "EXT_DB_PASS", "db_pass")
 
-S3_ENDPOINT = getattr(django_settings, 'S3_ENDPOINT', 's3_endpoint')
-S3_ACCESS_KEY = getattr(django_settings, 'S3_ACCESS_KEY', 's3_access_key')
-S3_SECRET_KEY = getattr(django_settings, 'S3_SECRET_KEY', 's3_secret_key')
-S3_BUCKET_NAME = getattr(django_settings, 'S3_BUCKET_NAME', 's3_bucket_name')
-S3_STATIC_BASE_PATH = getattr(django_settings, 'S3_STATIC_BASE_PATH', 's3_static_base_path')
+S3_ENDPOINT = getattr(django_settings, "S3_ENDPOINT", "s3_endpoint")
+S3_ACCESS_KEY = getattr(django_settings, "S3_ACCESS_KEY", "s3_access_key")
+S3_SECRET_KEY = getattr(django_settings, "S3_SECRET_KEY", "s3_secret_key")
+S3_BUCKET_NAME = getattr(django_settings, "S3_BUCKET_NAME", "s3_bucket_name")
+S3_STATIC_BASE_PATH = getattr(
+    django_settings, "S3_STATIC_BASE_PATH", "s3_static_base_path"
+)
```

### Comparing `magplan-3.1.0/src/magplan/context_processors.py` & `magplan-3.1.1/src/magplan/context_processors.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from django.contrib.sites.models import Site
 
 from magplan.models import Issue
 
 
 def inject_last_issues(request):
-    issues = Issue.on_current_site.order_by('-number').all()[:5]
+    issues = Issue.on_current_site.order_by("-number").all()[:5]
     return {
-        'navbar_issues': issues,
+        "navbar_issues": issues,
     }
 
 
 def inject_app_url(request):
     return {
-        'APP_URL': os.environ.get('APP_URL', None),
+        "APP_URL": os.environ.get("APP_URL", None),
     }
 
 
 def inject_sites(request):
     current_site: Site = Site.objects.get_current(request=request)
     return {
-        'current_site': current_site,
-        'sites': Site.objects.exclude(id=current_site.id),
+        "current_site": current_site,
+        "sites": Site.objects.exclude(id=current_site.id),
     }
```

### Comparing `magplan-3.1.0/src/magplan/dynamic_preferences_registry.py` & `magplan-3.1.1/src/magplan/dynamic_preferences_registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 from django import forms
 from django.contrib.sites.models import Site
 from dynamic_preferences.preferences import Section
 from dynamic_preferences.types import ChoicePreference
 from dynamic_preferences.users.registries import user_preferences_registry
 
-plan = Section('magplan')
+plan = Section("magplan")
 
 
 @user_preferences_registry.register
 class PlanUILanguage(ChoicePreference):
-    name = 'ui_language'
+    name = "ui_language"
     section = plan
-    choices = [
-        ('en', 'English'),
-        ('ru', 'Русский')
-    ]
-    default = 'ru'
-    widget = forms.Select(attrs={'class': 'form-control'})
-    verbose_name = 'Язык интерфейса плана'
+    choices = [("en", "English"), ("ru", "Русский")]
+    default = "ru"
+    widget = forms.Select(attrs={"class": "form-control"})
+    verbose_name = "Язык интерфейса плана"
 
 
 @user_preferences_registry.register
 class PostCommentNotificationLevel(ChoicePreference):
-    name = 'post_comment_notification_level'
+    name = "post_comment_notification_level"
     section = plan
     choices = [
-        ('none', 'Не присылать уведомлений о комментариях'),
-        ('related', 'Присылать только те, что относятся ко мне'),
-        ('all', 'Присылать все уведомления'),
+        ("none", "Не присылать уведомлений о комментариях"),
+        ("related", "Присылать только те, что относятся ко мне"),
+        ("all", "Присылать все уведомления"),
     ]
-    default = 'related'
-    widget = forms.Select(attrs={'class': 'form-control'})
-    verbose_name = 'Уведомления о комментариях к посту'
+    default = "related"
+    widget = forms.Select(attrs={"class": "form-control"})
+    verbose_name = "Уведомления о комментариях к посту"
 
 
 @user_preferences_registry.register
 class IdeaCommentNotificationLevel(ChoicePreference):
-    name = 'idea_comment_notification_level'
+    name = "idea_comment_notification_level"
     section = plan
     choices = [
-        ('none', 'Не присылать уведомлений о комментариях'),
-        ('related', 'Присылать только те, что относятся ко мне'),
-        ('all', 'Присылать все уведомления'),
+        ("none", "Не присылать уведомлений о комментариях"),
+        ("related", "Присылать только те, что относятся ко мне"),
+        ("all", "Присылать все уведомления"),
     ]
-    default = 'related'
-    widget = forms.Select(attrs={'class': 'form-control'})
-    verbose_name = 'Уведомления о комментариях к идее'
+    default = "related"
+    widget = forms.Select(attrs={"class": "form-control"})
+    verbose_name = "Уведомления о комментариях к идее"
+
 
 @user_preferences_registry.register
 class XMDEditorType(ChoicePreference):
-    name = 'xmd_editor_type'
+    name = "xmd_editor_type"
     section = plan
     choices = [
-        ('plain', 'Plain-text редактор'),
-        ('markdown', 'Markdown-редактор'),
+        ("plain", "Plain-text редактор"),
+        ("markdown", "Markdown-редактор"),
     ]
-    default = 'markdown'
-    widget = forms.Select(attrs={'class': 'form-control'})
-    verbose_name = 'Редактор для статей в XMD'
+    default = "markdown"
+    widget = forms.Select(attrs={"class": "form-control"})
+    verbose_name = "Редактор для статей в XMD"
+
 
 @user_preferences_registry.register
 class NewIdeaNotification(ChoicePreference):
-    name = 'new_idea_notification'
+    name = "new_idea_notification"
     section = plan
     choices = [
-        ('yes', 'Да'),
-        ('no', 'Нет'),
+        ("yes", "Да"),
+        ("no", "Нет"),
     ]
-    default = 'yes'
-    widget = forms.Select(attrs={'class': 'form-control'})
-    verbose_name = 'Присылать уведомелния о новых идеях?'
+    default = "yes"
+    widget = forms.Select(attrs={"class": "form-control"})
+    verbose_name = "Присылать уведомелния о новых идеях?"
+
 
 @user_preferences_registry.register
 class PlanCurrentSite(ChoicePreference):
-    name = 'current_site'
+    name = "current_site"
     section = plan
-    choices = [
-        (str(s.id), s.name)
-        for s in Site.objects.all()
-    ]
-    default = '1'
-    widget = forms.Select(attrs={'class': 'form-control'})
-    verbose_name = 'Текущий сайт'
+    choices = [(str(s.id), s.name) for s in Site.objects.all()]
+    default = "1"
+    widget = forms.Select(attrs={"class": "form-control"})
+    verbose_name = "Текущий сайт"
```

### Comparing `magplan-3.1.0/src/magplan/fixtures/db_test.json` & `magplan-3.1.1/src/magplan/fixtures/db_test.json`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/integrations/posts.py` & `magplan-3.1.1/src/magplan/integrations/posts.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import pymysql
 from django.conf import settings
 from sshtunnel import SSHTunnelForwarder
 
 from magplan.xmd.mappers import s3_public_mapper
 
 img_pattern = re.compile(
-    '^'  # Only from beginning
-    ' *'  # Some leading spaces may persist
-    '!\[.*?\]\((.+)\)'  # MD image pattern
-    ' *?'  # Some ending spaces may persis
-    '$'  # Capture urls only from last section
+    "^"  # Only from beginning
+    " *"  # Some leading spaces may persist
+    "!\[.*?\]\((.+)\)"  # MD image pattern
+    " *?"  # Some ending spaces may persis
+    "$"  # Capture urls only from last section
 )
 
 url_replace_pattern = re.compile(
-    '\]\((.+)\)$'  # FIXME: match real last () group
-)
+    "\]\((.+)\)$"
+)  # FIXME: match real last () group
 
 logger = logging.getLogger()
 
 
 @contextmanager
 def Lock(post):
     post.is_locked = True
@@ -34,27 +34,29 @@
     except Exception as e:
         raise e
     finally:
         post.is_locked = False
         post.save()
 
 
-def replace_images_paths(xmd: str, attachments: tp.List, mapper: tp.Callable = None) -> str:
+def replace_images_paths(
+    xmd: str, attachments: tp.List, mapper: tp.Callable = None
+) -> str:
     """Replaces all links to local images
     to absolute paths with mapper function.
 
     Can parse both regualar images and galleries.
     If provided link not found, it's left intact.
 
     Examples:
 
         ![](image1.jpg)
         ![](image1.jpg,image2.jpg)
     """
-    logger.debug('Started replace_images_paths')
+    logger.debug("Started replace_images_paths")
     if not mapper:
         mapper = s3_public_mapper
 
     result_lines = []
 
     for line in xmd.splitlines():
         # Extract image
@@ -62,93 +64,115 @@
         if not url_chunk:  # If no image in line
             result_lines.append(line)
             continue
 
         # Parse all images for galleries one
         filenames = [
             filename.strip()
-            for filename in url_chunk[0].split(',')  # First and only match group
+            for filename in url_chunk[0].split(
+                ","
+            )  # First and only match group
         ]
         absolute_url_chunks = [
-            mapper(filename, attachments)
-            for filename in filenames
+            mapper(filename, attachments) for filename in filenames
         ]
 
         # Build result line with new images
-        absolute_urs = ']({})'.format(','.join(absolute_url_chunks))
+        absolute_urs = "]({})".format(",".join(absolute_url_chunks))
         res_line = re.sub(url_replace_pattern, absolute_urs, line)
 
         result_lines.append(res_line)
 
-    logger.debug('Finishing replace_images_paths')
-    return '\n'.join(result_lines)
+    logger.debug("Finishing replace_images_paths")
+    return "\n".join(result_lines)
 
 
-def update_post_meta_field(conn: pymysql.Connection, object_id: int, meta_key: str, meta_value: str):
+def update_post_meta_field(
+    conn: pymysql.Connection, object_id: int, meta_key: str, meta_value: str
+):
     with conn.cursor() as cursor:
-        retrieve_query = 'SELECT meta_value FROM wp_postmeta WHERE post_id=%s and meta_key=%s limit 1;'
+        retrieve_query = "SELECT meta_value FROM wp_postmeta WHERE post_id=%s and meta_key=%s limit 1;"
         cursor.execute(retrieve_query, (object_id, meta_key))
 
         # Update existing if found
         existing_rows = cursor.fetchone()
         if existing_rows:
-            update_query = 'UPDATE wp_postmeta SET meta_value=%s WHERE post_id=%s and meta_key=%s;'
+            update_query = "UPDATE wp_postmeta SET meta_value=%s WHERE post_id=%s and meta_key=%s;"
         else:
-            update_query = 'INSERT INTO wp_postmeta (meta_value, post_id, meta_key) VALUES (%s, %s, %s);'
-        cursor.execute(update_query, (meta_value, object_id, meta_key,))
+            update_query = "INSERT INTO wp_postmeta (meta_value, post_id, meta_key) VALUES (%s, %s, %s);"
+        cursor.execute(
+            update_query,
+            (
+                meta_value,
+                object_id,
+                meta_key,
+            ),
+        )
 
     conn.commit()
 
 
-def update_post_field(conn: pymysql.Connection, object_id: int, key: str, value: str):
+def update_post_field(
+    conn: pymysql.Connection, object_id: int, key: str, value: str
+):
     with conn.cursor() as cursor:
-        update_query = f'UPDATE wp_posts SET {key}=%s WHERE ID=%s;'  # Injection-safe as key is trusted
-        cursor.execute(update_query, (value, object_id,))
+        update_query = f"UPDATE wp_posts SET {key}=%s WHERE ID=%s;"  # Injection-safe as key is trusted
+        cursor.execute(
+            update_query,
+            (
+                value,
+                object_id,
+            ),
+        )
 
     conn.commit()
 
 
 def update_ext_db_xmd(
-        post_id: int,
-        *,
-        xmd: str = None, title: str = None, css: str = None, post_date: str = None, post_date_gmt: str = None
+    post_id: int,
+    *,
+    xmd: str = None,
+    title: str = None,
+    css: str = None,
+    post_date: str = None,
+    post_date_gmt: str = None,
 ) -> None:
     """
     Updates provided kwargs for post with post_id in external DB
     """
-    logger.info('Staring updating external database')
+    logger.info("Staring updating external database")
 
     if not all(settings.EXT_DB.get(key) for key in settings.EXT_DB.keys()):
         return
 
     conf = settings.EXT_DB
 
     # Prepare settings for SSH tunnel connection
-    ssh_conn_args = ((conf['SSH_HOST'], int(conf['SSH_PORT'])),)
+    ssh_conn_args = ((conf["SSH_HOST"], int(conf["SSH_PORT"])),)
     ssh_conn_kwargs = {
-        'ssh_username': conf['SSH_USER'],
-        'ssh_password': conf['SSH_PASS'],
-        'remote_bind_address': (conf['EXT_DB_HOST'], int(conf['EXT_DB_PORT']))
+        "ssh_username": conf["SSH_USER"],
+        "ssh_password": conf["SSH_PASS"],
+        "remote_bind_address": (conf["EXT_DB_HOST"], int(conf["EXT_DB_PORT"])),
     }
 
     with SSHTunnelForwarder(*ssh_conn_args, **ssh_conn_kwargs) as tunnel:
         mysql_conn_settings = {
-            'host': tunnel.local_bind_host,
-            'port': tunnel.local_bind_port,
-            'user': conf['EXT_DB_USER'],
-            'passwd': conf['EXT_DB_PASS'],
-            'db': conf['EXT_DB_NAME'],
+            "host": tunnel.local_bind_host,
+            "port": tunnel.local_bind_port,
+            "user": conf["EXT_DB_USER"],
+            "passwd": conf["EXT_DB_PASS"],
+            "db": conf["EXT_DB_NAME"],
         }
         conn = pymysql.connect(**mysql_conn_settings)
 
         if xmd:
-            update_post_meta_field(conn, post_id, 'md', xmd)
+            update_post_meta_field(conn, post_id, "md", xmd)
         if css:
-            update_post_meta_field(conn, post_id, 'css', css)
+            update_post_meta_field(conn, post_id, "css", css)
         if title:
-            update_post_field(conn, post_id, 'post_title', title)
+            update_post_field(conn, post_id, "post_title", title)
         if post_date:
-            update_post_field(conn, post_id, 'post_date', post_date)
+            update_post_field(conn, post_id, "post_date", post_date)
         if post_date_gmt:
-            update_post_field(conn, post_id, 'post_date_gmt', post_date_gmt)
+            update_post_field(conn, post_id, "post_date_gmt", post_date_gmt)
 
         conn.close()
```

### Comparing `magplan-3.1.0/src/magplan/locale/en/LC_MESSAGES/django.mo` & `magplan-3.1.1/src/magplan/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/locale/en/LC_MESSAGES/django.po` & `magplan-3.1.1/src/magplan/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/locale/ru/LC_MESSAGES/django.mo` & `magplan-3.1.1/src/magplan/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/locale/ru/LC_MESSAGES/django.po` & `magplan-3.1.1/src/magplan/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/middleware.py` & `magplan-3.1.1/src/magplan/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,17 @@
     def __init__(self, get_response):
         self.get_response = get_response
         # One-time configuration and initialization.
 
     def __call__(self, request):
         # Set user language from settings
         try:
-            user_language = request.user.user.preferences.get('magplan__ui_language')
+            user_language = request.user.user.preferences.get(
+                "magplan__ui_language"
+            )
             translation.activate(user_language)
             request.session[translation.LANGUAGE_SESSION_KEY] = user_language
         except:
             # HACK: should not raise I18n errors if Accept-Language
             # or settings is not configured
             pass
```

### Comparing `magplan-3.1.0/src/magplan/migrations/0003_auto_20201121_1750.py` & `magplan-3.1.1/src/magplan/migrations/0003_auto_20201121_1750.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('magplan', '0002_auto_20201115_1140'),
+        ("magplan", "0002_auto_20201115_1140"),
     ]
 
     operations = [
         migrations.DeleteModel(
-            name='Widget',
+            name="Widget",
         ),
         migrations.DeleteModel(
-            name='Widgetype',
+            name="Widgetype",
         ),
         migrations.RemoveField(
-            model_name='post',
-            name='postype',
+            model_name="post",
+            name="postype",
         ),
         migrations.DeleteModel(
-            name='Postype',
+            name="Postype",
         ),
     ]
```

### Comparing `magplan-3.1.0/src/magplan/migrations/0006_auto_20210316_1840.py` & `magplan-3.1.1/src/magplan/migrations/0006_auto_20210316_1840.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,33 @@
 import django.db.models.deletion
 import django.db.models.manager
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('sites', '0002_alter_domain_unique'),
-        ('magplan', '0005_auto_20210213_1556'),
+        ("sites", "0002_alter_domain_unique"),
+        ("magplan", "0005_auto_20210213_1556"),
     ]
 
     operations = [
         migrations.AlterModelManagers(
-            name='post',
+            name="post",
             managers=[
-                ('objects', django.db.models.manager.Manager()),
-                ('on_site', django.contrib.sites.managers.CurrentSiteManager()),
+                ("objects", django.db.models.manager.Manager()),
+                (
+                    "on_site",
+                    django.contrib.sites.managers.CurrentSiteManager(),
+                ),
             ],
         ),
         migrations.AddField(
-            model_name='post',
-            name='site',
-            field=models.ForeignKey(default=1, on_delete=django.db.models.deletion.CASCADE, to='sites.site'),
+            model_name="post",
+            name="site",
+            field=models.ForeignKey(
+                default=1,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="sites.site",
+            ),
             preserve_default=False,
         ),
     ]
```

### Comparing `magplan-3.1.0/src/magplan/migrations/0007_auto_20210316_1900.py` & `magplan-3.1.1/src/magplan/migrations/0007_auto_20210316_1900.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 from django.db import migrations
 import django.db.models.manager
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('magplan', '0006_auto_20210316_1840'),
+        ("magplan", "0006_auto_20210316_1840"),
     ]
 
     operations = [
         migrations.AlterModelManagers(
-            name='post',
+            name="post",
             managers=[
-                ('objects', django.db.models.manager.Manager()),
-                ('on_current_site', django.contrib.sites.managers.CurrentSiteManager()),
+                ("objects", django.db.models.manager.Manager()),
+                (
+                    "on_current_site",
+                    django.contrib.sites.managers.CurrentSiteManager(),
+                ),
             ],
         ),
     ]
```

### Comparing `magplan-3.1.0/src/magplan/migrations/0010_auto_20210624_1041.py` & `magplan-3.1.1/src/magplan/migrations/0010_auto_20210624_1041.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,57 +6,88 @@
 import django.db.models.manager
 import magplan.models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('sites', '0002_alter_domain_unique'),
-        ('magplan', '0009_auto_20210523_1641'),
+        ("sites", "0002_alter_domain_unique"),
+        ("magplan", "0009_auto_20210523_1641"),
     ]
 
     operations = [
         migrations.AlterModelManagers(
-            name='idea',
+            name="idea",
             managers=[
-                ('objects', django.db.models.manager.Manager()),
-                ('on_current_site', django.contrib.sites.managers.CurrentSiteManager()),
+                ("objects", django.db.models.manager.Manager()),
+                (
+                    "on_current_site",
+                    django.contrib.sites.managers.CurrentSiteManager(),
+                ),
             ],
         ),
         migrations.AlterModelManagers(
-            name='issue',
+            name="issue",
             managers=[
-                ('objects', django.db.models.manager.Manager()),
-                ('on_current_site', django.contrib.sites.managers.CurrentSiteManager()),
+                ("objects", django.db.models.manager.Manager()),
+                (
+                    "on_current_site",
+                    django.contrib.sites.managers.CurrentSiteManager(),
+                ),
             ],
         ),
         migrations.AddField(
-            model_name='idea',
-            name='site',
-            field=models.ForeignKey(default=magplan.models.current_site_id, on_delete=django.db.models.deletion.CASCADE, to='sites.site'),
+            model_name="idea",
+            name="site",
+            field=models.ForeignKey(
+                default=magplan.models.current_site_id,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="sites.site",
+            ),
         ),
         migrations.AddField(
-            model_name='issue',
-            name='site',
-            field=models.ForeignKey(default=magplan.models.current_site_id, on_delete=django.db.models.deletion.CASCADE, to='sites.site'),
+            model_name="issue",
+            name="site",
+            field=models.ForeignKey(
+                default=magplan.models.current_site_id,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="sites.site",
+            ),
         ),
         migrations.AlterField(
-            model_name='post',
-            name='site',
-            field=models.ForeignKey(default=magplan.models.current_site_id, on_delete=django.db.models.deletion.CASCADE, to='sites.site'),
+            model_name="post",
+            name="site",
+            field=models.ForeignKey(
+                default=magplan.models.current_site_id,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="sites.site",
+            ),
         ),
         migrations.AlterField(
-            model_name='post',
-            name='slug',
-            field=models.SlugField(blank=True, max_length=255, null=True, verbose_name='Слаг для URL'),
+            model_name="post",
+            name="slug",
+            field=models.SlugField(
+                blank=True,
+                max_length=255,
+                null=True,
+                verbose_name="Слаг для URL",
+            ),
         ),
         migrations.AlterField(
-            model_name='section',
-            name='site',
-            field=models.ForeignKey(default=magplan.models.current_site_id, on_delete=django.db.models.deletion.CASCADE, to='sites.site'),
+            model_name="section",
+            name="site",
+            field=models.ForeignKey(
+                default=magplan.models.current_site_id,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="sites.site",
+            ),
         ),
         migrations.AlterField(
-            model_name='stage',
-            name='site',
-            field=models.ForeignKey(default=magplan.models.current_site_id, on_delete=django.db.models.deletion.CASCADE, to='sites.site'),
+            model_name="stage",
+            name="site",
+            field=models.ForeignKey(
+                default=magplan.models.current_site_id,
+                on_delete=django.db.models.deletion.CASCADE,
+                to="sites.site",
+            ),
         ),
     ]
```

### Comparing `magplan-3.1.0/src/magplan/migrations/0011_auto_20210624_1817.py` & `magplan-3.1.1/src/magplan/migrations/0011_auto_20210624_1817.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,44 @@
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('magplan', '0010_auto_20210624_1041'),
+        ("magplan", "0010_auto_20210624_1041"),
     ]
 
     operations = [
         migrations.AddField(
-            model_name='profile',
-            name='bio',
-            field=models.TextField(blank=True, null=True, verbose_name='Био'),
+            model_name="profile",
+            name="bio",
+            field=models.TextField(blank=True, null=True, verbose_name="Био"),
         ),
         migrations.AddField(
-            model_name='profile',
-            name='bio_generic',
-            field=models.TextField(blank=True, null=True, verbose_name='Био латинницей'),
+            model_name="profile",
+            name="bio_generic",
+            field=models.TextField(
+                blank=True, null=True, verbose_name="Био латинницей"
+            ),
         ),
         migrations.AddField(
-            model_name='profile',
-            name='f_name_generic',
-            field=models.CharField(blank=True, max_length=255, null=True, verbose_name='Имя латинницей'),
+            model_name="profile",
+            name="f_name_generic",
+            field=models.CharField(
+                blank=True,
+                max_length=255,
+                null=True,
+                verbose_name="Имя латинницей",
+            ),
         ),
         migrations.AddField(
-            model_name='profile',
-            name='l_name_generic',
-            field=models.CharField(blank=True, max_length=255, null=True, verbose_name='Фамилия латинницей'),
+            model_name="profile",
+            name="l_name_generic",
+            field=models.CharField(
+                blank=True,
+                max_length=255,
+                null=True,
+                verbose_name="Фамилия латинницей",
+            ),
         ),
     ]
```

### Comparing `magplan-3.1.0/src/magplan/models.py` & `magplan-3.1.1/src/magplan/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,37 +10,40 @@
 
 import django
 import html2text
 import requests
 from botocore.exceptions import ClientError
 from django.conf import settings
 from django.contrib.auth import get_user_model
-from django.contrib.contenttypes.fields import GenericRelation, GenericForeignKey
+from django.contrib.contenttypes.fields import (
+    GenericRelation,
+    GenericForeignKey,
+)
 from django.contrib.contenttypes.models import ContentType
 from django.contrib.postgres.fields import JSONField
 from django.contrib.sites.managers import CurrentSiteManager
 from django.contrib.sites.models import Site
 from django.core.mail import EmailMultiAlternatives
 from django.db import models
 from django.db.models import Q, QuerySet
 from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
 from django.template.loader import render_to_string
 from django.utils import timezone
 
-from magplan.conf import settings as  config
+from magplan.conf import settings as config
 from magplan.integrations.images import S3Client
 from magplan.integrations.posts import replace_images_paths, update_ext_db_xmd
 from magplan.xmd import render_md
 from magplan.xmd.mappers import s3_public_mapper as s3_image_mapper
 
-NEW_IDEA_NOTIFICATION_PREFERENCE_NAME = 'magplan__new_idea_notification'
-WP_DATE_FORMAT_STRING = '%Y-%m-%d %H:%M:%S'
+NEW_IDEA_NOTIFICATION_PREFERENCE_NAME = "magplan__new_idea_notification"
+WP_DATE_FORMAT_STRING = "%Y-%m-%d %H:%M:%S"
 
-S3_STATIC_BASE_PATH = os.environ.get('S3_STATIC_BASE_PATH')
+S3_STATIC_BASE_PATH = os.environ.get("S3_STATIC_BASE_PATH")
 
 from .xmd.mappers import plan_internal_mapper as plan_image_mapper
 
 UserModel = get_user_model()
 
 logger = logging.getLogger()
 
@@ -62,15 +65,18 @@
     return settings.SITE_ID
 
 
 class AbstractSiteModel(models.Model):
     """
     Support for multisite managers
     """
-    site = models.ForeignKey(Site, on_delete=models.CASCADE, default=current_site_id)
+
+    site = models.ForeignKey(
+        Site, on_delete=models.CASCADE, default=current_site_id
+    )
     objects = models.Manager()
     on_current_site = CurrentSiteManager()
 
     class Meta:
         abstract = True
 
     @classmethod
@@ -90,25 +96,25 @@
     def __str__(self):
         return self.display_name_default
 
     @property
     def display_name_default(self):
         p: Profile = self.profile
         if p.l_name and p.f_name:
-            return '%s %s' % (p.f_name, p.l_name)
+            return "%s %s" % (p.f_name, p.l_name)
         elif p.n_name:
             return p.n_name
         else:
             return self.email
 
     @property
     def display_name_generic(self):
         p: Profile = self.profile
         if p.l_name_generic and p.f_name_generic:
-            return '%s %s' % (p.f_name_generic, p.l_name_generic)
+            return "%s %s" % (p.f_name_generic, p.l_name_generic)
         elif p.n_name:
             return p.n_name
         else:
             return self.email
 
     @property
     def str_reverse(self):
@@ -131,182 +137,216 @@
         :return: True if a memeber, otherwise False
         """
         return self.groups.filter(name=group_name).exists()
 
 
 class Profile(AbstractBase):
     is_public = models.BooleanField(null=False, blank=False, default=False)
-    user = models.OneToOneField(User, on_delete=models.CASCADE, related_name='profile')
-    f_name = models.CharField('Имя', max_length=255, blank=True, null=True)
-    m_name = models.CharField('Отчество', max_length=255, blank=True, null=True)
-    l_name = models.CharField('Фамилия', max_length=255, blank=True, null=True)
-    n_name = models.CharField('Ник', max_length=255, blank=True, null=True)
-    bio = models.TextField('Био', blank=True, null=True)
+    user = models.OneToOneField(
+        User, on_delete=models.CASCADE, related_name="profile"
+    )
+    f_name = models.CharField("Имя", max_length=255, blank=True, null=True)
+    m_name = models.CharField(
+        "Отчество", max_length=255, blank=True, null=True
+    )
+    l_name = models.CharField("Фамилия", max_length=255, blank=True, null=True)
+    n_name = models.CharField("Ник", max_length=255, blank=True, null=True)
+    bio = models.TextField("Био", blank=True, null=True)
 
     # Global fields
-    f_name_generic = models.CharField('Имя латинницей', max_length=255, blank=True, null=True)
-    l_name_generic = models.CharField('Фамилия латинницей', max_length=255, blank=True, null=True)
-    bio_generic = models.TextField('Био латинницей', blank=True, null=True)
+    f_name_generic = models.CharField(
+        "Имя латинницей", max_length=255, blank=True, null=True
+    )
+    l_name_generic = models.CharField(
+        "Фамилия латинницей", max_length=255, blank=True, null=True
+    )
+    bio_generic = models.TextField("Био латинницей", blank=True, null=True)
 
     RUSSIA = 0
     UKRAINE = 1
     BELARUS = 2
     KAZAKHSTAN = 3
     COUNTRY_CHOICES = (
-        (RUSSIA, 'Россия'),
-        (UKRAINE, 'Украина'),
-        (BELARUS, 'Беларусь'),
-        (KAZAKHSTAN, 'Казахстан'),
+        (RUSSIA, "Россия"),
+        (UKRAINE, "Украина"),
+        (BELARUS, "Беларусь"),
+        (KAZAKHSTAN, "Казахстан"),
     )
     country = models.SmallIntegerField(
-        'Страна', choices=COUNTRY_CHOICES, default=RUSSIA
+        "Страна", choices=COUNTRY_CHOICES, default=RUSSIA
     )
-    city = models.CharField('Город или поселок', max_length=255, blank=True, null=True)
-    notes = models.TextField('Примечания', blank=True, null=True)
+    city = models.CharField(
+        "Город или поселок", max_length=255, blank=True, null=True
+    )
+    notes = models.TextField("Примечания", blank=True, null=True)
 
 
 class Section(AbstractSiteModel, AbstractBase):
     def __str__(self):
         return self.title
 
     slug = models.SlugField(null=False, blank=False, max_length=255)
     title = models.CharField(null=False, blank=False, max_length=255)
     description = models.TextField(null=True, blank=False)
     sort = models.SmallIntegerField(null=False, blank=False, default=0)
-    color = models.CharField(null=False, blank=False, default='000000', max_length=6)
+    color = models.CharField(
+        null=False, blank=False, default="000000", max_length=6
+    )
     is_archived = models.BooleanField(null=False, blank=False, default=False)
-    is_whitelisted = models.BooleanField(null=False, blank=False, default=False)
+    is_whitelisted = models.BooleanField(
+        null=False, blank=False, default=False
+    )
 
 
 class Magazine(AbstractBase):
     slug = models.SlugField(null=False, blank=False, max_length=255)
     title = models.CharField(null=False, blank=False, max_length=255)
     description = models.TextField(null=False, blank=True)
 
     def __str__(self):
         return self.title
 
 
 class Issue(AbstractSiteModel, AbstractBase):
     class Meta:
-        ordering = ['-number']
+        ordering = ["-number"]
 
     def __str__(self):
-        return '%s #%s' % (self.magazine, self.number)
+        return "%s #%s" % (self.magazine, self.number)
 
     number = models.SmallIntegerField(null=False, blank=False, default=0)
     title = models.CharField(null=True, blank=False, max_length=255)
     description = models.TextField(null=True, blank=False)
     magazine = models.ForeignKey(Magazine, on_delete=models.CASCADE)
     published_at = models.DateField(
         null=False, blank=False, default=datetime.date.today
     )
 
     @property
     def full_title(self) -> str:
-        return '{} #{} {}'.format(
-            'Хакер', self.number, self.title or ''
-        )
+        return "{} #{} {}".format("Хакер", self.number, self.title or "")
 
 
 class Stage(AbstractSiteModel, AbstractBase):
     def __str__(self):
         return self.title
 
     slug = models.SlugField(null=False, blank=False, max_length=255)
     title = models.CharField(null=False, blank=False, max_length=255)
     sort = models.SmallIntegerField(null=False, blank=False, default=0)
     duration = models.SmallIntegerField(null=True, blank=True, default=1)
-    assignee = models.ForeignKey(User, null=True, blank=True, on_delete=models.CASCADE)
+    assignee = models.ForeignKey(
+        User, null=True, blank=True, on_delete=models.CASCADE
+    )
     prev_stage = models.ForeignKey(
-        'self', related_name='n_stage', null=True, blank=True, on_delete=models.CASCADE
+        "self",
+        related_name="n_stage",
+        null=True,
+        blank=True,
+        on_delete=models.CASCADE,
     )
     next_stage = models.ForeignKey(
-        'self', related_name='p_stage', null=True, blank=True, on_delete=models.CASCADE
+        "self",
+        related_name="p_stage",
+        null=True,
+        blank=True,
+        on_delete=models.CASCADE,
+    )
+    skip_notification = models.BooleanField(
+        null=False, blank=False, default=False
     )
-    skip_notification = models.BooleanField(null=False, blank=False, default=False)
     meta = JSONField(default=dict)
 
 
 class Idea(AbstractSiteModel, AbstractBase):
-    AUTHOR_TYPE_NO = 'NO'
-    AUTHOR_TYPE_NEW = 'NW'
-    AUTHOR_TYPE_EXISTING = 'EX'
+    AUTHOR_TYPE_NO = "NO"
+    AUTHOR_TYPE_NEW = "NW"
+    AUTHOR_TYPE_EXISTING = "EX"
     AUTHOR_TYPE_CHOICES = [
-        (AUTHOR_TYPE_NO, 'Нет автора'),
-        (AUTHOR_TYPE_NEW, 'Новый автор'),
-        (AUTHOR_TYPE_EXISTING, 'Существующий автор(ы)'),
+        (AUTHOR_TYPE_NO, "Нет автора"),
+        (AUTHOR_TYPE_NEW, "Новый автор"),
+        (AUTHOR_TYPE_EXISTING, "Существующий автор(ы)"),
     ]
     title = models.CharField(
-        null=False, blank=False, max_length=255, verbose_name='Заголовок'
+        null=False, blank=False, max_length=255, verbose_name="Заголовок"
     )
-    description = models.TextField(verbose_name='Описание')
+    description = models.TextField(verbose_name="Описание")
     approved = models.BooleanField(null=True)
-    editor = models.ForeignKey(User, on_delete=models.CASCADE, related_name='editor')
+    editor = models.ForeignKey(
+        User, on_delete=models.CASCADE, related_name="editor"
+    )
     post = models.OneToOneField(
-        'Post', on_delete=models.SET_NULL, null=True, blank=True
+        "Post", on_delete=models.SET_NULL, null=True, blank=True
     )
-    comments = GenericRelation('Comment')
+    comments = GenericRelation("Comment")
     author_type = models.CharField(
         max_length=2,
         choices=AUTHOR_TYPE_CHOICES,
         default=AUTHOR_TYPE_NO,
-        verbose_name='Автор',
+        verbose_name="Автор",
     )
     authors_new = models.CharField(
-        max_length=255, null=True, blank=True, verbose_name='Новые автор'
+        max_length=255, null=True, blank=True, verbose_name="Новые автор"
     )
     authors = models.ManyToManyField(
-        User, verbose_name='Авторы', related_name='authors', blank=True
+        User, verbose_name="Авторы", related_name="authors", blank=True
     )
 
     def voted(self, user):
-        vote = next((v for v in self.votes.all() if v.user_id == user.id), None)
+        vote = next(
+            (v for v in self.votes.all() if v.user_id == user.id), None
+        )
 
         if vote:
             return True
         return False
 
     def _send_vote_notification(self, recipient: User) -> None:
-        subject = f'Новая идея «{self.title}». Голосуйте!'
+        subject = f"Новая идея «{self.title}». Голосуйте!"
 
-        context = {
-            'idea': self,
-            'APP_URL': os.environ.get('APP_URL')
-        }
-        message_html_content: str = render_to_string('email/new_idea.html', context)
+        context = {"idea": self, "APP_URL": os.environ.get("APP_URL")}
+        message_html_content: str = render_to_string(
+            "email/new_idea.html", context
+        )
         message_text_content: str = html2text.html2text(message_html_content)
 
-        msg = EmailMultiAlternatives(subject, message_text_content, config.PLAN_EMAIL_FROM,
-                                     [recipient.email])
-        msg.attach_alternative(message_html_content, 'text/html')
+        msg = EmailMultiAlternatives(
+            subject,
+            message_text_content,
+            config.PLAN_EMAIL_FROM,
+            [recipient.email],
+        )
+        msg.attach_alternative(message_html_content, "text/html")
         msg.send()
 
     def send_vote_notifications(self) -> None:
-        active_users: tp.List[User] = User.objects.filter(is_active=True).exclude(id=self.editor_id)
+        active_users: tp.List[User] = User.objects.filter(
+            is_active=True
+        ).exclude(id=self.editor_id)
         recipients: tp.List[User] = [
-            user for user in active_users
+            user
+            for user in active_users
             if user.preferences[NEW_IDEA_NOTIFICATION_PREFERENCE_NAME]
         ]
 
         for recipient in recipients:
             self._send_vote_notification(recipient)
 
     def __str__(self):
         return self.title
 
     class Meta:
         permissions = (
-            ('edit_extended_idea_attrs', 'Edit extended Idea attributes'),
-            ('recieve_idea_email_updates', 'Recieve email updates for Idea'),
+            ("edit_extended_idea_attrs", "Edit extended Idea attributes"),
+            ("recieve_idea_email_updates", "Recieve email updates for Idea"),
         )
 
     @property
     def comments_(self):
-        return self.comments.order_by('created_at').all
+        return self.comments.order_by("created_at").all
 
     @property
     def score(self):
         MAX_SCORE = 100
 
         all_scores = sum([v.score for v in self.votes.all()])
         max_scores = len(self.votes.all()) * MAX_SCORE
@@ -317,143 +357,161 @@
     def description_html(self):
         return render_md(self.description)
 
 
 class Post(AbstractSiteModel, AbstractBase):
     # Used for external parser configuration
     PAYWALL_NOTICE_HEAD = '<div class="paywall-notice">'
-    PAYWALL_NOTICE_BODY = 'Продолжение статьи доступно только продписчикам'
-    PAYWALL_NOTICE_TAIL = '</div>'
-    PAYWALL_NOTICE_RENDERED = '{}{}{}'.format(
+    PAYWALL_NOTICE_BODY = "Продолжение статьи доступно только продписчикам"
+    PAYWALL_NOTICE_TAIL = "</div>"
+    PAYWALL_NOTICE_RENDERED = "{}{}{}".format(
         PAYWALL_NOTICE_HEAD, PAYWALL_NOTICE_BODY, PAYWALL_NOTICE_TAIL
     )
 
     @property
     def full_title(self) -> str:
         if self.kicker is None:
             return self.title
 
-        separator = ' ' if self.kicker.endswith(('!', ':', '?')) else '. '
-        return f'{self.kicker}{separator}{self.title}'
+        separator = " " if self.kicker.endswith(("!", ":", "?")) else ". "
+        return f"{self.kicker}{separator}{self.title}"
 
     def __str__(self) -> str:
         return self.full_title
 
     POST_FORMAT_DEFAULT = 0
     POST_FORMAT_FEATURED = 1
     POST_FORMAT_CHOICES = (
-        (POST_FORMAT_DEFAULT, 'Default'),
-        (POST_FORMAT_FEATURED, 'Featured'),
+        (POST_FORMAT_DEFAULT, "Default"),
+        (POST_FORMAT_FEATURED, "Featured"),
     )
 
     format = models.SmallIntegerField(
         choices=POST_FORMAT_CHOICES, default=POST_FORMAT_DEFAULT
     )
 
     POST_FEATURES_DEFAULT = 0
     POST_FEATURES_ARCHIVE = 1
     POST_FEATURES_ADVERT = 2
     POST_FEATURES_TRANSLATED = 2
     POST_FEATURES_CHOICES = (
-        (POST_FEATURES_DEFAULT, 'Default'),
-        (POST_FEATURES_ARCHIVE, 'Archive'),
-        (POST_FEATURES_ADVERT, 'Advert'),
-        (POST_FEATURES_TRANSLATED, 'Translated'),
+        (POST_FEATURES_DEFAULT, "Default"),
+        (POST_FEATURES_ARCHIVE, "Archive"),
+        (POST_FEATURES_ADVERT, "Advert"),
+        (POST_FEATURES_TRANSLATED, "Translated"),
+    )
+    features = models.SmallIntegerField(
+        choices=POST_FEATURES_CHOICES, default=POST_FEATURES_DEFAULT
     )
-    features = models.SmallIntegerField(choices=POST_FEATURES_CHOICES,
-                                        default=POST_FEATURES_DEFAULT)
 
     finished_at = models.DateTimeField(
         null=False,
         blank=False,
         default=django.utils.timezone.now,
-        verbose_name='Дедлайн',
+        verbose_name="Дедлайн",
     )
     published_at = models.DateTimeField(
-        null=True, blank=True, verbose_name='Дата публикации'
+        null=True, blank=True, verbose_name="Дата публикации"
     )
     kicker = models.CharField(null=True, blank=True, max_length=255)
-    slug = models.SlugField(null=True, blank=True, max_length=255, verbose_name='Слаг для URL')
+    slug = models.SlugField(
+        null=True, blank=True, max_length=255, verbose_name="Слаг для URL"
+    )
     title = models.CharField(
-        null=True, blank=True, max_length=255, verbose_name='Заголовок статьи'
+        null=True, blank=True, max_length=255, verbose_name="Заголовок статьи"
     )
     description = models.TextField(
-        null=False, blank=True, verbose_name='Описание статьи'
+        null=False, blank=True, verbose_name="Описание статьи"
     )
     views = models.IntegerField(default=0)
     is_paywalled = models.BooleanField(default=False)
     xmd = models.TextField(null=True)
     html = models.TextField(null=True)
 
     editor = models.ForeignKey(
         User,
         null=True,
         on_delete=models.CASCADE,
         related_name="edited",
-        verbose_name='Редактор',
+        verbose_name="Редактор",
+    )
+    authors = models.ManyToManyField(User, verbose_name="Авторы")
+    stage = models.ForeignKey(
+        Stage, on_delete=models.CASCADE, verbose_name="Этап"
+    )
+    issues = models.ManyToManyField(
+        Issue, related_name="posts", verbose_name="Выпуски"
     )
-    authors = models.ManyToManyField(User, verbose_name='Авторы')
-    stage = models.ForeignKey(Stage, on_delete=models.CASCADE, verbose_name='Этап')
-    issues = models.ManyToManyField(Issue, related_name='posts', verbose_name='Выпуски')
     section = models.ForeignKey(
         Section,
         on_delete=models.CASCADE,
         null=False,
         blank=False,
-        verbose_name='Раздел',
+        verbose_name="Раздел",
     )
     last_updater = models.ForeignKey(
         User,
-        related_name='posts_updated',
-        verbose_name='Кто последний обновлял',
+        related_name="posts_updated",
+        verbose_name="Кто последний обновлял",
         null=True,
         on_delete=models.SET_NULL,
     )
 
     meta = JSONField(default=dict)
 
-    comments = GenericRelation('Comment')
+    comments = GenericRelation("Comment")
     is_locked = models.BooleanField(default=False)
     css = models.TextField(
-        null=True, blank=True, verbose_name='CSS-стили для статьи',
-        help_text=(
-            'CSS, который будет применяться к превью статьи'
-        )
+        null=True,
+        blank=True,
+        verbose_name="CSS-стили для статьи",
+        help_text=("CSS, который будет применяться к превью статьи"),
     )
 
     def imprint_updater(self, user: User) -> None:
         """Update updated_at timestamp and set provided user as last_updater.
 
         `created_at` may be overwritten further on DB-hook level.
         .save() method should be explicitly called.
         """
         self.last_updater = user
         self.updated_at = datetime.datetime.now()
 
     @property
     def images(self):
         return list(
-            filter(lambda a: a.type == Attachment.TYPE_IMAGE, self.attachment_set.all())
+            filter(
+                lambda a: a.type == Attachment.TYPE_IMAGE,
+                self.attachment_set.all(),
+            )
         )
 
     @property
     def pdfs(self):
         return list(
-            filter(lambda a: a.type == Attachment.TYPE_PDF, self.attachment_set.all())
+            filter(
+                lambda a: a.type == Attachment.TYPE_PDF,
+                self.attachment_set.all(),
+            )
         )
 
     @property
     def files(self):
         return list(
-            filter(lambda a: a.type == Attachment.TYPE_FILE, self.attachment_set.all())
+            filter(
+                lambda a: a.type == Attachment.TYPE_FILE,
+                self.attachment_set.all(),
+            )
         )
 
     @property
-    def featured_image(self) -> tp.Optional['Attachment']:
-        return self.attachment_set.filter(type=Attachment.TYPE_FEATURED_IMAGE).first()
+    def featured_image(self) -> tp.Optional["Attachment"]:
+        return self.attachment_set.filter(
+            type=Attachment.TYPE_FEATURED_IMAGE
+        ).first()
 
     @property
     def assignee(self):
         if self.stage and self.stage.assignee:
             return self.stage.assignee
         elif self.editor:
             return self.editor
@@ -472,19 +530,19 @@
         if self.stage.next_stage and self.stage.next_stage.assignee:
             return self.stage.next_stage.assignee
         else:
             return self.editor
 
     @property
     def comments_(self):
-        return self.comments.order_by('created_at').all
+        return self.comments.order_by("created_at").all
 
     @property
     def has_text(self):
-        return self.xmd is not None and self.xmd != ''
+        return self.xmd is not None and self.xmd != ""
 
     @property
     def is_default(self):
         return self.features == self.POST_FEATURES_DEFAULT
 
     @property
     def is_archive(self):
@@ -500,145 +558,150 @@
 
     @property
     def is_translated(self):
         return self.features == self.POST_FEATURES_TRANSLATED
 
     class Meta:
         permissions = (
-            ('recieve_post_email_updates', 'Recieve email updates for Post'),
-            ('edit_extended_post_attrs', 'Edit extended Post attributes'),
+            ("recieve_post_email_updates", "Recieve email updates for Post"),
+            ("edit_extended_post_attrs", "Edit extended Post attributes"),
             # Direct article creation
-            ('create_generic_post', 'Create generic post'),
-            ('create_archive_post', 'Create archive post'),
-            ('create_advert_post', 'Create advert post'),
-            ('create_regular_post', 'Create regular post'),
-            ('create_translated_post', 'Create translated post'),
+            ("create_generic_post", "Create generic post"),
+            ("create_archive_post", "Create archive post"),
+            ("create_advert_post", "Create advert post"),
+            ("create_regular_post", "Create regular post"),
+            ("create_translated_post", "Create translated post"),
         )
 
     @property
     def is_overdue(self):
-        if self.stage.slug in ('vault', 'published'):
+        if self.stage.slug in ("vault", "published"):
             return False
         return timezone.now() > self.finished_at
 
     @property
     def description_html(self):
         return render_md(self.description, render_lead=False)
 
     @property
     def wp_id(self):
-        return self.meta.get('wpid')
+        return self.meta.get("wpid")
 
     @property
     def lead(self) -> str:
         if not self.xmd:
-            return ''
+            return ""
 
-        paragraphs: List[str] = self.xmd.split('\n')
+        paragraphs: List[str] = self.xmd.split("\n")
         for paragraph in paragraphs:
             cleaned_paragraph = paragraph.strip()
             if not cleaned_paragraph:
                 continue
 
-            if cleaned_paragraph.startswith('$'):
+            if cleaned_paragraph.startswith("$"):
                 cleaned_paragraph = cleaned_paragraph[1:]
 
             cleaned_paragraph = cleaned_paragraph.strip()
             return cleaned_paragraph
 
-        return ''
+        return ""
 
     def build_xmd_blob(self, prepared_xmd: str) -> str:
         """Attaches CSS to XMD for remote CMS
 
-            >>> self.css ='foo'
-            'foo'
+        >>> self.css ='foo'
+        'foo'
 
-            >>> xmd = 'bar'
-            'bar'
+        >>> xmd = 'bar'
+        'bar'
 
-            >>> self.build_xmd_blob(self.xmd)
-            %style type=text/css
-            foo
-            %style
-            bar
+        >>> self.build_xmd_blob(self.xmd)
+        %style type=text/css
+        foo
+        %style
+        bar
         """
-        OPENING_STYLE_TAG = '%style type=text/css'
-        CLOSING_STYLE_TAG = '%style'
+        OPENING_STYLE_TAG = "%style type=text/css"
+        CLOSING_STYLE_TAG = "%style"
 
         if not prepared_xmd:
             return prepared_xmd
 
         if not self.css:
             return prepared_xmd
 
-        return '{}\n{}\n{}\n{}'.format(
-            OPENING_STYLE_TAG,
-            self.css,
-            CLOSING_STYLE_TAG,
-            prepared_xmd
+        return "{}\n{}\n{}\n{}".format(
+            OPENING_STYLE_TAG, self.css, CLOSING_STYLE_TAG, prepared_xmd
         )
 
     def upload(self):
         """Uploads post, metadata and attachments to remote CMS
 
         * self images uploaded to S3.
         * self content uploaded to WP with uploaded S3 images urls
 
         This method is long-running, can cause time-outs
         and should be run ONLY in async tasks with post lock.
 
             with Lock():
                 post.upload()
         """
-        logger.debug('Staring Post.upload')
+        logger.debug("Staring Post.upload")
         if not self.wp_id:
-            logger.warning('No wp_id, exiting')
+            logger.warning("No wp_id, exiting")
             return
 
         for image in self.images:
             image.upload_to_storage()
-        logger.debug('Uploaded images')
+        logger.debug("Uploaded images")
 
         # Upload to external DB
         prepared_xmd = replace_images_paths(
             xmd=self.xmd,
             attachments=self.images,
             mapper=s3_image_mapper,
         )
-        logger.debug('Replaced images paths')
+        logger.debug("Replaced images paths")
 
         upload_kwargs: tp.Dict[str, str] = {
-            'xmd': prepared_xmd,
-            'title': str(self),
-            'css': self.css,
+            "xmd": prepared_xmd,
+            "title": str(self),
+            "css": self.css,
         }
-        logger.debug('Prepared upload kwargs')
+        logger.debug("Prepared upload kwargs")
 
         if self.published_at and self.features == self.POST_FEATURES_ARCHIVE:
-            logger.debug('Running on archived post. Adding issues datetimes as publication dates')
-            post_date_gmt: str = self.published_at.strftime(WP_DATE_FORMAT_STRING)
-            post_date: str = self.published_at.astimezone().strftime(WP_DATE_FORMAT_STRING)
-
-            upload_kwargs['post_date_gmt'] = post_date_gmt
-            upload_kwargs['post_date'] = post_date
-            logger.debug('Added publication dates')
+            logger.debug(
+                "Running on archived post. Adding issues datetimes as publication dates"
+            )
+            post_date_gmt: str = self.published_at.strftime(
+                WP_DATE_FORMAT_STRING
+            )
+            post_date: str = self.published_at.astimezone().strftime(
+                WP_DATE_FORMAT_STRING
+            )
+
+            upload_kwargs["post_date_gmt"] = post_date_gmt
+            upload_kwargs["post_date"] = post_date
+            logger.debug("Added publication dates")
 
-        logger.debug('Ready to run upload to WP')
+        logger.debug("Ready to run upload to WP")
         update_ext_db_xmd(self.wp_id, **upload_kwargs)
 
     def render_xmd(self):
         if not self.has_text:
             return
 
         prepared_xmd: str = replace_images_paths(
             self.xmd, self.images, mapper=plan_image_mapper
         )
         self.html = _render_with_external_parser(
-            self.id, prepared_xmd, paywall_tag_html=Post.PAYWALL_NOTICE_RENDERED
+            self.id,
+            prepared_xmd,
+            paywall_tag_html=Post.PAYWALL_NOTICE_RENDERED,
         )
 
         if not self.html:
             self.html = render_md(self.xmd, attachments=self.images)
 
         if Post.PAYWALL_NOTICE_HEAD in self.html:
             self.is_paywalled = True
@@ -648,43 +711,40 @@
 
 class Attachment(AbstractBase):
     TYPE_IMAGE = 0
     TYPE_PDF = 1
     TYPE_FILE = 2
     TYPE_FEATURED_IMAGE = 3
     TYPE_CHOICES = (
-        (TYPE_IMAGE, 'Image'),
-        (TYPE_PDF, 'PDF'),
-        (TYPE_FILE, 'File'),
-        (TYPE_FEATURED_IMAGE, 'Featured image'),
+        (TYPE_IMAGE, "Image"),
+        (TYPE_PDF, "PDF"),
+        (TYPE_FILE, "File"),
+        (TYPE_FEATURED_IMAGE, "Featured image"),
     )
     type = models.SmallIntegerField(choices=TYPE_CHOICES, default=TYPE_IMAGE)
 
-    original_filename = models.CharField(null=False, blank=False, max_length=255)
-    file = models.FileField(upload_to='attachments/%Y/%m/%d/', max_length=2048)
+    original_filename = models.CharField(
+        null=False, blank=False, max_length=255
+    )
+    file = models.FileField(upload_to="attachments/%Y/%m/%d/", max_length=2048)
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     post = models.ForeignKey(Post, on_delete=models.CASCADE)
     meta = JSONField(default=dict)
 
     @property
     def s3_full_url(self):
-        return '{}/{}'.format(S3_STATIC_BASE_PATH, self.build_s3_object_path())
+        return "{}/{}".format(S3_STATIC_BASE_PATH, self.build_s3_object_path())
 
     def build_s3_object_path(self) -> str:
-        """Returns S3 object key path for upload with trailing slash
-        """
+        """Returns S3 object key path for upload with trailing slash"""
         dirname = os.path.dirname(self.file.name)
         basename = os.path.basename(self.file.name)
         hashed_dirname = hashlib.md5(dirname.encode()).hexdigest()
 
-        return 'images/{}/{}/{}'.format(
-            hashed_dirname,
-            self.id,
-            basename
-        )
+        return "images/{}/{}/{}".format(hashed_dirname, self.id, basename)
 
     def _guess_self_mimetype(self) -> tp.Optional[str]:
         try:
             return mimetypes.guess_type(self.file.path, strict=False)[0]
         except ValueError as exc:
             return None
 
@@ -692,94 +752,101 @@
         with S3Client() as (s3, S3_BUCKET_NAME):
             object_path = self.build_s3_object_path()
             try:
                 s3_object = s3.Object(S3_BUCKET_NAME, object_path)
                 s3_object.upload_file(
                     self.file.path,
                     ExtraArgs={
-                        'ACL': 'public-read',
-                        'ContentType': self._guess_self_mimetype()
-                    })
+                        "ACL": "public-read",
+                        "ContentType": self._guess_self_mimetype(),
+                    },
+                )
             except ClientError as e:
                 logging.error(e)
                 return False
             return True
 
-    def upload_to_storage(self, storage_type: StorageType = StorageType.S3) -> None:
+    def upload_to_storage(
+        self, storage_type: StorageType = StorageType.S3
+    ) -> None:
         if storage_type == StorageType.S3:
             self._upload_to_s3()
 
 
 class Comment(AbstractBase):
     SYSTEM_ACTION_SET_STAGE = 5
     SYSTEM_ACTION_UPDATE = 10
     SYSTEM_ACTION_CHANGE_META = 15
     SYSTEM_ACTION_CHOICES = (
-        (SYSTEM_ACTION_SET_STAGE, 'Set stage'),
-        (SYSTEM_ACTION_UPDATE, 'Update'),
-        (SYSTEM_ACTION_CHANGE_META, 'Change meta'),
+        (SYSTEM_ACTION_SET_STAGE, "Set stage"),
+        (SYSTEM_ACTION_UPDATE, "Update"),
+        (SYSTEM_ACTION_CHANGE_META, "Change meta"),
     )
 
     TYPE_SYSTEM = 5
     TYPE_PRIVATE = 10
     TYPE_PUBLIC = 15
     TYPE_CHOICES = (
-        (TYPE_SYSTEM, 'system'),
-        (TYPE_PRIVATE, 'private'),
-        (TYPE_PUBLIC, 'public'),
+        (TYPE_SYSTEM, "system"),
+        (TYPE_PRIVATE, "private"),
+        (TYPE_PUBLIC, "public"),
     )
     text = models.TextField(blank=True)
     type = models.SmallIntegerField(choices=TYPE_CHOICES, default=TYPE_PRIVATE)
     user = models.ForeignKey(User, on_delete=models.CASCADE)
 
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
     object_id = models.PositiveIntegerField()
-    commentable = GenericForeignKey('content_type', 'object_id')
+    commentable = GenericForeignKey("content_type", "object_id")
     meta = JSONField(default=dict)
 
     def __str__(self):
-        return '%s, %s:%s...' % (self.user_id, self.type, self.text[0:50])
+        return "%s, %s:%s..." % (self.user_id, self.type, self.text[0:50])
 
     @property
     def html(self):
         return render_md(self.text, render_lead=False)
 
     @property
     def changelog(self):
         try:
-            md = '\n'.join(self.meta['comment']['changelog'])
+            md = "\n".join(self.meta["comment"]["changelog"])
         except Exception:
-            md = ''
+            md = ""
 
         return render_md(md, render_lead=False)
 
 
 class Vote(AbstractBase):
     SCORE_0 = 0
     SCORE_25 = 25
     SCORE_50 = 50
     SCORE_75 = 75
     SCORE_100 = 100
     SCORE_CHOICES = (
-        (SCORE_0, 'Против таких статей в «Хакере»'),
-        (SCORE_25, 'Не верю, что выйдет хорошо'),
-        (SCORE_50, 'Тема нормальная, но не для меня'),
-        (SCORE_75, 'Почитал бы, встретив в журнале'),
-        (SCORE_100, 'Ради таких статей мог бы подписаться'),
+        (SCORE_0, "Против таких статей в «Хакере»"),
+        (SCORE_25, "Не верю, что выйдет хорошо"),
+        (SCORE_50, "Тема нормальная, но не для меня"),
+        (SCORE_75, "Почитал бы, встретив в журнале"),
+        (SCORE_100, "Ради таких статей мог бы подписаться"),
     )
     score = models.SmallIntegerField(choices=SCORE_CHOICES, default=SCORE_50)
     user = models.ForeignKey(User, on_delete=models.CASCADE)
-    idea = models.ForeignKey(Idea, on_delete=models.CASCADE, related_name='votes')
+    idea = models.ForeignKey(
+        Idea, on_delete=models.CASCADE, related_name="votes"
+    )
 
     @property
     def score_humanized(self):
         return self.__class__.SCORE_CHOICES
 
 
-def users_with_perm(perm_name: str, include_superuser: bool = True) -> List[User]:
+def users_with_perm(
+    perm_name: str, include_superuser: bool = True
+) -> List[User]:
     """Get all users by full permission name
 
     :param perm_name: permission name without app name
     :param include_superuser:
     :return:
     """
     return User.objects.filter(
@@ -797,43 +864,41 @@
 
 @receiver(post_save, sender=User)
 def save_user_profile(sender, instance, **kwargs):
     instance.profile.save()
 
 
 def _render_with_external_parser(
-        id: int, xmd: str, paywall_tag_html: str = Post.PAYWALL_NOTICE_RENDERED
+    id: int, xmd: str, paywall_tag_html: str = Post.PAYWALL_NOTICE_RENDERED
 ) -> tp.Optional[str]:
-    FAILBACK_SYNTAX_LANG = 'cpp'
+    FAILBACK_SYNTAX_LANG = "cpp"
 
     if not xmd:
         return None
 
     if not config.EXTERNAL_PARSER_URL:
         return None
 
     try:
         request_payload: tp.Dict[str, str] = {
-            'id': id,
-            'md': xmd,
-            'lang': FAILBACK_SYNTAX_LANG,
-            'xakepcut': paywall_tag_html,
+            "id": id,
+            "md": xmd,
+            "lang": FAILBACK_SYNTAX_LANG,
+            "xakepcut": paywall_tag_html,
         }
         request_headers: tp.Dict[str, str] = {  # unusued
-            'content-type': 'application/x-www-form-urlencoded; charset=utf-8'
+            "content-type": "application/x-www-form-urlencoded; charset=utf-8"
         }
         request_query_params: tp.Dict[str, str] = {
-            'x': config.EXTERNAL_PARSER_TOKEN or ''
+            "x": config.EXTERNAL_PARSER_TOKEN or ""
         }
 
         query_string = urllib.parse.urlencode(request_query_params)
-        prepared_url = f'{config.EXTERNAL_PARSER_URL}?{query_string}'
-        response = requests.post(
-            prepared_url, data=request_payload
-        )
+        prepared_url = f"{config.EXTERNAL_PARSER_URL}?{query_string}"
+        response = requests.post(prepared_url, data=request_payload)
         return response.text
 
     except Exception as exc:
         # TODO: add logger, no need to handle
         return None
 
 
@@ -845,11 +910,13 @@
     if not instance._state.adding:
         if instance.features == Post.POST_FEATURES_ARCHIVE:
             if instance.issues.count():
                 target_issue: Issue = instance.issues.first()
 
                 # Convert date to datetime
                 published_date: datetime.date = target_issue.published_at
-                published_datetime: datetime.datetime = datetime.datetime.combine(
-                    published_date, datetime.datetime.min.time()
+                published_datetime: datetime.datetime = (
+                    datetime.datetime.combine(
+                        published_date, datetime.datetime.min.time()
+                    )
                 )
                 instance.published_at = published_datetime
```

### Comparing `magplan-3.1.0/src/magplan/tasks/send_idea_comment_notification.py` & `magplan-3.1.1/src/magplan/tasks/send_idea_comment_notification.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 from magplan.conf import settings as config
 from django.contrib.contenttypes.models import ContentType
 from django.core.mail import EmailMultiAlternatives
 from django.template.loader import render_to_string
 
 from celery import shared_task
 from magplan.models import Comment, User
-from magplan.tasks.utils import _can_recieve_notification, _get_whitelisted_recipients
+from magplan.tasks.utils import (
+    _can_recieve_notification,
+    _get_whitelisted_recipients,
+)
 
-RECIEVE_NOTIFICATIONS_PERMISSION = 'main.recieve_idea_email_updates'
-NOTIFICATION_LEVEL_PREFERENCE = 'idea_comment_notification_level'
+RECIEVE_NOTIFICATIONS_PERMISSION = "main.recieve_idea_email_updates"
+NOTIFICATION_LEVEL_PREFERENCE = "idea_comment_notification_level"
 
 
 def _get_involved_users(comment: Comment) -> set:
     """
 
     :param comment:
     :return: Ø
@@ -64,39 +67,50 @@
     :return: Final set of actual recipients
     """
     recipients = set()
 
     involved_users = _get_involved_users(comment)
     recipients.update(involved_users)
 
-    whitelisted_recipients = _get_whitelisted_recipients(NOTIFICATION_LEVEL_PREFERENCE)
+    whitelisted_recipients = _get_whitelisted_recipients(
+        NOTIFICATION_LEVEL_PREFERENCE
+    )
     recipients.update(whitelisted_recipients)
 
     # Remove users, who cannot receive notifications
     # due to their permissions, comment ownership or settings
     recipients = {
         recipient
         for recipient in recipients
         if _can_recieve_notification(
-            recipient, comment, RECIEVE_NOTIFICATIONS_PERMISSION, NOTIFICATION_LEVEL_PREFERENCE
+            recipient,
+            comment,
+            RECIEVE_NOTIFICATIONS_PERMISSION,
+            NOTIFICATION_LEVEL_PREFERENCE,
         )
     }
 
     return recipients
 
 
 def _send_email(comment, recipients):
     subject = f"Комментарий к идее «{comment.commentable}» от {comment.user}"
     html_content = render_to_string(
         "email/new_comment.html",
-        {"comment": comment, "commentable_type": 'idea', "APP_URL": os.environ.get('APP_URL', None)},
+        {
+            "comment": comment,
+            "commentable_type": "idea",
+            "APP_URL": os.environ.get("APP_URL", None),
+        },
     )
     text_content = html2text.html2text(html_content)
-    msg = EmailMultiAlternatives(subject, text_content, config.PLAN_EMAIL_FROM, recipients)
-    msg.attach_alternative(html_content, 'text/html')
+    msg = EmailMultiAlternatives(
+        subject, text_content, config.PLAN_EMAIL_FROM, recipients
+    )
+    msg.attach_alternative(html_content, "text/html")
     msg.send()
 
 
 @shared_task
 def send_idea_comment_notification(comment_id: int) -> None:
     """Send email notification for idea comment
 
@@ -105,15 +119,15 @@
     - idea author (user)
     - everyone, who previously commented comment idea
 
     But only, if users have appropriate permission
     permission and not comment author.
     """
     logger = logging.getLogger()
-    logger.info('Sending notifications for comment #%s', comment_id)
+    logger.info("Sending notifications for comment #%s", comment_id)
 
     # Task will fail if comment is not found
     comment = Comment.objects.get(id=comment_id)
 
     recipients = _get_recipients(comment)
     if not recipients:
         return
```

### Comparing `magplan-3.1.0/src/magplan/tasks/send_post_comment_notification.py` & `magplan-3.1.1/src/magplan/tasks/send_post_comment_notification.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
 from django.core.mail import EmailMultiAlternatives
 from django.template.loader import render_to_string
 
 from magplan.conf import settings as config
 from magplan.models import Comment
-from magplan.tasks.utils import _can_recieve_notification, _get_whitelisted_recipients
+from magplan.tasks.utils import (
+    _can_recieve_notification,
+    _get_whitelisted_recipients,
+)
 
-RECIEVE_NOTIFICATIONS_PERMISSION = 'main.recieve_post_email_updates'
-NOTIFICATION_LEVEL_PREFERENCE = 'post_comment_notification_level'
+RECIEVE_NOTIFICATIONS_PERMISSION = "main.recieve_post_email_updates"
+NOTIFICATION_LEVEL_PREFERENCE = "post_comment_notification_level"
 
 
 def _get_involved_users(comment: Comment) -> set:
     """Return all users, who involved in working
     on current post
 
     :param comment: Comment for post, for which we count involved users
@@ -39,15 +42,17 @@
 
     # Add post authors and editors
     users.add(post.editor)
     users.update([author for author in post.authors.all()])
 
     # Add all previous commenters in the tread
     previous_comments = Comment.objects.filter(
-        content_type=ContentType.objects.get_for_model(post), object_id=post.id, type=Comment.TYPE_PRIVATE
+        content_type=ContentType.objects.get_for_model(post),
+        object_id=post.id,
+        type=Comment.TYPE_PRIVATE,
     ).exclude(id=comment.id)
 
     users.update([pc.user for pc in previous_comments])
 
     return users
 
 
@@ -68,39 +73,52 @@
     :return: Final set of actual recipients
     """
     recipients = set()
 
     involved_users = _get_involved_users(comment)
     recipients.update(involved_users)
 
-    whitelisted_recipients = _get_whitelisted_recipients(NOTIFICATION_LEVEL_PREFERENCE)
+    whitelisted_recipients = _get_whitelisted_recipients(
+        NOTIFICATION_LEVEL_PREFERENCE
+    )
     recipients.update(whitelisted_recipients)
 
     # Remove users, who cannot receive notifications
     # due to their permissions, comment ownership or settings
     recipients = {
         recipient
         for recipient in recipients
         if _can_recieve_notification(
-            recipient, comment, RECIEVE_NOTIFICATIONS_PERMISSION, NOTIFICATION_LEVEL_PREFERENCE
+            recipient,
+            comment,
+            RECIEVE_NOTIFICATIONS_PERMISSION,
+            NOTIFICATION_LEVEL_PREFERENCE,
         )
     }
 
     return recipients
 
 
 def _send_email(comment, recipients):
     subject = f"Комментарий к посту «{comment.commentable}» от {comment.user}"
-    commentable_type = "post" if comment.commentable.__class__.__name__ == "Post" else "idea"
+    commentable_type = (
+        "post" if comment.commentable.__class__.__name__ == "Post" else "idea"
+    )
     html_content = render_to_string(
         "email/new_comment.html",
-        {"comment": comment, "commentable_type": commentable_type, "APP_URL": os.environ.get("APP_URL", None)},
+        {
+            "comment": comment,
+            "commentable_type": commentable_type,
+            "APP_URL": os.environ.get("APP_URL", None),
+        },
     )
     text_content = html2text.html2text(html_content)
-    msg = EmailMultiAlternatives(subject, text_content, config.PLAN_EMAIL_FROM, recipients)
+    msg = EmailMultiAlternatives(
+        subject, text_content, config.PLAN_EMAIL_FROM, recipients
+    )
     msg.attach_alternative(html_content, "text/html")
     msg.send()
 
 
 @shared_task
 def send_post_comment_notification(comment_id: int) -> None:
     """Send email notification for post comment
@@ -111,15 +129,15 @@
     - comment post authors and editor
     - everyone, who previously commented comment post
 
     But only, if users have recieve_post_email_updates
     permission and not comment author.
     """
     logger = logging.getLogger()
-    logger.info('Sending notifications for comment #%s', comment_id)
+    logger.info("Sending notifications for comment #%s", comment_id)
 
     # Task will fail if comment is not found
     comment = Comment.objects.get(id=comment_id)
 
     recipients = _get_recipients(comment)
 
     if not recipients:
```

### Comparing `magplan-3.1.0/src/magplan/tasks/upload_post_to_wp.py` & `magplan-3.1.1/src/magplan/tasks/upload_post_to_wp.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
 from magplan.models import Post
 from magplan.integrations.posts import Lock
 
 
 logger = logging.getLogger()
 
+
 @shared_task
 def upload_post_to_wp(post_id: int) -> None:
-    logger.info('Starting task upload_post_to_wp...')
+    logger.info("Starting task upload_post_to_wp...")
 
     post = Post.objects.filter(id=post_id).first()
     if post is None:
         return
 
     with Lock(post):
-        logger.info('Lock for post %s acquired' % post.id)
+        logger.info("Lock for post %s acquired" % post.id)
         post.upload()
```

### Comparing `magplan-3.1.0/src/magplan/tasks/utils.py` & `magplan-3.1.1/src/magplan/tasks/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,46 +12,49 @@
 
     NB: relies on default setting == 'related'!
 
     :return: Set of users, who we should send
              every comment
     """
 
-    preferences = UserPreferenceModel.objects.prefetch_related('instance').filter(
-        section='magplan', name=pref_name, raw_value='all'
-    )
+    preferences = UserPreferenceModel.objects.prefetch_related(
+        "instance"
+    ).filter(section="magplan", name=pref_name, raw_value="all")
 
     return {p.instance for p in preferences}
 
 
 def _can_recieve_notification(
-        user: User, comment: Comment, perm_name: str, pref_name: str
+    user: User, comment: Comment, perm_name: str, pref_name: str
 ) -> bool:
     logger = logging.getLogger()
-    logger.debug('Checking permissions for recipient %s...' % user.email)
+    logger.debug("Checking permissions for recipient %s..." % user.email)
 
     if not user.has_perm(perm_name):
         logger.debug(
-            'Recipient %s decliened as it has no permission to receive post updates.'
+            "Recipient %s decliened as it has no permission to receive post updates."
             % user.email
         )
         return False
 
     if user == comment.user:
-        logger.debug('Recipient %s decliened as it\'s comment author' % user.email)
+        logger.debug(
+            "Recipient %s decliened as it's comment author" % user.email
+        )
         return False
 
     if config.SYSTEM_USER_ID and user.id == config.SYSTEM_USER_ID:
-        logger.debug('Recipient %s decliened as it\'s system user' % user.email)
+        logger.debug("Recipient %s decliened as it's system user" % user.email)
         return False
 
     # Disable notification for restricted notification users.
     # This util function is used only in magplan app
     # so it's better to hardcode section name
     # for better re-usabillty
-    if user.preferences['magplan__' + pref_name] == 'none':
+    if user.preferences["magplan__" + pref_name] == "none":
         logger.debug(
-            'Recipient %s decliened as it has turned notifications off' % user.email
+            "Recipient %s decliened as it has turned notifications off"
+            % user.email
         )
         return False
 
     return True
```

### Comparing `magplan-3.1.0/src/magplan/templates/_test_issues.py` & `magplan-3.1.1/src/magplan/templates/_test_issues.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 from django.test import Client, TestCase
-from plan.tests import _User, _Sections, _Section, _Stages, _Post, _Postype, _Issue
+from plan.tests import (
+    _User,
+    _Sections,
+    _Section,
+    _Stages,
+    _Post,
+    _Postype,
+    _Issue,
+)
 from django.urls import reverse
 from datetime import datetime
 from main.models import Issue
 
 
 class TestCreate(TestCase):
     @classmethod
     def setUpTestData(cls):
         cls.user = _User()
 
     def setUp(self):
-        self.ROUTE_NAME = 'issues_create'
+        self.ROUTE_NAME = "issues_create"
         self.client = Client()
 
     def test_redirect_to_login_if_not_authenticated(self):
         response = self.client.get(reverse(self.ROUTE_NAME))
-        self.assertRedirects(response, '%s?next=/admin/issues/new/' % reverse('login'))
+        self.assertRedirects(
+            response, "%s?next=/admin/issues/new/" % reverse("login")
+        )
 
     def test_should_render_issue_form(self):
         self.client.force_login(user=self.user)
         response = self.client.get(reverse(self.ROUTE_NAME))
 
         self.assertEqual(response.status_code, 200)
-        self.assertTemplateUsed(response, 'magplan/issues/_form.html')
+        self.assertTemplateUsed(response, "magplan/issues/_form.html")
 
     def test_issue_should_be_created(self):
         self.client.force_login(user=self.user)
 
         published_at = datetime.now()
-        response = self.client.post(reverse(self.ROUTE_NAME), {
-            'title': 'title',
-            'description': 'description',
-            'number': '123',
-            'published_at': published_at.strftime('%d.%m.%Y'),
-        })
+        response = self.client.post(
+            reverse(self.ROUTE_NAME),
+            {
+                "title": "title",
+                "description": "description",
+                "number": "123",
+                "published_at": published_at.strftime("%d.%m.%Y"),
+            },
+        )
 
-        self.assertRedirects(response, reverse('issues_index'))
+        self.assertRedirects(response, reverse("issues_index"))
         self.assertEqual(Issue.objects.filter(number=123), 1)
```

### Comparing `magplan-3.1.0/src/magplan/templates/email/_vote_from_email.html` & `magplan-3.1.1/src/magplan/templates/email/_vote_from_email.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/email/idea_approved.html` & `magplan-3.1.1/src/magplan/templates/email/idea_approved.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/email/new_comment.html` & `magplan-3.1.1/src/magplan/templates/email/new_comment.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/layout_plan.html` & `magplan-3.1.1/src/magplan/templates/layout_plan.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/articles/advert.html` & `magplan-3.1.1/src/magplan/templates/magplan/articles/advert.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/articles/archived.html` & `magplan-3.1.1/src/magplan/templates/magplan/articles/archived.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/articles/default.html` & `magplan-3.1.1/src/magplan/templates/magplan/articles/default.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/articles/index.html` & `magplan-3.1.1/src/magplan/templates/magplan/articles/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/articles/whitelisted.html` & `magplan-3.1.1/src/magplan/templates/magplan/articles/whitelisted.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/authors/_form.html` & `magplan-3.1.1/src/magplan/templates/magplan/authors/_form.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/authors/edit.html` & `magplan-3.1.1/src/magplan/templates/magplan/authors/edit.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/authors/index.html` & `magplan-3.1.1/src/magplan/templates/magplan/authors/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/authors/show.html` & `magplan-3.1.1/src/magplan/templates/magplan/authors/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/ideas/_approve_ideas.html` & `magplan-3.1.1/src/magplan/templates/magplan/ideas/_approve_ideas.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/ideas/_authors_list.html` & `magplan-3.1.1/src/magplan/templates/magplan/ideas/_authors_list.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/ideas/_form_base.html` & `magplan-3.1.1/src/magplan/templates/magplan/ideas/_form_base.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/ideas/_vote.html` & `magplan-3.1.1/src/magplan/templates/magplan/ideas/_vote.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/ideas/_voting_results.html` & `magplan-3.1.1/src/magplan/templates/magplan/ideas/_voting_results.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/ideas/index.html` & `magplan-3.1.1/src/magplan/templates/magplan/ideas/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/ideas/show.html` & `magplan-3.1.1/src/magplan/templates/magplan/ideas/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/index/index.html` & `magplan-3.1.1/src/magplan/templates/magplan/index/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/issues/_form.html` & `magplan-3.1.1/src/magplan/templates/magplan/issues/_form.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/issues/index.html` & `magplan-3.1.1/src/magplan/templates/magplan/issues/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/issues/show.html` & `magplan-3.1.1/src/magplan/templates/magplan/issues/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/partials/_navbar.sites.html` & `magplan-3.1.1/src/magplan/templates/magplan/partials/_navbar.sites.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/partials/_navbar_header_links.html` & `magplan-3.1.1/src/magplan/templates/magplan/partials/_navbar_header_links.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/partials/comments.html` & `magplan-3.1.1/src/magplan/templates/magplan/partials/comments.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/partials/navbar.html` & `magplan-3.1.1/src/magplan/templates/magplan/partials/navbar.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/partials/posts_table.html` & `magplan-3.1.1/src/magplan/templates/magplan/partials/posts_table.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_admin_set_stage.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_admin_set_stage.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_attachments.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_attachments.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_field_col.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_field_col.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_form_base.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_form_base.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_form_meta.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_form_meta.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_progress.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_progress.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_schedule.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_schedule.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/_stages.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/_stages.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/edit.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/edit.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/posts/show.html` & `magplan-3.1.1/src/magplan/templates/magplan/posts/show.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/sections/index.html` & `magplan-3.1.1/src/magplan/templates/magplan/sections/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templates/magplan/stages/index.html` & `magplan-3.1.1/src/magplan/templates/magplan/stages/index.html`

 * *Files identical despite different names*

### Comparing `magplan-3.1.0/src/magplan/templatetags/filters.py` & `magplan-3.1.1/src/magplan/templatetags/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,51 +13,51 @@
 
 register = template.Library()
 
 MAX_VOTE_OPTIONS_NUMBER = len(Vote.SCORE_CHOICES)
 VOTE_SCORE_STEP = 100 // (MAX_VOTE_OPTIONS_NUMBER - 1)
 FAILBACK_VOTE_INDEX = 2
 CSS_COLORS = (
-    'danger',
-    'warning',
-    'light',
-    'info',
-    'success',
+    "danger",
+    "warning",
+    "light",
+    "info",
+    "success",
 )
 
 EMOJI_SCORES = (
-    '🤮',
-    '🤨',
-    '😐',
-    '😏',
-    '😍',
+    "🤮",
+    "🤨",
+    "😐",
+    "😏",
+    "😍",
 )
 
 
-@register.filter(name='voted')
+@register.filter(name="voted")
 def voted(value, user):
     return value.voted(user)
 
 
-@register.filter(name='humanize_score_index')
+@register.filter(name="humanize_score_index")
 def humanize_score_index(index) -> str:
     if not isinstance(index, int):
         index = safe_cast(index, int, -1)
 
     if index == -1:  # error cast
         return Vote.SCORE_CHOICES[FAILBACK_VOTE_INDEX][1]
 
     score = index * VOTE_SCORE_STEP
 
     # Provide untrusted data
     # Underlying function will validate data
     return humanize_score(score)
 
 
-@register.filter(name='humanize_score')
+@register.filter(name="humanize_score")
 def humanize_score(value) -> str:
     if not isinstance(value, int):
         value = safe_cast(value, int, -1)
 
     if value == -1:  # error cast
         return Vote.SCORE_CHOICES[FAILBACK_VOTE_INDEX][1]
 
@@ -68,26 +68,23 @@
         return Vote.SCORE_CHOICES[FAILBACK_VOTE_INDEX][1]
 
     choice_index = value // VOTE_SCORE_STEP
 
     return Vote.SCORE_CHOICES[choice_index][1]
 
 
-@register.filter(name='times')
+@register.filter(name="times")
 def times(number):
     return range(number)
 
 
-@register.filter(name='trim_filename')
+@register.filter(name="trim_filename")
 def trim_filename(filename):
     if len(filename) > 30:
-        return '%s...%s' % (
-            filename[:10],
-            filename[-20:]
-        )
+        return "%s...%s" % (filename[:10], filename[-20:])
     return filename
 
 
 @register.filter
 def divide(value, arg):
     try:
         return int(value) / int(arg)
@@ -104,53 +101,61 @@
     def render(self, context):
         try:
             value = template.Variable(self.var_value).resolve(context)
         except template.VariableDoesNotExist:
             value = ""
         context[self.var_name] = value
 
-        return u""
+        return ""
 
 
-@register.tag(name='set')
+@register.tag(name="set")
 def set_var(parser, token):
     """
     {% set some_var = '123' %}
     """
     parts = token.split_contents()
     if len(parts) < 4:
         raise template.TemplateSyntaxError(
-            "'set' tag must be of the form: {% set <var_name> = <var_value> %}")
+            "'set' tag must be of the form: {% set <var_name> = <var_value> %}"
+        )
 
     return SetVarNode(parts[1], parts[3])
 
 
 @register.filter
 def can_be_moved_to_stage_by(post, user: SimpleLazyObject):
-    return (post.stage.assignee and post.stage.assignee == user.user) or \
-           (not post.stage.assignee and post.editor == user.user)
+    return (post.stage.assignee and post.stage.assignee == user.user) or (
+        not post.stage.assignee and post.editor == user.user
+    )
 
 
 @register.filter
 def sub(value, arg):
     return value - arg
 
 
 @register.filter
 def url_for_post_comments(post):
-    return reverse(posts.comments, kwargs={
-        'post_id': post.id,
-    })
+    return reverse(
+        posts.comments,
+        kwargs={
+            "post_id": post.id,
+        },
+    )
 
 
 @register.filter
 def url_for_idea_comments(idea):
-    return reverse(ideas.comments, kwargs={
-        'idea_id': idea.id,
-    })
+    return reverse(
+        ideas.comments,
+        kwargs={
+            "idea_id": idea.id,
+        },
+    )
 
 
 @register.filter
 def is_overdue(date):
     return date > datetime.datetime.now()
 
 
@@ -187,58 +192,58 @@
     datetime_obj|f = 0 else
     """
     # Convert 'datetime' => 'date' class for easier comparison
     date = datetime_obj.date()
     today = datetime.datetime.now().date()
 
     if date < today:
-        return 'past'
+        return "past"
     elif date == today:
-        return 'today'
+        return "today"
     else:
-        return ''
+        return ""
 
 
 @register.filter
 def get_item(dictionary, key):
     return dictionary[key]
 
 
 numeric_test = re.compile("^\d+$")
 
 
-@register.filter(name='get_attr')
+@register.filter(name="get_attr")
 def get_attr(value, arg):
     """Gets an attribute of an object dynamically from a string name"""
 
     if hasattr(value, str(arg)):
         return getattr(value, arg)
-    elif hasattr(value, 'has_key') and value.has_key(arg):
+    elif hasattr(value, "has_key") and value.has_key(arg):
         return value[arg]
     elif numeric_test.match(str(arg)) and len(value) > int(arg):
         return value[int(arg)]
     else:
         return settings.TEMPLATE_STRING_IF_INVALID
 
 
-@register.filter(name='score_css_color_by_index')
+@register.filter(name="score_css_color_by_index")
 def score_css_color_by_index(index):
     if not isinstance(index, int):
         index = safe_cast(index, int, -1)
 
     if index == -1:  # error cast
         return CSS_COLORS[FAILBACK_VOTE_INDEX]
 
     if not (0 <= index <= (MAX_VOTE_OPTIONS_NUMBER - 1)):
         return CSS_COLORS[FAILBACK_VOTE_INDEX]
 
     return CSS_COLORS[index]
 
 
-@register.filter(name='emoji_sign_by_index')
+@register.filter(name="emoji_sign_by_index")
 def emoji_sign_by_index(index):
     if not isinstance(index, int):
         index = safe_cast(index, int, -1)
 
     if index == -1:  # error cast
         return EMOJI_SCORES[FAILBACK_VOTE_INDEX]
```

### Comparing `magplan-3.1.0/src/magplan/urls.py` & `magplan-3.1.1/src/magplan/urls.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,52 +11,69 @@
     issues,
     posts,
     api,
     preferences,
 )
 
 urlpatterns = [
-
-    path('sections/', sections.index, name='sections_index'),
-    path('stages/', stages.index, name='stages_index'),
-
-    path('ideas/<int:idea_id>/comments/', ideas.comments, name='ideas_comments'),
-    path('ideas/<int:idea_id>/approve/', ideas.approve, name='ideas_approve'),
-    path('ideas/<int:idea_id>/vote/', ideas.vote, name='ideas_vote'),
-    path('ideas/<int:idea_id>/', ideas.show, name='ideas_show'),
-    path('ideas/', ideas.index, name='ideas_index'),
-
-    path('articles/search', articles.search, name='articles_search'),
-    path('articles/default', articles.default, name='articles_default'),
-    path('articles/archived', articles.archived, name='articles_archived'),
-    path('articles/advert', articles.advert, name='articles_advert'),
-    path('articles/whitelisted', articles.whitelisted, name='articles_whitelisted'),
-    path('articles/', articles.index, name='articles_index'),
-
-    path('issues/<int:issue_id>/', issues.show, name='issues_show'),
-    path('issues/new/', issues.create, name='issues_create'),
-    path('issues/', issues.index, name='issues_index'),
-
-    path('posts/<int:post_id>/attachments/delete/', posts.attachment_delete, name='posts_attachment_delete'),
-    path('posts/<int:post_id>/comments/', posts.comments, name='posts_comments'),
-    path('posts/<int:post_id>/set_stage/', posts.set_stage, name='posts_set_stage'),
-    path('posts/<int:post_id>/edit/', posts.edit, name='posts_edit'),
-    path('posts/<int:post_id>/edit_meta/', posts.edit_meta, name='posts_edit_meta'),
-    path('posts/<int:post_id>/download/', posts.download_content, name='posts_download_content'),
-    path('posts/<int:post_id>/send_to_wp/', posts.send_to_wp, name='posts_send_to_wp'),
-    path('posts/<int:post_id>/', posts.show, name='posts_show'),
-    path('posts', posts.create, name='posts_create'),
-
-    path('api/issues/search/', api.issues_search, name='api_issues_search'),
-    path('api/users/search/', api.authors_search, name='api_authors_search'),
-
-    path('authors/new/', authors.new, name='authors_new'),
-    path('authors/<int:user_id>/edit/', authors.edit, name='authors_edit'),
-    path('authors/<int:user_id>/', authors.show, name='authors_show'),
-    path('authors/', authors.index, name='authors_index'),
-
-    path('settings/', preferences.index, name='preferences_index'),
-
-
-
-    path('', index.index, name='index_index'),
+    path("sections/", sections.index, name="sections_index"),
+    path("stages/", stages.index, name="stages_index"),
+    path(
+        "ideas/<int:idea_id>/comments/", ideas.comments, name="ideas_comments"
+    ),
+    path("ideas/<int:idea_id>/approve/", ideas.approve, name="ideas_approve"),
+    path("ideas/<int:idea_id>/vote/", ideas.vote, name="ideas_vote"),
+    path("ideas/<int:idea_id>/", ideas.show, name="ideas_show"),
+    path("ideas/", ideas.index, name="ideas_index"),
+    path("articles/search", articles.search, name="articles_search"),
+    path("articles/default", articles.default, name="articles_default"),
+    path("articles/archived", articles.archived, name="articles_archived"),
+    path("articles/advert", articles.advert, name="articles_advert"),
+    path(
+        "articles/whitelisted",
+        articles.whitelisted,
+        name="articles_whitelisted",
+    ),
+    path("articles/", articles.index, name="articles_index"),
+    path("issues/<int:issue_id>/", issues.show, name="issues_show"),
+    path("issues/new/", issues.create, name="issues_create"),
+    path("issues/", issues.index, name="issues_index"),
+    path(
+        "posts/<int:post_id>/attachments/delete/",
+        posts.attachment_delete,
+        name="posts_attachment_delete",
+    ),
+    path(
+        "posts/<int:post_id>/comments/", posts.comments, name="posts_comments"
+    ),
+    path(
+        "posts/<int:post_id>/set_stage/",
+        posts.set_stage,
+        name="posts_set_stage",
+    ),
+    path("posts/<int:post_id>/edit/", posts.edit, name="posts_edit"),
+    path(
+        "posts/<int:post_id>/edit_meta/",
+        posts.edit_meta,
+        name="posts_edit_meta",
+    ),
+    path(
+        "posts/<int:post_id>/download/",
+        posts.download_content,
+        name="posts_download_content",
+    ),
+    path(
+        "posts/<int:post_id>/send_to_wp/",
+        posts.send_to_wp,
+        name="posts_send_to_wp",
+    ),
+    path("posts/<int:post_id>/", posts.show, name="posts_show"),
+    path("posts", posts.create, name="posts_create"),
+    path("api/issues/search/", api.issues_search, name="api_issues_search"),
+    path("api/users/search/", api.authors_search, name="api_authors_search"),
+    path("authors/new/", authors.new, name="authors_new"),
+    path("authors/<int:user_id>/edit/", authors.edit, name="authors_edit"),
+    path("authors/<int:user_id>/", authors.show, name="authors_show"),
+    path("authors/", authors.index, name="authors_index"),
+    path("settings/", preferences.index, name="preferences_index"),
+    path("", index.index, name="index_index"),
 ]
```

### Comparing `magplan-3.1.0/src/magplan/utils.py` & `magplan-3.1.1/src/magplan/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.conf import settings
 from django.contrib.sites.models import Site
 from django.http import HttpRequest
 
 
 def safe_cast(value: Any, to: Callable, on_error: Any = None) -> Any:
-    """"Safe casts value to type with provided casting constructor.
+    """ "Safe casts value to type with provided casting constructor.
 
     If cast falls for some reason, default on_error value is returned.*
 
     :param value: Source value to cast*
     :param to: Callable constructor, which can accept typed value*
     :param on_error: Value to return is cast falls: bad constructor, unacceptable source type*
      :return: casted value or fallback*
@@ -23,15 +23,15 @@
     return casted
 
 
 def get_current_site(request: HttpRequest, safe: bool = True) -> Site:
     """
     Returns selected on plan site from user settings
     """
-    current_site_id = request.user.preferences['magplan__current_site']  # noqa
+    current_site_id = request.user.preferences["magplan__current_site"]  # noqa
     if current_site_id:
         try:
             Site.objects.get(id=current_site_id)
         except Site.DoesNotExist:
             pass  # FIXME
 
     DEFAULT_SITE_ID: int = settings.SITE_ID
```

### Comparing `magplan-3.1.0/src/magplan/views/api.py` & `magplan-3.1.1/src/magplan/views/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 from django.http import JsonResponse
 
 from magplan.models import Issue, User
 
 
 @login_required
 def issues_search(request):
-    q = request.GET.get('q', None)
+    q = request.GET.get("q", None)
     issues = Issue.on_current_site.filter(number__exact=q)
     return JsonResponse(
-        [{'id': issue.id, 'text': issue.__str__()} for issue in issues]
-        , safe=False)
+        [{"id": issue.id, "text": issue.__str__()} for issue in issues],
+        safe=False,
+    )
 
 
 @login_required
 def authors_search(request):
-    q = request.GET.get('q', None)
+    q = request.GET.get("q", None)
 
     # FIXME: heavy request, should be optimized
     users = User.objects.filter(
-        Q(email__icontains=q) |
-        Q(meta__icontains=q) |
-        Q(profile__f_name__icontains=q) |
-        Q(profile__l_name__icontains=q) |
-        Q(profile__m_name__icontains=q)
+        Q(email__icontains=q)
+        | Q(meta__icontains=q)
+        | Q(profile__f_name__icontains=q)
+        | Q(profile__l_name__icontains=q)
+        | Q(profile__m_name__icontains=q)
     )
     return JsonResponse(
-        [{'id': user.id, 'text': user.__str__()} for user in users]
-        , safe=False)
+        [{"id": user.id, "text": user.__str__()} for user in users], safe=False
+    )
```

### Comparing `magplan-3.1.0/src/magplan/views/articles.py` & `magplan-3.1.1/src/magplan/views/articles.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,200 +4,235 @@
 from django.contrib.auth.decorators import login_required
 from django.db.models import Q, QuerySet
 from django.http import HttpRequest
 from django.shortcuts import render, redirect
 from django.urls import reverse
 from django.utils.timezone import now
 
-from magplan.forms import WhitelistedPostExtendedModelForm, AdPostExtendedModelForm, DefaultPostModelForm, \
-    ArchivedPostModelForm
+from magplan.forms import (
+    WhitelistedPostExtendedModelForm,
+    AdPostExtendedModelForm,
+    DefaultPostModelForm,
+    ArchivedPostModelForm,
+)
 from magplan.models import Post, Stage, User
 from magplan.utils import get_current_site
 
 
-def _get_filtered_posts_queryset(filter_: tp.Optional[str], current_user: User, queryset: QuerySet = None) -> QuerySet:
+def _get_filtered_posts_queryset(
+    filter_: tp.Optional[str], current_user: User, queryset: QuerySet = None
+) -> QuerySet:
     """
     Returns articles QuerySet, based on user request filters.
     """
 
     if queryset is None:
         queryset = Post.objects
-    posts = queryset \
-        .prefetch_related('section', 'stage', 'issues__magazine', 'editor__profile') \
-        .order_by('-updated_at')
+    posts = queryset.prefetch_related(
+        "section", "stage", "issues__magazine", "editor__profile"
+    ).order_by("-updated_at")
 
     # Get filtered queryset
-    if filter_ == 'self':
+    if filter_ == "self":
         posts = posts.filter(editor=current_user)
-    elif filter_ == 'overdue':
-        posts = posts \
-            .filter(finished_at__lte=datetime.datetime.now()) \
-            .exclude(stage__slug='vault') \
-            .exclude(stage__slug='published')
-    elif filter_ == 'vault':
-        posts = posts.filter(stage__slug='vault')
-    elif filter_ == 'all':
+    elif filter_ == "overdue":
+        posts = (
+            posts.filter(finished_at__lte=datetime.datetime.now())
+            .exclude(stage__slug="vault")
+            .exclude(stage__slug="published")
+        )
+    elif filter_ == "vault":
+        posts = posts.filter(stage__slug="vault")
+    elif filter_ == "all":
         # Don't apply any filters to get all posts
         pass
     else:
         # Render recent by default
         datetime_now = now()
         filter_kwargs = {
-            'updated_at__gte': datetime_now - datetime.timedelta(2 * 30),
-            'updated_at__lte': datetime_now,
+            "updated_at__gte": datetime_now - datetime.timedelta(2 * 30),
+            "updated_at__lte": datetime_now,
         }
         posts = posts.filter(**filter_kwargs)
 
     return posts
 
 
 def get_api_urls() -> tp.Dict[str, str]:
     return {
-        'api_authors_search_url': reverse('api_authors_search'),
-        'api_issues_search_url': reverse('api_issues_search'),
+        "api_authors_search_url": reverse("api_authors_search"),
+        "api_issues_search_url": reverse("api_issues_search"),
     }
 
 
 @login_required
 def index(request):
-    filter_ = request.GET.get('filter')
+    filter_ = request.GET.get("filter")
 
     current_context_site = get_current_site(request)
     queryset = Post.on_site(site=current_context_site)
     posts: QuerySet = _get_filtered_posts_queryset(
         filter_, request.user.user, queryset=queryset
     )
 
     # If user has any permissions to create any type of articles
-    has_create_articles_permissions = any((
-        request.user.has_perm('magplan.create_generic_post'),
-        request.user.has_perm('magplan.create_archive_post'),
-        request.user.has_perm('magplan.create_advert_post'),
-        request.user.has_perm('magplan.create_regular_post'),
-    ))
-
-    return render(request, 'magplan/articles/index.html', {
-        'posts': posts,
-        'filter_': filter_,
-        'has_create_articles_permissions': has_create_articles_permissions,
-    })
+    has_create_articles_permissions = any(
+        (
+            request.user.has_perm("magplan.create_generic_post"),
+            request.user.has_perm("magplan.create_archive_post"),
+            request.user.has_perm("magplan.create_advert_post"),
+            request.user.has_perm("magplan.create_regular_post"),
+        )
+    )
+
+    return render(
+        request,
+        "magplan/articles/index.html",
+        {
+            "posts": posts,
+            "filter_": filter_,
+            "has_create_articles_permissions": has_create_articles_permissions,
+        },
+    )
 
 
 @login_required
 def default(request: HttpRequest):
     form = DefaultPostModelForm()
 
-    if request.method == 'POST':
+    if request.method == "POST":
         form: Post = DefaultPostModelForm(request.POST)
 
         if form.is_valid():
             current_site = get_current_site(request)
             post: Post = form.save(commit=False)
 
             post.site = current_site
             post.editor = request.user.user
-            post.stage = Stage.on_current_site.get(slug='waiting')
+            post.stage = Stage.on_current_site.get(slug="waiting")
 
             post.save()
             form.save_m2m()
 
-            return redirect('posts_show', post.id)
+            return redirect("posts_show", post.id)
 
-    return render(request, 'magplan/articles/default.html', {
-        'form': form,
-        **get_api_urls(),
-    })
+    return render(
+        request,
+        "magplan/articles/default.html",
+        {
+            "form": form,
+            **get_api_urls(),
+        },
+    )
 
 
 @login_required
 def archived(request):
     form = ArchivedPostModelForm()
 
-    if request.method == 'POST':
+    if request.method == "POST":
         form = ArchivedPostModelForm(request.POST)
 
         if form.is_valid():
             post = form.save(commit=False)
             post.editor = request.user.user
-            post.stage = Stage.objects.get(slug='waiting')
+            post.stage = Stage.objects.get(slug="waiting")
 
             post.features = Post.POST_FEATURES_ARCHIVE
 
             post.save()
             form.save_m2m()
 
-            return redirect('posts_show', post.id)
+            return redirect("posts_show", post.id)
 
-    return render(request, 'magplan/articles/archived.html', {
-        'form': form,
-        **get_api_urls(),
-    })
+    return render(
+        request,
+        "magplan/articles/archived.html",
+        {
+            "form": form,
+            **get_api_urls(),
+        },
+    )
 
 
 @login_required
 def whitelisted(request):
     form = WhitelistedPostExtendedModelForm()
 
-    if request.method == 'POST':
+    if request.method == "POST":
         form = WhitelistedPostExtendedModelForm(request.POST)
 
         if form.is_valid():
             post = form.save(commit=False)
             post.editor = request.user.user
-            post.stage = Stage.objects.get(slug='waiting')
+            post.stage = Stage.objects.get(slug="waiting")
 
             post.save()
             form.save_m2m()
 
-            return redirect('posts_show', post.id)
+            return redirect("posts_show", post.id)
 
-    api_authors_search_url = reverse('api_authors_search')
-    api_issues_search_url = reverse('api_issues_search')
+    api_authors_search_url = reverse("api_authors_search")
+    api_issues_search_url = reverse("api_issues_search")
 
-    return render(request, 'magplan/articles/whitelisted.html', {
-        'form': form,
-        'api_authors_search_url': api_authors_search_url,
-        'api_issues_search_url': api_issues_search_url,
-    })
+    return render(
+        request,
+        "magplan/articles/whitelisted.html",
+        {
+            "form": form,
+            "api_authors_search_url": api_authors_search_url,
+            "api_issues_search_url": api_issues_search_url,
+        },
+    )
 
 
 @login_required
 def advert(request):
     form = AdPostExtendedModelForm()
 
-    if request.method == 'POST':
+    if request.method == "POST":
         form = AdPostExtendedModelForm(request.POST)
 
         if form.is_valid():
             post = form.save(commit=False)
             post.editor = request.user.user
-            post.stage = Stage.objects.get(slug='waiting')
+            post.stage = Stage.objects.get(slug="waiting")
 
             post.features = Post.POST_FEATURES_ADVERT
 
             post.save()
 
-            form.cleaned_data['issues'] = [form.cleaned_data['issues']]  # HACK: cast object as list to support m2m
+            form.cleaned_data["issues"] = [
+                form.cleaned_data["issues"]
+            ]  # HACK: cast object as list to support m2m
             form.save_m2m()
 
-            return redirect('posts_show', post.id)
+            return redirect("posts_show", post.id)
 
-    api_authors_search_url = reverse('api_authors_search')
+    api_authors_search_url = reverse("api_authors_search")
 
-    return render(request, 'magplan/articles/advert.html', {
-        'form': form,
-        'api_authors_search_url': api_authors_search_url,
-    })
+    return render(
+        request,
+        "magplan/articles/advert.html",
+        {
+            "form": form,
+            "api_authors_search_url": api_authors_search_url,
+        },
+    )
 
 
 @login_required
 def search(request):
-    if request.method == 'POST':
-        q = request.POST['search_query']
-        posts = (Post.objects
-                 .prefetch_related('section', 'stage', 'issues__magazine', 'editor__profile')
-                 .filter(Q(title__icontains=q) | Q(kicker__icontains=q)))
-
-        return render(request, 'magplan/articles/index.html', {
-            'posts': posts,
-            'q': q,
-        })
+    if request.method == "POST":
+        q = request.POST["search_query"]
+        posts = Post.objects.prefetch_related(
+            "section", "stage", "issues__magazine", "editor__profile"
+        ).filter(Q(title__icontains=q) | Q(kicker__icontains=q))
+
+        return render(
+            request,
+            "magplan/articles/index.html",
+            {
+                "posts": posts,
+                "q": q,
+            },
+        )
```

### Comparing `magplan-3.1.0/src/magplan/views/authors.py` & `magplan-3.1.1/src/magplan/views/authors.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,83 +5,107 @@
 from django.shortcuts import render, redirect
 
 from magplan.models import User, Post
 from magplan.forms import UserModelForm, ProfileModelForm
 
 
 @login_required
-@permission_required('magplan.manage_authors')
+@permission_required("magplan.manage_authors")
 def index(request):
-    users = User.objects.prefetch_related('profile').order_by('profile__l_name').all()
-    return render(request, 'magplan/authors/index.html', {
-        'users': users
-    })
+    users = (
+        User.objects.prefetch_related("profile")
+        .order_by("profile__l_name")
+        .all()
+    )
+    return render(request, "magplan/authors/index.html", {"users": users})
 
 
 @login_required
-@permission_required('magplan.manage_authors')
+@permission_required("magplan.manage_authors")
 def new(request):
-    if request.method == 'POST':
+    if request.method == "POST":
         user_form = UserModelForm(request.POST)
         profile_form = ProfileModelForm(request.POST)
 
         if user_form.is_valid() and profile_form.is_valid():
             user = user_form.save(commit=False)
             # Authors should be inactive by default
             user.is_active = False
             user.save()
 
-            profile_form = ProfileModelForm(request.POST, instance=user.profile)
+            profile_form = ProfileModelForm(
+                request.POST, instance=user.profile
+            )
             profile_form.save()
 
-            messages.add_message(request, messages.INFO, f'Автор «{user}» успешно создан')
+            messages.add_message(
+                request, messages.INFO, f"Автор «{user}» успешно создан"
+            )
 
-            return redirect('authors_edit', user.id)
+            return redirect("authors_edit", user.id)
 
     else:
         user_form = UserModelForm()
         profile_form = ProfileModelForm()
 
-    return render(request, 'magplan/authors/new.html', {
-        'user_form': user_form,
-        'profile_form': profile_form,
-    })
+    return render(
+        request,
+        "magplan/authors/new.html",
+        {
+            "user_form": user_form,
+            "profile_form": profile_form,
+        },
+    )
 
 
 @login_required
-@permission_required('magplan.manage_authors')
+@permission_required("magplan.manage_authors")
 def show(request, user_id):
     user = User.objects.get(id=user_id)
-    posts = (Post.objects.filter(Q(authors=user) | Q(editor=user))
-             .prefetch_related('authors', 'editor', 'stage', 'section')
-             .exclude(stage__slug='vault')
-             .order_by('created_at'))
-    return render(request, 'magplan/authors/show.html', {
-        'user': user,
-        'posts': posts,
-    })
+    posts = (
+        Post.objects.filter(Q(authors=user) | Q(editor=user))
+        .prefetch_related("authors", "editor", "stage", "section")
+        .exclude(stage__slug="vault")
+        .order_by("created_at")
+    )
+    return render(
+        request,
+        "magplan/authors/show.html",
+        {
+            "user": user,
+            "posts": posts,
+        },
+    )
 
 
 @login_required
-@permission_required('magplan.manage_authors')
+@permission_required("magplan.manage_authors")
 def edit(request, user_id):
     user = User.objects.get(id=user_id)
 
-    if request.method == 'POST':
+    if request.method == "POST":
         user_form = UserModelForm(request.POST, instance=user)
         profile_form = ProfileModelForm(request.POST, instance=user.profile)
 
         if user_form.is_valid() and profile_form.is_valid():
             user_form.save()
             profile_form.save()
 
-            messages.add_message(request, messages.INFO, f'Автор «{user}» успешно отредактирован')
+            messages.add_message(
+                request,
+                messages.INFO,
+                f"Автор «{user}» успешно отредактирован",
+            )
 
     else:
         user_form = UserModelForm(instance=user)
         profile_form = ProfileModelForm(instance=user.profile)
 
-    return render(request, 'magplan/authors/edit.html', {
-        'user_form': user_form,
-        'profile_form': profile_form,
-        'user': user,
-    })
+    return render(
+        request,
+        "magplan/authors/edit.html",
+        {
+            "user_form": user_form,
+            "profile_form": profile_form,
+            "user": user,
+        },
+    )
```

### Comparing `magplan-3.1.0/src/magplan/views/ideas.py` & `magplan-3.1.1/src/magplan/views/ideas.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from magplan.forms import (
     CommentModelForm,
     IdeaModelForm,
     PostBaseModelForm,
     IDEA_AUTHOR_SELF_CHOICE,
 )
 from magplan.models import Idea, Issue, Vote
-from magplan.tasks.send_idea_comment_notification import send_idea_comment_notification
+from magplan.tasks.send_idea_comment_notification import (
+    send_idea_comment_notification,
+)
 from magplan.tasks.send_idea_notification import send_idea_notification
 from magplan.utils import safe_cast
 
 IDEAS_PER_PAGE = 20
 
 # HACK
 AUTHOR_TYPE_DAY = datetime.date(2019, 6, 29)
@@ -51,15 +53,18 @@
             # Save authors, if existing specified
             if idea.author_type == Idea.AUTHOR_TYPE_EXISTING:
                 form.save_m2m()
 
                 # Handle virtual SELF choice (which is actual AUTHOR_TYPE_EXISTING)
                 # We did it after actual m2m save as form.save_m2m()will overwrite any
                 # model assignments usgin empty Form authors field. So saving one more time
-                if request.POST.get("author_type") == IDEA_AUTHOR_SELF_CHOICE.slug:
+                if (
+                    request.POST.get("author_type")
+                    == IDEA_AUTHOR_SELF_CHOICE.slug
+                ):
                     idea.authors.add(request.user.user)
                     idea.save()
 
             send_idea_notification.delay(idea.id)
 
             messages.add_message(
                 request,
@@ -124,15 +129,17 @@
         "markup",
         "proofreading_spell",
         "proofreading_chief_dpt",
         "proofreading_chief",
         "publishing",
     )
     opened_issues = (
-        Issue.on_current_site.filter(posts__stage__slug__in=article_stages_for_opened_issues)
+        Issue.on_current_site.filter(
+            posts__stage__slug__in=article_stages_for_opened_issues
+        )
         .order_by("number")
         .distinct()
         .all()[:5]
     )
 
     if not opened_issues:
         return None, []
@@ -148,15 +155,16 @@
 @login_required
 def show(request, idea_id):
     idea = Idea.objects.prefetch_related("votes__user").get(id=idea_id)
     initial_issues_suggesion, issues_suggesions = _get_suggestion_issues()
     form = PostBaseModelForm(
         initial={
             "issues": initial_issues_suggesion,
-            "finished_at": datetime.datetime.now() + datetime.timedelta(days=3),
+            "finished_at": datetime.datetime.now()
+            + datetime.timedelta(days=3),
         },
         instance=idea,
     )
 
     api_authors_search_url = reverse("api_authors_search")
     api_issues_search_url = reverse("api_issues_search")
 
@@ -186,33 +194,39 @@
     if request.method == "POST":
         score = request.POST.get("score", DEFAULT_VOTE_SCORE)
     else:
         score = request.GET.get("score", DEFAULT_VOTE_SCORE)
 
     score = safe_cast(score, to=int, on_error=DEFAULT_VOTE_SCORE)
 
-    allowed_scored: List[int] = [score_choice[0] for score_choice in Vote.SCORE_CHOICES]
+    allowed_scored: List[int] = [
+        score_choice[0] for score_choice in Vote.SCORE_CHOICES
+    ]
 
     if score not in allowed_scored:
         score = Vote.SCORE_50
 
     vote.score = score
     vote.save()
 
-    messages.add_message(request, messages.SUCCESS, "Ваш голос учтен. Спасибо!")
+    messages.add_message(
+        request, messages.SUCCESS, "Ваш голос учтен. Спасибо!"
+    )
 
     return redirect("ideas_show", idea_id=idea.id)
 
 
 @login_required
 def approve(request, idea_id):
     idea = Idea.objects.prefetch_related("votes__user").get(id=idea_id)
 
     if request.method == "POST":
-        idea.approved = True if request.POST.get("approve", False) == "1" else False
+        idea.approved = (
+            True if request.POST.get("approve", False) == "1" else False
+        )
         idea.save()
         messages.add_message(request, messages.INFO, "Статус идеи изменен.")
 
         # send email
         if idea.approved is True and idea.editor != request.user.user:
             subject = f"Идея «{idea}» прошла голосование! Ждем статью"
             html_content = render_to_string(
@@ -220,15 +234,18 @@
                 {
                     "idea": idea,
                     "APP_URL": os.environ.get("APP_URL", None),
                 },
             )
             text_content = html2text.html2text(html_content)
             msg = EmailMultiAlternatives(
-                subject, text_content, config.PLAN_EMAIL_FROM, [idea.editor.email]
+                subject,
+                text_content,
+                config.PLAN_EMAIL_FROM,
+                [idea.editor.email],
             )
             msg.attach_alternative(html_content, "text/html")
             msg.send()
 
     return redirect("ideas_show", idea_id=idea.id)
```

### Comparing `magplan-3.1.0/src/magplan/views/index.py` & `magplan-3.1.1/src/magplan/views/index.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,37 +50,37 @@
             yield start_date + datetime.timedelta(days)
 
 
 # Create your views here.
 @login_required
 def index(request):
     self_posts = (
-        Post.on_current_site.prefetch_related('stage')
+        Post.on_current_site.prefetch_related("stage")
         .filter(
             Q(stage__assignee__isnull=False, stage__assignee=request.user.user)
             | Q(stage__assignee__isnull=True, editor=request.user.user)
         )
-        .exclude(stage__slug__in=['vault', 'published'])
+        .exclude(stage__slug__in=["vault", "published"])
     )
 
     need_to_vote = Idea.on_current_site.filter(approved__isnull=True).exclude(
         votes__user=request.user.user
     )
 
     opened_issues = Issue.on_current_site.filter(
         posts__stage__slug__in=[
-            'waiting',
-            'proofreading_editor',
-            'precheck',
-            'spellcheck',
-            'markup',
-            'proofreading_spell',
-            'proofreading_chief_dpt',
-            'proofreading_chief',
-            'publishing',
+            "waiting",
+            "proofreading_editor",
+            "precheck",
+            "spellcheck",
+            "markup",
+            "proofreading_spell",
+            "proofreading_chief_dpt",
+            "proofreading_chief",
+            "publishing",
         ]
     ).distinct()
 
     # Count schedule
     schedule = {}
     time_start, time_end = get_schedule_starttime()
     scheduled_posts = Post.on_current_site.filter(
@@ -95,16 +95,18 @@
                 <= day.astimezone() + datetime.timedelta(days=1),
                 scheduled_posts,
             )
         )
 
     return render(
         request,
-        'magplan/index/index.html',
+        "magplan/index/index.html",
         {
-            'self_posts': self_posts,
-            'need_to_vote': need_to_vote,
-            'opened_issues': opened_issues,
-            'schedule': schedule,
-            'today': datetime.datetime.today().replace(hour=0, minute=0, second=0),
+            "self_posts": self_posts,
+            "need_to_vote": need_to_vote,
+            "opened_issues": opened_issues,
+            "schedule": schedule,
+            "today": datetime.datetime.today().replace(
+                hour=0, minute=0, second=0
+            ),
         },
     )
```

### Comparing `magplan-3.1.0/src/magplan/views/issues.py` & `magplan-3.1.1/src/magplan/views/issues.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from django.shortcuts import render, HttpResponse, redirect
 
 
 # Create your views here.
 @login_required
 def index(request):
     issues = (
-        Issue.on_current_site.all().order_by("-number").prefetch_related("magazine")
+        Issue.on_current_site.all()
+        .order_by("-number")
+        .prefetch_related("magazine")
     )
 
     return render(
         request,
         "magplan/issues/index.html",
         {
             "issues": issues,
@@ -55,15 +57,20 @@
         request,
         "magplan/issues/show.html",
         {
             "issue": issue,
             "posts": posts,
             "stats": {
                 "has_text": len(
-                    list(filter(lambda p: (p.xmd is not None) and (p.xmd != ""), posts))
+                    list(
+                        filter(
+                            lambda p: (p.xmd is not None) and (p.xmd != ""),
+                            posts,
+                        )
+                    )
                 ),
                 "incomplete": len(
                     list(filter(lambda p: p.stage.slug != "published", posts))
                 ),
             },
         },
     )
```

### Comparing `magplan-3.1.0/src/magplan/views/posts.py` & `magplan-3.1.1/src/magplan/views/posts.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,25 @@
     Attachment,
     Comment,
     Idea,
     Post,
     Stage,
     User,
 )
-from magplan.tasks.send_post_comment_notification import send_post_comment_notification
+from magplan.tasks.send_post_comment_notification import (
+    send_post_comment_notification,
+)
 from magplan.tasks.upload_post_to_wp import upload_post_to_wp
 from slugify import slugify
 
-IMAGE_MIME_TYPE_JPEG= 'image/jpeg'
+IMAGE_MIME_TYPE_JPEG = "image/jpeg"
 IMAGE_MIME_TYPES = {
-    'image/gif',
+    "image/gif",
     IMAGE_MIME_TYPE_JPEG,
-    'image/png',
+    "image/png",
 }
 
 
 def _get_arbitrary_chunk(post: Post) -> str:
     """Render instance specific template code
 
     Used to render some arbitrary HTML code in a context of Post instance.
@@ -55,18 +57,18 @@
     """
     instance_template = Template(config.PLAN_POSTS_INSTANCE_CHUNK)
     instance_chunk = instance_template.render(Context({"post": post}))
     return instance_chunk
 
 
 def _create_system_comment(
-        action_type, user, post, changelog=None, attachments=None, stage=None
+    action_type, user, post, changelog=None, attachments=None, stage=None
 ) -> Comment:
     """Create auto-generated system comment with post changes logs
-    
+
     :param action_type:
     :param user:
     :param post:
     :param changelog:
     :return:
     """
     if not config.SYSTEM_USER_ID:
@@ -120,15 +122,18 @@
     if "wp_id" in changed_fields:
         changed_fields.remove("wp_id")
 
     __ = lambda form, field: (
         ", ".join([str(i) for i in form.initial.get(field)]),
         ", ".join([str(i) for i in form.cleaned_data.get(field)]),
     )
-    _ = lambda form, field: (form.initial.get(field), form.cleaned_data.get(field))
+    _ = lambda form, field: (
+        form.initial.get(field),
+        form.cleaned_data.get(field),
+    )
     for changed_field in changed_fields:
         log = None
 
         if changed_field == "issues":
             log = '* выпуски сменились с "{0}" на "{1}"'.format(
                 *__(form, changed_field)
             )
@@ -169,16 +174,15 @@
     if user.has_perm("magplan.edit_extended_post_attrs"):
         return True
 
     return False
 
 
 def _save_attachments(
-        files: List, post: Post, user: User,
-        featured_image_file: Optional = None
+    files: List, post: Post, user: User, featured_image_file: Optional = None
 ) -> List[Attachment]:
     attachments = []
 
     with transaction.atomic():
         for file in files:
             # Delete files with the same filename,
             # uploaded for current post. Emulates overwrite without
@@ -206,15 +210,18 @@
             else:
                 attachment.type = Attachment.TYPE_FILE
 
             attachment.save()
             attachments.append(attachment)
 
         # This can be spoofed on client_side
-        if featured_image_file and featured_image_file.content_type == IMAGE_MIME_TYPE_JPEG:
+        if (
+            featured_image_file
+            and featured_image_file.content_type == IMAGE_MIME_TYPE_JPEG
+        ):
             # Delete any previously uploaded featured images
             Attachment.objects.filter(
                 post=post, type=Attachment.TYPE_FEATURED_IMAGE
             ).delete()
 
             attachment = Attachment(
                 post=post,
@@ -222,46 +229,41 @@
                 original_filename=featured_image_file.name,
                 type=Attachment.TYPE_FEATURED_IMAGE,
                 file=featured_image_file,
             )  # save original filename
 
             attachment.save()
 
-
     return attachments
 
 
 @login_required
 def show(request, post_id):
     post = Post.objects.prefetch_related(
         "editor", "authors", "stage", "section", "issues", "comments__user"
     ).get(id=post_id)
 
     post_meta_form = PostMetaForm(
-        initial={
-            'wp_id': post.meta.get('wpid')
-        },
-        instance=post
+        initial={"wp_id": post.meta.get("wpid")}, instance=post
     )
 
-    api_issues_search_url = reverse('api_issues_search')
+    api_issues_search_url = reverse("api_issues_search")
 
     return render(
         request,
         "magplan/posts/show.html",
         {
             "post": post,
             "stages": Stage.on_current_site.order_by("sort").all(),
             "instance_chunk": _get_arbitrary_chunk(post),
             "comment_form": CommentModelForm(),
             "meta_form": post_meta_form,
             "TYPE_CHOICES": Comment.TYPE_CHOICES,
             "SYSTEM_ACTION_CHOICES": Comment.SYSTEM_ACTION_CHOICES,
-            'api_issues_search_url': api_issues_search_url,
-
+            "api_issues_search_url": api_issues_search_url,
         },
     )
 
 
 @login_required
 def create(request):
     if request.method == "POST":
@@ -289,56 +291,68 @@
 @login_required
 def edit(request, post_id):
     post = Post.objects.prefetch_related(
         "editor", "authors", "stage", "section", "issues"
     ).get(id=post_id)
 
     if request.method == "POST":
-        form = PostExtendedModelForm(request.POST, request.FILES, instance=post)
+        form = PostExtendedModelForm(
+            request.POST, request.FILES, instance=post
+        )
 
         attachments_files = request.FILES.getlist("attachments")
-        featured_image_files = request.FILES.getlist('featured_image')
+        featured_image_files = request.FILES.getlist("featured_image")
         attachments = _save_attachments(
-            attachments_files, post, request.user.user,
+            attachments_files,
+            post,
+            request.user.user,
             featured_image_file=(
                 featured_image_files[0] if featured_image_files else None
-            )
+            ),
         )
 
         if form.is_valid():
             post.imprint_updater(request.user.user)
             form.save()
 
             _create_system_comment(
                 Comment.SYSTEM_ACTION_UPDATE,
                 request.user.user,
                 post,
                 attachments=attachments,
             )
             messages.add_message(
-                request, messages.SUCCESS, "Пост «%s» успешно отредактирован" % post
+                request,
+                messages.SUCCESS,
+                "Пост «%s» успешно отредактирован" % post,
             )
 
             return redirect("posts_edit", post_id)
 
         else:
             messages.add_message(
-                request, messages.ERROR, "При обновлении поста произошла ошибка ввода"
+                request,
+                messages.ERROR,
+                "При обновлении поста произошла ошибка ввода",
             )
 
     else:
         form = PostExtendedModelForm(instance=post)
 
-    api_authors_search_url = reverse('api_authors_search')
+    api_authors_search_url = reverse("api_authors_search")
 
-    return render(request, "magplan/posts/edit.html", {
-        "post": post,
-        "form": form,
-        'api_authors_search_url': api_authors_search_url
-    })
+    return render(
+        request,
+        "magplan/posts/edit.html",
+        {
+            "post": post,
+            "form": form,
+            "api_authors_search_url": api_authors_search_url,
+        },
+    )
 
 
 @login_required
 def edit_meta(request, post_id):
     try:
         post = Post.objects.get(id=post_id)
     except Post.DoesNotExist:
@@ -359,67 +373,82 @@
 
         form.save()
 
         # Create system comment with changelog
         changelog = _generate_changelog_for_form(form)
         if len(changelog) > 0:
             _create_system_comment(
-                Comment.SYSTEM_ACTION_CHANGE_META, request.user.user, post, changelog
+                Comment.SYSTEM_ACTION_CHANGE_META,
+                request.user.user,
+                post,
+                changelog,
             )
 
-        messages.add_message(request, messages.INFO, f"Пост {post} успешно обновлен!")
+        messages.add_message(
+            request, messages.INFO, f"Пост {post} успешно обновлен!"
+        )
 
     return redirect("posts_show", post_id)
 
 
 @login_required
 def set_stage(request, post_id, system=Comment.TYPE_SYSTEM):
-    post = Post.objects.prefetch_related("stage__n_stage", "stage__p_stage").get(
-        id=post_id
-    )
+    post = Post.objects.prefetch_related(
+        "stage__n_stage", "stage__p_stage"
+    ).get(id=post_id)
 
     raw_new_stage_id: Optional[str] = request.POST.get("new_stage_id")
     if not raw_new_stage_id:
         return HttpResponseForbidden()
 
-    new_stage_id: int =  int(raw_new_stage_id)
-        
+    new_stage_id: int = int(raw_new_stage_id)
 
     if request.method == "POST":
         if not _authorize_stage_change(request.user.user, post, new_stage_id):
             return HttpResponseForbidden()
 
         stage = Stage.objects.get(id=new_stage_id)
 
         # set deadline to current stage durtion. If no duration, append 1 day
         duration = stage.duration if stage.duration else 1
-        post.finished_at = post.finished_at + +datetime.timedelta(days=duration)
+        post.finished_at = post.finished_at + +datetime.timedelta(
+            days=duration
+        )
         post.stage = stage
         post.imprint_updater(request.user.user)
         post.save()
         messages.add_message(
             request, messages.INFO, "Текущий этап статьи «%s» обновлен" % post
         )
 
         # Create system comment
         _create_system_comment(
-            Comment.SYSTEM_ACTION_SET_STAGE, request.user.user, post, stage=post.stage
+            Comment.SYSTEM_ACTION_SET_STAGE,
+            request.user.user,
+            post,
+            stage=post.stage,
         )
 
         # TODO: extract method
         # Send email if stage allows it
-        if post.assignee != request.user.user and stage.skip_notification is False:
+        if (
+            post.assignee != request.user.user
+            and stage.skip_notification is False
+        ):
             subject = f"На вас назначена статья «{post}»"
             html_content = render_to_string(
                 "email/assigned_to_you.html",
                 {"post": post, "APP_URL": os.environ.get("APP_URL", None)},
             )
             text_content = html2text.html2text(html_content)
             msg = EmailMultiAlternatives(
-                subject, text_content, config.PLAN_EMAIL_FROM, [post.assignee.email]
+                subject,
+                text_content,
+                config.PLAN_EMAIL_FROM,
+                [post.assignee.email],
             )
             msg.attach_alternative(html_content, "text/html")
             msg.send()
 
             return redirect("posts_show", post_id)
 
     return redirect("posts_show", post.id)
@@ -493,16 +522,20 @@
             try:
                 zipfile.write(fs_path, arcname=filename)
             except Exception as e:
                 # TODO: handle not found files
                 pass
         zipfile.close()
 
-        resp = HttpResponse(s.getvalue(), content_type="application/x-zip-compressed")
-        resp["Content-Disposition"] = f"attachment; filename=content_{post_id}.zip"
+        resp = HttpResponse(
+            s.getvalue(), content_type="application/x-zip-compressed"
+        )
+        resp["Content-Disposition"] = (
+            f"attachment; filename=content_{post_id}.zip"
+        )
         return resp
 
 
 def send_to_wp(request: HttpRequest, post_id: int) -> HttpResponse:
     if request.method == "GET":
         post = get_object_or_404(Post, id=post_id)
         upload_post_to_wp.delay(post.id)
```

### Comparing `magplan-3.1.0/src/magplan/views/preferences.py` & `magplan-3.1.1/src/magplan/views/preferences.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 from django.shortcuts import redirect, render
 from dynamic_preferences.users.forms import user_preference_form_builder
 
 
 @login_required
 def index(request):
     PreferencesForm = user_preference_form_builder(instance=request.user.user)
-    if request.method == 'POST':
+    if request.method == "POST":
         form = PreferencesForm(request.POST)
         if form.is_valid():
             form.update_preferences()
             messages.add_message(
                 request, messages.SUCCESS, "Настройи успешно обновлены"
             )
 
-            return redirect('preferences_index')
+            return redirect("preferences_index")
         else:
             # TODO: check, if form reflects invalid
             #       payload for PreferencesForm
-            PreferencesForm = user_preference_form_builder(instance=request.user.user)
+            PreferencesForm = user_preference_form_builder(
+                instance=request.user.user
+            )
 
-    return render(request, 'magplan/preferences/index.html', {'form': PreferencesForm})
+    return render(
+        request, "magplan/preferences/index.html", {"form": PreferencesForm}
+    )
 
 
 @login_required
-def set_current_site(request: HttpRequest) -> HttpResponse:
-    ...
+def set_current_site(request: HttpRequest) -> HttpResponse: ...
```

### Comparing `magplan-3.1.0/src/magplan/xmd/lexers.py` & `magplan-3.1.1/src/magplan/xmd/lexers.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,109 +8,89 @@
         super(PanelBlockLexer, self).__init__(*args, **kwargs)
         self.has_lead = False
 
         self.enable_panel()
         self.enable_paywall()
 
     def enable_panel(self):
-        self.rules.panel_block = re.compile(r'\[ (.+)\n'
-                                            r'\n'
-                                            r'((?:.*?\n)*?)'
-                                            r'\n'
-                                            r'\]'
-                                            )
-        self.default_rules.insert(3, 'panel_block')
-        
-    def enable_paywall(self):
-        self.rules.paywall_block = re.compile(
-            r'^-{10,}'
+        self.rules.panel_block = re.compile(
+            r"\[ (.+)\n" r"\n" r"((?:.*?\n)*?)" r"\n" r"\]"
         )
-        self.default_rules.insert(1, 'paywall_block')
+        self.default_rules.insert(3, "panel_block")
+
+    def enable_paywall(self):
+        self.rules.paywall_block = re.compile(r"^-{10,}")
+        self.default_rules.insert(1, "paywall_block")
 
     def parse_panel_block(self, m):
         title = m.group(1)
         content = m.group(2)
 
         # We don't want trailing \n
         title = title.strip()
         content = content.strip()
 
         # Select style for panel,
         # or failback to default
-        if title == 'WWW':
-            self.tokens.append({
-                'type': 'panel_block_www_start'
-            })
-        elif title == 'INFO':
-            self.tokens.append({
-                'type': 'panel_block_info_start'
-            })
-        elif title == 'WARNING':
-            self.tokens.append({
-                'type': 'panel_block_warning_start'
-            })
-        elif title == 'GREETING':
-            self.tokens.append({
-                'type': 'panel_block_greeting_start'
-            })
-        elif title == 'TERM':
-            self.tokens.append({
-                'type': 'panel_block_term_start'
-            })
+        if title == "WWW":
+            self.tokens.append({"type": "panel_block_www_start"})
+        elif title == "INFO":
+            self.tokens.append({"type": "panel_block_info_start"})
+        elif title == "WARNING":
+            self.tokens.append({"type": "panel_block_warning_start"})
+        elif title == "GREETING":
+            self.tokens.append({"type": "panel_block_greeting_start"})
+        elif title == "TERM":
+            self.tokens.append({"type": "panel_block_term_start"})
         else:
-            self.tokens.append({
-                'type': 'panel_block_default_start',
-                'content': title
-            })
+            self.tokens.append(
+                {"type": "panel_block_default_start", "content": title}
+            )
 
         # Add nested tokens
-        if title == 'TERM':
+        if title == "TERM":
             # We treat term content as single
             # code block without nested elements
-            self.tokens.append({
-                'type': 'panel_block_term_code',
-                'content': content
-            })
+            self.tokens.append(
+                {"type": "panel_block_term_code", "content": content}
+            )
 
         else:
             self.parse(content)
 
         # Add panel end token
-        self.tokens.append({
-            'type': 'panel_block_end'
-        })
+        self.tokens.append({"type": "panel_block_end"})
 
     def parse_paragraph(self, m) -> None:
         """Parse paragraph, including lead case
 
         Lead is a first paragraph in document.
-        If 
+        If
 
         :param m: Match group for paragraph, where m.group(1) is text.
         :return:
         """
-        text: str = m.group(1).rstrip('\n')
-        is_lead: bool = False # Local marker
-        
+        text: str = m.group(1).rstrip("\n")
+        is_lead: bool = False  # Local marker
+
         # Are we parsing lead?
         if not self.has_lead:
             is_lead = True
             self.has_lead = True
-        
+
         # If it's lead, wrap with lead tokens,
         # otherwise parse as ususal paragraph
         if is_lead:
-            self.tokens.append({'type': 'lead_start'})
-            
+            self.tokens.append({"type": "lead_start"})
+
             # Strip '$ ' from text if exists
-            if text.startswith('$ '):
+            if text.startswith("$ "):
                 text = text[2:]
             self.has_lead = True
 
-        self.tokens.append({'type': 'paragraph', 'text': text})
+        self.tokens.append({"type": "paragraph", "text": text})
 
         if is_lead:
-            self.tokens.append({'type': 'lead_end'})
+            self.tokens.append({"type": "lead_end"})
 
-        
     def parse_paywall_block(self, m):
-        self.tokens.append({'type': 'paywall'})
+        self.tokens.append({"type": "paywall"})
```

### Comparing `magplan-3.1.0/src/magplan/xmd/mappers.py` & `magplan-3.1.1/src/magplan/xmd/mappers.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     if not attachments_:
         return filename
 
     return attachments_[0].file.url
 
 
 def s3_public_mapper(filename: str, attachments: List) -> str:
-    """Get public S3 filename for requested attachment
-
-    """
+    """Get public S3 filename for requested attachment"""
     # Find requested attachment from post attachments
     attachments_ = [
         attachment
         for attachment in attachments
         if attachment.original_filename == filename
     ]
     if not attachments_:
```

### Comparing `magplan-3.1.0/src/magplan/xmd/markdown.py` & `magplan-3.1.1/src/magplan/xmd/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,34 +14,34 @@
     def output_panel_block_greeting(self):
         return self.renderer.panel_block_greeting_start()
 
     def output_panel_block_term(self):
         return self.renderer.panel_block_term_start()
 
     def output_panel_block_term_code(self):
-        text = self.token.get('content', '')
+        text = self.token.get("content", "")
         return self.renderer.panel_block_term_code(text)
 
     def output_panel_block_default(self):
-        text = self.token.get('content', '')
+        text = self.token.get("content", "")
         return self.renderer.panel_block_default_start(text)
 
     def output_panel_block_end(self):
         return self.renderer.panel_block_end()
 
     def output_lead(self):
         """NOTE: this function should be called output_lead_start,
         but mistune has line:
-        
+
             # sepcial cases
             if t.endswith('_start'):
                 t = t[:-6]
-        
+
         which trims token name for some weird reason.
         """
         return self.renderer.lead_start()
 
     def output_lead_end(self):
         return self.renderer.lead_end()
-        
+
     def output_paywall(self):
         return self.renderer.paywall()
```

### Comparing `magplan-3.1.0/src/magplan/xmd/renderer.py` & `magplan-3.1.1/src/magplan/xmd/renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import typing as tp
 
 from mistune import Renderer
 
 
 class XMDRenderer(Renderer):
-    def __init__(self, image_mapper: tp.Callable, attachments: tp.List = None, *args, **kwargs):
+    def __init__(
+        self,
+        image_mapper: tp.Callable,
+        attachments: tp.List = None,
+        *args,
+        **kwargs
+    ):
         self.attachments = attachments or []
         self.image_mapper = image_mapper
 
         super(XMDRenderer, self).__init__(*args, **kwargs)
 
     def image(self, src, title, alt_text):
         # Map human-readable filename to urlencoded one
         urlencoded_filename = self.image_mapper(src, self.attachments)
 
         html = (
-            '<figure>'
+            "<figure>"
             '<img conf="%s" alt="%s" />'
-            '<figcaption>%s</figcaption>'
-            '</figure>'
+            "<figcaption>%s</figcaption>"
+            "</figure>"
         )
 
         return html % (urlencoded_filename, alt_text, alt_text)
 
     def panel_block_www_start(self):
         html = (
-            '<div class="panel www">'
-            '<div class="www-inner">'
-            '<h3>www</h3>'
+            '<div class="panel www">' '<div class="www-inner">' "<h3>www</h3>"
         )
         return html
 
     def panel_block_info_start(self):
         html = (
             '<div class="panel info">'
             '<div class="info-inner">'
-            '<h3>info</h3>'
+            "<h3>info</h3>"
         )
         return html
 
     def panel_block_warning_start(self):
         html = (
             '<div class="panel warning">'
             '<div class="warning-inner">'
-            '<h3>warning</h3>'
+            "<h3>warning</h3>"
         )
         return html
 
     def panel_block_greeting_start(self):
         html = (
             '<div class="panel greeting">'
             '<div class="greeting-inner">'
-            '<h3>greeting</h3>'
+            "<h3>greeting</h3>"
         )
         return html
 
     def panel_block_term_start(self):
         html = (
             '<div class="panel term">'
             '<div class="term-inner">'
@@ -63,41 +67,37 @@
         )
         return html
 
     def panel_block_default_start(self, text):
         html = (
             '<div class="panel default">'
             '<div class="default-inner">'
-            '<h3>%s</h3>'
+            "<h3>%s</h3>"
         )
         return html % text
 
     def panel_block_term_code(self, content):
-        html = (
-            '<pre><code>'
-            '%s'
-            '</code></pre>'
-        )
+        html = "<pre><code>" "%s" "</code></pre>"
         return html % content
 
     def panel_block_end(self):
-        html = '</div></div>'
+        html = "</div></div>"
         return html
 
     def lead_start(self) -> str:
-        html = '<div class=lead>'
+        html = "<div class=lead>"
 
         return html
 
     def lead_end(self) -> str:
-        html = '</div>'
+        html = "</div>"
 
         return html
 
     def paywall(self) -> str:
         html = (
             '<div class="paywall-notice">'
-            'Продолжение статьи доступно только продписчикам'
-            '</div>'
+            "Продолжение статьи доступно только продписчикам"
+            "</div>"
         )
 
         return html
```

### Comparing `magplan-3.1.0/src/magplan/xmd/tests/test_renderer.py` & `magplan-3.1.1/src/magplan/xmd/tests/test_renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Every block element test will be automatically
 wrapped inside `<p></p>\n`. Thats why every block
 
 test should include this wrapper tag.
 """
+
 from io import BytesIO
 from unittest import TestCase
 from unittest.mock import patch, Mock
 
 import pytest
 from django.core.files import File
 from django_dynamic_fixture import G
@@ -15,32 +16,42 @@
 from magplan.models import Attachment
 from magplan.xmd.renderer import XMDRenderer
 from magplan.xmd.mappers import plan_internal_mapper
 
 
 @pytest.mark.django_db
 class TestImage(TestCase):
-    MOCK_SRC = 'dummy.jpg'
-    MOCK_TITLE = 'title'
-    MOCK_ALT_TEXT = 'alt_text'
+    MOCK_SRC = "dummy.jpg"
+    MOCK_TITLE = "title"
+    MOCK_ALT_TEXT = "alt_text"
 
     def setUp(self):
-        file1 = File(name='file1.jpg', file=BytesIO(b'abcdef'))
-        attachment1 = G(Attachment, original_filename='user_friendly_filename1.jpg', file=file1)
+        file1 = File(name="file1.jpg", file=BytesIO(b"abcdef"))
+        attachment1 = G(
+            Attachment,
+            original_filename="user_friendly_filename1.jpg",
+            file=file1,
+        )
 
         self.mock_image_mapper = Mock()
 
-        self.renderer = XMDRenderer(image_mapper=self.mock_image_mapper, attachments=[attachment1])
+        self.renderer = XMDRenderer(
+            image_mapper=self.mock_image_mapper, attachments=[attachment1]
+        )
 
         self.expected_html = (
-            '<figure>'
+            "<figure>"
             '<img conf="dummy.jpg" alt="alt_text" /><figcaption>alt_text</figcaption>'
-            '</figure>'
+            "</figure>"
         )
 
     def test_render_image(self):
         self.mock_image_mapper.return_value = self.MOCK_SRC
 
-        html = self.renderer.image(self.MOCK_SRC, self.MOCK_TITLE, self.MOCK_ALT_TEXT)
+        html = self.renderer.image(
+            self.MOCK_SRC, self.MOCK_TITLE, self.MOCK_ALT_TEXT
+        )
 
-        self.mock_image_mapper.assert_called_with(self.MOCK_SRC, self.renderer.attachments)
+        self.mock_image_mapper.assert_called_with(
+            self.MOCK_SRC, self.renderer.attachments
+        )
         assert html == self.expected_html
```

### Comparing `magplan-3.1.0/src/magplan/xmd/tests/test_utils.py` & `magplan-3.1.1/src/magplan/xmd/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,35 @@
 from magplan.models import Attachment
 from magplan.xmd.utils import get_attachment_original_filename
 
 
 @pytest.mark.django_db
 class Test_get_attachment_original_filename(TestCase):
     def setUp(self):
-        file1 = File(
-            name='file1.jpg',
-            file=io.BytesIO(b'abcdef')
+        file1 = File(name="file1.jpg", file=io.BytesIO(b"abcdef"))
+        file2 = File(name="file2.jpg", file=io.BytesIO(b"abcdef"))
+
+        attachment1 = G(
+            Attachment,
+            original_filename="user_friendly_filename1.jpg",
+            file=file1,
         )
-        file2 = File(
-            name='file2.jpg',
-            file=io.BytesIO(b'abcdef')
+        attachment2 = G(
+            Attachment,
+            original_filename="user_friendly_filename2.jpg",
+            file=file2,
         )
-
-        attachment1 = G(Attachment, original_filename='user_friendly_filename1.jpg', file=file1)
-        attachment2 = G(Attachment, original_filename='user_friendly_filename2.jpg', file=file2)
         self.attachments = [attachment1, attachment2]
 
     def test_retrieve_filename(self):
         # filename is returned with full URL path and internal hash
         # So e're checking only filename matches.
-        filename = get_attachment_original_filename('user_friendly_filename1.jpg', self.attachments)
-        assert 'file1' in filename
+        filename = get_attachment_original_filename(
+            "user_friendly_filename1.jpg", self.attachments
+        )
+        assert "file1" in filename
 
     def test_non_existing_filename(self):
-        filename = get_attachment_original_filename('404.jpg', self.attachments)
+        filename = get_attachment_original_filename(
+            "404.jpg", self.attachments
+        )
         assert not filename
```

### Comparing `magplan-3.1.0/src/magplan/xmd/xmd.py` & `magplan-3.1.1/src/magplan/xmd/xmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from magplan.xmd.lexers import PanelBlockLexer
 from magplan.xmd.mappers import plan_internal_mapper as default_image_mapper
 from magplan.xmd.markdown import ExtendedMarkdown
 from magplan.xmd.renderer import XMDRenderer
 
 
 def render_md(
-        md_text: str,
-        image_mapper: tp.Callable = default_image_mapper,
-        attachments: tp.List = None,
-        render_lead=True,
-        *args, **kwargs
+    md_text: str,
+    image_mapper: tp.Callable = default_image_mapper,
+    attachments: tp.List = None,
+    render_lead=True,
+    *args,
+    **kwargs
 ) -> str:
     """Render markdown chunk with optional assets preprocessing.
 
     :param md_text: Markdown string to redner
     :param attachments: Attachments instances, used in provided MD
     :return: Rendered HTML string
     """
```

### Comparing `magplan-3.1.0/PKG-INFO` & `magplan-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magplan
-Version: 3.1.0
+Version: 3.1.1
 Summary: 
 Author: Ilya Rusanen
 Author-email: ilya@rusanen.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

