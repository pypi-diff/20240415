# Comparing `tmp/datanommer_models-1.1.0.tar.gz` & `tmp/datanommer_models-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanommer_models-1.1.0.tar", max compression
+gzip compressed data, was "datanommer_models-1.2.0.tar", max compression
```

## Comparing `datanommer_models-1.1.0.tar` & `datanommer_models-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_models-1.1.0/LICENSE
--rw-r--r--   0        0        0     1091 2023-09-22 07:24:59.659106 datanommer_models-1.1.0/NEWS.rst
--rw-r--r--   0        0        0      302 2022-01-17 12:04:04.000000 datanommer_models-1.1.0/README.rst
--rw-r--r--   0        0        0      916 2022-07-06 08:10:03.000000 datanommer_models-1.1.0/alembic.ini
--rw-r--r--   0        0        0    10843 2023-06-13 09:09:58.000000 datanommer_models-1.1.0/coverage.xml
--rw-r--r--   0        0        0    17223 2023-06-13 11:54:46.000000 datanommer_models-1.1.0/datanommer/models/__init__.py
--rw-r--r--   0        0        0     2793 2022-07-06 08:10:03.000000 datanommer_models-1.1.0/datanommer/models/alembic/env.py
--rw-r--r--   0        0        0      412 2022-07-06 08:10:03.000000 datanommer_models-1.1.0/datanommer/models/alembic/script.py.mako
--rw-r--r--   0        0        0      249 2022-07-06 08:10:03.000000 datanommer_models-1.1.0/datanommer/models/alembic/versions/5db25abc63be_init.py
--rw-r--r--   0        0        0      843 2022-07-06 08:10:03.000000 datanommer_models-1.1.0/datanommer/models/alembic/versions/951c40020acc_unique.py
--rw-r--r--   0        0        0     1271 2022-01-17 12:04:04.000000 datanommer_models-1.1.0/datanommer/models/testing/__init__.py
--rw-r--r--   0        0        0       44 2022-01-17 12:04:04.000000 datanommer_models-1.1.0/datanommer/models/testing/startup.sql
--rw-r--r--   0        0        0     4499 2023-09-22 07:24:59.659106 datanommer_models-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       45 2022-01-17 12:04:04.000000 datanommer_models-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1928 2022-01-20 08:43:17.000000 datanommer_models-1.1.0/tests/test_jsonencodeddict.py
--rw-r--r--   0        0        0    18949 2023-06-13 09:23:37.000000 datanommer_models-1.1.0/tests/test_model.py
--rw-r--r--   0        0        0      512 2023-09-18 08:58:03.625951 datanommer_models-1.1.0/tox.ini
--rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 datanommer_models-1.1.0/setup.py
--rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 datanommer_models-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_models-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1614 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/NEWS.rst
+-rw-r--r--   0        0        0      302 2022-01-17 12:04:04.000000 datanommer_models-1.2.0/README.rst
+-rw-r--r--   0        0        0      916 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/alembic.ini
+-rw-r--r--   0        0        0    11002 2024-04-11 07:27:40.911012 datanommer_models-1.2.0/coverage.xml
+-rw-r--r--   0        0        0    16874 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/datanommer/models/__init__.py
+-rw-r--r--   0        0        0     2793 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/env.py
+-rw-r--r--   0        0        0      412 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/script.py.mako
+-rw-r--r--   0        0        0      249 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/versions/5db25abc63be_init.py
+-rw-r--r--   0        0        0      843 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/versions/951c40020acc_unique.py
+-rw-r--r--   0        0        0     1453 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/datanommer/models/testing/__init__.py
+-rw-r--r--   0        0        0     4279 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2022-01-17 12:04:04.000000 datanommer_models-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1882 2024-04-15 09:57:21.429639 datanommer_models-1.2.0/tests/test_jsonencodeddict.py
+-rw-r--r--   0        0        0    20108 2024-04-15 09:57:21.429639 datanommer_models-1.2.0/tests/test_model.py
+-rw-r--r--   0        0        0      543 2024-04-15 09:57:21.429639 datanommer_models-1.2.0/tox.ini
+-rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 datanommer_models-1.2.0/PKG-INFO
```

### Comparing `datanommer_models-1.1.0/LICENSE` & `datanommer_models-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.1.0/alembic.ini` & `datanommer_models-1.2.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.1.0/coverage.xml` & `datanommer_models-1.2.0/coverage.xml`

 * *Files 2% similar despite different names*

#### Comparing `datanommer_models-1.1.0/coverage.xml` & `datanommer_models-1.2.0/coverage.xml`

```diff
@@ -1,236 +1,239 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.2.7" timestamp="1686647397983" lines-valid="217" lines-covered="214" line-rate="0.9862" branches-valid="98" branches-covered="98" branch-rate="1" complexity="0">
-  <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.2.7 -->
+<coverage version="7.4.4" timestamp="1712820460896" lines-valid="220" lines-covered="217" line-rate="0.9864" branches-valid="100" branches-covered="100" branch-rate="1" complexity="0">
+  <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.4.4 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/abompard/Fedora/apps/datanommer/datanommer.models/datanommer</source>
   </sources>
   <packages>
-    <package name="models" line-rate="0.9862" branch-rate="1" complexity="0">
+    <package name="models" line-rate="0.9864" branch-rate="1" complexity="0">
       <classes>
-        <class name="__init__.py" filename="models/__init__.py" complexity="0" line-rate="0.9862" branch-rate="1">
+        <class name="__init__.py" filename="models/__init__.py" complexity="0" line-rate="0.9864" branch-rate="1">
           <methods/>
           <lines>
             <line number="16" hits="1"/>
             <line number="17" hits="1"/>
             <line number="18" hits="1"/>
             <line number="19" hits="1"/>
             <line number="20" hits="1"/>
             <line number="21" hits="1"/>
             <line number="22" hits="1"/>
-            <line number="24" hits="1"/>
+            <line number="23" hits="1"/>
             <line number="25" hits="1"/>
-            <line number="44" hits="1"/>
-            <line number="45" hits="1"/>
-            <line number="46" hits="1"/>
-            <line number="53" hits="1"/>
+            <line number="47" hits="1"/>
+            <line number="48" hits="1"/>
+            <line number="49" hits="1"/>
             <line number="56" hits="1"/>
-            <line number="57" hits="1"/>
-            <line number="64" hits="1"/>
-            <line number="66" hits="1"/>
+            <line number="59" hits="1"/>
+            <line number="60" hits="1"/>
             <line number="67" hits="1"/>
-            <line number="69" hits="1"/>
             <line number="70" hits="1"/>
+            <line number="72" hits="1"/>
             <line number="73" hits="1"/>
-            <line number="76" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="77" hits="1"/>
-            <line number="79" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="80" hits="1"/>
+            <line number="75" hits="1"/>
+            <line number="76" hits="1"/>
+            <line number="79" hits="1"/>
             <line number="82" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="83" hits="1"/>
+            <line number="85" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="86" hits="1"/>
             <line number="88" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="89" hits="1"/>
-            <line number="90" hits="1"/>
-            <line number="91" hits="1"/>
-            <line number="93" hits="1"/>
-            <line number="94" hits="1"/>
-            <line number="96" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="94" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="95" hits="1"/>
+            <line number="96" hits="1"/>
             <line number="97" hits="1"/>
-            <line number="98" hits="1"/>
-            <line number="109" hits="1"/>
-            <line number="113" hits="1"/>
-            <line number="114" hits="1"/>
-            <line number="116" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="119" hits="1"/>
+            <line number="99" hits="1"/>
+            <line number="100" hits="1"/>
+            <line number="102" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="103" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="104" hits="1"/>
+            <line number="105" hits="1"/>
+            <line number="116" hits="1"/>
             <line number="120" hits="1"/>
             <line number="121" hits="1"/>
-            <line number="122" hits="1"/>
-            <line number="123" hits="1"/>
-            <line number="125" hits="1"/>
+            <line number="123" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="126" hits="1"/>
+            <line number="127" hits="1"/>
             <line number="128" hits="1"/>
             <line number="129" hits="1"/>
-            <line number="130" hits="0"/>
-            <line number="131" hits="0"/>
-            <line number="136" hits="0"/>
-            <line number="137" hits="1"/>
-            <line number="138" hits="1"/>
-            <line number="139" hits="1"/>
-            <line number="140" hits="1"/>
+            <line number="130" hits="1"/>
+            <line number="132" hits="1"/>
+            <line number="135" hits="1"/>
+            <line number="136" hits="1"/>
+            <line number="137" hits="0"/>
+            <line number="138" hits="0"/>
+            <line number="143" hits="0"/>
+            <line number="144" hits="1"/>
             <line number="145" hits="1"/>
+            <line number="146" hits="1"/>
             <line number="147" hits="1"/>
-            <line number="158" hits="1"/>
-            <line number="164" hits="1"/>
-            <line number="167" hits="1"/>
-            <line number="169" hits="1"/>
+            <line number="152" hits="1"/>
+            <line number="154" hits="1"/>
+            <line number="165" hits="1"/>
             <line number="171" hits="1"/>
-            <line number="172" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="173" hits="1"/>
-            <line number="175" hits="1"/>
-            <line number="177" hits="1"/>
-            <line number="178" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="179" hits="1"/>
+            <line number="174" hits="1"/>
+            <line number="176" hits="1"/>
+            <line number="178" hits="1"/>
+            <line number="179" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="180" hits="1"/>
             <line number="182" hits="1"/>
-            <line number="184" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="185" hits="1"/>
+            <line number="184" hits="1"/>
+            <line number="185" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="186" hits="1"/>
             <line number="187" hits="1"/>
-            <line number="190" hits="1"/>
-            <line number="198" hits="1"/>
-            <line number="207" hits="1"/>
-            <line number="208" hits="1"/>
-            <line number="209" hits="1"/>
-            <line number="211" hits="1"/>
-            <line number="212" hits="1"/>
-            <line number="213" hits="1"/>
+            <line number="189" hits="1"/>
+            <line number="191" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="192" hits="1"/>
+            <line number="194" hits="1"/>
+            <line number="197" hits="1"/>
+            <line number="205" hits="1"/>
             <line number="214" hits="1"/>
             <line number="215" hits="1"/>
             <line number="216" hits="1"/>
-            <line number="217" hits="1"/>
             <line number="218" hits="1"/>
             <line number="219" hits="1"/>
             <line number="220" hits="1"/>
             <line number="221" hits="1"/>
-            <line number="222" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="222" hits="1"/>
             <line number="223" hits="1"/>
             <line number="224" hits="1"/>
-            <line number="225" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="234" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="244" hits="1"/>
-            <line number="245" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="225" hits="1"/>
+            <line number="226" hits="1"/>
+            <line number="227" hits="1"/>
+            <line number="228" hits="1"/>
+            <line number="229" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="230" hits="1"/>
+            <line number="231" hits="1"/>
+            <line number="232" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="241" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="251" hits="1"/>
-            <line number="252" hits="1"/>
-            <line number="253" hits="1"/>
-            <line number="254" hits="1"/>
-            <line number="255" hits="1"/>
-            <line number="256" hits="1"/>
-            <line number="257" hits="1"/>
+            <line number="252" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="258" hits="1"/>
             <line number="259" hits="1"/>
-            <line number="260" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="260" hits="1"/>
             <line number="261" hits="1"/>
             <line number="262" hits="1"/>
-            <line number="263" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="263" hits="1"/>
             <line number="264" hits="1"/>
-            <line number="265" hits="1"/>
             <line number="266" hits="1"/>
+            <line number="267" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="268" hits="1"/>
             <line number="269" hits="1"/>
-            <line number="270" hits="1"/>
+            <line number="270" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="271" hits="1"/>
-            <line number="272" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="272" hits="1"/>
             <line number="273" hits="1"/>
-            <line number="279" hits="1"/>
-            <line number="284" hits="1"/>
-            <line number="285" hits="1"/>
-            <line number="287" hits="1"/>
-            <line number="288" hits="1"/>
-            <line number="290" hits="1"/>
-            <line number="291" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="275" hits="1"/>
+            <line number="276" hits="1"/>
+            <line number="277" hits="1"/>
+            <line number="278" hits="1"/>
+            <line number="279" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="280" hits="1"/>
+            <line number="286" hits="1"/>
+            <line number="291" hits="1"/>
             <line number="292" hits="1"/>
-            <line number="293" hits="1"/>
             <line number="294" hits="1"/>
-            <line number="295" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="296" hits="1"/>
+            <line number="295" hits="1"/>
+            <line number="297" hits="1"/>
+            <line number="298" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="299" hits="1"/>
             <line number="300" hits="1"/>
+            <line number="301" hits="1"/>
+            <line number="302" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="303" hits="1"/>
             <line number="307" hits="1"/>
-            <line number="308" hits="1"/>
-            <line number="310" hits="1"/>
-            <line number="311" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="312" hits="1"/>
             <line number="314" hits="1"/>
-            <line number="315" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="332" hits="1"/>
-            <line number="333" hits="1"/>
-            <line number="334" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="335" hits="1"/>
-            <line number="338" hits="1"/>
-            <line number="347" hits="1"/>
-            <line number="348" hits="1"/>
+            <line number="315" hits="1"/>
+            <line number="317" hits="1"/>
+            <line number="318" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="319" hits="1"/>
+            <line number="321" hits="1"/>
+            <line number="322" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="339" hits="1"/>
+            <line number="340" hits="1"/>
+            <line number="341" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="342" hits="1"/>
+            <line number="343" hits="1"/>
+            <line number="352" hits="1"/>
             <line number="353" hits="1"/>
-            <line number="355" hits="1"/>
-            <line number="356" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="408" hits="1"/>
-            <line number="409" hits="1"/>
-            <line number="410" hits="1"/>
-            <line number="411" hits="1"/>
-            <line number="412" hits="1"/>
-            <line number="413" hits="1"/>
+            <line number="359" hits="1"/>
+            <line number="361" hits="1"/>
+            <line number="362" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="414" hits="1"/>
             <line number="415" hits="1"/>
             <line number="416" hits="1"/>
+            <line number="417" hits="1"/>
             <line number="418" hits="1"/>
-            <line number="422" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="423" hits="1"/>
-            <line number="428" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="429" hits="1"/>
-            <line number="431" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="432" hits="1"/>
-            <line number="435" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="436" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="440" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="419" hits="1"/>
+            <line number="420" hits="1"/>
+            <line number="421" hits="1"/>
+            <line number="422" hits="1"/>
+            <line number="424" hits="1"/>
+            <line number="425" hits="1"/>
+            <line number="429" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="430" hits="1"/>
+            <line number="434" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="435" hits="1"/>
+            <line number="437" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="438" hits="1"/>
             <line number="441" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="442" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="444" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="445" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="446" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="447" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="448" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="450" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="451" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="453" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="454" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="459" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="457" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="458" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="460" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="464" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="461" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="465" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="466" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="468" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="469" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="470" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="474" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="472" hits="1"/>
+            <line number="473" hits="1"/>
             <line number="475" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="480" hits="1"/>
-            <line number="481" hits="1"/>
-            <line number="483" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="484" hits="1"/>
+            <line number="476" hits="1"/>
+            <line number="478" hits="1"/>
+            <line number="479" hits="1"/>
+            <line number="481" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="482" hits="1"/>
+            <line number="485" hits="1"/>
             <line number="486" hits="1"/>
-            <line number="487" hits="1"/>
-            <line number="489" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="489" hits="1"/>
             <line number="490" hits="1"/>
+            <line number="491" hits="1"/>
             <line number="493" hits="1"/>
-            <line number="494" hits="1"/>
-            <line number="497" hits="1"/>
-            <line number="498" hits="1"/>
-            <line number="499" hits="1"/>
-            <line number="501" hits="1"/>
-            <line number="502" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="508" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="511" hits="1"/>
+            <line number="494" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="500" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="503" hits="1"/>
+            <line number="504" hits="1"/>
+            <line number="505" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="506" hits="1"/>
+            <line number="507" hits="1"/>
+            <line number="508" hits="1"/>
+            <line number="509" hits="1"/>
+            <line number="510" hits="1"/>
             <line number="512" hits="1"/>
             <line number="513" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="514" hits="1"/>
-            <line number="515" hits="1"/>
-            <line number="516" hits="1"/>
             <line number="517" hits="1"/>
             <line number="518" hits="1"/>
-            <line number="520" hits="1"/>
-            <line number="521" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="519" hits="1"/>
             <line number="522" hits="1"/>
-            <line number="525" hits="1"/>
-            <line number="526" hits="1"/>
+            <line number="523" hits="1"/>
+            <line number="524" hits="1"/>
             <line number="527" hits="1"/>
-            <line number="530" hits="1"/>
-            <line number="531" hits="1"/>
-            <line number="532" hits="1"/>
+            <line number="528" hits="1"/>
             <line number="535" hits="1"/>
-            <line number="536" hits="1"/>
-            <line number="543" hits="1"/>
           </lines>
         </class>
       </classes>
     </package>
   </packages>
 </coverage>
```

### Comparing `datanommer_models-1.1.0/datanommer/models/__init__.py` & `datanommer_models-1.2.0/datanommer/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
+import importlib.metadata
 import json
 import logging
 import math
 import traceback
 import uuid
 from warnings import warn
 
-import pkg_resources
 from sqlalchemy import (
     and_,
     between,
     Column,
     create_engine,
     DateTime,
     DDL,
     event,
     ForeignKey,
+    func,
     Integer,
     not_,
     or_,
+    select,
     String,
     Table,
     text,
     TypeDecorator,
     Unicode,
     UnicodeText,
     UniqueConstraint,
@@ -58,14 +60,17 @@
     from psycopg2.errors import UniqueViolation
 except ImportError:  # pragma: no cover
     from psycopg2.errorcodes import lookup as lookup_error
 
     UniqueViolation = lookup_error("23505")
 
 
+__version__ = importlib.metadata.version("datanommer.models")
+
+
 log = logging.getLogger("datanommer")
 
 maker = sessionmaker()
 session = scoped_session(maker)
 
 DeclarativeBase = declarative_base()
 DeclarativeBase.query = session.query_property()
@@ -77,29 +82,30 @@
     if uri and engine:
         raise ValueError("uri and engine cannot both be specified")
 
     if uri is None and not engine:
         raise ValueError("One of uri or engine must be specified")
 
     if uri and not engine:
-        engine = create_engine(uri)
+        engine = create_engine(uri, future=True)
 
     # We need to hang our own attribute on the sqlalchemy session to stop
     # ourselves from initializing twice.  That is only a problem if the code
     # calling us isn't consistent.
     if getattr(session, "_datanommer_initialized", None):
         log.warning("Session already initialized.  Bailing")
         return
     session._datanommer_initialized = True
 
-    session.configure(bind=engine)
+    maker.configure(bind=engine)
     DeclarativeBase.query = session.query_property()
 
     if create:
-        session.execute(text("CREATE EXTENSION IF NOT EXISTS timescaledb"))
+        with engine.begin() as connection:
+            connection.execute(text("CREATE EXTENSION IF NOT EXISTS timescaledb"))
         DeclarativeBase.metadata.create_all(engine)
         # Loads the alembic configuration and generates the version table, with
         # the most recent revision stamped as head
         if alembic_ini is not None:  # pragma: no cover
             from alembic import command
             from alembic.config import Config
 
@@ -119,15 +125,15 @@
         # https://discuss.python.org/t/parse-z-timezone-suffix-in-datetime/2220
         try:
             sent_at = datetime.datetime.fromisoformat(sent_at.replace("Z", "+00:00"))
         except ValueError:
             log.exception("Failed to parse sent-at timestamp value")
             return
     else:
-        sent_at = datetime.datetime.utcnow()
+        sent_at = datetime.datetime.now(tz=datetime.timezone.utc)
 
     # Workaround schemas misbehaving
     try:
         usernames = message.usernames
     except Exception:
         log.exception(
             "Could not get the list of users from a message on %s with id %s",
@@ -306,15 +312,15 @@
                 }
             )
         session.execute(assoc_table.insert(), insert_values)
         session.flush()
 
     @classmethod
     def from_msg_id(cls, msg_id):
-        return cls.query.filter(cls.msg_id == msg_id).first()
+        return session.execute(select(cls).where(cls.msg_id == msg_id)).scalar_one_or_none()
 
     def as_dict(self, request=None):
         return dict(
             i=self.i,
             msg_id=self.msg_id,
             topic=self.topic,
             timestamp=self.timestamp,
@@ -329,31 +335,30 @@
             users=list(sorted(u.name for u in self.users)),
             packages=list(sorted(p.name for p in self.packages)),
         )
 
     def as_fedora_message_dict(self):
         headers = self.headers or {}
         if "sent-at" not in headers:
-            headers["sent-at"] = self.timestamp.astimezone(
-                datetime.timezone.utc
-            ).isoformat()
+            headers["sent-at"] = self.timestamp.astimezone(datetime.timezone.utc).isoformat()
         return dict(
             body=self.msg,
             headers=headers,
             id=self.msg_id,
             priority=headers.get("priority", 0),
             queue=None,
             topic=self.topic,
         )
 
     def __json__(self, request=None):
         warn(
             "The __json__() method has been renamed to as_dict(), and will be removed "
             "in the next major version",
             DeprecationWarning,
+            stacklevel=2,
         )
         return self.as_dict(request)
 
     @classmethod
     def grep(
         cls,
         start=None,
@@ -412,90 +417,76 @@
         not_packs = not_packages or []
         categories = categories or []
         not_cats = not_categories or []
         topics = topics or []
         not_topics = not_topics or []
         contains = contains or []
 
-        query = Message.query
+        Message = cls
+        query = select(Message)
 
         # A little argument validation.  We could provide some defaults in
         # these mixed cases.. but instead we'll just leave it up to our caller.
         if (start is not None and end is None) or (end is not None and start is None):
             raise ValueError(
-                "Either both start and end must be specified "
-                "or neither must be specified"
+                "Either both start and end must be specified or neither must be specified"
             )
 
         if start and end:
-            query = query.filter(between(Message.timestamp, start, end))
+            query = query.where(between(Message.timestamp, start, end))
 
         if msg_id:
-            query = query.filter(Message.msg_id == msg_id)
+            query = query.where(Message.msg_id == msg_id)
 
         # Add the four positive filters as necessary
         if users:
-            query = query.filter(
-                or_(*(Message.users.any(User.name == u) for u in users))
-            )
+            query = query.where(or_(*(Message.users.any(User.name == u) for u in users)))
 
         if packages:
-            query = query.filter(
-                or_(*(Message.packages.any(Package.name == p) for p in packages))
-            )
+            query = query.where(or_(*(Message.packages.any(Package.name == p) for p in packages)))
 
         if categories:
-            query = query.filter(
-                or_(*(Message.category == category for category in categories))
-            )
+            query = query.where(or_(*(Message.category == category for category in categories)))
 
         if topics:
-            query = query.filter(or_(*(Message.topic == topic for topic in topics)))
+            query = query.where(or_(*(Message.topic == topic for topic in topics)))
 
         if contains:
-            query = query.filter(
-                or_(*(Message.msg.like(f"%{contain}%") for contain in contains))
-            )
+            query = query.where(or_(*(Message.msg.like(f"%{contain}%") for contain in contains)))
 
         # And then the four negative filters as necessary
         if not_users:
-            query = query.filter(
-                not_(or_(*(Message.users.any(User.name == u) for u in not_users)))
-            )
+            query = query.where(not_(or_(*(Message.users.any(User.name == u) for u in not_users))))
 
         if not_packs:
-            query = query.filter(
+            query = query.where(
                 not_(or_(*(Message.packages.any(Package.name == p) for p in not_packs)))
             )
 
         if not_cats:
-            query = query.filter(
-                not_(or_(*(Message.category == category for category in not_cats)))
-            )
+            query = query.where(not_(or_(*(Message.category == category for category in not_cats))))
 
         if not_topics:
-            query = query.filter(
-                not_(or_(*(Message.topic == topic for topic in not_topics)))
-            )
+            query = query.where(not_(or_(*(Message.topic == topic for topic in not_topics))))
 
         # Finally, tag on our pagination arguments
-        total = query.count()
+        total = session.scalar(query.with_only_columns(func.count(Message.id)))
         query = query.order_by(getattr(Message.timestamp, order)())
 
         if not rows_per_page:
             pages = 1
         else:
             pages = int(math.ceil(total / float(rows_per_page)))
             query = query.offset(rows_per_page * (page - 1)).limit(rows_per_page)
 
         if defer:
             return total, page, query
         else:
             # Execute!
-            messages = query.all()
+            messages = session.scalars(query).all()
             return total, pages, messages
 
 
 class NamedSingleton:
     id = Column(Integer, primary_key=True, autoincrement=True)
     name = Column(UnicodeText, index=True, unique=True)
 
@@ -505,16 +496,16 @@
         Return the instance of the class with the specified name. If it doesn't
         already exist, create it.
         """
         # Use an in-memory cache to speed things up.
         if name in cls._cache:
             # If we cache the instance, SQLAlchemy will run this query anyway because the instance
             # will be from a different transaction. So just cache the id.
-            return cls.query.get(cls._cache[name])
-        obj = cls.query.filter_by(name=name).one_or_none()
+            return session.get(cls, cls._cache[name])
+        obj = session.execute(select(cls).where(cls.name == name)).scalar_one_or_none()
         if obj is None:
             obj = cls(name=name)
             session.add(obj)
             session.flush()
         cls._cache[name] = obj.id
         return obj
 
@@ -538,20 +529,7 @@
         table_class.__table__,
         "after_create",
         DDL(f"SELECT create_hypertable('{table_class.__tablename__}', 'timestamp');"),
     )
 
 
 _setup_hypertable(Message)
-
-
-# Set the version
-try:  # pragma: no cover
-    import importlib.metadata
-
-    __version__ = importlib.metadata.version("datanommer.models")
-except ImportError:  # pragma: no cover
-    try:
-        __version__ = pkg_resources.get_distribution("datanommer.models").version
-    except pkg_resources.DistributionNotFound:
-        # The app is not installed, but the flask dev server can run it nonetheless.
-        __version__ = None
```

### Comparing `datanommer_models-1.1.0/datanommer/models/alembic/env.py` & `datanommer_models-1.2.0/datanommer/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.1.0/datanommer/models/alembic/versions/951c40020acc_unique.py` & `datanommer_models-1.2.0/datanommer/models/alembic/versions/951c40020acc_unique.py`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.1.0/pyproject.toml` & `datanommer_models-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datanommer.models"
-version = "1.1.0"
+version = "1.2.0"
 description = "SQLAlchemy models for datanommer"
 authors = [
   "Fedora Infrastructure <admin@fedoraproject.org>"
 ]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/fedora-infra/datanommer"
@@ -21,114 +21,90 @@
     { path = "*.rst", format = "sdist" },
     { path = "*.xml", format = "sdist" },
     { path = "tests/*", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-SQLAlchemy = "^1.3.24"
+SQLAlchemy = "^1.3.24 || ^2.0.0"
 alembic = "^1.6.5"
 psycopg2 = "^2.9.1"
 fedora-messaging = ">=2.1.0"
+
+# Message schemas. The reference list of all message schemas is in
+# https://github.com/fedora-infra/fedora-messaging/blob/develop/docs/schema-packages.txt
 anitya-schema = {version = "*", optional = true}
 bodhi-messages = {version = "*", optional = true}
+bugzilla2fedmsg-schema = {version = "*", optional = true}
 ci-messages = {version = "*", optional = true}
 copr-messaging = {version = "*", optional = true}
 discourse2fedmsg-messages = {version = "*", optional = true}
 fedocal-messages = {version = "*", optional = true}
 fedorainfra-ansible-messages = {version = "*", optional = true}
 fedora-elections-messages = {version = "*", optional = true}
+fedora-messaging-git-hook-messages = {version = "*", optional = true}
 fedora-messaging-the-new-hotness-schema = {version = "*", optional = true}
 fedora-planet-messages = {version = "*", optional = true}
+fmn-messages = {version = "*", optional = true}
+kerneltest-messages = {version = "^1.0.0", optional = true}
 koji-fedoramessaging-messages = {version = "^1.2.2", optional = true}
+koschei-messages = {version = "*", optional = true}
+mediawiki-messages = {version = "*", optional = true}
+meetbot-messages = {version = "*", optional = true}
 mdapi-messages = {version = "*", optional = true}
 noggin-messages = {version = "*", optional = true}
 nuancier-messages = {version = "*", optional = true}
 pagure-messages = {version = "*", optional = true}
+tahrir-messages = {version = "*", optional = true}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 black = "*"
-isort = "*"
-flake8 = "*"
+ruff = "*"
 pytest = "*"
 liccheck = "*"
 pytest-cov = "*"
 pytest-postgresql = "*"
 pytest-mock = "*"
 bodhi-messages = "*"
 towncrier = "*"
 
 [tool.poetry.extras]
 schemas = [
   "anitya-schema",
   "bodhi-messages",
+  "bugzilla2fedmsg-schema",
   "ci-messages",
   "copr-messaging",
   "discourse2fedmsg-messages",
   "fedocal-messages",
   "fedorainfra-ansible-messages",
   "fedora-elections-messages",
+  "fedora-messaging-git-hook-messages",
   "fedora-messaging-the-new-hotness-schema",
   "fedora-planet-messages",
+  "fmn-messages",
+  "kerneltest-messages",
   "koji-fedoramessaging-messages",
+  "koschei-messages",
+  "mediawiki-messages",
+  "meetbot-messages",
   "mdapi-messages",
   "noggin-messages",
   "nuancier-messages",
   "pagure-messages",
+  "tahrir-messages",
 ]
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
-[tool.liccheck]
-authorized_licenses = [
-  "bsd",
-  "new bsd",
-  "simplified bsd",
-  "apache",
-  "apache 2.0",
-  "apache software",
-  "Apache License 2.0",
-  "Apache License, Version 2.0",
-  "gnu lgpl",
-  "gpl v2",
-  "GNU General Public License v2 or later (GPLv2+)",
-  "GNU General Public License v3 (GPLv3)",
-  "GNU General Public License v3 or later (GPLv3+)",
-  "GNU Library or Lesser General Public License (LGPL)",
-  "GNU Lesser General Public License v2 or later (LGPLv2+)",
-  "GNU Lesser General Public License v3 (LGPLv3)",
-  "GNU Lesser General Public License v3 or later (LGPLv3+)",
-  "GPLv3+",
-  "LGPLv2+",
-  "gpl v3",
-  "lgpl with exceptions or zpl",
-  "isc",
-  "isc license (iscl)",
-  "mit",
-  "python software foundation",
-  "zpl 2.1",
-  "mpl-2.0",
-  "MPL 2.0",
-  "Mozilla Public License 2.0 (MPL 2.0)",
-  "lgpl",
-  "CC0 (copyright waived)",
-  "Public Domain",
-  "Public Domain <http://unlicense.org>",
-  "Zope Public",
-  "The Unlicense (Unlicense)",
-]
-
-[tool.liccheck.authorized_packages]
-twisted = "23.8.0"
-
-
 [tool.towncrier]
 package = "datanommer.models"
 directory = "news/"
 title_format = "v{version}"
 issue_format = "{issue}"
 template = "../tools/towncrier/template.rst.j2"
 underlines = "=^-"
```

### Comparing `datanommer_models-1.1.0/tests/test_jsonencodeddict.py` & `datanommer_models-1.2.0/tests/test_jsonencodeddict.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import pytest
-from sqlalchemy import Column, create_engine, Integer, MetaData, Table
-from sqlalchemy.sql import select
+from sqlalchemy import Column, create_engine, Integer, MetaData, select, Table, text
 
 from datanommer.models import JSONEncodedDict
 
 
 @pytest.fixture
 def connection():
-    engine = create_engine("sqlite:///:memory:")
+    engine = create_engine("sqlite:///:memory:", future=True)
     with engine.connect() as connection:
         yield connection
 
 
 @pytest.fixture
 def table(connection):
     metadata = MetaData()
@@ -25,37 +24,33 @@
     yield table
     metadata.drop_all(connection)
 
 
 def test_jsonencodeddict(connection, table):
     connection.execute(table.insert().values(data={"foo": "bar"}))
     # Check that it's stored as a string
-    for row in connection.execute("SELECT data FROM test_table"):
-        assert row["data"] == '{"foo": "bar"}'
+    for row in connection.execute(text("SELECT data FROM test_table")):
+        assert row.data == '{"foo": "bar"}'
     # Check that SQLAlchemy retrieves it as a dict
     for row in connection.execute(select(table.c.data)):
-        assert row["data"] == {"foo": "bar"}
+        assert row.data == {"foo": "bar"}
 
 
 def test_jsonencodeddict_null(connection, table):
     # Make sure NULL values are supported
     connection.execute(table.insert().values(data=None))
     for row in connection.execute(select(table.c.data)):
-        assert row["data"] is None
+        assert row.data is None
 
 
 def test_jsonencodeddict_compare(connection, table):
     # Make sure NULL values are supported
     connection.execute(table.insert().values(data={"foo": "bar"}))
-    for row in connection.execute(
-        select(table.c.data).filter(table.c.data == {"foo": "bar"})
-    ):
-        assert row["data"] == {"foo": "bar"}
+    for row in connection.execute(select(table.c.data).where(table.c.data == {"foo": "bar"})):
+        assert row.data == {"foo": "bar"}
 
 
 def test_jsonencodeddict_compare_like(connection, table):
     # Make sure NULL values are supported
     connection.execute(table.insert().values(data={"foo": "bar"}))
-    for row in connection.execute(
-        select(table.c.data).filter(table.c.data.like("%foo%"))
-    ):
-        assert row["data"] == {"foo": "bar"}
+    for row in connection.execute(select(table.c.data).where(table.c.data.like("%foo%"))):
+        assert row.data == {"foo": "bar"}
```

### Comparing `datanommer_models-1.1.0/tests/test_model.py` & `datanommer_models-1.2.0/tests/test_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 import datetime
 import json
 import logging
 
 import pytest
 from bodhi.messages.schemas.update import UpdateCommentV1
 from fedora_messaging import message as fedora_message
-from sqlalchemy import create_engine
+from sqlalchemy import create_engine, func, select
 from sqlalchemy.exc import IntegrityError
-from sqlalchemy.orm.query import Query
+from sqlalchemy.sql.selectable import Select
 
-from datanommer.models import add, init, Message, Package, session, User
+import datanommer.models as dm
 
 
 def generate_message(
     topic="org.fedoraproject.test.a.nice.message",
-    body={"encouragement": "You're doing great!"},
+    body=None,
     headers=None,
 ):
+    body = body or {"encouragement": "You're doing great!"}
     return fedora_message.Message(topic=topic, body=body, headers=headers)
 
 
 def generate_bodhi_update_complete_message(text="testing testing"):
     msg = UpdateCommentV1(
         body={
             "comment": {
@@ -59,433 +60,435 @@
     )
     msg.topic = f"org.fedoraproject.stg.{msg.topic}"
     return msg
 
 
 def test_init_uri_and_engine():
     uri = "sqlite:///db.db"
-    engine = create_engine(uri)
+    engine = create_engine(uri, future=True)
 
     with pytest.raises(ValueError, match="uri and engine cannot both be specified"):
-        init(uri, engine=engine)
+        dm.init(uri, engine=engine)
 
 
 def test_init_no_uri_and_no_engine():
     with pytest.raises(ValueError, match="One of uri or engine must be specified"):
-        init()
+        dm.init()
 
 
 def test_init_with_engine(caplog):
     uri = "sqlite:///db.db"
-    engine = create_engine(uri)
+    engine = create_engine(uri, future=True)
 
-    init(engine=engine)
+    dm.init(engine=engine)
 
     assert not caplog.records
 
     # if the init with just the engine worked, trying it again will fail
-    init(engine=engine)
+    dm.init(engine=engine)
     assert caplog.records[0].message == "Session already initialized.  Bailing"
 
 
 def test_init_no_init_twice(datanommer_models, mocker, caplog):
-    init("sqlite:///db.db")
+    dm.init("sqlite:///db.db")
     assert caplog.records[0].message == "Session already initialized.  Bailing"
 
 
 def test_unclassified_category(datanommer_models):
     example_message = generate_message(topic="too.short")
-    add(example_message)
-    dbmsg = Message.query.first()
+    dm.add(example_message)
+    dbmsg = dm.session.scalar(select(dm.Message))
 
     assert dbmsg.category == "Unclassified"
 
 
 def test_from_msg_id(datanommer_models):
     example_message = generate_message()
     example_message.id = "ACUSTOMMESSAGEID"
-    add(example_message)
-    dbmsg = Message.from_msg_id("ACUSTOMMESSAGEID")
+    dm.add(example_message)
+    dbmsg = dm.Message.from_msg_id("ACUSTOMMESSAGEID")
 
     assert dbmsg.msg_id == "ACUSTOMMESSAGEID"
 
 
 def test_add_missing_msg_id(datanommer_models, caplog):
     caplog.set_level(logging.INFO)
     example_message = generate_message()
     example_message._properties.message_id = None
-    add(example_message)
-    dbmsg = Message.query.first()
+    dm.add(example_message)
+    dbmsg = dm.session.scalar(select(dm.Message))
     assert (
         "Message on org.fedoraproject.test.a.nice.message was received without a msg_id"
         in caplog.records[-1].message
     )
     assert dbmsg.msg_id is not None
 
 
 def test_add_missing_timestamp(datanommer_models):
     example_message = generate_message()
     example_message._properties.headers["sent-at"] = None
 
-    add(example_message)
+    dm.add(example_message)
 
-    dbmsg = Message.query.first()
-    timediff = datetime.datetime.utcnow() - dbmsg.timestamp
+    dbmsg = dm.session.scalar(select(dm.Message))
+    timediff = datetime.datetime.now() - dbmsg.timestamp
     # 10 seconds between adding the message and checking
     # the timestamp should be more than enough.
     assert timediff < datetime.timedelta(seconds=10)
 
 
 def test_add_timestamp_with_Z(datanommer_models):
     example_message = generate_message()
     example_message._properties.headers["sent-at"] = "2021-07-27T04:22:42Z"
 
-    add(example_message)
+    dm.add(example_message)
 
-    dbmsg = Message.query.first()
+    dbmsg = dm.session.scalar(select(dm.Message))
     assert dbmsg.timestamp.astimezone(datetime.timezone.utc) == datetime.datetime(
         2021, 7, 27, 4, 22, 42, tzinfo=datetime.timezone.utc
     )
 
 
 def test_add_timestamp_with_junk(datanommer_models, caplog):
     example_message = generate_message()
     example_message._properties.headers["sent-at"] = "2021-07-27T04:22:42JUNK"
 
-    add(example_message)
+    dm.add(example_message)
 
     assert "Failed to parse sent-at timestamp value" in caplog.records[0].message
 
-    assert Message.query.count() == 0
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 0
 
 
 def test_add_and_check_for_others(datanommer_models):
     # There are no users or packages at the start
-    assert User.query.count() == 0
-    assert Package.query.count() == 0
+    assert dm.session.scalar(select(func.count(dm.User.id))) == 0
+    assert dm.session.scalar(select(func.count(dm.Package.id))) == 0
 
     # Then add a message
-    add(generate_bodhi_update_complete_message())
+    dm.add(generate_bodhi_update_complete_message())
 
     # There should now be two of each
-    assert User.query.count() == 2
-    assert Package.query.count() == 2
+    assert dm.session.scalar(select(func.count(dm.User.id))) == 2
+    assert dm.session.scalar(select(func.count(dm.Package.id))) == 2
 
     # If we add it again, there should be no duplicates
-    add(generate_bodhi_update_complete_message())
-    assert User.query.count() == 2
-    assert Package.query.count() == 2
+    dm.add(generate_bodhi_update_complete_message())
+    assert dm.session.scalar(select(func.count(dm.User.id))) == 2
+    assert dm.session.scalar(select(func.count(dm.Package.id))) == 2
 
     # Add a new username
-    add(generate_bodhi_update_complete_message(text="this is @abompard in a comment"))
-    assert User.query.count() == 3
-    assert Package.query.count() == 2
+    dm.add(generate_bodhi_update_complete_message(text="this is @abompard in a comment"))
+    assert dm.session.scalar(select(func.count(dm.User.id))) == 3
+    assert dm.session.scalar(select(func.count(dm.Package.id))) == 2
 
 
 def test_add_nothing(datanommer_models):
-    assert Message.query.count() == 0
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 0
 
 
 def test_add_and_check(datanommer_models):
-    add(generate_message())
-    session.flush()
-    assert Message.query.count() == 1
+    dm.add(generate_message())
+    dm.session.flush()
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
 
 
 def test_categories(datanommer_models):
-    add(generate_bodhi_update_complete_message())
-    session.flush()
-    obj = Message.query.first()
+    dm.add(generate_bodhi_update_complete_message())
+    dm.session.flush()
+    obj = dm.session.scalar(select(dm.Message))
     assert obj.category == "bodhi"
 
 
 def test_categories_with_umb(datanommer_models):
-    add(generate_message(topic="/topic/VirtualTopic.eng.brew.task.closed"))
-    session.flush()
-    obj = Message.query.first()
+    dm.add(generate_message(topic="/topic/VirtualTopic.eng.brew.task.closed"))
+    dm.session.flush()
+    obj = dm.session.scalar(select(dm.Message))
     assert obj.category == "brew"
 
 
 def test_grep_all(datanommer_models):
     example_message = generate_message()
-    add(example_message)
-    session.flush()
-    t, p, r = Message.grep()
+    print("example message:", repr(example_message))
+    print(repr(example_message.body))
+    dm.add(example_message)
+    dm.session.flush()
+    t, p, r = dm.Message.grep()
     assert t == 1
     assert p == 1
     assert len(r) == 1
+    print(repr(r))
     assert r[0].msg == example_message.body
 
 
 def test_grep_category(datanommer_models):
     example_message = generate_message(topic="org.fedoraproject.prod.bodhi.newupdate")
-    add(example_message)
-    session.flush()
-    t, p, r = Message.grep(categories=["bodhi"])
+    dm.add(example_message)
+    dm.session.flush()
+    t, p, r = dm.Message.grep(categories=["bodhi"])
     assert t == 1
     assert p == 1
     assert len(r) == 1
     assert r[0].msg == example_message.body
 
 
 def test_grep_not_category(datanommer_models):
     example_message = generate_message(topic="org.fedoraproject.prod.bodhi.newupdate")
-    add(example_message)
-    session.flush()
-    t, p, r = Message.grep(not_categories=["bodhi"])
+    dm.add(example_message)
+    dm.session.flush()
+    t, p, r = dm.Message.grep(not_categories=["bodhi"])
     assert t == 0
     assert p == 0
     assert len(r) == 0
 
 
 def test_add_headers(datanommer_models):
     example_headers = {"foo": "bar", "baz": 1, "wibble": ["zork", "zap"]}
     example_message = generate_message(
         topic="org.fedoraproject.prod.bodhi.newupdate", headers=example_headers
     )
-    add(example_message)
-    dbmsg = Message.query.first()
+    dm.add(example_message)
+    dbmsg = dm.session.scalar(select(dm.Message))
     assert dbmsg.headers["foo"] == "bar"
     assert dbmsg.headers["baz"] == 1
     assert dbmsg.headers["wibble"] == ["zork", "zap"]
 
 
 def test_grep_topics(datanommer_models):
     example_message = generate_message(topic="org.fedoraproject.prod.bodhi.newupdate")
-    add(example_message)
-    session.flush()
-    t, p, r = Message.grep(topics=["org.fedoraproject.prod.bodhi.newupdate"])
+    dm.add(example_message)
+    dm.session.flush()
+    t, p, r = dm.Message.grep(topics=["org.fedoraproject.prod.bodhi.newupdate"])
     assert t == 1
     assert p == 1
     assert len(r) == 1
     assert r[0].msg == example_message.body
 
 
 def test_grep_not_topics(datanommer_models):
     example_message = generate_message(topic="org.fedoraproject.prod.bodhi.newupdate")
-    add(example_message)
-    session.flush()
-    t, p, r = Message.grep(not_topics=["org.fedoraproject.prod.bodhi.newupdate"])
+    dm.add(example_message)
+    dm.session.flush()
+    t, p, r = dm.Message.grep(not_topics=["org.fedoraproject.prod.bodhi.newupdate"])
     assert t == 0
     assert p == 0
     assert len(r) == 0
 
 
 def test_grep_start_end_validation(datanommer_models):
     with pytest.raises(
         ValueError,
         match="Either both start and end must be specified or neither must be specified",
     ):
-        Message.grep(start="2020-03-26")
+        dm.Message.grep(start="2020-03-26")
     with pytest.raises(
         ValueError,
         match="Either both start and end must be specified or neither must be specified",
     ):
-        Message.grep(end="2020-03-26")
+        dm.Message.grep(end="2020-03-26")
 
 
 def test_grep_start_end(datanommer_models):
     example_message = generate_message()
     example_message._properties.headers["sent-at"] = "2021-04-01T00:00:01"
-    add(example_message)
+    dm.add(example_message)
 
     bodhi_example_message = generate_bodhi_update_complete_message()
     bodhi_example_message._properties.headers["sent-at"] = "2021-06-01T00:00:01"
-    add(bodhi_example_message)
+    dm.add(bodhi_example_message)
 
-    session.flush()
-    total, pages, messages = Message.grep(start="2021-04-01", end="2021-05-01")
+    dm.session.flush()
+    total, pages, messages = dm.Message.grep(start="2021-04-01", end="2021-05-01")
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
     assert messages[0].msg == example_message.body
 
-    total, pages, messages = Message.grep(start="2021-06-01", end="2021-07-01")
+    total, pages, messages = dm.Message.grep(start="2021-06-01", end="2021-07-01")
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
     assert messages[0].msg == bodhi_example_message.body
 
 
 def test_grep_msg_id(datanommer_models):
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
     bodhi_example_message = generate_bodhi_update_complete_message()
-    add(bodhi_example_message)
+    dm.add(bodhi_example_message)
 
-    session.flush()
-    total, pages, messages = Message.grep(msg_id=example_message.id)
+    dm.session.flush()
+    total, pages, messages = dm.Message.grep(msg_id=example_message.id)
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
     assert messages[0].msg == example_message.body
 
-    total, pages, messages = Message.grep(msg_id=bodhi_example_message.id)
+    total, pages, messages = dm.Message.grep(msg_id=bodhi_example_message.id)
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
     assert messages[0].msg == bodhi_example_message.body
 
-    total, pages, messages = Message.grep(msg_id="NOTAMESSAGEID")
+    total, pages, messages = dm.Message.grep(msg_id="NOTAMESSAGEID")
     assert total == 0
     assert pages == 0
     assert len(messages) == 0
 
 
 def test_grep_users(datanommer_models):
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
     bodhi_example_message = generate_bodhi_update_complete_message()
-    add(bodhi_example_message)
+    dm.add(bodhi_example_message)
 
-    session.flush()
+    dm.session.flush()
 
-    total, pages, messages = Message.grep(users=["dudemcpants"])
+    total, pages, messages = dm.Message.grep(users=["dudemcpants"])
 
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
 
     assert messages[0].msg == bodhi_example_message.body
 
 
 def test_grep_not_users(datanommer_models):
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
     bodhi_example_message = generate_bodhi_update_complete_message()
-    add(bodhi_example_message)
+    dm.add(bodhi_example_message)
 
-    session.flush()
+    dm.session.flush()
 
-    total, pages, messages = Message.grep(not_users=["dudemcpants"])
+    total, pages, messages = dm.Message.grep(not_users=["dudemcpants"])
 
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
 
     assert messages[0].msg == example_message.body
 
 
 def test_grep_packages(datanommer_models):
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
     bodhi_example_message = generate_bodhi_update_complete_message()
-    add(bodhi_example_message)
+    dm.add(bodhi_example_message)
 
-    session.flush()
+    dm.session.flush()
 
-    total, pages, messages = Message.grep(packages=["kernel"])
+    total, pages, messages = dm.Message.grep(packages=["kernel"])
 
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
 
     assert messages[0].msg == bodhi_example_message.body
 
 
 def test_grep_not_packages(datanommer_models):
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
     bodhi_example_message = generate_bodhi_update_complete_message()
-    add(bodhi_example_message)
+    dm.add(bodhi_example_message)
 
-    session.flush()
+    dm.session.flush()
 
-    total, pages, messages = Message.grep(not_packages=["kernel"])
+    total, pages, messages = dm.Message.grep(not_packages=["kernel"])
 
     assert total == 1
     assert pages == 1
     assert len(messages) == 1
 
     assert messages[0].msg == example_message.body
 
 
 def test_grep_contains(datanommer_models):
     example_message = generate_message(topic="org.fedoraproject.prod.bodhi.newupdate")
-    add(example_message)
-    session.flush()
-    t, p, r = Message.grep(contains=["doing"])
+    dm.add(example_message)
+    dm.session.flush()
+    t, p, r = dm.Message.grep(contains=["doing"])
     assert t == 1
     assert p == 1
     assert len(r) == 1
     assert r[0].msg == example_message.body
 
 
 def test_grep_rows_per_page_none(datanommer_models):
     for x in range(0, 200):
         example_message = generate_message()
         example_message.id = f"{x}"
-        add(example_message)
+        dm.add(example_message)
 
-    session.flush()
+    dm.session.flush()
 
-    total, pages, messages = Message.grep()
+    total, pages, messages = dm.Message.grep()
     assert total == 200
     assert pages == 2
     assert len(messages) == 100
 
-    total, pages, messages = Message.grep(rows_per_page=None)
+    total, pages, messages = dm.Message.grep(rows_per_page=None)
     assert total == 200
     assert pages == 1
     assert len(messages) == 200
 
 
 def test_grep_rows_per_page_zero(datanommer_models):
     for x in range(0, 200):
         example_message = generate_message()
         example_message.id = f"{x}"
-        add(example_message)
-    session.flush()
+        dm.add(example_message)
+    dm.session.flush()
 
     try:
-        total, pages, messages = Message.grep(rows_per_page=0)
+        total, pages, messages = dm.Message.grep(rows_per_page=0)
     except ZeroDivisionError as e:
-        assert False, e
+        pytest.fail(e)
     assert total == 200
     assert pages == 1
     assert len(messages) == 200
 
 
 def test_grep_defer(datanommer_models):
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
-    session.flush()
+    dm.session.flush()
 
-    total, pages, query = Message.grep(defer=True)
-    assert isinstance(query, Query)
+    total, pages, query = dm.Message.grep(defer=True)
+    assert isinstance(query, Select)
 
-    assert query.all() == Message.grep()[2]
+    assert dm.session.scalars(query).all() == dm.Message.grep()[2]
 
 
 def test_add_duplicate(datanommer_models, caplog):
     example_message = generate_message()
-    add(example_message)
-    add(example_message)
+    dm.add(example_message)
+    dm.add(example_message)
     # if no exception was thrown, then we successfully ignored the
     # duplicate message
-    assert Message.query.count() == 1
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
     assert (
-        "Skipping message from org.fedoraproject.test.a.nice.message"
-        in caplog.records[0].message
+        "Skipping message from org.fedoraproject.test.a.nice.message" in caplog.records[0].message
     )
 
 
 def test_add_integrity_error(datanommer_models, mocker, caplog):
     mock_session_add = mocker.patch("datanommer.models.session.add")
     mock_session_add.side_effect = IntegrityError("asdf", "asd", "asdas")
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
     assert "Unknown Integrity Error: message" in caplog.records[0].message
-    assert Message.query.count() == 0
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 0
 
 
 def test_add_duplicate_package(datanommer_models):
     # Define a special message schema and register it
     class MessageWithPackages(fedora_message.Message):
         @property
         def packages(self):
@@ -495,19 +498,19 @@
     fedora_message._class_to_schema_name[MessageWithPackages] = "MessageWithPackages"
     example_message = MessageWithPackages(
         topic="org.fedoraproject.test.a.nice.message",
         body={"encouragement": "You're doing great!"},
         headers=None,
     )
     try:
-        add(example_message)
+        dm.add(example_message)
     except IntegrityError as e:
-        assert False, e
-    assert Message.query.count() == 1
-    dbmsg = Message.query.first()
+        pytest.fail(e)
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
+    dbmsg = dm.session.scalar(select(dm.Message))
     assert len(dbmsg.packages) == 1
     assert dbmsg.packages[0].name == "pkg"
 
 
 def test_add_message_with_error_on_packages(datanommer_models, caplog):
     # Define a special message schema and register it
     class CustomMessage(fedora_message.Message):
@@ -522,106 +525,107 @@
     fedora_message._class_to_schema_name[CustomMessage] = "CustomMessage"
     example_message = CustomMessage(
         topic="org.fedoraproject.test.a.nice.message",
         body={"encouragement": "You're doing great!"},
         headers=None,
     )
     try:
-        add(example_message)
+        dm.add(example_message)
     except KeyError as e:
-        assert False, e
-    assert Message.query.count() == 1
+        pytest.fail(e)
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
     assert caplog.records[0].message == (
         f"Could not get the list of packages from a message on "
         f"org.fedoraproject.test.a.nice.message with id {example_message.id}"
     )
 
 
 def test_as_fedora_message_dict(datanommer_models):
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
-    dbmsg = Message.query.first()
+    dbmsg = dm.session.scalar(select(dm.Message))
 
     message_json = json.dumps(dbmsg.as_fedora_message_dict())
 
     # this should be the same as if we use the fedora_messaging dump function
     assert json.loads(fedora_message.dumps(example_message)) == json.loads(message_json)
 
 
 def test_as_fedora_message_dict_old_headers(datanommer_models):
     # Messages received with fedmsg don't have the sent-at header
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
-    dbmsg = Message.query.first()
+    dbmsg = dm.session.scalar(select(dm.Message))
     del dbmsg.headers["sent-at"]
 
     message_dict = dbmsg.as_fedora_message_dict()
     print(message_dict)
     print(json.loads(fedora_message.dumps(example_message)))
 
     # this should be the same as if we use the fedora_messaging dump function
     assert json.loads(fedora_message.dumps(example_message)) == message_dict
 
 
 def test_as_fedora_message_dict_no_headers(datanommer_models):
     # Messages can have no headers
     example_message = generate_message()
-    add(example_message)
+    dm.add(example_message)
 
-    dbmsg = Message.query.first()
+    dbmsg = dm.session.scalar(select(dm.Message))
     assert len(dbmsg.headers.keys()) == 4
 
     # Clear the headers
     dbmsg.headers = None
 
     try:
         message_dict = dbmsg.as_fedora_message_dict()
     except TypeError as e:
-        assert False, e
+        pytest.fail(e)
 
     assert list(message_dict["headers"].keys()) == ["sent-at"]
 
 
 def test_as_dict(datanommer_models):
-    add(generate_message())
-    dbmsg = Message.query.first()
+    dm.add(generate_message())
+    dbmsg = dm.session.scalar(select(dm.Message))
     message_dict = dbmsg.as_dict()
 
     # we should have 14 keys in this dict
     assert len(message_dict) == 14
     assert message_dict["msg"] == {"encouragement": "You're doing great!"}
     assert message_dict["topic"] == "org.fedoraproject.test.a.nice.message"
 
 
 def test_as_dict_with_users_and_packages(datanommer_models):
-    add(generate_bodhi_update_complete_message())
-    dbmsg = Message.query.first()
+    dm.add(generate_bodhi_update_complete_message())
+    dbmsg = dm.session.scalar(select(dm.Message))
     message_dict = dbmsg.as_dict()
 
     assert message_dict["users"] == ["dudemcpants", "ryanlerch"]
     assert message_dict["packages"] == ["abrt-addon-python3", "kernel"]
 
 
 def test___json__deprecated(datanommer_models, caplog, mocker):
     mock_as_dict = mocker.patch("datanommer.models.Message.as_dict")
 
-    add(generate_message())
+    dm.add(generate_message())
 
     with pytest.warns(DeprecationWarning):
-        Message.query.first().__json__()
+        dbmsg = dm.session.scalar(select(dm.Message))
+        dbmsg.__json__()
 
     mock_as_dict.assert_called_once()
 
 
 def test_singleton_create(datanommer_models):
-    Package.get_or_create("foobar")
-    assert [p.name for p in Package.query.all()] == ["foobar"]
+    dm.Package.get_or_create("foobar")
+    assert [p.name for p in dm.session.scalars(select(dm.Package))] == ["foobar"]
 
 
 def test_singleton_get_existing(datanommer_models):
-    p1 = Package.get_or_create("foobar")
+    p1 = dm.Package.get_or_create("foobar")
     # Clear the in-memory cache
-    Package._cache.clear()
-    p2 = Package.get_or_create("foobar")
+    dm.Package._cache.clear()
+    p2 = dm.Package.get_or_create("foobar")
     assert p1.id == p2.id
```

### Comparing `datanommer_models-1.1.0/tox.ini` & `datanommer_models-1.2.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 sitepackages = false
 skip_install = true
 # Use allowlist for poetry when poetry 1.2+ is more widespread
 # allowlist_externals =
 #     poetry
 deps =
     poetry>=1.2
+env =
+    SQLALCHEMY_WARN_20=1
 commands_pre =
     poetry install --all-extras
 commands =
     poetry run pytest -c ../pyproject.toml {posargs}
 
 [testenv:licenses]
 allowlist_externals =
```

### Comparing `datanommer_models-1.1.0/PKG-INFO` & `datanommer_models-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 Metadata-Version: 2.1
-Name: datanommer-models
-Version: 1.1.0
+Name: datanommer.models
+Version: 1.2.0
 Summary: SQLAlchemy models for datanommer
 Home-page: https://github.com/fedora-infra/datanommer
 License: GPL-3.0-or-later
 Author: Fedora Infrastructure
 Author-email: admin@fedoraproject.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: schemas
-Requires-Dist: SQLAlchemy (>=1.3.24,<2.0.0)
+Requires-Dist: SQLAlchemy (>=1.3.24,<3.0.0)
 Requires-Dist: alembic (>=1.6.5,<2.0.0)
 Requires-Dist: anitya-schema ; extra == "schemas"
 Requires-Dist: bodhi-messages ; extra == "schemas"
+Requires-Dist: bugzilla2fedmsg-schema ; extra == "schemas"
 Requires-Dist: ci-messages ; extra == "schemas"
 Requires-Dist: copr-messaging ; extra == "schemas"
 Requires-Dist: discourse2fedmsg-messages ; extra == "schemas"
 Requires-Dist: fedocal-messages ; extra == "schemas"
 Requires-Dist: fedora-elections-messages ; extra == "schemas"
 Requires-Dist: fedora-messaging (>=2.1.0)
+Requires-Dist: fedora-messaging-git-hook-messages ; extra == "schemas"
 Requires-Dist: fedora-messaging-the-new-hotness-schema ; extra == "schemas"
 Requires-Dist: fedora-planet-messages ; extra == "schemas"
 Requires-Dist: fedorainfra-ansible-messages ; extra == "schemas"
+Requires-Dist: fmn-messages ; extra == "schemas"
+Requires-Dist: kerneltest-messages (>=1.0.0,<2.0.0) ; extra == "schemas"
 Requires-Dist: koji-fedoramessaging-messages (>=1.2.2,<2.0.0) ; extra == "schemas"
+Requires-Dist: koschei-messages ; extra == "schemas"
 Requires-Dist: mdapi-messages ; extra == "schemas"
+Requires-Dist: mediawiki-messages ; extra == "schemas"
+Requires-Dist: meetbot-messages ; extra == "schemas"
 Requires-Dist: noggin-messages ; extra == "schemas"
 Requires-Dist: nuancier-messages ; extra == "schemas"
 Requires-Dist: pagure-messages ; extra == "schemas"
 Requires-Dist: psycopg2 (>=2.9.1,<3.0.0)
+Requires-Dist: tahrir-messages ; extra == "schemas"
 Project-URL: Repository, https://github.com/fedora-infra/datanommer
 Description-Content-Type: text/x-rst
 
 datanommer.models
 =================
 
 This package contains the SQLAlchemy data model for datanommer.
```

