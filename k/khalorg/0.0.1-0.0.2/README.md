# Comparing `tmp/khalorg-0.0.1.tar.gz` & `tmp/khalorg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khalorg-0.0.1.tar", last modified: Mon Apr  8 19:33:19 2024, max compression
+gzip compressed data, was "khalorg-0.0.2.tar", last modified: Mon Apr 15 19:50:24 2024, max compression
```

## Comparing `khalorg-0.0.1.tar` & `khalorg-0.0.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.214148 khalorg-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.182148 khalorg-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.186148 khalorg-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 19:33:09.000000 khalorg-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-08 19:33:09.000000 khalorg-0.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 19:33:09.000000 khalorg-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-08 19:33:09.000000 khalorg-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 19:33:09.000000 khalorg-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 19:33:09.000000 khalorg-0.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-08 19:33:19.214148 khalorg-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-08 19:33:09.000000 khalorg-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.198148 khalorg-0.0.1/demo/
--rw-r--r--   0 runner    (1001) docker     (127)   474334 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)   814156 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/edit.gif
--rw-r--r--   0 runner    (1001) docker     (127)   805028 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/list.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    40467 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/meeting.org
--rw-r--r--   0 runner    (1001) docker     (127)  5848880 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/neovim-plugin.gif
--rw-r--r--   0 runner    (1001) docker     (127)   330668 2024-04-08 19:33:09.000000 khalorg-0.0.1/demo/new.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.198148 khalorg-0.0.1/extras/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4045 2024-04-08 19:33:09.000000 khalorg-0.0.1/extras/calsync
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-08 19:33:09.000000 khalorg-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:33:19.214148 khalorg-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 19:33:09.000000 khalorg-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.186148 khalorg-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.198148 khalorg-0.0.1/src/khalorg/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/src/khalorg/khal/
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/khal/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/src/khalorg/org/
--rw-r--r--   0 runner    (1001) docker     (127)    19368 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/org/agenda_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/org/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/rrule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/src/khalorg/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_delete_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_edit_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_list_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/description_new_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/khal_format.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 19:33:09.000000 khalorg-0.0.1/src/khalorg/static/khalorg_format.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.214148 khalorg-0.0.1/src/khalorg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 19:33:19.000000 khalorg-0.0.1/src/khalorg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.202148 khalorg-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/agenda_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/khalorg_tester
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.206148 khalorg-0.0.1/tests/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.210148 khalorg-0.0.1/tests/static/agenda_items/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/all_day.org
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/all_day_until_with_time.org
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/body_first.org
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/demo.org
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/duplicate.org
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/minimal.org
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps.org
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps_unsorted.org
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/no_heading.org
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/no_time_stamp.org
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/not_first_child.org
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/not_first_heading.org
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/not_first_level.org
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/past.org
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_allday.org
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_and_non_recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved.org
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved_expected.org
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_monthly.org
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/recurring_not_supported.org
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_1th.org
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_allday.org
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_and_non_recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_duplicates.org
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_monthly.org
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_not_supported.org
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/scheduled_and_deadline.org
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/short_timestamp.org
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/timestamp_scheduled_deadline.org
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/two_items.org
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/two_timestamps.org
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/valid.org
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/agenda_items/valid_no_until.org
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/config_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/khalorg_format_full.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_combined.ini
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_default.ini
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_khal
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/static/test_config_user.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.210148 khalorg-0.0.1/tests/test_khal/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_khal/test_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:33:19.214148 khalorg-0.0.1/tests/test_org/
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_org/test_agenda_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_org/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-08 19:33:09.000000 khalorg-0.0.1/tests/test_rrule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.790639 khalorg-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.762639 khalorg-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.762639 khalorg-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-15 19:50:14.000000 khalorg-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 19:50:14.000000 khalorg-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:50:14.000000 khalorg-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-15 19:50:14.000000 khalorg-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-15 19:50:14.000000 khalorg-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 19:50:14.000000 khalorg-0.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-15 19:50:24.790639 khalorg-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-15 19:50:14.000000 khalorg-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.774639 khalorg-0.0.2/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)   474334 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   814156 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/edit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   805028 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/list.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40467 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/meeting.org
+-rw-r--r--   0 runner    (1001) docker     (127)  5848880 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/neovim-plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   330668 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/new.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.774639 khalorg-0.0.2/extras/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4045 2024-04-15 19:50:14.000000 khalorg-0.0.2/extras/calsync
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-15 19:50:14.000000 khalorg-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:50:24.790639 khalorg-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 19:50:14.000000 khalorg-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.762639 khalorg-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.774639 khalorg-0.0.2/src/khalorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/src/khalorg/khal/
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/src/khalorg/org/
+-rw-r--r--   0 runner    (1001) docker     (127)    19368 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/org/agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/org/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/rrule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/src/khalorg/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_delete_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_edit_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_list_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_new_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/khal_format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/khalorg_format.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/src/khalorg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/khalorg_tester
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.782639 khalorg-0.0.2/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/tests/static/agenda_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/all_day.org
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/all_day_until_with_time.org
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/body_first.org
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/demo.org
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/duplicate.org
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/minimal.org
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps.org
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps_unsorted.org
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/no_heading.org
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/no_time_stamp.org
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/not_first_child.org
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/not_first_heading.org
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/not_first_level.org
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/past.org
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_allday.org
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_and_non_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved.org
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved_expected.org
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_monthly.org
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_not_supported.org
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_1th.org
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_allday.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_and_non_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_duplicates.org
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_monthly.org
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_not_supported.org
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/scheduled_and_deadline.org
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/short_timestamp.org
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/timestamp_scheduled_deadline.org
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/two_items.org
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/two_timestamps.org
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/valid.org
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/valid_no_until.org
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/config_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/khalorg_format_full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_combined.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_default.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_khal
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_user.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/tests/test_khal/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/test_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/tests/test_org/
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_org/test_agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_org/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_rrule.py
```

### Comparing `khalorg-0.0.1/.github/workflows/release.yml` & `khalorg-0.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/CHANGELOG.md` & `khalorg-0.0.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/CONTRIBUTING.md` & `khalorg-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/LICENCE` & `khalorg-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/PKG-INFO` & `khalorg-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khalorg
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interface between Org mode and Khal cli calendar.
 Author: BartSte
 License: MIT License
 Keywords: khal,org mode,vdirsyncer,CalDav,agenda,emacs,neovim,orgmode-nvim
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `khalorg-0.0.1/README.md` & `khalorg-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/demo/delete.gif` & `khalorg-0.0.2/demo/delete.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/demo/edit.gif` & `khalorg-0.0.2/demo/edit.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/demo/list.gif` & `khalorg-0.0.2/demo/list.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/demo/logo.jpg` & `khalorg-0.0.2/demo/logo.jpg`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/demo/neovim-plugin.gif` & `khalorg-0.0.2/demo/neovim-plugin.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/demo/new.gif` & `khalorg-0.0.2/demo/new.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/extras/calsync` & `khalorg-0.0.2/extras/calsync`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/pyproject.toml` & `khalorg-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "khal>=0.11",
     "vdirsyncer",
     "orgparse"
 ]
-version = "0.0.1"
+version = "0.0.2"
 
 [project.optional-dependencies]
 debug = ["ipdb", "ipython"]
 test = ["pytest"]
 build = ["build", "twine"]
 
 [project.scripts]
```

### Comparing `khalorg-0.0.1/src/khalorg/cli.py` & `khalorg-0.0.2/src/khalorg/cli.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/commands.py` & `khalorg-0.0.2/src/khalorg/commands.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/helpers.py` & `khalorg-0.0.2/src/khalorg/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/khal/args.py` & `khalorg-0.0.2/src/khalorg/khal/args.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/khal/calendar.py` & `khalorg-0.0.2/src/khalorg/khal/calendar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+from os.path import dirname, join
+import sys
 from datetime import date, datetime
 from typing import Callable, Iterable, TypedDict, Union
 
 from khal.cli import build_collection
 from khal.controllers import Event
 from khal.khalendar import CalendarCollection
 from khal.khalendar.vdir import NotFoundError
@@ -80,16 +82,17 @@
 
         Args:
         ----
             name: name of the khal calendar
         """
         path_config: Union[str, None] = find_configuration_file()
 
-        new_item_args: list = ["python3", "-m", "khal", "new"]
-        list_args: list = ["python3", "-m", "khal", "list", "-df", ""]
+        khal_bin: str = join(dirname(sys.executable), 'khal')
+        new_item_args: list = [khal_bin, "new"]
+        list_args: list = [khal_bin, "list", "-df", ""]
 
         self._collection: CalendarCollection
         self._new_item: Callable = subprocess_callback(new_item_args)
         self._list_command: Callable = subprocess_callback(list_args)
 
         self.name: str = name
         self.config: dict = get_config(path_config)
```

### Comparing `khalorg-0.0.1/src/khalorg/khal/checker.py` & `khalorg-0.0.2/src/khalorg/khal/checker.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/khal/helpers.py` & `khalorg-0.0.2/src/khalorg/khal/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import sys
 from datetime import date, datetime
 from subprocess import STDOUT, CalledProcessError, check_output
 from typing import Callable
 
 from khalorg import paths
 
 Time = date | datetime
@@ -68,15 +67,15 @@
         return try_check_output([*cmd, *args]).decode()
 
     return callback
 
 
 def try_check_output(args: list) -> bytes:
     try:
-        return check_output(args, stderr=STDOUT, executable=sys.executable)
+        return check_output(args, stderr=STDOUT)
     except CalledProcessError as error:
         error_message: str = (
             f"The following arguments were sent to khal:\n\n{' '.join(args)}"
             "\n\nNext, the following error was received from khal:\n\n"
             f"{error.output.decode()}\n\n"
         )
         logging.critical(error_message)
```

### Comparing `khalorg-0.0.1/src/khalorg/org/agenda_items.py` & `khalorg-0.0.2/src/khalorg/org/agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/org/helpers.py` & `khalorg-0.0.2/src/khalorg/org/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/rrule.py` & `khalorg-0.0.2/src/khalorg/rrule.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg/static/description_list_command.txt` & `khalorg-0.0.2/src/khalorg/static/description_list_command.txt`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/src/khalorg.egg-info/PKG-INFO` & `khalorg-0.0.2/src/khalorg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khalorg
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interface between Org mode and Khal cli calendar.
 Author: BartSte
 License: MIT License
 Keywords: khal,org mode,vdirsyncer,CalDav,agenda,emacs,neovim,orgmode-nvim
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `khalorg-0.0.1/src/khalorg.egg-info/SOURCES.txt` & `khalorg-0.0.2/src/khalorg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/agenda_items.py` & `khalorg-0.0.2/tests/agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/helpers.py` & `khalorg-0.0.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/khalorg_tester` & `khalorg-0.0.2/tests/khalorg_tester`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/duplicate.org` & `khalorg-0.0.2/tests/static/agenda_items/duplicate.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps.org` & `khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/multiple_timestamps_unsorted.org` & `khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps_unsorted.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved.org` & `khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/recurring_first_item_moved_expected.org` & `khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved_expected.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/rrule_recurring.org` & `khalorg-0.0.2/tests/static/agenda_items/rrule_recurring.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_and_non_recurring.org` & `khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_and_non_recurring.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/rrule_recurring_duplicates.org` & `khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_duplicates.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/agenda_items/two_items.org` & `khalorg-0.0.2/tests/static/agenda_items/two_items.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/static/test_config_khal` & `khalorg-0.0.2/tests/static/test_config_khal`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_cli.py` & `khalorg-0.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_commands.py` & `khalorg-0.0.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_helpers.py` & `khalorg-0.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_khal/helpers.py` & `khalorg-0.0.2/tests/test_khal/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_khal/test_args.py` & `khalorg-0.0.2/tests/test_khal/test_args.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_khal/test_calendar.py` & `khalorg-0.0.2/tests/test_khal/test_calendar.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_khal/test_checker.py` & `khalorg-0.0.2/tests/test_khal/test_checker.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_org/test_agenda_items.py` & `khalorg-0.0.2/tests/test_org/test_agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_org/test_helpers.py` & `khalorg-0.0.2/tests/test_org/test_helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.1/tests/test_rrule.py` & `khalorg-0.0.2/tests/test_rrule.py`

 * *Files identical despite different names*

