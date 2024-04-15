# Comparing `tmp/zigzag-dse-3.0.0.tar.gz` & `tmp/zigzag_dse-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigzag-dse-3.0.0.tar", last modified: Tue Mar 19 15:14:20 2024, max compression
+gzip compressed data, was "zigzag_dse-3.1.0.tar", last modified: Mon Apr 15 09:56:04 2024, max compression
```

## Comparing `zigzag-dse-3.0.0.tar` & `zigzag_dse-3.1.0.tar`

### file list

```diff
@@ -1,306 +1,322 @@
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:20.049492 zigzag-dse-3.0.0/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1074 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/LICENSE
--rw-r--r--   0 asymons  (27005) micas     (3600)       88 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/MANIFEST.in
--rw-r--r--   0 asymons  (27005) micas     (3600)    10722 2024-03-19 15:14:20.047491 zigzag-dse-3.0.0/PKG-INFO
--rw-r--r--   0 asymons  (27005) micas     (3600)     8519 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/README.md
--rw-r--r--   0 asymons  (27005) micas     (3600)     1601 2024-03-19 15:11:44.000000 zigzag-dse-3.0.0/pyproject.toml
--rw-r--r--   0 asymons  (27005) micas     (3600)       38 2024-03-19 15:14:20.049492 zigzag-dse-3.0.0/setup.cfg
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.531470 zigzag-dse-3.0.0/tests/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.535470 zigzag-dse-3.0.0/tests/main/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.582472 zigzag-dse-3.0.0/tests/main/test_imc/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/tests/main/test_imc/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1572 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/tests/main/test_imc/test_aimc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1545 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/tests/main/test_imc/test_dimc.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.591472 zigzag-dse-3.0.0/tests/main/test_origin/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_origin/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1253 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_origin/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1261 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_origin/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1266 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_origin/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1262 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_origin/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1250 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_origin/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.601473 zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2044 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2690 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2118 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2087 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2378 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.610473 zigzag-dse-3.0.0/tests/main/test_without_unused_memory/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_without_unused_memory/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1284 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1303 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1315 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1309 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1294 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.616474 zigzag-dse-3.0.0/zigzag/
--rw-r--r--   0 asymons  (27005) micas     (3600)       22 2024-03-19 15:11:44.000000 zigzag-dse-3.0.0/zigzag/__init__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2497 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/__main__.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    19803 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/api.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.618474 zigzag-dse-3.0.0/zigzag/classes/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/__init__.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.621474 zigzag-dse-3.0.0/zigzag/classes/cacti/
--rw-r--r--   0 asymons  (27005) micas     (3600)      291 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/README.md
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.623474 zigzag-dse-3.0.0/zigzag/classes/cacti/__pycache__/
--rw-r--r--   0 asymons  (27005) micas     (3600)     3547 2024-02-27 13:47:53.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.751479 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/
--rw-r--r--   0 asymons  (27005) micas     (3600)     6576 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     6555 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     6920 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     5324 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/README
--rw-r--r--   0 asymons  (27005) micas     (3600)     9282 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/TSV.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3322 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/TSV.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    41184 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/Ucache.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3607 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/Ucache.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     5116 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/arbiter.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2771 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/arbiter.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     2057 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/area.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2416 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/area.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     8474 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/bank.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2664 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/bank.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    29279 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/basic_circuit.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     7364 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/basic_circuit.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    11041 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cache.cfg_temp
--rw-r--r--   0 asymons  (27005) micas     (3600)    32713 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
--rwxr-xr-x   0 asymons  (27005) micas     (3600)  2421320 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti
--rw-r--r--   0 asymons  (27005) micas     (3600)      173 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti.i
--rw-r--r--   0 asymons  (27005) micas     (3600)     1334 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti.mk
--rw-r--r--   0 asymons  (27005) micas     (3600)    25297 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5586 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_interface.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)    27215 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_interface.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     3747 2024-02-27 14:13:55.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_top.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7561 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/component.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2837 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/component.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     9565 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/const.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     5001 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/contention.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     7349 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/crossbar.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3204 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/crossbar.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     9849 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/ddr3.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)    62337 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/decoder.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     7405 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/decoder.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     3712 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/dram.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     9750 2024-03-19 15:11:36.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
--rw-r--r--   0 asymons  (27005) micas     (3600)    17411 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)      878 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    46185 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio_technology.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     9068 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio_technology.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    23772 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/htree2.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3595 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/htree2.h
--rw-r--r--   0 asymons  (27005) micas     (3600)   133713 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/io.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2116 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/io.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     9850 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/lpddr.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     7217 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/main.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)      407 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/makefile
--rw-r--r--   0 asymons  (27005) micas     (3600)    94813 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/mat.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     6122 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/mat.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    16630 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)      553 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    11483 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     4490 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad_parameters.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    29014 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memorybus.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     5426 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memorybus.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    19629 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/nuca.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3306 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/nuca.h
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.840483 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/
--rw-r--r--   0 asymons  (27005) micas     (3600)   134304 2024-01-03 17:20:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   352744 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   157960 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   124352 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   156624 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   155192 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
--rwxr-xr-x   0 asymons  (27005) micas     (3600)  2421320 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
--rw-r--r--   0 asymons  (27005) micas     (3600)   175768 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   159768 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   160680 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   207224 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   145592 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   180464 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   178384 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   411960 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   192248 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   270320 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   569648 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   280416 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   204480 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   256824 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   313848 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   124400 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   175432 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   128080 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   144976 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   228000 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   232752 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
--rw-r--r--   0 asymons  (27005) micas     (3600)   111980 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/parameter.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)    20306 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/parameter.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     5286 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/powergating.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3055 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/powergating.h
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1886 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/regression.test
--rw-r--r--   0 asymons  (27005) micas     (3600)    10212 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/router.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     3721 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/router.h
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.849483 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8781 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     8768 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     8780 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)     8784 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.853483 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/self_gen/
--rw-r--r--   0 asymons  (27005) micas     (3600)     9545 2024-03-19 15:11:38.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
--rw-r--r--   0 asymons  (27005) micas     (3600)      579 2024-03-19 15:11:40.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
--rw-r--r--   0 asymons  (27005) micas     (3600)     8332 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/subarray.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     2542 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/subarray.h
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.871484 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/
--rw-r--r--   0 asymons  (27005) micas     (3600)       25 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    23666 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     3842 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4575 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4759 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4755 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    24571 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4758 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    24570 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)     4742 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
--rw-r--r--   0 asymons  (27005) micas     (3600)    15087 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/technology.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)    41317 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/uca.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     4035 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/uca.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     2064 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/version_cacti.h
--rw-r--r--   0 asymons  (27005) micas     (3600)    29856 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/wire.cc
--rw-r--r--   0 asymons  (27005) micas     (3600)     4375 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/wire.h
--rw-r--r--   0 asymons  (27005) micas     (3600)     7626 2024-02-27 13:47:51.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_parser.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.873484 zigzag-dse-3.0.0/zigzag/classes/cacti/self_gen/
--rw-r--r--   0 asymons  (27005) micas     (3600)     9549 2024-02-27 13:04:58.000000 zigzag-dse-3.0.0/zigzag/classes/cacti/self_gen/cache.cfg
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.877484 zigzag-dse-3.0.0/zigzag/classes/cost_model/
--rw-r--r--   0 asymons  (27005) micas     (3600)    66253 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/cost_model/cost_model.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    20548 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/cost_model/cost_model_for_sram_imc.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.547471 zigzag-dse-3.0.0/zigzag/classes/hardware/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.903485 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/
--rw-r--r--   0 asymons  (27005) micas     (3600)    22537 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/AimcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    40916 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/DimcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2102 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/ImcArray.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1207 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/accelerator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9229 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/adder_hierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6468 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/core.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      877 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/dimension.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    32673 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/get_cacti_cost.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    10610 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/imc_unit.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    11471 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/memory_hierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3781 2024-02-21 09:50:55.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/memory_instance.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    12113 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/memory_level.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3096 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/operational_array.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1742 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/operational_unit.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.550471 zigzag-dse-3.0.0/zigzag/classes/io/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.905485 zigzag-dse-3.0.0/zigzag/classes/io/accelerator/
--rw-r--r--   0 asymons  (27005) micas     (3600)     2799 2024-02-01 21:03:54.000000 zigzag-dse-3.0.0/zigzag/classes/io/accelerator/parser.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.917486 zigzag-dse-3.0.0/zigzag/classes/io/onnx/
--rw-r--r--   0 asymons  (27005) micas     (3600)     7699 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/io/onnx/conv.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      976 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/io/onnx/default.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5776 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/io/onnx/gemm.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     4073 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/io/onnx/matmul.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5079 2024-02-05 12:45:14.000000 zigzag-dse-3.0.0/zigzag/classes/io/onnx/model.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1311 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/io/onnx/parser.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7792 2024-02-05 12:45:09.000000 zigzag-dse-3.0.0/zigzag/classes/io/onnx/utils.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.922486 zigzag-dse-3.0.0/zigzag/classes/mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)    40589 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/mapping/combined_mapping.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/mapping/loop.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9463 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/mapping/mapping_assist_funcs.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.924486 zigzag-dse-3.0.0/zigzag/classes/mapping/memory/
--rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/mapping/memory/data_layout.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.925486 zigzag-dse-3.0.0/zigzag/classes/mapping/spatial/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8091 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/mapping/spatial/spatial_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.928486 zigzag-dse-3.0.0/zigzag/classes/mapping/temporal/
--rw-r--r--   0 asymons  (27005) micas     (3600)      442 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/mapping/temporal/temporal_loop.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7328 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/mapping/temporal/temporal_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.556471 zigzag-dse-3.0.0/zigzag/classes/opt/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.930487 zigzag-dse-3.0.0/zigzag/classes/opt/spatial/
--rw-r--r--   0 asymons  (27005) micas     (3600)    50477 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/opt/spatial/generator.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.557471 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.936487 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/
--rw-r--r--   0 asymons  (27005) micas     (3600)    11540 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/engine.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      534 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/loop.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    16495 2024-02-21 09:50:55.000000 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/memory_allocator.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2901 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/multipermute.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.939487 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/salsa/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8704 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/salsa/engine.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3571 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/opt/temporal/salsa/state.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.969488 zigzag-dse-3.0.0/zigzag/classes/stages/
--rw-r--r--   0 asymons  (27005) micas     (3600)     3338 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/stages/CostModelStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1503 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/DumpStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3212 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/GeneralParameterIteratorStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2087 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/LomaStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2245 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/MainInputParserStages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      989 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/ONNXModelParserStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5834 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/PEArrayScalingStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1522 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/PlotTemporalMappingsStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5951 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/ReduceStages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9522 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/RemoveUnusedMemoryStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6158 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/RunOptStages.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     6449 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/SalsaStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7298 2024-03-19 15:05:18.000000 zigzag-dse-3.0.0/zigzag/classes/stages/SaveStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    30038 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/SearchUnusedMemoryStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    21259 2024-02-21 09:50:55.000000 zigzag-dse-3.0.0/zigzag/classes/stages/SpatialMappingConversionStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    14699 2024-02-21 09:50:55.000000 zigzag-dse-3.0.0/zigzag/classes/stages/SpatialMappingGeneratorStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2520 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/Stage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3834 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/TemporalOrderingConversionStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2110 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/classes/stages/WorkloadStage.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2906 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/stages/__init__.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.977489 zigzag-dse-3.0.0/zigzag/classes/workload/
--rw-r--r--   0 asymons  (27005) micas     (3600)     2477 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/workload/dnn_workload.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     2033 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/workload/dummy_node.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    21581 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/workload/layer_node.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1352 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/workload/onnx_workload.py
--rw-r--r--   0 asymons  (27005) micas     (3600)    14521 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/classes/workload/test_layer_node.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.564471 zigzag-dse-3.0.0/zigzag/inputs/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.563471 zigzag-dse-3.0.0/zigzag/inputs/examples/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.989489 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    10181 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Aimc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     8496 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     9857 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Dimc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5897 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Edge_TPU_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5817 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Eyeriss_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7146 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Meta_prototype.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     5162 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/TPU_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     7335 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.999489 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/
--rw-r--r--   0 asymons  (27005) micas     (3600)      561 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/ascend_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      196 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/default.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)      566 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/default_imc.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      832 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/edge_tpu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      560 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/meta_prototype_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      610 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/tesla_npu_like.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      557 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/tpu_like.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:20.005490 zigzag-dse-3.0.0/zigzag/inputs/examples/workload/
--rw-r--r--   0 asymons  (27005) micas     (3600)     4067 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/workload/alexnet.onnx
--rw-r--r--   0 asymons  (27005) micas     (3600)    71724 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/workload/mobilenetv2.onnx
--rw-r--r--   0 asymons  (27005) micas     (3600)    18600 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/workload/resnet18.onnx
--rw-r--r--   0 asymons  (27005) micas     (3600)    19065 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/inputs/examples/workload/resnet18.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.564471 zigzag-dse-3.0.0/zigzag/inputs/validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.565471 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.567471 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.566471 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:20.015490 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     7275 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     9625 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     7893 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1584 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     6082 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    12159 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.568472 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:20.024490 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    12159 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     5910 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     1723 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)    13681 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     7526 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py
--rwxr-xr-x   0 asymons  (27005) micas     (3600)     3566 2024-03-19 14:49:36.000000 zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py
--rw-r--r--   0 asymons  (27005) micas     (3600)      736 2024-01-03 17:30:21.000000 zigzag-dse-3.0.0/zigzag/utils.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:19.570472 zigzag-dse-3.0.0/zigzag/visualization/
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:20.027491 zigzag-dse-3.0.0/zigzag/visualization/graph/
--rw-r--r--   0 asymons  (27005) micas     (3600)     1527 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/visualization/graph/memory_hierarchy.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     1280 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/visualization/graph/workload.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:20.030491 zigzag-dse-3.0.0/zigzag/visualization/results/
--rw-r--r--   0 asymons  (27005) micas     (3600)     8785 2024-03-19 14:52:57.000000 zigzag-dse-3.0.0/zigzag/visualization/results/plot_cme.py
--rw-r--r--   0 asymons  (27005) micas     (3600)     3951 2024-01-03 17:20:41.000000 zigzag-dse-3.0.0/zigzag/visualization/results/print_mapping.py
-drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-03-19 15:14:20.044491 zigzag-dse-3.0.0/zigzag_dse.egg-info/
--rw-r--r--   0 asymons  (27005) micas     (3600)    10722 2024-03-19 15:14:19.000000 zigzag-dse-3.0.0/zigzag_dse.egg-info/PKG-INFO
--rw-r--r--   0 asymons  (27005) micas     (3600)    12231 2024-03-19 15:14:19.000000 zigzag-dse-3.0.0/zigzag_dse.egg-info/SOURCES.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)        1 2024-03-19 15:14:19.000000 zigzag-dse-3.0.0/zigzag_dse.egg-info/dependency_links.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)       52 2024-03-19 15:14:19.000000 zigzag-dse-3.0.0/zigzag_dse.egg-info/entry_points.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)      144 2024-03-19 15:14:19.000000 zigzag-dse-3.0.0/zigzag_dse.egg-info/requires.txt
--rw-r--r--   0 asymons  (27005) micas     (3600)       18 2024-03-19 15:14:19.000000 zigzag-dse-3.0.0/zigzag_dse.egg-info/top_level.txt
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.806481 zigzag_dse-3.1.0/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1074 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/LICENSE
+-rw-r--r--   0 asymons  (27005) micas     (3600)       88 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/MANIFEST.in
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10722 2024-04-15 09:56:04.803480 zigzag_dse-3.1.0/PKG-INFO
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8519 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/README.md
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1601 2024-04-15 09:51:10.000000 zigzag_dse-3.1.0/pyproject.toml
+-rw-r--r--   0 asymons  (27005) micas     (3600)       38 2024-04-15 09:56:04.806481 zigzag_dse-3.1.0/setup.cfg
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.046449 zigzag_dse-3.1.0/tests/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.051449 zigzag_dse-3.1.0/tests/main/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.104452 zigzag_dse-3.1.0/tests/main/test_imc/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/tests/main/test_imc/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1572 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/tests/main/test_imc/test_aimc.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1545 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/tests/main/test_imc/test_dimc.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.117452 zigzag_dse-3.1.0/tests/main/test_origin/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1253 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1261 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1266 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1262 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1250 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_origin/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.131452 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2044 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2690 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2118 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2087 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2378 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.143453 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1284 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1303 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1315 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1309 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1294 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.151453 zigzag_dse-3.1.0/zigzag/
+-rw-r--r--   0 asymons  (27005) micas     (3600)       22 2024-04-15 09:51:10.000000 zigzag_dse-3.1.0/zigzag/__init__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2497 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/__main__.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    19803 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/api.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.152453 zigzag_dse-3.1.0/zigzag/classes/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/__init__.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.156453 zigzag_dse-3.1.0/zigzag/classes/cacti/
+-rw-r--r--   0 asymons  (27005) micas     (3600)      291 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/README.md
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.157454 zigzag_dse-3.1.0/zigzag/classes/cacti/__pycache__/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3547 2024-02-27 13:47:53.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.316460 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6576 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6555 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6920 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5324 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/README
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9282 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/TSV.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3322 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/TSV.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    41184 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/Ucache.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3607 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/Ucache.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5116 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/arbiter.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2771 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/arbiter.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2057 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/area.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2416 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/area.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8474 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/bank.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2664 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/bank.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    29279 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/basic_circuit.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7364 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/basic_circuit.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    11041 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cache.cfg_temp
+-rw-r--r--   0 asymons  (27005) micas     (3600)    32713 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cache_old.cfg.out
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)  2421320 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti
+-rw-r--r--   0 asymons  (27005) micas     (3600)      173 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti.i
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1334 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti.mk
+-rw-r--r--   0 asymons  (27005) micas     (3600)    25297 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5586 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_interface.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)    27215 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_interface.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3747 2024-02-27 14:13:55.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_top.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7561 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/component.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2837 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/component.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9565 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/const.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5001 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/contention.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7349 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/crossbar.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3204 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/crossbar.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9849 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/ddr3.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)    62337 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/decoder.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7405 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/decoder.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3712 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/dram.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9750 2024-03-19 15:11:36.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml
+-rw-r--r--   0 asymons  (27005) micas     (3600)    17411 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)      878 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    46185 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio_technology.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9068 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio_technology.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    23772 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/htree2.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3595 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/htree2.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)   133713 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/io.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2116 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/io.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9850 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/lpddr.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7217 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/main.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)      407 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/makefile
+-rw-r--r--   0 asymons  (27005) micas     (3600)    94813 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/mat.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6122 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/mat.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    16630 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)      553 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    11483 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad_parameters.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4490 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad_parameters.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    29014 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memorybus.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5426 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memorybus.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    19629 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/nuca.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3306 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/nuca.h
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.456466 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/
+-rw-r--r--   0 asymons  (27005) micas     (3600)   134304 2024-01-03 17:20:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   352744 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   157960 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   124352 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/area.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   156624 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   155192 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)  2421320 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti
+-rw-r--r--   0 asymons  (27005) micas     (3600)   175768 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   159768 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/component.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   160680 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   207224 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   145592 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   180464 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   178384 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   411960 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/io.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   192248 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/main.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   270320 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   569648 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   280416 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   204480 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   256824 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   313848 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   124400 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   175432 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/router.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   128080 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   144976 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   228000 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   232752 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
+-rw-r--r--   0 asymons  (27005) micas     (3600)   111980 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/parameter.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)    20306 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/parameter.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5286 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/powergating.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3055 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/powergating.h
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     1886 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/regression.test
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10212 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/router.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3721 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/router.h
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.468466 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8781 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8768 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8780 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8784 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.515468 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9545 2024-03-19 15:11:38.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      579 2024-03-19 15:11:40.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 09:35:55.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8238395692842152875.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 09:35:55.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8238395692842152875.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:53:15.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8667919883845363313.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:53:15.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_-8667919883845363313.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 09:35:38.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2159937366902611545.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 09:35:38.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2159937366902611545.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:49:21.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2582313971359678716.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:49:22.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_2582313971359678716.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:40:34.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_3347886556911868882.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:40:35.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_3347886556911868882.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_6701911052272027327.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_6701911052272027327.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9580 2024-04-15 08:36:19.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_748814760220054032.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-04-15 08:36:20.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_748814760220054032.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9578 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_a.cfg
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3720 2024-04-15 09:40:56.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache_a.cfg.out
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8332 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/subarray.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2542 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/subarray.h
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.539469 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/
+-rw-r--r--   0 asymons  (27005) micas     (3600)       25 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)    23666 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3842 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4575 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4759 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4755 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)    24571 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4758 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)    24570 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4742 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat
+-rw-r--r--   0 asymons  (27005) micas     (3600)    15087 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/technology.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)    41317 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/uca.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4035 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/uca.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2064 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/version_cacti.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)    29856 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/wire.cc
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4375 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/wire.h
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7626 2024-02-27 13:47:51.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_parser.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.541469 zigzag_dse-3.1.0/zigzag/classes/cacti/self_gen/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9549 2024-02-27 13:04:58.000000 zigzag_dse-3.1.0/zigzag/classes/cacti/self_gen/cache.cfg
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.547470 zigzag_dse-3.1.0/zigzag/classes/cost_model/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    66253 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    20548 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model_for_sram_imc.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.065450 zigzag_dse-3.1.0/zigzag/classes/hardware/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.583471 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    22537 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/AimcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    40916 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/DimcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2102 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/ImcArray.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1207 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/accelerator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9229 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/adder_hierarchy.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6468 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/core.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      877 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/dimension.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    32673 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/get_cacti_cost.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10610 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/imc_unit.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    11471 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_hierarchy.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3781 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_instance.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    12113 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_level.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3096 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_array.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1742 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_unit.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.068450 zigzag_dse-3.1.0/zigzag/classes/io/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.585471 zigzag_dse-3.1.0/zigzag/classes/io/accelerator/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2799 2024-02-01 21:03:54.000000 zigzag_dse-3.1.0/zigzag/classes/io/accelerator/parser.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.604472 zigzag_dse-3.1.0/zigzag/classes/io/onnx/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7699 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/conv.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      976 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/default.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5776 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/gemm.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4073 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/matmul.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5079 2024-02-05 12:45:14.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/model.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1311 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/parser.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7792 2024-02-05 12:45:09.000000 zigzag_dse-3.1.0/zigzag/classes/io/onnx/utils.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.612472 zigzag_dse-3.1.0/zigzag/classes/mapping/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    40589 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/combined_mapping.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      578 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/loop.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9463 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/mapping_assist_funcs.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.614472 zigzag_dse-3.1.0/zigzag/classes/mapping/memory/
+-rw-r--r--   0 asymons  (27005) micas     (3600)        0 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/memory/data_layout.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.617473 zigzag_dse-3.1.0/zigzag/classes/mapping/spatial/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8091 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/spatial/spatial_mapping.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.622473 zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/
+-rw-r--r--   0 asymons  (27005) micas     (3600)      442 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/temporal_loop.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7328 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/temporal_mapping.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.075450 zigzag_dse-3.1.0/zigzag/classes/opt/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.625473 zigzag_dse-3.1.0/zigzag/classes/opt/spatial/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    50477 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/opt/spatial/generator.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.077450 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.636474 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    11540 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/engine.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      534 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/loop.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    16495 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/memory_allocator.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2901 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/multipermute.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.641474 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8704 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/engine.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3571 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/state.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.692476 zigzag_dse-3.1.0/zigzag/classes/stages/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3338 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/stages/CostModelStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1503 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/DumpStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3212 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/GeneralParameterIteratorStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2087 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/LomaStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2245 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/MainInputParserStages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      989 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/ONNXModelParserStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5834 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/PEArrayScalingStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1522 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/PlotTemporalMappingsStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5951 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/ReduceStages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9522 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/RemoveUnusedMemoryStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6158 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/RunOptStages.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     6449 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SalsaStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7298 2024-03-19 15:05:18.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SaveStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    30038 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SearchUnusedMemoryStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    21259 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SpatialMappingConversionStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    14699 2024-02-21 09:50:55.000000 zigzag_dse-3.1.0/zigzag/classes/stages/SpatialMappingGeneratorStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2520 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/Stage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     3834 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/TemporalOrderingConversionStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2110 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/classes/stages/WorkloadStage.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2906 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/stages/__init__.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.704476 zigzag_dse-3.1.0/zigzag/classes/workload/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2771 2024-04-15 08:09:03.000000 zigzag_dse-3.1.0/zigzag/classes/workload/dnn_workload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     2033 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/workload/dummy_node.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    20779 2024-04-15 08:33:58.000000 zigzag_dse-3.1.0/zigzag/classes/workload/layer_node.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1352 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/workload/onnx_workload.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)    14521 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/classes/workload/test_layer_node.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.084451 zigzag_dse-3.1.0/zigzag/inputs/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.083451 zigzag_dse-3.1.0/zigzag/inputs/examples/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.723477 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    10181 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Aimc.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8496 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     9857 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Dimc.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5897 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Edge_TPU_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5817 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Eyeriss_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7146 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Meta_prototype.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     5162 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/TPU_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     7335 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Tesla_NPU_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.739478 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/
+-rw-r--r--   0 asymons  (27005) micas     (3600)      561 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/ascend_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      196 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/default.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)      566 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/default_imc.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      832 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/edge_tpu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      560 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/meta_prototype_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      610 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/tesla_npu_like.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      557 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/tpu_like.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.749478 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4067 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/alexnet.onnx
+-rw-r--r--   0 asymons  (27005) micas     (3600)    71724 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/mobilenetv2.onnx
+-rw-r--r--   0 asymons  (27005) micas     (3600)    18600 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/resnet18.onnx
+-rw-r--r--   0 asymons  (27005) micas     (3600)    19065 2024-04-15 09:48:52.000000 zigzag_dse-3.1.0/zigzag/inputs/examples/workload/resnet18.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.084451 zigzag_dse-3.1.0/zigzag/inputs/validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.085451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.088451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.087451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.764479 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     7275 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     9625 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     7893 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     1584 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     6082 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    12159 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.089451 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.778479 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    12159 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     5910 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     1723 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)    13681 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     7526 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py
+-rwxr-xr-x   0 asymons  (27005) micas     (3600)     3566 2024-03-19 14:49:36.000000 zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)      736 2024-01-03 17:30:21.000000 zigzag_dse-3.1.0/zigzag/utils.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.091451 zigzag_dse-3.1.0/zigzag/visualization/
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.782479 zigzag_dse-3.1.0/zigzag/visualization/graph/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1527 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/visualization/graph/memory_hierarchy.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     1280 2024-01-03 17:20:41.000000 zigzag_dse-3.1.0/zigzag/visualization/graph/workload.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.786480 zigzag_dse-3.1.0/zigzag/visualization/results/
+-rw-r--r--   0 asymons  (27005) micas     (3600)     8785 2024-03-19 14:52:57.000000 zigzag_dse-3.1.0/zigzag/visualization/results/plot_cme.py
+-rw-r--r--   0 asymons  (27005) micas     (3600)     4220 2024-04-15 08:09:03.000000 zigzag_dse-3.1.0/zigzag/visualization/results/print_mapping.py
+drwxr-xr-x   0 asymons  (27005) micas     (3600)        0 2024-04-15 09:56:04.801480 zigzag_dse-3.1.0/zigzag_dse.egg-info/
+-rw-r--r--   0 asymons  (27005) micas     (3600)    10722 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/PKG-INFO
+-rw-r--r--   0 asymons  (27005) micas     (3600)    13397 2024-04-15 09:56:04.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/SOURCES.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)        1 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/dependency_links.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)       52 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/entry_points.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)      144 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/requires.txt
+-rw-r--r--   0 asymons  (27005) micas     (3600)       18 2024-04-15 09:56:03.000000 zigzag_dse-3.1.0/zigzag_dse.egg-info/top_level.txt
```

### Comparing `zigzag-dse-3.0.0/LICENSE` & `zigzag_dse-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/PKG-INFO` & `zigzag_dse-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 3.0.0
+Version: 3.1.0
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2021 MICAS (KU Leuven)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zigzag-dse-3.0.0/README.md` & `zigzag_dse-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/pyproject.toml` & `zigzag_dse-3.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["."]  # ["."] by default
 include = ["*"]  # ["*"] by default
 exclude = ["inputs*", "outputs*", "docs*"]
 namespaces = true  # true by default
 
 [project]
 name = "zigzag-dse"
-version = "3.0.0"
+version = "3.1.0"
 description = "ZigZag - Deep Learning Hardware Design Space Exploration"
 readme = "README.md"
 authors = [{ name = "Arne Symons", email = "arne.symons@kuleuven.be" }, { name = "Linyan Mei", email = "linyan.mei@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
 [project.urls]
 Homepage = "https://github.com/ZigZag-Project/zigzag"
 
 [project.scripts]
 realpython = "zigzag.__main__:main"
 
 [tool.bumpver]
-current_version = "3.0.0"
+current_version = "3.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zigzag-dse-3.0.0/tests/main/test_imc/test_aimc.py` & `zigzag_dse-3.1.0/tests/main/test_imc/test_aimc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_imc/test_dimc.py` & `zigzag_dse-3.1.0/tests/main/test_imc/test_dimc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_origin/test_ascend_like.py` & `zigzag_dse-3.1.0/tests/main/test_origin/test_ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_origin/test_edge_tpu_like.py` & `zigzag_dse-3.1.0/tests/main/test_origin/test_edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_origin/test_meta_prototype_like.py` & `zigzag_dse-3.1.0/tests/main/test_origin/test_meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_origin/test_tesla_npu_like.py` & `zigzag_dse-3.1.0/tests/main/test_origin/test_tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_origin/test_tpu_like.py` & `zigzag_dse-3.1.0/tests/main/test_origin/test_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py` & `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py` & `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py` & `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py` & `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py` & `zigzag_dse-3.1.0/tests/main/test_with_mix_spatial_mapping/test_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_ascend_like.py` & `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_edge_tpu_like.py` & `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_meta_prototype_like.py` & `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_tesla_npu_like.py` & `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/tests/main/test_without_unused_memory/test_tpu_like.py` & `zigzag_dse-3.1.0/tests/main/test_without_unused_memory/test_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/__main__.py` & `zigzag_dse-3.1.0/zigzag/__main__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/api.py` & `zigzag_dse-3.1.0/zigzag/api.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/__pycache__/cacti_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/2DDRAM_Samsung2GbDDR2.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/2DDRAM_micron1Gb.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/3DDRAM_Samsung3D8Gb_extened.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/README` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/README`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/TSV.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/TSV.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/TSV.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/TSV.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/Ucache.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/Ucache.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/Ucache.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/Ucache.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/arbiter.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/arbiter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/arbiter.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/arbiter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/area.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/area.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/area.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/area.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/bank.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/bank.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/bank.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/bank.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/basic_circuit.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/basic_circuit.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/basic_circuit.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/basic_circuit.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cache.cfg_temp` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cache.cfg_temp`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cache_old.cfg.out` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cache_old.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti.mk` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti.mk`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_config_creator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_interface.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_interface.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_interface.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_interface.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/cacti_top.py` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/cacti_top.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/component.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/component.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/component.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/component.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/const.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/const.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/contention.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/contention.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/crossbar.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/crossbar.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/crossbar.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/crossbar.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/ddr3.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/ddr3.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/decoder.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/decoder.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/decoder.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/decoder.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/dram.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/dram.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/example_mem_pool.yaml`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio_technology.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio_technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/extio_technology.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/extio_technology.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/htree2.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/htree2.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/htree2.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/htree2.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/io.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/io.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/io.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/io.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/lpddr.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/lpddr.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/main.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/main.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/mat.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/mat.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/mat.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/mat.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad_parameters.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad_parameters.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memcad_parameters.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memcad_parameters.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memorybus.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memorybus.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/memorybus.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/memorybus.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/nuca.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/nuca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/nuca.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/nuca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/TSV.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/Ucache.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/arbiter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/area.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/area.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/bank.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/basic_circuit.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/cacti_interface.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/component.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/component.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/crossbar.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/decoder.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/extio_technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/htree2.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/io.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/io.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/main.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/main.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/mat.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memcad_parameters.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/memorybus.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/nuca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/parameter.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/powergating.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/router.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/router.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/subarray.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/technology.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/uca.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/obj_dbg/wire.o`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/parameter.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/parameter.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/parameter.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/parameter.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/powergating.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/powergating.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/powergating.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/powergating.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/regression.test` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/regression.test`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/router.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/router.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/router.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/router.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/subarray.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/subarray.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/subarray.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/subarray.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/180nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/22nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/32nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/45nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/65nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/90nm-old.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/tech_params/90nm.dat`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/technology.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/technology.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/uca.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/uca.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/uca.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/uca.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/version_cacti.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/version_cacti.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/wire.cc` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/wire.cc`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_master/wire.h` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_master/wire.h`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/cacti_parser.py` & `zigzag_dse-3.1.0/zigzag/classes/cacti/cacti_parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cacti/self_gen/cache.cfg` & `zigzag_dse-3.1.0/zigzag/classes/cacti/self_gen/cache.cfg`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cost_model/cost_model.py` & `zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/cost_model/cost_model_for_sram_imc.py` & `zigzag_dse-3.1.0/zigzag/classes/cost_model/cost_model_for_sram_imc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/AimcArray.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/AimcArray.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/DimcArray.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/DimcArray.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/ImcArray.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/ImcArray.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/accelerator.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/accelerator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/adder_hierarchy.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/adder_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/core.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/core.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/dimension.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/dimension.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/get_cacti_cost.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/get_cacti_cost.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/imc_unit.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/imc_unit.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/memory_hierarchy.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/memory_instance.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_instance.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/memory_level.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/memory_level.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/operational_array.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_array.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/hardware/architecture/operational_unit.py` & `zigzag_dse-3.1.0/zigzag/classes/hardware/architecture/operational_unit.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/accelerator/parser.py` & `zigzag_dse-3.1.0/zigzag/classes/io/accelerator/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/onnx/conv.py` & `zigzag_dse-3.1.0/zigzag/classes/io/onnx/conv.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/onnx/default.py` & `zigzag_dse-3.1.0/zigzag/classes/io/onnx/default.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/onnx/gemm.py` & `zigzag_dse-3.1.0/zigzag/classes/io/onnx/gemm.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/onnx/matmul.py` & `zigzag_dse-3.1.0/zigzag/classes/io/onnx/matmul.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/onnx/model.py` & `zigzag_dse-3.1.0/zigzag/classes/io/onnx/model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/onnx/parser.py` & `zigzag_dse-3.1.0/zigzag/classes/io/onnx/parser.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/io/onnx/utils.py` & `zigzag_dse-3.1.0/zigzag/classes/io/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/mapping/combined_mapping.py` & `zigzag_dse-3.1.0/zigzag/classes/mapping/combined_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/mapping/loop.py` & `zigzag_dse-3.1.0/zigzag/classes/mapping/loop.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/mapping/mapping_assist_funcs.py` & `zigzag_dse-3.1.0/zigzag/classes/mapping/mapping_assist_funcs.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/mapping/spatial/spatial_mapping.py` & `zigzag_dse-3.1.0/zigzag/classes/mapping/spatial/spatial_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/mapping/temporal/temporal_mapping.py` & `zigzag_dse-3.1.0/zigzag/classes/mapping/temporal/temporal_mapping.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/opt/spatial/generator.py` & `zigzag_dse-3.1.0/zigzag/classes/opt/spatial/generator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/engine.py` & `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/loop.py` & `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/loop.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/memory_allocator.py` & `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/opt/temporal/loma/multipermute.py` & `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/loma/multipermute.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/opt/temporal/salsa/engine.py` & `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/engine.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/opt/temporal/salsa/state.py` & `zigzag_dse-3.1.0/zigzag/classes/opt/temporal/salsa/state.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/CostModelStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/CostModelStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/DumpStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/DumpStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/GeneralParameterIteratorStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/GeneralParameterIteratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/LomaStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/LomaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/MainInputParserStages.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/MainInputParserStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/ONNXModelParserStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/ONNXModelParserStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/PEArrayScalingStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/PEArrayScalingStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/PlotTemporalMappingsStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/PlotTemporalMappingsStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/ReduceStages.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/ReduceStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/RemoveUnusedMemoryStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/RemoveUnusedMemoryStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/RunOptStages.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/RunOptStages.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/SalsaStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/SalsaStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/SaveStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/SaveStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/SearchUnusedMemoryStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/SearchUnusedMemoryStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/SpatialMappingConversionStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/SpatialMappingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/SpatialMappingGeneratorStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/SpatialMappingGeneratorStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/Stage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/Stage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/TemporalOrderingConversionStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/TemporalOrderingConversionStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/WorkloadStage.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/WorkloadStage.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/stages/__init__.py` & `zigzag_dse-3.1.0/zigzag/classes/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/workload/dnn_workload.py` & `zigzag_dse-3.1.0/zigzag/classes/workload/dnn_workload.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,22 +18,27 @@
         self.layer_node_list = []
 
         for layer_id, layer in workload.items():
             # TODO Support other type of layers, such as concatenation, max pooling, BN, etc.
             #  What is special about max pooling?
             # elif type(layer_id) == str and layer_id[0:6] == 'concat':
             #     continue
-            if layer["operator_type"] in mapping.keys():
-                for attr_name, attr_va in mapping[layer["operator_type"]].items():
+            layer_name = layer.get("name", f"Layer {layer_id}")
+            operator_type = layer.get("operator_type", None)
+            if layer_name in mapping.keys():
+                for attr_name, attr_va in mapping[layer_name].items():
+                    layer[attr_name] = attr_va
+            elif operator_type in mapping.keys():
+                for attr_name, attr_va in mapping[operator_type].items():
                     layer[attr_name] = attr_va
             else:
                 for attr_name, attr_va in mapping["default"].items():
                     layer[attr_name] = attr_va
             # For each item in the dict generate the LayerNode and add it to the dnn graph G
-            layer_node = LayerNode(layer_id, layer)
+            layer_node = LayerNode(layer_id, layer, node_name=layer_name)
             # Save this layer_id and LayerNode pair in the layer_id_to_obj dict
             layer_id_to_obj[layer_id] = layer_node
             # self.add_node(layer_id, info=layer_node)
             self.add_node(layer_node)
             self.layer_node_list.append(layer_node)
             # Find all of its operand sources and add edges accordingly
             edges = []
```

### Comparing `zigzag-dse-3.0.0/zigzag/classes/workload/dummy_node.py` & `zigzag_dse-3.1.0/zigzag/classes/workload/dummy_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/workload/layer_node.py` & `zigzag_dse-3.1.0/zigzag/classes/workload/layer_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
         return pr_loop, pr_loop_list, pr_scaling_factors
 
     def get_core_allocation(self):
         return self.core_allocation
 
     def __str__(self):
-        return f"LayerNode_{self.id}"
+        return f"{self.name}"
 
     def __repr__(self):
         return str(self)
 
     ## JSON representation used for saving this object to a json file.
     def __jsonrepr__(self):
         return {
@@ -265,45 +265,30 @@
         return eval("lambda n: " + equal_sign_right)
 
     def extract_pr_loop_info(self, equation_relations):
         pr_loop: Dict[str, list] = {}
         pr_loop_list: List[str] = []
         pr_scaling_factors: Dict[str, list] = {}
         padding: Dict[str, int] = {}
+        # Regex pattern to find dimensions and coefficients of form dim1 = coef_2*dim2 + coef_3*dim3
+        pattern = r"(\w+)\s*=\s*(?:(\w+)\s*\*\s*)?(\w+)\s*\+\s*(?:(\w+)\s*\*\s*)?(\w+)"
         for relation in equation_relations:
-            relation_disassembly = re.findall("[a-zA-Z]+", relation)
+            match = re.search(pattern, relation)
+            if match:
+                dim1, coef_2, dim2, coef_3, dim3 = match.groups()
+                coef_2 = int(coef_2) if coef_2 is not None else 1
+                coef_3 = int(coef_3) if coef_3 is not None else 1
+            else:
+                raise ValueError(f"Please make sure {relation} is of the form 'dim1 = a*dim2 + b*dim3'")
 
-            assert (
-                len(relation_disassembly) == 3
-            ), f"equation_relation {relation} does not involve a linear relationship between two dimension iterators."
-
-            key = relation_disassembly[0].upper()
-            val = [loop_dim.upper() for loop_dim in relation_disassembly[1:]]
+            key = dim1.upper()
+            val = (dim2.upper(), dim3.upper())
             pr_loop[key] = val
-            pr_loop_list.extend([key] + val)
-
-            # To extract the scaling factors for the different loop dimension iterators, we need to make sure
-            # there is a scaling factor present in the equation. If it is not present, raise an exception.
-            scaling_factors = {}
-            for val_lower in relation_disassembly[1:]:
-                if relation[relation.index(val_lower) - 1] == "*":
-                    if not relation[relation.index(val_lower) - 2].isdigit():
-                        raise NotImplementedError(
-                            f"Please use a scaling factor for every dimension iterator on the RHS of equation {relation}"
-                        )
-                    else:
-                        scaling_factors[val_lower] = int(
-                            re.findall("(\\d+)(?=\\*" + val_lower + ")", relation)[0]
-                        )
-                else:
-                    scaling_factors[val_lower] = 1
-            # scaling_factors = re.findall('[0-9]+', relation)
-            assert (
-                len(scaling_factors) == 2
-            ), f"Please remove any constants in the equation relation {relation}."
+            pr_loop_list.extend((key,) + val)
+            scaling_factors = {dim2: coef_2, dim3: coef_3}
             pr_scaling_factors[key] = scaling_factors
 
         return pr_loop, pr_loop_list, pr_scaling_factors
 
     @staticmethod
     def extract_r_ir_loop_info(equation, loop_dim_size, pr_loop, pr_loop_list):
         operand_loop_dim: Dict[str, Dict] = {}
```

### Comparing `zigzag-dse-3.0.0/zigzag/classes/workload/onnx_workload.py` & `zigzag_dse-3.1.0/zigzag/classes/workload/onnx_workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/classes/workload/test_layer_node.py` & `zigzag_dse-3.1.0/zigzag/classes/workload/test_layer_node.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Aimc.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Aimc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Ascend_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Dimc.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Dimc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Edge_TPU_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Edge_TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Eyeriss_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Eyeriss_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Meta_prototype.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Meta_prototype.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/TPU_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/TPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/hardware/Tesla_NPU_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/hardware/Tesla_NPU_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/ascend_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/ascend_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/default_imc.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/default_imc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/edge_tpu_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/edge_tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/meta_prototype_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/meta_prototype_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/tesla_npu_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/tesla_npu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/mapping/tpu_like.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/mapping/tpu_like.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/workload/alexnet.onnx` & `zigzag_dse-3.1.0/zigzag/inputs/examples/workload/alexnet.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/workload/mobilenetv2.onnx` & `zigzag_dse-3.1.0/zigzag/inputs/examples/workload/mobilenetv2.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/workload/resnet18.onnx` & `zigzag_dse-3.1.0/zigzag/inputs/examples/workload/resnet18.onnx`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/examples/workload/resnet18.py` & `zigzag_dse-3.1.0/zigzag/inputs/examples/workload/resnet18.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc1_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc2_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc3_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/aimc_validation.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/aimc_validation/22-28nm/dimc_cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_cost_model.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation4.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/dimc_validation_subfunc4.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py` & `zigzag_dse-3.1.0/zigzag/inputs/validation/hardware/sram_imc/dimc_validation/28nm/model_extration_28nm.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/utils.py` & `zigzag_dse-3.1.0/zigzag/utils.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/visualization/graph/memory_hierarchy.py` & `zigzag_dse-3.1.0/zigzag/visualization/graph/memory_hierarchy.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/visualization/graph/workload.py` & `zigzag_dse-3.1.0/zigzag/visualization/graph/workload.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag/visualization/results/plot_cme.py` & `zigzag_dse-3.1.0/zigzag/visualization/results/plot_cme.py`

 * *Files identical despite different names*

### Comparing `zigzag-dse-3.0.0/zigzag_dse.egg-info/PKG-INFO` & `zigzag_dse-3.1.0/zigzag_dse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigzag-dse
-Version: 3.0.0
+Version: 3.1.0
 Summary: ZigZag - Deep Learning Hardware Design Space Exploration
 Author-email: Arne Symons <arne.symons@kuleuven.be>, Linyan Mei <linyan.mei@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2021 MICAS (KU Leuven)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zigzag-dse-3.0.0/zigzag_dse.egg-info/SOURCES.txt` & `zigzag_dse-3.1.0/zigzag_dse.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,30 @@
 zigzag/classes/cacti/cacti_master/obj_dbg/wire.o
 zigzag/classes/cacti/cacti_master/sample_config_files/ddr3_cache.cfg
 zigzag/classes/cacti/cacti_master/sample_config_files/diff_ddr3_cache.cfg
 zigzag/classes/cacti/cacti_master/sample_config_files/lpddr3_cache.cfg
 zigzag/classes/cacti/cacti_master/sample_config_files/wideio_cache.cfg
 zigzag/classes/cacti/cacti_master/self_gen/cache.cfg
 zigzag/classes/cacti/cacti_master/self_gen/cache.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_-8238395692842152875.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_-8238395692842152875.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_-8667919883845363313.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_-8667919883845363313.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_2159937366902611545.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_2159937366902611545.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_2582313971359678716.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_2582313971359678716.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_3347886556911868882.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_3347886556911868882.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_6701911052272027327.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_6701911052272027327.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_748814760220054032.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_748814760220054032.cfg.out
+zigzag/classes/cacti/cacti_master/self_gen/cache_a.cfg
+zigzag/classes/cacti/cacti_master/self_gen/cache_a.cfg.out
 zigzag/classes/cacti/cacti_master/tech_params/16nm.dat
 zigzag/classes/cacti/cacti_master/tech_params/180nm-old.dat
 zigzag/classes/cacti/cacti_master/tech_params/180nm.dat
 zigzag/classes/cacti/cacti_master/tech_params/22nm.dat
 zigzag/classes/cacti/cacti_master/tech_params/32nm.dat
 zigzag/classes/cacti/cacti_master/tech_params/45nm.dat
 zigzag/classes/cacti/cacti_master/tech_params/65nm-old.dat
```

