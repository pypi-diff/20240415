# Comparing `tmp/raichu-0.0.2.tar.gz` & `tmp/raichu-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raichu-0.0.2.tar", last modified: Tue Nov  1 13:10:55 2022, max compression
+gzip compressed data, was "raichu-1.0.0.tar", last modified: Mon Apr 15 15:52:56 2024, max compression
```

## Comparing `raichu-0.0.2.tar` & `raichu-1.0.0.tar`

### file list

```diff
@@ -1,464 +1,494 @@
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.444871 raichu-0.0.2/
--rw-r--r--   0 barbara    (501) staff       (20)      169 2022-11-01 13:10:55.444687 raichu-0.0.2/PKG-INFO
--rw-r--r--   0 barbara    (501) staff       (20)      203 2022-04-07 11:54:31.000000 raichu-0.0.2/README.md
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.291454 raichu-0.0.2/bin/
--rw-r--r--   0 barbara    (501) staff       (20)     3137 2022-05-02 12:36:20.000000 raichu-0.0.2/bin/raichu
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.295844 raichu-0.0.2/interactive/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/interactive/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     1655 2022-04-17 16:18:30.000000 raichu-0.0.2/interactive/background.py
--rw-r--r--   0 barbara    (501) staff       (20)    38866 2022-05-01 17:29:00.000000 raichu-0.0.2/interactive/buttons.py
--rw-r--r--   0 barbara    (501) staff       (20)     2595 2022-05-01 12:51:17.000000 raichu-0.0.2/interactive/domain.py
--rw-r--r--   0 barbara    (501) staff       (20)     4354 2022-05-02 15:38:29.000000 raichu-0.0.2/interactive/gene.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.296171 raichu-0.0.2/interactive/images/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/interactive/images/__init__.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.303132 raichu-0.0.2/interactive/images/domains/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/interactive/images/domains/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    13363 2022-04-13 17:02:54.000000 raichu-0.0.2/interactive/images/domains/a.png
--rw-r--r--   0 barbara    (501) staff       (20)    13470 2022-04-14 07:32:59.000000 raichu-0.0.2/interactive/images/domains/a_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17374 2022-04-13 17:02:35.000000 raichu-0.0.2/interactive/images/domains/acp.png
--rw-r--r--   0 barbara    (501) staff       (20)    17372 2022-04-14 07:32:26.000000 raichu-0.0.2/interactive/images/domains/acp_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13468 2022-04-13 17:04:13.000000 raichu-0.0.2/interactive/images/domains/at.png
--rw-r--r--   0 barbara    (501) staff       (20)    13414 2022-04-14 07:35:16.000000 raichu-0.0.2/interactive/images/domains/at_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14370 2022-04-13 17:03:11.000000 raichu-0.0.2/interactive/images/domains/c.png
--rw-r--r--   0 barbara    (501) staff       (20)    14334 2022-04-14 07:33:37.000000 raichu-0.0.2/interactive/images/domains/c_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13271 2022-04-13 17:05:03.000000 raichu-0.0.2/interactive/images/domains/dh.png
--rw-r--r--   0 barbara    (501) staff       (20)    13201 2022-04-14 07:36:35.000000 raichu-0.0.2/interactive/images/domains/dh_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    11416 2022-04-13 17:03:29.000000 raichu-0.0.2/interactive/images/domains/e.png
--rw-r--r--   0 barbara    (501) staff       (20)    11408 2022-04-14 07:34:15.000000 raichu-0.0.2/interactive/images/domains/e_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13101 2022-04-13 17:05:18.000000 raichu-0.0.2/interactive/images/domains/er.png
--rw-r--r--   0 barbara    (501) staff       (20)    13218 2022-04-14 07:37:04.000000 raichu-0.0.2/interactive/images/domains/er_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14279 2022-04-13 17:04:47.000000 raichu-0.0.2/interactive/images/domains/kr.png
--rw-r--r--   0 barbara    (501) staff       (20)    14317 2022-04-14 07:36:07.000000 raichu-0.0.2/interactive/images/domains/kr_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16398 2022-04-13 17:04:28.000000 raichu-0.0.2/interactive/images/domains/ks.png
--rw-r--r--   0 barbara    (501) staff       (20)    16402 2022-04-14 07:35:43.000000 raichu-0.0.2/interactive/images/domains/ks_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13835 2022-04-13 17:05:36.000000 raichu-0.0.2/interactive/images/domains/nmt.png
--rw-r--r--   0 barbara    (501) staff       (20)    13911 2022-04-14 07:37:51.000000 raichu-0.0.2/interactive/images/domains/nmt_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-13 17:02:14.000000 raichu-0.0.2/interactive/images/domains/pcp.png
--rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-14 07:32:16.000000 raichu-0.0.2/interactive/images/domains/pcp_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    11757 2022-04-13 17:03:45.000000 raichu-0.0.2/interactive/images/domains/te.png
--rw-r--r--   0 barbara    (501) staff       (20)    11784 2022-04-14 07:34:50.000000 raichu-0.0.2/interactive/images/domains/te_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34945 2022-04-14 08:27:48.000000 raichu-0.0.2/interactive/images/icon.png
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.306779 raichu-0.0.2/interactive/images/kr_subtypes/
--rw-r--r--   0 barbara    (501) staff       (20)     6853 2022-04-16 14:37:34.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR.png
--rw-r--r--   0 barbara    (501) staff       (20)    10255 2022-04-16 14:40:44.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_A1.png
--rw-r--r--   0 barbara    (501) staff       (20)    10233 2022-04-16 14:40:58.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_A1_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14129 2022-04-16 14:40:22.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_A2.png
--rw-r--r--   0 barbara    (501) staff       (20)    13940 2022-04-16 14:40:36.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_A2_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)     9104 2022-04-16 14:39:53.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_B1.png
--rw-r--r--   0 barbara    (501) staff       (20)     9076 2022-04-16 14:40:07.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_B1_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    12935 2022-04-16 14:39:32.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_B2.png
--rw-r--r--   0 barbara    (501) staff       (20)    12803 2022-04-16 14:39:45.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_B2_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    11395 2022-04-16 14:39:06.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_C1.png
--rw-r--r--   0 barbara    (501) staff       (20)    11318 2022-04-16 14:39:21.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_C1_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    14939 2022-04-16 14:38:43.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_C2.png
--rw-r--r--   0 barbara    (501) staff       (20)    14756 2022-04-16 14:38:56.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_C2_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)     6819 2022-04-16 14:38:16.000000 raichu-0.0.2/interactive/images/kr_subtypes/KR_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/interactive/images/kr_subtypes/__init__.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.421851 raichu-0.0.2/interactive/images/nrps_substrates/
--rw-r--r--   0 barbara    (501) staff       (20)    29614 2022-04-15 19:51:37.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    29531 2022-04-15 19:51:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29732 2022-04-15 19:50:40.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    30295 2022-04-15 19:50:55.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    42828 2022-04-15 19:59:58.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png
--rw-r--r--   0 barbara    (501) staff       (20)    40729 2022-04-15 20:00:18.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:51:06.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    30420 2022-04-15 19:51:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29315 2022-04-15 19:31:17.000000 raichu-0.0.2/interactive/images/nrps_substrates/(R)beta-tyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    29122 2022-04-15 19:31:33.000000 raichu-0.0.2/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34021 2022-04-15 19:27:06.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png
--rw-r--r--   0 barbara    (501) staff       (20)    31793 2022-04-15 19:27:22.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28970 2022-04-15 19:48:46.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    28787 2022-04-15 19:49:02.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27662 2022-04-15 17:47:25.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    30028 2022-04-15 17:47:47.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27300 2022-04-15 19:48:17.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    27047 2022-04-15 19:48:34.000000 raichu-0.0.2/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    41323 2022-04-15 17:53:10.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    40856 2022-04-15 17:53:29.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25318 2022-04-15 19:41:11.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoadipicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24974 2022-04-15 19:41:27.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:49:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Aminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23130 2022-04-15 19:50:28.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27411 2022-04-15 19:49:12.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    27276 2022-04-15 19:49:28.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23030 2022-04-15 19:22:32.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Methylserine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22312 2022-04-15 19:22:46.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-Methylserine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30762 2022-04-15 17:48:14.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-carboxyquinoxaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    29202 2022-04-15 17:48:52.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21732 2022-04-15 18:06:09.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-hydroxyisovalerate.png
--rw-r--r--   0 barbara    (501) staff       (20)    22544 2022-04-15 18:06:25.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21505 2022-04-15 18:49:40.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-methyl-beta-alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21077 2022-04-15 18:49:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    36652 2022-04-15 20:03:20.000000 raichu-0.0.2/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    35330 2022-04-15 20:03:33.000000 raichu-0.0.2/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25798 2022-04-15 19:59:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23250 2022-04-15 19:59:46.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    36143 2022-04-15 19:58:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    35659 2022-04-15 19:59:13.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22618 2022-04-15 18:05:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-aminopropanimidamide.png
--rw-r--r--   0 barbara    (501) staff       (20)    22388 2022-04-15 18:05:57.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    39152 2022-04-15 19:30:48.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    38713 2022-04-15 19:31:04.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30192 2022-04-15 19:00:25.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxyglutamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    30391 2022-04-15 19:00:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31392 2022-04-15 19:30:19.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-methyltyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    30693 2022-04-15 19:30:35.000000 raichu-0.0.2/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    37365 2022-04-15 19:29:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    36877 2022-04-15 19:30:07.000000 raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27121 2022-04-15 19:55:37.000000 raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25672 2022-04-15 19:55:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31631 2022-04-15 18:52:08.000000 raichu-0.0.2/interactive/images/nrps_substrates/4,5-dehydroarginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    31245 2022-04-15 18:52:24.000000 raichu-0.0.2/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    38385 2022-04-15 17:46:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    35115 2022-04-15 17:47:09.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24864 2022-04-15 19:39:08.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    24656 2022-04-15 19:39:27.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28181 2022-04-15 19:25:04.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    28922 2022-04-15 19:25:19.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25868 2022-04-15 19:02:08.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-methylglutamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24839 2022-04-15 19:02:29.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24797 2022-04-15 19:18:33.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-methylproline.png
--rw-r--r--   0 barbara    (501) staff       (20)    24917 2022-04-15 19:18:49.000000 raichu-0.0.2/interactive/images/nrps_substrates/4-methylproline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16493 2022-04-15 18:48:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16392 2022-04-15 18:49:28.000000 raichu-0.0.2/interactive/images/nrps_substrates/Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    13602 2022-04-15 18:04:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/Alaninol.png
--rw-r--r--   0 barbara    (501) staff       (20)    13514 2022-04-15 18:05:22.000000 raichu-0.0.2/interactive/images/nrps_substrates/Alaninol_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24271 2022-04-15 19:58:29.000000 raichu-0.0.2/interactive/images/nrps_substrates/Anticapsin.png
--rw-r--r--   0 barbara    (501) staff       (20)    24821 2022-04-15 19:58:43.000000 raichu-0.0.2/interactive/images/nrps_substrates/Anticapsin_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23158 2022-04-15 18:51:35.000000 raichu-0.0.2/interactive/images/nrps_substrates/Arginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22351 2022-04-15 18:51:52.000000 raichu-0.0.2/interactive/images/nrps_substrates/Arginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21621 2022-04-15 18:53:20.000000 raichu-0.0.2/interactive/images/nrps_substrates/Asparagine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21080 2022-04-15 18:53:35.000000 raichu-0.0.2/interactive/images/nrps_substrates/Asparagine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23527 2022-04-15 18:54:54.000000 raichu-0.0.2/interactive/images/nrps_substrates/AsparticAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23278 2022-04-15 18:55:10.000000 raichu-0.0.2/interactive/images/nrps_substrates/AsparticAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    35623 2022-04-15 19:58:02.000000 raichu-0.0.2/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    35114 2022-04-15 19:58:20.000000 raichu-0.0.2/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19216 2022-04-15 19:42:23.000000 raichu-0.0.2/interactive/images/nrps_substrates/Citrulline.png
--rw-r--r--   0 barbara    (501) staff       (20)    20529 2022-04-15 19:42:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/Citrulline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17085 2022-04-15 18:57:37.000000 raichu-0.0.2/interactive/images/nrps_substrates/Cysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17879 2022-04-15 18:57:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/Cysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25588 2022-04-15 19:47:11.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25308 2022-04-15 19:47:22.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23524 2022-04-15 19:46:29.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25188 2022-04-15 19:46:49.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25783 2022-04-15 19:40:35.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24378 2022-04-15 19:40:56.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23608 2022-04-15 19:47:33.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23287 2022-04-15 19:47:50.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25855 2022-04-15 18:03:18.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png
--rw-r--r--   0 barbara    (501) staff       (20)    25575 2022-04-15 18:03:32.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    35436 2022-04-15 20:02:49.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    33762 2022-04-15 20:03:07.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    15814 2022-04-15 18:47:50.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16164 2022-04-15 18:48:05.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24190 2022-04-15 18:51:04.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Arginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23965 2022-04-15 18:51:24.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Arginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23867 2022-04-15 18:52:47.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Asparagine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22155 2022-04-15 18:53:06.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Asparagine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24591 2022-04-15 18:54:13.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-AsparticAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24267 2022-04-15 18:54:43.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21764 2022-04-15 19:41:54.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Citrulline.png
--rw-r--r--   0 barbara    (501) staff       (20)    21249 2022-04-15 19:42:12.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Citrulline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18606 2022-04-15 18:55:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Cysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16731 2022-04-15 18:56:20.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Cysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24393 2022-04-15 19:01:41.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-GlutamicAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    24049 2022-04-15 19:01:57.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23556 2022-04-15 18:59:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Glutamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22325 2022-04-15 19:00:07.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Glutamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25709 2022-04-15 19:04:01.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Histidine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25190 2022-04-15 19:04:17.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Histidine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21390 2022-04-15 19:21:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Homoserine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21180 2022-04-15 19:22:18.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Homoserine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27223 2022-04-15 19:29:28.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Homotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26985 2022-04-15 19:29:41.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31175 2022-04-15 20:02:25.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    31281 2022-04-15 20:02:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21305 2022-04-15 19:05:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19584 2022-04-15 19:05:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18201 2022-04-15 19:08:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Leucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17837 2022-04-15 19:08:56.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Leucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20952 2022-04-15 19:09:44.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Lysine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20688 2022-04-15 19:09:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Lysine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22663 2022-04-15 19:11:19.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Methionine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22585 2022-04-15 19:11:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Methionine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22299 2022-04-15 20:02:00.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-PhenylGlycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23920 2022-04-15 20:02:14.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28064 2022-04-15 19:13:14.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Phenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    27859 2022-04-15 19:13:28.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22124 2022-04-15 20:05:08.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Pipecolicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22915 2022-04-15 20:05:27.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18477 2022-04-15 19:18:02.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Proline.png
--rw-r--r--   0 barbara    (501) staff       (20)    17643 2022-04-15 19:18:21.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Proline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16148 2022-04-15 19:21:15.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Serine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16632 2022-04-15 19:21:29.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Serine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20138 2022-04-15 19:23:45.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19101 2022-04-15 19:24:01.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31764 2022-04-15 19:26:12.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Tryptophan.png
--rw-r--r--   0 barbara    (501) staff       (20)    31258 2022-04-15 19:26:31.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Tryptophan_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25906 2022-04-15 19:29:01.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Tyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25970 2022-04-15 19:29:16.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Tyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17416 2022-04-15 19:33:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Valine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17876 2022-04-15 19:33:58.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-Valine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23148 2022-04-15 19:06:01.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23181 2022-04-15 19:06:15.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20985 2022-04-15 19:24:11.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20334 2022-04-15 19:24:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    33952 2022-04-15 19:13:38.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    34678 2022-04-15 19:13:52.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25846 2022-04-15 19:35:06.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    25587 2022-04-15 19:35:19.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24721 2022-04-15 18:57:03.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-methylcysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24505 2022-04-15 18:57:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21642 2022-04-15 17:58:25.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-cycloOrnithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21479 2022-04-15 17:58:41.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29667 2022-04-15 18:56:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-cysteicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    29381 2022-04-15 18:56:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-cysteicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29226 2022-04-15 17:46:15.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png
--rw-r--r--   0 barbara    (501) staff       (20)    28550 2022-04-15 17:46:34.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24770 2022-04-15 19:52:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-enduracididine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25682 2022-04-15 19:53:04.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-enduracididine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22241 2022-04-15 17:57:52.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-homoserinelactone.png
--rw-r--r--   0 barbara    (501) staff       (20)    22473 2022-04-15 17:58:11.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22735 2022-04-15 19:34:15.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-isovaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    22465 2022-04-15 19:34:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-isovaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    30522 2022-04-15 19:53:52.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-kynurenine.png
--rw-r--r--   0 barbara    (501) staff       (20)    29353 2022-04-15 19:54:07.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-kynurenine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    41215 2022-04-15 17:07:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-lysergicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    41529 2022-04-15 17:07:56.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-lysergicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25178 2022-04-15 17:53:52.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22574 2022-04-15 17:54:07.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20125 2022-04-15 19:54:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-ornithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19709 2022-04-15 19:55:22.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-ornithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28423 2022-04-15 19:56:55.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-phosphinothricin.png
--rw-r--r--   0 barbara    (501) staff       (20)    28205 2022-04-15 19:57:09.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21871 2022-04-15 19:08:08.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-tert-Leucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21647 2022-04-15 19:08:27.000000 raichu-0.0.2/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21113 2022-04-15 19:45:57.000000 raichu-0.0.2/interactive/images/nrps_substrates/Dehydrobutyrine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21341 2022-04-15 19:46:14.000000 raichu-0.0.2/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22142 2022-04-15 19:01:12.000000 raichu-0.0.2/interactive/images/nrps_substrates/GlutamicAcid.png
--rw-r--r--   0 barbara    (501) staff       (20)    21175 2022-04-15 19:01:30.000000 raichu-0.0.2/interactive/images/nrps_substrates/GlutamicAcid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23165 2022-04-15 18:59:19.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glutamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23031 2022-04-15 18:59:42.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glutamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17898 2022-04-15 19:02:50.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17697 2022-04-15 19:03:09.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19769 2022-04-15 18:02:48.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glycocyamine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21086 2022-04-15 18:03:06.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glycocyamine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    15692 2022-04-15 18:02:08.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glycolicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    16640 2022-04-15 18:02:29.000000 raichu-0.0.2/interactive/images/nrps_substrates/Glycolicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24850 2022-04-15 19:03:33.000000 raichu-0.0.2/interactive/images/nrps_substrates/Histidine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23428 2022-04-15 19:03:48.000000 raichu-0.0.2/interactive/images/nrps_substrates/Histidine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27835 2022-04-15 19:12:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/Homophenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    28660 2022-04-15 19:13:04.000000 raichu-0.0.2/interactive/images/nrps_substrates/Homophenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20085 2022-04-15 19:20:19.000000 raichu-0.0.2/interactive/images/nrps_substrates/Homoserine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20528 2022-04-15 19:20:35.000000 raichu-0.0.2/interactive/images/nrps_substrates/Homoserine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25447 2022-04-15 19:28:07.000000 raichu-0.0.2/interactive/images/nrps_substrates/Homotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23415 2022-04-15 19:28:20.000000 raichu-0.0.2/interactive/images/nrps_substrates/Homotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28468 2022-04-15 20:01:09.000000 raichu-0.0.2/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    28646 2022-04-15 20:01:40.000000 raichu-0.0.2/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19848 2022-04-15 19:04:43.000000 raichu-0.0.2/interactive/images/nrps_substrates/Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20339 2022-04-15 19:04:57.000000 raichu-0.0.2/interactive/images/nrps_substrates/Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21246 2022-04-15 20:04:41.000000 raichu-0.0.2/interactive/images/nrps_substrates/L-piperazicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    20649 2022-04-15 20:04:56.000000 raichu-0.0.2/interactive/images/nrps_substrates/L-piperazicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17518 2022-04-15 19:07:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/Leucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    15410 2022-04-15 19:07:57.000000 raichu-0.0.2/interactive/images/nrps_substrates/Leucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20333 2022-04-15 19:09:15.000000 raichu-0.0.2/interactive/images/nrps_substrates/Lysine.png
--rw-r--r--   0 barbara    (501) staff       (20)    19916 2022-04-15 19:09:34.000000 raichu-0.0.2/interactive/images/nrps_substrates/Lysine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22102 2022-04-15 19:10:58.000000 raichu-0.0.2/interactive/images/nrps_substrates/Methionine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21961 2022-04-15 19:11:10.000000 raichu-0.0.2/interactive/images/nrps_substrates/Methionine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27813 2022-04-15 19:12:27.000000 raichu-0.0.2/interactive/images/nrps_substrates/N-acetylphenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26592 2022-04-15 19:12:41.000000 raichu-0.0.2/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20839 2022-04-15 19:32:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/Norvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    20626 2022-04-15 19:32:47.000000 raichu-0.0.2/interactive/images/nrps_substrates/Norvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16556 2022-04-15 19:54:29.000000 raichu-0.0.2/interactive/images/nrps_substrates/Ornithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17189 2022-04-15 19:54:43.000000 raichu-0.0.2/interactive/images/nrps_substrates/Ornithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26375 2022-04-15 19:12:02.000000 raichu-0.0.2/interactive/images/nrps_substrates/Phenylalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    25087 2022-04-15 19:12:17.000000 raichu-0.0.2/interactive/images/nrps_substrates/Phenylalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21576 2022-04-15 20:04:15.000000 raichu-0.0.2/interactive/images/nrps_substrates/Pipecolicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    19819 2022-04-15 20:04:30.000000 raichu-0.0.2/interactive/images/nrps_substrates/Pipecolicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20332 2022-04-15 19:17:31.000000 raichu-0.0.2/interactive/images/nrps_substrates/Proline.png
--rw-r--r--   0 barbara    (501) staff       (20)    20084 2022-04-15 19:17:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/Proline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    32150 2022-04-15 17:03:55.000000 raichu-0.0.2/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    28251 2022-04-15 17:04:40.000000 raichu-0.0.2/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21333 2022-04-15 19:43:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/R-coronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    21941 2022-04-15 19:43:48.000000 raichu-0.0.2/interactive/images/nrps_substrates/R-coronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:43:02.000000 raichu-0.0.2/interactive/images/nrps_substrates/R-norcoronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22773 2022-04-15 19:43:16.000000 raichu-0.0.2/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    17234 2022-04-15 19:19:18.000000 raichu-0.0.2/interactive/images/nrps_substrates/Serine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17342 2022-04-15 19:19:31.000000 raichu-0.0.2/interactive/images/nrps_substrates/Serine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18484 2022-04-15 19:23:19.000000 raichu-0.0.2/interactive/images/nrps_substrates/Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17304 2022-04-15 19:23:34.000000 raichu-0.0.2/interactive/images/nrps_substrates/Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    31342 2022-04-15 19:25:43.000000 raichu-0.0.2/interactive/images/nrps_substrates/Tryptophan.png
--rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:26:56.000000 raichu-0.0.2/interactive/images/nrps_substrates/Tryptophan_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25101 2022-04-15 19:27:42.000000 raichu-0.0.2/interactive/images/nrps_substrates/Tyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24311 2022-04-15 19:27:56.000000 raichu-0.0.2/interactive/images/nrps_substrates/Tyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16390 2022-04-15 19:32:05.000000 raichu-0.0.2/interactive/images/nrps_substrates/Valine.png
--rw-r--r--   0 barbara    (501) staff       (20)    16071 2022-04-15 19:32:22.000000 raichu-0.0.2/interactive/images/nrps_substrates/Valine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/interactive/images/nrps_substrates/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    21812 2022-04-15 19:06:24.000000 raichu-0.0.2/interactive/images/nrps_substrates/allo-Isoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22026 2022-04-15 19:06:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    19013 2022-04-15 19:24:37.000000 raichu-0.0.2/interactive/images/nrps_substrates/allo-Threonine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17084 2022-04-15 19:24:50.000000 raichu-0.0.2/interactive/images/nrps_substrates/allo-Threonine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34193 2022-04-15 19:14:24.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    33802 2022-04-15 19:14:43.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20539 2022-04-15 19:38:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-ethylnorvaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    21837 2022-04-15 19:38:50.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25078 2022-04-15 18:04:22.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25232 2022-04-15 18:04:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21753 2022-04-15 18:03:44.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    19502 2022-04-15 18:04:10.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23125 2022-04-15 18:58:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-methylcysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    21614 2022-04-15 18:58:56.000000 raichu-0.0.2/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18232 2022-04-15 18:48:23.000000 raichu-0.0.2/interactive/images/nrps_substrates/beta-Alanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    17866 2022-04-15 18:48:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/beta-Alanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22745 2022-04-15 19:10:12.000000 raichu-0.0.2/interactive/images/nrps_substrates/beta-lysine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22631 2022-04-15 19:10:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/beta-lysine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27655 2022-04-15 19:57:20.000000 raichu-0.0.2/interactive/images/nrps_substrates/capreomycidine.png
--rw-r--r--   0 barbara    (501) staff       (20)    27032 2022-04-15 19:57:47.000000 raichu-0.0.2/interactive/images/nrps_substrates/capreomycidine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23007 2022-04-15 19:44:40.000000 raichu-0.0.2/interactive/images/nrps_substrates/coronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    22918 2022-04-15 19:44:54.000000 raichu-0.0.2/interactive/images/nrps_substrates/coronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20766 2022-04-15 17:58:50.000000 raichu-0.0.2/interactive/images/nrps_substrates/cycloOrnithine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20540 2022-04-15 17:59:07.000000 raichu-0.0.2/interactive/images/nrps_substrates/cycloOrnithine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28850 2022-04-15 18:58:10.000000 raichu-0.0.2/interactive/images/nrps_substrates/cysteicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    29414 2022-04-15 18:58:28.000000 raichu-0.0.2/interactive/images/nrps_substrates/cysteicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22320 2022-04-15 18:55:32.000000 raichu-0.0.2/interactive/images/nrps_substrates/dehydro-cysteine.png
--rw-r--r--   0 barbara    (501) staff       (20)    22028 2022-04-15 18:55:49.000000 raichu-0.0.2/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20723 2022-04-15 18:47:18.000000 raichu-0.0.2/interactive/images/nrps_substrates/dehydroalanine.png
--rw-r--r--   0 barbara    (501) staff       (20)    20497 2022-04-15 18:47:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/dehydroalanine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24909 2022-04-15 19:28:37.000000 raichu-0.0.2/interactive/images/nrps_substrates/dehydrotyrosine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24347 2022-04-15 19:28:51.000000 raichu-0.0.2/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    32343 2022-04-15 17:07:03.000000 raichu-0.0.2/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png
--rw-r--r--   0 barbara    (501) staff       (20)    31754 2022-04-15 17:07:23.000000 raichu-0.0.2/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27766 2022-04-15 19:52:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/enduracididine.png
--rw-r--r--   0 barbara    (501) staff       (20)    27194 2022-04-15 19:52:40.000000 raichu-0.0.2/interactive/images/nrps_substrates/enduracididine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23358 2022-04-15 18:50:34.000000 raichu-0.0.2/interactive/images/nrps_substrates/homoarginine.png
--rw-r--r--   0 barbara    (501) staff       (20)    24247 2022-04-15 18:50:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/homoarginine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    23746 2022-04-15 19:05:09.000000 raichu-0.0.2/interactive/images/nrps_substrates/homoisoleucine.png
--rw-r--r--   0 barbara    (501) staff       (20)    23630 2022-04-15 19:05:24.000000 raichu-0.0.2/interactive/images/nrps_substrates/homoisoleucine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22096 2022-04-15 17:57:02.000000 raichu-0.0.2/interactive/images/nrps_substrates/homoserinelactone.png
--rw-r--r--   0 barbara    (501) staff       (20)    21719 2022-04-15 17:57:34.000000 raichu-0.0.2/interactive/images/nrps_substrates/homoserinelactone_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26982 2022-04-15 17:06:27.000000 raichu-0.0.2/interactive/images/nrps_substrates/hydrocinnamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25601 2022-04-15 17:06:44.000000 raichu-0.0.2/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26043 2022-04-15 17:05:53.000000 raichu-0.0.2/interactive/images/nrps_substrates/hydroxypicolinicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25858 2022-04-15 17:06:13.000000 raichu-0.0.2/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21960 2022-04-15 19:33:08.000000 raichu-0.0.2/interactive/images/nrps_substrates/isovaline.png
--rw-r--r--   0 barbara    (501) staff       (20)    21200 2022-04-15 19:33:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/isovaline_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26809 2022-04-15 19:53:26.000000 raichu-0.0.2/interactive/images/nrps_substrates/kynurenine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26107 2022-04-15 19:53:41.000000 raichu-0.0.2/interactive/images/nrps_substrates/kynurenine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24972 2022-04-15 17:54:33.000000 raichu-0.0.2/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    26606 2022-04-15 17:54:50.000000 raichu-0.0.2/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21926 2022-04-15 19:44:05.000000 raichu-0.0.2/interactive/images/nrps_substrates/norcoronamicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    20749 2022-04-15 19:44:27.000000 raichu-0.0.2/interactive/images/nrps_substrates/norcoronamicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    18052 2022-04-15 18:08:44.000000 raichu-0.0.2/interactive/images/nrps_substrates/nrp.png
--rw-r--r--   0 barbara    (501) staff       (20)    17895 2022-04-15 18:09:02.000000 raichu-0.0.2/interactive/images/nrps_substrates/nrp_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25531 2022-04-15 17:05:15.000000 raichu-0.0.2/interactive/images/nrps_substrates/phenylaceticacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    25533 2022-04-15 17:05:36.000000 raichu-0.0.2/interactive/images/nrps_substrates/phenylaceticacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26331 2022-04-15 20:00:39.000000 raichu-0.0.2/interactive/images/nrps_substrates/phenylglycine.png
--rw-r--r--   0 barbara    (501) staff       (20)    26106 2022-04-15 20:00:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/phenylglycine_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    27784 2022-04-15 19:56:30.000000 raichu-0.0.2/interactive/images/nrps_substrates/phosphinothricin.png
--rw-r--r--   0 barbara    (501) staff       (20)    27870 2022-04-15 19:56:42.000000 raichu-0.0.2/interactive/images/nrps_substrates/phosphinothricin_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24381 2022-04-15 16:53:14.000000 raichu-0.0.2/interactive/images/nrps_substrates/salicylicacid.png
--rw-r--r--   0 barbara    (501) staff       (20)    23788 2022-04-15 17:51:37.000000 raichu-0.0.2/interactive/images/nrps_substrates/salicylicacid_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21002 2022-04-15 19:06:59.000000 raichu-0.0.2/interactive/images/nrps_substrates/tert-Leu.png
--rw-r--r--   0 barbara    (501) staff       (20)    20891 2022-04-15 19:07:24.000000 raichu-0.0.2/interactive/images/nrps_substrates/tert-Leu_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    16198 2022-04-15 18:01:40.000000 raichu-0.0.2/interactive/images/nrps_substrates/valinol.png
--rw-r--r--   0 barbara    (501) staff       (20)    16320 2022-04-15 18:01:54.000000 raichu-0.0.2/interactive/images/nrps_substrates/valinol_highlight.png
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.431520 raichu-0.0.2/interactive/images/pks_starter_substrates/
--rw-r--r--   0 barbara    (501) staff       (20)    29850 2022-05-01 12:06:56.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2R-hMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    26673 2022-05-01 12:07:06.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2R-hMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25251 2022-05-01 12:06:33.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2R-mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    23606 2022-05-01 12:06:48.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2R-mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    33676 2022-05-01 12:06:14.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2S-hMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    33230 2022-05-01 12:06:24.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2S-hMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    26972 2022-05-01 12:05:48.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2S-mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    26664 2022-05-01 12:06:03.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2S-mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24670 2022-05-01 12:07:17.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    24923 2022-05-01 12:07:25.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/2mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25417 2022-05-01 12:05:22.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/3mBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    25187 2022-05-01 12:05:39.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/3mBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    20866 2022-05-01 12:05:03.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/Ac.png
--rw-r--r--   0 barbara    (501) staff       (20)    21010 2022-05-01 12:05:13.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/Ac_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25026 2022-05-01 12:04:44.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/Benz.png
--rw-r--r--   0 barbara    (501) staff       (20)    25713 2022-05-01 12:04:54.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/Benz_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    34080 2022-05-01 12:04:21.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/CHC.png
--rw-r--r--   0 barbara    (501) staff       (20)    33079 2022-05-01 12:04:32.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/CHC_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21110 2022-05-01 12:03:36.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/Prop.png
--rw-r--r--   0 barbara    (501) staff       (20)    20850 2022-05-01 12:03:52.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/Prop_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    32496 2022-05-01 12:40:12.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/ceMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    31629 2022-05-01 12:40:20.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/ceMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    29134 2022-05-01 12:04:02.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/hMal.png
--rw-r--r--   0 barbara    (501) staff       (20)    28542 2022-05-01 12:04:10.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/hMal_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    22191 2022-05-01 16:48:04.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/isoBut.png
--rw-r--r--   0 barbara    (501) staff       (20)    21953 2022-05-01 16:48:17.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/isoBut_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    41464 2022-05-01 12:03:11.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/tCPDA.png
--rw-r--r--   0 barbara    (501) staff       (20)    40950 2022-05-01 12:03:25.000000 raichu-0.0.2/interactive/images/pks_starter_substrates/tCPDA_highlight.png
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.436330 raichu-0.0.2/interactive/images/pks_substrates/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/interactive/images/pks_substrates/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    24949 2022-04-16 08:01:15.000000 raichu-0.0.2/interactive/images/pks_substrates/ethylmalonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    25556 2022-04-16 08:01:32.000000 raichu-0.0.2/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    24099 2022-04-16 07:57:17.000000 raichu-0.0.2/interactive/images/pks_substrates/malonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    23782 2022-04-16 07:59:21.000000 raichu-0.0.2/interactive/images/pks_substrates/malonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    28684 2022-04-16 08:02:38.000000 raichu-0.0.2/interactive/images/pks_substrates/methoxymalonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    28317 2022-04-16 08:02:54.000000 raichu-0.0.2/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    25513 2022-04-16 07:58:33.000000 raichu-0.0.2/interactive/images/pks_substrates/methylmalonylcoa.png
--rw-r--r--   0 barbara    (501) staff       (20)    25625 2022-04-16 07:58:50.000000 raichu-0.0.2/interactive/images/pks_substrates/methylmalonylcoa_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)    21959 2022-04-16 08:04:06.000000 raichu-0.0.2/interactive/images/pks_substrates/wildcard.png
--rw-r--r--   0 barbara    (501) staff       (20)    22218 2022-04-16 08:04:28.000000 raichu-0.0.2/interactive/images/pks_substrates/wildcard_highlight.png
--rw-r--r--   0 barbara    (501) staff       (20)      913 2022-04-14 09:57:57.000000 raichu-0.0.2/interactive/insertion_point.py
--rw-r--r--   0 barbara    (501) staff       (20)    11853 2022-05-02 15:50:16.000000 raichu-0.0.2/interactive/load_antismash.py
--rw-r--r--   0 barbara    (501) staff       (20)     4136 2022-05-02 13:04:31.000000 raichu-0.0.2/interactive/load_tabular.py
--rw-r--r--   0 barbara    (501) staff       (20)     3769 2022-04-19 13:35:36.000000 raichu-0.0.2/interactive/module.py
--rw-r--r--   0 barbara    (501) staff       (20)      306 2022-04-15 16:35:29.000000 raichu-0.0.2/interactive/parsers.py
--rw-r--r--   0 barbara    (501) staff       (20)     5462 2022-10-24 15:18:24.000000 raichu-0.0.2/interactive/render_cluster.py
--rw-r--r--   0 barbara    (501) staff       (20)    27124 2022-05-05 14:52:33.000000 raichu-0.0.2/interactive/run_raichu.py
--rw-r--r--   0 barbara    (501) staff       (20)     2083 2022-05-05 14:48:17.000000 raichu-0.0.2/interactive/style.py
--rw-r--r--   0 barbara    (501) staff       (20)    18130 2022-05-08 06:33:46.000000 raichu-0.0.2/interactive/substrate.py
--rw-r--r--   0 barbara    (501) staff       (20)     1117 2022-04-14 09:00:39.000000 raichu-0.0.2/interactive/textbox.py
--rw-r--r--   0 barbara    (501) staff       (20)       89 2021-09-16 23:05:31.000000 raichu-0.0.2/pyproject.toml
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.438302 raichu-0.0.2/raichu/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-0.0.2/raichu/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     4296 2022-10-27 13:31:49.000000 raichu-0.0.2/raichu/attach_to_domain.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.439523 raichu-0.0.2/raichu/central_chain_detection/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/central_chain_detection/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     2386 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/central_chain_detection/find_central_chain.py
--rw-r--r--   0 barbara    (501) staff       (20)    16999 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/central_chain_detection/label_central_chain.py
--rw-r--r--   0 barbara    (501) staff       (20)     3361 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/class_domain.py
--rw-r--r--   0 barbara    (501) staff       (20)     8832 2022-11-01 13:05:55.000000 raichu-0.0.2/raichu/cluster.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.440909 raichu-0.0.2/raichu/data/
--rw-r--r--   0 barbara    (501) staff       (20)     6623 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/data/PARAS_smiles.txt
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/data/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)      137 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/data/at_elongation_specificities.txt
--rw-r--r--   0 barbara    (501) staff       (20)      269 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/data/at_specificities.txt
--rw-r--r--   0 barbara    (501) staff       (20)      481 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/data/attributes.py
--rw-r--r--   0 barbara    (501) staff       (20)     4289 2022-10-31 13:16:58.000000 raichu-0.0.2/raichu/data/molecular_moieties.py
--rw-r--r--   0 barbara    (501) staff       (20)     3834 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/data/substrate_to_abbreviation.txt
--rw-r--r--   0 barbara    (501) staff       (20)     8380 2022-10-31 13:16:58.000000 raichu-0.0.2/raichu/data/trans_at.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.441386 raichu-0.0.2/raichu/domain/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/domain/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)    10027 2022-11-01 12:52:53.000000 raichu-0.0.2/raichu/domain/domain.py
--rw-r--r--   0 barbara    (501) staff       (20)     5418 2022-10-27 12:08:17.000000 raichu-0.0.2/raichu/domain/domain_types.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.442244 raichu-0.0.2/raichu/drawing/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/drawing/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     8234 2022-10-31 13:16:38.000000 raichu-0.0.2/raichu/drawing/bubbles.py
--rw-r--r--   0 barbara    (501) staff       (20)     3110 2022-10-27 11:37:23.000000 raichu-0.0.2/raichu/drawing/colours.py
--rw-r--r--   0 barbara    (501) staff       (20)    72871 2022-10-31 15:55:17.000000 raichu-0.0.2/raichu/drawing/drawer.py
--rw-r--r--   0 barbara    (501) staff       (20)    22726 2022-11-01 07:44:04.000000 raichu-0.0.2/raichu/module.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.444243 raichu-0.0.2/raichu/reactions/
--rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/reactions/__init__.py
--rw-r--r--   0 barbara    (501) staff       (20)     9298 2022-10-25 19:29:36.000000 raichu-0.0.2/raichu/reactions/chain_release.py
--rw-r--r--   0 barbara    (501) staff       (20)     1001 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/reactions/general.py
--rw-r--r--   0 barbara    (501) staff       (20)     4180 2022-10-24 15:18:24.000000 raichu-0.0.2/raichu/reactions/nrps_elongation_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     3397 2022-10-31 13:12:39.000000 raichu-0.0.2/raichu/reactions/nrps_tailoring_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)     4424 2022-10-27 13:17:17.000000 raichu-0.0.2/raichu/reactions/pks_elongation_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)    30573 2022-11-01 07:54:16.000000 raichu-0.0.2/raichu/reactions/pks_tailoring_reactions.py
--rw-r--r--   0 barbara    (501) staff       (20)    15776 2022-10-27 14:03:41.000000 raichu-0.0.2/raichu/run_raichu.py
--rw-r--r--   0 barbara    (501) staff       (20)     9823 2022-11-01 11:37:41.000000 raichu-0.0.2/raichu/run_raichu_trans_at.py
--rw-r--r--   0 barbara    (501) staff       (20)     5928 2022-10-31 13:16:58.000000 raichu-0.0.2/raichu/substrate.py
-drwxr-xr-x   0 barbara    (501) staff       (20)        0 2022-11-01 13:10:55.439059 raichu-0.0.2/raichu.egg-info/
--rw-r--r--   0 barbara    (501) staff       (20)      169 2022-11-01 13:10:55.000000 raichu-0.0.2/raichu.egg-info/PKG-INFO
--rw-r--r--   0 barbara    (501) staff       (20)    24421 2022-11-01 13:10:55.000000 raichu-0.0.2/raichu.egg-info/SOURCES.txt
--rw-r--r--   0 barbara    (501) staff       (20)        1 2022-11-01 13:10:55.000000 raichu-0.0.2/raichu.egg-info/dependency_links.txt
--rw-r--r--   0 barbara    (501) staff       (20)       30 2022-11-01 13:10:55.000000 raichu-0.0.2/raichu.egg-info/requires.txt
--rw-r--r--   0 barbara    (501) staff       (20)       19 2022-11-01 13:10:55.000000 raichu-0.0.2/raichu.egg-info/top_level.txt
--rw-r--r--   0 barbara    (501) staff       (20)       38 2022-11-01 13:10:55.444929 raichu-0.0.2/setup.cfg
--rw-r--r--   0 barbara    (501) staff       (20)      593 2022-11-01 13:10:44.000000 raichu-0.0.2/setup.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.415982 raichu-1.0.0/
+-rw-r--r--   0 barbara    (501) staff       (20)     1091 2022-11-01 19:03:21.000000 raichu-1.0.0/LICENSE.txt
+-rw-r--r--   0 barbara    (501) staff       (20)      322 2024-04-15 15:52:56.415674 raichu-1.0.0/PKG-INFO
+-rw-r--r--   0 barbara    (501) staff       (20)     2255 2024-04-15 15:19:04.000000 raichu-1.0.0/README.md
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.243041 raichu-1.0.0/bin/
+-rw-r--r--   0 barbara    (501) staff       (20)     3137 2022-05-02 12:36:20.000000 raichu-1.0.0/bin/raichu
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.248049 raichu-1.0.0/interactive/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1655 2022-04-17 16:18:30.000000 raichu-1.0.0/interactive/background.py
+-rw-r--r--   0 barbara    (501) staff       (20)    38866 2022-05-01 17:29:00.000000 raichu-1.0.0/interactive/buttons.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2595 2022-05-01 12:51:17.000000 raichu-1.0.0/interactive/domain.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4354 2022-05-02 15:38:29.000000 raichu-1.0.0/interactive/gene.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.248446 raichu-1.0.0/interactive/images/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.255629 raichu-1.0.0/interactive/images/domains/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/domains/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    13363 2022-04-13 17:02:54.000000 raichu-1.0.0/interactive/images/domains/a.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13470 2022-04-14 07:32:59.000000 raichu-1.0.0/interactive/images/domains/a_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17374 2022-04-13 17:02:35.000000 raichu-1.0.0/interactive/images/domains/acp.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17372 2022-04-14 07:32:26.000000 raichu-1.0.0/interactive/images/domains/acp_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13468 2022-04-13 17:04:13.000000 raichu-1.0.0/interactive/images/domains/at.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13414 2022-04-14 07:35:16.000000 raichu-1.0.0/interactive/images/domains/at_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14370 2022-04-13 17:03:11.000000 raichu-1.0.0/interactive/images/domains/c.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14334 2022-04-14 07:33:37.000000 raichu-1.0.0/interactive/images/domains/c_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13271 2022-04-13 17:05:03.000000 raichu-1.0.0/interactive/images/domains/dh.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13201 2022-04-14 07:36:35.000000 raichu-1.0.0/interactive/images/domains/dh_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11416 2022-04-13 17:03:29.000000 raichu-1.0.0/interactive/images/domains/e.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11408 2022-04-14 07:34:15.000000 raichu-1.0.0/interactive/images/domains/e_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13101 2022-04-13 17:05:18.000000 raichu-1.0.0/interactive/images/domains/er.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13218 2022-04-14 07:37:04.000000 raichu-1.0.0/interactive/images/domains/er_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14279 2022-04-13 17:04:47.000000 raichu-1.0.0/interactive/images/domains/kr.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14317 2022-04-14 07:36:07.000000 raichu-1.0.0/interactive/images/domains/kr_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16398 2022-04-13 17:04:28.000000 raichu-1.0.0/interactive/images/domains/ks.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16402 2022-04-14 07:35:43.000000 raichu-1.0.0/interactive/images/domains/ks_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13835 2022-04-13 17:05:36.000000 raichu-1.0.0/interactive/images/domains/nmt.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13911 2022-04-14 07:37:51.000000 raichu-1.0.0/interactive/images/domains/nmt_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-13 17:02:14.000000 raichu-1.0.0/interactive/images/domains/pcp.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15728 2022-04-14 07:32:16.000000 raichu-1.0.0/interactive/images/domains/pcp_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11757 2022-04-13 17:03:45.000000 raichu-1.0.0/interactive/images/domains/te.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11784 2022-04-14 07:34:50.000000 raichu-1.0.0/interactive/images/domains/te_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34945 2022-04-14 08:27:48.000000 raichu-1.0.0/interactive/images/icon.png
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.259540 raichu-1.0.0/interactive/images/kr_subtypes/
+-rw-r--r--   0 barbara    (501) staff       (20)     6853 2022-04-16 14:37:34.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR.png
+-rw-r--r--   0 barbara    (501) staff       (20)    10255 2022-04-16 14:40:44.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A1.png
+-rw-r--r--   0 barbara    (501) staff       (20)    10233 2022-04-16 14:40:58.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A1_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14129 2022-04-16 14:40:22.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A2.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13940 2022-04-16 14:40:36.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_A2_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)     9104 2022-04-16 14:39:53.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B1.png
+-rw-r--r--   0 barbara    (501) staff       (20)     9076 2022-04-16 14:40:07.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B1_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    12935 2022-04-16 14:39:32.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B2.png
+-rw-r--r--   0 barbara    (501) staff       (20)    12803 2022-04-16 14:39:45.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_B2_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11395 2022-04-16 14:39:06.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C1.png
+-rw-r--r--   0 barbara    (501) staff       (20)    11318 2022-04-16 14:39:21.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C1_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14939 2022-04-16 14:38:43.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C2.png
+-rw-r--r--   0 barbara    (501) staff       (20)    14756 2022-04-16 14:38:56.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_C2_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)     6819 2022-04-16 14:38:16.000000 raichu-1.0.0/interactive/images/kr_subtypes/KR_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/kr_subtypes/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.383620 raichu-1.0.0/interactive/images/nrps_substrates/
+-rw-r--r--   0 barbara    (501) staff       (20)    29614 2022-04-15 19:51:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29531 2022-04-15 19:51:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29732 2022-04-15 19:50:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30295 2022-04-15 19:50:55.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    42828 2022-04-15 19:59:58.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png
+-rw-r--r--   0 barbara    (501) staff       (20)    40729 2022-04-15 20:00:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:51:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30420 2022-04-15 19:51:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29315 2022-04-15 19:31:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29122 2022-04-15 19:31:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34021 2022-04-15 19:27:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31793 2022-04-15 19:27:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28970 2022-04-15 19:48:46.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28787 2022-04-15 19:49:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27662 2022-04-15 17:47:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30028 2022-04-15 17:47:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27300 2022-04-15 19:48:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27047 2022-04-15 19:48:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41323 2022-04-15 17:53:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    40856 2022-04-15 17:53:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25318 2022-04-15 19:41:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24974 2022-04-15 19:41:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:49:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23130 2022-04-15 19:50:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27411 2022-04-15 19:49:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27276 2022-04-15 19:49:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23030 2022-04-15 19:22:32.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22312 2022-04-15 19:22:46.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30762 2022-04-15 17:48:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29202 2022-04-15 17:48:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21732 2022-04-15 18:06:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22544 2022-04-15 18:06:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21505 2022-04-15 18:49:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21077 2022-04-15 18:49:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    36652 2022-04-15 20:03:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35330 2022-04-15 20:03:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25798 2022-04-15 19:59:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23250 2022-04-15 19:59:46.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    36143 2022-04-15 19:58:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35659 2022-04-15 19:59:13.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22618 2022-04-15 18:05:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22388 2022-04-15 18:05:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    39152 2022-04-15 19:30:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    38713 2022-04-15 19:31:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30192 2022-04-15 19:00:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30391 2022-04-15 19:00:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31392 2022-04-15 19:30:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30693 2022-04-15 19:30:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    37365 2022-04-15 19:29:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    36877 2022-04-15 19:30:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27121 2022-04-15 19:55:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25672 2022-04-15 19:55:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31631 2022-04-15 18:52:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31245 2022-04-15 18:52:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    38385 2022-04-15 17:46:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35115 2022-04-15 17:47:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24864 2022-04-15 19:39:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24656 2022-04-15 19:39:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28181 2022-04-15 19:25:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28922 2022-04-15 19:25:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25868 2022-04-15 19:02:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24839 2022-04-15 19:02:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24797 2022-04-15 19:18:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24917 2022-04-15 19:18:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16493 2022-04-15 18:48:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16392 2022-04-15 18:49:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13602 2022-04-15 18:04:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alaninol.png
+-rw-r--r--   0 barbara    (501) staff       (20)    13514 2022-04-15 18:05:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/Alaninol_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24271 2022-04-15 19:58:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24821 2022-04-15 19:58:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23158 2022-04-15 18:51:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/Arginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22351 2022-04-15 18:51:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/Arginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21621 2022-04-15 18:53:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/Asparagine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21080 2022-04-15 18:53:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/Asparagine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23527 2022-04-15 18:54:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23278 2022-04-15 18:55:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35623 2022-04-15 19:58:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35114 2022-04-15 19:58:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19216 2022-04-15 19:42:23.000000 raichu-1.0.0/interactive/images/nrps_substrates/Citrulline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20529 2022-04-15 19:42:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/Citrulline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17085 2022-04-15 18:57:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/Cysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17879 2022-04-15 18:57:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/Cysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25588 2022-04-15 19:47:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25308 2022-04-15 19:47:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23524 2022-04-15 19:46:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25188 2022-04-15 19:46:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25783 2022-04-15 19:40:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24378 2022-04-15 19:40:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23608 2022-04-15 19:47:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23287 2022-04-15 19:47:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25855 2022-04-15 18:03:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25575 2022-04-15 18:03:32.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    35436 2022-04-15 20:02:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33762 2022-04-15 20:03:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15814 2022-04-15 18:47:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16164 2022-04-15 18:48:05.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24190 2022-04-15 18:51:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23965 2022-04-15 18:51:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23867 2022-04-15 18:52:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22155 2022-04-15 18:53:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24591 2022-04-15 18:54:13.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24267 2022-04-15 18:54:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21764 2022-04-15 19:41:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21249 2022-04-15 19:42:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18606 2022-04-15 18:55:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16731 2022-04-15 18:56:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24393 2022-04-15 19:01:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24049 2022-04-15 19:01:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23556 2022-04-15 18:59:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22325 2022-04-15 19:00:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25709 2022-04-15 19:04:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25190 2022-04-15 19:04:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21390 2022-04-15 19:21:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21180 2022-04-15 19:22:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27223 2022-04-15 19:29:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26985 2022-04-15 19:29:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31175 2022-04-15 20:02:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31281 2022-04-15 20:02:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21305 2022-04-15 19:05:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19584 2022-04-15 19:05:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18201 2022-04-15 19:08:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17837 2022-04-15 19:08:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20952 2022-04-15 19:09:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20688 2022-04-15 19:09:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22663 2022-04-15 19:11:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22585 2022-04-15 19:11:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22299 2022-04-15 20:02:00.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23920 2022-04-15 20:02:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28064 2022-04-15 19:13:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27859 2022-04-15 19:13:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22124 2022-04-15 20:05:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22915 2022-04-15 20:05:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18477 2022-04-15 19:18:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Proline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17643 2022-04-15 19:18:21.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Proline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16148 2022-04-15 19:21:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Serine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16632 2022-04-15 19:21:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Serine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20138 2022-04-15 19:23:45.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19101 2022-04-15 19:24:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31764 2022-04-15 19:26:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31258 2022-04-15 19:26:31.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25906 2022-04-15 19:29:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25970 2022-04-15 19:29:16.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17416 2022-04-15 19:33:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Valine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17876 2022-04-15 19:33:58.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-Valine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23148 2022-04-15 19:06:01.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23181 2022-04-15 19:06:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20985 2022-04-15 19:24:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20334 2022-04-15 19:24:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33952 2022-04-15 19:13:38.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34678 2022-04-15 19:13:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25846 2022-04-15 19:35:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25587 2022-04-15 19:35:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24721 2022-04-15 18:57:03.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24505 2022-04-15 18:57:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21642 2022-04-15 17:58:25.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21479 2022-04-15 17:58:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29667 2022-04-15 18:56:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29381 2022-04-15 18:56:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29226 2022-04-15 17:46:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28550 2022-04-15 17:46:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24770 2022-04-15 19:52:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25682 2022-04-15 19:53:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22241 2022-04-15 17:57:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22473 2022-04-15 17:58:11.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22735 2022-04-15 19:34:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22465 2022-04-15 19:34:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30522 2022-04-15 19:53:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29353 2022-04-15 19:54:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41215 2022-04-15 17:07:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41529 2022-04-15 17:07:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25178 2022-04-15 17:53:52.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22574 2022-04-15 17:54:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20125 2022-04-15 19:54:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19709 2022-04-15 19:55:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28423 2022-04-15 19:56:55.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28205 2022-04-15 19:57:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21871 2022-04-15 19:08:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21647 2022-04-15 19:08:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21113 2022-04-15 19:45:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21341 2022-04-15 19:46:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22142 2022-04-15 19:01:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21175 2022-04-15 19:01:30.000000 raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23165 2022-04-15 18:59:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glutamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23031 2022-04-15 18:59:42.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glutamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17898 2022-04-15 19:02:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17697 2022-04-15 19:03:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19769 2022-04-15 18:02:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21086 2022-04-15 18:03:06.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15692 2022-04-15 18:02:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16640 2022-04-15 18:02:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24850 2022-04-15 19:03:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/Histidine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23428 2022-04-15 19:03:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/Histidine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27835 2022-04-15 19:12:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28660 2022-04-15 19:13:04.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20085 2022-04-15 19:20:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homoserine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20528 2022-04-15 19:20:35.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homoserine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25447 2022-04-15 19:28:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23415 2022-04-15 19:28:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28468 2022-04-15 20:01:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28646 2022-04-15 20:01:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19848 2022-04-15 19:04:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20339 2022-04-15 19:04:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21246 2022-04-15 20:04:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20649 2022-04-15 20:04:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17518 2022-04-15 19:07:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/Leucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    15410 2022-04-15 19:07:57.000000 raichu-1.0.0/interactive/images/nrps_substrates/Leucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20333 2022-04-15 19:09:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/Lysine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19916 2022-04-15 19:09:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/Lysine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22102 2022-04-15 19:10:58.000000 raichu-1.0.0/interactive/images/nrps_substrates/Methionine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21961 2022-04-15 19:11:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/Methionine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27813 2022-04-15 19:12:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26592 2022-04-15 19:12:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20839 2022-04-15 19:32:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/Norvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20626 2022-04-15 19:32:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/Norvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16556 2022-04-15 19:54:29.000000 raichu-1.0.0/interactive/images/nrps_substrates/Ornithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17189 2022-04-15 19:54:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Ornithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26375 2022-04-15 19:12:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25087 2022-04-15 19:12:17.000000 raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21576 2022-04-15 20:04:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19819 2022-04-15 20:04:30.000000 raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20332 2022-04-15 19:17:31.000000 raichu-1.0.0/interactive/images/nrps_substrates/Proline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20084 2022-04-15 19:17:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/Proline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    32150 2022-04-15 17:03:55.000000 raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28251 2022-04-15 17:04:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21333 2022-04-15 19:43:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21941 2022-04-15 19:43:48.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23048 2022-04-15 19:43:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22773 2022-04-15 19:43:16.000000 raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17234 2022-04-15 19:19:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/Serine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17342 2022-04-15 19:19:31.000000 raichu-1.0.0/interactive/images/nrps_substrates/Serine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18484 2022-04-15 19:23:19.000000 raichu-1.0.0/interactive/images/nrps_substrates/Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17304 2022-04-15 19:23:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31342 2022-04-15 19:25:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan.png
+-rw-r--r--   0 barbara    (501) staff       (20)    30842 2022-04-15 19:26:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25101 2022-04-15 19:27:42.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24311 2022-04-15 19:27:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16390 2022-04-15 19:32:05.000000 raichu-1.0.0/interactive/images/nrps_substrates/Valine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16071 2022-04-15 19:32:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/Valine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    21812 2022-04-15 19:06:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22026 2022-04-15 19:06:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19013 2022-04-15 19:24:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17084 2022-04-15 19:24:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34193 2022-04-15 19:14:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33802 2022-04-15 19:14:43.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20539 2022-04-15 19:38:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21837 2022-04-15 19:38:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25078 2022-04-15 18:04:22.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25232 2022-04-15 18:04:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21753 2022-04-15 18:03:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    19502 2022-04-15 18:04:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23125 2022-04-15 18:58:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21614 2022-04-15 18:58:56.000000 raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18232 2022-04-15 18:48:23.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17866 2022-04-15 18:48:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22745 2022-04-15 19:10:12.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22631 2022-04-15 19:10:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27655 2022-04-15 19:57:20.000000 raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27032 2022-04-15 19:57:47.000000 raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23007 2022-04-15 19:44:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22918 2022-04-15 19:44:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20766 2022-04-15 17:58:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20540 2022-04-15 17:59:07.000000 raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28850 2022-04-15 18:58:10.000000 raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29414 2022-04-15 18:58:28.000000 raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22320 2022-04-15 18:55:32.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22028 2022-04-15 18:55:49.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20723 2022-04-15 18:47:18.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20497 2022-04-15 18:47:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24909 2022-04-15 19:28:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24347 2022-04-15 19:28:51.000000 raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    32343 2022-04-15 17:07:03.000000 raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31754 2022-04-15 17:07:23.000000 raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27766 2022-04-15 19:52:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/enduracididine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27194 2022-04-15 19:52:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/enduracididine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23358 2022-04-15 18:50:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoarginine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24247 2022-04-15 18:50:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoarginine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23746 2022-04-15 19:05:09.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23630 2022-04-15 19:05:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22096 2022-04-15 17:57:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21719 2022-04-15 17:57:34.000000 raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26982 2022-04-15 17:06:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25601 2022-04-15 17:06:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26043 2022-04-15 17:05:53.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25858 2022-04-15 17:06:13.000000 raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21960 2022-04-15 19:33:08.000000 raichu-1.0.0/interactive/images/nrps_substrates/isovaline.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21200 2022-04-15 19:33:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/isovaline_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26809 2022-04-15 19:53:26.000000 raichu-1.0.0/interactive/images/nrps_substrates/kynurenine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26107 2022-04-15 19:53:41.000000 raichu-1.0.0/interactive/images/nrps_substrates/kynurenine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24972 2022-04-15 17:54:33.000000 raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26606 2022-04-15 17:54:50.000000 raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21926 2022-04-15 19:44:05.000000 raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20749 2022-04-15 19:44:27.000000 raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    18052 2022-04-15 18:08:44.000000 raichu-1.0.0/interactive/images/nrps_substrates/nrp.png
+-rw-r--r--   0 barbara    (501) staff       (20)    17895 2022-04-15 18:09:02.000000 raichu-1.0.0/interactive/images/nrps_substrates/nrp_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25531 2022-04-15 17:05:15.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25533 2022-04-15 17:05:36.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26331 2022-04-15 20:00:39.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26106 2022-04-15 20:00:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27784 2022-04-15 19:56:30.000000 raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin.png
+-rw-r--r--   0 barbara    (501) staff       (20)    27870 2022-04-15 19:56:42.000000 raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24381 2022-04-15 16:53:14.000000 raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23788 2022-04-15 17:51:37.000000 raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21002 2022-04-15 19:06:59.000000 raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20891 2022-04-15 19:07:24.000000 raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16198 2022-04-15 18:01:40.000000 raichu-1.0.0/interactive/images/nrps_substrates/valinol.png
+-rw-r--r--   0 barbara    (501) staff       (20)    16320 2022-04-15 18:01:54.000000 raichu-1.0.0/interactive/images/nrps_substrates/valinol_highlight.png
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.395629 raichu-1.0.0/interactive/images/pks_starter_substrates/
+-rw-r--r--   0 barbara    (501) staff       (20)    29850 2022-05-01 12:06:56.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26673 2022-05-01 12:07:06.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25251 2022-05-01 12:06:33.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23606 2022-05-01 12:06:48.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33676 2022-05-01 12:06:14.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33230 2022-05-01 12:06:24.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26972 2022-05-01 12:05:48.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    26664 2022-05-01 12:06:03.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24670 2022-05-01 12:07:17.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24923 2022-05-01 12:07:25.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25417 2022-05-01 12:05:22.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25187 2022-05-01 12:05:39.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20866 2022-05-01 12:05:03.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Ac.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21010 2022-05-01 12:05:13.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Ac_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25026 2022-05-01 12:04:44.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Benz.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25713 2022-05-01 12:04:54.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Benz_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    34080 2022-05-01 12:04:21.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/CHC.png
+-rw-r--r--   0 barbara    (501) staff       (20)    33079 2022-05-01 12:04:32.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/CHC_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21110 2022-05-01 12:03:36.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Prop.png
+-rw-r--r--   0 barbara    (501) staff       (20)    20850 2022-05-01 12:03:52.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/Prop_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    32496 2022-05-01 12:40:12.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    31629 2022-05-01 12:40:20.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    29134 2022-05-01 12:04:02.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/hMal.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28542 2022-05-01 12:04:10.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/hMal_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22191 2022-05-01 16:48:04.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21953 2022-05-01 16:48:17.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    41464 2022-05-01 12:03:11.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA.png
+-rw-r--r--   0 barbara    (501) staff       (20)    40950 2022-05-01 12:03:25.000000 raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA_highlight.png
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.399265 raichu-1.0.0/interactive/images/pks_substrates/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/interactive/images/pks_substrates/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    24949 2022-04-16 08:01:15.000000 raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25556 2022-04-16 08:01:32.000000 raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    24099 2022-04-16 07:57:17.000000 raichu-1.0.0/interactive/images/pks_substrates/malonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    23782 2022-04-16 07:59:21.000000 raichu-1.0.0/interactive/images/pks_substrates/malonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28684 2022-04-16 08:02:38.000000 raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    28317 2022-04-16 08:02:54.000000 raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25513 2022-04-16 07:58:33.000000 raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa.png
+-rw-r--r--   0 barbara    (501) staff       (20)    25625 2022-04-16 07:58:50.000000 raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)    21959 2022-04-16 08:04:06.000000 raichu-1.0.0/interactive/images/pks_substrates/wildcard.png
+-rw-r--r--   0 barbara    (501) staff       (20)    22218 2022-04-16 08:04:28.000000 raichu-1.0.0/interactive/images/pks_substrates/wildcard_highlight.png
+-rw-r--r--   0 barbara    (501) staff       (20)      913 2022-04-14 09:57:57.000000 raichu-1.0.0/interactive/insertion_point.py
+-rw-r--r--   0 barbara    (501) staff       (20)    11853 2022-05-02 15:50:16.000000 raichu-1.0.0/interactive/load_antismash.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4136 2022-05-02 13:04:31.000000 raichu-1.0.0/interactive/load_tabular.py
+-rw-r--r--   0 barbara    (501) staff       (20)     3769 2022-04-19 13:35:36.000000 raichu-1.0.0/interactive/module.py
+-rw-r--r--   0 barbara    (501) staff       (20)      306 2022-04-15 16:35:29.000000 raichu-1.0.0/interactive/parsers.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5462 2022-10-24 15:18:24.000000 raichu-1.0.0/interactive/render_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    27124 2022-05-05 14:52:33.000000 raichu-1.0.0/interactive/run_raichu.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2083 2022-05-05 14:48:17.000000 raichu-1.0.0/interactive/style.py
+-rw-r--r--   0 barbara    (501) staff       (20)    18130 2022-05-08 06:33:46.000000 raichu-1.0.0/interactive/substrate.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1117 2022-04-14 09:00:39.000000 raichu-1.0.0/interactive/textbox.py
+-rw-r--r--   0 barbara    (501) staff       (20)       89 2021-09-16 23:05:31.000000 raichu-1.0.0/pyproject.toml
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.402906 raichu-1.0.0/raichu/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-04-13 14:19:28.000000 raichu-1.0.0/raichu/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     3656 2024-02-08 09:09:32.000000 raichu-1.0.0/raichu/alkaloid.py
+-rw-r--r--   0 barbara    (501) staff       (20)    37295 2024-04-15 15:44:13.000000 raichu-1.0.0/raichu/antismash.py
+-rw-r--r--   0 barbara    (501) staff       (20)    11162 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/attach_to_domain.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.404211 raichu-1.0.0/raichu/central_chain_detection/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/central_chain_detection/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     9199 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/central_chain_detection/find_central_chain.py
+-rw-r--r--   0 barbara    (501) staff       (20)    19314 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/central_chain_detection/label_central_chain.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4124 2023-05-01 07:37:35.000000 raichu-1.0.0/raichu/class_domain.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.405841 raichu-1.0.0/raichu/cluster/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2023-05-07 08:18:53.000000 raichu-1.0.0/raichu/cluster/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)      736 2023-05-07 08:52:51.000000 raichu-1.0.0/raichu/cluster/alkaloid_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    16380 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/cluster/base_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    15618 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/cluster/modular_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)    16428 2023-05-07 17:50:23.000000 raichu-1.0.0/raichu/cluster/ripp_cluster.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5799 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/cluster/terpene_cluster.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.408417 raichu-1.0.0/raichu/data/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)      137 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/at_elongation_specificities.txt
+-rw-r--r--   0 barbara    (501) staff       (20)      269 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/at_specificities.txt
+-rw-r--r--   0 barbara    (501) staff       (20)     4969 2023-12-08 12:52:08.000000 raichu-1.0.0/raichu/data/attributes.py
+-rw-r--r--   0 barbara    (501) staff       (20)    20943 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/metadata.txt
+-rw-r--r--   0 barbara    (501) staff       (20)    10888 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/molecular_moieties.py
+-rw-r--r--   0 barbara    (501) staff       (20)    14079 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/smiles.txt
+-rw-r--r--   0 barbara    (501) staff       (20)     3834 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/data/substrate_to_abbreviation.txt
+-rw-r--r--   0 barbara    (501) staff       (20)     9683 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/data/trans_at.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.409217 raichu-1.0.0/raichu/domain/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/domain/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    10455 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/domain/domain.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5614 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/domain/domain_types.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.411412 raichu-1.0.0/raichu/drawing/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/drawing/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     9301 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/drawing/bubbles.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5636 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/drawing/colours.py
+-rw-r--r--   0 barbara    (501) staff       (20)    83982 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/drawing/drawer.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1613 2023-05-07 18:03:32.000000 raichu-1.0.0/raichu/drawing/pathway.py
+-rw-r--r--   0 barbara    (501) staff       (20)      678 2023-05-07 08:52:51.000000 raichu-1.0.0/raichu/drawing/ripp_drawing.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5734 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/general.py
+-rw-r--r--   0 barbara    (501) staff       (20)    25860 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/module.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.413792 raichu-1.0.0/raichu/reactions/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2022-10-24 15:18:24.000000 raichu-1.0.0/raichu/reactions/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)    12341 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/chain_release.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1001 2024-02-08 15:43:23.000000 raichu-1.0.0/raichu/reactions/general.py
+-rw-r--r--   0 barbara    (501) staff       (20)    19163 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/general_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4530 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/nrps_elongation_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     5632 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/nrps_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     4658 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/pks_elongation_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     1125 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/pks_sidechain_chirality.py
+-rw-r--r--   0 barbara    (501) staff       (20)    34020 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/reactions/pks_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2403 2023-05-01 07:37:35.000000 raichu-1.0.0/raichu/reactions/ripp_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)     6737 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/representations.py
+-rw-r--r--   0 barbara    (501) staff       (20)    21201 2024-02-08 09:09:32.000000 raichu-1.0.0/raichu/ripp.py
+-rw-r--r--   0 barbara    (501) staff       (20)    38926 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/run_raichu.py
+-rw-r--r--   0 barbara    (501) staff       (20)     2806 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/smiles_handling.py
+-rw-r--r--   0 barbara    (501) staff       (20)     6667 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/substrate.py
+-rw-r--r--   0 barbara    (501) staff       (20)    32389 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/tailoring_enzymes.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414171 raichu-1.0.0/raichu/test/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)     9670 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/generate_test_data.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414366 raichu-1.0.0/raichu/test/test_data/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/test_data/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414490 raichu-1.0.0/raichu/test/unit/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/__init__.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.414863 raichu-1.0.0/raichu/test/unit/reactions/
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/reactions/__init__.py
+-rw-r--r--   0 barbara    (501) staff       (20)        0 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/reactions/test_general_tailoring_reactions.py
+-rw-r--r--   0 barbara    (501) staff       (20)      416 2024-04-15 15:19:04.000000 raichu-1.0.0/raichu/test/unit/reactions/test_nrps_tailoring_reactions.py
+drwxr-xr-x   0 barbara    (501) staff       (20)        0 2024-04-15 15:52:56.415203 raichu-1.0.0/raichu.egg-info/
+-rw-r--r--   0 barbara    (501) staff       (20)      322 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/PKG-INFO
+-rw-r--r--   0 barbara    (501) staff       (20)    25323 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/SOURCES.txt
+-rw-r--r--   0 barbara    (501) staff       (20)        1 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/dependency_links.txt
+-rw-r--r--   0 barbara    (501) staff       (20)       47 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/requires.txt
+-rw-r--r--   0 barbara    (501) staff       (20)       19 2024-04-15 15:52:56.000000 raichu-1.0.0/raichu.egg-info/top_level.txt
+-rw-r--r--   0 barbara    (501) staff       (20)       38 2024-04-15 15:52:56.416037 raichu-1.0.0/setup.cfg
+-rw-r--r--   0 barbara    (501) staff       (20)      650 2024-04-15 15:48:01.000000 raichu-1.0.0/setup.py
```

### Comparing `raichu-0.0.2/bin/raichu` & `raichu-1.0.0/bin/raichu`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/background.py` & `raichu-1.0.0/interactive/background.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/buttons.py` & `raichu-1.0.0/interactive/buttons.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/domain.py` & `raichu-1.0.0/interactive/domain.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/gene.py` & `raichu-1.0.0/interactive/gene.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/a.png` & `raichu-1.0.0/interactive/images/domains/a.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/a_highlight.png` & `raichu-1.0.0/interactive/images/domains/a_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/acp.png` & `raichu-1.0.0/interactive/images/domains/acp.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/acp_highlight.png` & `raichu-1.0.0/interactive/images/domains/acp_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/at.png` & `raichu-1.0.0/interactive/images/domains/at.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/at_highlight.png` & `raichu-1.0.0/interactive/images/domains/at_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/c.png` & `raichu-1.0.0/interactive/images/domains/c.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/c_highlight.png` & `raichu-1.0.0/interactive/images/domains/c_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/dh.png` & `raichu-1.0.0/interactive/images/domains/dh.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/dh_highlight.png` & `raichu-1.0.0/interactive/images/domains/dh_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/e.png` & `raichu-1.0.0/interactive/images/domains/e.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/e_highlight.png` & `raichu-1.0.0/interactive/images/domains/e_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/er.png` & `raichu-1.0.0/interactive/images/domains/er.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/er_highlight.png` & `raichu-1.0.0/interactive/images/domains/er_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/kr.png` & `raichu-1.0.0/interactive/images/domains/kr.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/kr_highlight.png` & `raichu-1.0.0/interactive/images/domains/kr_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/ks.png` & `raichu-1.0.0/interactive/images/domains/ks.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/ks_highlight.png` & `raichu-1.0.0/interactive/images/domains/ks_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/nmt.png` & `raichu-1.0.0/interactive/images/domains/nmt.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/nmt_highlight.png` & `raichu-1.0.0/interactive/images/domains/nmt_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/pcp.png` & `raichu-1.0.0/interactive/images/domains/pcp.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/pcp_highlight.png` & `raichu-1.0.0/interactive/images/domains/pcp_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/te.png` & `raichu-1.0.0/interactive/images/domains/te.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/domains/te_highlight.png` & `raichu-1.0.0/interactive/images/domains/te_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/icon.png` & `raichu-1.0.0/interactive/images/icon.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_A1.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_A1.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_A1_highlight.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_A1_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_A2.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_A2.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_A2_highlight.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_A2_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_B1.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_B1.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_B1_highlight.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_B1_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_B2.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_B2.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_B2_highlight.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_B2_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_C1.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_C1.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_C1_highlight.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_C1_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_C2.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_C2.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_C2_highlight.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_C2_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/kr_subtypes/KR_highlight.png` & `raichu-1.0.0/interactive/images/kr_subtypes/KR_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2R,3R)-2,3-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2S)-2,3-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3R)-2-amino-3-hydroxy-4-(4-nitrophenyl)butanoate_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(2S,3S)-2,3-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(R)beta-tyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/(R)beta-tyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,3-Dehydro-Tryptophan_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,3-diamino-3-methyl-propanoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,3-dihydroxybenzoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2,4-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Amino-9,10-epoxy-8-oxodecanoidacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoadipicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoadipicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Aminobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Aminoisobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Methylserine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-Methylserine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-Methylserine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-carboxyquinoxaline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-carboxyquinoxaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-hydroxyisovalerate.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-hydroxyisovalerate_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-methyl-beta-alanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/2-methyl-beta-alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3,5-dihydroxyphenylglycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-(3-Pyridyl)-Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-[(1R,2R)-2-Nitrocyclopropyl]-L-alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-aminopropanimidamide.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-aminopropanimidamide_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxy-4-O-methyl-5-methyltyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxyglutamine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-hydroxyglutamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-methyltyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/3-methyltyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyhomotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4,5-Dihydroxyornithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4,5-dehydroarginine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4,5-dehydroarginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyindole-3-carboxylicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyvaline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-Hydroxyvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-butenyl-4-methylthreonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-methylglutamicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-methylglutamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-methylproline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/4-methylproline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/4-methylproline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Alanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Alanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Alaninol.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Alaninol.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Alaninol_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Alaninol_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Anticapsin.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Anticapsin_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Anticapsin_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Arginine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Arginine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Arginine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Arginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Asparagine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Asparagine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Asparagine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Asparagine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/AsparticAcid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/AsparticAcid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/AsparticAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Beta-hydroxycyclohex-2-enylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Citrulline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Citrulline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Citrulline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Citrulline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Cysteine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Cysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Cysteine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Cysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2,3-Diaminopropionicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2,4-diaminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminoadipicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2-Aminobutyricacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-2-hydroxyisovalerate_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-3,5-dihydroxyphenylglycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Alanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Alanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Arginine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Arginine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Arginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Asparagine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Asparagine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Asparagine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-AsparticAcid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-AsparticAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Citrulline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Citrulline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Citrulline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Cysteine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Cysteine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Cysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-GlutamicAcid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-GlutamicAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Glutamine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Glutamine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Glutamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Histidine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Histidine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Histidine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Homoserine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Homoserine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Homoserine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Homotyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Homotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-HydroxyPhenylGlycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Isoleucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Isoleucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Leucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Leucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Leucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Lysine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Lysine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Lysine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Methionine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Methionine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Methionine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-PhenylGlycine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-PhenylGlycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Phenylalanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Phenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Pipecolicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Pipecolicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Proline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Proline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Proline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Proline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Serine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Serine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Serine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Serine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Threonine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Threonine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Tryptophan.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Tryptophan_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Tryptophan_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Tyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Tyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Tyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Valine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Valine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-Valine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-Valine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Isoleucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Threonine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-allo-Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-amino-phenyl-valericacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-ethylnorvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-methylcysteine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-alpha-methylcysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-cycloOrnithine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-cycloOrnithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-cysteicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-cysteicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-cysteicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-dihydroxyphenylthiazolgroup_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-enduracididine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-enduracididine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-enduracididine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-homoserinelactone.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-homoserinelactone_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-isovaline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-isovaline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-isovaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-kynurenine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-kynurenine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-kynurenine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-lysergicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-lysergicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-lysergicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-methyl-2-aminooctanoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-ornithine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-ornithine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-ornithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-phosphinothricin.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-phosphinothricin_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-tert-Leucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/D-tert-Leucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Dehydrobutyrine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Dehydrobutyrine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/GlutamicAcid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/GlutamicAcid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/GlutamicAcid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glutamine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glutamine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glutamine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glutamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glycine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glycine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glycine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glycocyamine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glycocyamine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glycocyamine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glycolicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Glycolicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Glycolicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Histidine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Histidine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Histidine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Histidine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Homophenylalanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Homophenylalanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Homophenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Homoserine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Homoserine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Homoserine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Homoserine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Homotyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Homotyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Homotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Isoleucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Isoleucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/L-piperazicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/L-piperazicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/L-piperazicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Leucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Leucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Leucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Leucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Lysine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Lysine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Lysine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Lysine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Methionine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Methionine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Methionine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Methionine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/N-acetylphenylalanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/N-acetylphenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Norvaline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Norvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Norvaline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Norvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Ornithine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Ornithine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Ornithine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Ornithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Phenylalanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Phenylalanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Phenylalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Pipecolicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Pipecolicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Pipecolicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Proline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Proline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Proline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Proline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Quinoline-2-carboxylicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/R-coronamicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/R-coronamicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/R-coronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/R-norcoronamicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/R-norcoronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Serine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Serine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Serine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Serine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Threonine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Threonine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Tryptophan.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Tryptophan_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Tryptophan_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Tyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Tyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Tyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Valine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Valine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/Valine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/Valine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/allo-Isoleucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/allo-Isoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/allo-Threonine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/allo-Threonine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/allo-Threonine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-amino-phenyl-valericacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-ethylnorvaline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ethylnorvaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisocaproicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-ketoisovalericacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-methylcysteine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/alpha-methylcysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/beta-Alanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/beta-Alanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/beta-Alanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/beta-lysine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/beta-lysine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/beta-lysine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/capreomycidine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/capreomycidine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/capreomycidine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/coronamicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/coronamicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/coronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/cycloOrnithine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/cycloOrnithine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/cycloOrnithine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/cysteicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/cysteicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/cysteicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dehydro-cysteine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dehydro-cysteine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dehydroalanine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dehydroalanine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dehydroalanine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dehydrotyrosine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dehydrotyrosine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/dihydroxyphenylthiazolgroup_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/enduracididine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/enduracididine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/enduracididine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/enduracididine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/homoarginine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/homoarginine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/homoarginine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/homoarginine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/homoisoleucine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/homoisoleucine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/homoisoleucine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/homoserinelactone.png` & `raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/homoserinelactone_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/homoserinelactone_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/hydrocinnamicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/hydrocinnamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/hydroxypicolinicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/hydroxypicolinicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/isovaline.png` & `raichu-1.0.0/interactive/images/nrps_substrates/isovaline.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/isovaline_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/isovaline_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/kynurenine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/kynurenine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/kynurenine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/kynurenine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/methyl-2-aminooctanoicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/norcoronamicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/norcoronamicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/norcoronamicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/nrp.png` & `raichu-1.0.0/interactive/images/nrps_substrates/nrp.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/nrp_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/nrp_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/phenylaceticacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/phenylaceticacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/phenylaceticacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/phenylglycine.png` & `raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/phenylglycine_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/phenylglycine_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/phosphinothricin.png` & `raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/phosphinothricin_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/phosphinothricin_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/salicylicacid.png` & `raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/salicylicacid_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/salicylicacid_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/tert-Leu.png` & `raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/tert-Leu_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/tert-Leu_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/valinol.png` & `raichu-1.0.0/interactive/images/nrps_substrates/valinol.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/nrps_substrates/valinol_highlight.png` & `raichu-1.0.0/interactive/images/nrps_substrates/valinol_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2R-hMal.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2R-hMal_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-hMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2R-mBut.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2R-mBut_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2R-mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2S-hMal.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2S-hMal_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-hMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2S-mBut.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2S-mBut_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2S-mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2mBut.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/2mBut_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/2mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/3mBut.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/3mBut_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/3mBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/Ac.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/Ac.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/Ac_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/Ac_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/Benz.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/Benz.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/Benz_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/Benz_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/CHC.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/CHC.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/CHC_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/CHC_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/Prop.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/Prop.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/Prop_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/Prop_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/ceMal.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/ceMal_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/ceMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/hMal.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/hMal.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/hMal_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/hMal_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/isoBut.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/isoBut_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/isoBut_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/tCPDA.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_starter_substrates/tCPDA_highlight.png` & `raichu-1.0.0/interactive/images/pks_starter_substrates/tCPDA_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/ethylmalonylcoa.png` & `raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png` & `raichu-1.0.0/interactive/images/pks_substrates/ethylmalonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/malonylcoa.png` & `raichu-1.0.0/interactive/images/pks_substrates/malonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/malonylcoa_highlight.png` & `raichu-1.0.0/interactive/images/pks_substrates/malonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/methoxymalonylcoa.png` & `raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png` & `raichu-1.0.0/interactive/images/pks_substrates/methoxymalonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/methylmalonylcoa.png` & `raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/methylmalonylcoa_highlight.png` & `raichu-1.0.0/interactive/images/pks_substrates/methylmalonylcoa_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/wildcard.png` & `raichu-1.0.0/interactive/images/pks_substrates/wildcard.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/images/pks_substrates/wildcard_highlight.png` & `raichu-1.0.0/interactive/images/pks_substrates/wildcard_highlight.png`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/insertion_point.py` & `raichu-1.0.0/interactive/insertion_point.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/load_antismash.py` & `raichu-1.0.0/interactive/load_antismash.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/load_tabular.py` & `raichu-1.0.0/interactive/load_tabular.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/module.py` & `raichu-1.0.0/interactive/module.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/render_cluster.py` & `raichu-1.0.0/interactive/render_cluster.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/run_raichu.py` & `raichu-1.0.0/interactive/run_raichu.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/style.py` & `raichu-1.0.0/interactive/style.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/substrate.py` & `raichu-1.0.0/interactive/substrate.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/interactive/textbox.py` & `raichu-1.0.0/interactive/textbox.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/raichu/central_chain_detection/label_central_chain.py` & `raichu-1.0.0/raichu/central_chain_detection/label_central_chain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,126 @@
 from pikachu.reactions.functional_groups import GroupDefiner, find_atoms, find_bonds
-from pikachu.general import read_smiles
-from raichu.data.attributes import ATTRIBUTES
 from raichu.reactions.general import initialise_atom_attributes
-from raichu.attach_to_domain import attach_to_domain_pk
+
+import timeout_decorator
 from raichu.data.molecular_moieties import AMINO_FATTY_ACID, AMINO_ACID_BACKBONE, N_AMINO_ACID, C1_AMINO_ACID, \
     C2_AMINO_ACID, BETA_AMINO_ACID_BACKBONE, B_N_AMINO_ACID, B_C1_AMINO_ACID, B_C2_AMINO_ACID, B_C3_AMINO_ACID, \
-    B_LEAVING_BOND, ACID_C1
+    B_LEAVING_BOND, ACID_C1, OH_AMINO_ACID, N_AMINO_ACID_ATTACHED, C1_AMINO_ACID_ATTACHED, C2_AMINO_ACID_ATTACHED
 
 POLYKETIDE_S = GroupDefiner('Sulphur atom polyketide', 'SC(C)=O', 0)
+POLYKETIDE_S_INSERTED_O = GroupDefiner('Sulphur atom polyketide inserted O', 'SC(O)=O', 0)
+POLYKETIDE_S_REDUCED_STARTER = GroupDefiner('Sulphur atom polyketide', 'SC(C)O', 0)
+
+
+class CentralChain:
+    def __init__(self, structure, chain_type):
+        self.structure = structure
+        if chain_type in ['ripp', 'nrps', 'pks']:
+            self.chain_type = chain_type
+        else:
+            raise ValueError(f"Expected 'ripp', 'nrps', or 'pks' as central chain type; got {chain_type}")
+
+    def label_central_chain(self):
+        raise NotImplementedError
+
+
+class PksCentralChain(CentralChain):
+    def __init__(self, structure):
+        super().__init__(structure, chain_type='pks')
 
 
+class NrpsCentralChain(CentralChain):
+    def __init__(self, structure):
+        super().__init__(structure, chain_type='nrps')
+
+
+class RippCentralChain(CentralChain):
+    def __init__(self, structure):
+        super().__init__(structure, chain_type='ripp')
+
+
+@timeout_decorator.timeout(3)
 def label_pk_central_chain(pk_starter_unit):
     """Finds the the atoms in the central chain of the polyketide starter unit,
     sets the in_central_chain Atom object attribute to True/False accordingly,
     after which the pk_starter_unit Structure object is returned.
 
     pk_starter_unit: PIKAChU Structure object of the PK starter unit
     """
 
     initialise_atom_attributes(pk_starter_unit)
     central_chain = []
     visited = []
 
     # Check if structure is a polyketide, define sulphur attached to domain
     locations_sulphur = find_atoms(POLYKETIDE_S, pk_starter_unit)
+    if len(locations_sulphur) == 0:
+        locations_sulphur = find_atoms(POLYKETIDE_S_INSERTED_O, pk_starter_unit)
+        if len(locations_sulphur) == 0:
+            locations_sulphur = find_atoms(POLYKETIDE_S_REDUCED_STARTER, pk_starter_unit)
     assert len(locations_sulphur) == 1
+    
     sulphur_polyketide = locations_sulphur[0]
     central_chain.append(sulphur_polyketide)
 
     # Iterate over atom neighbours, check if the atom belongs to the central
     # carbon chain (i.e., not a methyl/ethyl/methoxy sidechain) and add to list
     for neighbour in sulphur_polyketide.neighbours:
         if neighbour.type == 'C':
             chain_carbon = neighbour
             end_carbon = False
             central_chain.append(chain_carbon)
             visited.append(chain_carbon)
 
             while not end_carbon:
+
                 for next_atom in chain_carbon.neighbours:
                     ethyl_branch = False
                     inside_cycle = False
                     methyl_group = False
 
                     # Build lists of neighbouring atom types
-                    if next_atom.type == 'C' and next_atom not in visited:
+                    if next_atom.type == 'C' and next_atom not in visited or \
+                            (next_atom.type == 'O' and next_atom not in visited and
+                             len(next_atom.get_neighbours('C')) == 2):
 
                         # Keep track of carbon neighbours
 
                         # Confirm carbon doesn't belong to ethyl sidebranch
                         types = []
                         c_neighbours = next_atom.get_neighbours('C')
                         if len(c_neighbours) == 2 and next_atom.get_neighbour('O') is None:
 
-                            for atom in c_neighbours:
-                                for neighbour in atom.neighbours:
-                                    types.append(neighbour.type)
+                            for carbon_neighbour in c_neighbours:
+                                for branch_neighbour in carbon_neighbour.neighbours:
+                                    types.append(branch_neighbour.type)
 
                             if types.count('H') == 4 and types.count('C') == 4:
                                 ethyl_branch = True
 
-                            for atom in c_neighbours:
-                                if atom not in visited and atom != next_atom:
+                            for carbon_neighbour in c_neighbours:
+                                if carbon_neighbour not in visited and carbon_neighbour != next_atom:
                                     ethyl_branch = False
 
                             visited.append(chain_carbon)
 
                         # Carbon in a terminal carboxylic acid group is the
                         # final carbon in the central chain
                         if len(next_atom.get_neighbours('O')) == 2:
+                            for oxygen in next_atom.get_neighbours('O'):
+                                if next_atom.get_bond(oxygen).type == 'single':
+                                    central_chain.append(oxygen)
+                                    visited.append(oxygen)
                             central_chain.append(next_atom)
                             end_carbon = True
                             visited.append(chain_carbon)
 
                         # Confirm carbon is not part of cycle
                         if len(c_neighbours) == 2:
-                            if all(atom.in_ring(pk_starter_unit) for atom in c_neighbours):
-                                print(15)
+                            if all(carbon.in_ring(pk_starter_unit) for carbon in c_neighbours):
                                 visited.append(next_atom)
                                 inside_cycle = True
                                 end_carbon = True
 
                         # Case if carbon is part of a benzene ring
                         if len(c_neighbours) == 3 and len(next_atom.neighbours) == 3:
                             # central_chain.append(next_atom) #added 10/04/2021
@@ -117,29 +157,30 @@
                             methyl_group = True
 
                             # Terminal methyl group is not a side branch:
                             count_c_neighbours_not_visited = 0
                             for neighbouring_atom in chain_carbon.neighbours:
                                 if neighbouring_atom.type == 'C' and neighbouring_atom not in visited:
                                     count_c_neighbours_not_visited += 1
+
                             if count_c_neighbours_not_visited < 2:
                                 methyl_group = False
                                 visited.append(chain_carbon)
-                                for neighbour in chain_carbon.neighbours:
-                                    if neighbour.type == 'C' and neighbour not in visited:
+                                for carbon_neighbour in chain_carbon.neighbours:
+                                    if carbon_neighbour.type == 'C' and carbon_neighbour not in visited:
                                         next_neighbours = []
-                                        for next_neighbour in neighbour.neighbours:
+                                        for next_neighbour in carbon_neighbour.neighbours:
                                             next_neighbours.append(
                                                 next_neighbour.type)
                                         if next_neighbours.count('H') == 3 or (
                                                 next_neighbours.count(
                                                         'H') == 2 and (
                                                 next_neighbours.count(
                                                         '*')) == 1):
-                                            central_chain.append(neighbour)
+                                            central_chain.append(carbon_neighbour)
                                 end_carbon = True
 
                             visited.append(chain_carbon)
 
                         # Identification of central chain carbon atoms through
                         # exclusion
                         if not ethyl_branch and not methyl_group and not \
@@ -152,41 +193,61 @@
     for atom in pk_starter_unit.graph:
         if atom in central_chain:
             atom.annotations.in_central_chain = True
         else:
             atom.annotations.in_central_chain = False
 
 
+def label_ripp_central_chain(peptide):
+    initialise_atom_attributes(peptide)
+
+    n_atoms_aa = find_atoms(N_AMINO_ACID_ATTACHED, peptide)
+    c1_atoms_aa = find_atoms(C1_AMINO_ACID_ATTACHED, peptide)
+    c2_atoms_aa = find_atoms(C2_AMINO_ACID_ATTACHED, peptide)
+    oh_atoms_aa = find_atoms(OH_AMINO_ACID, peptide)
+
+    for nitrogen in n_atoms_aa:
+        nitrogen.annotations.in_central_chain = True
+        nitrogen.annotations.n_atom_nmeth = True
+    for carbon in c1_atoms_aa:
+        carbon.annotations.in_central_chain = True
+        carbon.annotations.chiral_c_ep = True
+    for carbon in c2_atoms_aa:
+        carbon.annotations.in_central_chain = True
+    for oxygen in oh_atoms_aa:
+        oxygen.annotations.in_central_chain = True
+
+
 def label_nrp_central_chain(peptide, module_type='elongation'):
     initialise_atom_attributes(peptide)
 
     as_normal = False
     if module_type == 'starter':
         if peptide.find_substructures(AMINO_FATTY_ACID):
             acid = peptide
             label_acid_central_chain(acid)
         else:
             as_normal = True
 
     if as_normal or module_type == 'elongation':
-
         if peptide.find_substructures(AMINO_ACID_BACKBONE):
             n_atoms_aa = find_atoms(N_AMINO_ACID, peptide)
             c1_atoms_aa = find_atoms(C1_AMINO_ACID, peptide)
             c2_atoms_aa = find_atoms(C2_AMINO_ACID, peptide)
 
             assert len(n_atoms_aa) == 1
             assert len(c1_atoms_aa) == 1
             assert len(c2_atoms_aa) == 1
 
             n_atoms_aa[0].annotations.in_central_chain = True
             n_atoms_aa[0].annotations.n_atom_nmeth = True
             c1_atoms_aa[0].annotations.in_central_chain = True
             c1_atoms_aa[0].annotations.chiral_c_ep = True
             c2_atoms_aa[0].annotations.in_central_chain = True
+
         elif peptide.find_substructures(BETA_AMINO_ACID_BACKBONE):
             n_atoms_aa = find_atoms(B_N_AMINO_ACID, peptide)
             c1_atoms_aa = find_atoms(B_C1_AMINO_ACID, peptide)
             c2_atoms_aa = find_atoms(B_C2_AMINO_ACID, peptide)
             c3_atoms_aa = find_atoms(B_C3_AMINO_ACID, peptide)
 
             assert len(n_atoms_aa) == 1
@@ -226,15 +287,15 @@
 
 
 def label_acid_central_chain(acid):
     c1_atom = None
     c2_atom = None
     oh_o_atom = None
     oh_h_atom = None
-    visited = []
+    backbone = []
 
     c1_atoms_aa = find_atoms(ACID_C1, acid)
     if c1_atoms_aa:
         c1_atom = c1_atoms_aa[0]
 
     assert c1_atom
 
@@ -269,106 +330,105 @@
     assert oh_o_atom
     assert oh_h_atom
 
     c1_atom.annotations.in_central_chain = True
     c2_atom.annotations.in_central_chain = True
     c2_atom.annotations.c2_acid = True
 
-    visited.append(c1_atom)
-    visited.append(c2_atom)
+    backbone.append(c1_atom)
+    backbone.append(c2_atom)
 
-    starting_point = c1_atom
+    last_backbone_atom = c1_atom
     endpoint = False
-    ring_members = 0
-    if starting_point.in_ring(acid):
-        ring_members += 1
 
     # Add atoms in chain with exactly 2 non-H neighbours to the central chain
     while not endpoint:
-        for neighbour in starting_point.get_non_hydrogen_neighbours():
-            neighbour_in_ring = neighbour.in_ring(acid)
-            if neighbour_in_ring:
-                ring_members += 1
-            neighbour_found = False
-            if len(neighbour.get_non_hydrogen_bonds()) == 2 and neighbour.type == 'C' and neighbour not in visited \
-                    and not (ring_members > 2 and neighbour_in_ring):
-                neighbour.annotations.in_central_chain = True
-                visited.append(neighbour)
-                starting_point = neighbour
-                neighbour_found = True
-
-            if not neighbour_found and neighbour.type == 'C' and neighbour not in visited and \
-                    len(neighbour.get_non_hydrogen_bonds()) >= 2 and not (ring_members > 2 and neighbour_in_ring):
-                terminal_count = 0
-                for atom in neighbour.neighbours:
-                    if atom not in visited and len(atom.get_non_hydrogen_bonds()) == 1:
-                        terminal_count += 1
-
-                if len(neighbour.get_non_hydrogen_bonds()) - terminal_count == 2:
-                    neighbour.annotations.in_central_chain = True
-                    visited.append(neighbour)
-                    starting_point = neighbour
-                    neighbour_found = True
-
-                if neighbour_found:
-                    break
-
-            if not neighbour_found and len(neighbour.get_non_hydrogen_bonds()) == 2 and neighbour not in visited \
-                    and not (ring_members > 2 and neighbour_in_ring):
-                neighbour.annotations.in_central_chain = True
-                visited.append(neighbour)
-                starting_point = neighbour
-                break
-
-            neighbours = []
-            for nb in starting_point.get_non_hydrogen_neighbours():
-                if nb not in visited:
-                    neighbours.append(nb)
-
-            if any(atom.in_ring(acid) for atom in neighbours) and neighbour_in_ring:
-                endpoint = True
-                for atom in neighbours:
-                    if len(atom.get_non_hydrogen_bonds()) == 1 and atom.get_non_hydrogen_bonds()[0].type == 'single':
-                        atom.annotations.in_central_chain = True
-                break
-
-            elif not any(len(atom.get_non_hydrogen_bonds()) == 2 for atom in neighbours):
-
-                endpoint = True
-
-                for atom in neighbours:
-                    terminal_count = 0
-                    for atom_2 in atom.neighbours:
-                        if atom_2 not in visited and len(atom_2.get_non_hydrogen_bonds()) == 1:
-                            terminal_count += 1
-
-                    if len(atom.get_non_hydrogen_bonds()) - terminal_count == 2:
-                        endpoint = False
-                        break
-
-                if endpoint:
-
-                    # Add the last atom in the chain to the central chain
-                    for atom in neighbours:
-                        if len(atom.get_non_hydrogen_bonds()) == 1 and atom.get_non_hydrogen_bonds()[0].type == 'single':
-                            atom.annotations.in_central_chain = True
-                    break
-
-
-if __name__ == "__main__":
-    starter_units_antismash = ['SC(=O)CC', 'SC(CC(O)=O)=O', 'SC(CC(O)=O)=O',
-                               'SC(C(C(O)=O)CC)=O', 'SC(C(C(O)=O)OC)=O',
-                               'SC(C*)=O',
-                               'SC(C(C)CC)=O', 'SC(C1C(CCC1)C(=O)O)=O',
-                               'SC(C)=O',
-                               'SC(C1=CC=CC=C1)=O', 'SC(CC(C)C)=O',
-                               'SC(C(C(=O)O)CC[Cl])=O']
-    starter_unit_error = 'SC(C1=CC=CC=C1)=O'
-    struct = read_smiles(starter_unit_error)
-    struct.add_attributes(ATTRIBUTES, boolean=True)
-    struct = attach_to_domain_pk(struct)
-    label_pk_central_chain(struct)
-    struct.print_graph()
-    for atom in struct.graph:
-        print(atom, atom.annotations.in_central_chain)
 
+        neighbours = last_backbone_atom.get_non_hydrogen_neighbours()[:]
+        for neighbour in last_backbone_atom.get_non_hydrogen_neighbours():
+            if neighbour in backbone:
+                neighbours.remove(neighbour)
+
+        if not neighbours:
+            endpoint = True
+
+        else:
+            # If the last backbone atom was the first ring member
+            if last_backbone_atom.in_ring(acid):
+                ring_members = last_backbone_atom.get_ring(acid)
+                outgoing_pairs = []
+                for atom in ring_members:
+                    for neighbour in atom.get_non_hydrogen_neighbours():
+                        if neighbour not in ring_members and neighbour not in backbone and not neighbour.in_ring(acid):
+                            outgoing_pairs.append((atom, neighbour))
+
+                if not outgoing_pairs:
+                    endpoint = True
+
+                else:
+                    longest_index = -1
+                    largest_subtree = 0
+                    best_shortest_path = None
+                    for i, pair in enumerate(outgoing_pairs):
+                        ring_atom, outgoing_atom = pair
+                        shortest_path = find_shortest_path_ring(ring_atom, last_backbone_atom, ring_members)
+                        subtree_size = acid.get_subtree_size(outgoing_atom, set(ring_members))
+                        if len(shortest_path) < 4 and subtree_size > largest_subtree:
+                            longest_index = i
+                            best_shortest_path = shortest_path
+
+                    if longest_index >= 0:
+
+                        backbone_ring_atom, next_backbone_atom = outgoing_pairs[longest_index]
+                        for atom in best_shortest_path:
+                            shortest_path_atom = acid.get_atom(atom)
+                            if shortest_path_atom not in backbone:
+                                shortest_path_atom.annotations.in_central_chain = True
+                                backbone.append(shortest_path_atom)
+                            next_backbone_atom = acid.get_atom(next_backbone_atom)
+                            next_backbone_atom.annotations.in_central_chain = True
+                            backbone.append(next_backbone_atom)
+                            last_backbone_atom = next_backbone_atom
+                    else:
+                        endpoint = True
+
+            else:
+                longest_index = -1
+                largest_subtree = 0
+
+                for i, neighbour in enumerate(neighbours):
+                    subtree_size = acid.get_subtree_size(neighbour, set(backbone))
+                    if subtree_size > largest_subtree:
+                        largest_subtree = subtree_size
+                        longest_index = i
+
+                if longest_index >= 0:
+                    next_backbone_atom = acid.get_atom(neighbours[longest_index])
+                else:
+                    next_backbone_atom = acid.get_atom(neighbours[0])
+
+                next_backbone_atom.annotations.in_central_chain = True
+                backbone.append(next_backbone_atom)
+                last_backbone_atom = next_backbone_atom
+
+
+def find_shortest_path_ring(atom_1, atom_2, atom_list):
+    max_distance = len(atom_list) // 2
+    atom_1_idx = None
+    atom_2_idx = None
+    for i, atom in enumerate(atom_list):
+        if atom == atom_1:
+            atom_1_idx = i
+        if atom == atom_2:
+            atom_2_idx = i
+
+    assert atom_1_idx is not None
+    assert atom_2_idx is not None
+
+    large_index = max([atom_1_idx, atom_2_idx])
+    small_index = min([atom_1_idx, atom_2_idx])
+
+    shortest_path = atom_list[small_index:large_index + 1]
+    if len(shortest_path) - 1 > max_distance:
+        shortest_path = atom_list[large_index:] + atom_list[:small_index + 1]
 
+    return shortest_path
```

### Comparing `raichu-0.0.2/raichu/class_domain.py` & `raichu-1.0.0/raichu/class_domain.py`

 * *Files 18% similar despite different names*

```diff
@@ -94,9 +94,32 @@
     sulphur = Atom('S', 1, None, 0, False)
     structure.add_bond(domain, sulphur, 'single', 0)
     structure.refine_structure()
 
     return structure
 
 
+def make_scaffold_peptide(type):
+    """
+    Returns a Domain of the input type containing the appropriate nr in the
+    Structure object
 
+    domain_type: Str, domain type
+    next_atom_nr: Int, 'atom nr' of the domain in the structure
+    """
+    structure = Structure()
 
+    domain = CarrierDomain('I', 0, None, 0, False)
+
+    structure.add_disconnected_atom(domain)
+    if type == "Follower":
+
+        oxygen = Atom('N', 1, None, 0, False)
+        structure.add_bond(domain, oxygen, 'single', 0)
+
+    if type == "Leader":
+
+        oxygen = Atom('O', 1, None, 0, False)
+        structure.add_bond(domain, oxygen, 'single', 0)
+    structure.refine_structure()
+    domain.annotations.set_annotation('domain_type', type)
+    return structure
```

### Comparing `raichu-0.0.2/raichu/data/substrate_to_abbreviation.txt` & `raichu-1.0.0/raichu/data/substrate_to_abbreviation.txt`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/raichu/data/trans_at.py` & `raichu-1.0.0/raichu/data/trans_at.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,26 +33,31 @@
                                           'LACST': [],
                                           'SHDB': [('DUMMY_KR', None), ('DUMMY_GDH', None)],
                                           'OUT': [],
                                           'BETA_OH': [('DUMMY_KR', None)],
                                           'ZDB': [('DUMMY_KR', None), ('DUMMY_ZDH', None)],
                                           'BETA_MEDB': [('DUMMY_KR', None), ('DUMMY_EDH', None),
                                                                      ('DUMMY_BMT', None)],
-                                          'TRANS_AT_PKS': [], 'OXA': [],
+                                          'MISCELLANEOUS': [], 'OXA': [],
                                           'ALPHAME_BETA_D_OH': [('DUMMY_ALMT', None), ('DUMMY_KR', 'A1')],
                                           'ALPHAME_BETAOH': [('DUMMY_AMT', None), ('DUMMY_KR', None)],
                                           'NON_ELONGATING_ALPHAME_EDB': [('DUMMY_AMT', None),
                                                                                       ('DUMMY_KR', None),
                                                                                       ('DUMMY_EDH', None)],
                                           'RED': [('DUMMY_KR', None), ('DUMMY_DH', None),
-                                                                   ('DUMMY_ER', None)]}
+                                                                   ('DUMMY_ER', None)],
+                                          "EXOMETHYLENE": [('DUMMY_AMT', None), ('DUMMY_EMO', None)],
+                                          'ALPHAME_ZDB': [('DUMMY_KR', None), ('DUMMY_ZDH', None), ('DUMMY_AMT', None)],
+                                          'ALPHA_D_ME_SHDB': [('DUMMY_KR', None), ('DUMMY_GDH', None), ('DUMMY_AMT', None)],
+                                          'ALPHAME_DB': [('DUMMY_KR', None), ('DUMMY_DH', None), ('DUMMY_AMT', None)],
+                                          'ALPHAME_KETO': [('DUMMY_AMT', None)],
+                                          'NON_ELONGATING_SHDB': [('DUMMY_KR', None), ('DUMMY_GDH', None)]}
+
 
-# TODO: Map all these SMILES to names, make Enums for them
 TRANSATOR_CLADE_TO_STARTER_SUBSTRATE = {'NON_ELONGATING_DB': 'ACETYL_COA',
-                                        # TODO: choose SMILES
                                         'BETA_OH_KETO': 'ACETYL_COA',
                                         'NON_ELONGATING_BETA_OH': 'ACETYL_COA',
                                         'ALPHA_OH': 'ACETYL_COA',
                                         'EDB': "ACETYL_COA",
                                         'ARST': 'PHENYLACETYLCOA', 'PYR': 'ACETYL_COA',
                                         'ALPHAME_EDB': "ACETYL_COA",
                                         'OXI': 'ACETYL_COA', 'AA': 'GLYCINE',
@@ -66,30 +71,36 @@
                                         'BETA_L_OH': "ACETYL_COA",
                                         'BR': 'ACETYL_COA',
                                         'ALPHABETA_OH': 'ACETYL_COA',
                                         'UNST': 'PROPIONYL_COA', 'ST': 'ACETYL_COA',
                                         'MEOST': 'METHOXYFORMYL_COA',
                                         'ACST': 'ACETYL_COA',
                                         'ALPHAME': 'ACETYL_COA',
-                                        'BETA_D_OME': "MACETYL_COA",
+                                        'BETA_D_OME': "ACETYL_COA",
                                         'NON_ELONGATING_PYR': 'ACETYL_COA',
                                         'BETA_ME': 'ACETYL_COA',
                                         'BETA_OH_EDB': 'ACETYL_COA',
                                         'NON_ELONGATING_OXA': 'ACETYL_COA',
                                         'LACST': 'LACTYL_COA',
                                         'SHDB': 'ACETYL_COA',
                                         'OUT': 'ACETYL_COA',
                                         'BETA_OH': "ACETYL_COA",
                                         'ZDB': 'ACETYL_COA',
                                         'BETA_MEDB': "ACETYL_COA",
-                                        'TRANS_AT_PKS': 'ACETYL_COA', 'OXA': 'ACETYL_COA',
+                                        'MISCELLANEOUS': 'ACETYL_COA', 'OXA': 'ACETYL_COA',
                                         'ALPHAME_BETA_D_OH': 'ACETYL_COA',
                                         'ALPHAME_BETAOH': 'ACETYL_COA',
                                         'NON_ELONGATING_ALPHAME_EDB': "ACETYL_COA",
-                                        'RED': 'ACETYL_COA'}
+                                        'RED': 'ACETYL_COA',
+                                        "EXOMETHYLENE": 'ACETYL_COA',
+                                        'ALPHAME_ZDB': 'ACETYL_COA',
+                                        'ALPHA_D_ME_SHDB': 'ACETYL_COA',
+                                        'ALPHAME_DB': 'ACETYL_COA',
+                                        'ALPHAME_KETO': 'ACETYL_COA',
+                                        'NON_ELONGATING_SHDB': 'ACETYL_COA'}
 
 TRANSATOR_CLADE_TO_ELONGATING = {'NON_ELONGATING_DB': False,
                                  'BETA_OH_KETO': True,
                                  'NON_ELONGATING_BETA_OH': False,
                                  'ALPHA_OH': True, 'EDB': True,
                                  'ARST': True, 'PYR': True,
                                  'ALPHAME_EDB': True, 'OXI': True,
@@ -104,12 +115,18 @@
                                  'ALPHAME': True, 'BETA_D_OME': True,
                                  'NON_ELONGATING_PYR': False,
                                  'BETA_ME': True, 'BETA_OH_EDB': True,
                                  'NON_ELONGATING_OXA': False,
                                  'LACST': True,
                                  'SHDB': True, 'OUT': True,
                                  'BETA_OH': True, 'ZDB': True,
-                                 'BETA_MEDB': True, 'TRANS_AT_PKS': True,
+                                 'BETA_MEDB': True, 'MISCELLANEOUS': True,
                                  'OXA': True, 'ALPHAME_BETA_D_OH': True,
                                  'ALPHAME_BETAOH': True,
                                  'NON_ELONGATING_ALPHAME_EDB': False,
-                                 'RED': True}
+                                 'RED': True,
+                                 "EXOMETHYLENE": True,
+                                 "ALPHAME_ZDB": True,
+                                 'ALPHA_D_ME_SHDB': True,
+                                 'ALPHAME_DB': True,
+                                 'ALPHAME_KETO': True,
+                                 'NON_ELONGATING_SHDB': False}
```

### Comparing `raichu-0.0.2/raichu/domain/domain.py` & `raichu-1.0.0/raichu/domain/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Union, Tuple
 from pikachu.chem.structure import Structure
 from pikachu.general import read_smiles
 from raichu.substrate import NRPSSubstrate, PKSSubstrate
-from raichu.reactions.pks_tailoring_reactions import ketoreduction, enoylreduction, dehydration, alpha_L_methyl_transferase,alpha_methyl_transferase,smallest_cyclisation,alpha_hydroxylase,gamma_beta_dehydratase,beta_hydroxy_methyl_transferase,beta_methyl_transferase
-from raichu.reactions.nrps_tailoring_reactions import epimerize, n_methylate
+from raichu.reactions.pks_tailoring_reactions import exo_methylen_oxidase, ketoreduction, enoylreduction, dehydration, alpha_L_methyl_transferase, alpha_methyl_transferase, smallest_cyclisation, alpha_hydroxylase, gamma_beta_dehydratase, beta_hydroxy_methyl_transferase, beta_methyl_transferase
+from raichu.reactions.nrps_tailoring_reactions import epimerize, n_methylate, nrps_cyclodehydration, nrps_oxidation
 from raichu.reactions.pks_elongation_reactions import pks_elongation
 from raichu.reactions.nrps_elongation_reactions import nrps_elongation
 from raichu.reactions.chain_release import release_linear_reduction, release_linear_thioesterase
 from raichu.domain.domain_types import DomainSuperClass, RecognitionDomainType, CarrierDomainType, \
     TailoringDomainType, SynthesisDomainType, TerminationDomainType, KSDomainSubtype, KRDomainSubtype, ERDomainSubtype
 
 from dataclasses import dataclass
 
 
 @dataclass
 class Domain:
     supertype: DomainSuperClass
     type: Union[TailoringDomainType, CarrierDomainType, SynthesisDomainType, RecognitionDomainType,
                 TerminationDomainType]
-    subtype: Union[None, KRDomainSubtype, KSDomainSubtype]
+    subtype: Union[None, KRDomainSubtype, KSDomainSubtype, ERDomainSubtype]
     domain_name: Union[str, None]
     active: bool = True
     gene: Union[str, None] = None
     used: bool = True
 
     def __post_init__(self):
         if self.domain_name is None:
@@ -63,47 +63,52 @@
 
         super().__init__(superclass, domain_type, domain_subtype, domain_name, active=active, used=used)
 
     def do_tailoring(self, structure) -> Tuple[Structure, bool]:
         """
         Performs tailoring reaction
         """
-        #STILL MISSING: E/Z-configured double bonds, E/Z-Gamma-beta-dehydrogenase
         if self.type.name == 'KR' or self.type.name == 'DUMMY_KR':
             return ketoreduction(structure, self.subtype)
         elif self.type.name == 'DH' or self.type.name == 'DUMMY_DH':
             return dehydration(structure)
         elif self.type.name == 'EDH' or self.type.name == 'DUMMY_EDH':
-            return dehydration(structure,"E")
+            return dehydration(structure, "E")
         elif self.type.name == 'ZDH' or self.type.name == 'DUMMY_ZDH':
-            return dehydration(structure,"Z")
+            return dehydration(structure, "Z")
         elif self.type.name == 'ER' or self.type.name == 'DUMMY_ER':
             return enoylreduction(structure, self.subtype)
         elif self.type.name == 'ALMT' or self.type.name == 'DUMMY_ALMT':
             return alpha_L_methyl_transferase(structure)
         elif self.type.name == 'AMT' or self.type.name == 'DUMMY_AMT':
             return alpha_methyl_transferase(structure)
         elif self.type.name == 'SC' or self.type.name == 'DUMMY_SC':
             return smallest_cyclisation(structure)
         elif self.type.name == 'AH' or self.type.name == 'DUMMY_AH':
             return alpha_hydroxylase(structure)
         elif self.type.name == 'GDH' or self.type.name == 'DUMMY_GDH':
             return gamma_beta_dehydratase(structure)
         elif self.type.name == 'EGDH' or self.type.name == 'DUMMY_EGDH':
-            return gamma_beta_dehydratase(structure,"E")
+            return gamma_beta_dehydratase(structure, "E")
         elif self.type.name == 'ZGDH' or self.type.name == 'DUMMY_ZGDH':
-            return gamma_beta_dehydratase(structure,"Z")
+            return gamma_beta_dehydratase(structure, "Z")
         elif self.type.name == 'OMT' or self.type.name == 'DUMMY_OMT':
             return beta_hydroxy_methyl_transferase(structure)
         elif self.type.name == 'BMT' or self.type.name == 'DUMMY_BMT':
             return beta_methyl_transferase(structure)
+        elif self.type.name == 'EMO' or self.type.name == 'DUMMY_EMO':
+            return exo_methylen_oxidase(structure)
         elif self.type.name == 'E':
             return epimerize(structure)
         elif self.type.name == 'nMT':
             return n_methylate(structure)
+        elif self.type.name == 'CYC':
+            return nrps_cyclodehydration(structure)
+        elif self.type.name == 'OX':
+            return nrps_oxidation(structure)
         else:
             raise Warning(f"Tailoring domain {self.domain_name} not recognised by RAIChU. Ignored.")
 
 
 class SynthesisDomain(Domain):
     def __init__(self, domain_type: str, domain_subtype: Union[str, None] = None, active: bool = True,
                  domain_name: Union[str, None] = None, is_elongating: bool = True,
@@ -124,39 +129,42 @@
         """
         Performs elongation reaction
         """
         if self.type.name == 'C' or self.type.name == "DUMMY_C":
             if self.is_elongating:
                 building_block = read_smiles(substrate.smiles)
                 return nrps_elongation(building_block, structure)
+            else:
+                return structure
         elif self.type.name == 'KS' or self.type.name == "DUMMY_KS":
             if self.is_elongating:
                 if self.subtype is None or self.subtype.name in [v.name for v in KSDomainSubtype]:
                     building_block = substrate.elongation_monomer
                     return pks_elongation(structure, building_block)
                 else:
                     raise ValueError(f"RAIChU does not support domain subtype {self.subtype.name}")
+            else:
+                return structure
         else:
             raise ValueError(f"Unknown type of synthesis domain: {self.type}")
 
 
 class RecognitionDomain(Domain):
     def __init__(self, domain_type: str, substrate_name: str, domain_subtype: Union[str, None] = None,
                  active: bool = True, domain_name: Union[str, None] = None, used: bool = True) -> None:
 
         superclass = DomainSuperClass.from_string("RECOGNITION")
         domain_type = RecognitionDomainType.from_string(domain_type)
 
-
         if domain_subtype is not None:
             raise ValueError(f"RAIChU does not support domain subtypes for {domain_type.name}")
 
         super().__init__(superclass, domain_type, domain_subtype, domain_name, active=active, used=used)
 
-        if self.type.name == 'A' or self.type.name == 'DUMMY_A':
+        if self.type.name == 'A' or self.type.name == 'DUMMY_A' or self.type.name == 'CAL':
             self.substrate = NRPSSubstrate(substrate_name)
         elif self.type.name == 'AT' or self.type.name == 'DUMMY_AT':
             self.substrate = PKSSubstrate(substrate_name)
         else:
             raise ValueError(f"Unknown type of recognition domain: {self.type}")
 
     @property
```

### Comparing `raichu-0.0.2/raichu/domain/domain_types.py` & `raichu-1.0.0/raichu/domain/domain_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     """
     An Enum representing the types of recognition domains supported by RAIChU
     """
     A = 1
     AT = 2
     DUMMY_A = 3
     DUMMY_AT = 4
+    CAL = 5
 
     @staticmethod
     def from_string(label: str) -> "RecognitionDomainType":
         for value in RecognitionDomainType:
             if str(value.name) == label:
                 return value
         raise ValueError(f"Unknown recognition domain type: {label}")
@@ -115,14 +116,17 @@
     DUMMY_OMT = 17 #Beta-Hydroxymethyltransferase
     DUMMY_BMT = 18 #Beta-Methyltransferase
     DUMMY_ER = 19
     DUMMY_KR = 20
     DUMMY_DH = 21
     DUMMY_E = 22
     DUMMY_nMT = 23
+    CYC = 24
+    OX = 25
+    DUMMY_EMO = 26
 
     @staticmethod
     def from_string(label: str) -> "TailoringDomainType":
         for value in TailoringDomainType:
             if str(value.name) == label:
                 return value
         raise ValueError(f"Unknown tailoring domain type: {label}")
@@ -181,27 +185,33 @@
     BETA_ME = 25
     EDB = 26
     BETA_MEDB = 27
     NON_ELONGATING_DB = 28
     ALPHAME_EDB = 29
     ALPHAME = 30
     ALPHAME_BETA_L_OH = 31
-    TRANS_AT_PKS = 32
-    AA = 33
-    DB = 34
-    RED = 35
-    PYR = 36
-    ALPHAME_BETA_D_OH = 37
-    NON_ELONGATING = 38
-    MEOST = 39
-    BETA_L_OH = 40
-    ZDB = 41
-    KETO = 42
-    ALPHA_OH = 43
-    NON_ELONGATING_PYR = 44
+    AA = 32
+    DB = 33
+    RED = 34
+    PYR = 35
+    ALPHAME_BETA_D_OH = 36
+    NON_ELONGATING = 37
+    MEOST = 38
+    BETA_L_OH = 39
+    ZDB = 40
+    KETO = 41
+    ALPHA_OH = 42
+    NON_ELONGATING_PYR = 43
+    MISCELLANEOUS = 44
+    EXOMETHYLENE = 45
+    ALPHAME_ZDB = 46
+    ALPHA_D_ME_SHDB = 47
+    ALPHAME_DB = 48
+    ALPHAME_KETO = 49
+    NON_ELONGATING_SHDB = 50
 
     @staticmethod
     def from_string(label: str) -> "KSDomainSubtype":
         for value in KSDomainSubtype:
             if str(value.name) == label:
                 return value
         raise ValueError(f"Unknown KS domain subtype: {label}")
```

### Comparing `raichu-0.0.2/raichu/drawing/bubbles.py` & `raichu-1.0.0/raichu/drawing/bubbles.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-
-from raichu.drawing.colours import OUTLINE_COLOURS, FILL_COLOURS, DOMAIN_ABBREVIATIONS, TRANSPARENT_OUTLINE_COLOURS, \
-    TRANSPARENT_FILL_COLOURS, TRANSPARENT_TEXT_COLOURS, TEXT_COLOUR
+from raichu.drawing.colours import (
+    OUTLINE_COLOURS,
+    FILL_COLOURS,
+    DOMAIN_ABBREVIATIONS,
+    TRANSPARENT_OUTLINE_COLOURS,
+    TRANSPARENT_FILL_COLOURS,
+    TRANSPARENT_TEXT_COLOURS,
+    TEXT_COLOUR,
+)
 
 
 def make_circle(x_coord, y_coord, domain):
     """Easy function to draw circle for the domain visualization. Returns
     matplotlib.patches.circle object of a circle with radius 4
 
     x_coord: int, x-coordinate of the center of the circle to be drawn
@@ -18,16 +24,18 @@
         outline_colour = TRANSPARENT_OUTLINE_COLOURS[domain.type.name]
 
     circle = f"""<circle r="14" cx="{int(x_coord)}" cy="{int(y_coord)}" stroke="{outline_colour}"
        fill="{colour}" stroke-width="1"/>"""
     return circle
 
 
-def draw_rectangle(gene_name, x, y, width, height=12, text_colour='white'):
-    rectangle = f"""<rect x="{x}" y="{y}" width="{width}" height="{height}" fill="black" />"""
+def draw_rectangle(gene_name, x, y, width, height=12, text_colour="white"):
+    rectangle = (
+        f"""<rect x="{x}" y="{y}" width="{width}" height="{height}" fill="black" />"""
+    )
     text_x = x + width / 2
     text_y = y + height / 2
     text = f"""<text x="{text_x}" y="{text_y}" fill="{text_colour}" text-anchor="middle" font-family="verdana" font-size = "{8}">\
 <tspan y="{text_y}" dy="0.35em">{gene_name}</tspan></text>"""
 
     svg_rect = f"""<g id="gene_banner_{gene_name}">"""
     svg_rect += rectangle
@@ -41,15 +49,15 @@
     line = f"""<line x1="{start_x}" x2="{end_x}" y1="{y}" y2="{y}" stroke-width="2" stroke="black" />"""
     return line
 
 
 def make_module_text(start_x, end_x, y, module_nr, offset_1=True):
     if offset_1:
         module_nr += 1
-    text_x = start_x + (end_x - start_x)/2
+    text_x = start_x + (end_x - start_x) / 2
     text = f"""<text x="{text_x}" y="{y}" fill="'black" text-anchor="middle" font-family="verdana" font-size = "{12}">\
 <tspan y="{y}" dy="0.35em">Module {module_nr}</tspan></text>"""
     return text
 
 
 def draw_bubbles(cluster, widths, delta_x=29, bubble_height=80, min_gene_padding=20, min_module_padding=10):
     x = 30.0
@@ -59,63 +67,81 @@
     cp_positions_bubbles = []
     previous_space_right = 0.0
     previous_cp_position = 0.0
 
     for i, module in enumerate(cluster.modules):
         current_y = bubble_height
         for j, domain in enumerate(module.domains):
+
+            # Take note of whether the domain is part of a new gene (modules can be split across multiple genes)
             new_gene = False
             if j < len(module.domains) - 1:
                 current_gene = domain.gene
                 next_gene = module.domains[j + 1].gene
                 if current_gene != next_gene:
                     new_gene = True
 
-            if domain.supertype.name == 'UNKNOWN' or domain.supertype.name == 'TAILORING':
+            # Move up bubbles representing unknown and tailoring domains
+
+            if domain.supertype.name == "UNKNOWN" or domain.supertype.name == "TAILORING":
 
                 if current_y == bubble_height - 7:
                     level_change = False
                 else:
                     level_change = True
 
                 current_y = bubble_height - 7
+
             else:
                 if current_y == bubble_height:
                     level_change = False
                 else:
                     level_change = True
                 current_y = bubble_height
 
+            # If there is a level change, you can place the bubble closer to the previous one
+
             if level_change and j != 0:
                 x_bubbles -= 1
                 x -= 1
 
-            if domain.supertype.name == "CARRIER" and domain.used:
+            # Only note the position of the cp domain if the module is not broken
+
+            if domain.supertype.name == "CARRIER" and domain.used and not module.is_broken:
                 cp_positions_bubbles.append(x_bubbles)
 
+                # Record how much space the structures take up left and right
+
                 current_space_left, current_space_right = widths[i]
 
                 minimum_x = previous_cp_position + current_space_left + previous_space_right
 
+                # If structures take up more space than the bubbles, shift the CP domain to the right
+
                 x = max([minimum_x, x])
                 cp_positions.append(x)
                 previous_space_right = current_space_right
                 previous_cp_position = x
 
             x_bubbles += delta_x
             x += delta_x
+
+            # If a new gene is introduced, move the bubbles over
+
             if new_gene:
                 x_bubbles += min_gene_padding
                 x += min_gene_padding
 
         x += min_module_padding
         x_bubbles += min_module_padding
 
     module_shifts = []
 
+    # Calculate how much each module has to shift
+
     for i, cp_position in enumerate(cp_positions):
         module_shift = cp_positions[i] - cp_positions_bubbles[i]
         for shift in module_shifts:
             module_shift -= shift
         module_shifts.append(module_shift)
 
     if module_shifts:
@@ -132,23 +158,29 @@
     current_gene = None
     gene_start = 0
     gene_end = 0
     gene_rects = []
     genes = []
     module_texts = []
 
+    correct_modules = 0
+
     for i, module in enumerate(cluster.modules):
+
         start_x = current_x - 15
         current_y = bubble_height
+
         for j, domain in enumerate(module.domains):
             if domain.gene not in genes:
                 genes.append(domain.gene)
             if current_gene and domain.gene != current_gene:
                 width = gene_end - gene_start
-                gene_rects.append(draw_rectangle(current_gene, gene_start, bubble_height - 75, width))
+                gene_rects.append(
+                    draw_rectangle(current_gene, gene_start, bubble_height - 75, width)
+                )
                 gene_start = current_x - 15
             elif not current_gene:
                 gene_start = current_x - 15
 
             current_gene = domain.gene
 
             new_gene = False
@@ -157,17 +189,20 @@
                 if current_gene != next_gene:
                     new_gene = True
 
             abbreviation = DOMAIN_ABBREVIATIONS.get(domain.type.name)
             if abbreviation is None:
                 abbreviation = DOMAIN_ABBREVIATIONS.get(domain.domain_name)
                 if abbreviation is None:
-                    abbreviation = ''
+                    abbreviation = ""
 
-            if domain.supertype.name == 'UNKNOWN' or domain.supertype.name == 'TAILORING':
+            if (
+                domain.supertype.name == "UNKNOWN"
+                or domain.supertype.name == "TAILORING"
+            ):
                 if current_y == bubble_height - 7:
                     level_change = False
                 else:
                     level_change = True
 
                 current_y = bubble_height - 7
             else:
@@ -200,28 +235,37 @@
 
                 current_x += min_gene_padding
 
         # Shift modules based on width of structures
 
         module_shift = 0.0
 
-        if i != len(cluster.modules) - 1:
-            module_shift = module_shifts[i + 1]
+        if not cluster.modules[i].is_broken:
+            correct_modules += 1
+
+        if i != len(cluster.modules) - 1 and not cluster.modules[i + 1].is_broken:
+
+            module_shift = module_shifts[correct_modules]
 
         end_x = current_x - 15
-        lines.append(draw_line(start_x, end_x, y=bubble_height - 26))
-        module_texts.append(make_module_text(start_x, end_x, bubble_height - 34, i))
 
-        current_x += (min_module_padding + module_shift)
+        if not cluster.modules[i].is_broken:
+
+            lines.append(draw_line(start_x, end_x, y=bubble_height - 26))
+            module_texts.append(make_module_text(start_x, end_x, bubble_height - 34, correct_modules - 1))
+
+        current_x += min_module_padding + module_shift
 
     if gene_start and gene_end:
         width = gene_end - gene_start
-        gene_rects.append((draw_rectangle(current_gene, gene_start, bubble_height - 75, width)))
+        gene_rects.append(
+            (draw_rectangle(current_gene, gene_start, bubble_height - 75, width))
+        )
 
-    svg = ''
+    svg = ""
 
     svg += f"""<g id="domain_circles">\n"""
     for i, circle in enumerate(circles):
         text = texts[i]
         svg += f"""<g id="domain_bubble_{i}">\n"""
         svg += f"{circle}\n"
         svg += f"{text}\n"
@@ -239,13 +283,7 @@
         module_text = module_texts[i]
         svg += f"{line}\n"
         svg += f"{module_text}\n"
         svg += "</g>\n"
     svg += "</g>\n"
 
     return svg, cp_positions, current_x
-
-
-
-
-
-
```

### Comparing `raichu-0.0.2/raichu/drawing/drawer.py` & `raichu-1.0.0/raichu/drawing/drawer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,43 @@
+from collections import OrderedDict
+from typing import Optional, List, Tuple, Dict, Set, Union
+
 from pikachu.drawing.drawing import *
 from pikachu.math_functions import *
-from pikachu.smiles.smiles import Smiles
+from pikachu.chem.atom import Atom
+from pikachu.chem.bond import Bond
+
+from raichu.central_chain_detection.find_central_chain import find_central_chain, find_central_chain_not_attached, \
+    find_central_chain_ripp, reorder_central_chain
+from raichu.central_chain_detection.label_central_chain import label_ripp_central_chain
+
 
-from raichu.central_chain_detection.find_central_chain import find_central_chain
+def get_ring(atom, structure):
+    cycles = structure.cycles.all_cycles
+
+    for i, cycle in enumerate(cycles):
+        if atom in cycle:
+            return cycle
+
+    return None
 
 
 class RaichuDrawer(Drawer):
     def __init__(self, structure, options=None, save_png=None, dont_show=False,
-                 coords_only=True, dpi=100, save_svg=None):
+                 coords_only=True, dpi=100, save_svg=None, draw_Cs_in_pink=False, add_url=False, horizontal=False,
+                 ripp=False, make_linear=True):
         self.dont_show = dont_show
         self.dpi = dpi
+        self.draw_Cs_in_pink = draw_Cs_in_pink
+        self.add_url = add_url
+        self.horizontal = horizontal
+        self.ripp = ripp
+        self.make_linear = make_linear
+        self.line_width = 2
+
         if options is None:
             self.options = Options()
         else:
             self.options = options
         if save_png is None:
             self.save_png = None
         else:
@@ -27,345 +51,266 @@
             assert save_svg.endswith('.svg')
             self.save_svg = save_svg
         super().__init__(structure, options=None, coords_only=coords_only)
 
     def center_on_carrier_domain(self):
         pass
 
-    def export_to_json(self):
-        json_structure = {"atoms": [],
-                          "bonds": [],
-                          "modules": []}
-
-        ring_centers_x = []
-        ring_centers_y = []
-
-        for ring in self.rings:
-            self.set_ring_center(ring)
-
-            ring_centers_x.append(ring.center.x)
-            ring_centers_y.append(ring.center.y)
-
-        for bond_nr, bond in self.structure.bonds.items():
-            if bond.atom_1.draw.positioned and bond.atom_2.draw.positioned:
-                json_bond = {"id": bond.nr,
-                             "atom_1": bond.atom_1.nr,
-                             "atom_2": bond.atom_2.nr,
-                             "type": bond.type,
-                             "chiral": False,
-                             "lines": []}
-
-                if bond in self.chiral_bonds:
-
-                    orientation, chiral_center = self.chiral_bond_to_orientation[bond]
-                    json_bond["chiral"] = True
-                    json_bond["wedge_orientation"] = orientation
-                    json_bond["wedge_origin"] = chiral_center.nr
-                elif (bond.atom_1.type == 'S' and bond.atom_2.annotations.domain_type or \
-                      (bond.atom_2.type == 'S' and bond.atom_1.annotations.domain_type)):
-                    json_bond["type"] = "squiggle"
-
-        # If the starter unit contains an unknown moiety, number this R1
-        for atom in self.structure.graph:
-            if atom.type == '*' and not atom.annotations.unknown_index:
-                atom.annotations.unknown_index = 1
-        for atom in self.structure.graph:
-            if atom.draw.positioned:
-                json_atom = {"id": atom.nr,
-                             "type": atom.type,
-                             "text": '',
-                             "atom_x": atom.draw.position.x,
-                             "atom_y": atom.draw.position.y}
-
-                if atom.type != 'C' and atom.draw.positioned:
-                    text_h = ''
-                    text_h_pos = None
-
-                    if atom.type != 'C' or atom.draw.draw_explicit:
-                        text = atom.type
+    def find_clashing_atoms(self) -> List[Tuple[Atom, Atom]]:
+        clashing_atoms = []
+        for i, atom_1 in enumerate(self.drawn_atoms):
+            for j in range(i + 1, len(self.drawn_atoms)):
+                atom_2 = self.drawn_atoms[j]
+                if not self.structure.bond_exists(atom_1, atom_2):
+                    distance = Vector.subtract_vectors(atom_1.draw.position, atom_2.draw.position).get_squared_length()
+                    if atom_1.has_neighbour('H') and atom_2.has_neighbour('H') and atom_1.type != 'C' and \
+                            atom_2.type != 'C':
+                        max_distance = self.options.bond_length_squared * 1.5
+                    # elif atom_1.has_neighbour('H') or atom_2.has_neighbour('H'):
+                    #     max_distance = self.options.bond_length_squared / 1.5
                     else:
-                        text = ''
-
-                    if atom.annotations.domain_type:
-                        text = atom.annotations.domain_type
-
-                    horizontal_alignment = 'center'
-
-                    orientation = self.get_hydrogen_text_orientation(atom)
-                    if orientation == 'H_above_atom':
-                        text_h_pos = Vector(atom.draw.position.x, atom.draw.position.y + 6)
-                    if orientation == 'H_below_atom':
-                        text_h_pos = Vector(atom.draw.position.x, atom.draw.position.y - 6)
-
-                    atom_draw_position = Vector(atom.draw.position.x, atom.draw.position.y)
-
-                    if atom.type == '*':
-                        neighbouring_c = atom.get_neighbour('C')
-                        assert neighbouring_c
-                        # In order to not let the number of the sidechain overlap
-                        # with the bond, move Rx symbol along hor. axis depending on
-                        # if group is added to the left or right of the chain
-                        delta_x_r = self.get_delta_x_sidechain(atom, neighbouring_c)
-                        atom_draw_position.x += delta_x_r
-                        text = fr'$R_{atom.annotations.unknown_index}$'
-
-                    if not atom.charge and (atom.type != 'C' or atom.draw.draw_explicit):
-
-                        if atom.draw.has_hydrogen:
-                            hydrogen_count = 0
-                            for neighbour in atom.neighbours:
-                                if neighbour.type == 'H' and not neighbour.draw.is_drawn:
-                                    hydrogen_count += 1
-
-                            if hydrogen_count:
-
-                                if hydrogen_count > 1:
-                                    if orientation == 'H_before_atom':
-                                        text = r'$H_{hydrogens}{atom_type}$'.format(hydrogens=hydrogen_count,
-                                                                                    atom_type=atom.type)
-                                        horizontal_alignment = 'right'
-                                        atom_draw_position.x += 3
-                                    elif orientation == 'H_below_atom' or orientation == 'H_above_atom':
-                                        text = atom.type
-                                        text_h = r'$H_{hydrogens}$'.format(hydrogens=hydrogen_count)
-
-                                    else:
-                                        text = r'${atom_type}H_{hydrogens}$'.format(hydrogens=hydrogen_count,
-                                                                                    atom_type=atom.type)
-                                        horizontal_alignment = 'left'
-                                        atom_draw_position.x -= 3
-                                elif hydrogen_count == 1:
-                                    if orientation == 'H_before_atom':
-                                        text = f'H{atom.type}'
-                                        horizontal_alignment = 'right'
-                                        atom_draw_position.x += 3
-                                    elif orientation == 'H_below_atom' or orientation == 'H_above_atom':
-                                        text = atom.type
-                                        text_h = 'H'
-                                    else:
-                                        text = f'{atom.type}H'
-                                        horizontal_alignment = 'left'
-                                        atom_draw_position.x -= 3
-
-                    elif atom.charge:
-                        if atom.charge > 0:
-                            charge_symbol = '+'
-                        else:
-                            charge_symbol = '-'
-
-                        hydrogen_count = 0
-                        for neighbour in atom.neighbours:
-                            if neighbour.type == 'H' and not neighbour.draw.is_drawn:
-                                hydrogen_count += 1
-
-                        if not hydrogen_count:
-
-                            if abs(atom.charge) > 1:
-
-                                text = r'${atom_type}^{charge}{charge_symbol}$'.format(charge=atom.charge,
-                                                                                       atom_type=atom.type,
-                                                                                       charge_symbol=charge_symbol)
-                            elif abs(atom.charge) == 1:
-                                text = r'${atom_type}^{charge_symbol}$'.format(atom_type=atom.type,
-                                                                               charge_symbol=charge_symbol)
-
-                            horizontal_alignment = 'left'
-                            atom_draw_position.x -= 3
-                        else:
-
-                            if hydrogen_count > 1:
-                                if orientation == 'H_before_atom':
-                                    if abs(atom.charge) > 1:
-                                        text = r'$H_{hydrogens}{atom_type}^{charge}{charge_symbol}$'.format(
-                                            hydrogens=hydrogen_count,
-                                            atom_type=atom.type,
-                                            charge=atom.charge,
-                                            charge_symbol=charge_symbol)
-                                    elif abs(atom.charge) == 1:
-                                        text = r'$H_{hydrogens}{atom_type}^{charge_symbol}$'.format(
-                                            hydrogens=hydrogen_count,
-                                            atom_type=atom.type,
-                                            charge_symbol=charge_symbol)
-
-                                    horizontal_alignment = 'right'
-                                    atom_draw_position.x += 3
-                                elif orientation == 'H_above_atom' or orientation == 'H_below_atom':
-                                    text_h = r'$H_{hydrogens}$'.format(hydrogens=hydrogen_count)
-                                    if abs(atom.charge) > 1:
-                                        text = r'${atom_type}^{charge}{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                               charge=atom.charge,
-                                                                                               charge_symbol=charge_symbol)
-                                    elif abs(atom.charge) == 1:
-                                        text = r'${atom_type}^{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                       charge_symbol=charge_symbol)
-                                else:
-                                    if abs(atom.charge) > 1:
-                                        text = r'${atom_type}H_{hydrogens}^{charge}{charge_symbol}$'.format(
-                                            hydrogens=hydrogen_count,
-                                            atom_type=atom.type,
-                                            charge=atom.charge,
-                                            charge_symbol=charge_symbol)
-                                    elif abs(atom.charge) == 1:
-                                        text = r'${atom_type}H_{hydrogens}^{charge_symbol}$'.format(
-                                            hydrogens=hydrogen_count,
-                                            atom_type=atom.type,
-                                            charge_symbol=charge_symbol)
-
-                                    horizontal_alignment = 'left'
-                                    atom_draw_position.x -= 3
-                            elif hydrogen_count == 1:
-                                if orientation == 'H_before_atom':
-                                    if abs(atom.charge) > 1:
-
-                                        text = r'$H{atom_type}^{charge}{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                                charge=atom.charge,
-                                                                                                charge_symbol=charge_symbol)
-                                    elif abs(atom.charge) == 1:
-                                        text = r'$H{atom_type}^{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                        charge_symbol=charge_symbol)
-                                    horizontal_alignment = 'right'
-                                    atom_draw_position.x += 3
-                                elif orientation == 'H_above_atom' or orientation == 'H_below_atom':
-                                    text_h = 'H'
-                                    if abs(atom.charge) > 1:
-
-                                        text = r'${atom_type}^{charge}{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                               charge=atom.charge,
-                                                                                               charge_symbol=charge_symbol)
-                                    elif abs(atom.charge) == 1:
-                                        text = r'${atom_type}^{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                       charge_symbol=charge_symbol)
-
-                                else:
-                                    if abs(atom.charge) > 1:
-                                        text = r'${atom_type}H^{charge}{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                                charge=atom.charge,
-                                                                                                charge_symbol=charge_symbol)
-
-                                    elif abs(atom.charge) == 1:
-                                        text = r'${atom_type}H^{charge_symbol}$'.format(atom_type=atom.type,
-                                                                                        charge_symbol=charge_symbol)
-                                    horizontal_alignment = 'left'
-                                    atom_draw_position.x -= 3
-
-                    if text:
-                        plt.text(atom_draw_position.x, atom_draw_position.y,
-                                 text,
-                                 horizontalalignment=horizontal_alignment,
-                                 verticalalignment='center',
-                                 color=atom.draw.colour)
-                    if text_h:
-                        plt.text(text_h_pos.x, text_h_pos.y,
-                                 text_h,
-                                 horizontalalignment='center',
-                                 verticalalignment='center',
-                                 color=atom.draw.colour)
-
-        # If a png filename is included in the initialization of the
-        # Raichu_drawer object, don't show the structure, but do save it as a
-        # png image to the provided filename
-        if self.dont_show:
-            return self
-
-        elif self.save_png is None and not self.dont_show and self.save_svg is None:
-            plt.show()
-
-        else:
-            if self.save_png:
-                plt.savefig(self.save_png)
-            elif self.save_svg:
-                plt.savefig(self.save_svg)
-            plt.clf()
-            plt.close()
+                        max_distance = self.options.bond_length_squared / 2
+                    if distance <= max_distance:
+                        clashing_atoms.append((atom_1, atom_2))
+
+        return clashing_atoms
+    
+    def find_out_of_bound_atoms(self, minimum_y) -> List[Atom]:
+        clashing_atoms = []
+        for i, atom in enumerate(self.drawn_atoms):
+            if atom.draw.position.y < minimum_y and atom.type != 'I':
+                clashing_atoms.append(atom)
+        return clashing_atoms
 
+    # TODO: add an option in pikachu Options object to set the min bond distance between which to consider fine-tuning
     def finetune_overlap_resolution(self, masked_bonds=None, highest_atom=None):
 
         if not masked_bonds:
             masked_bonds = set()
 
         else:
             masked_bonds = set(masked_bonds)
 
-        if self.total_overlap_score > self.options.overlap_sensitivity:
-            clashing_atoms = self.find_clashing_atoms()
+        # if self.total_overlap_score > self.options.overlap_sensitivity:
+        clashing_atoms = self.find_clashing_atoms()
 
-            best_bonds = []
-            for atom_1, atom_2 in clashing_atoms:
-                shortest_path = self.find_shortest_path(atom_1, atom_2)
-                rotatable_bonds = []
-                distances = []
+        best_bonds = []
+        for atom_1, atom_2 in clashing_atoms:
 
-                for i, bond in enumerate(shortest_path):
-                    distance_1 = i
-                    distance_2 = len(shortest_path) - i
+            shortest_path = self.find_shortest_path(atom_1, atom_2)
+            rotatable_bonds = []
+            distances = []
+
+            for i, bond in enumerate(shortest_path):
+                distance_1 = i
+                distance_2 = len(shortest_path) - i
+
+                average_distance = len(shortest_path) / 2
+
+                distance_metric = abs(
+                    average_distance - distance_1) + abs(average_distance - distance_2)
+
+                if self.bond_is_rotatable(bond) and bond not in masked_bonds:
+                    rotatable_bonds.append(bond)
+                    distances.append(distance_metric)
+
+            best_bond = None
+            optimal_distance = float('inf')
+            for i, distance in enumerate(distances):
+                if distance < optimal_distance:
+                    # if highest_atom:
+                    #     if atom_1.draw.position.y < highest_atom.draw.position.y and \
+                    #             atom_2.draw.position.y < highest_atom.draw.position.y:
+                    #         best_bond = rotatable_bonds[i]
+                    #         optimal_distance = distance
+                    # else:
+                        best_bond = rotatable_bonds[i]
+                        optimal_distance = distance
+
+            if best_bond:
+                best_bonds.append(best_bond)
+
+        best_bonds = list(set(best_bonds))
+
+        for best_bond in best_bonds:
+            if self.total_overlap_score > self.options.overlap_sensitivity:
+
+                subtree_size_1 = self.get_subgraph_size(
+                    best_bond.atom_1, {best_bond.atom_2})
+                subtree_size_2 = self.get_subgraph_size(
+                    best_bond.atom_2, {best_bond.atom_1})
+
+                if subtree_size_1 < subtree_size_2:
+                    rotating_atom = best_bond.atom_1
+                    parent_atom = best_bond.atom_2
+                else:
+                    rotating_atom = best_bond.atom_2
+                    parent_atom = best_bond.atom_1
 
-                    average_distance = len(shortest_path) / 2
+                overlap_score, _, _ = self.get_overlap_score()
 
-                    distance_metric = abs(average_distance - distance_1) + abs(average_distance - distance_2)
+                self.rotate_subtree(rotating_atom, parent_atom, math.radians(
+                    15), parent_atom.draw.position)
 
-                    if self.bond_is_rotatable(bond) and bond not in masked_bonds:
-                        rotatable_bonds.append(bond)
-                        distances.append(distance_metric)
+                new_overlap_score, _, _ = self.get_overlap_score()
 
-                best_bond = None
-                optimal_distance = float('inf')
-                for i, distance in enumerate(distances):
-                    if distance < optimal_distance:
-                        if highest_atom:
-                            if not atom_1.draw.position.x > highest_atom.draw.position.x and atom_2.draw.position.x > highest_atom.draw.position.x:
-                                best_bond = rotatable_bonds[i]
-                                optimal_distance = distance
-                        else:
-                            best_bond = rotatable_bonds[i]
-                            optimal_distance = distance
+                scores = [new_overlap_score]
 
-                if best_bond:
-                    best_bonds.append(best_bond)
+                for i in range(12):
+                    self.rotate_subtree(rotating_atom, parent_atom, math.radians(
+                        30), parent_atom.draw.position)
+                    new_overlap_score, _, _ = self.get_overlap_score()
+                    scores.append(new_overlap_score)
 
-            best_bonds = list(set(best_bonds))
+                assert len(scores) == 13
+                scores = scores[:12]
 
-            for best_bond in best_bonds:
-                if self.total_overlap_score > self.options.overlap_sensitivity:
+                best_i = 0
+                best_score = scores[0]
 
-                    subtree_size_1 = self.get_subgraph_size(best_bond.atom_1, {best_bond.atom_2})
-                    subtree_size_2 = self.get_subgraph_size(best_bond.atom_2, {best_bond.atom_1})
+                for i, score in enumerate(scores):
+                    if score < best_score:
+                        best_score = score
+                        best_i = i
 
-                    if subtree_size_1 < subtree_size_2:
-                        rotating_atom = best_bond.atom_1
-                        parent_atom = best_bond.atom_2
-                    else:
-                        rotating_atom = best_bond.atom_2
-                        parent_atom = best_bond.atom_1
+                self.total_overlap_score = best_score
 
-                    overlap_score, _, _ = self.get_overlap_score()
+                self.rotate_subtree(rotating_atom, parent_atom, math.radians(
+                    30 * best_i + 1), parent_atom.draw.position)
+    
+    def finetune_overlap_bubbles(self, masked_bonds=None, highest_atom=None):
 
-                    scores = [overlap_score]
-
-                    for i in range(12):
-                        self.rotate_subtree(rotating_atom, parent_atom, math.radians(30), parent_atom.draw.position)
-                        new_overlap_score, _, _ = self.get_overlap_score()
-                        scores.append(new_overlap_score)
+        if not masked_bonds:
+            masked_bonds = set()
 
-                    assert len(scores) == 13
+        else:
+            masked_bonds = set(masked_bonds)
 
-                    scores = scores[:12]
+        domain = None
+        
+        # Find minimum y
 
-                    best_i = 0
-                    best_score = scores[0]
+        for atom in self.structure.graph:
+            if atom.type == 'I':
+                if atom.annotations.domain_type in ["Leader", "Follower", "ACP", "PCP"]:
+                    domain = atom
+        # Add also padding for hydrogens drawn as a atom label but not as an explicit hydrogen (e.g. HN)
+        assert domain is not None
+
+        minimum_y = domain.draw.position.y + 5
+        
+        clashing_atoms = self.find_out_of_bound_atoms(minimum_y)
+
+        best_bonds = []
+        for atom_1 in clashing_atoms:
+
+            shortest_path = self.find_shortest_path(atom_1, domain)
+            rotatable_bonds = []
+            distances = []
+
+            for i, bond in enumerate(shortest_path):
+                distance_1 = i
+                distance_2 = len(shortest_path) - i
+
+                average_distance = len(shortest_path) / 2
+
+                distance_metric = abs(
+                    average_distance - distance_1) + abs(average_distance - distance_2)
+
+                if self.bond_is_rotatable(bond) and bond not in masked_bonds:
+                    rotatable_bonds.append(bond)
+                    distances.append(distance_metric)
+
+            best_bond = None
+            optimal_distance = float('inf')
+            for i, distance in enumerate(distances):
+                if distance < optimal_distance:
+                    # if highest_atom:
+                    #     if atom_1.draw.position.y < highest_atom.draw.position.y and \
+                    #             atom_2.draw.position.y < highest_atom.draw.position.y:
+                    #         best_bond = rotatable_bonds[i]
+                    #         optimal_distance = distance
+                    # else:
+                    best_bond = rotatable_bonds[i]
+                    optimal_distance = distance
+
+            if best_bond:
+                best_bonds.append(best_bond)
+
+        best_bonds = list(set(best_bonds))
+
+        for best_bond in best_bonds:
+            if len(self.find_out_of_bound_atoms(minimum_y))>0:
+
+                path1 = self.find_shortest_path(best_bond.atom_1, domain)
+                path2 = self.find_shortest_path(best_bond.atom_2, domain)
+                
+                if len(path2) < len(path1):
+                    rotating_atom = best_bond.atom_1
+                    parent_atom = best_bond.atom_2
+                else:
+                    rotating_atom = best_bond.atom_2
+                    parent_atom = best_bond.atom_1
 
-                    for i, score in enumerate(scores):
-                        if score < best_score:
-                            best_score = score
-                            best_i = i
+                new_overlap_score, _, _ = self.get_overlap_score()
 
-                    self.total_overlap_score = best_score
+                scores = [new_overlap_score]
+                overlappings = [len(self.find_out_of_bound_atoms(minimum_y))]
 
-                    self.rotate_subtree(rotating_atom, parent_atom, math.radians(30 * best_i + 1), parent_atom.draw.position)
+                self.rotate_subtree(rotating_atom, parent_atom, math.radians(
+                    15), parent_atom.draw.position)
+
+                for i in range(12):
+                    self.rotate_subtree(rotating_atom, parent_atom, math.radians(
+                        30), parent_atom.draw.position)
+                    overlappings.append(len(self.find_out_of_bound_atoms(minimum_y)))
+                    new_overlap_score, _, _ = self.get_overlap_score()
+                    scores.append(new_overlap_score)
+
+                assert len(scores) == 13
+                scores = scores[:12]
+
+                assert len(overlappings) == 13
+                overlappings = overlappings[:12]
+
+                best_i = 0
+                best_overlapping = overlappings[0]
+                best_score = self.total_overlap_score
+                for i, overlapping in enumerate(overlappings):
+                    if overlapping < best_overlapping and scores[i] < self.options.overlap_sensitivity + self.total_overlap_score:
+                        best_overlapping = overlapping
+                        best_i = i
+                        best_score = scores[i]
+                self.rotate_subtree(rotating_atom, parent_atom, math.radians(
+                    30 * best_i + 1), parent_atom.draw.position)
+                self.total_overlap_score = best_score
+                
+
+    def draw(self, coords_only: bool = False) -> None:
+
+        if not self.options.draw_hydrogens:
+            self.hide_hydrogens()
+
+        self.get_atom_nr_to_atom()
+        self.define_rings()
+
+        if not self.multiple:
+            self._process_structure()
+            if self.make_linear:
+                self.linearise()
+            self.set_chiral_bonds()
+            if not coords_only:
+                self.draw_structure()
+        else:
+            self.restore_ring_information()
 
+    # TODO: replace this entirely with PIKAChU's svg drawer
     def draw_structure(self):
+        # Find the plotting dimensions of the molecule such that the canvas can be scaled to fit the molecule
+
         min_x = 100000000
         max_x = -100000000
         min_y = 100000000
         max_y = -100000000
 
         for atom in self.structure.graph:
             if atom.draw.positioned:
@@ -376,245 +321,237 @@
                 if atom.draw.position.x > max_x:
                     max_x = atom.draw.position.x
                 if atom.draw.position.y > max_y:
                     max_y = atom.draw.position.y
 
         height = max_y - min_y
         width = max_x - min_x
-        self.line_width = 2
 
-        fig, ax = plt.subplots(figsize=((width + 2 * self.options.padding) /
-        50.0, (height + 2 * self.options.padding) / 50.0), dpi=self.dpi)
+        fig, ax = plt.subplots(figsize=((width + 2 * self.options.padding) / 50.0,
+                                        (height + 2 * self.options.padding) / 50.0), dpi=100)
 
         ax.set_aspect('equal', adjustable='box')
         ax.axis('off')
 
-        ax.set_xlim(
-            [min_x - self.options.padding, max_x + self.options.padding])
-        ax.set_ylim(
-            [min_y - self.options.padding, max_y + self.options.padding])
-        plt.subplots_adjust(left=0, bottom=0, right=1, top=1, wspace=0,
-                            hspace=0)
+        ax.set_xlim([min_x - self.options.padding, max_x + self.options.padding])
+        ax.set_ylim([min_y - self.options.padding, max_y + self.options.padding])
+        plt.subplots_adjust(left=0, bottom=0, right=1, top=1, wspace=0, hspace=0)
 
-        params = {'mathtext.default': 'regular', }
+        params = {'mathtext.default': 'regular'}
         plt.rcParams.update(params)
 
         ring_centers_x = []
         ring_centers_y = []
 
         for ring in self.rings:
             self.set_ring_center(ring)
 
             ring_centers_x.append(ring.center.x)
             ring_centers_y.append(ring.center.y)
 
         for bond_nr, bond in self.structure.bonds.items():
             if bond.atom_1.draw.positioned and bond.atom_2.draw.positioned:
-                line = Line(bond.atom_1.draw.position,
-                            bond.atom_2.draw.position, bond.atom_1,
-                            bond.atom_2)
+                line = Line(bond.atom_1.draw.position, bond.atom_2.draw.position, bond.atom_1, bond.atom_2)
                 midpoint = line.get_midpoint()
-                truncated_line = line.get_truncated_line(
-                    self.options.short_bond_length)
+
                 if bond.type == 'single':
                     if bond in self.chiral_bonds:
                         orientation, chiral_center = self.chiral_bond_to_orientation[bond]
-                        self.plot_chiral_bond(orientation, chiral_center, line,
-                                              ax, midpoint)
+                        self._plot_chiral_bond(orientation, chiral_center, line, ax, midpoint)
                     else:
-                        if (bond.atom_1.type == 'S' and
-                                bond.atom_2.annotations.domain_type or
-                                (bond.atom_2.type == 'S' and
-                                 bond.atom_1.annotations.domain_type)):
-                            self.plot_halflines_s_domain(line, ax, midpoint)
-                        else:
-                            self.plot_halflines(line, ax, midpoint)
+                        self._plot_halflines(line, ax, midpoint)
                 elif bond.type == 'double':
-                    if not self.is_terminal(
-                            bond.atom_1) and not self.is_terminal(bond.atom_2):
-                        self.plot_halflines(line, ax, midpoint)
+                    if not self._is_terminal(bond.atom_1) and not self._is_terminal(bond.atom_2):
+                        self._plot_halflines(line, ax, midpoint)
 
-                        common_ring_numbers = self.get_common_rings(
-                            bond.atom_1, bond.atom_2)
+                        common_ring_numbers = self._get_common_rings(bond.atom_1, bond.atom_2)
 
                         if common_ring_numbers:
                             common_rings = []
                             for ring_nr in common_ring_numbers:
                                 common_rings.append(self.get_ring(ring_nr))
 
                             common_rings.sort(key=lambda x: len(x.members))
                             common_ring = common_rings[0]
                             ring_centre = common_ring.center
-                            second_line = line.double_line_towards_center(
-                                ring_centre, self.options.bond_spacing,
-                                self.options.double_bond_length)
+                            second_line = line.double_line_towards_center(ring_centre, self.options.bond_spacing,
+                                                                          self.options.double_bond_length)
                             second_line_midpoint = second_line.get_midpoint()
-                            self.plot_halflines_double(second_line, ax,
-                                                       second_line_midpoint)
+                            self._plot_halflines_double(second_line, ax, second_line_midpoint)
 
                         else:
-                            bond_neighbours = bond.atom_1.drawn_neighbours +\
-                                              bond.atom_2.drawn_neighbours
+                            bond_neighbours = bond.atom_1.drawn_neighbours + bond.atom_2.drawn_neighbours
                             if bond_neighbours:
-                                vectors = [atom.draw.position for atom in
-                                           bond_neighbours]
-                                gravitational_point = Vector.get_average(
-                                    vectors)
-                                second_line = line.double_line_towards_center(
-                                    gravitational_point,
-                                    self.options.bond_spacing,
-                                    self.options.double_bond_length)
+                                vectors = [atom.draw.position for atom in bond_neighbours]
+                                gravitational_point = Vector.get_average(vectors)
+                                second_line = line.double_line_towards_center(gravitational_point,
+                                                                              self.options.bond_spacing,
+                                                                              self.options.double_bond_length)
                                 second_line_midpoint = second_line.get_midpoint()
-                                self.plot_halflines_double(second_line, ax,
-                                                           second_line_midpoint)
+                                self._plot_halflines_double(second_line, ax, second_line_midpoint)
                             else:
                                 print("Shouldn't happen!")
                     else:
-                        if self.is_terminal(bond.atom_1) and self.is_terminal(
-                                bond.atom_2):
-                            dummy_1 = Vector(bond.atom_1.draw.position.x + 1,
-                                             bond.atom_1.draw.position.y + 1)
-                            dummy_2 = Vector(bond.atom_1.draw.position.x - 1,
-                                             bond.atom_1.draw.position.y - 1)
-                            double_bond_line_1 = line.double_line_towards_center(
-                                dummy_1,
-                                self.options.bond_spacing / 2.0,
-                                self.options.double_bond_length)
+                        if self._is_terminal(bond.atom_1) and self._is_terminal(bond.atom_2):
+                            dummy_1 = Vector(bond.atom_1.draw.position.x + 1, bond.atom_1.draw.position.y + 1)
+                            dummy_2 = Vector(bond.atom_1.draw.position.x - 1, bond.atom_1.draw.position.y - 1)
+                            double_bond_line_1 = line.double_line_towards_center(dummy_1,
+                                                                                 self.options.bond_spacing / 2.0,
+                                                                                 self.options.double_bond_length)
                             double_bond_line_1_midpoint = double_bond_line_1.get_midpoint()
-                            double_bond_line_2 = line.double_line_towards_center(
-                                dummy_2,
-                                self.options.bond_spacing / 2.0,
-                                self.options.double_bond_length)
+                            double_bond_line_2 = line.double_line_towards_center(dummy_2,
+                                                                                 self.options.bond_spacing / 2.0,
+                                                                                 self.options.double_bond_length)
                             double_bond_line_2_midpoint = double_bond_line_2.get_midpoint()
 
-                            self.plot_halflines_double(double_bond_line_1, ax,
-                                                       double_bond_line_1_midpoint)
-                            self.plot_halflines_double(double_bond_line_2, ax,
-                                                       double_bond_line_2_midpoint)
+                            self._plot_halflines_double(double_bond_line_1, ax, double_bond_line_1_midpoint)
+                            self._plot_halflines_double(double_bond_line_2, ax, double_bond_line_2_midpoint)
 
                         else:
 
-                            if self.is_terminal(bond.atom_1):
+                            if self._is_terminal(bond.atom_1):
                                 terminal_atom = bond.atom_1
                                 branched_atom = bond.atom_2
                             else:
                                 terminal_atom = bond.atom_2
                                 branched_atom = bond.atom_1
 
                             if len(branched_atom.drawn_neighbours) >= 3:
-                                closest_two = self.get_sorted_distances_from_list(
-                                    terminal_atom,
-                                    branched_atom.drawn_neighbours)
+                                closest_two = self.get_sorted_distances_from_list(terminal_atom,
+                                                                                  branched_atom.drawn_neighbours)
                                 closest_atom_1 = closest_two[0][1]
                                 closest_atom_2 = closest_two[1][1]
 
-                                line = Line(terminal_atom.draw.position,
-                                            branched_atom.draw.position,
-                                            terminal_atom, branched_atom)
-
-                                bond_1_line = Line(branched_atom.draw.position,
-                                                   closest_atom_1.draw.position,
-                                                   branched_atom,
-                                                   closest_atom_1)
-                                bond_2_line = Line(branched_atom.draw.position,
-                                                   closest_atom_2.draw.position,
-                                                   branched_atom,
-                                                   closest_atom_1)
-
-                                double_bond_line_1 = line.double_line_towards_center(
-                                    closest_atom_1.draw.position,
-                                    self.options.bond_spacing / 2.0,
-                                    self.options.double_bond_length)
-                                double_bond_line_2 = line.double_line_towards_center(
-                                    closest_atom_2.draw.position,
-                                    self.options.bond_spacing / 2.0,
-                                    self.options.double_bond_length)
-
-                                double_bond_line_1_midpoint = \
-                                    double_bond_line_1.get_midpoint()
-                                double_bond_line_2_midpoint = \
-                                    double_bond_line_2.get_midpoint()
-
-                                intersection_1 = double_bond_line_1.find_intersection(
-                                    bond_1_line)
-                                intersection_2 = double_bond_line_2.find_intersection(
-                                    bond_2_line)
-
-                                if terminal_atom.draw.position.x >\
-                                        branched_atom.draw.position.x:
-                                    double_bond_line_1.point_1 = intersection_1
-                                    double_bond_line_2.point_1 = intersection_2
+                                line = Line(terminal_atom.draw.position, branched_atom.draw.position, terminal_atom,
+                                            branched_atom)
+
+                                double_bond_line_1, double_bond_line_2 = line.get_perpendicular_lines(
+                                    self.options.bond_spacing / 2.0)
+                                terminal_atom_pos_1 = double_bond_line_1.get_atom_coords(terminal_atom)
+                                terminal_atom_pos_2 = double_bond_line_2.get_atom_coords(terminal_atom)
+
+                                closest_atom_to_pos_1 = terminal_atom_pos_1.get_closest_atom(closest_atom_1,
+                                                                                             closest_atom_2)
+                                closest_atom_to_pos_2 = terminal_atom_pos_2.get_closest_atom(closest_atom_1,
+                                                                                             closest_atom_2)
+
+                                bond_1_line = Line(branched_atom.draw.position, closest_atom_to_pos_1.draw.position,
+                                                   branched_atom, closest_atom_to_pos_1)
+                                bond_2_line = Line(branched_atom.draw.position, closest_atom_to_pos_2.draw.position,
+                                                   branched_atom, closest_atom_to_pos_2)
+
+                                double_bond_line_1_midpoint = double_bond_line_1.get_midpoint()
+                                double_bond_line_2_midpoint = double_bond_line_2.get_midpoint()
+
+                                intersection_1 = double_bond_line_1.find_intersection(bond_1_line)
+                                intersection_2 = double_bond_line_2.find_intersection(bond_2_line)
+
+                                if terminal_atom.draw.position.x > branched_atom.draw.position.x:
+                                    # check for parallel lines
+                                    if intersection_1 and intersection_1.x < 100000 and intersection_1.y < 100000:
+                                        double_bond_line_1.point_1 = intersection_1
+                                    if intersection_2 and intersection_2.x < 100000 and intersection_2.y < 100000:
+                                        double_bond_line_2.point_1 = intersection_2
+
                                 else:
-                                    double_bond_line_1.point_2 = intersection_1
-                                    double_bond_line_2.point_2 = intersection_2
+                                    # check for parallel lines
+                                    if intersection_1 and intersection_1.x < 100000 and intersection_1.y < 100000:
+                                        double_bond_line_1.point_2 = intersection_1
+                                    if intersection_2 and intersection_2.x < 100000 and intersection_2.y < 100000:
+                                        double_bond_line_2.point_2 = intersection_2
 
-                                self.plot_halflines(double_bond_line_1, ax,
-                                                    double_bond_line_1_midpoint)
-                                self.plot_halflines(double_bond_line_2, ax,
-                                                    double_bond_line_2_midpoint)
+                                self._plot_halflines(double_bond_line_1, ax, double_bond_line_1_midpoint)
+                                self._plot_halflines(double_bond_line_2, ax, double_bond_line_2_midpoint)
 
                             else:
-                                pass
+                                self._plot_halflines(line, ax, midpoint)
+
+                                bond_neighbours = bond.atom_1.drawn_neighbours + bond.atom_2.drawn_neighbours
+                                if bond_neighbours:
+                                    vectors = [atom.draw.position for atom in bond_neighbours]
+                                    gravitational_point = Vector.get_average(vectors)
+                                    second_line = line.get_parallel_line(gravitational_point,
+                                                                         self.options.bond_spacing)
+                                    second_line_midpoint = second_line.get_midpoint()
+                                    self._plot_halflines(second_line, ax, second_line_midpoint)
+                                else:
+                                    print("Shouldn't happen!")
+
+                elif bond.type == 'triple':
+                    self._plot_halflines(line, ax, midpoint)
+                    line_1, line_2 = line.get_parallel_lines(self.options.bond_spacing)
+                    line_1_midpoint = line_1.get_midpoint()
+                    line_2_midpoint = line_2.get_midpoint()
+                    self._plot_halflines(line_1, ax, line_1_midpoint)
+                    self._plot_halflines(line_2, ax, line_2_midpoint)
 
         # If the starter unit contains an unknown moiety, number this R1
         for atom in self.structure.graph:
             if atom.type == '*' and not atom.annotations.unknown_index:
                 atom.annotations.unknown_index = 1
         for atom in self.structure.graph:
-            if atom.type != 'C' and atom.draw.positioned:
+            if ((atom.type != 'C' or self.draw_Cs_in_pink) and getattr(atom.annotations,"domain_type", None) not in ["Follower", "Leader"]) and atom.draw.positioned:
                 text_h = ''
                 text_h_pos = None
 
-                if atom.type != 'C' or atom.draw.draw_explicit:
+                if (atom.type != 'C' or self.draw_Cs_in_pink or atom.draw.draw_explicit) :
                     text = atom.type
                 else:
                     text = ''
 
-                if atom.annotations.domain_type:
-                    text = atom.annotations.domain_type
+                if hasattr(atom.annotations, "domain_type") and atom.annotations.domain_type:
+                    if atom.annotations.domain_type in ["Follower", "Leader"]:
+                        text = ""
+                    else:
+                        text = atom.annotations.domain_type
 
                 horizontal_alignment = 'center'
 
-                orientation = self.get_hydrogen_text_orientation(atom)
+                orientation = self._get_hydrogen_text_orientation(atom)
                 if orientation == 'H_above_atom':
-                    text_h_pos = Vector(atom.draw.position.x, atom.draw.position.y + 6)
+                    text_h_pos = Vector(
+                        atom.draw.position.x, atom.draw.position.y + 6)
                 if orientation == 'H_below_atom':
-                    text_h_pos = Vector(atom.draw.position.x, atom.draw.position.y - 6)
+                    text_h_pos = Vector(
+                        atom.draw.position.x, atom.draw.position.y - 6)
 
-                atom_draw_position = Vector(atom.draw.position.x, atom.draw.position.y)
+                atom_draw_position = Vector(
+                    atom.draw.position.x, atom.draw.position.y)
 
                 if atom.type == '*':
                     neighbouring_c = atom.get_neighbour('C')
                     assert neighbouring_c
                     # In order to not let the number of the sidechain overlap
                     # with the bond, move Rx symbol along hor. axis depending on
                     # if group is added to the left or right of the chain
-                    delta_x_r = self.get_delta_x_sidechain(atom, neighbouring_c)
+                    delta_x_r = self.get_delta_x_sidechain(
+                        atom, neighbouring_c)
                     atom_draw_position.x += delta_x_r
                     text = fr'$R_{atom.annotations.unknown_index}$'
 
-                if not atom.charge and (atom.type != 'C' or atom.draw.draw_explicit):
+                if not atom.charge and (atom.type != 'C' or self.draw_Cs_in_pink or atom.draw.draw_explicit) and getattr(atom.annotations, "domain_type", None) not in ["Follower", "Leader"]:
 
                     if atom.draw.has_hydrogen:
                         hydrogen_count = 0
                         for neighbour in atom.neighbours:
                             if neighbour.type == 'H' and not neighbour.draw.is_drawn:
                                 hydrogen_count += 1
 
-                        if hydrogen_count:
+                        if hydrogen_count and not (atom.type == 'C' and self.draw_Cs_in_pink or getattr(atom.annotations, "domain_type", None) in ["Follower", "Leader"]):
 
                             if hydrogen_count > 1:
                                 if orientation == 'H_before_atom':
                                     text = r'$H_{hydrogens}{atom_type}$'.format(hydrogens=hydrogen_count,
                                                                                 atom_type=atom.type)
                                     horizontal_alignment = 'right'
                                     atom_draw_position.x += 3
                                 elif orientation == 'H_below_atom' or orientation == 'H_above_atom':
                                     text = atom.type
-                                    text_h = r'$H_{hydrogens}$'.format(hydrogens=hydrogen_count)
+                                    text_h = r'$H_{hydrogens}$'.format(
+                                        hydrogens=hydrogen_count)
 
                                 else:
                                     text = r'${atom_type}H_{hydrogens}$'.format(hydrogens=hydrogen_count,
                                                                                 atom_type=atom.type)
                                     horizontal_alignment = 'left'
                                     atom_draw_position.x -= 3
                             elif hydrogen_count == 1:
@@ -669,15 +606,16 @@
                                         hydrogens=hydrogen_count,
                                         atom_type=atom.type,
                                         charge_symbol=charge_symbol)
 
                                 horizontal_alignment = 'right'
                                 atom_draw_position.x += 3
                             elif orientation == 'H_above_atom' or orientation == 'H_below_atom':
-                                text_h = r'$H_{hydrogens}$'.format(hydrogens=hydrogen_count)
+                                text_h = r'$H_{hydrogens}$'.format(
+                                    hydrogens=hydrogen_count)
                                 if abs(atom.charge) > 1:
                                     text = r'${atom_type}^{charge}{charge_symbol}$'.format(atom_type=atom.type,
                                                                                            charge=atom.charge,
                                                                                            charge_symbol=charge_symbol)
                                 elif abs(atom.charge) == 1:
                                     text = r'${atom_type}^{charge_symbol}$'.format(atom_type=atom.type,
                                                                                    charge_symbol=charge_symbol)
@@ -727,26 +665,44 @@
 
                                 elif abs(atom.charge) == 1:
                                     text = r'${atom_type}H^{charge_symbol}$'.format(atom_type=atom.type,
                                                                                     charge_symbol=charge_symbol)
                                 horizontal_alignment = 'left'
                                 atom_draw_position.x -= 3
 
-                if text:
-                    plt.text(atom_draw_position.x, atom_draw_position.y,
-                             text,
-                             horizontalalignment=horizontal_alignment,
-                             verticalalignment='center',
-                             color=atom.draw.colour)
-                if text_h:
-                    plt.text(text_h_pos.x, text_h_pos.y,
-                             text_h,
-                             horizontalalignment='center',
-                             verticalalignment='center',
-                             color=atom.draw.colour)
+                atom_color = atom.draw.colour
+                if self.draw_Cs_in_pink:
+                    if atom.type == 'C':
+                        atom_color = "magenta"
+                if self.add_url:
+                    if text:
+                        plt.text(atom_draw_position.x, atom_draw_position.y,
+                                 text, url=str(atom),
+                                 horizontalalignment=horizontal_alignment,
+                                 verticalalignment='center',
+                                 color=atom_color)
+                    if text_h:
+                        plt.text(text_h_pos.x, text_h_pos.y,
+                                 text_h, url=str(atom),
+                                 horizontalalignment='center',
+                                 verticalalignment='center',
+                                 color=atom_color)
+                else:
+                    if text:
+                        plt.text(atom_draw_position.x, atom_draw_position.y,
+                                 text,
+                                 horizontalalignment=horizontal_alignment,
+                                 verticalalignment='center',
+                                 color=atom_color)
+                    if text_h:
+                        plt.text(text_h_pos.x, text_h_pos.y,
+                                 text_h,
+                                 horizontalalignment='center',
+                                 verticalalignment='center',
+                                 color=atom_color)
 
         # If a png filename is included in the initialization of the
         # Raichu_drawer object, don't show the structure, but do save it as a
         # png image to the provided filename
         if self.dont_show:
             return self
 
@@ -757,546 +713,667 @@
             if self.save_png:
                 plt.savefig(self.save_png)
             elif self.save_svg:
                 plt.savefig(self.save_svg)
             plt.clf()
             plt.close()
 
+    def colour_modules(self):
+        pass
 
-    def process_structure(self):
-        self.position()
-        self.structure.refresh_structure()
-        self.restore_ring_information()
-        self.resolve_primary_overlaps()
-        self.total_overlap_score, sorted_overlap_scores, atom_to_scores = self.get_overlap_score()
+    def place_top_atom(self, backbone_atoms, attachment_point):
 
-        for i in range(self.options.overlap_resolution_iterations):
-            for bond in self.drawn_bonds:
-                if self.bond_is_rotatable(bond):
-
-                    tree_depth_1 = self.get_subgraph_size(bond.atom_1,
-                                                          {bond.atom_2})
-                    tree_depth_2 = self.get_subgraph_size(bond.atom_2,
-                                                          {bond.atom_1})
-
-                    atom_1 = bond.atom_2
-                    atom_2 = bond.atom_1
-
-                    if tree_depth_1 > tree_depth_2:
-                        atom_1 = bond.atom_1
-                        atom_2 = bond.atom_2
-
-                    subtree_overlap_score, _ = self.get_subtree_overlap_score(
-                        atom_2, atom_1, atom_to_scores)
-
-                    if subtree_overlap_score > self.options.overlap_sensitivity:
-                        neighbours_2 = atom_2.drawn_neighbours[:]
-                        neighbours_2.remove(atom_1)
-
-                        if len(neighbours_2) == 1:
-                            neighbour = neighbours_2[0]
-                            angle = neighbour.draw.position.get_rotation_away_from_vector(
-                                atom_1.draw.position, atom_2.draw.position,
-                                math.radians(120))
-
-                            self.rotate_subtree(neighbour, atom_2, angle,
-                                                atom_2.draw.position)
-
-                            new_overlap_score, _, _ = self.get_overlap_score()
-                            if new_overlap_score > self.total_overlap_score:
-                                self.rotate_subtree(neighbour, atom_2,
-                                                    -angle,
-                                                    atom_2.draw.position)
-                            else:
-                                self.total_overlap_score = new_overlap_score
 
-                        elif len(neighbours_2) == 2:
-                            if atom_2.draw.rings and atom_1.draw.rings:
-                                continue
-
-                            neighbour_1 = neighbours_2[0]
-                            neighbour_2 = neighbours_2[1]
-                            if len(neighbour_1.draw.rings) == 1 and len(
-                                    neighbour_2.draw.rings) == 1:
-                                # If the neighbours are in different rings,
-                                # or in rings at all, do nothing
-                                if neighbour_1.draw.rings[0] != \
-                                        neighbour_2.draw.rings[0]:
-                                    continue
-                                elif neighbour_1.draw.rings or neighbour_2.draw.rings:
-                                    continue
-                                else:
-                                    angle_1 = neighbour_1.draw.position.get_rotation_away_from_vector(
-                                        atom_1.position, atom_2.position,
-                                        math.radians(120))
-                                    angle_2 = neighbour_2.draw.position.get_rotation_away_from_vector(
-                                        atom_1.position, atom_2.position,
-                                        math.radians(120))
-
-                                    self.rotate_subtree(neighbour_1,
-                                                        atom_2,
-                                                        angle_1,
-                                                        atom_2.position)
-                                    self.rotate_subtree(neighbour_2,
-                                                        atom_2,
-                                                        angle_2,
-                                                        atom_2.position)
-
-                                    new_overlap_score, _, _ = self.get_overlap_score()
-
-                                    if new_overlap_score > self.total_overlap_score:
-                                        self.rotate_subtree(neighbour_1,
-                                                            atom_2,
-                                                            -angle_1,
-                                                            atom_2.position)
-                                        self.rotate_subtree(neighbour_2,
-                                                            atom_2,
-                                                            -angle_2,
-                                                            atom_2.position)
-                                    else:
-                                        self.total_overlap_score = new_overlap_score
-                        self.total_overlap_score, sorted_overlap_scores, atom_to_scores = self.get_overlap_score()
-
-
-        # substructure search to see if structure is a polyketide or NRP
-
-        is_polyketide = False
-        is_nrp = False
-        if self.structure.find_substructures(
-                Smiles('SC(=O)').smiles_to_structure()):
-            if self.structure.find_substructures(
-                    Smiles('SC(CN)=O').smiles_to_structure()):
-                is_nrp = True
+        # Fix position of the S and C atom and the S-C angle
+        top_atom = backbone_atoms[0]
+        first_carbon = backbone_atoms[1]
+
+        top_atom.draw.position.x = first_carbon.draw.position.x
+        top_atom.draw.position.y = first_carbon.draw.position.y + 15
+
+        angle = get_angle(first_carbon.draw.position,
+                          top_atom.draw.position)
+
+        angle_degrees = round(math.degrees(angle), 3)
+
+        correct_angle_deg = -120
+        delta_angle_deg = correct_angle_deg - angle_degrees
+        delta_angle_rad = math.radians(delta_angle_deg)
+
+        self.rotate_subtree(top_atom, first_carbon, delta_angle_rad,
+                            first_carbon.draw.position)
+
+        # Fix position domain straight above sulphur atom
+        attachment_point.draw.position.x = top_atom.draw.position.x
+        attachment_point.draw.position.y = top_atom.draw.position.y + 15
+
+
+    @staticmethod
+    def get_opposite_placement(placement):
+        if placement == 'right':
+            return 'left'
+        elif placement == 'left':
+            return 'right'
+        else:
+            raise ValueError("Only placements accepted are 'left' and 'right'.")
+
+    def get_placements(self, backbone, atom_to_ring, stop_linearising):
+        backbone_to_placement = OrderedDict()
+        for i, atom in enumerate(backbone):
+            if atom == stop_linearising:
+                break
+
+            if i == 0:
+                backbone_to_placement[atom] = 'right'
+            elif i == 1:
+                backbone_to_placement[atom] = 'left'
             else:
-                is_polyketide = True
+                if atom not in backbone_to_placement:
+                    previous_placement = backbone_to_placement.get(backbone[i - 1])
+                    ring = atom_to_ring.get(atom)
+                    if ring and len(ring) == 2:
+                        if ring[0] in backbone_to_placement:
+                            backbone_to_placement[ring[1]] = backbone_to_placement.get(ring[0])
+                        else:
+                            backbone_to_placement[atom] = self.get_opposite_placement(previous_placement)
+                    elif hasattr(atom, "domain_type") and atom.annotations.domain_type == "Leader":
+                        backbone_to_placement[atom] = previous_placement
+                    else:
+                        backbone_to_placement[atom] = self.get_opposite_placement(previous_placement)
+
+        return backbone_to_placement
+
+    def fix_rings(self, rings, backbone_atoms, backbone_to_placement):
+        for ring in rings:
+            if len(ring) == 1:
+                atom_1 = ring[0]
+                if atom_1 == backbone_atoms[-1]:
+                    continue
+                drawing_ring = self.get_ring(atom_1.draw.rings[0])
+                center = Vector(0, 0)
+                for atom in drawing_ring.members:
+                    center.add(atom.draw.position)
+
+                center.divide(len(drawing_ring.members))
+                angle = get_angle(atom_1.draw.position,
+                                  center)
+                
+                if backbone_to_placement[atom_1] == 'right':
+                    desired_angle = 180
+                else:
+                    desired_angle = 0.0
+                required_rotation_deg = desired_angle - angle
+                required_rotation_rad = math.radians(required_rotation_deg)
+
+                masked = {atom_1}
+                first_atom_cycle = None
+                for next_atom in atom_1.neighbours:
+                    if next_atom.type != 'H' and next_atom not in backbone_atoms and next_atom in drawing_ring.members:
+                        first_atom_cycle = next_atom
+
+                assert first_atom_cycle
+
+                # for atom in drawing_ring.members:
+                for atom in self.traverse_substructure(first_atom_cycle, masked):
+                    if atom != atom_1:
+                        atom.draw.position.rotate_around_vector(required_rotation_rad, atom_1.draw.position)
+
+            elif len(ring) == 2:
+                atom_1, atom_2 = ring
+                masked = {atom_1, atom_2}
+
+                first_atom_cycle = None
+                for next_atom in atom_1.neighbours:
+                    if next_atom.type != 'H' and next_atom not in backbone_atoms:
+                        first_atom_cycle = next_atom
+
+                assert first_atom_cycle
+
+                if backbone_to_placement[atom_1] == backbone_to_placement[atom_2] == 'right':
+                    if atom_1.draw.position.x > first_atom_cycle.draw.position.x:
+                        for atom in self.traverse_substructure(first_atom_cycle, masked):
+                            delta_x = 2 * (atom_1.draw.position.x - atom.draw.position.x)
+                            atom.draw.position.x += delta_x
+
+                elif backbone_to_placement[atom_1] == backbone_to_placement[atom_2] == 'left':
+
+                    if atom_1.draw.position.x < first_atom_cycle.draw.position.x:
+                        for atom in self.traverse_substructure(first_atom_cycle, masked):
+                            delta_x = 2 * (atom.draw.position.x - atom_1.draw.position.x)
+                            atom.draw.position.x -= delta_x
+
+    def get_overlap_score(self) -> Tuple[float, List[Tuple[float, Atom]], Dict[Atom, float]]:
+        total = 0.0
+
+        overlap_scores = {}
+        for atom in self.drawn_atoms:
+            overlap_scores[atom] = 0.0
+
+        for i, atom_1 in enumerate(self.drawn_atoms):
+            for j in range(i + 1, len(self.drawn_atoms)):
+                atom_2 = self.drawn_atoms[j]
+                distance = Vector.subtract_vectors(atom_1.draw.position, atom_2.draw.position).get_squared_length()
+                if atom_1 not in atom_2.neighbours:
+                    if distance < self.options.bond_length_squared + 1:
+
+                        if atom_1.has_neighbour('H') and atom_2.has_neighbour('H') and atom_1.type != 'C' \
+                                and atom_2.type != 'C':
+
+                            weight = self.options.overlap_sensitivity + abs((self.options.bond_length - math.sqrt(distance))) / self.options.bond_length
+
+                        else:
+                            weight = abs((self.options.bond_length - math.sqrt(distance))) / self.options.bond_length
+                        total += weight
+                        overlap_scores[atom_1] += weight
+                        overlap_scores[atom_2] += weight
+
+        sorted_overlaps = []
+
+        for atom in self.drawn_atoms:
+            sorted_overlaps.append((overlap_scores[atom], atom))
+
+        sorted_overlaps.sort(key=lambda x: x[0], reverse=True)
+
+        return total, sorted_overlaps, overlap_scores
+
+    def linearise(self):
+
+        attachment_point = None
+        domains = []
 
-        attached_to_domain = False
         for atom in self.structure.graph:
-            if atom.type == 'S':
-                sulphur = atom
-                for neighbour in sulphur.neighbours:
-                    if neighbour.annotations.domain_type:
-                        attached_to_domain = True
-                        domain = neighbour
+            if atom.type == 'I':
+                if atom.annotations.domain_type in ["Leader", "Follower", "ACP", "PCP"]:
+                    domains.append(atom)
+                    # Ensures the follower peptide is set as attachment point if both leader and follower are present
+                    if not attachment_point:
+                        attachment_point = atom
+                    elif attachment_point.annotations.domain_type == "Leader":
+                        attachment_point = atom
+
+        if attachment_point and attachment_point.annotations.domain_type == "Leader":
+            horizontal_rotation = 'anticlockwise'
+        else:
+            horizontal_rotation = 'clockwise'
+
+        if self.ripp:
+            label_ripp_central_chain(self.structure)
+
+        self.structure.refresh_structure()
+
+        if attachment_point:
+            if self.ripp:
+                backbone_atoms = find_central_chain_ripp(self.structure)
+            else:
+                backbone_atoms = find_central_chain(self.structure)
+        else:
+            backbone_atoms = find_central_chain_not_attached(self.structure)
+
+        if attachment_point:
+
+            self.place_top_atom(backbone_atoms, attachment_point)
 
         self.structure.refresh_structure()
+        backbone, full_rings, rings, atom_to_ring, stop_linearising = reorder_central_chain(backbone_atoms, self)
+        if len(domains) == 2:
+            for domain in domains:
+                if domain.annotations.domain_type == 'Leader':
+                    backbone.append(domain)
+
+        backbone_to_placement = self.get_placements(backbone, atom_to_ring, stop_linearising)
+
+        i = 0
+
+        while i < len(backbone) - 1:
+
+            atom_1 = backbone[i]
+            atom_2 = backbone[i + 1]
+
+            if atom_1 not in backbone_to_placement or atom_2 not in backbone_to_placement:
+                break
 
-        ### NRPS + PK code: Force pk/peptide backbone to be drawn straight:
-        # If struct=PK/NRP, find central chain and attached domain
-        if attached_to_domain and (is_nrp or is_polyketide):
-            backbone_atoms = find_central_chain(self.structure)
-            pcp = None
-            for atom in self.structure.graph:
-                if atom.annotations.domain_type:
-                    pcp = atom
-
-            assert pcp
-
-            # Fix position of the S and C atom and the S-C angle
-            sulphur = backbone_atoms[0]
-            first_carbon = backbone_atoms[1]
-
-            sulphur.draw.position.x = first_carbon.draw.position.x
-            sulphur.draw.position.y = first_carbon.draw.position.y + 15
-
-            angle = get_angle(first_carbon.draw.position,
-                              sulphur.draw.position)
-            angle_degrees = round(math.degrees(angle), 3)
-
-            correct_angle_deg = -120
-            delta_angle_deg = correct_angle_deg - angle_degrees
-            delta_angle_rad = math.radians(delta_angle_deg)
-
-            self.rotate_subtree(sulphur, first_carbon, delta_angle_rad,
-                                first_carbon.draw.position)
-
-            # Fix position domain straight above sulphur atom
-            pcp.draw.position.x = sulphur.draw.position.x
-            pcp.draw.position.y = sulphur.draw.position.y + 15
-
-            # Rotate all other bonds in peptide backbone of NRP
-            i = 0
-            fixed_atoms = set()
-            while i < (len(backbone_atoms) - 1):
-                atom1 = backbone_atoms[i]
-                atom2 = backbone_atoms[i + 1]
-                angle = get_angle(atom1.draw.position, atom2.draw.position)
-                angle_degrees = round(math.degrees(angle), 3)
-
-                # Save angle last two atoms, needed later
-                if i == (len(backbone_atoms) - 2):
-                    last_angle_degrees = angle_degrees
-
-                # Special case for amino acids with cyclic backbone (proline)
-                if atom1.inside_ring and atom2.inside_ring:
-                    if angle_degrees != 90.0:
-                        correct_angle_deg = 90
-                        delta_angle_deg = correct_angle_deg - angle_degrees
-                        delta_angle_rad = math.radians(delta_angle_deg)
-                        self.rotate_subtree(atom2, atom1, delta_angle_rad,
-                                            atom1.draw.position)
-                    i += 1
-
-                    # Flip cyclic backbone amino acid if necessary
-                    if atom1.draw.position.x > backbone_atoms[i - 2].draw.position.x:
-                        first_atom_cycle = None
-                        for next_atom in atom1.neighbours:
-                            print(next_atom, next_atom.type)
-                            if next_atom.type != 'H' and next_atom not in backbone_atoms:
-                                first_atom_cycle = next_atom
-                        assert first_atom_cycle
-                        if atom1.draw.position.x > first_atom_cycle.draw.position.x:
-                            masked = {atom1, atom2}
-                            for atom in self.traverse_substructure(
-                                    first_atom_cycle, masked):
-                                delta_x = 2 * (atom1.draw.position.x - atom.draw.position.x)
-                                atom.draw.position.x += delta_x
-
-                    if atom1.draw.position.x < backbone_atoms[i - 2].draw.position.x:
-                        first_atom_cycle = None
-                        for next_atom in atom1.neighbours:
-                            if next_atom.type != 'H' and next_atom not in backbone_atoms:
-                                first_atom_cycle = next_atom
-                        assert first_atom_cycle
-                        if atom1.draw.position.x < first_atom_cycle.draw.position.x:
-                            masked = {atom1, atom2}
-                            for atom in self.traverse_substructure(first_atom_cycle, masked):
-                                delta_x = 2 * (atom.draw.position.x - atom1.draw.position.x)
-                                atom.draw.position.x -= delta_x
-
-                # Fix bond angle backbone atoms if second backbone atom (one
-                # with larger position.x) is inside ring, and the first is not
-                elif atom2 != backbone_atoms[-1] and atom2.inside_ring and not atom1.inside_ring and \
-                        backbone_atoms[i + 2].inside_ring:
-                    if atom2 not in fixed_atoms:
-                        if round(math.degrees(get_angle(
-                                backbone_atoms[i - 1].draw.position,
-                                backbone_atoms[i].draw.position)),
-                                 3) == 120.0:
-                            correct_angle_deg = 60.0
-                            first_angle_cyclic = 60.0
-                        elif round(math.degrees(get_angle(
-                                backbone_atoms[i - 1].draw.position,
-                                backbone_atoms[i].draw.position)),
-                                   3) == 60.0:
-                            correct_angle_deg = 120.0
-                            first_angle_cyclic = 120.0
+            current_angle = get_angle(atom_1.draw.position, atom_2.draw.position)
+
+            if backbone_to_placement[atom_1] == 'right' and backbone_to_placement[atom_2] == 'left':
+                desired_angle = 60.0
+            elif backbone_to_placement[atom_1] == 'left' and backbone_to_placement[atom_2] == 'right':
+                desired_angle = 120.0
+            elif backbone_to_placement[atom_1] == backbone_to_placement[atom_2]:
+                desired_angle = 90.0
+            else:
+                raise ValueError("Only supported orientations are 'left' and 'right'.")
+
+            required_rotation_deg = desired_angle - current_angle
+            required_rotation_rad = math.radians(required_rotation_deg)
+
+            if not (atom_2 in atom_to_ring and atom_1 in atom_to_ring and atom_to_ring[atom_2] == atom_to_ring[atom_1]):
+
+                self.rotate_subtree(atom_2, atom_1, required_rotation_rad,
+                                    atom_1.draw.position)
+            else:
+                if len(atom_to_ring[atom_2]) == 2:
+                    self.rotate_subtree(atom_2, atom_1, required_rotation_rad,
+                                        atom_1.draw.position)
+                elif len(atom_to_ring[atom_2]) == 3:
+                    if atom_2 == atom_to_ring[atom_2][1]:
+
+                        self.rotate_subtree(atom_2, atom_1, required_rotation_rad,
+                                            atom_1.draw.position)
+                    elif atom_2 == atom_to_ring[atom_2][2]:
+
+                        ring = atom_to_ring[atom_2]
+                        ring_atoms = []
+                        sidechain_atoms = []
+                        for atom in atom_2.get_ring(self.structure):
+                            if atom not in backbone:
+                                ring_atoms.append(atom)
+
+                        if abs(required_rotation_deg) > 90:
+                            for atom in ring_atoms:
+                                for neighbour in atom.neighbours:
+                                    if neighbour.type != 'H':
+                                        for sidechain_atom in self.traverse_substructure(neighbour,
+                                                                                         set(ring_atoms + backbone)):
+                                            if sidechain_atom not in sidechain_atoms and \
+                                                    sidechain_atom not in ring_atoms and sidechain_atom not in backbone:
+                                                sidechain_atoms.append(sidechain_atom)
+
+                            for ring_atom in ring_atoms:
+                                ring_atom.draw.position.mirror_about_line(ring[0].draw.position, ring[1].draw.position)
+                            for sidechain_atom in sidechain_atoms:
+                                sidechain_atom.draw.position.mirror_about_line(ring[0].draw.position, ring[1].draw.position)
+                        self.rotate_subtree_ring(atom_2, set(ring_atoms + [atom_1]), required_rotation_rad,
+                                                 atom_1.draw.position)
+
+            i += 1
+
+        atoms_in_rings = []
+        for ring in full_rings:
+            for atom in ring:
+                atoms_in_rings.append(atom)
+        atoms_in_rings = set(atoms_in_rings)
+
+        self.fix_rings(rings, backbone, backbone_to_placement)
+
+        self.position_sidechains(backbone, backbone_to_placement, atoms_in_rings)
+
+        # self.resolve_primary_overlaps()
+        self.total_overlap_score, sorted_overlap_scores, atom_to_scores = self.get_overlap_score()
+        central_chain_bonds = set()
+
+        for bond in self.structure.bonds.values():
+            # if bond.atom_1.annotations.in_central_chain or \
+            #         bond.atom_2.annotations.in_central_chain:
+            if bond.atom_1 in backbone or bond.atom_2 in backbone:
+                central_chain_bonds.add(bond)
+
+        self.finetune_overlap_resolution(
+            masked_bonds=central_chain_bonds, highest_atom=backbone[0])
+
+        self.resolve_secondary_overlaps(sorted_overlap_scores)
+
+        if self.horizontal:
+            if horizontal_rotation == 'clockwise':
+                self.rotate_structure(-1.5707)
+            else:
+                self.rotate_structure(1.5707)
+
+    def resolve_overlaps(self, linear: bool = True, masked_bonds: Optional[Set["Bond"]] = None) -> None:
+        """
+
+        Parameters
+        ----------
+        linear: bool, if True, resolve overlaps for a linearised molecule; if False,
+            resolve overlaps for a non-linearised molecule
+        masked_bonds: set of bonds, bonds that are not allowed to be rotated
+
+        """
+        if not linear:
+
+            self.resolve_primary_overlaps()
+            self.total_overlap_score, sorted_overlap_scores, atom_to_scores = self.get_overlap_score()
+            self.finetune_overlap_resolution()
+            self.resolve_secondary_overlaps(sorted_overlap_scores)
+
+        else:
+
+            pass
+
+    def find_high_atoms(self, atoms: List[Atom], max_y: float) -> List[Atom]:
+        """
+        Returns atoms that are drawn too high on the plot
+        Parameters
+        ----------
+        atoms: list of [Atom, ->]
+        max_y: float, maximum vertical y coordinate an atom is allowed to have
+
+        Returns
+        -------
+        high_atoms: list of [Atom, ->], atoms with a y coordinate higher than max_y
+        """
+        high_atoms: List[Atom] = []
+        for atom in atoms:
+            if atom.draw.position.y > max_y:
+                high_atoms.append(atom)
+        return high_atoms
+
+    def find_clashing_sidechain_atoms(self, sidechain_atoms):
+        clashing_atoms: List[Tuple[Atom, Atom]] = []
+        for i, atom_1 in enumerate(self.drawn_atoms):
+            for j in range(i + 1, len(self.drawn_atoms)):
+                atom_2 = self.drawn_atoms[j]
+                if atom_1 in sidechain_atoms and not self.structure.bond_exists(atom_1, atom_2):
+                    distance = Vector.subtract_vectors(atom_1.draw.position, atom_2.draw.position).get_squared_length()
+                    if atom_1.has_neighbour('H') and atom_2.has_neighbour('H') and atom_1.type != 'C' and \
+                            atom_2.type != 'C':
+                        max_distance = self.options.bond_length_squared * 1.5
+                    elif atom_1.has_neighbour('H') or atom_2.has_neighbour('H'):
+                        max_distance = self.options.bond_length_squared
+                    else:
+                        max_distance = self.options.bond_length_squared * 0.8
+                    if distance <= max_distance:
+                        clashing_atoms.append((atom_1, atom_2))
+
+        return clashing_atoms
+
+    def resolve_sidechain_overlaps(self, backbone, backbone_to_placement, backbone_rings, central_chain_bonds):
+        max_y = backbone[0].draw.position.y
+        placed_atoms: List[Atom] = []
+        backbone_to_sidechain: Dict[Atom, List[List[Atom]]] = {}
+        backbone_to_rotatable_bonds: Dict[Atom, List[Bond]] = {}
+
+        for backbone_atom in backbone:
+            sidechains = self.get_sidechains(backbone, backbone_atom, backbone_rings)
+            backbone_to_sidechain[backbone_atom] = sidechains
+            beta_atoms: List[Atom] = self.get_beta_atoms(backbone, backbone_atom, backbone_rings)
+            for sidechain in sidechains:
+                beta_atom: Optional[Atom] = None
+
+                for atom in sidechain:
+                    if atom in beta_atoms:
+                        beta_atom = atom
+                        break
+
+                assert beta_atom
+
+                sidechain_bonds = self.get_sidechain_bonds(sidechain)
+                masked_bond = self.structure.bond_lookup[beta_atom][backbone_atom]
+                rotatable_bonds: List[Bond] = []
+
+                for bond in sidechain_bonds:
+                    if self.bond_is_rotatable(bond) and bond != masked_bond:
+                        rotatable_bonds.append(bond)
+                backbone_to_rotatable_bonds[backbone_atom] = rotatable_bonds
+
+
+            if len(sidechains) == 2:
+                pass
+            elif len(sidechains) == 1:
+                sidechain = sidechains[0]
+                atoms_to_adjust: List[Atom] = self.find_high_atoms(sidechain, max_y)
+                clashing_atoms = self.find_clashing_sidechain_atoms(sidechain)
+                if clashing_atoms or atoms_to_adjust:
+                    beta_atoms: List[Atom] = self.get_beta_atoms(backbone, backbone_atom, backbone_rings)
+                    assert len(beta_atoms) == 1
+                    beta_atom = beta_atoms[0]
+
+                    sidechain_bonds = self.get_sidechain_bonds(sidechain)
+                    rotatable_bonds: List[Bond] = []
+
+                    masked_bond = self.structure.bond_lookup[beta_atom][backbone_atom]
+                    for bond in sidechain_bonds:
+                        if self.bond_is_rotatable(bond) and bond != masked_bond and \
+                                (bond.atom_1 in beta_atoms or bond.atom_2 in beta_atoms):
+                            rotatable_bonds.append(bond)
+
+                    if not rotatable_bonds:
+                        for bond in sidechain_bonds:
+                            if self.bond_is_rotatable(bond) and bond != masked_bond:
+                                rotatable_bonds.append(bond)
+
+    def resolve_secondary_overlaps(self, sorted_scores: List[Tuple[float, Atom]]) -> None:
+        for score, atom in sorted_scores:
+            if score > self.options.overlap_sensitivity:
+                if len(atom.drawn_neighbours) <= 1:
+                    if atom.drawn_neighbours and atom.drawn_neighbours[0]._adjacent_to_stereobond():
+                        continue
+
+                    closest_atom = self.get_closest_atom(atom)
+
+                    drawn_neighbours = closest_atom.drawn_neighbours
+
+                    if len(drawn_neighbours) <= 1:
+                        if not closest_atom.draw.previous_position:
+                            closest_position = drawn_neighbours[0].draw.position
                         else:
-                            print('should not happen!!!')
-                        delta_angle_deg = correct_angle_deg - angle_degrees
-                        delta_angle_rad = math.radians(delta_angle_deg)
-                        self.rotate_subtree(atom2, atom1, delta_angle_rad,
-                                            atom1.draw.position)
+                            closest_position = closest_atom.draw.previous_position
 
-                        fixed_atoms.add(atom2)
-                        i = 0
                     else:
-                        if angle_degrees == 120.0:
-                            first_angle_cyclic = 120.0
-                        elif angle_degrees == 60.0:
-                            first_angle_cyclic = 60.0
-                        i += 1
-
-                # Other way around... (first one in ring, after cycle)
-                elif atom1.inside_ring and not atom2.inside_ring and \
-                        backbone_atoms[i - 1].inside_ring:
-                    if first_angle_cyclic == 60.0:
-                        correct_angle_deg = 120.0
-                    elif first_angle_cyclic == 120.0:
-                        correct_angle_deg = 60.0
-                    if angle_degrees != correct_angle_deg:
-                        delta_angle_deg = correct_angle_deg - angle_degrees
-                        delta_angle_rad = math.radians(delta_angle_deg)
-                        self.rotate_subtree(atom2, atom1, delta_angle_rad,
-                                            atom1.draw.position)
-                        i = 0
+                        if not closest_atom.draw.previous_position:
+                            closest_position = drawn_neighbours[0].draw.position
+                        else:
+                            closest_position = closest_atom.draw.position
+
+                    if not atom.draw.previous_position:
+                        atom_previous_position = atom.drawn_neighbours[0].draw.position
                     else:
-                        i += 1
-                else:
-                    if angle_degrees != 120.0 and angle_degrees != 60:
-                        if round(math.degrees(get_angle(
-                                backbone_atoms[i - 1].draw.position,
-                                backbone_atoms[i].draw.position)),
-                                 3) == 120.0:
-                            correct_angle_deg = 60.0
-                        elif round(math.degrees(get_angle(
-                                backbone_atoms[i - 1].draw.position,
-                                backbone_atoms[i].draw.position)),
-                                   3) == 60.0:
-                            correct_angle_deg = 120.0
-                        delta_angle_deg = correct_angle_deg - angle_degrees
-                        delta_angle_rad = math.radians(delta_angle_deg)
-                        self.rotate_subtree(atom2, atom1, delta_angle_rad,
-                                            atom1.draw.position)
-                        i = 0
+                        atom_previous_position = atom.draw.previous_position
+                    #
+                    # atom.draw.position.rotate_away_from_vector(closest_position, atom_previous_position,
+                    #                                            math.radians(20))
+
+    def rotate_subtree_ring(self, root, masked, angle, center):
+        for atom in self.traverse_substructure(root, masked):
+            atom.draw.position.rotate_around_vector(angle, center)
+            for anchored_ring in atom.draw.anchored_rings:
+                if anchored_ring.center:
+                    anchored_ring.center.rotate_around_vector(angle, center)
+
+    def get_beta_atoms(self, backbone: List[Atom], backbone_atom: Atom, backbone_rings: List[Atom]) -> List[Atom]:
+        """
+        Returns atoms directly adjacent to the backbone atom that is not in the same ring as a backbone atom
+
+        Parameters
+        ----------
+        backbone: list of [Atom, ->] with each atom a backbone atom
+        backbone_atom: Atom instance, backbone atom for which the sidechains are determined
+        backbone_rings: list of [Atom, ->] with each atom a member of a ring that overlaps with the backbone
+
+        Returns
+        -------
+        beta_atoms: list of [Atom, ->], representing the atoms directly adjacent to the backbone atom
+        """
+        beta_atoms: List[Atom] = []
+        for neighbour in backbone_atom.neighbours:
+            if neighbour.type != 'H' and not neighbour.annotations.domain_type:
+                if neighbour not in backbone and neighbour not in backbone_rings:
+                    beta_atoms.append(neighbour)
+
+        return beta_atoms
+
+
+
+    def get_sidechains(self, backbone: List[Atom], backbone_atom: Atom, backbone_rings: List[Atom]) -> List[List[Atom]]:
+        """
+        Returns the non-ring sidechains of a backbone atom
+
+        Parameters
+        ----------
+        backbone: list of [Atom, ->] with each atom a backbone atom
+        backbone_atom: Atom instance, backbone atom for which the sidechains are determined
+        backbone_rings: list of [Atom, ->] with each atom a member of a ring that overlaps with the backbone
+
+        Returns
+        -------
+        sidechains: list of [[Atom, ->] ->], representing the sidechains coming out of the backbone atom
+
+        """
+        sidechains: List[List[Atom]] = []
+        beta_atoms = self.get_beta_atoms(backbone, backbone_atom, backbone_rings)
+        for beta_atom in beta_atoms:
+            sidechain: List[Atom] = []
+
+            for atom in self.traverse_substructure(beta_atom, {backbone_atom}):
+                sidechain.append(atom)
+            sidechains.append(sidechain)
+        return sidechains
+
+    def get_sidechain_bonds(self, sidechain: List[Atom]) -> List[Bond]:
+        """
+        Returns a list of bonds that exist between sidechain atoms
+
+        Parameters
+        ----------
+        sidechain: list of [Atom, ->]
+
+        Returns
+        -------
+        sidechain_bonds: list of [Bond, ->]
+
+        """
+        bonds: Set[Bond] = set()
+
+        for atom in sidechain:
+            for neighbour in atom.neighbours:
+                if neighbour in sidechain:
+                    bonds.add(self.structure.bond_lookup[atom][neighbour])
+
+        sidechain_bonds: List[Bond] = list(bonds)
+
+        return sidechain_bonds
+
+    def position_sidechains(self, backbone, backbone_to_placement, atoms_in_rings):
+        backbone_atom_before = None
+        backbone_to_neighbours = {}
+
+        for backbone_atom in backbone:
+            neighbours = []
+            for neighbour in backbone_atom.neighbours:
+                if neighbour.type != 'H' and not neighbour.annotations.domain_type:
+                    if neighbour not in backbone and neighbour not in atoms_in_rings \
+                            and neighbour not in neighbours:
+                        neighbours.append(neighbour)
+            backbone_to_neighbours[backbone_atom] = neighbours
+
+        for backbone_atom, neighbours in backbone_to_neighbours.items():
+            if backbone_atom in backbone_to_placement:
+                placement = backbone_to_placement[backbone_atom]
+                if len(neighbours) == 0:
+                    pass
+                elif len(neighbours) == 1:
+                    neighbour = neighbours[0]
+
+                    current_angle = get_angle(backbone_atom.draw.position, neighbour.draw.position)
+
+                    if placement == 'right':
+                        desired_angle = 180.0
+                    elif placement == 'left':
+                        desired_angle = 0.0
                     else:
-                        if i >= 1:
-                            if angle_degrees == 120.0:
-                                if round(math.degrees(get_angle(
-                                        backbone_atoms[
-                                            i - 1].draw.position,
-                                        backbone_atoms[i].draw.position)),
-                                         3) == 120:
-                                    correct_angle_deg = 60.0
-                                    delta_angle_deg = correct_angle_deg - angle_degrees
-                                    delta_angle_rad = math.radians(
-                                        delta_angle_deg)
-                                    self.rotate_subtree(atom2, atom1,
-                                                        delta_angle_rad,
-                                                        atom1.draw.position)
-                                    i = 0
-                                else:
-                                    i += 1
-                            elif angle_degrees == 60.0:
-                                if round(math.degrees(get_angle(
-                                        backbone_atoms[
-                                            i - 1].draw.position,
-                                        backbone_atoms[i].draw.position)),
-                                         3) == 60:
-                                    correct_angle_deg = 120.0
-                                    delta_angle_deg = correct_angle_deg - angle_degrees
-                                    delta_angle_rad = math.radians(
-                                        delta_angle_deg)
-                                    self.rotate_subtree(atom2, atom1,
-                                                        delta_angle_rad,
-                                                        atom1.draw.position)
-                                    i = 0
-                                else:
-                                    i += 1
+                        raise ValueError("Placement must be 'left' or 'right'.")
+                    # if ring in central chain but last member or tertiary carbon
+                    if backbone_atom in atoms_in_rings and backbone_atom_before in atoms_in_rings and backbone_atom_before:
+                        desired_angle += 180
+
+                    required_rotation_deg = desired_angle - current_angle
+                    required_rotation_rad = math.radians(required_rotation_deg)
+
+                    self.rotate_subtree(neighbour, backbone_atom, required_rotation_rad, backbone_atom.draw.position)
+
+                elif len(neighbours) == 2:
+                    neighbour_1, neighbour_2 = neighbours
+
+                    current_angle_1 = get_angle(backbone_atom.draw.position, neighbour_1.draw.position)
+                    current_angle_2 = get_angle(backbone_atom.draw.position, neighbour_2.draw.position)
+
+                    if placement == 'right':
+                        desired_angle_1 = 140.0
+                        desired_angle_2 = 220.0
+                    elif placement == 'left':
+                        desired_angle_1 = 40.0
+                        desired_angle_2 = -40.0
+                    else:
+                        raise ValueError("Placement must be 'left' or 'right'.")
+
+                    required_rotation_deg_1 = desired_angle_1 - current_angle_1
+                    required_rotation_rad_1 = math.radians(required_rotation_deg_1)
+
+                    required_rotation_deg_2 = desired_angle_2 - current_angle_2
+                    required_rotation_rad_2 = math.radians(required_rotation_deg_2)
+
+                    self.rotate_subtree(neighbour_1, backbone_atom, required_rotation_rad_1, backbone_atom.draw.position)
+                    self.rotate_subtree(neighbour_2, backbone_atom, required_rotation_rad_2, backbone_atom.draw.position)
+                elif len(neighbours) == 3:
+                    if backbone_atom != backbone[-1]:
+                        raise ValueError("Central backbone atoms can only have two non-backbone neighbours at most")
+                    else:
+                        neighbour_1, neighbour_2, neighbour_3 = neighbours
+
+                        current_angle_1 = get_angle(backbone_atom.draw.position, neighbour_1.draw.position)
+                        current_angle_2 = get_angle(backbone_atom.draw.position, neighbour_2.draw.position)
+                        current_angle_3 = get_angle(backbone_atom.draw.position, neighbour_3.draw.position)
+
+                        if placement == 'right':
+                            desired_angle_1 = 140.0
+                            desired_angle_2 = 220.0
+                            desired_angle_3 = 60.0
+                        elif placement == 'left':
+                            desired_angle_1 = 40.0
+                            desired_angle_2 = -40.0
+                            desired_angle_3 = 120.0
                         else:
-                            i += 1
+                            raise ValueError("Placement must be 'left' or 'right'.")
 
-            # Force pk/amino acid sidechains to stick out straight from each side
-            i = 1
-            while i < (len(backbone_atoms)):
-                terminal_carboxylic_acid = False
-                atom = backbone_atoms[i]
-                atom_neighbours = []
-                atom_neighbour_types = []
-                connected_to_sidechain = False
-                for neighbour in atom.neighbours:
-                    atom_neighbours.append(neighbour)
-                    atom_neighbour_types.append(neighbour.type)
-
-                    if neighbour not in backbone_atoms and \
-                            neighbour.type != 'H' and neighbour.type != 'S' and\
-                            neighbour.type == 'O' and \
-                            self.structure.bond_lookup[neighbour][atom].type == 'double':
-                        first_atom_sidechain = neighbour
-                        connected_to_sidechain = True
-                        if backbone_atoms[i - 1].draw.position.x < \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'right'
-                        elif backbone_atoms[i - 1].draw.position.x > \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'left'
-                    elif neighbour not in backbone_atoms and \
-                            neighbour.type != 'H' and neighbour.type != 'S' and\
-                            not neighbour.inside_ring:
-                        first_atom_sidechain = neighbour
-                        connected_to_sidechain = True
-                        if backbone_atoms[i - 1].draw.position.x < \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'right'
-                        elif backbone_atoms[i - 1].draw.position.x > \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'left'
-
-                    elif neighbour not in backbone_atoms and \
-                            neighbour.type != 'H' and neighbour.type != 'S' and \
-                            neighbour.inside_ring and any(
-                            bond.type == 'double' for bond in
-                            neighbour.bonds) and atom == backbone_atoms[-1]:
-                        first_atom_sidechain = neighbour
-                        connected_to_sidechain = True
-                        if backbone_atoms[i - 1].draw.position.x < \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'diagonal_right'
-                        elif backbone_atoms[i - 1].draw.position.x > \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'diagonal_left'
-
-                    elif neighbour not in backbone_atoms and \
-                            neighbour.type != 'H' and neighbour.type != 'S' and \
-                            neighbour.in_ring(self.structure) and not atom.in_ring(self.structure):
-                        first_atom_sidechain = neighbour
-                        connected_to_sidechain = True
-                        if backbone_atoms[i - 1].draw.position.x < \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'right'
-                        elif backbone_atoms[i - 1].draw.position.x > \
-                                backbone_atoms[i].draw.position.x:
-                            sidechain_orientation = 'left'
-
-                    # If bond is directly connected to sidechain, check&rotate
-                    if connected_to_sidechain:
-                        angle = get_angle(atom.draw.position,
-                                          first_atom_sidechain.draw.position)
-                        angle_degrees = round(math.degrees(angle), 3)
-                        # Check if it is a terminal carboxylic acid group
-                        if atom_neighbour_types.count('O') == 2 and len(
-                                atom_neighbour_types) == 3:
-                            for next_atom in atom_neighbours:
-                                if next_atom.type == 'O':
-                                    if \
-                                    self.structure.bond_lookup[next_atom][atom].type == 'single':
-                                        hydroxyl = next_atom
-                                        angle2 = get_angle(
-                                            atom.draw.position,
-                                            hydroxyl.draw.position)
-                                        angle_degrees2 = round(
-                                            math.degrees(angle2),
-                                            3)
-                                        if last_angle_degrees == 120.0:
-                                            correct_angle_deg = 60.0
-                                        elif last_angle_degrees == 60.0:
-                                            correct_angle_deg = 120.0
-                                        delta_angle_deg = correct_angle_deg - angle_degrees2
-                                        delta_angle_rad = math.radians(
-                                            delta_angle_deg)
-                                        self.rotate_subtree(hydroxyl,
-                                                            atom,
-                                                            delta_angle_rad,
-                                                            atom.draw.position)
-                                    elif \
-                                    self.structure.bond_lookup[next_atom][
-                                        atom].type == 'double':
-                                        carbonyl = next_atom
-                                        angle2 = get_angle(
-                                            atom.draw.position,
-                                            carbonyl.draw.position)
-                                        angle_degrees2 = round(
-                                            math.degrees(angle2),
-                                            3)
-                                        correct_angle_deg = 0
-                                        delta_angle_deg = correct_angle_deg - angle_degrees2
-                                        delta_angle_rad = math.radians(
-                                            delta_angle_deg)
-                                        self.rotate_subtree(carbonyl, atom,
-                                                            delta_angle_rad,
-                                                            atom.draw.position)
-                                    terminal_carboxylic_acid = True
-                        if not terminal_carboxylic_acid:
-                            if sidechain_orientation == 'right':
-                                correct_angle_deg = 180
-                            elif sidechain_orientation == 'left':
-                                correct_angle_deg = 0
-                            elif sidechain_orientation == 'diagonal_left':
-                                correct_angle_deg = 120
-                            elif sidechain_orientation == 'diagonal_right':
-                                correct_angle_deg = 60
-                            delta_angle_deg = correct_angle_deg - angle_degrees
-                            delta_angle_rad = math.radians(delta_angle_deg)
-                            self.rotate_subtree(first_atom_sidechain, atom,
-                                                delta_angle_rad,
-                                                atom.draw.position)
-                i += 1
-
-            # If the drawer rotated the entire structure, correct this
-            angle = get_angle(pcp.draw.position,
-                              sulphur.draw.position)
-            angle_degrees = round(math.degrees(angle), 3)
-            if angle_degrees != 90.0:
-                correct_angle_deg = 90
-                delta_angle_deg = correct_angle_deg - angle_degrees
-                delta_angle_rad = math.radians(delta_angle_deg)
-                self.rotate_subtree(sulphur, pcp, delta_angle_rad,
-                                    pcp.draw.position)
-
-            # Fix rotation bulky sidechains so carboxyl groups dont need to move
-            i = 1
-            while i < (len(backbone_atoms)):
-                atom = backbone_atoms[i]
-                atom_neighbours = []
-                atom_neighbour_types = []
-                for neighbour in atom.neighbours:
-                    atom_neighbours.append(neighbour)
-                    atom_neighbour_types.append(neighbour.type)
-                    if neighbour not in backbone_atoms and \
-                            neighbour.type != 'H' and neighbour.type != 'S' and\
-                            not neighbour.inside_ring:
-                        first_atom_sidechain = neighbour
-                        for further_atom in first_atom_sidechain.neighbours:
-                            types = []
-                            for further_atom_neighbour in further_atom.neighbours:
-                                types.append(further_atom_neighbour.type)
-                            if further_atom.type == 'C' and further_atom not in backbone_atoms and (
-                                    (types.count(
-                                            'C') == 3) or (
-                                            types.count('O') == 2 and
-                                            types.count('H') == 0) or
-                                    (types.count('N') == 1 and
-                                     types.count('O') == 1 and
-                                     types.count('H') == 0) or
-                                    (types.count('C') == 2 and
-                                     types.count('N') == 1 and
-                                     types.count('H') == 0)):
-                                angle_bulky_sidechain = get_angle(
-                                    first_atom_sidechain.draw.position,
-                                    further_atom.draw.position)
-                                angle_bulky_sidechain = round(
-                                    math.degrees(angle_bulky_sidechain), 3)
-                                if atom.draw.position.x < first_atom_sidechain.draw.position.x:
-                                    correct_angle_deg = 160
-                                elif further_atom.draw.position.x < first_atom_sidechain.draw.position.x:
-                                    correct_angle_deg = 20
-                                delta_angle_deg = correct_angle_deg - angle_bulky_sidechain
-                                delta_angle_rad = math.radians(
-                                    delta_angle_deg)
-                                self.rotate_subtree(further_atom,
-                                                    first_atom_sidechain,
-                                                    delta_angle_rad,
-                                                    first_atom_sidechain.draw.position)
-                    # Fix incorrect rotation carbonyl groups
-                    if neighbour.type == 'O' and \
-                            self.structure.bond_lookup[atom][
-                                neighbour].type == 'double':
-                        correctly_rotated = True
-                        if neighbour.draw.position.x > atom.draw.position.x and atom.draw.position.x < \
-                                backbone_atoms[i - 1].draw.position.x:
-                            correct_angle_deg = 0
-                            correctly_rotated = False
-                        elif neighbour.draw.position.y != atom.draw.position.y and atom.draw.position.x < \
-                                backbone_atoms[i - 1].draw.position.x:
-                            correct_angle_deg = 0
-                            correctly_rotated = False
-                        elif neighbour.draw.position.x < atom.draw.position.x and atom.draw.position.x > \
-                                backbone_atoms[i - 1].draw.position.x:
-                            correct_angle_deg = 180
-                            correctly_rotated = False
-                        elif neighbour.draw.position.y != atom.draw.position.y and atom.draw.position.x > \
-                                backbone_atoms[i - 1].draw.position.x:
-                            correct_angle_deg = 180
-                            correctly_rotated = False
-                        if not correctly_rotated:
-                            angle = get_angle(atom.draw.position,
-                                              neighbour.draw.position)
-                            angle_degrees = round(math.degrees(angle), 3)
-                            delta_angle_deg = correct_angle_deg - angle_degrees
-                            delta_angle_rad = math.radians(delta_angle_deg)
-                            self.rotate_subtree(neighbour,
-                                                atom, delta_angle_rad,
-                                                atom.draw.position)
-                i += 1
+                        required_rotation_deg_1 = desired_angle_1 - current_angle_1
+                        required_rotation_rad_1 = math.radians(required_rotation_deg_1)
 
-            # self.resolve_primary_overlaps()
-            self.total_overlap_score, sorted_overlap_scores, atom_to_scores = self.get_overlap_score()
-            central_chain_bonds = set()
-            for bond in self.structure.bonds.values():
-                if bond.atom_1.annotations.in_central_chain or\
-                        bond.atom_2.annotations.in_central_chain:
-                    central_chain_bonds.add(bond)
+                        required_rotation_deg_2 = desired_angle_2 - current_angle_2
+                        required_rotation_rad_2 = math.radians(required_rotation_deg_2)
 
-            self.finetune_overlap_resolution(masked_bonds=central_chain_bonds, highest_atom=sulphur)
-            self.resolve_secondary_overlaps(sorted_overlap_scores)
+                        required_rotation_deg_3 = desired_angle_3 - current_angle_3
+                        required_rotation_rad_3 = math.radians(required_rotation_deg_3)
+
+                        self.rotate_subtree(neighbour_1, backbone_atom, required_rotation_rad_1,
+                                            backbone_atom.draw.position)
+                        self.rotate_subtree(neighbour_2, backbone_atom, required_rotation_rad_2,
+                                            backbone_atom.draw.position)
+                        self.rotate_subtree(neighbour_3, backbone_atom, required_rotation_rad_3,
+                                            backbone_atom.draw.position)
 
-    # End NRPS rotation code
+                else:
+                    raise ValueError("Terminal backbone atoms can only have three non-backbone neighbours at most")
+                backbone_atom_before = backbone_atom
+            # We are in a ring that we cannot linearise; rotate the whole ring straight down
+            else:
+                drawing_ring = self.get_ring(backbone_atom.draw.rings[0])
+                center = Vector(0, 0)
+                for atom in drawing_ring.members:
+                    center.add(atom.draw.position)
+
+                center.divide(len(drawing_ring.members))
+                angle = get_angle(backbone_atom_before.draw.position,
+                                  center)
+
+                desired_angle = 90.0
+
+                required_rotation_deg = desired_angle - angle
+                required_rotation_rad = math.radians(required_rotation_deg)
+
+                masked = {backbone_atom_before}
+
+                # for atom in drawing_ring.members:
+                for atom in self.traverse_substructure(backbone_atom, masked):
+
+                    if atom != backbone_atom_before:
+                        atom.draw.position.rotate_around_vector(required_rotation_rad, backbone_atom_before.draw.position)
+                break
 
     def plot_halflines_s_domain(self, line, ax, midpoint):
-        truncated_line = line.get_truncated_line(self.options.short_bond_length)
+        truncated_line = line.get_truncated_line(
+            self.options.short_bond_length)
         self.plot_line_dashed(truncated_line, ax, color='#a6a6a6')
 
     def plot_line_dashed(self, line, ax, color='grey'):
         with matplotlib.rc_context({'path.sketch': (5, 10, 1)}):
             ax.plot([line.point_1.x, line.point_2.x],
                     [line.point_1.y, line.point_2.y], color=color,
                     linewidth=self.line_width/1.5)
@@ -1315,11 +1392,282 @@
         elif (carbon_x - sidechainatom_x) > 10:
             delta_x = -1.5
         else:
             delta_x = 0.0
 
         return delta_x
 
+    def draw_svg(self, annotation: Union[None, str] = None, numbered_atoms: List = None) -> str:
+
+        self.set_annotation_for_grouping(annotation)
+
+        ring_centers_x = []
+        ring_centers_y = []
+
+        for ring in self.rings:
+            self.set_ring_center(ring)
+
+            ring_centers_x.append(ring.center.x)
+            ring_centers_y.append(ring.center.y)
+
+        for bond_nr, bond in self.structure.bonds.items():
+            if bond.atom_1.draw.positioned and bond.atom_2.draw.positioned:
+                line = Line(bond.atom_1.draw.position, bond.atom_2.draw.position, bond.atom_1, bond.atom_2)
+                midpoint = line.get_midpoint()
+
+                if bond.type == 'single':
+                    if bond in self.chiral_bonds:
+
+                        orientation, chiral_center = self.chiral_bond_to_orientation[bond]
+                        self._draw_chiral_bond(orientation, chiral_center, line, midpoint)
+                    else:
+                        self._draw_halflines(line, midpoint)
+                elif bond.type == 'double':
+                    if not self._is_terminal(bond.atom_1) and not self._is_terminal(bond.atom_2):
+                        self._draw_halflines(line, midpoint)
+
+                        common_ring_numbers = self._get_common_rings(bond.atom_1, bond.atom_2)
+
+                        if common_ring_numbers:
+                            common_rings = []
+                            for ring_nr in common_ring_numbers:
+                                common_rings.append(self.get_ring(ring_nr))
+
+                            common_rings.sort(key=lambda x: len(x.members))
+                            common_ring = common_rings[0]
+                            ring_centre = common_ring.center
+                            second_line = line.double_line_towards_center(ring_centre, self.options.bond_spacing,
+                                                                          self.options.double_bond_length)
+                            second_line_midpoint = second_line.get_midpoint()
+                            self._draw_halflines_double(second_line, second_line_midpoint)
+
+                        else:
+                            bond_neighbours = bond.atom_1.drawn_neighbours + bond.atom_2.drawn_neighbours
+                            if bond_neighbours:
+                                vectors = [atom.draw.position for atom in bond_neighbours]
+                                gravitational_point = Vector.get_average(vectors)
+                                second_line = line.double_line_towards_center(gravitational_point,
+                                                                              self.options.bond_spacing,
+                                                                              self.options.double_bond_length)
+                                second_line_midpoint = second_line.get_midpoint()
+                                self._draw_halflines_double(second_line, second_line_midpoint)
+                            else:
+                                print("Shouldn't happen!")
+                    else:
+                        if self._is_terminal(bond.atom_1) and self._is_terminal(bond.atom_2):
+                            dummy_1 = Vector(bond.atom_1.draw.position.x + 1, bond.atom_1.draw.position.y + 1)
+                            dummy_2 = Vector(bond.atom_1.draw.position.x - 1, bond.atom_1.draw.position.y - 1)
+                            double_bond_line_1 = line.double_line_towards_center(dummy_1,
+                                                                                 self.options.bond_spacing / 2.0,
+                                                                                 self.options.double_bond_length)
+                            double_bond_line_1_midpoint = double_bond_line_1.get_midpoint()
+                            double_bond_line_2 = line.double_line_towards_center(dummy_2,
+                                                                                 self.options.bond_spacing / 2.0,
+                                                                                 self.options.double_bond_length)
+                            double_bond_line_2_midpoint = double_bond_line_2.get_midpoint()
+
+                            self._draw_halflines_double(double_bond_line_1, double_bond_line_1_midpoint)
+                            self._draw_halflines_double(double_bond_line_2, double_bond_line_2_midpoint)
+
+                        else:
+
+                            if self._is_terminal(bond.atom_1):
+                                terminal_atom = bond.atom_1
+                                branched_atom = bond.atom_2
+                            else:
+                                terminal_atom = bond.atom_2
+                                branched_atom = bond.atom_1
+
+                            if len(branched_atom.drawn_neighbours) >= 3:
+                                closest_two = self.get_sorted_distances_from_list(terminal_atom,
+                                                                                  branched_atom.drawn_neighbours)
+                                closest_atom_1 = closest_two[0][1]
+                                closest_atom_2 = closest_two[1][1]
+
+                                line = Line(terminal_atom.draw.position, branched_atom.draw.position, terminal_atom,
+                                            branched_atom)
+
+                                double_bond_line_1, double_bond_line_2 = line.get_perpendicular_lines(
+                                    self.options.bond_spacing / 2.0)
+                                terminal_atom_pos_1 = double_bond_line_1.get_atom_coords(terminal_atom)
+                                terminal_atom_pos_2 = double_bond_line_2.get_atom_coords(terminal_atom)
+
+                                closest_atom_to_pos_1 = terminal_atom_pos_1.get_closest_atom(closest_atom_1,
+                                                                                             closest_atom_2)
+                                closest_atom_to_pos_2 = terminal_atom_pos_2.get_closest_atom(closest_atom_1,
+                                                                                             closest_atom_2)
+
+                                bond_1_line = Line(branched_atom.draw.position, closest_atom_to_pos_1.draw.position,
+                                                   branched_atom, closest_atom_to_pos_1)
+                                bond_2_line = Line(branched_atom.draw.position, closest_atom_to_pos_2.draw.position,
+                                                   branched_atom, closest_atom_to_pos_2)
+
+                                double_bond_line_1_midpoint = double_bond_line_1.get_midpoint()
+                                double_bond_line_2_midpoint = double_bond_line_2.get_midpoint()
+
+                                intersection_1 = double_bond_line_1.find_intersection(bond_1_line)
+                                intersection_2 = double_bond_line_2.find_intersection(bond_2_line)
+
+                                if terminal_atom.draw.position.x > branched_atom.draw.position.x:
+                                    # check for parallel lines
+                                    if intersection_1 and intersection_1.x < 100000 and intersection_1.y < 100000:
+                                        double_bond_line_1.point_1 = intersection_1
+                                    if intersection_2 and intersection_2.x < 100000 and intersection_2.y < 100000:
+                                        double_bond_line_2.point_1 = intersection_2
+
+                                else:
+                                    # check for parallel lines
+                                    if intersection_1 and intersection_1.x < 100000 and intersection_1.y < 100000:
+                                        double_bond_line_1.point_2 = intersection_1
+                                    if intersection_2 and intersection_2.x < 100000 and intersection_2.y < 100000:
+                                        double_bond_line_2.point_2 = intersection_2
+
+                                self._draw_halflines(double_bond_line_1, double_bond_line_1_midpoint)
+                                self._draw_halflines(double_bond_line_2, double_bond_line_2_midpoint)
+
+                            else:
+                                self._draw_halflines(line, midpoint)
+
+                                bond_neighbours = bond.atom_1.drawn_neighbours + bond.atom_2.drawn_neighbours
+                                if bond_neighbours:
+                                    vectors = [atom.draw.position for atom in bond_neighbours]
+                                    gravitational_point = Vector.get_average(vectors)
+                                    second_line = line.get_parallel_line(gravitational_point,
+                                                                         self.options.bond_spacing)
+                                    second_line_midpoint = second_line.get_midpoint()
+                                    self._draw_halflines(second_line, second_line_midpoint)
+                                else:
+                                    print("Shouldn't happen!")
+
+                elif bond.type == 'triple':
+                    self._draw_halflines(line, midpoint)
+                    line_1, line_2 = line.get_parallel_lines(self.options.bond_spacing)
+                    line_1_midpoint = line_1.get_midpoint()
+                    line_2_midpoint = line_2.get_midpoint()
+                    self._draw_halflines(line_1, line_1_midpoint)
+                    self._draw_halflines(line_2, line_2_midpoint)
+
+        for atom in self.structure.graph:
+            if atom.draw.positioned:
+                svg_text = ''
+                svg_h_text = ''
+                svg_charge_text = ''
+                svg_h_count_text = ''
+
+                if atom.type != 'C' or atom.draw.draw_explicit or atom.charge:
+                    if atom.type == 'C' and not atom.charge:
+                        svg_text = self._draw_text('.', atom.draw.position.x, atom.draw.position.y - 2,
+                                                   color=atom.draw.colour)
+                    else:
+                        svg_text = self._draw_text(atom.type, atom.draw.position.x, atom.draw.position.y,
+                                                   color=atom.draw.colour)
+                if hasattr(atom, "domain_type") and atom.annotations.domain_type in ["Leader", "Follower", "ACP", "PCP"]:
+                    svg_text = ''
+
+                        # TODO: Make this possible in svg writing
+                        # text = self.set_r_group_indices_subscript(atom.type)
+
+                orientation = self._get_hydrogen_text_orientation(atom)
+
+                # Swap up-down orientation due to swapped svg coordinate system
+                if orientation == 'H_below_atom':
+                    orientation = 'H_above_atom'
+                elif orientation == 'H_above_atom':
+                    orientation = 'H_below_atom'
+
+                if atom.type != 'C' or atom.draw.draw_explicit or atom.charge:
+
+                    hydrogen_count = 0
+
+                    for neighbour in atom.neighbours:
+                        if neighbour.type == 'H' and not neighbour.draw.is_drawn:
+                            hydrogen_count += 1
+
+                    h_x = atom.draw.position.x
+                    h_y = atom.draw.position.y
+                    h_subscript_x = atom.draw.position.x
+                    h_subscript_y = atom.draw.position.y + 3
+                    charge_x = atom.draw.position.x + 6
+                    charge_y = atom.draw.position.y - 3
+
+                    if orientation == 'H_below_atom':
+                        h_y = atom.draw.position.y + 7
+                        h_subscript_x += 2
+                        h_subscript_y += 10
+                    elif orientation == 'H_above_atom':
+                        h_y = atom.draw.position.y - 7
+                        h_subscript_x += 2
+                        h_subscript_y -= 4
+                    elif orientation == 'H_before_atom':
+                        if hydrogen_count > 1:
+                            h_x -= 10
+                            h_subscript_x -= 5
+                        elif hydrogen_count == 1:
+                            h_x -= 6
+                    else:
+                        h_x += len(atom.type) * 6
+                        h_subscript_x += len(atom.type) * 6 + 5
+
+                    if abs(atom.charge):
+                        if hydrogen_count and orientation == 'H_after_atom':
+                            if hydrogen_count > 1:
+                                charge_x += len(atom.type) * 6 + 7
+                            else:
+                                charge_x += len(atom.type) * 6 + 2
+
+                    h_pos = Vector(h_x, h_y)
+                    h_subscript_pos = Vector(h_subscript_x, h_subscript_y)
+                    charge_pos = Vector(charge_x, charge_y)
+
+                    if hydrogen_count:
+                        svg_h_text = self._draw_text('H', h_pos.x, h_pos.y,
+                                                     color=atom.draw.colour)
+                        if hydrogen_count > 1:
+                            svg_h_count_text = self._draw_text(hydrogen_count, h_subscript_pos.x, h_subscript_pos.y,
+                                                               font_size=self.options.svg_font_size_small,
+                                                               color=atom.draw.colour)
+                    if atom.charge:
+                        if atom.charge > 0:
+                            charge_symbol = '+'
+                        else:
+                            charge_symbol = '-'
+
+                        if abs(atom.charge) > 1:
+                            charge_text = f"{abs(atom.charge)}{charge_symbol}"
+                        else:
+                            charge_text = charge_symbol
+
+                        svg_charge_text = self._draw_text(charge_text, charge_pos.x, charge_pos.y,
+                                                          font_size=self.options.svg_font_size_small,
+                                                          color=atom.draw.colour)
+
+                if svg_text or svg_h_text or svg_charge_text or svg_h_count_text:
+                    if self.structure_id:
+                        text_group = f'<g id="atom_{atom}_{self.structure_id}_text">\n'
+                    else:
+                        text_group = f'<g id="atom_{atom}_text">\n'
+                    if svg_text:
+                        text_group += svg_text
+                        text_group += '\n'
+                    if svg_h_text:
+                        text_group += svg_h_text
+                        text_group += '\n'
+                    if svg_charge_text:
+                        text_group += svg_charge_text
+                        text_group += '\n'
+                    if svg_h_count_text:
+                        text_group += svg_h_count_text
+                        text_group += '\n'
+                    text_group += '</g>'
+                    self._add_svg_element(text_group, atom)
+
+        if numbered_atoms:
+            self.show_atom_numbers(numbered_atoms)
+
+        svg = self._assemble_svg()
+        return svg
+
+
 def get_angle(vector1, vector2):
     difference = Vector.subtract_vectors(vector1, vector2)
     difference_angle = difference.angle()
-    return difference_angle
+    return math.degrees(difference_angle)
```

### Comparing `raichu-0.0.2/raichu/module.py` & `raichu-1.0.0/raichu/module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from typing import List, Union
 
 from pikachu.general import read_smiles
 from pikachu.chem.structure import Structure
+from pikachu.chem.atom import Atom
 
-from raichu.domain.domain import Domain, TailoringDomain, RecognitionDomain, \
-    SynthesisDomain, CarrierDomain, TerminationDomain
-from raichu.central_chain_detection.label_central_chain import label_pk_central_chain, label_nrp_central_chain
+from raichu.class_domain import CarrierDomain as ClassCarrierDomain
+from raichu.domain.domain import (
+    Domain,
+    TailoringDomain,
+    RecognitionDomain,
+    SynthesisDomain,
+    CarrierDomain,
+    TerminationDomain,
+)
+from raichu.central_chain_detection.label_central_chain import (
+    label_pk_central_chain,
+    label_nrp_central_chain,
+)
 from raichu.attach_to_domain import attach_to_domain_pk, attach_to_domain_nrp
 from enum import Enum, unique
-from pikachu.drawing.drawing import Drawer
-from raichu.drawing.drawer import RaichuDrawer
+from raichu.substrate import PKSSubstrate
+
 
 @unique
 class ModuleType(Enum):
     NRPS = 1
     PKS = 2
 
     @staticmethod
@@ -41,17 +52,20 @@
 @unique
 class NRPSDomainType(Enum):
     A = 1
     C = 2
     PCP = 3
     E = 4
     nMT = 5
-    TE = 6
-    TD = 7
-    UNKNOWN = 8
+    CYC = 6
+    TE = 7
+    TD = 8
+    UNKNOWN = 9
+    OX = 10
+    CAL = 11
 
     @staticmethod
     def from_string(label: str) -> "NRPSDomainType":
         for value in NRPSDomainType:
             if str(value.name) == label:
                 return value
         raise ValueError(f"Unknown NRPS domain type: {label}")
@@ -75,128 +89,195 @@
     DUMMY_EDH = 14  # Z-configured double bonds
     DUMMY_AH = 15  # Alpha-hydroxylase
     DUMMY_GDH = 16  # Gamma-beta-dehydrogenase
     DUMMY_ZGDH = 17  # Z-Gamma-beta-dehydrogenase
     DUMMY_EGDH = 18  # E-Gamma-beta-dehydrogenase
     DUMMY_OMT = 19  # Beta-Hydroxymethyltransferase
     DUMMY_BMT = 20  # Beta-Methyltransferase
+    CAL = 21
+    DUMMY_AT = 22
 
     @staticmethod
     def from_string(label: str) -> "PKSDomainType":
         for value in PKSDomainType:
             if str(value.name) == label:
                 return value
         raise ValueError(f"Unknown PKS domain type: {label}")
 
 
 class _Module:
 
-    def __init__(self, nr: int, module_type: str, domains: List[Domain], *,
-                 module_subtype: Union[str, None] = None,
-                 starter: bool = False, terminator: bool = False) -> None:
+    def __init__(
+        self,
+        nr: int,
+        module_type: str,
+        domains: List[Domain],
+        *,
+        module_subtype: Union[str, None] = None,
+        starter: bool = False,
+        terminator: bool = False,
+    ) -> None:
         self.id = nr
         self.type = ModuleType.from_string(module_type)
         self.subtype = None
 
         if module_subtype is not None:
-            if self.type.name == 'PKS':
+            if self.type.name == "PKS":
                 self.subtype = PKSModuleSubtype.from_string(module_subtype)
             else:
-                raise ValueError(f"Module subtypes not supported for {self.type.name} modules.")
+                raise ValueError(
+                    f"Module subtypes not supported for {self.type.name} modules."
+                )
 
         self.domains = domains
 
         self.recognition_domain = None
         self.synthesis_domain = None
         self.carrier_domain = None
         self.termination_domain = None
 
         self.tailoring_domains = []
 
+        self.is_broken = False
         self.is_starter_module = starter
         self.is_termination_module = terminator
 
         for domain in self.domains:
-            if self.type.name == 'NRPS':
-                assert domain.type.name in [v.name for v in NRPSDomainType]
-            if self.type.name == 'PKS':
-                assert domain.type.name in [v.name for v in PKSDomainType]
+            if self.type.name == "NRPS":
+                if domain.type.name not in [v.name for v in NRPSDomainType]:
+                    raise ValueError(f"Unknown NRPS domain type {domain.type.name}")
+            if self.type.name == "PKS":
+                if domain.type.name not in [v.name for v in PKSDomainType]:
+                    raise ValueError(f"Unknown PKS domain type {domain.type.name}")
 
             if domain.used and domain.active:
                 if isinstance(domain, TailoringDomain):
-                    if domain.type.name not in [d.type.name for d in self.tailoring_domains]:
+                    if domain.type.name not in [
+                        d.type.name for d in self.tailoring_domains
+                    ]:
                         self.tailoring_domains.append(domain)
                     else:
-                        raise ValueError(f"Cannot have two used tailoring domains of type {domain.type.name} in one \
-module. Remove domain or set the 'used' or 'active' flag to False")
+                        raise ValueError(
+                            f"Cannot have two used tailoring domains of type {domain.type.name} in one \
+module. Remove domain or set the 'used' or 'active' flag to False"
+                        )
 
                 if isinstance(domain, RecognitionDomain):
                     if not self.recognition_domain:
                         self.recognition_domain = domain
                     else:
-                        raise ValueError(f"Cannot have more than one used recognition domain in one \
-module. Remove a domain or set the 'used' or 'active' flag to False")
+                        raise ValueError(
+                            f"Cannot have more than one used recognition domain in one \
+module. Remove a domain or set the 'used' or 'active' flag to False"
+                        )
 
                 if isinstance(domain, SynthesisDomain) and domain.is_elongating:
                     if not self.synthesis_domain:
                         self.synthesis_domain = domain
                     else:
-                        raise ValueError("Cannot have more than one used and elongating synthesis domains \
-in one module. Remove a domain, set the 'used' or 'active' flag to False, or set the 'is_elongating' flag to False.")
+                        raise ValueError(
+                            "Cannot have more than one used and elongating synthesis domains \
+in one module. Remove a domain, set the 'used' or 'active' flag to False, or set the 'is_elongating' flag to False."
+                        )
 
                 if isinstance(domain, CarrierDomain):
                     if not self.carrier_domain:
                         self.carrier_domain = domain
                     else:
-                        raise ValueError("Cannot have more than one used carrier domain in one \
-module. Remove a domain or set the 'used' or 'active' flag to False")
+                        raise ValueError(
+                            "Cannot have more than one used carrier domain in one \
+module. Remove a domain or set the 'used' or 'active' flag to False"
+                        )
 
                 if isinstance(domain, TerminationDomain):
                     if not self.termination_domain:
                         self.termination_domain = domain
                         if not self.is_termination_module:
                             self.termination_domain.used = False
                     else:
-                        raise ValueError("Cannot have more than one used termination domain in one \
-module. Remove a domain or set the 'used' or 'active' flag to False")
-
+                        raise ValueError(
+                            "Cannot have more than one used termination domain in one \
+module. Remove a domain or set the 'used' or 'active' flag to False"
+                        )
+        # I would rather implement a "dont do anything"- broken module
         if not self.is_starter_module and not self.synthesis_domain:
-            if self.type.name == 'NRPS':
-                self.synthesis_domain = SynthesisDomain('C')
-            elif self.type.name == 'PKS':
-                self.synthesis_domain = SynthesisDomain('KS')
+            if "CYC" in [domain.type.name for domain in self.tailoring_domains]:
+                self.synthesis_domain = SynthesisDomain("DUMMY_C")
+            else:
+                self.is_broken = True
+
+        if (
+            not self.is_starter_module
+            and self.recognition_domain
+            and self.recognition_domain.domain_name == "CAL"
+        ):
+            self.is_broken = True
+
+        if module_subtype != "PKS_TRANS" and not self.recognition_domain:
+            self.is_broken = True
 
         if self.is_termination_module and not self.termination_domain:
             self.termination_domain = TerminationDomain("DUMMY_TE")
 
+        if not self.carrier_domain:
+            self.is_broken = True
+
+        if self.is_broken:
+            for domain in self.domains:
+                domain.used = False
+
+        for domain in self.domains[:]:
+            if "DUMMY" in domain.type.name:
+                self.domains.remove(domain)
+
     def run_module(self, structure: Union[Structure, None] = None):
         raise NotImplementedError
 
     def get_tailoring_domain(self, domain_name: str) -> Union[TailoringDomain, None]:
         for domain in self.tailoring_domains:
             if domain.type.name == domain_name:
                 return domain
 
         return
 
+    def add_module_label(self, structure):
+        for atom in structure.graph:
+            if type(atom) == Atom and not atom.annotations.has_annotation("module_nr"):
+                atom.annotations.add_annotation("module_nr", f"module_{self.id + 1:02}")
+
+            if type(atom) == ClassCarrierDomain:
+                for neighbour in structure.graph[atom]:
+                    if neighbour.type == "S":
+                        if not neighbour.annotations.has_annotation("module_nr"):
+                            neighbour.annotations.add_annotation(
+                                "module_nr", f"module_{self.id + 1:02}"
+                            )
+                        else:
+                            neighbour.annotations.module_nr = f"module_{self.id + 1:02}"
+
     def do_pks_tailoring(self, structure: Structure) -> Structure:
         kr_domain = self.get_tailoring_domain("KR")
         dh_domain = self.get_tailoring_domain("DH")
         er_domain = self.get_tailoring_domain("ER")
 
         if kr_domain and kr_domain.active and kr_domain.used:
             assert kr_domain.subtype is not None
             structure, kr_tailored = kr_domain.do_tailoring(structure)
             if kr_tailored:
-                if not kr_domain.subtype.name == 'C1' and not kr_domain.subtype.name == 'C2':
+                if (
+                    not kr_domain.subtype.name == "C1"
+                    and not kr_domain.subtype.name == "C2"
+                ):
                     if dh_domain and dh_domain.active and dh_domain.used:
                         structure, dh_tailored = dh_domain.do_tailoring(structure)
                         if dh_tailored:
                             if er_domain and er_domain.active and er_domain.used:
-                                structure, er_tailored = er_domain.do_tailoring(structure)
+                                structure, er_tailored = er_domain.do_tailoring(
+                                    structure
+                                )
                                 if not er_tailored:
                                     er_domain.used = False
 
                         else:
                             dh_domain.used = False
                             if er_domain:
                                 er_domain.used = False
@@ -211,73 +292,150 @@
                 dh_domain.used = False
             if er_domain:
                 er_domain.used = False
 
         return structure
 
     def do_nrps_tailoring(self, structure: Structure) -> Structure:
-        e_domain = self.get_tailoring_domain('E')
-        n_mt_domain = self.get_tailoring_domain('nMT')
+        e_domain = self.get_tailoring_domain("E")
+        n_mt_domain = self.get_tailoring_domain("nMT")
+        cyc_domain = self.get_tailoring_domain("CYC")
+        ox_domain = self.get_tailoring_domain("OX")
 
         if e_domain and e_domain.active and e_domain.used:
             structure, epimerized = e_domain.do_tailoring(structure)
             if not epimerized:
                 e_domain.used = False
         if n_mt_domain and n_mt_domain.active and n_mt_domain.used:
+
             structure, methylated = n_mt_domain.do_tailoring(structure)
             if not methylated:
                 n_mt_domain.used = False
 
+        if cyc_domain and cyc_domain.active and cyc_domain.used:
+            structure, cyclised = cyc_domain.do_tailoring(structure)
+            if not cyclised:
+                cyc_domain.used = False
+
+            if ox_domain and ox_domain.active and ox_domain.used:
+                structure, oxidated = ox_domain.do_tailoring(structure)
+                if not oxidated:
+                    ox_domain.used = False
+
+        elif ox_domain:
+            ox_domain.used = False
+
         return structure
 
     def release_chain(self, structure: Structure) -> Structure:
         assert structure
         assert self.termination_domain
 
         released_structure = self.termination_domain.release_chain(structure)
 
         return released_structure
 
 
 class LinearPKSModule(_Module):
 
     def __init__(self, nr, domains, starter=False, terminator=False):
-        super().__init__(nr, "PKS", domains, starter=starter, terminator=terminator, module_subtype="PKS_CIS")
+        super().__init__(
+            nr,
+            "PKS",
+            domains,
+            starter=starter,
+            terminator=terminator,
+            module_subtype="PKS_CIS",
+        )
 
     def run_module(self, structure: Union[Structure, None] = None) -> Structure:
-        if structure is None:
-            assert self.is_starter_module
-            starter_unit = read_smiles(self.recognition_domain.substrate.smiles)
-            label_pk_central_chain(starter_unit)
-            structure = attach_to_domain_pk(starter_unit)
+        if self.is_broken:
+            return structure
         else:
-            structure = self.synthesis_domain.do_elongation(structure, self.recognition_domain.substrate)
-
-        structure = self.do_pks_tailoring(structure)
-        # RaichuDrawer(structure).draw_structure()
-        return structure
+            if self.recognition_domain:
+                if structure is None:
+                    assert self.is_starter_module
+
+                    if self.recognition_domain.domain_name != 'CAL':
+                        if not self.recognition_domain.substrate.starter_monomer:
+                            raise ValueError("Substrate of cis-AT PKS starter module is not a starter substrate")
+                        structure = self.recognition_domain.substrate.starter_monomer.attach_to_acp()
+
+                    else:
+                        starter_unit = read_smiles(
+                            self.recognition_domain.substrate.smiles
+                        )
+                        label_nrp_central_chain(starter_unit)
+                        structure = attach_to_domain_nrp(starter_unit)
+
+                else:
+                    structure = self.synthesis_domain.do_elongation(
+                        structure, self.recognition_domain.substrate
+                    )
+
+                structure = self.do_pks_tailoring(structure)
+            self.add_module_label(structure)
+            return structure
 
 
 class IterativePKSModule(_Module):
-    def __init__(self, nr, domains, starter=False, terminator=False, iterations: int = 1) -> None:
-        super().__init__(nr, "PKS", domains, starter=starter, terminator=terminator, module_subtype="PKS_ITER")
+    def __init__(
+        self, nr, domains, starter=False, terminator=False, iterations: int = 1
+    ) -> None:
+        super().__init__(
+            nr,
+            "PKS",
+            domains,
+            starter=starter,
+            terminator=terminator,
+            module_subtype="PKS_ITER",
+        )
         self.iterations = iterations
 
     def run_module(self, structure=None):
-        self.do_pks_tailoring(structure)
-        raise NotImplementedError
+        if self.is_broken:
+            return structure
+        else:
+            for i in range(0, self.iterations):
+                if self.recognition_domain:
+                    # make new substrate to enable reuse of substrate
+                    substrate = PKSSubstrate(self.recognition_domain.substrate.name)
+                    if structure is None:
+                        assert self.is_starter_module
+                        if not self.recognition_domain.substrate.starter_monomer:
+                            substrate = PKSSubstrate("ACETYL_COA")
+                        structure = substrate.starter_monomer.attach_to_acp()
+
+                    else:
+                        structure = self.synthesis_domain.do_elongation(
+                            structure, substrate
+                        )
+
+                    structure = self.do_pks_tailoring(structure)
+            self.add_module_label(structure)
+            return structure
 
 
 class TransATPKSModule(_Module):
-    def __init__(self, nr, domains, substrate_name="MALONYL_COA", starter=False, terminator=False) -> None:
-        super().__init__(nr, "PKS", domains, starter=starter, terminator=terminator, module_subtype="PKS_TRANS")
+    def __init__(
+        self, nr, domains, substrate_name="MALONYL_COA", starter=False, terminator=False
+    ) -> None:
+        super().__init__(
+            nr,
+            "PKS",
+            domains,
+            starter=starter,
+            terminator=terminator,
+            module_subtype="PKS_TRANS",
+        )
         if not self.recognition_domain:
             self.recognition_domain = RecognitionDomain("DUMMY_AT", substrate_name)
 
     def do_pks_tailoring(self, structure: Structure) -> Structure:
+
         kr_domain = self.get_tailoring_domain("KR")
         if not kr_domain:
             kr_domain = self.get_tailoring_domain("DUMMY_KR")
         dh_domain = self.get_tailoring_domain("DH")
         if not dh_domain:
             dh_domain = self.get_tailoring_domain("DUMMY_DH")
         edh_domain = self.get_tailoring_domain("EDH")
@@ -291,14 +449,17 @@
             er_domain = self.get_tailoring_domain("DUMMY_ER")
         almt_domain = self.get_tailoring_domain("ALMT")
         if not almt_domain:
             almt_domain = self.get_tailoring_domain("DUMMY_ALMT")
         amt_domain = self.get_tailoring_domain("AMT")
         if not amt_domain:
             amt_domain = self.get_tailoring_domain("DUMMY_AMT")
+        emo_domain = self.get_tailoring_domain("EMO")
+        if not amt_domain:
+            emo_domain = self.get_tailoring_domain("DUMMY_EMO")
         sc_domain = self.get_tailoring_domain("SC")
         if not sc_domain:
             sc_domain = self.get_tailoring_domain("DUMMY_SC")
         ah_domain = self.get_tailoring_domain("AH")
         if not ah_domain:
             ah_domain = self.get_tailoring_domain("DUMMY_AH")
         gdh_domain = self.get_tailoring_domain("GDH")
@@ -313,192 +474,180 @@
         omt_domain = self.get_tailoring_domain("OMT")
         if not omt_domain:
             omt_domain = self.get_tailoring_domain("DUMMY_OMT")
         bmt_domain = self.get_tailoring_domain("BMT")
         if not bmt_domain:
             bmt_domain = self.get_tailoring_domain("DUMMY_BMT")
 
+        if ah_domain and ah_domain.active and ah_domain.used:
+            structure, ah_tailored = ah_domain.do_tailoring(structure)
+            if not ah_tailored:
+                ah_domain.used = False
+        if amt_domain and amt_domain.active and amt_domain.used:
+            structure, amt_tailored = amt_domain.do_tailoring(structure)
+            if not amt_tailored:
+                amt_domain.used = False
+            if emo_domain and emo_domain.active and emo_domain.used:
+                structure, emo_tailored = emo_domain.do_tailoring(structure)
+                if not emo_tailored:
+                    emo_domain.used = False
+            structure.refresh_structure()
+        if almt_domain and almt_domain.active and almt_domain.used:
+            structure, almt_tailored = almt_domain.do_tailoring(structure)
+            if not almt_tailored:
+                almt_domain.used = False
+            if emo_domain and emo_domain.active and emo_domain.used:
+                structure, emo_tailored = emo_domain.do_tailoring(structure)
+                if not emo_tailored:
+                    emo_domain.used = False
         if kr_domain and kr_domain.active and kr_domain.used:
             assert kr_domain.subtype is not None
 
             structure, kr_tailored = kr_domain.do_tailoring(structure)
-            if not kr_tailored or kr_domain.subtype.name == 'C1' or kr_domain.subtype.name == 'C2':
+            if (
+                not kr_tailored
+                or kr_domain.subtype.name == "C1"
+                or kr_domain.subtype.name == "C2"
+            ):
                 kr_domain.used = False
                 if omt_domain:
                     omt_domain.used = False
                 if dh_domain:
                     dh_domain.used = False
                 if bmt_domain:
                     bmt_domain.used = False
                 if er_domain:
                     er_domain.used = False
-            if not kr_domain.subtype.name == 'C1' and not kr_domain.subtype.name == 'C2':
+            if (
+                not kr_domain.subtype.name == "C1"
+                and not kr_domain.subtype.name == "C2"
+            ):
+                if bmt_domain and bmt_domain.active and bmt_domain.used:
+                    structure, bmt_tailored = bmt_domain.do_tailoring(structure)
+                    if not bmt_tailored:
+                        bmt_domain.used = False
                 if omt_domain and omt_domain.active and omt_domain.used:
                     structure, omt_tailored = omt_domain.do_tailoring(structure)
                     if not omt_tailored:
                         omt_domain.used = False
                 elif dh_domain and dh_domain.active and dh_domain.used:
                     structure, dh_tailored = dh_domain.do_tailoring(structure)
                     if not dh_tailored:
                         dh_domain.used = False
-                        if bmt_domain:
-                            bmt_domain.used = False
                         if er_domain:
                             er_domain.used = False
                     else:
                         if er_domain and er_domain.active and er_domain.used:
                             structure, er_tailored = er_domain.do_tailoring(structure)
                             if not er_tailored:
                                 er_domain.used = False
-                                if bmt_domain:
-                                    bmt_domain.used = False
-                            else:
-                                if bmt_domain and bmt_domain.active and bmt_domain.used:
-                                    structure, bmt_tailored = bmt_domain.do_tailoring(structure)
-                                    if not bmt_tailored:
-                                        bmt_domain.used = False
                 elif edh_domain and edh_domain.active and edh_domain.used:
                     structure, edh_tailored = edh_domain.do_tailoring(structure)
                     if not edh_tailored:
                         edh_domain.used = False
-                        if bmt_domain:
-                            bmt_domain.used = False
+
                         if er_domain:
                             er_domain.used = False
+
                     else:
                         if er_domain and er_domain.active and er_domain.used:
                             structure, er_tailored = er_domain.do_tailoring(structure)
                             if not er_tailored:
                                 er_domain.used = False
-                                if bmt_domain:
-                                    bmt_domain.used = False
-                            else:
-                                if bmt_domain and bmt_domain.active and bmt_domain.used:
-                                    structure, bmt_tailored = bmt_domain.do_tailoring(structure)
-                                    if not bmt_tailored:
-                                        bmt_domain.used = False
                 elif zdh_domain and zdh_domain.active and zdh_domain.used:
                     structure, zdh_tailored = zdh_domain.do_tailoring(structure)
                     if not zdh_tailored:
                         zdh_domain.used = False
-                        if bmt_domain:
-                            bmt_domain.used = False
                         if er_domain:
                             er_domain.used = False
                     else:
                         if er_domain and er_domain.active and er_domain.used:
                             structure, er_tailored = er_domain.do_tailoring(structure)
                             if not er_tailored:
                                 er_domain.used = False
-                                if bmt_domain:
-                                    bmt_domain.used = False
-                            else:
-                                if bmt_domain and bmt_domain.active and bmt_domain.used:
-                                    structure, bmt_tailored = bmt_domain.do_tailoring(structure)
-                                    if not bmt_tailored:
-                                        bmt_domain.used = False
                 elif gdh_domain and gdh_domain.active and gdh_domain.used:
                     structure, gdh_domain_tailored = gdh_domain.do_tailoring(structure)
                     if not gdh_domain_tailored:
                         gdh_domain.used = False
-                        if bmt_domain:
-                            bmt_domain.used = False
                         if er_domain:
                             er_domain.used = False
                     else:
                         if er_domain and er_domain.active and er_domain.used:
                             structure, er_tailored = er_domain.do_tailoring(structure)
                             if not er_tailored:
                                 er_domain.used = False
-                                if bmt_domain:
-                                    bmt_domain.used = False
-                            else:
-                                if bmt_domain and bmt_domain.active and bmt_domain.used:
-                                    structure, bmt_tailored = bmt_domain.do_tailoring(structure)
-                                    if not bmt_tailored:
-                                        bmt_domain.used = False
                 elif egdh_domain and egdh_domain.active and egdh_domain.used:
-                    structure, egdh_domain_tailored = egdh_domain.do_tailoring(structure)
+                    structure, egdh_domain_tailored = egdh_domain.do_tailoring(
+                        structure
+                    )
                     if not egdh_domain_tailored:
                         egdh_domain.used = False
-                        if bmt_domain:
-                            bmt_domain.used = False
                         if er_domain:
                             er_domain.used = False
                     else:
                         if er_domain and er_domain.active and er_domain.used:
                             structure, er_tailored = er_domain.do_tailoring(structure)
                             if not er_tailored:
                                 er_domain.used = False
-                                if bmt_domain:
-                                    bmt_domain.used = False
-                            else:
-                                if bmt_domain and bmt_domain.active and bmt_domain.used:
-                                    structure, bmt_tailored = bmt_domain.do_tailoring(structure)
-                                    if not bmt_tailored:
-                                        bmt_domain.used = False
                 elif zgdh_domain and zgdh_domain.active and zgdh_domain.used:
-                    structure, zgdh_domain_tailored = zgdh_domain.do_tailoring(structure)
+                    structure, zgdh_domain_tailored = zgdh_domain.do_tailoring(
+                        structure
+                    )
                     if not zgdh_domain_tailored:
                         zgdh_domain.used = False
-                        if bmt_domain:
-                            bmt_domain.used = False
                         if er_domain:
                             er_domain.used = False
                     else:
                         if er_domain and er_domain.active and er_domain.used:
                             structure, er_tailored = er_domain.do_tailoring(structure)
                             if not er_tailored:
                                 er_domain.used = False
-                                if bmt_domain:
-                                    bmt_domain.used = False
-                            else:
-                                if bmt_domain and bmt_domain.active and bmt_domain.used:
-                                    structure, bmt_tailored = bmt_domain.do_tailoring(structure)
-                                    if not bmt_tailored:
-                                        bmt_domain.used = False
-        if amt_domain and amt_domain.active and amt_domain.used:
-            structure, amt_tailored = amt_domain.do_tailoring(structure)
-            if not amt_tailored:
-                amt_domain.used = False
-        if almt_domain and almt_domain.active and almt_domain.used:
-            structure, almt_tailored = almt_domain.do_tailoring(structure)
-            if not almt_tailored:
-                almt_domain.used = False
         if sc_domain and sc_domain.active and sc_domain.used:
             structure, sc_tailored = sc_domain.do_tailoring(structure)
             if not sc_tailored:
                 sc_domain.used = False
-        if ah_domain and ah_domain.active and ah_domain.used:
-            structure, ah_tailored = ah_domain.do_tailoring(structure)
-            if not ah_tailored:
-                ah_domain.used = False
+
+        structure.refresh_structure()
         return structure
 
     def run_module(self, structure: Union[Structure, None] = None) -> Structure:
-        if structure is None:
-            assert self.is_starter_module
-            starter_unit = read_smiles(self.recognition_domain.substrate.smiles)
-            label_pk_central_chain(starter_unit)
-            structure = attach_to_domain_pk(starter_unit)
+        if self.is_broken:
+            return structure
         else:
-            structure = self.synthesis_domain.do_elongation(structure, self.recognition_domain.substrate)
-        structure = self.do_pks_tailoring(structure)
-        return structure
+            if self.recognition_domain:
+                if structure is None:
+                    assert self.is_starter_module
+                    structure = (
+                        self.recognition_domain.substrate.starter_monomer.attach_to_acp()
+                    )
+                else:
+                    structure = self.synthesis_domain.do_elongation(
+                        structure, self.recognition_domain.substrate
+                    )
+                structure = self.do_pks_tailoring(structure)
+            self.add_module_label(structure)
+            return structure
 
 
 class NRPSModule(_Module):
 
     def __init__(self, nr, domains, starter=False, terminator=False):
         super().__init__(nr, "NRPS", domains, starter=starter, terminator=terminator)
 
     def run_module(self, structure=None) -> Structure:
-        if structure is None:
-            assert self.is_starter_module
-            starter_unit = read_smiles(self.recognition_domain.substrate.smiles)
-            label_nrp_central_chain(starter_unit)
-            structure = attach_to_domain_nrp(starter_unit)
+        if self.is_broken:
+            return structure
         else:
-            structure = self.synthesis_domain.do_elongation(structure, self.recognition_domain.substrate)
-
-        structure = self.do_nrps_tailoring(structure)
-        return structure
+            if self.recognition_domain:
+                if structure is None:
+                    assert self.is_starter_module
+                    starter_unit = read_smiles(self.recognition_domain.substrate.smiles)
+                    label_nrp_central_chain(starter_unit)
+                    structure = attach_to_domain_nrp(starter_unit)
+                else:
+                    structure = self.synthesis_domain.do_elongation(
+                        structure, self.recognition_domain.substrate
+                    )
+
+                structure = self.do_nrps_tailoring(structure)
+            self.add_module_label(structure)
+            return structure
```

### Comparing `raichu-0.0.2/raichu/reactions/chain_release.py` & `raichu-1.0.0/raichu/reactions/chain_release.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 
 from pikachu.chem.structure import Structure
 from pikachu.reactions.functional_groups import find_bonds, find_atoms
 from pikachu.reactions.basic_reactions import hydrolysis, internal_condensation
 from pikachu.general import structure_to_smiles
 
-from raichu.data.molecular_moieties import SC_BOND, O_OH, O_BETAPROPRIOLACTONE_O,\
-    O_BETAPROPRIOLACTONE_TERMINAL_O
+from raichu.data.molecular_moieties import SC_BOND, SC_BOND_MINIMAL, O_OH, O_BETAPROPRIOLACTONE_O,\
+    O_BETAPROPRIOLACTONE_TERMINAL_O, O_BETAPROPRIOLACTONE_KETO_OH, O_BETAPROPRIOLACTONE_KETO_C
 from raichu.reactions.general import initialise_atom_attributes
 from raichu.drawing.drawer import RaichuDrawer
 
 
 def release_linear_reduction(chain_intermediate: Structure) -> Structure:
     sc_bonds = find_bonds(SC_BOND, chain_intermediate)
+    if not sc_bonds:
+        sc_bonds = find_bonds(SC_BOND_MINIMAL, chain_intermediate)
     if len(sc_bonds) != 1:
         raise ValueError("Cannot release product from carrier domain as no SC bond is present")
 
     sc_bond = sc_bonds[0]
 
     carbon = sc_bond.get_neighbour('C')
     sulphur = sc_bond.get_neighbour('S')
@@ -24,14 +26,17 @@
     chain_intermediate.break_bond(sc_bond)
 
     chain_intermediate.add_atom('H', [carbon])
     chain_intermediate.add_atom('H', [sulphur])
 
     initialise_atom_attributes(chain_intermediate)
 
+    carbon = chain_intermediate.get_atom(carbon)
+    carbon.annotations.set_annotation('terminal_c', True)
+
     structures = chain_intermediate.split_disconnected_structures()
     for structure in structures:
         if carbon in structure.graph:
             structure.refresh_structure()
             return structure
 
     raise RuntimeError("Could not release chain through reduction.")
@@ -43,14 +48,17 @@
     PIKAChU Structure object
 
     chain_intermediate: PIKAChU Structure object of the polyketide chain
     intermediate, either attached to a PKS domain or not
     """
     # Find S-H bond in chain intermediate and break the bond and define atoms
     sc_bonds = find_bonds(SC_BOND, chain_intermediate)
+    if not sc_bonds:
+        sc_bonds = find_bonds(SC_BOND_MINIMAL, chain_intermediate)
+
     assert len(sc_bonds) == 1
     carbon = sc_bonds[0].get_neighbour('C')
 
     linear_product = None
 
     structures = hydrolysis(chain_intermediate, sc_bonds[0])
     for structure in structures:
@@ -72,14 +80,15 @@
         if oxygen.has_neighbour('H'):
             terminal_oxygen = oxygen
             break
 
     assert terminal_oxygen
 
     terminal_oxygen.annotations.set_annotation('terminal_o', True)
+    linear_product.refresh_structure()
 
     return linear_product
 
 
 def cyclic_release(linear_product, o_oh_n_amino):
     """Performs the thioesterase reactions on the input chain_intermediate
      using the -OH group defined by the input O-atom participating in that
@@ -112,43 +121,59 @@
     oh_bond = terminal_oxygen.get_bond(terminal_carbon)
 
     cyclic_product, water = internal_condensation(linear_product, oh_bond, h_bond)
 
     return cyclic_product
 
 
-def find_o_betapropriolactone(polyketide):
+def find_o_betapropriolactone(polyketide, release_type='condensative'):
     """
     Finds and returns the oxygen atom (PIKAChU atom object) in the -OH group
     that shouldn't be used by the thioesterase_circular_product function, as
     this will create a beta-propriolactone compound, which does not occur in
     polyketide synthesis, if present. Otherwise the function returns None
 
     polyketide: PIKAChU structure object of a polyketide
     """
-    o_propriolactone = find_atoms(O_BETAPROPRIOLACTONE_O, polyketide)
-    o_propriolactone_terminal = find_atoms(O_BETAPROPRIOLACTONE_TERMINAL_O, polyketide)
-
-    assert len(o_propriolactone) == len(o_propriolactone_terminal)
+    if release_type == 'condensative':
+        o_propriolactone = find_atoms(O_BETAPROPRIOLACTONE_O, polyketide)
+        o_propriolactone_terminal = find_atoms(O_BETAPROPRIOLACTONE_TERMINAL_O, polyketide)
+
+        assert len(o_propriolactone) == len(o_propriolactone_terminal)
+
+        o_beta_propriolactones = []
+
+        for i, atom in enumerate(o_propriolactone):
+            terminal_o = o_propriolactone_terminal[i]
+            if terminal_o.annotations.terminal_o:
+                o_beta_propriolactones.append(atom)
+
+        if len(o_beta_propriolactones) == 0:
+            return None
+        elif len(o_beta_propriolactones) == 1:
+            return o_beta_propriolactones[0]
+        else:
+            raise ValueError('Error: this molecule is not a polyketide, as the \
+            carbon in the beta ketone/hydroxyl group is bound to an additional \
+             oxygen atom')
+
+    elif release_type == 'oxidative':
+        # assumes structure search is deterministic
+
+        o_propriolactones = find_atoms(O_BETAPROPRIOLACTONE_KETO_OH, polyketide)
+        o_propriolactones_terminal = find_atoms(O_BETAPROPRIOLACTONE_KETO_C, polyketide)
+
+        assert len(o_propriolactones_terminal) == len(o_propriolactones)
+
+        for i, oh in enumerate(o_propriolactones):
+            terminal_c = o_propriolactones_terminal[i]
+            if getattr(terminal_c.annotations, "terminal_c"):
+                return oh
 
-    o_beta_propriolactones = []
-
-    for i, atom in enumerate(o_propriolactone):
-        terminal_o = o_propriolactone_terminal[i]
-        if terminal_o.annotations.terminal_o:
-            o_beta_propriolactones.append(atom)
-
-    if len(o_beta_propriolactones) == 0:
         return None
-    elif len(o_beta_propriolactones) == 1:
-        return o_beta_propriolactones[0]
-    else:
-        raise ValueError('Error: this molecule is not a polyketide, as the \
-        carbon in the beta ketone/hydroxyl group is bound to an additional \
-         oxygen atom')
 
 
 def thioesterase_all_products(chain_intermediate, out_folder=None):
     """Performs all thioesterase reactions on the input chain_intermediate
      using all internal amino and -OH groups except for the -OH group that
      leads to the formation of a beta-propriolactone compound, which does not
      occur in polyketide synthesis. Returns a list of PIKAChU Structure objects
@@ -179,15 +204,15 @@
         if atom.type == 'N':
             if len(atom.get_neighbours('H')) == 2 and atom.has_neighbour('C') and not atom.aromatic and atom \
                     not in amino_n_atoms_filtered:
                 amino_n_atoms_filtered.append(atom)
 
     # Define -OH group that should not be used to carry out the thioesterase
     # reaction (distance -S and internal -OH group)
-    o_not_to_use = find_o_betapropriolactone(linear_product)
+    # o_not_to_use = find_o_betapropriolactone(linear_product)
 
     list_product_drawings = []
     circular_smiles = []
 
     # Perform all possible thioesterase reactions leading to the formation of
     # circular products using the internal amino groups, save Structure objects
     # to list
@@ -245,7 +270,46 @@
     else:
 
         # Draw all products
         for product in list_product_drawings:
             RaichuDrawer(product)
 
     return list_product_drawings
+
+
+def find_all_o_n_atoms_for_cyclization(chain_intermediate):
+    """Performs all thioesterase reactions on the input chain_intermediate
+     using all internal amino and -OH groups except for the -OH group that
+     leads to the formation of a beta-propriolactone compound, which does not
+     occur in polyketide synthesis. Returns a list of PIKAChU Structure objects
+     of all possible thioesterase products.
+
+     chain_intermediate: PIKAChU Structure object of a polyketide/NRP
+    """
+    # Perform first thioesterase reaction, generating linear polyketide/NRP
+    chain_intermediate.refresh_structure()
+    for atom in chain_intermediate.graph:
+        atom.hybridise()
+    chain_intermediate_copy = chain_intermediate.deepcopy()
+    # Find OH groups in polyketide/NRP, perform cyclization for each -OH group
+    chain_intermediate_copy.refresh_structure()
+    o_oh_atoms = find_atoms(O_OH, chain_intermediate_copy)
+    o_oh_atoms_filtered = []
+    for atom in o_oh_atoms:
+        if atom not in o_oh_atoms_filtered and any(neighbour.type == 'H' for neighbour in atom.neighbours):
+            o_oh_atoms_filtered.append(atom)
+
+    # Find amino gruops in polyketide/NRP, perform cyclization for each group
+    chain_intermediate_copy = chain_intermediate.deepcopy()
+    chain_intermediate_copy.refresh_structure()
+    chain_intermediate.set_connectivities()
+    chain_intermediate.set_atom_neighbours()
+    amino_n_atoms_filtered = []
+    for atom in chain_intermediate_copy.graph:
+        if atom.type == 'N':
+            n_neighbour_types = []
+            for neighbour in atom.neighbours:
+                n_neighbour_types.append(neighbour.type)
+            if atom not in amino_n_atoms_filtered and n_neighbour_types.count('H') == 2 and n_neighbour_types.count('C') == 1:
+                amino_n_atoms_filtered.append(atom)
+
+    return o_oh_atoms_filtered + amino_n_atoms_filtered
```

### Comparing `raichu-0.0.2/raichu/reactions/general.py` & `raichu-1.0.0/raichu/reactions/general.py`

 * *Files identical despite different names*

### Comparing `raichu-0.0.2/raichu/reactions/nrps_elongation_reactions.py` & `raichu-1.0.0/raichu/reactions/nrps_elongation_reactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pikachu.reactions.basic_reactions import condensation, hydrolysis
 from pikachu.reactions.functional_groups import find_bonds, find_atoms
-from raichu.class_domain import ATTRIBUTES
+from raichu.data.attributes import ATTRIBUTES
 from raichu.central_chain_detection.label_central_chain import label_nrp_central_chain
-from raichu.data.molecular_moieties import THIOESTERBOND, THIOESTER_CARBON, N_AMINO_ACID, B_N_AMINO_ACID
+from raichu.data.molecular_moieties import THIOESTERBOND, THIOESTER_CARBON, N_AMINO_ACID, B_N_AMINO_ACID, \
+    THIOESTERBOND_OXYGEN_INSERTED, THIOESTER_CARBON_OXYGEN_INSERTED
 from raichu.reactions.general import label_rest_groups, initialise_atom_attributes, reset_nrp_annotations
 from raichu.attach_to_domain import attach_to_domain_nrp
 
 
 def nrps_elongation(amino_acid, chain_intermediate):
     """
     Returns the NRPS condensation product as a PIKAChU Structure object
@@ -73,14 +74,18 @@
 
     thioester_structure: PIKAChU Structure object of a thioester (R-C(S)=O)
     """
     # Find thioester bond in the input structure
     found_bonds_thioester = find_bonds(THIOESTERBOND, thioester_structure)
     found_carbon_thioester = find_atoms(THIOESTER_CARBON, thioester_structure)
 
+    if len(found_bonds_thioester) == 0:
+        found_bonds_thioester = find_bonds(THIOESTERBOND_OXYGEN_INSERTED, thioester_structure)
+        found_carbon_thioester = find_atoms(THIOESTER_CARBON_OXYGEN_INSERTED, thioester_structure)
+
     assert len(found_carbon_thioester) == 1
     assert len(found_bonds_thioester) == 1
 
     carbon_thioester = found_carbon_thioester[0]
     sh_bond = found_bonds_thioester[0]
 
     structures = hydrolysis(thioester_structure, sh_bond)
@@ -101,13 +106,14 @@
             oxygen_hydroxyl = oxygen
             break
 
     assert oxygen_hydroxyl
 
     oh_bond = combined.bond_lookup[oxygen_hydroxyl][carbon_thioester]
 
+    # TODO: Target unlabelled atom
     for atom in combined.graph:
         if not hasattr(atom.annotations, 'in_central_chain'):
             for attribute in ATTRIBUTES:
                 atom.annotations.add_annotation(attribute, False)
 
     return combined, oh_bond
```

### Comparing `raichu-0.0.2/raichu/reactions/pks_elongation_reactions.py` & `raichu-1.0.0/raichu/reactions/pks_elongation_reactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pikachu.reactions.functional_groups import combine_structures
-from pikachu.general import draw_structure
-from raichu.data.molecular_moieties import THIOESTERBOND
+from raichu.data.molecular_moieties import THIOESTERBOND, THIOESTERBOND_OXYGEN_INSERTED
 from raichu.reactions.general import label_rest_groups
+from raichu.reactions.pks_sidechain_chirality import set_sidechain_chirality
 
 
 def pks_elongation(chain_intermediate, elongation_monomer):
     """
     Returns a Structure object of the PK chain after a single elongation step
     elongation step.
 
@@ -34,14 +34,16 @@
     assert h_to_remove_1 and h_to_remove_2
 
     # If the elongation unit contains a wildcard, add a number to the
     # '*' atom to display in the structure drawing
     label_rest_groups(elongation_monomer.structure, chain_intermediate)
 
     thioester_bonds = find_bonds(chain_intermediate, THIOESTERBOND)
+    if len(thioester_bonds) == 0:
+        thioester_bonds = find_bonds(chain_intermediate, THIOESTERBOND_OXYGEN_INSERTED)
 
     assert len(thioester_bonds) == 1
     for bond in thioester_bonds:
         if bond.atom_1.type == 'S':
             s_pkchain = bond.atom_1
             c_pkchain = bond.atom_2
         elif bond.atom_2.type == 'S':
@@ -57,14 +59,15 @@
     # Find thioester bond in growing chain, define Cs to attach new unit
 
     # Breaking the thioester bond in the PK chain
     for atom in chain_intermediate.graph:
         atom.hybridise()
     for bond in thioester_bonds[:]:
         chain_intermediate.break_bond(bond)
+
     chain_intermediate.get_connectivities()
     chain_intermediate.set_connectivities()
     chain_intermediate.set_atom_neighbours()
     chain_intermediate.make_bond_lookup()
 
     # Refresh malonylunit
 
@@ -80,25 +83,28 @@
     combined.set_atom_neighbours()
     combined.make_bond_lookup()
 
     # Adding the bonds to form the new molecule after the single elongation step
     new_bond_nr = combined.find_next_bond_nr()
     combined.make_bond(elongation_monomer.c_to_pk_intermediate, c_pkchain, new_bond_nr)
     new_bond_nr = combined.find_next_bond_nr()
+
     combined.make_bond(elongation_monomer.c_to_s, s_pkchain, new_bond_nr)
     combined.get_connectivities()
     combined.set_connectivities()
     combined.set_atom_neighbours()
     combined.make_bond_lookup()
     for bond_nr, bond in combined.bonds.items():
         bond.set_bond_summary()
 
     for atom in combined.graph:
         atom.annotations.c2_acid = False
 
+    set_sidechain_chirality(combined)
+
     return combined
 
 
 def find_bonds(structure, bond_type):
     """
     Returns a list of Pikachu.bond objects of the bonds of the indicated type
     in the structure of interest
```

### Comparing `raichu-0.0.2/raichu/reactions/pks_tailoring_reactions.py` & `raichu-1.0.0/raichu/reactions/pks_tailoring_reactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from pikachu.reactions.functional_groups import BondDefiner, GroupDefiner, find_atoms, find_bonds, combine_structures
 from pikachu.reactions.basic_reactions import internal_condensation
 from pikachu.chem.chirality import same_chirality
 from pikachu.chem.structure import Structure
 from raichu.domain.domain_types import KRDomainSubtype, ERDomainSubtype
 from raichu.reactions.general import initialise_atom_attributes
+from raichu.reactions.pks_sidechain_chirality import set_sidechain_chirality
+from raichu.reactions.general_tailoring_reactions import single_bond_oxidation
 from pikachu.general import read_smiles
 from raichu.data.attributes import ATTRIBUTES
 
 FIRST_C = GroupDefiner('first_c', r'CC(S)=O', 1)
 RECENT_ALPHA_C = GroupDefiner('recent_alpha_c', r'CCC(S)=O', 1)
 RECENT_BETA_C = GroupDefiner('recent_beta_c', r'CCC(S)=O', 0)
 RECENT_BETA_C_OH = GroupDefiner('recent_beta_c_oh', r'OCCC(S)=O', 0)
@@ -23,64 +25,70 @@
 RECENT_REDUCTION_CC_SHIFTED = BondDefiner('recent_reduction_C-C_shifted', r'CC(O)CC(S)=O', 0, 1)
 RECENT_DEHYDRATION = BondDefiner('recent_dehydration', r'SC(C=CC)=O', 2, 3)
 RECENT_EONYL_REDUCTION = BondDefiner('recent_eonyl_reduction', r"CCCC(S)=O", 2, 3)
 RECENT_EONYL_REDUCTION_CC = BondDefiner('recent_eonyl_reduction', r"CCCC(S)=O", 2, 1)
 RECENT_REDUCTION_OH = BondDefiner('recent_reduction_C-H', r'[H]OC(C)CC(S)=O', 0, 1)
 RECENT_REDUCTION_TOP_C = GroupDefiner('recent_reduction_top_c', r'[H]C(C)=C([H])C(S)=O', 5)
 RECENT_REDUCTION_TOP_H = GroupDefiner('recent_reduction_top_h', r'[H]C(C)=C([H])C(S)=O', 4)
-RECENT_REDUCTION_TOP_METHYL = GroupDefiner('recent_reduction_top_methyl', r'[H]\C(C)=C(\C)C(S)=O', 4)
+# RECENT_REDUCTION_TOP_METHYL = GroupDefiner('recent_reduction_top_methyl', r'[H]\C(C)=C(\C)C(S)=O', 4)
+RECENT_REDUCTION_TOP_METHYL = GroupDefiner('recent_reduction_top_methyl', r'[H]C(C)=C(C)C(S)=O', 4)
+RECENT_REDUCTION_TOP_METHOXY = GroupDefiner(
+    'recent_reduction_top_methoxy', r'[H]C(C)=C(OC)C(S)=O', 4)
 RECENT_REDUCTION_BOTTOM_C = GroupDefiner('recent_reduction_bottom_c', r'[H]C(C)=C([H])C(S)=O', 2)
 RECENT_REDUCTION_BOTTOM_H = GroupDefiner('recent_reduction_bottom_h', r'[H]C(C)=C([H])C(S)=O', 0)
+
 RECENT_REDUCTION_SHIFTED_TOP_C = GroupDefiner('recent_reduction_shifted_top_c', r'[H]\C(C)=C(\[H])CC(S)=O', 5)
 RECENT_REDUCTION_SHIFTED_TOP_H = GroupDefiner('recent_reduction_shifted_top_h', r'[H]\C(C)=C(\[H])CC(S)=O', 4)
 RECENT_REDUCTION_SHIFTED_BOTTOM_C = GroupDefiner('recent_reduction_shifted_bottom_c', r'[H]\C(C)=C(\[H])CC(S)=O', 2)
 RECENT_REDUCTION_SHIFTED_BOTTOM_H = GroupDefiner('recent_reduction_shifted_bottom_h', r'[H]\C(C)=C(\[H])CC(S)=O', 0)
 RECENT_REDUCTION_SHIFTED_BOTTOM_METHYL = GroupDefiner('recent_reduction_shifted_bottom_methyl',
                                                       r'[H]\C(CC(S)=O)=C(\C)CC', 7)
 S_KR = GroupDefiner('C1 atom before KR reaction', r'SC(C)=O', 0)
 ER_MMAL_CARBON = GroupDefiner('Chiral carbon atom after enoylreduction of mmal', r'SC(=O)C(C)CC', 3)
 ER_S_CARBON = GroupDefiner('S-carbon atom after enoylreduction of mmal', r'SC(=O)C(C)CC', 1)
 HYDROXYL_GROUP_TWO_MODULES_UPSTREAM_ALPHA_WITH_DOUBLE_BOND = BondDefiner("hydroxyl_group_two_module_upstream_alpha_with_double_bond",
-                                                                         r"OC\C=C\CCC(S)=O", 0, 1)
+                                                                         r"[H]OC\C=C\CCC(S)=O", 1, 2)
 HYDROXYL_GROUP_TWO_MODULES_UPSTREAM_BETA_WITH_DOUBLE_BOND = BondDefiner("hydroxyl_group_two_module_upstream_beta_with_double_bond",
-                                                                        r"OCC\C=C\CCC(S)=O", 0, 1)
+                                                                        r"[H]OCC\C=C\CCC(S)=O", 1, 2)
 HYDROXYL_GROUP_TWO_MODULES_UPSTREAM_ALPHA_WITH_DOUBLE_BOND_SHIFTED = BondDefiner("hydroxyl_group_two_module_upstream_alpha_with_double_bond_shifted",
-                                                                                 r"O\C=C\CCCC(S)=O", 0, 1)
+                                                                                 r"[H]O\C=C\CCCC(S)=O", 1, 2)
 HYDROXYL_GROUP_TWO_MODULES_UPSTREAM_BETA_WITH_DOUBLE_BOND_SHIFTED = BondDefiner("hydroxyl_group_two_module_upstream_beta_with_double_bond_shifted",
-                                                                                r"OC\C=C\CCCC(S)=O", 0, 1)
+                                                                                r"[H]OC\C=C\CCCC(S)=O", 1, 2)
 HYDROXYL_GROUP_TWO_MODULES_UPSTREAM_ALPHA = BondDefiner("hydroxyl_group_two_module_upstream_alpha",
-                                                        "OCCCCCC(S)=O", 0, 1)
+                                                        "[H]OCCCCCC(S)=O", 1, 2)
 HYDROXYL_GROUP_TWO_MODULES_UPSTREAM_BETA = BondDefiner("hydroxyl_group_two_module_upstream_beta",
-                                                       "OCCCCCCC(S)=O", 0, 1)
-
+                                                       "[H]OCCCCCCC(S)=O", 1, 2)
 
 # STILL MISSING: E/Z-configured double bonds, E/Z-Gamma-beta-dehydrogenase
 
+
 def ketoreduction(chain_intermediate: Structure, kr_type: KRDomainSubtype) -> Tuple[Structure, bool]:
     """
     Performs the ketoreductase reaction on the PKS chain intermediate, returns
     the reaction product as a PIKAChU Structure object
 
     chain_intermediate: PIKAChU Structure object, PKS chain intermediate just
     after a PKS elongation step
     """
 
     if kr_type.name == 'C1':
+        set_sidechain_chirality(chain_intermediate)
         return chain_intermediate, False
 
     chiral_c = None
 
     # Find chiral carbon atom
     chiral_c_locations = find_atoms(RECENT_REDUCTION_MMAL_CHIRAL_C, chain_intermediate)
 
     # Identify beta-ketone bond, identify O- and C-atom participating in bond
 
     beta_ketone_bonds = find_bonds(RECENT_ELONGATION, chain_intermediate)
 
     if not len(beta_ketone_bonds) == 1:
+        set_sidechain_chirality(chain_intermediate)
         return chain_intermediate, False
 
     beta_ketone_bond = beta_ketone_bonds[0]
 
     carbonyl_oxygen = beta_ketone_bond.get_neighbour('O')
     carbonyl_carbon = beta_ketone_bond.get_neighbour('C')
 
@@ -149,15 +157,15 @@
     # See if the previous elongation step was performed using methylmalonyl-CoA,
     # perform epimerization if required
 
     if chiral_c_locations:
 
         chiral_c = chiral_c_locations[0]
 
-    if chiral_c:
+    if chiral_c and kr_type.name != "UNKNOWN":
         sulphur_locations = find_atoms(S_KR, chain_intermediate)
         assert len(sulphur_locations) == 1
         sulphur = sulphur_locations[0]
         assert sulphur
 
         c_1 = None
         for neighbour in sulphur.neighbours:
@@ -197,46 +205,51 @@
                 chiral_c.chiral = 'counterclockwise'
             else:
                 chiral_c.chiral = 'clockwise'
         elif kr_type.name == "UNKNOWN":
             chiral_c.chiral = None
         else:
             raise ValueError(f'KR domain of type {kr_type.name} is not supported by RAIChU or does not exist')
+    elif kr_type.name == "UNKNOWN" and chiral_c:
+        chiral_c.chiral = None
 
     chain_intermediate.refresh_structure()
     return chain_intermediate, True
 
 
 def dehydration(chain_intermediate: Structure, chirality=None) -> Tuple[Structure, bool]:
     """
     Performs the dehydratase reaction on the PKS chain intermediate, returns
     the reaction product as a PIKAChU Structure object
 
     chain_intermediate: PIKAChU Structure object, PKS chain intermediate where
     the beta ketone group has been recently reduced by the KR domain
     """
-
     # Find and define the atoms that participate in the bond changes
     co_bonds = find_bonds(RECENT_REDUCTION_COH, chain_intermediate)
     cc_bonds = find_bonds(RECENT_REDUCTION_CC, chain_intermediate)
 
+    # check if H attached to O
+    hydrogen = None
     if not len(co_bonds) == 1 or not len(cc_bonds) == 1:
         return chain_intermediate, False
 
     c1 = None
     c2 = None
     o_oh = None
 
     co_bond = co_bonds[0]
 
     for neighbour in co_bond.neighbours:
         if neighbour.type == 'C':
             c2 = neighbour
         elif neighbour.type == 'O':
             o_oh = neighbour
+            if "H" not in [atom.type for atom in neighbour.neighbours]:
+                return chain_intermediate, False
 
     cc_bond = cc_bonds[0]
 
     for neighbour in cc_bond.neighbours:
         if neighbour != c2:
             c1 = neighbour
 
@@ -278,22 +291,40 @@
     else:
         chain_intermediate = structure_2
 
     chain_intermediate.refresh_structure()
     double_bond = chain_intermediate.bond_lookup[c1][c2]
     # implement stereochemistry
     if chirality:
-        main_chain_top_c = find_atoms(RECENT_REDUCTION_TOP_C, chain_intermediate)[0]
-        main_chain_bottom_c = find_atoms(RECENT_REDUCTION_BOTTOM_C, chain_intermediate)[0]
+        main_chain_top_c = chain_intermediate.get_atom(find_atoms(RECENT_REDUCTION_TOP_C, chain_intermediate)[0])
+        main_chain_bottom_c = chain_intermediate.get_atom(find_atoms(RECENT_REDUCTION_BOTTOM_C, chain_intermediate)[0])
         main_chain_top_h = find_atoms(RECENT_REDUCTION_TOP_H, chain_intermediate)
+        main_chain_bottom_h = find_atoms(RECENT_REDUCTION_BOTTOM_H, chain_intermediate)
+
         if not main_chain_top_h:
-            main_chain_top_h = find_atoms(RECENT_REDUCTION_TOP_METHYL, chain_intermediate)[0]
+            main_chain_top_h = [neighbour for neighbour in c1.neighbours if not neighbour.annotations.in_central_chain]
+        #     print(main_chain_top_h)
+        #     main_chain_top_h = find_atoms(RECENT_REDUCTION_TOP_METHYL, chain_intermediate)
+        #
+        #     if not main_chain_top_h:
+        #         main_chain_top_h = find_atoms(RECENT_REDUCTION_TOP_METHOXY, chain_intermediate)
+        # assert main_chain_top_h
+
+        main_chain_top_h = chain_intermediate.get_atom(main_chain_top_h[0])
+
+        if not main_chain_bottom_h:
+
+            main_chain_bottom_h = chain_intermediate.get_atom([neighbour for neighbour in c2.neighbours if not neighbour.annotations.in_central_chain][0])
         else:
-            main_chain_top_h = main_chain_top_h[0]
-        main_chain_bottom_h = find_atoms(RECENT_REDUCTION_BOTTOM_H, chain_intermediate)[0]
+            main_chain_bottom_h = chain_intermediate.get_atom(main_chain_bottom_h[0])
+        
+        # If not all can be found, don't do stereochemistry (sometimes true for cyclic substrates before)
+        if not main_chain_top_h or not main_chain_bottom_h or not main_chain_top_c or not main_chain_bottom_c:
+            return chain_intermediate, True
+        
         if chirality == "E":
             double_bond.chiral_dict = {main_chain_top_c: {main_chain_bottom_c: 'trans',
                                                           main_chain_bottom_h: 'cis'},
                                        main_chain_top_h: {main_chain_bottom_c: 'cis',
                                                           main_chain_bottom_h: 'trans'},
                                        main_chain_bottom_c: {main_chain_top_c: 'trans',
                                                              main_chain_top_h: 'cis'},
@@ -305,14 +336,15 @@
                                        main_chain_top_h: {main_chain_bottom_c: 'trans',
                                                           main_chain_bottom_h: 'cis'},
                                        main_chain_bottom_c: {main_chain_top_c: 'cis',
                                                              main_chain_top_h: 'trans'},
                                        main_chain_bottom_h: {main_chain_top_c: 'trans',
                                                              main_chain_top_h: 'cis'}}
         double_bond.chiral = True
+
     chain_intermediate.refresh_structure()
 
     return chain_intermediate, True
 
 
 def enoylreduction(chain_intermediate: Structure, er_subtype: ERDomainSubtype) -> Tuple[Structure, bool]:
     """
@@ -395,15 +427,15 @@
     bond_1 = oxygen.get_bond(hydrogen_1)
     hydrogen_2 = target_atom.get_neighbour('H')
     if not hydrogen_2:
         raise Exception("Can't oxidate this atom!")
 
     bond_2 = target_atom.get_bond(hydrogen_2)
 
-    hydroxylated_structure = combine_structures([structure, hydroxyl_group])
+    hydroxylated_structure = combine_structures([hydroxyl_group, structure])
 
     hydroxylated_structure.break_bond(bond_1)
     hydroxylated_structure.break_bond(bond_2)
 
     hydroxylated_structure.make_bond(oxygen, target_atom, hydroxylated_structure.find_next_bond_nr())
     hydroxylated_structure.make_bond(hydrogen_1, hydrogen_2, hydroxylated_structure.find_next_bond_nr())
 
@@ -430,15 +462,15 @@
 
     hydrogen_2 = target_atom.get_neighbour('H')
     if not hydrogen_2:
         raise Exception("Can't methylate this atom!")
 
     bond_2 = target_atom.get_bond(hydrogen_2)
 
-    methylated_structure = combine_structures([structure, methyl_group])
+    methylated_structure = combine_structures([ methyl_group, structure])
 
     methylated_structure.break_bond(bond_1)
     methylated_structure.break_bond(bond_2)
 
     methylated_structure.make_bond(carbon, target_atom, methylated_structure.find_next_bond_nr())
     methylated_structure.make_bond(hydrogen_1, hydrogen_2, methylated_structure.find_next_bond_nr())
 
@@ -467,33 +499,50 @@
 def smallest_cyclisation(structure: Structure) -> Tuple[Structure, bool]:
     """
     Cyclises with the OH group two modules upstream to the smalles possible ring
 
     structure: PIKAChU Structure object
     """
     # reduce Ketogroup first
+
     structure_oh, did_reduction = ketoreduction(structure, KRDomainSubtype(1))
     if not did_reduction:
         return structure, False
-
     oh_bond = find_OH_two_modules_upstream(structure_oh)
+    oxygen = None
+
     if not oh_bond:
-        print("No hydroxy group two modules upstream availiable")
+        # TODO: Add print statement to verbose mode
+        # print("No hydroxy-group available two modules upstream")
         return structure, False
 
     oh_bond = oh_bond[0]
+    for atom in oh_bond.neighbours:
+        if atom.type == 'O' and atom.has_neighbour('H'):
+            oxygen = atom
+    if not oxygen:
+        # TODO: Add print statement to verbose mode
+        # print("No hydroxy group available two modules upstream")
+        return structure, False
+    else:
+        carbon = oxygen.get_neighbour('C')
+        if carbon.in_ring(structure_oh):
+            # TODO: Add print statement to verbose mode
+            # print("No hydroxy group available two modules upstream")
+            return structure, False
+    
     h_bond = find_bonds(RECENT_REDUCTION_OH, structure_oh)[0]
-    structure_oh = internal_condensation(structure_oh, oh_bond, h_bond)[0]
+    structure_ohh = internal_condensation(structure_oh, oh_bond, h_bond)[0]
 
-    return structure_oh, True
+    return structure_ohh, True
 
 
 def alpha_methyl_transferase(structure: Structure) -> Tuple[Structure, bool]:
     """
-    Returns the structure thats methylated at the alpha-c.
+    Returns the structure that is methylated at the alpha-c.
 
     structure: PIKAChU Structure object
     target_atom:  PIKAChU atom object
     """
     # find atom to add methylgroup
     alpha_c = find_atoms(RECENT_ALPHA_C, structure)
     if alpha_c:
@@ -502,14 +551,33 @@
             return structure, True
         else:
             return structure, False
     else:
         return structure, False
 
 
+def exo_methylen_oxidase(structure: Structure) -> Tuple[Structure, bool]:
+    """
+    Returns the structure thats has a exomethylengroup at the alpha-c.
+
+    structure: PIKAChU Structure object
+    target_atom:  PIKAChU atom object
+    """
+    # find atom
+    alpha_c = find_atoms(RECENT_ALPHA_C, structure)
+    methyl_c = [neighbour for neighbour in alpha_c.neighbours() if neighbour.type == "C" and not neighbour.get("in_central_chain")][0]
+    if alpha_c and methyl_c:
+        if alpha_c[0].has_neighbour("H"):
+            structure = single_bond_oxidation(alpha_c, methyl_c, structure)
+            return structure, True
+        else:
+            return structure, False
+    else:
+        return structure, False
+
 def beta_methyl_transferase(structure: Structure) -> Tuple[Structure, bool]:
     """
     Returns the structure thats methylated at the beta-c.
 
     structure: PIKAChU Structure object
     target_atom:  PIKAChU atom object
     """
@@ -641,37 +709,41 @@
 
     for neighbour in co_bond.neighbours:
         if neighbour.type == 'C':
             c2 = neighbour
         elif neighbour.type == 'O':
             o_oh = neighbour
 
+    if not o_oh.has_neighbour('H'):
+        return chain_intermediate, False
+
     cc_bond = cc_bonds[0]
 
     for neighbour in cc_bond.neighbours:
         if neighbour != c2:
             c1 = neighbour
 
-    # Remove hydroxyl group from c2
-    chain_intermediate.break_bond(co_bond)
-
     # Remove H-atom from c1
     bond_to_break = None
     hydrogen = None
 
     for atom in chain_intermediate.graph:
         if atom == c1:
             for neighbour in atom.neighbours:
                 if neighbour.type == 'H':
                     hydrogen = neighbour
                     for bond in neighbour.bonds:
                         bond_to_break = bond
                     break
 
-    assert bond_to_break and hydrogen
+    if not bond_to_break or not hydrogen:
+        return chain_intermediate, False
+    
+    # Remove hydroxyl group from c2
+    chain_intermediate.break_bond(co_bond)
 
     chain_intermediate.break_bond(bond_to_break)
 
     # Patch. When the bond is broken, the electron is not removed from
     # the orbitals of the C atom.
     c1 = chain_intermediate.get_atom(c1)
 
@@ -689,24 +761,27 @@
         chain_intermediate = structure_1
     else:
         chain_intermediate = structure_2
 
     chain_intermediate.refresh_structure()
 
     # implement stereochemistry
+
     if chirality:
 
-        main_chain_top_c = find_atoms(RECENT_REDUCTION_SHIFTED_TOP_C, chain_intermediate)[0]
-        main_chain_bottom_c = find_atoms(RECENT_REDUCTION_SHIFTED_BOTTOM_C, chain_intermediate)[0]
+        main_chain_top_c = chain_intermediate.get_atom(find_atoms(RECENT_REDUCTION_SHIFTED_TOP_C, chain_intermediate)[0])
+        main_chain_bottom_c = chain_intermediate.get_atom(find_atoms(RECENT_REDUCTION_SHIFTED_BOTTOM_C, chain_intermediate)[0])
         main_chain_top_h = find_atoms(RECENT_REDUCTION_SHIFTED_TOP_H, chain_intermediate)
-        main_chain_bottom_h = find_atoms(RECENT_REDUCTION_SHIFTED_BOTTOM_H, chain_intermediate)[0]
+        main_chain_bottom_h = chain_intermediate.get_atom(find_atoms(RECENT_REDUCTION_SHIFTED_BOTTOM_H, chain_intermediate)[0])
         if not main_chain_bottom_h:
-            main_chain_bottom_h = find_atoms(RECENT_REDUCTION_SHIFTED_BOTTOM_METHYL, chain_intermediate)[0]
+            main_chain_bottom_h = chain_intermediate.get_atom(find_atoms(RECENT_REDUCTION_SHIFTED_BOTTOM_METHYL, chain_intermediate)[0])
         else:
-            main_chain_bottom_h = main_chain_bottom_h[0]
+
+            main_chain_bottom_h = chain_intermediate.get_atom(main_chain_bottom_h[0])
+
         if chirality == "E":
             double_bond.chiral_dict = {main_chain_top_c: {main_chain_bottom_c: 'trans',
                                                           main_chain_bottom_h: 'cis'},
                                        main_chain_top_h: {main_chain_bottom_c: 'cis',
                                                           main_chain_bottom_h: 'trans'},
                                        main_chain_bottom_c: {main_chain_top_c: 'trans',
                                                              main_chain_top_h: 'cis'},
@@ -719,8 +794,9 @@
                                                           main_chain_bottom_h: 'trans'},
                                        main_chain_bottom_c: {main_chain_top_c: 'cis',
                                                              main_chain_top_h: 'trans'},
                                        main_chain_bottom_h: {main_chain_top_c: 'trans',
                                                              main_chain_top_h: 'cis'}}
         double_bond.chiral = True
     chain_intermediate.refresh_structure()
+
     return chain_intermediate, True
```

### Comparing `raichu-0.0.2/raichu/substrate.py` & `raichu-1.0.0/raichu/substrate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,60 @@
-from paras.features import get_smiles
-from raichu.data.molecular_moieties import make_elongation_monomer
+from raichu.smiles_handling import get_smiles
+from raichu.data.molecular_moieties import make_elongation_monomer, make_starter_monomer
 from enum import Enum, unique
 
-_PKS_TO_SMILES = {"WILDCARD": r"SC(C([*])C(O)=O)=O",
-                  "MALONYL_COA": r"SC(CC(O)=O)=O",
-                  "METHYLMALONYL_COA": r"SC([C@H](C)C(O)=O)=O",
-                  "METHOXYMALONYL_ACP": r"SC(C(C(O)=O)OC)=O",
-                  "METHYLBUTYRYL_COA_2S": r"SC(=O)[C@@H](C)CC",
-                  "METHYLBUTYRYL_COA_2R": r"SC(=O)[C@H](C)CC",
-                  "ETHYLMALONYL_COA": r"SC(C(C(O)=O)CC)=O",
-                  "PROPIONYL_COA": r"SC(=O)CC",
-                  "ACETYL_COA": r"SC(C)=O",
-                  "BENZOYL_COA": r"SC(C1=CC=CC=C1)=O",
-                  "METHYL_BUTYRYL_COA_3": r"SC(=O)CC(C)C",
-                  "METHYL_BUTYRYL_COA_2": r"SC(=O)C(C)CC",
-                  "TRANS_CYCLOPENTANE_DICARBOXYL_COA": r"SC([C@H]1[C@@H](CCC1)C(=O)O)=O",
-                  "CYCLOHEXANE_CARBOXYL_COA": r"SC(=O)C1CCCCC1",
-                  "HYDROXY_MALONYL_COA_2": r"SC(=O)C(C(=O)O)O",
-                  "HYDROXY_MALONYL_COA_2R": r"SC(=O)[C@@H](C(=O)O)O",
-                  "HYDROXY_MALONYL_COA_2S": r"SC(=O)[C@H](C(=O)O)O",
-                  "CHLOROETHYL_MALONYL_COA": r"SC(C(C(=O)O)CC[Cl])=O",
-                  "ISOBUTYRYL_COA": r"SC(=O)C(C)C",
-                  "GLYCINE": "C(C(=O)O)N",
-                  "HYDROXY_PROPENOYL_COA_3_23E": r"[H]\C(O)=C/C(S)=O",
-                  "HYDROXY_BUTENOYL_COA_3_23E": r"C\C(O)=C/C(S)=O",
-                  "DIHYDROXY_BUTANOLYL_COA_2R3": r"CC(O)[C@@H](O)C(O)S",
-                  "TRIHYDROXY_PROPANOLYL_COA_233": r"OC(O)C(O)C(O)S",
-                  "O_METHYLACETYL_COA": r"COC(S)=O",
-                  "HYDROXY_PROPENOYL_COA_3_23Z": r"[H]\C(O)=C\C(S)=O",
-                  "OXOMALONYL_COA_2": r"OC(=O)C(=O)C(S)=O",
-                  "METHYL_HYDROXY_PROPENOYL_COA_2_3_23Z": r"[H]\C(O)=C(/C)C(S)=O",
-                  "DIHYDROXY_BUTANOLYL_COA_23": r"CC(O)C(O)C(O)S",
-                  "DIHYDROXY_BUTANOLYL_COA_2S3S": r"C[C@H](O)[C@H](O)C(O)S",
-                  "HEPTATRIENOYL_COA": r"SC(=O)C1=CC=CC=C3",
-                  "HYDROXYPROPIONYL_COA_2R": r"C[C@@H](O)C(S)=O",
-                  "DIHYDROXY_PROPANOLYL_COA_33": r"OC(O)CC(O)S",
-                  "LACTYL_COA": r"C[C@@H](O)C(S)=O",
-                  "PHENYLACETYLCOA": r"SC(=O)CC1=CC=CC=C1",
-                  "METHOXYFORMYL_COA": r"COC(S)=O"
-                  }
+
+_PKS_TO_SMILES = {
+    "WILDCARD": r"SC(C([*])C(O)=O)=O",
+    "WILDCARD_STARTER": r"SC(C([*]))=O",
+    "MALONYL_COA": r"SC(CC(O)=O)=O",
+    "METHYLMALONYL_COA": r"SC([C@H](C)C(O)=O)=O",
+    "METHOXYMALONYL_COA": r"SC(C(C(O)=O)OC)=O",
+    "METHYLBUTYRYL_COA_2S": r"SC(=O)[C@@H](C)CC",
+    "METHYLBUTYRYL_COA_2R": r"SC(=O)[C@H](C)CC",
+    "ETHYLMALONYL_COA": r"SC(C(C(O)=O)CC)=O",
+    "PROPIONYL_COA": r"SC(=O)CC",
+    "ACETYL_COA": r"SC(C)=O",
+    "BENZOYL_COA": r"SC(C1=CC=CC=C1)=O",
+    "METHYL_BUTYRYL_COA_3": r"SC(=O)CC(C)C",
+    "METHYL_BUTYRYL_COA_2": r"SC(=O)C(C)CC",
+    "TRANS_CYCLOPENTANE_DICARBOXYL_COA": r"SC([C@H]1[C@@H](CCC1)C(=O)O)=O",
+    "CYCLOHEXANE_CARBOXYL_COA": r"SC(=O)C1CCCCC1",
+    "HYDROXY_MALONYL_COA_2": r"SC(=O)C(C(=O)O)O",
+    "HYDROXY_MALONYL_COA_2R": r"SC(=O)[C@@H](C(=O)O)O",
+    "HYDROXY_MALONYL_COA_2S": r"SC(=O)[C@H](C(=O)O)O",
+    "CHLOROETHYL_MALONYL_COA": r"SC(C(C(=O)O)CC[Cl])=O",
+    "ISOBUTYRYL_COA": r"SC(=O)C(C)C",
+    "GLYCINE": "SC(CN)=O",
+    "HYDROXY_PROPENOYL_COA_3_23E": r"[H]\C(O)=C/C(S)=O",
+    "HYDROXY_BUTENOYL_COA_3_23E": r"C\C(O)=C/C(S)=O",
+    # "DIHYDROXY_BUTANOLYL_COA_2R3": r"CC(O)[C@@H](O)C(O)S",
+    # "TRIHYDROXY_PROPANOLYL_COA_233": r"OC(O)C(O)C(O)S",
+    "O_METHYLACETYL_COA": r"COC(S)=O",
+    "HYDROXY_PROPENOYL_COA_3_23Z": r"[H]\C(O)=C\C(S)=O",
+    "OXOMALONYL_COA_2": r"OC(=O)C(=O)C(S)=O",
+    "METHYL_HYDROXY_PROPENOYL_COA_2_3_23Z": r"[H]\C(O)=C(/C)C(S)=O",
+    # "DIHYDROXY_BUTANOLYL_COA_23": r"CC(O)C(O)C(O)S",
+    # "DIHYDROXY_BUTANOLYL_COA_2S3S": r"C[C@H](O)[C@H](O)C(O)S",
+    "HEPTATRIENOYL_COA": r"SC(=O)C=CC=CC=C",
+    "HYDROXYPROPIONYL_COA_2R": r"C[C@@H](O)C(S)=O",
+    # "DIHYDROXY_PROPANOLYL_COA_33": r"OC(O)CC(O)S",
+    "LACTYL_COA": r"C[C@@H](O)C(S)=O",
+    "PHENYLACETYLCOA": r"SC(=O)CC1=CC=CC=C1",
+    "METHOXYFORMYL_COA": r"COC(S)=O",
+}
+
+_TERPENE_PRECURSOR_TO_SMILES = {
+    "DIMETHYLALLYL_PYROPHOSPHATE": r"CC(=CCOP(=O)(O)OP(=O)(O)O)C",
+    "GERANYL_PYROPHOSPHATE": r"O=P(O)(O)OP(=O)(OC/C=C(/CC\C=C(/C)C)C)O",
+    "FARNESYL_PYROPHOSPHATE": r"CC(=CCC/C(=C/CC/C(=C/COP(=O)(O)OP(=O)(O)O)/C)/C)C",
+    "GERANYLGERANYL_PYROPHOSPHATE": r"O=P(O)(O)OP(=O)(O)OC/C=C(/CC\C=C(/C)CC\C=C(/C)CC\C=C(/C)C)C",
+    "SQUALENE": r"CC(=CCC/C(=C/CC/C(=C/CC/C=C(/CC/C=C(/CCC=C(C)C)\C)\C)/C)/C)C",
+    "PHYTOENE": r"CC(=CCC/C(=C/CC/C(=C/CC/C(=C/C=C\C=C(/C)\CC/C=C(\C)/CC/C=C(\C)/CCC=C(C)C)/C)/C)/C)C",
+}
 
 
 @unique
 class PksStarterSubstrate(Enum):
     PROPIONYL_COA = 1
     ACETYL_COA = 2
     BENZOYL_COA = 3
@@ -54,53 +66,50 @@
     HYDROXY_MALONYL_COA_2S = 9  # 2S-hydroxymalonyl-CoA
     HYDROXY_MALONYL_COA_2R = 10  # 2R-hydroxymalonyl-CoA
     CHLOROETHYL_MALONYL_COA = 11
     ISOBUTYRYL_COA = 12
     GLYCINE = 13
     HYDROXY_PROPENOYL_COA_3_23E = 14  # 3-hydroxy-2,3-E-propenoyl-CoA
     HYDROXY_BUTENOYL_COA_3_23E = 15  # 3-hydroxy-2,3-E-butenoyl-CoA
-    DIHYDROXY_BUTANOLYL_COA_2R3 = 16  # 2R,3-dihydroxy-butanolyl-CoA
-    TRIHYDROXY_PROPANOLYL_COA_233 = 17  # 2,3,3-trihydroxy-propanolyl-CoA
-    O_METHYLACETYL_COA = 18  # O-methylacetyl-CoA
-    HYDROXY_PROPENOYL_COA_3_23Z = 19  # 3-hydroxy-2,3-Z-propenoyl-CoA
-    OXOMALONYL_COA_2 = 20  # 2-oxomalonyl-CoA
-    METHYL_HYDROXY_PROPENOYL_COA_2_3_23Z = 21  # 2-methyl-3-hydroxy-2,3-Z-propenoyl-CoA
-    DIHYDROXY_BUTANOLYL_COA_23 = 22  # 2,3-dihydroxy-butanolyl-CoA
-    DIHYDROXY_BUTANOLYL_COA_2S3S = 23  # 2S,3S-dihydroxy-butanolyl-CoA
-    HEPTATRIENOYL_COA = 24  # 2,4,6-heptatrienoyl-CoA
-    HYDROXYPROPIONYL_COA_2R = 25  # 2R-hydroxypropionyl-CoA
-    DIHYDROXY_PROPANOLYL_COA_33 = 26  # 3,3-dihydroxy-propanolyl-CoA
-    LACTYL_COA=27
-    PHENYLACETYLCOA=28
-    METHOXYFORMYL_COA=29
+    O_METHYLACETYL_COA = 16  # O-methylacetyl-CoA
+    HYDROXY_PROPENOYL_COA_3_23Z = 17  # 3-hydroxy-2,3-Z-propenoyl-CoA
+    OXOMALONYL_COA_2 = 18  # 2-oxomalonyl-CoA
+    METHYL_HYDROXY_PROPENOYL_COA_2_3_23Z = 19  # 2-methyl-3-hydroxy-2,3-Z-propenoyl-CoA
+    HEPTATRIENOYL_COA = 20  # 2,4,6-heptatrienoyl-CoA
+    HYDROXYPROPIONYL_COA_2R = 21  # 2R-hydroxypropionyl-CoA
+    LACTYL_COA = 22
+    PHENYLACETYLCOA = 23
+    METHOXYFORMYL_COA = 24
+    WILDCARD_STARTER = 25
 
     @staticmethod
     def from_string(label: str):
-        for value in PksElongationSubstrate:
+        for value in PksStarterSubstrate:
             if str(value) == label:
                 return value
         raise ValueError(f"Unknown PKS starter substrate: {label}")
 
     @staticmethod
     def get_smiles(label: str):
-        for value in PksElongationSubstrate:
+        for value in PksStarterSubstrate:
             if str(value) == label:
                 return _PKS_TO_SMILES[value]
 
         raise ValueError(f"Unknown PKS starter substrate: {label}")
 
 
 @unique
 class PksElongationSubstrate(Enum):
     WILDCARD = 1
     MALONYL_COA = 2
     METHYLMALONYL_COA = 3
-    METHOXYMALONYL_ACP = 4
-    METHYLBUTYRYL_COA_2S = 5
-    METHYLBUTYRYL_COA_2R = 6
+    METHOXYMALONYL_COA = 4
+    # TODO: something is wrong with those substrates
+    # METHYLBUTYRYL_COA_2S = 5
+    # METHYLBUTYRYL_COA_2R = 6
     ETHYLMALONYL_COA = 7
 
     @staticmethod
     def from_string(label: str):
         for value in PksElongationSubstrate:
             if str(value) == label:
                 return value
@@ -123,19 +132,42 @@
 
 class NRPSSubstrate(Substrate):
     def __init__(self, name: str) -> None:
         smiles = get_smiles(name)
         super().__init__(name, smiles)
 
 
+class AminoAcidSubstrate(Substrate):
+    def __init__(self, name: str) -> None:
+        smiles = get_smiles(name)
+        super().__init__(name, smiles)
+
+
 class PKSSubstrate(Substrate):
     def __init__(self, name: str) -> None:
         smiles = _PKS_TO_SMILES.get(name, None)
         if smiles is None:
+
             raise ValueError(f"Cannot fetch SMILES string for PKS substrate {name}.")
         super().__init__(name, smiles)
-        if name in [v.name for v in PksElongationSubstrate]:
+        if name == "WILDCARD":
+            self.smiles = _PKS_TO_SMILES.get("WILDCARD_STARTER", None)
+            self.starter_monomer = make_starter_monomer("WILDCARD_STARTER", self.smiles)
+            self.elongation_monomer = make_elongation_monomer(self.name)
+        elif name in [v.name for v in PksElongationSubstrate]:
             self.elongation_monomer = make_elongation_monomer(self.name)
+            self.starter_monomer = None
         elif name in [v.name for v in PksStarterSubstrate]:
             self.elongation_monomer = None
+            self.starter_monomer = make_starter_monomer(self.name, self.smiles)
         else:
             raise ValueError(f"PKS substrate {self.name} is not recognised by RAIChU.")
+
+
+class TerpeneCyclaseSubstrate(Substrate):
+    def __init__(self, name: str) -> None:
+        smiles = _TERPENE_PRECURSOR_TO_SMILES.get(name, None)
+        if smiles is None:
+            raise ValueError(
+                f"Cannot fetch SMILES string for terpene cyclase substrate {name}."
+            )
+        super().__init__(name, smiles)
```

### Comparing `raichu-0.0.2/raichu.egg-info/SOURCES.txt` & `raichu-1.0.0/raichu.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 bin/raichu
 interactive/__init__.py
 interactive/background.py
 interactive/buttons.py
@@ -257,14 +258,16 @@
 interactive/images/nrps_substrates/Homoserine_highlight.png
 interactive/images/nrps_substrates/Homotyrosine.png
 interactive/images/nrps_substrates/Homotyrosine_highlight.png
 interactive/images/nrps_substrates/HydroxyPhenylGlycine.png
 interactive/images/nrps_substrates/HydroxyPhenylGlycine_highlight.png
 interactive/images/nrps_substrates/Isoleucine.png
 interactive/images/nrps_substrates/Isoleucine_highlight.png
+interactive/images/nrps_substrates/Isovaline.png
+interactive/images/nrps_substrates/Isovaline_highlight.png
 interactive/images/nrps_substrates/L-piperazicacid.png
 interactive/images/nrps_substrates/L-piperazicacid_highlight.png
 interactive/images/nrps_substrates/Leucine.png
 interactive/images/nrps_substrates/Leucine_highlight.png
 interactive/images/nrps_substrates/Lysine.png
 interactive/images/nrps_substrates/Lysine_highlight.png
 interactive/images/nrps_substrates/Methionine.png
@@ -403,44 +406,68 @@
 interactive/images/pks_substrates/methoxymalonylcoa.png
 interactive/images/pks_substrates/methoxymalonylcoa_highlight.png
 interactive/images/pks_substrates/methylmalonylcoa.png
 interactive/images/pks_substrates/methylmalonylcoa_highlight.png
 interactive/images/pks_substrates/wildcard.png
 interactive/images/pks_substrates/wildcard_highlight.png
 raichu/__init__.py
+raichu/alkaloid.py
+raichu/antismash.py
 raichu/attach_to_domain.py
 raichu/class_domain.py
-raichu/cluster.py
+raichu/general.py
 raichu/module.py
+raichu/representations.py
+raichu/ripp.py
 raichu/run_raichu.py
-raichu/run_raichu_trans_at.py
+raichu/smiles_handling.py
 raichu/substrate.py
+raichu/tailoring_enzymes.py
 raichu.egg-info/PKG-INFO
 raichu.egg-info/SOURCES.txt
 raichu.egg-info/dependency_links.txt
 raichu.egg-info/requires.txt
 raichu.egg-info/top_level.txt
 raichu/central_chain_detection/__init__.py
 raichu/central_chain_detection/find_central_chain.py
 raichu/central_chain_detection/label_central_chain.py
-raichu/data/PARAS_smiles.txt
+raichu/cluster/__init__.py
+raichu/cluster/alkaloid_cluster.py
+raichu/cluster/base_cluster.py
+raichu/cluster/modular_cluster.py
+raichu/cluster/ripp_cluster.py
+raichu/cluster/terpene_cluster.py
 raichu/data/__init__.py
 raichu/data/at_elongation_specificities.txt
 raichu/data/at_specificities.txt
 raichu/data/attributes.py
+raichu/data/metadata.txt
 raichu/data/molecular_moieties.py
+raichu/data/smiles.txt
 raichu/data/substrate_to_abbreviation.txt
 raichu/data/trans_at.py
 raichu/domain/__init__.py
 raichu/domain/domain.py
 raichu/domain/domain_types.py
 raichu/drawing/__init__.py
 raichu/drawing/bubbles.py
 raichu/drawing/colours.py
 raichu/drawing/drawer.py
+raichu/drawing/pathway.py
+raichu/drawing/ripp_drawing.py
 raichu/reactions/__init__.py
 raichu/reactions/chain_release.py
 raichu/reactions/general.py
+raichu/reactions/general_tailoring_reactions.py
 raichu/reactions/nrps_elongation_reactions.py
 raichu/reactions/nrps_tailoring_reactions.py
 raichu/reactions/pks_elongation_reactions.py
-raichu/reactions/pks_tailoring_reactions.py
+raichu/reactions/pks_sidechain_chirality.py
+raichu/reactions/pks_tailoring_reactions.py
+raichu/reactions/ripp_reactions.py
+raichu/test/__init__.py
+raichu/test/generate_test_data.py
+raichu/test/test_data/__init__.py
+raichu/test/unit/__init__.py
+raichu/test/unit/reactions/__init__.py
+raichu/test/unit/reactions/test_general_tailoring_reactions.py
+raichu/test/unit/reactions/test_nrps_tailoring_reactions.py
```

### Comparing `raichu-0.0.2/setup.py` & `raichu-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '1.0.0'
 DESCRIPTION = 'RAIChU'
-LONG_DESCRIPTION = 'An interactive PKS/NRPS visualizer.'
+LONG_DESCRIPTION = 'A package to automatically draw natural product biosynthesis pathways.'
 
 print(find_packages())
 
 setup(
     name="raichu",
     version=VERSION,
+    
     author="Barbara Terlouw",
     author_email="barbara.r.terlouw@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(exclude="build"),
     package_data={"": ["*.png", "*.svg", "*.txt"]},
     install_requires=['matplotlib',
-                      'pikachu-chem',
-                      'paras'],
+                      'biopython==1.76',
+                      'pikachu-chem>=1.1.1'],
     scripts=["bin/raichu"],)
```

