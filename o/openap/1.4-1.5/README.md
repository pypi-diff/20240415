# Comparing `tmp/openap-1.4.tar.gz` & `tmp/openap-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openap-1.4.tar", max compression
+gzip compressed data, was "openap-1.5.tar", max compression
```

## Comparing `openap-1.4.tar` & `openap-1.5.tar`

### file list

```diff
@@ -1,110 +1,111 @@
--rw-r--r--   0        0        0     7652 2024-04-09 13:17:35.717328 openap-1.4/LICENSE
--rw-r--r--   0        0        0     2685 2024-04-09 13:17:35.717328 openap-1.4/README.md
--rw-r--r--   0        0        0      272 2024-04-09 13:17:35.717328 openap-1.4/openap/__init__.py
--rw-r--r--   0        0        0      991 2024-04-09 13:17:35.717328 openap-1.4/openap/casadi/__init__.py
--rw-r--r--   0        0        0     8774 2024-04-09 13:17:35.717328 openap-1.4/openap/casadi/aero_override.py
--rw-r--r--   0        0        0      271 2024-04-09 13:17:35.717328 openap-1.4/openap/casadi/numpy_override.py
--rw-r--r--   0        0        0     3044 2024-04-09 13:17:35.717328 openap-1.4/openap/contrail.py
--rw-r--r--   0        0        0     1045 2024-04-09 13:17:35.717328 openap-1.4/openap/data/.gitignore
--rw-r--r--   0        0        0    35141 2024-04-09 13:17:35.717328 openap-1.4/openap/data/LICENSE
--rw-r--r--   0        0        0      239 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/_synonym.csv
--rw-r--r--   0        0        0      626 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a19n.yml
--rw-r--r--   0        0        0      702 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a20n.yml
--rw-r--r--   0        0        0      676 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a21n.yml
--rw-r--r--   0        0        0      735 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a319.yml
--rw-r--r--   0        0        0      761 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a320.yml
--rw-r--r--   0        0        0      734 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a321.yml
--rw-r--r--   0        0        0      700 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a332.yml
--rw-r--r--   0        0        0      768 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a333.yml
--rw-r--r--   0        0        0      629 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a343.yml
--rw-r--r--   0        0        0      585 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a359.yml
--rw-r--r--   0        0        0      627 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/a388.yml
--rw-r--r--   0        0        0      563 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b37m.yml
--rw-r--r--   0        0        0      565 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b38m.yml
--rw-r--r--   0        0        0      564 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b39m.yml
--rw-r--r--   0        0        0      565 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b3xm.yml
--rw-r--r--   0        0        0      585 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b734.yml
--rw-r--r--   0        0        0      635 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b737.yml
--rw-r--r--   0        0        0      603 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b738.yml
--rw-r--r--   0        0        0      602 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b739.yml
--rw-r--r--   0        0        0      607 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b744.yml
--rw-r--r--   0        0        0      568 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b748.yml
--rw-r--r--   0        0        0      582 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b752.yml
--rw-r--r--   0        0        0      602 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b763.yml
--rw-r--r--   0        0        0      650 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b772.yml
--rw-r--r--   0        0        0      604 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b773.yml
--rw-r--r--   0        0        0      575 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b77w.yml
--rw-r--r--   0        0        0      665 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b788.yml
--rw-r--r--   0        0        0      649 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/b789.yml
--rw-r--r--   0        0        0      556 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/c550.yml
--rw-r--r--   0        0        0      564 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e145.yml
--rw-r--r--   0        0        0      573 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e170.yml
--rw-r--r--   0        0        0      567 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e190.yml
--rw-r--r--   0        0        0      567 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e195.yml
--rw-r--r--   0        0        0      579 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/e75l.yml
--rw-r--r--   0        0        0      600 2024-04-09 13:17:35.717328 openap-1.4/openap/data/aircraft/glf6.yml
--rw-r--r--   0        0        0      328 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/_synonym.csv
--rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a20n.yml
--rw-r--r--   0        0        0      186 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a319.yml
--rw-r--r--   0        0        0      186 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a320.yml
--rw-r--r--   0        0        0      186 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a321.yml
--rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a332.yml
--rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a333.yml
--rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a343.yml
--rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a359.yml
--rw-r--r--   0        0        0      190 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/a388.yml
--rw-r--r--   0        0        0      191 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b38m.yml
--rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b734.yml
--rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b737.yml
--rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b738.yml
--rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b739.yml
--rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b744.yml
--rw-r--r--   0        0        0      187 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b748.yml
--rw-r--r--   0        0        0      189 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b752.yml
--rw-r--r--   0        0        0      195 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b772.yml
--rw-r--r--   0        0        0      191 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b77w.yml
--rw-r--r--   0        0        0      187 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b788.yml
--rw-r--r--   0        0        0      187 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/b789.yml
--rw-r--r--   0        0        0      193 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/c550.yml
--rw-r--r--   0        0        0      192 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/e190.yml
--rw-r--r--   0        0        0      192 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/e195.yml
--rw-r--r--   0        0        0      192 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/e75l.yml
--rw-r--r--   0        0        0      198 2024-04-09 13:17:35.717328 openap-1.4/openap/data/dragpolar/glf6.yml
--rw-r--r--   0        0        0    81420 2024-04-09 13:17:35.717328 openap-1.4/openap/data/engine/engines.csv
--rw-r--r--   0        0        0   762442 2024-04-09 13:17:35.725328 openap-1.4/openap/data/nav/airports.csv
--rw-r--r--   0        0        0  3591430 2024-04-09 13:17:35.741328 openap-1.4/openap/data/nav/fix.dat
--rw-r--r--   0        0        0  2043823 2024-04-09 13:17:35.749328 openap-1.4/openap/data/nav/nav.dat
--rw-r--r--   0        0        0      418 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/_synonym.csv
--rw-r--r--   0        0        0     4391 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/a319.txt
--rw-r--r--   0        0        0     4386 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/a320.txt
--rw-r--r--   0        0        0     4337 2024-04-09 13:17:35.749328 openap-1.4/openap/data/wrap/a321.txt
--rw-r--r--   0        0        0     4371 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a332.txt
--rw-r--r--   0        0        0     4385 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a333.txt
--rw-r--r--   0        0        0     4434 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a343.txt
--rw-r--r--   0        0        0     4381 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/a388.txt
--rw-r--r--   0        0        0     4396 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b737.txt
--rw-r--r--   0        0        0     4323 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b738.txt
--rw-r--r--   0        0        0     4370 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b739.txt
--rw-r--r--   0        0        0     4378 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b744.txt
--rw-r--r--   0        0        0     4363 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b752.txt
--rw-r--r--   0        0        0     4386 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b763.txt
--rw-r--r--   0        0        0     4359 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b77w.txt
--rw-r--r--   0        0        0     4378 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b788.txt
--rw-r--r--   0        0        0     4383 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/b789.txt
--rw-r--r--   0        0        0     4340 2024-04-09 13:17:35.753328 openap-1.4/openap/data/wrap/e190.txt
--rw-r--r--   0        0        0     6063 2024-04-09 13:17:35.753328 openap-1.4/openap/drag.py
--rw-r--r--   0        0        0     6174 2024-04-09 13:17:35.753328 openap-1.4/openap/emission.py
--rw-r--r--   0        0        0      560 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/__init__.py
--rw-r--r--   0        0        0    10408 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/aero.py
--rw-r--r--   0        0        0     4971 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/filters.py
--rw-r--r--   0        0        0     2873 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/nav.py
--rw-r--r--   0        0        0     2486 2024-04-09 13:17:35.753328 openap-1.4/openap/extra/statistics.py
--rw-r--r--   0        0        0     5806 2024-04-09 13:17:35.753328 openap-1.4/openap/fuel.py
--rw-r--r--   0        0        0     6076 2024-04-09 13:17:35.753328 openap-1.4/openap/kinematic.py
--rw-r--r--   0        0        0    12961 2024-04-09 13:17:35.753328 openap-1.4/openap/phase.py
--rw-r--r--   0        0        0     3681 2024-04-09 13:17:35.753328 openap-1.4/openap/prop.py
--rw-r--r--   0        0        0     6371 2024-04-09 13:17:35.753328 openap-1.4/openap/thrust.py
--rw-r--r--   0        0        0       27 2024-04-09 13:17:35.753328 openap-1.4/openap/traj/__init__.py
--rw-r--r--   0        0        0    17416 2024-04-09 13:17:35.753328 openap-1.4/openap/traj/gen.py
--rw-r--r--   0        0        0     1107 2024-04-09 13:17:35.753328 openap-1.4/pyproject.toml
--rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 openap-1.4/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-04-15 20:52:38.416125 openap-1.5/LICENSE
+-rw-r--r--   0        0        0     2685 2024-04-15 20:52:38.416125 openap-1.5/README.md
+-rw-r--r--   0        0        0      272 2024-04-15 20:52:38.416125 openap-1.5/openap/__init__.py
+-rw-r--r--   0        0        0      991 2024-04-15 20:52:38.416125 openap-1.5/openap/casadi/__init__.py
+-rw-r--r--   0        0        0     8774 2024-04-15 20:52:38.416125 openap-1.5/openap/casadi/aero_override.py
+-rw-r--r--   0        0        0      271 2024-04-15 20:52:38.416125 openap-1.5/openap/casadi/numpy_override.py
+-rw-r--r--   0        0        0     3044 2024-04-15 20:52:38.416125 openap-1.5/openap/contrail.py
+-rw-r--r--   0        0        0     1045 2024-04-15 20:52:38.416125 openap-1.5/openap/data/.gitignore
+-rw-r--r--   0        0        0    35141 2024-04-15 20:52:38.416125 openap-1.5/openap/data/LICENSE
+-rw-r--r--   0        0        0      239 2024-04-15 20:52:38.416125 openap-1.5/openap/data/aircraft/_synonym.csv
+-rw-r--r--   0        0        0      626 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a19n.yml
+-rw-r--r--   0        0        0      702 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a20n.yml
+-rw-r--r--   0        0        0      676 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a21n.yml
+-rw-r--r--   0        0        0      735 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a319.yml
+-rw-r--r--   0        0        0      761 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a320.yml
+-rw-r--r--   0        0        0      734 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a321.yml
+-rw-r--r--   0        0        0      700 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a332.yml
+-rw-r--r--   0        0        0      768 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a333.yml
+-rw-r--r--   0        0        0      629 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a343.yml
+-rw-r--r--   0        0        0      585 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a359.yml
+-rw-r--r--   0        0        0      627 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/a388.yml
+-rw-r--r--   0        0        0      563 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b37m.yml
+-rw-r--r--   0        0        0      565 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b38m.yml
+-rw-r--r--   0        0        0      564 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b39m.yml
+-rw-r--r--   0        0        0      565 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b3xm.yml
+-rw-r--r--   0        0        0      585 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b734.yml
+-rw-r--r--   0        0        0      635 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b737.yml
+-rw-r--r--   0        0        0      603 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b738.yml
+-rw-r--r--   0        0        0      602 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b739.yml
+-rw-r--r--   0        0        0      607 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b744.yml
+-rw-r--r--   0        0        0      568 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b748.yml
+-rw-r--r--   0        0        0      582 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b752.yml
+-rw-r--r--   0        0        0      602 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b763.yml
+-rw-r--r--   0        0        0      650 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b772.yml
+-rw-r--r--   0        0        0      604 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b773.yml
+-rw-r--r--   0        0        0      575 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b77w.yml
+-rw-r--r--   0        0        0      665 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b788.yml
+-rw-r--r--   0        0        0      649 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/b789.yml
+-rw-r--r--   0        0        0      556 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/c550.yml
+-rw-r--r--   0        0        0      564 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/e145.yml
+-rw-r--r--   0        0        0      573 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/e170.yml
+-rw-r--r--   0        0        0      567 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/e190.yml
+-rw-r--r--   0        0        0      567 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/e195.yml
+-rw-r--r--   0        0        0      579 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/e75l.yml
+-rw-r--r--   0        0        0      600 2024-04-15 20:52:38.420125 openap-1.5/openap/data/aircraft/glf6.yml
+-rw-r--r--   0        0        0      328 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/_synonym.csv
+-rw-r--r--   0        0        0      189 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a20n.yml
+-rw-r--r--   0        0        0      186 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a319.yml
+-rw-r--r--   0        0        0      186 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a320.yml
+-rw-r--r--   0        0        0      186 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a321.yml
+-rw-r--r--   0        0        0      190 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a332.yml
+-rw-r--r--   0        0        0      190 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a333.yml
+-rw-r--r--   0        0        0      190 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a343.yml
+-rw-r--r--   0        0        0      190 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a359.yml
+-rw-r--r--   0        0        0      190 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/a388.yml
+-rw-r--r--   0        0        0      191 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b38m.yml
+-rw-r--r--   0        0        0      189 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b734.yml
+-rw-r--r--   0        0        0      189 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b737.yml
+-rw-r--r--   0        0        0      189 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b738.yml
+-rw-r--r--   0        0        0      189 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b739.yml
+-rw-r--r--   0        0        0      189 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b744.yml
+-rw-r--r--   0        0        0      187 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b748.yml
+-rw-r--r--   0        0        0      189 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b752.yml
+-rw-r--r--   0        0        0      195 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b772.yml
+-rw-r--r--   0        0        0      191 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b77w.yml
+-rw-r--r--   0        0        0      187 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b788.yml
+-rw-r--r--   0        0        0      187 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/b789.yml
+-rw-r--r--   0        0        0      193 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/c550.yml
+-rw-r--r--   0        0        0      192 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/e190.yml
+-rw-r--r--   0        0        0      192 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/e195.yml
+-rw-r--r--   0        0        0      192 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/e75l.yml
+-rw-r--r--   0        0        0      198 2024-04-15 20:52:38.420125 openap-1.5/openap/data/dragpolar/glf6.yml
+-rw-r--r--   0        0        0    81420 2024-04-15 20:52:38.420125 openap-1.5/openap/data/engine/engines.csv
+-rw-r--r--   0        0        0   762442 2024-04-15 20:52:38.424125 openap-1.5/openap/data/nav/airports.csv
+-rw-r--r--   0        0        0  3591430 2024-04-15 20:52:38.444125 openap-1.5/openap/data/nav/fix.dat
+-rw-r--r--   0        0        0  2043823 2024-04-15 20:52:38.452125 openap-1.5/openap/data/nav/nav.dat
+-rw-r--r--   0        0        0      418 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/_synonym.csv
+-rw-r--r--   0        0        0     4391 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/a319.txt
+-rw-r--r--   0        0        0     4386 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/a320.txt
+-rw-r--r--   0        0        0     4337 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/a321.txt
+-rw-r--r--   0        0        0     4371 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/a332.txt
+-rw-r--r--   0        0        0     4385 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/a333.txt
+-rw-r--r--   0        0        0     4434 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/a343.txt
+-rw-r--r--   0        0        0     4381 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/a388.txt
+-rw-r--r--   0        0        0     4396 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b737.txt
+-rw-r--r--   0        0        0     4323 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b738.txt
+-rw-r--r--   0        0        0     4370 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b739.txt
+-rw-r--r--   0        0        0     4378 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b744.txt
+-rw-r--r--   0        0        0     4363 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b752.txt
+-rw-r--r--   0        0        0     4386 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b763.txt
+-rw-r--r--   0        0        0     4359 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b77w.txt
+-rw-r--r--   0        0        0     4378 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b788.txt
+-rw-r--r--   0        0        0     4383 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/b789.txt
+-rw-r--r--   0        0        0     4340 2024-04-15 20:52:38.452125 openap-1.5/openap/data/wrap/e190.txt
+-rw-r--r--   0        0        0     6106 2024-04-15 20:52:38.452125 openap-1.5/openap/drag.py
+-rw-r--r--   0        0        0     6174 2024-04-15 20:52:38.452125 openap-1.5/openap/emission.py
+-rw-r--r--   0        0        0      560 2024-04-15 20:52:38.452125 openap-1.5/openap/extra/__init__.py
+-rw-r--r--   0        0        0    10408 2024-04-15 20:52:38.452125 openap-1.5/openap/extra/aero.py
+-rw-r--r--   0        0        0     4971 2024-04-15 20:52:38.452125 openap-1.5/openap/extra/filters.py
+-rw-r--r--   0        0        0     5119 2024-04-15 20:52:38.452125 openap-1.5/openap/extra/fuzzy.py
+-rw-r--r--   0        0        0     2873 2024-04-15 20:52:38.456125 openap-1.5/openap/extra/nav.py
+-rw-r--r--   0        0        0     2486 2024-04-15 20:52:38.456125 openap-1.5/openap/extra/statistics.py
+-rw-r--r--   0        0        0     5806 2024-04-15 20:52:38.456125 openap-1.5/openap/fuel.py
+-rw-r--r--   0        0        0     6076 2024-04-15 20:52:38.456125 openap-1.5/openap/kinematic.py
+-rw-r--r--   0        0        0    13137 2024-04-15 20:52:38.456125 openap-1.5/openap/phase.py
+-rw-r--r--   0        0        0     3720 2024-04-15 20:52:38.456125 openap-1.5/openap/prop.py
+-rw-r--r--   0        0        0     6371 2024-04-15 20:52:38.456125 openap-1.5/openap/thrust.py
+-rw-r--r--   0        0        0       27 2024-04-15 20:52:38.456125 openap-1.5/openap/traj/__init__.py
+-rw-r--r--   0        0        0    17416 2024-04-15 20:52:38.456125 openap-1.5/openap/traj/gen.py
+-rw-r--r--   0        0        0     1084 2024-04-15 20:52:38.456125 openap-1.5/pyproject.toml
+-rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 openap-1.5/PKG-INFO
```

### Comparing `openap-1.4/LICENSE` & `openap-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openap-1.4/README.md` & `openap-1.5/README.md`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/casadi/__init__.py` & `openap-1.5/openap/casadi/__init__.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/casadi/aero_override.py` & `openap-1.5/openap/casadi/aero_override.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/contrail.py` & `openap-1.5/openap/contrail.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/.gitignore` & `openap-1.5/openap/data/.gitignore`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/LICENSE` & `openap-1.5/openap/data/LICENSE`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a19n.yml` & `openap-1.5/openap/data/aircraft/a19n.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a20n.yml` & `openap-1.5/openap/data/aircraft/a20n.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a21n.yml` & `openap-1.5/openap/data/aircraft/a21n.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a319.yml` & `openap-1.5/openap/data/aircraft/a319.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a320.yml` & `openap-1.5/openap/data/aircraft/a320.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a321.yml` & `openap-1.5/openap/data/aircraft/a321.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a332.yml` & `openap-1.5/openap/data/aircraft/a332.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a333.yml` & `openap-1.5/openap/data/aircraft/a333.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a343.yml` & `openap-1.5/openap/data/aircraft/a343.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a359.yml` & `openap-1.5/openap/data/aircraft/a359.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/a388.yml` & `openap-1.5/openap/data/aircraft/a388.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b37m.yml` & `openap-1.5/openap/data/aircraft/b37m.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b38m.yml` & `openap-1.5/openap/data/aircraft/b38m.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b39m.yml` & `openap-1.5/openap/data/aircraft/b39m.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b3xm.yml` & `openap-1.5/openap/data/aircraft/b3xm.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b734.yml` & `openap-1.5/openap/data/aircraft/b734.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b737.yml` & `openap-1.5/openap/data/aircraft/b737.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b738.yml` & `openap-1.5/openap/data/aircraft/b738.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b739.yml` & `openap-1.5/openap/data/aircraft/b739.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b744.yml` & `openap-1.5/openap/data/aircraft/b744.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b748.yml` & `openap-1.5/openap/data/aircraft/b748.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b752.yml` & `openap-1.5/openap/data/aircraft/b752.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b763.yml` & `openap-1.5/openap/data/aircraft/b763.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b772.yml` & `openap-1.5/openap/data/aircraft/b772.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b773.yml` & `openap-1.5/openap/data/aircraft/b773.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b77w.yml` & `openap-1.5/openap/data/aircraft/b77w.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b788.yml` & `openap-1.5/openap/data/aircraft/b788.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/b789.yml` & `openap-1.5/openap/data/aircraft/b789.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/c550.yml` & `openap-1.5/openap/data/aircraft/c550.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/e145.yml` & `openap-1.5/openap/data/aircraft/e145.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/e170.yml` & `openap-1.5/openap/data/aircraft/e170.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/e190.yml` & `openap-1.5/openap/data/aircraft/e190.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/e195.yml` & `openap-1.5/openap/data/aircraft/e195.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/e75l.yml` & `openap-1.5/openap/data/aircraft/e75l.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/aircraft/glf6.yml` & `openap-1.5/openap/data/aircraft/glf6.yml`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/engine/engines.csv` & `openap-1.5/openap/data/engine/engines.csv`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/nav/airports.csv` & `openap-1.5/openap/data/nav/airports.csv`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/nav/fix.dat` & `openap-1.5/openap/data/nav/fix.dat`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/nav/nav.dat` & `openap-1.5/openap/data/nav/nav.dat`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/a319.txt` & `openap-1.5/openap/data/wrap/a319.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/a320.txt` & `openap-1.5/openap/data/wrap/a320.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/a321.txt` & `openap-1.5/openap/data/wrap/a321.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/a332.txt` & `openap-1.5/openap/data/wrap/a332.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/a333.txt` & `openap-1.5/openap/data/wrap/a333.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/a343.txt` & `openap-1.5/openap/data/wrap/a343.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/a388.txt` & `openap-1.5/openap/data/wrap/a388.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b737.txt` & `openap-1.5/openap/data/wrap/b737.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b738.txt` & `openap-1.5/openap/data/wrap/b738.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b739.txt` & `openap-1.5/openap/data/wrap/b739.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b744.txt` & `openap-1.5/openap/data/wrap/b744.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b752.txt` & `openap-1.5/openap/data/wrap/b752.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b763.txt` & `openap-1.5/openap/data/wrap/b763.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b77w.txt` & `openap-1.5/openap/data/wrap/b77w.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b788.txt` & `openap-1.5/openap/data/wrap/b788.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/b789.txt` & `openap-1.5/openap/data/wrap/b789.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/data/wrap/e190.txt` & `openap-1.5/openap/data/wrap/e190.txt`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/drag.py` & `openap-1.5/openap/drag.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,16 @@
             syno = polar_synonym.query("orig==@self.ac")
             if self.use_synonym and syno.shape[0] > 0:
                 ac = syno.new.iloc[0]
             else:
                 raise RuntimeError(f"Drag polar for {self.ac} not avaiable in OpenAP.")
 
         f = dir_dragpolar + ac + ".yml"
-        dragpolar = yaml.safe_load(open(f))
+        with open(f, "r") as file:
+            dragpolar = yaml.safe_load(file.read())
         return dragpolar
 
     @ndarrayconvert
     def _cl(self, mass, tas, alt):
         v = tas * self.aero.kts
         h = alt * self.aero.ft
```

### Comparing `openap-1.4/openap/emission.py` & `openap-1.5/openap/emission.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/extra/__init__.py` & `openap-1.5/openap/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/extra/aero.py` & `openap-1.5/openap/extra/aero.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/extra/filters.py` & `openap-1.5/openap/extra/filters.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/extra/nav.py` & `openap-1.5/openap/extra/nav.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/extra/statistics.py` & `openap-1.5/openap/extra/statistics.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/fuel.py` & `openap-1.5/openap/fuel.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/kinematic.py` & `openap-1.5/openap/kinematic.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/phase.py` & `openap-1.5/openap/phase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 """Using fuzzy logic to indentify flight phase in trajectory data."""
 
 import numpy as np
-import skfuzzy as fuzz
 from matplotlib import pyplot as plt
 
+from openap.extra import fuzzy
+
 
 class FlightPhase(object):
     """Fuzzy logic flight phase identification."""
 
     def __init__(self):
         """Initialize of the FlightPhase object."""
         super(FlightPhase, self).__init__()
 
         # logic states
         self.alt_range = np.arange(0, 40000, 1)
         self.roc_range = np.arange(-4000, 4000, 0.1)
         self.spd_range = np.arange(0, 600, 1)
         self.states = np.arange(0, 6, 0.01)
 
-        self.alt_gnd = fuzz.zmf(self.alt_range, 0, 200)
-        self.alt_lo = fuzz.gaussmf(self.alt_range, 10000, 10000)
-        self.alt_hi = fuzz.gaussmf(self.alt_range, 35000, 20000)
-
-        self.roc_zero = fuzz.gaussmf(self.roc_range, 0, 100)
-        self.roc_plus = fuzz.smf(self.roc_range, 10, 1000)
-        self.roc_minus = fuzz.zmf(self.roc_range, -1000, -10)
-
-        self.spd_hi = fuzz.gaussmf(self.spd_range, 600, 100)
-        self.spd_md = fuzz.gaussmf(self.spd_range, 300, 100)
-        self.spd_lo = fuzz.gaussmf(self.spd_range, 0, 50)
-
-        self.state_ground = fuzz.gaussmf(self.states, 1, 0.1)
-        self.state_climb = fuzz.gaussmf(self.states, 2, 0.1)
-        self.state_descent = fuzz.gaussmf(self.states, 3, 0.1)
-        self.state_cruise = fuzz.gaussmf(self.states, 4, 0.1)
-        self.state_level = fuzz.gaussmf(self.states, 5, 0.1)
+        self.alt_gnd = fuzzy.zmf(self.alt_range, 0, 200)
+        self.alt_lo = fuzzy.gaussmf(self.alt_range, 10000, 10000)
+        self.alt_hi = fuzzy.gaussmf(self.alt_range, 35000, 20000)
+
+        self.roc_zero = fuzzy.gaussmf(self.roc_range, 0, 100)
+        self.roc_plus = fuzzy.smf(self.roc_range, 10, 1000)
+        self.roc_minus = fuzzy.zmf(self.roc_range, -1000, -10)
+
+        self.spd_hi = fuzzy.gaussmf(self.spd_range, 600, 100)
+        self.spd_md = fuzzy.gaussmf(self.spd_range, 300, 100)
+        self.spd_lo = fuzzy.gaussmf(self.spd_range, 0, 50)
+
+        self.state_ground = fuzzy.gaussmf(self.states, 1, 0.1)
+        self.state_climb = fuzzy.gaussmf(self.states, 2, 0.1)
+        self.state_descent = fuzzy.gaussmf(self.states, 3, 0.1)
+        self.state_cruise = fuzzy.gaussmf(self.states, 4, 0.1)
+        self.state_level = fuzzy.gaussmf(self.states, 5, 0.1)
 
-        self.state_lable_map = {1: 'GND', 2: 'CL', 3: 'DE', 4: 'CR', 5:'LVL'}
+        self.state_lable_map = {1: "GND", 2: "CL", 3: "DE", 4: "CR", 5: "LVL"}
 
         self.ts = None
         self.alt = None
         self.spd = None
         self.roc = None
 
     def set_trajectory(self, ts, alt, spd, roc):
@@ -55,15 +56,15 @@
         """
         self.ts = ts - ts[0]
         self.alt = alt
         self.spd = spd
         self.roc = roc
 
         if len(set([len(self.ts), len(self.alt), len(self.spd), len(self.roc)])) > 1:
-            raise RuntimeError('Input lists must have same length.')
+            raise RuntimeError("Input lists must have same length.")
 
         self.ndata = len(self.ts)
 
         return
 
     def phaselabel(self, twindow=60):
         """Fuzzy logic for determining phase label.
@@ -73,27 +74,29 @@
 
         Returns:
             list: Labels could be: ground [GND], climb [CL], descent [DE],
                 cruise [CR], leveling [LVL].
 
         """
         if self.ts is None:
-            raise RuntimeError('Trajectory data not set, run set_trajectory(ts, alt, spd, roc) first')
+            raise RuntimeError(
+                "Trajectory data not set, run set_trajectory(ts, alt, spd, roc) first"
+            )
 
         idxs = np.arange(0, self.ndata)
 
-        labels = ['NA'] * self.ndata
+        labels = ["NA"] * self.ndata
 
         twindows = self.ts // twindow
 
         for tw in range(0, int(max(twindows))):
             if tw not in twindows:
                 continue
 
-            mask = (twindows == tw)
+            mask = twindows == tw
 
             idxchk = idxs[mask]
             altchk = self.alt[mask]
             spdchk = self.spd[mask]
             rocchk = self.roc[mask]
 
             # mean value or extream value as range
@@ -102,25 +105,27 @@
             roc = max(min(np.mean(rocchk), self.roc_range[-1]), self.roc_range[0])
 
             # make sure values are within the boundaries
             alt = max(min(alt, self.alt_range[-1]), self.alt_range[0])
             spd = max(min(spd, self.spd_range[-1]), self.spd_range[0])
             roc = max(min(roc, self.roc_range[-1]), self.roc_range[0])
 
-            alt_level_gnd = fuzz.interp_membership(self.alt_range, self.alt_gnd, alt)
-            alt_level_lo = fuzz.interp_membership(self.alt_range, self.alt_lo, alt)
-            alt_level_hi = fuzz.interp_membership(self.alt_range, self.alt_hi, alt)
-
-            spd_level_hi = fuzz.interp_membership(self.spd_range, self.spd_hi, spd)
-            spd_level_md = fuzz.interp_membership(self.spd_range, self.spd_md, spd)
-            spd_level_lo = fuzz.interp_membership(self.spd_range, self.spd_lo, spd)
-
-            roc_level_zero = fuzz.interp_membership(self.roc_range, self.roc_zero, roc)
-            roc_level_plus = fuzz.interp_membership(self.roc_range, self.roc_plus, roc)
-            roc_level_minus = fuzz.interp_membership(self.roc_range, self.roc_minus, roc)
+            alt_level_gnd = fuzzy.interp_membership(self.alt_range, self.alt_gnd, alt)
+            alt_level_lo = fuzzy.interp_membership(self.alt_range, self.alt_lo, alt)
+            alt_level_hi = fuzzy.interp_membership(self.alt_range, self.alt_hi, alt)
+
+            spd_level_hi = fuzzy.interp_membership(self.spd_range, self.spd_hi, spd)
+            spd_level_md = fuzzy.interp_membership(self.spd_range, self.spd_md, spd)
+            spd_level_lo = fuzzy.interp_membership(self.spd_range, self.spd_lo, spd)
+
+            roc_level_zero = fuzzy.interp_membership(self.roc_range, self.roc_zero, roc)
+            roc_level_plus = fuzzy.interp_membership(self.roc_range, self.roc_plus, roc)
+            roc_level_minus = fuzzy.interp_membership(
+                self.roc_range, self.roc_minus, roc
+            )
 
             # print alt_level_gnd, alt_level_lo, alt_level_hi
             # print roc_level_zero, roc_level_plus, roc_level_minus
             # print spd_level_hi, spd_level_md, spd_level_lo
 
             rule_ground = min(alt_level_gnd, roc_level_zero, spd_level_lo)
             state_activate_ground = np.fmin(rule_ground, self.state_ground)
@@ -134,85 +139,88 @@
             rule_cruise = min(alt_level_hi, roc_level_zero, spd_level_hi)
             state_activate_cruise = np.fmin(rule_cruise, self.state_cruise)
 
             rule_level = min(alt_level_lo, roc_level_zero, spd_level_md)
             state_activate_level = np.fmin(rule_level, self.state_level)
 
             aggregated = np.max(
-                np.vstack([
-                    state_activate_ground,
-                    state_activate_climb,
-                    state_activate_descent,
-                    state_activate_cruise,
-                    state_activate_level,
-                ]), axis=0
+                np.vstack(
+                    [
+                        state_activate_ground,
+                        state_activate_climb,
+                        state_activate_descent,
+                        state_activate_cruise,
+                        state_activate_level,
+                    ]
+                ),
+                axis=0,
             )
 
-            state_raw = fuzz.defuzz(self.states, aggregated, 'lom')
+            state_raw = fuzzy.defuzz(self.states, aggregated, "lom")
             state = int(round(state_raw))
             if state > 6:
                 state = 6
             if state < 1:
                 state = 1
 
             if len(idxchk) > 0:
                 label = self.state_lable_map[state]
-                labels[idxchk[0]:(idxchk[-1]+1)] = [label] * len(idxchk)
+                labels[idxchk[0] : (idxchk[-1] + 1)] = [label] * len(idxchk)
 
         return labels
 
     def plot_logics(self):
         """Visualize fuzzy logic membership functions."""
         plt.figure(figsize=(10, 8))
 
         plt.subplot(411)
-        plt.plot(self.alt_range, self.alt_gnd, lw=2, label='Ground')
-        plt.plot(self.alt_range, self.alt_lo, lw=2, label='Low')
-        plt.plot(self.alt_range, self.alt_hi, lw=2, label='High')
+        plt.plot(self.alt_range, self.alt_gnd, lw=2, label="Ground")
+        plt.plot(self.alt_range, self.alt_lo, lw=2, label="Low")
+        plt.plot(self.alt_range, self.alt_hi, lw=2, label="High")
         plt.ylim([-0.05, 1.05])
-        plt.ylabel('Altitude (ft)')
+        plt.ylabel("Altitude (ft)")
         plt.yticks([0, 1])
         plt.legend()
 
         plt.subplot(412)
-        plt.plot(self.roc_range, self.roc_zero, lw=2, label='Zero')
-        plt.plot(self.roc_range, self.roc_plus, lw=2, label='Positive')
-        plt.plot(self.roc_range, self.roc_minus, lw=2, label='Negative')
+        plt.plot(self.roc_range, self.roc_zero, lw=2, label="Zero")
+        plt.plot(self.roc_range, self.roc_plus, lw=2, label="Positive")
+        plt.plot(self.roc_range, self.roc_minus, lw=2, label="Negative")
         plt.ylim([-0.05, 1.05])
-        plt.ylabel('RoC (ft/m)')
+        plt.ylabel("RoC (ft/m)")
         plt.yticks([0, 1])
         plt.legend()
 
         plt.subplot(413)
-        plt.plot(self.spd_range, self.spd_hi, lw=2, label='High')
-        plt.plot(self.spd_range, self.spd_md, lw=2, label='Midium')
-        plt.plot(self.spd_range, self.spd_lo, lw=2, label='Low')
+        plt.plot(self.spd_range, self.spd_hi, lw=2, label="High")
+        plt.plot(self.spd_range, self.spd_md, lw=2, label="Midium")
+        plt.plot(self.spd_range, self.spd_lo, lw=2, label="Low")
         plt.ylim([-0.05, 1.05])
-        plt.ylabel('Speed (kt)')
+        plt.ylabel("Speed (kt)")
         plt.yticks([0, 1])
         plt.legend()
 
         plt.subplot(414)
-        plt.plot(self.states, self.state_ground, lw=2, label='ground')
-        plt.plot(self.states, self.state_climb, lw=2, label='climb')
-        plt.plot(self.states, self.state_descent, lw=2, label='descent')
-        plt.plot(self.states, self.state_cruise, lw=2, label='cruise')
-        plt.plot(self.states, self.state_level, lw=2, label='level flight')
+        plt.plot(self.states, self.state_ground, lw=2, label="ground")
+        plt.plot(self.states, self.state_climb, lw=2, label="climb")
+        plt.plot(self.states, self.state_descent, lw=2, label="descent")
+        plt.plot(self.states, self.state_cruise, lw=2, label="cruise")
+        plt.plot(self.states, self.state_level, lw=2, label="level flight")
         plt.ylim([-0.05, 1.05])
-        plt.ylabel('Flight Phases')
+        plt.ylabel("Flight Phases")
         plt.yticks([0, 1])
-        plt.legend(prop={'size': 7})
+        plt.legend(prop={"size": 7})
         plt.show()
 
     def _get_to_ic(self):
         # get the data chunk up to certain ft
         istart = 0
         iend = 0
         for i in range(0, self.ndata):
-            if self.alt[i] < 1500:     # ft
+            if self.alt[i] < 1500:  # ft
                 iend = i
                 continue
             else:
                 break
 
         # keep only the chunk in taking-off states, break at starting point
         spdtmp = self.spd[iend]
@@ -221,56 +229,55 @@
                 break
             elif self.spd[i] < 5:
                 break
             else:
                 istart = i
                 spdtmp = self.spd[i]
 
-
         # ignore too long take-off
         if self.ts[iend] - self.ts[istart] > 300:
             return None
 
         # ignore insufficient chunk size
         if iend - istart < 10:
             return None
 
         # ignore no in air data
         if self.alt[iend] < 200:
             return None
 
         # find the liftoff moment
         ilof = istart
-        for i in range(istart+1, iend):
-            if abs(self.alt[i] - self.alt[i-1]) > 10:
+        for i in range(istart + 1, iend):
+            if abs(self.alt[i] - self.alt[i - 1]) > 10:
                 ilof = i
                 break
 
         # not sufficient data
         if ilof - istart < 5:
             return None
 
-        return (istart, ilof, iend+1)
+        return (istart, ilof, iend + 1)
 
     def _get_fa_ld(self):
 
         # get the approach + landing data chunk (h=0)
         istart = 0
         iend = 0
 
         for i in reversed(list(range(0, self.ndata))):
-            if self.alt[i] < 1500:     # ft
+            if self.alt[i] < 1500:  # ft
                 istart = i
             else:
                 break
 
         # keep only the chunk in landing deceleration states, break at taxing point
         spdtmp = self.spd[istart]
         for i in range(istart, self.ndata):
-            if self.spd[i] <= 50 and self.spd[i] >= spdtmp:       # kts
+            if self.spd[i] <= 50 and self.spd[i] >= spdtmp:  # kts
                 break
             elif self.spd[i] < 30:
                 break
             else:
                 iend = i
                 spdtmp = self.spd[i]
 
@@ -284,51 +291,51 @@
 
         # # ignore where the end speed too high, ie. not breaked
         # if spd[iend] > 60: # kts
         #     return None
 
         # find the landing moment
         ild = iend
-        for i in reversed(list(range(istart, iend-1))):
-            if abs(self.alt[i] - self.alt[i+1]) > 10:
+        for i in reversed(list(range(istart, iend - 1))):
+            if abs(self.alt[i] - self.alt[i + 1]) > 10:
                 ild = i
                 break
 
         # ignore ground or air data sample less than 4
         if ild - istart < 5 or iend - ild < 5:
             return None
 
-        return (istart, ild, iend+1)
+        return (istart, ild, iend + 1)
 
     def _get_cl(self):
         labels = np.array(self.phaselabel())
 
-        if 'CL' not in labels:
+        if "CL" not in labels:
             return None
 
-        idx = np.where(np.array(labels) == 'CL')[0]
+        idx = np.where(np.array(labels) == "CL")[0]
 
         istart = idx[0]
         iend = idx[-1]
 
         return istart, iend
 
     def _get_de(self):
 
         labels = np.array(self.phaselabel())
 
-        if 'DE' not in labels:
+        if "DE" not in labels:
             return None
 
-        idx = np.where(np.array(labels) == 'DE')[0]
+        idx = np.where(np.array(labels) == "DE")[0]
 
         istart = idx[0]
         iend = idx[-1]
 
-        if 'LVL' in labels[istart:iend]:
+        if "LVL" in labels[istart:iend]:
             isCDA = False
         else:
             isCDA = True
 
         return istart, iend, isCDA
 
     def _get_cr(self):
@@ -393,18 +400,18 @@
             iend = len(self.ts)
         else:
             ifa = None
             ild = None
             iend = len(self.ts)
 
         idx = {
-            'TO': ito,
-            'IC': iic,
-            'CL': icl,
-            'CR': icr,
-            'DE': ide,
-            'FA': ifa,
-            'LD': ild,
-            'END': iend
+            "TO": ito,
+            "IC": iic,
+            "CL": icl,
+            "CR": icr,
+            "DE": ide,
+            "FA": ifa,
+            "LD": ild,
+            "END": iend,
         }
 
         return idx
```

### Comparing `openap-1.4/openap/prop.py` & `openap-1.5/openap/prop.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,16 @@
         if use_synonym and syno.shape[0] > 0:
             new_ac = syno.new.iloc[0]
             files = glob.glob(dir_aircraft + new_ac + ".yml")
         else:
             raise RuntimeError(f"Aircraft {ac} not avaiable in OpenAP.")
 
     f = files[0]
-    acdict = yaml.safe_load(open(f))
+    with open(f, "r") as file:
+        acdict = yaml.safe_load(file.read())
 
     return acdict
 
 
 @lru_cache()
 def aircraft_engine_options(ac):
     """Get engine options of an aircraft type.
```

### Comparing `openap-1.4/openap/thrust.py` & `openap-1.5/openap/thrust.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/openap/traj/gen.py` & `openap-1.5/openap/traj/gen.py`

 * *Files identical despite different names*

### Comparing `openap-1.4/pyproject.toml` & `openap-1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openap"
-version = "1.4"
+version = "1.5"
 description = "Open Aircraft Performance Model (OpenAP) in Python"
 homepage = "https://openap.dev"
 repository = "https://github.com/junzis/openap"
 authors = ["Junzi Sun <j.sun-1@tudelft.nl>"]
 license = "GNU Lesser General Public License v3 (LGPLv3)"
 readme = "README.md"
 classifiers = [
@@ -17,15 +17,14 @@
 packages = [{ include = "openap", from = "." }]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 numpy = ">=1.24"
 scipy = ">=1.7"
-scikit-fuzzy = ">=0.4"
 pandas = ">=1.2"
 pyyaml = ">=5.1"
 matplotlib = ">=3.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
```

### Comparing `openap-1.4/PKG-INFO` & `openap-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openap
-Version: 1.4
+Version: 1.5
 Summary: Open Aircraft Performance Model (OpenAP) in Python
 Home-page: https://openap.dev
 License: GNU Lesser General Public License v3 (LGPLv3)
 Author: Junzi Sun
 Author-email: j.sun-1@tudelft.nl
 Requires-Python: >=3.9
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: matplotlib (>=3.1)
 Requires-Dist: numpy (>=1.24)
 Requires-Dist: pandas (>=1.2)
 Requires-Dist: pyyaml (>=5.1)
-Requires-Dist: scikit-fuzzy (>=0.4)
 Requires-Dist: scipy (>=1.7)
 Project-URL: Repository, https://github.com/junzis/openap
 Description-Content-Type: text/markdown
 
 # Open Aircraft Performance Model (OpenAP) and Toolkit
 
 This repository contains the OpenAP model data and Python packages for aircraft performance and emission calculations.
```

