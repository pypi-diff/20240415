# Comparing `tmp/libfmos-python-20240118.tar.gz` & `tmp/libfmos-python-20240415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfmos-python-20240118.tar", last modified: Thu Jan 18 05:01:10 2024, max compression
+gzip compressed data, was "libfmos-python-20240415.tar", last modified: Mon Apr 15 18:29:22 2024, max compression
```

## Comparing `libfmos-python-20240118.tar` & `libfmos-python-20240415.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2024-01-18 04:50:44.000000 libfmos-20240118/libfmos.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/libfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2023 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzfse_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2269 2024-01-18 04:53:54.000000 libfmos-20240118/libfmos/libfmos_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzfse_decoder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-01-18 04:51:47.000000 libfmos-20240118/libfmos/libfmos_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7799 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_adc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3441 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzfse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1321 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_adc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2271 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-12-03 09:04:57.000000 libfmos-20240118/libfmos/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25840 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzvn.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6380 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzfse_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3271 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzfse_decoder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60280 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzfse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-01-18 04:53:54.000000 libfmos-20240118/libfmos/libfmos.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1326 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_lzvn.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-18 04:50:45.000000 libfmos-20240118/libfmos/libfmos_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27551 2024-01-18 04:53:48.000000 libfmos-20240118/libfmos/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-18 04:50:44.000000 libfmos-20240118/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-18 04:53:47.000000 libfmos-20240118/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 04:50:44.000000 libfmos-20240118/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-18 04:53:48.000000 libfmos-20240118/depcomp
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2161 2024-01-18 04:50:44.000000 libfmos-20240118/libfmos.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:04:58.000000 libfmos-20240118/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:04:58.000000 libfmos-20240118/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:04:58.000000 libfmos-20240118/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:04:58.000000 libfmos-20240118/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:04:58.000000 libfmos-20240118/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:04:58.000000 libfmos-20240118/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:04:58.000000 libfmos-20240118/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-18 04:53:45.000000 libfmos-20240118/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-18 04:53:45.000000 libfmos-20240118/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:04:58.000000 libfmos-20240118/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-18 04:53:45.000000 libfmos-20240118/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:04:58.000000 libfmos-20240118/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:04:58.000000 libfmos-20240118/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:04:58.000000 libfmos-20240118/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:04:58.000000 libfmos-20240118/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-18 04:53:45.000000 libfmos-20240118/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:04:58.000000 libfmos-20240118/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:04:58.000000 libfmos-20240118/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-18 04:53:45.000000 libfmos-20240118/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:04:58.000000 libfmos-20240118/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:04:58.000000 libfmos-20240118/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:04:58.000000 libfmos-20240118/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:04:58.000000 libfmos-20240118/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/include/libfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1067 2024-01-18 04:50:44.000000 libfmos-20240118/include/libfmos/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1065 2024-01-18 04:53:54.000000 libfmos-20240118/include/libfmos/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4831 2024-01-18 04:50:44.000000 libfmos-20240118/include/libfmos/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-01-18 04:53:54.000000 libfmos-20240118/include/libfmos/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-18 04:51:38.000000 libfmos-20240118/include/libfmos/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-01-18 04:50:44.000000 libfmos-20240118/include/libfmos/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-18 04:50:44.000000 libfmos-20240118/include/libfmos/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-01-18 04:53:54.000000 libfmos-20240118/include/libfmos/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5171 2024-01-18 04:50:44.000000 libfmos-20240118/include/libfmos.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      437 2024-01-18 04:50:44.000000 libfmos-20240118/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5171 2024-01-18 04:53:54.000000 libfmos-20240118/include/libfmos.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22141 2024-01-18 04:53:48.000000 libfmos-20240118/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-18 04:50:44.000000 libfmos-20240118/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-18 04:50:44.000000 libfmos-20240118/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-18 04:50:44.000000 libfmos-20240118/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-18 04:50:44.000000 libfmos-20240118/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-18 04:50:44.000000 libfmos-20240118/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-18 04:50:44.000000 libfmos-20240118/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-18 04:50:44.000000 libfmos-20240118/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-18 04:50:44.000000 libfmos-20240118/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-18 04:50:44.000000 libfmos-20240118/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-01-18 04:53:54.000000 libfmos-20240118/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10268 2024-01-18 04:53:47.000000 libfmos-20240118/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-01-18 04:53:54.000000 libfmos-20240118/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-18 04:50:44.000000 libfmos-20240118/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-18 04:50:44.000000 libfmos-20240118/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-18 04:50:44.000000 libfmos-20240118/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19189 2024-01-18 04:53:48.000000 libfmos-20240118/common/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-12-03 09:04:52.000000 libfmos-20240118/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:04:52.000000 libfmos-20240118/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-18 04:53:47.000000 libfmos-20240118/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-01-18 04:50:45.000000 libfmos-20240118/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-01-18 04:53:54.000000 libfmos-20240118/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/libfmos.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/libfmos-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-18 04:50:44.000000 libfmos-20240118/dpkg/libfmos-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-01-18 04:53:54.000000 libfmos-20240118/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-18 04:50:44.000000 libfmos-20240118/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)   942110 2024-01-18 04:53:47.000000 libfmos-20240118/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/pyfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_libfmos.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1196 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_lzvn.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_lzfse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4867 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_lzvn.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      660 2023-12-03 09:04:58.000000 libfmos-20240118/pyfmos/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4873 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_lzfse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1191 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_adc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4398 2024-01-18 04:51:38.000000 libfmos-20240118/pyfmos/pyfmos.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4874 2024-01-18 04:50:45.000000 libfmos-20240118/pyfmos/pyfmos_adc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32127 2024-01-18 04:53:48.000000 libfmos-20240118/pyfmos/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-18 04:53:47.000000 libfmos-20240118/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-18 04:53:47.000000 libfmos-20240118/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_lzfse_decoder/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4971 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/fmos_test_lzfse_decoder/fmos_test_lzfse_decoder.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_adc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4941 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/fmos_test_adc/fmos_test_adc.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/libfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6277 2024-01-18 04:50:48.000000 libfmos-20240118/msvscpp/libfmos/libfmos.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      660 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-01-18 04:50:48.000000 libfmos-20240118/msvscpp/fmos_test_notify/fmos_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/pyfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5317 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/pyfmos/pyfmos.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_lzfse_bit_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4980 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/fmos_test_lzfse_bit_stream/fmos_test_lzfse_bit_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_lzfse/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4947 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/fmos_test_lzfse/fmos_test_lzfse.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-01-18 04:50:48.000000 libfmos-20240118/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4780 2024-01-18 04:50:48.000000 libfmos-20240118/msvscpp/fmos_test_error/fmos_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4786 2024-01-18 04:50:48.000000 libfmos-20240118/msvscpp/fmos_test_support/fmos_test_support.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9803 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/libfmos.sln
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16817 2024-01-18 04:53:48.000000 libfmos-20240118/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-01-18 04:50:48.000000 libfmos-20240118/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-18 04:50:48.000000 libfmos-20240118/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/msvscpp/fmos_test_lzvn/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4944 2024-01-18 04:51:26.000000 libfmos-20240118/msvscpp/fmos_test_lzvn/fmos_test_lzvn.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-18 04:50:44.000000 libfmos-20240118/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      283 2024-01-18 04:50:44.000000 libfmos-20240118/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-18 04:53:47.000000 libfmos-20240118/INSTALL
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-18 04:50:44.000000 libfmos-20240118/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-01-18 04:50:44.000000 libfmos-20240118/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-18 04:53:47.000000 libfmos-20240118/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-18 04:50:44.000000 libfmos-20240118/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-01-18 04:50:44.000000 libfmos-20240118/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:04:52.000000 libfmos-20240118/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27046 2024-01-18 04:53:48.000000 libfmos-20240118/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-18 04:53:42.000000 libfmos-20240118/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-18 04:53:48.000000 libfmos-20240118/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      208 2023-12-03 09:04:52.000000 libfmos-20240118/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      126 2023-12-03 09:04:58.000000 libfmos-20240118/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2281 2024-01-18 04:50:45.000000 libfmos-20240118/manuals/libfmos.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19393 2024-01-18 04:53:48.000000 libfmos-20240118/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   109351 2024-01-18 04:50:45.000000 libfmos-20240118/tests/pyfmos_test_lzfse.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4813 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_adc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13719 2024-01-18 04:51:26.000000 libfmos-20240118/tests/fmos_test_lzfse_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4667 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_lzvn.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2698 2024-01-18 04:51:26.000000 libfmos-20240118/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-18 04:50:45.000000 libfmos-20240118/tests/pyfmos_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-18 04:50:45.000000 libfmos-20240118/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3830 2024-01-18 04:51:38.000000 libfmos-20240118/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_libfmos.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1690 2024-01-18 04:50:45.000000 libfmos-20240118/tests/pyfmos_test_lzvn.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-18 04:50:45.000000 libfmos-20240118/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-01-18 04:50:45.000000 libfmos-20240118/tests/pyfmos_test_adc.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43629 2024-01-18 04:53:48.000000 libfmos-20240118/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48212 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_lzfse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6194 2024-01-18 04:51:26.000000 libfmos-20240118/tests/fmos_test_lzfse_decoder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-01-18 04:50:45.000000 libfmos-20240118/tests/fmos_test_macros.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4104 2024-01-18 04:51:38.000000 libfmos-20240118/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-01-18 04:50:45.000000 libfmos-20240118/ossfuzz/ossfuzz_libfmos.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1279 2024-01-18 04:50:45.000000 libfmos-20240118/ossfuzz/adc_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2023-12-03 09:04:59.000000 libfmos-20240118/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2024-01-18 04:50:45.000000 libfmos-20240118/ossfuzz/lzfse_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28001 2024-01-18 04:53:48.000000 libfmos-20240118/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1281 2024-01-18 04:50:45.000000 libfmos-20240118/ossfuzz/lzvn_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-18 04:53:45.000000 libfmos-20240118/ltmain.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1948 2024-01-18 04:53:54.000000 libfmos-20240118/libfmos.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:04:58.000000 libfmos-20240118/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:04:58.000000 libfmos-20240118/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:04:58.000000 libfmos-20240118/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:04:58.000000 libfmos-20240118/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:04:58.000000 libfmos-20240118/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:04:58.000000 libfmos-20240118/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:04:58.000000 libfmos-20240118/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:04:58.000000 libfmos-20240118/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:04:58.000000 libfmos-20240118/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-01-18 04:53:54.000000 libfmos-20240118/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:04:58.000000 libfmos-20240118/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:04:58.000000 libfmos-20240118/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34462 2024-01-18 04:53:47.000000 libfmos-20240118/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24068 2024-01-18 04:53:48.000000 libfmos-20240118/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-01-18 04:53:41.000000 libfmos-20240118/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-18 05:01:10.000000 libfmos-20240118/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-18 04:53:40.000000 libfmos-20240118/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23581 2024-01-18 04:53:48.000000 libfmos-20240118/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56474 2024-01-18 04:53:46.000000 libfmos-20240118/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4264 2024-01-18 04:50:44.000000 libfmos-20240118/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-01-18 05:01:10.867761 libfmos-20240118/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2024-04-15 16:24:35.000000 libfmos-20240415/libfmos.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:20.000000 libfmos-20240415/libfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2023 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzfse_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2269 2024-04-15 16:39:52.000000 libfmos-20240415/libfmos/libfmos_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzfse_decoder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-15 16:29:22.000000 libfmos-20240415/libfmos/libfmos_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7799 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_adc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3441 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzfse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1321 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_adc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2271 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1240 2024-04-15 16:26:34.000000 libfmos-20240415/libfmos/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25840 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzvn.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6380 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzfse_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3271 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzfse_decoder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60280 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzfse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-04-15 16:39:52.000000 libfmos-20240415/libfmos/libfmos.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1326 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_lzvn.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-15 16:24:37.000000 libfmos-20240415/libfmos/libfmos_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27922 2024-04-15 16:39:37.000000 libfmos-20240415/libfmos/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-15 16:24:35.000000 libfmos-20240415/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-15 16:39:37.000000 libfmos-20240415/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 16:24:35.000000 libfmos-20240415/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-15 16:39:37.000000 libfmos-20240415/depcomp
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2161 2024-04-15 16:24:35.000000 libfmos-20240415/libfmos.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:19.000000 libfmos-20240415/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:04:58.000000 libfmos-20240415/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:04:58.000000 libfmos-20240415/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:04:58.000000 libfmos-20240415/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:04:58.000000 libfmos-20240415/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:04:58.000000 libfmos-20240415/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-04 04:21:25.000000 libfmos-20240415/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-15 16:24:37.000000 libfmos-20240415/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-15 16:39:34.000000 libfmos-20240415/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-15 16:39:34.000000 libfmos-20240415/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:04:58.000000 libfmos-20240415/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-15 16:39:34.000000 libfmos-20240415/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:04:58.000000 libfmos-20240415/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-15 16:24:37.000000 libfmos-20240415/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-15 16:24:37.000000 libfmos-20240415/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:04:58.000000 libfmos-20240415/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-15 16:39:34.000000 libfmos-20240415/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:04:58.000000 libfmos-20240415/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:04:58.000000 libfmos-20240415/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-15 16:39:34.000000 libfmos-20240415/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:04:58.000000 libfmos-20240415/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:04:58.000000 libfmos-20240415/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:04:58.000000 libfmos-20240415/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-04 04:21:25.000000 libfmos-20240415/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:19.000000 libfmos-20240415/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:19.000000 libfmos-20240415/include/libfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1067 2024-04-15 16:24:36.000000 libfmos-20240415/include/libfmos/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1065 2024-04-15 16:39:51.000000 libfmos-20240415/include/libfmos/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4831 2024-04-15 16:24:36.000000 libfmos-20240415/include/libfmos/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-15 16:39:51.000000 libfmos-20240415/include/libfmos/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-15 16:28:06.000000 libfmos-20240415/include/libfmos/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-15 16:24:36.000000 libfmos-20240415/include/libfmos/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-15 16:24:36.000000 libfmos-20240415/include/libfmos/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-15 16:39:51.000000 libfmos-20240415/include/libfmos/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5171 2024-04-15 16:24:36.000000 libfmos-20240415/include/libfmos.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      388 2024-04-15 16:25:05.000000 libfmos-20240415/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5171 2024-04-15 16:39:51.000000 libfmos-20240415/include/libfmos.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22121 2024-04-15 16:39:37.000000 libfmos-20240415/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:20.000000 libfmos-20240415/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-15 16:24:36.000000 libfmos-20240415/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-15 16:24:36.000000 libfmos-20240415/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-15 16:24:36.000000 libfmos-20240415/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-15 16:24:36.000000 libfmos-20240415/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-15 16:24:36.000000 libfmos-20240415/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-15 16:24:36.000000 libfmos-20240415/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-15 16:24:36.000000 libfmos-20240415/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-15 16:25:05.000000 libfmos-20240415/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-15 16:24:36.000000 libfmos-20240415/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-15 16:39:52.000000 libfmos-20240415/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10268 2024-04-15 16:39:36.000000 libfmos-20240415/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-15 16:39:52.000000 libfmos-20240415/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-15 16:24:36.000000 libfmos-20240415/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-15 16:24:36.000000 libfmos-20240415/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-15 16:24:36.000000 libfmos-20240415/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19196 2024-04-15 16:39:37.000000 libfmos-20240415/common/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1329 2024-04-15 16:26:17.000000 libfmos-20240415/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:04:52.000000 libfmos-20240415/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-15 16:39:37.000000 libfmos-20240415/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:19.000000 libfmos-20240415/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-15 16:24:37.000000 libfmos-20240415/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:19.000000 libfmos-20240415/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-15 16:39:52.000000 libfmos-20240415/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/libfmos.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/libfmos-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-15 16:24:35.000000 libfmos-20240415/dpkg/libfmos-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-04-15 16:39:52.000000 libfmos-20240415/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-15 16:24:35.000000 libfmos-20240415/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)   943144 2024-04-15 16:39:36.000000 libfmos-20240415/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:20.000000 libfmos-20240415/pyfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_libfmos.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1196 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_lzvn.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_lzfse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4867 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_lzvn.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      656 2024-04-15 16:26:44.000000 libfmos-20240415/pyfmos/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4873 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_lzfse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1191 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_adc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4398 2024-04-15 16:28:06.000000 libfmos-20240415/pyfmos/pyfmos.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4874 2024-04-15 16:24:37.000000 libfmos-20240415/pyfmos/pyfmos_adc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32379 2024-04-15 16:39:37.000000 libfmos-20240415/pyfmos/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-15 16:39:37.000000 libfmos-20240415/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-15 16:39:37.000000 libfmos-20240415/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_lzfse_decoder/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4971 2024-04-15 16:24:55.000000 libfmos-20240415/msvscpp/fmos_test_lzfse_decoder/fmos_test_lzfse_decoder.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_adc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4941 2024-04-15 16:24:55.000000 libfmos-20240415/msvscpp/fmos_test_adc/fmos_test_adc.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/libfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6277 2024-04-15 16:24:41.000000 libfmos-20240415/msvscpp/libfmos/libfmos.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      631 2024-04-15 16:26:59.000000 libfmos-20240415/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4866 2024-04-15 16:24:41.000000 libfmos-20240415/msvscpp/fmos_test_notify/fmos_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/pyfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5317 2024-04-15 16:24:55.000000 libfmos-20240415/msvscpp/pyfmos/pyfmos.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_lzfse_bit_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4980 2024-04-15 16:24:55.000000 libfmos-20240415/msvscpp/fmos_test_lzfse_bit_stream/fmos_test_lzfse_bit_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_lzfse/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4947 2024-04-15 16:24:55.000000 libfmos-20240415/msvscpp/fmos_test_lzfse/fmos_test_lzfse.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-15 16:24:41.000000 libfmos-20240415/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4780 2024-04-15 16:24:41.000000 libfmos-20240415/msvscpp/fmos_test_error/fmos_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4786 2024-04-15 16:24:41.000000 libfmos-20240415/msvscpp/fmos_test_support/fmos_test_support.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9803 2024-04-15 16:24:55.000000 libfmos-20240415/msvscpp/libfmos.sln
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16817 2024-04-15 16:39:37.000000 libfmos-20240415/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-15 16:24:41.000000 libfmos-20240415/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-15 16:24:41.000000 libfmos-20240415/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/msvscpp/fmos_test_lzvn/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4944 2024-04-15 16:24:55.000000 libfmos-20240415/msvscpp/fmos_test_lzvn/fmos_test_lzvn.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-15 16:24:36.000000 libfmos-20240415/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      283 2024-04-15 16:24:35.000000 libfmos-20240415/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-15 16:39:37.000000 libfmos-20240415/INSTALL
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-15 16:24:35.000000 libfmos-20240415/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-04-15 16:24:35.000000 libfmos-20240415/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-15 16:39:37.000000 libfmos-20240415/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-15 16:24:35.000000 libfmos-20240415/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-04-15 16:24:55.000000 libfmos-20240415/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:04:52.000000 libfmos-20240415/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:20.000000 libfmos-20240415/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27579 2024-04-15 16:39:37.000000 libfmos-20240415/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-15 16:39:30.000000 libfmos-20240415/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-15 16:39:37.000000 libfmos-20240415/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      208 2023-12-03 09:04:52.000000 libfmos-20240415/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       97 2024-04-15 16:27:12.000000 libfmos-20240415/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2281 2024-04-15 16:24:37.000000 libfmos-20240415/manuals/libfmos.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19393 2024-04-15 16:39:37.000000 libfmos-20240415/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   109351 2024-04-15 16:24:37.000000 libfmos-20240415/tests/pyfmos_test_lzfse.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4813 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_adc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13719 2024-04-15 16:24:55.000000 libfmos-20240415/tests/fmos_test_lzfse_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4667 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_lzvn.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2715 2024-04-15 16:34:03.000000 libfmos-20240415/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-15 16:24:37.000000 libfmos-20240415/tests/pyfmos_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-15 16:24:37.000000 libfmos-20240415/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4053 2024-04-15 16:30:24.000000 libfmos-20240415/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_libfmos.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1690 2024-04-15 16:24:37.000000 libfmos-20240415/tests/pyfmos_test_lzvn.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-15 16:24:37.000000 libfmos-20240415/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-04-15 16:24:37.000000 libfmos-20240415/tests/pyfmos_test_adc.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44007 2024-04-15 16:39:37.000000 libfmos-20240415/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48212 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_lzfse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6194 2024-04-15 16:24:55.000000 libfmos-20240415/tests/fmos_test_lzfse_decoder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-15 16:24:37.000000 libfmos-20240415/tests/fmos_test_macros.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4073 2024-04-15 16:28:28.000000 libfmos-20240415/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-15 16:24:37.000000 libfmos-20240415/ossfuzz/ossfuzz_libfmos.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1279 2024-04-15 16:24:37.000000 libfmos-20240415/ossfuzz/adc_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1081 2024-04-15 16:27:37.000000 libfmos-20240415/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2024-04-15 16:24:37.000000 libfmos-20240415/ossfuzz/lzfse_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28132 2024-04-15 16:39:37.000000 libfmos-20240415/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1281 2024-04-15 16:24:37.000000 libfmos-20240415/ossfuzz/lzvn_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-15 16:39:33.000000 libfmos-20240415/ltmain.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1948 2024-04-15 16:39:52.000000 libfmos-20240415/libfmos.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:21.000000 libfmos-20240415/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:04:58.000000 libfmos-20240415/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:04:58.000000 libfmos-20240415/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:04:58.000000 libfmos-20240415/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:04:58.000000 libfmos-20240415/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:04:58.000000 libfmos-20240415/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:04:58.000000 libfmos-20240415/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:04:58.000000 libfmos-20240415/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:04:58.000000 libfmos-20240415/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:04:58.000000 libfmos-20240415/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-15 16:39:51.000000 libfmos-20240415/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:04:58.000000 libfmos-20240415/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:04:58.000000 libfmos-20240415/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34344 2024-04-15 16:39:37.000000 libfmos-20240415/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:20.000000 libfmos-20240415/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24263 2024-04-15 16:39:37.000000 libfmos-20240415/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-15 16:39:28.000000 libfmos-20240415/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-15 18:29:20.000000 libfmos-20240415/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-15 16:39:26.000000 libfmos-20240415/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23730 2024-04-15 16:39:37.000000 libfmos-20240415/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56474 2024-04-15 16:39:35.000000 libfmos-20240415/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4264 2024-04-15 16:24:35.000000 libfmos-20240415/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-04-15 18:29:22.062444 libfmos-20240415/PKG-INFO
```

### Comparing `libfmos-20240118/libfmos/libfmos_lzfse_bit_stream.h` & `libfmos-20240415/libfmos/libfmos_lzfse_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_definitions.h` & `libfmos-20240415/libfmos/libfmos_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfmos/definitions.h> are copied here
  * for local use of libfmos
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFMOS_VERSION					20240118
+#define LIBFMOS_VERSION					20240415
 
 /* The version string
  */
-#define LIBFMOS_VERSION_STRING				"20240118"
+#define LIBFMOS_VERSION_STRING				"20240415"
 
 #endif /* !defined( HAVE_LOCAL_LIBFMOS ) */
 
 #define LIBFMOS_LZFSE_NUMBER_OF_LITERAL_STATES		1024
 #define LIBFMOS_LZFSE_NUMBER_OF_LITERAL_SYMBOLS		256
 
 #define LIBFMOS_LZFSE_NUMBER_OF_L_VALUE_STATES		64
```

### Comparing `libfmos-20240118/libfmos/libfmos_lzfse_decoder.c` & `libfmos-20240415/libfmos/libfmos_lzfse_decoder.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_types.h` & `libfmos-20240415/libfmos/libfmos_types.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_adc.c` & `libfmos-20240415/libfmos/libfmos_adc.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_lzfse.h` & `libfmos-20240415/libfmos/libfmos_lzfse.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_notify.h` & `libfmos-20240415/libfmos/libfmos_notify.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos.rc.in` & `libfmos-20240415/libfmos/libfmos.rc.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_adc.h` & `libfmos-20240415/libfmos/libfmos_adc.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_definitions.h.in` & `libfmos-20240415/libfmos/libfmos_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_support.c` & `libfmos-20240415/libfmos/libfmos_support.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_error.c` & `libfmos-20240415/libfmos/libfmos_error.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/Makefile.am` & `libfmos-20240415/libfmos/Makefile.am`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFMOS_DLL_EXPORT@
 
 lib_LTLIBRARIES = libfmos.la
@@ -35,21 +35,19 @@
 libfmos_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfmos_definitions.h.in \
 	libfmos.rc \
 	libfmos.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfmos_definitions.h \
+	libfmos.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfmos_definitions.h
-	-rm -f libfmos.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmos ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmos_la_SOURCES)
```

### Comparing `libfmos-20240118/libfmos/libfmos_unused.h` & `libfmos-20240415/libfmos/libfmos_unused.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_lzvn.c` & `libfmos-20240415/libfmos/libfmos_lzvn.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_libcnotify.h` & `libfmos-20240415/libfmos/libfmos_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_lzfse_bit_stream.c` & `libfmos-20240415/libfmos/libfmos_lzfse_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_lzfse_decoder.h` & `libfmos-20240415/libfmos/libfmos_lzfse_decoder.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_libcerror.h` & `libfmos-20240415/libfmos/libfmos_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_lzfse.c` & `libfmos-20240415/libfmos/libfmos_lzfse.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_notify.c` & `libfmos-20240415/libfmos/libfmos_notify.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos.c` & `libfmos-20240415/libfmos/libfmos.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_error.h` & `libfmos-20240415/libfmos/libfmos_error.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_support.h` & `libfmos-20240415/libfmos/libfmos_support.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos.rc` & `libfmos-20240415/libfmos/libfmos.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support common Mac OS specific formats\0"
-      VALUE "FileVersion",		"20240118" "\0"
+      VALUE "FileVersion",		"20240415" "\0"
       VALUE "InternalName",		"libfmos.dll\0"
       VALUE "LegalCopyright",		"(C) 2019-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfmos.dll\0"
       VALUE "ProductName",		"libfmos\0"
-      VALUE "ProductVersion",		"20240118" "\0"
+      VALUE "ProductVersion",		"20240415" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfmos/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfmos-20240118/libfmos/libfmos_lzvn.h` & `libfmos-20240415/libfmos/libfmos_lzvn.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/libfmos_extern.h` & `libfmos-20240415/libfmos/libfmos_extern.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos/Makefile.in` & `libfmos-20240415/libfmos/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -426,16 +426,16 @@
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
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFMOS_DLL_EXPORT@
 
 lib_LTLIBRARIES = libfmos.la
@@ -464,15 +464,18 @@
 
 libfmos_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfmos_definitions.h.in \
 	libfmos.rc \
 	libfmos.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfmos_definitions.h \
+	libfmos.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -711,24 +714,35 @@
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
+		-rm -f ./$(DEPDIR)/libfmos.Plo
+	-rm -f ./$(DEPDIR)/libfmos_adc.Plo
+	-rm -f ./$(DEPDIR)/libfmos_error.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse_decoder.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzvn.Plo
+	-rm -f ./$(DEPDIR)/libfmos_notify.Plo
+	-rm -f ./$(DEPDIR)/libfmos_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -820,19 +834,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfmos_definitions.h
-	-rm -f libfmos.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmos ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmos_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfmos-20240118/COPYING` & `libfmos-20240415/COPYING`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/install-sh` & `libfmos-20240415/install-sh`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/depcomp` & `libfmos-20240415/depcomp`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos.spec.in` & `libfmos-20240415/libfmos.spec.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/tests.m4` & `libfmos-20240415/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/lib-prefix.m4` & `libfmos-20240415/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/progtest.m4` & `libfmos-20240415/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/gettext.m4` & `libfmos-20240415/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/lib-ld.m4` & `libfmos-20240415/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/common.m4` & `libfmos-20240415/m4/common.m4`

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

### Comparing `libfmos-20240118/m4/libcthreads.m4` & `libfmos-20240415/m4/libcthreads.m4`

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

### Comparing `libfmos-20240118/m4/ltversion.m4` & `libfmos-20240415/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/ltsugar.m4` & `libfmos-20240415/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/host-cpu-c-abi.m4` & `libfmos-20240415/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/libtool.m4` & `libfmos-20240415/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/po.m4` & `libfmos-20240415/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/libcerror.m4` & `libfmos-20240415/m4/libcerror.m4`

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

### Comparing `libfmos-20240118/m4/libcnotify.m4` & `libfmos-20240415/m4/libcnotify.m4`

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

### Comparing `libfmos-20240118/m4/intlmacosx.m4` & `libfmos-20240415/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/lt~obsolete.m4` & `libfmos-20240415/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/lib-link.m4` & `libfmos-20240415/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/iconv.m4` & `libfmos-20240415/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/ltoptions.m4` & `libfmos-20240415/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/nls.m4` & `libfmos-20240415/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/python.m4` & `libfmos-20240415/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/types.m4` & `libfmos-20240415/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/m4/pthread.m4` & `libfmos-20240415/m4/pthread.m4`

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

### Comparing `libfmos-20240118/include/libfmos/definitions.h.in` & `libfmos-20240415/include/libfmos/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos/definitions.h` & `libfmos-20240415/include/libfmos/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  */
 
 #if !defined( _LIBFMOS_DEFINITIONS_H )
 #define _LIBFMOS_DEFINITIONS_H
 
 #include <libfmos/types.h>
 
-#define LIBFMOS_VERSION		20240118
+#define LIBFMOS_VERSION		20240415
 
 /* The version string
  */
-#define LIBFMOS_VERSION_STRING	"20240118"
+#define LIBFMOS_VERSION_STRING	"20240415"
 
 #endif /* !defined( _LIBFMOS_DEFINITIONS_H ) */
```

### Comparing `libfmos-20240118/include/libfmos/types.h.in` & `libfmos-20240415/include/libfmos/types.h.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos/types.h` & `libfmos-20240415/include/libfmos/types.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos/features.h.in` & `libfmos-20240415/include/libfmos/features.h.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos/error.h` & `libfmos-20240415/include/libfmos/error.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos/extern.h` & `libfmos-20240415/include/libfmos/extern.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos/features.h` & `libfmos-20240415/include/libfmos/features.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos.h.in` & `libfmos-20240415/include/libfmos.h.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/libfmos.h` & `libfmos-20240415/include/libfmos.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/include/Makefile.in` & `libfmos-20240415/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -400,15 +400,20 @@
 
 EXTRA_DIST = \
 	libfmos.h.in \
 	libfmos/definitions.h.in \
 	libfmos/features.h.in \
 	libfmos/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfmos.h \
+	libfmos/definitions.h \
+	libfmos/features.h \
+	libfmos/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -605,23 +610,25 @@
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
@@ -703,17 +710,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfmos.h
-	-rm -f libfmos/definitions.h
-	-rm -f libfmos/features.h
-	-rm -f libfmos/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfmos-20240118/common/config_borlandc.h` & `libfmos-20240415/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/file_stream.h` & `libfmos-20240415/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/memory.h` & `libfmos-20240415/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/byte_stream.h` & `libfmos-20240415/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/common.h` & `libfmos-20240415/common/common.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/config_winapi.h` & `libfmos-20240415/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/system_string.h` & `libfmos-20240415/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/types.h.in` & `libfmos-20240415/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/types.h` & `libfmos-20240415/common/types.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/config.h.in` & `libfmos-20240415/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/config.h` & `libfmos-20240415/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -319,24 +319,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfmos"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfmos 20240118"
+#define PACKAGE_STRING "libfmos 20240415"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfmos"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240118"
+#define PACKAGE_VERSION "20240415"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -354,15 +354,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240118"
+#define VERSION "20240415"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfmos-20240118/common/wide_string.h` & `libfmos-20240415/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/narrow_string.h` & `libfmos-20240415/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/config_msc.h` & `libfmos-20240415/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/common/Makefile.in` & `libfmos-20240415/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -354,15 +354,17 @@
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
@@ -370,15 +372,18 @@
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
@@ -546,23 +551,25 @@
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
@@ -642,15 +649,10 @@
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

### Comparing `libfmos-20240118/config.guess` & `libfmos-20240415/config.guess`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/dpkg/copyright` & `libfmos-20240415/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/dpkg/control` & `libfmos-20240415/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/dpkg/rules` & `libfmos-20240415/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/COPYING.LESSER` & `libfmos-20240415/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/configure` & `libfmos-20240415/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfmos 20240118.
+# Generated by GNU Autoconf 2.71 for libfmos 20240415.
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
 PACKAGE_NAME='libfmos'
 PACKAGE_TARNAME='libfmos'
-PACKAGE_VERSION='20240118'
-PACKAGE_STRING='libfmos 20240118'
+PACKAGE_VERSION='20240415'
+PACKAGE_STRING='libfmos 20240415'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfmos.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1482,15 +1482,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfmos 20240118 to adapt to many kinds of systems.
+\`configure' configures libfmos 20240415 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1553,15 +1553,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfmos 20240118:";;
+     short | recursive ) echo "Configuration of libfmos 20240415:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1717,15 +1717,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfmos configure 20240118
+libfmos configure 20240415
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2438,15 +2438,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfmos $as_me 20240118, which was
+It was created by libfmos $as_me 20240415, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -3927,15 +3927,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfmos'
- VERSION='20240118'
+ VERSION='20240415'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23468,15 +23468,15 @@
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
@@ -23967,15 +23967,16 @@
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
@@ -24117,15 +24118,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24219,15 +24220,15 @@
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
@@ -25859,15 +25860,15 @@
 
 
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
@@ -25921,47 +25922,52 @@
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
@@ -25995,15 +26001,15 @@
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
@@ -26037,15 +26043,15 @@
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
@@ -26080,15 +26086,15 @@
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
@@ -26122,15 +26128,15 @@
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
@@ -26164,15 +26170,15 @@
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
@@ -26206,15 +26212,15 @@
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
@@ -26248,15 +26254,15 @@
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
@@ -26291,15 +26297,15 @@
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
@@ -26333,15 +26339,15 @@
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
@@ -26375,15 +26381,15 @@
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
@@ -26417,15 +26423,15 @@
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
@@ -26459,15 +26465,15 @@
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
@@ -26502,15 +26508,15 @@
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
@@ -26544,15 +26550,15 @@
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
@@ -26586,15 +26592,15 @@
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
@@ -26628,15 +26634,15 @@
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
@@ -26670,15 +26676,15 @@
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
@@ -26713,67 +26719,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
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
 
@@ -26861,15 +26876,15 @@
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
@@ -27319,15 +27334,16 @@
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
@@ -27382,15 +27398,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -28596,15 +28612,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfmos $as_me 20240118, which was
+This file was extended by libfmos $as_me 20240415, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -28664,15 +28680,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfmos config.status 20240118
+libfmos config.status 20240415
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfmos-20240118/pyfmos/pyfmos_python.h` & `libfmos-20240415/pyfmos/pyfmos_python.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_libfmos.h` & `libfmos-20240415/pyfmos/pyfmos_libfmos.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_unused.h` & `libfmos-20240415/pyfmos/pyfmos_unused.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_lzvn.h` & `libfmos-20240415/pyfmos/pyfmos_lzvn.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_lzfse.h` & `libfmos-20240415/pyfmos/pyfmos_lzfse.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_error.c` & `libfmos-20240415/pyfmos/pyfmos_error.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_lzvn.c` & `libfmos-20240415/pyfmos/pyfmos_lzvn.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/Makefile.am` & `libfmos-20240415/pyfmos/Makefile.am`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBFMOS_DLL_IMPORT@
 
 pyexec_LTLIBRARIES = pyfmos.la
 
 pyfmos_la_SOURCES = \
 	pyfmos.c pyfmos.h \
@@ -23,13 +23,11 @@
 	../libfmos/libfmos.la
 
 pyfmos_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfmos_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfmos-20240118/pyfmos/pyfmos_libcerror.h` & `libfmos-20240415/pyfmos/pyfmos_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_lzfse.c` & `libfmos-20240415/pyfmos/pyfmos_lzfse.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_error.h` & `libfmos-20240415/pyfmos/pyfmos_error.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_adc.h` & `libfmos-20240415/pyfmos/pyfmos_adc.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos.h` & `libfmos-20240415/pyfmos/pyfmos.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos.c` & `libfmos-20240415/pyfmos/pyfmos.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/pyfmos_adc.c` & `libfmos-20240415/pyfmos/pyfmos_adc.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/pyfmos/Makefile.in` & `libfmos-20240415/pyfmos/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -429,16 +429,16 @@
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
 @HAVE_PYTHON_TRUE@	@LIBFMOS_DLL_IMPORT@
 
 @HAVE_PYTHON_TRUE@pyexec_LTLIBRARIES = pyfmos.la
 @HAVE_PYTHON_TRUE@pyfmos_la_SOURCES = \
 @HAVE_PYTHON_TRUE@	pyfmos.c pyfmos.h \
 @HAVE_PYTHON_TRUE@	pyfmos_adc.c pyfmos_adc.h \
@@ -452,15 +452,16 @@
 
 @HAVE_PYTHON_TRUE@pyfmos_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../libfmos/libfmos.la
 
 @HAVE_PYTHON_TRUE@pyfmos_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfmos_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -726,24 +727,31 @@
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
+		-rm -f ./$(DEPDIR)/pyfmos_la-pyfmos.Plo
+	-rm -f ./$(DEPDIR)/pyfmos_la-pyfmos_adc.Plo
+	-rm -f ./$(DEPDIR)/pyfmos_la-pyfmos_error.Plo
+	-rm -f ./$(DEPDIR)/pyfmos_la-pyfmos_lzfse.Plo
+	-rm -f ./$(DEPDIR)/pyfmos_la-pyfmos_lzvn.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -832,13 +840,10 @@
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

### Comparing `libfmos-20240118/compile` & `libfmos-20240415/compile`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/missing` & `libfmos-20240415/missing`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/fmos_test_lzfse_decoder/fmos_test_lzfse_decoder.vcproj` & `libfmos-20240415/msvscpp/fmos_test_lzfse_decoder/fmos_test_lzfse_decoder.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/fmos_test_adc/fmos_test_adc.vcproj` & `libfmos-20240415/msvscpp/fmos_test_adc/fmos_test_adc.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/libfmos/libfmos.vcproj` & `libfmos-20240415/msvscpp/libfmos/libfmos.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/Makefile.am` & `libfmos-20240415/msvscpp/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -13,13 +13,11 @@
 	libfmos/libfmos.vcproj \
 	pyfmos/pyfmos.vcproj \
 	libfmos.sln
 
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

### Comparing `libfmos-20240118/msvscpp/fmos_test_notify/fmos_test_notify.vcproj` & `libfmos-20240415/msvscpp/fmos_test_notify/fmos_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/pyfmos/pyfmos.vcproj` & `libfmos-20240415/msvscpp/pyfmos/pyfmos.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/fmos_test_lzfse_bit_stream/fmos_test_lzfse_bit_stream.vcproj` & `libfmos-20240415/msvscpp/fmos_test_lzfse_bit_stream/fmos_test_lzfse_bit_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/fmos_test_lzfse/fmos_test_lzfse.vcproj` & `libfmos-20240415/msvscpp/fmos_test_lzfse/fmos_test_lzfse.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/libcthreads/libcthreads.vcproj` & `libfmos-20240415/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/fmos_test_error/fmos_test_error.vcproj` & `libfmos-20240415/msvscpp/fmos_test_error/fmos_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/fmos_test_support/fmos_test_support.vcproj` & `libfmos-20240415/msvscpp/fmos_test_support/fmos_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/libfmos.sln` & `libfmos-20240415/msvscpp/libfmos.sln`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/Makefile.in` & `libfmos-20240415/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,16 @@
 	libfmos/libfmos.vcproj \
 	pyfmos/pyfmos.vcproj \
 	libfmos.sln
 
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
@@ -467,23 +468,25 @@
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
@@ -562,13 +565,10 @@
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

### Comparing `libfmos-20240118/msvscpp/libcnotify/libcnotify.vcproj` & `libfmos-20240415/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/libcerror/libcerror.vcproj` & `libfmos-20240415/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/msvscpp/fmos_test_lzvn/fmos_test_lzvn.vcproj` & `libfmos-20240415/msvscpp/fmos_test_lzvn/fmos_test_lzvn.vcproj`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/INSTALL` & `libfmos-20240415/INSTALL`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/config.sub` & `libfmos-20240415/config.sub`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/setup.py` & `libfmos-20240415/setup.py`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/acinclude.m4` & `libfmos-20240415/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/config.rpath` & `libfmos-20240415/config.rpath`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_thread.h` & `libfmos-20240415/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_read_write_lock.h` & `libfmos-20240415/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_thread.c` & `libfmos-20240415/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_thread_pool.h` & `libfmos-20240415/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_support.h` & `libfmos-20240415/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_lock.h` & `libfmos-20240415/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_unused.h` & `libfmos-20240415/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_lock.c` & `libfmos-20240415/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_condition.h` & `libfmos-20240415/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_repeating_thread.h` & `libfmos-20240415/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/Makefile.am` & `libfmos-20240415/libcthreads/Makefile.am`

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

### Comparing `libfmos-20240118/libcthreads/libcthreads_support.c` & `libfmos-20240415/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_mutex.c` & `libfmos-20240415/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_queue.c` & `libfmos-20240415/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_mutex.h` & `libfmos-20240415/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_types.h` & `libfmos-20240415/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_thread_attributes.h` & `libfmos-20240415/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_condition.c` & `libfmos-20240415/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_error.c` & `libfmos-20240415/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_read_write_lock.c` & `libfmos-20240415/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_libcerror.h` & `libfmos-20240415/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_definitions.h` & `libfmos-20240415/libcthreads/libcthreads_definitions.h`

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

### Comparing `libfmos-20240118/libcthreads/libcthreads_thread_pool.c` & `libfmos-20240415/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_error.h` & `libfmos-20240415/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_thread_attributes.c` & `libfmos-20240415/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_extern.h` & `libfmos-20240415/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/libcthreads_repeating_thread.c` & `libfmos-20240415/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcthreads/Makefile.in` & `libfmos-20240415/libcthreads/Makefile.in`

 * *Files 9% similar despite different names*

```diff
@@ -420,16 +420,16 @@
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
@@ -444,15 +444,16 @@
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
@@ -662,24 +663,37 @@
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
 
@@ -773,17 +787,14 @@
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

### Comparing `libfmos-20240118/libcthreads/libcthreads_queue.h` & `libfmos-20240415/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/test-driver` & `libfmos-20240415/test-driver`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/manuals/libfmos.3` & `libfmos-20240415/manuals/libfmos.3`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/manuals/Makefile.in` & `libfmos-20240415/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,16 @@
 top_srcdir = @top_srcdir@
 man_MANS = \
 	libfmos.3
 
 EXTRA_DIST = \
 	libfmos.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -531,23 +532,25 @@
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
@@ -628,13 +631,10 @@
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

### Comparing `libfmos-20240118/tests/pyfmos_test_lzfse.py` & `libfmos-20240415/tests/pyfmos_test_lzfse.py`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_adc.c` & `libfmos-20240415/tests/fmos_test_adc.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_support.c` & `libfmos-20240415/tests/fmos_test_support.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_lzfse_bit_stream.c` & `libfmos-20240415/tests/fmos_test_lzfse_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_libcnotify.h` & `libfmos-20240415/tests/fmos_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_lzvn.c` & `libfmos-20240415/tests/fmos_test_lzvn.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/Makefile.am` & `libfmos-20240415/tests/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFMOS_DLL_IMPORT@
 
 TESTS = \
@@ -129,13 +129,12 @@
 	fmos_test_macros.h \
 	fmos_test_support.c \
 	fmos_test_unused.h
 
 fmos_test_support_LDADD = \
 	../libfmos/libfmos.la
 
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

### Comparing `libfmos-20240118/tests/pyfmos_test_support.py` & `libfmos-20240415/tests/pyfmos_test_support.py`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_error.c` & `libfmos-20240415/tests/fmos_test_error.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_libcerror.h` & `libfmos-20240415/tests/fmos_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/test_python_module.sh` & `libfmos-20240415/tests/test_python_module.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
+EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="adc lzfse lzvn support";
 TEST_FUNCTIONS_WITH_INPUT="";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
@@ -120,20 +121,17 @@
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
@@ -143,15 +141,19 @@
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
 
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
@@ -164,16 +166,19 @@
 	then
 		test_python_function_with_input "${TEST_FUNCTION}";
 		RESULT=$?;
 	else
 		test_python_function "${TEST_FUNCTION}";
 		RESULT=$?;
 	fi
-
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 exit ${RESULT};
```

### Comparing `libfmos-20240118/tests/fmos_test_libfmos.h` & `libfmos-20240415/tests/fmos_test_libfmos.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/pyfmos_test_lzvn.py` & `libfmos-20240415/tests/pyfmos_test_lzvn.py`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/test_runner.sh` & `libfmos-20240415/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_notify.c` & `libfmos-20240415/tests/fmos_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/pyfmos_test_adc.py` & `libfmos-20240415/tests/pyfmos_test_adc.py`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/Makefile.in` & `libfmos-20240415/tests/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -631,16 +631,16 @@
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
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ \
 	@LIBFMOS_DLL_IMPORT@
 
 TESTS = \
@@ -753,16 +753,18 @@
 	fmos_test_macros.h \
 	fmos_test_support.c \
 	fmos_test_unused.h
 
 fmos_test_support_LDADD = \
 	../libfmos/libfmos.la
 
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
@@ -1170,24 +1172,34 @@
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
+		-rm -f ./$(DEPDIR)/fmos_test_adc.Po
+	-rm -f ./$(DEPDIR)/fmos_test_error.Po
+	-rm -f ./$(DEPDIR)/fmos_test_lzfse.Po
+	-rm -f ./$(DEPDIR)/fmos_test_lzfse_bit_stream.Po
+	-rm -f ./$(DEPDIR)/fmos_test_lzfse_decoder.Po
+	-rm -f ./$(DEPDIR)/fmos_test_lzvn.Po
+	-rm -f ./$(DEPDIR)/fmos_test_notify.Po
+	-rm -f ./$(DEPDIR)/fmos_test_support.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1278,13 +1290,10 @@
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

### Comparing `libfmos-20240118/tests/fmos_test_lzfse.c` & `libfmos-20240415/tests/fmos_test_lzfse.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_unused.h` & `libfmos-20240415/tests/fmos_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_lzfse_decoder.c` & `libfmos-20240415/tests/fmos_test_lzfse_decoder.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/fmos_test_macros.h` & `libfmos-20240415/tests/fmos_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/tests/test_library.sh` & `libfmos-20240415/tests/test_library.sh`

 * *Files 2% similar despite different names*

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
 
 LIBRARY_TESTS="adc error lzfse lzfse_bit_stream lzfse_decoder lzvn notify support";
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

### Comparing `libfmos-20240118/ossfuzz/ossfuzz_libfmos.h` & `libfmos-20240415/ossfuzz/ossfuzz_libfmos.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/ossfuzz/adc_fuzzer.cc` & `libfmos-20240415/ossfuzz/adc_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/ossfuzz/Makefile.am` & `libfmos-20240415/ossfuzz/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
 	adc_fuzzer \
 	lzfse_fuzzer \
 	lzvn_fuzzer
 
 adc_fuzzer_SOURCES = \
@@ -29,20 +29,18 @@
 	ossfuzz_libfmos.h
 
 lzvn_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libfmos/libfmos.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on adc_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(adc_fuzzer_SOURCES)
 	@echo "Running splint on lzfse_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzfse_fuzzer_SOURCES)
 	@echo "Running splint on lzvn_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzvn_fuzzer_SOURCES)
```

### Comparing `libfmos-20240118/ossfuzz/lzfse_fuzzer.cc` & `libfmos-20240415/ossfuzz/lzfse_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/ossfuzz/Makefile.in` & `libfmos-20240415/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -426,16 +426,16 @@
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
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@adc_fuzzer_SOURCES = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	adc_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfmos.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@adc_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
@@ -453,15 +453,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	lzvn_fuzzer.cc \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libfmos.h
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@lzvn_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfmos/libfmos.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -713,23 +714,28 @@
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
+		-rm -f ./$(DEPDIR)/adc_fuzzer.Po
+	-rm -f ./$(DEPDIR)/lzfse_fuzzer.Po
+	-rm -f ./$(DEPDIR)/lzvn_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -815,17 +821,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on adc_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(adc_fuzzer_SOURCES)
 	@echo "Running splint on lzfse_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzfse_fuzzer_SOURCES)
 	@echo "Running splint on lzvn_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(lzvn_fuzzer_SOURCES)
```

### Comparing `libfmos-20240118/ossfuzz/lzvn_fuzzer.cc` & `libfmos-20240415/ossfuzz/lzvn_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/ltmain.sh` & `libfmos-20240415/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libfmos.spec` & `libfmos-20240415/libfmos.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfmos
-Version: 20240118
+Version: 20240415
 Release: 1
 Summary: Library to support common Mac OS specific formats
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfmos
    
@@ -76,10 +76,10 @@
 %files -n libfmos-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Thu Jan 18 2024 Joachim Metz <joachim.metz@gmail.com> 20240118-1
+* Mon Apr 15 2024 Joachim Metz <joachim.metz@gmail.com> 20240415-1
 - Auto-generated
```

### Comparing `libfmos-20240118/po/remove-potcdate.sin` & `libfmos-20240415/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/po/Makefile.in.in` & `libfmos-20240415/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/po/en@quot.header` & `libfmos-20240415/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/po/en@boldquot.header` & `libfmos-20240415/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/po/insert-header.sin` & `libfmos-20240415/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/po/Makevars` & `libfmos-20240415/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/po/Makevars.in` & `libfmos-20240415/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/po/Rules-quot` & `libfmos-20240415/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/Makefile.in` & `libfmos-20240415/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -506,16 +506,23 @@
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
+	libfmos.pc \
+	libfmos.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfmos.pc
 
 all: all-recursive
 
@@ -932,23 +939,26 @@
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
 
@@ -1048,22 +1058,10 @@
 	(cd $(srcdir)/common && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcerror && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcthreads && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcnotify && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfmos && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfmos.pc
-	-rm -f libfmos.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfmos-20240118/libcnotify/libcnotify_definitions.h` & `libfmos-20240415/libcnotify/libcnotify_definitions.h`

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

### Comparing `libfmos-20240118/libcnotify/libcnotify_extern.h` & `libfmos-20240415/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_support.c` & `libfmos-20240415/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_stream.h` & `libfmos-20240415/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/Makefile.am` & `libfmos-20240415/libcnotify/Makefile.am`

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

### Comparing `libfmos-20240118/libcnotify/libcnotify_unused.h` & `libfmos-20240415/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_verbose.h` & `libfmos-20240415/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_print.h` & `libfmos-20240415/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_stream.c` & `libfmos-20240415/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_support.h` & `libfmos-20240415/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_verbose.c` & `libfmos-20240415/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/Makefile.in` & `libfmos-20240415/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -398,30 +398,31 @@
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
@@ -624,24 +625,30 @@
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
 
@@ -728,17 +735,14 @@
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

### Comparing `libfmos-20240118/libcnotify/libcnotify_libcerror.h` & `libfmos-20240415/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcnotify/libcnotify_print.c` & `libfmos-20240415/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_system.c` & `libfmos-20240415/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_error.c` & `libfmos-20240415/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_extern.h` & `libfmos-20240415/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/Makefile.am` & `libfmos-20240415/libcerror/Makefile.am`

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

### Comparing `libfmos-20240118/libcerror/libcerror_types.h` & `libfmos-20240415/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_support.h` & `libfmos-20240415/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_error.h` & `libfmos-20240415/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_system.h` & `libfmos-20240415/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_definitions.h` & `libfmos-20240415/libcerror/libcerror_definitions.h`

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

### Comparing `libfmos-20240118/libcerror/libcerror_support.c` & `libfmos-20240415/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/libcerror_unused.h` & `libfmos-20240415/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/libcerror/Makefile.in` & `libfmos-20240415/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -395,28 +395,29 @@
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
@@ -618,24 +619,29 @@
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
 
@@ -721,17 +727,14 @@
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

### Comparing `libfmos-20240118/aclocal.m4` & `libfmos-20240415/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfmos-20240118/configure.ac` & `libfmos-20240415/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfmos],
- [20240118],
+ [20240415],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfmos.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

