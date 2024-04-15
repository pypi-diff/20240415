# Comparing `tmp/legend_daq2lh5-1.2.0a2.tar.gz` & `tmp/legend_daq2lh5-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_daq2lh5-1.2.0a2.tar", last modified: Wed Feb 28 09:55:40 2024, max compression
+gzip compressed data, was "legend_daq2lh5-1.2.1.tar", last modified: Mon Apr 15 09:03:18 2024, max compression
```

## Comparing `legend_daq2lh5-1.2.0a2.tar` & `legend_daq2lh5-1.2.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.024122 legend_daq2lh5-1.2.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-02-28 09:55:40.024122 legend_daq2lh5-1.2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-28 09:55:40.028122 legend_daq2lh5-1.2.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.012122 legend_daq2lh5-1.2.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.016122 legend_daq2lh5-1.2.0a2/src/daq2lh5/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-28 09:55:39.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.016122 legend_daq2lh5-1.2.0a2/src/daq2lh5/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/buffer_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/buffer_processor/buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/buffer_processor/lh5_buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/build_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.016122 legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/data_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14130 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/data_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.016122 legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.020122 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20867 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_digitizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    33088 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_flashcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_run_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17687 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/src/daq2lh5/raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.024122 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-02-28 09:55:39.000000 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-28 09:55:40.000000 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:55:39.000000 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-28 09:55:39.000000 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 09:55:39.000000 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-28 09:55:39.000000 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-28 09:55:39.000000 legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.020122 legend_daq2lh5-1.2.0a2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.020122 legend_daq2lh5-1.2.0a2/tests/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (127)    55148 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.020122 legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
--rw-r--r--   0 runner    (1001) docker     (127)    43754 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_lh5_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.024122 legend_daq2lh5-1.2.0a2/tests/compass/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/compass/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/compass/test_compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/compass/test_compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/compass/test_compass_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.024122 legend_daq2lh5-1.2.0a2/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/configs/fc-out-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/configs/orca-out-spec-cli.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/configs/orca-out-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.024122 legend_daq2lh5-1.2.0a2/tests/fc/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/fc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/fc/test_fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/fc/test_fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/fc/test_fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/fc/test_fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 09:55:40.024122 legend_daq2lh5-1.2.0a2/tests/orca/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/orca/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/orca/test_or_run_decoder_for_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/orca/test_orca_fc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/orca/test_orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/test_build_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/test_daq_to_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-02-28 09:55:31.000000 legend_daq2lh5-1.2.0a2/tests/test_raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.125933 legend_daq2lh5-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-15 09:03:18.125933 legend_daq2lh5-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-15 09:03:18.125933 legend_daq2lh5-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.109933 legend_daq2lh5-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/daq2lh5/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/lh5_buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/build_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/compass/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/data_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/data_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.113933 legend_daq2lh5-1.2.1/src/daq2lh5/fc/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.117933 legend_daq2lh5-1.2.1/src/daq2lh5/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20867 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33096 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_flashcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_run_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17688 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/src/daq2lh5/raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:03:17.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 09:03:18.000000 legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.117933 legend_daq2lh5-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (127)    55148 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43754 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/buffer_processor/test_lh5_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/compass/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/test_compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/test_compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/compass/test_compass_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/configs/fc-out-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/configs/orca-out-spec-cli.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/configs/orca-out-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/fc/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/fc/test_fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:03:18.121933 legend_daq2lh5-1.2.1/tests/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/test_or_run_decoder_for_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/test_orca_fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/orca/test_orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_build_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_daq_to_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-15 09:03:12.000000 legend_daq2lh5-1.2.1/tests/test_raw_buffer.py
```

### Comparing `legend_daq2lh5-1.2.0a2/LICENSE` & `legend_daq2lh5-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/PKG-INFO` & `legend_daq2lh5-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_daq2lh5
-Version: 1.2.0a2
+Version: 1.2.1
 Summary: Convert digitizer data to LH5
 Home-page: https://github.com/legend-exp/legend-daq2lh5
 Author: Jason Detwiler
 Author-email: jasondet@uw.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dspeed>=1.3.0a4
 Requires-Dist: h5py>=3.2.0
 Requires-Dist: hdf5plugin
-Requires-Dist: legend-pydataobj>=1.5.0a1
+Requires-Dist: legend-pydataobj>=1.6
 Requires-Dist: numpy>=1.21
 Requires-Dist: pyfcutils
 Requires-Dist: tqdm>=4.27
 Requires-Dist: xmltodict
 Provides-Extra: all
 Requires-Dist: legend-daq2lh5[docs,test]; extra == "all"
 Provides-Extra: docs
@@ -56,20 +56,24 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-daq2lh5?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-daq2lh5)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-daq2lh5?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-daq2lh5?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/legend-daq2lh5)
 [![Read the Docs](https://img.shields.io/readthedocs/legend-daq2lh5?logo=readthedocs)](https://legend-daq2lh5.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10721223.svg)](https://doi.org/10.5281/zenodo.10721223)
 
 JSON-configurable conversion of digitized data into
 [LEGEND HDF5](https://legend-exp.github.io/legend-data-format-specs/dev/hdf5/),
 with optional data pre-processing via [dspeed](https://dspeed.readthedocs.io)
 and data compression via [legend-pydataobj](https://legend-pydataobj.readthedocs.io).
 
 Currently supported DAQ data formats:
 * [FlashCam](https://www.mizzi-computer.de/home)
 * [CoMPASS](https://www.caen.it/products/compass)
 * [ORCA](https://github.com/unc-enap/Orca), reading out:
   - FlashCam
   - [Struck SIS3302](https://www.struck.de/sis3302.htm)
   - [Struck SIS3316](https://www.struck.de/sis3316.html)
+
+If you are using this software, consider
+[citing](https://doi.org/10.5281/zenodo.10721223)!
```

### Comparing `legend_daq2lh5-1.2.0a2/README.md` & `legend_daq2lh5-1.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-daq2lh5?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-daq2lh5)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-daq2lh5?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-daq2lh5?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/legend-daq2lh5)
 [![Read the Docs](https://img.shields.io/readthedocs/legend-daq2lh5?logo=readthedocs)](https://legend-daq2lh5.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10721223.svg)](https://doi.org/10.5281/zenodo.10721223)
 
 JSON-configurable conversion of digitized data into
 [LEGEND HDF5](https://legend-exp.github.io/legend-data-format-specs/dev/hdf5/),
 with optional data pre-processing via [dspeed](https://dspeed.readthedocs.io)
 and data compression via [legend-pydataobj](https://legend-pydataobj.readthedocs.io).
 
 Currently supported DAQ data formats:
 * [FlashCam](https://www.mizzi-computer.de/home)
 * [CoMPASS](https://www.caen.it/products/compass)
 * [ORCA](https://github.com/unc-enap/Orca), reading out:
   - FlashCam
   - [Struck SIS3302](https://www.struck.de/sis3302.htm)
   - [Struck SIS3316](https://www.struck.de/sis3316.html)
+
+If you are using this software, consider
+[citing](https://doi.org/10.5281/zenodo.10721223)!
```

### Comparing `legend_daq2lh5-1.2.0a2/setup.cfg` & `legend_daq2lh5-1.2.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 [options]
 packages = find:
 install_requires = 
 	dspeed>=1.3.0a4
 	h5py>=3.2.0
 	hdf5plugin
-	legend-pydataobj>=1.5.0a1
+	legend-pydataobj>=1.6
 	numpy>=1.21
 	pyfcutils
 	tqdm>=4.27
 	xmltodict
 python_requires = >=3.9
 include_package_data = True
 package_dir =
```

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/__init__.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/__init__.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/buffer_processor/buffer_processor.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/buffer_processor/lh5_buffer_processor.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/buffer_processor/lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/build_raw.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/build_raw.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/cli.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """legend-daq2lh5's command line interface utilities."""
+
 from __future__ import annotations
 
 import argparse
 import os
 import sys
 
 import numpy as np
```

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_config_parser.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_config_parser.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_event_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_header_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/compass/compass_streamer.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/compass/compass_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/data_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/data_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Base classes for decoding data into raw LGDO Tables or files
 """
+
 from __future__ import annotations
 
 import lgdo
 import numpy as np
 from lgdo import LGDO
 from lgdo.lh5 import LH5Store
+from lgdo.lh5 import datatype as dtypeutils
 
 
 class DataDecoder:
     r"""Decodes packets from a data stream.
 
     Most decoders will repeatedly decode the same set of values from each
     packet.  The values that get decoded need to be described by a dict stored
@@ -201,43 +203,43 @@
                                 el
                             ]
 
                 data_obj.add_field(field, wf_table)
                 continue
 
             # Parse datatype for remaining lgdos
-            datatype, shape, elements = lgdo.lh5.utils.parse_datatype(datatype)
+            lgdotype = dtypeutils.datatype(datatype)
 
             # ArrayOfEqualSizedArrays
-            if datatype == "array_of_equalsized_arrays":
+            if lgdotype is lgdo.ArrayOfEqualSizedArrays:
                 length = attrs.pop("length")
                 # only arrays of 1D arrays are supported at present
                 dims = (1, 1)
                 aoesa = lgdo.ArrayOfEqualSizedArrays(
                     shape=(size, length), dtype=dtype, dims=dims, attrs=attrs
                 )
                 data_obj.add_field(field, aoesa)
                 continue
 
             # VectorOfVectors
-            if elements.startswith("array"):
+            if lgdotype is lgdo.VectorOfVectors:
                 length_guess = size
                 if "length_guess" in attrs:
                     length_guess = attrs.pop("length_guess")
                 vov = lgdo.VectorOfVectors(
                     shape_guess=(size, length_guess), dtype=dtype, attrs=attrs
                 )
                 data_obj.add_field(field, vov)
                 continue
 
             # if we get here, got a bad datatype
             raise RuntimeError(
                 type(self).__name__,
                 ": do not know how to make a",
-                datatype,
+                lgdotype.__name__,
                 "for",
                 field,
             )
 
         return data_obj
 
     def put_in_garbage(self, packet: int, packet_id: int, code: int) -> None:
```

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/data_streamer.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/data_streamer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Base classes for streaming data.
 """
+
 from __future__ import annotations
 
 import fnmatch
 import logging
 from abc import ABC, abstractmethod
 
 from .raw_buffer import RawBuffer, RawBufferLibrary, RawBufferList
```

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_config_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_event_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_status_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/fc/fc_streamer.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/fc/fc_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/logging.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module implements some helpers for setting up logging."""
+
 import logging
 
 import colorlog
 
 DEBUG = logging.DEBUG
 INFO = logging.INFO
 WARNING = logging.WARNING
```

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_base.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_base.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_digitizers.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_digitizers.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_flashcam.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_flashcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,36 +417,36 @@
                 i_cd + 13
             ]
             for j in range(5):
                 tbl["card_n_other_errors"].flattened_data.nda[
                     (fd0 + i_card) * 5 + j
                 ] = packet[i_cd + 14 + j]
             for j in range(5):
-                tbl["card_temps"].flattened_data.nda[
-                    (fd0 + i_card) * 5 + j
-                ] = int_packet[i_cd + 19 + j]
+                tbl["card_temps"].flattened_data.nda[(fd0 + i_card) * 5 + j] = (
+                    int_packet[i_cd + 19 + j]
+                )
             for j in range(6):
-                tbl["card_voltages"].flattened_data.nda[
-                    (fd0 + i_card) * 6 + j
-                ] = int_packet[i_cd + 24 + j]
+                tbl["card_voltages"].flattened_data.nda[(fd0 + i_card) * 6 + j] = (
+                    int_packet[i_cd + 24 + j]
+                )
             tbl["card_main_current"].flattened_data.nda[fd0 + i_card] = int_packet[
                 i_cd + 30
             ]
             tbl["card_humidity"].flattened_data.nda[fd0 + i_card] = int_packet[
                 i_cd + 31
             ]
             for j in range(2):
-                tbl["card_adc_temps"].flattened_data.nda[
-                    (fd0 + i_card) * 2 + j
-                ] = int_packet[i_cd + 32 + j]
+                tbl["card_adc_temps"].flattened_data.nda[(fd0 + i_card) * 2 + j] = (
+                    int_packet[i_cd + 32 + j]
+                )
             # packet[34] is empty / dummy
             for j in range(4):
-                tbl["card_cti_links"].flattened_data.nda[
-                    (fd0 + i_card) * 4 + j
-                ] = packet[i_cd + 35 + j]
+                tbl["card_cti_links"].flattened_data.nda[(fd0 + i_card) * 4 + j] = (
+                    packet[i_cd + 35 + j]
+                )
             for j in range(256):
                 value = packet[i_cd + 39 + j] if j < n_link_states else 0
                 tbl["card_link_states"].flattened_data.nda[
                     (fd0 + i_card) * 256 + j
                 ] = value
 
         rb.loc += 1
```

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_header.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_header_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_header_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_packet.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Provides convenience functions for working with ORCA packets.
 
 An ORCA packet is represented by a one-dimensional :class:`numpy.ndarray` of
 type :class:`numpy.uint32`.
 """
+
 from __future__ import annotations
 
 import logging
 
 import numpy as np
 import numpy.typing as npt
```

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_run_decoder.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_run_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/orca/orca_streamer.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/orca/orca_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/src/daq2lh5/raw_buffer.py` & `legend_daq2lh5-1.2.1/src/daq2lh5/raw_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         "{name}" : {
           "key_list" : [ "*" ],
           "out_stream" : "$DATADIR/{file_key}_{name}.lh5"
         }
       }
     }
 """
+
 from __future__ import annotations
 
 import os
 
 import lgdo
 from lgdo import LGDO
 from lgdo.lh5 import LH5Store
```

### Comparing `legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/PKG-INFO` & `legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_daq2lh5
-Version: 1.2.0a2
+Version: 1.2.1
 Summary: Convert digitizer data to LH5
 Home-page: https://github.com/legend-exp/legend-daq2lh5
 Author: Jason Detwiler
 Author-email: jasondet@uw.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dspeed>=1.3.0a4
 Requires-Dist: h5py>=3.2.0
 Requires-Dist: hdf5plugin
-Requires-Dist: legend-pydataobj>=1.5.0a1
+Requires-Dist: legend-pydataobj>=1.6
 Requires-Dist: numpy>=1.21
 Requires-Dist: pyfcutils
 Requires-Dist: tqdm>=4.27
 Requires-Dist: xmltodict
 Provides-Extra: all
 Requires-Dist: legend-daq2lh5[docs,test]; extra == "all"
 Provides-Extra: docs
@@ -56,20 +56,24 @@
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Codecov](https://img.shields.io/codecov/c/github/legend-exp/legend-daq2lh5?logo=codecov)](https://app.codecov.io/gh/legend-exp/legend-daq2lh5)
 ![GitHub issues](https://img.shields.io/github/issues/legend-exp/legend-daq2lh5?logo=github)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/legend-exp/legend-daq2lh5?logo=github)
 ![License](https://img.shields.io/github/license/legend-exp/legend-daq2lh5)
 [![Read the Docs](https://img.shields.io/readthedocs/legend-daq2lh5?logo=readthedocs)](https://legend-daq2lh5.readthedocs.io)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10721223.svg)](https://doi.org/10.5281/zenodo.10721223)
 
 JSON-configurable conversion of digitized data into
 [LEGEND HDF5](https://legend-exp.github.io/legend-data-format-specs/dev/hdf5/),
 with optional data pre-processing via [dspeed](https://dspeed.readthedocs.io)
 and data compression via [legend-pydataobj](https://legend-pydataobj.readthedocs.io).
 
 Currently supported DAQ data formats:
 * [FlashCam](https://www.mizzi-computer.de/home)
 * [CoMPASS](https://www.caen.it/products/compass)
 * [ORCA](https://github.com/unc-enap/Orca), reading out:
   - FlashCam
   - [Struck SIS3302](https://www.struck.de/sis3302.htm)
   - [Struck SIS3316](https://www.struck.de/sis3316.html)
+
+If you are using this software, consider
+[citing](https://doi.org/10.5281/zenodo.10721223)!
```

### Comparing `legend_daq2lh5-1.2.0a2/src/legend_daq2lh5.egg-info/SOURCES.txt` & `legend_daq2lh5-1.2.1/src/legend_daq2lh5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor.py` & `legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json` & `legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json` & `legend_daq2lh5-1.2.1/tests/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/buffer_processor/test_lh5_buffer_processor.py` & `legend_daq2lh5-1.2.1/tests/buffer_processor/test_lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/compass/conftest.py` & `legend_daq2lh5-1.2.1/tests/compass/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/compass/test_compass_event_decoder.py` & `legend_daq2lh5-1.2.1/tests/compass/test_compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/compass/test_compass_header_decoder.py` & `legend_daq2lh5-1.2.1/tests/compass/test_compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/compass/test_compass_streamer.py` & `legend_daq2lh5-1.2.1/tests/compass/test_compass_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/conftest.py` & `legend_daq2lh5-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/fc/test_fc_config_decoder.py` & `legend_daq2lh5-1.2.1/tests/fc/test_fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/fc/test_fc_event_decoder.py` & `legend_daq2lh5-1.2.1/tests/fc/test_fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/fc/test_fc_status_decoder.py` & `legend_daq2lh5-1.2.1/tests/fc/test_fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/fc/test_fc_streamer.py` & `legend_daq2lh5-1.2.1/tests/fc/test_fc_streamer.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/orca/test_or_run_decoder_for_run.py` & `legend_daq2lh5-1.2.1/tests/orca/test_or_run_decoder_for_run.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/orca/test_orca_fc.py` & `legend_daq2lh5-1.2.1/tests/orca/test_orca_fc.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/orca/test_orca_packet.py` & `legend_daq2lh5-1.2.1/tests/orca/test_orca_packet.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/test_build_raw.py` & `legend_daq2lh5-1.2.1/tests/test_build_raw.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/test_cli.py` & `legend_daq2lh5-1.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/test_daq_to_raw.py` & `legend_daq2lh5-1.2.1/tests/test_daq_to_raw.py`

 * *Files identical despite different names*

### Comparing `legend_daq2lh5-1.2.0a2/tests/test_raw_buffer.py` & `legend_daq2lh5-1.2.1/tests/test_raw_buffer.py`

 * *Files identical despite different names*

