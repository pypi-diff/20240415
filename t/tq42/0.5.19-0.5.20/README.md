# Comparing `tmp/tq42-0.5.19.tar.gz` & `tmp/tq42-0.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tq42-0.5.19.tar", max compression
+gzip compressed data, was "tq42-0.5.20.tar", max compression
```

## Comparing `tq42-0.5.19.tar` & `tq42-0.5.20.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11357 2024-04-12 12:56:03.669864 tq42-0.5.19/LICENSE
--rw-r--r--   0        0        0     6029 2024-04-12 12:56:03.669864 tq42-0.5.19/README.md
--rw-r--r--   0        0        0      749 2024-04-12 12:56:03.693863 tq42-0.5.19/pyproject.toml
--rw-r--r--   0        0        0       76 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/__init__.py
--rwxr-xr-x   0        0        0      977 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/__main__.py
--rw-r--r--   0        0        0     2990 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/algorithm.py
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/cli_functions.py
--rw-r--r--   0        0        0     1017 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/compute_group.py
--rw-r--r--   0        0        0     1053 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/experiment_group.py
--rw-r--r--   0        0        0     1478 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/experiment_run_group.py
--rw-r--r--   0        0        0      420 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/organization_group.py
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/output_format/__init__.py
--rw-r--r--   0        0        0     3243 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/output_format/formatter.py
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/parsers/__init__.py
--rw-r--r--   0        0        0     2688 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/parsers/params_checker.py
--rw-r--r--   0        0        0     5891 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/parsers/tq42parser.py
--rw-r--r--   0        0        0      783 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/project_dataset_group.py
--rw-r--r--   0        0        0      719 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/project_group.py
--rw-r--r--   0        0        0     1201 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/tq42_all.py
--rw-r--r--   0        0        0     3500 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/tq42_help.py
--rw-r--r--   0        0        0     7998 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/client.py
--rw-r--r--   0        0        0     2091 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/compute.py
--rw-r--r--   0        0        0     2734 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/dataset.py
--rw-r--r--   0        0        0     2311 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/exception_handling.py
--rw-r--r--   0        0        0     1854 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/exceptions.py
--rw-r--r--   0        0        0     3974 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/experiment.py
--rw-r--r--   0        0        0     5969 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/experiment_run.py
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/__init__.py
--rw-r--r--   0        0        0      573 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/conftest.py
--rw-r--r--   0        0        0     3396 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/functional_test_config.py
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/__init__.py
--rw-r--r--   0        0        0     1474 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_cli.py
--rw-r--r--   0        0        0     1523 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_compute_group.py
--rw-r--r--   0        0        0     1190 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py
--rw-r--r--   0        0        0     2404 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py
--rw-r--r--   0        0        0      678 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_organization_group.py
--rw-r--r--   0        0        0     1222 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_project_group.py
--rw-r--r--   0        0        0      689 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_functional_cache_utils.py
--rw-r--r--   0        0        0     5721 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_functional_tq42_api.py
--rw-r--r--   0        0        0     1371 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_polling_function.py
--rw-r--r--   0        0        0      437 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_test_config.py
--rw-r--r--   0        0        0     3038 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/organization.py
--rw-r--r--   0        0        0     5355 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/project.py
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/__init__.py
--rw-r--r--   0        0        0     4861 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/test_output_format.py
--rw-r--r--   0        0        0     6185 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/test_tq42_help.py
--rw-r--r--   0        0        0     3787 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/test_tq42_help_flags.py
--rw-r--r--   0        0        0      892 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_cache_utils.py
--rw-r--r--   0        0        0      806 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_compute.py
--rw-r--r--   0        0        0     2202 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_config_environment.py
--rw-r--r--   0        0        0     1890 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_dirs.py
--rw-r--r--   0        0        0      825 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_example.py
--rw-r--r--   0        0        0     1475 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_imports.py
--rw-r--r--   0        0        0      159 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_package_version.py
--rw-r--r--   0        0        0     7800 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_tq42_api.py
--rw-r--r--   0        0        0     7617 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_tq42_error_handling.py
--rw-r--r--   0        0        0    10198 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_utils.py
--rwxr-xr-x   0        0        0       48 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/README.md
--rw-r--r--   0        0        0      147 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/config.json
--rwxr-xr-x   0        0        0      460 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/test_convert_colon_separated_string_to_dict.txt
--rwxr-xr-x   0        0        0      210 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/test_utils_get_id.txt
--rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/__init__.py
--rw-r--r--   0        0        0      547 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/constants.py
--rw-r--r--   0        0        0     1256 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/dirs.py
--rw-r--r--   0        0        0     1828 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/environment_utils.py
--rw-r--r--   0        0        0      365 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/file_handling.py
--rw-r--r--   0        0        0      147 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/config.json
--rwxr-xr-x   0        0        0      132 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/cpu_configs.json
--rwxr-xr-x   0        0        0      829 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/hardware_configs.json
--rw-r--r--   0        0        0    14166 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/help.json
--rw-r--r--   0        0        0     2342 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/help_flags.json
--rw-r--r--   0        0        0      491 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/insufficient_permission_error.txt
--rw-r--r--   0        0        0      130 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/invalid_arguments_error.txt
--rw-r--r--   0        0        0      191 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/local_permission_error.txt
--rw-r--r--   0        0        0      470 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/no_default_error.txt
--rwxr-xr-x   0        0        0      657 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/tq42_commands.txt
--rw-r--r--   0        0        0      411 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/text_files/unauthenticated_error.txt
--rw-r--r--   0        0        0     2284 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/token_manager.py
--rw-r--r--   0        0        0     4469 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/utils.py
--rw-r--r--   0        0        0      966 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/utils_for_cache.py
--rw-r--r--   0        0        0     6690 1970-01-01 00:00:00.000000 tq42-0.5.19/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-15 08:06:56.029517 tq42-0.5.20/LICENSE
+-rw-r--r--   0        0        0     6029 2024-04-15 08:06:56.029517 tq42-0.5.20/README.md
+-rw-r--r--   0        0        0      749 2024-04-15 08:06:56.053517 tq42-0.5.20/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/__init__.py
+-rwxr-xr-x   0        0        0      977 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/__main__.py
+-rw-r--r--   0        0        0     2990 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/algorithm.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/cli_functions.py
+-rw-r--r--   0        0        0     1017 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/compute_group.py
+-rw-r--r--   0        0        0     1053 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/experiment_group.py
+-rw-r--r--   0        0        0     1478 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/experiment_run_group.py
+-rw-r--r--   0        0        0      420 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/organization_group.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/output_format/__init__.py
+-rw-r--r--   0        0        0     3243 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/output_format/formatter.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/parsers/__init__.py
+-rw-r--r--   0        0        0     2688 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/parsers/params_checker.py
+-rw-r--r--   0        0        0     5891 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/parsers/tq42parser.py
+-rw-r--r--   0        0        0      783 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/project_dataset_group.py
+-rw-r--r--   0        0        0      719 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/project_group.py
+-rw-r--r--   0        0        0     1201 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/tq42_all.py
+-rw-r--r--   0        0        0     3500 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/cli/tq42_help.py
+-rw-r--r--   0        0        0     9637 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/client.py
+-rw-r--r--   0        0        0     2091 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/compute.py
+-rw-r--r--   0        0        0     2734 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/dataset.py
+-rw-r--r--   0        0        0     2355 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/exception_handling.py
+-rw-r--r--   0        0        0     2033 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/exceptions.py
+-rw-r--r--   0        0        0     3974 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/experiment.py
+-rw-r--r--   0        0        0     5969 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/experiment_run.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/functional_tests/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/functional_tests/conftest.py
+-rw-r--r--   0        0        0     3396 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/functional_tests/functional_test_config.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/functional_tests/invoke_cli/__init__.py
+-rw-r--r--   0        0        0     1474 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_cli.py
+-rw-r--r--   0        0        0     1523 2024-04-15 08:06:56.053517 tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_compute_group.py
+-rw-r--r--   0        0        0     1190 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py
+-rw-r--r--   0        0        0     2404 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py
+-rw-r--r--   0        0        0      678 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_organization_group.py
+-rw-r--r--   0        0        0     1222 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_project_group.py
+-rw-r--r--   0        0        0      689 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/test_functional_cache_utils.py
+-rw-r--r--   0        0        0     5721 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/test_functional_tq42_api.py
+-rw-r--r--   0        0        0     1371 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/test_polling_function.py
+-rw-r--r--   0        0        0      437 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/functional_tests/test_test_config.py
+-rw-r--r--   0        0        0     3038 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/organization.py
+-rw-r--r--   0        0        0     5355 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/project.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/cli/__init__.py
+-rw-r--r--   0        0        0     4861 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/cli/test_output_format.py
+-rw-r--r--   0        0        0     6185 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/cli/test_tq42_help.py
+-rw-r--r--   0        0        0     3787 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/cli/test_tq42_help_flags.py
+-rw-r--r--   0        0        0      892 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_cache_utils.py
+-rw-r--r--   0        0        0      806 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_compute.py
+-rw-r--r--   0        0        0     2253 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_config_environment.py
+-rw-r--r--   0        0        0     1890 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_dirs.py
+-rw-r--r--   0        0        0      825 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_example.py
+-rw-r--r--   0        0        0     1475 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_imports.py
+-rw-r--r--   0        0        0      159 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_package_version.py
+-rw-r--r--   0        0        0     7800 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_tq42_api.py
+-rw-r--r--   0        0        0     7617 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_tq42_error_handling.py
+-rw-r--r--   0        0        0    10223 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/test_utils.py
+-rwxr-xr-x   0        0        0       48 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/testdata/README.md
+-rw-r--r--   0        0        0      147 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/testdata/config.json
+-rwxr-xr-x   0        0        0      460 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/testdata/test_convert_colon_separated_string_to_dict.txt
+-rwxr-xr-x   0        0        0      210 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/tests/testdata/test_utils_get_id.txt
+-rw-r--r--   0        0        0        0 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/__init__.py
+-rw-r--r--   0        0        0      547 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/dirs.py
+-rw-r--r--   0        0        0     1828 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/environment_utils.py
+-rw-r--r--   0        0        0      365 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/file_handling.py
+-rw-r--r--   0        0        0      147 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/config.json
+-rwxr-xr-x   0        0        0      132 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/cpu_configs.json
+-rwxr-xr-x   0        0        0      829 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/hardware_configs.json
+-rw-r--r--   0        0        0    14166 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/help.json
+-rw-r--r--   0        0        0     2342 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/help_flags.json
+-rw-r--r--   0        0        0      491 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/insufficient_permission_error.txt
+-rw-r--r--   0        0        0      130 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/invalid_arguments_error.txt
+-rw-r--r--   0        0        0      191 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/local_permission_error.txt
+-rw-r--r--   0        0        0      470 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/no_default_error.txt
+-rwxr-xr-x   0        0        0      657 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/tq42_commands.txt
+-rw-r--r--   0        0        0      411 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/text_files/unauthenticated_error.txt
+-rw-r--r--   0        0        0     2284 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/token_manager.py
+-rw-r--r--   0        0        0     4469 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/utils.py
+-rw-r--r--   0        0        0      966 2024-04-15 08:06:56.057517 tq42-0.5.20/tq42/utils/utils_for_cache.py
+-rw-r--r--   0        0        0     6690 1970-01-01 00:00:00.000000 tq42-0.5.20/PKG-INFO
```

### Comparing `tq42-0.5.19/LICENSE` & `tq42-0.5.20/LICENSE`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/README.md` & `tq42-0.5.20/README.md`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/pyproject.toml` & `tq42-0.5.20/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 include = ["utils/text_files/*.txt", "utils/text_files/config.json", "tests/testdata/*.txt"]
 
 [tool.poetry]
 name = "tq42"
-version = "0.5.19"
+version = "0.5.20"
 description = "tq42 sdk"
 readme = "README.md"
 authors = ["Terra Quantum AG"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "2.31.0"
```

### Comparing `tq42-0.5.19/tq42/__main__.py` & `tq42-0.5.20/tq42/__main__.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/algorithm.py` & `tq42-0.5.20/tq42/algorithm.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/cli_functions.py` & `tq42-0.5.20/tq42/cli/cli_functions.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/compute_group.py` & `tq42-0.5.20/tq42/cli/compute_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/experiment_group.py` & `tq42-0.5.20/tq42/cli/experiment_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/experiment_run_group.py` & `tq42-0.5.20/tq42/cli/experiment_run_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/output_format/formatter.py` & `tq42-0.5.20/tq42/cli/output_format/formatter.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/parsers/params_checker.py` & `tq42-0.5.20/tq42/cli/parsers/params_checker.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/parsers/tq42parser.py` & `tq42-0.5.20/tq42/cli/parsers/tq42parser.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/project_dataset_group.py` & `tq42-0.5.20/tq42/cli/project_dataset_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/project_group.py` & `tq42-0.5.20/tq42/cli/project_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/tq42_all.py` & `tq42-0.5.20/tq42/cli/tq42_all.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/cli/tq42_help.py` & `tq42-0.5.20/tq42/cli/tq42_help.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/client.py` & `tq42-0.5.20/tq42/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from com.terraquantum.project.v1.project import (
     project_service_pb2_grpc as pb2_proj_grpc,
 )
 from com.terraquantum.experiment.v1.dataset import (
     dataset_service_pb2_grpc as pb2_data_grpc,
 )
 from tq42.utils.environment_utils import environment_default_set
+from tq42.exceptions import AuthenticationError
 
 
 class ConfigEnvironment:
     """
     URLs determining environment
     """
 
@@ -50,14 +51,18 @@
         return "https://auth.{}/oauth/device/code".format(self.base_url)
 
     @property
     def audience(self):
         return "https://graphql-gateway.{}/graphql".format(self.base_url)
 
     @property
+    def client_credential_flow_audience(self):
+        return "https://api.{}".format(self.base_url)
+
+    @property
     def headers(self):
         return {"Content-Type": "application/x-www-form-urlencoded"}
 
     @property
     def code_data(self):
         return {
             "client_id": self.client_id,
@@ -75,14 +80,22 @@
     def refresh_token_data(self, refresh_token):
         return {
             "grant_type": "refresh_token",
             "refresh_token": refresh_token,
             "client_id": self.client_id,
         }
 
+    def client_credentials_data(self, client_id, client_secret, audience):
+        return {
+            "client_id": client_id,
+            "client_secret": client_secret,
+            "grant_type": "client_credentials",
+            "audience": audience,
+        }
+
 
 class TQ42Client(object):
     """
     Visit tq42.com/help for more details on all commands.
     """
 
     def __call__(self, **kwargs):
@@ -131,27 +144,56 @@
         self.organization_client = pb2_org_grpc.OrganizationServiceStub(self.channel)
         self.project_client = pb2_proj_grpc.ProjectServiceStub(self.channel)
         self.experiment_client = pb2_exp_grpc.ExperimentServiceStub(self.channel)
         self.dataset_client = pb2_data_grpc.DatasetServiceStub(self.channel)
         self.experiment_run_client = pb2_exp_run_grpc.ExperimentRunServiceStub(
             self.channel
         )
+        self.credential_flow_client_id = os.getenv("AUTH_CLIENT_ID")
+        self.credential_flow_client_secret = os.getenv("AUTH_CLIENT_SECRET")
+
+    @handle_generic_sdk_errors
+    def login_without_user_interaction(self):
+        response = requests.post(
+            self.environment.auth_url_token,
+            data=self.environment.client_credentials_data(
+                client_id=self.credential_flow_client_id,
+                client_secret=self.credential_flow_client_secret,
+                audience=self.environment.client_credential_flow_audience,
+            ),
+            headers=self.environment.headers,
+        )
+
+        response_json = response.json()
+        access_token = response_json.get("access_token")
+
+        if not access_token:
+            raise AuthenticationError(
+                "No access token can be retrieved from the response."
+            )
+
+        self.save_access_token(access_token)
 
     @handle_generic_sdk_errors
     def login(self):
+        if self.credential_flow_client_id and self.credential_flow_client_secret:
+            self.login_without_user_interaction()
+        else:
+            self.login_with_user_interaction()
+
+    def login_with_user_interaction(self):
         """
         This function will open a window in your browser where you must enter your TQ42 username and password to
         authenticate. To access TQ42 services with Python commands, you need a TQ42 account. When running TQ42 Python
         commands, your environment needs to have access to your TQ42 account credentials.
 
         For details, see
          https://terra-quantum-tq42sdk-docs.readthedocs-hosted.com/en/latest/README.html#authentication
         """
         # Send the POST request and print the response
-
         response = requests.post(
             self.environment.auth_url_code,
             data=self.environment.code_data,
             headers=self.environment.headers,
         )
 
         json_response = response.json()
@@ -173,46 +215,51 @@
         while True:
             # Send the POST request to get access token and extract the JSON response
             response_token = requests.post(
                 self.environment.auth_url_token,
                 data=data_token,
                 headers=self.environment.headers,
             )
-            json_token = response_token.json()
-            # If we received an access token, print it and break out of the loop
-            if "access_token" in json_token:
-                access_token = json_token["access_token"]
+            response_json = response_token.json()
+
+            refresh_token = response_json.get("refresh_token")
+            access_token = response_json.get("access_token")
 
-                save_location = utils.save_token(
-                    service_name="access_token",
-                    backup_save_path=self.token_file_path,
-                    token=access_token,
-                )
-
-                print(
-                    f"Authentication is successful, access token is saved in: {save_location}."
-                )
-
-                env_set = environment_default_set(client=self)
-                print(env_set)
-
-            if "refresh_token" in json_token:
-                refresh_token = json_token["refresh_token"]
-                utils.save_token(
-                    service_name="refresh_token",
-                    backup_save_path=self.refresh_token_file_path,
-                    token=refresh_token,
-                )
-                current_datetime = datetime.now()
-                file_handling.write_to_file(self.timestamp_file_path, current_datetime)
+            # If we received an access token, print it and break out of the loop
+            if refresh_token and access_token:
+                self.save_access_token(access_token)
+                self.save_refresh_token(refresh_token)
                 break
 
             # Otherwise, wait for the specified interval before polling again
             time.sleep(interval)
 
+    def save_access_token(self, access_token: str):
+        save_location = utils.save_token(
+            service_name="access_token",
+            backup_save_path=self.token_file_path,
+            token=access_token,
+        )
+
+        print(
+            f"Authentication is successful, access token is saved in: {save_location}."
+        )
+
+        env_set = environment_default_set(client=self)
+        print(env_set)
+
+    def save_refresh_token(self, refresh_token: str):
+        utils.save_token(
+            service_name="refresh_token",
+            backup_save_path=self.refresh_token_file_path,
+            token=refresh_token,
+        )
+        current_datetime = datetime.now()
+        file_handling.write_to_file(self.timestamp_file_path, current_datetime)
+
     def is_config_filepath_default(self, config_file):
         return config_file == self.default_config_file
 
     @property
     def token_file_path(self):
         return self.token_manager.token_file_path
```

### Comparing `tq42-0.5.19/tq42/compute.py` & `tq42-0.5.20/tq42/compute.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/dataset.py` & `tq42-0.5.20/tq42/dataset.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/exception_handling.py` & `tq42-0.5.20/tq42/exception_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,15 @@
                 command=traceback.extract_stack()[0].line
             ) from None
         except exceptions.NoMatchingAttributeError as e:
             raise exceptions.InvalidArgumentError(
                 command=traceback.extract_stack()[0].line, details=e.details
             )
         except (
+            exceptions.AuthenticationError,
             exceptions.PermissionDeniedError,
             exceptions.UnauthenticatedError,
             exceptions.InvalidArgumentError,
             exceptions.NoDefaultError,
             exceptions.ExceedRetriesError,
             exceptions.LocalPermissionError,
             exceptions.ExperimentRunCancelError,
```

### Comparing `tq42-0.5.19/tq42/exceptions.py` & `tq42-0.5.20/tq42/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,7 +68,13 @@
     def __str__(self):
         return read_file(local_permission_error_file)
 
 
 class ExperimentRunCancelError(TQ42APIError):
     def __str__(self):
         return "Cannot cancel a run that was already completed or cancelled."
+
+
+class AuthenticationError(TQ42APIError):
+    def __init__(self, message="Authentication error occurred."):
+        self.message = message
+        super().__init__(self.message)
```

### Comparing `tq42-0.5.19/tq42/experiment.py` & `tq42-0.5.20/tq42/experiment.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/experiment_run.py` & `tq42-0.5.20/tq42/experiment_run.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/conftest.py` & `tq42-0.5.20/tq42/functional_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/functional_test_config.py` & `tq42-0.5.20/tq42/functional_tests/functional_test_config.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_cli.py` & `tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_cli.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_compute_group.py` & `tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_compute_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py` & `tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py` & `tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_organization_group.py` & `tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_organization_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_project_group.py` & `tq42-0.5.20/tq42/functional_tests/invoke_cli/test_functional_project_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/test_functional_cache_utils.py` & `tq42-0.5.20/tq42/functional_tests/test_functional_cache_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/test_functional_tq42_api.py` & `tq42-0.5.20/tq42/functional_tests/test_functional_tq42_api.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/functional_tests/test_polling_function.py` & `tq42-0.5.20/tq42/functional_tests/test_polling_function.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/organization.py` & `tq42-0.5.20/tq42/organization.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/project.py` & `tq42-0.5.20/tq42/project.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/cli/test_output_format.py` & `tq42-0.5.20/tq42/tests/cli/test_output_format.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/cli/test_tq42_help.py` & `tq42-0.5.20/tq42/tests/cli/test_tq42_help.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/cli/test_tq42_help_flags.py` & `tq42-0.5.20/tq42/tests/cli/test_tq42_help_flags.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_cache_utils.py` & `tq42-0.5.20/tq42/tests/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_compute.py` & `tq42-0.5.20/tq42/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_config_environment.py` & `tq42-0.5.20/tq42/tests/test_config_environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,17 @@
             "client_id": env.client_id,
         }
         actual = env.token_data("DEVICE CODE")
         self.assertEqual(expected, actual)
 
     def test_int_urls(self):
         env = ConfigEnvironment(
-            "int.terraquantum.io", "CLIENT ID", "openid profile email"
+            "int.terraquantum.io",
+            "CLIENT ID",
+            "openid profile email",
         )
         self.assertEqual("api.int.terraquantum.io", env.host)
         self.assertEqual(
             "https://graphql-gateway.int.terraquantum.io/graphql", env.audience
         )
         self.assertEqual(
             "https://auth.int.terraquantum.io/oauth/device/code", env.auth_url_code
@@ -47,16 +49,19 @@
             "https://auth.int.terraquantum.io/oauth/token", env.auth_url_token
         )
         self.code_data_test(env)
         self.token_data_test(env)
 
     def test_staging_urls(self):
         env = ConfigEnvironment(
-            "staging.terraquantum.io", "CLIENT ID", "openid profile email"
+            "staging.terraquantum.io",
+            "CLIENT ID",
+            "openid profile email",
         )
+
         self.assertEqual("api.staging.terraquantum.io", env.host)
         self.assertEqual(
             "https://graphql-gateway.staging.terraquantum.io/graphql", env.audience
         )
         self.assertEqual(
             "https://auth.staging.terraquantum.io/oauth/device/code", env.auth_url_code
         )
```

### Comparing `tq42-0.5.19/tq42/tests/test_dirs.py` & `tq42-0.5.20/tq42/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_example.py` & `tq42-0.5.20/tq42/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_imports.py` & `tq42-0.5.20/tq42/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_tq42_api.py` & `tq42-0.5.20/tq42/tests/test_tq42_api.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_tq42_error_handling.py` & `tq42-0.5.20/tq42/tests/test_tq42_error_handling.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/tests/test_utils.py` & `tq42-0.5.20/tq42/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,17 @@
 
         # load config file
         alt_config_file = dirs.text_files_dir("config.json")
         with open(alt_config_file, encoding="utf-8") as f:
             config_data = json.load(f)
 
         environment = ConfigEnvironment(
-            config_data["base_url"], config_data["client_id"], config_data["scope"]
+            config_data["base_url"],
+            config_data["client_id"],
+            config_data["scope"],
         )
 
         token_manager = TokenManager(environment, None)
 
         success = token_manager.renew_expring_token()
         # old token timestamp should renew token
         self.assertTrue(success)
```

### Comparing `tq42-0.5.19/tq42/utils/constants.py` & `tq42-0.5.20/tq42/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/dirs.py` & `tq42-0.5.20/tq42/utils/dirs.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/environment_utils.py` & `tq42-0.5.20/tq42/utils/environment_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/text_files/hardware_configs.json` & `tq42-0.5.20/tq42/utils/text_files/hardware_configs.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/text_files/help.json` & `tq42-0.5.20/tq42/utils/text_files/help.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/text_files/help_flags.json` & `tq42-0.5.20/tq42/utils/text_files/help_flags.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/text_files/tq42_commands.txt` & `tq42-0.5.20/tq42/utils/text_files/tq42_commands.txt`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/token_manager.py` & `tq42-0.5.20/tq42/utils/token_manager.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/utils.py` & `tq42-0.5.20/tq42/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/tq42/utils/utils_for_cache.py` & `tq42-0.5.20/tq42/utils/utils_for_cache.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.19/PKG-INFO` & `tq42-0.5.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tq42
-Version: 0.5.19
+Version: 0.5.20
 Summary: tq42 sdk
 Author: Terra Quantum AG
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

