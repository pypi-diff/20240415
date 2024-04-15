# Comparing `tmp/autograder-3.7.6.tar.gz` & `tmp/autograder-3.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autograder-3.7.6.tar", max compression
+gzip compressed data, was "autograder-3.7.7.tar", max compression
```

## Comparing `autograder-3.7.6.tar` & `autograder-3.7.7.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0    35149 2022-09-05 19:55:36.738954 autograder-3.7.6/LICENSE
--rw-r--r--   0        0        0     3616 2023-09-02 17:15:05.940040 autograder-3.7.6/README.md
--rw-r--r--   0        0        0      293 2023-09-02 17:15:33.653374 autograder-3.7.6/autograder/__init__.py
--rw-r--r--   0        0        0     5161 2022-09-11 13:24:13.560384 autograder-3.7.6/autograder/__main__.py
--rwxr-xr-x   0        0        0    14468 2022-09-11 13:20:25.967043 autograder-3.7.6/autograder/autograder.py
--rw-r--r--   0        0        0     3681 2022-11-12 21:01:16.184324 autograder-3.7.6/autograder/config_manager.py
--rw-r--r--   0        0        0     1585 2022-11-12 21:01:16.184324 autograder-3.7.6/autograder/default_config.toml
--rw-r--r--   0        0        0     1592 2021-11-06 13:34:04.650139 autograder-3.7.6/autograder/default_stdout_formatters.py
--rw-r--r--   0        0        0     4224 2022-09-11 13:38:46.430414 autograder-3.7.6/autograder/guide.py
--rw-r--r--   0        0        0     5460 2022-09-05 21:52:16.892085 autograder-3.7.6/autograder/output_summary.py
--rw-r--r--   0        0        0       42 2021-11-06 13:33:47.767131 autograder-3.7.6/autograder/plagiarism_detection/__init__.py
--rw-r--r--   0        0        0      219 2022-09-10 19:33:29.180243 autograder-3.7.6/autograder/plagiarism_detection/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      217 2022-09-05 23:37:04.605237 autograder-3.7.6/autograder/plagiarism_detection/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      950 2022-09-10 19:33:29.290242 autograder-3.7.6/autograder/plagiarism_detection/__pycache__/comparison.cpython-310.pyc
--rw-r--r--   0        0        0      940 2022-09-05 23:37:04.665237 autograder-3.7.6/autograder/plagiarism_detection/__pycache__/comparison.cpython-38.pyc
--rw-r--r--   0        0        0     4557 2022-09-10 20:46:01.923024 autograder-3.7.6/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-310.pyc
--rw-r--r--   0        0        0     4545 2022-09-10 23:15:01.340636 autograder-3.7.6/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-38.pyc
--rw-r--r--   0        0        0      991 2022-01-21 16:45:36.894782 autograder-3.7.6/autograder/plagiarism_detection/comparison.py
--rw-r--r--   0        0        0    61144 2022-09-05 21:52:14.985419 autograder-3.7.6/autograder/plagiarism_detection/lexers/CLexer.py
--rw-r--r--   0        0        0    68274 2022-09-05 21:52:15.045419 autograder-3.7.6/autograder/plagiarism_detection/lexers/CppLexer.py
--rw-r--r--   0        0        0    48062 2022-09-05 21:52:15.088752 autograder-3.7.6/autograder/plagiarism_detection/lexers/Java8Lexer.py
--rw-r--r--   0        0        0    53591 2022-09-05 21:52:15.172085 autograder-3.7.6/autograder/plagiarism_detection/lexers/Python3Lexer.py
--rw-r--r--   0        0        0   321527 2022-09-05 21:52:23.902085 autograder-3.7.6/autograder/plagiarism_detection/lexers/Python3Parser.py
--rw-r--r--   0        0        0    33114 2022-09-10 19:33:29.440241 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-310.pyc
--rw-r--r--   0        0        0    34436 2022-09-05 23:37:04.795237 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-38.pyc
--rw-r--r--   0        0        0    36630 2022-09-10 19:33:29.460241 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-310.pyc
--rw-r--r--   0        0        0    38283 2022-09-05 23:37:04.808571 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-38.pyc
--rw-r--r--   0        0        0    26902 2022-09-10 19:33:29.476908 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-310.pyc
--rw-r--r--   0        0        0    28140 2022-09-05 23:37:04.825237 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-38.pyc
--rw-r--r--   0        0        0    32380 2022-09-10 19:33:29.493574 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-310.pyc
--rw-r--r--   0        0        0    33523 2022-09-05 23:37:04.835237 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-38.pyc
--rw-r--r--   0        0        0   212675 2022-09-10 19:33:29.526907 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-310.pyc
--rw-r--r--   0        0        0   240915 2022-09-05 23:37:04.871904 autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-38.pyc
--rw-r--r--   0        0        0     7039 2022-09-10 20:45:19.749922 autograder-3.7.6/autograder/plagiarism_detection/plagiarism_detection.py
--rw-r--r--   0        0        0     2989 2022-09-10 19:33:25.106932 autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-310.pyc
--rw-r--r--   0        0        0     2931 2022-09-05 21:53:10.398751 autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-37.pyc
--rw-r--r--   0        0        0     2962 2022-09-05 22:12:29.258717 autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-38.pyc
--rw-r--r--   0        0        0     3004 2021-10-09 21:09:14.154520 autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0      967 2022-09-11 15:01:57.513916 autograder-3.7.6/autograder/testcase_types/cpython/helpers/test_helper.py
--rw-r--r--   0        0        0     2535 2022-09-05 21:52:16.955419 autograder-3.7.6/autograder/testcase_types/cpython/python.py
--rw-r--r--   0        0        0      330 2022-11-15 20:28:39.940754 autograder-3.7.6/autograder/testcase_types/cpython/templates/__pycache__/sample_student_submission.cpython-310.pyc
--rw-r--r--   0        0        0      127 2022-09-11 11:11:16.770114 autograder-3.7.6/autograder/testcase_types/cpython/templates/sample_student_submission.py
--rw-r--r--   0        0        0        3 2022-09-11 11:07:21.840106 autograder-3.7.6/autograder/testcase_types/cpython/templates/tests/output/testcase_template2.txt
--rw-r--r--   0        0        0      435 2022-11-15 20:28:39.940754 autograder-3.7.6/autograder/testcase_types/cpython/templates/tests/testcases/__pycache__/testcase_template1.cpython-310.pyc
--rw-r--r--   0        0        0      377 2022-11-15 20:28:39.940754 autograder-3.7.6/autograder/testcase_types/cpython/templates/tests/testcases/__pycache__/testcase_template2.cpython-310.pyc
--rw-r--r--   0        0        0      542 2021-10-09 21:09:05.787862 autograder-3.7.6/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template1.py
--rw-r--r--   0        0        0      675 2021-10-09 21:09:05.787862 autograder-3.7.6/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template2.py
--rw-r--r--   0        0        0     5534 2022-09-10 19:33:25.106932 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-310.pyc
--rw-r--r--   0        0        0     5350 2022-09-05 21:53:10.398751 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-37.pyc
--rw-r--r--   0        0        0     5448 2022-09-05 22:12:29.262050 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-38.pyc
--rw-r--r--   0        0        0     2423 2021-10-09 21:09:14.151186 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-39.pyc
--rw-r--r--   0        0        0      712 2022-04-13 15:23:59.812404 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-310.pyc
--rw-r--r--   0        0        0      694 2021-11-06 13:45:35.760141 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-37.pyc
--rw-r--r--   0        0        0      708 2022-09-05 22:12:29.262050 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-38.pyc
--rw-r--r--   0        0        0      698 2021-10-09 21:09:14.151186 autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-39.pyc
--rw-r--r--   0        0        0      160 2022-09-11 11:21:28.940134 autograder-3.7.6/autograder/testcase_types/gcc/c++_templates/sample_student_submission.cpp
--rw-r--r--   0        0        0        3 2022-09-11 11:19:23.403463 autograder-3.7.6/autograder/testcase_types/gcc/c++_templates/tests/output/testcase_template2.txt
--rw-r--r--   0        0        0      711 2021-10-09 21:09:05.787862 autograder-3.7.6/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template1.cpp
--rw-r--r--   0        0        0      840 2021-10-09 21:09:05.787862 autograder-3.7.6/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template2.cpp
--rw-r--r--   0        0        0     6444 2022-09-05 21:52:19.555419 autograder-3.7.6/autograder/testcase_types/gcc/c.py
--rw-r--r--   0        0        0      160 2022-09-11 11:20:38.173466 autograder-3.7.6/autograder/testcase_types/gcc/c_templates/sample_student_submission.c
--rw-r--r--   0        0        0        3 2022-09-11 11:17:17.256793 autograder-3.7.6/autograder/testcase_types/gcc/c_templates/tests/output/testcase_template2.txt
--rw-r--r--   0        0        0      711 2022-09-11 11:18:40.240129 autograder-3.7.6/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template1.c
--rw-r--r--   0        0        0      840 2022-09-11 11:18:41.780129 autograder-3.7.6/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template2.c
--rw-r--r--   0        0        0      334 2021-11-06 13:34:04.656806 autograder-3.7.6/autograder/testcase_types/gcc/cpp.py
--rw-r--r--   0        0        0     1432 2021-11-06 13:34:04.656806 autograder-3.7.6/autograder/testcase_types/gcc/helpers/test_helper.c
--rw-r--r--   0        0        0     6119 2022-02-20 10:04:56.616976 autograder-3.7.6/autograder/testcase_types/gcc/memleak/memleak_detector.c
--rw-r--r--   0        0        0     1736 2022-01-20 15:25:56.194487 autograder-3.7.6/autograder/testcase_types/gcc/memleak/memleak_detector.h
--rw-r--r--   0        0        0     4842 2022-09-10 19:33:25.103598 autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-310.pyc
--rw-r--r--   0        0        0     4739 2022-09-05 21:53:10.395417 autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-37.pyc
--rw-r--r--   0        0        0     4806 2022-09-05 22:12:29.258717 autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-38.pyc
--rw-r--r--   0        0        0     4485 2021-10-09 21:09:14.147853 autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-39.pyc
--rw-r--r--   0        0        0   859016 2021-10-09 21:09:05.791195 autograder-3.7.6/autograder/testcase_types/javac/extra/jna.jar
--rw-r--r--   0        0        0     1988 2022-01-20 15:25:56.194487 autograder-3.7.6/autograder/testcase_types/javac/helpers/TestHelper.java
--rw-r--r--   0        0        0     5356 2022-09-05 21:52:16.955419 autograder-3.7.6/autograder/testcase_types/javac/java.py
--rw-r--r--   0        0        0      195 2022-09-11 11:32:34.956824 autograder-3.7.6/autograder/testcase_types/javac/templates/SampleHomework.java
--rw-r--r--   0        0        0        3 2022-09-11 11:23:57.383473 autograder-3.7.6/autograder/testcase_types/javac/templates/tests/output/TestCaseTemplate2.txt
--rw-r--r--   0        0        0      661 2022-09-11 11:31:25.900155 autograder-3.7.6/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate1.java
--rw-r--r--   0        0        0      782 2021-10-09 21:09:05.794529 autograder-3.7.6/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate2.java
--rw-r--r--   0        0        0        0 2021-10-09 21:09:05.794529 autograder-3.7.6/autograder/testcase_utils/__init__.py
--rw-r--r--   0        0        0      161 2022-04-13 15:23:59.782389 autograder-3.7.6/autograder/testcase_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      155 2022-02-13 18:29:25.062875 autograder-3.7.6/autograder/testcase_utils/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      159 2022-09-05 22:12:29.245384 autograder-3.7.6/autograder/testcase_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     8946 2022-11-15 20:28:39.944087 autograder-3.7.6/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-310.pyc
--rw-r--r--   0        0        0     8789 2022-09-05 21:53:10.385417 autograder-3.7.6/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-37.pyc
--rw-r--r--   0        0        0     8929 2022-10-09 15:54:12.476564 autograder-3.7.6/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-38.pyc
--rw-r--r--   0        0        0      836 2022-09-10 19:33:25.090265 autograder-3.7.6/autograder/testcase_utils/__pycache__/exit_codes.cpython-310.pyc
--rw-r--r--   0        0        0      882 2022-02-13 18:29:25.066209 autograder-3.7.6/autograder/testcase_utils/__pycache__/exit_codes.cpython-37.pyc
--rw-r--r--   0        0        0     1000 2022-09-10 10:51:30.363403 autograder-3.7.6/autograder/testcase_utils/__pycache__/exit_codes.cpython-38.pyc
--rw-r--r--   0        0        0     3857 2022-09-10 22:52:27.414732 autograder-3.7.6/autograder/testcase_utils/__pycache__/shell.cpython-310.pyc
--rw-r--r--   0        0        0     3770 2022-09-05 21:53:10.385417 autograder-3.7.6/autograder/testcase_utils/__pycache__/shell.cpython-37.pyc
--rw-r--r--   0        0        0     3851 2022-09-10 23:14:56.230664 autograder-3.7.6/autograder/testcase_utils/__pycache__/shell.cpython-38.pyc
--rw-r--r--   0        0        0     8015 2022-09-10 19:45:46.589529 autograder-3.7.6/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-310.pyc
--rw-r--r--   0        0        0     7765 2022-09-05 21:53:10.388751 autograder-3.7.6/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-37.pyc
--rw-r--r--   0        0        0     7924 2022-09-10 23:14:56.237331 autograder-3.7.6/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-38.pyc
--rw-r--r--   0        0        0     3522 2022-09-10 21:04:49.873501 autograder-3.7.6/autograder/testcase_utils/__pycache__/submission.cpython-310.pyc
--rw-r--r--   0        0        0     3071 2022-04-18 19:12:50.958380 autograder-3.7.6/autograder/testcase_utils/__pycache__/submission.cpython-37.pyc
--rw-r--r--   0        0        0     3500 2022-09-10 23:14:56.230664 autograder-3.7.6/autograder/testcase_utils/__pycache__/submission.cpython-38.pyc
--rw-r--r--   0        0        0     1736 2022-09-10 19:33:25.093598 autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0        0        0     1627 2022-04-13 15:23:59.792394 autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310.pyc
--rw-r--r--   0        0        0     1579 2022-02-13 18:29:25.066209 autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-37.pyc
--rw-r--r--   0        0        0     1722 2022-09-05 23:25:00.105258 autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38-pytest-7.1.3.pyc
--rw-r--r--   0        0        0     1609 2022-09-05 22:12:29.248717 autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2022-04-18 19:45:17.481634 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_io.cpython-310.pyc
--rw-r--r--   0        0        0     2185 2022-04-13 19:57:32.485201 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_io.cpython-37.pyc
--rw-r--r--   0        0        0     2218 2022-09-05 22:12:29.248717 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_io.cpython-38.pyc
--rw-r--r--   0        0        0     2000 2022-09-10 19:33:25.096932 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_picker.cpython-310.pyc
--rw-r--r--   0        0        0     1966 2022-09-05 21:53:10.388751 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_picker.cpython-37.pyc
--rw-r--r--   0        0        0     1988 2022-09-05 22:12:29.252050 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_picker.cpython-38.pyc
--rw-r--r--   0        0        0     1534 2022-11-15 20:28:39.944087 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1513 2022-02-13 18:29:25.066209 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-37.pyc
--rw-r--r--   0        0        0     1535 2022-10-09 15:54:12.479897 autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-38.pyc
--rw-r--r--   0        0        0    10084 2022-10-09 16:10:28.209869 autograder-3.7.6/autograder/testcase_utils/abstract_testcase.py
--rw-r--r--   0        0        0      592 2022-09-08 23:21:17.730053 autograder-3.7.6/autograder/testcase_utils/exit_codes.py
--rw-r--r--   0        0        0     3791 2022-09-10 21:47:28.899458 autograder-3.7.6/autograder/testcase_utils/shell.py
--rw-r--r--   0        0        0     9788 2022-09-10 19:45:19.486345 autograder-3.7.6/autograder/testcase_utils/stdout_testcase.py
--rw-r--r--   0        0        0     3154 2022-09-10 20:48:22.798917 autograder-3.7.6/autograder/testcase_utils/submission.py
--rw-r--r--   0        0        0     1355 2022-01-21 16:45:39.461210 autograder-3.7.6/autograder/testcase_utils/test_helper_formatter.py
--rw-r--r--   0        0        0     2128 2022-04-13 19:48:21.759986 autograder-3.7.6/autograder/testcase_utils/testcase_io.py
--rw-r--r--   0        0        0     1896 2022-09-05 21:52:16.912085 autograder-3.7.6/autograder/testcase_utils/testcase_picker.py
--rw-r--r--   0        0        0     1624 2022-09-11 15:02:08.527250 autograder-3.7.6/autograder/testcase_utils/testcase_result_validator.py
--rw-r--r--   0        0        0     2016 2022-09-11 13:02:08.843672 autograder-3.7.6/autograder/util.py
--rw-r--r--   0        0        0     2210 2023-09-02 17:15:44.833374 autograder-3.7.6/pyproject.toml
--rw-r--r--   0        0        0     5736 1970-01-01 00:00:00.000000 autograder-3.7.6/setup.py
--rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 autograder-3.7.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-05 19:55:36.738954 autograder-3.7.7/LICENSE
+-rw-r--r--   0        0        0     3580 2024-02-08 20:10:31.226726 autograder-3.7.7/README.md
+-rw-r--r--   0        0        0      293 2023-09-02 17:15:33.653374 autograder-3.7.7/autograder/__init__.py
+-rw-r--r--   0        0        0     5161 2022-09-11 13:24:13.560384 autograder-3.7.7/autograder/__main__.py
+-rwxr-xr-x   0        0        0    14468 2022-09-11 13:20:25.967043 autograder-3.7.7/autograder/autograder.py
+-rw-r--r--   0        0        0     3681 2022-11-12 21:01:16.184324 autograder-3.7.7/autograder/config_manager.py
+-rw-r--r--   0        0        0     1585 2022-11-12 21:01:16.184324 autograder-3.7.7/autograder/default_config.toml
+-rw-r--r--   0        0        0     1592 2021-11-06 13:34:04.650139 autograder-3.7.7/autograder/default_stdout_formatters.py
+-rw-r--r--   0        0        0     4434 2024-02-08 20:10:31.433392 autograder-3.7.7/autograder/guide.py
+-rw-r--r--   0        0        0     5460 2022-09-05 21:52:16.892085 autograder-3.7.7/autograder/output_summary.py
+-rw-r--r--   0        0        0       42 2021-11-06 13:33:47.767131 autograder-3.7.7/autograder/plagiarism_detection/__init__.py
+-rw-r--r--   0        0        0      219 2022-09-10 19:33:29.180243 autograder-3.7.7/autograder/plagiarism_detection/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      217 2022-09-05 23:37:04.605237 autograder-3.7.7/autograder/plagiarism_detection/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      950 2022-09-10 19:33:29.290242 autograder-3.7.7/autograder/plagiarism_detection/__pycache__/comparison.cpython-310.pyc
+-rw-r--r--   0        0        0      940 2022-09-05 23:37:04.665237 autograder-3.7.7/autograder/plagiarism_detection/__pycache__/comparison.cpython-38.pyc
+-rw-r--r--   0        0        0     4557 2022-09-10 20:46:01.923024 autograder-3.7.7/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-310.pyc
+-rw-r--r--   0        0        0     4545 2022-09-10 23:15:01.340636 autograder-3.7.7/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-38.pyc
+-rw-r--r--   0        0        0      991 2022-01-21 16:45:36.894782 autograder-3.7.7/autograder/plagiarism_detection/comparison.py
+-rw-r--r--   0        0        0    61144 2022-09-05 21:52:14.985419 autograder-3.7.7/autograder/plagiarism_detection/lexers/CLexer.py
+-rw-r--r--   0        0        0    68274 2022-09-05 21:52:15.045419 autograder-3.7.7/autograder/plagiarism_detection/lexers/CppLexer.py
+-rw-r--r--   0        0        0    48062 2022-09-05 21:52:15.088752 autograder-3.7.7/autograder/plagiarism_detection/lexers/Java8Lexer.py
+-rw-r--r--   0        0        0    53591 2022-09-05 21:52:15.172085 autograder-3.7.7/autograder/plagiarism_detection/lexers/Python3Lexer.py
+-rw-r--r--   0        0        0   321527 2022-09-05 21:52:23.902085 autograder-3.7.7/autograder/plagiarism_detection/lexers/Python3Parser.py
+-rw-r--r--   0        0        0    33114 2022-09-10 19:33:29.440241 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-310.pyc
+-rw-r--r--   0        0        0    34436 2022-09-05 23:37:04.795237 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-38.pyc
+-rw-r--r--   0        0        0    36630 2022-09-10 19:33:29.460241 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-310.pyc
+-rw-r--r--   0        0        0    38283 2022-09-05 23:37:04.808571 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-38.pyc
+-rw-r--r--   0        0        0    26902 2022-09-10 19:33:29.476908 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-310.pyc
+-rw-r--r--   0        0        0    28140 2022-09-05 23:37:04.825237 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-38.pyc
+-rw-r--r--   0        0        0    32380 2022-09-10 19:33:29.493574 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-310.pyc
+-rw-r--r--   0        0        0    33523 2022-09-05 23:37:04.835237 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-38.pyc
+-rw-r--r--   0        0        0   212675 2022-09-10 19:33:29.526907 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-310.pyc
+-rw-r--r--   0        0        0   240915 2022-09-05 23:37:04.871904 autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-38.pyc
+-rw-r--r--   0        0        0     7039 2022-09-10 20:45:19.749922 autograder-3.7.7/autograder/plagiarism_detection/plagiarism_detection.py
+-rw-r--r--   0        0        0     2989 2022-09-10 19:33:25.106932 autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-310.pyc
+-rw-r--r--   0        0        0     2931 2022-09-05 21:53:10.398751 autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-37.pyc
+-rw-r--r--   0        0        0     2962 2022-09-05 22:12:29.258717 autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-38.pyc
+-rw-r--r--   0        0        0     3004 2021-10-09 21:09:14.154520 autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0      967 2022-09-11 15:01:57.513916 autograder-3.7.7/autograder/testcase_types/cpython/helpers/test_helper.py
+-rw-r--r--   0        0        0     2535 2022-09-05 21:52:16.955419 autograder-3.7.7/autograder/testcase_types/cpython/python.py
+-rw-r--r--   0        0        0      330 2022-11-15 20:28:39.940754 autograder-3.7.7/autograder/testcase_types/cpython/templates/__pycache__/sample_student_submission.cpython-310.pyc
+-rw-r--r--   0        0        0      127 2022-09-11 11:11:16.770114 autograder-3.7.7/autograder/testcase_types/cpython/templates/sample_student_submission.py
+-rw-r--r--   0        0        0        3 2022-09-11 11:07:21.840106 autograder-3.7.7/autograder/testcase_types/cpython/templates/tests/output/testcase_template2.txt
+-rw-r--r--   0        0        0      435 2022-11-15 20:28:39.940754 autograder-3.7.7/autograder/testcase_types/cpython/templates/tests/testcases/__pycache__/testcase_template1.cpython-310.pyc
+-rw-r--r--   0        0        0      377 2022-11-15 20:28:39.940754 autograder-3.7.7/autograder/testcase_types/cpython/templates/tests/testcases/__pycache__/testcase_template2.cpython-310.pyc
+-rw-r--r--   0        0        0      542 2021-10-09 21:09:05.787862 autograder-3.7.7/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template1.py
+-rw-r--r--   0        0        0      675 2021-10-09 21:09:05.787862 autograder-3.7.7/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template2.py
+-rw-r--r--   0        0        0     5534 2022-09-10 19:33:25.106932 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-310.pyc
+-rw-r--r--   0        0        0     5350 2022-09-05 21:53:10.398751 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-37.pyc
+-rw-r--r--   0        0        0     5448 2022-09-05 22:12:29.262050 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-38.pyc
+-rw-r--r--   0        0        0     2423 2021-10-09 21:09:14.151186 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-39.pyc
+-rw-r--r--   0        0        0      712 2022-04-13 15:23:59.812404 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-310.pyc
+-rw-r--r--   0        0        0      694 2021-11-06 13:45:35.760141 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-37.pyc
+-rw-r--r--   0        0        0      708 2022-09-05 22:12:29.262050 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-38.pyc
+-rw-r--r--   0        0        0      698 2021-10-09 21:09:14.151186 autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-39.pyc
+-rw-r--r--   0        0        0      160 2022-09-11 11:21:28.940134 autograder-3.7.7/autograder/testcase_types/gcc/c++_templates/sample_student_submission.cpp
+-rw-r--r--   0        0        0        3 2022-09-11 11:19:23.403463 autograder-3.7.7/autograder/testcase_types/gcc/c++_templates/tests/output/testcase_template2.txt
+-rw-r--r--   0        0        0      711 2021-10-09 21:09:05.787862 autograder-3.7.7/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template1.cpp
+-rw-r--r--   0        0        0      840 2021-10-09 21:09:05.787862 autograder-3.7.7/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template2.cpp
+-rw-r--r--   0        0        0     6444 2022-09-05 21:52:19.555419 autograder-3.7.7/autograder/testcase_types/gcc/c.py
+-rw-r--r--   0        0        0      160 2022-09-11 11:20:38.173466 autograder-3.7.7/autograder/testcase_types/gcc/c_templates/sample_student_submission.c
+-rw-r--r--   0        0        0        3 2022-09-11 11:17:17.256793 autograder-3.7.7/autograder/testcase_types/gcc/c_templates/tests/output/testcase_template2.txt
+-rw-r--r--   0        0        0      711 2022-09-11 11:18:40.240129 autograder-3.7.7/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template1.c
+-rw-r--r--   0        0        0      840 2022-09-11 11:18:41.780129 autograder-3.7.7/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template2.c
+-rw-r--r--   0        0        0      334 2021-11-06 13:34:04.656806 autograder-3.7.7/autograder/testcase_types/gcc/cpp.py
+-rw-r--r--   0        0        0     1432 2021-11-06 13:34:04.656806 autograder-3.7.7/autograder/testcase_types/gcc/helpers/test_helper.c
+-rw-r--r--   0        0        0     6119 2022-02-20 10:04:56.616976 autograder-3.7.7/autograder/testcase_types/gcc/memleak/memleak_detector.c
+-rw-r--r--   0        0        0     1736 2022-01-20 15:25:56.194487 autograder-3.7.7/autograder/testcase_types/gcc/memleak/memleak_detector.h
+-rw-r--r--   0        0        0     4842 2022-09-10 19:33:25.103598 autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-310.pyc
+-rw-r--r--   0        0        0     4739 2022-09-05 21:53:10.395417 autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-37.pyc
+-rw-r--r--   0        0        0     4806 2022-09-05 22:12:29.258717 autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-38.pyc
+-rw-r--r--   0        0        0     4485 2021-10-09 21:09:14.147853 autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-39.pyc
+-rw-r--r--   0        0        0   859016 2021-10-09 21:09:05.791195 autograder-3.7.7/autograder/testcase_types/javac/extra/jna.jar
+-rw-r--r--   0        0        0     1988 2022-01-20 15:25:56.194487 autograder-3.7.7/autograder/testcase_types/javac/helpers/TestHelper.java
+-rw-r--r--   0        0        0     5356 2022-09-05 21:52:16.955419 autograder-3.7.7/autograder/testcase_types/javac/java.py
+-rw-r--r--   0        0        0      195 2022-09-11 11:32:34.956824 autograder-3.7.7/autograder/testcase_types/javac/templates/SampleHomework.java
+-rw-r--r--   0        0        0        3 2022-09-11 11:23:57.383473 autograder-3.7.7/autograder/testcase_types/javac/templates/tests/output/TestCaseTemplate2.txt
+-rw-r--r--   0        0        0      661 2022-09-11 11:31:25.900155 autograder-3.7.7/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate1.java
+-rw-r--r--   0        0        0      782 2021-10-09 21:09:05.794529 autograder-3.7.7/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate2.java
+-rw-r--r--   0        0        0        0 2021-10-09 21:09:05.794529 autograder-3.7.7/autograder/testcase_utils/__init__.py
+-rw-r--r--   0        0        0      161 2022-04-13 15:23:59.782389 autograder-3.7.7/autograder/testcase_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      155 2022-02-13 18:29:25.062875 autograder-3.7.7/autograder/testcase_utils/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      159 2022-09-05 22:12:29.245384 autograder-3.7.7/autograder/testcase_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8946 2022-11-15 20:28:39.944087 autograder-3.7.7/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-310.pyc
+-rw-r--r--   0        0        0     8789 2022-09-05 21:53:10.385417 autograder-3.7.7/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-37.pyc
+-rw-r--r--   0        0        0     8929 2022-10-09 15:54:12.476564 autograder-3.7.7/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-38.pyc
+-rw-r--r--   0        0        0      836 2022-09-10 19:33:25.090265 autograder-3.7.7/autograder/testcase_utils/__pycache__/exit_codes.cpython-310.pyc
+-rw-r--r--   0        0        0      882 2022-02-13 18:29:25.066209 autograder-3.7.7/autograder/testcase_utils/__pycache__/exit_codes.cpython-37.pyc
+-rw-r--r--   0        0        0     1000 2022-09-10 10:51:30.363403 autograder-3.7.7/autograder/testcase_utils/__pycache__/exit_codes.cpython-38.pyc
+-rw-r--r--   0        0        0     3857 2022-09-10 22:52:27.414732 autograder-3.7.7/autograder/testcase_utils/__pycache__/shell.cpython-310.pyc
+-rw-r--r--   0        0        0     3770 2022-09-05 21:53:10.385417 autograder-3.7.7/autograder/testcase_utils/__pycache__/shell.cpython-37.pyc
+-rw-r--r--   0        0        0     3851 2022-09-10 23:14:56.230664 autograder-3.7.7/autograder/testcase_utils/__pycache__/shell.cpython-38.pyc
+-rw-r--r--   0        0        0     8015 2022-09-10 19:45:46.589529 autograder-3.7.7/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-310.pyc
+-rw-r--r--   0        0        0     7765 2022-09-05 21:53:10.388751 autograder-3.7.7/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-37.pyc
+-rw-r--r--   0        0        0     7924 2022-09-10 23:14:56.237331 autograder-3.7.7/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-38.pyc
+-rw-r--r--   0        0        0     3522 2022-09-10 21:04:49.873501 autograder-3.7.7/autograder/testcase_utils/__pycache__/submission.cpython-310.pyc
+-rw-r--r--   0        0        0     3071 2022-04-18 19:12:50.958380 autograder-3.7.7/autograder/testcase_utils/__pycache__/submission.cpython-37.pyc
+-rw-r--r--   0        0        0     3500 2022-09-10 23:14:56.230664 autograder-3.7.7/autograder/testcase_utils/__pycache__/submission.cpython-38.pyc
+-rw-r--r--   0        0        0     1736 2022-09-10 19:33:25.093598 autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     1736 2024-04-15 04:10:09.804780 autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310-pytest-7.4.4.pyc
+-rw-r--r--   0        0        0     1627 2022-04-13 15:23:59.792394 autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310.pyc
+-rw-r--r--   0        0        0     1579 2022-02-13 18:29:25.066209 autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-37.pyc
+-rw-r--r--   0        0        0     1722 2022-09-05 23:25:00.105258 autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     1609 2022-09-05 22:12:29.248717 autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2022-04-18 19:45:17.481634 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_io.cpython-310.pyc
+-rw-r--r--   0        0        0     2185 2022-04-13 19:57:32.485201 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_io.cpython-37.pyc
+-rw-r--r--   0        0        0     2218 2022-09-05 22:12:29.248717 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_io.cpython-38.pyc
+-rw-r--r--   0        0        0     2000 2022-09-10 19:33:25.096932 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_picker.cpython-310.pyc
+-rw-r--r--   0        0        0     1966 2022-09-05 21:53:10.388751 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_picker.cpython-37.pyc
+-rw-r--r--   0        0        0     1988 2022-09-05 22:12:29.252050 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_picker.cpython-38.pyc
+-rw-r--r--   0        0        0     1534 2022-11-15 20:28:39.944087 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1513 2022-02-13 18:29:25.066209 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-37.pyc
+-rw-r--r--   0        0        0     1535 2022-10-09 15:54:12.479897 autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-38.pyc
+-rw-r--r--   0        0        0    10084 2022-10-09 16:10:28.209869 autograder-3.7.7/autograder/testcase_utils/abstract_testcase.py
+-rw-r--r--   0        0        0      592 2022-09-08 23:21:17.730053 autograder-3.7.7/autograder/testcase_utils/exit_codes.py
+-rw-r--r--   0        0        0     3791 2022-09-10 21:47:28.899458 autograder-3.7.7/autograder/testcase_utils/shell.py
+-rw-r--r--   0        0        0     9788 2022-09-10 19:45:19.486345 autograder-3.7.7/autograder/testcase_utils/stdout_testcase.py
+-rw-r--r--   0        0        0     3154 2022-09-10 20:48:22.798917 autograder-3.7.7/autograder/testcase_utils/submission.py
+-rw-r--r--   0        0        0     1355 2022-01-21 16:45:39.461210 autograder-3.7.7/autograder/testcase_utils/test_helper_formatter.py
+-rw-r--r--   0        0        0     2128 2022-04-13 19:48:21.759986 autograder-3.7.7/autograder/testcase_utils/testcase_io.py
+-rw-r--r--   0        0        0     1896 2022-09-05 21:52:16.912085 autograder-3.7.7/autograder/testcase_utils/testcase_picker.py
+-rw-r--r--   0        0        0     1624 2022-09-11 15:02:08.527250 autograder-3.7.7/autograder/testcase_utils/testcase_result_validator.py
+-rw-r--r--   0        0        0     2016 2022-09-11 13:02:08.843672 autograder-3.7.7/autograder/util.py
+-rw-r--r--   0        0        0     2203 2024-04-15 04:14:39.816632 autograder-3.7.7/pyproject.toml
+-rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 autograder-3.7.7/PKG-INFO
```

### Comparing `autograder-3.7.6/LICENSE` & `autograder-3.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/README.md` & `autograder-3.7.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 <p align="center">
-  <a href="https://ovsyanka83.github.io/autograder/"><img src="https://raw.githubusercontent.com/Ovsyanka83/autograder/main/docs/_media/logo_with_text.svg" alt="AutoGrader"></a>
+  <a href="https://zmievsa.github.io/autograder/"><img src="https://raw.githubusercontent.com/zmievsa/autograder/main/docs/_media/logo_with_text.svg" alt="AutoGrader"></a>
 </p>
 <p align="center">
   <b>A simple, secure, and versatile way to automatically grade programming assignments</b>
 </p>
 
 ---
 
 <p align="center">
-<a href="https://github.com/ovsyanka83/autograder/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
-    <img src="https://github.com/Ovsyanka83/autograder/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
+<a href="https://github.com/zmievsa/autograder/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
+    <img src="https://github.com/zmievsa/autograder/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
 </a>
-<a href="https://codecov.io/gh/ovsyanka83/autograder" target="_blank">
-    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/autograder?color=%2334D058" alt="Coverage">
+<a href="https://codecov.io/gh/zmievsa/autograder" target="_blank">
+    <img src="https://img.shields.io/codecov/c/github/zmievsa/autograder?color=%2334D058" alt="Coverage">
 </a>
 <a href="https://pypi.org/project/autograder/" target="_blank">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autograder?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/autograder/" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/autograder?color=%2334D058" alt="Supported Python versions">
 </a>
 </p>
 
 ## Features
 
 * Blazingly fast (can grade hundreads of submissions using dozens of testcases in a few minutes. Seconds if grading python)
-* [Easy to grade](https://ovsyanka83.github.io/autograder/#/?id=usage)
-* [Easy-to-write testcases](https://ovsyanka83.github.io/autograder/#/?id=writing-testcases)  
-* Testcase grade can be based on [student's stdout](https://ovsyanka83.github.io/autograder/#/?id=helper-functions)
+* [Easy to grade](https://zmievsa.github.io/autograder/#/?id=usage)
+* [Easy-to-write testcases](https://zmievsa.github.io/autograder/#/?id=writing-testcases)  
+* Testcase grade can be based on [student's stdout](https://zmievsa.github.io/autograder/#/?id=helper-functions)
 * Can grade C, C++, Java, and Python code in regular mode
 * Can grade any programming language in stdout-only mode
 * A file with testcase grades and details can be generated for each student
-* You can customize the total points for the assignment, maximum running time of student's program, file names to be considered for grading, formatters for checking student stdout, and [so much more](https://github.com/Ovsyanka83/autograder/blob/master/autograder/default_config.toml).
-* [Anti Cheating capabilities](https://ovsyanka83.github.io/autograder/#/?id=anti-cheating) that make it nearly impossible for students to cheat
+* You can customize the total points for the assignment, maximum running time of student's program, file names to be considered for grading, formatters for checking student stdout, and [so much more](https://github.com/zmievsa/autograder/blob/master/autograder/default_config.toml).
+* [Anti Cheating capabilities](https://zmievsa.github.io/autograder/#/?id=anti-cheating) that make it nearly impossible for students to cheat
 * Grading submissions in multiple programming languages at once
 * JSON result output supported if autograder needs to be integrated as a part of a larger utility
 * Can check submissions for similarity (plagiarism)
 * Can detect and report memory leaks in C/C++ code
 
 ## Installation
 
@@ -50,15 +50,15 @@
 ### Updates
 
 `pip install -U --no-cache-dir autograder`
 
 ## Quickstart
 
 * Run `autograder guide path/to/directory/you'd/like/to/grade`. The guide will create all of the necessary configurations and directories for grading and will explain how to grade.
-* Read the [usage](https://ovsyanka83.github.io/autograder/#/?id=usage) section of the docs
+* Read the [usage](https://zmievsa.github.io/autograder/#/?id=usage) section of the docs
 
 ## Supported Platforms
 
 * Linux is fully supported
 * OS X is fully supported
 * Windows is partially supported:
   * Stdout-testcases that require shebang lines are not and cannot be supported
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
                                  _[_A_u_t_o_G_r_a_d_e_r_]
     AA ssiimmppllee,, sseeccuurree,, aanndd vveerrssaattiillee wwaayy ttoo aauuttoommaattiiccaallllyy ggrraaddee pprrooggrraammmmiinngg
                                   aassssiiggnnmmeennttss
 ---
                _[_T_e_s_t_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 ## Features * Blazingly fast (can grade hundreads of submissions using dozens
 of testcases in a few minutes. Seconds if grading python) * [Easy to grade]
-(https://ovsyanka83.github.io/autograder/#/?id=usage) * [Easy-to-write
-testcases](https://ovsyanka83.github.io/autograder/#/?id=writing-testcases) *
-Testcase grade can be based on [student's stdout](https://ovsyanka83.github.io/
-autograder/#/?id=helper-functions) * Can grade C, C++, Java, and Python code in
-regular mode * Can grade any programming language in stdout-only mode * A file
-with testcase grades and details can be generated for each student * You can
-customize the total points for the assignment, maximum running time of
-student's program, file names to be considered for grading, formatters for
-checking student stdout, and [so much more](https://github.com/Ovsyanka83/
-autograder/blob/master/autograder/default_config.toml). * [Anti Cheating
-capabilities](https://ovsyanka83.github.io/autograder/#/?id=anti-cheating) that
-make it nearly impossible for students to cheat * Grading submissions in
-multiple programming languages at once * JSON result output supported if
-autograder needs to be integrated as a part of a larger utility * Can check
-submissions for similarity (plagiarism) * Can detect and report memory leaks in
-C/C++ code ## Installation * Run `pip install autograder` * To grade various
-programming languages, you'd need to install: * `gcc`/`clang` for C/C++ support
-* `Java JDK` for java support * `make` for compiled stdout-only testcase
-support * Any interpreter/compiler necessary to run stdout-only testcases. For
-example, testcases with ruby in their shebang lines will require the ruby
-interpreter ### Updates `pip install -U --no-cache-dir autograder` ##
-Quickstart * Run `autograder guide path/to/directory/you'd/like/to/grade`. The
-guide will create all of the necessary configurations and directories for
-grading and will explain how to grade. * Read the [usage](https://
-ovsyanka83.github.io/autograder/#/?id=usage) section of the docs ## Supported
-Platforms * Linux is fully supported * OS X is fully supported * Windows is
-partially supported: * Stdout-testcases that require shebang lines are not and
-cannot be supported ## Supported Programming Languages * Java * C * C++ *
-CPython (3.8-3.11) * Any programming language if stdout-only grading is used
+(https://zmievsa.github.io/autograder/#/?id=usage) * [Easy-to-write testcases]
+(https://zmievsa.github.io/autograder/#/?id=writing-testcases) * Testcase grade
+can be based on [student's stdout](https://zmievsa.github.io/autograder/#/
+?id=helper-functions) * Can grade C, C++, Java, and Python code in regular mode
+* Can grade any programming language in stdout-only mode * A file with testcase
+grades and details can be generated for each student * You can customize the
+total points for the assignment, maximum running time of student's program,
+file names to be considered for grading, formatters for checking student
+stdout, and [so much more](https://github.com/zmievsa/autograder/blob/master/
+autograder/default_config.toml). * [Anti Cheating capabilities](https://
+zmievsa.github.io/autograder/#/?id=anti-cheating) that make it nearly
+impossible for students to cheat * Grading submissions in multiple programming
+languages at once * JSON result output supported if autograder needs to be
+integrated as a part of a larger utility * Can check submissions for similarity
+(plagiarism) * Can detect and report memory leaks in C/C++ code ## Installation
+* Run `pip install autograder` * To grade various programming languages, you'd
+need to install: * `gcc`/`clang` for C/C++ support * `Java JDK` for java
+support * `make` for compiled stdout-only testcase support * Any interpreter/
+compiler necessary to run stdout-only testcases. For example, testcases with
+ruby in their shebang lines will require the ruby interpreter ### Updates `pip
+install -U --no-cache-dir autograder` ## Quickstart * Run `autograder guide
+path/to/directory/you'd/like/to/grade`. The guide will create all of the
+necessary configurations and directories for grading and will explain how to
+grade. * Read the [usage](https://zmievsa.github.io/autograder/#/?id=usage)
+section of the docs ## Supported Platforms * Linux is fully supported * OS X is
+fully supported * Windows is partially supported: * Stdout-testcases that
+require shebang lines are not and cannot be supported ## Supported Programming
+Languages * Java * C * C++ * CPython (3.8-3.11) * Any programming language if
+stdout-only grading is used
```

### Comparing `autograder-3.7.6/autograder/__main__.py` & `autograder-3.7.7/autograder/__main__.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/autograder.py` & `autograder-3.7.7/autograder/autograder.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/config_manager.py` & `autograder-3.7.7/autograder/config_manager.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/default_config.toml` & `autograder-3.7.7/autograder/default_config.toml`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/default_stdout_formatters.py` & `autograder-3.7.7/autograder/default_stdout_formatters.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/output_summary.py` & `autograder-3.7.7/autograder/output_summary.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/__pycache__/comparison.cpython-310.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/__pycache__/comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/__pycache__/comparison.cpython-38.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/__pycache__/comparison.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-310.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-38.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/__pycache__/plagiarism_detection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/comparison.py` & `autograder-3.7.7/autograder/plagiarism_detection/comparison.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/CLexer.py` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/CLexer.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/CppLexer.py` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/CppLexer.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/Java8Lexer.py` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/Java8Lexer.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/Python3Lexer.py` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/Python3Parser.py` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-310.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-38.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CLexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-310.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-38.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/CppLexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-310.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-38.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Java8Lexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-310.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-38.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Lexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-310.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-38.pyc` & `autograder-3.7.7/autograder/plagiarism_detection/lexers/__pycache__/Python3Parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/plagiarism_detection/plagiarism_detection.py` & `autograder-3.7.7/autograder/plagiarism_detection/plagiarism_detection.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/__pycache__/python.cpython-39.pyc` & `autograder-3.7.7/autograder/testcase_types/cpython/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/helpers/test_helper.py` & `autograder-3.7.7/autograder/testcase_types/cpython/helpers/test_helper.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/python.py` & `autograder-3.7.7/autograder/testcase_types/cpython/python.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template1.py` & `autograder-3.7.7/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template1.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template2.py` & `autograder-3.7.7/autograder/testcase_types/cpython/templates/tests/testcases/testcase_template2.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/c.cpython-39.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/c.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/__pycache__/cpp.cpython-39.pyc` & `autograder-3.7.7/autograder/testcase_types/gcc/__pycache__/cpp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template1.cpp` & `autograder-3.7.7/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template1.cpp`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template2.cpp` & `autograder-3.7.7/autograder/testcase_types/gcc/c++_templates/tests/testcases/testcase_template2.cpp`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/c.py` & `autograder-3.7.7/autograder/testcase_types/gcc/c.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template1.c` & `autograder-3.7.7/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template1.c`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template2.c` & `autograder-3.7.7/autograder/testcase_types/gcc/c_templates/tests/testcases/testcase_template2.c`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/helpers/test_helper.c` & `autograder-3.7.7/autograder/testcase_types/gcc/helpers/test_helper.c`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/memleak/memleak_detector.c` & `autograder-3.7.7/autograder/testcase_types/gcc/memleak/memleak_detector.c`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/gcc/memleak/memleak_detector.h` & `autograder-3.7.7/autograder/testcase_types/gcc/memleak/memleak_detector.h`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/__pycache__/java.cpython-39.pyc` & `autograder-3.7.7/autograder/testcase_types/javac/__pycache__/java.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/extra/jna.jar` & `autograder-3.7.7/autograder/testcase_types/javac/extra/jna.jar`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/helpers/TestHelper.java` & `autograder-3.7.7/autograder/testcase_types/javac/helpers/TestHelper.java`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/java.py` & `autograder-3.7.7/autograder/testcase_types/javac/java.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate1.java` & `autograder-3.7.7/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate1.java`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate2.java` & `autograder-3.7.7/autograder/testcase_types/javac/templates/tests/testcases/TestCaseTemplate2.java`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/abstract_testcase.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/exit_codes.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/exit_codes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/exit_codes.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/exit_codes.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/exit_codes.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/exit_codes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/shell.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/shell.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/shell.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/shell.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/shell.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/shell.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/stdout_testcase.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/submission.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/submission.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/submission.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/submission.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/submission.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/submission.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310-pytest-7.1.3.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38-pytest-7.1.3.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/test_helper_formatter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_io.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_io.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_io.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_io.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_io.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_io.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_picker.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_picker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_picker.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_picker.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_picker.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_picker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-310.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-37.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-38.pyc` & `autograder-3.7.7/autograder/testcase_utils/__pycache__/testcase_result_validator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/abstract_testcase.py` & `autograder-3.7.7/autograder/testcase_utils/abstract_testcase.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/exit_codes.py` & `autograder-3.7.7/autograder/testcase_utils/exit_codes.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/shell.py` & `autograder-3.7.7/autograder/testcase_utils/shell.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/stdout_testcase.py` & `autograder-3.7.7/autograder/testcase_utils/stdout_testcase.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/submission.py` & `autograder-3.7.7/autograder/testcase_utils/submission.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/test_helper_formatter.py` & `autograder-3.7.7/autograder/testcase_utils/test_helper_formatter.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/testcase_io.py` & `autograder-3.7.7/autograder/testcase_utils/testcase_io.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/testcase_picker.py` & `autograder-3.7.7/autograder/testcase_utils/testcase_picker.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/testcase_utils/testcase_result_validator.py` & `autograder-3.7.7/autograder/testcase_utils/testcase_result_validator.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/autograder/util.py` & `autograder-3.7.7/autograder/util.py`

 * *Files identical despite different names*

### Comparing `autograder-3.7.6/pyproject.toml` & `autograder-3.7.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "autograder"
-version = "3.7.6"
+version = "3.7.7"
 description = "A simple, secure, and versatile way to automatically grade programming assignments"
 authors = ["Stanislav Zmiev <zmievsa@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
-documentation = "https://ovsyanka83.github.io/autograder/"
-repository = "https://github.com/Ovsyanka83/autograder"
-# this might be unnecessary, I don't remember and am too lazy too google
+documentation = "https://zmievsa.github.io/autograder/"
+repository = "https://github.com/zmievsa/autograder"
+# this might be unnecessary, I don't remember and am too lazy to google
 include = ["autograder/**/*"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Topic :: Education :: Testing",
 ]
```

### Comparing `autograder-3.7.6/PKG-INFO` & `autograder-3.7.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: autograder
-Version: 3.7.6
+Version: 3.7.7
 Summary: A simple, secure, and versatile way to automatically grade programming assignments
-Home-page: https://github.com/Ovsyanka83/autograder
+Home-page: https://github.com/zmievsa/autograder
 License: GPL-3.0
 Author: Stanislav Zmiev
 Author-email: zmievsa@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Education
@@ -17,53 +17,53 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education :: Testing
 Requires-Dist: antlr4-python3-runtime (==4.9.2)
 Requires-Dist: numba (>=0.56.2,<0.57.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: tomlkit (>=0.11.4,<0.12.0)
-Project-URL: Documentation, https://ovsyanka83.github.io/autograder/
-Project-URL: Repository, https://github.com/Ovsyanka83/autograder
+Project-URL: Documentation, https://zmievsa.github.io/autograder/
+Project-URL: Repository, https://github.com/zmievsa/autograder
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <a href="https://ovsyanka83.github.io/autograder/"><img src="https://raw.githubusercontent.com/Ovsyanka83/autograder/main/docs/_media/logo_with_text.svg" alt="AutoGrader"></a>
+  <a href="https://zmievsa.github.io/autograder/"><img src="https://raw.githubusercontent.com/zmievsa/autograder/main/docs/_media/logo_with_text.svg" alt="AutoGrader"></a>
 </p>
 <p align="center">
   <b>A simple, secure, and versatile way to automatically grade programming assignments</b>
 </p>
 
 ---
 
 <p align="center">
-<a href="https://github.com/ovsyanka83/autograder/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
-    <img src="https://github.com/Ovsyanka83/autograder/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
+<a href="https://github.com/zmievsa/autograder/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
+    <img src="https://github.com/zmievsa/autograder/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
 </a>
-<a href="https://codecov.io/gh/ovsyanka83/autograder" target="_blank">
-    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/autograder?color=%2334D058" alt="Coverage">
+<a href="https://codecov.io/gh/zmievsa/autograder" target="_blank">
+    <img src="https://img.shields.io/codecov/c/github/zmievsa/autograder?color=%2334D058" alt="Coverage">
 </a>
 <a href="https://pypi.org/project/autograder/" target="_blank">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autograder?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/autograder/" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/autograder?color=%2334D058" alt="Supported Python versions">
 </a>
 </p>
 
 ## Features
 
 * Blazingly fast (can grade hundreads of submissions using dozens of testcases in a few minutes. Seconds if grading python)
-* [Easy to grade](https://ovsyanka83.github.io/autograder/#/?id=usage)
-* [Easy-to-write testcases](https://ovsyanka83.github.io/autograder/#/?id=writing-testcases)  
-* Testcase grade can be based on [student's stdout](https://ovsyanka83.github.io/autograder/#/?id=helper-functions)
+* [Easy to grade](https://zmievsa.github.io/autograder/#/?id=usage)
+* [Easy-to-write testcases](https://zmievsa.github.io/autograder/#/?id=writing-testcases)  
+* Testcase grade can be based on [student's stdout](https://zmievsa.github.io/autograder/#/?id=helper-functions)
 * Can grade C, C++, Java, and Python code in regular mode
 * Can grade any programming language in stdout-only mode
 * A file with testcase grades and details can be generated for each student
-* You can customize the total points for the assignment, maximum running time of student's program, file names to be considered for grading, formatters for checking student stdout, and [so much more](https://github.com/Ovsyanka83/autograder/blob/master/autograder/default_config.toml).
-* [Anti Cheating capabilities](https://ovsyanka83.github.io/autograder/#/?id=anti-cheating) that make it nearly impossible for students to cheat
+* You can customize the total points for the assignment, maximum running time of student's program, file names to be considered for grading, formatters for checking student stdout, and [so much more](https://github.com/zmievsa/autograder/blob/master/autograder/default_config.toml).
+* [Anti Cheating capabilities](https://zmievsa.github.io/autograder/#/?id=anti-cheating) that make it nearly impossible for students to cheat
 * Grading submissions in multiple programming languages at once
 * JSON result output supported if autograder needs to be integrated as a part of a larger utility
 * Can check submissions for similarity (plagiarism)
 * Can detect and report memory leaks in C/C++ code
 
 ## Installation
 
@@ -77,15 +77,15 @@
 ### Updates
 
 `pip install -U --no-cache-dir autograder`
 
 ## Quickstart
 
 * Run `autograder guide path/to/directory/you'd/like/to/grade`. The guide will create all of the necessary configurations and directories for grading and will explain how to grade.
-* Read the [usage](https://ovsyanka83.github.io/autograder/#/?id=usage) section of the docs
+* Read the [usage](https://zmievsa.github.io/autograder/#/?id=usage) section of the docs
 
 ## Supported Platforms
 
 * Linux is fully supported
 * OS X is fully supported
 * Windows is partially supported:
   * Stdout-testcases that require shebang lines are not and cannot be supported
```

#### html2text {}

```diff
@@ -1,52 +1,51 @@
-Metadata-Version: 2.1 Name: autograder Version: 3.7.6 Summary: A simple,
+Metadata-Version: 2.1 Name: autograder Version: 3.7.7 Summary: A simple,
 secure, and versatile way to automatically grade programming assignments Home-
-page: https://github.com/Ovsyanka83/autograder License: GPL-3.0 Author:
-Stanislav Zmiev Author-email: zmievsa@gmail.com Requires-Python: >=3.8,<3.12
-Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
-:: Console Classifier: Intended Audience :: Education Classifier: License ::
-OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Education :: Testing Requires-Dist: antlr4-python3-runtime
-(==4.9.2) Requires-Dist: numba (>=0.56.2,<0.57.0) Requires-Dist: numpy
-(>=1.22.4,<2.0.0) Requires-Dist: tomlkit (>=0.11.4,<0.12.0) Project-URL:
-Documentation, https://ovsyanka83.github.io/autograder/ Project-URL:
-Repository, https://github.com/Ovsyanka83/autograder Description-Content-Type:
-text/markdown
+page: https://github.com/zmievsa/autograder License: GPL-3.0 Author: Stanislav
+Zmiev Author-email: zmievsa@gmail.com Requires-Python: >=3.8,<3.12 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Console
+Classifier: Intended Audience :: Education Classifier: License :: OSI Approved
+:: GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Education :: Testing Requires-Dist: antlr4-python3-runtime (==4.9.2)
+Requires-Dist: numba (>=0.56.2,<0.57.0) Requires-Dist: numpy (>=1.22.4,<2.0.0)
+Requires-Dist: tomlkit (>=0.11.4,<0.12.0) Project-URL: Documentation, https://
+zmievsa.github.io/autograder/ Project-URL: Repository, https://github.com/
+zmievsa/autograder Description-Content-Type: text/markdown
                                  _[_A_u_t_o_G_r_a_d_e_r_]
     AA ssiimmppllee,, sseeccuurree,, aanndd vveerrssaattiillee wwaayy ttoo aauuttoommaattiiccaallllyy ggrraaddee pprrooggrraammmmiinngg
                                   aassssiiggnnmmeennttss
 ---
                _[_T_e_s_t_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 ## Features * Blazingly fast (can grade hundreads of submissions using dozens
 of testcases in a few minutes. Seconds if grading python) * [Easy to grade]
-(https://ovsyanka83.github.io/autograder/#/?id=usage) * [Easy-to-write
-testcases](https://ovsyanka83.github.io/autograder/#/?id=writing-testcases) *
-Testcase grade can be based on [student's stdout](https://ovsyanka83.github.io/
-autograder/#/?id=helper-functions) * Can grade C, C++, Java, and Python code in
-regular mode * Can grade any programming language in stdout-only mode * A file
-with testcase grades and details can be generated for each student * You can
-customize the total points for the assignment, maximum running time of
-student's program, file names to be considered for grading, formatters for
-checking student stdout, and [so much more](https://github.com/Ovsyanka83/
-autograder/blob/master/autograder/default_config.toml). * [Anti Cheating
-capabilities](https://ovsyanka83.github.io/autograder/#/?id=anti-cheating) that
-make it nearly impossible for students to cheat * Grading submissions in
-multiple programming languages at once * JSON result output supported if
-autograder needs to be integrated as a part of a larger utility * Can check
-submissions for similarity (plagiarism) * Can detect and report memory leaks in
-C/C++ code ## Installation * Run `pip install autograder` * To grade various
-programming languages, you'd need to install: * `gcc`/`clang` for C/C++ support
-* `Java JDK` for java support * `make` for compiled stdout-only testcase
-support * Any interpreter/compiler necessary to run stdout-only testcases. For
-example, testcases with ruby in their shebang lines will require the ruby
-interpreter ### Updates `pip install -U --no-cache-dir autograder` ##
-Quickstart * Run `autograder guide path/to/directory/you'd/like/to/grade`. The
-guide will create all of the necessary configurations and directories for
-grading and will explain how to grade. * Read the [usage](https://
-ovsyanka83.github.io/autograder/#/?id=usage) section of the docs ## Supported
-Platforms * Linux is fully supported * OS X is fully supported * Windows is
-partially supported: * Stdout-testcases that require shebang lines are not and
-cannot be supported ## Supported Programming Languages * Java * C * C++ *
-CPython (3.8-3.11) * Any programming language if stdout-only grading is used
+(https://zmievsa.github.io/autograder/#/?id=usage) * [Easy-to-write testcases]
+(https://zmievsa.github.io/autograder/#/?id=writing-testcases) * Testcase grade
+can be based on [student's stdout](https://zmievsa.github.io/autograder/#/
+?id=helper-functions) * Can grade C, C++, Java, and Python code in regular mode
+* Can grade any programming language in stdout-only mode * A file with testcase
+grades and details can be generated for each student * You can customize the
+total points for the assignment, maximum running time of student's program,
+file names to be considered for grading, formatters for checking student
+stdout, and [so much more](https://github.com/zmievsa/autograder/blob/master/
+autograder/default_config.toml). * [Anti Cheating capabilities](https://
+zmievsa.github.io/autograder/#/?id=anti-cheating) that make it nearly
+impossible for students to cheat * Grading submissions in multiple programming
+languages at once * JSON result output supported if autograder needs to be
+integrated as a part of a larger utility * Can check submissions for similarity
+(plagiarism) * Can detect and report memory leaks in C/C++ code ## Installation
+* Run `pip install autograder` * To grade various programming languages, you'd
+need to install: * `gcc`/`clang` for C/C++ support * `Java JDK` for java
+support * `make` for compiled stdout-only testcase support * Any interpreter/
+compiler necessary to run stdout-only testcases. For example, testcases with
+ruby in their shebang lines will require the ruby interpreter ### Updates `pip
+install -U --no-cache-dir autograder` ## Quickstart * Run `autograder guide
+path/to/directory/you'd/like/to/grade`. The guide will create all of the
+necessary configurations and directories for grading and will explain how to
+grade. * Read the [usage](https://zmievsa.github.io/autograder/#/?id=usage)
+section of the docs ## Supported Platforms * Linux is fully supported * OS X is
+fully supported * Windows is partially supported: * Stdout-testcases that
+require shebang lines are not and cannot be supported ## Supported Programming
+Languages * Java * C * C++ * CPython (3.8-3.11) * Any programming language if
+stdout-only grading is used
```

