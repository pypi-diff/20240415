# Comparing `tmp/arm-test-data-0.0.8.tar.gz` & `tmp/arm-test-data-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm-test-data-0.0.8.tar", last modified: Mon Mar 25 18:47:07 2024, max compression
+gzip compressed data, was "arm-test-data-0.0.9.tar", last modified: Wed Mar 27 19:55:04 2024, max compression
```

## Comparing `arm-test-data-0.0.8.tar` & `arm-test-data-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:47:07.228098 arm-test-data-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:47:07.224098 arm-test-data-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:47:07.228098 arm-test-data-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-03-25 18:47:07.228098 arm-test-data-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:47:07.228098 arm-test-data-0.0.8/arm_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/arm_test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/arm_test_data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/arm_test_data/registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-25 18:47:06.000000 arm-test-data-0.0.8/arm_test_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:47:07.228098 arm-test-data-0.0.8/arm_test_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-03-25 18:47:06.000000 arm-test-data-0.0.8/arm_test_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-25 18:47:07.000000 arm-test-data-0.0.8/arm_test_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:47:06.000000 arm-test-data-0.0.8/arm_test_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 18:47:06.000000 arm-test-data-0.0.8/arm_test_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 18:47:06.000000 arm-test-data-0.0.8/arm_test_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/make_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 18:46:54.000000 arm-test-data-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 18:47:07.228098 arm-test-data-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:55:04.736840 arm-test-data-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:55:04.732839 arm-test-data-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:55:04.732839 arm-test-data-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-03-27 19:55:04.736840 arm-test-data-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:55:04.732839 arm-test-data-0.0.9/arm_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/arm_test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/arm_test_data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/arm_test_data/registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-27 19:55:04.000000 arm-test-data-0.0.9/arm_test_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:55:04.736840 arm-test-data-0.0.9/arm_test_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8958 2024-03-27 19:55:04.000000 arm-test-data-0.0.9/arm_test_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-27 19:55:04.000000 arm-test-data-0.0.9/arm_test_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:55:04.000000 arm-test-data-0.0.9/arm_test_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 19:55:04.000000 arm-test-data-0.0.9/arm_test_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-27 19:55:04.000000 arm-test-data-0.0.9/arm_test_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/make_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 19:54:54.000000 arm-test-data-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:55:04.736840 arm-test-data-0.0.9/setup.cfg
```

### Comparing `arm-test-data-0.0.8/.github/workflows/ci.yaml` & `arm-test-data-0.0.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `arm-test-data-0.0.8/.github/workflows/pypi-release.yml` & `arm-test-data-0.0.9/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `arm-test-data-0.0.8/.gitignore` & `arm-test-data-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `arm-test-data-0.0.8/LICENSE` & `arm-test-data-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arm-test-data-0.0.8/PKG-INFO` & `arm-test-data-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-test-data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides utility functions for accessing data repository for ARM data examples/notebooks
 Author: Atmospheric Data Community Toolkit Dev Team
 License: MIT License
         
         Copyright (c) 2023 ARM User Facility
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `arm-test-data-0.0.8/README.md` & `arm-test-data-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `arm-test-data-0.0.8/arm_test_data/dataset.py` & `arm-test-data-0.0.9/arm_test_data/dataset.py`

 * *Files identical despite different names*

### Comparing `arm-test-data-0.0.8/arm_test_data/registry.txt` & `arm-test-data-0.0.9/arm_test_data/registry.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 201509021500.bi 27f1065949fbe89b1c74b885d4de64c8e7af138556037fe7f9d340ac6d5db3eb
-AAFNAV_COR_20181104_R0.ict 5de076da3b7eb2e3b6dc4bbd26605d9a49ab00da56c761d2a70f348ea1794f82
-NEON.D18.BARR.DP1.00002.001.000.010.001.SAAT_1min.2022-10.expanded.20221107T205629Z.csv dc0b5fefaa4face49011a90197b0557b4c61dc84946ed5d82da2456c4b7d6c20
-NEON.D18.BARR.DP1.00002.001.sensor_positions.20221107T205629Z.csv a0b9c558ee40be981e57e21e123ea3f500246f686d6947316af92364b7a5ef31
-NEON.D18.BARR.DP1.00002.001.variables.20221201T110553Z.csv d21e2896b88adb25e78f024c55d268c0dd5ca4cb7853f97cd0ab88950a9d2014
-anltwr_mar19met.data d622714395b37499312d09f48aa08ca47b4a10cbdcb170db79acfe3733702ae7
+AAFNAV_COR_20181104_R0.ict 27f2a9f2cb4c6b4c46dcd23f55ec7a698c183fc6330fb1c76d7749bcf5b47889
+NEON.D18.BARR.DP1.00002.001.000.010.001.SAAT_1min.2022-10.expanded.20221107T205629Z.csv 613bc7f56592667ff333161d81fe71e6f05569413007465b72cb21bd072317fc
+NEON.D18.BARR.DP1.00002.001.sensor_positions.20221107T205629Z.csv 8d482e02ef0254b845e193c37875cc9048ea9f197b3ad451fb78fcfeec42629c
+NEON.D18.BARR.DP1.00002.001.variables.20221201T110553Z.csv 0b5d1ea07a6156085ebadbd78f3154171caf07406414d19ef227148aef6e641a
+anltwr_mar19met.data a44d37b45545c917731babcef2deb16775e0fbfd4bc69c3c36c5d909e3c6544e
 ayp22199.21m 20490713dbe93174842902e8712d2617f7f468fad1fc3dd7bddefb6e81d965f7
 ayp22200.00m 3f1499d4cfb9b7f6404bfffbc3bb3653807861ebcf2371372d5533b2a5069279
-brw21001.dat e238fc434e763fd4c1fe0cfe67b07b8fe746aaf55d7dcccdeedd6d583202d107
-brw_12_2020_hour.dat 4e9e859e68d3db1e89da84d262d144596cb2e90ec59ea2e7aca5e08582b71028
-brw_CCl4_Day.dat 792405e91729f5849ce83863425dcad1b7e19c7ec2a124dec45fd0aa152bcc45
-co2_brw_surface-insitu_1_ccgg_MonthlyData.txt 06c1156aba19825e3f5a5f97d8a73dba216ab23bc33dd92e3cf41e725b12422c
+brw21001.dat f40e5365092996966f4d9d080636b47c96afb8f58824a5884a7a64c873b84736
+brw_12_2020_hour.dat 560fb1f7b7b5e957ea69175704233b777914ed9ec652d760511128f97aae540c
+brw_CCl4_Day.dat 308cd66e6729b8446274b61eb0abfa0192df739f0ec63efedac71112b5c23947
+co2_brw_surface-insitu_1_ccgg_MonthlyData.txt 60b48b28d2bbc970659d12ce63353525ccc91c0611d9f78cf5702f9bff6ac060
 ctd21125.15w 35c271163967fe249a0122e77f592d59754f463e0ddd834bd1804b4ce285be12
 ctd22187.00t.txt 414559c37cf336e5609914bbd5e6ceecd8ed9d9f16ca606ca2d37244b4422544
 enametC1.b1.20221109.000000.cdf 0f6e1580e1cd0b93f53b9ada2bfea2df40c18fbd574c7f292cbfb65398f2cfa3
 gucmetM1.b1.20230301.000000.cdf 507690c5823ad88e5047e70c1a88a46cd873a02380172743fe1d1ccf7eed957d
-houstonaug300.0summer2010080100 a873bc065bcd5e13966a1eb02e87acfe3bc2f2a4f70e70860d2bb1d28ed82524
+houstonaug300.0summer2010080100 aa3499b3c331e5477b4cd319ec1df80519539dc555fdc1ec1c7e105311542251
 maraosmetM1.a1.20180201.000000.nc b0f09897712422405857878eb411555bde37519d18de575b221f3e5bb52dcd07
 marirtsstM1.b1.20190320.000000.nc c3d979b66fb702694701aede0204ab241c30e7449cd89308a94a07c953754ef1
 marnavM1.a1.20180201.000000.nc 350bb0ae1ccba11131a15fbce276c1b8fab0daa10755fcd5ed446bad7c458243
-met_brw_insitu_1_obop_hour_2020.txt ef2b3f577a104b0a813cc269e1873e447e6034e8527ee7c4a39205dc0df3a101
+met_brw_insitu_1_obop_hour_2020.txt f2dbbc3c97754d6c1cf7fa8095f35461d1091b07b50f59a2c87f8f4dcaae0272
 met_lcl.nc c937216bcc66b2c34fef9cdac4be410a8698e55d78cc8f4e19e2f05018b3570c
 mosaossp2M1.00.20191216.000601.raw.20191216000000.ini fc4178a644755b715dc3c0d3573eb8fd09916f5561c14a68aad64fe21311d686
 mosaossp2M1.00.20191216.130601.raw.20191216x193.sp2b 9660a548c5d3eee157c325d0a931372189c195f21c101e27916fc46da69c8092
 mosaossp2auxM1.00.20191217.010801.raw.20191216000000.hk 35223771c33b592c22b9c428c6504589150b06f58f90e9cf24ca44686a079175
 nsacloudphaseC1.c1.20180601.000000.nc 8c94876f91fde3785bbacb07d7a7ff66e821df669c8146da8cce8584a2407556
 nsasurfspecalb1mlawerC1.c1.20160609.080000.nc 84f97d09cec0f8c5d8d8ddfd96d5625be4860cfa3593fc12a9f44d80bff8e144
 sgp30ebbrE13.b1.20190601.000000.nc 93ef098581a2c9a4915d5d7cfc77ca27c4f3a38958e07b816c33b28cb925f6c5
@@ -43,16 +43,16 @@
 sgpmetE13.b1.20190102.000000.cdf f74dac2ee6edcccb5ab18dc9af19bea14b8e1c4b7d45c542e7a2fd79737c9eea
 sgpmetE13.b1.20190103.000000.cdf 35369af0e8bb1dd6039e4cf2644ed46c332283956ef2b501bda74e338a3f0140
 sgpmetE13.b1.20190104.000000.cdf 5d4591d042bc73122a7184b4983941d0b99a177305f84c45dfca852c8645743f
 sgpmetE13.b1.20190105.000000.cdf 235f18bb97cb085b8b68fafbe2415e42f2f91dce58a3c0a62fda944814c54813
 sgpmetE13.b1.20190106.000000.cdf 8d782af1ab1f2a6c8a3621e33bf17e21f86568d473eeb32efc7b6a96be372d4b
 sgpmetE13.b1.20190107.000000.cdf 33172799e128b40d3d9c45b65ac728b6b99e4d5fec3ac0a68385873b021e83fc
 sgpmetE13.b1.20190508.000000.cdf aa97f7f14b1a853735df638a940d051e91c45fc454b912566b16dbb0e1799c50
-sgpmetE13.b1.20210401.000000.csv a04117a44a916efa86a1fdd119481838d3146d1558579951c3aa60d18c677448
-sgpmetE13.b1.yaml 1132225195ddf5785e599a884907d23c09fcda5dfeb8e52be57dc9ff363b3a42
+sgpmetE13.b1.20210401.000000.csv 337332c03146696e53001dfefe22325537f3f8a1c84e662b9de45224672705e9
+sgpmetE13.b1.yaml 663e806bf20eb790aa05b15208a3994fe5317e774fd3b44f2fd10461c746cfae
 sgpmetE15.b1.20190508.000000.cdf 4c16df95bcefced0d163c408b11748533d4af958fb7626d37be8bd0ec706f0b3
 sgpmetE31.b1.20190508.000000.cdf 3aa08694164787ae69ad992d577b7f615dfb730bb43ccea6b51edcc06459147d
 sgpmetE32.b1.20190508.000000.cdf 669444dd3aed778a89c560cd6312f46ac054e0195e9000f6427942c3991e1c7d
 sgpmetE33.b1.20190508.000000.cdf 1921e65e6abfcf920b7d948524c613eee3ac529c293960205335945f9b9e56fc
 sgpmetE34.b1.20190508.000000.cdf f27a795a19af54e38b270565af9c2ebc56fe78ab32449a89756a3da15872d754
 sgpmetE35.b1.20190508.000000.cdf 7fcf103504500c0a74468f974d9304ac586c5d0c2e04b7dd53a0d331d7343019
 sgpmetE36.b1.20190508.000000.cdf a0ba48d96499864bb8b137283134ae0a7fa1a677d5b9581a36197ef6c60f4c1d
@@ -60,29 +60,29 @@
 sgpmetE38.b1.20190508.000000.cdf f7981fae7a8f9557ba26052ea485da450185e48dc006e9c2f85eda9fd11e01d7
 sgpmetE39.b1.20190508.000000.cdf 6360c5bbadcfddb6154a136b58b8252c784c87fac0bb98f3bbfee78e8aa4c8bb
 sgpmetE40.b1.20190508.000000.cdf 54dfc093943784c782ed1e211e74869872ba13b90eaf9294142eb4325802b6c9
 sgpmetE9.b1.20190508.000000.cdf b8d2870a65ca0d9113938ab139220d340fb6ed71d877e3419c1aaa6db784224d
 sgpmet_no_time.nc 8f943a9167b5ab84224a5a66b5b487684635945f832c1c7de2cb6ee483319f2b
 sgpmet_test_time.nc 0cb5c8444459e1d9a743a25bbb78a69dc2a342b86367d7b93badf19242a20d76
 sgpmfrsr7nchE11.b1.20210329.070000.nc de1b307c24091fa16293635d1ff79cd05efa92e4f502674eb4968a7aa29caf38
-sgpmfrsr7nchE11.b1.yaml 83bb47e31073383d23272ca4104aa5bc601707f6f6d2ef923f698ab7bd4731e9
+sgpmfrsr7nchE11.b1.yaml b1f4c9fdcb23582960df142903e005db7bb87619040e79409fd104403acf1b1e
 sgpmmcrC1.b1.1.cdf b003d83526eb88c88d892fb29ed837347fa3c0d172cef1ffa07e8461df0679de
 sgpmmcrC1.b1.2.cdf 5b281de250aeaad9c9f5b1b8f1189197cc7b560b5456c3cb60930ad9beb9290b
 sgpmplpolfsC1.b1.20190502.000000.cdf 4aac939de00224a78da3c807e75a74e8eee982bc6a146e6c9bd7407b93118dcd
 sgprlC1.a0.20160131.000000.nc 268100c8f613e2c6461350b3c7ad5400ac62c1f59028b5bb066887d2d86d85e3
 sgpsebsE14.b1.20190601.000000.cdf aa303a669592505ceae4f0f5f5faeb1af141c604507153963de0fd1d7709a742
 sgpsirsE13.b1.20190101.000000.cdf 5319dce8baee58e68d184ebe0db3d2e78d9848449c3bba7e7b54e9061ea24b0c
 sgpsondewnpnC1.b1.20190101.053200.cdf fda7734596114373665cf34e3f89ef07f915933763b5c6e949694eeeca0fe24d
 sgpstampE13.b1.20200101.000000.nc 1e4294796668aae5a1966a13bbb620d835b2da2ce789d10ad91afcfbed70c265
 sgpstampE31.b1.20200101.000000.nc 86f578b522ae682eb20686a2d3a2b7e6cda396cdb1b14ce53087b4924fb1ddbb
 sgpstampE32.b1.20200101.000000.nc 19b178f4f93b79f0a56e2cd24e3f59b292680e72175b7c00774d7da70c82a64e
 sgpstampE33.b1.20200101.000000.nc bceee025bf3dd81cfcd8c2e89cfcbc465e7ce942e3ea380e94839623fe435a3d
 sgpstampE34.b1.20200101.000000.nc fb6677d675ee8a25570cbdb518a8b39093690baa7309a776ce2125f680802b70
 sgpstampE9.b1.20200101.000000.nc c9cad1cad5a5818a259cdcecc3c1379704dca82e2ace0a0b25b0da19f231b03c
-sodar.20230404.mnd f0b7d5815b170e4b29bf61689f70058b5afa808a1f5a64656aca0147b51c12db
+sodar.20230404.mnd dd03abaedb0646e55c47345a9f5639deb0c6c50a8f22f3cfc28218cf7a223165
 twpsondewnpnC3.b1.20060119.050300.custom.cdf 6db6f555e7e7a4c5a30da88d5949317674fe23720c71d7f3b5cd2f7354b5a128
 twpsondewnpnC3.b1.20060119.112000.custom.cdf bd69dfa3eccd533b372df14c7a206130fab054cddbf493005e9ac204ce875f4e
 twpsondewnpnC3.b1.20060119.163300.custom.cdf 456491abac0ec31a0808f6631f64bbda72e32df649285e936fe1d660775c3396
 twpsondewnpnC3.b1.20060119.231600.custom.cdf 11e8c0cc3ab9fcc1cd4043602f2a9fe75dad5cbc74093e2ce5057fcba427915b
 twpsondewnpnC3.b1.20060120.043800.custom.cdf 48d32fd24cb39fe44d8f3ce622e58f88ad55f5b24a299c7bfd35335533b9dfc9
 twpsondewnpnC3.b1.20060120.111900.custom.cdf 70446c96bc4d9d0bfd84145ff44ee156b2563d65fea95131d17c22d51f50a54d
 twpsondewnpnC3.b1.20060120.170800.custom.cdf 346646cb9dbe61bdd9c5f7243e31123964b182fcdd57ef69f96eeaf5a4a38892
@@ -100,8 +100,8 @@
 twpsondewnpnC3.b1.20060123.171600.custom.cdf 952e18fec12d15a077175af593756098d691c2f38504b75f4efabe8b4ce98812
 twpsondewnpnC3.b1.20060123.231500.custom.cdf 0094f0973afa9e2a6d2629448aa66a930bad6cd9ef9a7c7dbc887f09b5c795f0
 twpsondewnpnC3.b1.20060124.051500.custom.cdf 663f87075fc8b7d8f0d03df0a46a7a04cfd02933ec977ff252a07b284ab1e42e
 twpsondewnpnC3.b1.20060124.111800.custom.cdf b8742dede3d7151e01fba6f9d9e5dce0dd26c46f85a4e87d5790d9aecdb6d024
 twpsondewnpnC3.b1.20060124.171700.custom.cdf 07eb0914120342ba73dfbdc601a06037357e64be594f90563fabbe4687dd6aea
 twpsondewnpnC3.b1.20060124.231500.custom.cdf 883c5c4c55cc1ac4533064d548ffc33ec37e2f5fe99ea39b221782ddefb72db4
 twpvisstgridirtemp.c1.20050705.002500.nc b26f9206c3a1706f43eb623c67c1bf4854f8847f89367b819aebbb70842bba18
-vdis.b1 41e81340f054aa4aa0ecb83f4c9a491659bcf19c97d995b96caf849c9c46617d
+vdis.b1 a1770fc0f655196c717f52eea62442370c3be186b420b31f81a26b52dcafb1ba
```

### Comparing `arm-test-data-0.0.8/arm_test_data.egg-info/PKG-INFO` & `arm-test-data-0.0.9/arm_test_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-test-data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Provides utility functions for accessing data repository for ARM data examples/notebooks
 Author: Atmospheric Data Community Toolkit Dev Team
 License: MIT License
         
         Copyright (c) 2023 ARM User Facility
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `arm-test-data-0.0.8/pyproject.toml` & `arm-test-data-0.0.9/pyproject.toml`

 * *Files identical despite different names*

