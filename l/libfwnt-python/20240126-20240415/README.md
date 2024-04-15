# Comparing `tmp/libfwnt-python-20240126.tar.gz` & `tmp/libfwnt-python-20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwnt-python-20240126.tar", last modified: Sat Jan 27 06:12:54 2024, max compression
+gzip compressed data, was "libfwnt-python-20240415.tar", last modified: Mon Apr 15 15:23:30 2024, max compression
```

## Comparing `libfwnt-python-20240126.tar` & `libfwnt-python-20240415.tar`

### file list

```diff
@@ -1,363 +1,363 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-26 05:37:56.000000 libfwnt-20240126/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-26 05:42:19.000000 libfwnt-20240126/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-26 05:37:56.000000 libfwnt-20240126/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-26 05:42:19.000000 libfwnt-20240126/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:52.000000 libfwnt-20240126/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-26 05:42:16.000000 libfwnt-20240126/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-26 05:42:16.000000 libfwnt-20240126/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-26 05:42:16.000000 libfwnt-20240126/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-26 05:42:16.000000 libfwnt-20240126/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-26 05:42:16.000000 libfwnt-20240126/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:09:13.000000 libfwnt-20240126/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:52.000000 libfwnt-20240126/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14831 2024-01-26 05:42:26.000000 libfwnt-20240126/include/libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14831 2024-01-26 05:37:56.000000 libfwnt-20240126/include/libfwnt.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2024-01-26 05:37:56.000000 libfwnt-20240126/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:52.000000 libfwnt-20240126/include/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2355 2024-01-26 05:37:56.000000 libfwnt-20240126/include/libfwnt/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2353 2024-01-26 05:42:26.000000 libfwnt-20240126/include/libfwnt/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-01-26 05:37:56.000000 libfwnt-20240126/include/libfwnt/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4962 2024-01-26 05:42:26.000000 libfwnt-20240126/include/libfwnt/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-26 05:39:03.000000 libfwnt-20240126/include/libfwnt/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-01-26 05:37:56.000000 libfwnt-20240126/include/libfwnt/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-26 05:37:56.000000 libfwnt-20240126/include/libfwnt/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-26 05:42:26.000000 libfwnt-20240126/include/libfwnt/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22577 2024-01-26 05:42:19.000000 libfwnt-20240126/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-26 05:37:56.000000 libfwnt-20240126/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-26 05:37:56.000000 libfwnt-20240126/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-26 05:37:56.000000 libfwnt-20240126/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-26 05:37:56.000000 libfwnt-20240126/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-26 05:37:56.000000 libfwnt-20240126/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-26 05:37:56.000000 libfwnt-20240126/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-26 05:37:56.000000 libfwnt-20240126/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-26 05:37:56.000000 libfwnt-20240126/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-26 05:37:56.000000 libfwnt-20240126/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-01-26 05:42:26.000000 libfwnt-20240126/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10523 2024-01-26 05:42:19.000000 libfwnt-20240126/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11150 2024-01-26 05:42:26.000000 libfwnt-20240126/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-26 05:37:56.000000 libfwnt-20240126/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-26 05:37:56.000000 libfwnt-20240126/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-26 05:37:56.000000 libfwnt-20240126/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19625 2024-01-26 05:42:19.000000 libfwnt-20240126/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/pyfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2580 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12322 2024-01-26 05:38:46.000000 libfwnt-20240126/pyfwnt/pyfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10174 2024-01-26 05:38:46.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1191 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1125 2023-12-03 09:09:14.000000 libfwnt-20240126/pyfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2674 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13320 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10887 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2306 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12389 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2618 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7539 2024-01-26 05:38:46.000000 libfwnt-20240126/pyfwnt/pyfwnt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4861 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44669 2024-01-26 05:42:19.000000 libfwnt-20240126/pyfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16307 2024-01-26 05:38:46.000000 libfwnt-20240126/pyfwnt/pyfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4873 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-01-26 05:37:57.000000 libfwnt-20240126/pyfwnt/pyfwnt_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      402 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1585 2023-12-03 09:09:12.000000 libfwnt-20240126/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:12.000000 libfwnt-20240126/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-26 05:42:19.000000 libfwnt-20240126/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:52.000000 libfwnt-20240126/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-01-26 05:37:57.000000 libfwnt-20240126/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:52.000000 libfwnt-20240126/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/libfwnt-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-01-26 05:42:26.000000 libfwnt-20240126/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/libfwnt-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-26 05:37:56.000000 libfwnt-20240126/dpkg/libfwnt.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-01-26 05:42:26.000000 libfwnt-20240126/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-26 05:37:56.000000 libfwnt-20240126/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1065998 2024-01-26 05:42:18.000000 libfwnt-20240126/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-26 05:42:19.000000 libfwnt-20240126/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-26 05:42:19.000000 libfwnt-20240126/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_lzx/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5011 2024-01-26 05:38:46.000000 libfwnt-20240126/msvscpp/fwnt_test_lzx/fwnt_test_lzx.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4850 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_error/fwnt_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_security_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5135 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_security_descriptor/fwnt_test_security_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/pyfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6655 2024-01-26 05:38:46.000000 libfwnt-20240126/msvscpp/pyfwnt/pyfwnt.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      964 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_bit_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5108 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_bit_stream/fwnt_test_bit_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_lznt1/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5017 2024-01-26 05:38:46.000000 libfwnt-20240126/msvscpp/fwnt_test_lznt1/fwnt_test_lznt1.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_lzxpress/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5026 2024-01-26 05:38:46.000000 libfwnt-20240126/msvscpp/fwnt_test_lzxpress/fwnt_test_lzxpress.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_huffman_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5114 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_huffman_tree/fwnt_test_huffman_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_access_control_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5138 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_access_control_entry/fwnt_test_access_control_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_access_control_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5135 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_access_control_list/fwnt_test_access_control_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4856 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_support/fwnt_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7509 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/libfwnt/libfwnt.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13589 2024-01-26 05:38:46.000000 libfwnt-20240126/msvscpp/libfwnt.sln
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17557 2024-01-26 05:42:19.000000 libfwnt-20240126/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_security_identifier/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5135 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_security_identifier/fwnt_test_security_identifier.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/msvscpp/fwnt_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4936 2024-01-26 05:38:02.000000 libfwnt-20240126/msvscpp/fwnt_test_notify/fwnt_test_notify.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-26 05:37:56.000000 libfwnt-20240126/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      280 2024-01-26 05:37:56.000000 libfwnt-20240126/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-26 05:42:19.000000 libfwnt-20240126/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27076 2024-01-26 05:42:19.000000 libfwnt-20240126/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-26 05:42:10.000000 libfwnt-20240126/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-26 05:37:56.000000 libfwnt-20240126/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1962 2024-01-26 05:42:26.000000 libfwnt-20240126/libfwnt.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-01-26 05:37:56.000000 libfwnt-20240126/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-26 05:42:19.000000 libfwnt-20240126/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-26 05:37:56.000000 libfwnt-20240126/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-01-26 05:37:56.000000 libfwnt-20240126/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:12.000000 libfwnt-20240126/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27482 2024-01-26 05:42:19.000000 libfwnt-20240126/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-26 05:42:13.000000 libfwnt-20240126/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-26 05:42:19.000000 libfwnt-20240126/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1068 2023-12-03 09:09:12.000000 libfwnt-20240126/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      126 2023-12-03 09:09:13.000000 libfwnt-20240126/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19829 2024-01-26 05:42:19.000000 libfwnt-20240126/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7262 2024-01-26 05:37:57.000000 libfwnt-20240126/manuals/libfwnt.3
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/fwnt_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3709 2024-01-26 05:39:03.000000 libfwnt-20240126/tests/pyfwnt_test_security_descriptor.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/pyfwnt_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-01-26 05:39:03.000000 libfwnt-20240126/tests/pyfwnt_test_access_control_list.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20620 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/fwnt_test_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   339752 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16283 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/fwnt_test_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2001 2024-01-26 05:39:03.000000 libfwnt-20240126/tests/pyfwnt_test_security_identifier.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3901 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/pyfwnt_test_lzxpress.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4166 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_libfwnt.h
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-01-26 05:39:18.000000 libfwnt-20240126/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  4532151 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17759 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/fwnt_test_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29450 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/fwnt_test_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2024-01-26 05:39:03.000000 libfwnt-20240126/tests/pyfwnt_test_access_control_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14361 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/fwnt_test_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   236623 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/pyfwnt_test_lzx.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77922 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/pyfwnt_test_lznt1.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76378 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49401 2024-01-26 05:42:19.000000 libfwnt-20240126/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21514 2024-01-26 05:38:46.000000 libfwnt-20240126/tests/fwnt_test_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-01-26 05:37:57.000000 libfwnt-20240126/tests/fwnt_test_memory.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-01-26 05:39:03.000000 libfwnt-20240126/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1306 2024-01-26 05:37:57.000000 libfwnt-20240126/ossfuzz/lzxpress_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2240 2023-12-03 09:09:27.000000 libfwnt-20240126/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1279 2024-01-26 05:37:57.000000 libfwnt-20240126/ossfuzz/lzx_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-01-26 05:37:57.000000 libfwnt-20240126/ossfuzz/ossfuzz_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-01-26 05:37:57.000000 libfwnt-20240126/ossfuzz/security_identifier_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2024-01-26 05:37:57.000000 libfwnt-20240126/ossfuzz/lznt1_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33361 2024-01-26 05:42:19.000000 libfwnt-20240126/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-01-26 05:37:57.000000 libfwnt-20240126/ossfuzz/security_descriptor_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1305 2024-01-26 05:37:57.000000 libfwnt-20240126/ossfuzz/lzxpress_huffman_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-26 05:42:16.000000 libfwnt-20240126/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-01-26 05:38:46.000000 libfwnt-20240126/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3472 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1822 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2023-12-03 09:09:13.000000 libfwnt-20240126/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2024-01-26 05:42:26.000000 libfwnt-20240126/libfwnt/libfwnt.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-01-26 05:38:46.000000 libfwnt-20240126/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-01-26 05:42:26.000000 libfwnt-20240126/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-01-26 05:38:46.000000 libfwnt-20240126/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29790 2024-01-26 05:42:19.000000 libfwnt-20240126/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-01-26 05:38:46.000000 libfwnt-20240126/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt/libfwnt_access_control_entry.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:14.000000 libfwnt-20240126/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:14.000000 libfwnt-20240126/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:14.000000 libfwnt-20240126/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:14.000000 libfwnt-20240126/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:14.000000 libfwnt-20240126/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:14.000000 libfwnt-20240126/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:14.000000 libfwnt-20240126/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:14.000000 libfwnt-20240126/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:14.000000 libfwnt-20240126/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-01-26 05:42:26.000000 libfwnt-20240126/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:14.000000 libfwnt-20240126/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:14.000000 libfwnt-20240126/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34962 2024-01-26 05:42:19.000000 libfwnt-20240126/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24504 2024-01-26 05:42:19.000000 libfwnt-20240126/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-01-26 05:42:12.000000 libfwnt-20240126/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-27 06:12:53.000000 libfwnt-20240126/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-26 05:42:11.000000 libfwnt-20240126/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24017 2024-01-26 05:42:19.000000 libfwnt-20240126/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2235 2024-01-26 05:37:56.000000 libfwnt-20240126/libfwnt.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56503 2024-01-26 05:42:18.000000 libfwnt-20240126/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4475 2024-01-26 05:37:56.000000 libfwnt-20240126/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-01-27 06:12:54.658964 libfwnt-20240126/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-15 14:42:32.000000 libfwnt-20240415/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-15 15:00:19.000000 libfwnt-20240415/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 14:42:32.000000 libfwnt-20240415/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-15 15:00:19.000000 libfwnt-20240415/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-15 14:42:35.000000 libfwnt-20240415/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-12 04:19:31.000000 libfwnt-20240415/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-15 14:42:35.000000 libfwnt-20240415/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-15 15:00:15.000000 libfwnt-20240415/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-15 15:00:15.000000 libfwnt-20240415/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-15 15:00:15.000000 libfwnt-20240415/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-15 14:42:35.000000 libfwnt-20240415/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-15 14:42:35.000000 libfwnt-20240415/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-15 15:00:15.000000 libfwnt-20240415/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-15 15:00:15.000000 libfwnt-20240415/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:13.000000 libfwnt-20240415/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-12 04:19:31.000000 libfwnt-20240415/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14831 2024-04-15 15:00:34.000000 libfwnt-20240415/include/libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14831 2024-04-15 14:42:34.000000 libfwnt-20240415/include/libfwnt.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      388 2024-04-15 14:42:55.000000 libfwnt-20240415/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/include/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2355 2024-04-15 14:42:34.000000 libfwnt-20240415/include/libfwnt/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2353 2024-04-15 15:00:34.000000 libfwnt-20240415/include/libfwnt/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-15 14:42:34.000000 libfwnt-20240415/include/libfwnt/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4962 2024-04-15 15:00:34.000000 libfwnt-20240415/include/libfwnt/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-15 14:46:34.000000 libfwnt-20240415/include/libfwnt/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-15 14:42:34.000000 libfwnt-20240415/include/libfwnt/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-15 14:42:34.000000 libfwnt-20240415/include/libfwnt/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-15 15:00:34.000000 libfwnt-20240415/include/libfwnt/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22557 2024-04-15 15:00:19.000000 libfwnt-20240415/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-15 14:42:33.000000 libfwnt-20240415/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-15 14:42:33.000000 libfwnt-20240415/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-15 14:42:33.000000 libfwnt-20240415/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-15 14:42:33.000000 libfwnt-20240415/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-15 14:42:33.000000 libfwnt-20240415/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-15 14:42:33.000000 libfwnt-20240415/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-15 14:42:33.000000 libfwnt-20240415/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-15 14:45:26.000000 libfwnt-20240415/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-15 14:42:33.000000 libfwnt-20240415/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-15 15:00:34.000000 libfwnt-20240415/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10523 2024-04-15 15:00:18.000000 libfwnt-20240415/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11150 2024-04-15 15:00:34.000000 libfwnt-20240415/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-15 14:42:33.000000 libfwnt-20240415/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-15 14:42:33.000000 libfwnt-20240415/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-15 14:42:33.000000 libfwnt-20240415/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19632 2024-04-15 15:00:19.000000 libfwnt-20240415/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:28.000000 libfwnt-20240415/pyfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2580 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12322 2024-04-15 14:47:18.000000 libfwnt-20240415/pyfwnt/pyfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10174 2024-04-15 14:47:18.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1191 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-04-15 14:44:56.000000 libfwnt-20240415/pyfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2674 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13320 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10887 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2306 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12389 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2618 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7539 2024-04-15 14:47:18.000000 libfwnt-20240415/pyfwnt/pyfwnt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4861 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45345 2024-04-15 15:00:19.000000 libfwnt-20240415/pyfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16307 2024-04-15 14:47:18.000000 libfwnt-20240415/pyfwnt/pyfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4873 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-04-15 14:42:35.000000 libfwnt-20240415/pyfwnt/pyfwnt_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      402 2024-04-15 14:42:32.000000 libfwnt-20240415/libfwnt.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1393 2024-04-15 14:43:49.000000 libfwnt-20240415/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:12.000000 libfwnt-20240415/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-15 15:00:19.000000 libfwnt-20240415/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-15 14:42:35.000000 libfwnt-20240415/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/libfwnt-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-15 15:00:34.000000 libfwnt-20240415/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/libfwnt-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-15 14:42:32.000000 libfwnt-20240415/dpkg/libfwnt.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      479 2024-04-15 15:00:34.000000 libfwnt-20240415/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-15 14:42:32.000000 libfwnt-20240415/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1067147 2024-04-15 15:00:17.000000 libfwnt-20240415/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-15 15:00:19.000000 libfwnt-20240415/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-15 15:00:19.000000 libfwnt-20240415/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_lzx/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5011 2024-04-15 14:42:52.000000 libfwnt-20240415/msvscpp/fwnt_test_lzx/fwnt_test_lzx.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4850 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_error/fwnt_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_security_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5135 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_security_descriptor/fwnt_test_security_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/pyfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6655 2024-04-15 14:42:52.000000 libfwnt-20240415/msvscpp/pyfwnt/pyfwnt.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      935 2024-04-15 14:44:03.000000 libfwnt-20240415/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_bit_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5108 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_bit_stream/fwnt_test_bit_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_lznt1/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5017 2024-04-15 14:42:52.000000 libfwnt-20240415/msvscpp/fwnt_test_lznt1/fwnt_test_lznt1.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_lzxpress/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5026 2024-04-15 14:42:52.000000 libfwnt-20240415/msvscpp/fwnt_test_lzxpress/fwnt_test_lzxpress.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_huffman_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5114 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_huffman_tree/fwnt_test_huffman_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_access_control_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5138 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_access_control_entry/fwnt_test_access_control_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_access_control_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5135 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_access_control_list/fwnt_test_access_control_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4856 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_support/fwnt_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7509 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/libfwnt/libfwnt.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13589 2024-04-15 14:42:52.000000 libfwnt-20240415/msvscpp/libfwnt.sln
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17557 2024-04-15 15:00:19.000000 libfwnt-20240415/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_security_identifier/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5135 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_security_identifier/fwnt_test_security_identifier.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/msvscpp/fwnt_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4936 2024-04-15 14:42:41.000000 libfwnt-20240415/msvscpp/fwnt_test_notify/fwnt_test_notify.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-15 14:42:33.000000 libfwnt-20240415/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      280 2024-04-15 14:42:32.000000 libfwnt-20240415/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-15 15:00:19.000000 libfwnt-20240415/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:28.000000 libfwnt-20240415/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27576 2024-04-15 15:00:19.000000 libfwnt-20240415/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-15 15:00:06.000000 libfwnt-20240415/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-15 14:42:32.000000 libfwnt-20240415/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1962 2024-04-15 15:00:34.000000 libfwnt-20240415/libfwnt.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-04-15 14:42:32.000000 libfwnt-20240415/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-15 15:00:19.000000 libfwnt-20240415/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-15 14:42:32.000000 libfwnt-20240415/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-04-15 14:42:52.000000 libfwnt-20240415/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:12.000000 libfwnt-20240415/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28015 2024-04-15 15:00:19.000000 libfwnt-20240415/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-15 15:00:10.000000 libfwnt-20240415/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-15 15:00:19.000000 libfwnt-20240415/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1068 2023-12-03 09:09:12.000000 libfwnt-20240415/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       97 2024-04-15 14:44:18.000000 libfwnt-20240415/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19829 2024-04-15 15:00:19.000000 libfwnt-20240415/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7262 2024-04-15 14:42:35.000000 libfwnt-20240415/manuals/libfwnt.3
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-04-15 14:42:52.000000 libfwnt-20240415/tests/fwnt_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3709 2024-04-15 14:47:18.000000 libfwnt-20240415/tests/pyfwnt_test_security_descriptor.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/pyfwnt_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-04-15 14:47:18.000000 libfwnt-20240415/tests/pyfwnt_test_access_control_list.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20620 2024-04-15 14:42:52.000000 libfwnt-20240415/tests/fwnt_test_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   339752 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16283 2024-04-15 14:42:52.000000 libfwnt-20240415/tests/fwnt_test_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2001 2024-04-15 14:47:18.000000 libfwnt-20240415/tests/pyfwnt_test_security_identifier.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3901 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/pyfwnt_test_lzxpress.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4183 2024-04-15 14:53:53.000000 libfwnt-20240415/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_libfwnt.h
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4138 2024-04-15 14:50:04.000000 libfwnt-20240415/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  4532151 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17759 2024-04-15 14:42:52.000000 libfwnt-20240415/tests/fwnt_test_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29450 2024-04-15 14:42:52.000000 libfwnt-20240415/tests/fwnt_test_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1217 2024-04-15 14:47:18.000000 libfwnt-20240415/tests/pyfwnt_test_access_control_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14361 2024-04-15 14:42:52.000000 libfwnt-20240415/tests/fwnt_test_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   236623 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/pyfwnt_test_lzx.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77922 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/pyfwnt_test_lznt1.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    76378 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50029 2024-04-15 15:00:19.000000 libfwnt-20240415/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21514 2024-04-15 14:42:52.000000 libfwnt-20240415/tests/fwnt_test_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-15 14:42:35.000000 libfwnt-20240415/tests/fwnt_test_memory.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4151 2024-04-15 14:48:43.000000 libfwnt-20240415/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:29.000000 libfwnt-20240415/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1306 2024-04-15 14:42:34.000000 libfwnt-20240415/ossfuzz/lzxpress_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2236 2024-04-15 14:44:29.000000 libfwnt-20240415/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1279 2024-04-15 14:42:34.000000 libfwnt-20240415/ossfuzz/lzx_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-15 14:42:34.000000 libfwnt-20240415/ossfuzz/ossfuzz_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-04-15 14:42:34.000000 libfwnt-20240415/ossfuzz/security_identifier_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2024-04-15 14:42:34.000000 libfwnt-20240415/ossfuzz/lznt1_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33643 2024-04-15 15:00:19.000000 libfwnt-20240415/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-04-15 14:42:34.000000 libfwnt-20240415/ossfuzz/security_descriptor_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1305 2024-04-15 14:42:34.000000 libfwnt-20240415/ossfuzz/lzxpress_huffman_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-15 15:00:14.000000 libfwnt-20240415/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:28.000000 libfwnt-20240415/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-04-15 14:47:04.000000 libfwnt-20240415/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3472 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1822 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-15 14:45:15.000000 libfwnt-20240415/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2024-04-15 15:00:34.000000 libfwnt-20240415/libfwnt/libfwnt.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-15 14:47:04.000000 libfwnt-20240415/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-04-15 15:00:34.000000 libfwnt-20240415/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-04-15 14:47:04.000000 libfwnt-20240415/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30455 2024-04-15 15:00:19.000000 libfwnt-20240415/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-15 14:47:04.000000 libfwnt-20240415/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-04-15 14:42:34.000000 libfwnt-20240415/libfwnt/libfwnt_access_control_entry.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:28.000000 libfwnt-20240415/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:14.000000 libfwnt-20240415/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:14.000000 libfwnt-20240415/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:14.000000 libfwnt-20240415/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:14.000000 libfwnt-20240415/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:14.000000 libfwnt-20240415/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:14.000000 libfwnt-20240415/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:14.000000 libfwnt-20240415/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:14.000000 libfwnt-20240415/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:14.000000 libfwnt-20240415/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-15 15:00:34.000000 libfwnt-20240415/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:14.000000 libfwnt-20240415/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:14.000000 libfwnt-20240415/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34844 2024-04-15 15:00:19.000000 libfwnt-20240415/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:28.000000 libfwnt-20240415/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24699 2024-04-15 15:00:19.000000 libfwnt-20240415/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-15 15:00:09.000000 libfwnt-20240415/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 15:23:27.000000 libfwnt-20240415/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-15 15:00:08.000000 libfwnt-20240415/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24166 2024-04-15 15:00:19.000000 libfwnt-20240415/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2235 2024-04-15 14:42:32.000000 libfwnt-20240415/libfwnt.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56503 2024-04-15 15:00:17.000000 libfwnt-20240415/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4475 2024-04-15 14:42:32.000000 libfwnt-20240415/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2024-04-15 15:23:30.429415 libfwnt-20240415/PKG-INFO
```

### Comparing `libfwnt-20240126/COPYING` & `libfwnt-20240415/COPYING`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/install-sh` & `libfwnt-20240415/install-sh`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/depcomp` & `libfwnt-20240415/depcomp`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/tests.m4` & `libfwnt-20240415/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/lib-prefix.m4` & `libfwnt-20240415/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/progtest.m4` & `libfwnt-20240415/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/gettext.m4` & `libfwnt-20240415/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/lib-ld.m4` & `libfwnt-20240415/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/libcdata.m4` & `libfwnt-20240415/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libfwnt-20240126/m4/common.m4` & `libfwnt-20240415/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libfwnt-20240126/m4/libcthreads.m4` & `libfwnt-20240415/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libfwnt-20240126/m4/ltversion.m4` & `libfwnt-20240415/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/ltsugar.m4` & `libfwnt-20240415/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/host-cpu-c-abi.m4` & `libfwnt-20240415/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/libtool.m4` & `libfwnt-20240415/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/po.m4` & `libfwnt-20240415/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/libcerror.m4` & `libfwnt-20240415/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libfwnt-20240126/m4/libcnotify.m4` & `libfwnt-20240415/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libfwnt-20240126/m4/intlmacosx.m4` & `libfwnt-20240415/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/lt~obsolete.m4` & `libfwnt-20240415/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/lib-link.m4` & `libfwnt-20240415/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/iconv.m4` & `libfwnt-20240415/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/ltoptions.m4` & `libfwnt-20240415/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/nls.m4` & `libfwnt-20240415/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/python.m4` & `libfwnt-20240415/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/types.m4` & `libfwnt-20240415/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/m4/pthread.m4` & `libfwnt-20240415/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libfwnt-20240126/include/libfwnt.h` & `libfwnt-20240415/include/libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt.h.in` & `libfwnt-20240415/include/libfwnt.h.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt/definitions.h.in` & `libfwnt-20240415/include/libfwnt/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt/definitions.h` & `libfwnt-20240415/include/libfwnt/definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWNT_DEFINITIONS_H )
 #define _LIBFWNT_DEFINITIONS_H
 
 #include <libfwnt/types.h>
 
-#define LIBFWNT_VERSION				20240126
+#define LIBFWNT_VERSION				20240415
 
 /* The version string
  */
-#define LIBFWNT_VERSION_STRING			"20240126"
+#define LIBFWNT_VERSION_STRING			"20240415"
 
 /* The byte order definitions
  */
 enum LIBFWNT_ENDIAN
 {
 	LIBFWNT_ENDIAN_BIG			= (int) 'b',
 	LIBFWNT_ENDIAN_LITTLE			= (int) 'l'
```

### Comparing `libfwnt-20240126/include/libfwnt/types.h.in` & `libfwnt-20240415/include/libfwnt/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt/types.h` & `libfwnt-20240415/include/libfwnt/types.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt/features.h.in` & `libfwnt-20240415/include/libfwnt/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt/error.h` & `libfwnt-20240415/include/libfwnt/error.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt/extern.h` & `libfwnt-20240415/include/libfwnt/extern.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/libfwnt/features.h` & `libfwnt-20240415/include/libfwnt/features.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/include/Makefile.in` & `libfwnt-20240415/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,20 @@
 
 EXTRA_DIST = \
 	libfwnt.h.in \
 	libfwnt/definitions.h.in \
 	libfwnt/features.h.in \
 	libfwnt/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwnt.h \
+	libfwnt/definitions.h \
+	libfwnt/features.h \
+	libfwnt/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -615,23 +620,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -713,17 +720,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfwnt.h
-	-rm -f libfwnt/definitions.h
-	-rm -f libfwnt/features.h
-	-rm -f libfwnt/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwnt-20240126/common/config_borlandc.h` & `libfwnt-20240415/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/file_stream.h` & `libfwnt-20240415/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/memory.h` & `libfwnt-20240415/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/byte_stream.h` & `libfwnt-20240415/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/common.h` & `libfwnt-20240415/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/config_winapi.h` & `libfwnt-20240415/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/system_string.h` & `libfwnt-20240415/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/types.h.in` & `libfwnt-20240415/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/types.h` & `libfwnt-20240415/common/types.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/config.h.in` & `libfwnt-20240415/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/config.h` & `libfwnt-20240415/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -328,24 +328,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwnt"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwnt 20240126"
+#define PACKAGE_STRING "libfwnt 20240415"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwnt"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240126"
+#define PACKAGE_VERSION "20240415"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -363,15 +363,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240126"
+#define VERSION "20240415"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwnt-20240126/common/wide_string.h` & `libfwnt-20240415/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/narrow_string.h` & `libfwnt-20240415/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/config_msc.h` & `libfwnt-20240415/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/common/Makefile.in` & `libfwnt-20240415/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -380,15 +382,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -556,23 +561,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -652,15 +659,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_libcerror.h` & `libfwnt-20240415/pyfwnt/pyfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_security_descriptor.h` & `libfwnt-20240415/pyfwnt/pyfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_error.h` & `libfwnt-20240415/pyfwnt/pyfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_security_identifier.c` & `libfwnt-20240415/pyfwnt/pyfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_entries.c` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_entries.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_libfwnt.h` & `libfwnt-20240415/pyfwnt/pyfwnt_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_lzx.h` & `libfwnt-20240415/pyfwnt/pyfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_error.c` & `libfwnt-20240415/pyfwnt/pyfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/Makefile.am` & `libfwnt-20240415/pyfwnt/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBFWNT_DLL_IMPORT@
 
 pyexec_LTLIBRARIES = pyfwnt.la
 
 pyfwnt_la_SOURCES = \
@@ -32,13 +32,11 @@
 	@LIBCDATA_LIBADD@
 
 pyfwnt_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfwnt_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_integer.h` & `libfwnt-20240415/pyfwnt/pyfwnt_integer.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_lzxpress.c` & `libfwnt-20240415/pyfwnt/pyfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_entries.h` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_entries.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_entry.c` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_lzxpress.h` & `libfwnt-20240415/pyfwnt/pyfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_types.c` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_types.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_security_identifier.h` & `libfwnt-20240415/pyfwnt/pyfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_list.c` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_entry.h` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_types.h` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_types.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_python.h` & `libfwnt-20240415/pyfwnt/pyfwnt_python.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt.c` & `libfwnt-20240415/pyfwnt/pyfwnt.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_unused.h` & `libfwnt-20240415/pyfwnt/pyfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_lzx.c` & `libfwnt-20240415/pyfwnt/pyfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt.h` & `libfwnt-20240415/pyfwnt/pyfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/Makefile.in` & `libfwnt-20240415/pyfwnt/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -461,16 +461,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBFWNT_DLL_IMPORT@
 
 @HAVE_PYTHON_TRUE@pyexec_LTLIBRARIES = pyfwnt.la
 @HAVE_PYTHON_TRUE@pyfwnt_la_SOURCES = \
 @HAVE_PYTHON_TRUE@	pyfwnt.c pyfwnt.h \
@@ -493,15 +493,16 @@
 @HAVE_PYTHON_TRUE@pyfwnt_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../libfwnt/libfwnt.la \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyfwnt_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfwnt_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -823,24 +824,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_access_control_entries.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_access_control_entry.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_access_control_list.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_access_control_types.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_error.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_lznt1.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_lzx.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_lzxpress.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_security_descriptor.Plo
+	-rm -f ./$(DEPDIR)/pyfwnt_la-pyfwnt_security_identifier.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -936,13 +951,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_security_descriptor.c` & `libfwnt-20240415/pyfwnt/pyfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_lznt1.h` & `libfwnt-20240415/pyfwnt/pyfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_lznt1.c` & `libfwnt-20240415/pyfwnt/pyfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_access_control_list.h` & `libfwnt-20240415/pyfwnt/pyfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/pyfwnt/pyfwnt_integer.c` & `libfwnt-20240415/pyfwnt/pyfwnt_integer.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/Makefile.am` & `libfwnt-20240415/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -47,16 +47,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfwnt.pc \
+	libfwnt.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfwnt.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -69,19 +76,7 @@
 	(cd $(srcdir)/libcerror && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcthreads && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcnotify && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfwnt.pc
-	-rm -f libfwnt.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfwnt-20240126/config.guess` & `libfwnt-20240415/config.guess`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/dpkg/copyright` & `libfwnt-20240415/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/dpkg/control` & `libfwnt-20240415/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/dpkg/rules` & `libfwnt-20240415/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/COPYING.LESSER` & `libfwnt-20240415/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/configure` & `libfwnt-20240415/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwnt 20240126.
+# Generated by GNU Autoconf 2.71 for libfwnt 20240415.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfwnt'
 PACKAGE_TARNAME='libfwnt'
-PACKAGE_VERSION='20240126'
-PACKAGE_STRING='libfwnt 20240126'
+PACKAGE_VERSION='20240415'
+PACKAGE_STRING='libfwnt 20240415'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwnt.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1496,15 +1496,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwnt 20240126 to adapt to many kinds of systems.
+\`configure' configures libfwnt 20240415 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1567,15 +1567,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwnt 20240126:";;
+     short | recursive ) echo "Configuration of libfwnt 20240415:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1738,15 +1738,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwnt configure 20240126
+libfwnt configure 20240415
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2459,15 +2459,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwnt $as_me 20240126, which was
+It was created by libfwnt $as_me 20240415, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -3948,15 +3948,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwnt'
- VERSION='20240126'
+ VERSION='20240415'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23489,15 +23489,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -23988,15 +23988,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24138,15 +24139,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24240,15 +24241,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -25880,15 +25881,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -25942,47 +25943,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26016,15 +26022,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26058,15 +26064,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26101,15 +26107,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26143,15 +26149,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26185,15 +26191,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26227,15 +26233,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26269,15 +26275,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26312,15 +26318,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26354,15 +26360,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26396,15 +26402,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26438,15 +26444,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26480,15 +26486,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26523,15 +26529,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26565,15 +26571,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26607,15 +26613,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26649,15 +26655,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26691,15 +26697,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26734,67 +26740,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
 
 fi
 
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
+
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+fi
+
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -26882,15 +26897,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30661,15 +30676,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30694,15 +30710,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -30772,15 +30788,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31230,15 +31246,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31293,15 +31310,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32513,15 +32530,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwnt $as_me 20240126, which was
+This file was extended by libfwnt $as_me 20240415, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -32581,15 +32598,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwnt config.status 20240126
+libfwnt config.status 20240415
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwnt-20240126/compile` & `libfwnt-20240415/compile`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/missing` & `libfwnt-20240415/missing`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_lzx/fwnt_test_lzx.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_lzx/fwnt_test_lzx.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_error/fwnt_test_error.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_error/fwnt_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_security_descriptor/fwnt_test_security_descriptor.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_security_descriptor/fwnt_test_security_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/pyfwnt/pyfwnt.vcproj` & `libfwnt-20240415/msvscpp/pyfwnt/pyfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/Makefile.am` & `libfwnt-20240415/msvscpp/Makefile.am`

 * *Files 21% similar despite different names*

```diff
@@ -18,13 +18,11 @@
 	libfwnt/libfwnt.vcproj \
 	pyfwnt/pyfwnt.vcproj \
 	libfwnt.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_bit_stream/fwnt_test_bit_stream.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_bit_stream/fwnt_test_bit_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_lznt1/fwnt_test_lznt1.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_lznt1/fwnt_test_lznt1.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/libcdata/libcdata.vcproj` & `libfwnt-20240415/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_lzxpress/fwnt_test_lzxpress.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_lzxpress/fwnt_test_lzxpress.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_huffman_tree/fwnt_test_huffman_tree.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_huffman_tree/fwnt_test_huffman_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_access_control_entry/fwnt_test_access_control_entry.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_access_control_entry/fwnt_test_access_control_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/libcthreads/libcthreads.vcproj` & `libfwnt-20240415/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_access_control_list/fwnt_test_access_control_list.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_access_control_list/fwnt_test_access_control_list.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_support/fwnt_test_support.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_support/fwnt_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/libfwnt/libfwnt.vcproj` & `libfwnt-20240415/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/libfwnt.sln` & `libfwnt-20240415/msvscpp/libfwnt.sln`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/Makefile.in` & `libfwnt-20240415/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,16 @@
 	libfwnt/libfwnt.vcproj \
 	pyfwnt/pyfwnt.vcproj \
 	libfwnt.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -482,23 +483,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -577,13 +580,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwnt-20240126/msvscpp/libcnotify/libcnotify.vcproj` & `libfwnt-20240415/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/libcerror/libcerror.vcproj` & `libfwnt-20240415/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_security_identifier/fwnt_test_security_identifier.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_security_identifier/fwnt_test_security_identifier.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/msvscpp/fwnt_test_notify/fwnt_test_notify.vcproj` & `libfwnt-20240415/msvscpp/fwnt_test_notify/fwnt_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/INSTALL` & `libfwnt-20240415/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_list_element.h` & `libfwnt-20240415/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_array.h` & `libfwnt-20240415/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_definitions.h` & `libfwnt-20240415/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libfwnt-20240126/libcdata/libcdata_libcerror.h` & `libfwnt-20240415/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_unused.h` & `libfwnt-20240415/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_btree.h` & `libfwnt-20240415/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_btree.c` & `libfwnt-20240415/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_support.c` & `libfwnt-20240415/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_list.c` & `libfwnt-20240415/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_extern.h` & `libfwnt-20240415/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_list.h` & `libfwnt-20240415/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_btree_values_list.h` & `libfwnt-20240415/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/Makefile.am` & `libfwnt-20240415/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libfwnt-20240126/libcdata/libcdata_btree_node.h` & `libfwnt-20240415/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_range_list_value.h` & `libfwnt-20240415/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_range_list.h` & `libfwnt-20240415/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_range_list.c` & `libfwnt-20240415/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_array.c` & `libfwnt-20240415/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_list_element.c` & `libfwnt-20240415/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_libcthreads.h` & `libfwnt-20240415/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_tree_node.h` & `libfwnt-20240415/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_error.h` & `libfwnt-20240415/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_types.h` & `libfwnt-20240415/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_btree_node.c` & `libfwnt-20240415/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_tree_node.c` & `libfwnt-20240415/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_support.h` & `libfwnt-20240415/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/Makefile.in` & `libfwnt-20240415/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -426,16 +426,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -452,15 +452,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -670,24 +671,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -781,17 +795,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwnt-20240126/libcdata/libcdata_range_list_value.c` & `libfwnt-20240415/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_btree_values_list.c` & `libfwnt-20240415/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcdata/libcdata_error.c` & `libfwnt-20240415/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt.spec` & `libfwnt-20240415/libfwnt.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfwnt
-Version: 20240126
+Version: 20240415
 Release: 1
 Summary: Library to support common Windows NT specific formats
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwnt
     
@@ -76,10 +76,10 @@
 %files -n libfwnt-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Fri Jan 26 2024 Joachim Metz <joachim.metz@gmail.com> 20240126-1
+* Mon Apr 15 2024 Joachim Metz <joachim.metz@gmail.com> 20240415-1
 - Auto-generated
```

### Comparing `libfwnt-20240126/config.sub` & `libfwnt-20240415/config.sub`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/setup.py` & `libfwnt-20240415/setup.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/acinclude.m4` & `libfwnt-20240415/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/config.rpath` & `libfwnt-20240415/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_thread.h` & `libfwnt-20240415/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_read_write_lock.h` & `libfwnt-20240415/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_thread.c` & `libfwnt-20240415/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_thread_pool.h` & `libfwnt-20240415/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_support.h` & `libfwnt-20240415/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_lock.h` & `libfwnt-20240415/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_unused.h` & `libfwnt-20240415/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_lock.c` & `libfwnt-20240415/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_condition.h` & `libfwnt-20240415/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_repeating_thread.h` & `libfwnt-20240415/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/Makefile.am` & `libfwnt-20240415/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libfwnt-20240126/libcthreads/libcthreads_support.c` & `libfwnt-20240415/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_mutex.c` & `libfwnt-20240415/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_queue.c` & `libfwnt-20240415/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_mutex.h` & `libfwnt-20240415/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_types.h` & `libfwnt-20240415/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_thread_attributes.h` & `libfwnt-20240415/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_condition.c` & `libfwnt-20240415/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_error.c` & `libfwnt-20240415/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_read_write_lock.c` & `libfwnt-20240415/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_libcerror.h` & `libfwnt-20240415/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_definitions.h` & `libfwnt-20240415/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libfwnt-20240126/libcthreads/libcthreads_thread_pool.c` & `libfwnt-20240415/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_error.h` & `libfwnt-20240415/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_thread_attributes.c` & `libfwnt-20240415/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_extern.h` & `libfwnt-20240415/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/libcthreads_repeating_thread.c` & `libfwnt-20240415/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcthreads/Makefile.in` & `libfwnt-20240415/libcthreads/Makefile.in`

 * *Files 11% similar despite different names*

```diff
@@ -430,16 +430,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -454,15 +454,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -672,24 +673,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -783,17 +797,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwnt-20240126/libcthreads/libcthreads_queue.h` & `libfwnt-20240415/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/test-driver` & `libfwnt-20240415/test-driver`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ChangeLog` & `libfwnt-20240415/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/manuals/Makefile.in` & `libfwnt-20240415/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,16 @@
 top_srcdir = @top_srcdir@
 man_MANS = \
 	libfwnt.3
 
 EXTRA_DIST = \
 	libfwnt.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -541,23 +542,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -638,13 +641,10 @@
 	mostlyclean mostlyclean-generic mostlyclean-libtool pdf pdf-am \
 	ps ps-am sources-am sources-local splint-am splint-local \
 	tags-am uninstall uninstall-am uninstall-man uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwnt-20240126/manuals/libfwnt.3` & `libfwnt-20240415/manuals/libfwnt.3`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_notify.c` & `libfwnt-20240415/tests/fwnt_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_security_descriptor.py` & `libfwnt-20240415/tests/pyfwnt_test_security_descriptor.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_support.py` & `libfwnt-20240415/tests/pyfwnt_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_access_control_list.py` & `libfwnt-20240415/tests/pyfwnt_test_access_control_list.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_security_descriptor.c` & `libfwnt-20240415/tests/fwnt_test_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_lzx.c` & `libfwnt-20240415/tests/fwnt_test_lzx.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_libcerror.h` & `libfwnt-20240415/tests/fwnt_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_huffman_tree.c` & `libfwnt-20240415/tests/fwnt_test_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_libcnotify.h` & `libfwnt-20240415/tests/fwnt_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_memory.c` & `libfwnt-20240415/tests/fwnt_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_security_identifier.py` & `libfwnt-20240415/tests/pyfwnt_test_security_identifier.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_lzxpress.py` & `libfwnt-20240415/tests/pyfwnt_test_lzxpress.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/Makefile.am` & `libfwnt-20240415/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFWNT_DLL_IMPORT@
 
@@ -184,13 +184,12 @@
 	fwnt_test_macros.h \
 	fwnt_test_support.c \
 	fwnt_test_unused.h
 
 fwnt_test_support_LDADD = \
 	../libfwnt/libfwnt.la
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libfwnt-20240126/tests/fwnt_test_libfwnt.h` & `libfwnt-20240415/tests/fwnt_test_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/test_python_module.sh` & `libfwnt-20240415/tests/test_python_module.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="access_control_entry access_control_list lznt1 lzx lzxpress security_descriptor security_identifier support";
@@ -121,20 +121,17 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libfwnt-20240126/tests/fwnt_test_lzxpress.c` & `libfwnt-20240415/tests/fwnt_test_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_support.c` & `libfwnt-20240415/tests/fwnt_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_unused.h` & `libfwnt-20240415/tests/fwnt_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/test_runner.sh` & `libfwnt-20240415/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_access_control_list.c` & `libfwnt-20240415/tests/fwnt_test_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_security_identifier.c` & `libfwnt-20240415/tests/fwnt_test_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_access_control_entry.py` & `libfwnt-20240415/tests/pyfwnt_test_access_control_entry.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_bit_stream.c` & `libfwnt-20240415/tests/fwnt_test_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_lzx.py` & `libfwnt-20240415/tests/pyfwnt_test_lzx.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/pyfwnt_test_lznt1.py` & `libfwnt-20240415/tests/pyfwnt_test_lznt1.py`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_lznt1.c` & `libfwnt-20240415/tests/fwnt_test_lznt1.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_macros.h` & `libfwnt-20240415/tests/fwnt_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_error.c` & `libfwnt-20240415/tests/fwnt_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/Makefile.in` & `libfwnt-20240415/tests/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -680,16 +680,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFWNT_DLL_IMPORT@
 
@@ -853,16 +853,18 @@
 	fwnt_test_macros.h \
 	fwnt_test_support.c \
 	fwnt_test_unused.h
 
 fwnt_test_support_LDADD = \
 	../libfwnt/libfwnt.la
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1291,24 +1293,39 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/fwnt_test_access_control_entry.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_access_control_list.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_bit_stream.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_error.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_huffman_tree.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_lznt1.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_lzx.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_lzxpress.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_memory.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_notify.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_security_descriptor.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_security_identifier.Po
+	-rm -f ./$(DEPDIR)/fwnt_test_support.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1404,13 +1421,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwnt-20240126/tests/fwnt_test_access_control_entry.c` & `libfwnt-20240415/tests/fwnt_test_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/fwnt_test_memory.h` & `libfwnt-20240415/tests/fwnt_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/tests/test_library.sh` & `libfwnt-20240415/tests/test_library.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="access_control_entry access_control_list bit_stream error huffman_tree lznt1 lzx lzxpress notify security_descriptor security_identifier support";
 LIBRARY_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libfwnt-20240126/ossfuzz/lzxpress_fuzzer.cc` & `libfwnt-20240415/ossfuzz/lzxpress_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ossfuzz/Makefile.am` & `libfwnt-20240415/ossfuzz/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
 	lznt1_fuzzer \
 	lzx_fuzzer \
 	lzxpress_fuzzer \
 	lzxpress_huffman_fuzzer \
 	security_descriptor_fuzzer \
@@ -56,20 +56,18 @@
 	security_identifier_fuzzer.cc
 
 security_identifier_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libfwnt/libfwnt.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on lznt1_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lznt1_fuzzer_SOURCES)
 	@echo "Running splint on lzx_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzx_fuzzer_SOURCES)
 	@echo "Running splint on lzxpress_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzxpress_fuzzer_SOURCES)
```

### Comparing `libfwnt-20240126/ossfuzz/lzx_fuzzer.cc` & `libfwnt-20240415/ossfuzz/lzx_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ossfuzz/ossfuzz_libfwnt.h` & `libfwnt-20240415/ossfuzz/ossfuzz_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ossfuzz/security_identifier_fuzzer.cc` & `libfwnt-20240415/ossfuzz/security_identifier_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ossfuzz/lznt1_fuzzer.cc` & `libfwnt-20240415/ossfuzz/lznt1_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ossfuzz/Makefile.in` & `libfwnt-20240415/ossfuzz/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -469,16 +469,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@lznt1_fuzzer_SOURCES = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	lznt1_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfwnt.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@lznt1_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
@@ -520,15 +520,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfwnt.h \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	security_identifier_fuzzer.cc
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@security_identifier_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfwnt/libfwnt.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -795,23 +796,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/lznt1_fuzzer.Po
+	-rm -f ./$(DEPDIR)/lzx_fuzzer.Po
+	-rm -f ./$(DEPDIR)/lzxpress_fuzzer.Po
+	-rm -f ./$(DEPDIR)/lzxpress_huffman_fuzzer.Po
+	-rm -f ./$(DEPDIR)/security_descriptor_fuzzer.Po
+	-rm -f ./$(DEPDIR)/security_identifier_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -900,17 +909,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on lznt1_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lznt1_fuzzer_SOURCES)
 	@echo "Running splint on lzx_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzx_fuzzer_SOURCES)
 	@echo "Running splint on lzxpress_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzxpress_fuzzer_SOURCES)
```

### Comparing `libfwnt-20240126/ossfuzz/security_descriptor_fuzzer.cc` & `libfwnt-20240415/ossfuzz/security_descriptor_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ossfuzz/lzxpress_huffman_fuzzer.cc` & `libfwnt-20240415/ossfuzz/lzxpress_huffman_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/ltmain.sh` & `libfwnt-20240415/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_locale_identifier.h` & `libfwnt-20240415/libfwnt/libfwnt_locale_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_lzxpress.c` & `libfwnt-20240415/libfwnt/libfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_extern.h` & `libfwnt-20240415/libfwnt/libfwnt_extern.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_security_identifier.c` & `libfwnt-20240415/libfwnt/libfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_libcerror.h` & `libfwnt-20240415/libfwnt/libfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_bit_stream.c` & `libfwnt-20240415/libfwnt/libfwnt_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_error.h` & `libfwnt-20240415/libfwnt/libfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_definitions.h.in` & `libfwnt-20240415/libfwnt/libfwnt_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_lznt1.h` & `libfwnt-20240415/libfwnt/libfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt.c` & `libfwnt-20240415/libfwnt/libfwnt.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_notify.c` & `libfwnt-20240415/libfwnt/libfwnt_notify.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/Makefile.am` & `libfwnt-20240415/libfwnt/Makefile.am`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFWNT_DLL_EXPORT@
 
@@ -44,21 +44,19 @@
 libfwnt_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfwnt_definitions.h.in \
 	libfwnt.rc \
 	libfwnt.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwnt_definitions.h \
+	libfwnt.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfwnt_definitions.h
-	-rm -f libfwnt.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
```

### Comparing `libfwnt-20240126/libfwnt/libfwnt_security_identifier.h` & `libfwnt-20240415/libfwnt/libfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt.rc` & `libfwnt-20240415/libfwnt/libfwnt.rc`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support common Windows NT specific formats\0"
-      VALUE "FileVersion",		"20240126" "\0"
+      VALUE "FileVersion",		"20240415" "\0"
       VALUE "InternalName",		"libfwnt.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwnt.dll\0"
       VALUE "ProductName",		"libfwnt\0"
-      VALUE "ProductVersion",		"20240126" "\0"
+      VALUE "ProductVersion",		"20240415" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwnt/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwnt-20240126/libfwnt/libfwnt_support.h` & `libfwnt-20240415/libfwnt/libfwnt_support.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_huffman_tree.h` & `libfwnt-20240415/libfwnt/libfwnt_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt.rc.in` & `libfwnt-20240415/libfwnt/libfwnt.rc.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_error.c` & `libfwnt-20240415/libfwnt/libfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_access_control_list.h` & `libfwnt-20240415/libfwnt/libfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_security_descriptor.c` & `libfwnt-20240415/libfwnt/libfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_access_control_list.c` & `libfwnt-20240415/libfwnt/libfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_definitions.h` & `libfwnt-20240415/libfwnt/libfwnt_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwnt/definitions.h> are copied here
  * for local use of libfwnt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWNT_VERSION					20240126
+#define LIBFWNT_VERSION					20240415
 
 /* The version string
  */
-#define LIBFWNT_VERSION_STRING				"20240126"
+#define LIBFWNT_VERSION_STRING				"20240415"
 
 
 /* The endian definitions
  */
 #define LIBFWNT_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWNT_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
```

### Comparing `libfwnt-20240126/libfwnt/libfwnt_huffman_tree.c` & `libfwnt-20240415/libfwnt/libfwnt_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_debug.c` & `libfwnt-20240415/libfwnt/libfwnt_debug.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_lznt1.c` & `libfwnt-20240415/libfwnt/libfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_notify.h` & `libfwnt-20240415/libfwnt/libfwnt_notify.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_locale_identifier.c` & `libfwnt-20240415/libfwnt/libfwnt_locale_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_debug.h` & `libfwnt-20240415/libfwnt/libfwnt_debug.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_libcdata.h` & `libfwnt-20240415/libfwnt/libfwnt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_lzx.h` & `libfwnt-20240415/libfwnt/libfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_unused.h` & `libfwnt-20240415/libfwnt/libfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_libcnotify.h` & `libfwnt-20240415/libfwnt/libfwnt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_access_control_entry.c` & `libfwnt-20240415/libfwnt/libfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_lzxpress.h` & `libfwnt-20240415/libfwnt/libfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_security_descriptor.h` & `libfwnt-20240415/libfwnt/libfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_lzx.c` & `libfwnt-20240415/libfwnt/libfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/Makefile.in` & `libfwnt-20240415/libfwnt/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -445,16 +445,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFWNT_DLL_EXPORT@
 
@@ -492,15 +492,18 @@
 
 libfwnt_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfwnt_definitions.h.in \
 	libfwnt.rc \
 	libfwnt.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfwnt_definitions.h \
+	libfwnt.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -745,24 +748,41 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwnt.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_access_control_entry.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_access_control_list.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_error.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_locale_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lznt1.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzx.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzxpress.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -860,19 +880,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfwnt_definitions.h
-	-rm -f libfwnt.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwnt-20240126/libfwnt/libfwnt_bit_stream.h` & `libfwnt-20240415/libfwnt/libfwnt_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_types.h` & `libfwnt-20240415/libfwnt/libfwnt_types.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_support.c` & `libfwnt-20240415/libfwnt/libfwnt_support.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libfwnt/libfwnt_access_control_entry.h` & `libfwnt-20240415/libfwnt/libfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/remove-potcdate.sin` & `libfwnt-20240415/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/Makefile.in.in` & `libfwnt-20240415/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/en@quot.header` & `libfwnt-20240415/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/en@boldquot.header` & `libfwnt-20240415/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/insert-header.sin` & `libfwnt-20240415/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/Makevars` & `libfwnt-20240415/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/Makevars.in` & `libfwnt-20240415/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/po/Rules-quot` & `libfwnt-20240415/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/Makefile.in` & `libfwnt-20240415/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -517,16 +517,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libfwnt.pc \
+	libfwnt.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfwnt.pc
 
 all: all-recursive
 
@@ -943,23 +950,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1060,22 +1070,10 @@
 	(cd $(srcdir)/libcerror && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcthreads && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcnotify && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfwnt.pc
-	-rm -f libfwnt.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfwnt-20240126/libcnotify/libcnotify_definitions.h` & `libfwnt-20240415/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libfwnt-20240126/libcnotify/libcnotify_extern.h` & `libfwnt-20240415/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_support.c` & `libfwnt-20240415/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_stream.h` & `libfwnt-20240415/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/Makefile.am` & `libfwnt-20240415/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libfwnt-20240126/libcnotify/libcnotify_unused.h` & `libfwnt-20240415/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_verbose.h` & `libfwnt-20240415/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_print.h` & `libfwnt-20240415/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_stream.c` & `libfwnt-20240415/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_support.h` & `libfwnt-20240415/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_verbose.c` & `libfwnt-20240415/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/Makefile.in` & `libfwnt-20240415/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -408,30 +408,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -634,24 +635,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -738,17 +745,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwnt-20240126/libcnotify/libcnotify_libcerror.h` & `libfwnt-20240415/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcnotify/libcnotify_print.c` & `libfwnt-20240415/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_system.c` & `libfwnt-20240415/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_error.c` & `libfwnt-20240415/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_extern.h` & `libfwnt-20240415/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/Makefile.am` & `libfwnt-20240415/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libfwnt-20240126/libcerror/libcerror_types.h` & `libfwnt-20240415/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_support.h` & `libfwnt-20240415/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_error.h` & `libfwnt-20240415/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_system.h` & `libfwnt-20240415/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_definitions.h` & `libfwnt-20240415/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libfwnt-20240126/libcerror/libcerror_support.c` & `libfwnt-20240415/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/libcerror_unused.h` & `libfwnt-20240415/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/libcerror/Makefile.in` & `libfwnt-20240415/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -405,28 +405,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -628,24 +629,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -731,17 +737,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfwnt-20240126/libfwnt.spec.in` & `libfwnt-20240415/libfwnt.spec.in`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/aclocal.m4` & `libfwnt-20240415/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwnt-20240126/configure.ac` & `libfwnt-20240415/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwnt],
- [20240126],
+ [20240415],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwnt.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

