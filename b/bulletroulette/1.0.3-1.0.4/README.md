# Comparing `tmp/bulletroulette-1.0.3.tar.gz` & `tmp/bulletroulette-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulletroulette-1.0.3.tar", last modified: Sun Apr 14 03:23:11 2024, max compression
+gzip compressed data, was "bulletroulette-1.0.4.tar", last modified: Mon Apr 15 12:17:48 2024, max compression
```

## Comparing `bulletroulette-1.0.3.tar` & `bulletroulette-1.0.4.tar`

### file list

```diff
@@ -1,71 +1,69 @@
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:23:11.625085 bulletroulette-1.0.3/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-13 02:31:44.000000 bulletroulette-1.0.3/LICENSE
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      183 2024-04-14 03:20:19.000000 bulletroulette-1.0.3/MANIFEST.in
--rw-r--r--   0 gqx       (1000) gqx       (1000)     1944 2024-04-14 03:23:11.625085 bulletroulette-1.0.3/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      934 2024-04-13 11:46:05.000000 bulletroulette-1.0.3/README.md
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:23:11.597086 bulletroulette-1.0.3/bulletroulette/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       98 2024-04-14 00:21:35.000000 bulletroulette-1.0.3/bulletroulette/__init__.py
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:23:11.625085 bulletroulette-1.0.3/bulletroulette/assets/
--rw-------   0 gqx       (1000) gqx       (1000)     4216 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/A.png
--rw-------   0 gqx       (1000) gqx       (1000)     4273 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/B.png
--rw-------   0 gqx       (1000) gqx       (1000)     4252 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/C.png
--rw-------   0 gqx       (1000) gqx       (1000)     4138 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/D.png
--rw-------   0 gqx       (1000) gqx       (1000)     2114 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/DELETE.png
--rw-------   0 gqx       (1000) gqx       (1000)     3620 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/E.png
--rw-------   0 gqx       (1000) gqx       (1000)     2702 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/ENTER.png
--rw-------   0 gqx       (1000) gqx       (1000)     3576 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/F.png
--rw-------   0 gqx       (1000) gqx       (1000)     4297 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/G.png
--rw-------   0 gqx       (1000) gqx       (1000)     3598 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/H.png
--rw-------   0 gqx       (1000) gqx       (1000)     3592 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/I.png
--rw-------   0 gqx       (1000) gqx       (1000)     3790 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/J.png
--rw-------   0 gqx       (1000) gqx       (1000)     4139 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/K.png
--rw-------   0 gqx       (1000) gqx       (1000)     3505 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/L.png
--rw-------   0 gqx       (1000) gqx       (1000)     3964 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/M.png
--rw-------   0 gqx       (1000) gqx       (1000)     4052 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/N.png
--rw-------   0 gqx       (1000) gqx       (1000)     4271 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/O.png
--rw-------   0 gqx       (1000) gqx       (1000)     3931 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/P.png
--rw-------   0 gqx       (1000) gqx       (1000)     4456 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/Q.png
--rw-------   0 gqx       (1000) gqx       (1000)     4171 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/R.png
--rw-------   0 gqx       (1000) gqx       (1000)     4263 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/S.png
--rwx------   0 gqx       (1000) gqx       (1000) 10050868 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/Simhei.ttf
--rw-------   0 gqx       (1000) gqx       (1000)     3701 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/T.png
--rw-------   0 gqx       (1000) gqx       (1000)     3887 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/U.png
--rw-------   0 gqx       (1000) gqx       (1000)     4313 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/V.png
--rw-------   0 gqx       (1000) gqx       (1000)     4535 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/W.png
--rw-------   0 gqx       (1000) gqx       (1000)     4286 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/X.png
--rw-------   0 gqx       (1000) gqx       (1000)     3987 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/Y.png
--rw-------   0 gqx       (1000) gqx       (1000)     3920 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/Z.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      208 2024-04-13 02:21:31.000000 bulletroulette-1.0.3/bulletroulette/assets/__init__.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    25284 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/beer.png
--rwx------   0 gqx       (1000) gqx       (1000)  1526669 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/bg.png
--rwx------   0 gqx       (1000) gqx       (1000)  1107220 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/bgmsc.ogg
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    56254 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/binary.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     6692 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/blank.png
--rwx------   0 gqx       (1000) gqx       (1000)   192078 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/blank.wav
--rwx------   0 gqx       (1000) gqx       (1000)     5494 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/charge.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)   117887 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/dealershootplayer.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    43271 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/dealershootself.png
--rw-------   0 gqx       (1000) gqx       (1000)    97047 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/gun.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    61801 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/handcuff.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    64423 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/knife.png
--rwx------   0 gqx       (1000) gqx       (1000)    96078 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/livedealer.wav
--rwx------   0 gqx       (1000) gqx       (1000)   432078 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/liveplayer.wav
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    12620 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/liveround.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    15499 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/magnifier.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    34020 2024-04-13 01:14:24.000000 bulletroulette-1.0.3/bulletroulette/assets/noneprop.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)   130200 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/pill.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    43256 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/propbox.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    33816 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/smoke.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)   432984 2024-04-09 13:27:21.000000 bulletroulette-1.0.3/bulletroulette/assets/super.png
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1143 2024-04-14 02:40:49.000000 bulletroulette-1.0.3/bulletroulette/data.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     3187 2024-04-14 02:40:51.000000 bulletroulette-1.0.3/bulletroulette/roles.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)    13727 2024-04-14 02:40:53.000000 bulletroulette-1.0.3/bulletroulette/run.py
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1009 2024-04-14 02:41:24.000000 bulletroulette-1.0.3/bulletroulette/sprites.py
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-14 03:23:11.625085 bulletroulette-1.0.3/bulletroulette.egg-info/
--rw-r--r--   0 gqx       (1000) gqx       (1000)     1944 2024-04-14 03:23:11.000000 bulletroulette-1.0.3/bulletroulette.egg-info/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1924 2024-04-14 03:23:11.000000 bulletroulette-1.0.3/bulletroulette.egg-info/SOURCES.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-14 03:23:11.000000 bulletroulette-1.0.3/bulletroulette.egg-info/dependency_links.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       14 2024-04-14 03:23:11.000000 bulletroulette-1.0.3/bulletroulette.egg-info/requires.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       15 2024-04-14 03:23:11.000000 bulletroulette-1.0.3/bulletroulette.egg-info/top_level.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-14 03:23:11.629085 bulletroulette-1.0.3/setup.cfg
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1621 2024-04-14 03:22:53.000000 bulletroulette-1.0.3/setup.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-13 02:31:44.000000 bulletroulette-1.0.4/LICENSE
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)      183 2024-04-14 03:20:19.000000 bulletroulette-1.0.4/MANIFEST.in
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     4173 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     3163 2024-04-14 10:02:38.000000 bulletroulette-1.0.4/README.md
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.604539 bulletroulette-1.0.4/bulletroulette/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       98 2024-04-14 00:21:35.000000 bulletroulette-1.0.4/bulletroulette/__init__.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/bulletroulette/assets/
+-rw-------   0 gqx       (1000) gqx       (1000)     4216 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/A.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4273 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/B.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4252 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/C.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4138 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/D.png
+-rw-------   0 gqx       (1000) gqx       (1000)     2114 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/DELETE.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3620 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/E.png
+-rw-------   0 gqx       (1000) gqx       (1000)     2702 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/ENTER.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3576 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/F.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4297 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/G.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3598 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/H.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3592 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/I.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3790 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/J.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4139 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/K.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3505 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/L.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3964 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/M.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4052 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/N.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4271 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/O.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3931 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/P.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4456 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Q.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4171 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/R.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4263 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/S.png
+-rwx------   0 gqx       (1000) gqx       (1000) 10050868 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Simhei.ttf
+-rw-------   0 gqx       (1000) gqx       (1000)     3701 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/T.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3887 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/U.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4313 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/V.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4535 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/W.png
+-rw-------   0 gqx       (1000) gqx       (1000)     4286 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/X.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3987 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Y.png
+-rw-------   0 gqx       (1000) gqx       (1000)     3920 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/Z.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    25284 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/beer.png
+-rwx------   0 gqx       (1000) gqx       (1000)  1526669 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/bg.png
+-rwx------   0 gqx       (1000) gqx       (1000)  1107220 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/bgmsc.ogg
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     6692 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/blank.png
+-rwx------   0 gqx       (1000) gqx       (1000)   192078 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/blank.wav
+-rwx------   0 gqx       (1000) gqx       (1000)     5494 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/charge.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)   117887 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/dealershootplayer.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    43271 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/dealershootself.png
+-rw-------   0 gqx       (1000) gqx       (1000)    97047 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/gun.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    61801 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/handcuff.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    64423 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/knife.png
+-rwx------   0 gqx       (1000) gqx       (1000)    96078 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/livedealer.wav
+-rwx------   0 gqx       (1000) gqx       (1000)   432078 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/liveplayer.wav
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    12620 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/liveround.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    15499 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/magnifier.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    34020 2024-04-13 01:14:24.000000 bulletroulette-1.0.4/bulletroulette/assets/noneprop.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)   130200 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/pill.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    43256 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/propbox.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    33816 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/smoke.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)   432984 2024-04-09 13:27:21.000000 bulletroulette-1.0.4/bulletroulette/assets/super.png
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1143 2024-04-14 02:40:49.000000 bulletroulette-1.0.4/bulletroulette/data.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     3187 2024-04-14 02:40:51.000000 bulletroulette-1.0.4/bulletroulette/roles.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)    13690 2024-04-14 10:45:40.000000 bulletroulette-1.0.4/bulletroulette/run.py
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1009 2024-04-14 02:41:24.000000 bulletroulette-1.0.4/bulletroulette/sprites.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/bulletroulette.egg-info/
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     4173 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1857 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/SOURCES.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/dependency_links.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       14 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/requires.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       15 2024-04-15 12:17:48.000000 bulletroulette-1.0.4/bulletroulette.egg-info/top_level.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-15 12:17:48.632538 bulletroulette-1.0.4/setup.cfg
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1621 2024-04-15 12:17:41.000000 bulletroulette-1.0.4/setup.py
```

### Comparing `bulletroulette-1.0.3/LICENSE` & `bulletroulette-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/A.png` & `bulletroulette-1.0.4/bulletroulette/assets/A.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/B.png` & `bulletroulette-1.0.4/bulletroulette/assets/B.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/C.png` & `bulletroulette-1.0.4/bulletroulette/assets/C.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/D.png` & `bulletroulette-1.0.4/bulletroulette/assets/D.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/DELETE.png` & `bulletroulette-1.0.4/bulletroulette/assets/DELETE.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/E.png` & `bulletroulette-1.0.4/bulletroulette/assets/E.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/ENTER.png` & `bulletroulette-1.0.4/bulletroulette/assets/ENTER.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/F.png` & `bulletroulette-1.0.4/bulletroulette/assets/F.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/G.png` & `bulletroulette-1.0.4/bulletroulette/assets/G.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/H.png` & `bulletroulette-1.0.4/bulletroulette/assets/H.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/I.png` & `bulletroulette-1.0.4/bulletroulette/assets/I.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/J.png` & `bulletroulette-1.0.4/bulletroulette/assets/J.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/K.png` & `bulletroulette-1.0.4/bulletroulette/assets/K.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/L.png` & `bulletroulette-1.0.4/bulletroulette/assets/L.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/M.png` & `bulletroulette-1.0.4/bulletroulette/assets/M.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/N.png` & `bulletroulette-1.0.4/bulletroulette/assets/N.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/O.png` & `bulletroulette-1.0.4/bulletroulette/assets/O.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/P.png` & `bulletroulette-1.0.4/bulletroulette/assets/P.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/Q.png` & `bulletroulette-1.0.4/bulletroulette/assets/Q.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/R.png` & `bulletroulette-1.0.4/bulletroulette/assets/R.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/S.png` & `bulletroulette-1.0.4/bulletroulette/assets/S.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/Simhei.ttf` & `bulletroulette-1.0.4/bulletroulette/assets/Simhei.ttf`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/T.png` & `bulletroulette-1.0.4/bulletroulette/assets/T.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/U.png` & `bulletroulette-1.0.4/bulletroulette/assets/U.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/V.png` & `bulletroulette-1.0.4/bulletroulette/assets/V.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/W.png` & `bulletroulette-1.0.4/bulletroulette/assets/W.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/X.png` & `bulletroulette-1.0.4/bulletroulette/assets/X.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/Y.png` & `bulletroulette-1.0.4/bulletroulette/assets/Y.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/Z.png` & `bulletroulette-1.0.4/bulletroulette/assets/Z.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/beer.png` & `bulletroulette-1.0.4/bulletroulette/assets/beer.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/bg.png` & `bulletroulette-1.0.4/bulletroulette/assets/bg.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/bgmsc.ogg` & `bulletroulette-1.0.4/bulletroulette/assets/bgmsc.ogg`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/blank.png` & `bulletroulette-1.0.4/bulletroulette/assets/blank.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/blank.wav` & `bulletroulette-1.0.4/bulletroulette/assets/blank.wav`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/charge.png` & `bulletroulette-1.0.4/bulletroulette/assets/charge.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/dealershootplayer.png` & `bulletroulette-1.0.4/bulletroulette/assets/dealershootplayer.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/dealershootself.png` & `bulletroulette-1.0.4/bulletroulette/assets/dealershootself.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/gun.png` & `bulletroulette-1.0.4/bulletroulette/assets/gun.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/handcuff.png` & `bulletroulette-1.0.4/bulletroulette/assets/handcuff.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/knife.png` & `bulletroulette-1.0.4/bulletroulette/assets/knife.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/livedealer.wav` & `bulletroulette-1.0.4/bulletroulette/assets/livedealer.wav`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/liveplayer.wav` & `bulletroulette-1.0.4/bulletroulette/assets/liveplayer.wav`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/liveround.png` & `bulletroulette-1.0.4/bulletroulette/assets/liveround.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/magnifier.png` & `bulletroulette-1.0.4/bulletroulette/assets/magnifier.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/noneprop.png` & `bulletroulette-1.0.4/bulletroulette/assets/noneprop.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/pill.png` & `bulletroulette-1.0.4/bulletroulette/assets/pill.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/propbox.png` & `bulletroulette-1.0.4/bulletroulette/assets/propbox.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/smoke.png` & `bulletroulette-1.0.4/bulletroulette/assets/smoke.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/assets/super.png` & `bulletroulette-1.0.4/bulletroulette/assets/super.png`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/data.py` & `bulletroulette-1.0.4/bulletroulette/data.py`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/roles.py` & `bulletroulette-1.0.4/bulletroulette/roles.py`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette/run.py` & `bulletroulette-1.0.4/bulletroulette/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 __version__ = "1.0" # 版本说明（没什么用）
 
 # 外部导入
 cannotuseGUI = False
 from random import shuffle
 from time import sleep
 import pygame
-from os import chdir
+from os import chdir,path
 from traceback import print_exc
 # 模块导入
 from bulletroulette.roles import *
 from bulletroulette.data import *
 from bulletroulette.sprites import *
 # 以下是主程序
-file = __file__
-while file[-1] != "/":
-    file = file[:-1]
-chdir(file)
+chdir(path.dirname(__file__))
 health = [2,4,6]
 buckshots = [ # 子弹（1代表实，0代表空）
         [
             [1,0,0],
             [1,1,0,0]
         ],
         [
```

### Comparing `bulletroulette-1.0.3/bulletroulette/sprites.py` & `bulletroulette-1.0.4/bulletroulette/sprites.py`

 * *Files identical despite different names*

### Comparing `bulletroulette-1.0.3/bulletroulette.egg-info/SOURCES.txt` & `bulletroulette-1.0.4/bulletroulette.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,17 @@
 bulletroulette/assets/T.png
 bulletroulette/assets/U.png
 bulletroulette/assets/V.png
 bulletroulette/assets/W.png
 bulletroulette/assets/X.png
 bulletroulette/assets/Y.png
 bulletroulette/assets/Z.png
-bulletroulette/assets/__init__.py
 bulletroulette/assets/beer.png
 bulletroulette/assets/bg.png
 bulletroulette/assets/bgmsc.ogg
-bulletroulette/assets/binary.png
 bulletroulette/assets/blank.png
 bulletroulette/assets/blank.wav
 bulletroulette/assets/charge.png
 bulletroulette/assets/dealershootplayer.png
 bulletroulette/assets/dealershootself.png
 bulletroulette/assets/gun.png
 bulletroulette/assets/handcuff.png
```

### Comparing `bulletroulette-1.0.3/setup.py` & `bulletroulette-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="bulletroulette",  # 模块名称
-    version="1.0.3",  # 当前版本
+    version="1.0.4",  # 当前版本
     author="GQX",  # 作者
     author_email="kill114514251@outlook.com",  # 作者邮箱
     description="模仿steam游戏“恶魔轮盘”，目前没有提供开发接口（只能单纯玩）",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/BinaryGuo/Buckshot_Roulette",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

