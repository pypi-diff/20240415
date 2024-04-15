# Comparing `tmp/ocdskit-1.1.8.tar.gz` & `tmp/ocdskit-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdskit-1.1.8.tar", last modified: Mon Jun 26 20:40:52 2023, max compression
+gzip compressed data, was "ocdskit-1.1.9.tar", last modified: Fri Jan  5 17:25:28 2024, max compression
```

## Comparing `ocdskit-1.1.8.tar` & `ocdskit-1.1.9.tar`

### file list

```diff
@@ -1,208 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.717928 ocdskit-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-26 20:40:43.000000 ocdskit-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 20:40:43.000000 ocdskit-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-26 20:40:52.717928 ocdskit-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-26 20:40:43.000000 ocdskit-1.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/combine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/mapping_sheet.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/packager.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/upgrade.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/ocds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli/schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 20:40:43.000000 ocdskit-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.685927 ocdskit-1.1.8/ocdskit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.689928 ocdskit-1.1.8/ocdskit/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/combine_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/combine_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/mapping_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/package_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/package_releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/schema_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/schema_strict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/set_closed_codelist_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/split_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/split_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/mapping_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/packager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-06-26 20:40:43.000000 ocdskit-1.1.8/ocdskit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.689928 ocdskit-1.1.8/ocdskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 20:40:52.000000 ocdskit-1.1.8/ocdskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 20:40:43.000000 ocdskit-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 20:40:52.717928 ocdskit-1.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.689928 ocdskit-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.693928 ocdskit-1.1.8/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)   109677 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/cassettes/test_combine-test_merge_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  3538926 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/cassettes/test_combine-test_merge_with_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    81406 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/cassettes/test_packager-test_output_package_no_streaming.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.697928 ocdskit-1.1.8/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.701928 ocdskit-1.1.8/tests/commands/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)   108359 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_extensions_with_releases[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)    81764 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package_packages[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)   110211 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_package_uri_published_date_version[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_compile-test_command_unknown_version[True].yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_language.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_no_inherit_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_array.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_location.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_combine_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_combine_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_mapping_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_package_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_package_releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_schema_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_schema_strict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_set_closed_codelist_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_split_record_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_split_release_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/commands/test_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.713928 ocdskit-1.1.8/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.713928 ocdskit-1.1.8/tests/fixtures/bods/
--rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/bods/components.json
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/bods/person-statement.json
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-record-packages_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/combine-release-packages_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/compile_extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/compile_no-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/compile_warning.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_false.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_mixed.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_null.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_number.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_true.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/detect-format_whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/encoding_ascii.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/encoding_utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)   164096 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_bods.csv
--rw-r--r--   0 runner    (1001) docker     (123)   165693 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_codelist.csv
--rw-r--r--   0 runner    (1001) docker     (123)   164755 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension-field.csv
--rw-r--r--   0 runner    (1001) docker     (123)   173802 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension.csv
--rw-r--r--   0 runner    (1001) docker     (123)   174656 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170180 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_array.csv
--rw-r--r--   0 runner    (1001) docker     (123)   177039 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_language.csv
--rw-r--r--   0 runner    (1001) docker     (123)   177811 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_location.csv
--rw-r--r--   0 runner    (1001) docker     (123)   174640 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv
--rw-r--r--   0 runner    (1001) docker     (123)    95829 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_no-deprecated.csv
--rw-r--r--   0 runner    (1001) docker     (123)    67545 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_oc4ids.csv
--rw-r--r--   0 runner    (1001) docker     (123)   164096 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_order-by.csv
--rw-r--r--   0 runner    (1001) docker     (123)    67509 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/mapping-sheet_sedl.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/ocds-sample-data.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)    56591 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/project-schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:40:52.717928 ocdskit-1.1.8/tests/fixtures/realdata/
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/compile_encoding_encoding.json
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18778 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_linked-releases.json
--rw-r--r--   0 runner    (1001) docker     (123)    54140 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_package.json
--rw-r--r--   0 runner    (1001) docker     (123)    55971 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_package_1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_record-package.json
--rw-r--r--   0 runner    (1001) docker     (123)    54149 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_split.json
--rw-r--r--   0 runner    (1001) docker     (123)   111387 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/record-package_versioned.json
--rw-r--r--   0 runner    (1001) docker     (123)    36724 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    20515 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_record-package.json
--rw-r--r--   0 runner    (1001) docker     (123)    36542 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/release-package_split.json
--rw-r--r--   0 runner    (1001) docker     (123)    38730 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_maximal.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-1-2-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-1-2-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record-package_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record_minimal-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record_minimal-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/record_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_additional-contact-points.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_maximal.json
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-1-2-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-1-2-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-1-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal-no-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_unknown-version.json
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_url-error.json
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_url-timeout.json
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_urls.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-package_warning.json
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-packages.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-packages.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    88734 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/release_minimal_pretty.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/schema-strict.json
--rw-r--r--   0 runner    (1001) docker     (123)    62362 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/sedl-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/fixtures/test-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/test_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-26 20:40:43.000000 ocdskit-1.1.8/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.054663 ocdskit-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-05 17:25:20.000000 ocdskit-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-05 17:25:20.000000 ocdskit-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-01-05 17:25:28.054663 ocdskit-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-01-05 17:25:20.000000 ocdskit-1.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.022662 ocdskit-1.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.026662 ocdskit-1.1.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/combine.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/mapping_sheet.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/packager.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/upgrade.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.026662 ocdskit-1.1.9/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/cli/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/cli/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/cli/ocds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/cli/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-05 17:25:20.000000 ocdskit-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.026662 ocdskit-1.1.9/ocdskit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.030663 ocdskit-1.1.9/ocdskit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/combine_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/combine_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/indent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/mapping_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/package_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/package_releases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/schema_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/schema_strict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/set_closed_codelist_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/split_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/split_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8991 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/mapping_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-01-05 17:25:20.000000 ocdskit-1.1.9/ocdskit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.054663 ocdskit-1.1.9/ocdskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-01-05 17:25:27.000000 ocdskit-1.1.9/ocdskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-01-05 17:25:28.000000 ocdskit-1.1.9/ocdskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 17:25:27.000000 ocdskit-1.1.9/ocdskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-05 17:25:27.000000 ocdskit-1.1.9/ocdskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-05 17:25:27.000000 ocdskit-1.1.9/ocdskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-05 17:25:27.000000 ocdskit-1.1.9/ocdskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-05 17:25:20.000000 ocdskit-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-05 17:25:28.054663 ocdskit-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.030663 ocdskit-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.034663 ocdskit-1.1.9/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_combine_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_combine_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_indent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_mapping_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_package_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_package_releases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_schema_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_schema_strict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_set_closed_codelist_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_split_record_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_split_release_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/commands/test_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.050663 ocdskit-1.1.9/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.050663 ocdskit-1.1.9/tests/fixtures/bods/
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/bods/components.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/bods/person-statement.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/combine-record-packages_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/combine-release-packages_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/compile_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/compile_no-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/compile_warning.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_array.json
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_false.json
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_mixed.json
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_null.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_number.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_object.json
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_true.json
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/detect-format_whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/encoding_ascii.json
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/encoding_utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (127)   164096 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14709 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_bods.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   165693 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_codelist.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   164755 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension-field.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   173802 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   174656 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   170180 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_array.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   177039 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_language.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   177811 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_location.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   174640 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    95829 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_no-deprecated.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    67545 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_oc4ids.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   164096 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_order-by.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    67509 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/mapping-sheet_sedl.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/ocds-sample-data.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/project-schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 17:25:28.054663 ocdskit-1.1.9/tests/fixtures/realdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/compile_encoding_encoding.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/compiled-release-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/compiled-release-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18778 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_linked-releases.json
+-rw-r--r--   0 runner    (1001) docker     (127)    54140 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_package.json
+-rw-r--r--   0 runner    (1001) docker     (127)    55971 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_package_1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_record-package.json
+-rw-r--r--   0 runner    (1001) docker     (127)    54149 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_split.json
+-rw-r--r--   0 runner    (1001) docker     (127)   111387 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/record-package_versioned.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36724 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24612 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.0-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.0-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.1-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.1-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20609 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_encoding-utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_record-package.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36542 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/release-package_split.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38730 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/versioned-release-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/realdata/versioned-release-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record-package_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record-package_maximal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record-package_minimal-1-2-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record-package_minimal-1-2-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record-package_minimal-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record-package_minimal-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record-package_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record_minimal-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record_minimal-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/record_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_additional-contact-points.json
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_maximal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_minimal-1-2-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_minimal-1-2-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_minimal-1-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_minimal-no-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_unknown-version.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_url-error.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_url-timeout.json
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_urls.json
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-package_warning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-packages.json
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-packages.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    88734 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release_1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release_1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release_minimal-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release_minimal-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/release_minimal_pretty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/schema-strict.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62362 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/sedl-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/fixtures/test-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/test_packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-01-05 17:25:20.000000 ocdskit-1.1.9/tests/test_util.py
```

### Comparing `ocdskit-1.1.8/LICENSE` & `ocdskit-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/PKG-INFO` & `ocdskit-1.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 Metadata-Version: 2.1
 Name: ocdskit
-Version: 1.1.8
+Version: 1.1.9
 Summary: A suite of command-line tools for working with OCDS data
 Home-page: https://github.com/open-contracting/ocdskit
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: ijson>=2.5
+Requires-Dist: jsonref
+Requires-Dist: ocdsmerge>=0.6
+Requires-Dist: ocdsextensionregistry>=0.1.2
 Provides-Extra: perf
+Requires-Dist: orjson>=3; extra == "perf"
 Provides-Extra: test
+Requires-Dist: coveralls; extra == "test"
+Requires-Dist: jsonpointer; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
 
 |PyPI Version| |Build Status| |Coverage Status| |Python Version|
 
 A suite of command-line tools for working with OCDS data to:
 
 * create compiled releases, versioned releases and record packages
 * upgrade from an old version of OCDS to a new version
@@ -37,13 +49,13 @@
 
    Want to `download OCDS data <https://data.open-contracting.org/>`__? Use the `OCP Data Registry <https://data.open-contracting.org/>`__.
 
 If you are viewing this on GitHub or PyPI, open the `full documentation <https://ocdskit.readthedocs.io/>`__ for additional details.
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdskit.svg
    :target: https://pypi.org/project/ocdskit/
-.. |Build Status| image:: https://github.com/open-contracting/ocdskit/workflows/CI/badge.svg
-   :target: https://github.com/open-contracting/ocdskit/actions?query=workflow%3ACI
+.. |Build Status| image:: https://github.com/open-contracting/ocdskit/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/open-contracting/ocdskit/actions/workflows/ci.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocdskit/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/ocdskit?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdskit.svg
    :target: https://pypi.org/project/ocdskit/
```

### Comparing `ocdskit-1.1.8/README.rst` & `ocdskit-1.1.9/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
    Want to `download OCDS data <https://data.open-contracting.org/>`__? Use the `OCP Data Registry <https://data.open-contracting.org/>`__.
 
 If you are viewing this on GitHub or PyPI, open the `full documentation <https://ocdskit.readthedocs.io/>`__ for additional details.
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdskit.svg
    :target: https://pypi.org/project/ocdskit/
-.. |Build Status| image:: https://github.com/open-contracting/ocdskit/workflows/CI/badge.svg
-   :target: https://github.com/open-contracting/ocdskit/actions?query=workflow%3ACI
+.. |Build Status| image:: https://github.com/open-contracting/ocdskit/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/open-contracting/ocdskit/actions/workflows/ci.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocdskit/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/ocdskit?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdskit.svg
    :target: https://pypi.org/project/ocdskit/
```

### Comparing `ocdskit-1.1.8/docs/Makefile` & `ocdskit-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/docs/changelog.rst` & `ocdskit-1.1.9/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.1.9 (2024-01-05)
+------------------
+
+Added
+~~~~~
+
+-  :meth:`ocdskit.util.is_linked_release` accepts a ``maximum_properties`` argument (default 3).
+
 1.1.8 (2023-06-26)
 ------------------
 
 Changed
 ~~~~~~~
 
 -  :ref:`schema-strict`: Add ``minItems`` last, to match existing schema.
```

### Comparing `ocdskit-1.1.8/docs/cli/examples.rst` & `ocdskit-1.1.9/docs/cli/examples.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/docs/cli/ocds.rst` & `ocdskit-1.1.9/docs/cli/ocds.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/docs/cli/schema.rst` & `ocdskit-1.1.9/docs/cli/schema.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/docs/cli.rst` & `ocdskit-1.1.9/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/docs/conf.py` & `ocdskit-1.1.9/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Kit"
 copyright = "2017, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "1.1.8"
+version = "1.1.9"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdskit-1.1.8/docs/contributing.rst` & `ocdskit-1.1.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/docs/index.rst` & `ocdskit-1.1.9/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 .. code-block:: bash
 
     pip install ocdskit
 
 To improve performance, install as ``pip install ocdskit[perf]``, unless you are using `PyPy <https://www.pypy.org>`__.
 
-OCDS Kit requires Python 3.7 or greater. Users with Python 2 as their default Python interpreter must either run ``pip3 install ocdskit``, set up a Python 3 virtual environment, or `use OCDS Kit within a Docker container <https://hub.docker.com/r/ricardoe/ocdskit/>`__.
+OCDS Kit requires a `supported version <https://endoflife.date/python>`__ of Python 3. Users with Python 2 as their default Python interpreter must either run ``pip3 install ocdskit``, set up a Python 3 virtual environment, or `use OCDS Kit within a Docker container <https://hub.docker.com/r/ricardoe/ocdskit/>`__.
 
 OCDS Kit can be used either via its :doc:`command-line interface <cli>` or as a :doc:`Python library <library>`.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents
```

### Comparing `ocdskit-1.1.8/docs/library.rst` & `ocdskit-1.1.9/docs/library.rst`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/__main__.py` & `ocdskit-1.1.9/ocdskit/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/combine.py` & `ocdskit-1.1.9/ocdskit/combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 
 from ocdsextensionregistry import ProfileBuilder
 from ocdsmerge import Merger
 from ocdsmerge.util import get_release_schema_url
 
 from ocdskit.exceptions import MissingRecordsWarning, MissingReleasesWarning
 from ocdskit.packager import Packager
-from ocdskit.util import (_empty_record_package, _empty_release_package, _remove_empty_optional_metadata,
-                          _resolve_metadata, _update_package_metadata, get_ocds_patch_tag)
+from ocdskit.util import (
+    _empty_record_package,
+    _empty_release_package,
+    _remove_empty_optional_metadata,
+    _resolve_metadata,
+    _update_package_metadata,
+    get_ocds_patch_tag,
+)
 
 DEFAULT_VERSION = '1.1'  # fields might be deprecated
 
 
 def _package(key, items, uri, publisher, published_date, version, extensions=None):
     if publisher is None:
         publisher = {}
```

### Comparing `ocdskit-1.1.8/ocdskit/commands/base.py` & `ocdskit-1.1.9/ocdskit/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,15 @@
 
     def items(self, **kwargs):
         """
         Yields the items in the input. If an item is an array, yields each entry of the array.
         """
         for item in super().items(**kwargs):
             if isinstance(item, list):
-                for i in item:
-                    yield i
+                yield from item
             else:
                 yield item
 
     def add_package_arguments(self, infix, prefix='', version='1.1'):
         """
         Adds arguments for setting package metadata to the subparser.
         """
```

### Comparing `ocdskit-1.1.8/ocdskit/commands/combine_record_packages.py` & `ocdskit-1.1.9/ocdskit/commands/combine_record_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/combine_release_packages.py` & `ocdskit-1.1.9/ocdskit/commands/combine_release_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/compile.py` & `ocdskit-1.1.9/ocdskit/commands/compile.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/detect_format.py` & `ocdskit-1.1.9/ocdskit/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/indent.py` & `ocdskit-1.1.9/ocdskit/commands/indent.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/mapping_sheet.py` & `ocdskit-1.1.9/ocdskit/commands/mapping_sheet.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/package_records.py` & `ocdskit-1.1.9/ocdskit/commands/package_records.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/package_releases.py` & `ocdskit-1.1.9/ocdskit/commands/package_releases.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/schema_report.py` & `ocdskit-1.1.9/ocdskit/commands/schema_report.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/schema_strict.py` & `ocdskit-1.1.9/ocdskit/commands/schema_strict.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/set_closed_codelist_enums.py` & `ocdskit-1.1.9/ocdskit/commands/set_closed_codelist_enums.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/split_record_packages.py` & `ocdskit-1.1.9/ocdskit/commands/split_record_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/split_release_packages.py` & `ocdskit-1.1.9/ocdskit/commands/split_release_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/commands/upgrade.py` & `ocdskit-1.1.9/ocdskit/commands/upgrade.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import OrderedDict
+from collections import OrderedDict  # for move_to_end()
 
 from ocdskit import upgrade
 from ocdskit.commands.base import OCDSCommand
 from ocdskit.exceptions import CommandError
 
 
 class Command(OCDSCommand):
```

### Comparing `ocdskit-1.1.8/ocdskit/exceptions.py` & `ocdskit-1.1.9/ocdskit/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/mapping_sheet.py` & `ocdskit-1.1.9/ocdskit/mapping_sheet.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/packager.py` & `ocdskit-1.1.9/ocdskit/packager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 import os
 import warnings
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from tempfile import NamedTemporaryFile
 
 from ocdskit.exceptions import InconsistentVersionError, MissingOcidKeyError
-from ocdskit.util import (_empty_record_package, _remove_empty_optional_metadata, _resolve_metadata,
-                          _update_package_metadata, get_ocds_minor_version, is_release, json_dumps, jsonlib)
+from ocdskit.util import (
+    _empty_record_package,
+    _remove_empty_optional_metadata,
+    _resolve_metadata,
+    _update_package_metadata,
+    get_ocds_minor_version,
+    is_release,
+    json_dumps,
+    jsonlib,
+)
 
 try:
     import sqlite3
 
     USING_SQLITE = True
 
     def adapt_json(data):
@@ -36,14 +44,15 @@
 
 class Packager:
     """
     The Packager context manager helps to build a single record package, or a stream of compiled releases or merged
     releases. Release packages and/or individual releases can be added to the packager. All releases should use the
     same version of OCDS.
     """
+
     def __init__(self):
         self.package = _empty_record_package()
         self.version = None
 
         if USING_SQLITE:
             self.backend = SQLiteBackend()
         else:
@@ -252,14 +261,13 @@
 
         self.buffer = []
 
     def get_releases_by_ocid(self):
         self.connection.execute("CREATE INDEX IF NOT EXISTS ocid_idx ON releases(ocid)")
 
         results = self.connection.execute("SELECT * FROM releases ORDER BY ocid")
-        for ocid, rows in itertools.groupby(results, lambda row: row[0]):
-            yield ocid, rows
+        yield from itertools.groupby(results, lambda row: row[0])
 
     def close(self):
         self.file.close()
         self.connection.close()
         os.unlink(self.file.name)
```

### Comparing `ocdskit-1.1.8/ocdskit/schema.py` & `ocdskit-1.1.9/ocdskit/schema.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/ocdskit/upgrade.py` & `ocdskit-1.1.9/ocdskit/upgrade.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import json
 import logging
-from collections import OrderedDict
+from collections import OrderedDict  # for move_to_end()
 from copy import deepcopy
 from hashlib import md5
 
-from ocdskit.util import (_cast_as_list, get_ocds_minor_version, is_package, is_record, is_record_package,
-                          is_release_package)
+from ocdskit.util import (
+    _cast_as_list,
+    get_ocds_minor_version,
+    is_package,
+    is_record,
+    is_record_package,
+    is_release_package,
+)
 
 logger = logging.getLogger('ocdskit')
 
 # See https://standard.open-contracting.org/1.0/en/schema/reference/#identifier
 organization_identification_1_0 = (
     (None, ('name',)),
     ('identifier', ('scheme', 'id', 'legalName', 'uri')),
```

### Comparing `ocdskit-1.1.8/ocdskit/util.py` & `ocdskit-1.1.9/ocdskit/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,25 +183,25 @@
 def is_compiled_release(data):
     """
     Returns whether the data is a compiled release (embedded or linked).
     """
     return 'tag' in data and isinstance(data['tag'], list) and 'compiled' in data['tag']
 
 
-def is_linked_release(data):
+def is_linked_release(data, maximum_properties=3):
     """
     Returns whether the data is a linked release.
 
     A linked release has required ``url`` and ``date`` fields and an optional ``tag`` field. An embedded release has
     required ``date`` and ``tag`` fields (among others), and it can have a ``url`` field as an additional field.
 
     To distinguish a linked release from an embedded release, we test for the presence of the required ``url`` field
     and test whether the number of fields is fewer than three.
     """
-    return 'url' in data and len(data) <= 3
+    return 'url' in data and len(data) <= maximum_properties
 
 
 def detect_format(path, root_path='', reader=open):
     """
     Returns the format of OCDS data, and whether the OCDS data is concatenated or in an array.
 
     If the OCDS data is concatenated or in an array, assumes that all items have the same format as the first item.
```

### Comparing `ocdskit-1.1.8/ocdskit.egg-info/PKG-INFO` & `ocdskit-1.1.9/ocdskit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 Metadata-Version: 2.1
 Name: ocdskit
-Version: 1.1.8
+Version: 1.1.9
 Summary: A suite of command-line tools for working with OCDS data
 Home-page: https://github.com/open-contracting/ocdskit
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: ijson>=2.5
+Requires-Dist: jsonref
+Requires-Dist: ocdsmerge>=0.6
+Requires-Dist: ocdsextensionregistry>=0.1.2
 Provides-Extra: perf
+Requires-Dist: orjson>=3; extra == "perf"
 Provides-Extra: test
+Requires-Dist: coveralls; extra == "test"
+Requires-Dist: jsonpointer; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: furo; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
 
 |PyPI Version| |Build Status| |Coverage Status| |Python Version|
 
 A suite of command-line tools for working with OCDS data to:
 
 * create compiled releases, versioned releases and record packages
 * upgrade from an old version of OCDS to a new version
@@ -37,13 +49,13 @@
 
    Want to `download OCDS data <https://data.open-contracting.org/>`__? Use the `OCP Data Registry <https://data.open-contracting.org/>`__.
 
 If you are viewing this on GitHub or PyPI, open the `full documentation <https://ocdskit.readthedocs.io/>`__ for additional details.
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/ocdskit.svg
    :target: https://pypi.org/project/ocdskit/
-.. |Build Status| image:: https://github.com/open-contracting/ocdskit/workflows/CI/badge.svg
-   :target: https://github.com/open-contracting/ocdskit/actions?query=workflow%3ACI
+.. |Build Status| image:: https://github.com/open-contracting/ocdskit/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/open-contracting/ocdskit/actions/workflows/ci.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/ocdskit/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/ocdskit?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdskit.svg
    :target: https://pypi.org/project/ocdskit/
```

### Comparing `ocdskit-1.1.8/ocdskit.egg-info/SOURCES.txt` & `ocdskit-1.1.9/ocdskit.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -56,17 +56,14 @@
 ocdskit/commands/split_release_packages.py
 ocdskit/commands/upgrade.py
 tests/__init__.py
 tests/conftest.py
 tests/test_combine.py
 tests/test_packager.py
 tests/test_util.py
-tests/cassettes/test_combine-test_merge_empty.yaml
-tests/cassettes/test_combine-test_merge_with_schema.yaml
-tests/cassettes/test_packager-test_output_package_no_streaming.yaml
 tests/commands/__init__.py
 tests/commands/test_combine_record_packages.py
 tests/commands/test_combine_release_packages.py
 tests/commands/test_compile.py
 tests/commands/test_detect_format.py
 tests/commands/test_echo.py
 tests/commands/test_indent.py
@@ -75,27 +72,14 @@
 tests/commands/test_package_releases.py
 tests/commands/test_schema_report.py
 tests/commands/test_schema_strict.py
 tests/commands/test_set_closed_codelist_enums.py
 tests/commands/test_split_record_packages.py
 tests/commands/test_split_release_packages.py
 tests/commands/test_upgrade.py
-tests/commands/cassettes/test_compile-test_command[True].yaml
-tests/commands/cassettes/test_compile-test_command_extensions_with_releases[True].yaml
-tests/commands/cassettes/test_compile-test_command_package[True].yaml
-tests/commands/cassettes/test_compile-test_command_package_packages[True].yaml
-tests/commands/cassettes/test_compile-test_command_package_uri_published_date_version[True].yaml
-tests/commands/cassettes/test_compile-test_command_unknown_version[True].yaml
-tests/commands/cassettes/test_mapping_sheet-test_command_extension.yaml
-tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field.yaml
-tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_alternative.yaml
-tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_language.yaml
-tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_and_no_inherit_extension.yaml
-tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_array.yaml
-tests/commands/cassettes/test_mapping_sheet-test_command_extension_and_extension_field_location.yaml
 tests/fixtures/combine-record-packages_minimal-maximal-extensions.json
 tests/fixtures/combine-record-packages_minimal.json
 tests/fixtures/combine-release-packages_minimal-maximal-extensions.json
 tests/fixtures/combine-release-packages_minimal.json
 tests/fixtures/compile_extensions.json
 tests/fixtures/compile_no-extensions.json
 tests/fixtures/compile_warning.json
```

### Comparing `ocdskit-1.1.8/setup.cfg` & `ocdskit-1.1.9/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = ocdskit
-version = 1.1.8
+version = 1.1.9
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = A suite of command-line tools for working with OCDS data
 url = https://github.com/open-contracting/ocdskit
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 install_requires = 
 	ijson>=2.5
@@ -40,15 +40,14 @@
 perf = 
 	orjson>=3
 test = 
 	coveralls
 	jsonpointer
 	pytest
 	pytest-cov
-	pytest-vcr
 docs = 
 	furo
 	sphinx
 	sphinx-autobuild
 
 [egg_info]
 tag_build =
```

### Comparing `ocdskit-1.1.8/tests/__init__.py` & `ocdskit-1.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_combine_record_packages.py` & `ocdskit-1.1.9/tests/commands/test_combine_record_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_combine_release_packages.py` & `ocdskit-1.1.9/tests/commands/test_combine_release_packages.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_compile.py` & `ocdskit-1.1.9/tests/commands/test_compile.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,174 +25,158 @@
 
     args[args.index('compile') + 1:0] = ['--root-path', 'releases.item']
     if remove_package_metadata:
         expected = _remove_package_metadata(expected)
     assert_streaming(capsys, monkeypatch, main, args, stdin, expected)
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command(capsys, monkeypatch):
     assert_compile_command(capsys, monkeypatch, main, ['--ascii', 'compile'],
                            ['realdata/release-package-1.json', 'realdata/release-package-2.json'],
                            ['realdata/compiled-release-1.json', 'realdata/compiled-release-2.json'])
 
 
 @pytest.mark.usefixtures('sqlite')
 def test_command_extensions_with_packages(capsys, monkeypatch):
     assert_streaming(capsys, monkeypatch, main, ['compile'],
                      ['release-package_additional-contact-points.json'], ['compile_extensions.json'])
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_extensions_with_releases(capsys, monkeypatch):
     assert_streaming(capsys, monkeypatch, main, ['compile', '--root-path', 'releases.item'],
                      ['release-package_additional-contact-points.json'], ['compile_no-extensions.json'])
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_versioned(capsys, monkeypatch):
     assert_compile_command(capsys, monkeypatch, main, ['--ascii', 'compile', '--versioned'],
                            ['realdata/release-package-1.json', 'realdata/release-package-2.json'],
                            ['realdata/versioned-release-1.json', 'realdata/versioned-release-2.json'])
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package(capsys, monkeypatch):
     assert_compile_command(capsys, monkeypatch, main, ['compile', '--package'],
                            ['realdata/release-package-1.json', 'realdata/release-package-2.json'],
                            ['realdata/record-package_package.json'], remove_package_metadata=True)
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package_uri_published_date_version(capsys, monkeypatch):
     actual = run_streaming(capsys, monkeypatch, main, ['compile', '--package', '--uri', 'http://example.com/x.json',
                                                        '--published-date', '2010-01-01T00:00:00Z', '--version', 'X'],
                            ['release-package_minimal.json'])
 
     package = json.loads(actual.out)
     assert package['uri'] == 'http://example.com/x.json'
     assert package['publishedDate'] == '2010-01-01T00:00:00Z'
     assert package['version'] == 'X'
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package_publisher(capsys, monkeypatch):
     actual = run_streaming(capsys, monkeypatch, main, ['compile', '--package', '--publisher-name', 'Acme Inc.',
                                                        '--publisher-uri', 'http://example.com/', '--publisher-scheme',
                                                        'scheme', '--publisher-uid', '12345'],
                            ['release-package_minimal.json'])
 
     package = json.loads(actual.out)
     assert package['publisher']['name'] == 'Acme Inc.'
     assert package['publisher']['uri'] == 'http://example.com/'
     assert package['publisher']['scheme'] == 'scheme'
     assert package['publisher']['uid'] == '12345'
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package_fake(capsys, monkeypatch):
     actual = run_streaming(capsys, monkeypatch, main, ['compile', '--package', '--fake'],
                            ['release-package_minimal.json'])
 
     package = json.loads(actual.out)
     assert package['uri'] == 'placeholder:'
     assert package['publishedDate'] == '9999-01-01T00:00:00Z'
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package_packages(capsys, monkeypatch):
     actual = run_streaming(capsys, monkeypatch, main, ['compile', '--package'],
                            ['release_minimal.json'])
 
     package = json.loads(actual.out)
     assert 'packages' not in package
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_warning(capsys, monkeypatch, caplog):
     actual = run_streaming(capsys, monkeypatch, main, ['compile'],
                            ['release-package_warning.json'])
 
     assert actual.out == read('compile_warning.json')
     assert actual.err == "ocds-213czf-1: Multiple objects have the `id` value '1' in the `parties` array\n"
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package_linked_releases_with_packages(capsys, monkeypatch):
     assert_streaming(capsys, monkeypatch, main, ['compile', '--package', '--linked-releases'],
                      ['realdata/release-package-1.json', 'realdata/release-package-2.json'],
                      ['realdata/record-package_linked-releases.json'])
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package_linked_releases_with_releases(capsys, monkeypatch):
     assert_streaming(capsys, monkeypatch, main, ['compile', '--package', '--linked-releases', '--root-path',
                                                  'releases.item'],
                      ['realdata/release-package-1.json', 'realdata/release-package-2.json'],
                      _remove_package_metadata(['realdata/record-package_package.json']))
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_package_versioned(capsys, monkeypatch):
     assert_compile_command(capsys, monkeypatch, main, ['compile', '--package', '--versioned'],
                            ['realdata/release-package-1.json', 'realdata/release-package-2.json'],
                            ['realdata/record-package_versioned.json'], remove_package_metadata=True)
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_version_mismatch(capsys, monkeypatch, caplog):
     with caplog.at_level(logging.ERROR):
         assert_streaming_error(capsys, monkeypatch, main, ['compile', '--package', '--versioned'],
                                ['realdata/release-package_1.1-1.json', 'realdata/release-package_1.0-1.json'])
 
         assert len(caplog.records) == 1
         assert caplog.records[0].levelname == 'CRITICAL'
         assert caplog.records[0].message == "item 1: version error: this item uses version 1.0, but earlier items " \
             "used version 1.1\nTry first upgrading items to the same version:\n  cat file [file ...] | ocdskit " \
             "upgrade 1.0:1.1 | ocdskit compile --package --versioned"
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_missing_ocid(capsys, monkeypatch, caplog):
     stdin = b'{"id":"1","date":"2001-02-03T04:05:06Z","tag":["planning"],"initiationType":"tender"}'
 
     with caplog.at_level(logging.ERROR):
         assert_streaming_error(capsys, monkeypatch, main, ['compile'], stdin)
 
         assert len(caplog.records) == 1
         assert caplog.records[0].levelname == 'CRITICAL'
         assert caplog.records[0].message == 'The `ocid` field of at least one release is missing.'
 
 
-@pytest.mark.vcr()
 @pytest.mark.usefixtures('sqlite')
 def test_command_unknown_version(capsys, monkeypatch, caplog):
     with caplog.at_level(logging.ERROR):
         assert_streaming_error(capsys, monkeypatch, main, ['compile'], ['release-package_unknown-version.json'])
 
         assert len(caplog.records) == 1
         assert caplog.records[0].levelname == 'CRITICAL'
         assert caplog.records[0].message == 'The `version` value ("X") of a release package is not recognized.'
 
 
-@pytest.mark.vcr()
 def test_command_without_sqlite(capsys, monkeypatch, caplog):
     ocdskit.combine.sqlite = False
 
     # To check the warning, not the output.
     run_streaming(capsys, monkeypatch, main, ['compile'], ['release-package_minimal.json'])
 
     assert len(caplog.records) == 1
```

### Comparing `ocdskit-1.1.8/tests/commands/test_detect_format.py` & `ocdskit-1.1.9/tests/commands/test_detect_format.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_echo.py` & `ocdskit-1.1.9/tests/commands/test_echo.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_indent.py` & `ocdskit-1.1.9/tests/commands/test_indent.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_mapping_sheet.py` & `ocdskit-1.1.9/tests/commands/test_mapping_sheet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import platform
+
 import pytest
 
 from ocdskit.__main__ import main
 from tests import assert_command, assert_command_error, path
 
 
 def test_command(capsys, monkeypatch):
@@ -24,15 +26,14 @@
 
 def test_command_order_by(capsys, monkeypatch):
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--order-by', 'path', path('release-schema.json')],
                    'mapping-sheet_order-by.csv')
 
 
-@pytest.mark.vcr()
 def test_command_extension(capsys, monkeypatch):
     url = 'https://github.com/open-contracting-extensions/ocds_lots_extension/archive/v1.1.4.zip'
 
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', path('release-schema.json'), '--extension', url],
                    'mapping-sheet_extension.csv')
 
@@ -40,65 +41,63 @@
 def test_command_extension_field(capsys, monkeypatch):
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--extension-field', 'extension',
                     path('release-schema.json')],
                    'mapping-sheet_extension-field.csv')
 
 
-@pytest.mark.vcr()
 def test_command_extension_and_extension_field(capsys, monkeypatch):
     url = 'https://github.com/open-contracting-extensions/ocds_lots_extension/archive/v1.1.4.zip'
 
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--extension-field', 'extension',
                     path('release-schema.json'), '--extension', url],
                    'mapping-sheet_extension_extension-field.csv')
 
 
-@pytest.mark.vcr()
 def test_command_extension_and_extension_field_alternative(capsys, monkeypatch):
     url = 'https://github.com/open-contracting-extensions/ocds_lots_extension/archive/v1.1.4.zip'
 
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--extension-field', 'alternative',
                     path('release-schema.json'), '--extension', url],
                    'mapping-sheet_extension_extension-field.csv')
 
 
-@pytest.mark.vcr()
 def test_command_extension_and_extension_field_and_no_inherit_extension(capsys, monkeypatch):
     url = 'https://github.com/open-contracting-extensions/ocds_lots_extension/archive/v1.1.4.zip'
 
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--extension-field', 'extension',
                     path('release-schema.json'), '--extension', url, '--no-inherit-extension'],
                    'mapping-sheet_extension_extension-field_no-inherit-extension.csv')
 
 
-@pytest.mark.vcr()
+@pytest.mark.skipif(
+    platform.system() in ('Darwin', 'Linux') and platform.python_implementation() == 'PyPy',
+    reason='CI outputs /opt/hostedtoolcache/PyPy/3.9.18/x64/lib/pypy3.9/site-packages/certifi/cacert.pem None'
+)
 def test_command_extension_and_extension_field_and_language(capsys, monkeypatch):
-    url = 'https://extensions.open-contracting.org/es/extensions/lots/master/'
+    url = 'https://extensions.open-contracting.org/es/extensions/lots/v1.1.5/'
 
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--extension-field', 'extension',
                     path('release-schema.json'), '--extension', url, '--language', 'es'],
                    'mapping-sheet_extension_extension-field_language.csv')
 
 
-@pytest.mark.vcr()
 def test_command_extension_and_extension_field_location(capsys, monkeypatch):
     url = 'https://github.com/open-contracting-extensions/ocds_location_extension/archive/v1.1.4.zip'
 
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--extension-field', 'extension',
                     path('release-schema.json'), '--extension', url],
                    'mapping-sheet_extension_extension-field_location.csv')
 
 
-@pytest.mark.vcr()
 def test_command_extension_and_extension_field_array(capsys, monkeypatch):
     url = 'https://github.com/open-contracting-extensions/ocds_additionalContactPoints_extension/archive/master.zip'
 
     assert_command(capsys, monkeypatch, main,
                    ['mapping-sheet', '--infer-required', '--extension-field', 'extension',
                     path('release-schema.json'), '--extension', url],
                    'mapping-sheet_extension_extension-field_array.csv')
```

### Comparing `ocdskit-1.1.8/tests/commands/test_package_records.py` & `ocdskit-1.1.9/tests/commands/test_package_records.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_package_releases.py` & `ocdskit-1.1.9/tests/commands/test_package_releases.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_schema_report.py` & `ocdskit-1.1.9/tests/commands/test_schema_report.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_schema_strict.py` & `ocdskit-1.1.9/tests/commands/test_schema_strict.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_set_closed_codelist_enums.py` & `ocdskit-1.1.9/tests/commands/test_set_closed_codelist_enums.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/commands/test_upgrade.py` & `ocdskit-1.1.9/tests/commands/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/bods/components.json` & `ocdskit-1.1.9/tests/fixtures/bods/components.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/bods/person-statement.json` & `ocdskit-1.1.9/tests/fixtures/bods/person-statement.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json` & `ocdskit-1.1.9/tests/fixtures/combine-record-packages_minimal-maximal-extensions.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json` & `ocdskit-1.1.9/tests/fixtures/combine-release-packages_minimal-maximal-extensions.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_bods.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_bods.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_codelist.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_codelist.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension-field.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension-field.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_array.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_array.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_language.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_language.csv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -308,43 +308,43 @@
 tender,tender/amendment/id,ID,An identifier for this amendment: often the amendment number,string,0..1,,,1.1,,
 tender,tender/amendment/description,Description,"A free text, or semi-structured, description of the changes made in this amendment.",string,0..1,,,1.1,,
 tender,tender/amendment/amendsReleaseID,Amended release (identifier),Provide the identifier (release.id) of the OCDS release (from this contracting process) that provides the values for this contracting process **before** the amendment was made.,string,0..1,,,1.1,,
 tender,tender/amendment/releaseID,Amending release (identifier),Provide the identifier (release.id) of the OCDS release (from this contracting process) that provides the values for this contracting process **after** the amendment was made.,string,0..1,,,1.1,,
 tender,tender/amendment/changes,Amended fields,"An array change objects describing the fields changed, and their former values. (Deprecated in 1.1)",array,0..n,,,1.1,"A free-text or semi-structured string describing the changes made in each amendment can be provided in the amendment.description field. To provide structured information on the fields that have changed, publishers should provide releases indicating the state of the contracting process before and after the amendment.  ",
 tender,tender/amendment/changes/property,Property,"The property name that has been changed relative to the place the amendment is. For example if the contract value has changed, then the property under changes within the contract.amendment would be value.amount. (Deprecated in 1.1)",string,1..1,,,1.1,,
 tender,tender/amendment/changes/former_value,Former Value,"The previous value of the changed property, in whatever type the property is. (Deprecated in 1.1)","array, integer, number, object, string",0..1,,,1.1,,
+tender,tender/lots,Lotes,"Un proceso de licitación se puede dividir en lotes, donde los licitadores pueden ofertar en uno o más lotes. Los detalles de cada lote se pueden proporcionar aquí. Los artículos, documentos y otras características pueden hacer referencia al lote al que están relacionados con el uso de relatedLot. Cuando no se indique ningún identificador relacionado, los valores deben interpretarse como aplicables a toda la licitación. Las propiedades de la licitación pueden ser sobreescritas para un lote dado a través de su inclusión en el objeto Lot.",array,0..n,,,,,Lotes
+,tender/lots,Lotes,Un lote es una agrupación de artículos en una licitación que se pueden ofertar o adjudicar juntos.,object,,,,,,Lotes
+tender,tender/lots/id,ID Lote,"Un identificador local para este lote, tal como un número de lote. Esto se utiliza en las referencias relatedLots en el nivel de artículo, documento y adjudicación.",string,1..1,,,,,Lotes
+tender,tender/lots/title,Título,Un título para este lote.,string,0..1,,,,,Lotes
+tender,tender/lots/description,Descripción,Una descripción de este lote.,string,0..1,,,,,Lotes
+tender,tender/lots/status,Estatus de lote,El estado actual del proceso relacionado a este lote.,string,0..1,"Enum: planning, planned, active, cancelled, unsuccessful, complete, withdrawn",,,,Lotes
+tender,tender/lots/value,Valor del lote,El valor máximo estimado de este lote.,object,0..1,,,,,Lotes
+tender,tender/lots/value,Value,,object,0..1,,,,,Lotes
+tender,tender/lots/value/amount,Amount,Amount as a number.,number,0..1,,,,,Lotes
+tender,tender/lots/value/currency,Currency,The currency for each amount should always be specified using the uppercase 3-letter currency code from ISO4217.,string,0..1,"Enum: ADP, AED, AFA, AFN, ALK, ALL, AMD, ANG, AOA, AOK, AON, AOR, ARA, ARP, ARS, ARY, ATS, AUD, AWG, AYM, AZM, AZN, BAD, BAM, BBD, BDT, BEC, BEF, BEL, BGJ, BGK, BGL, BGN, BHD, BIF, BMD, BND, BOB, BOP, BOV, BRB, BRC, BRE, BRL, BRN, BRR, BSD, BTN, BUK, BWP, BYB, BYN, BYR, BZD, CAD, CDF, CHC, CHE, CHF, CHW, CLF, CLP, CNY, COP, COU, CRC, CSD, CSJ, CSK, CUC, CUP, CVE, CYP, CZK, DDM, DEM, DJF, DKK, DOP, DZD, ECS, ECV, EEK, EGP, ERN, ESA, ESB, ESP, ETB, EUR, FIM, FJD, FKP, FRF, GBP, GEK, GEL, GHC, GHP, GHS, GIP, GMD, GNE, GNF, GNS, GQE, GRD, GTQ, GWE, GWP, GYD, HKD, HNL, HRD, HRK, HTG, HUF, IDR, IEP, ILP, ILR, ILS, INR, IQD, IRR, ISJ, ISK, ITL, JMD, JOD, JPY, KES, KGS, KHR, KMF, KPW, KRW, KWD, KYD, KZT, LAJ, LAK, LBP, LKR, LRD, LSL, LSM, LTL, LTT, LUC, LUF, LUL, LVL, LVR, LYD, MAD, MDL, MGA, MGF, MKD, MLF, MMK, MNT, MOP, MRO, MTL, MTP, MUR, MVQ, MVR, MWK, MXN, MXP, MXV, MYR, MZE, MZM, MZN, NAD, NGN, NIC, NIO, NLG, NOK, NPR, NZD, OMR, PAB, PEH, PEI, PEN, PES, PGK, PHP, PKR, PLN, PLZ, PTE, PYG, QAR, RHD, ROK, ROL, RON, RSD, RUB, RUR, RWF, SAR, SBD, SCR, SDD, SDG, SDP, SEK, SGD, SHP, SIT, SKK, SLL, SOS, SRD, SRG, SSP, STD, SUR, SVC, SYP, SZL, THB, TJR, TJS, TMM, TMT, TND, TOP, TPE, TRL, TRY, TTD, TWD, TZS, UAH, UAK, UGS, UGW, UGX, USD, USN, USS, UYI, UYN, UYP, UYU, UZS, VEB, VEF, VNC, VND, VUV, WST, XAF, XAG, XAU, XBA, XBB, XBC, XBD, XCD, XDR, XEU, XFO, XFU, XOF, XPD, XPF, XPT, XRE, XSU, XTS, XUA, XXX, YDD, YER, YUD, YUM, YUN, ZAL, ZAR, ZMK, ZMW, ZRN, ZRZ, ZWC, ZWD, ZWL, ZWN, ZWR",,,,Lotes
+tender,tender/lots/contractPeriod,Período del contrato,"El período sobre el cual se estima o especifica que el contrato estará activo. Si el lote no especifica fechas explícitas, se puede usar el campo `duration`.",object,0..1,,,,,Lotes
+tender,tender/lots/contractPeriod,Period,    ,object,0..1,,,,,Lotes
+tender,tender/lots/contractPeriod/startDate,Start date,"The start date for the period. When known, a precise start date must always be provided.",string,0..1,date-time,,,,Lotes
+tender,tender/lots/contractPeriod/endDate,End date,"The end date for the period. When known, a precise end date must always be provided.",string,0..1,date-time,,,,Lotes
+tender,tender/lots/contractPeriod/maxExtentDate,Maximum extent,"The period cannot be extended beyond this date. This field is optional, and can be used to express the maximum available data for extension or renewal of this period.",string,0..1,date-time,,,,Lotes
+tender,tender/lots/contractPeriod/durationInDays,Duration (days),"The maximum duration of this period in days. A user interface may wish to collect or display this data in months or years as appropriate, but should convert it into days when completing this field. This field can be used when exact dates are not known.  Where a startDate and endDate are given, this field is optional, and should reflect the difference between those two days. Where a startDate and maxExtentDate are given, this field is optional, and should reflect the difference between startDate and maxExtentDate.",integer,0..1,,,,,Lotes
 tender,tender/lotDetails,Detalles del lote,"Si esta licitación está dividida en lotes, aquí pueden darse detalles de los criterios que aplican para hacer una oferta en estos lotes.",object,0..1,,,,,Lotes
-tender,tender/lotDetails/awardCriteriaDetails,Detalles de criterios de adjudicación,Cualquier información detallada o adicional sobre la adjudicación o los criterios de selección.,string,0..1,,,,,Lotes
-tender,tender/lotDetails/maximumLotsAwardedPerSupplier,Lotes máximos por proveedor,El número máximo de lotes que pueden adjudicarse a un proveedor como parte de este proceso de contratación.,integer,0..1,,,,,Lotes
 tender,tender/lotDetails/maximumLotsBidPerSupplier,Lotes máximos por proveedor,El número máximo de lotes por los que un proveedor puede ofertar como parte de este proceso de contratación.,integer,0..1,,,,,Lotes
+tender,tender/lotDetails/maximumLotsAwardedPerSupplier,Lotes máximos por proveedor,El número máximo de lotes que pueden adjudicarse a un proveedor como parte de este proceso de contratación.,integer,0..1,,,,,Lotes
+tender,tender/lotDetails/awardCriteriaDetails,Detalles de criterios de adjudicación,Cualquier información detallada o adicional sobre la adjudicación o los criterios de selección.,string,0..1,,,,,Lotes
 tender,tender/lotGroups,Grupos de lote,"Cuando el comprador se reserva el derecho de combinar lotes, o desea especificar el valor total para un grupo de lotes, se utiliza un grupo de lotes para capturar esta información.",array,0..n,,,,,Lotes
 ,tender/lotGroups,Grupo del lote,"Cuando el comprador se reserva el derecho de combinar lotes, o desea especificar el valor total para un grupo de lotes, se utiliza un grupo de lotes para capturar esta información.",object,,,,,,Lotes
 tender,tender/lotGroups/id,Identificador del grupo de lote,Un identificador local para este grupo de lotes.,string,1..1,,,,,Lotes
+tender,tender/lotGroups/relatedLots,Lotes relacionados,Una lista de los identificadores de los lotes que forman este grupo. Los lotes pueden aparecer en más de un grupo.,array,0..n,,,,,Lotes
+tender,tender/lotGroups/optionToCombine,Opción de combinar,El comprador se reserva el derecho de combinar los lotes de este grupo al adjudicar un contrato.,boolean,0..1,,,,,Lotes
 tender,tender/lotGroups/maximumValue,Valor máximo,El valor máximo estimado de los lotes de este grupo. Este puede ser inferior a la suma total de los valores de los lotes.,object,0..1,,,,,Lotes
 tender,tender/lotGroups/maximumValue,Value,,object,0..1,,,,,Lotes
 tender,tender/lotGroups/maximumValue/amount,Amount,Amount as a number.,number,0..1,,,,,Lotes
 tender,tender/lotGroups/maximumValue/currency,Currency,The currency for each amount should always be specified using the uppercase 3-letter currency code from ISO4217.,string,0..1,"Enum: ADP, AED, AFA, AFN, ALK, ALL, AMD, ANG, AOA, AOK, AON, AOR, ARA, ARP, ARS, ARY, ATS, AUD, AWG, AYM, AZM, AZN, BAD, BAM, BBD, BDT, BEC, BEF, BEL, BGJ, BGK, BGL, BGN, BHD, BIF, BMD, BND, BOB, BOP, BOV, BRB, BRC, BRE, BRL, BRN, BRR, BSD, BTN, BUK, BWP, BYB, BYN, BYR, BZD, CAD, CDF, CHC, CHE, CHF, CHW, CLF, CLP, CNY, COP, COU, CRC, CSD, CSJ, CSK, CUC, CUP, CVE, CYP, CZK, DDM, DEM, DJF, DKK, DOP, DZD, ECS, ECV, EEK, EGP, ERN, ESA, ESB, ESP, ETB, EUR, FIM, FJD, FKP, FRF, GBP, GEK, GEL, GHC, GHP, GHS, GIP, GMD, GNE, GNF, GNS, GQE, GRD, GTQ, GWE, GWP, GYD, HKD, HNL, HRD, HRK, HTG, HUF, IDR, IEP, ILP, ILR, ILS, INR, IQD, IRR, ISJ, ISK, ITL, JMD, JOD, JPY, KES, KGS, KHR, KMF, KPW, KRW, KWD, KYD, KZT, LAJ, LAK, LBP, LKR, LRD, LSL, LSM, LTL, LTT, LUC, LUF, LUL, LVL, LVR, LYD, MAD, MDL, MGA, MGF, MKD, MLF, MMK, MNT, MOP, MRO, MTL, MTP, MUR, MVQ, MVR, MWK, MXN, MXP, MXV, MYR, MZE, MZM, MZN, NAD, NGN, NIC, NIO, NLG, NOK, NPR, NZD, OMR, PAB, PEH, PEI, PEN, PES, PGK, PHP, PKR, PLN, PLZ, PTE, PYG, QAR, RHD, ROK, ROL, RON, RSD, RUB, RUR, RWF, SAR, SBD, SCR, SDD, SDG, SDP, SEK, SGD, SHP, SIT, SKK, SLL, SOS, SRD, SRG, SSP, STD, SUR, SVC, SYP, SZL, THB, TJR, TJS, TMM, TMT, TND, TOP, TPE, TRL, TRY, TTD, TWD, TZS, UAH, UAK, UGS, UGW, UGX, USD, USN, USS, UYI, UYN, UYP, UYU, UZS, VEB, VEF, VNC, VND, VUV, WST, XAF, XAG, XAU, XBA, XBB, XBC, XBD, XCD, XDR, XEU, XFO, XFU, XOF, XPD, XPF, XPT, XRE, XSU, XTS, XUA, XXX, YDD, YER, YUD, YUM, YUN, ZAL, ZAR, ZMK, ZMW, ZRN, ZRZ, ZWC, ZWD, ZWL, ZWN, ZWR",,,,Lotes
-tender,tender/lotGroups/optionToCombine,Opción de combinar,El comprador se reserva el derecho de combinar los lotes de este grupo al adjudicar un contrato.,boolean,0..1,,,,,Lotes
-tender,tender/lotGroups/relatedLots,Lotes relacionados,Una lista de los identificadores de los lotes que forman este grupo. Los lotes pueden aparecer en más de un grupo.,array,0..n,,,,,Lotes
-tender,tender/lots,Lotes,"Un proceso de licitación se puede dividir en lotes, donde los licitadores pueden ofertar en uno o más lotes. Los detalles de cada lote se pueden proporcionar aquí. Los artículos, documentos y otras características pueden hacer referencia al lote al que están relacionados con el uso de relatedLot. Cuando no se indique ningún identificador relacionado, los valores deben interpretarse como aplicables a toda la licitación. Las propiedades de la licitación pueden ser sobreescritas para un lote dado a través de su inclusión en el objeto Lot.",array,0..n,,,,,Lotes
-,tender/lots,Lotes,Un lote es una agrupación de artículos en una licitación que se pueden ofertar o adjudicar juntos.,object,,,,,,Lotes
-tender,tender/lots/contractPeriod,Período del contrato,"El período sobre el cual se estima o especifica que el contrato estará activo. Si el lote no especifica fechas explícitas, se puede usar el campo `duration`.",object,0..1,,,,,Lotes
-tender,tender/lots/contractPeriod,Period,    ,object,0..1,,,,,Lotes
-tender,tender/lots/contractPeriod/startDate,Start date,"The start date for the period. When known, a precise start date must always be provided.",string,0..1,date-time,,,,Lotes
-tender,tender/lots/contractPeriod/endDate,End date,"The end date for the period. When known, a precise end date must always be provided.",string,0..1,date-time,,,,Lotes
-tender,tender/lots/contractPeriod/maxExtentDate,Maximum extent,"The period cannot be extended beyond this date. This field is optional, and can be used to express the maximum available data for extension or renewal of this period.",string,0..1,date-time,,,,Lotes
-tender,tender/lots/contractPeriod/durationInDays,Duration (days),"The maximum duration of this period in days. A user interface may wish to collect or display this data in months or years as appropriate, but should convert it into days when completing this field. This field can be used when exact dates are not known.  Where a startDate and endDate are given, this field is optional, and should reflect the difference between those two days. Where a startDate and maxExtentDate are given, this field is optional, and should reflect the difference between startDate and maxExtentDate.",integer,0..1,,,,,Lotes
-tender,tender/lots/description,Descripción,Una descripción de este lote.,string,0..1,,,,,Lotes
-tender,tender/lots/id,ID Lote,"Un identificador local para este lote, tal como un número de lote. Esto se utiliza en las referencias relatedLots en el nivel de artículo, documento y adjudicación.",string,1..1,,,,,Lotes
-tender,tender/lots/status,Estatus de lote,El estado actual del proceso relacionado a este lote.,string,0..1,"Enum: planning, planned, active, cancelled, unsuccessful, complete, withdrawn",,,,Lotes
-tender,tender/lots/title,Título,Un título para este lote.,string,0..1,,,,,Lotes
-tender,tender/lots/value,Valor del lote,El valor máximo estimado de este lote.,object,0..1,,,,,Lotes
-tender,tender/lots/value,Value,,object,0..1,,,,,Lotes
-tender,tender/lots/value/amount,Amount,Amount as a number.,number,0..1,,,,,Lotes
-tender,tender/lots/value/currency,Currency,The currency for each amount should always be specified using the uppercase 3-letter currency code from ISO4217.,string,0..1,"Enum: ADP, AED, AFA, AFN, ALK, ALL, AMD, ANG, AOA, AOK, AON, AOR, ARA, ARP, ARS, ARY, ATS, AUD, AWG, AYM, AZM, AZN, BAD, BAM, BBD, BDT, BEC, BEF, BEL, BGJ, BGK, BGL, BGN, BHD, BIF, BMD, BND, BOB, BOP, BOV, BRB, BRC, BRE, BRL, BRN, BRR, BSD, BTN, BUK, BWP, BYB, BYN, BYR, BZD, CAD, CDF, CHC, CHE, CHF, CHW, CLF, CLP, CNY, COP, COU, CRC, CSD, CSJ, CSK, CUC, CUP, CVE, CYP, CZK, DDM, DEM, DJF, DKK, DOP, DZD, ECS, ECV, EEK, EGP, ERN, ESA, ESB, ESP, ETB, EUR, FIM, FJD, FKP, FRF, GBP, GEK, GEL, GHC, GHP, GHS, GIP, GMD, GNE, GNF, GNS, GQE, GRD, GTQ, GWE, GWP, GYD, HKD, HNL, HRD, HRK, HTG, HUF, IDR, IEP, ILP, ILR, ILS, INR, IQD, IRR, ISJ, ISK, ITL, JMD, JOD, JPY, KES, KGS, KHR, KMF, KPW, KRW, KWD, KYD, KZT, LAJ, LAK, LBP, LKR, LRD, LSL, LSM, LTL, LTT, LUC, LUF, LUL, LVL, LVR, LYD, MAD, MDL, MGA, MGF, MKD, MLF, MMK, MNT, MOP, MRO, MTL, MTP, MUR, MVQ, MVR, MWK, MXN, MXP, MXV, MYR, MZE, MZM, MZN, NAD, NGN, NIC, NIO, NLG, NOK, NPR, NZD, OMR, PAB, PEH, PEI, PEN, PES, PGK, PHP, PKR, PLN, PLZ, PTE, PYG, QAR, RHD, ROK, ROL, RON, RSD, RUB, RUR, RWF, SAR, SBD, SCR, SDD, SDG, SDP, SEK, SGD, SHP, SIT, SKK, SLL, SOS, SRD, SRG, SSP, STD, SUR, SVC, SYP, SZL, THB, TJR, TJS, TMM, TMT, TND, TOP, TPE, TRL, TRY, TTD, TWD, TZS, UAH, UAK, UGS, UGW, UGX, USD, USN, USS, UYI, UYN, UYP, UYU, UZS, VEB, VEF, VNC, VND, VUV, WST, XAF, XAG, XAU, XBA, XBB, XBC, XBD, XCD, XDR, XEU, XFO, XFU, XOF, XPD, XPF, XPT, XRE, XSU, XTS, XUA, XXX, YDD, YER, YUD, YUM, YUN, ZAL, ZAR, ZMK, ZMW, ZRN, ZRZ, ZWC, ZWD, ZWL, ZWN, ZWR",,,,Lotes
 ,awards,Awards,"Information from the award phase of the contracting process. There may be more than one award per contracting process e.g. because the contract is split among different providers, or because it is a standing offer.",array,0..n,,,,,
 ,awards,Award,"An award for the given procurement. There may be more than one award per contracting process e.g. because the contract is split among different providers, or because it is a standing offer.",object,,,,,,
 awards,awards/id,Award ID,The identifier for this award. It must be unique and cannot change within the Open Contracting Process it is part of (defined by a single ocid). See the identifier guidance for further details.,"integer, string",1..1,,http://standard.open-contracting.org/{{version}}/{{lang}}/schema/identifiers/,,,
 awards,awards/title,Title,Award title,string,0..1,,,,,
 awards,awards/description,Description,Award description,string,0..1,,,,,
 awards,awards/status,Award status,The current status of the award drawn from the awardStatus codelist,string,0..1,"Enum: pending, active, cancelled, unsuccessful",http://standard.open-contracting.org/{{version}}/{{lang}}/schema/codelists/#award-status,,,
 awards,awards/date,Award date,The date of the contract award. This is usually the date on which a decision to award was made.,string,0..1,date-time,,,,
```

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_location.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_location.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_extension_extension-field_no-inherit-extension.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_no-deprecated.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_no-deprecated.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_oc4ids.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_oc4ids.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_order-by.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_order-by.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/mapping-sheet_sedl.csv` & `ocdskit-1.1.9/tests/fixtures/mapping-sheet_sedl.csv`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/ocds-sample-data.json.gz` & `ocdskit-1.1.9/tests/fixtures/ocds-sample-data.json.gz`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/project-schema.json` & `ocdskit-1.1.9/tests/fixtures/project-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/compile_encoding_encoding.json` & `ocdskit-1.1.9/tests/fixtures/realdata/compile_encoding_encoding.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/compiled-release-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/compiled-release-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/compiled-release-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package-1-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package-1-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package-1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.0.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_1.0.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_1.1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_1.1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_linked-releases.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_linked-releases.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_package.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_package.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_package_1.1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_package_1.1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_record-package.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_record-package.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_split.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_split.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/record-package_versioned.json` & `ocdskit-1.1.9/tests/fixtures/realdata/record-package_versioned.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package-1-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package-1-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package-1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.0-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.0-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.0-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.1-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_1.1-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_1.1-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_encoding-iso-8859-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_encoding-utf-8.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_encoding-utf-8.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_record-package.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_record-package.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/release-package_split.json` & `ocdskit-1.1.9/tests/fixtures/realdata/release-package_split.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-1.json` & `ocdskit-1.1.9/tests/fixtures/realdata/versioned-release-1.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/realdata/versioned-release-2.json` & `ocdskit-1.1.9/tests/fixtures/realdata/versioned-release-2.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/release-package-schema.json` & `ocdskit-1.1.9/tests/fixtures/release-package-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/release-package_additional-contact-points.json` & `ocdskit-1.1.9/tests/fixtures/release-package_additional-contact-points.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/release-packages.jsonl` & `ocdskit-1.1.9/tests/fixtures/release-packages.jsonl`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/release-schema.json` & `ocdskit-1.1.9/tests/fixtures/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/schema-strict.json` & `ocdskit-1.1.9/tests/fixtures/schema-strict.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/sedl-schema.json` & `ocdskit-1.1.9/tests/fixtures/sedl-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/fixtures/test-schema.json` & `ocdskit-1.1.9/tests/fixtures/test-schema.json`

 * *Files identical despite different names*

### Comparing `ocdskit-1.1.8/tests/test_combine.py` & `ocdskit-1.1.9/tests/test_combine.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,55 +13,50 @@
             for item in json.loads(read(filename))['records']]
 
     actual = package_records(data)
 
     assert actual == json.loads(read('realdata/record-package_record-package.json'))
 
 
-@pytest.mark.vcr()
 def test_merge_empty():
     compiled_releases = list(merge([]))
 
     assert compiled_releases == []
 
 
-@pytest.mark.vcr()
 def test_merge_with_schema():
     builder = ProfileBuilder('1__1__4', {'additionalContactPoint': 'master'})
     schema = builder.patched_release_schema()
 
     data = json.loads(read('release-package_additional-contact-points.json'))['releases']
     compiled_release = list(merge(data, schema=schema))[0]
 
     assert compiled_release == json.loads(read('compile_extensions.json'))
 
 
-@pytest.mark.vcr()
 def test_merge_without_schema():
     data = json.loads(read('release-package_additional-contact-points.json'))['releases']
     compiled_release = list(merge(data))[0]
 
     assert compiled_release == json.loads(read('compile_no-extensions.json'))
 
 
-@pytest.mark.vcr()
 def test_merge_warning():
     data = json.loads(read('release-package_warning.json'))['releases']
 
     with pytest.warns(DuplicateIdValueWarning) as records:
         compiled_release = list(merge(data))[0]
 
     assert compiled_release == json.loads(read('compile_warning.json'))
 
     assert [record.message for record in records] == [
         ("ocds-213czf-1: Multiple objects have the `id` value '1' in the `parties` array"),
     ]
 
 
-@pytest.mark.vcr()
 def test_compile_release_packages():
     with pytest.warns(DeprecationWarning) as records:
         compiled_releases = list(compile_release_packages([]))
 
     assert compiled_releases == []
     assert len(records) == 1
     assert str(records[0].message) == 'compile_release_packages() is deprecated. Use merge() instead.'
```

### Comparing `ocdskit-1.1.8/tests/test_packager.py` & `ocdskit-1.1.9/tests/test_packager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import json
 
-import pytest
 from ocdsmerge import Merger
 from ocdsmerge.util import get_release_schema_url, get_tags
 
 from ocdskit.packager import Packager
 from tests import read
 
 
-@pytest.mark.vcr()
 def test_output_package_no_streaming():
     data = [json.loads(read(filename)) for filename in
             ('realdata/release-package-1.json', 'realdata/release-package-2.json')]
 
     with Packager() as packager:
         packager.package['version'] = '1.1'
         packager.add(data)
```

### Comparing `ocdskit-1.1.8/tests/test_util.py` & `ocdskit-1.1.9/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import gzip
 import json
 
 import pytest
 
-from ocdskit.util import (detect_format, get_ocds_minor_version, is_compiled_release, is_linked_release, is_package,
-                          is_record, is_record_package, is_release, is_release_package, json_dump)
+from ocdskit.util import (
+    detect_format,
+    get_ocds_minor_version,
+    is_compiled_release,
+    is_linked_release,
+    is_package,
+    is_record,
+    is_record_package,
+    is_release,
+    is_release_package,
+    json_dump,
+)
 from tests import path, read
 
 
 # Same fixture files as in test_detect_format.py, except for concatenated JSON files.
 @pytest.mark.parametrize('filename,expected', [
     ('record-package_minimal.json', True),
     ('release-package_minimal.json', True),
```

