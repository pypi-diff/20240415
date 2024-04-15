# Comparing `tmp/pdfminer_rtl-0.0.2.dev3.tar.gz` & `tmp/pdfminer_rtl-0.0.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfminer_rtl-0.0.2.dev3.tar", last modified: Mon Apr 15 13:52:30 2024, max compression
+gzip compressed data, was "pdfminer_rtl-0.0.2.dev5.tar", last modified: Mon Apr 15 13:58:43 2024, max compression
```

## Comparing `pdfminer_rtl-0.0.2.dev3.tar` & `pdfminer_rtl-0.0.2.dev5.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.291328 pdfminer_rtl-0.0.2.dev3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16518 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/CHANGELOG.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2662 2024-04-15 13:22:04.000000 pdfminer_rtl-0.0.2.dev3/CONTRIBUTING.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1093 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      160 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1141 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/Makefile
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 13:52:30.291328 pdfminer_rtl-0.0.2.dev3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1766 2024-04-15 13:34:22.000000 pdfminer_rtl-0.0.2.dev3/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.151328 pdfminer_rtl-0.0.2.dev3/cmaprsrc/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/README.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2046762 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_CNS1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1900416 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_GB1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2681742 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Japan1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1028252 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Korea1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1310 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/noxfile.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.167328 pdfminer_rtl-0.0.2.dev3/pdfminer/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      260 2024-04-15 13:20:38.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3600 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/_saslprep.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      929 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/arcfour.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2097 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/ascii85.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/ccitt.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.263328 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20551 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19882 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22969 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19883 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25942 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25964 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25732 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25757 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25670 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25688 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24226 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24021 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21027 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24275 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24079 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20874 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42594 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42549 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42602 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42557 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56943 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17615 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17564 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59548 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59481 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43982 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43924 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      320 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETenms-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      438 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETenms-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20429 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20455 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22272 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25721 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25750 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22307 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22118 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22111 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68254 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68199 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89872 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68148 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68102 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23815 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23806 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23339 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23322 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23650 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23647 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21945 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21956 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19781 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45212 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45167 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44853 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44816 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53104 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53050 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43618 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44187 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44144 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59508 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59473 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      840 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      839 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hiragana-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hiragana-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24040 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24078 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23563 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55016 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55041 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23644 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51788 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51698 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27769 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27820 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Katakana-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Katakana-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21708 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/README.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23030 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23048 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Roman-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Roman-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67395 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87819 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87751 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87400 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87327 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82631 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82562 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97445 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97441 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101331 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101490 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101357 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90500 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90368 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      412 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1402 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35852 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58054 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57928 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57910 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57780 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54764 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54684 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58081 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57960 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57940 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57811 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54829 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54749 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57903 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57778 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57930 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57808 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60683 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61278 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61298 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61286 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61309 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54151 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54172 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19826 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/WP-Symbol-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/WP-Symbol-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138237 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   204425 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112987 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   120859 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16052 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmapdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/converter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/data_structures.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3983 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/encodingdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112611 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/fontmetrics.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   130804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/glyphlist.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7276 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/high_level.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9165 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/image.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/jbig2.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8531 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/latin_enc.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38624 2024-04-15 12:59:08.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3177 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/lzw.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfcolor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8787 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdevice.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37267 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdocument.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37946 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdffont.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34539 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfinterp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6932 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfpage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5896 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11965 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdftypes.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)    19890 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/psparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/py.typed
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1358 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/runlength.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/settings.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.287328 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6909 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      206 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-15 13:52:30.291328 pdfminer_rtl-0.0.2.dev3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2104 2024-04-15 13:49:59.000000 pdfminer_rtl-0.0.2.dev3/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.271328 pdfminer_rtl-0.0.2.dev3/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9692 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_converter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5420 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_encodingdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_font_size.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_highlevel_extracttext.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5038 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1809 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfdocument.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3972 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfencoding.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      604 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdffont.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_ccitt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_crypto.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3730 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_psparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      582 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfpage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_tools_dumppdf.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5766 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_tools_pdf2txt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3912 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.283328 pdfminer_rtl-0.0.2.dev3/tools/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/__init__.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     1646 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/conv_afm.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     6089 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/conv_cmap.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)      911 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/conv_glyphlist.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)    14316 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/dumppdf.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     9779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/pdf2txt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6266 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/pdfdiff.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     2761 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/pdfstats.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1415 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/prof.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:58:43.135323 pdfminer_rtl-0.0.2.dev5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16518 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/CHANGELOG.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2662 2024-04-15 13:22:04.000000 pdfminer_rtl-0.0.2.dev5/CONTRIBUTING.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1093 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      160 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1141 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/Makefile
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 13:58:43.135323 pdfminer_rtl-0.0.2.dev5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1766 2024-04-15 13:34:22.000000 pdfminer_rtl-0.0.2.dev5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:58:43.051323 pdfminer_rtl-0.0.2.dev5/cmaprsrc/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/cmaprsrc/README.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2046762 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_CNS1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1900416 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_GB1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2681742 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_Japan1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1028252 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_Korea1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1310 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/noxfile.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:58:43.063323 pdfminer_rtl-0.0.2.dev5/pdfminer/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      260 2024-04-15 13:20:38.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3600 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/_saslprep.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      929 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/arcfour.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2097 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/ascii85.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/ccitt.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:58:43.127323 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20551 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19882 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22969 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19883 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25942 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25964 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25732 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25757 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25670 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25688 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24226 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24021 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21027 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24275 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24079 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20874 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42594 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42549 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42602 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5pc-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42557 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5pc-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56943 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17615 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS1-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17564 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS1-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59548 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETHK-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59481 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETHK-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43982 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETen-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43924 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETen-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      320 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETenms-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      438 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETenms-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20429 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20455 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22272 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25721 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25750 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22307 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22118 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22111 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68254 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68199 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK2K-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89872 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK2K-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68148 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBKp-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68102 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBKp-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23815 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23806 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23339 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23322 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23650 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23647 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21945 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBpc-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21956 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBpc-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19781 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45212 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdla-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45167 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdla-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44853 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdlb-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44816 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdlb-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53104 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKgccs-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53050 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKgccs-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm314-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43618 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm314-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44187 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm471-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44144 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm471-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59508 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKscs-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59473 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKscs-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      840 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Hankaku-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      839 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Hankaku-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Hiragana-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Hiragana-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24040 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24078 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23563 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55016 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-Johab-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55041 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-Johab-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23644 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51788 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51698 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27769 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27820 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Katakana-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Katakana-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21708 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/NWP-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/NWP-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/README.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23030 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23048 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Roman-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Roman-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67395 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87819 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87751 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87400 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87327 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82631 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82562 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97445 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97441 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101331 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101490 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101357 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90500 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90368 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      412 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1402 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35852 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58054 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57928 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57910 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57780 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54764 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54684 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58081 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57960 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57940 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57811 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54829 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54749 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57903 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57778 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57930 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57808 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60683 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61278 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61298 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61286 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61309 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54151 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54172 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19826 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/WP-Symbol-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/WP-Symbol-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138237 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   204425 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112987 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   120859 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16052 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/cmapdb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/converter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/data_structures.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3983 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/encodingdb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112611 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/fontmetrics.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   130804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/glyphlist.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7276 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/high_level.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9165 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/image.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/jbig2.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8531 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/latin_enc.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38629 2024-04-15 13:57:59.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/layout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3177 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/lzw.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdfcolor.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8787 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdfdevice.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37267 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdfdocument.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37946 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdffont.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34539 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdfinterp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6932 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdfpage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5896 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdfparser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11965 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/pdftypes.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)    19890 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/psparser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/py.typed
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1358 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/runlength.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/settings.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/pdfminer/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:58:43.135323 pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 13:58:42.000000 pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6909 2024-04-15 13:58:42.000000 pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-15 13:58:42.000000 pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      206 2024-04-15 13:58:42.000000 pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2024-04-15 13:58:42.000000 pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-15 13:58:43.135323 pdfminer_rtl-0.0.2.dev5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2104 2024-04-15 13:49:59.000000 pdfminer_rtl-0.0.2.dev5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:58:43.131322 pdfminer_rtl-0.0.2.dev5/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9692 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_converter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5420 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_encodingdb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_font_size.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_highlevel_extracttext.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5038 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_layout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1809 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_pdfdocument.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3972 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_pdfencoding.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      604 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_pdffont.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_pdfminer_ccitt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_pdfminer_crypto.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3730 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_pdfminer_psparser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      582 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_pdfpage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_tools_dumppdf.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5766 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_tools_pdf2txt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3912 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tests/test_utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:58:43.135323 pdfminer_rtl-0.0.2.dev5/tools/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/__init__.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     1646 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/conv_afm.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     6089 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/conv_cmap.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      911 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/conv_glyphlist.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)    14316 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/dumppdf.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     9779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/pdf2txt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6266 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/pdfdiff.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     2761 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/pdfstats.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1415 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev5/tools/prof.py
```

### Comparing `pdfminer_rtl-0.0.2.dev3/CHANGELOG.md` & `pdfminer_rtl-0.0.2.dev5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/CONTRIBUTING.md` & `pdfminer_rtl-0.0.2.dev5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/LICENSE` & `pdfminer_rtl-0.0.2.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/Makefile` & `pdfminer_rtl-0.0.2.dev5/Makefile`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/PKG-INFO` & `pdfminer_rtl-0.0.2.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.rtl
-Version: 0.0.2.dev3
+Version: 0.0.2.dev5
 Summary: PDF parser and analyzer
 Home-page: https://github.com/taneron/pdfminerrtl
 Author: Yusuke Shinyama + Philippe Guglielmetti + Taner
 Author-email: pdfminerrtl@rust.8shield.net
 License: MIT
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
```

### Comparing `pdfminer_rtl-0.0.2.dev3/README.md` & `pdfminer_rtl-0.0.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/cmaprsrc/README.txt` & `pdfminer_rtl-0.0.2.dev5/cmaprsrc/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_CNS1.txt` & `pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_CNS1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_GB1.txt` & `pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_GB1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Japan1.txt` & `pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_Japan1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Korea1.txt` & `pdfminer_rtl-0.0.2.dev5/cmaprsrc/cid2code_Adobe_Korea1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/noxfile.py` & `pdfminer_rtl-0.0.2.dev5/noxfile.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/_saslprep.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/_saslprep.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/arcfour.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/arcfour.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/ascii85.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/ascii85.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/ccitt.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/78ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/83pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/83pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90msp-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90msp-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/90pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Add-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5pc-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/B5pc-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS1-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS1-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/CNS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETHK-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETHK-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETen-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/ETen-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Ext-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GB-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK2K-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBK2K-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBKp-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBKp-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBT-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBTpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBTpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/GBpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdla-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdla-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdlb-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKdlb-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKgccs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKgccs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm314-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm314-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm471-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKm471-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKscs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/HKscs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Hankaku-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/Hankaku-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-Johab-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-Johab-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCms-UHC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/KSCpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/NWP-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/NWP-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/README.txt` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniGB-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/UniKS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/V.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/cmapdb.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/cmapdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/converter.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/data_structures.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/data_structures.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/encodingdb.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/fontmetrics.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/glyphlist.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/high_level.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/high_level.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/image.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/image.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/jbig2.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/jbig2.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/latin_enc.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/latin_enc.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/layout.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,15 @@
         BA.resolve_implicit_levels(storage, False)
         BA.reorder_resolved_levels(storage, False)
         self.apply_mirroring(storage)
         self._objs = [_ch['ch'] for _ch in storage['chars']]
         return
     
     # for fixing the bidi assertion in resolve_implicit_levels() bug https://github.com/alihoseiny/word_cloud_fa/issues/3
-    def removeWeirdChars(text):
+    def removeWeirdChars(self,text):
         weridPatterns = re.compile("["
                                u"\U0001F600-\U0001F64F"  # emoticons
                                u"\U0001F300-\U0001F5FF"  # symbols & pictographs
                                u"\U0001F680-\U0001F6FF"  # transport & map symbols
                                u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
                                u"\U00002702-\U000027B0"
                                u"\U000024C2-\U0001F251"
```

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/lzw.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/lzw.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfcolor.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdfcolor.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdevice.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdfdevice.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdocument.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdffont.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfinterp.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdfinterp.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfpage.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfparser.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdfparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/pdftypes.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/pdftypes.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/psparser.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/runlength.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/runlength.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer/utils.py` & `pdfminer_rtl-0.0.2.dev5/pdfminer/utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/PKG-INFO` & `pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.rtl
-Version: 0.0.2.dev3
+Version: 0.0.2.dev5
 Summary: PDF parser and analyzer
 Home-page: https://github.com/taneron/pdfminerrtl
 Author: Yusuke Shinyama + Philippe Guglielmetti + Taner
 Author-email: pdfminerrtl@rust.8shield.net
 License: MIT
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
```

### Comparing `pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/SOURCES.txt` & `pdfminer_rtl-0.0.2.dev5/pdfminer.rtl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/setup.py` & `pdfminer_rtl-0.0.2.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_converter.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_encodingdb.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_font_size.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_font_size.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_highlevel_extracttext.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_highlevel_extracttext.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_layout.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_pdfdocument.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_pdfencoding.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_pdfencoding.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_pdffont.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_ccitt.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_pdfminer_ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_crypto.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_pdfminer_crypto.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_psparser.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_pdfminer_psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_pdfpage.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_tools_dumppdf.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_tools_dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_tools_pdf2txt.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_tools_pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tests/test_utils.py` & `pdfminer_rtl-0.0.2.dev5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/conv_afm.py` & `pdfminer_rtl-0.0.2.dev5/tools/conv_afm.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/conv_cmap.py` & `pdfminer_rtl-0.0.2.dev5/tools/conv_cmap.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/conv_glyphlist.py` & `pdfminer_rtl-0.0.2.dev5/tools/conv_glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/dumppdf.py` & `pdfminer_rtl-0.0.2.dev5/tools/dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/pdf2txt.py` & `pdfminer_rtl-0.0.2.dev5/tools/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/pdfdiff.py` & `pdfminer_rtl-0.0.2.dev5/tools/pdfdiff.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/pdfstats.py` & `pdfminer_rtl-0.0.2.dev5/tools/pdfstats.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.2.dev3/tools/prof.py` & `pdfminer_rtl-0.0.2.dev5/tools/prof.py`

 * *Files identical despite different names*

