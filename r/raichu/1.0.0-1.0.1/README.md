# Comparing `tmp/raichu-1.0.0.tar.gz` & `tmp/raichu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raichu-1.0.0.tar", last modified: Mon Apr 15 15:52:56 2024, max compression
+gzip compressed data, was "raichu-1.0.1.tar", last modified: Mon Apr 15 15:59:57 2024, max compression
```

## Comparing `raichu-1.0.0.tar` & `raichu-1.0.1.tar`

### file list

```diff
@@ -1,494 +1,494 @@
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.415982 raichu-1.0.0/
--rw-r--r--   0 barbara    (501) staff       (20)     1091 2022-11-01 19:03:21.000000 raichu-1.0.0/LICENSE.txt
--rw-r--r--   0 barbara    (501) staff       (20)      322 2024-04-15 15:52:56.415674 raichu-1.0.0/PKG-INFO
--rw-r--r--   0 barbara    (501) staff       (20)     2255 2024-04-15 15:19:04.000000 raichu-1.0.0/README.md
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.243041 raichu-1.0.0/bin/
--rw-r--r--   0 barbara    (501) staff       (20)     3137 2022-05-02 12:36:20.000000 raichu-1.0.0/bin/raichu
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.248049 raichu-1.0.0/interactive/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     1655 2022-04-17 16:18:30.000000 raichu-1.0.0/interactive/background.py
--rw-r--r--   0 barbara    (501) staff       (20)    38866 2022-05-01 17:29:00.000000 raichu-1.0.0/interactive/buttons.py
--rw-r--r--   0 barbara    (501) staff       (20)     2595 2022-05-01 12:51:17.000000 raichu-1.0.0/interactive/domain.py
--rw-r--r--   0 barbara    (501) staff       (20)     4354 2022-05-02 15:38:29.000000 raichu-1.0.0/interactive/gene.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.248446 raichu-1.0.0/interactive/images/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/__init__.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.255629 raichu-1.0.0/interactive/images/domains/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/domains/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    13363 2022-04-13 17:02:54.000000 raichu-1.0.0/interactive/images/domains/a.png
--rw-r--r--   0 barbara    (501) staff       (20)    13470 2022-04-14 07:32:59.000000 raichu-1.0.0/interactive/images/domains/a_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17374 2022-04-13 17:02:35.000000 raichu-1.0.0/interactive/images/domains/acp.png
--rw-r--r--   0 barbara    (501) staff       (20)    17372 2022-04-14 07:32:26.000000 raichu-1.0.0/interactive/images/domains/acp_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13468 2022-04-13 17:04:13.000000 raichu-1.0.0/interactive/images/domains/at.png
--rw-r--r--   0 barbara    (501) staff       (20)    13414 2022-04-14 07:35:16.000000 raichu-1.0.0/interactive/images/domains/at_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14370 2022-04-13 17:03:11.000000 raichu-1.0.0/interactive/images/domains/c.png
--rw-r--r--   0 barbara    (501) staff       (20)    14334 2022-04-14 07:33:37.000000 raichu-1.0.0/interactive/images/domains/c_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13271 2022-04-13 17:05:03.000000 raichu-1.0.0/interactive/images/domains/dh.png
--rw-r--r--   0 barbara    (501) staff       (20)    13201 2022-04-14 07:36:35.000000 raichu-1.0.0/interactive/images/domains/dh_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    11416 2022-04-13 17:03:29.000000 raichu-1.0.0/interactive/images/domains/e.png
--rw-r--r--   0 barbara    (501) staff       (20)    11408 2022-04-14 07:34:15.000000 raichu-1.0.0/interactive/images/domains/e_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13101 2022-04-13 17:05:18.000000 raichu-1.0.0/interactive/images/domains/er.png
--rw-r--r--   0 barbara    (501) staff       (20)    13218 2022-04-14 07:37:04.000000 raichu-1.0.0/interactive/images/domains/er_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14279 2022-04-13 17:04:47.000000 raichu-1.0.0/interactive/images/domains/kr.png
--rw-r--r--   0 barbara    (501) staff       (20)    14317 2022-04-14 07:36:07.000000 raichu-1.0.0/interactive/images/domains/kr_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16398 2022-04-13 17:04:28.000000 raichu-1.0.0/interactive/images/domains/ks.png
--rw-r--r--   0 barbara    (501) staff       (20)    16402 2022-04-14 07:35:43.000000 raichu-1.0.0/interactive/images/domains/ks_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13835 2022-04-13 17:05:36.000000 raichu-1.0.0/interactive/images/domains/nmt.png
--rw-r--r--   0 barbara    (501) staff       (20)    13911 2022-04-14 07:37:51.000000 raichu-1.0.0/interactive/images/domains/nmt_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-13 17:02:14.000000 raichu-1.0.0/interactive/images/domains/pcp.png
--rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-14 07:32:16.000000 raichu-1.0.0/interactive/images/domains/pcp_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    11757 2022-04-13 17:03:45.000000 raichu-1.0.0/interactive/images/domains/te.png
--rw-r--r--   0 barbara    (501) staff       (20)    11784 2022-04-14 07:34:50.000000 raichu-1.0.0/interactive/images/domains/te_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34945 2022-04-14 08:27:48.000000 raichu-1.0.0/interactive/images/icon.png
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.259540 raichu-1.0.0/interactive/images/kr_subtypes/
--rw-r--r--   0 barbara    (501) staff       (20)     6853 2022-04-16 14:37:34.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR.png
--rw-r--r--   0 barbara    (501) staff       (20)    10255 2022-04-16 14:40:44.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A1.png
--rw-r--r--   0 barbara    (501) staff       (20)    10233 2022-04-16 14:40:58.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A1_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14129 2022-04-16 14:40:22.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A2.png
--rw-r--r--   0 barbara    (501) staff       (20)    13940 2022-04-16 14:40:36.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A2_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)     9104 2022-04-16 14:39:53.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B1.png
--rw-r--r--   0 barbara    (501) staff       (20)     9076 2022-04-16 14:40:07.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B1_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    12935 2022-04-16 14:39:32.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B2.png
--rw-r--r--   0 barbara    (501) staff       (20)    12803 2022-04-16 14:39:45.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B2_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    11395 2022-04-16 14:39:06.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C1.png
--rw-r--r--   0 barbara    (501) staff       (20)    11318 2022-04-16 14:39:21.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C1_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14939 2022-04-16 14:38:43.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C2.png
--rw-r--r--   0 barbara    (501) staff       (20)    14756 2022-04-16 14:38:56.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C2_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)     6819 2022-04-16 14:38:16.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/kr_subtypes/__init__.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.383620 raichu-1.0.0/interactive/images/nrps_substrates/
--rw-r--r--   0 barbara    (501) staff       (20)    29614 2022-04-15 19:51:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    29531 2022-04-15 19:51:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29732 2022-04-15 19:50:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    30295 2022-04-15 19:50:55.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    42828 2022-04-15 19:59:58.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png
--rw-r--r--   0 barbara    (501) staff       (20)    40729 2022-04-15 20:00:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:51:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    30420 2022-04-15 19:51:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29315 2022-04-15 19:31:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    29122 2022-04-15 19:31:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34021 2022-04-15 19:27:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png
--rw-r--r--   0 barbara    (501) staff       (20)    31793 2022-04-15 19:27:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28970 2022-04-15 19:48:46.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    28787 2022-04-15 19:49:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27662 2022-04-15 17:47:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    30028 2022-04-15 17:47:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27300 2022-04-15 19:48:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    27047 2022-04-15 19:48:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    41323 2022-04-15 17:53:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    40856 2022-04-15 17:53:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25318 2022-04-15 19:41:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24974 2022-04-15 19:41:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:49:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23130 2022-04-15 19:50:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27411 2022-04-15 19:49:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    27276 2022-04-15 19:49:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23030 2022-04-15 19:22:32.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22312 2022-04-15 19:22:46.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30762 2022-04-15 17:48:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    29202 2022-04-15 17:48:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21732 2022-04-15 18:06:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate.png
--rw-r--r--   0 barbara    (501) staff       (20)    22544 2022-04-15 18:06:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21505 2022-04-15 18:49:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21077 2022-04-15 18:49:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    36652 2022-04-15 20:03:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    35330 2022-04-15 20:03:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25798 2022-04-15 19:59:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23250 2022-04-15 19:59:46.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    36143 2022-04-15 19:58:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    35659 2022-04-15 19:59:13.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22618 2022-04-15 18:05:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide.png
--rw-r--r--   0 barbara    (501) staff       (20)    22388 2022-04-15 18:05:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    39152 2022-04-15 19:30:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    38713 2022-04-15 19:31:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30192 2022-04-15 19:00:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    30391 2022-04-15 19:00:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31392 2022-04-15 19:30:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    30693 2022-04-15 19:30:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    37365 2022-04-15 19:29:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    36877 2022-04-15 19:30:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27121 2022-04-15 19:55:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25672 2022-04-15 19:55:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31631 2022-04-15 18:52:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    31245 2022-04-15 18:52:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    38385 2022-04-15 17:46:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    35115 2022-04-15 17:47:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24864 2022-04-15 19:39:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    24656 2022-04-15 19:39:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28181 2022-04-15 19:25:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    28922 2022-04-15 19:25:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25868 2022-04-15 19:02:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24839 2022-04-15 19:02:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24797 2022-04-15 19:18:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline.png
--rw-r--r--   0 barbara    (501) staff       (20)    24917 2022-04-15 19:18:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16493 2022-04-15 18:48:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16392 2022-04-15 18:49:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13602 2022-04-15 18:04:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alaninol.png
--rw-r--r--   0 barbara    (501) staff       (20)    13514 2022-04-15 18:05:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alaninol_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24271 2022-04-15 19:58:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin.png
--rw-r--r--   0 barbara    (501) staff       (20)    24821 2022-04-15 19:58:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23158 2022-04-15 18:51:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/Arginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22351 2022-04-15 18:51:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/Arginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21621 2022-04-15 18:53:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/Asparagine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21080 2022-04-15 18:53:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/Asparagine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23527 2022-04-15 18:54:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23278 2022-04-15 18:55:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    35623 2022-04-15 19:58:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    35114 2022-04-15 19:58:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19216 2022-04-15 19:42:23.000000 raichu-1.0.0/interactive/images/nrps_substrates/Citrulline.png
--rw-r--r--   0 barbara    (501) staff       (20)    20529 2022-04-15 19:42:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/Citrulline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17085 2022-04-15 18:57:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/Cysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17879 2022-04-15 18:57:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/Cysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25588 2022-04-15 19:47:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25308 2022-04-15 19:47:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23524 2022-04-15 19:46:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25188 2022-04-15 19:46:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25783 2022-04-15 19:40:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24378 2022-04-15 19:40:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23608 2022-04-15 19:47:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23287 2022-04-15 19:47:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25855 2022-04-15 18:03:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png
--rw-r--r--   0 barbara    (501) staff       (20)    25575 2022-04-15 18:03:32.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    35436 2022-04-15 20:02:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    33762 2022-04-15 20:03:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    15814 2022-04-15 18:47:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16164 2022-04-15 18:48:05.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24190 2022-04-15 18:51:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23965 2022-04-15 18:51:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23867 2022-04-15 18:52:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22155 2022-04-15 18:53:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24591 2022-04-15 18:54:13.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24267 2022-04-15 18:54:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21764 2022-04-15 19:41:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline.png
--rw-r--r--   0 barbara    (501) staff       (20)    21249 2022-04-15 19:42:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18606 2022-04-15 18:55:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16731 2022-04-15 18:56:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24393 2022-04-15 19:01:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24049 2022-04-15 19:01:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23556 2022-04-15 18:59:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22325 2022-04-15 19:00:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25709 2022-04-15 19:04:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25190 2022-04-15 19:04:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21390 2022-04-15 19:21:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21180 2022-04-15 19:22:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27223 2022-04-15 19:29:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26985 2022-04-15 19:29:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31175 2022-04-15 20:02:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    31281 2022-04-15 20:02:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21305 2022-04-15 19:05:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19584 2022-04-15 19:05:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18201 2022-04-15 19:08:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17837 2022-04-15 19:08:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20952 2022-04-15 19:09:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20688 2022-04-15 19:09:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22663 2022-04-15 19:11:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22585 2022-04-15 19:11:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22299 2022-04-15 20:02:00.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23920 2022-04-15 20:02:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28064 2022-04-15 19:13:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    27859 2022-04-15 19:13:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22124 2022-04-15 20:05:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22915 2022-04-15 20:05:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18477 2022-04-15 19:18:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Proline.png
--rw-r--r--   0 barbara    (501) staff       (20)    17643 2022-04-15 19:18:21.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Proline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16148 2022-04-15 19:21:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Serine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16632 2022-04-15 19:21:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Serine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20138 2022-04-15 19:23:45.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19101 2022-04-15 19:24:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31764 2022-04-15 19:26:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan.png
--rw-r--r--   0 barbara    (501) staff       (20)    31258 2022-04-15 19:26:31.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25906 2022-04-15 19:29:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25970 2022-04-15 19:29:16.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17416 2022-04-15 19:33:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Valine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17876 2022-04-15 19:33:58.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Valine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23148 2022-04-15 19:06:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23181 2022-04-15 19:06:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20985 2022-04-15 19:24:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20334 2022-04-15 19:24:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    33952 2022-04-15 19:13:38.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    34678 2022-04-15 19:13:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25846 2022-04-15 19:35:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    25587 2022-04-15 19:35:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24721 2022-04-15 18:57:03.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24505 2022-04-15 18:57:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21642 2022-04-15 17:58:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21479 2022-04-15 17:58:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29667 2022-04-15 18:56:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    29381 2022-04-15 18:56:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29226 2022-04-15 17:46:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png
--rw-r--r--   0 barbara    (501) staff       (20)    28550 2022-04-15 17:46:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24770 2022-04-15 19:52:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25682 2022-04-15 19:53:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22241 2022-04-15 17:57:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone.png
--rw-r--r--   0 barbara    (501) staff       (20)    22473 2022-04-15 17:58:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22735 2022-04-15 19:34:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    22465 2022-04-15 19:34:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30522 2022-04-15 19:53:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine.png
--rw-r--r--   0 barbara    (501) staff       (20)    29353 2022-04-15 19:54:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    41215 2022-04-15 17:07:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    41529 2022-04-15 17:07:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25178 2022-04-15 17:53:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22574 2022-04-15 17:54:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20125 2022-04-15 19:54:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19709 2022-04-15 19:55:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28423 2022-04-15 19:56:55.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin.png
--rw-r--r--   0 barbara    (501) staff       (20)    28205 2022-04-15 19:57:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21871 2022-04-15 19:08:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21647 2022-04-15 19:08:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21113 2022-04-15 19:45:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21341 2022-04-15 19:46:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22142 2022-04-15 19:01:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    21175 2022-04-15 19:01:30.000000 raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23165 2022-04-15 18:59:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glutamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23031 2022-04-15 18:59:42.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glutamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17898 2022-04-15 19:02:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17697 2022-04-15 19:03:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19769 2022-04-15 18:02:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21086 2022-04-15 18:03:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    15692 2022-04-15 18:02:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    16640 2022-04-15 18:02:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24850 2022-04-15 19:03:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/Histidine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23428 2022-04-15 19:03:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/Histidine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27835 2022-04-15 19:12:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    28660 2022-04-15 19:13:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20085 2022-04-15 19:20:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homoserine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20528 2022-04-15 19:20:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homoserine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25447 2022-04-15 19:28:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23415 2022-04-15 19:28:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28468 2022-04-15 20:01:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    28646 2022-04-15 20:01:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19848 2022-04-15 19:04:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20339 2022-04-15 19:04:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21246 2022-04-15 20:04:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    20649 2022-04-15 20:04:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17518 2022-04-15 19:07:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/Leucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    15410 2022-04-15 19:07:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/Leucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20333 2022-04-15 19:09:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/Lysine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19916 2022-04-15 19:09:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/Lysine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22102 2022-04-15 19:10:58.000000 raichu-1.0.0/interactive/images/nrps_substrates/Methionine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21961 2022-04-15 19:11:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/Methionine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27813 2022-04-15 19:12:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26592 2022-04-15 19:12:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20839 2022-04-15 19:32:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/Norvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    20626 2022-04-15 19:32:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/Norvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16556 2022-04-15 19:54:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/Ornithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17189 2022-04-15 19:54:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Ornithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26375 2022-04-15 19:12:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25087 2022-04-15 19:12:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21576 2022-04-15 20:04:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    19819 2022-04-15 20:04:30.000000 raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20332 2022-04-15 19:17:31.000000 raichu-1.0.0/interactive/images/nrps_substrates/Proline.png
--rw-r--r--   0 barbara    (501) staff       (20)    20084 2022-04-15 19:17:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/Proline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    32150 2022-04-15 17:03:55.000000 raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    28251 2022-04-15 17:04:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21333 2022-04-15 19:43:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    21941 2022-04-15 19:43:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:43:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22773 2022-04-15 19:43:16.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17234 2022-04-15 19:19:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/Serine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17342 2022-04-15 19:19:31.000000 raichu-1.0.0/interactive/images/nrps_substrates/Serine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18484 2022-04-15 19:23:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17304 2022-04-15 19:23:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31342 2022-04-15 19:25:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan.png
--rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:26:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25101 2022-04-15 19:27:42.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24311 2022-04-15 19:27:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16390 2022-04-15 19:32:05.000000 raichu-1.0.0/interactive/images/nrps_substrates/Valine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16071 2022-04-15 19:32:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/Valine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    21812 2022-04-15 19:06:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22026 2022-04-15 19:06:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19013 2022-04-15 19:24:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17084 2022-04-15 19:24:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34193 2022-04-15 19:14:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    33802 2022-04-15 19:14:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20539 2022-04-15 19:38:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    21837 2022-04-15 19:38:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25078 2022-04-15 18:04:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25232 2022-04-15 18:04:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21753 2022-04-15 18:03:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    19502 2022-04-15 18:04:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23125 2022-04-15 18:58:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21614 2022-04-15 18:58:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18232 2022-04-15 18:48:23.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17866 2022-04-15 18:48:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22745 2022-04-15 19:10:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22631 2022-04-15 19:10:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27655 2022-04-15 19:57:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine.png
--rw-r--r--   0 barbara    (501) staff       (20)    27032 2022-04-15 19:57:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23007 2022-04-15 19:44:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22918 2022-04-15 19:44:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20766 2022-04-15 17:58:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20540 2022-04-15 17:59:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28850 2022-04-15 18:58:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    29414 2022-04-15 18:58:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22320 2022-04-15 18:55:32.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22028 2022-04-15 18:55:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20723 2022-04-15 18:47:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20497 2022-04-15 18:47:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24909 2022-04-15 19:28:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24347 2022-04-15 19:28:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    32343 2022-04-15 17:07:03.000000 raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png
--rw-r--r--   0 barbara    (501) staff       (20)    31754 2022-04-15 17:07:23.000000 raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27766 2022-04-15 19:52:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/enduracididine.png
--rw-r--r--   0 barbara    (501) staff       (20)    27194 2022-04-15 19:52:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/enduracididine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23358 2022-04-15 18:50:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoarginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24247 2022-04-15 18:50:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoarginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23746 2022-04-15 19:05:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23630 2022-04-15 19:05:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22096 2022-04-15 17:57:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone.png
--rw-r--r--   0 barbara    (501) staff       (20)    21719 2022-04-15 17:57:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26982 2022-04-15 17:06:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25601 2022-04-15 17:06:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26043 2022-04-15 17:05:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25858 2022-04-15 17:06:13.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21960 2022-04-15 19:33:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/isovaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    21200 2022-04-15 19:33:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/isovaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26809 2022-04-15 19:53:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/kynurenine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26107 2022-04-15 19:53:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/kynurenine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24972 2022-04-15 17:54:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    26606 2022-04-15 17:54:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21926 2022-04-15 19:44:05.000000 raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    20749 2022-04-15 19:44:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18052 2022-04-15 18:08:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/nrp.png
--rw-r--r--   0 barbara    (501) staff       (20)    17895 2022-04-15 18:09:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/nrp_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25531 2022-04-15 17:05:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25533 2022-04-15 17:05:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26331 2022-04-15 20:00:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26106 2022-04-15 20:00:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27784 2022-04-15 19:56:30.000000 raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin.png
--rw-r--r--   0 barbara    (501) staff       (20)    27870 2022-04-15 19:56:42.000000 raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24381 2022-04-15 16:53:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23788 2022-04-15 17:51:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21002 2022-04-15 19:06:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu.png
--rw-r--r--   0 barbara    (501) staff       (20)    20891 2022-04-15 19:07:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16198 2022-04-15 18:01:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/valinol.png
--rw-r--r--   0 barbara    (501) staff       (20)    16320 2022-04-15 18:01:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/valinol_highlight.png
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.395629 raichu-1.0.0/interactive/images/pks_starter_substrates/
--rw-r--r--   0 barbara    (501) staff       (20)    29850 2022-05-01 12:06:56.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    26673 2022-05-01 12:07:06.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25251 2022-05-01 12:06:33.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    23606 2022-05-01 12:06:48.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    33676 2022-05-01 12:06:14.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    33230 2022-05-01 12:06:24.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26972 2022-05-01 12:05:48.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    26664 2022-05-01 12:06:03.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24670 2022-05-01 12:07:17.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    24923 2022-05-01 12:07:25.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25417 2022-05-01 12:05:22.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    25187 2022-05-01 12:05:39.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20866 2022-05-01 12:05:03.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Ac.png
--rw-r--r--   0 barbara    (501) staff       (20)    21010 2022-05-01 12:05:13.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Ac_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25026 2022-05-01 12:04:44.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Benz.png
--rw-r--r--   0 barbara    (501) staff       (20)    25713 2022-05-01 12:04:54.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Benz_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34080 2022-05-01 12:04:21.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/CHC.png
--rw-r--r--   0 barbara    (501) staff       (20)    33079 2022-05-01 12:04:32.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/CHC_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21110 2022-05-01 12:03:36.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Prop.png
--rw-r--r--   0 barbara    (501) staff       (20)    20850 2022-05-01 12:03:52.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Prop_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    32496 2022-05-01 12:40:12.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    31629 2022-05-01 12:40:20.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29134 2022-05-01 12:04:02.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/hMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    28542 2022-05-01 12:04:10.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/hMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22191 2022-05-01 16:48:04.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    21953 2022-05-01 16:48:17.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    41464 2022-05-01 12:03:11.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA.png
--rw-r--r--   0 barbara    (501) staff       (20)    40950 2022-05-01 12:03:25.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA_highlight.png
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.399265 raichu-1.0.0/interactive/images/pks_substrates/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/pks_substrates/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    24949 2022-04-16 08:01:15.000000 raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    25556 2022-04-16 08:01:32.000000 raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24099 2022-04-16 07:57:17.000000 raichu-1.0.0/interactive/images/pks_substrates/malonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    23782 2022-04-16 07:59:21.000000 raichu-1.0.0/interactive/images/pks_substrates/malonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28684 2022-04-16 08:02:38.000000 raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    28317 2022-04-16 08:02:54.000000 raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25513 2022-04-16 07:58:33.000000 raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    25625 2022-04-16 07:58:50.000000 raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21959 2022-04-16 08:04:06.000000 raichu-1.0.0/interactive/images/pks_substrates/wildcard.png
--rw-r--r--   0 barbara    (501) staff       (20)    22218 2022-04-16 08:04:28.000000 raichu-1.0.0/interactive/images/pks_substrates/wildcard_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)      913 2022-04-14 09:57:57.000000 raichu-1.0.0/interactive/insertion_point.py
--rw-r--r--   0 barbara    (501) staff       (20)    11853 2022-05-02 15:50:16.000000 raichu-1.0.0/interactive/load_antismash.py
--rw-r--r--   0 barbara    (501) staff       (20)     4136 2022-05-02 13:04:31.000000 raichu-1.0.0/interactive/load_tabular.py
--rw-r--r--   0 barbara    (501) staff       (20)     3769 2022-04-19 13:35:36.000000 raichu-1.0.0/interactive/module.py
--rw-r--r--   0 barbara    (501) staff       (20)      306 2022-04-15 16:35:29.000000 raichu-1.0.0/interactive/parsers.py
--rw-r--r--   0 barbara    (501) staff       (20)     5462 2022-10-24 15:18:24.000000 raichu-1.0.0/interactive/render_cluster.py
--rw-r--r--   0 barbara    (501) staff       (20)    27124 2022-05-05 14:52:33.000000 raichu-1.0.0/interactive/run_raichu.py
--rw-r--r--   0 barbara    (501) staff       (20)     2083 2022-05-05 14:48:17.000000 raichu-1.0.0/interactive/style.py
--rw-r--r--   0 barbara    (501) staff       (20)    18130 2022-05-08 06:33:46.000000 raichu-1.0.0/interactive/substrate.py
--rw-r--r--   0 barbara    (501) staff       (20)     1117 2022-04-14 09:00:39.000000 raichu-1.0.0/interactive/textbox.py
--rw-r--r--   0 barbara    (501) staff       (20)       89 2021-09-16 23:05:31.000000 raichu-1.0.0/pyproject.toml
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.402906 raichu-1.0.0/raichu/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/raichu/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     3656 2024-02-08 09:09:32.000000 raichu-1.0.0/raichu/alkaloid.py
--rw-r--r--   0 barbara    (501) staff       (20)    37295 2024-04-15 15:44:13.000000 raichu-1.0.0/raichu/antismash.py
--rw-r--r--   0 barbara    (501) staff       (20)    11162 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/attach_to_domain.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.404211 raichu-1.0.0/raichu/central_chain_detection/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/central_chain_detection/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     9199 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/central_chain_detection/find_central_chain.py
--rw-r--r--   0 barbara    (501) staff       (20)    19314 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/central_chain_detection/label_central_chain.py
--rw-r--r--   0 barbara    (501) staff       (20)     4124 2023-05-01 07:37:35.000000 raichu-1.0.0/raichu/class_domain.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.405841 raichu-1.0.0/raichu/cluster/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2023-05-07 08:18:53.000000 raichu-1.0.0/raichu/cluster/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)      736 2023-05-07 08:52:51.000000 raichu-1.0.0/raichu/cluster/alkaloid_cluster.py
--rw-r--r--   0 barbara    (501) staff       (20)    16380 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/cluster/base_cluster.py
--rw-r--r--   0 barbara    (501) staff       (20)    15618 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/cluster/modular_cluster.py
--rw-r--r--   0 barbara    (501) staff       (20)    16428 2023-05-07 17:50:23.000000 raichu-1.0.0/raichu/cluster/ripp_cluster.py
--rw-r--r--   0 barbara    (501) staff       (20)     5799 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/cluster/terpene_cluster.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.408417 raichu-1.0.0/raichu/data/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)      137 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/at_elongation_specificities.txt
--rw-r--r--   0 barbara    (501) staff       (20)      269 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/at_specificities.txt
--rw-r--r--   0 barbara    (501) staff       (20)     4969 2023-12-08 12:52:08.000000 raichu-1.0.0/raichu/data/attributes.py
--rw-r--r--   0 barbara    (501) staff       (20)    20943 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/metadata.txt
--rw-r--r--   0 barbara    (501) staff       (20)    10888 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/molecular_moieties.py
--rw-r--r--   0 barbara    (501) staff       (20)    14079 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/smiles.txt
--rw-r--r--   0 barbara    (501) staff       (20)     3834 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/substrate_to_abbreviation.txt
--rw-r--r--   0 barbara    (501) staff       (20)     9683 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/trans_at.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.409217 raichu-1.0.0/raichu/domain/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/domain/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    10455 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/domain/domain.py
--rw-r--r--   0 barbara    (501) staff       (20)     5614 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/domain/domain_types.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.411412 raichu-1.0.0/raichu/drawing/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/drawing/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     9301 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/drawing/bubbles.py
--rw-r--r--   0 barbara    (501) staff       (20)     5636 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/drawing/colours.py
--rw-r--r--   0 barbara    (501) staff       (20)    83982 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/drawing/drawer.py
--rw-r--r--   0 barbara    (501) staff       (20)     1613 2023-05-07 18:03:32.000000 raichu-1.0.0/raichu/drawing/pathway.py
--rw-r--r--   0 barbara    (501) staff       (20)      678 2023-05-07 08:52:51.000000 raichu-1.0.0/raichu/drawing/ripp_drawing.py
--rw-r--r--   0 barbara    (501) staff       (20)     5734 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/general.py
--rw-r--r--   0 barbara    (501) staff       (20)    25860 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/module.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.413792 raichu-1.0.0/raichu/reactions/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/reactions/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    12341 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/chain_release.py
--rw-r--r--   0 barbara    (501) staff       (20)     1001 2024-02-08 15:43:23.000000 raichu-1.0.0/raichu/reactions/general.py
--rw-r--r--   0 barbara    (501) staff       (20)    19163 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/general_tailoring_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     4530 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/nrps_elongation_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     5632 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/nrps_tailoring_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     4658 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/pks_elongation_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     1125 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/pks_sidechain_chirality.py
--rw-r--r--   0 barbara    (501) staff       (20)    34020 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/pks_tailoring_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     2403 2023-05-01 07:37:35.000000 raichu-1.0.0/raichu/reactions/ripp_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     6737 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/representations.py
--rw-r--r--   0 barbara    (501) staff       (20)    21201 2024-02-08 09:09:32.000000 raichu-1.0.0/raichu/ripp.py
--rw-r--r--   0 barbara    (501) staff       (20)    38926 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/run_raichu.py
--rw-r--r--   0 barbara    (501) staff       (20)     2806 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/smiles_handling.py
--rw-r--r--   0 barbara    (501) staff       (20)     6667 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/substrate.py
--rw-r--r--   0 barbara    (501) staff       (20)    32389 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/tailoring_enzymes.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414171 raichu-1.0.0/raichu/test/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     9670 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/generate_test_data.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414366 raichu-1.0.0/raichu/test/test_data/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/test_data/__init__.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414490 raichu-1.0.0/raichu/test/unit/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/__init__.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414863 raichu-1.0.0/raichu/test/unit/reactions/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/reactions/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/reactions/test_general_tailoring_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)      416 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/reactions/test_nrps_tailoring_reactions.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.415203 raichu-1.0.0/raichu.egg-info/
--rw-r--r--   0 barbara    (501) staff       (20)      322 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/PKG-INFO
--rw-r--r--   0 barbara    (501) staff       (20)    25323 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/SOURCES.txt
--rw-r--r--   0 barbara    (501) staff       (20)        1 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/dependency_links.txt
--rw-r--r--   0 barbara    (501) staff       (20)       47 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/requires.txt
--rw-r--r--   0 barbara    (501) staff       (20)       19 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/top_level.txt
--rw-r--r--   0 barbara    (501) staff       (20)       38 2024-04-15 15:52:56.416037 raichu-1.0.0/setup.cfg
--rw-r--r--   0 barbara    (501) staff       (20)      650 2024-04-15 15:48:01.000000 raichu-1.0.0/setup.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.702271 raichu-1.0.1/
+-rw-r--r--   0 barbara    (501) staff       (20)     1091 2022-11-01 19:03:21.000000 raichu-1.0.1/LICENSE.txt
+-rw-r--r--   0 barbara    (501) staff       (20)      322 2024-04-15 15:59:57.701947 raichu-1.0.1/PKG-INFO
+-rw-r--r--   0 barbara    (501) staff       (20)     2255 2024-04-15 15:19:04.000000 raichu-1.0.1/README.md
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.518856 raichu-1.0.1/bin/
+-rw-r--r--   0 barbara    (501) staff       (20)     3137 2022-05-02 12:36:20.000000 raichu-1.0.1/bin/raichu
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.524619 raichu-1.0.1/interactive/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/interactive/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1655 2022-04-17 16:18:30.000000 raichu-1.0.1/interactive/background.py
+-rw-r--r--   0 barbara    (501) staff       (20)    38866 2022-05-01 17:29:00.000000 raichu-1.0.1/interactive/buttons.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2595 2022-05-01 12:51:17.000000 raichu-1.0.1/interactive/domain.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4354 2022-05-02 15:38:29.000000 raichu-1.0.1/interactive/gene.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.524993 raichu-1.0.1/interactive/images/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/interactive/images/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.535932 raichu-1.0.1/interactive/images/domains/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/interactive/images/domains/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    13363 2022-04-13 17:02:54.000000 raichu-1.0.1/interactive/images/domains/a.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13470 2022-04-14 07:32:59.000000 raichu-1.0.1/interactive/images/domains/a_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17374 2022-04-13 17:02:35.000000 raichu-1.0.1/interactive/images/domains/acp.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17372 2022-04-14 07:32:26.000000 raichu-1.0.1/interactive/images/domains/acp_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13468 2022-04-13 17:04:13.000000 raichu-1.0.1/interactive/images/domains/at.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13414 2022-04-14 07:35:16.000000 raichu-1.0.1/interactive/images/domains/at_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14370 2022-04-13 17:03:11.000000 raichu-1.0.1/interactive/images/domains/c.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14334 2022-04-14 07:33:37.000000 raichu-1.0.1/interactive/images/domains/c_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13271 2022-04-13 17:05:03.000000 raichu-1.0.1/interactive/images/domains/dh.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13201 2022-04-14 07:36:35.000000 raichu-1.0.1/interactive/images/domains/dh_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11416 2022-04-13 17:03:29.000000 raichu-1.0.1/interactive/images/domains/e.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11408 2022-04-14 07:34:15.000000 raichu-1.0.1/interactive/images/domains/e_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13101 2022-04-13 17:05:18.000000 raichu-1.0.1/interactive/images/domains/er.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13218 2022-04-14 07:37:04.000000 raichu-1.0.1/interactive/images/domains/er_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14279 2022-04-13 17:04:47.000000 raichu-1.0.1/interactive/images/domains/kr.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14317 2022-04-14 07:36:07.000000 raichu-1.0.1/interactive/images/domains/kr_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16398 2022-04-13 17:04:28.000000 raichu-1.0.1/interactive/images/domains/ks.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16402 2022-04-14 07:35:43.000000 raichu-1.0.1/interactive/images/domains/ks_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13835 2022-04-13 17:05:36.000000 raichu-1.0.1/interactive/images/domains/nmt.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13911 2022-04-14 07:37:51.000000 raichu-1.0.1/interactive/images/domains/nmt_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-13 17:02:14.000000 raichu-1.0.1/interactive/images/domains/pcp.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-14 07:32:16.000000 raichu-1.0.1/interactive/images/domains/pcp_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11757 2022-04-13 17:03:45.000000 raichu-1.0.1/interactive/images/domains/te.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11784 2022-04-14 07:34:50.000000 raichu-1.0.1/interactive/images/domains/te_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34945 2022-04-14 08:27:48.000000 raichu-1.0.1/interactive/images/icon.png
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.540544 raichu-1.0.1/interactive/images/kr_subtypes/
+-rw-r--r--   0 barbara    (501) staff       (20)     6853 2022-04-16 14:37:34.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR.png
+-rw-r--r--   0 barbara    (501) staff       (20)    10255 2022-04-16 14:40:44.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_A1.png
+-rw-r--r--   0 barbara    (501) staff       (20)    10233 2022-04-16 14:40:58.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_A1_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14129 2022-04-16 14:40:22.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_A2.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13940 2022-04-16 14:40:36.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_A2_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)     9104 2022-04-16 14:39:53.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_B1.png
+-rw-r--r--   0 barbara    (501) staff       (20)     9076 2022-04-16 14:40:07.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_B1_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    12935 2022-04-16 14:39:32.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_B2.png
+-rw-r--r--   0 barbara    (501) staff       (20)    12803 2022-04-16 14:39:45.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_B2_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11395 2022-04-16 14:39:06.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_C1.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11318 2022-04-16 14:39:21.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_C1_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14939 2022-04-16 14:38:43.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_C2.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14756 2022-04-16 14:38:56.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_C2_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)     6819 2022-04-16 14:38:16.000000 raichu-1.0.1/interactive/images/kr_subtypes/KR_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/interactive/images/kr_subtypes/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.669325 raichu-1.0.1/interactive/images/nrps_substrates/
+-rw-r--r--   0 barbara    (501) staff       (20)    29614 2022-04-15 19:51:37.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29531 2022-04-15 19:51:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29732 2022-04-15 19:50:40.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30295 2022-04-15 19:50:55.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    42828 2022-04-15 19:59:58.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png
+-rw-r--r--   0 barbara    (501) staff       (20)    40729 2022-04-15 20:00:18.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:51:06.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30420 2022-04-15 19:51:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29315 2022-04-15 19:31:17.000000 raichu-1.0.1/interactive/images/nrps_substrates/(R)beta-tyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29122 2022-04-15 19:31:33.000000 raichu-1.0.1/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34021 2022-04-15 19:27:06.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31793 2022-04-15 19:27:22.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28970 2022-04-15 19:48:46.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28787 2022-04-15 19:49:02.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27662 2022-04-15 17:47:25.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30028 2022-04-15 17:47:47.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27300 2022-04-15 19:48:17.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27047 2022-04-15 19:48:34.000000 raichu-1.0.1/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41323 2022-04-15 17:53:10.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    40856 2022-04-15 17:53:29.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25318 2022-04-15 19:41:11.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoadipicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24974 2022-04-15 19:41:27.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:49:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Aminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23130 2022-04-15 19:50:28.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27411 2022-04-15 19:49:12.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27276 2022-04-15 19:49:28.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23030 2022-04-15 19:22:32.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Methylserine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22312 2022-04-15 19:22:46.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-Methylserine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30762 2022-04-15 17:48:14.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-carboxyquinoxaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29202 2022-04-15 17:48:52.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21732 2022-04-15 18:06:09.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-hydroxyisovalerate.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22544 2022-04-15 18:06:25.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21505 2022-04-15 18:49:40.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-methyl-beta-alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21077 2022-04-15 18:49:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    36652 2022-04-15 20:03:20.000000 raichu-1.0.1/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35330 2022-04-15 20:03:33.000000 raichu-1.0.1/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25798 2022-04-15 19:59:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23250 2022-04-15 19:59:46.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    36143 2022-04-15 19:58:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35659 2022-04-15 19:59:13.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22618 2022-04-15 18:05:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-aminopropanimidamide.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22388 2022-04-15 18:05:57.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    39152 2022-04-15 19:30:48.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    38713 2022-04-15 19:31:04.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30192 2022-04-15 19:00:25.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxyglutamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30391 2022-04-15 19:00:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31392 2022-04-15 19:30:19.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-methyltyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30693 2022-04-15 19:30:35.000000 raichu-1.0.1/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    37365 2022-04-15 19:29:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    36877 2022-04-15 19:30:07.000000 raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27121 2022-04-15 19:55:37.000000 raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25672 2022-04-15 19:55:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31631 2022-04-15 18:52:08.000000 raichu-1.0.1/interactive/images/nrps_substrates/4,5-dehydroarginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31245 2022-04-15 18:52:24.000000 raichu-1.0.1/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    38385 2022-04-15 17:46:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35115 2022-04-15 17:47:09.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24864 2022-04-15 19:39:08.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24656 2022-04-15 19:39:27.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28181 2022-04-15 19:25:04.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28922 2022-04-15 19:25:19.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25868 2022-04-15 19:02:08.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-methylglutamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24839 2022-04-15 19:02:29.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24797 2022-04-15 19:18:33.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-methylproline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24917 2022-04-15 19:18:49.000000 raichu-1.0.1/interactive/images/nrps_substrates/4-methylproline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16493 2022-04-15 18:48:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16392 2022-04-15 18:49:28.000000 raichu-1.0.1/interactive/images/nrps_substrates/Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13602 2022-04-15 18:04:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/Alaninol.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13514 2022-04-15 18:05:22.000000 raichu-1.0.1/interactive/images/nrps_substrates/Alaninol_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24271 2022-04-15 19:58:29.000000 raichu-1.0.1/interactive/images/nrps_substrates/Anticapsin.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24821 2022-04-15 19:58:43.000000 raichu-1.0.1/interactive/images/nrps_substrates/Anticapsin_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23158 2022-04-15 18:51:35.000000 raichu-1.0.1/interactive/images/nrps_substrates/Arginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22351 2022-04-15 18:51:52.000000 raichu-1.0.1/interactive/images/nrps_substrates/Arginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21621 2022-04-15 18:53:20.000000 raichu-1.0.1/interactive/images/nrps_substrates/Asparagine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21080 2022-04-15 18:53:35.000000 raichu-1.0.1/interactive/images/nrps_substrates/Asparagine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23527 2022-04-15 18:54:54.000000 raichu-1.0.1/interactive/images/nrps_substrates/AsparticAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23278 2022-04-15 18:55:10.000000 raichu-1.0.1/interactive/images/nrps_substrates/AsparticAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35623 2022-04-15 19:58:02.000000 raichu-1.0.1/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35114 2022-04-15 19:58:20.000000 raichu-1.0.1/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19216 2022-04-15 19:42:23.000000 raichu-1.0.1/interactive/images/nrps_substrates/Citrulline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20529 2022-04-15 19:42:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/Citrulline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17085 2022-04-15 18:57:37.000000 raichu-1.0.1/interactive/images/nrps_substrates/Cysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17879 2022-04-15 18:57:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/Cysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25588 2022-04-15 19:47:11.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25308 2022-04-15 19:47:22.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23524 2022-04-15 19:46:29.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25188 2022-04-15 19:46:49.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25783 2022-04-15 19:40:35.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24378 2022-04-15 19:40:56.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23608 2022-04-15 19:47:33.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23287 2022-04-15 19:47:50.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25855 2022-04-15 18:03:18.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25575 2022-04-15 18:03:32.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35436 2022-04-15 20:02:49.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33762 2022-04-15 20:03:07.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15814 2022-04-15 18:47:50.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16164 2022-04-15 18:48:05.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24190 2022-04-15 18:51:04.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Arginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23965 2022-04-15 18:51:24.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Arginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23867 2022-04-15 18:52:47.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Asparagine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22155 2022-04-15 18:53:06.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Asparagine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24591 2022-04-15 18:54:13.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-AsparticAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24267 2022-04-15 18:54:43.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21764 2022-04-15 19:41:54.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Citrulline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21249 2022-04-15 19:42:12.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Citrulline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18606 2022-04-15 18:55:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Cysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16731 2022-04-15 18:56:20.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Cysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24393 2022-04-15 19:01:41.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-GlutamicAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24049 2022-04-15 19:01:57.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23556 2022-04-15 18:59:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Glutamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22325 2022-04-15 19:00:07.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Glutamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25709 2022-04-15 19:04:01.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Histidine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25190 2022-04-15 19:04:17.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Histidine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21390 2022-04-15 19:21:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Homoserine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21180 2022-04-15 19:22:18.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Homoserine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27223 2022-04-15 19:29:28.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Homotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26985 2022-04-15 19:29:41.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31175 2022-04-15 20:02:25.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31281 2022-04-15 20:02:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21305 2022-04-15 19:05:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19584 2022-04-15 19:05:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18201 2022-04-15 19:08:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Leucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17837 2022-04-15 19:08:56.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Leucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20952 2022-04-15 19:09:44.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Lysine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20688 2022-04-15 19:09:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Lysine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22663 2022-04-15 19:11:19.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Methionine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22585 2022-04-15 19:11:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Methionine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22299 2022-04-15 20:02:00.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-PhenylGlycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23920 2022-04-15 20:02:14.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28064 2022-04-15 19:13:14.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Phenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27859 2022-04-15 19:13:28.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22124 2022-04-15 20:05:08.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Pipecolicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22915 2022-04-15 20:05:27.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18477 2022-04-15 19:18:02.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Proline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17643 2022-04-15 19:18:21.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Proline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16148 2022-04-15 19:21:15.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Serine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16632 2022-04-15 19:21:29.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Serine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20138 2022-04-15 19:23:45.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19101 2022-04-15 19:24:01.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31764 2022-04-15 19:26:12.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Tryptophan.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31258 2022-04-15 19:26:31.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Tryptophan_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25906 2022-04-15 19:29:01.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Tyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25970 2022-04-15 19:29:16.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Tyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17416 2022-04-15 19:33:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Valine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17876 2022-04-15 19:33:58.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-Valine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23148 2022-04-15 19:06:01.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23181 2022-04-15 19:06:15.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20985 2022-04-15 19:24:11.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20334 2022-04-15 19:24:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33952 2022-04-15 19:13:38.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34678 2022-04-15 19:13:52.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25846 2022-04-15 19:35:06.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25587 2022-04-15 19:35:19.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24721 2022-04-15 18:57:03.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-methylcysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24505 2022-04-15 18:57:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21642 2022-04-15 17:58:25.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-cycloOrnithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21479 2022-04-15 17:58:41.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29667 2022-04-15 18:56:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-cysteicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29381 2022-04-15 18:56:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-cysteicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29226 2022-04-15 17:46:15.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28550 2022-04-15 17:46:34.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24770 2022-04-15 19:52:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-enduracididine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25682 2022-04-15 19:53:04.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-enduracididine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22241 2022-04-15 17:57:52.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-homoserinelactone.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22473 2022-04-15 17:58:11.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22735 2022-04-15 19:34:15.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-isovaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22465 2022-04-15 19:34:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-isovaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30522 2022-04-15 19:53:52.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-kynurenine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29353 2022-04-15 19:54:07.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-kynurenine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41215 2022-04-15 17:07:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-lysergicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41529 2022-04-15 17:07:56.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-lysergicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25178 2022-04-15 17:53:52.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22574 2022-04-15 17:54:07.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20125 2022-04-15 19:54:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-ornithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19709 2022-04-15 19:55:22.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-ornithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28423 2022-04-15 19:56:55.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-phosphinothricin.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28205 2022-04-15 19:57:09.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21871 2022-04-15 19:08:08.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-tert-Leucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21647 2022-04-15 19:08:27.000000 raichu-1.0.1/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21113 2022-04-15 19:45:57.000000 raichu-1.0.1/interactive/images/nrps_substrates/Dehydrobutyrine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21341 2022-04-15 19:46:14.000000 raichu-1.0.1/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22142 2022-04-15 19:01:12.000000 raichu-1.0.1/interactive/images/nrps_substrates/GlutamicAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21175 2022-04-15 19:01:30.000000 raichu-1.0.1/interactive/images/nrps_substrates/GlutamicAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23165 2022-04-15 18:59:19.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glutamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23031 2022-04-15 18:59:42.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glutamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17898 2022-04-15 19:02:50.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17697 2022-04-15 19:03:09.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19769 2022-04-15 18:02:48.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glycocyamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21086 2022-04-15 18:03:06.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glycocyamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15692 2022-04-15 18:02:08.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glycolicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16640 2022-04-15 18:02:29.000000 raichu-1.0.1/interactive/images/nrps_substrates/Glycolicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24850 2022-04-15 19:03:33.000000 raichu-1.0.1/interactive/images/nrps_substrates/Histidine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23428 2022-04-15 19:03:48.000000 raichu-1.0.1/interactive/images/nrps_substrates/Histidine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27835 2022-04-15 19:12:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/Homophenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28660 2022-04-15 19:13:04.000000 raichu-1.0.1/interactive/images/nrps_substrates/Homophenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20085 2022-04-15 19:20:19.000000 raichu-1.0.1/interactive/images/nrps_substrates/Homoserine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20528 2022-04-15 19:20:35.000000 raichu-1.0.1/interactive/images/nrps_substrates/Homoserine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25447 2022-04-15 19:28:07.000000 raichu-1.0.1/interactive/images/nrps_substrates/Homotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23415 2022-04-15 19:28:20.000000 raichu-1.0.1/interactive/images/nrps_substrates/Homotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28468 2022-04-15 20:01:09.000000 raichu-1.0.1/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28646 2022-04-15 20:01:40.000000 raichu-1.0.1/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19848 2022-04-15 19:04:43.000000 raichu-1.0.1/interactive/images/nrps_substrates/Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20339 2022-04-15 19:04:57.000000 raichu-1.0.1/interactive/images/nrps_substrates/Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21246 2022-04-15 20:04:41.000000 raichu-1.0.1/interactive/images/nrps_substrates/L-piperazicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20649 2022-04-15 20:04:56.000000 raichu-1.0.1/interactive/images/nrps_substrates/L-piperazicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17518 2022-04-15 19:07:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/Leucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15410 2022-04-15 19:07:57.000000 raichu-1.0.1/interactive/images/nrps_substrates/Leucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20333 2022-04-15 19:09:15.000000 raichu-1.0.1/interactive/images/nrps_substrates/Lysine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19916 2022-04-15 19:09:34.000000 raichu-1.0.1/interactive/images/nrps_substrates/Lysine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22102 2022-04-15 19:10:58.000000 raichu-1.0.1/interactive/images/nrps_substrates/Methionine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21961 2022-04-15 19:11:10.000000 raichu-1.0.1/interactive/images/nrps_substrates/Methionine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27813 2022-04-15 19:12:27.000000 raichu-1.0.1/interactive/images/nrps_substrates/N-acetylphenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26592 2022-04-15 19:12:41.000000 raichu-1.0.1/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20839 2022-04-15 19:32:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/Norvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20626 2022-04-15 19:32:47.000000 raichu-1.0.1/interactive/images/nrps_substrates/Norvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16556 2022-04-15 19:54:29.000000 raichu-1.0.1/interactive/images/nrps_substrates/Ornithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17189 2022-04-15 19:54:43.000000 raichu-1.0.1/interactive/images/nrps_substrates/Ornithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26375 2022-04-15 19:12:02.000000 raichu-1.0.1/interactive/images/nrps_substrates/Phenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25087 2022-04-15 19:12:17.000000 raichu-1.0.1/interactive/images/nrps_substrates/Phenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21576 2022-04-15 20:04:15.000000 raichu-1.0.1/interactive/images/nrps_substrates/Pipecolicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19819 2022-04-15 20:04:30.000000 raichu-1.0.1/interactive/images/nrps_substrates/Pipecolicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20332 2022-04-15 19:17:31.000000 raichu-1.0.1/interactive/images/nrps_substrates/Proline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20084 2022-04-15 19:17:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/Proline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    32150 2022-04-15 17:03:55.000000 raichu-1.0.1/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28251 2022-04-15 17:04:40.000000 raichu-1.0.1/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21333 2022-04-15 19:43:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/R-coronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21941 2022-04-15 19:43:48.000000 raichu-1.0.1/interactive/images/nrps_substrates/R-coronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:43:02.000000 raichu-1.0.1/interactive/images/nrps_substrates/R-norcoronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22773 2022-04-15 19:43:16.000000 raichu-1.0.1/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17234 2022-04-15 19:19:18.000000 raichu-1.0.1/interactive/images/nrps_substrates/Serine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17342 2022-04-15 19:19:31.000000 raichu-1.0.1/interactive/images/nrps_substrates/Serine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18484 2022-04-15 19:23:19.000000 raichu-1.0.1/interactive/images/nrps_substrates/Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17304 2022-04-15 19:23:34.000000 raichu-1.0.1/interactive/images/nrps_substrates/Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31342 2022-04-15 19:25:43.000000 raichu-1.0.1/interactive/images/nrps_substrates/Tryptophan.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:26:56.000000 raichu-1.0.1/interactive/images/nrps_substrates/Tryptophan_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25101 2022-04-15 19:27:42.000000 raichu-1.0.1/interactive/images/nrps_substrates/Tyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24311 2022-04-15 19:27:56.000000 raichu-1.0.1/interactive/images/nrps_substrates/Tyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16390 2022-04-15 19:32:05.000000 raichu-1.0.1/interactive/images/nrps_substrates/Valine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16071 2022-04-15 19:32:22.000000 raichu-1.0.1/interactive/images/nrps_substrates/Valine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/interactive/images/nrps_substrates/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    21812 2022-04-15 19:06:24.000000 raichu-1.0.1/interactive/images/nrps_substrates/allo-Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22026 2022-04-15 19:06:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19013 2022-04-15 19:24:37.000000 raichu-1.0.1/interactive/images/nrps_substrates/allo-Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17084 2022-04-15 19:24:50.000000 raichu-1.0.1/interactive/images/nrps_substrates/allo-Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34193 2022-04-15 19:14:24.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33802 2022-04-15 19:14:43.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20539 2022-04-15 19:38:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-ethylnorvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21837 2022-04-15 19:38:50.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25078 2022-04-15 18:04:22.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25232 2022-04-15 18:04:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21753 2022-04-15 18:03:44.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19502 2022-04-15 18:04:10.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23125 2022-04-15 18:58:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-methylcysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21614 2022-04-15 18:58:56.000000 raichu-1.0.1/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18232 2022-04-15 18:48:23.000000 raichu-1.0.1/interactive/images/nrps_substrates/beta-Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17866 2022-04-15 18:48:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/beta-Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22745 2022-04-15 19:10:12.000000 raichu-1.0.1/interactive/images/nrps_substrates/beta-lysine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22631 2022-04-15 19:10:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/beta-lysine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27655 2022-04-15 19:57:20.000000 raichu-1.0.1/interactive/images/nrps_substrates/capreomycidine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27032 2022-04-15 19:57:47.000000 raichu-1.0.1/interactive/images/nrps_substrates/capreomycidine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23007 2022-04-15 19:44:40.000000 raichu-1.0.1/interactive/images/nrps_substrates/coronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22918 2022-04-15 19:44:54.000000 raichu-1.0.1/interactive/images/nrps_substrates/coronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20766 2022-04-15 17:58:50.000000 raichu-1.0.1/interactive/images/nrps_substrates/cycloOrnithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20540 2022-04-15 17:59:07.000000 raichu-1.0.1/interactive/images/nrps_substrates/cycloOrnithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28850 2022-04-15 18:58:10.000000 raichu-1.0.1/interactive/images/nrps_substrates/cysteicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29414 2022-04-15 18:58:28.000000 raichu-1.0.1/interactive/images/nrps_substrates/cysteicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22320 2022-04-15 18:55:32.000000 raichu-1.0.1/interactive/images/nrps_substrates/dehydro-cysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22028 2022-04-15 18:55:49.000000 raichu-1.0.1/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20723 2022-04-15 18:47:18.000000 raichu-1.0.1/interactive/images/nrps_substrates/dehydroalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20497 2022-04-15 18:47:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/dehydroalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24909 2022-04-15 19:28:37.000000 raichu-1.0.1/interactive/images/nrps_substrates/dehydrotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24347 2022-04-15 19:28:51.000000 raichu-1.0.1/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    32343 2022-04-15 17:07:03.000000 raichu-1.0.1/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31754 2022-04-15 17:07:23.000000 raichu-1.0.1/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27766 2022-04-15 19:52:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/enduracididine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27194 2022-04-15 19:52:40.000000 raichu-1.0.1/interactive/images/nrps_substrates/enduracididine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23358 2022-04-15 18:50:34.000000 raichu-1.0.1/interactive/images/nrps_substrates/homoarginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24247 2022-04-15 18:50:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/homoarginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23746 2022-04-15 19:05:09.000000 raichu-1.0.1/interactive/images/nrps_substrates/homoisoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23630 2022-04-15 19:05:24.000000 raichu-1.0.1/interactive/images/nrps_substrates/homoisoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22096 2022-04-15 17:57:02.000000 raichu-1.0.1/interactive/images/nrps_substrates/homoserinelactone.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21719 2022-04-15 17:57:34.000000 raichu-1.0.1/interactive/images/nrps_substrates/homoserinelactone_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26982 2022-04-15 17:06:27.000000 raichu-1.0.1/interactive/images/nrps_substrates/hydrocinnamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25601 2022-04-15 17:06:44.000000 raichu-1.0.1/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26043 2022-04-15 17:05:53.000000 raichu-1.0.1/interactive/images/nrps_substrates/hydroxypicolinicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25858 2022-04-15 17:06:13.000000 raichu-1.0.1/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21960 2022-04-15 19:33:08.000000 raichu-1.0.1/interactive/images/nrps_substrates/isovaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21200 2022-04-15 19:33:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/isovaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26809 2022-04-15 19:53:26.000000 raichu-1.0.1/interactive/images/nrps_substrates/kynurenine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26107 2022-04-15 19:53:41.000000 raichu-1.0.1/interactive/images/nrps_substrates/kynurenine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24972 2022-04-15 17:54:33.000000 raichu-1.0.1/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26606 2022-04-15 17:54:50.000000 raichu-1.0.1/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21926 2022-04-15 19:44:05.000000 raichu-1.0.1/interactive/images/nrps_substrates/norcoronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20749 2022-04-15 19:44:27.000000 raichu-1.0.1/interactive/images/nrps_substrates/norcoronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18052 2022-04-15 18:08:44.000000 raichu-1.0.1/interactive/images/nrps_substrates/nrp.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17895 2022-04-15 18:09:02.000000 raichu-1.0.1/interactive/images/nrps_substrates/nrp_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25531 2022-04-15 17:05:15.000000 raichu-1.0.1/interactive/images/nrps_substrates/phenylaceticacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25533 2022-04-15 17:05:36.000000 raichu-1.0.1/interactive/images/nrps_substrates/phenylaceticacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26331 2022-04-15 20:00:39.000000 raichu-1.0.1/interactive/images/nrps_substrates/phenylglycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26106 2022-04-15 20:00:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/phenylglycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27784 2022-04-15 19:56:30.000000 raichu-1.0.1/interactive/images/nrps_substrates/phosphinothricin.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27870 2022-04-15 19:56:42.000000 raichu-1.0.1/interactive/images/nrps_substrates/phosphinothricin_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24381 2022-04-15 16:53:14.000000 raichu-1.0.1/interactive/images/nrps_substrates/salicylicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23788 2022-04-15 17:51:37.000000 raichu-1.0.1/interactive/images/nrps_substrates/salicylicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21002 2022-04-15 19:06:59.000000 raichu-1.0.1/interactive/images/nrps_substrates/tert-Leu.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20891 2022-04-15 19:07:24.000000 raichu-1.0.1/interactive/images/nrps_substrates/tert-Leu_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16198 2022-04-15 18:01:40.000000 raichu-1.0.1/interactive/images/nrps_substrates/valinol.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16320 2022-04-15 18:01:54.000000 raichu-1.0.1/interactive/images/nrps_substrates/valinol_highlight.png
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.679104 raichu-1.0.1/interactive/images/pks_starter_substrates/
+-rw-r--r--   0 barbara    (501) staff       (20)    29850 2022-05-01 12:06:56.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2R-hMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26673 2022-05-01 12:07:06.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2R-hMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25251 2022-05-01 12:06:33.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2R-mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23606 2022-05-01 12:06:48.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2R-mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33676 2022-05-01 12:06:14.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2S-hMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33230 2022-05-01 12:06:24.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2S-hMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26972 2022-05-01 12:05:48.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2S-mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26664 2022-05-01 12:06:03.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2S-mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24670 2022-05-01 12:07:17.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24923 2022-05-01 12:07:25.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/2mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25417 2022-05-01 12:05:22.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/3mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25187 2022-05-01 12:05:39.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/3mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20866 2022-05-01 12:05:03.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/Ac.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21010 2022-05-01 12:05:13.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/Ac_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25026 2022-05-01 12:04:44.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/Benz.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25713 2022-05-01 12:04:54.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/Benz_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34080 2022-05-01 12:04:21.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/CHC.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33079 2022-05-01 12:04:32.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/CHC_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21110 2022-05-01 12:03:36.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/Prop.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20850 2022-05-01 12:03:52.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/Prop_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    32496 2022-05-01 12:40:12.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/ceMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31629 2022-05-01 12:40:20.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/ceMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29134 2022-05-01 12:04:02.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/hMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28542 2022-05-01 12:04:10.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/hMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22191 2022-05-01 16:48:04.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/isoBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21953 2022-05-01 16:48:17.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/isoBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41464 2022-05-01 12:03:11.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/tCPDA.png
+-rw-r--r--   0 barbara    (501) staff       (20)    40950 2022-05-01 12:03:25.000000 raichu-1.0.1/interactive/images/pks_starter_substrates/tCPDA_highlight.png
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.684573 raichu-1.0.1/interactive/images/pks_substrates/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/interactive/images/pks_substrates/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    24949 2022-04-16 08:01:15.000000 raichu-1.0.1/interactive/images/pks_substrates/ethylmalonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25556 2022-04-16 08:01:32.000000 raichu-1.0.1/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24099 2022-04-16 07:57:17.000000 raichu-1.0.1/interactive/images/pks_substrates/malonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23782 2022-04-16 07:59:21.000000 raichu-1.0.1/interactive/images/pks_substrates/malonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28684 2022-04-16 08:02:38.000000 raichu-1.0.1/interactive/images/pks_substrates/methoxymalonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28317 2022-04-16 08:02:54.000000 raichu-1.0.1/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25513 2022-04-16 07:58:33.000000 raichu-1.0.1/interactive/images/pks_substrates/methylmalonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25625 2022-04-16 07:58:50.000000 raichu-1.0.1/interactive/images/pks_substrates/methylmalonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21959 2022-04-16 08:04:06.000000 raichu-1.0.1/interactive/images/pks_substrates/wildcard.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22218 2022-04-16 08:04:28.000000 raichu-1.0.1/interactive/images/pks_substrates/wildcard_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)      913 2022-04-14 09:57:57.000000 raichu-1.0.1/interactive/insertion_point.py
+-rw-r--r--   0 barbara    (501) staff       (20)    11853 2022-05-02 15:50:16.000000 raichu-1.0.1/interactive/load_antismash.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4136 2022-05-02 13:04:31.000000 raichu-1.0.1/interactive/load_tabular.py
+-rw-r--r--   0 barbara    (501) staff       (20)     3769 2022-04-19 13:35:36.000000 raichu-1.0.1/interactive/module.py
+-rw-r--r--   0 barbara    (501) staff       (20)      306 2022-04-15 16:35:29.000000 raichu-1.0.1/interactive/parsers.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5462 2022-10-24 15:18:24.000000 raichu-1.0.1/interactive/render_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    27124 2022-05-05 14:52:33.000000 raichu-1.0.1/interactive/run_raichu.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2083 2022-05-05 14:48:17.000000 raichu-1.0.1/interactive/style.py
+-rw-r--r--   0 barbara    (501) staff       (20)    18130 2022-05-08 06:33:46.000000 raichu-1.0.1/interactive/substrate.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1117 2022-04-14 09:00:39.000000 raichu-1.0.1/interactive/textbox.py
+-rw-r--r--   0 barbara    (501) staff       (20)       89 2021-09-16 23:05:31.000000 raichu-1.0.1/pyproject.toml
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.689069 raichu-1.0.1/raichu/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.1/raichu/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     3656 2024-02-08 09:09:32.000000 raichu-1.0.1/raichu/alkaloid.py
+-rw-r--r--   0 barbara    (501) staff       (20)    37295 2024-04-15 15:44:13.000000 raichu-1.0.1/raichu/antismash.py
+-rw-r--r--   0 barbara    (501) staff       (20)    11162 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/attach_to_domain.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.690620 raichu-1.0.1/raichu/central_chain_detection/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/central_chain_detection/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     9199 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/central_chain_detection/find_central_chain.py
+-rw-r--r--   0 barbara    (501) staff       (20)    19314 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/central_chain_detection/label_central_chain.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4124 2023-05-01 07:37:35.000000 raichu-1.0.1/raichu/class_domain.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.692520 raichu-1.0.1/raichu/cluster/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2023-05-07 08:18:53.000000 raichu-1.0.1/raichu/cluster/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)      736 2023-05-07 08:52:51.000000 raichu-1.0.1/raichu/cluster/alkaloid_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    16380 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/cluster/base_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    15618 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/cluster/modular_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    16428 2023-05-07 17:50:23.000000 raichu-1.0.1/raichu/cluster/ripp_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5799 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/cluster/terpene_cluster.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.694860 raichu-1.0.1/raichu/data/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/data/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)      137 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/data/at_elongation_specificities.txt
+-rw-r--r--   0 barbara    (501) staff       (20)      269 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/data/at_specificities.txt
+-rw-r--r--   0 barbara    (501) staff       (20)     4969 2023-12-08 12:52:08.000000 raichu-1.0.1/raichu/data/attributes.py
+-rw-r--r--   0 barbara    (501) staff       (20)    20943 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/data/metadata.txt
+-rw-r--r--   0 barbara    (501) staff       (20)    10888 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/data/molecular_moieties.py
+-rw-r--r--   0 barbara    (501) staff       (20)    14079 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/data/smiles.txt
+-rw-r--r--   0 barbara    (501) staff       (20)     3834 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/data/substrate_to_abbreviation.txt
+-rw-r--r--   0 barbara    (501) staff       (20)     9683 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/data/trans_at.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.695659 raichu-1.0.1/raichu/domain/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/domain/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    10455 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/domain/domain.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5614 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/domain/domain_types.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.697780 raichu-1.0.1/raichu/drawing/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/drawing/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     9301 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/drawing/bubbles.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5636 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/drawing/colours.py
+-rw-r--r--   0 barbara    (501) staff       (20)    83982 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/drawing/drawer.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1613 2023-05-07 18:03:32.000000 raichu-1.0.1/raichu/drawing/pathway.py
+-rw-r--r--   0 barbara    (501) staff       (20)      678 2023-05-07 08:52:51.000000 raichu-1.0.1/raichu/drawing/ripp_drawing.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5734 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/general.py
+-rw-r--r--   0 barbara    (501) staff       (20)    25860 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/module.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.700102 raichu-1.0.1/raichu/reactions/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.1/raichu/reactions/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    12341 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/reactions/chain_release.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1001 2024-02-08 15:43:23.000000 raichu-1.0.1/raichu/reactions/general.py
+-rw-r--r--   0 barbara    (501) staff       (20)    19163 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/reactions/general_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4530 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/reactions/nrps_elongation_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5632 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/reactions/nrps_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4658 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/reactions/pks_elongation_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1125 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/reactions/pks_sidechain_chirality.py
+-rw-r--r--   0 barbara    (501) staff       (20)    34020 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/reactions/pks_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2403 2023-05-01 07:37:35.000000 raichu-1.0.1/raichu/reactions/ripp_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     6737 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/representations.py
+-rw-r--r--   0 barbara    (501) staff       (20)    21201 2024-02-08 09:09:32.000000 raichu-1.0.1/raichu/ripp.py
+-rw-r--r--   0 barbara    (501) staff       (20)    38926 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/run_raichu.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2806 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/smiles_handling.py
+-rw-r--r--   0 barbara    (501) staff       (20)     6667 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/substrate.py
+-rw-r--r--   0 barbara    (501) staff       (20)    32389 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/tailoring_enzymes.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.700477 raichu-1.0.1/raichu/test/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/test/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     9670 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/test/generate_test_data.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.700691 raichu-1.0.1/raichu/test/test_data/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/test/test_data/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.700813 raichu-1.0.1/raichu/test/unit/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/test/unit/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.701191 raichu-1.0.1/raichu/test/unit/reactions/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/test/unit/reactions/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/test/unit/reactions/test_general_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)      416 2024-04-15 15:19:04.000000 raichu-1.0.1/raichu/test/unit/reactions/test_nrps_tailoring_reactions.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:59:57.701519 raichu-1.0.1/raichu.egg-info/
+-rw-r--r--   0 barbara    (501) staff       (20)      322 2024-04-15 15:59:57.000000 raichu-1.0.1/raichu.egg-info/PKG-INFO
+-rw-r--r--   0 barbara    (501) staff       (20)    25323 2024-04-15 15:59:57.000000 raichu-1.0.1/raichu.egg-info/SOURCES.txt
+-rw-r--r--   0 barbara    (501) staff       (20)        1 2024-04-15 15:59:57.000000 raichu-1.0.1/raichu.egg-info/dependency_links.txt
+-rw-r--r--   0 barbara    (501) staff       (20)       47 2024-04-15 15:59:57.000000 raichu-1.0.1/raichu.egg-info/requires.txt
+-rw-r--r--   0 barbara    (501) staff       (20)       19 2024-04-15 15:59:57.000000 raichu-1.0.1/raichu.egg-info/top_level.txt
+-rw-r--r--   0 barbara    (501) staff       (20)       38 2024-04-15 15:59:57.702328 raichu-1.0.1/setup.cfg
+-rw-r--r--   0 barbara    (501) staff       (20)      650 2024-04-15 15:59:45.000000 raichu-1.0.1/setup.py
```

### Comparing `raichu-1.0.0/LICENSE.txt` & `raichu-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/README.md` & `raichu-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/bin/raichu` & `raichu-1.0.1/bin/raichu`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/background.py` & `raichu-1.0.1/interactive/background.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/buttons.py` & `raichu-1.0.1/interactive/buttons.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/domain.py` & `raichu-1.0.1/interactive/domain.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/gene.py` & `raichu-1.0.1/interactive/gene.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/a.png` & `raichu-1.0.1/interactive/images/domains/a.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/a_highlight.png` & `raichu-1.0.1/interactive/images/domains/a_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/acp.png` & `raichu-1.0.1/interactive/images/domains/acp.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/acp_highlight.png` & `raichu-1.0.1/interactive/images/domains/acp_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/at.png` & `raichu-1.0.1/interactive/images/domains/at.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/at_highlight.png` & `raichu-1.0.1/interactive/images/domains/at_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/c.png` & `raichu-1.0.1/interactive/images/domains/c.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/c_highlight.png` & `raichu-1.0.1/interactive/images/domains/c_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/dh.png` & `raichu-1.0.1/interactive/images/domains/dh.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/dh_highlight.png` & `raichu-1.0.1/interactive/images/domains/dh_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/e.png` & `raichu-1.0.1/interactive/images/domains/e.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/e_highlight.png` & `raichu-1.0.1/interactive/images/domains/e_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/er.png` & `raichu-1.0.1/interactive/images/domains/er.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/er_highlight.png` & `raichu-1.0.1/interactive/images/domains/er_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/kr.png` & `raichu-1.0.1/interactive/images/domains/kr.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/kr_highlight.png` & `raichu-1.0.1/interactive/images/domains/kr_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/ks.png` & `raichu-1.0.1/interactive/images/domains/ks.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/ks_highlight.png` & `raichu-1.0.1/interactive/images/domains/ks_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/nmt.png` & `raichu-1.0.1/interactive/images/domains/nmt.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/nmt_highlight.png` & `raichu-1.0.1/interactive/images/domains/nmt_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/pcp.png` & `raichu-1.0.1/interactive/images/domains/pcp.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/pcp_highlight.png` & `raichu-1.0.1/interactive/images/domains/pcp_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/te.png` & `raichu-1.0.1/interactive/images/domains/te.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/domains/te_highlight.png` & `raichu-1.0.1/interactive/images/domains/te_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/icon.png` & `raichu-1.0.1/interactive/images/icon.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_A1.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_A1.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_A1_highlight.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_A1_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_A2.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_A2.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_A2_highlight.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_A2_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_B1.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_B1.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_B1_highlight.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_B1_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_B2.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_B2.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_B2_highlight.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_B2_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_C1.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_C1.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_C1_highlight.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_C1_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_C2.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_C2.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_C2_highlight.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_C2_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/kr_subtypes/KR_highlight.png` & `raichu-1.0.1/interactive/images/kr_subtypes/KR_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(R)beta-tyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoadipicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Aminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Methylserine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-Methylserine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-carboxyquinoxaline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-hydroxyisovalerate.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-methyl-beta-alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-aminopropanimidamide.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxyglutamine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-methyltyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4,5-dehydroarginine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-methylglutamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-methylproline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/4-methylproline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Alanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Alanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Alaninol.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Alaninol.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Alaninol_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Alaninol_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Anticapsin.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Anticapsin_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Arginine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Arginine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Arginine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Arginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Asparagine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Asparagine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Asparagine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Asparagine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/AsparticAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/AsparticAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Citrulline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Citrulline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Citrulline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Citrulline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Cysteine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Cysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Cysteine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Cysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Arginine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Arginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Asparagine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Asparagine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-AsparticAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Citrulline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Citrulline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Cysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Cysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-GlutamicAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Glutamine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Glutamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Histidine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Histidine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Homoserine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Homoserine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Homotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Leucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Leucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Lysine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Lysine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Methionine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Methionine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-PhenylGlycine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Phenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Pipecolicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Proline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Proline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Proline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Proline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Serine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Serine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Serine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Serine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Tryptophan.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Tryptophan_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Tyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Tyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Valine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Valine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-Valine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-Valine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-methylcysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-cycloOrnithine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-cysteicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-cysteicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-enduracididine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-enduracididine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-homoserinelactone.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-isovaline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-isovaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-kynurenine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-kynurenine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-lysergicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-lysergicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-ornithine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-ornithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-phosphinothricin.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-tert-Leucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Dehydrobutyrine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/GlutamicAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/GlutamicAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glutamine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glutamine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glutamine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glutamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glycine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glycine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glycine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glycocyamine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glycocyamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glycolicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Glycolicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Histidine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Histidine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Histidine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Histidine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Homophenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Homophenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Homoserine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Homoserine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Homoserine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Homoserine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Homotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Homotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/L-piperazicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/L-piperazicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Leucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Leucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Leucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Leucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Lysine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Lysine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Lysine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Lysine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Methionine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Methionine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Methionine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Methionine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/N-acetylphenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Norvaline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Norvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Norvaline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Norvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Ornithine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Ornithine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Ornithine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Ornithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Phenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Phenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Pipecolicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Pipecolicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Proline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Proline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Proline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Proline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/R-coronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/R-coronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/R-norcoronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Serine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Serine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Serine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Serine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Threonine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Threonine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Tryptophan.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Tryptophan_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Tyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Tyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Valine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Valine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/Valine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/Valine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/allo-Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/allo-Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/allo-Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-ethylnorvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-methylcysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/beta-Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/beta-Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/beta-lysine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/beta-lysine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/capreomycidine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/capreomycidine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/coronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/coronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/cycloOrnithine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/cycloOrnithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/cysteicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/cysteicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dehydro-cysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dehydroalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dehydroalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dehydrotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/enduracididine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/enduracididine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/enduracididine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/enduracididine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/homoarginine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/homoarginine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/homoarginine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/homoarginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/homoisoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/homoisoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone.png` & `raichu-1.0.1/interactive/images/nrps_substrates/homoserinelactone.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/homoserinelactone_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/hydrocinnamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/hydroxypicolinicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/isovaline.png` & `raichu-1.0.1/interactive/images/nrps_substrates/isovaline.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/isovaline_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/isovaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/kynurenine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/kynurenine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/kynurenine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/kynurenine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/norcoronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/norcoronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/nrp.png` & `raichu-1.0.1/interactive/images/nrps_substrates/nrp.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/nrp_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/nrp_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/phenylaceticacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/phenylaceticacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine.png` & `raichu-1.0.1/interactive/images/nrps_substrates/phenylglycine.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/phenylglycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin.png` & `raichu-1.0.1/interactive/images/nrps_substrates/phosphinothricin.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/phosphinothricin_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid.png` & `raichu-1.0.1/interactive/images/nrps_substrates/salicylicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/salicylicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu.png` & `raichu-1.0.1/interactive/images/nrps_substrates/tert-Leu.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/tert-Leu_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/valinol.png` & `raichu-1.0.1/interactive/images/nrps_substrates/valinol.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/nrps_substrates/valinol_highlight.png` & `raichu-1.0.1/interactive/images/nrps_substrates/valinol_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2R-hMal.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2R-hMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2R-mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2R-mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2S-hMal.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2S-hMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2S-mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2S-mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/2mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/3mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/3mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/Ac.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/Ac.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/Ac_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/Ac_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/Benz.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/Benz.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/Benz_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/Benz_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/CHC.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/CHC.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/CHC_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/CHC_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/Prop.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/Prop.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/Prop_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/Prop_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/ceMal.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/ceMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/hMal.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/hMal.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/hMal_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/hMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/isoBut.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/isoBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/tCPDA.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA_highlight.png` & `raichu-1.0.1/interactive/images/pks_starter_substrates/tCPDA_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa.png` & `raichu-1.0.1/interactive/images/pks_substrates/ethylmalonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png` & `raichu-1.0.1/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/malonylcoa.png` & `raichu-1.0.1/interactive/images/pks_substrates/malonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/malonylcoa_highlight.png` & `raichu-1.0.1/interactive/images/pks_substrates/malonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa.png` & `raichu-1.0.1/interactive/images/pks_substrates/methoxymalonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png` & `raichu-1.0.1/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa.png` & `raichu-1.0.1/interactive/images/pks_substrates/methylmalonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa_highlight.png` & `raichu-1.0.1/interactive/images/pks_substrates/methylmalonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/wildcard.png` & `raichu-1.0.1/interactive/images/pks_substrates/wildcard.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/images/pks_substrates/wildcard_highlight.png` & `raichu-1.0.1/interactive/images/pks_substrates/wildcard_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/insertion_point.py` & `raichu-1.0.1/interactive/insertion_point.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/load_antismash.py` & `raichu-1.0.1/interactive/load_antismash.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/load_tabular.py` & `raichu-1.0.1/interactive/load_tabular.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/module.py` & `raichu-1.0.1/interactive/module.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/render_cluster.py` & `raichu-1.0.1/interactive/render_cluster.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/run_raichu.py` & `raichu-1.0.1/interactive/run_raichu.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/style.py` & `raichu-1.0.1/interactive/style.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/substrate.py` & `raichu-1.0.1/interactive/substrate.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/interactive/textbox.py` & `raichu-1.0.1/interactive/textbox.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/alkaloid.py` & `raichu-1.0.1/raichu/alkaloid.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/antismash.py` & `raichu-1.0.1/raichu/antismash.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/attach_to_domain.py` & `raichu-1.0.1/raichu/attach_to_domain.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/central_chain_detection/find_central_chain.py` & `raichu-1.0.1/raichu/central_chain_detection/find_central_chain.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/central_chain_detection/label_central_chain.py` & `raichu-1.0.1/raichu/central_chain_detection/label_central_chain.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/class_domain.py` & `raichu-1.0.1/raichu/class_domain.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/cluster/alkaloid_cluster.py` & `raichu-1.0.1/raichu/cluster/alkaloid_cluster.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/cluster/base_cluster.py` & `raichu-1.0.1/raichu/cluster/base_cluster.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/cluster/modular_cluster.py` & `raichu-1.0.1/raichu/cluster/modular_cluster.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/cluster/ripp_cluster.py` & `raichu-1.0.1/raichu/cluster/ripp_cluster.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/cluster/terpene_cluster.py` & `raichu-1.0.1/raichu/cluster/terpene_cluster.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/data/attributes.py` & `raichu-1.0.1/raichu/data/attributes.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/data/metadata.txt` & `raichu-1.0.1/raichu/data/metadata.txt`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/data/molecular_moieties.py` & `raichu-1.0.1/raichu/data/molecular_moieties.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/data/smiles.txt` & `raichu-1.0.1/raichu/data/smiles.txt`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/data/substrate_to_abbreviation.txt` & `raichu-1.0.1/raichu/data/substrate_to_abbreviation.txt`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/data/trans_at.py` & `raichu-1.0.1/raichu/data/trans_at.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/domain/domain.py` & `raichu-1.0.1/raichu/domain/domain.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/domain/domain_types.py` & `raichu-1.0.1/raichu/domain/domain_types.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/drawing/bubbles.py` & `raichu-1.0.1/raichu/drawing/bubbles.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/drawing/colours.py` & `raichu-1.0.1/raichu/drawing/colours.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/drawing/drawer.py` & `raichu-1.0.1/raichu/drawing/drawer.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/drawing/pathway.py` & `raichu-1.0.1/raichu/drawing/pathway.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/drawing/ripp_drawing.py` & `raichu-1.0.1/raichu/drawing/ripp_drawing.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/general.py` & `raichu-1.0.1/raichu/general.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/module.py` & `raichu-1.0.1/raichu/module.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/chain_release.py` & `raichu-1.0.1/raichu/reactions/chain_release.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/general.py` & `raichu-1.0.1/raichu/reactions/general.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/general_tailoring_reactions.py` & `raichu-1.0.1/raichu/reactions/general_tailoring_reactions.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/nrps_elongation_reactions.py` & `raichu-1.0.1/raichu/reactions/nrps_elongation_reactions.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/nrps_tailoring_reactions.py` & `raichu-1.0.1/raichu/reactions/nrps_tailoring_reactions.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/pks_elongation_reactions.py` & `raichu-1.0.1/raichu/reactions/pks_elongation_reactions.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/pks_sidechain_chirality.py` & `raichu-1.0.1/raichu/reactions/pks_sidechain_chirality.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/pks_tailoring_reactions.py` & `raichu-1.0.1/raichu/reactions/pks_tailoring_reactions.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/reactions/ripp_reactions.py` & `raichu-1.0.1/raichu/reactions/ripp_reactions.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/representations.py` & `raichu-1.0.1/raichu/representations.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/ripp.py` & `raichu-1.0.1/raichu/ripp.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/run_raichu.py` & `raichu-1.0.1/raichu/run_raichu.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/smiles_handling.py` & `raichu-1.0.1/raichu/smiles_handling.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/substrate.py` & `raichu-1.0.1/raichu/substrate.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/tailoring_enzymes.py` & `raichu-1.0.1/raichu/tailoring_enzymes.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu/test/generate_test_data.py` & `raichu-1.0.1/raichu/test/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/raichu.egg-info/SOURCES.txt` & `raichu-1.0.1/raichu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raichu-1.0.0/setup.py` & `raichu-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'RAIChU'
 LONG_DESCRIPTION = 'A package to automatically draw natural product biosynthesis pathways.'
 
 print(find_packages())
 
 setup(
     name="raichu",
@@ -13,10 +13,10 @@
     author="Barbara Terlouw",
     author_email="barbara.r.terlouw@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(exclude="build"),
     package_data={"": ["*.png", "*.svg", "*.txt"]},
     install_requires=['matplotlib',
-                      'biopython==1.76',
+                      'biopython>=1.76',
                       'pikachu-chem>=1.1.1'],
     scripts=["bin/raichu"],)
```

