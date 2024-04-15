# Comparing `tmp/pdfminer_rtl-0.0.1.tar.gz` & `tmp/pdfminer_rtl-0.0.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfminer_rtl-0.0.1.tar", last modified: Mon Apr 15 11:27:54 2024, max compression
+gzip compressed data, was "pdfminer_rtl-0.0.2.dev3.tar", last modified: Mon Apr 15 13:52:30 2024, max compression
```

## Comparing `pdfminer_rtl-0.0.1.tar` & `pdfminer_rtl-0.0.2.dev3.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 11:27:54.822143 pdfminer_rtl-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16518 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/CHANGELOG.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2662 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/CONTRIBUTING.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1093 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      160 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1141 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/Makefile
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4142 2024-04-15 11:27:54.822143 pdfminer_rtl-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2573 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 11:27:54.702143 pdfminer_rtl-0.0.1/cmaprsrc/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/cmaprsrc/README.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2046762 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_CNS1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1900416 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_GB1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2681742 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_Japan1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1028252 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_Korea1.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1310 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/noxfile.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 11:27:54.718143 pdfminer_rtl-0.0.1/pdfminer/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      260 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3600 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/_saslprep.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      929 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/arcfour.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2097 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/ascii85.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/ccitt.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 11:27:54.806143 pdfminer_rtl-0.0.1/pdfminer/cmap/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20551 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19882 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22969 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19883 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25942 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25964 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25732 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25757 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25670 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25688 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24226 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24021 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21027 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Add-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24275 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Add-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24079 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Add-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20874 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Add-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42594 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42549 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42602 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/B5pc-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42557 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/B5pc-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/CNS-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56943 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/CNS-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17615 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/CNS1-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17564 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/CNS1-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/CNS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/CNS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59548 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/ETHK-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59481 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/ETHK-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43982 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/ETen-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43924 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/ETen-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      320 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/ETenms-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      438 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/ETenms-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20429 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20455 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22272 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25721 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25750 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22307 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22118 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GB-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22111 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GB-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GB-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GB-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68254 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBK-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68199 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBK-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBK2K-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89872 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBK2K-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68148 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBKp-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68102 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBKp-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23815 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23806 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23339 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23322 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23650 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23647 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21945 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21956 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/GBpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19781 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45212 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKdla-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45167 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKdla-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44853 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKdlb-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44816 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKdlb-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53104 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKgccs-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53050 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKgccs-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKm314-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43618 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKm314-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44187 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKm471-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44144 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKm471-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59508 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKscs-B5-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59473 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/HKscs-B5-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      840 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Hankaku-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      839 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Hankaku-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Hiragana-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Hiragana-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24040 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24078 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23563 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55016 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-Johab-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55041 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-Johab-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23644 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51788 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51698 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27769 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27820 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Katakana-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Katakana-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21708 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/NWP-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/NWP-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/README.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23030 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/RKSJ-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23048 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/RKSJ-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Roman-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/Roman-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67395 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87819 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87751 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87400 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87327 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82631 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82562 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97445 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97441 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101331 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101490 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101357 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90500 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90368 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      412 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1402 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35852 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58054 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57928 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57910 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57780 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54764 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54684 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58081 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57960 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57940 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57811 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54829 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54749 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57903 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57778 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57930 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57808 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60683 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61278 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61298 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61286 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61309 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54151 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54172 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19826 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/WP-Symbol-H.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/WP-Symbol-V.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138237 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   204425 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112987 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   120859 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16052 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/cmapdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/converter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/data_structures.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3983 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/encodingdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112611 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/fontmetrics.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   130804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/glyphlist.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7276 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/high_level.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9165 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/image.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/jbig2.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8531 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/latin_enc.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37163 2024-04-15 09:41:02.000000 pdfminer_rtl-0.0.1/pdfminer/layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3177 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/lzw.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdfcolor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8787 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdfdevice.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37267 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdfdocument.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37946 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdffont.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34539 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdfinterp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6932 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdfpage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5896 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdfparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11965 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/pdftypes.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)    19890 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/psparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/py.typed
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1358 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/runlength.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/settings.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/pdfminer/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 11:27:54.814143 pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4142 2024-04-15 11:27:54.000000 pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6909 2024-04-15 11:27:54.000000 pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-15 11:27:54.000000 pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      206 2024-04-15 11:27:54.000000 pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2024-04-15 11:27:54.000000 pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-15 11:27:54.822143 pdfminer_rtl-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1943 2024-04-15 11:26:42.000000 pdfminer_rtl-0.0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 11:27:54.810143 pdfminer_rtl-0.0.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9692 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_converter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5420 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_encodingdb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_font_size.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_highlevel_extracttext.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5038 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_layout.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1809 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_pdfdocument.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3972 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_pdfencoding.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      604 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_pdffont.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_pdfminer_ccitt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_pdfminer_crypto.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3730 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_pdfminer_psparser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      582 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_pdfpage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_tools_dumppdf.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5766 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_tools_pdf2txt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3912 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tests/test_utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 11:27:54.814143 pdfminer_rtl-0.0.1/tools/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/__init__.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     1646 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/conv_afm.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     6089 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/conv_cmap.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)      911 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/conv_glyphlist.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)    14316 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/dumppdf.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     9779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/pdf2txt.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6266 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/pdfdiff.py
--rwxrwxrwx   0 codespace  (1000) codespace  (1000)     2761 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/pdfstats.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1415 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.1/tools/prof.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.291328 pdfminer_rtl-0.0.2.dev3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16518 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/CHANGELOG.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2662 2024-04-15 13:22:04.000000 pdfminer_rtl-0.0.2.dev3/CONTRIBUTING.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1093 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      160 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1141 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/Makefile
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 13:52:30.291328 pdfminer_rtl-0.0.2.dev3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1766 2024-04-15 13:34:22.000000 pdfminer_rtl-0.0.2.dev3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.151328 pdfminer_rtl-0.0.2.dev3/cmaprsrc/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/README.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2046762 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_CNS1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1900416 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_GB1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  2681742 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Japan1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)  1028252 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Korea1.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1310 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/noxfile.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.167328 pdfminer_rtl-0.0.2.dev3/pdfminer/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      260 2024-04-15 13:20:38.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3600 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/_saslprep.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      929 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/arcfour.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2097 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/ascii85.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/ccitt.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.263328 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20551 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19882 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22969 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19883 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25942 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25964 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26305 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25732 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25757 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25670 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25688 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24226 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24021 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21027 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24275 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24079 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20874 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42594 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42549 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42602 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    42557 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56990 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    56943 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17615 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17564 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21723 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59548 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59481 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43982 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43924 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      320 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETenms-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      438 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETenms-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20429 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20455 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22272 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25721 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25750 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22307 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22118 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    22111 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68254 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68199 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    89872 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68148 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    68102 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23815 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23806 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23339 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23322 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23650 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23647 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21945 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21956 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19781 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45212 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    45167 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44853 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44816 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53104 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    53050 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    43618 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44187 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    44144 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59508 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59473 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      840 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      839 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hiragana-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hiragana-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24040 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    24078 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23563 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55016 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    55041 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23644 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51667 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51788 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    51698 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27769 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27820 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Katakana-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      404 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Katakana-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21708 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3917 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/README.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23030 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    23048 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Roman-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      394 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Roman-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    67395 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87819 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87751 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87400 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    87327 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82631 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    82562 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97445 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    97441 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101459 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101331 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101490 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   101357 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90500 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    90368 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      412 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1402 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35852 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58054 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57928 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57910 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57780 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54764 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54684 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    58081 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57960 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57940 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57811 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54829 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54749 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57903 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57778 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57930 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    57808 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60683 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    60699 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61278 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61298 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61286 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    61309 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54151 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    54172 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19826 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/WP-Symbol-H.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/WP-Symbol-V.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   138237 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   204425 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112987 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   120859 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16052 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/cmapdb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35934 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/converter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1654 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/data_structures.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3983 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/encodingdb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   112611 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/fontmetrics.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   130804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/glyphlist.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7276 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/high_level.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9165 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/image.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11391 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/jbig2.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8531 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/latin_enc.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    38624 2024-04-15 12:59:08.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/layout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3177 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/lzw.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      821 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfcolor.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8787 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdevice.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37267 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdocument.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    37946 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdffont.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34539 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfinterp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6932 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfpage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5896 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdfparser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11965 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/pdftypes.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)    19890 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/psparser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/py.typed
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1358 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/runlength.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/settings.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20804 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/pdfminer/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.287328 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     3358 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6909 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      206 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2024-04-15 13:52:30.000000 pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-15 13:52:30.291328 pdfminer_rtl-0.0.2.dev3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2104 2024-04-15 13:49:59.000000 pdfminer_rtl-0.0.2.dev3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.271328 pdfminer_rtl-0.0.2.dev3/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9692 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_converter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5420 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_encodingdb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_font_size.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7694 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_highlevel_extracttext.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5038 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_layout.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1809 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfdocument.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3972 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfencoding.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      604 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdffont.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4532 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_ccitt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_crypto.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3730 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_psparser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      582 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_pdfpage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1505 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_tools_dumppdf.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5766 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_tools_pdf2txt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3912 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tests/test_utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-15 13:52:30.283328 pdfminer_rtl-0.0.2.dev3/tools/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/__init__.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     1646 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/conv_afm.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     6089 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/conv_cmap.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      911 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/conv_glyphlist.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)    14316 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/dumppdf.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     9779 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/pdf2txt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6266 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/pdfdiff.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     2761 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/pdfstats.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1415 2024-04-15 09:29:26.000000 pdfminer_rtl-0.0.2.dev3/tools/prof.py
```

### Comparing `pdfminer_rtl-0.0.1/CHANGELOG.md` & `pdfminer_rtl-0.0.2.dev3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/CONTRIBUTING.md` & `pdfminer_rtl-0.0.2.dev3/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 * Use [licensecheck](https://pypi.org/project/licensecheck/) to validate if new packages are compatible.
 
 ## Getting started
 
 1. Clone the repository
 
     ```sh
-    git clone https://github.com/pdfminer/pdfminer.six
-    cd pdfminer.six
+    git clone https://github.com/pdfminer/pdfminer.rtl
+    cd pdfminer.rtl
     ```
 
 2. Install dev dependencies
 
     ```sh
     pip install -e .[dev]
     ```
```

### Comparing `pdfminer_rtl-0.0.1/LICENSE` & `pdfminer_rtl-0.0.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/Makefile` & `pdfminer_rtl-0.0.2.dev3/Makefile`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/PKG-INFO` & `pdfminer_rtl-0.0.2.dev3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pdfminer.rtl
-Version: 0.0.1
+Version: 0.0.2.dev3
 Summary: PDF parser and analyzer
 Home-page: https://github.com/taneron/pdfminerrtl
-Author: Yusuke Shinyama + Philippe Guglielmetti
-Author-email: pdfminer@goulu.net
+Author: Yusuke Shinyama + Philippe Guglielmetti + Taner
+Author-email: pdfminerrtl@rust.8shield.net
 License: MIT
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,37 +35,28 @@
 Requires-Dist: mypy==0.931; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Provides-Extra: image
 Requires-Dist: Pillow; extra == "image"
 
-pdfminer.six
+pdfminer.rtl
 ============
 
-[![Continuous integration](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml/badge.svg)](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml)
-[![PyPI version](https://img.shields.io/pypi/v/pdfminer.six.svg)](https://pypi.python.org/pypi/pdfminer.six/)
-[![gitter](https://badges.gitter.im/pdfminer-six/Lobby.svg)](https://gitter.im/pdfminer-six/Lobby?utm_source=badge&utm_medium)
 
-*We fathom PDF*
+This is a fork of pdfminer.six that attempts to add RTL support with python-bidi. This version is experimental and probably buggy. Please don't rely on it for critical projects.
 
-Pdfminer.six is a community maintained fork of the original PDFMiner. It is a tool for extracting information from PDF
-documents. It focuses on getting and analyzing text data. Pdfminer.six extracts the text from a page directly from the
-sourcecode of the PDF. It can also be used to get the exact location, font or color of the text.
-
-It is built in a modular way such that each component of pdfminer.six can be replaced easily. You can implement your own
-interpreter or rendering device that uses the power of pdfminer.six for other purposes than text analysis.
-
-Check out the full documentation on
+Check out the full original documentation on
 [Read the Docs](https://pdfminersix.readthedocs.io).
 
 
 Features
 --------
 
+* (Added RTL support)
 * Written entirely in Python.
 * Parse, analyze, and convert PDF documents.
 * Extract content as text, images, html or [hOCR](https://en.wikipedia.org/wiki/HOCR).
 * PDF-1.7 specification support. (well, almost).
 * CJK languages and vertical writing scripts support.
 * Various font types (Type1, TrueType, Type3, and CID) support.
 * Support for extracting images (JPG, JBIG2, Bitmaps).
@@ -77,37 +68,32 @@
 * Tagged contents extraction.
 * Automatic layout analysis.
 
 How to use
 ----------
 
 * Install Python 3.8 or newer.
-* Install pdfminer.six.
+* Install pdfminer.rtl.
 
-  `pip install pdfminer.six`
+  `pip install pdfminer.rtl`
 
 * (Optionally) install extra dependencies for extracting images.
 
-  `pip install 'pdfminer.six[image]'`
+  `pip install 'pdfminer.rtl[image]'`
 
 * Use the command-line interface to extract text from pdf.
 
   `pdf2txt.py example.pdf`
 
 * Or use it with Python. 
 
 ```python
 from pdfminer.high_level import extract_text
 
 text = extract_text("example.pdf")
 print(text)
 ```
 
-Contributing
-------------
-
-Be sure to read the [contribution guidelines](https://github.com/pdfminer/pdfminer.six/blob/master/CONTRIBUTING.md). 
-
 Acknowledgement
 ---------------
 
-This repository includes code from `pyHanko` ; the original license has been included [here](/docs/licenses/LICENSE.pyHanko).
+This repository includes code from `pyHanko` ; the original license has been included [here](/docs/licenses/LICENSE.pyHanko) and to all the other contirbutors of the original project see [here](https://github.com/pdfminer/pdfminer.six/graphs/contributors)
```

### Comparing `pdfminer_rtl-0.0.1/README.md` & `pdfminer_rtl-0.0.2.dev3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-pdfminer.six
+pdfminer.rtl
 ============
 
-[![Continuous integration](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml/badge.svg)](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml)
-[![PyPI version](https://img.shields.io/pypi/v/pdfminer.six.svg)](https://pypi.python.org/pypi/pdfminer.six/)
-[![gitter](https://badges.gitter.im/pdfminer-six/Lobby.svg)](https://gitter.im/pdfminer-six/Lobby?utm_source=badge&utm_medium)
 
-*We fathom PDF*
+This is a fork of pdfminer.six that attempts to add RTL support with python-bidi. This version is experimental and probably buggy. Please don't rely on it for critical projects.
 
-Pdfminer.six is a community maintained fork of the original PDFMiner. It is a tool for extracting information from PDF
-documents. It focuses on getting and analyzing text data. Pdfminer.six extracts the text from a page directly from the
-sourcecode of the PDF. It can also be used to get the exact location, font or color of the text.
-
-It is built in a modular way such that each component of pdfminer.six can be replaced easily. You can implement your own
-interpreter or rendering device that uses the power of pdfminer.six for other purposes than text analysis.
-
-Check out the full documentation on
+Check out the full original documentation on
 [Read the Docs](https://pdfminersix.readthedocs.io).
 
 
 Features
 --------
 
+* (Added RTL support)
 * Written entirely in Python.
 * Parse, analyze, and convert PDF documents.
 * Extract content as text, images, html or [hOCR](https://en.wikipedia.org/wiki/HOCR).
 * PDF-1.7 specification support. (well, almost).
 * CJK languages and vertical writing scripts support.
 * Various font types (Type1, TrueType, Type3, and CID) support.
 * Support for extracting images (JPG, JBIG2, Bitmaps).
@@ -36,37 +27,32 @@
 * Tagged contents extraction.
 * Automatic layout analysis.
 
 How to use
 ----------
 
 * Install Python 3.8 or newer.
-* Install pdfminer.six.
+* Install pdfminer.rtl.
 
-  `pip install pdfminer.six`
+  `pip install pdfminer.rtl`
 
 * (Optionally) install extra dependencies for extracting images.
 
-  `pip install 'pdfminer.six[image]'`
+  `pip install 'pdfminer.rtl[image]'`
 
 * Use the command-line interface to extract text from pdf.
 
   `pdf2txt.py example.pdf`
 
 * Or use it with Python. 
 
 ```python
 from pdfminer.high_level import extract_text
 
 text = extract_text("example.pdf")
 print(text)
 ```
 
-Contributing
-------------
-
-Be sure to read the [contribution guidelines](https://github.com/pdfminer/pdfminer.six/blob/master/CONTRIBUTING.md). 
-
 Acknowledgement
 ---------------
 
-This repository includes code from `pyHanko` ; the original license has been included [here](/docs/licenses/LICENSE.pyHanko).
+This repository includes code from `pyHanko` ; the original license has been included [here](/docs/licenses/LICENSE.pyHanko) and to all the other contirbutors of the original project see [here](https://github.com/pdfminer/pdfminer.six/graphs/contributors)
```

### Comparing `pdfminer_rtl-0.0.1/cmaprsrc/README.txt` & `pdfminer_rtl-0.0.2.dev3/cmaprsrc/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_CNS1.txt` & `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_CNS1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_GB1.txt` & `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_GB1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_Japan1.txt` & `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Japan1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/cmaprsrc/cid2code_Adobe_Korea1.txt` & `pdfminer_rtl-0.0.2.dev3/cmaprsrc/cid2code_Adobe_Korea1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/noxfile.py` & `pdfminer_rtl-0.0.2.dev3/noxfile.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/_saslprep.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/_saslprep.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/arcfour.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/arcfour.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/ascii85.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/ascii85.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/ccitt.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78ms-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/78ms-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/78ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/83pv-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/83pv-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/83pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/90ms-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/90ms-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/90msp-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/90msp-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90msp-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/90pv-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/90pv-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/90pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Add-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Add-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Add-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Add-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Add-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/B5pc-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/B5pc-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/B5pc-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/CNS-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/CNS-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/CNS1-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/CNS1-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS1-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/CNS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/CNS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/CNS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/ETHK-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/ETHK-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETHK-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/ETen-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/ETen-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/ETen-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Ext-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Ext-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GB-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GB-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GB-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GB-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GB-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBK-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBK-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBK2K-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBK2K-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBK2K-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBKp-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBKp-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBKp-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBT-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBT-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBTpc-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBTpc-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBTpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBpc-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/GBpc-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/GBpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKdla-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKdla-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdla-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKdlb-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKdlb-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKdlb-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKgccs-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKgccs-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKgccs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKm314-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKm314-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm314-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKm471-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKm471-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKm471-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKscs-B5-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/HKscs-B5-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/HKscs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Hankaku-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/Hankaku-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/Hankaku-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-Johab-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-Johab-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-Johab-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSCms-UHC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCms-UHC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSCpc-EUC-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/KSCpc-EUC-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/KSCpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/NWP-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/NWP-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/NWP-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/README.txt` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/RKSJ-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/RKSJ-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniGB-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniGB-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UCS2-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UCS2-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF16-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF16-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF32-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF32-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF8-H.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/UniKS-UTF8-V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/UniKS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/V.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/cmapdb.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/cmapdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/converter.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/data_structures.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/data_structures.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/encodingdb.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/fontmetrics.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/glyphlist.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/high_level.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/high_level.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/image.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/image.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/jbig2.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/jbig2.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/latin_enc.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/latin_enc.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/layout.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import heapq
 import logging
 import unicodedata as UD
 import bidi.algorithm as BA
+import re
 from typing import (
     Dict,
     Generic,
     Iterable,
     Iterator,
     List,
     Optional,
@@ -567,35 +568,65 @@
                     UD.mirrored(unichar) and \
                     self._embedding_direction(_ch['level']) == 'R':
                 _ch['ch']._text = BA.MIRRORED.get(unichar, unichar)
 
     def bidi_textline(self):
         """Reorder Char in Textlines"""
         storage = BA.get_empty_storage()
-        text = self.get_text()
+        weirdtext = self.get_text()
+
+        text = self.removeWeirdChars(weirdtext)
+
         base_level = self.get_base_level(text)
         storage['base_level'] = base_level
         storage['base_dir'] = ('L', 'R')[base_level]
         self.get_embedding_levels(self._objs, storage)
         BA.explicit_embed_and_overrides(storage)
         BA.resolve_weak_types(storage)
         BA.resolve_neutral_types(storage, False)
         BA.resolve_implicit_levels(storage, False)
         BA.reorder_resolved_levels(storage, False)
         self.apply_mirroring(storage)
         self._objs = [_ch['ch'] for _ch in storage['chars']]
         return
     
+    # for fixing the bidi assertion in resolve_implicit_levels() bug https://github.com/alihoseiny/word_cloud_fa/issues/3
+    def removeWeirdChars(text):
+        weridPatterns = re.compile("["
+                               u"\U0001F600-\U0001F64F"  # emoticons
+                               u"\U0001F300-\U0001F5FF"  # symbols & pictographs
+                               u"\U0001F680-\U0001F6FF"  # transport & map symbols
+                               u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
+                               u"\U00002702-\U000027B0"
+                               u"\U000024C2-\U0001F251"
+                               u"\U0001f926-\U0001f937"
+                               u'\U00010000-\U0010ffff'
+                               u"\u200d"
+                               u"\u2640-\u2642"
+                               u"\u2600-\u2B55"
+                               u"\u23cf"
+                               u"\u23e9"
+                               u"\u231a"
+                               u"\u3030"
+                               u"\ufe0f"
+                               u"\u2069"
+                               u"\u2066"
+                               u"\u200c"
+                               u"\u2068"
+                               u"\u2067"
+                               "]+", flags=re.UNICODE)
+        return weridPatterns.sub(r'', text)
     
 
     # until here
 
     def analyze(self, laparams: LAParams) -> None:
         for obj in self._objs:
             obj.analyze(laparams)
+        # this was added too
         self.bidi_textline()
         LTContainer.add(self, LTAnno("\n"))
         return
 
     def find_neighbors(
         self, plane: Plane[LTComponentT], ratio: float
     ) -> List["LTTextLine"]:
```

### Comparing `pdfminer_rtl-0.0.1/pdfminer/lzw.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/lzw.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdfcolor.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfcolor.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdfdevice.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdevice.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdfdocument.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdffont.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdfinterp.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfinterp.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdfpage.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdfparser.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdfparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/pdftypes.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/pdftypes.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/psparser.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/runlength.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/runlength.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer/utils.py` & `pdfminer_rtl-0.0.2.dev3/pdfminer/utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/PKG-INFO` & `pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pdfminer.rtl
-Version: 0.0.1
+Version: 0.0.2.dev3
 Summary: PDF parser and analyzer
 Home-page: https://github.com/taneron/pdfminerrtl
-Author: Yusuke Shinyama + Philippe Guglielmetti
-Author-email: pdfminer@goulu.net
+Author: Yusuke Shinyama + Philippe Guglielmetti + Taner
+Author-email: pdfminerrtl@rust.8shield.net
 License: MIT
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,37 +35,28 @@
 Requires-Dist: mypy==0.931; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Provides-Extra: image
 Requires-Dist: Pillow; extra == "image"
 
-pdfminer.six
+pdfminer.rtl
 ============
 
-[![Continuous integration](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml/badge.svg)](https://github.com/pdfminer/pdfminer.six/actions/workflows/actions.yml)
-[![PyPI version](https://img.shields.io/pypi/v/pdfminer.six.svg)](https://pypi.python.org/pypi/pdfminer.six/)
-[![gitter](https://badges.gitter.im/pdfminer-six/Lobby.svg)](https://gitter.im/pdfminer-six/Lobby?utm_source=badge&utm_medium)
 
-*We fathom PDF*
+This is a fork of pdfminer.six that attempts to add RTL support with python-bidi. This version is experimental and probably buggy. Please don't rely on it for critical projects.
 
-Pdfminer.six is a community maintained fork of the original PDFMiner. It is a tool for extracting information from PDF
-documents. It focuses on getting and analyzing text data. Pdfminer.six extracts the text from a page directly from the
-sourcecode of the PDF. It can also be used to get the exact location, font or color of the text.
-
-It is built in a modular way such that each component of pdfminer.six can be replaced easily. You can implement your own
-interpreter or rendering device that uses the power of pdfminer.six for other purposes than text analysis.
-
-Check out the full documentation on
+Check out the full original documentation on
 [Read the Docs](https://pdfminersix.readthedocs.io).
 
 
 Features
 --------
 
+* (Added RTL support)
 * Written entirely in Python.
 * Parse, analyze, and convert PDF documents.
 * Extract content as text, images, html or [hOCR](https://en.wikipedia.org/wiki/HOCR).
 * PDF-1.7 specification support. (well, almost).
 * CJK languages and vertical writing scripts support.
 * Various font types (Type1, TrueType, Type3, and CID) support.
 * Support for extracting images (JPG, JBIG2, Bitmaps).
@@ -77,37 +68,32 @@
 * Tagged contents extraction.
 * Automatic layout analysis.
 
 How to use
 ----------
 
 * Install Python 3.8 or newer.
-* Install pdfminer.six.
+* Install pdfminer.rtl.
 
-  `pip install pdfminer.six`
+  `pip install pdfminer.rtl`
 
 * (Optionally) install extra dependencies for extracting images.
 
-  `pip install 'pdfminer.six[image]'`
+  `pip install 'pdfminer.rtl[image]'`
 
 * Use the command-line interface to extract text from pdf.
 
   `pdf2txt.py example.pdf`
 
 * Or use it with Python. 
 
 ```python
 from pdfminer.high_level import extract_text
 
 text = extract_text("example.pdf")
 print(text)
 ```
 
-Contributing
-------------
-
-Be sure to read the [contribution guidelines](https://github.com/pdfminer/pdfminer.six/blob/master/CONTRIBUTING.md). 
-
 Acknowledgement
 ---------------
 
-This repository includes code from `pyHanko` ; the original license has been included [here](/docs/licenses/LICENSE.pyHanko).
+This repository includes code from `pyHanko` ; the original license has been included [here](/docs/licenses/LICENSE.pyHanko) and to all the other contirbutors of the original project see [here](https://github.com/pdfminer/pdfminer.six/graphs/contributors)
```

### Comparing `pdfminer_rtl-0.0.1/pdfminer.rtl.egg-info/SOURCES.txt` & `pdfminer_rtl-0.0.2.dev3/pdfminer.rtl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/setup.py` & `pdfminer_rtl-0.0.2.dev3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 
 root_dir = Path(__file__).parent
 with open(root_dir / "README.md", "rt") as f:
     readme = f.read()
 
 setup(
     name="pdfminer.rtl",
+    version="0.0.2",
     setuptools_git_versioning={
         "enabled": True,
+        "template": "{tag}",
+         "dev_template": "{tag}.dev{ccount}",
+        "dirty_template": "{tag}.dev{ccount}",
     },
     setup_requires=["setuptools-git-versioning<2"],
     packages=["pdfminer"],
     package_data={"pdfminer": ["cmap/*.pickle.gz", "py.typed"]},
     install_requires=[
         "charset-normalizer >= 2.0.0",
         "cryptography >= 36.0.0",
@@ -25,16 +29,16 @@
         "docs": ["sphinx", "sphinx-argparse"],
         "image": ["Pillow"],
     },
     description="PDF parser and analyzer",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
-    author="Yusuke Shinyama + Philippe Guglielmetti",
-    author_email="pdfminer@goulu.net",
+    author="Yusuke Shinyama + Philippe Guglielmetti + Taner",
+    author_email="pdfminerrtl@rust.8shield.net",
     url="https://github.com/taneron/pdfminerrtl",
     scripts=[
         "tools/pdf2txt.py",
         "tools/dumppdf.py",
     ],
     keywords=[
         "pdf parser",
```

### Comparing `pdfminer_rtl-0.0.1/tests/test_converter.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_encodingdb.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_font_size.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_font_size.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_highlevel_extracttext.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_highlevel_extracttext.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_layout.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_pdfdocument.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_pdfencoding.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_pdfencoding.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_pdffont.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_pdfminer_ccitt.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_pdfminer_crypto.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_crypto.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_pdfminer_psparser.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_pdfminer_psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_pdfpage.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_tools_dumppdf.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_tools_dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_tools_pdf2txt.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_tools_pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tests/test_utils.py` & `pdfminer_rtl-0.0.2.dev3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/conv_afm.py` & `pdfminer_rtl-0.0.2.dev3/tools/conv_afm.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/conv_cmap.py` & `pdfminer_rtl-0.0.2.dev3/tools/conv_cmap.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/conv_glyphlist.py` & `pdfminer_rtl-0.0.2.dev3/tools/conv_glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/dumppdf.py` & `pdfminer_rtl-0.0.2.dev3/tools/dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/pdf2txt.py` & `pdfminer_rtl-0.0.2.dev3/tools/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/pdfdiff.py` & `pdfminer_rtl-0.0.2.dev3/tools/pdfdiff.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/pdfstats.py` & `pdfminer_rtl-0.0.2.dev3/tools/pdfstats.py`

 * *Files identical despite different names*

### Comparing `pdfminer_rtl-0.0.1/tools/prof.py` & `pdfminer_rtl-0.0.2.dev3/tools/prof.py`

 * *Files identical despite different names*

