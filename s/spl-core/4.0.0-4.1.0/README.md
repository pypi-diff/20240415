# Comparing `tmp/spl_core-4.0.0.tar.gz` & `tmp/spl_core-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_core-4.0.0.tar", max compression
+gzip compressed data, was "spl_core-4.1.0.tar", max compression
```

## Comparing `spl_core-4.0.0.tar` & `spl_core-4.1.0.tar`

### file list

```diff
@@ -1,65 +1,68 @@
--rw-r--r--   0        0        0     1099 2024-04-02 12:32:36.762329 spl_core-4.0.0/LICENSE
--rw-r--r--   0        0        0      824 2024-04-02 12:32:36.762329 spl_core-4.0.0/README.md
--rw-r--r--   0        0        0     4308 2024-04-02 12:32:37.774333 spl_core-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-02 12:32:37.774333 spl_core-4.0.0/src/spl_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/common/__init__.py
--rw-r--r--   0        0        0     2054 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/common/cmake.py
--rw-r--r--   0        0        0      462 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/common/path.py
--rw-r--r--   0        0        0        0 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/gcov_maid/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/gcov_maid/gcov_maid.py
--rw-r--r--   0        0        0        0 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/kconfig/__init__.py
--rw-r--r--   0        0        0     9795 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/kconfig/kconfig.py
--rw-r--r--   0        0        0        0 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/creator.py
--rw-r--r--   0        0        0      239 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/cookiecutter.json
--rw-r--r--   0        0        0       33 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.flake8
--rw-r--r--   0        0        0      599 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore
--rw-r--r--   0        0        0      269 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-kits.json
--rw-r--r--   0        0        0      718 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json
--rw-r--r--   0        0        0      626 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json
--rw-r--r--   0        0        0     1103 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json
--rw-r--r--   0        0        0     1369 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json
--rw-r--r--   0        0        0     2853 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json
--rw-r--r--   0        0        0     1400 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt
--rw-r--r--   0        0        0      598 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig
--rw-r--r--   0        0        0     1108 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE
--rw-r--r--   0        0        0      563 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/Pipfile
--rw-r--r--   0        0        0      337 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/README.md
--rw-r--r--   0        0        0       73 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.bat
--rw-r--r--   0        0        0    10528 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1
--rw-r--r--   0        0        0     6705 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py
--rw-r--r--   0        0        0   123927 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in
--rw-r--r--   0        0        0       90 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/common/index.rst
--rw-r--r--   0        0        0      594 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst
--rw-r--r--   0        0        0     1072 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE
--rw-r--r--   0        0        0    63071 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css
--rw-r--r--   0        0        0       44 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_architecture/index.rst
--rw-r--r--   0        0        0       95 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_requirements/index.rst
--rw-r--r--   0        0        0     1217 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt
--rw-r--r--   0        0        0     1021 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst
--rw-r--r--   0        0        0       46 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/install-mandatory.bat
--rw-r--r--   0        0        0      127 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/pytest.ini
--rw-r--r--   0        0        0     1077 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json
--rw-r--r--   0        0        0     1518 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py
--rw-r--r--   0        0        0      941 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py
--rw-r--r--   0        0        0      617 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py
--rw-r--r--   0        0        0      348 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/tools/setup/git-config.ps1
--rw-r--r--   0        0        0      123 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/CMakeLists.txt
--rw-r--r--   0        0        0     7588 2024-04-02 12:32:36.766329 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png
--rw-r--r--   0        0        0      477 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/design.rst
--rw-r--r--   0        0        0      135 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/index.rst
--rw-r--r--   0        0        0      433 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.c
--rw-r--r--   0        0        0       40 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.h
--rw-r--r--   0        0        0     1048 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc
--rw-r--r--   0        0        0       68 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/CMakeLists.txt
--rw-r--r--   0        0        0      311 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/doc/index.rst
--rw-r--r--   0        0        0      272 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/src/main.c
--rw-r--r--   0        0        0      714 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake
--rw-r--r--   0        0        0      183 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/gcc/toolchain.cmake
--rw-r--r--   0        0        0       57 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/variant/cookiecutter.json
--rw-r--r--   0        0        0       94 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.cmake
--rw-r--r--   0        0        0       24 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.txt
--rw-r--r--   0        0        0       77 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/parts.cmake
--rw-r--r--   0        0        0      532 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/variant.py
--rw-r--r--   0        0        0     1279 2024-04-02 12:32:36.770330 spl_core-4.0.0/src/spl_core/project_creator/workspace_artifacts.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 spl_core-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-15 13:43:43.996442 spl_core-4.1.0/LICENSE
+-rw-r--r--   0        0        0      824 2024-04-15 13:43:43.996442 spl_core-4.1.0/README.md
+-rw-r--r--   0        0        0     4335 2024-04-15 13:43:44.936452 spl_core-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-15 13:43:44.936452 spl_core-4.1.0/src/spl_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/common/__init__.py
+-rw-r--r--   0        0        0     2054 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/common/cmake.py
+-rw-r--r--   0        0        0     2019 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/common/command_line_executor.py
+-rw-r--r--   0        0        0      462 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/common/path.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/gcov_maid/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/gcov_maid/gcov_maid.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/kconfig/__init__.py
+-rw-r--r--   0        0        0     9795 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/kconfig/kconfig.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/__init__.py
+-rw-r--r--   0        0        0     7342 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/creator.py
+-rw-r--r--   0        0        0      239 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0       33 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.flake8
+-rw-r--r--   0        0        0      599 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore
+-rw-r--r--   0        0        0      269 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-kits.json
+-rw-r--r--   0        0        0      718 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json
+-rw-r--r--   0        0        0      626 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json
+-rw-r--r--   0        0        0     1103 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json
+-rw-r--r--   0        0        0     1369 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json
+-rw-r--r--   0        0        0     2853 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json
+-rw-r--r--   0        0        0     1400 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt
+-rw-r--r--   0        0        0      598 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig
+-rw-r--r--   0        0        0     1108 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE
+-rw-r--r--   0        0        0      513 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/Pipfile
+-rw-r--r--   0        0        0      337 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/README.md
+-rw-r--r--   0        0        0       73 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.bat
+-rw-r--r--   0        0        0    10528 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1
+-rw-r--r--   0        0        0     6705 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py
+-rw-r--r--   0        0        0   123927 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in
+-rw-r--r--   0        0        0       90 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/common/index.rst
+-rw-r--r--   0        0        0      594 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst
+-rw-r--r--   0        0        0     1072 2024-04-15 13:43:44.000443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE
+-rw-r--r--   0        0        0    63071 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css
+-rw-r--r--   0        0        0       44 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_architecture/index.rst
+-rw-r--r--   0        0        0       95 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/software_requirements/index.rst
+-rw-r--r--   0        0        0     1217 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt
+-rw-r--r--   0        0        0     1021 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst
+-rw-r--r--   0        0        0       46 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/install-mandatory.bat
+-rw-r--r--   0        0        0      127 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/pytest.ini
+-rw-r--r--   0        0        0     1077 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json
+-rw-r--r--   0        0        0     1518 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py
+-rw-r--r--   0        0        0      941 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py
+-rw-r--r--   0        0        0      617 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py
+-rw-r--r--   0        0        0      348 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/tools/setup/git-config.ps1
+-rw-r--r--   0        0        0      123 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/CMakeLists.txt
+-rw-r--r--   0        0        0     7588 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png
+-rw-r--r--   0        0        0      477 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/design.rst
+-rw-r--r--   0        0        0      135 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/index.rst
+-rw-r--r--   0        0        0      433 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.c
+-rw-r--r--   0        0        0       40 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/src/component.h
+-rw-r--r--   0        0        0     1048 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc
+-rw-r--r--   0        0        0       68 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/CMakeLists.txt
+-rw-r--r--   0        0        0      311 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/doc/index.rst
+-rw-r--r--   0        0        0      272 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/main/src/main.c
+-rw-r--r--   0        0        0      714 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake
+-rw-r--r--   0        0        0      183 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/gcc/toolchain.cmake
+-rw-r--r--   0        0        0       57 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/variant/cookiecutter.json
+-rw-r--r--   0        0        0       94 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.cmake
+-rw-r--r--   0        0        0       24 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/config.txt
+-rw-r--r--   0        0        0       77 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/templates/variant/{{cookiecutter.flavor}}/{{cookiecutter.subsystem}}/parts.cmake
+-rw-r--r--   0        0        0      532 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/variant.py
+-rw-r--r--   0        0        0     1279 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/project_creator/workspace_artifacts.py
+-rw-r--r--   0        0        0     2256 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/test_utils/base_variant_test_runner.py
+-rw-r--r--   0        0        0     2172 2024-04-15 13:43:44.004443 spl_core-4.1.0/src/spl_core/test_utils/spl_build.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 spl_core-4.1.0/PKG-INFO
```

### Comparing `spl_core-4.0.0/LICENSE` & `spl_core-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/README.md` & `spl_core-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/pyproject.toml` & `spl_core-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spl-core"
-version = "4.0.0"
+version = "4.1.0"
 description = "Software Product Line Support for CMake"
 authors = ["Avengineers <karsten.guenther@kamg.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/avengineers/spl-core"
 documentation = "https://spl-core.readthedocs.io"
 classifiers = [
@@ -51,14 +51,15 @@
 doxysphinx = "*"
 sphinx-rtd-size = "*"
 sphinxcontrib-datatemplates = "*"
 sphinxcontrib-plantuml = "*"
 sphinx-copybutton = "*"
 sphinx-new-tab-link = "*"
 pipenv = "*"
+pypeline-runner = "^0.2.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `spl_core-4.0.0/src/spl_core/common/cmake.py` & `spl_core-4.1.0/src/spl_core/common/cmake.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/gcov_maid/gcov_maid.py` & `spl_core-4.1.0/src/spl_core/gcov_maid/gcov_maid.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/kconfig/kconfig.py` & `spl_core-4.1.0/src/spl_core/kconfig/kconfig.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/creator.py` & `spl_core-4.1.0/src/spl_core/project_creator/creator.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/cmake-variants.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/KConfig`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/build.ps1`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/conf.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/components/index.rst`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/doxygen-awesome/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/doc/test_report_template.txt`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/index.rst`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/scoopfile.json`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_build.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/test_unittests.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/test/utils.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/doc/_images/screenshot.png`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_components -%} components {%- endif %}/component/test/test_component.cc`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake` & `spl_core-4.1.0/src/spl_core/project_creator/templates/project/{{cookiecutter.name}}/{% if cookiecutter.touch_tools -%} tools {%- endif %}/toolchains/clang/toolchain.cmake`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/variant.py` & `spl_core-4.1.0/src/spl_core/project_creator/variant.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/src/spl_core/project_creator/workspace_artifacts.py` & `spl_core-4.1.0/src/spl_core/project_creator/workspace_artifacts.py`

 * *Files identical despite different names*

### Comparing `spl_core-4.0.0/PKG-INFO` & `spl_core-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spl-core
-Version: 4.0.0
+Version: 4.1.0
 Summary: Software Product Line Support for CMake
 Home-page: https://github.com/avengineers/spl-core
 License: MIT
 Author: Avengineers
 Author-email: karsten.guenther@kamg.de
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

