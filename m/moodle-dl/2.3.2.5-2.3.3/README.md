# Comparing `tmp/moodle-dl-2.3.2.5.tar.gz` & `tmp/moodle_dl-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodle-dl-2.3.2.5.tar", last modified: Fri Mar 29 08:53:58 2024, max compression
+gzip compressed data, was "moodle_dl-2.3.3.tar", last modified: Mon Apr 15 13:20:33 2024, max compression
```

## Comparing `moodle-dl-2.3.2.5.tar` & `moodle_dl-2.3.3.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.553621 moodle-dl-2.3.2.5/moodle_dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.557621 moodle-dl-2.3.2.5/moodle_dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25813 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/cli/config_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/cli/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/cli/moodle_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/cli/notifications_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.557621 moodle-dl-2.3.2.5/moodle_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/download_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.557621 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/echo360.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/helixmedia_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/kalvidres_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/opencast_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/owncloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/sharepointfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/fake_download_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    41212 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/downloader/task.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.561621 moodle-dl-2.3.2.5/moodle_dl/moodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/cookie_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/core_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.561621 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/lesson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/quiz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/mods/workshop.py
--rw-r--r--   0 runner    (1001) docker     (127)    29312 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/moodle_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/moodle_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/request_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18485 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/moodle/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.561621 moodle-dl-2.3.2.5/moodle_dl/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.561621 moodle-dl-2.3.2.5/moodle_dl/notifications/console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/console/console_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/moodle_dl/notifications/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/discord/discord_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/discord/discord_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/discord/discord_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/moodle_dl/notifications/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/mail/header.png
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/mail/header_extender.png
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/mail/mail_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/mail/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/mail/mail_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/notification_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/telegram_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/telegram_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/telegram_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/xmpp_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/xmpp_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/xmpp_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    54232 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/moodle_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/moodle_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-03-29 08:53:58.000000 moodle-dl-2.3.2.5/moodle_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-29 08:53:58.000000 moodle-dl-2.3.2.5/moodle_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 08:53:58.000000 moodle-dl-2.3.2.5/moodle_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 08:53:58.000000 moodle-dl-2.3.2.5/moodle_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 08:53:58.000000 moodle-dl-2.3.2.5/moodle_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-29 08:53:58.000000 moodle-dl-2.3.2.5/moodle_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-29 08:53:58.000000 moodle-dl-2.3.2.5/moodle_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 08:53:58.565621 moodle-dl-2.3.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-29 08:53:50.000000 moodle-dl-2.3.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.670647 moodle_dl-2.3.3/moodle_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.670647 moodle_dl-2.3.3/moodle_dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25813 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/config_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/moodle_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/cli/notifications_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.674647 moodle_dl-2.3.3/moodle_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/download_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.674647 moodle_dl-2.3.3/moodle_dl/downloader/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/echo360.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/helixmedia_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/kalvidres_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/opencast_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/owncloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepointfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/fake_download_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41220 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/downloader/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.674647 moodle_dl-2.3.3/moodle_dl/moodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/cookie_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/core_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/moodle/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/book.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/lesson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/mods/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29312 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/moodle_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/moodle_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/request_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/moodle/result_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/console/console_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/header_extender.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/notification_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.678648 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/moodle_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/moodle_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 13:20:33.000000 moodle_dl-2.3.3/moodle_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:20:33.682648 moodle_dl-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-15 13:20:22.000000 moodle_dl-2.3.3/setup.py
```

### Comparing `moodle-dl-2.3.2.5/LICENSE` & `moodle_dl-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/PKG-INFO` & `moodle_dl-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.2.5
+Version: 2.3.3
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle-dl-2.3.2.5/README.md` & `moodle_dl-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/cli/__init__.py` & `moodle_dl-2.3.3/moodle_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/cli/config_wizard.py` & `moodle_dl-2.3.3/moodle_dl/cli/config_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/cli/database_manager.py` & `moodle_dl-2.3.3/moodle_dl/cli/database_manager.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/cli/moodle_wizard.py` & `moodle_dl-2.3.3/moodle_dl/cli/moodle_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/cli/notifications_wizard.py` & `moodle_dl-2.3.3/moodle_dl/cli/notifications_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/config.py` & `moodle_dl-2.3.3/moodle_dl/config.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/database.py` & `moodle_dl-2.3.3/moodle_dl/database.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/download_service.py` & `moodle_dl-2.3.3/moodle_dl/downloader/download_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/__init__.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/echo360.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/echo360.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/googledrive.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/googledrive.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/helixmedia_lti.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/helixmedia_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/kalvidres_lti.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/kalvidres_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/opencast_lti.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/opencast_lti.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/owncloud.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/owncloud.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/sharepoint.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/extractors/sharepointfiles.py` & `moodle_dl-2.3.3/moodle_dl/downloader/extractors/sharepointfiles.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/fake_download_service.py` & `moodle_dl-2.3.3/moodle_dl/downloader/fake_download_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/downloader/task.py` & `moodle_dl-2.3.3/moodle_dl/downloader/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         # if a flat path is requested
         if not course.create_directory_structure:
             return PT.flat_path_of_file(storage_path, course_name, file.content_filepath)
 
         # TODO: Get mod names automated; all mods should be in a sub-folder
         # If the file is located in a folder or in an assignment,
         # it should be saved in a sub-folder (with the name of the module).
-        if file.module_modname.endswith(('assign', 'data', 'folder', 'forum', 'lesson', 'page', 'quiz', 'workshop')):
+        if file.module_modname.endswith(('assign', 'book', 'data', 'folder', 'forum', 'lesson', 'page', 'quiz', 'workshop')):
             return PT.path_of_file_in_module(
                 storage_path, course_name, file.section_name, file.module_name, file.content_filepath
             )
         return PT.path_of_file(storage_path, course_name, file.section_name, file.content_filepath)
 
     def add_token_to_url(self, url: str) -> str:
         """
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/main.py` & `moodle_dl-2.3.3/moodle_dl/main.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/cookie_handler.py` & `moodle_dl-2.3.3/moodle_dl/moodle/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/core_handler.py` & `moodle_dl-2.3.3/moodle_dl/moodle/core_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         sections = []
         for section in course_sections:
             sections.append({"id": section.get("id"), "name": section.get("name")})
 
         return sections
 
-    async def async_load_course_cores(self, courses: List[Course]) -> Dict[int, List[Dict]]:
+    async def async_load_core_contents(self, courses: List[Course]) -> Dict[int, List[Dict]]:
         """
         Loads all course core structures for every given course
         @param entries: List of all section entries, indexed by course id
         """
         total_courses = len(courses)
 
         if total_courses == 0:
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/__init__.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from moodle_dl.config import ConfigHelper
 from moodle_dl.moodle.mods.common import MoodleMod
 from moodle_dl.moodle.request_helper import RequestHelper
 from moodle_dl.types import Course
 
 from moodle_dl.moodle.mods.assign import AssignMod  # noqa: F401 isort:skip
+from moodle_dl.moodle.mods.book import BookMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.data import DataMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.folder import FolderMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.forum import ForumMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.lesson import LessonMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.page import PageMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.quiz import QuizMod  # noqa: F401 isort:skip
 from moodle_dl.moodle.mods.workshop import WorkshopMod  # noqa: F401 isort:skip
@@ -31,17 +32,21 @@
 ) -> List[MoodleMod]:
     result = []
     for mod in ALL_MODS:
         result.append(mod(request_helper, moodle_version, user_id, last_timestamps, config))
     return result
 
 
-async def fetch_mods_files(mods_to_fetch: List[MoodleMod], courses_to_load: List[Course]) -> Dict[str, Dict]:
+async def fetch_mods_files(
+    mods_to_fetch: List[MoodleMod], courses_to_load: List[Course], core_contents: Dict[int, List[Dict]]
+) -> Dict[str, Dict]:
     "@return: Dictionary of all fetched files, indexed by mod name, then by courses, then module id"
-    mods_results = await asyncio.gather(*[mod.fetch_mod_entries(courses_to_load) for mod in mods_to_fetch])
+    mods_results = await asyncio.gather(
+        *[mod.fetch_mod_entries(courses_to_load, core_contents) for mod in mods_to_fetch]
+    )
     result = {}
     for idx, mod in enumerate(mods_to_fetch):
         result[mod.MOD_NAME] = mods_results[idx]
     return result
 
 
 def get_mod_plurals():
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/assign.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/assign.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     MOD_MIN_VERSION = 2012120300  # 2.4
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         # TODO: Add condition for assignments not only submissions
         return config.get_download_submissions() or (not (file.module_modname.endswith(cls.MOD_NAME) and file.deleted))
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         assign_courses = (
             await self.client.async_post('mod_assign_get_assignments', self.get_data_for_mod_entries_endpoint(courses))
         ).get('courses', [])
 
         result = {}
         for assign_course in assign_courses:
             course_id = assign_course.get('id', 0)
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/common.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,19 +46,21 @@
         Return True if moodle-dl is configured to downloaded the given file
         This condition is applied after comparing the current status with the local database
         """
         # TODO: Make module download conditions more granular and more generally
         # (do not only filter "deleted" mod files but all?)
         pass
 
-    async def fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         if self.version < self.MOD_MIN_VERSION:
             return {}
 
-        result = await self.real_fetch_mod_entries(courses)
+        result = await self.real_fetch_mod_entries(courses, core_contents)
         logging.info('Loaded all %s', self.MOD_PLURAL_NAME)
         return result
 
     def get_indexed_ids_of_mod_instances(self, mod_instances: Dict[int, Dict[int, Dict]]):
         """
         @param mod_instances: Dictionary of all mod instanced, indexed by courses, then module id
         """
@@ -74,15 +76,17 @@
         # Create a dictionary with all the courses we want to request
         course_ids = {}
         for idx, course in enumerate(courses):
             course_ids[str(idx)] = course.id
         return {'courseids': course_ids}
 
     @abstractmethod
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         """
         Fetches the mod entries for all courses
         @return: Dictionary of all course modules of that mod type, indexed by course id, then course module id
         """
         pass
 
     @staticmethod
@@ -202,13 +206,22 @@
             if isinstance(feature_result, list):
                 result.extend(feature_result)
             elif feature_result is not None:
                 result.append(feature_result)
         return result
 
     @staticmethod
+    def get_module_in_core_contents(course_id: int, module_id: int, core_contents: Dict[int, List[Dict]]) -> Dict:
+        course_section = core_contents.get(course_id, [])
+        for section in course_section:
+            for module in section.get('modules', []):
+                if module.get('id', 0) == module_id:
+                    return module
+        return {}
+
+    @staticmethod
     def add_module(result: Dict, course_id: int, module_id: int, module: Dict):
         if course_id not in result:
             result[course_id] = {}
         if module_id in result[course_id]:
             logging.debug('Got duplicated module %s in course %s', module_id, course_id)
         result[course_id][module_id] = module
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/data.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     MOD_PLURAL_NAME = 'databases'
     MOD_MIN_VERSION = 2015051100  # 2.9
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         return config.get_download_databases() or file.content_type != 'database_file'
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         databases = (
             await self.client.async_post(
                 'mod_data_get_databases_by_courses', self.get_data_for_mod_entries_endpoint(courses)
             )
         ).get('databases', [])
 
         result = {}
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/folder.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/folder.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,24 +11,27 @@
     MOD_MIN_VERSION = 2017051500  # 3.3
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         # TODO: Add download condition
         return True
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         folders = (
             await self.client.async_post(
                 'mod_folder_get_folders_by_courses', self.get_data_for_mod_entries_endpoint(courses)
             )
         ).get('folders', [])
 
         result = {}
         for folder in folders:
             course_id = folder.get('course', 0)
+            module_id = folder.get('coursemodule', 0)
             folder_files = folder.get('introfiles', [])
             folder_time_modified = folder.get('timemodified', 0)
             self.set_props_of_files(folder_files, type='folder_file')
 
             folder_intro = folder.get('intro', '')
             if folder_intro != '':
                 folder_files.append(
@@ -38,18 +41,20 @@
                         'description': folder_intro,
                         'timemodified': folder_time_modified,
                         'filter_urls_during_search_containing': ['/mod_folder/intro'],
                         'type': 'description',
                     }
                 )
 
+            folder_files += self.get_module_in_core_contents(course_id, module_id, core_contents).get('contents', [])
+
             self.add_module(
                 result,
                 course_id,
-                folder.get('coursemodule', 0),
+                module_id,
                 {
                     'id': folder.get('id', 0),
                     'name': folder.get('name', 'unnamed folder'),
                     'timemodified': folder_time_modified,
                     'files': folder_files,
                 },
             )
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/forum.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/forum.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     MOD_MIN_VERSION = 2013051400  # 2.5
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         # TODO: Add download condition, currently forums get filtered on API Call, and are not deleted at all
         return True
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         forums = await self.client.async_post(
             'mod_forum_get_forums_by_courses', self.get_data_for_mod_entries_endpoint(courses)
         )
 
         result = {}
         for forum in forums:
             course_id = forum.get('course', 0)
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/lesson.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/lesson.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     MOD_PLURAL_NAME = 'lessons'
     MOD_MIN_VERSION = 2017051500  # 3.3
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         return config.get_download_lessons() or (not (file.module_modname.endswith(cls.MOD_NAME) and file.deleted))
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         lessons = (
             await self.client.async_post(
                 'mod_lesson_get_lessons_by_courses', self.get_data_for_mod_entries_endpoint(courses)
             )
         ).get('lessons', [])
 
         result = {}
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/page.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     MOD_MIN_VERSION = 2017051500  # 3.3
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         # TODO: Add download condition
         return True
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         pages = (
             await self.client.async_post(
                 'mod_page_get_pages_by_courses', self.get_data_for_mod_entries_endpoint(courses)
             )
         ).get('pages', [])
 
         result = {}
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/quiz.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/quiz.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     MOD_PLURAL_NAME = 'quizzes'
     MOD_MIN_VERSION = 2016052300  # 3.1
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         return config.get_download_quizzes() or (not (file.module_modname.endswith(cls.MOD_NAME) and file.deleted))
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         quizzes = (
             await self.client.async_post(
                 'mod_quiz_get_quizzes_by_courses', self.get_data_for_mod_entries_endpoint(courses)
             )
         ).get('quizzes', [])
 
         result = {}
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/mods/workshop.py` & `moodle_dl-2.3.3/moodle_dl/moodle/mods/workshop.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     MOD_PLURAL_NAME = 'workshops'
     MOD_MIN_VERSION = 2017111300  # 3.4
 
     @classmethod
     def download_condition(cls, config: ConfigHelper, file: File) -> bool:
         return config.get_download_workshops() or (not (file.module_modname.endswith(cls.MOD_NAME) and file.deleted))
 
-    async def real_fetch_mod_entries(self, courses: List[Course]) -> Dict[int, Dict[int, Dict]]:
+    async def real_fetch_mod_entries(
+        self, courses: List[Course], core_contents: Dict[int, List[Dict]]
+    ) -> Dict[int, Dict[int, Dict]]:
         workshops = (
             await self.client.async_post(
                 'mod_workshop_get_workshops_by_courses', self.get_data_for_mod_entries_endpoint(courses)
             )
         ).get('workshops', [])
 
         result = {}
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/moodle_constants.py` & `moodle_dl-2.3.3/moodle_dl/moodle/moodle_constants.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/moodle_service.py` & `moodle_dl-2.3.3/moodle_dl/moodle/moodle_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,21 +108,21 @@
         cookie_handler = None
         if self.config.get_download_also_with_cookie():
             cookie_handler = CookieHandler(request_helper, version, self.config, self.opts)
             cookie_handler.check_and_fetch_cookies(privatetoken, user_id)
 
         courses = self.get_courses_list(core_handler, user_id)
 
+        core_contents = await core_handler.async_load_core_contents(courses)
         mods = get_all_mods(request_helper, version, user_id, database.get_last_timestamp_per_mod_module(), self.config)
-        fetched_mods_files = await fetch_mods_files(mods, courses)
-        course_cores = await core_handler.async_load_course_cores(courses)
+        fetched_mods_files = await fetch_mods_files(mods, courses, core_contents)
 
         logging.debug('Combine API results...')
         ResultBuilder(moodle_url, version, get_mod_plurals()).add_files_to_courses(
-            courses, course_cores, fetched_mods_files
+            courses, core_contents, fetched_mods_files
         )
 
         logging.debug('Checking for changes...')
         changes = database.changes_of_new_version(courses)
         changes = self.add_options_to_courses(changes)
         changes = self.filter_courses(changes, self.config, cookie_handler, courses)
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/request_helper.py` & `moodle_dl-2.3.3/moodle_dl/moodle/request_helper.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/moodle/result_builder.py` & `moodle_dl-2.3.3/moodle_dl/moodle/result_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,14 @@
             if location['module_modname'] in ['kalvidres', 'helixmedia', 'lti']:
                 location['module_modname'] = 'cookie_mod-' + location['module_modname']
                 files += self._handle_cookie_mod(module_url, **location)
 
             elif location['module_modname'].startswith(('resource', 'akarifolder', 'url', 'index_mod')):
                 files += self._handle_files(module_contents, **location)
 
-            elif location['module_modname'].startswith(('folder')):
-                # Modules whose content is directly linked, and additional content exists in their module.
-                if location['module_modname'] in fetched_mods:
-                    # find mod module with same module_id
-                    mod = fetched_mods.get(location['module_modname'], {}).get(location['module_id'], {})
-                    mod['on_main_page'] = True
-                    mod_files = mod.get('files', [])
-                    module_contents += mod_files
-
-                files += self._handle_files(module_contents, **location)
-
             elif location['module_modname'] in fetched_mods:
                 # find mod module with same module_id
                 mod = fetched_mods.get(location['module_modname'], {}).get(location['module_id'], {})
                 mod['on_main_page'] = True
                 mod_files = mod.get('files', [])
                 files += self._handle_files(mod_files, **location)
             else:
@@ -430,22 +419,22 @@
         )
 
         return files
 
     def add_files_to_courses(
         self,
         courses: List[Course],
-        course_cores: Dict[int, List[Dict]],
+        core_contents: Dict[int, List[Dict]],
         fetched_mods_files: Dict[str, Dict],
     ):
         """
         @param fetched_mods_files:
             Dictionary of all fetched mod modules files, indexed by mod name, then by courses, then module id
         """
         for course in courses:
-            course_sections = course_cores.get(course.id, [])
+            course_sections = core_contents.get(course.id, [])
 
             fetched_mods = {}
             for mod_name, mod_courses in fetched_mods_files.items():
                 fetched_mods[mod_name] = mod_courses.get(course.id, {})
 
             course.files = self.get_files_in_sections(course_sections, fetched_mods)
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/__init__.py` & `moodle_dl-2.3.3/moodle_dl/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/console/console_service.py` & `moodle_dl-2.3.3/moodle_dl/notifications/console/console_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/discord/discord_formatter.py` & `moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_formatter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/discord/discord_service.py` & `moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/discord/discord_shooter.py` & `moodle_dl-2.3.3/moodle_dl/notifications/discord/discord_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/mail/header.png` & `moodle_dl-2.3.3/moodle_dl/notifications/mail/header.png`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/mail/header_extender.png` & `moodle_dl-2.3.3/moodle_dl/notifications/mail/header_extender.png`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/mail/mail_formater.py` & `moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/mail/mail_service.py` & `moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/mail/mail_shooter.py` & `moodle_dl-2.3.3/moodle_dl/notifications/mail/mail_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/notification_service.py` & `moodle_dl-2.3.3/moodle_dl/notifications/notification_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/telegram_formater.py` & `moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/telegram_service.py` & `moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/telegram/telegram_shooter.py` & `moodle_dl-2.3.3/moodle_dl/notifications/telegram/telegram_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/xmpp_formater.py` & `moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_formater.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/xmpp_service.py` & `moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_service.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/notifications/xmpp/xmpp_shooter.py` & `moodle_dl-2.3.3/moodle_dl/notifications/xmpp/xmpp_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/types.py` & `moodle_dl-2.3.3/moodle_dl/types.py`

 * *Files identical despite different names*

### Comparing `moodle-dl-2.3.2.5/moodle_dl/utils.py` & `moodle_dl-2.3.3/moodle_dl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,14 +433,17 @@
         if name is None:
             return None
 
         # Moodle saves the title of a section in HTML-Format,
         # so we need to unescape the string
         name = html.unescape(name)
 
+        # Moodle and other websites often use full width characters and other weird UTF-8 codes, we normalize this
+        name = unicodedata.normalize('NFKC', name)
+
         name = name.replace('\n', ' ')
         name = name.replace('\r', ' ')
         name = name.replace('\t', ' ')
         name = name.replace('\xad', '')
         while '  ' in name:
             name = name.replace('  ', ' ')
         name = PathTools.sanitize_filename(name, PathTools.restricted_filenames)
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl.egg-info/PKG-INFO` & `moodle_dl-2.3.3/moodle_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.2.5
+Version: 2.3.3
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle-dl-2.3.2.5/moodle_dl.egg-info/SOURCES.txt` & `moodle_dl-2.3.3/moodle_dl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 moodle_dl/moodle/core_handler.py
 moodle_dl/moodle/moodle_constants.py
 moodle_dl/moodle/moodle_service.py
 moodle_dl/moodle/request_helper.py
 moodle_dl/moodle/result_builder.py
 moodle_dl/moodle/mods/__init__.py
 moodle_dl/moodle/mods/assign.py
+moodle_dl/moodle/mods/book.py
 moodle_dl/moodle/mods/common.py
 moodle_dl/moodle/mods/data.py
 moodle_dl/moodle/mods/folder.py
 moodle_dl/moodle/mods/forum.py
 moodle_dl/moodle/mods/lesson.py
 moodle_dl/moodle/mods/page.py
 moodle_dl/moodle/mods/quiz.py
```

### Comparing `moodle-dl-2.3.2.5/setup.py` & `moodle_dl-2.3.3/setup.py`

 * *Files identical despite different names*

