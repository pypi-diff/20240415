# Comparing `tmp/mqt_qmap-2.5.0.tar.gz` & `tmp/mqt_qmap-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt_qmap-2.5.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "mqt_qmap-2.5.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `mqt_qmap-2.5.0.tar` & `mqt_qmap-2.5.1.tar`

### file list

```diff
@@ -1,502 +1,501 @@
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.clang-format
--rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.clang-tidy
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.cmake-format.yaml
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.git_archival.txt
--rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.gitattributes
--rw-r--r--   0        0        0     2009 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.gitignore
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.gitmodules
--rw-r--r--   0        0        0     3174 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      947 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1818 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/CMakeLists.txt
--rw-r--r--   0        0        0     1116 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/LICENSE.md
--rw-r--r--   0        0        0     6965 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/README.md
--rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/cmake/ExternalDependencies.cmake
--rw-r--r--   0        0        0     6040 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/cmake/FindZ3.cmake
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/cmake/try_z3.cpp
--rw-r--r--   0        0        0     2493 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/0410184_169.qasm
--rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/3_17_13.qasm
--rw-r--r--   0        0        0     2466 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4_49_16.qasm
--rw-r--r--   0        0        0     1692 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt10-v1_81.qasm
--rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt11_82.qasm
--rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt11_83.qasm
--rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt11_84.qasm
--rw-r--r--   0        0        0     2852 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt12-v0_86.qasm
--rw-r--r--   0        0        0     2796 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt12-v0_87.qasm
--rw-r--r--   0        0        0     2198 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt12-v0_88.qasm
--rw-r--r--   0        0        0     2566 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt12-v1_89.qasm
--rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt13-v1_93.qasm
--rw-r--r--   0        0        0     1268 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt13_90.qasm
--rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt13_91.qasm
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt13_92.qasm
--rw-r--r--   0        0        0     2896 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt4-v0_72.qasm
--rw-r--r--   0        0        0     4436 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt4-v0_73.qasm
--rw-r--r--   0        0        0     2676 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt4-v0_78.qasm
--rw-r--r--   0        0        0     2620 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt4-v0_79.qasm
--rw-r--r--   0        0        0     2030 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt4-v0_80.qasm
--rw-r--r--   0        0        0     3058 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt4-v1_74.qasm
--rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt5_75.qasm
--rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt5_76.qasm
--rw-r--r--   0        0        0     1502 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4gt5_77.qasm
--rw-r--r--   0        0        0      828 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod5-bdd_287.qasm
--rw-r--r--   0        0        0      820 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod5-v0_18.qasm
--rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod5-v0_19.qasm
--rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod5-v0_20.qasm
--rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod5-v1_22.qasm
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod5-v1_23.qasm
--rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod5-v1_24.qasm
--rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod7-v0_94.qasm
--rw-r--r--   0        0        0     1862 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/4mod7-v1_96.qasm
--rw-r--r--   0        0        0   392516 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/9symml_195.qasm
--rw-r--r--   0        0        0     5198 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/C17_204.qasm
--rw-r--r--   0        0        0    39954 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/adr4_197.qasm
--rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/aj-e11_165.qasm
--rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-bdd_288.qasm
--rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v0_26.qasm
--rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v0_27.qasm
--rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v1_28.qasm
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v1_29.qasm
--rw-r--r--   0        0        0     5614 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v2_30.qasm
--rw-r--r--   0        0        0     5022 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v2_31.qasm
--rw-r--r--   0        0        0     1854 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v2_32.qasm
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v2_33.qasm
--rw-r--r--   0        0        0      636 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v3_34.qasm
--rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v3_35.qasm
--rw-r--r--   0        0        0     1326 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v4_36.qasm
--rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/alu-v4_37.qasm
--rw-r--r--   0        0        0   391826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/clip_206.qasm
--rw-r--r--   0        0        0    14286 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/cm152a_212.qasm
--rw-r--r--   0        0        0    20843 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/cm42a_207.qasm
--rw-r--r--   0        0        0     7196 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/cm82a_208.qasm
--rw-r--r--   0        0        0   131904 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/cm85a_209.qasm
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/cnt3-5_179.qasm
--rw-r--r--   0        0        0     5770 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/cnt3-5_180.qasm
--rw-r--r--   0        0        0   208397 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/co14_215.qasm
--rw-r--r--   0        0        0    10534 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/con1_216.qasm
--rw-r--r--   0        0        0    69118 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/cycle10_2_110.qasm
--rw-r--r--   0        0        0    21415 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/dc1_220.qasm
--rw-r--r--   0        0        0   110003 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/dc2_222.qasm
--rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/decod24-bdd_294.qasm
--rw-r--r--   0        0        0     3782 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/decod24-enable_126.qasm
--rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/decod24-v0_38.qasm
--rw-r--r--   0        0        0      996 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/decod24-v1_41.qasm
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/decod24-v2_43.qasm
--rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/decod24-v3_45.qasm
--rw-r--r--   0        0        0   437419 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/dist_223.qasm
--rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ex-1_166.qasm
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ex1_226.qasm
--rw-r--r--   0        0        0     6990 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ex2_227.qasm
--rw-r--r--   0        0        0     4482 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ex3_229.qasm
--rw-r--r--   0        0        0    13306 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/f2_232.qasm
--rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/graycode6_47.qasm
--rw-r--r--   0        0        0  4363639 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ground_state_estimation_10.qasm
--rw-r--r--   0        0        0      661 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_0.qasm
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_1.qasm
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_2.qasm
--rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_3.qasm
--rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_4.qasm
--rw-r--r--   0        0        0      577 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_5.qasm
--rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_6.qasm
--rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_7.qasm
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_8.qasm
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_3_9.qasm
--rw-r--r--   0        0        0     1354 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_0.qasm
--rw-r--r--   0        0        0      708 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_1.qasm
--rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_2.qasm
--rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_4.qasm
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_5.qasm
--rw-r--r--   0        0        0     1116 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_6.qasm
--rw-r--r--   0        0        0     1462 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_7.qasm
--rw-r--r--   0        0        0     1818 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_8.qasm
--rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_4_9.qasm
--rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_0.qasm
--rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_1.qasm
--rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_2.qasm
--rw-r--r--   0        0        0     1775 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_3.qasm
--rw-r--r--   0        0        0     1891 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_4.qasm
--rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_5.qasm
--rw-r--r--   0        0        0     1825 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_6.qasm
--rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_8.qasm
--rw-r--r--   0        0        0     1319 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/grover/grover_5_9.qasm
--rw-r--r--   0        0        0   105189 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ham15_107.qasm
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ham3_102.qasm
--rw-r--r--   0        0        0     3626 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ham7_104.qasm
--rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/hwb4_49.qasm
--rw-r--r--   0        0        0    14826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/hwb5_53.qasm
--rw-r--r--   0        0        0    74068 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/hwb6_56.qasm
--rw-r--r--   0        0        0   268308 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/hwb7_59.qasm
--rw-r--r--   0        0        0   763334 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/hwb8_113.qasm
--rw-r--r--   0        0        0  2285870 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/hwb9_119.qasm
--rw-r--r--   0        0        0   126570 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/inc_237.qasm
--rw-r--r--   0        0        0     6471 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ising_model_10.qasm
--rw-r--r--   0        0        0     8523 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ising_model_13.qasm
--rw-r--r--   0        0        0    10590 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/ising_model_16.qasm
--rw-r--r--   0        0        0   252636 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/life_238.qasm
--rw-r--r--   0        0        0     6784 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/majority_239.qasm
--rw-r--r--   0        0        0   298284 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/max46_240.qasm
--rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/miller_11.qasm
--rw-r--r--   0        0        0     3226 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mini-alu_167.qasm
--rw-r--r--   0        0        0     1966 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mini_alu_305.qasm
--rw-r--r--   0        0        0    57016 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/misex1_241.qasm
--rw-r--r--   0        0        0   221059 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mlp4_245.qasm
--rw-r--r--   0        0        0     2748 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod10_171.qasm
--rw-r--r--   0        0        0     2016 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod10_176.qasm
--rw-r--r--   0        0        0     6136 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod5adder_127.qasm
--rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod5d1_63.qasm
--rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod5d2_64.qasm
--rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod5mils_65.qasm
--rw-r--r--   0        0        0     4916 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod8-10_177.qasm
--rw-r--r--   0        0        0     3832 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/mod8-10_178.qasm
--rw-r--r--   0        0        0     3254 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/one-two-three-v0_97.qasm
--rw-r--r--   0        0        0     1670 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/one-two-three-v0_98.qasm
--rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/one-two-three-v1_99.qasm
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/one-two-three-v2_100.qasm
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/one-two-three-v3_101.qasm
--rw-r--r--   0        0        0  1490891 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/plus63mod4096_163.qasm
--rw-r--r--   0        0        0  2193234 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/plus63mod8192_164.qasm
--rw-r--r--   0        0        0    20843 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/pm1_249.qasm
--rwxr-xr-x   0        0        0     2177 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/qe_qft_4.qasm
--rwxr-xr-x   0        0        0     3359 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/qe_qft_5.qasm
--rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/qelib1.inc
--rw-r--r--   0        0        0     3101 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/qft_10.qasm
--rw-r--r--   0        0        0     8240 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/qft_16.qasm
--rw-r--r--   0        0        0    37214 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/radd_250.qasm
--rw-r--r--   0        0        0      438 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd32-v0_66.qasm
--rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd32-v1_68.qasm
--rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd32_270.qasm
--rw-r--r--   0        0        0    11474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd53_130.qasm
--rw-r--r--   0        0        0     5178 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd53_131.qasm
--rw-r--r--   0        0        0     6450 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd53_133.qasm
--rw-r--r--   0        0        0     3338 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd53_135.qasm
--rw-r--r--   0        0        0     1522 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd53_138.qasm
--rw-r--r--   0        0        0    14250 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd53_251.qasm
--rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd53_311.qasm
--rw-r--r--   0        0        0     2608 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd73_140.qasm
--rw-r--r--   0        0        0    58528 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd73_252.qasm
--rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd84_142.qasm
--rw-r--r--   0        0        0   155519 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/rd84_253.qasm
--rw-r--r--   0        0        0   197202 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/root_255.qasm
--rw-r--r--   0        0        0   454252 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sao2_257.qasm
--rw-r--r--   0        0        0     8610 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sf_274.qasm
--rw-r--r--   0        0        0     8586 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sf_276.qasm
--rw-r--r--   0        0        0   112420 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sqn_258.qasm
--rw-r--r--   0        0        0    34411 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sqrt8_260.qasm
--rw-r--r--   0        0        0    22929 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/squar5_261.qasm
--rw-r--r--   0        0        0    85837 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/square_root_7.qasm
--rw-r--r--   0        0        0   738665 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sym10_262.qasm
--rw-r--r--   0        0        0    42826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sym6_145.qasm
--rw-r--r--   0        0        0     3177 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sym6_316.qasm
--rw-r--r--   0        0        0     3846 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sym9_146.qasm
--rw-r--r--   0        0        0   236604 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sym9_148.qasm
--rw-r--r--   0        0        0   392516 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sym9_193.qasm
--rw-r--r--   0        0        0     2446 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/sys6-v0_111.qasm
--rw-r--r--   0        0        0  2033562 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf1_149.qasm
--rw-r--r--   0        0        0   616794 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf1_278.qasm
--rw-r--r--   0        0        0   885338 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf2_152.qasm
--rw-r--r--   0        0        0   227956 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf2_277.qasm
--rw-r--r--   0        0        0  4658428 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf3_155.qasm
--rw-r--r--   0        0        0  1407914 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf3_279.qasm
--rw-r--r--   0        0        0  5679154 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf4_187.qasm
--rw-r--r--   0        0        0  1808634 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf5_158.qasm
--rw-r--r--   0        0        0   558434 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf5_280.qasm
--rw-r--r--   0        0        0  1973576 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/urf6_160.qasm
--rw-r--r--   0        0        0    11060 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/wim_266.qasm
--rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/xor5_254.qasm
--rw-r--r--   0        0        0    34394 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/examples/z4_268.qasm
--rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/ibm_qx4.arch
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/ibm_qx5.arch
--rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/ibmq_bogota.arch
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/ibmq_casablanca.arch
--rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/ibmq_london.arch
--rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/ibmq_tokyo.arch
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/ibmq_yorktown.arch
--rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/architectures/linear_10qubit.arch
--rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/calibration/ibmq_london.csv
--rw-r--r--   0        0        0     3906 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.cirrus.yml
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.clang-format
--rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.clang-tidy
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.cmake-format.yaml
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.git
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.git_archival.txt
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.gitattributes
--rw-r--r--   0        0        0     2009 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.gitignore
--rw-r--r--   0        0        0     3405 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/.readthedocs.yaml
--rwxr-xr-x   0        0        0     2786 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/CMakeLists.txt
--rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/LICENSE.md
--rw-r--r--   0        0        0     6778 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/README.md
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/Cache.cmake
--rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/CompilerOptions.cmake
--rw-r--r--   0        0        0     5318 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/CompilerWarnings.cmake
--rw-r--r--   0        0        0     3231 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/ExternalDependencies.cmake
--rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/FindGMP.cmake
--rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/GetVersion.cmake
--rw-r--r--   0        0        0      795 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/PackageAddTest.cmake
--rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/Sanitizers.cmake
--rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/StandardProjectSettings.cmake
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/cmake/mqt-core-config.cmake.in
--rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/eval/CMakeLists.txt
--rw-r--r--   0        0        0     8559 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/eval/eval_dd_package.cpp
--rw-r--r--   0        0        0     4046 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/CircuitOptimizer.hpp
--rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/Definitions.hpp
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/Permutation.hpp
--rw-r--r--   0        0        0    40622 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/QuantumComputation.hpp
--rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/BernsteinVazirani.hpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/Entanglement.hpp
--rw-r--r--   0        0        0     1528 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp
--rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/Grover.hpp
--rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/QFT.hpp
--rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/QPE.hpp
--rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/RandomCliffordCircuit.hpp
--rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/WState.hpp
--rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Benchmark.hpp
--rw-r--r--   0        0        0     5333 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/CachedEdge.hpp
--rw-r--r--   0        0        0     4947 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Complex.hpp
--rw-r--r--   0        0        0     4498 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/ComplexNumbers.hpp
--rw-r--r--   0        0        0     6127 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/ComplexValue.hpp
--rw-r--r--   0        0        0     3551 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/ComputeTable.hpp
--rw-r--r--   0        0        0     3723 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/DDDefinitions.hpp
--rw-r--r--   0        0        0     1491 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/DDpackageConfig.hpp
--rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/DensityNoiseTable.hpp
--rw-r--r--   0        0        0    15110 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Edge.hpp
--rw-r--r--   0        0        0    32823 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Export.hpp
--rw-r--r--   0        0        0     1459 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/FunctionalityConstruction.hpp
--rw-r--r--   0        0        0     6331 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/GateMatrixDefinitions.hpp
--rw-r--r--   0        0        0     6484 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/MemoryManager.hpp
--rw-r--r--   0        0        0     8048 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Node.hpp
--rw-r--r--   0        0        0    16737 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/NoiseFunctionality.hpp
--rw-r--r--   0        0        0    10072 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Operations.hpp
--rw-r--r--   0        0        0    84951 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Package.hpp
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Package_fwd.hpp
--rw-r--r--   0        0        0    10422 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/RealNumber.hpp
--rw-r--r--   0        0        0     8768 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/RealNumberUniqueTable.hpp
--rw-r--r--   0        0        0     1672 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Simulation.hpp
--rw-r--r--   0        0        0     2021 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/StochasticNoiseOperationTable.hpp
--rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/UnaryComputeTable.hpp
--rw-r--r--   0        0        0    12324 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/UniqueTable.hpp
--rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp
--rw-r--r--   0        0        0    11654 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/PackageStatistics.hpp
--rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/Statistics.hpp
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/TableStatistics.hpp
--rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp
--rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Ecc.hpp
--rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Id.hpp
--rw-r--r--   0        0        0     2452 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q18Surface.hpp
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q3Shor.hpp
--rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q5Laflamme.hpp
--rw-r--r--   0        0        0     1000 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q7Steane.hpp
--rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q9Shor.hpp
--rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q9Surface.hpp
--rw-r--r--   0        0        0     5179 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/ClassicControlledOperation.hpp
--rw-r--r--   0        0        0     4959 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/CompoundOperation.hpp
--rw-r--r--   0        0        0     1993 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/Control.hpp
--rw-r--r--   0        0        0    15630 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/Expression.hpp
--rw-r--r--   0        0        0     3508 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/NonUnitaryOperation.hpp
--rw-r--r--   0        0        0     6345 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/OpType.hpp
--rw-r--r--   0        0        0     6369 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/Operation.hpp
--rw-r--r--   0        0        0     4193 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/StandardOperation.hpp
--rw-r--r--   0        0        0     6218 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/SymbolicOperation.hpp
--rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Exception.hpp
--rw-r--r--   0        0        0     1359 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Gate.hpp
--rw-r--r--   0        0        0     5284 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp
--rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp
--rw-r--r--   0        0        0     5441 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Parser.hpp
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Scanner.hpp
--rw-r--r--   0        0        0    13570 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Statement.hpp
--rw-r--r--   0        0        0     7101 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/StdGates.hpp
--rw-r--r--   0        0        0     9447 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Token.hpp
--rw-r--r--   0        0        0     5987 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Types.hpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/CompilerPass.hpp
--rw-r--r--   0        0        0     5047 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp
--rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/python/pybind11.hpp
--rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/python/qiskit/QuantumCircuit.hpp
--rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/FunctionalityConstruction.hpp
--rw-r--r--   0        0        0     5874 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Rational.hpp
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Rules.hpp
--rw-r--r--   0        0        0     1688 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Simplify.hpp
--rw-r--r--   0        0        0     4335 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Utils.hpp
--rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/ZXDefinitions.hpp
--rw-r--r--   0        0        0     5135 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/ZXDiagram.hpp
--rw-r--r--   0        0        0     3143 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/noxfile.py
--rw-r--r--   0        0        0     8247 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/pyproject.toml
--rw-r--r--   0        0        0     9262 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/CMakeLists.txt
--rw-r--r--   0        0        0    51831 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/CircuitOptimizer.cpp
--rw-r--r--   0        0        0    35005 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/QuantumComputation.cpp
--rw-r--r--   0        0        0     3268 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/BernsteinVazirani.cpp
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/Entanglement.cpp
--rw-r--r--   0        0        0     4452 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/GoogleRandomCircuitSampling.cpp
--rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/Grover.cpp
--rw-r--r--   0        0        0     2721 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/QFT.cpp
--rw-r--r--   0        0        0     4327 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/QPE.cpp
--rw-r--r--   0        0        0     5790 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/RandomCliffordCircuit.cpp
--rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/WState.cpp
--rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/Benchmark.cpp
--rw-r--r--   0        0        0     1204 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/CMakeLists.txt
--rw-r--r--   0        0        0     5653 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/CachedEdge.cpp
--rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/Complex.cpp
--rw-r--r--   0        0        0     1805 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/ComplexNumbers.cpp
--rw-r--r--   0        0        0     8904 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/ComplexValue.cpp
--rw-r--r--   0        0        0    19407 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/Edge.cpp
--rw-r--r--   0        0        0     6299 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/FunctionalityConstruction.cpp
--rw-r--r--   0        0        0     2028 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/MemoryManager.cpp
--rw-r--r--   0        0        0     2437 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/Node.cpp
--rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/NoiseFunctionality.cpp
--rw-r--r--   0        0        0     4605 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/Operations.cpp
--rw-r--r--   0        0        0     3235 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/RealNumber.cpp
--rw-r--r--   0        0        0     9683 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/RealNumberUniqueTable.cpp
--rw-r--r--   0        0        0    16243 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/Simulation.cpp
--rw-r--r--   0        0        0     2914 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/statistics/MemoryManagerStatistics.cpp
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/statistics/Statistics.cpp
--rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/statistics/TableStatistics.cpp
--rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/dd/statistics/UniqueTableStatistics.cpp
--rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/CMakeLists.txt
--rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Ecc.cpp
--rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q18Surface.cpp
--rw-r--r--   0        0        0     4684 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q3Shor.cpp
--rw-r--r--   0        0        0     5422 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q5Laflamme.cpp
--rw-r--r--   0        0        0     8433 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q7Steane.cpp
--rw-r--r--   0        0        0     7053 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q9Shor.cpp
--rw-r--r--   0        0        0     5996 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q9Surface.cpp
--rw-r--r--   0        0        0      513 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/__init__.py
--rw-r--r--   0        0        0      954 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/__main__.py
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_compat/__init__.py
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_compat/typing.py
--rw-r--r--   0        0        0    16336 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_core/__init__.pyi
--rw-r--r--   0        0        0    12827 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_core/operations.pyi
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_core/symbolic.pyi
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_version.pyi
--rw-r--r--   0        0        0     1350 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/commands.py
--rw-r--r--   0        0        0    11961 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/evaluation.py
--rw-r--r--   0        0        0     1830 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/io.py
--rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/operations.py
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/plugins/__init__.py
--rw-r--r--   0        0        0    13175 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/plugins/qiskit.py
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/py.typed
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/symbolic.py
--rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/operations/ClassicControlledOperation.cpp
--rw-r--r--   0        0        0     4966 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/operations/CompoundOperation.cpp
--rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/operations/Expression.cpp
--rw-r--r--   0        0        0     6153 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/operations/NonUnitaryOperation.cpp
--rw-r--r--   0        0        0     4433 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/operations/Operation.cpp
--rw-r--r--   0        0        0    18185 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/operations/StandardOperation.cpp
--rw-r--r--   0        0        0    13162 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/operations/SymbolicOperation.cpp
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/GRCSParser.cpp
--rw-r--r--   0        0        0    31737 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/QASM3Parser.cpp
--rw-r--r--   0        0        0    10485 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/QCParser.cpp
--rw-r--r--   0        0        0     8949 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/RealParser.cpp
--rw-r--r--   0        0        0     8273 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/TFCParser.cpp
--rw-r--r--   0        0        0    26220 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Parser.cpp
--rw-r--r--   0        0        0    12777 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Scanner.cpp
--rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Statement.cpp
--rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Types.cpp
--rw-r--r--   0        0        0    17353 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp
--rw-r--r--   0        0        0    10210 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp
--rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/CMakeLists.txt
--rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/module.cpp
--rw-r--r--   0        0        0     1791 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_classic_controlled_operation.cpp
--rw-r--r--   0        0        0     3048 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_compound_operation.cpp
--rw-r--r--   0        0        0     1604 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_control.cpp
--rw-r--r--   0        0        0     1996 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_non_unitary_operation.cpp
--rw-r--r--   0        0        0     4168 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_operation.cpp
--rw-r--r--   0        0        0     2172 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_optype.cpp
--rw-r--r--   0        0        0     4525 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_standard_operation.cpp
--rw-r--r--   0        0        0     4540 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_symbolic_operation.cpp
--rw-r--r--   0        0        0    18393 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/qiskit/QuantumCircuit.cpp
--rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/register_operations.cpp
--rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/register_permutation.cpp
--rw-r--r--   0        0        0    25063 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/register_quantum_computation.cpp
--rw-r--r--   0        0        0      319 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/register_symbolic.cpp
--rw-r--r--   0        0        0     4638 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/symbolic/register_expression.cpp
--rw-r--r--   0        0        0     1794 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/symbolic/register_term.cpp
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/python/symbolic/register_variable.cpp
--rw-r--r--   0        0        0     3009 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/zx/CMakeLists.txt
--rw-r--r--   0        0        0    25831 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/zx/FunctionalityConstruction.cpp
--rw-r--r--   0        0        0     1809 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/zx/Rational.cpp
--rw-r--r--   0        0        0    10647 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/zx/Rules.cpp
--rw-r--r--   0        0        0     2829 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/zx/Simplify.cpp
--rw-r--r--   0        0        0     4310 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/zx/Utils.cpp
--rw-r--r--   0        0        0    11414 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/extern/mqt-core/src/zx/ZXDiagram.cpp
--rw-r--r--   0        0        0    19848 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/Architecture.hpp
--rw-r--r--   0        0        0     2929 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/DataLogger.hpp
--rw-r--r--   0        0        0    12296 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/Mapper.hpp
--rw-r--r--   0        0        0     6661 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/MappingResults.hpp
--rw-r--r--   0        0        0     6081 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/CliffordSynthesizer.hpp
--rw-r--r--   0        0        0     3161 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/Configuration.hpp
--rw-r--r--   0        0        0     3586 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/Results.hpp
--rw-r--r--   0        0        0     4964 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/Tableau.hpp
--rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/TargetMetric.hpp
--rw-r--r--   0        0        0     6140 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/GateEncoder.hpp
--rw-r--r--   0        0        0     1313 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/MultiGateEncoder.hpp
--rw-r--r--   0        0        0     2725 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/ObjectiveEncoder.hpp
--rw-r--r--   0        0        0     2709 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/SATEncoder.hpp
--rw-r--r--   0        0        0     1471 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/SingleGateEncoder.hpp
--rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/TableauEncoder.hpp
--rw-r--r--   0        0        0     4322 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/AvailableArchitecture.hpp
--rw-r--r--   0        0        0     1484 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/CommanderGrouping.hpp
--rw-r--r--   0        0        0     4175 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/Configuration.hpp
--rw-r--r--   0        0        0     2158 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/EarlyTermination.hpp
--rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/Encoding.hpp
--rw-r--r--   0        0        0     5592 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/Heuristic.hpp
--rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/InitialLayout.hpp
--rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/Layering.hpp
--rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/LookaheadHeuristic.hpp
--rw-r--r--   0        0        0      867 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/Method.hpp
--rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/configuration/SwapReduction.hpp
--rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/exact/ExactMapper.hpp
--rw-r--r--   0        0        0    17377 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/heuristic/HeuristicMapper.hpp
--rw-r--r--   0        0        0     4252 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/heuristic/UniquePriorityQueue.hpp
--rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/Encodings.hpp
--rw-r--r--   0        0        0     4962 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/Logic.hpp
--rw-r--r--   0        0        0     1647 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/LogicBlock.hpp
--rw-r--r--   0        0        0     7407 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/LogicTerm.hpp
--rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/Model.hpp
--rw-r--r--   0        0        0     4304 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/Z3Logic.hpp
--rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/Z3Model.hpp
--rw-r--r--   0        0        0     2809 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/logicblocks/util_logicblock.hpp
--rw-r--r--   0        0        0     6973 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/include/utils.hpp
--rw-r--r--   0        0        0     3164 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/noxfile.py
--rw-r--r--   0        0        0     8229 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    23988 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/Architecture.cpp
--rw-r--r--   0        0        0     3475 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/CMakeLists.txt
--rw-r--r--   0        0        0     9078 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/DataLogger.cpp
--rw-r--r--   0        0        0    20091 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/Mapper.cpp
--rw-r--r--   0        0        0    20963 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/CliffordSynthesizer.cpp
--rw-r--r--   0        0        0    13141 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/Tableau.cpp
--rw-r--r--   0        0        0    12221 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/GateEncoder.cpp
--rw-r--r--   0        0        0     6880 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/MultiGateEncoder.cpp
--rw-r--r--   0        0        0     2187 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/ObjectiveEncoder.cpp
--rw-r--r--   0        0        0     4750 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/SATEncoder.cpp
--rw-r--r--   0        0        0     7782 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/SingleGateEncoder.cpp
--rw-r--r--   0        0        0     5773 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/TableauEncoder.cpp
--rw-r--r--   0        0        0     2889 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/configuration/Configuration.cpp
--rw-r--r--   0        0        0    31730 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/exact/ExactMapper.cpp
--rw-r--r--   0        0        0    63067 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/heuristic/HeuristicMapper.cpp
--rw-r--r--   0        0        0      953 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/logicblocks/CMakeLists.txt
--rw-r--r--   0        0        0     5104 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/logicblocks/Encodings.cpp
--rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/logicblocks/LogicBlock.cpp
--rw-r--r--   0        0        0    19341 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/logicblocks/LogicTerm.cpp
--rw-r--r--   0        0        0    14528 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/logicblocks/Z3Logic.cpp
--rw-r--r--   0        0        0     1047 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/logicblocks/Z3Model.cpp
--rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/__init__.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/_version.py
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/_version.pyi
--rw-r--r--   0        0        0     7609 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/clifford_synthesis.py
--rw-r--r--   0        0        0     9526 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/compile.py
--rw-r--r--   0        0        0   171627 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/libs/ibm_guadalupe_16.pickle
--rw-r--r--   0        0        0   341613 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/libs/rigetti_16.pickle
--rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/load_architecture.py
--rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/load_calibration.py
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/py.typed
--rw-r--r--   0        0        0    17501 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/pyqmap.pyi
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/qiskit/backend.py
--rw-r--r--   0        0        0    16106 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/subarchitectures.py
--rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/visualization/__init__.py
--rw-r--r--   0        0        0    13850 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/visualization/search_visualizer.py
--rw-r--r--   0        0        0    90165 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/mqt/qmap/visualization/visualize_search_graph.py
--rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/python/CMakeLists.txt
--rw-r--r--   0        0        0    33293 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/python/bindings.cpp
--rw-r--r--   0        0        0    10035 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/src/utils.cpp
--rw-r--r--   0        0        0    11343 2022-11-09 12:37:21.000000 mqt_qmap-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.clang-format
+-rw-r--r--   0        0        0     2575 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.clang-tidy
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.cmake-format.yaml
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.git_archival.txt
+-rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.gitattributes
+-rw-r--r--   0        0        0     2009 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.gitignore
+-rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.gitmodules
+-rw-r--r--   0        0        0     3517 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      947 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1818 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1116 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/LICENSE.md
+-rw-r--r--   0        0        0     6965 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/README.md
+-rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/cmake/ExternalDependencies.cmake
+-rw-r--r--   0        0        0     6040 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/cmake/FindZ3.cmake
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/cmake/try_z3.cpp
+-rw-r--r--   0        0        0     2493 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/0410184_169.qasm
+-rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/3_17_13.qasm
+-rw-r--r--   0        0        0     2466 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4_49_16.qasm
+-rw-r--r--   0        0        0     1692 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt10-v1_81.qasm
+-rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt11_82.qasm
+-rw-r--r--   0        0        0      332 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt11_83.qasm
+-rw-r--r--   0        0        0      262 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt11_84.qasm
+-rw-r--r--   0        0        0     2852 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt12-v0_86.qasm
+-rw-r--r--   0        0        0     2796 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt12-v0_87.qasm
+-rw-r--r--   0        0        0     2198 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt12-v0_88.qasm
+-rw-r--r--   0        0        0     2566 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt12-v1_89.qasm
+-rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt13-v1_93.qasm
+-rw-r--r--   0        0        0     1268 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt13_90.qasm
+-rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt13_91.qasm
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt13_92.qasm
+-rw-r--r--   0        0        0     2896 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt4-v0_72.qasm
+-rw-r--r--   0        0        0     4436 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt4-v0_73.qasm
+-rw-r--r--   0        0        0     2676 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt4-v0_78.qasm
+-rw-r--r--   0        0        0     2620 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt4-v0_79.qasm
+-rw-r--r--   0        0        0     2030 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt4-v0_80.qasm
+-rw-r--r--   0        0        0     3058 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt4-v1_74.qasm
+-rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt5_75.qasm
+-rw-r--r--   0        0        0     1092 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt5_76.qasm
+-rw-r--r--   0        0        0     1502 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4gt5_77.qasm
+-rw-r--r--   0        0        0      828 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod5-bdd_287.qasm
+-rw-r--r--   0        0        0      820 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod5-v0_18.qasm
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod5-v0_19.qasm
+-rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod5-v0_20.qasm
+-rw-r--r--   0        0        0      298 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod5-v1_22.qasm
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod5-v1_23.qasm
+-rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod5-v1_24.qasm
+-rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod7-v0_94.qasm
+-rw-r--r--   0        0        0     1862 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/4mod7-v1_96.qasm
+-rw-r--r--   0        0        0   392516 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/9symml_195.qasm
+-rw-r--r--   0        0        0     5198 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/C17_204.qasm
+-rw-r--r--   0        0        0    39954 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/adr4_197.qasm
+-rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/aj-e11_165.qasm
+-rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-bdd_288.qasm
+-rw-r--r--   0        0        0      988 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v0_26.qasm
+-rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v0_27.qasm
+-rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v1_28.qasm
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v1_29.qasm
+-rw-r--r--   0        0        0     5614 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v2_30.qasm
+-rw-r--r--   0        0        0     5022 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v2_31.qasm
+-rw-r--r--   0        0        0     1854 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v2_32.qasm
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v2_33.qasm
+-rw-r--r--   0        0        0      636 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v3_34.qasm
+-rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v3_35.qasm
+-rw-r--r--   0        0        0     1326 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v4_36.qasm
+-rw-r--r--   0        0        0      474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/alu-v4_37.qasm
+-rw-r--r--   0        0        0   391826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/clip_206.qasm
+-rw-r--r--   0        0        0    14286 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/cm152a_212.qasm
+-rw-r--r--   0        0        0    20843 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/cm42a_207.qasm
+-rw-r--r--   0        0        0     7196 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/cm82a_208.qasm
+-rw-r--r--   0        0        0   131904 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/cm85a_209.qasm
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/cnt3-5_179.qasm
+-rw-r--r--   0        0        0     5770 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/cnt3-5_180.qasm
+-rw-r--r--   0        0        0   208397 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/co14_215.qasm
+-rw-r--r--   0        0        0    10534 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/con1_216.qasm
+-rw-r--r--   0        0        0    69118 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/cycle10_2_110.qasm
+-rw-r--r--   0        0        0    21415 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/dc1_220.qasm
+-rw-r--r--   0        0        0   110003 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/dc2_222.qasm
+-rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/decod24-bdd_294.qasm
+-rw-r--r--   0        0        0     3782 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/decod24-enable_126.qasm
+-rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/decod24-v0_38.qasm
+-rw-r--r--   0        0        0      996 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/decod24-v1_41.qasm
+-rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/decod24-v2_43.qasm
+-rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/decod24-v3_45.qasm
+-rw-r--r--   0        0        0   437419 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/dist_223.qasm
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ex-1_166.qasm
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ex1_226.qasm
+-rw-r--r--   0        0        0     6990 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ex2_227.qasm
+-rw-r--r--   0        0        0     4482 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ex3_229.qasm
+-rw-r--r--   0        0        0    13306 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/f2_232.qasm
+-rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/graycode6_47.qasm
+-rw-r--r--   0        0        0  4363639 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ground_state_estimation_10.qasm
+-rw-r--r--   0        0        0      661 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_0.qasm
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_1.qasm
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_2.qasm
+-rw-r--r--   0        0        0      621 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_3.qasm
+-rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_4.qasm
+-rw-r--r--   0        0        0      577 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_5.qasm
+-rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_6.qasm
+-rw-r--r--   0        0        0      273 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_7.qasm
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_8.qasm
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_3_9.qasm
+-rw-r--r--   0        0        0     1354 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_0.qasm
+-rw-r--r--   0        0        0      708 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_1.qasm
+-rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_2.qasm
+-rw-r--r--   0        0        0     1744 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_4.qasm
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_5.qasm
+-rw-r--r--   0        0        0     1116 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_6.qasm
+-rw-r--r--   0        0        0     1462 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_7.qasm
+-rw-r--r--   0        0        0     1818 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_8.qasm
+-rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_4_9.qasm
+-rw-r--r--   0        0        0     1109 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_0.qasm
+-rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_1.qasm
+-rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_2.qasm
+-rw-r--r--   0        0        0     1775 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_3.qasm
+-rw-r--r--   0        0        0     1891 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_4.qasm
+-rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_5.qasm
+-rw-r--r--   0        0        0     1825 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_6.qasm
+-rw-r--r--   0        0        0     1545 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_8.qasm
+-rw-r--r--   0        0        0     1319 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/grover/grover_5_9.qasm
+-rw-r--r--   0        0        0   105189 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ham15_107.qasm
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ham3_102.qasm
+-rw-r--r--   0        0        0     3626 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ham7_104.qasm
+-rw-r--r--   0        0        0     2648 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/hwb4_49.qasm
+-rw-r--r--   0        0        0    14826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/hwb5_53.qasm
+-rw-r--r--   0        0        0    74068 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/hwb6_56.qasm
+-rw-r--r--   0        0        0   268308 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/hwb7_59.qasm
+-rw-r--r--   0        0        0   763334 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/hwb8_113.qasm
+-rw-r--r--   0        0        0  2285870 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/hwb9_119.qasm
+-rw-r--r--   0        0        0   126570 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/inc_237.qasm
+-rw-r--r--   0        0        0     6471 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ising_model_10.qasm
+-rw-r--r--   0        0        0     8523 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ising_model_13.qasm
+-rw-r--r--   0        0        0    10590 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/ising_model_16.qasm
+-rw-r--r--   0        0        0   252636 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/life_238.qasm
+-rw-r--r--   0        0        0     6784 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/majority_239.qasm
+-rw-r--r--   0        0        0   298284 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/max46_240.qasm
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/miller_11.qasm
+-rw-r--r--   0        0        0     3226 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mini-alu_167.qasm
+-rw-r--r--   0        0        0     1966 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mini_alu_305.qasm
+-rw-r--r--   0        0        0    57016 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/misex1_241.qasm
+-rw-r--r--   0        0        0   221059 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mlp4_245.qasm
+-rw-r--r--   0        0        0     2748 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod10_171.qasm
+-rw-r--r--   0        0        0     2016 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod10_176.qasm
+-rw-r--r--   0        0        0     6136 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod5adder_127.qasm
+-rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod5d1_63.qasm
+-rw-r--r--   0        0        0      650 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod5d2_64.qasm
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod5mils_65.qasm
+-rw-r--r--   0        0        0     4916 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod8-10_177.qasm
+-rw-r--r--   0        0        0     3832 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/mod8-10_178.qasm
+-rw-r--r--   0        0        0     3254 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/one-two-three-v0_97.qasm
+-rw-r--r--   0        0        0     1670 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/one-two-three-v0_98.qasm
+-rw-r--r--   0        0        0     1516 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/one-two-three-v1_99.qasm
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/one-two-three-v2_100.qasm
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/one-two-three-v3_101.qasm
+-rw-r--r--   0        0        0  1490891 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/plus63mod4096_163.qasm
+-rw-r--r--   0        0        0  2193234 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/plus63mod8192_164.qasm
+-rw-r--r--   0        0        0    20843 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/pm1_249.qasm
+-rwxr-xr-x   0        0        0     2177 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/qe_qft_4.qasm
+-rwxr-xr-x   0        0        0     3359 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/qe_qft_5.qasm
+-rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/qelib1.inc
+-rw-r--r--   0        0        0     3101 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/qft_10.qasm
+-rw-r--r--   0        0        0     8240 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/qft_16.qasm
+-rw-r--r--   0        0        0    37214 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/radd_250.qasm
+-rw-r--r--   0        0        0      438 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd32-v0_66.qasm
+-rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd32-v1_68.qasm
+-rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd32_270.qasm
+-rw-r--r--   0        0        0    11474 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd53_130.qasm
+-rw-r--r--   0        0        0     5178 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd53_131.qasm
+-rw-r--r--   0        0        0     6450 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd53_133.qasm
+-rw-r--r--   0        0        0     3338 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd53_135.qasm
+-rw-r--r--   0        0        0     1522 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd53_138.qasm
+-rw-r--r--   0        0        0    14250 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd53_251.qasm
+-rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd53_311.qasm
+-rw-r--r--   0        0        0     2608 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd73_140.qasm
+-rw-r--r--   0        0        0    58528 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd73_252.qasm
+-rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd84_142.qasm
+-rw-r--r--   0        0        0   155519 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/rd84_253.qasm
+-rw-r--r--   0        0        0   197202 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/root_255.qasm
+-rw-r--r--   0        0        0   454252 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sao2_257.qasm
+-rw-r--r--   0        0        0     8610 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sf_274.qasm
+-rw-r--r--   0        0        0     8586 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sf_276.qasm
+-rw-r--r--   0        0        0   112420 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sqn_258.qasm
+-rw-r--r--   0        0        0    34411 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sqrt8_260.qasm
+-rw-r--r--   0        0        0    22929 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/squar5_261.qasm
+-rw-r--r--   0        0        0    85837 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/square_root_7.qasm
+-rw-r--r--   0        0        0   738665 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sym10_262.qasm
+-rw-r--r--   0        0        0    42826 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sym6_145.qasm
+-rw-r--r--   0        0        0     3177 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sym6_316.qasm
+-rw-r--r--   0        0        0     3846 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sym9_146.qasm
+-rw-r--r--   0        0        0   236604 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sym9_148.qasm
+-rw-r--r--   0        0        0   392516 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sym9_193.qasm
+-rw-r--r--   0        0        0     2446 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/sys6-v0_111.qasm
+-rw-r--r--   0        0        0  2033562 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf1_149.qasm
+-rw-r--r--   0        0        0   616794 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf1_278.qasm
+-rw-r--r--   0        0        0   885338 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf2_152.qasm
+-rw-r--r--   0        0        0   227956 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf2_277.qasm
+-rw-r--r--   0        0        0  4658428 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf3_155.qasm
+-rw-r--r--   0        0        0  1407914 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf3_279.qasm
+-rw-r--r--   0        0        0  5679154 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf4_187.qasm
+-rw-r--r--   0        0        0  1808634 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf5_158.qasm
+-rw-r--r--   0        0        0   558434 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf5_280.qasm
+-rw-r--r--   0        0        0  1973576 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/urf6_160.qasm
+-rw-r--r--   0        0        0    11060 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/wim_266.qasm
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/xor5_254.qasm
+-rw-r--r--   0        0        0    34394 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/examples/z4_268.qasm
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/ibm_qx4.arch
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/ibm_qx5.arch
+-rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/ibmq_bogota.arch
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/ibmq_casablanca.arch
+-rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/ibmq_london.arch
+-rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/ibmq_tokyo.arch
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/ibmq_yorktown.arch
+-rw-r--r--   0        0        0       75 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/architectures/linear_10qubit.arch
+-rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/calibration/ibmq_london.csv
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.clang-format
+-rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.clang-tidy
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.cmake-format.yaml
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.git
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.git_archival.txt
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.gitattributes
+-rw-r--r--   0        0        0     2009 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.gitignore
+-rw-r--r--   0        0        0     3529 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/.readthedocs.yaml
+-rwxr-xr-x   0        0        0     2786 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/CMakeLists.txt
+-rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/LICENSE.md
+-rw-r--r--   0        0        0     6778 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/README.md
+-rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/Cache.cmake
+-rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/CompilerOptions.cmake
+-rw-r--r--   0        0        0     5318 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/CompilerWarnings.cmake
+-rw-r--r--   0        0        0     3231 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/ExternalDependencies.cmake
+-rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/FindGMP.cmake
+-rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/GetVersion.cmake
+-rw-r--r--   0        0        0      795 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/PackageAddTest.cmake
+-rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/Sanitizers.cmake
+-rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/cmake/mqt-core-config.cmake.in
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/eval/CMakeLists.txt
+-rw-r--r--   0        0        0     8559 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/eval/eval_dd_package.cpp
+-rw-r--r--   0        0        0     4668 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/CircuitOptimizer.hpp
+-rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/Definitions.hpp
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/Permutation.hpp
+-rw-r--r--   0        0        0    41610 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/QuantumComputation.hpp
+-rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/BernsteinVazirani.hpp
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/Entanglement.hpp
+-rw-r--r--   0        0        0     1528 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/Grover.hpp
+-rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/QFT.hpp
+-rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/QPE.hpp
+-rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/RandomCliffordCircuit.hpp
+-rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/WState.hpp
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Benchmark.hpp
+-rw-r--r--   0        0        0     6105 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/CachedEdge.hpp
+-rw-r--r--   0        0        0     4947 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Complex.hpp
+-rw-r--r--   0        0        0     4498 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/ComplexNumbers.hpp
+-rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/ComplexValue.hpp
+-rw-r--r--   0        0        0     3619 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/ComputeTable.hpp
+-rw-r--r--   0        0        0     3723 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/DDDefinitions.hpp
+-rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/DDpackageConfig.hpp
+-rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/DensityNoiseTable.hpp
+-rw-r--r--   0        0        0    16220 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Edge.hpp
+-rw-r--r--   0        0        0    32823 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Export.hpp
+-rw-r--r--   0        0        0     1459 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/FunctionalityConstruction.hpp
+-rw-r--r--   0        0        0     6331 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/GateMatrixDefinitions.hpp
+-rw-r--r--   0        0        0     6484 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/MemoryManager.hpp
+-rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Node.hpp
+-rw-r--r--   0        0        0     4421 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/NoiseFunctionality.hpp
+-rw-r--r--   0        0        0     9048 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Operations.hpp
+-rw-r--r--   0        0        0    93777 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Package.hpp
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Package_fwd.hpp
+-rw-r--r--   0        0        0    10422 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/RealNumber.hpp
+-rw-r--r--   0        0        0     8768 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/RealNumberUniqueTable.hpp
+-rw-r--r--   0        0        0     1672 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Simulation.hpp
+-rw-r--r--   0        0        0     2021 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/StochasticNoiseOperationTable.hpp
+-rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/UnaryComputeTable.hpp
+-rw-r--r--   0        0        0    12308 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/UniqueTable.hpp
+-rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp
+-rw-r--r--   0        0        0    11654 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/PackageStatistics.hpp
+-rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/Statistics.hpp
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/TableStatistics.hpp
+-rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp
+-rw-r--r--   0        0        0     3103 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Ecc.hpp
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Id.hpp
+-rw-r--r--   0        0        0     2452 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q18Surface.hpp
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q3Shor.hpp
+-rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q5Laflamme.hpp
+-rw-r--r--   0        0        0     1000 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q7Steane.hpp
+-rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q9Shor.hpp
+-rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q9Surface.hpp
+-rw-r--r--   0        0        0     5055 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/ClassicControlledOperation.hpp
+-rw-r--r--   0        0        0     4923 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/CompoundOperation.hpp
+-rw-r--r--   0        0        0     1993 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/Control.hpp
+-rw-r--r--   0        0        0    15630 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/Expression.hpp
+-rw-r--r--   0        0        0     3600 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/NonUnitaryOperation.hpp
+-rw-r--r--   0        0        0     6345 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/OpType.hpp
+-rw-r--r--   0        0        0     6092 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/Operation.hpp
+-rw-r--r--   0        0        0     3590 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/StandardOperation.hpp
+-rw-r--r--   0        0        0     5717 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/SymbolicOperation.hpp
+-rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Exception.hpp
+-rw-r--r--   0        0        0     1359 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Gate.hpp
+-rw-r--r--   0        0        0     5284 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp
+-rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp
+-rw-r--r--   0        0        0     5441 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Parser.hpp
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Scanner.hpp
+-rw-r--r--   0        0        0    13570 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Statement.hpp
+-rw-r--r--   0        0        0     7101 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/StdGates.hpp
+-rw-r--r--   0        0        0     9447 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Token.hpp
+-rw-r--r--   0        0        0     5987 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Types.hpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/CompilerPass.hpp
+-rw-r--r--   0        0        0     5047 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp
+-rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp
+-rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/python/pybind11.hpp
+-rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/python/qiskit/QuantumCircuit.hpp
+-rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/FunctionalityConstruction.hpp
+-rw-r--r--   0        0        0     5874 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Rational.hpp
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Rules.hpp
+-rw-r--r--   0        0        0     1688 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Simplify.hpp
+-rw-r--r--   0        0        0     4335 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Utils.hpp
+-rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/ZXDefinitions.hpp
+-rw-r--r--   0        0        0     5135 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/ZXDiagram.hpp
+-rw-r--r--   0        0        0     3352 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/noxfile.py
+-rw-r--r--   0        0        0     8282 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/pyproject.toml
+-rw-r--r--   0        0        0     9262 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/CMakeLists.txt
+-rw-r--r--   0        0        0    59473 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/CircuitOptimizer.cpp
+-rw-r--r--   0        0        0    35083 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/QuantumComputation.cpp
+-rw-r--r--   0        0        0     3263 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/BernsteinVazirani.cpp
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/Entanglement.cpp
+-rw-r--r--   0        0        0     4387 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/GoogleRandomCircuitSampling.cpp
+-rw-r--r--   0        0        0     3073 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/Grover.cpp
+-rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/QFT.cpp
+-rw-r--r--   0        0        0     4317 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/QPE.cpp
+-rw-r--r--   0        0        0     5785 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/RandomCliffordCircuit.cpp
+-rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/WState.cpp
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/Benchmark.cpp
+-rw-r--r--   0        0        0     1204 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/CMakeLists.txt
+-rw-r--r--   0        0        0     5653 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/CachedEdge.cpp
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/Complex.cpp
+-rw-r--r--   0        0        0     1805 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/ComplexNumbers.cpp
+-rw-r--r--   0        0        0     8904 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/ComplexValue.cpp
+-rw-r--r--   0        0        0    21653 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/Edge.cpp
+-rw-r--r--   0        0        0     6592 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/FunctionalityConstruction.cpp
+-rw-r--r--   0        0        0     2028 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/MemoryManager.cpp
+-rw-r--r--   0        0        0     2437 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/Node.cpp
+-rw-r--r--   0        0        0    16109 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/NoiseFunctionality.cpp
+-rw-r--r--   0        0        0     4408 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/Operations.cpp
+-rw-r--r--   0        0        0     3235 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/RealNumber.cpp
+-rw-r--r--   0        0        0     9683 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/RealNumberUniqueTable.cpp
+-rw-r--r--   0        0        0    16155 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/Simulation.cpp
+-rw-r--r--   0        0        0     2914 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/statistics/MemoryManagerStatistics.cpp
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/statistics/Statistics.cpp
+-rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/statistics/TableStatistics.cpp
+-rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/dd/statistics/UniqueTableStatistics.cpp
+-rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/CMakeLists.txt
+-rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Ecc.cpp
+-rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q18Surface.cpp
+-rw-r--r--   0        0        0     4465 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q3Shor.cpp
+-rw-r--r--   0        0        0     5384 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q5Laflamme.cpp
+-rw-r--r--   0        0        0     8164 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q7Steane.cpp
+-rw-r--r--   0        0        0     6993 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q9Shor.cpp
+-rw-r--r--   0        0        0     5996 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q9Surface.cpp
+-rw-r--r--   0        0        0      513 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/__init__.py
+-rw-r--r--   0        0        0      954 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/__main__.py
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_compat/__init__.py
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_compat/typing.py
+-rw-r--r--   0        0        0    16637 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_core/__init__.pyi
+-rw-r--r--   0        0        0    11935 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_core/operations.pyi
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_core/symbolic.pyi
+-rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_version.pyi
+-rw-r--r--   0        0        0     1350 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/commands.py
+-rw-r--r--   0        0        0    11961 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/evaluation.py
+-rw-r--r--   0        0        0     1814 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/io.py
+-rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/operations.py
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/plugins/__init__.py
+-rw-r--r--   0        0        0    13057 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/plugins/qiskit.py
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/py.typed
+-rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/symbolic.py
+-rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/operations/ClassicControlledOperation.cpp
+-rw-r--r--   0        0        0     4850 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/operations/CompoundOperation.cpp
+-rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/operations/Expression.cpp
+-rw-r--r--   0        0        0     6254 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/operations/NonUnitaryOperation.cpp
+-rw-r--r--   0        0        0     4489 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/operations/Operation.cpp
+-rw-r--r--   0        0        0    16967 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/operations/StandardOperation.cpp
+-rw-r--r--   0        0        0    12020 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/operations/SymbolicOperation.cpp
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/GRCSParser.cpp
+-rw-r--r--   0        0        0    31466 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/QASM3Parser.cpp
+-rw-r--r--   0        0        0    10467 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/QCParser.cpp
+-rw-r--r--   0        0        0     8912 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/RealParser.cpp
+-rw-r--r--   0        0        0     8273 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/TFCParser.cpp
+-rw-r--r--   0        0        0    26220 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Parser.cpp
+-rw-r--r--   0        0        0    13173 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Scanner.cpp
+-rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Statement.cpp
+-rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Types.cpp
+-rw-r--r--   0        0        0    17353 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp
+-rw-r--r--   0        0        0    10210 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp
+-rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/CMakeLists.txt
+-rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/module.cpp
+-rw-r--r--   0        0        0     1784 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_classic_controlled_operation.cpp
+-rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_compound_operation.cpp
+-rw-r--r--   0        0        0     1604 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_control.cpp
+-rw-r--r--   0        0        0     1886 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_non_unitary_operation.cpp
+-rw-r--r--   0        0        0     3932 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_operation.cpp
+-rw-r--r--   0        0        0     2172 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_optype.cpp
+-rw-r--r--   0        0        0     3843 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_standard_operation.cpp
+-rw-r--r--   0        0        0     4031 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_symbolic_operation.cpp
+-rw-r--r--   0        0        0    18179 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/qiskit/QuantumCircuit.cpp
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/register_operations.cpp
+-rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/register_permutation.cpp
+-rw-r--r--   0        0        0    25756 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/register_quantum_computation.cpp
+-rw-r--r--   0        0        0      319 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/register_symbolic.cpp
+-rw-r--r--   0        0        0     4638 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/symbolic/register_expression.cpp
+-rw-r--r--   0        0        0     1794 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/symbolic/register_term.cpp
+-rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/python/symbolic/register_variable.cpp
+-rw-r--r--   0        0        0     3009 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/zx/CMakeLists.txt
+-rw-r--r--   0        0        0    25831 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/zx/FunctionalityConstruction.cpp
+-rw-r--r--   0        0        0     1809 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/zx/Rational.cpp
+-rw-r--r--   0        0        0    10647 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/zx/Rules.cpp
+-rw-r--r--   0        0        0     2829 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/zx/Simplify.cpp
+-rw-r--r--   0        0        0     4310 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/zx/Utils.cpp
+-rw-r--r--   0        0        0    11414 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/extern/mqt-core/src/zx/ZXDiagram.cpp
+-rw-r--r--   0        0        0    19848 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/Architecture.hpp
+-rw-r--r--   0        0        0     2929 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/DataLogger.hpp
+-rw-r--r--   0        0        0    12296 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/Mapper.hpp
+-rw-r--r--   0        0        0     6661 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/MappingResults.hpp
+-rw-r--r--   0        0        0     6081 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/CliffordSynthesizer.hpp
+-rw-r--r--   0        0        0     3161 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/Configuration.hpp
+-rw-r--r--   0        0        0     3586 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/Results.hpp
+-rw-r--r--   0        0        0     4964 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/Tableau.hpp
+-rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/TargetMetric.hpp
+-rw-r--r--   0        0        0     6140 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/GateEncoder.hpp
+-rw-r--r--   0        0        0     1313 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/MultiGateEncoder.hpp
+-rw-r--r--   0        0        0     2725 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/ObjectiveEncoder.hpp
+-rw-r--r--   0        0        0     2709 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/SATEncoder.hpp
+-rw-r--r--   0        0        0     1471 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/SingleGateEncoder.hpp
+-rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/TableauEncoder.hpp
+-rw-r--r--   0        0        0     4322 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/AvailableArchitecture.hpp
+-rw-r--r--   0        0        0     1484 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/CommanderGrouping.hpp
+-rw-r--r--   0        0        0     4175 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/Configuration.hpp
+-rw-r--r--   0        0        0     2158 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/EarlyTermination.hpp
+-rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/Encoding.hpp
+-rw-r--r--   0        0        0     5592 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/Heuristic.hpp
+-rw-r--r--   0        0        0     1182 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/InitialLayout.hpp
+-rw-r--r--   0        0        0     1383 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/Layering.hpp
+-rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/LookaheadHeuristic.hpp
+-rw-r--r--   0        0        0      867 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/Method.hpp
+-rw-r--r--   0        0        0     1168 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/configuration/SwapReduction.hpp
+-rw-r--r--   0        0        0     1134 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/exact/ExactMapper.hpp
+-rw-r--r--   0        0        0    17377 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/heuristic/HeuristicMapper.hpp
+-rw-r--r--   0        0        0     4252 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/heuristic/UniquePriorityQueue.hpp
+-rw-r--r--   0        0        0     2216 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/Encodings.hpp
+-rw-r--r--   0        0        0     4962 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/Logic.hpp
+-rw-r--r--   0        0        0     1647 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/LogicBlock.hpp
+-rw-r--r--   0        0        0     7407 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/LogicTerm.hpp
+-rw-r--r--   0        0        0      633 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/Model.hpp
+-rw-r--r--   0        0        0     4304 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/Z3Logic.hpp
+-rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/Z3Model.hpp
+-rw-r--r--   0        0        0     2809 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/logicblocks/util_logicblock.hpp
+-rw-r--r--   0        0        0     6973 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/include/utils.hpp
+-rw-r--r--   0        0        0     3370 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/noxfile.py
+-rw-r--r--   0        0        0     8225 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0    23988 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/Architecture.cpp
+-rw-r--r--   0        0        0     3475 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/CMakeLists.txt
+-rw-r--r--   0        0        0     9078 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/DataLogger.cpp
+-rw-r--r--   0        0        0    20198 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/Mapper.cpp
+-rw-r--r--   0        0        0    20963 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/CliffordSynthesizer.cpp
+-rw-r--r--   0        0        0    13141 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/Tableau.cpp
+-rw-r--r--   0        0        0    12191 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/GateEncoder.cpp
+-rw-r--r--   0        0        0     6880 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/MultiGateEncoder.cpp
+-rw-r--r--   0        0        0     2187 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/ObjectiveEncoder.cpp
+-rw-r--r--   0        0        0     4750 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/SATEncoder.cpp
+-rw-r--r--   0        0        0     7782 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/SingleGateEncoder.cpp
+-rw-r--r--   0        0        0     5773 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/TableauEncoder.cpp
+-rw-r--r--   0        0        0     2889 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/configuration/Configuration.cpp
+-rw-r--r--   0        0        0    31715 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/exact/ExactMapper.cpp
+-rw-r--r--   0        0        0    62858 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/heuristic/HeuristicMapper.cpp
+-rw-r--r--   0        0        0      953 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/logicblocks/CMakeLists.txt
+-rw-r--r--   0        0        0     5104 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/logicblocks/Encodings.cpp
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/logicblocks/LogicBlock.cpp
+-rw-r--r--   0        0        0    19341 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/logicblocks/LogicTerm.cpp
+-rw-r--r--   0        0        0    14528 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/logicblocks/Z3Logic.cpp
+-rw-r--r--   0        0        0     1047 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/logicblocks/Z3Model.cpp
+-rw-r--r--   0        0        0     1684 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/__init__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/_version.py
+-rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/_version.pyi
+-rw-r--r--   0        0        0     7609 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/clifford_synthesis.py
+-rw-r--r--   0        0        0     9526 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/compile.py
+-rw-r--r--   0        0        0   171627 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/libs/ibm_guadalupe_16.pickle
+-rw-r--r--   0        0        0   341613 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/libs/rigetti_16.pickle
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/load_architecture.py
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/load_calibration.py
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/py.typed
+-rw-r--r--   0        0        0    17501 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/pyqmap.pyi
+-rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/qiskit/backend.py
+-rw-r--r--   0        0        0    16106 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/subarchitectures.py
+-rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/visualization/__init__.py
+-rw-r--r--   0        0        0    13850 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/visualization/search_visualizer.py
+-rw-r--r--   0        0        0    90165 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/mqt/qmap/visualization/visualize_search_graph.py
+-rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/python/CMakeLists.txt
+-rw-r--r--   0        0        0    33293 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/python/bindings.cpp
+-rw-r--r--   0        0        0    10035 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/src/utils.cpp
+-rw-r--r--   0        0        0    11346 2022-11-09 12:37:21.000000 mqt_qmap-2.5.1/PKG-INFO
```

### Comparing `mqt_qmap-2.5.0/.clang-tidy` & `mqt_qmap-2.5.1/.clang-tidy`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/.gitignore` & `mqt_qmap-2.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/.pre-commit-config.yaml` & `mqt_qmap-2.5.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   autoupdate_commit_msg: "⬆️🪝 update pre-commit hooks"
   autofix_commit_msg: "🎨 pre-commit fixes"
   skip: [mypy]
 
 repos:
   # Standard hooks
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
@@ -29,33 +29,38 @@
       - id: trailing-whitespace
 
   # Clean jupyter notebooks
   - repo: https://github.com/srstevenson/nb-clean
     rev: 3.2.0
     hooks:
       - id: nb-clean
+        args:
+          - --remove-empty-cells
+          - --preserve-cell-metadata
+          - raw_mimetype
+          - --
 
   # Handling unwanted unicode characters
   - repo: https://github.com/sirosen/texthooks
-    rev: 0.6.4
+    rev: 0.6.6
     hooks:
       - id: fix-ligatures
       - id: fix-smartquotes
 
   # Check for common mistakes
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   # Python linting using ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
         types_or: [python, pyi, jupyter]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
@@ -64,15 +69,15 @@
     rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.*]
 
   # Check static types with mypy
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         files: ^(src/mqt|test/python)
         args: []
         additional_dependencies:
           - importlib_resources
           - numpy
@@ -84,15 +89,15 @@
     rev: v2.2.6
     hooks:
       - id: codespell
         args: ["-L", "wille,linz,applys", "--skip", "*.ipynb"]
 
   # Clang-format the C++ part of the code base automatically
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v17.0.6
+    rev: v18.1.3
     hooks:
       - id: clang-format
         types_or: [c++, c, cuda]
 
   # CMake format and lint the CMakeLists.txt files
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: v0.6.13
@@ -113,7 +118,14 @@
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest|Mqt|Tum
         exclude: .pre-commit-config.yaml
+
+  # Check best practices for scientific Python code
+  - repo: https://github.com/scientific-python/cookie
+    rev: 2024.03.10
+    hooks:
+      - id: sp-repo-review
+        additional_dependencies: ["repo-review[cli]"]
```

### Comparing `mqt_qmap-2.5.0/.readthedocs.yaml` & `mqt_qmap-2.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/CMakeLists.txt` & `mqt_qmap-2.5.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/LICENSE.md` & `mqt_qmap-2.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/README.md` & `mqt_qmap-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/cmake/ExternalDependencies.cmake` & `mqt_qmap-2.5.1/cmake/ExternalDependencies.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/cmake/FindZ3.cmake` & `mqt_qmap-2.5.1/cmake/FindZ3.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/cmake/cmake_uninstall.cmake.in` & `mqt_qmap-2.5.1/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/0410184_169.qasm` & `mqt_qmap-2.5.1/examples/0410184_169.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4_49_16.qasm` & `mqt_qmap-2.5.1/examples/4_49_16.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt10-v1_81.qasm` & `mqt_qmap-2.5.1/examples/4gt10-v1_81.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt12-v0_86.qasm` & `mqt_qmap-2.5.1/examples/4gt12-v0_86.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt12-v0_87.qasm` & `mqt_qmap-2.5.1/examples/4gt12-v0_87.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt12-v0_88.qasm` & `mqt_qmap-2.5.1/examples/4gt12-v0_88.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt12-v1_89.qasm` & `mqt_qmap-2.5.1/examples/4gt12-v1_89.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt13-v1_93.qasm` & `mqt_qmap-2.5.1/examples/4gt13-v1_93.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt13_90.qasm` & `mqt_qmap-2.5.1/examples/4gt13_90.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt13_91.qasm` & `mqt_qmap-2.5.1/examples/4gt13_91.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt13_92.qasm` & `mqt_qmap-2.5.1/examples/4gt13_92.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt4-v0_72.qasm` & `mqt_qmap-2.5.1/examples/4gt4-v0_72.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt4-v0_73.qasm` & `mqt_qmap-2.5.1/examples/4gt4-v0_73.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt4-v0_78.qasm` & `mqt_qmap-2.5.1/examples/4gt4-v0_78.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt4-v0_79.qasm` & `mqt_qmap-2.5.1/examples/4gt4-v0_79.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt4-v0_80.qasm` & `mqt_qmap-2.5.1/examples/4gt4-v0_80.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt4-v1_74.qasm` & `mqt_qmap-2.5.1/examples/4gt4-v1_74.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt5_75.qasm` & `mqt_qmap-2.5.1/examples/4gt5_75.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt5_76.qasm` & `mqt_qmap-2.5.1/examples/4gt5_76.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4gt5_77.qasm` & `mqt_qmap-2.5.1/examples/4gt5_77.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4mod5-bdd_287.qasm` & `mqt_qmap-2.5.1/examples/4mod5-bdd_287.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4mod5-v0_18.qasm` & `mqt_qmap-2.5.1/examples/4mod5-v0_18.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4mod5-v1_23.qasm` & `mqt_qmap-2.5.1/examples/4mod5-v1_23.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4mod7-v0_94.qasm` & `mqt_qmap-2.5.1/examples/4mod7-v0_94.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/4mod7-v1_96.qasm` & `mqt_qmap-2.5.1/examples/4mod7-v1_96.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/9symml_195.qasm` & `mqt_qmap-2.5.1/examples/9symml_195.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/C17_204.qasm` & `mqt_qmap-2.5.1/examples/C17_204.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/adr4_197.qasm` & `mqt_qmap-2.5.1/examples/adr4_197.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/aj-e11_165.qasm` & `mqt_qmap-2.5.1/examples/aj-e11_165.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/alu-bdd_288.qasm` & `mqt_qmap-2.5.1/examples/alu-bdd_288.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/alu-v0_26.qasm` & `mqt_qmap-2.5.1/examples/alu-v0_26.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/alu-v2_30.qasm` & `mqt_qmap-2.5.1/examples/alu-v2_30.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/alu-v2_31.qasm` & `mqt_qmap-2.5.1/examples/alu-v2_31.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/alu-v2_32.qasm` & `mqt_qmap-2.5.1/examples/alu-v2_32.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/alu-v3_34.qasm` & `mqt_qmap-2.5.1/examples/alu-v3_34.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/alu-v4_36.qasm` & `mqt_qmap-2.5.1/examples/alu-v4_36.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/clip_206.qasm` & `mqt_qmap-2.5.1/examples/clip_206.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/cm152a_212.qasm` & `mqt_qmap-2.5.1/examples/cm152a_212.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/cm42a_207.qasm` & `mqt_qmap-2.5.1/examples/cm42a_207.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/cm82a_208.qasm` & `mqt_qmap-2.5.1/examples/cm82a_208.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/cm85a_209.qasm` & `mqt_qmap-2.5.1/examples/cm85a_209.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/cnt3-5_179.qasm` & `mqt_qmap-2.5.1/examples/cnt3-5_179.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/cnt3-5_180.qasm` & `mqt_qmap-2.5.1/examples/cnt3-5_180.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/co14_215.qasm` & `mqt_qmap-2.5.1/examples/co14_215.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/con1_216.qasm` & `mqt_qmap-2.5.1/examples/con1_216.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/cycle10_2_110.qasm` & `mqt_qmap-2.5.1/examples/cycle10_2_110.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/dc1_220.qasm` & `mqt_qmap-2.5.1/examples/dc1_220.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/dc2_222.qasm` & `mqt_qmap-2.5.1/examples/dc2_222.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/decod24-bdd_294.qasm` & `mqt_qmap-2.5.1/examples/decod24-bdd_294.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/decod24-enable_126.qasm` & `mqt_qmap-2.5.1/examples/decod24-enable_126.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/decod24-v0_38.qasm` & `mqt_qmap-2.5.1/examples/decod24-v0_38.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/decod24-v1_41.qasm` & `mqt_qmap-2.5.1/examples/decod24-v1_41.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/decod24-v2_43.qasm` & `mqt_qmap-2.5.1/examples/decod24-v2_43.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/decod24-v3_45.qasm` & `mqt_qmap-2.5.1/examples/decod24-v3_45.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/dist_223.qasm` & `mqt_qmap-2.5.1/examples/dist_223.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ex2_227.qasm` & `mqt_qmap-2.5.1/examples/ex2_227.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ex3_229.qasm` & `mqt_qmap-2.5.1/examples/ex3_229.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/f2_232.qasm` & `mqt_qmap-2.5.1/examples/f2_232.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ground_state_estimation_10.qasm` & `mqt_qmap-2.5.1/examples/ground_state_estimation_10.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_3_0.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_3_0.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_3_3.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_3_3.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_3_5.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_3_5.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_3_6.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_3_6.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_0.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_0.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_1.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_1.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_2.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_2.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_4.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_4.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_5.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_5.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_6.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_6.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_7.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_7.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_8.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_8.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_4_9.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_4_9.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_0.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_0.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_1.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_1.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_2.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_2.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_3.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_3.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_4.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_4.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_5.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_5.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_6.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_6.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_8.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_8.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/grover/grover_5_9.qasm` & `mqt_qmap-2.5.1/examples/grover/grover_5_9.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ham15_107.qasm` & `mqt_qmap-2.5.1/examples/ham15_107.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ham7_104.qasm` & `mqt_qmap-2.5.1/examples/ham7_104.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/hwb4_49.qasm` & `mqt_qmap-2.5.1/examples/hwb4_49.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/hwb5_53.qasm` & `mqt_qmap-2.5.1/examples/hwb5_53.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/hwb6_56.qasm` & `mqt_qmap-2.5.1/examples/hwb6_56.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/hwb7_59.qasm` & `mqt_qmap-2.5.1/examples/hwb7_59.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/hwb8_113.qasm` & `mqt_qmap-2.5.1/examples/hwb8_113.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/hwb9_119.qasm` & `mqt_qmap-2.5.1/examples/hwb9_119.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/inc_237.qasm` & `mqt_qmap-2.5.1/examples/inc_237.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ising_model_10.qasm` & `mqt_qmap-2.5.1/examples/ising_model_10.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ising_model_13.qasm` & `mqt_qmap-2.5.1/examples/ising_model_13.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/ising_model_16.qasm` & `mqt_qmap-2.5.1/examples/ising_model_16.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/life_238.qasm` & `mqt_qmap-2.5.1/examples/life_238.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/majority_239.qasm` & `mqt_qmap-2.5.1/examples/majority_239.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/max46_240.qasm` & `mqt_qmap-2.5.1/examples/max46_240.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/miller_11.qasm` & `mqt_qmap-2.5.1/examples/miller_11.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mini-alu_167.qasm` & `mqt_qmap-2.5.1/examples/mini-alu_167.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mini_alu_305.qasm` & `mqt_qmap-2.5.1/examples/mini_alu_305.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/misex1_241.qasm` & `mqt_qmap-2.5.1/examples/misex1_241.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mlp4_245.qasm` & `mqt_qmap-2.5.1/examples/mlp4_245.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mod10_171.qasm` & `mqt_qmap-2.5.1/examples/mod10_171.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mod10_176.qasm` & `mqt_qmap-2.5.1/examples/mod10_176.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mod5adder_127.qasm` & `mqt_qmap-2.5.1/examples/mod5adder_127.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mod5d2_64.qasm` & `mqt_qmap-2.5.1/examples/mod5d2_64.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mod8-10_177.qasm` & `mqt_qmap-2.5.1/examples/mod8-10_177.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/mod8-10_178.qasm` & `mqt_qmap-2.5.1/examples/mod8-10_178.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/one-two-three-v0_97.qasm` & `mqt_qmap-2.5.1/examples/one-two-three-v0_97.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/one-two-three-v0_98.qasm` & `mqt_qmap-2.5.1/examples/one-two-three-v0_98.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/one-two-three-v1_99.qasm` & `mqt_qmap-2.5.1/examples/one-two-three-v1_99.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/one-two-three-v2_100.qasm` & `mqt_qmap-2.5.1/examples/one-two-three-v2_100.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/one-two-three-v3_101.qasm` & `mqt_qmap-2.5.1/examples/one-two-three-v3_101.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/plus63mod4096_163.qasm` & `mqt_qmap-2.5.1/examples/plus63mod4096_163.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/plus63mod8192_164.qasm` & `mqt_qmap-2.5.1/examples/plus63mod8192_164.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/pm1_249.qasm` & `mqt_qmap-2.5.1/examples/pm1_249.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/qe_qft_4.qasm` & `mqt_qmap-2.5.1/examples/qe_qft_4.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/qe_qft_5.qasm` & `mqt_qmap-2.5.1/examples/qe_qft_5.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/qelib1.inc` & `mqt_qmap-2.5.1/examples/qelib1.inc`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/qft_10.qasm` & `mqt_qmap-2.5.1/examples/qft_10.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/qft_16.qasm` & `mqt_qmap-2.5.1/examples/qft_16.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/radd_250.qasm` & `mqt_qmap-2.5.1/examples/radd_250.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd32_270.qasm` & `mqt_qmap-2.5.1/examples/rd32_270.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd53_130.qasm` & `mqt_qmap-2.5.1/examples/rd53_130.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd53_131.qasm` & `mqt_qmap-2.5.1/examples/rd53_131.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd53_133.qasm` & `mqt_qmap-2.5.1/examples/rd53_133.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd53_135.qasm` & `mqt_qmap-2.5.1/examples/rd53_135.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd53_138.qasm` & `mqt_qmap-2.5.1/examples/rd53_138.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd53_251.qasm` & `mqt_qmap-2.5.1/examples/rd53_251.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd53_311.qasm` & `mqt_qmap-2.5.1/examples/rd53_311.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd73_140.qasm` & `mqt_qmap-2.5.1/examples/rd73_140.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd73_252.qasm` & `mqt_qmap-2.5.1/examples/rd73_252.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd84_142.qasm` & `mqt_qmap-2.5.1/examples/rd84_142.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/rd84_253.qasm` & `mqt_qmap-2.5.1/examples/rd84_253.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/root_255.qasm` & `mqt_qmap-2.5.1/examples/root_255.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sao2_257.qasm` & `mqt_qmap-2.5.1/examples/sao2_257.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sf_274.qasm` & `mqt_qmap-2.5.1/examples/sf_274.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sf_276.qasm` & `mqt_qmap-2.5.1/examples/sf_276.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sqn_258.qasm` & `mqt_qmap-2.5.1/examples/sqn_258.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sqrt8_260.qasm` & `mqt_qmap-2.5.1/examples/sqrt8_260.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/squar5_261.qasm` & `mqt_qmap-2.5.1/examples/squar5_261.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/square_root_7.qasm` & `mqt_qmap-2.5.1/examples/square_root_7.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sym10_262.qasm` & `mqt_qmap-2.5.1/examples/sym10_262.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sym6_145.qasm` & `mqt_qmap-2.5.1/examples/sym6_145.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sym6_316.qasm` & `mqt_qmap-2.5.1/examples/sym6_316.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sym9_146.qasm` & `mqt_qmap-2.5.1/examples/sym9_146.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sym9_148.qasm` & `mqt_qmap-2.5.1/examples/sym9_148.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sym9_193.qasm` & `mqt_qmap-2.5.1/examples/sym9_193.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/sys6-v0_111.qasm` & `mqt_qmap-2.5.1/examples/sys6-v0_111.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf1_149.qasm` & `mqt_qmap-2.5.1/examples/urf1_149.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf1_278.qasm` & `mqt_qmap-2.5.1/examples/urf1_278.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf2_152.qasm` & `mqt_qmap-2.5.1/examples/urf2_152.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf2_277.qasm` & `mqt_qmap-2.5.1/examples/urf2_277.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf3_155.qasm` & `mqt_qmap-2.5.1/examples/urf3_155.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf3_279.qasm` & `mqt_qmap-2.5.1/examples/urf3_279.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf4_187.qasm` & `mqt_qmap-2.5.1/examples/urf4_187.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf5_158.qasm` & `mqt_qmap-2.5.1/examples/urf5_158.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf5_280.qasm` & `mqt_qmap-2.5.1/examples/urf5_280.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/urf6_160.qasm` & `mqt_qmap-2.5.1/examples/urf6_160.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/wim_266.qasm` & `mqt_qmap-2.5.1/examples/wim_266.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/examples/z4_268.qasm` & `mqt_qmap-2.5.1/examples/z4_268.qasm`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/calibration/ibmq_london.csv` & `mqt_qmap-2.5.1/extern/calibration/ibmq_london.csv`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/.clang-tidy` & `mqt_qmap-2.5.1/extern/mqt-core/.clang-tidy`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/.gitignore` & `mqt_qmap-2.5.1/extern/mqt-core/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/.pre-commit-config.yaml` & `mqt_qmap-2.5.1/extern/mqt-core/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   autoupdate_commit_msg: "⬆️🪝 update pre-commit hooks"
   autofix_commit_msg: "🎨 pre-commit fixes"
   skip: [mypy]
 
 repos:
   # Standard hooks
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-toml
@@ -31,43 +31,48 @@
       - id: trailing-whitespace
 
   # Clean jupyter notebooks
   - repo: https://github.com/srstevenson/nb-clean
     rev: 3.2.0
     hooks:
       - id: nb-clean
+        args:
+          - --remove-empty-cells
+          - --preserve-cell-metadata
+          - raw_mimetype
+          - --
 
   # Handling unwanted unicode characters
   - repo: https://github.com/sirosen/texthooks
-    rev: 0.6.4
+    rev: 0.6.6
     hooks:
       - id: fix-ligatures
       - id: fix-smartquotes
 
   # Check for common mistakes
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   # Python linting using ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
         types_or: [python, pyi, jupyter]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
   # Static type checking using mypy
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         files: ^(src/mqt|test/python)
         args: []
         additional_dependencies:
           - pytest
           - pandas-stubs
@@ -77,15 +82,15 @@
     rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.*]
 
   # Clang-format the C++ part of the code base automatically
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v17.0.6
+    rev: v18.1.3
     hooks:
       - id: clang-format
         types_or: [c++, c, cuda]
 
   # CMake format and lint the CMakeLists.txt files
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: v0.6.13
@@ -116,11 +121,11 @@
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest|Mqt|Tum
         exclude: .pre-commit-config.yaml
 
   # Check best practices for scientific Python code
   - repo: https://github.com/scientific-python/cookie
-    rev: 2024.01.24
+    rev: 2024.03.10
     hooks:
       - id: sp-repo-review
         additional_dependencies: ["repo-review[cli]"]
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/.readthedocs.yaml` & `mqt_qmap-2.5.1/extern/mqt-core/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/CMakeLists.txt` & `mqt_qmap-2.5.1/extern/mqt-core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/LICENSE.md` & `mqt_qmap-2.5.1/extern/mqt-core/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/README.md` & `mqt_qmap-2.5.1/extern/mqt-core/README.md`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/Cache.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/CompilerOptions.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/CompilerOptions.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/CompilerWarnings.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/ExternalDependencies.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/ExternalDependencies.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/FindGMP.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/GetVersion.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/GetVersion.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/PackageAddTest.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/PackageAddTest.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/PreventInSourceBuilds.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/Sanitizers.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/Sanitizers.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/StandardProjectSettings.cmake` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/cmake_uninstall.cmake.in` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/cmake/mqt-core-config.cmake.in` & `mqt_qmap-2.5.1/extern/mqt-core/cmake/mqt-core-config.cmake.in`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/eval/eval_dd_package.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/eval/eval_dd_package.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/CircuitOptimizer.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/CircuitOptimizer.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -70,14 +70,27 @@
    * with every SWAP gate and, eventually, the initial layout of the circuit is
    * set to the tracked permutation. Any unassigned qubit in the initial layout
    * is assigned to the first available position (favoring an identity mapping).
    * @param qc the quantum circuit
    */
   static void backpropagateOutputPermutation(QuantumComputation& qc);
 
+  /**
+   * @brief Collects all operations in the circuit into blocks of a maximum
+   * size.
+   * @details The circuit is traversed and operations are collected into blocks
+   * of a maximum size. The blocks are then appended to the circuit in the order
+   * they were collected. Each block is realized as a compound operation.
+   * Light optimizations are applied to the blocks, such as removing identity
+   * gates and fusing single-qubit gates.
+   * @param qc the quantum circuit
+   * @param maxBlockSize the maximum size of a block
+   */
+  static void collectBlocks(QuantumComputation& qc, std::size_t maxBlockSize);
+
 protected:
   static void removeDiagonalGatesBeforeMeasureRecursive(
       DAG& dag, DAGReverseIterators& dagIterators, Qubit idx,
       const qc::Operation* until);
   static bool removeDiagonalGate(DAG& dag, DAGReverseIterators& dagIterators,
                                  Qubit idx, DAGReverseIterator& it,
                                  qc::Operation* op);
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/Definitions.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/Definitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/Permutation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/Permutation.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/QuantumComputation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/QuantumComputation.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -302,14 +302,21 @@
 
   [[nodiscard]] virtual std::size_t getNops() const { return ops.size(); }
   [[nodiscard]] std::size_t getNqubits() const { return nqubits + nancillae; }
   [[nodiscard]] std::size_t getNancillae() const { return nancillae; }
   [[nodiscard]] std::size_t getNqubitsWithoutAncillae() const {
     return nqubits;
   }
+  [[nodiscard]] std::size_t getNmeasuredQubits() const {
+    return getNqubits() - getNgarbageQubits();
+  }
+  [[nodiscard]] std::size_t getNgarbageQubits() const {
+    return static_cast<std::size_t>(
+        std::count(getGarbage().begin(), getGarbage().end(), true));
+  }
   [[nodiscard]] std::size_t getNcbits() const { return nclassics; }
   [[nodiscard]] std::string getName() const { return name; }
   [[nodiscard]] const QuantumRegisterMap& getQregs() const { return qregs; }
   [[nodiscard]] const ClassicalRegisterMap& getCregs() const { return cregs; }
   [[nodiscard]] const QuantumRegisterMap& getANCregs() const { return ancregs; }
   [[nodiscard]] decltype(mt)& getGenerator() { return mt; }
 
@@ -363,19 +370,38 @@
    * @brief Sets the given logical qubit to be ancillary
    * @details Removes the qubit from the qubit register and adds it to the
    * ancillary register, if such a register exists. Otherwise a new ancillary
    * register is created.
    * @param logicalQubitIndex
    */
   void setLogicalQubitAncillary(Qubit logicalQubitIndex);
+  /**
+   * @brief Sets all logical qubits in the range [minLogicalQubitIndex,
+   * maxLogicalQubitIndex] to be ancillary
+   * @details Removes the qubits from the qubit register and adds it to the
+   * ancillary register, if such a register exists. Otherwise a new ancillary
+   * register is created.
+   * @param minLogicalQubitIndex first qubit that is set to be ancillary
+   * @param maxLogicalQubitIndex last qubit that is set to be ancillary
+   */
+  void setLogicalQubitsAncillary(Qubit minLogicalQubitIndex,
+                                 Qubit maxLogicalQubitIndex);
   [[nodiscard]] bool
   logicalQubitIsGarbage(const Qubit logicalQubitIndex) const {
     return garbage[logicalQubitIndex];
   }
   void setLogicalQubitGarbage(Qubit logicalQubitIndex);
+  /**
+   * @brief Sets all logical qubits in the range [minLogicalQubitIndex,
+   * maxLogicalQubitIndex] to be garbage
+   * @param minLogicalQubitIndex first qubit that is set to be garbage
+   * @param maxLogicalQubitIndex last qubit that is set to be garbage
+   */
+  void setLogicalQubitsGarbage(Qubit minLogicalQubitIndex,
+                               Qubit maxLogicalQubitIndex);
   [[nodiscard]] const std::vector<bool>& getAncillary() const {
     return ancillary;
   }
   [[nodiscard]] const std::vector<bool>& getGarbage() const { return garbage; }
 
   /// checks whether the given logical qubit exists in the initial layout.
   /// \param logicalQubitIndex the logical qubit index to check
@@ -404,15 +430,15 @@
 #define DEFINE_SINGLE_TARGET_OPERATION(op)                                     \
   void op(const Qubit target) { mc##op(Controls{}, target); }                  \
   void c##op(const Control& control, const Qubit target) {                     \
     mc##op(Controls{control}, target);                                         \
   }                                                                            \
   void mc##op(const Controls& controls, const Qubit target) {                  \
     checkQubitRange(target, controls);                                         \
-    emplace_back<StandardOperation>(getNqubits(), controls, target,            \
+    emplace_back<StandardOperation>(controls, target,                          \
                                     OP_NAME_TO_TYPE.at(#op));                  \
   }
 
   DEFINE_SINGLE_TARGET_OPERATION(i)
   DEFINE_SINGLE_TARGET_OPERATION(x)
   DEFINE_SINGLE_TARGET_OPERATION(y)
   DEFINE_SINGLE_TARGET_OPERATION(z)
@@ -434,22 +460,21 @@
              const Qubit target) {                                             \
     mc##op(param, Controls{control}, target);                                  \
   }                                                                            \
   void mc##op(const SymbolOrNumber&(param), const Controls& controls,          \
               const Qubit target) {                                            \
     checkQubitRange(target, controls);                                         \
     if (std::holds_alternative<fp>(param)) {                                   \
-      emplace_back<StandardOperation>(getNqubits(), controls, target,          \
+      emplace_back<StandardOperation>(controls, target,                        \
                                       OP_NAME_TO_TYPE.at(#op),                 \
                                       std::vector{std::get<fp>(param)});       \
     } else {                                                                   \
       addVariables(param);                                                     \
-      emplace_back<SymbolicOperation>(getNqubits(), controls, target,          \
-                                      OP_NAME_TO_TYPE.at(#op),                 \
-                                      std::vector{param});                     \
+      emplace_back<SymbolicOperation>(                                         \
+          controls, target, OP_NAME_TO_TYPE.at(#op), std::vector{param});      \
     }                                                                          \
   }
 
   DEFINE_SINGLE_TARGET_SINGLE_PARAMETER_OPERATION(rx, theta)
   DEFINE_SINGLE_TARGET_SINGLE_PARAMETER_OPERATION(ry, theta)
   DEFINE_SINGLE_TARGET_SINGLE_PARAMETER_OPERATION(rz, theta)
   DEFINE_SINGLE_TARGET_SINGLE_PARAMETER_OPERATION(p, theta)
@@ -465,19 +490,19 @@
   }                                                                            \
   void mc##op(const SymbolOrNumber&(param0), const SymbolOrNumber&(param1),    \
               const Controls& controls, const Qubit target) {                  \
     checkQubitRange(target, controls);                                         \
     if (std::holds_alternative<fp>(param0) &&                                  \
         std::holds_alternative<fp>(param1)) {                                  \
       emplace_back<StandardOperation>(                                         \
-          getNqubits(), controls, target, OP_NAME_TO_TYPE.at(#op),             \
+          controls, target, OP_NAME_TO_TYPE.at(#op),                           \
           std::vector{std::get<fp>(param0), std::get<fp>(param1)});            \
     } else {                                                                   \
       addVariables(param0, param1);                                            \
-      emplace_back<SymbolicOperation>(getNqubits(), controls, target,          \
+      emplace_back<SymbolicOperation>(controls, target,                        \
                                       OP_NAME_TO_TYPE.at(#op),                 \
                                       std::vector{param0, param1});            \
     }                                                                          \
   }
 
   DEFINE_SINGLE_TARGET_TWO_PARAMETER_OPERATION(u2, phi, lambda)
 
@@ -496,20 +521,20 @@
               const SymbolOrNumber&(param2), const Controls& controls,         \
               const Qubit target) {                                            \
     checkQubitRange(target, controls);                                         \
     if (std::holds_alternative<fp>(param0) &&                                  \
         std::holds_alternative<fp>(param1) &&                                  \
         std::holds_alternative<fp>(param2)) {                                  \
       emplace_back<StandardOperation>(                                         \
-          getNqubits(), controls, target, OP_NAME_TO_TYPE.at(#op),             \
+          controls, target, OP_NAME_TO_TYPE.at(#op),                           \
           std::vector{std::get<fp>(param0), std::get<fp>(param1),              \
                       std::get<fp>(param2)});                                  \
     } else {                                                                   \
       addVariables(param0, param1, param2);                                    \
-      emplace_back<SymbolicOperation>(getNqubits(), controls, target,          \
+      emplace_back<SymbolicOperation>(controls, target,                        \
                                       OP_NAME_TO_TYPE.at(#op),                 \
                                       std::vector{param0, param1, param2});    \
     }                                                                          \
   }
 
   DEFINE_SINGLE_TARGET_THREE_PARAMETER_OPERATION(u, theta, phi, lambda)
 
@@ -520,15 +545,15 @@
   void c##op(const Control& control, const Qubit target0,                      \
              const Qubit target1) {                                            \
     mc##op(Controls{control}, target0, target1);                               \
   }                                                                            \
   void mc##op(const Controls& controls, const Qubit target0,                   \
               const Qubit target1) {                                           \
     checkQubitRange(target0, target1, controls);                               \
-    emplace_back<StandardOperation>(getNqubits(), controls, target0, target1,  \
+    emplace_back<StandardOperation>(controls, target0, target1,                \
                                     OP_NAME_TO_TYPE.at(#op));                  \
   }
 
   DEFINE_TWO_TARGET_OPERATION(swap)
   DEFINE_TWO_TARGET_OPERATION(dcx)
   DEFINE_TWO_TARGET_OPERATION(ecr)
   DEFINE_TWO_TARGET_OPERATION(iswap)
@@ -545,21 +570,21 @@
              const Qubit target0, const Qubit target1) {                       \
     mc##op(param, Controls{control}, target0, target1);                        \
   }                                                                            \
   void mc##op(const SymbolOrNumber&(param), const Controls& controls,          \
               const Qubit target0, const Qubit target1) {                      \
     checkQubitRange(target0, target1, controls);                               \
     if (std::holds_alternative<fp>(param)) {                                   \
-      emplace_back<StandardOperation>(getNqubits(), controls, target0,         \
-                                      target1, OP_NAME_TO_TYPE.at(#op),        \
+      emplace_back<StandardOperation>(controls, target0, target1,              \
+                                      OP_NAME_TO_TYPE.at(#op),                 \
                                       std::vector{std::get<fp>(param)});       \
     } else {                                                                   \
       addVariables(param);                                                     \
-      emplace_back<SymbolicOperation>(getNqubits(), controls, target0,         \
-                                      target1, OP_NAME_TO_TYPE.at(#op),        \
+      emplace_back<SymbolicOperation>(controls, target0, target1,              \
+                                      OP_NAME_TO_TYPE.at(#op),                 \
                                       std::vector{param});                     \
     }                                                                          \
   }
 
   DEFINE_TWO_TARGET_SINGLE_PARAMETER_OPERATION(rxx, theta)
   DEFINE_TWO_TARGET_SINGLE_PARAMETER_OPERATION(ryy, theta)
   DEFINE_TWO_TARGET_SINGLE_PARAMETER_OPERATION(rzz, theta)
@@ -578,20 +603,20 @@
   void mc##op(const SymbolOrNumber&(param0), const SymbolOrNumber&(param1),    \
               const Controls& controls, const Qubit target0,                   \
               const Qubit target1) {                                           \
     checkQubitRange(target0, target1, controls);                               \
     if (std::holds_alternative<fp>(param0) &&                                  \
         std::holds_alternative<fp>(param1)) {                                  \
       emplace_back<StandardOperation>(                                         \
-          getNqubits(), controls, target0, target1, OP_NAME_TO_TYPE.at(#op),   \
+          controls, target0, target1, OP_NAME_TO_TYPE.at(#op),                 \
           std::vector{std::get<fp>(param0), std::get<fp>(param1)});            \
     } else {                                                                   \
       addVariables(param0, param1);                                            \
-      emplace_back<SymbolicOperation>(getNqubits(), controls, target0,         \
-                                      target1, OP_NAME_TO_TYPE.at(#op),        \
+      emplace_back<SymbolicOperation>(controls, target0, target1,              \
+                                      OP_NAME_TO_TYPE.at(#op),                 \
                                       std::vector{param0, param1});            \
     }                                                                          \
   }
 
   DEFINE_TWO_TARGET_TWO_PARAMETER_OPERATION(xx_minus_yy, theta, beta)
   DEFINE_TWO_TARGET_TWO_PARAMETER_OPERATION(xx_plus_yy, theta, beta)
 
@@ -602,56 +627,55 @@
 #undef DEFINE_TWO_TARGET_OPERATION
 #undef DEFINE_TWO_TARGET_SINGLE_PARAMETER_OPERATION
 #undef DEFINE_TWO_TARGET_TWO_PARAMETER_OPERATION
 
   void measure(const Qubit qubit, const std::size_t bit) {
     checkQubitRange(qubit);
     checkBitRange(bit);
-    emplace_back<NonUnitaryOperation>(getNqubits(), qubit, bit);
+    emplace_back<NonUnitaryOperation>(qubit, bit);
   }
 
   void measure(Qubit qubit, const std::pair<std::string, Bit>& registerBit);
 
   void measure(const Targets& qubits, const std::vector<Bit>& bits) {
     checkQubitRange(qubits);
     checkBitRange(bits);
-    emplace_back<NonUnitaryOperation>(getNqubits(), qubits, bits);
+    emplace_back<NonUnitaryOperation>(qubits, bits);
   }
 
   /**
    * @brief Add measurements to all qubits
    * @param addBits Whether to add new classical bits to the circuit
    * @details This function adds measurements to all qubits in the circuit and
    * appends a new classical register (named "meas") to the circuit if addBits
    * is true. Otherwise, qubit q is measured into classical bit q.
    */
   void measureAll(bool addBits = true);
 
   void reset(const Qubit target) {
     checkQubitRange(target);
-    emplace_back<NonUnitaryOperation>(getNqubits(), std::vector<Qubit>{target},
-                                      qc::Reset);
+    emplace_back<NonUnitaryOperation>(std::vector<Qubit>{target}, qc::Reset);
   }
   void reset(const Targets& targets) {
     checkQubitRange(targets);
-    emplace_back<NonUnitaryOperation>(getNqubits(), targets, qc::Reset);
+    emplace_back<NonUnitaryOperation>(targets, qc::Reset);
   }
 
   void barrier() {
     std::vector<Qubit> targets(getNqubits());
     std::iota(targets.begin(), targets.end(), 0);
-    emplace_back<StandardOperation>(getNqubits(), targets, qc::Barrier);
+    emplace_back<StandardOperation>(targets, qc::Barrier);
   }
   void barrier(const Qubit target) {
     checkQubitRange(target);
-    emplace_back<StandardOperation>(getNqubits(), target, qc::Barrier);
+    emplace_back<StandardOperation>(target, qc::Barrier);
   }
   void barrier(const Targets& targets) {
     checkQubitRange(targets);
-    emplace_back<StandardOperation>(getNqubits(), targets, qc::Barrier);
+    emplace_back<StandardOperation>(targets, qc::Barrier);
   }
 
   void classicControlled(const OpType op, const Qubit target,
                          const ClassicalRegister& controlRegister,
                          const std::uint64_t expectedValue = 1U,
                          const std::vector<fp>& params = {}) {
     classicControlled(op, target, Controls{}, controlRegister, expectedValue,
@@ -668,16 +692,16 @@
   void classicControlled(const OpType op, const Qubit target,
                          const Controls& controls,
                          const ClassicalRegister& controlRegister,
                          const std::uint64_t expectedValue = 1U,
                          const std::vector<fp>& params = {}) {
     checkQubitRange(target, controls);
     checkClassicalRegister(controlRegister);
-    std::unique_ptr<Operation> gate = std::make_unique<StandardOperation>(
-        getNqubits(), controls, target, op, params);
+    std::unique_ptr<Operation> gate =
+        std::make_unique<StandardOperation>(controls, target, op, params);
     emplace_back<ClassicControlledOperation>(std::move(gate), controlRegister,
                                              expectedValue);
   }
 
   /// strip away qubits with no operations applied to them and which do not pop
   /// up in the output permutation \param force if true, also strip away idle
   /// qubits occurring in the output permutation
@@ -814,15 +838,15 @@
     std::stringstream ss;
     dumpOpenQASM(ss, qasm3);
     return ss.str();
   }
 
   // this convenience method allows to turn a circuit into a compound operation.
   std::unique_ptr<CompoundOperation> asCompoundOperation() {
-    return std::make_unique<CompoundOperation>(getNqubits(), std::move(ops));
+    return std::make_unique<CompoundOperation>(std::move(ops));
   }
 
   // this convenience method allows to turn a circuit into an operation.
   std::unique_ptr<Operation> asOperation() {
     if (ops.empty()) {
       return {};
     }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/BernsteinVazirani.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/BernsteinVazirani.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/Grover.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/Grover.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/algorithms/RandomCliffordCircuit.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/algorithms/RandomCliffordCircuit.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Benchmark.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Benchmark.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/CachedEdge.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/CachedEdge.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 ///-----------------------------------------------------------------------------
 ///                        \n Type traits and typedefs \n
 ///-----------------------------------------------------------------------------
 template <typename T>
 using isVector = std::enable_if_t<std::is_same_v<T, vNode>, bool>;
 template <typename T>
+using isMatrix = std::enable_if_t<std::is_same_v<T, mNode>, bool>;
+template <typename T>
 using isMatrixVariant =
     std::enable_if_t<std::is_same_v<T, mNode> || std::is_same_v<T, dNode>,
                      bool>;
 
 /**
  * @brief A DD node with a cached edge weight
  * @details Some DD operations create intermediate results that are not part of
@@ -96,14 +98,22 @@
    * @brief Create a one terminal edge.
    * @return A one terminal edge.
    */
   [[nodiscard]] static constexpr CachedEdge one() {
     return terminal(ComplexValue(1.));
   }
 
+  /**
+   * @brief Check whether this is a terminal.
+   * @return whether this is a terminal
+   */
+  [[nodiscard]] constexpr bool isTerminal() const {
+    return Node::isTerminal(p);
+  }
+
   ///---------------------------------------------------------------------------
   ///                     \n Methods for vector DDs \n
   ///---------------------------------------------------------------------------
 
   /**
    * @brief Get a normalized vector DD from a fresh node and a list of edges.
    * @tparam T template parameter to enable this method only for vNode
@@ -132,14 +142,30 @@
    * @param cn a reference to the complex number manager (for adding new
    * complex numbers)
    * @return the normalized (density) matrix DD
    */
   template <typename T = Node, isMatrixVariant<T> = true>
   static CachedEdge normalize(Node* p, const std::array<CachedEdge, NEDGE>& e,
                               MemoryManager<Node>& mm, ComplexNumbers& cn);
+
+  /**
+   * @brief Check whether the matrix represented by the DD is the identity.
+   * @tparam T template parameter to enable this function only for matrix nodes
+   * @return whether the matrix is the identity
+   */
+  template <typename T = Node, isMatrixVariant<T> = true>
+  [[nodiscard]] bool isIdentity(const bool upToGlobalPhase = true) const {
+    if (!isTerminal()) {
+      return false;
+    }
+    if (upToGlobalPhase) {
+      return !w.exactlyZero();
+    }
+    return w.exactlyOne();
+  }
 };
 
 } // namespace dd
 
 namespace std {
 template <class Node> struct hash<dd::CachedEdge<Node>> {
   std::size_t operator()(dd::CachedEdge<Node> const& e) const noexcept;
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Complex.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Complex.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/ComplexNumbers.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/ComplexNumbers.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/ComplexValue.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/ComplexValue.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,21 @@
    * @brief Check whether the complex number is exactly equal to zero.
    * @return True if the complex number is exactly equal to zero, false
    * otherwise.
    */
   [[nodiscard]] bool exactlyZero() const noexcept { return r == 0. && i == 0.; }
 
   /**
+   * @brief Check whether the complex number is exactly equal to one.
+   * @return True if the complex number is exactly equal to one, false
+   * otherwise.
+   */
+  [[nodiscard]] bool exactlyOne() const noexcept { return r == 1. && i == 0.; }
+
+  /**
    * @brief Check whether the complex number is approximately equal to the
    * given complex number.
    * @param c The complex number to compare to.
    * @returns True if the complex number is approximately equal to the given
    * complex number, false otherwise.
    * @see RealNumber::approximatelyEquals
    */
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/ComputeTable.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/ComputeTable.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,16 @@
     if (entry.leftOperand != leftOperand) {
       return result;
     }
     if (entry.rightOperand != rightOperand) {
       return result;
     }
 
-    if constexpr (std::is_same_v<RightOperandType, dEdge>) {
+    if constexpr (std::is_same_v<RightOperandType, dNode*> ||
+                  std::is_same_v<RightOperandType, dCachedEdge>) {
       // Since density matrices are reduced representations of matrices, a
       // density matrix may not be returned when a matrix is required and vice
       // versa
       if (!dNode::isTerminal(entry.result.p) &&
           dNode::isDensityMatrixNode(entry.result.p->flags) !=
               useDensityMatrix) {
         return result;
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/DDDefinitions.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/DDDefinitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/DDpackageConfig.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/DDpackageConfig.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,72 @@
 #pragma once
 
+#include "operations/OpType.hpp"
+
 #include <cstddef>
 
 namespace dd {
 struct DDPackageConfig {
   // Note the order of parameters here must be the *same* as in the template
   // definition.
   static constexpr std::size_t UT_VEC_NBUCKET = 32768U;
   static constexpr std::size_t UT_VEC_INITIAL_ALLOCATION_SIZE = 2048U;
   static constexpr std::size_t UT_MAT_NBUCKET = 32768U;
   static constexpr std::size_t UT_MAT_INITIAL_ALLOCATION_SIZE = 2048U;
   static constexpr std::size_t CT_VEC_ADD_NBUCKET = 16384U;
   static constexpr std::size_t CT_MAT_ADD_NBUCKET = 16384U;
+  static constexpr std::size_t CT_VEC_ADD_MAG_NBUCKET = 16384U;
+  static constexpr std::size_t CT_MAT_ADD_MAG_NBUCKET = 16384U;
+  static constexpr std::size_t CT_VEC_CONJ_NBUCKET = 4096U;
   static constexpr std::size_t CT_MAT_CONJ_TRANS_NBUCKET = 4096U;
   static constexpr std::size_t CT_MAT_VEC_MULT_NBUCKET = 16384U;
   static constexpr std::size_t CT_MAT_MAT_MULT_NBUCKET = 16384U;
   static constexpr std::size_t CT_VEC_KRON_NBUCKET = 4096U;
   static constexpr std::size_t CT_MAT_KRON_NBUCKET = 4096U;
   static constexpr std::size_t CT_VEC_INNER_PROD_NBUCKET = 4096U;
   static constexpr std::size_t CT_DM_NOISE_NBUCKET = 1U;
   static constexpr std::size_t UT_DM_NBUCKET = 1U;
   static constexpr std::size_t UT_DM_INITIAL_ALLOCATION_SIZE = 1U;
   static constexpr std::size_t CT_DM_DM_MULT_NBUCKET = 1U;
   static constexpr std::size_t CT_DM_ADD_NBUCKET = 1U;
 
   // The number of different quantum operations. I.e., the number of operations
-  // defined in the QFR OpType.hpp This parameter is required to initialize the
+  // defined in OpType.hpp. This parameter is required to initialize the
   // StochasticNoiseOperationTable.hpp
   static constexpr std::size_t STOCHASTIC_CACHE_OPS = 1;
 };
+
+struct StochasticNoiseSimulatorDDPackageConfig : public dd::DDPackageConfig {
+  static constexpr std::size_t STOCHASTIC_CACHE_OPS = qc::OpType::OpCount;
+
+  static constexpr std::size_t CT_VEC_ADD_MAG_NBUCKET = 1U;
+  static constexpr std::size_t CT_MAT_ADD_MAG_NBUCKET = 1U;
+  static constexpr std::size_t CT_VEC_CONJ_NBUCKET = 1U;
+};
+
+struct DensityMatrixSimulatorDDPackageConfig : public dd::DDPackageConfig {
+  static constexpr std::size_t UT_DM_NBUCKET = 65536U;
+  static constexpr std::size_t UT_DM_INITIAL_ALLOCATION_SIZE = 4096U;
+
+  static constexpr std::size_t CT_DM_DM_MULT_NBUCKET = 16384U;
+  static constexpr std::size_t CT_DM_ADD_NBUCKET = 16384U;
+  static constexpr std::size_t CT_DM_NOISE_NBUCKET = 4096U;
+
+  static constexpr std::size_t UT_MAT_NBUCKET = 16384U;
+  static constexpr std::size_t CT_MAT_ADD_NBUCKET = 4096U;
+  static constexpr std::size_t CT_VEC_ADD_NBUCKET = 4096U;
+  static constexpr std::size_t CT_MAT_CONJ_TRANS_NBUCKET = 4096U;
+
+  static constexpr std::size_t CT_MAT_MAT_MULT_NBUCKET = 1U;
+  static constexpr std::size_t CT_MAT_VEC_MULT_NBUCKET = 1U;
+  static constexpr std::size_t UT_VEC_NBUCKET = 1U;
+  static constexpr std::size_t UT_VEC_INITIAL_ALLOCATION_SIZE = 1U;
+  static constexpr std::size_t UT_MAT_INITIAL_ALLOCATION_SIZE = 1U;
+  static constexpr std::size_t CT_VEC_KRON_NBUCKET = 1U;
+  static constexpr std::size_t CT_MAT_KRON_NBUCKET = 1U;
+  static constexpr std::size_t CT_VEC_INNER_PROD_NBUCKET = 1U;
+  static constexpr std::size_t STOCHASTIC_CACHE_OPS = 1U;
+  static constexpr std::size_t CT_VEC_ADD_MAG_NBUCKET = 1U;
+  static constexpr std::size_t CT_MAT_ADD_MAG_NBUCKET = 1U;
+  static constexpr std::size_t CT_VEC_CONJ_NBUCKET = 1U;
+};
 } // namespace dd
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/DensityNoiseTable.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/DensityNoiseTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Edge.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Edge.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -111,21 +111,22 @@
    */
   [[nodiscard]] constexpr bool isOneTerminal() const {
     return isTerminal() && w.exactlyOne();
   }
 
   /**
    * @brief Get a single element of the vector or matrix represented by the DD
+   * @param numQubits number of qubits in the considered DD
    * @param decisions string {0, 1, 2, 3}^n describing which outgoing edge
    * should be followed (for vectors entries are limited to 0 and 1) If string
    * is longer than required, the additional characters are ignored.
    * @return the complex amplitude of the specified element
    */
   [[nodiscard]] std::complex<fp>
-  getValueByPath(const std::string& decisions) const;
+  getValueByPath(std::size_t numQubits, const std::string& decisions) const;
 
   /**
    * @brief Get the size of the DD
    * @details The size of a DD is defined as the number of nodes (including the
    * terminal node) in the DD.
    * @return the size of the DD
    */
@@ -240,73 +241,87 @@
 
   /**
    * @brief Check whether the matrix represented by the DD is the identity
    * @tparam T template parameter to enable this function only for matrix nodes
    * @return whether the matrix is the identity
    */
   template <typename T = Node, isMatrixVariant<T> = true>
-  [[nodiscard]] bool isIdentity() const {
-    return Node::isIdentity(p);
+  [[nodiscard]] bool isIdentity(const bool upToGlobalPhase = true) const {
+    if (!isTerminal()) {
+      return false;
+    }
+    if (upToGlobalPhase) {
+      return !w.exactlyZero();
+    }
+    return w.exactlyOne();
   }
 
   /**
    * @brief Get a single element of the matrix represented by the DD
    * @tparam T template parameter to enable this function only for matrix nodes
+   * @param numQubits number of qubits in the considered DD
    * @param i row index of the element
    * @param j column index of the element
    * @return the complex value of the entry
    */
   template <typename T = Node, isMatrixVariant<T> = true>
-  [[nodiscard]] std::complex<fp> getValueByIndex(std::size_t i,
-                                                 std::size_t j) const;
+  [[nodiscard]] std::complex<fp>
+  getValueByIndex(std::size_t numQubits, std::size_t i, std::size_t j) const;
 
   /**
    * @brief Get the matrix represented by the DD
    * @tparam T template parameter to enable this function only for matrix nodes
+   * @param numQubits number of qubits in the considered DD
    * @param threshold entries with a magnitude below this threshold will be
    * ignored
    * @return the matrix
    */
   template <typename T = Node, isMatrixVariant<T> = true>
-  [[nodiscard]] CMat getMatrix(fp threshold = 0.) const;
+  [[nodiscard]] CMat getMatrix(std::size_t numQubits, fp threshold = 0.) const;
 
   /**
    * @brief Get the sparse matrix represented by the DD
    * @tparam T template parameter to enable this function only for matrix nodes
+   * @param numQubits number of qubits in the considered DD
    * @param threshold entries with a magnitude below this threshold will be
    * ignored
    * @return the sparse matrix
    */
   template <typename T = Node, isMatrixVariant<T> = true>
-  [[nodiscard]] SparseCMat getSparseMatrix(fp threshold = 0.) const;
+  [[nodiscard]] SparseCMat getSparseMatrix(std::size_t numQubits,
+                                           fp threshold = 0.) const;
 
   /**
    * @brief Print the matrix represented by the DD
    * @tparam T template parameter to enable this function only for matrix nodes
+   * @param numQubits number of qubits in the considered DD
    * @note This function scales exponentially with the number of qubits.
    */
   template <typename T = Node, isMatrixVariant<T> = true>
-  void printMatrix() const;
+  void printMatrix(std::size_t numQubits) const;
 
 private:
   /**
    * @brief Recursively traverse the DD and call a function for each non-zero
    * matrix entry.
    * @tparam T template parameter to enable this function only for matrix nodes
    * @param amp the accumulated amplitude from previous traversals
    * @param i the current row index in the matrix
    * @param j the current column index in the matrix
    * @param f This function is called for each non-zero matrix entry with the
    * row index, the column index and the amplitude as arguments.
+   * @param level the current level in the DD (ranges from 1 to n for regular
+   * nodes and is 0 for the terminal node)
    * @param threshold entries with a magnitude below this threshold will be
    * ignored
    */
   template <typename T = Node, isMatrixVariant<T> = true>
   void traverseMatrix(const std::complex<fp>& amp, std::size_t i, std::size_t j,
-                      MatrixEntryFunc f, fp threshold = 0.) const;
+                      MatrixEntryFunc f, std::size_t level,
+                      fp threshold = 0.) const;
 
   ///---------------------------------------------------------------------------
   ///                  \n Methods for density matrix DDs \n
   ///---------------------------------------------------------------------------
 public:
   template <typename T = Node, isDensityMatrix<T> = true>
   [[maybe_unused]] static void setDensityConjugateTrue(Edge& e) {
@@ -349,44 +364,50 @@
   static void applyDmChangesToEdge(Edge& x) {
     Node::applyDmChangesToNode(x.p);
   }
 
   /**
    * @brief Get the sparse probability vector for the underlying density matrix
    * @tparam T template parameter to enable this function only for dNode
+   * @param numQubits number of qubits in the considered DD
    * @param threshold probabilities below this threshold will be ignored
    * @return the sparse probability vector
    */
   template <typename T = Node, isDensityMatrix<T> = true>
-  [[nodiscard]] SparsePVec getSparseProbabilityVector(fp threshold = 0.) const;
+  [[nodiscard]] SparsePVec getSparseProbabilityVector(std::size_t numQubits,
+                                                      fp threshold = 0.) const;
 
   /**
    * @brief Get the sparse probability vector for the underlying density matrix
    * @tparam T template parameter to enable this function only for dNode
+   * @param numQubits number of qubits in the considered DD
    * @param threshold probabilities below this threshold will be ignored
    * @return the sparse probability vector (using strings as keys)
    */
   template <typename T = Node, isDensityMatrix<T> = true>
   [[nodiscard]] SparsePVecStrKeys
-  getSparseProbabilityVectorStrKeys(fp threshold = 0.) const;
+  getSparseProbabilityVectorStrKeys(std::size_t numQubits,
+                                    fp threshold = 0.) const;
 
 private:
   /**
    * @brief Recursively traverse diagonal of the DD and call a function for each
    * non-zero entry.
    * @tparam T template parameter to enable this function only for dNode
    * @param prob the accumulated probability from previous traversals
    * @param i the current diagonal index in the matrix
    * @param f This function is called for each non-zero entry with the
    * diagonal index and the probability as arguments.
+   * @param level the current level in the DD (ranges from 1 to n for regular
+   * nodes and is 0 for the terminal node)
    * @param threshold probabilities below this threshold will be ignored
    */
   template <typename T = Node, isDensityMatrix<T> = true>
   void traverseDiagonal(const fp& prob, std::size_t i, ProbabilityFunc f,
-                        fp threshold = 0.) const;
+                        std::size_t level, fp threshold = 0.) const;
 };
 } // namespace dd
 
 ///-----------------------------------------------------------------------------
 ///                         \n Hash related code \n
 ///-----------------------------------------------------------------------------
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Export.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Export.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/FunctionalityConstruction.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/FunctionalityConstruction.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/GateMatrixDefinitions.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/GateMatrixDefinitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/MemoryManager.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/MemoryManager.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Node.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Node.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -35,71 +35,53 @@
  */
 struct mNode {                        // NOLINT(readability-identifier-naming)
   std::array<Edge<mNode>, NEDGE> e{}; // edges out of this node
   mNode* next{};                      // used to link nodes in unique table
   RefCount ref{};                     // reference count
   Qubit v{};                          // variable index
   std::uint8_t flags = 0;
-  // 32 = unused (was used to mark a node with is symmetric).
-  // 16 = marks a node resembling identity
+  // 32 = unused (was used to mark a node which is symmetric)
+  // 16 = unused (was used to mark a node resembling the identity)
   // 8 = marks a reduced dm node,
   // 4 = marks a dm (tmp flag),
   // 2 = mark first path edge (tmp flag),
-  // 1 = mark path is conjugated (tmp flag))
+  // 1 = mark path is conjugated (tmp flag)
 
   [[nodiscard]] static constexpr bool isTerminal(const mNode* p) noexcept {
     return p == nullptr;
   }
   [[nodiscard]] static constexpr mNode* getTerminal() noexcept {
     return nullptr;
   }
-
-  [[nodiscard]] inline bool isIdentity() const noexcept {
-    return (flags & static_cast<std::uint8_t>(16U)) != 0;
-  }
-  [[nodiscard]] static constexpr bool isIdentity(const mNode* p) noexcept {
-    return p == nullptr || p->isIdentity();
-  }
-  inline void setIdentity(const bool identity) noexcept {
-    if (identity) {
-      flags = (flags | static_cast<std::uint8_t>(16U));
-    } else {
-      flags = (flags & static_cast<std::uint8_t>(~16U));
-    }
-  }
 };
 using mEdge = Edge<mNode>;
 using mCachedEdge = CachedEdge<mNode>;
 
 /**
  * @brief A density matrix DD node
  * @details Data Layout |24|24|24|24|8|4|2|1| = 111B (space for one more byte)
  */
 struct dNode {                        // NOLINT(readability-identifier-naming)
   std::array<Edge<dNode>, NEDGE> e{}; // edges out of this node
   dNode* next{};                      // used to link nodes in unique table
   RefCount ref{};                     // reference count
   Qubit v{};                          // variable index
   std::uint8_t flags = 0;
-  // 32 = unused (was used to mark a node with is symmetric).
-  // 16 = marks a node resembling identity
+  // 32 = unused (was used to mark a node which is symmetric)
+  // 16 = unused (was used to mark a node resembling the identity)
   // 8 = marks a reduced dm node,
   // 4 = marks a dm (tmp flag),
   // 2 = mark first path edge (tmp flag),
-  // 1 = mark path is conjugated (tmp flag))
+  // 1 = mark path is conjugated (tmp flag)
 
-  static constexpr bool isTerminal(const dNode* p) noexcept {
-    return p == nullptr;
+  static bool isTerminal(const dNode* p) noexcept {
+    return (reinterpret_cast<std::uintptr_t>(p) & (~7ULL)) == 0ULL;
   }
   static constexpr dNode* getTerminal() noexcept { return nullptr; }
 
-  [[nodiscard]] static constexpr bool isIdentity(const dNode* p) noexcept {
-    return p == nullptr;
-  }
-
   [[nodiscard]] [[maybe_unused]] static constexpr bool
   tempDensityMatrixFlagsEqual(const std::uint8_t a,
                               const std::uint8_t b) noexcept {
     return getDensityMatrixTempFlags(a) == getDensityMatrixTempFlags(b);
   }
 
   [[nodiscard]] static constexpr bool
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/NoiseFunctionality.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/NoiseFunctionality.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,468 +1,444 @@
-#pragma once
+#include "dd/NoiseFunctionality.hpp"
 
-#include "dd/ComplexNumbers.hpp"
-#include "dd/GateMatrixDefinitions.hpp"
-#include "dd/Node.hpp"
-#include "dd/Package.hpp"
-#include "operations/OpType.hpp"
-#include "operations/Operation.hpp"
-
-#include <algorithm>
-#include <array>
-#include <cassert>
-#include <complex>
-#include <map>
-#include <optional>
-#include <random>
-#include <utility>
-#include <vector>
+namespace {
 
-namespace dd {
-
-using NrEdges = std::tuple_size<decltype(dNode::e)>;
-using ArrayOfEdges = std::array<dCachedEdge, NrEdges::value>;
-
-// noise operations available for deterministic noise aware quantum circuit
-// simulation
-enum NoiseOperations : std::uint8_t {
-  AmplitudeDamping,
-  PhaseFlip,
-  Depolarization,
-  Identity
-};
-
-template <class Config> class StochasticNoiseFunctionality {
-public:
-  StochasticNoiseFunctionality(const std::unique_ptr<Package<Config>>& dd,
-                               const std::size_t nq,
-                               double gateNoiseProbability,
-                               double amplitudeDampingProb,
-                               double multiQubitGateFactor,
-                               std::vector<NoiseOperations> effects)
-      : package(dd), nQubits(nq), dist(0.0, 1.0L),
-        noiseProbability(gateNoiseProbability),
-        noiseProbabilityMulti(gateNoiseProbability * multiQubitGateFactor),
-        sqrtAmplitudeDampingProbability(std::sqrt(amplitudeDampingProb)),
-        oneMinusSqrtAmplitudeDampingProbability(
-            std::sqrt(1 - amplitudeDampingProb)),
-        sqrtAmplitudeDampingProbabilityMulti(std::sqrt(gateNoiseProbability) *
-                                             multiQubitGateFactor),
-        oneMinusSqrtAmplitudeDampingProbabilityMulti(
-            std::sqrt(1 - multiQubitGateFactor * amplitudeDampingProb)),
-        ampDampingTrue({0, sqrtAmplitudeDampingProbability, 0, 0}),
-        ampDampingTrueMulti({0, sqrtAmplitudeDampingProbabilityMulti, 0, 0}),
-        ampDampingFalse({1, 0, 0, oneMinusSqrtAmplitudeDampingProbability}),
-        ampDampingFalseMulti(
-            {1, 0, 0, oneMinusSqrtAmplitudeDampingProbabilityMulti}),
-        noiseEffects(std::move(effects)),
-        identityDD(package->makeIdent(nQubits)) {
-    package->incRef(identityDD);
-  }
-
-  ~StochasticNoiseFunctionality() { package->decRef(identityDD); }
-
-protected:
-  // NOLINTNEXTLINE(cppcoreguidelines-avoid-const-or-ref-data-members)
-  const std::unique_ptr<Package<Config>>& package;
-  std::size_t nQubits;
-  std::uniform_real_distribution<fp> dist;
-
-  double noiseProbability;
-  double noiseProbabilityMulti;
-  fp sqrtAmplitudeDampingProbability;
-  fp oneMinusSqrtAmplitudeDampingProbability;
-  fp sqrtAmplitudeDampingProbabilityMulti;
-  fp oneMinusSqrtAmplitudeDampingProbabilityMulti;
-  GateMatrix ampDampingTrue{};
-  GateMatrix ampDampingTrueMulti{};
-  GateMatrix ampDampingFalse{};
-  GateMatrix ampDampingFalseMulti{};
-  std::vector<NoiseOperations> noiseEffects;
-  mEdge identityDD;
-
-  [[nodiscard]] std::size_t getNumberOfQubits() const { return nQubits; }
-  [[nodiscard]] double getNoiseProbability(bool multiQubitNoiseFlag) const {
-    return multiQubitNoiseFlag ? noiseProbabilityMulti : noiseProbability;
-  }
-
-  [[nodiscard]] qc::OpType
-  getAmplitudeDampingOperationType(bool multiQubitNoiseFlag,
-                                   bool amplitudeDampingFlag) const {
-    if (amplitudeDampingFlag) {
-      return multiQubitNoiseFlag ? qc::MultiATrue : qc::ATrue;
-    }
-    return multiQubitNoiseFlag ? qc::MultiAFalse : qc::AFalse;
-  }
-
-  [[nodiscard]] GateMatrix
-  getAmplitudeDampingOperationMatrix(bool multiQubitNoiseFlag,
-                                     bool amplitudeDampingFlag) const {
-    if (amplitudeDampingFlag) {
-      return multiQubitNoiseFlag ? ampDampingTrueMulti : ampDampingTrue;
-    }
-    return multiQubitNoiseFlag ? ampDampingFalseMulti : ampDampingFalse;
-  }
-
-public:
-  [[nodiscard]] mEdge getIdentityDD() const { return identityDD; }
-  void setNoiseEffects(std::vector<NoiseOperations> newNoiseEffects) {
-    noiseEffects = std::move(newNoiseEffects);
-  }
-
-  void applyNoiseOperation(const std::set<qc::Qubit>& targets, mEdge operation,
-                           vEdge& state, std::mt19937_64& generator) {
-    const bool multiQubitOperation = targets.size() > 1;
-
-    for (const auto& target : targets) {
-      auto stackedOperation = generateNoiseOperation(
-          operation, target, generator, false, multiQubitOperation);
-      auto tmp = package->multiply(stackedOperation, state);
-
-      if (ComplexNumbers::mag2(tmp.w) < dist(generator)) {
-        // The probability of amplitude damping does not only depend on the
-        // noise probability, but also the quantum state. Due to the
-        // normalization constraint of decision diagrams the probability for
-        // applying amplitude damping stands in the root edge weight, of the dd
-        // after the noise has been applied
-        stackedOperation = generateNoiseOperation(operation, target, generator,
-                                                  true, multiQubitOperation);
-        tmp = package->multiply(stackedOperation, state);
-      }
-      tmp.w = Complex::one();
-
-      package->incRef(tmp);
-      package->decRef(state);
-      state = tmp;
-
-      // I only need to apply the operations once
-      operation = identityDD;
+std::vector<dd::NoiseOperations>
+initializeNoiseEffects(const std::string& cNoiseEffects) {
+  std::vector<dd::NoiseOperations> noiseOperationVector{};
+  for (const auto noise : cNoiseEffects) {
+    switch (noise) {
+    case 'A':
+      noiseOperationVector.push_back(dd::AmplitudeDamping);
+      break;
+    case 'P':
+      noiseOperationVector.push_back(dd::PhaseFlip);
+      break;
+    case 'D':
+      noiseOperationVector.push_back(dd::Depolarization);
+      break;
+    case 'I':
+      noiseOperationVector.push_back(dd::Identity);
+      break;
+    default:
+      throw std::runtime_error("Unknown noise operation '" + cNoiseEffects +
+                               "'\n");
     }
   }
+  return noiseOperationVector;
+}
+} // namespace
 
-protected:
-  [[nodiscard]] mEdge stackOperation(mEdge operation, const qc::Qubit target,
-                                     const qc::OpType noiseOperation,
-                                     const GateMatrix matrix) {
-    if (const auto* op = package->stochasticNoiseOperationCache.lookup(
-            noiseOperation, target);
-        op != nullptr) {
-      return package->multiply(*op, operation);
-    }
-    const auto gateDD =
-        package->makeGateDD(matrix, getNumberOfQubits(), target);
-    package->stochasticNoiseOperationCache.insert(noiseOperation, target,
-                                                  gateDD);
-    return package->multiply(gateDD, operation);
-  }
-
-  mEdge generateNoiseOperation(mEdge operation, qc::Qubit target,
-                               std::mt19937_64& generator,
-                               bool amplitudeDamping,
-                               bool multiQubitOperation) {
-    for (const auto& noiseType : noiseEffects) {
-      const auto effect = noiseType == AmplitudeDamping
-                              ? getAmplitudeDampingOperationType(
-                                    multiQubitOperation, amplitudeDamping)
-                              : returnNoiseOperation(noiseType, dist(generator),
-                                                     multiQubitOperation);
-      switch (effect) {
-      case (qc::I): {
-        continue;
-      }
-      case (qc::MultiATrue):
-      case (qc::ATrue): {
-        const GateMatrix amplitudeDampingMatrix =
-            getAmplitudeDampingOperationMatrix(multiQubitOperation, true);
-        operation =
-            stackOperation(operation, target, effect, amplitudeDampingMatrix);
-        break;
-      }
-      case (qc::MultiAFalse):
-      case (qc::AFalse): {
-        const GateMatrix amplitudeDampingMatrix =
-            getAmplitudeDampingOperationMatrix(multiQubitOperation, false);
-        operation =
-            stackOperation(operation, target, effect, amplitudeDampingMatrix);
-        break;
-      }
-      case (qc::X): {
-        operation = stackOperation(operation, target, effect, X_MAT);
-        break;
-      }
-      case (qc::Y): {
-        operation = stackOperation(operation, target, effect, Y_MAT);
-        break;
-      }
-      case (qc::Z): {
-        operation = stackOperation(operation, target, effect, Z_MAT);
-        break;
-      }
-      default: {
-        throw std::runtime_error("Unknown noise operation '" +
-                                 std::to_string(effect) + "'\n");
-      }
-      }
+namespace dd {
+StochasticNoiseFunctionality::StochasticNoiseFunctionality(
+    const std::unique_ptr<Package<StochasticNoiseSimulatorDDPackageConfig>>& dd,
+    const std::size_t nq, double gateNoiseProbability,
+    double amplitudeDampingProb, double multiQubitGateFactor,
+    const std::string& cNoiseEffects)
+    : package(dd.get()), nQubits(nq), dist(0.0, 1.0L),
+      noiseProbability(gateNoiseProbability),
+      noiseProbabilityMulti(gateNoiseProbability * multiQubitGateFactor),
+      sqrtAmplitudeDampingProbability(std::sqrt(amplitudeDampingProb)),
+      oneMinusSqrtAmplitudeDampingProbability(
+          std::sqrt(1 - amplitudeDampingProb)),
+      sqrtAmplitudeDampingProbabilityMulti(std::sqrt(gateNoiseProbability) *
+                                           multiQubitGateFactor),
+      oneMinusSqrtAmplitudeDampingProbabilityMulti(
+          std::sqrt(1 - multiQubitGateFactor * amplitudeDampingProb)),
+      ampDampingTrue({0, sqrtAmplitudeDampingProbability, 0, 0}),
+      ampDampingTrueMulti({0, sqrtAmplitudeDampingProbabilityMulti, 0, 0}),
+      ampDampingFalse({1, 0, 0, oneMinusSqrtAmplitudeDampingProbability}),
+      ampDampingFalseMulti(
+          {1, 0, 0, oneMinusSqrtAmplitudeDampingProbabilityMulti}),
+      noiseEffects(initializeNoiseEffects(cNoiseEffects)),
+      identityDD(package->makeIdent()) {
+  sanityCheckOfNoiseProbabilities(gateNoiseProbability, amplitudeDampingProb,
+                                  multiQubitGateFactor);
+  package->incRef(identityDD);
+}
+
+double StochasticNoiseFunctionality::getNoiseProbability(
+    bool multiQubitNoiseFlag) const {
+  return multiQubitNoiseFlag ? noiseProbabilityMulti : noiseProbability;
+}
+
+qc::OpType StochasticNoiseFunctionality::getAmplitudeDampingOperationType(
+    const bool multiQubitNoiseFlag, const bool amplitudeDampingFlag) {
+  if (amplitudeDampingFlag) {
+    return multiQubitNoiseFlag ? qc::MultiATrue : qc::ATrue;
+  }
+  return multiQubitNoiseFlag ? qc::MultiAFalse : qc::AFalse;
+}
+
+GateMatrix StochasticNoiseFunctionality::getAmplitudeDampingOperationMatrix(
+    const bool multiQubitNoiseFlag, const bool amplitudeDampingFlag) const {
+  if (amplitudeDampingFlag) {
+    return multiQubitNoiseFlag ? ampDampingTrueMulti : ampDampingTrue;
+  }
+  return multiQubitNoiseFlag ? ampDampingFalseMulti : ampDampingFalse;
+}
+
+void StochasticNoiseFunctionality::applyNoiseOperation(
+    const std::set<qc::Qubit>& targets, mEdge operation, vEdge& state,
+    std::mt19937_64& generator) {
+  const bool multiQubitOperation = targets.size() > 1;
+
+  for (const auto& target : targets) {
+    auto stackedOperation = generateNoiseOperation(operation, target, generator,
+                                                   false, multiQubitOperation);
+    auto tmp = package->multiply(stackedOperation, state);
+
+    if (ComplexNumbers::mag2(tmp.w) < dist(generator)) {
+      // The probability of amplitude damping does not only depend on the
+      // noise probability, but also the quantum state. Due to the
+      // normalization constraint of decision diagrams the probability for
+      // applying amplitude damping stands in the root edge weight, of the dd
+      // after the noise has been applied
+      stackedOperation = generateNoiseOperation(operation, target, generator,
+                                                true, multiQubitOperation);
+      tmp = package->multiply(stackedOperation, state);
+    }
+    tmp.w = Complex::one();
+
+    package->incRef(tmp);
+    package->decRef(state);
+    state = tmp;
+
+    // I only need to apply the operations once
+    operation = identityDD;
+  }
+}
+
+mEdge StochasticNoiseFunctionality::stackOperation(
+    mEdge operation, const qc::Qubit target, const qc::OpType noiseOperation,
+    const GateMatrix matrix) {
+  if (const auto* op =
+          package->stochasticNoiseOperationCache.lookup(noiseOperation, target);
+      op != nullptr) {
+    return package->multiply(*op, operation);
+  }
+  const auto gateDD = package->makeGateDD(matrix, target);
+  package->stochasticNoiseOperationCache.insert(noiseOperation, target, gateDD);
+  return package->multiply(gateDD, operation);
+}
+
+mEdge StochasticNoiseFunctionality::generateNoiseOperation(
+    mEdge operation, qc::Qubit target, std::mt19937_64& generator,
+    const bool amplitudeDamping, const bool multiQubitOperation) {
+  for (const auto& noiseType : noiseEffects) {
+    const auto effect = noiseType == AmplitudeDamping
+                            ? getAmplitudeDampingOperationType(
+                                  multiQubitOperation, amplitudeDamping)
+                            : returnNoiseOperation(noiseType, dist(generator),
+                                                   multiQubitOperation);
+    switch (effect) {
+    case (qc::I): {
+      continue;
+    }
+    case (qc::MultiATrue):
+    case (qc::ATrue): {
+      const GateMatrix amplitudeDampingMatrix =
+          getAmplitudeDampingOperationMatrix(multiQubitOperation, true);
+      operation =
+          stackOperation(operation, target, effect, amplitudeDampingMatrix);
+      break;
+    }
+    case (qc::MultiAFalse):
+    case (qc::AFalse): {
+      const GateMatrix amplitudeDampingMatrix =
+          getAmplitudeDampingOperationMatrix(multiQubitOperation, false);
+      operation =
+          stackOperation(operation, target, effect, amplitudeDampingMatrix);
+      break;
+    }
+    case (qc::X): {
+      operation = stackOperation(operation, target, effect, X_MAT);
+      break;
+    }
+    case (qc::Y): {
+      operation = stackOperation(operation, target, effect, Y_MAT);
+      break;
+    }
+    case (qc::Z): {
+      operation = stackOperation(operation, target, effect, Z_MAT);
+      break;
+    }
+    default: {
+      throw std::runtime_error("Unknown noise operation '" +
+                               std::to_string(effect) + "'\n");
+    }
+    }
+  }
+  return operation;
+}
+
+qc::OpType StochasticNoiseFunctionality::returnNoiseOperation(
+    NoiseOperations noiseOperation, const double prob,
+    const bool multiQubitNoiseFlag) const {
+  switch (noiseOperation) {
+  case NoiseOperations::Depolarization: {
+    if (prob >= (getNoiseProbability(multiQubitNoiseFlag) * 0.75)) {
+      // prob > prob apply qc::I, also 25 % of the time when depolarization is
+      // applied nothing happens
+      return qc::I;
     }
-    return operation;
+    if (prob < (getNoiseProbability(multiQubitNoiseFlag) * 0.25)) {
+      // if 0 < prob < 0.25 (25 % of the time when applying depolarization)
+      // apply qc::X
+      return qc::X;
+    }
+    if (prob < (getNoiseProbability(multiQubitNoiseFlag) * 0.5)) {
+      // if 0.25 < prob < 0.5 (25 % of the time when applying depolarization)
+      // apply qc::Y
+      return qc::Y;
+    }
+    // if 0.5 < prob < 0.75 (25 % of the time when applying depolarization)
+    // apply qc::Z
+    return qc::Z;
   }
-
-  [[nodiscard]] qc::OpType
-  returnNoiseOperation(NoiseOperations noiseOperation, double prob,
-                       bool multiQubitNoiseFlag) const {
-    switch (noiseOperation) {
-    case NoiseOperations::Depolarization: {
-      if (prob >= (getNoiseProbability(multiQubitNoiseFlag) * 0.75)) {
-        // prob > prob apply qc::I, also 25 % of the time when depolarization is
-        // applied nothing happens
-        return qc::I;
-      }
-      if (prob < (getNoiseProbability(multiQubitNoiseFlag) * 0.25)) {
-        // if 0 < prob < 0.25 (25 % of the time when applying depolarization)
-        // apply qc::X
-        return qc::X;
-      }
-      if (prob < (getNoiseProbability(multiQubitNoiseFlag) * 0.5)) {
-        // if 0.25 < prob < 0.5 (25 % of the time when applying depolarization)
-        // apply qc::Y
-        return qc::Y;
-      }
-      // if 0.5 < prob < 0.75 (25 % of the time when applying depolarization)
-      // apply qc::Z
-      return qc::Z;
-    }
-    case NoiseOperations::PhaseFlip: {
-      if (prob > getNoiseProbability(multiQubitNoiseFlag)) {
-        return qc::I;
-      }
-      return qc::Z;
-    }
-    case NoiseOperations::Identity: {
+  case NoiseOperations::PhaseFlip: {
+    if (prob > getNoiseProbability(multiQubitNoiseFlag)) {
       return qc::I;
     }
-    default:
-      throw std::runtime_error(std::string{"Unknown noise effect '"} +
-                               std::to_string(noiseOperation) + "'");
-    }
+    return qc::Z;
   }
-};
-
-template <class Config> class DeterministicNoiseFunctionality {
-public:
-  DeterministicNoiseFunctionality(const std::unique_ptr<Package<Config>>& dd,
-                                  const std::size_t nq,
-                                  double noiseProbabilitySingleQubit,
-                                  double noiseProbabilityMultiQubit,
-                                  double ampDampProbSingleQubit,
-                                  double ampDampProbMultiQubit,
-                                  std::vector<NoiseOperations> effects)
-      : package(dd), nQubits(nq),
-        noiseProbSingleQubit(noiseProbabilitySingleQubit),
-        noiseProbMultiQubit(noiseProbabilityMultiQubit),
-        ampDampingProbSingleQubit(ampDampProbSingleQubit),
-        ampDampingProbMultiQubit(ampDampProbMultiQubit),
-        noiseEffects(std::move(effects)) {}
-
-protected:
-  // NOLINTNEXTLINE(cppcoreguidelines-avoid-const-or-ref-data-members)
-  const std::unique_ptr<Package<Config>>& package;
-  std::size_t nQubits;
-
-  double noiseProbSingleQubit;
-  double noiseProbMultiQubit;
-  double ampDampingProbSingleQubit;
-  double ampDampingProbMultiQubit;
-
-  std::vector<NoiseOperations> noiseEffects;
-
-  [[nodiscard]] std::size_t getNumberOfQubits() const { return nQubits; }
-
-public:
-  void applyNoiseEffects(dEdge& originalEdge,
-                         const std::unique_ptr<qc::Operation>& qcOperation) {
-    auto usedQubits = qcOperation->getUsedQubits();
-    dCachedEdge nodeAfterNoise = {};
-    dEdge::applyDmChangesToEdge(originalEdge);
-    nodeAfterNoise = applyNoiseEffects(originalEdge, usedQubits, false);
-    dEdge::revertDmChangesToEdge(originalEdge);
-    auto r = dEdge{nodeAfterNoise.p, package->cn.lookup(nodeAfterNoise.w)};
-    package->incRef(r);
-    dEdge::alignDensityEdge(originalEdge);
-    package->decRef(originalEdge);
-    originalEdge = r;
-    dEdge::setDensityMatrixTrue(originalEdge);
-  }
-
-private:
-  dCachedEdge applyNoiseEffects(dEdge& originalEdge,
-                                const std::set<qc::Qubit>& usedQubits,
-                                bool firstPathEdge) {
-    const auto originalWeight = static_cast<ComplexValue>(originalEdge.w);
-    if (originalEdge.isTerminal() || originalEdge.p->v < *usedQubits.begin()) {
-      return {originalEdge.p, originalWeight};
-    }
-
-    auto originalCopy = dEdge{originalEdge.p, Complex::one()};
-    ArrayOfEdges newEdges{};
+  case NoiseOperations::Identity: {
+    return qc::I;
+  }
+  default:
+    throw std::runtime_error(std::string{"Unknown noise effect '"} +
+                             std::to_string(noiseOperation) + "'");
+  }
+}
+
+DeterministicNoiseFunctionality::DeterministicNoiseFunctionality(
+    const std::unique_ptr<Package<DensityMatrixSimulatorDDPackageConfig>>& dd,
+    const std::size_t nq, double noiseProbabilitySingleQubit,
+    double noiseProbabilityMultiQubit, double ampDampProbSingleQubit,
+    double ampDampProbMultiQubit, const std::string& cNoiseEffects)
+    : package(dd.get()), nQubits(nq),
+      noiseProbSingleQubit(noiseProbabilitySingleQubit),
+      noiseProbMultiQubit(noiseProbabilityMultiQubit),
+      ampDampingProbSingleQubit(ampDampProbSingleQubit),
+      ampDampingProbMultiQubit(ampDampProbMultiQubit),
+      noiseEffects(initializeNoiseEffects(cNoiseEffects)) {
+  sanityCheckOfNoiseProbabilities(noiseProbabilitySingleQubit,
+                                  ampDampProbSingleQubit, 1);
+  sanityCheckOfNoiseProbabilities(noiseProbabilityMultiQubit,
+                                  ampDampProbMultiQubit, 1);
+}
+
+void DeterministicNoiseFunctionality::applyNoiseEffects(
+    dEdge& originalEdge, const std::unique_ptr<qc::Operation>& qcOperation) {
+  auto usedQubits = qcOperation->getUsedQubits();
+  dCachedEdge nodeAfterNoise = {};
+  dEdge::applyDmChangesToEdge(originalEdge);
+  nodeAfterNoise = applyNoiseEffects(originalEdge, usedQubits, false,
+                                     static_cast<Qubit>(nQubits));
+  dEdge::revertDmChangesToEdge(originalEdge);
+  auto r = dEdge{nodeAfterNoise.p, package->cn.lookup(nodeAfterNoise.w)};
+  package->incRef(r);
+  dEdge::alignDensityEdge(originalEdge);
+  package->decRef(originalEdge);
+  originalEdge = r;
+  dEdge::setDensityMatrixTrue(originalEdge);
+}
+
+dCachedEdge DeterministicNoiseFunctionality::applyNoiseEffects(
+    dEdge& originalEdge, const std::set<qc::Qubit>& usedQubits,
+    const bool firstPathEdge, const Qubit level) {
+
+  const auto originalWeight = static_cast<ComplexValue>(originalEdge.w);
+  if (originalEdge.isZeroTerminal() || level <= *usedQubits.begin()) {
+    return {originalEdge.p, originalWeight};
+  }
+
+  auto originalCopy = dEdge{originalEdge.p, Complex::one()};
+  ArrayOfEdges newEdges{};
+  const auto nextLevel = static_cast<dd::Qubit>(level - 1U);
+  if (originalEdge.isIdentity()) {
+    newEdges[0] =
+        applyNoiseEffects(originalCopy, usedQubits, firstPathEdge, nextLevel);
+    newEdges[3] =
+        applyNoiseEffects(originalCopy, usedQubits, firstPathEdge, nextLevel);
+  } else {
     for (std::size_t i = 0; i < newEdges.size(); i++) {
       auto& successor = originalCopy.p->e[i];
       if (firstPathEdge || i == 1) {
         // If I am to the firstPathEdge I cannot minimize the necessary
         // operations anymore
         dEdge::applyDmChangesToEdge(successor);
-        newEdges[i] = applyNoiseEffects(successor, usedQubits, true);
+        newEdges[i] = applyNoiseEffects(successor, usedQubits, true, nextLevel);
         dEdge::revertDmChangesToEdge(successor);
       } else if (i == 2) {
         // Since e[1] == e[2] (due to density matrix representation), I can skip
         // calculating e[2]
         newEdges[2] = newEdges[1];
       } else {
         dEdge::applyDmChangesToEdge(successor);
-        newEdges[i] = applyNoiseEffects(successor, usedQubits, false);
+        newEdges[i] =
+            applyNoiseEffects(successor, usedQubits, false, nextLevel);
         dEdge::revertDmChangesToEdge(successor);
       }
     }
-    if (std::any_of(usedQubits.begin(), usedQubits.end(),
-                    [originalEdge](const qc::Qubit qubit) {
-                      return originalEdge.p->v == qubit;
-                    })) {
-      for (auto const& type : noiseEffects) {
-        switch (type) {
-        case AmplitudeDamping:
-          applyAmplitudeDampingToEdges(
-              newEdges, (usedQubits.size() == 1) ? ampDampingProbSingleQubit
-                                                 : ampDampingProbMultiQubit);
-          break;
-        case PhaseFlip:
-          applyPhaseFlipToEdges(newEdges, (usedQubits.size() == 1)
-                                              ? noiseProbSingleQubit
-                                              : noiseProbMultiQubit);
-          break;
-        case Depolarization:
-          applyDepolarisationToEdges(newEdges, (usedQubits.size() == 1)
-                                                   ? noiseProbSingleQubit
-                                                   : noiseProbMultiQubit);
-          break;
-        case Identity:
-          continue;
-        }
+  }
+  if (std::any_of(
+          usedQubits.begin(), usedQubits.end(),
+          [&nextLevel](const qc::Qubit qubit) { return nextLevel == qubit; })) {
+    for (auto const& type : noiseEffects) {
+      switch (type) {
+      case AmplitudeDamping:
+        applyAmplitudeDampingToEdges(newEdges, (usedQubits.size() == 1)
+                                                   ? ampDampingProbSingleQubit
+                                                   : ampDampingProbMultiQubit);
+        break;
+      case PhaseFlip:
+        applyPhaseFlipToEdges(newEdges, (usedQubits.size() == 1)
+                                            ? noiseProbSingleQubit
+                                            : noiseProbMultiQubit);
+        break;
+      case Depolarization:
+        applyDepolarisationToEdges(newEdges, (usedQubits.size() == 1)
+                                                 ? noiseProbSingleQubit
+                                                 : noiseProbMultiQubit);
+        break;
+      case Identity:
+        continue;
       }
     }
+  }
 
-    auto e = package->makeDDNode(originalCopy.p->v, newEdges, firstPathEdge);
-    if (e.w.exactlyZero()) {
-      return e;
-    }
-    e.w = e.w * originalWeight;
+  auto e = package->makeDDNode(nextLevel, newEdges, firstPathEdge);
+  if (e.w.exactlyZero()) {
     return e;
   }
+  e.w = e.w * originalWeight;
+  return e;
+}
 
-  void applyPhaseFlipToEdges(ArrayOfEdges& e, double probability) {
-    const auto complexProb = 1. - 2. * probability;
+void DeterministicNoiseFunctionality::applyPhaseFlipToEdges(
+    ArrayOfEdges& e, const double probability) {
+  const auto complexProb = 1. - 2. * probability;
 
-    // e[0] = e[0]
-    // e[1] = (1-2p)*e[1]
-    if (!e[1].w.exactlyZero()) {
-      e[1].w *= complexProb;
-    }
-    // e[2] = (1-2p)*e[2]
-    if (!e[2].w.exactlyZero()) {
-      e[2].w *= complexProb;
-    }
-    // e[3] = e[3]
+  // e[0] = e[0]
+  // e[1] = (1-2p)*e[1]
+  if (!e[1].w.exactlyZero()) {
+    e[1].w *= complexProb;
   }
+  // e[2] = (1-2p)*e[2]
+  if (!e[2].w.exactlyZero()) {
+    e[2].w *= complexProb;
+  }
+  // e[3] = e[3]
+}
 
-  void applyAmplitudeDampingToEdges(ArrayOfEdges& e, double probability) {
-    // e[0] = e[0] + p*e[3]
-    if (!e[3].w.exactlyZero()) {
-      if (!e[0].w.exactlyZero()) {
-        const auto var =
-            static_cast<Qubit>(std::max({e[0].p != nullptr ? e[0].p->v : 0,
-                                         e[1].p != nullptr ? e[1].p->v : 0,
-                                         e[2].p != nullptr ? e[2].p->v : 0,
-                                         e[3].p != nullptr ? e[3].p->v : 0}));
-        e[0] = package->add2(e[0], {e[3].p, e[3].w * probability}, var);
-      } else {
-        e[0] = {e[3].p, e[3].w * probability};
-      }
-    }
-
-    // e[1] = sqrt(1-p)*e[1]
-    if (!e[1].w.exactlyZero()) {
-      e[1].w *= std::sqrt(1 - probability);
-    }
-
-    // e[2] = sqrt(1-p)*e[2]
-    if (!e[2].w.exactlyZero()) {
-      e[2].w *= std::sqrt(1 - probability);
+void DeterministicNoiseFunctionality::applyAmplitudeDampingToEdges(
+    ArrayOfEdges& e, const double probability) {
+  // e[0] = e[0] + p*e[3]
+  if (!e[3].w.exactlyZero()) {
+    if (!e[0].w.exactlyZero()) {
+      const auto var = static_cast<Qubit>(std::max(
+          {e[0].p != nullptr ? e[0].p->v : 0, e[1].p != nullptr ? e[1].p->v : 0,
+           e[2].p != nullptr ? e[2].p->v : 0,
+           e[3].p != nullptr ? e[3].p->v : 0}));
+      e[0] = package->add2(e[0], {e[3].p, e[3].w * probability}, var);
+    } else {
+      e[0] = {e[3].p, e[3].w * probability};
     }
+  }
 
-    // e[3] = (1-p)*e[3]
-    if (!e[3].w.exactlyZero()) {
-      e[3].w *= (1 - probability);
-    }
+  // e[1] = sqrt(1-p)*e[1]
+  if (!e[1].w.exactlyZero()) {
+    e[1].w *= std::sqrt(1 - probability);
   }
 
-  void applyDepolarisationToEdges(ArrayOfEdges& e, double probability) {
-    std::array<dCachedEdge, 2> helperEdge{};
+  // e[2] = sqrt(1-p)*e[2]
+  if (!e[2].w.exactlyZero()) {
+    e[2].w *= std::sqrt(1 - probability);
+  }
 
-    const auto var = static_cast<Qubit>(std::max(
-        {e[0].p != nullptr ? e[0].p->v : 0, e[1].p != nullptr ? e[1].p->v : 0,
-         e[2].p != nullptr ? e[2].p->v : 0,
-         e[3].p != nullptr ? e[3].p->v : 0}));
+  // e[3] = (1-p)*e[3]
+  if (!e[3].w.exactlyZero()) {
+    e[3].w *= (1 - probability);
+  }
+}
 
-    auto oldE0Edge = e[0];
+void DeterministicNoiseFunctionality::applyDepolarisationToEdges(
+    ArrayOfEdges& e, const double probability) {
+  std::array<dCachedEdge, 2> helperEdge{};
 
-    // e[0] = 0.5*((2-p)*e[0] + p*e[3])
-    {
-      // helperEdge[0] = 0.5*((2-p)*e[0]
-      helperEdge[0].p = e[0].p;
-      if (!e[0].w.exactlyZero()) {
-        helperEdge[0].w = e[0].w * (2 - probability) * 0.5;
-      } else {
-        helperEdge[0].w = 0;
-      }
+  const auto var = static_cast<Qubit>(std::max(
+      {e[0].p != nullptr ? e[0].p->v : 0, e[1].p != nullptr ? e[1].p->v : 0,
+       e[2].p != nullptr ? e[2].p->v : 0, e[3].p != nullptr ? e[3].p->v : 0}));
 
-      // helperEdge[1] = 0.5*p*e[3]
-      helperEdge[1].p = e[3].p;
-      if (!e[3].w.exactlyZero()) {
-        helperEdge[1].w = e[3].w * probability * 0.5;
-      } else {
-        helperEdge[1].w = 0;
-      }
+  auto oldE0Edge = e[0];
 
-      // e[0] = helperEdge[0] + helperEdge[1]
-      e[0] = package->add2(helperEdge[0], helperEdge[1], var);
+  // e[0] = 0.5*((2-p)*e[0] + p*e[3])
+  {
+    // helperEdge[0] = 0.5*((2-p)*e[0]
+    helperEdge[0].p = e[0].p;
+    if (!e[0].w.exactlyZero()) {
+      helperEdge[0].w = e[0].w * (2 - probability) * 0.5;
+    } else {
+      helperEdge[0].w = 0;
     }
 
-    // e[1]=(1-p)*e[1]
-    if (!e[1].w.exactlyZero()) {
-      e[1].w *= (1 - probability);
-    }
-    // e[2]=(1-p)*e[2]
-    if (!e[2].w.exactlyZero()) {
-      e[2].w *= (1 - probability);
+    // helperEdge[1] = 0.5*p*e[3]
+    helperEdge[1].p = e[3].p;
+    if (!e[3].w.exactlyZero()) {
+      helperEdge[1].w = e[3].w * probability * 0.5;
+    } else {
+      helperEdge[1].w = 0;
     }
 
-    // e[3] = 0.5*((2-p)*e[3]) + 0.5*(p*e[0])
-    {
-      // helperEdge[0] = 0.5*((2-p)*e[3])
-      helperEdge[0].p = e[3].p;
-      if (!e[3].w.exactlyZero()) {
-        helperEdge[0].w = e[3].w * (2 - probability) * 0.5;
-      } else {
-        helperEdge[0].w = 0;
-      }
+    // e[0] = helperEdge[0] + helperEdge[1]
+    e[0] = package->add2(helperEdge[0], helperEdge[1], var);
+  }
 
-      // helperEdge[1] = 0.5*p*e[0]
-      helperEdge[1].p = oldE0Edge.p;
-      if (!oldE0Edge.w.exactlyZero()) {
-        helperEdge[1].w = oldE0Edge.w * probability * 0.5;
-      } else {
-        helperEdge[1].w = 0;
-      }
-      e[3] = package->add2(helperEdge[0], helperEdge[1], var);
-    }
+  // e[1]=(1-p)*e[1]
+  if (!e[1].w.exactlyZero()) {
+    e[1].w *= (1 - probability);
+  }
+  // e[2]=(1-p)*e[2]
+  if (!e[2].w.exactlyZero()) {
+    e[2].w *= (1 - probability);
   }
-};
 
+  // e[3] = 0.5*((2-p)*e[3]) + 0.5*(p*e[0])
+  {
+    // helperEdge[0] = 0.5*((2-p)*e[3])
+    helperEdge[0].p = e[3].p;
+    if (!e[3].w.exactlyZero()) {
+      helperEdge[0].w = e[3].w * (2 - probability) * 0.5;
+    } else {
+      helperEdge[0].w = 0;
+    }
+
+    // helperEdge[1] = 0.5*p*e[0]
+    helperEdge[1].p = oldE0Edge.p;
+    if (!oldE0Edge.w.exactlyZero()) {
+      helperEdge[1].w = oldE0Edge.w * probability * 0.5;
+    } else {
+      helperEdge[1].w = 0;
+    }
+    e[3] = package->add2(helperEdge[0], helperEdge[1], var);
+  }
+}
+
+void sanityCheckOfNoiseProbabilities(const double noiseProbability,
+                                     const double amplitudeDampingProb,
+                                     const double multiQubitGateFactor) {
+  if (noiseProbability < 0 || amplitudeDampingProb < 0 ||
+      noiseProbability * multiQubitGateFactor > 1 ||
+      amplitudeDampingProb * multiQubitGateFactor > 1) {
+    throw std::runtime_error(
+        "Error probabilities are faulty!"
+        "\n single qubit error probability: " +
+        std::to_string(noiseProbability) + " multi qubit error probability: " +
+        std::to_string(noiseProbability * multiQubitGateFactor) +
+        "\n single qubit amplitude damping  probability: " +
+        std::to_string(amplitudeDampingProb) +
+        " multi qubit amplitude damping  probability: " +
+        std::to_string(amplitudeDampingProb * multiQubitGateFactor));
+  }
+}
 } // namespace dd
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Operations.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Operations.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 qc::MatrixDD
 getStandardOperationDD(const qc::StandardOperation* op, Package<Config>& dd,
                        const qc::Controls& controls, const qc::Qubit target,
                        const bool inverse) {
   GateMatrix gm;
 
   const auto type = op->getType();
-  const auto nqubits = op->getNqubits();
-  const auto startQubit = op->getStartingQubit();
   const auto& parameter = op->getParameter();
 
   switch (type) {
   case qc::I:
     gm = I_MAT;
     break;
   case qc::H:
@@ -84,26 +82,24 @@
     gm = inverse ? rzMat(-parameter[0U]) : rzMat(parameter[0U]);
     break;
   default:
     std::ostringstream oss{};
     oss << "DD for gate" << op->getName() << " not available!";
     throw qc::QFRException(oss.str());
   }
-  return dd.makeGateDD(gm, nqubits, controls, target, startQubit);
+  return dd.makeGateDD(gm, controls, target);
 }
 
 // two-target Operations
 template <class Config>
 qc::MatrixDD
 getStandardOperationDD(const qc::StandardOperation* op, Package<Config>& dd,
                        const qc::Controls& controls, qc::Qubit target0,
                        qc::Qubit target1, const bool inverse) {
   const auto type = op->getType();
-  const auto nqubits = op->getNqubits();
-  const auto startQubit = op->getStartingQubit();
   const auto& parameter = op->getParameter();
 
   if (type == qc::DCX && inverse) {
     // DCX is not self-inverse, but the inverse is just swapping the targets
     std::swap(target0, target1);
   }
 
@@ -152,64 +148,49 @@
     break;
   default:
     std::ostringstream oss{};
     oss << "DD for gate " << op->getName() << " not available!";
     throw qc::QFRException(oss.str());
   }
 
-  return dd.makeTwoQubitGateDD(gm, nqubits, controls, target0, target1,
-                               startQubit);
+  return dd.makeTwoQubitGateDD(gm, controls, target0, target1);
 }
 
 // The methods with a permutation parameter apply these Operations according to
 // the mapping specified by the permutation, e.g.
 //      if perm[0] = 1 and perm[1] = 0
 //      then cx 0 1 will be translated to cx perm[0] perm[1] == cx 1 0
 
 template <class Config>
 qc::MatrixDD getDD(const qc::Operation* op, Package<Config>& dd,
                    qc::Permutation& permutation, const bool inverse = false) {
   const auto type = op->getType();
-  const auto nqubits = op->getNqubits();
-
-  // check whether the operation can be handled by the underlying DD package
-  if (nqubits > Package<Config>::MAX_POSSIBLE_QUBITS) {
-    throw qc::QFRException(
-        "Requested too many qubits to be handled by the DD package. Qubit "
-        "datatype only allows up to " +
-        std::to_string(Package<Config>::MAX_POSSIBLE_QUBITS) +
-        " qubits, while " + std::to_string(nqubits) +
-        " were requested. If you want to use more than " +
-        std::to_string(Package<Config>::MAX_POSSIBLE_QUBITS) +
-        " qubits, you have to recompile the package with a wider Qubit type in "
-        "`include/dd/DDDefinitions.hpp!`");
-  }
 
   // if a permutation is provided and the current operation is a SWAP, this
   // routine just updates the permutation
   if (!permutation.empty() && type == qc::SWAP && !op->isControlled()) {
     const auto& targets = op->getTargets();
 
     const auto target0 = targets[0U];
     const auto target1 = targets[1U];
     // update permutation
     std::swap(permutation.at(target0), permutation.at(target1));
-    return dd.makeIdent(nqubits);
+    return dd.makeIdent();
   }
 
   if (type == qc::Barrier) {
-    return dd.makeIdent(nqubits);
+    return dd.makeIdent();
   }
 
   if (type == qc::GPhase) {
     auto phase = op->getParameter()[0U];
     if (inverse) {
       phase = -phase;
     }
-    auto id = dd.makeIdent(nqubits);
+    auto id = dd.makeIdent();
     id.w = dd.cn.lookup(std::cos(phase), std::sin(phase));
     return id;
   }
 
   if (const auto* standardOp = dynamic_cast<const qc::StandardOperation*>(op)) {
     auto targets = op->getTargets();
     auto controls = op->getControls();
@@ -225,15 +206,15 @@
     }
     assert(targets.size() == 1);
     return getStandardOperationDD(standardOp, dd, controls, targets[0U],
                                   inverse);
   }
 
   if (const auto* compoundOp = dynamic_cast<const qc::CompoundOperation*>(op)) {
-    auto e = dd.makeIdent(op->getNqubits());
+    auto e = dd.makeIdent();
     if (inverse) {
       for (const auto& operation : *compoundOp) {
         e = dd.multiply(e, getInverseDD(operation.get(), dd, permutation));
       }
     } else {
       for (const auto& operation : *compoundOp) {
         e = dd.multiply(getDD(operation.get(), dd, permutation), e);
@@ -277,18 +258,17 @@
 // apply swaps 'on' DD in order to change 'from' to 'to'
 // where |from| >= |to|
 template <class DDType, class Config>
 void changePermutation(DDType& on, qc::Permutation& from,
                        const qc::Permutation& to, Package<Config>& dd,
                        const bool regular = true) {
   assert(from.size() >= to.size());
-  if (on.isTerminal()) {
+  if (on.isZeroTerminal()) {
     return;
   }
-  assert(on.p != nullptr);
 
   // iterate over (k,v) pairs of second permutation
   for (const auto& [i, goal] : to) {
     // search for key in the first map
     auto it = from.find(i);
     if (it == from.end()) {
       throw qc::QFRException(
@@ -309,16 +289,15 @@
         j = key;
         break;
       }
     }
 
     // swap i and j
     auto saved = on;
-    const auto swapDD =
-        dd.makeTwoQubitGateDD(SWAP_MAT, on.p->v + 1U, from.at(i), from.at(j));
+    const auto swapDD = dd.makeTwoQubitGateDD(SWAP_MAT, from.at(i), from.at(j));
     if constexpr (std::is_same_v<DDType, qc::VectorDD>) {
       on = dd.multiply(swapDD, on);
     } else {
       // the regular flag only has an effect on matrix DDs
       if (regular) {
         on = dd.multiply(swapDD, on);
       } else {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Package.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Package.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -80,15 +80,14 @@
                                   "package with a wider Qubit type!");
     }
     nqubits = nq;
     vUniqueTable.resize(nqubits);
     mUniqueTable.resize(nqubits);
     dUniqueTable.resize(nqubits);
     stochasticNoiseOperationCache.resize(nqubits);
-    idTable.resize(nqubits);
   }
 
   // reset package state
   void reset() {
     clearUniqueTables();
     resetMemoryManagers();
     clearComputeTables();
@@ -261,15 +260,14 @@
     // been collected
     if (mCollect > 0 || dCollect > 0) {
       matrixAdd.clear();
       conjugateMatrixTranspose.clear();
       matrixKronecker.clear();
       matrixVectorMultiplication.clear();
       matrixMatrixMultiplication.clear();
-      clearIdentityTable();
       stochasticNoiseOperationCache.clear();
       densityAdd.clear();
       densityDensityMultiplication.clear();
       densityNoise.clear();
     }
     // invalidate all compute tables where any component of the entry contains
     // numbers from the complex table if any complex numbers were collected
@@ -510,201 +508,165 @@
     return {matrixDD.p, cn.lookup(matrixDD.w)};
   }
 
   ///
   /// Matrix nodes, edges and quantum gates
   ///
   // build matrix representation for a single gate on an n-qubit circuit
-  mEdge makeGateDD(const GateMatrix& mat, const std::size_t n,
-                   const qc::Qubit target, const std::size_t start = 0) {
-    return makeGateDD(mat, n, qc::Controls{}, target, start);
-  }
-  mEdge makeGateDD(const GateMatrix& mat, const std::size_t n,
-                   const qc::Control& control, const qc::Qubit target,
-                   const std::size_t start = 0) {
-    return makeGateDD(mat, n, qc::Controls{control}, target, start);
-  }
-  mEdge makeGateDD(const GateMatrix& mat, const std::size_t n,
-                   const qc::Controls& controls, const qc::Qubit target,
-                   const std::size_t start = 0) {
-    if (n + start > nqubits) {
+  mEdge makeGateDD(const GateMatrix& mat, const qc::Qubit target) {
+    return makeGateDD(mat, qc::Controls{}, target);
+  }
+  mEdge makeGateDD(const GateMatrix& mat, const qc::Control& control,
+                   const qc::Qubit target) {
+    return makeGateDD(mat, qc::Controls{control}, target);
+  }
+  mEdge makeGateDD(const GateMatrix& mat, const qc::Controls& controls,
+                   const qc::Qubit target) {
+    if (std::any_of(controls.begin(), controls.end(),
+                    [this](const auto& c) {
+                      return c.qubit > static_cast<Qubit>(nqubits - 1U);
+                    }) ||
+        target > static_cast<Qubit>(nqubits - 1U)) {
       throw std::runtime_error{
-          "Requested gate with " + std::to_string(n + start) +
-          " qubits, but current package configuration only supports up to " +
+          "Requested gate acting on qubit(s) with index larger than " +
+          std::to_string(nqubits - 1U) +
+          " while the package configuration only supports up to " +
           std::to_string(nqubits) +
           " qubits. Please allocate a larger package instance."};
     }
-    std::array<mEdge, NEDGE> em{};
-    auto it = controls.begin();
+    std::array<mCachedEdge, NEDGE> em{};
     for (auto i = 0U; i < NEDGE; ++i) {
-      em[i] = mEdge::terminal(cn.lookup(mat[i]));
+      em[i] = mCachedEdge::terminal(mat[i]);
+    }
+
+    if (controls.empty()) {
+      // Single qubit operation
+      const auto e = makeDDNode(static_cast<Qubit>(target), em);
+      return {e.p, cn.lookup(e.w)};
     }
 
+    auto it = controls.begin();
+    auto edges = std::array{mCachedEdge::zero(), mCachedEdge::zero(),
+                            mCachedEdge::zero(), mCachedEdge::zero()};
+
     // process lines below target
-    auto z = static_cast<Qubit>(start);
-    for (; z < static_cast<Qubit>(target); ++z) {
+    for (; it != controls.end() && it->qubit < target; ++it) {
       for (auto i1 = 0U; i1 < RADIX; ++i1) {
         for (auto i2 = 0U; i2 < RADIX; ++i2) {
           auto i = i1 * RADIX + i2;
-          if (it != controls.end() && it->qubit == z) {
-            auto edges = std::array{mEdge::zero(), mEdge::zero(), mEdge::zero(),
-                                    mEdge::zero()};
-            if (it->type == qc::Control::Type::Neg) { // neg. control
-              edges[0] = em[i];
-              if (i1 == i2) {
-                if (z == 0U) {
-                  edges[3] = mEdge::one();
-                } else {
-                  edges[3] = makeIdent(start, z - 1U);
-                }
-              }
-            } else { // pos. control
-              edges[3] = em[i];
-              if (i1 == i2) {
-                if (z == 0U) {
-                  edges[0] = mEdge::one();
-                } else {
-                  edges[0] = makeIdent(start, z - 1U);
-                }
-              }
-            }
-            em[i] = makeDDNode(z, edges);
-          } else { // not connected
-            em[i] = makeDDNode(
-                z, std::array{em[i], mEdge::zero(), mEdge::zero(), em[i]});
+          if (it->type == qc::Control::Type::Neg) { // neg. control
+            edges[0] = em[i];
+            edges[3] = (i1 == i2) ? mCachedEdge::one() : mCachedEdge::zero();
+          } else { // pos. control
+            edges[0] = (i1 == i2) ? mCachedEdge::one() : mCachedEdge::zero();
+            edges[3] = em[i];
           }
+          em[i] = makeDDNode(static_cast<Qubit>(it->qubit), edges);
         }
       }
-      if (it != controls.end() && it->qubit == z) {
-        ++it;
-      }
     }
 
     // target line
-    auto e = makeDDNode(z, em);
+    auto e = makeDDNode(static_cast<Qubit>(target), em);
 
     // process lines above target
-    for (; z < static_cast<Qubit>(n - 1 + start); z++) {
-      auto q = static_cast<Qubit>(z + 1);
-      if (it != controls.end() && it->qubit == static_cast<qc::Qubit>(q)) {
-        if (it->type == qc::Control::Type::Neg) { // neg. control
-          e = makeDDNode(q, std::array{e, mEdge::zero(), mEdge::zero(),
-                                       makeIdent(start, q - 1U)});
-        } else { // pos. control
-          e = makeDDNode(q, std::array{makeIdent(start, q - 1U), mEdge::zero(),
-                                       mEdge::zero(), e});
-        }
-        ++it;
-      } else { // not connected
-        e = makeDDNode(q, std::array{e, mEdge::zero(), mEdge::zero(), e});
+    for (; it != controls.end(); ++it) {
+      if (it->type == qc::Control::Type::Neg) { // neg. control
+        edges[0] = e;
+        edges[3] = mCachedEdge::one();
+        e = makeDDNode(static_cast<Qubit>(it->qubit), edges);
+      } else { // pos. control
+        edges[0] = mCachedEdge::one();
+        edges[3] = e;
+        e = makeDDNode(static_cast<Qubit>(it->qubit), edges);
       }
     }
-    return e;
+    return {e.p, cn.lookup(e.w)};
   }
 
   /**
   Creates the DD for a two-qubit gate
   @param mat Matrix representation of the gate
-  @param n Number of qubits in the circuit
   @param target0 First target qubit
   @param target1 Second target qubit
-  @param start Start index for the DD
   @return DD representing the gate
   @throws std::runtime_error if the number of qubits is larger than the package
   configuration
   **/
-  mEdge makeTwoQubitGateDD(const TwoQubitGateMatrix& mat, const std::size_t n,
-                           const qc::Qubit target0, const qc::Qubit target1,
-                           const std::size_t start = 0) {
-    return makeTwoQubitGateDD(mat, n, qc::Controls{}, target0, target1, start);
+  mEdge makeTwoQubitGateDD(const TwoQubitGateMatrix& mat,
+                           const qc::Qubit target0, const qc::Qubit target1) {
+    return makeTwoQubitGateDD(mat, qc::Controls{}, target0, target1);
   }
 
   /**
   Creates the DD for a two-qubit gate
   @param mat Matrix representation of the gate
-  @param n Number of qubits in the circuit
   @param controls Control qubits of the two-qubit gate
   @param target0 First target qubit
   @param target1 Second target qubit
-  @param start Start index for the DD
   @return DD representing the gate
   @throws std::runtime_error if the number of qubits is larger than the package
   configuration
   **/
-  mEdge makeTwoQubitGateDD(const TwoQubitGateMatrix& mat, const std::size_t n,
+  mEdge makeTwoQubitGateDD(const TwoQubitGateMatrix& mat,
                            const qc::Controls& controls,
-                           const qc::Qubit target0, const qc::Qubit target1,
-                           const std::size_t start = 0) {
+                           const qc::Qubit target0, const qc::Qubit target1) {
     // sanity check
-    if (n + start > nqubits) {
+    if (std::any_of(controls.begin(), controls.end(),
+                    [this](const auto& c) {
+                      return c.qubit > static_cast<Qubit>(nqubits - 1U);
+                    }) ||
+        target0 > static_cast<Qubit>(nqubits - 1U) ||
+        target1 > static_cast<Qubit>(nqubits - 1U)) {
       throw std::runtime_error{
-          "Requested gate with " + std::to_string(n + start) +
-          " qubits, but current package configuration only supports up to " +
+          "Requested gate acting on qubit(s) with index larger than " +
+          std::to_string(nqubits - 1U) +
+          " while the package configuration only supports up to " +
           std::to_string(nqubits) +
           " qubits. Please allocate a larger package instance."};
     }
 
     // create terminal edge matrix
-    std::array<std::array<mEdge, NEDGE>, NEDGE> em{};
+    std::array<std::array<mCachedEdge, NEDGE>, NEDGE> em{};
     for (auto i1 = 0U; i1 < NEDGE; i1++) {
       const auto& matRow = mat.at(i1);
       auto& emRow = em.at(i1);
       for (auto i2 = 0U; i2 < NEDGE; i2++) {
-        emRow.at(i2) = mEdge::terminal(cn.lookup(matRow.at(i2)));
+        emRow.at(i2) = mCachedEdge::terminal(matRow.at(i2));
       }
     }
 
     // process lines below smaller target
     auto it = controls.begin();
-    auto z = static_cast<Qubit>(start);
     const auto smallerTarget = std::min(target0, target1);
-    for (; z < smallerTarget; ++z) {
+
+    auto edges = std::array{mCachedEdge::zero(), mCachedEdge::zero(),
+                            mCachedEdge::zero(), mCachedEdge::zero()};
+
+    for (; it != controls.end() && it->qubit < smallerTarget; ++it) {
       for (auto row = 0U; row < NEDGE; ++row) {
         for (auto col = 0U; col < NEDGE; ++col) {
-          if (it != controls.end() && it->qubit == z) {
-            auto edges = std::array{mEdge::zero(), mEdge::zero(), mEdge::zero(),
-                                    mEdge::zero()};
-            if (it->type == qc::Control::Type::Neg) { // negative control
-              edges[0] = em[row][col];
-              if (row == col) {
-                if (z == 0U) {
-                  edges[3] = mEdge::one();
-                } else {
-                  edges[3] = makeIdent(start, z - 1U);
-                }
-              }
-            } else { // positive control
-              edges[3] = em[row][col];
-              if (row == col) {
-                if (z == 0U) {
-                  edges[0] = mEdge::one();
-                } else {
-                  edges[0] = makeIdent(start, z - 1U);
-                }
-              }
-            }
-            em[row][col] = makeDDNode(z, edges);
-          } else { // not connected
-            em[row][col] =
-                makeDDNode(z, std::array{em[row][col], mEdge::zero(),
-                                         mEdge::zero(), em[row][col]});
+          if (it->type == qc::Control::Type::Neg) { // negative control
+            edges[0] = em[row][col];
+            edges[3] = (row == col) ? mCachedEdge::one() : mCachedEdge::zero();
+          } else { // positive control
+            edges[0] = (row == col) ? mCachedEdge::one() : mCachedEdge::zero();
+            edges[3] = em[row][col];
           }
+          em[row][col] = makeDDNode(static_cast<Qubit>(it->qubit), edges);
         }
       }
-      if (it != controls.end() && it->qubit == z) {
-        it++;
-      }
     }
 
     // process the smaller target by taking the 16 submatrices and appropriately
     // combining them into four DDs.
-    std::array<mEdge, NEDGE> em0{};
+    std::array<mCachedEdge, NEDGE> em0{};
     for (std::size_t row = 0; row < RADIX; ++row) {
       for (std::size_t col = 0; col < RADIX; ++col) {
-        std::array<mEdge, NEDGE> local{};
+        std::array<mCachedEdge, NEDGE> local{};
         if (target0 > target1) {
           for (std::size_t i = 0; i < RADIX; ++i) {
             for (std::size_t j = 0; j < RADIX; ++j) {
               local.at(i * RADIX + j) =
                   em.at(row * RADIX + i).at(col * RADIX + j);
             }
           }
@@ -712,91 +674,56 @@
           for (std::size_t i = 0; i < RADIX; ++i) {
             for (std::size_t j = 0; j < RADIX; ++j) {
               local.at(i * RADIX + j) =
                   em.at(i * RADIX + row).at(j * RADIX + col);
             }
           }
         }
-        em0.at(row * RADIX + col) = makeDDNode(z, local);
+        em0.at(row * RADIX + col) =
+            makeDDNode(static_cast<Qubit>(smallerTarget), local);
       }
     }
 
     // process lines between the two targets
-    for (++z; z < std::max(target0, target1); ++z) {
+    const auto largerTarget = std::max(target0, target1);
+    for (; it != controls.end() && it->qubit < largerTarget; ++it) {
       for (auto i = 0U; i < NEDGE; ++i) {
-        if (it != controls.end() && it->qubit == z) {
-          auto edges = std::array{mEdge::zero(), mEdge::zero(), mEdge::zero(),
-                                  mEdge::zero()};
-          if (it->type == qc::Control::Type::Neg) { // negative control
-            edges[0] = em0[i];
-            if (i == 0 || i == NEDGE - 1) {
-              edges[3] = makeIdent(start, z - 1U);
-            }
-          } else { // positive control
-            edges[3] = em0[i];
-            if (i == 0 || i == NEDGE - 1) {
-              edges[0] = makeIdent(start, z - 1U);
-            }
-          }
-          em0[i] = makeDDNode(z, edges);
-        } else { // not connected
-          em0[i] = makeDDNode(
-              z, std::array{em0[i], mEdge::zero(), mEdge::zero(), em0[i]});
+        if (it->type == qc::Control::Type::Neg) { // negative control
+          edges[0] = em0[i];
+          edges[3] =
+              (i == 0 || i == 3) ? mCachedEdge::one() : mCachedEdge::zero();
+        } else { // positive control
+          edges[0] =
+              (i == 0 || i == 3) ? mCachedEdge::one() : mCachedEdge::zero();
+          edges[3] = em0[i];
         }
-      }
-      if (it != controls.end() && it->qubit == z) {
-        ++it;
+        em0[i] = makeDDNode(static_cast<Qubit>(it->qubit), edges);
       }
     }
 
     // process the larger target by combining the four DDs from the smaller
     // target
-    auto e = makeDDNode(z, em0);
+    auto e = makeDDNode(static_cast<Qubit>(largerTarget), em0);
 
     // process lines above the larger target
-    const auto end = static_cast<Qubit>(n + start);
-    for (++z; z < end; ++z) {
-      if (it != controls.end() && it->qubit == z) {
-        if (it->type == qc::Control::Type::Neg) { // negative control
-          e = makeDDNode(z, std::array{e, mEdge::zero(), mEdge::zero(),
-                                       makeIdent(start, z - 1U)});
-        } else { // positive control
-          e = makeDDNode(z, std::array{makeIdent(start, z - 1U), mEdge::zero(),
-                                       mEdge::zero(), e});
-        }
-        ++it;
-      } else { // not connected (current qubit is not a control/target qubit)
-        e = makeDDNode(z, std::array{e, mEdge::zero(), mEdge::zero(), e});
+    for (; it != controls.end(); ++it) {
+      if (it->type == qc::Control::Type::Neg) { // negative control
+        edges[0] = e;
+        edges[3] = mCachedEdge::one();
+      } else { // positive control
+        edges[0] = mCachedEdge::one();
+        edges[3] = e;
       }
+      e = makeDDNode(static_cast<Qubit>(it->qubit), edges);
     }
 
-    return e;
+    return {e.p, cn.lookup(e.w)};
   }
 
 private:
-  // check whether node represents a symmetric matrix or the identity
-  void checkSpecialMatrices(mNode* p) {
-    if (mNode::isTerminal(p)) {
-      return;
-    }
-
-    // check if matrix resembles identity
-    p->setIdentity(false);
-    const auto& e0 = p->e[0];
-    const auto& e1 = p->e[1];
-    const auto& e2 = p->e[2];
-    const auto& e3 = p->e[3];
-    if (!mNode::isIdentity(e0.p) || !e1.w.exactlyZero() ||
-        !e2.w.exactlyZero() || !e0.w.exactlyOne() || !e3.w.exactlyOne() ||
-        !mNode::isIdentity(e3.p)) {
-      return;
-    }
-    p->setIdentity(true);
-  }
-
   vCachedEdge makeStateFromVector(const CVec::const_iterator& begin,
                                   const CVec::const_iterator& end,
                                   const Qubit level) {
     if (level == 0U) {
       assert(std::distance(begin, end) == 2);
       const auto zeroSuccessor = vCachedEdge::terminal(*begin);
       const auto oneSuccessor = vCachedEdge::terminal(*(begin + 1));
@@ -876,25 +803,32 @@
       p->flags = 0;
       if constexpr (std::is_same_v<Node, dNode>) {
         p->setDensityMatrixNodeFlag(generateDensityMatrix);
       }
     }
 
     auto e = EdgeType<Node>::normalize(p, edges, memoryManager, cn);
+    if constexpr (std::is_same_v<Node, mNode> || std::is_same_v<Node, dNode>) {
+      if (!e.isTerminal()) {
+        const auto& es = e.p->e;
+        // Check if node resembles the identity. If so, skip it.
+        if ((es[0].p == es[3].p) &&
+            (es[0].w.exactlyOne() && es[1].w.exactlyZero() &&
+             es[2].w.exactlyZero() && es[3].w.exactlyOne())) {
+          auto* ptr = es[0].p;
+          memoryManager.returnEntry(e.p);
+          return EdgeType<Node>{ptr, e.w};
+        }
+      }
+    }
 
     // look it up in the unique tables
     auto& uniqueTable = getUniqueTable<Node>();
     auto* l = uniqueTable.lookup(e.p);
 
-    // set specific node properties for matrices
-    if constexpr (std::is_same_v<Node, mNode>) {
-      if (l == e.p) {
-        checkSpecialMatrices(l);
-      }
-    }
     return EdgeType<Node>{l, e.w};
   }
 
   template <class Node>
   Edge<Node> deleteEdge(const Edge<Node>& e, const Qubit v,
                         const std::size_t edgeIdx) {
     std::unordered_map<Node*, Edge<Node>> nodes{};
@@ -940,23 +874,24 @@
   ///
   /// Compute table definitions
   ///
 public:
   void clearComputeTables() {
     vectorAdd.clear();
     matrixAdd.clear();
+    vectorAddMagnitudes.clear();
+    matrixAddMagnitudes.clear();
+    conjugateVector.clear();
     conjugateMatrixTranspose.clear();
     matrixMatrixMultiplication.clear();
     matrixVectorMultiplication.clear();
     vectorInnerProduct.clear();
     vectorKronecker.clear();
     matrixKronecker.clear();
 
-    clearIdentityTable();
-
     stochasticNoiseOperationCache.clear();
     densityAdd.clear();
     densityDensityMultiplication.clear();
     densityNoise.clear();
   }
 
   ///
@@ -1167,29 +1102,29 @@
 
   char measureOneCollapsing(dEdge& e, const Qubit index, std::mt19937_64& mt) {
     char measuredResult = '0';
     dEdge::alignDensityEdge(e);
     const auto nrQubits = e.p->v + 1U;
     dEdge::setDensityMatrixTrue(e);
 
-    auto const measZeroDd = makeGateDD(MEAS_ZERO_MAT, nrQubits, index);
+    auto const measZeroDd = makeGateDD(MEAS_ZERO_MAT, index);
 
     auto tmp0 = conjugateTranspose(measZeroDd);
-    auto tmp1 = multiply(e, densityFromMatrixEdge(tmp0), 0, false);
-    auto tmp2 = multiply(densityFromMatrixEdge(measZeroDd), tmp1, 0, true);
-    auto densityMatrixTrace = trace(tmp2);
+    auto tmp1 = multiply(e, densityFromMatrixEdge(tmp0), false);
+    auto tmp2 = multiply(densityFromMatrixEdge(measZeroDd), tmp1, true);
+    auto densityMatrixTrace = trace(tmp2, nrQubits);
 
     std::uniform_real_distribution<fp> dist(0., 1.);
     if (const auto threshold = dist(mt); threshold > densityMatrixTrace.r) {
-      auto const measOneDd = makeGateDD(MEAS_ONE_MAT, nrQubits, index);
+      auto const measOneDd = makeGateDD(MEAS_ONE_MAT, index);
       tmp0 = conjugateTranspose(measOneDd);
-      tmp1 = multiply(e, densityFromMatrixEdge(tmp0), 0, false);
-      tmp2 = multiply(densityFromMatrixEdge(measOneDd), tmp1, 0, true);
+      tmp1 = multiply(e, densityFromMatrixEdge(tmp0), false);
+      tmp2 = multiply(densityFromMatrixEdge(measOneDd), tmp1, true);
       measuredResult = '1';
-      densityMatrixTrace = trace(tmp2);
+      densityMatrixTrace = trace(tmp2, nrQubits);
     }
 
     incRef(tmp2);
     dEdge::alignDensityEdge(e);
     decRef(e);
     e = tmp2;
     dEdge::setDensityMatrixTrue(e);
@@ -1213,16 +1148,15 @@
    * measured)
    */
   void performCollapsingMeasurement(vEdge& rootEdge, const Qubit index,
                                     const fp probability,
                                     const bool measureZero) {
     GateMatrix measurementMatrix = measureZero ? MEAS_ZERO_MAT : MEAS_ONE_MAT;
 
-    const auto measurementGate =
-        makeGateDD(measurementMatrix, rootEdge.p->v + 1U, index);
+    const auto measurementGate = makeGateDD(measurementMatrix, index);
 
     vEdge e = multiply(measurementGate, rootEdge);
 
     assert(probability > 0.);
     e.w = cn.lookup(e.w / std::sqrt(probability));
     incRef(e);
     decRef(rootEdge);
@@ -1247,14 +1181,29 @@
     } else if constexpr (std::is_same_v<Node, mNode>) {
       return matrixAdd;
     } else if constexpr (std::is_same_v<Node, dNode>) {
       return densityAdd;
     }
   }
 
+  ComputeTable<vCachedEdge, vCachedEdge, vCachedEdge,
+               Config::CT_VEC_ADD_MAG_NBUCKET>
+      vectorAddMagnitudes{};
+  ComputeTable<mCachedEdge, mCachedEdge, mCachedEdge,
+               Config::CT_MAT_ADD_MAG_NBUCKET>
+      matrixAddMagnitudes{};
+
+  template <class Node> [[nodiscard]] auto& getAddMagnitudesComputeTable() {
+    if constexpr (std::is_same_v<Node, vNode>) {
+      return vectorAddMagnitudes;
+    } else if constexpr (std::is_same_v<Node, mNode>) {
+      return matrixAddMagnitudes;
+    }
+  }
+
   template <class Node>
   Edge<Node> add(const Edge<Node>& x, const Edge<Node>& y) {
     Qubit var{};
     if (!x.isTerminal()) {
       var = x.p->v;
     }
     if (!y.isTerminal() && (y.p->v) > var) {
@@ -1287,38 +1236,60 @@
       return *r;
     }
 
     constexpr std::size_t n = std::tuple_size_v<decltype(x.p->e)>;
     std::array<CachedEdge<Node>, n> edge{};
     for (std::size_t i = 0U; i < n; i++) {
       CachedEdge<Node> e1{};
-      if (!Node::isTerminal(x.p)) {
+      if constexpr (std::is_same_v<Node, mNode> ||
+                    std::is_same_v<Node, dNode>) {
+        if (x.isIdentity() || x.p->v < var) {
+          // [ 0 | 1 ]   [ x | 0 ]
+          // --------- = ---------
+          // [ 2 | 3 ]   [ 0 | x ]
+          if (i == 0 || i == 3) {
+            e1 = x;
+          }
+        } else {
+          auto& xSuccessor = x.p->e[i];
+          e1 = {xSuccessor.p, 0};
+          if (!xSuccessor.w.exactlyZero()) {
+            e1.w = x.w * xSuccessor.w;
+          }
+        }
+      } else {
         auto& xSuccessor = x.p->e[i];
         e1 = {xSuccessor.p, 0};
         if (!xSuccessor.w.exactlyZero()) {
           e1.w = x.w * xSuccessor.w;
         }
-      } else {
-        e1 = x;
-        if (y.p->e[i].isTerminal()) {
-          e1 = CachedEdge<Node>::zero();
-        }
       }
       CachedEdge<Node> e2{};
-      if (!Node::isTerminal(y.p)) {
+      if constexpr (std::is_same_v<Node, mNode> ||
+                    std::is_same_v<Node, dNode>) {
+        if (y.isIdentity() || y.p->v < var) {
+          // [ 0 | 1 ]   [ y | 0 ]
+          // --------- = ---------
+          // [ 2 | 3 ]   [ 0 | y ]
+          if (i == 0 || i == 3) {
+            e2 = y;
+          }
+        } else {
+          auto& ySuccessor = y.p->e[i];
+          e2 = {ySuccessor.p, 0};
+          if (!ySuccessor.w.exactlyZero()) {
+            e2.w = y.w * ySuccessor.w;
+          }
+        }
+      } else {
         auto& ySuccessor = y.p->e[i];
         e2 = {ySuccessor.p, 0};
         if (!ySuccessor.w.exactlyZero()) {
           e2.w = y.w * ySuccessor.w;
         }
-      } else {
-        e2 = y;
-        if (x.p->e[i].isTerminal()) {
-          e2 = CachedEdge<Node>::zero();
-        }
       }
 
       if constexpr (std::is_same_v<Node, dNode>) {
         dNode::applyDmChangesToNode(e1.p);
         dNode::applyDmChangesToNode(e2.p);
         edge[i] = add2(e1, e2, var - 1);
         dNode::revertDmChangesToNode(e2.p);
@@ -1328,46 +1299,167 @@
       }
     }
     auto r = makeDDNode(var, edge);
     computeTable.insert(x, y, r);
     return r;
   }
 
+  /**
+   For two vectors (or matrices) x and y it returns a result r such that for
+   each index i: r[i] = sqrt(|x[i]|^2 + |y[i]|^2)
+   @param x DD representation of the first operand
+   @param y DD representation of the first operand
+   @param var number of qubits in the DD
+   @return DD representing the result
+   **/
+  template <class Node>
+  CachedEdge<Node> addMagnitudes(const CachedEdge<Node>& x,
+                                 const CachedEdge<Node>& y, const Qubit var) {
+    if (x.w.exactlyZero()) {
+      if (y.w.exactlyZero()) {
+        return CachedEdge<Node>::zero();
+      }
+      const auto rWeight = y.w.mag();
+      return {y.p, rWeight};
+    }
+    if (y.w.exactlyZero()) {
+      const auto rWeight = x.w.mag();
+      return {x.p, rWeight};
+    }
+    if (x.p == y.p) {
+      const auto rWeight = std::sqrt(x.w.mag2() + y.w.mag2());
+      return {x.p, rWeight};
+    }
+
+    auto& computeTable = getAddMagnitudesComputeTable<Node>();
+    if (const auto* r = computeTable.lookup(x, y); r != nullptr) {
+      return *r;
+    }
+
+    constexpr std::size_t n = std::tuple_size_v<decltype(x.p->e)>;
+    std::array<CachedEdge<Node>, n> edge{};
+    for (std::size_t i = 0U; i < n; i++) {
+      CachedEdge<Node> e1{};
+      if constexpr (std::is_same_v<Node, mNode> ||
+                    std::is_same_v<Node, dNode>) {
+        if (x.isIdentity() || x.p->v < var) {
+          if (i == 0 || i == 3) {
+            e1 = x;
+          }
+        } else {
+          auto& xSuccessor = x.p->e[i];
+          e1 = {xSuccessor.p, 0};
+          if (!xSuccessor.w.exactlyZero()) {
+            e1.w = x.w * xSuccessor.w;
+          }
+        }
+      } else {
+        auto& xSuccessor = x.p->e[i];
+        e1 = {xSuccessor.p, 0};
+        if (!xSuccessor.w.exactlyZero()) {
+          e1.w = x.w * xSuccessor.w;
+        }
+      }
+      CachedEdge<Node> e2{};
+      if constexpr (std::is_same_v<Node, mNode> ||
+                    std::is_same_v<Node, dNode>) {
+        if (y.isIdentity() || y.p->v < var) {
+          if (i == 0 || i == 3) {
+            e2 = y;
+          }
+        } else {
+          auto& ySuccessor = y.p->e[i];
+          e2 = {ySuccessor.p, 0};
+          if (!ySuccessor.w.exactlyZero()) {
+            e2.w = y.w * ySuccessor.w;
+          }
+        }
+      } else {
+        auto& ySuccessor = y.p->e[i];
+        e2 = {ySuccessor.p, 0};
+        if (!ySuccessor.w.exactlyZero()) {
+          e2.w = y.w * ySuccessor.w;
+        }
+      }
+      edge[i] = addMagnitudes(e1, e2, var - 1);
+    }
+    auto r = makeDDNode(var, edge);
+    computeTable.insert(x, y, r);
+    return r;
+  }
+
+  ///
+  /// Vector conjugation
+  ///
+  UnaryComputeTable<vNode*, vCachedEdge, Config::CT_VEC_CONJ_NBUCKET>
+      conjugateVector{};
+
+  vEdge conjugate(const vEdge& a) {
+    auto r = conjugateRec(a);
+    return {r.p, cn.lookup(r.w)};
+  }
+
+  vCachedEdge conjugateRec(const vEdge& a) {
+    if (a.isZeroTerminal()) {
+      return vCachedEdge::zero();
+    }
+
+    if (a.isTerminal()) {
+      return {a.p, ComplexNumbers::conj(a.w)};
+    }
+
+    if (const auto* r = conjugateVector.lookup(a.p); r != nullptr) {
+      return {r->p, r->w * ComplexNumbers::conj(a.w)};
+    }
+
+    std::array<vCachedEdge, 2> e{};
+    e[0] = conjugateRec(a.p->e[0]);
+    e[1] = conjugateRec(a.p->e[1]);
+    auto res = makeDDNode(a.p->v, e);
+    conjugateVector.insert(a.p, res);
+    res.w = res.w * ComplexNumbers::conj(a.w);
+    return res;
+  }
+
   ///
   /// Matrix (conjugate) transpose
   ///
-  UnaryComputeTable<mEdge, mEdge, Config::CT_MAT_CONJ_TRANS_NBUCKET>
+  UnaryComputeTable<mNode*, mCachedEdge, Config::CT_MAT_CONJ_TRANS_NBUCKET>
       conjugateMatrixTranspose{};
 
   mEdge conjugateTranspose(const mEdge& a) {
+    auto r = conjugateTransposeRec(a);
+    return {r.p, cn.lookup(r.w)};
+  }
+
+  mCachedEdge conjugateTransposeRec(const mEdge& a) {
     if (a.isTerminal()) { // terminal case
       return {a.p, ComplexNumbers::conj(a.w)};
     }
 
     // check if in compute table
-    if (const auto* r = conjugateMatrixTranspose.lookup(a); r != nullptr) {
-      return *r;
+    if (const auto* r = conjugateMatrixTranspose.lookup(a.p); r != nullptr) {
+      return {r->p, r->w * ComplexNumbers::conj(a.w)};
     }
 
-    std::array<mEdge, NEDGE> e{};
+    std::array<mCachedEdge, NEDGE> e{};
     // conjugate transpose submatrices and rearrange as required
     for (auto i = 0U; i < RADIX; ++i) {
       for (auto j = 0U; j < RADIX; ++j) {
-        e[RADIX * i + j] = conjugateTranspose(a.p->e[RADIX * j + i]);
+        e[RADIX * i + j] = conjugateTransposeRec(a.p->e[RADIX * j + i]);
       }
     }
     // create new top node
     auto res = makeDDNode(a.p->v, e);
 
-    // adjust top weight including conjugate
-    res.w = cn.lookup(res.w * ComplexNumbers::conj(a.w));
-
     // put it in the compute table
-    conjugateMatrixTranspose.insert(a, res);
-    return res;
+    conjugateMatrixTranspose.insert(a.p, res);
+
+    // adjust top weight including conjugate
+    return {res.p, res.w * ComplexNumbers::conj(a.w)};
   }
 
   ///
   /// Multiplication
   ///
   ComputeTable<mNode*, vNode*, vCachedEdge, Config::CT_MAT_VEC_MULT_NBUCKET>
       matrixVectorMultiplication{};
@@ -1385,28 +1477,27 @@
     } else if constexpr (std::is_same_v<RightOperandNode, dNode>) {
       return densityDensityMultiplication;
     }
   }
 
   dEdge applyOperationToDensity(dEdge& e, const mEdge& operation) {
     auto tmp0 = conjugateTranspose(operation);
-    auto tmp1 = multiply(e, densityFromMatrixEdge(tmp0), 0, false);
-    auto tmp2 = multiply(densityFromMatrixEdge(operation), tmp1, 0, true);
+    auto tmp1 = multiply(e, densityFromMatrixEdge(tmp0), false);
+    auto tmp2 = multiply(densityFromMatrixEdge(operation), tmp1, true);
     incRef(tmp2);
     dEdge::alignDensityEdge(e);
     decRef(e);
     e = tmp2;
     dEdge::setDensityMatrixTrue(e);
     return e;
   }
 
   template <class LeftOperandNode, class RightOperandNode>
   Edge<RightOperandNode>
   multiply(const Edge<LeftOperandNode>& x, const Edge<RightOperandNode>& y,
-           const Qubit start = 0,
            [[maybe_unused]] const bool generateDensityMatrix = false) {
     using LEdge = Edge<LeftOperandNode>;
     using REdge = Edge<RightOperandNode>;
     static_assert(std::disjunction_v<std::is_same<LEdge, mEdge>,
                                      std::is_same<LEdge, dEdge>>,
                   "Left operand must be a matrix or density matrix");
     static_assert(std::disjunction_v<std::is_same<REdge, vEdge>,
@@ -1422,58 +1513,76 @@
       if (!xCopy.isTerminal()) {
         var = xCopy.p->v;
       }
       if (!y.isTerminal() && yCopy.p->v > var) {
         var = yCopy.p->v;
       }
 
-      const auto e = multiply2(xCopy, yCopy, var, start, generateDensityMatrix);
+      const auto e = multiply2(xCopy, yCopy, var, generateDensityMatrix);
       dEdge::revertDmChangesToEdges(xCopy, yCopy);
       return cn.lookup(e);
     } else {
       if (!x.isTerminal()) {
         var = x.p->v;
       }
       if (!y.isTerminal() && y.p->v > var) {
         var = y.p->v;
       }
-      const auto e = multiply2(x, y, var, start);
+      const auto e = multiply2(x, y, var);
       return cn.lookup(e);
     }
   }
 
 private:
   template <class LeftOperandNode, class RightOperandNode>
   CachedEdge<RightOperandNode>
   multiply2(const Edge<LeftOperandNode>& x, const Edge<RightOperandNode>& y,
-            const Qubit var, const Qubit start = 0,
+            const Qubit var,
             [[maybe_unused]] const bool generateDensityMatrix = false) {
     using LEdge = Edge<LeftOperandNode>;
     using REdge = Edge<RightOperandNode>;
     using ResultEdge = CachedEdge<RightOperandNode>;
 
     if (x.w.exactlyZero() || y.w.exactlyZero()) {
       return ResultEdge::zero();
     }
 
     const auto xWeight = static_cast<ComplexValue>(x.w);
     const auto yWeight = static_cast<ComplexValue>(y.w);
     const auto rWeight = xWeight * yWeight;
     if (x.isIdentity()) {
-      return {y.p, rWeight};
+      if constexpr (!std::is_same_v<RightOperandNode, dNode>) {
+        return {y.p, rWeight};
+      } else {
+        if (y.isIdentity() ||
+            (dNode::isDensityMatrixTempFlagSet(y.p->flags) &&
+             generateDensityMatrix) ||
+            (!dNode::isDensityMatrixTempFlagSet(y.p->flags) &&
+             !generateDensityMatrix)) {
+          return {y.p, rWeight};
+        }
+      }
     }
 
     if constexpr (std::is_same_v<RightOperandNode, mNode> ||
                   std::is_same_v<RightOperandNode, dNode>) {
       if (y.isIdentity()) {
-        return {x.p, rWeight};
+        if constexpr (!std::is_same_v<LeftOperandNode, dNode>) {
+          return {x.p, rWeight};
+        } else {
+          if (x.isIdentity() ||
+              (dNode::isDensityMatrixTempFlagSet(x.p->flags) &&
+               generateDensityMatrix) ||
+              (!dNode::isDensityMatrixTempFlagSet(x.p->flags) &&
+               !generateDensityMatrix)) {
+            return {x.p, rWeight};
+          }
+        }
       }
     }
-    assert(x.p != nullptr);
-    assert(y.p != nullptr);
 
     auto& computeTable = getMultiplicationComputeTable<RightOperandNode>();
     if (const auto* r = computeTable.lookup(x.p, y.p, generateDensityMatrix);
         r != nullptr) {
       return {r->p, r->w * rWeight};
     }
 
@@ -1485,56 +1594,74 @@
     std::array<ResultEdge, n> edge{};
     for (auto i = 0U; i < rows; i++) {
       for (auto j = 0U; j < cols; j++) {
         auto idx = cols * i + j;
         edge[idx] = ResultEdge::zero();
         for (auto k = 0U; k < rows; k++) {
           const auto xIdx = rows * i + k;
-          LEdge e1 = x.p->e[xIdx];
+          LEdge e1{};
+          if (x.p != nullptr && x.p->v == var) {
+            e1 = x.p->e[xIdx];
+          } else {
+            if (xIdx == 0 || xIdx == 3) {
+              e1 = LEdge{x.p, Complex::one()};
+            } else {
+              e1 = LEdge::zero();
+            }
+          }
 
           const auto yIdx = j + cols * k;
-          REdge e2 = y.p->e[yIdx];
+          REdge e2{};
+          if (y.p != nullptr && y.p->v == var) {
+            e2 = y.p->e[yIdx];
+          } else {
+            if (yIdx == 0 || yIdx == 3) {
+              e2 = REdge{y.p, Complex::one()};
+            } else {
+              e2 = REdge::zero();
+            }
+          }
 
           const auto v = static_cast<Qubit>(var - 1);
           if constexpr (std::is_same_v<LeftOperandNode, dNode>) {
             dCachedEdge m;
             dEdge::applyDmChangesToEdges(e1, e2);
             if (!generateDensityMatrix || idx == 1) {
               // When generateDensityMatrix is false or I have the first edge I
               // don't optimize anything and set generateDensityMatrix to false
               // for all child edges
-              m = multiply2(e1, e2, v, start, false);
+              m = multiply2(e1, e2, v, false);
             } else if (idx == 2) {
               // When I have the second edge and generateDensityMatrix == false,
               // then edge[2] == edge[1]
               if (k == 0) {
                 if (edge[1].w.approximatelyZero()) {
                   edge[2] = ResultEdge::zero();
                 } else {
                   edge[2] = edge[1];
                 }
               }
               continue;
             } else {
-              m = multiply2(e1, e2, v, start, generateDensityMatrix);
+              m = multiply2(e1, e2, v, generateDensityMatrix);
             }
 
             if (k == 0 || edge[idx].w.exactlyZero()) {
               edge[idx] = m;
             } else if (!m.w.exactlyZero()) {
               dNode::applyDmChangesToNode(edge[idx].p);
               dNode::applyDmChangesToNode(m.p);
               edge[idx] = add2(edge[idx], m, v);
               dNode::revertDmChangesToNode(m.p);
               dNode::revertDmChangesToNode(edge[idx].p);
             }
             // Undo modifications on density matrices
             dEdge::revertDmChangesToEdges(e1, e2);
           } else {
-            auto m = multiply2(e1, e2, v, start);
+            auto m = multiply2(e1, e2, v);
 
             if (k == 0 || edge[idx].w.exactlyZero()) {
               edge[idx] = m;
             } else if (!m.w.exactlyZero()) {
               edge[idx] = add2(edge[idx], m, v);
             }
           }
@@ -1564,18 +1691,15 @@
   **/
   ComplexValue innerProduct(const vEdge& x, const vEdge& y) {
     if (x.isTerminal() || y.isTerminal() || x.w.approximatelyZero() ||
         y.w.approximatelyZero()) { // the 0 case
       return 0;
     }
 
-    auto w = x.p->v;
-    if (y.p->v > w) {
-      w = y.p->v;
-    }
+    const auto w = std::max(x.p->v, y.p->v);
     // Overall normalization factor needs to be conjugated
     // before input into recursive private function
     auto xCopy = vEdge{x.p, ComplexNumbers::conj(x.w)};
     return innerProduct(xCopy, y, w + 1U);
   }
 
   fp fidelity(const vEdge& x, const vEdge& y) {
@@ -1696,19 +1820,19 @@
       @note This function calls the multiply() function to apply the operator to
   the quantum state, then calls innerProduct() to calculate the overlap between
   the original state and the applied state i.e. <Psi| Psi'> = <Psi| (Op|Psi>).
             It also calls the garbageCollect() function to free up any unused
   memory.
   **/
   fp expectationValue(const mEdge& x, const vEdge& y) {
-    assert(!x.isTerminal() && !y.isTerminal());
-    if (x.p->v != y.p->v) {
+    assert(!x.isZeroTerminal() && !y.isTerminal());
+    if (!x.isTerminal() && x.p->v > y.p->v) {
       throw std::invalid_argument(
-          "Observable and state must act on the same number of qubits to "
-          "compute the expectation value.");
+          "Observable must not act on more qubits than the state to compute the"
+          "expectation value.");
     }
 
     auto yPrime = multiply(x, y);
     const ComplexValue expValue = innerProduct(y, yPrime);
 
     assert(RealNumber::approximatelyZero(expValue.i));
     return expValue.r;
@@ -1729,35 +1853,28 @@
     } else {
       return matrixKronecker;
     }
   }
 
   template <class Node>
   Edge<Node> kronecker(const Edge<Node>& x, const Edge<Node>& y,
-                       const bool incIdx = true) {
+                       const std::size_t yNumQubits, const bool incIdx = true) {
     if constexpr (std::is_same_v<Node, dNode>) {
       throw std::invalid_argument(
           "Kronecker is currently not supported for density matrices");
     }
 
-    const auto e = kronecker2(x, y, incIdx);
+    const auto e = kronecker2(x, y, yNumQubits, incIdx);
     return cn.lookup(e);
   }
 
-  // extent the DD pointed to by `e` with `h` identities on top and `l`
-  // identities at the bottom
-  mEdge extend(const mEdge& e, const Qubit h, const Qubit l = 0) {
-    auto f = (l > 0) ? kronecker(e, makeIdent(l)) : e;
-    auto g = (h > 0) ? kronecker(makeIdent(h), f) : f;
-    return g;
-  }
-
 private:
   template <class Node>
   CachedEdge<Node> kronecker2(const Edge<Node>& x, const Edge<Node>& y,
+                              const std::size_t yNumQubits,
                               const bool incIdx = true) {
     if (x.w.exactlyZero() || y.w.exactlyZero()) {
       return CachedEdge<Node>::zero();
     }
     const auto xWeight = static_cast<ComplexValue>(x.w);
     if (xWeight.approximatelyZero()) {
       return CachedEdge<Node>::zero();
@@ -1767,64 +1884,76 @@
       return CachedEdge<Node>::zero();
     }
     const auto rWeight = xWeight * yWeight;
     if (rWeight.approximatelyZero()) {
       return CachedEdge<Node>::zero();
     }
 
-    if (x.isTerminal()) {
-      return {y.p, rWeight};
+    if (x.isTerminal() && y.isTerminal()) {
+      return {x.p, rWeight};
     }
 
+    if constexpr (std::is_same_v<Node, mNode> || std::is_same_v<Node, dNode>) {
+      if (x.isIdentity()) {
+        return {y.p, rWeight};
+      }
+    } else {
+      if (x.isTerminal()) {
+        return {y.p, rWeight};
+      }
+    }
+
+    // check if we already computed the product before and return the result
     auto& computeTable = getKroneckerComputeTable<Node>();
     if (const auto* r = computeTable.lookup(x.p, y.p); r != nullptr) {
       return {r->p, rWeight};
     }
 
     constexpr std::size_t n = std::tuple_size_v<decltype(x.p->e)>;
-    // special case handling for matrices
-    if constexpr (n == NEDGE) {
-      if (x.p->isIdentity()) {
-        auto idx = incIdx ? static_cast<Qubit>(y.p->v + 1) : y.p->v;
-        const auto yCopy = Edge<Node>{y.p, Complex::one()};
-        auto e = makeDDNode(idx, std::array{yCopy, Edge<Node>::zero(),
-                                            Edge<Node>::zero(), yCopy});
-        for (auto i = 0; i < x.p->v; ++i) {
-          idx = incIdx ? (e.p->v + 1) : e.p->v;
-          e = makeDDNode(
-              idx, std::array{e, Edge<Node>::zero(), Edge<Node>::zero(), e});
-        }
-        computeTable.insert(x.p, y.p, {e.p, e.w});
-        return {e.p, rWeight};
-      }
-    }
-
     std::array<CachedEdge<Node>, n> edge{};
     for (auto i = 0U; i < n; ++i) {
-      edge[i] = kronecker2(x.p->e[i], y, incIdx);
+      edge[i] = kronecker2(x.p->e[i], y, yNumQubits, incIdx);
     }
 
-    auto idx = incIdx ? (y.p->v + x.p->v + 1) : x.p->v;
-    auto e = makeDDNode(static_cast<Qubit>(idx), edge, true);
+    // Increase the qubit index
+    Qubit idx = x.p->v;
+    if (incIdx) {
+      // use the given number of qubits if y is an identity
+      if constexpr (std::is_same_v<Node, mNode> ||
+                    std::is_same_v<Node, dNode>) {
+        if (y.isIdentity()) {
+          idx += static_cast<Qubit>(yNumQubits);
+        } else {
+          idx += static_cast<Qubit>(y.p->v + 1U);
+        }
+      } else {
+        idx += static_cast<Qubit>(y.p->v + 1U);
+      }
+    }
+    auto e = makeDDNode(idx, edge, true);
     computeTable.insert(x.p, y.p, {e.p, e.w});
     return {e.p, rWeight};
   }
 
   ///
   /// (Partial) trace
   ///
 public:
   mEdge partialTrace(const mEdge& a, const std::vector<bool>& eliminate) {
-    auto r = trace(a, eliminate);
-    return cn.lookup(r);
+    auto r = trace(a, eliminate, eliminate.size());
+    return {r.p, cn.lookup(r.w)};
   }
 
-  template <class Node> ComplexValue trace(const Edge<Node>& a) {
-    const auto eliminate = std::vector<bool>(nqubits, true);
-    return trace(a, eliminate).w;
+  template <class Node>
+  ComplexValue trace(const Edge<Node>& a, const std::size_t numQubits) {
+    if (a.isIdentity()) {
+      return a.w * std::pow(2, numQubits);
+    }
+    const auto eliminate = std::vector<bool>(numQubits, true);
+    return trace(a, eliminate, numQubits).w;
   }
 
   /**
         Checks if a given matrix is close to the identity matrix, while ignoring
     any potential garbage qubits and ignoring the diagonal weights if
     `checkCloseToOne` is set to false.
         @param m An mEdge that represents the DD of the matrix.
@@ -1844,42 +1973,48 @@
                                       checkCloseToOne);
   }
 
 private:
   /// TODO: introduce a compute table for the trace?
   template <class Node>
   CachedEdge<Node> trace(const Edge<Node>& a,
-                         const std::vector<bool>& eliminate,
+                         const std::vector<bool>& eliminate, std::size_t level,
                          std::size_t alreadyEliminated = 0) {
     const auto aWeight = static_cast<ComplexValue>(a.w);
     if (aWeight.approximatelyZero()) {
       return CachedEdge<Node>::zero();
     }
 
-    if (Node::isTerminal(a.p) ||
-        std::none_of(eliminate.begin(), eliminate.end(),
+    if (std::none_of(eliminate.begin(), eliminate.end(),
                      [](bool v) { return v; })) {
       return CachedEdge<Node>{a.p, aWeight};
     }
 
+    if (a.isIdentity()) {
+      const auto elims =
+          std::count(eliminate.begin(),
+                     eliminate.begin() + static_cast<int64_t>(level), true);
+      return CachedEdge<Node>{a.p, aWeight * std::pow(2, elims)};
+    }
+
     const auto v = a.p->v;
     if (eliminate[v]) {
       const auto elims = alreadyEliminated + 1;
-      auto r = add2(trace(a.p->e[0], eliminate, elims),
-                    trace(a.p->e[3], eliminate, elims), v - 1);
+      auto r = add2(trace(a.p->e[0], eliminate, level - 1, elims),
+                    trace(a.p->e[3], eliminate, level - 1, elims), v - 1);
 
       r.w = r.w * aWeight;
       return r;
     }
 
     std::array<CachedEdge<Node>, NEDGE> edge{};
     std::transform(a.p->e.cbegin(), a.p->e.cend(), edge.begin(),
-                   [this, &eliminate, &alreadyEliminated](
-                       const Edge<Node>& e) -> CachedEdge<Node> {
-                     return trace(e, eliminate, alreadyEliminated);
+                   [this, &eliminate, &alreadyEliminated,
+                    &level](const Edge<Node>& e) -> CachedEdge<Node> {
+                     return trace(e, eliminate, level - 1, alreadyEliminated);
                    });
     const auto adjustedV =
         static_cast<Qubit>(static_cast<std::size_t>(a.p->v) -
                            (static_cast<std::size_t>(std::count(
                                 eliminate.begin(), eliminate.end(), true)) -
                             alreadyEliminated));
     auto r = makeDDNode(adjustedV, edge);
@@ -1888,36 +2023,35 @@
   }
 
   bool isCloseToIdentityRecursive(const mEdge& m,
                                   std::unordered_set<decltype(m.p)>& visited,
                                   const dd::fp tol,
                                   const std::vector<bool>& garbage,
                                   const bool checkCloseToOne) {
-    // immediately return if this node has already been visited
-    if (visited.find(m.p) != visited.end()) {
+    // immediately return if this node is identical to the identity or zero
+    if (m.isTerminal()) {
       return true;
     }
 
-    // immediately return if this node is identical to the identity
-    if (m.isTerminal() || m.p->isIdentity()) {
+    // immediately return if this node has already been visited
+    if (visited.find(m.p) != visited.end()) {
       return true;
     }
 
     const auto n = m.p->v;
 
     if (garbage.size() > n && garbage[n]) {
       return isCloseToIdentityRecursive(m.p->e[0U], visited, tol, garbage,
                                         checkCloseToOne) &&
              isCloseToIdentityRecursive(m.p->e[1U], visited, tol, garbage,
                                         checkCloseToOne) &&
              isCloseToIdentityRecursive(m.p->e[2U], visited, tol, garbage,
                                         checkCloseToOne) &&
              isCloseToIdentityRecursive(m.p->e[3U], visited, tol, garbage,
                                         checkCloseToOne);
-      ;
     }
 
     // check whether any of the middle successors is non-zero, i.e., m = [ x 0 0
     // y ]
     const auto mag1 = dd::ComplexNumbers::mag2(m.p->e[1U].w);
     const auto mag2 = dd::ComplexNumbers::mag2(m.p->e[2U].w);
     if (mag1 > tol || mag2 > tol) {
@@ -1963,155 +2097,188 @@
     return ident3;
   }
 
 public:
   ///
   /// Identity matrices
   ///
-  // create n-qubit identity DD. makeIdent(n) === makeIdent(0, n-1)
-  mEdge makeIdent(const std::size_t n) {
-    if (n == 0U) {
-      return mEdge::one();
-    }
-    return makeIdent(0, n - 1);
-  }
-  mEdge makeIdent(const std::size_t leastSignificantQubit,
-                  const std::size_t mostSignificantQubit) {
-    if (mostSignificantQubit < leastSignificantQubit) {
-      return mEdge::one();
-    }
-
-    const auto& entry = idTable.at(mostSignificantQubit);
-    if (leastSignificantQubit == 0 && entry.p != nullptr) {
-      return entry;
-    }
-
-    if (mostSignificantQubit >= 1) {
-      const auto& prevEntry = idTable.at(mostSignificantQubit - 1);
-      if (!prevEntry.isTerminal()) {
-        idTable.at(mostSignificantQubit) = makeDDNode(
-            static_cast<Qubit>(mostSignificantQubit),
-            std::array{prevEntry, mEdge::zero(), mEdge::zero(), prevEntry});
-        return idTable[mostSignificantQubit];
-      }
-    }
-
-    auto e = makeDDNode(
-        static_cast<Qubit>(leastSignificantQubit),
-        std::array{mEdge::one(), mEdge::zero(), mEdge::zero(), mEdge::one()});
-    for (auto k = leastSignificantQubit + 1; k <= mostSignificantQubit; ++k) {
-      e = makeDDNode(static_cast<Qubit>(k),
-                     std::array{e, mEdge::zero(), mEdge::zero(), e});
-    }
-    if (leastSignificantQubit == 0) {
-      idTable.at(mostSignificantQubit) = e;
-    }
-    return e;
-  }
-
-  // identity table access and reset
-  [[nodiscard]] const auto& getIdentityTable() const { return idTable; }
+  // create identity DD represented by the one-terminal.
+  mEdge makeIdent() { return mEdge::one(); }
 
-  void clearIdentityTable() {
-    for (auto& entry : idTable) {
-      entry.p = nullptr;
-    }
-  }
-
-  mEdge createInitialMatrix(const std::size_t n,
-                            const std::vector<bool>& ancillary) {
-    auto e = makeIdent(n);
-    incRef(e);
+  mEdge createInitialMatrix(const std::vector<bool>& ancillary) {
+    auto e = makeIdent();
     return reduceAncillae(e, ancillary);
   }
 
-private:
-  std::vector<mEdge> idTable{};
-
   ///
   /// Noise Operations
   ///
-public:
   StochasticNoiseOperationTable<mEdge, Config::STOCHASTIC_CACHE_OPS>
       stochasticNoiseOperationCache{nqubits};
   DensityNoiseTable<dEdge, dEdge, Config::CT_DM_NOISE_NBUCKET> densityNoise{};
 
   ///
   /// Ancillary and garbage reduction
   ///
   mEdge reduceAncillae(mEdge& e, const std::vector<bool>& ancillary,
                        const bool regular = true) {
-    // return if no more garbage left
+    // return if no more ancillaries left
     if (std::none_of(ancillary.begin(), ancillary.end(),
                      [](bool v) { return v; }) ||
-        e.isTerminal()) {
+        e.isZeroTerminal()) {
       return e;
     }
+
+    // if we have only identities and no other nodes
+    if (e.isIdentity()) {
+      auto g = e;
+      for (auto i = 0U; i < ancillary.size(); ++i) {
+        if (ancillary[i]) {
+          g = makeDDNode(
+              static_cast<Qubit>(i),
+              std::array{g, mEdge::zero(), mEdge::zero(), mEdge::zero()});
+        }
+      }
+      incRef(g);
+      return g;
+    }
+
     Qubit lowerbound = 0;
     for (auto i = 0U; i < ancillary.size(); ++i) {
       if (ancillary[i]) {
         lowerbound = static_cast<Qubit>(i);
         break;
       }
     }
-    if (e.p->v < lowerbound) {
-      return e;
+
+    auto g = CachedEdge<mNode>{e.p, 1.};
+    if (e.p->v >= lowerbound) {
+      g = reduceAncillaeRecursion(e.p, ancillary, lowerbound, regular);
+    }
+
+    for (std::size_t i = e.p->v + 1; i < ancillary.size(); ++i) {
+      if (ancillary[i]) {
+        g = makeDDNode(static_cast<Qubit>(i),
+                       std::array{g, mCachedEdge::zero(), mCachedEdge::zero(),
+                                  mCachedEdge::zero()});
+      }
     }
-    const auto f = reduceAncillaeRecursion(e.p, ancillary, lowerbound, regular);
-    const auto res = mEdge{f.p, cn.lookup(e.w * f.w)};
+    const auto res = mEdge{g.p, cn.lookup(g.w * e.w)};
     incRef(res);
     decRef(e);
     return res;
   }
 
-  // Garbage reduction works for reversible circuits --- to be thoroughly tested
-  // for quantum circuits
-  vEdge reduceGarbage(vEdge& e, const std::vector<bool>& garbage) {
+  /**
+  For each garbage qubit q, sums all the entries for q = 0 and q = 1 and sets
+  the entry for q = 0 to the sum and the entry for q = 1 to zero. In order to be
+  sure that the probabilities of the resulting state are the sum of the
+  probabilities of the initial state, we don't simply compute a sum, but we
+  compute `sqrt(|a|^2 + |b|^2)` for two entries `a` and `b`.
+  @param e DD representation of the matrix/vector
+  @param garbage vector that describes which qubits are garbage and which ones
+  are not. If garbage[i] = true, then qubit q_i is considered garbage
+  @param normalizeWeights By default set to `false`. If set to `true`,  the
+  function changes all weights in the DD to their magnitude, also for
+  non-garbage qubits. This is used for checking partial equivalence of circuits.
+  For partial equivalence, only the measurement probabilities are considered, so
+  we need to consider only the magnitudes of each entry.
+  @return DD representing of the reduced matrix/vector
+  **/
+  vEdge reduceGarbage(vEdge& e, const std::vector<bool>& garbage,
+                      const bool normalizeWeights = false) {
     // return if no more garbage left
-    if (std::none_of(garbage.begin(), garbage.end(),
-                     [](bool v) { return v; }) ||
-        e.isTerminal()) {
+    if (!normalizeWeights && (std::none_of(garbage.begin(), garbage.end(),
+                                           [](bool v) { return v; }) ||
+                              e.isTerminal())) {
       return e;
     }
     Qubit lowerbound = 0;
     for (std::size_t i = 0U; i < garbage.size(); ++i) {
       if (garbage[i]) {
         lowerbound = static_cast<Qubit>(i);
         break;
       }
     }
-    if (e.p->v < lowerbound) {
+    if (!normalizeWeights && e.p->v < lowerbound) {
       return e;
     }
-    const auto f = reduceGarbageRecursion(e.p, garbage, lowerbound);
-    const auto res = vEdge{f.p, cn.lookup(e.w * f.w)};
+    const auto f =
+        reduceGarbageRecursion(e.p, garbage, lowerbound, normalizeWeights);
+    auto weight = e.w * f.w;
+    if (normalizeWeights) {
+      weight = weight.mag();
+    }
+    const auto res = vEdge{f.p, cn.lookup(weight)};
     incRef(res);
     decRef(e);
     return res;
   }
   mEdge reduceGarbage(mEdge& e, const std::vector<bool>& garbage,
-                      const bool regular = true) {
+                      const bool regular = true,
+                      const bool normalizeWeights = false) {
     // return if no more garbage left
-    if (std::none_of(garbage.begin(), garbage.end(),
-                     [](bool v) { return v; }) ||
-        e.isTerminal()) {
+    if (!normalizeWeights && (std::none_of(garbage.begin(), garbage.end(),
+                                           [](bool v) { return v; }) ||
+                              e.isZeroTerminal())) {
       return e;
     }
+
+    // if we have only identities and no other nodes
+    if (e.isIdentity()) {
+      auto g = e;
+      for (auto i = 0U; i < garbage.size(); ++i) {
+        if (garbage[i]) {
+          if (regular) {
+            g = makeDDNode(static_cast<Qubit>(i),
+                           std::array{g, g, mEdge::zero(), mEdge::zero()});
+          } else {
+            g = makeDDNode(static_cast<Qubit>(i),
+                           std::array{g, mEdge::zero(), g, mEdge::zero()});
+          }
+        }
+      }
+      incRef(g);
+      return g;
+    }
+
     Qubit lowerbound = 0;
     for (auto i = 0U; i < garbage.size(); ++i) {
       if (garbage[i]) {
         lowerbound = static_cast<Qubit>(i);
         break;
       }
     }
-    if (e.p->v < lowerbound) {
-      return e;
+
+    auto g = CachedEdge<mNode>{e.p, 1.};
+    if (e.p->v >= lowerbound || normalizeWeights) {
+      g = reduceGarbageRecursion(e.p, garbage, lowerbound, regular,
+                                 normalizeWeights);
+    }
+
+    for (std::size_t i = e.p->v + 1; i < garbage.size(); ++i) {
+      if (garbage[i]) {
+        if (regular) {
+          g = makeDDNode(
+              static_cast<Qubit>(i),
+              std::array{g, g, mCachedEdge::zero(), mCachedEdge::zero()});
+        } else {
+          g = makeDDNode(
+              static_cast<Qubit>(i),
+              std::array{g, mCachedEdge::zero(), g, mCachedEdge::zero()});
+        }
+      }
+    }
+
+    auto weight = g.w * e.w;
+    if (normalizeWeights) {
+      weight = weight.mag();
     }
-    const auto f = reduceGarbageRecursion(e.p, garbage, lowerbound, regular);
-    const auto res = mEdge{f.p, cn.lookup(e.w * f.w)};
+    const auto res = mEdge{g.p, cn.lookup(weight)};
+
     incRef(res);
     decRef(e);
     return res;
   }
 
 private:
   mCachedEdge reduceAncillaeRecursion(mNode* p,
@@ -2121,31 +2288,63 @@
     if (p->v < lowerbound) {
       return {p, 1.};
     }
 
     std::array<mCachedEdge, NEDGE> edges{};
     std::bitset<NEDGE> handled{};
     for (auto i = 0U; i < NEDGE; ++i) {
-      if (!handled.test(i)) {
-        if (p->e[i].isTerminal()) {
-          edges[i] = {p->e[i].p, p->e[i].w};
-        } else {
-          edges[i] = reduceAncillaeRecursion(p->e[i].p, ancillary, lowerbound,
-                                             regular);
-          for (auto j = i + 1; j < NEDGE; ++j) {
-            if (p->e[i].p == p->e[j].p) {
-              edges[j] = edges[i];
-              edges[j].w = edges[j].w * p->e[j].w;
-              handled.set(j);
-            }
+      if (ancillary[p->v]) {
+        // no need to reduce ancillaries for entries that will be zeroed anyway
+        if ((i == 3) || (i == 1 && regular) || (i == 2 && !regular)) {
+          continue;
+        }
+      }
+      if (handled.test(i)) {
+        continue;
+      }
+
+      if (p->e[i].isZeroTerminal()) {
+        edges[i] = {p->e[i].p, p->e[i].w};
+        handled.set(i);
+        continue;
+      }
+
+      if (p->e[i].isIdentity()) {
+        auto g = mCachedEdge::one();
+        for (auto j = lowerbound; j < p->v; ++j) {
+          if (ancillary[j]) {
+            g = makeDDNode(j, std::array{g, mCachedEdge::zero(),
+                                         mCachedEdge::zero(),
+                                         mCachedEdge::zero()});
           }
-          edges[i].w = edges[i].w * p->e[i].w;
         }
+        edges[i] = {g.p, p->e[i].w};
         handled.set(i);
+        continue;
+      }
+
+      edges[i] =
+          reduceAncillaeRecursion(p->e[i].p, ancillary, lowerbound, regular);
+      for (Qubit j = p->e[i].p->v + 1U; j < p->v; ++j) {
+        if (ancillary[j]) {
+          edges[i] = makeDDNode(j, std::array{edges[i], mCachedEdge::zero(),
+                                              mCachedEdge::zero(),
+                                              mCachedEdge::zero()});
+        }
+      }
+
+      for (auto j = i + 1U; j < NEDGE; ++j) {
+        if (p->e[i].p == p->e[j].p) {
+          edges[j] = edges[i];
+          edges[j].w = edges[j].w * p->e[j].w;
+          handled.set(j);
+        }
       }
+      edges[i].w = edges[i].w * p->e[i].w;
+      handled.set(i);
     }
     if (!ancillary[p->v]) {
       return makeDDNode(p->v, edges);
     }
 
     // something to reduce for this qubit
     if (regular) {
@@ -2153,88 +2352,149 @@
                                          edges[2], mCachedEdge::zero()});
     }
     return makeDDNode(p->v, std::array{edges[0], edges[1], mCachedEdge::zero(),
                                        mCachedEdge::zero()});
   }
 
   vCachedEdge reduceGarbageRecursion(vNode* p, const std::vector<bool>& garbage,
-                                     const Qubit lowerbound) {
-    if (p->v < lowerbound) {
+                                     const Qubit lowerbound,
+                                     const bool normalizeWeights = false) {
+    if (!normalizeWeights && p->v < lowerbound) {
       return {p, 1.};
     }
 
     std::array<vCachedEdge, RADIX> edges{};
     std::bitset<RADIX> handled{};
     for (auto i = 0U; i < RADIX; ++i) {
       if (!handled.test(i)) {
         if (p->e[i].isTerminal()) {
-          edges[i] = {p->e[i].p, p->e[i].w};
+          const auto weight = normalizeWeights
+                                  ? ComplexNumbers::mag(p->e[i].w)
+                                  : static_cast<ComplexValue>(p->e[i].w);
+          edges[i] = {p->e[i].p, weight};
         } else {
-          edges[i] = reduceGarbageRecursion(p->e[i].p, garbage, lowerbound);
+          edges[i] = reduceGarbageRecursion(p->e[i].p, garbage, lowerbound,
+                                            normalizeWeights);
           for (auto j = i + 1; j < RADIX; ++j) {
             if (p->e[i].p == p->e[j].p) {
               edges[j] = edges[i];
               edges[j].w = edges[j].w * p->e[j].w;
+              if (normalizeWeights) {
+                edges[j].w = edges[j].w.mag();
+              }
               handled.set(j);
             }
           }
           edges[i].w = edges[i].w * p->e[i].w;
+          if (normalizeWeights) {
+            edges[i].w = edges[i].w.mag();
+          }
         }
         handled.set(i);
       }
     }
     if (!garbage[p->v]) {
       return makeDDNode(p->v, edges);
     }
     // something to reduce for this qubit
-    return makeDDNode(p->v, std::array{add2(edges[0], edges[1], p->v - 1),
-                                       vCachedEdge ::zero()});
+    return makeDDNode(p->v,
+                      std::array{addMagnitudes(edges[0], edges[1], p->v - 1),
+                                 vCachedEdge ::zero()});
   }
   mCachedEdge reduceGarbageRecursion(mNode* p, const std::vector<bool>& garbage,
                                      const Qubit lowerbound,
-                                     const bool regular = true) {
-    if (p->v < lowerbound) {
+                                     const bool regular = true,
+                                     const bool normalizeWeights = false) {
+    if (!normalizeWeights && p->v < lowerbound) {
       return {p, 1.};
     }
 
     std::array<mCachedEdge, NEDGE> edges{};
     std::bitset<NEDGE> handled{};
     for (auto i = 0U; i < NEDGE; ++i) {
-      if (!handled.test(i)) {
-        if (p->e[i].isTerminal()) {
-          edges[i] = {p->e[i].p, p->e[i].w};
-        } else {
-          edges[i] =
-              reduceGarbageRecursion(p->e[i].p, garbage, lowerbound, regular);
-          for (auto j = i + 1; j < NEDGE; ++j) {
-            if (p->e[i].p == p->e[j].p) {
-              edges[j] = edges[i];
-              edges[j].w = edges[j].w * p->e[j].w;
-              handled.set(j);
+      if (handled.test(i)) {
+        continue;
+      }
+
+      if (p->e[i].isZeroTerminal()) {
+        edges[i] = mCachedEdge::zero();
+        handled.set(i);
+        continue;
+      }
+
+      if (p->e[i].isIdentity()) {
+        edges[i] = mCachedEdge::one();
+        for (auto j = lowerbound; j < p->v; ++j) {
+          if (garbage[j]) {
+            if (regular) {
+              edges[i] = makeDDNode(j, std::array{edges[i], edges[i],
+                                                  mCachedEdge::zero(),
+                                                  mCachedEdge::zero()});
+            } else {
+              edges[i] =
+                  makeDDNode(j, std::array{edges[i], mCachedEdge::zero(),
+                                           edges[i], mCachedEdge::zero()});
             }
           }
+        }
+        if (normalizeWeights) {
+          edges[i].w = edges[i].w * ComplexNumbers::mag(p->e[i].w);
+        } else {
           edges[i].w = edges[i].w * p->e[i].w;
         }
         handled.set(i);
+        continue;
       }
+
+      edges[i] = reduceGarbageRecursion(p->e[i].p, garbage, lowerbound, regular,
+                                        normalizeWeights);
+      for (Qubit j = p->e[i].p->v + 1U; j < p->v; ++j) {
+        if (garbage[j]) {
+          if (regular) {
+            edges[i] = makeDDNode(j, std::array{edges[i], edges[i],
+                                                mCachedEdge::zero(),
+                                                mCachedEdge::zero()});
+          } else {
+            edges[i] = makeDDNode(j, std::array{edges[i], mCachedEdge::zero(),
+                                                edges[i], mCachedEdge::zero()});
+          }
+        }
+      }
+
+      for (auto j = i + 1; j < NEDGE; ++j) {
+        if (p->e[i].p == p->e[j].p) {
+          edges[j] = edges[i];
+          edges[j].w = edges[j].w * p->e[j].w;
+          if (normalizeWeights) {
+            edges[j].w = edges[j].w.mag();
+          }
+          handled.set(j);
+        }
+      }
+      edges[i].w = edges[i].w * p->e[i].w;
+      if (normalizeWeights) {
+        edges[i].w = edges[i].w.mag();
+      }
+      handled.set(i);
     }
     if (!garbage[p->v]) {
       return makeDDNode(p->v, edges);
     }
 
     if (regular) {
       return makeDDNode(p->v,
-                        std::array{add2(edges[0], edges[2], p->v - 1),
-                                   add2(edges[1], edges[3], p->v - 1),
+                        std::array{addMagnitudes(edges[0], edges[2], p->v - 1),
+                                   addMagnitudes(edges[1], edges[3], p->v - 1),
                                    mCachedEdge::zero(), mCachedEdge::zero()});
     }
-    return makeDDNode(p->v, std::array{add2(edges[0], edges[1], p->v - 1),
-                                       mCachedEdge::zero(),
-                                       add2(edges[2], edges[3], p->v - 1),
-                                       mCachedEdge::zero()});
+    return makeDDNode(p->v,
+                      std::array{addMagnitudes(edges[0], edges[1], p->v - 1),
+                                 mCachedEdge::zero(),
+                                 addMagnitudes(edges[2], edges[3], p->v - 1),
+                                 mCachedEdge::zero()});
   }
 
   ///
   /// Vector and matrix extraction from DDs
   ///
 public:
   // transfers a decision diagram from another package to this package
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/RealNumber.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/RealNumber.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/RealNumberUniqueTable.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/RealNumberUniqueTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/Simulation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/Simulation.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/StochasticNoiseOperationTable.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/StochasticNoiseOperationTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/UnaryComputeTable.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/UnaryComputeTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/UniqueTable.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/UniqueTable.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -297,16 +297,15 @@
     }
   };
 
   void print() {
     auto q = nvars - 1U;
     for (auto it = tables.rbegin(); it != tables.rend(); ++it) {
       auto& table = *it;
-      std::cout << "\tq" << q << ":"
-                << "\n";
+      std::cout << "\tq" << q << ":" << "\n";
       for (std::size_t key = 0; key < table.size(); ++key) {
         auto p = table[key];
         if (p != nullptr) {
           std::cout << "\tkey=" << key << ": ";
         }
 
         while (p != nullptr) {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/PackageStatistics.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/PackageStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/Statistics.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/Statistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/TableStatistics.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/TableStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Ecc.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Ecc.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -99,13 +99,13 @@
    * */
   virtual void writeDecoding() = 0;
 
   virtual void mapGate(const qc::Operation& gate) = 0;
 
   void gateNotAvailableError(const qc::Operation& gate) const {
     std::stringstream stream;
-    stream << "Gate " << gate << " not supported to encode in error code "
-           << ecc.name << "!";
+    stream << "Gate " << toString(gate.getType())
+           << " not supported to encode in error code " << ecc.name << "!";
     throw qc::QFRException(stream.str());
   }
 };
 } // namespace ecc
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q18Surface.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q18Surface.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q3Shor.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q3Shor.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q5Laflamme.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q5Laflamme.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q7Steane.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q7Steane.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q9Shor.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q9Shor.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/ecc/Q9Surface.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/ecc/Q9Surface.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/ClassicControlledOperation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/ClassicControlledOperation.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
   // expected value
   ClassicControlledOperation(std::unique_ptr<qc::Operation>& operation,
                              ClassicalRegister controlReg,
                              std::uint64_t expectedVal = 1U,
                              ComparisonKind kind = ComparisonKind::Eq)
       : op(std::move(operation)), controlRegister(std::move(controlReg)),
         expectedValue(expectedVal), comparisonKind(kind) {
-    nqubits = op->getNqubits();
     name = "c_" + shortName(op->getType());
     parameter.reserve(3);
     parameter.emplace_back(static_cast<fp>(controlRegister.first));
     parameter.emplace_back(static_cast<fp>(controlRegister.second));
     parameter.emplace_back(static_cast<fp>(expectedValue));
     type = ClassicControlled;
   }
@@ -69,19 +68,14 @@
 
   [[nodiscard]] auto getControlRegister() const { return controlRegister; }
 
   [[nodiscard]] auto getExpectedValue() const { return expectedValue; }
 
   [[nodiscard]] auto getOperation() const { return op.get(); }
 
-  void setNqubits(std::size_t nq) override {
-    nqubits = nq;
-    op->setNqubits(nq);
-  }
-
   [[nodiscard]] const Targets& getTargets() const override {
     return op->getTargets();
   }
 
   Targets& getTargets() override { return op->getTargets(); }
 
   [[nodiscard]] std::size_t getNtargets() const override {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/CompoundOperation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/CompoundOperation.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 namespace qc {
 
 class CompoundOperation final : public Operation {
 private:
   std::vector<std::unique_ptr<Operation>> ops{};
 
 public:
-  explicit CompoundOperation(std::size_t nq);
+  explicit CompoundOperation();
 
-  CompoundOperation(std::size_t nq,
-                    std::vector<std::unique_ptr<Operation>>&& operations);
+  explicit CompoundOperation(
+      std::vector<std::unique_ptr<Operation>>&& operations);
 
   CompoundOperation(const CompoundOperation& co);
 
   CompoundOperation& operator=(const CompoundOperation& co);
 
   [[nodiscard]] std::unique_ptr<Operation> clone() const override;
 
-  void setNqubits(std::size_t nq) override;
-
   [[nodiscard]] bool isCompoundOperation() const override;
 
   [[nodiscard]] bool isNonUnitaryOperation() const override;
 
   [[nodiscard]] inline bool isSymbolicOperation() const override;
 
   void addControl(Control c) override;
@@ -37,15 +35,16 @@
   Controls::iterator removeControl(Controls::iterator it) override;
 
   [[nodiscard]] bool equals(const Operation& op, const Permutation& perm1,
                             const Permutation& perm2) const override;
   [[nodiscard]] bool equals(const Operation& operation) const override;
 
   std::ostream& print(std::ostream& os, const Permutation& permutation,
-                      std::size_t prefixWidth) const override;
+                      std::size_t prefixWidth,
+                      std::size_t nqubits) const override;
 
   [[nodiscard]] bool actsOn(Qubit i) const override;
 
   void addDepthContribution(std::vector<std::size_t>& depths) const override;
 
   void dumpOpenQASM(std::ostream& of, const RegisterNames& qreg,
                     const RegisterNames& creg, size_t indent,
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/Control.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/Control.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/Expression.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/Expression.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/NonUnitaryOperation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/NonUnitaryOperation.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 
 namespace qc {
 
 class NonUnitaryOperation final : public Operation {
 protected:
   std::vector<Bit> classics{}; // vector for the classical bits to measure into
 
-  void printMeasurement(std::ostream& os, const std::vector<Qubit>& q,
-                        const std::vector<Bit>& c,
-                        const Permutation& permutation) const;
+  static void printMeasurement(std::ostream& os, const std::vector<Qubit>& q,
+                               const std::vector<Bit>& c,
+                               const Permutation& permutation,
+                               std::size_t nqubits);
   void printReset(std::ostream& os, const std::vector<Qubit>& q,
-                  const Permutation& permutation) const;
+                  const Permutation& permutation, std::size_t nqubits) const;
 
 public:
   // Measurement constructor
-  NonUnitaryOperation(std::size_t nq, std::vector<Qubit> qubitRegister,
+  NonUnitaryOperation(std::vector<Qubit> qubitRegister,
                       std::vector<Bit> classicalRegister);
-  NonUnitaryOperation(std::size_t nq, Qubit qubit, Bit cbit);
+  NonUnitaryOperation(Qubit qubit, Bit cbit);
 
   // General constructor
-  NonUnitaryOperation(std::size_t nq, Targets qubits, OpType op = Reset);
+  explicit NonUnitaryOperation(Targets qubits, OpType op = Reset);
 
   [[nodiscard]] std::unique_ptr<Operation> clone() const override {
     return std::make_unique<NonUnitaryOperation>(*this);
   }
 
   [[nodiscard]] bool isUnitary() const override { return false; }
 
@@ -69,15 +70,16 @@
   [[nodiscard]] bool equals(const Operation& op, const Permutation& perm1,
                             const Permutation& perm2) const override;
   [[nodiscard]] bool equals(const Operation& operation) const override {
     return equals(operation, {}, {});
   }
 
   std::ostream& print(std::ostream& os, const Permutation& permutation,
-                      std::size_t prefixWidth) const override;
+                      std::size_t prefixWidth,
+                      std::size_t nqubits) const override;
 
   void dumpOpenQASM(std::ostream& of, const RegisterNames& qreg,
                     const RegisterNames& creg, size_t indent,
                     bool openQASM3) const override;
 
   void invert() override {
     throw QFRException("Inverting a non-unitary operation is not supported.");
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/OpType.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/OpType.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/Operation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/Operation.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 namespace qc {
 class Operation {
 protected:
   Controls controls{};
   Targets targets{};
   std::vector<fp> parameter{};
 
-  std::size_t nqubits = 0;
-  Qubit startQubit = 0;
   OpType type = None;
   std::string name{};
 
   static bool isWholeQubitRegister(const RegisterNames& reg, std::size_t start,
                                    std::size_t end) {
     return !reg.empty() && reg[start].first == reg[end].first &&
            (start == 0 || reg[start].first != reg[start - 1].first) &&
@@ -54,26 +52,22 @@
 
   [[nodiscard]] virtual const Controls& getControls() const { return controls; }
   virtual Controls& getControls() { return controls; }
   [[nodiscard]] virtual std::size_t getNcontrols() const {
     return controls.size();
   }
 
-  [[nodiscard]] std::size_t getNqubits() const { return nqubits; }
-
   [[nodiscard]] const std::vector<fp>& getParameter() const {
     return parameter;
   }
   std::vector<fp>& getParameter() { return parameter; }
 
   [[nodiscard]] const std::string& getName() const { return name; }
   [[nodiscard]] virtual OpType getType() const { return type; }
 
-  [[nodiscard]] virtual Qubit getStartingQubit() const { return startQubit; }
-
   [[nodiscard]] virtual std::set<Qubit> getUsedQubits() const {
     const auto& opTargets = getTargets();
     const auto& opControls = getControls();
     std::set<Qubit> usedQubits = {opTargets.begin(), opTargets.end()};
     for (const auto& control : opControls) {
       usedQubits.insert(control.qubit);
     }
@@ -83,16 +77,14 @@
   [[nodiscard]] std::unique_ptr<Operation> getInverted() const {
     auto op = clone();
     op->invert();
     return op;
   }
 
   // Setter
-  virtual void setNqubits(const std::size_t nq) { nqubits = nq; }
-
   virtual void setTargets(const Targets& t) { targets = t; }
 
   virtual void setControls(const Controls& c) {
     clearControls();
     addControls(c);
   }
 
@@ -164,21 +156,20 @@
                                     const Permutation& perm1,
                                     const Permutation& perm2) const;
   [[nodiscard]] virtual bool equals(const Operation& op) const {
     return equals(op, {}, {});
   }
 
   virtual std::ostream& printParameters(std::ostream& os) const;
-  std::ostream& print(std::ostream& os) const { return print(os, {}, 0); }
-  virtual std::ostream& print(std::ostream& os, const Permutation& permutation,
-                              std::size_t prefixWidth) const;
-
-  friend std::ostream& operator<<(std::ostream& os, const Operation& op) {
-    return op.print(os);
+  std::ostream& print(std::ostream& os, const std::size_t nqubits) const {
+    return print(os, {}, 0, nqubits);
   }
+  virtual std::ostream& print(std::ostream& os, const Permutation& permutation,
+                              std::size_t prefixWidth,
+                              std::size_t nqubits) const;
 
   void dumpOpenQASM2(std::ostream& of, const RegisterNames& qreg,
                      const RegisterNames& creg) const {
     dumpOpenQASM(of, qreg, creg, 0, false);
   }
   void dumpOpenQASM3(std::ostream& of, const RegisterNames& qreg,
                      const RegisterNames& creg) const {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/StandardOperation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/StandardOperation.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -23,50 +23,39 @@
   }
 
   OpType parseU3(fp& theta, fp& phi, fp& lambda);
   OpType parseU2(fp& phi, fp& lambda);
   OpType parseU1(fp& lambda);
 
   void checkUgate();
-  void setup(std::size_t nq, Qubit startingQubit = 0);
+  void setup();
 
   void dumpOpenQASMTeleportation(std::ostream& of,
                                  const RegisterNames& qreg) const;
 
 public:
   StandardOperation() = default;
 
   // Standard Constructors
-  StandardOperation(std::size_t nq, Qubit target, OpType g,
-                    std::vector<fp> params = {}, Qubit startingQubit = 0);
-  StandardOperation(std::size_t nq, const Targets& targ, OpType g,
-                    std::vector<fp> params = {}, Qubit startingQubit = 0);
-
-  StandardOperation(std::size_t nq, Control control, Qubit target, OpType g,
-                    const std::vector<fp>& params = {},
-                    Qubit startingQubit = 0);
-  StandardOperation(std::size_t nq, Control control, const Targets& targ,
-                    OpType g, const std::vector<fp>& params = {},
-                    Qubit startingQubit = 0);
-
-  StandardOperation(std::size_t nq, const Controls& c, Qubit target, OpType g,
-                    const std::vector<fp>& params = {},
-                    Qubit startingQubit = 0);
-  StandardOperation(std::size_t nq, const Controls& c, const Targets& targ,
-                    OpType g, const std::vector<fp>& params = {},
-                    Qubit startingQubit = 0);
-
-  // MCT Constructor
-  StandardOperation(std::size_t nq, const Controls& c, Qubit target,
-                    Qubit startingQubit = 0);
+  StandardOperation(Qubit target, OpType g, std::vector<fp> params = {});
+  StandardOperation(const Targets& targ, OpType g, std::vector<fp> params = {});
+
+  StandardOperation(Control control, Qubit target, OpType g,
+                    const std::vector<fp>& params = {});
+  StandardOperation(Control control, const Targets& targ, OpType g,
+                    const std::vector<fp>& params = {});
+
+  StandardOperation(const Controls& c, Qubit target, OpType g,
+                    const std::vector<fp>& params = {});
+  StandardOperation(const Controls& c, const Targets& targ, OpType g,
+                    const std::vector<fp>& params = {});
 
   // MCF (cSWAP), Peres, parameterized two target Constructor
-  StandardOperation(std::size_t nq, const Controls& c, Qubit target0,
-                    Qubit target1, OpType g, const std::vector<fp>& params = {},
-                    Qubit startingQubit = 0);
+  StandardOperation(const Controls& c, Qubit target0, Qubit target1, OpType g,
+                    const std::vector<fp>& params = {});
 
   [[nodiscard]] std::unique_ptr<Operation> clone() const override {
     return std::make_unique<StandardOperation>(*this);
   }
 
   [[nodiscard]] bool isStandardOperation() const override { return true; }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/operations/SymbolicOperation.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/operations/SymbolicOperation.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -55,16 +55,15 @@
 
   static Symbolic& getSymbol(SymbolOrNumber& param) {
     return std::get<Symbolic>(param);
   }
 
   static fp& getNumber(SymbolOrNumber& param) { return std::get<fp>(param); }
 
-  void setup(std::size_t nq, const std::vector<SymbolOrNumber>& params,
-             Qubit startingQubit = 0);
+  void setup(const std::vector<SymbolOrNumber>& params);
 
   [[nodiscard]] static fp
   getInstantiation(const SymbolOrNumber& symOrNum,
                    const VariableAssignment& assignment);
 
   void negateSymbolicParameter(std::size_t index);
 
@@ -90,40 +89,32 @@
   }
 
   void setSymbolicParameter(const Symbolic& par, const std::size_t i) {
     symbolicParameter.at(i) = par;
   }
 
   // Standard Constructors
-  SymbolicOperation(std::size_t nq, Qubit target, OpType g,
-                    const std::vector<SymbolOrNumber>& params = {},
-                    Qubit startingQubit = 0);
-  SymbolicOperation(std::size_t nq, const Targets& targ, OpType g,
-                    const std::vector<SymbolOrNumber>& params = {},
-                    Qubit startingQubit = 0);
-
-  SymbolicOperation(std::size_t nq, Control control, Qubit target, OpType g,
-                    const std::vector<SymbolOrNumber>& params = {},
-                    Qubit startingQubit = 0);
-  SymbolicOperation(std::size_t nq, Control control, const Targets& targ,
-                    OpType g, const std::vector<SymbolOrNumber>& params = {},
-                    Qubit startingQubit = 0);
-
-  SymbolicOperation(std::size_t nq, const Controls& c, Qubit target, OpType g,
-                    const std::vector<SymbolOrNumber>& params = {},
-                    Qubit startingQubit = 0);
-  SymbolicOperation(std::size_t nq, const Controls& c, const Targets& targ,
-                    OpType g, const std::vector<SymbolOrNumber>& params = {},
-                    Qubit startingQubit = 0);
+  SymbolicOperation(Qubit target, OpType g,
+                    const std::vector<SymbolOrNumber>& params = {});
+  SymbolicOperation(const Targets& targ, OpType g,
+                    const std::vector<SymbolOrNumber>& params = {});
+
+  SymbolicOperation(Control control, Qubit target, OpType g,
+                    const std::vector<SymbolOrNumber>& params = {});
+  SymbolicOperation(Control control, const Targets& targ, OpType g,
+                    const std::vector<SymbolOrNumber>& params = {});
+
+  SymbolicOperation(const Controls& c, Qubit target, OpType g,
+                    const std::vector<SymbolOrNumber>& params = {});
+  SymbolicOperation(const Controls& c, const Targets& targ, OpType g,
+                    const std::vector<SymbolOrNumber>& params = {});
 
   // MCF (cSWAP), Peres, parameterized two target Constructor
-  SymbolicOperation(std::size_t nq, const Controls& c, Qubit target0,
-                    Qubit target1, OpType g,
-                    const std::vector<SymbolOrNumber>& params = {},
-                    Qubit startingQubit = 0);
+  SymbolicOperation(const Controls& c, Qubit target0, Qubit target1, OpType g,
+                    const std::vector<SymbolOrNumber>& params = {});
 
   [[nodiscard]] std::unique_ptr<Operation> clone() const override {
     return std::make_unique<SymbolicOperation>(*this);
   }
 
   [[nodiscard]] inline bool isSymbolicOperation() const override {
     return std::any_of(symbolicParameter.begin(), symbolicParameter.end(),
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Exception.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Exception.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Gate.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Gate.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Parser.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Parser.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Scanner.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Scanner.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Statement.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Statement.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/StdGates.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/StdGates.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Token.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Token.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Types.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/Types.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/python/qiskit/QuantumCircuit.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/python/qiskit/QuantumCircuit.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/FunctionalityConstruction.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/FunctionalityConstruction.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Rational.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Rational.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Rules.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Rules.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Simplify.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Simplify.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/Utils.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/Utils.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/ZXDefinitions.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/ZXDefinitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/include/mqt-core/zx/ZXDiagram.hpp` & `mqt_qmap-2.5.1/extern/mqt-core/include/mqt-core/zx/ZXDiagram.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/noxfile.py` & `mqt_qmap-2.5.1/extern/mqt-core/noxfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Nox sessions."""
 
 from __future__ import annotations
 
 import argparse
 import os
+import shutil
 import sys
 from typing import TYPE_CHECKING
 
 import nox
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
+nox.needs_version = ">=2024.3.2"
+nox.options.default_venv_backend = "uv|virtualenv"
+
 nox.options.sessions = ["lint", "tests"]
 
 PYTHON_ALL_VERSIONS = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 BUILD_REQUIREMENTS = [
     "scikit-build-core[pyproject]>=0.8.1",
     "setuptools_scm>=7",
-    "pybind11>=2.11",
+    "pybind11>=2.12",
 ]
 
 if os.environ.get("CI", None):
     nox.options.error_on_missing_interpreters = True
 
 
 @nox.session(reuse_venv=True)
@@ -42,54 +46,57 @@
 ) -> None:
     posargs = list(session.posargs)
     env = {"PIP_DISABLE_PIP_VERSION_CHECK": "1"}
 
     if os.environ.get("CI", None) and sys.platform == "win32":
         env["CMAKE_GENERATOR"] = "Ninja"
 
+    if shutil.which("cmake") is None and shutil.which("cmake3") is None:
+        session.install("cmake")
+    if shutil.which("ninja") is None:
+        session.install("ninja")
+
     _extras = ["test", *extras]
     if "--cov" in posargs:
         _extras.append("coverage")
         posargs.append("--cov-config=pyproject.toml")
 
     session.install(*BUILD_REQUIREMENTS, *install_args, env=env)
-    install_arg = f".[{','.join(_extras)}]"
+    install_arg = f"-ve.[{','.join(_extras)}]"
     session.install("--no-build-isolation", install_arg, *install_args, env=env)
     session.run("pytest", *run_args, *posargs, env=env)
 
 
 @nox.session(reuse_venv=True, python=PYTHON_ALL_VERSIONS)
 def tests(session: nox.Session) -> None:
     """Run the test suite."""
     _run_tests(session)
 
 
-@nox.session()
+@nox.session(reuse_venv=True, venv_backend="uv")
 def minimums(session: nox.Session) -> None:
     """Test the minimum versions of dependencies."""
     _run_tests(
         session,
-        install_args=["--constraint=test/python/constraints.txt"],
+        install_args=["--resolution=lowest-direct"],
         run_args=["-Wdefault"],
+        extras=["qiskit", "evaluation"],
     )
-    session.run("pip", "list")
+    session.run("uv", "pip", "list")
 
 
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
-    """Build the docs. Pass "--serve" to serve. Pass "-b linkcheck" to check links."""
+    """Build the docs. Use "--non-interactive" to avoid serving. Pass "-b linkcheck" to check links."""
     parser = argparse.ArgumentParser()
-    parser.add_argument("--serve", action="store_true", help="Serve after building")
     parser.add_argument("-b", dest="builder", default="html", help="Build target (default: html)")
     args, posargs = parser.parse_known_args(session.posargs)
 
-    if args.builder != "html" and args.serve:
-        session.error("Must not specify non-HTML builder with --serve")
-
-    extra_installs = ["sphinx-autobuild"] if args.serve else []
+    serve = args.builder == "html" and session.interactive
+    extra_installs = ["sphinx-autobuild"] if serve else []
     session.install(*BUILD_REQUIREMENTS, *extra_installs)
     session.install("--no-build-isolation", "-ve.[docs]")
     session.chdir("docs")
 
     if args.builder == "linkcheck":
         session.run("sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs)
         return
@@ -99,11 +106,11 @@
         "-T",  # full tracebacks
         f"-b={args.builder}",
         ".",
         f"_build/{args.builder}",
         *posargs,
     )
 
-    if args.serve:
+    if serve:
         session.run("sphinx-autobuild", *shared_args)
     else:
         session.run("sphinx-build", "--keep-going", *shared_args)
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/pyproject.toml` & `mqt_qmap-2.5.1/extern/mqt-core/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["scikit-build-core>=0.8.1", "setuptools-scm>=7", "pybind11>=2.11"]
+requires = ["scikit-build-core>=0.8.1", "setuptools-scm>=7", "pybind11>=2.12"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "mqt-core"
 description = "The Backbone of the Munich Quantum Toolkit"
 readme = "README.md"
 authors = [
@@ -33,15 +33,15 @@
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest>=7.0", "pytest-console-scripts>=1.4", "mqt.core[qiskit, evaluation]"]
-coverage = ["mqt.core[test]", "pytest-cov"]
+coverage = ["mqt.core[test]", "pytest-cov>=4"]
 evaluation = [
     "pandas[output_formatting]>=2.0; python_version < '3.9'",
     "pandas[output-formatting]>=2.1.2; python_version >= '3.9'",
 ]
 docs = [
     "furo>=2023.08.17",
     "sphinx",
@@ -257,14 +257,15 @@
 
 
 [tool.cibuildwheel]
 build = "cp3*"
 skip = "*-musllinux_*"
 archs = "auto64"
 test-command = "python -c \"from mqt import core\""
+test-skip = "cp38-macosx_arm64"
 build-frontend = "build"
 
 [tool.cibuildwheel.linux]
 environment = { DEPLOY = "ON" }
 
 [tool.cibuildwheel.macos]
 environment = { MACOSX_DEPLOYMENT_TARGET = "10.15" }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/CMakeLists.txt` & `mqt_qmap-2.5.1/extern/mqt-core/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/CircuitOptimizer.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/CircuitOptimizer.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #include "CircuitOptimizer.hpp"
 
+#include <algorithm>
 #include <cassert>
+#include <utility>
+#include <vector>
 
 namespace qc {
 void CircuitOptimizer::removeIdentities(QuantumComputation& qc) {
   // delete the identities from circuit
   auto it = qc.ops.begin();
   while (it != qc.ops.end()) {
     if ((*it)->getType() == I) {
@@ -34,17 +37,15 @@
     }
   }
 }
 
 void CircuitOptimizer::swapReconstruction(QuantumComputation& qc) {
   Qubit highestPhysicalQubit = 0;
   for (const auto& q : qc.initialLayout) {
-    if (q.first > highestPhysicalQubit) {
-      highestPhysicalQubit = q.first;
-    }
+    highestPhysicalQubit = std::max(q.first, highestPhysicalQubit);
   }
 
   auto dag = DAG(highestPhysicalQubit + 1);
 
   for (auto& it : qc.ops) {
     if (!it->isStandardOperation()) {
       addNonStandardOperationToDag(dag, &it);
@@ -122,17 +123,15 @@
 
   removeIdentities(qc);
 }
 
 DAG CircuitOptimizer::constructDAG(QuantumComputation& qc) {
   Qubit highestPhysicalQubit = 0;
   for (const auto& q : qc.initialLayout) {
-    if (q.first > highestPhysicalQubit) {
-      highestPhysicalQubit = q.first;
-    }
+    highestPhysicalQubit = std::max(q.first, highestPhysicalQubit);
   }
 
   auto dag = DAG(highestPhysicalQubit + 1);
 
   for (auto& it : qc.ops) {
     if (!it->isStandardOperation()) {
       addNonStandardOperationToDag(dag, &it);
@@ -153,18 +152,17 @@
 }
 
 void CircuitOptimizer::addNonStandardOperationToDag(
     DAG& dag, std::unique_ptr<Operation>* op) {
   const auto& gate = *op;
   // compound operations are added "as-is"
   if (gate->isCompoundOperation()) {
-    for (std::size_t i = 0U; i < gate->getNqubits(); ++i) {
-      if (gate->actsOn(static_cast<Qubit>(i))) {
-        dag.at(i).push_back(op);
-      }
+    const auto usedQubits = gate->getUsedQubits();
+    for (const auto q : usedQubits) {
+      dag.at(q).push_back(op);
     }
   } else if (gate->isNonUnitaryOperation()) {
     for (const auto& b : gate->getTargets()) {
       dag.at(b).push_back(op);
     }
   } else if (gate->isClassicControlledOperation()) {
     auto* cop =
@@ -185,17 +183,15 @@
       {qc::I, qc::I},     {qc::X, qc::X},     {qc::Y, qc::Y},
       {qc::Z, qc::Z},     {qc::H, qc::H},     {qc::S, qc::Sdg},
       {qc::Sdg, qc::S},   {qc::T, qc::Tdg},   {qc::Tdg, qc::T},
       {qc::SX, qc::SXdg}, {qc::SXdg, qc::SX}, {qc::Barrier, qc::Barrier}};
 
   Qubit highestPhysicalQubit = 0;
   for (const auto& q : qc.initialLayout) {
-    if (q.first > highestPhysicalQubit) {
-      highestPhysicalQubit = q.first;
-    }
+    highestPhysicalQubit = std::max(q.first, highestPhysicalQubit);
   }
 
   auto dag = DAG(highestPhysicalQubit + 1);
 
   for (auto& it : qc.ops) {
     if (!it->isStandardOperation()) {
       addNonStandardOperationToDag(dag, &it);
@@ -256,37 +252,34 @@
       // check if current operation is the inverse of the previous operation
       if (inverseIt != INVERSE_MAP.end() &&
           it->getType() == inverseIt->second) {
         compop->pop_back();
         it->setGate(qc::I);
       } else {
         compop->emplace_back<StandardOperation>(
-            it->getNqubits(), it->getTargets().at(0), it->getType(),
-            it->getParameter());
+            it->getTargets().at(0), it->getType(), it->getParameter());
         it->setGate(I);
       }
 
       continue;
     }
 
     // single qubit op
 
     // check if current operation is the inverse of the previous operation
     auto inverseIt = INVERSE_MAP.find((*op)->getType());
     if (inverseIt != INVERSE_MAP.end() && it->getType() == inverseIt->second) {
       (*op)->setGate(qc::I);
       it->setGate(qc::I);
     } else {
-      auto compop = std::make_unique<CompoundOperation>(it->getNqubits());
+      auto compop = std::make_unique<CompoundOperation>();
       compop->emplace_back<StandardOperation>(
-          (*op)->getNqubits(), (*op)->getTargets().at(0), (*op)->getType(),
-          (*op)->getParameter());
+          (*op)->getTargets().at(0), (*op)->getType(), (*op)->getParameter());
       compop->emplace_back<StandardOperation>(
-          it->getNqubits(), it->getTargets().at(0), it->getType(),
-          it->getParameter());
+          it->getTargets().at(0), it->getType(), it->getParameter());
       it->setGate(I);
       (*op) = std::move(compop);
       dag.at(target).push_back(op);
     }
   }
 
   removeIdentities(qc);
@@ -597,69 +590,59 @@
                                      bool isDirectedArchitecture) {
   // decompose SWAPS in three cnot and optionally in four H
   auto it = qc.ops.begin();
   while (it != qc.ops.end()) {
     if ((*it)->isStandardOperation()) {
       if ((*it)->getType() == qc::SWAP) {
         const auto targets = (*it)->getTargets();
-        const auto nqubits = (*it)->getNqubits();
         it = qc.ops.erase(it);
-        it = qc.ops.insert(
-            it, std::make_unique<StandardOperation>(
-                    nqubits, Control{targets[0]}, targets[1], qc::X));
+        it = qc.ops.insert(it, std::make_unique<StandardOperation>(
+                                   Control{targets[0]}, targets[1], qc::X));
         if (isDirectedArchitecture) {
-          it = qc.ops.insert(it, std::make_unique<StandardOperation>(
-                                     nqubits, targets[0], qc::H));
-          it = qc.ops.insert(it, std::make_unique<StandardOperation>(
-                                     nqubits, targets[1], qc::H));
           it = qc.ops.insert(
-              it, std::make_unique<StandardOperation>(
-                      nqubits, Control{targets[0]}, targets[1], qc::X));
-          it = qc.ops.insert(it, std::make_unique<StandardOperation>(
-                                     nqubits, targets[0], qc::H));
+              it, std::make_unique<StandardOperation>(targets[0], qc::H));
+          it = qc.ops.insert(
+              it, std::make_unique<StandardOperation>(targets[1], qc::H));
           it = qc.ops.insert(it, std::make_unique<StandardOperation>(
-                                     nqubits, targets[1], qc::H));
-        } else {
+                                     Control{targets[0]}, targets[1], qc::X));
+          it = qc.ops.insert(
+              it, std::make_unique<StandardOperation>(targets[0], qc::H));
           it = qc.ops.insert(
-              it, std::make_unique<StandardOperation>(
-                      nqubits, Control{targets[1]}, targets[0], qc::X));
+              it, std::make_unique<StandardOperation>(targets[1], qc::H));
+        } else {
+          it = qc.ops.insert(it, std::make_unique<StandardOperation>(
+                                     Control{targets[1]}, targets[0], qc::X));
         }
-        it = qc.ops.insert(
-            it, std::make_unique<StandardOperation>(
-                    nqubits, Control{targets[0]}, targets[1], qc::X));
+        it = qc.ops.insert(it, std::make_unique<StandardOperation>(
+                                   Control{targets[0]}, targets[1], qc::X));
       } else {
         ++it;
       }
     } else if ((*it)->isCompoundOperation()) {
       auto* compOp = dynamic_cast<qc::CompoundOperation*>((*it).get());
       auto cit = compOp->begin();
       while (cit != compOp->end()) {
         if ((*cit)->isStandardOperation() && (*cit)->getType() == qc::SWAP) {
           const auto targets = (*cit)->getTargets();
-          const auto nqubits = compOp->getNqubits();
           cit = compOp->erase(cit);
-          cit = compOp->insert<StandardOperation>(
-              cit, nqubits, Control{targets[0]}, targets[1], qc::X);
+          cit = compOp->insert<StandardOperation>(cit, Control{targets[0]},
+                                                  targets[1], qc::X);
           if (isDirectedArchitecture) {
-            cit = compOp->insert<StandardOperation>(cit, nqubits, targets[0],
-                                                    qc::H);
-            cit = compOp->insert<StandardOperation>(cit, nqubits, targets[1],
-                                                    qc::H);
-            cit = compOp->insert<StandardOperation>(
-                cit, nqubits, Control{targets[0]}, targets[1], qc::X);
-            cit = compOp->insert<StandardOperation>(cit, nqubits, targets[0],
-                                                    qc::H);
-            cit = compOp->insert<StandardOperation>(cit, nqubits, targets[1],
-                                                    qc::H);
+            cit = compOp->insert<StandardOperation>(cit, targets[0], qc::H);
+            cit = compOp->insert<StandardOperation>(cit, targets[1], qc::H);
+            cit = compOp->insert<StandardOperation>(cit, Control{targets[0]},
+                                                    targets[1], qc::X);
+            cit = compOp->insert<StandardOperation>(cit, targets[0], qc::H);
+            cit = compOp->insert<StandardOperation>(cit, targets[1], qc::H);
           } else {
-            cit = compOp->insert<StandardOperation>(
-                cit, nqubits, Control{targets[1]}, targets[0], qc::X);
+            cit = compOp->insert<StandardOperation>(cit, Control{targets[1]},
+                                                    targets[0], qc::X);
           }
-          cit = compOp->insert<StandardOperation>(
-              cit, nqubits, Control{targets[0]}, targets[1], qc::X);
+          cit = compOp->insert<StandardOperation>(cit, Control{targets[0]},
+                                                  targets[1], qc::X);
         } else {
           ++cit;
         }
       }
       ++it;
     } else {
       ++it;
@@ -736,21 +719,14 @@
         changeTargets(targets, replacementMap);
       }
       it++;
     } else {
       it++;
     }
   }
-  // if anything has been modified the number of qubits of each gate has to be
-  // adjusted
-  if (!replacementMap.empty()) {
-    for (auto& op : qc.ops) {
-      op->setNqubits(qc.getNqubits());
-    }
-  }
 }
 
 void CircuitOptimizer::changeTargets(
     Targets& targets, const std::map<Qubit, Qubit>& replacementMap) {
   for (auto& target : targets) {
     auto newTargetIt = replacementMap.find(target);
     if (newTargetIt != replacementMap.end()) {
@@ -872,23 +848,21 @@
             // get the underlying operation
             const auto* standardOp =
                 dynamic_cast<qc::StandardOperation*>(classicOp->getOperation());
             if (standardOp == nullptr) {
               std::stringstream ss{};
               ss << "Underlying operation of classic-controlled operation is "
                     "not a StandardOperation.\n";
-              classicOp->print(ss);
+              classicOp->print(ss, qc.nqubits);
               throw QFRException(ss.str());
             }
 
             // get all the necessary information for reconstructing the
             // operation
-            const auto nqubits = standardOp->getNqubits();
             const auto type = standardOp->getType();
-
             const auto targs = standardOp->getTargets();
             for (const auto& target : targs) {
               if (target == measurementQubit) {
                 throw qc::QFRException(
                     "Implicit reset operation in circuit detected. Measuring a "
                     "qubit and then targeting the same qubit with a "
                     "classic-controlled operation is not allowed at the "
@@ -921,18 +895,17 @@
             }
             if (insertionPointInvalidated) {
               currentInsertionPoint = opIt;
             }
 
             itInvalidated = (it >= currentInsertionPoint);
             // insert the new operation (invalidated all pointer onwards)
-            currentInsertionPoint =
-                qc.insert(currentInsertionPoint,
-                          std::make_unique<qc::StandardOperation>(
-                              nqubits, controls, targs, type, parameters));
+            currentInsertionPoint = qc.insert(
+                currentInsertionPoint, std::make_unique<qc::StandardOperation>(
+                                           controls, targs, type, parameters));
 
             if (itInvalidated) {
               it = currentInsertionPoint;
             }
             // advance just after the currently inserted operation
             ++currentInsertionPoint;
             // the inner loop also has to restart from here due to the
@@ -1198,17 +1171,15 @@
   std::advance(it, -movedOperations);
   return it;
 }
 
 void CircuitOptimizer::cancelCNOTs(QuantumComputation& qc) {
   Qubit highestPhysicalQubit = 0;
   for (const auto& q : qc.initialLayout) {
-    if (q.first > highestPhysicalQubit) {
-      highestPhysicalQubit = q.first;
-    }
+    highestPhysicalQubit = std::max(q.first, highestPhysicalQubit);
   }
 
   auto dag = DAG(highestPhysicalQubit + 1U);
 
   for (auto& it : qc.ops) {
     if (!it->isStandardOperation()) {
       addNonStandardOperationToDag(dag, &it);
@@ -1371,26 +1342,23 @@
     std::vector<std::unique_ptr<Operation>>& ops) {
   for (auto it = ops.begin(); it != ops.end(); ++it) {
     auto& op = *it;
     if (op->getType() == qc::X && op->getNcontrols() > 0) {
       const auto& controls = op->getControls();
       assert(op->getNtargets() == 1U);
       const auto target = op->getTargets()[0];
-      const auto nqubits = op->getNqubits();
 
       // -c-    ---c---
       //  |  =     |
       // -X-    -H-Z-H-
       std::array<std::unique_ptr<Operation>, 3U> replacementOps{};
-      replacementOps[0] =
-          std::make_unique<StandardOperation>(nqubits, target, H);
+      replacementOps[0] = std::make_unique<StandardOperation>(target, H);
       replacementOps[1] =
-          std::make_unique<StandardOperation>(nqubits, controls, target, Z);
-      replacementOps[2] =
-          std::make_unique<StandardOperation>(nqubits, target, H);
+          std::make_unique<StandardOperation>(controls, target, Z);
+      replacementOps[2] = std::make_unique<StandardOperation>(target, H);
 
       it = ops.insert(it, std::make_move_iterator(replacementOps.begin()),
                       std::make_move_iterator(replacementOps.end()));
 
       // advance to the original operation and delete it
       std::advance(it, 3);
       it = ops.erase(it);
@@ -1506,8 +1474,256 @@
         continue;
       }
 
       // case 4: nothing to do
     }
   }
 }
+
+/**
+ * @brief Disjoint Set Union data structure for qubits
+ *
+ * This data structure is used to maintain a relationship between qubits and
+ * blocks they belong to. The blocks are formed by operations that act on the
+ * same qubits.
+ */
+struct DSU {
+  std::unordered_map<Qubit, Qubit> parent;
+  std::unordered_map<Qubit, std::vector<Qubit>> bitBlocks;
+  std::unordered_map<Qubit, std::vector<QuantumComputation::iterator>>
+      gateBlocks;
+  std::size_t maxBlockSize = 0;
+
+  /**
+   * @brief Find the block that a qubit belongs to.
+   * @param index Qubit to find the block for
+   * @return The block that the qubit belongs to
+   */
+  Qubit findBlock(const Qubit index) {
+    if (parent.find(index) == parent.end()) {
+      parent[index] = index;
+      bitBlocks[index] = {index};
+      gateBlocks[index] = {};
+    }
+    if (parent[index] == index) {
+      return index;
+    }
+    parent[index] = findBlock(parent[index]);
+    return parent[index];
+  }
+
+  void unionBlock(Qubit block1, Qubit block2) {
+    auto parent1 = findBlock(block1);
+    auto parent2 = findBlock(block2);
+    if (parent1 == parent2) {
+      return;
+    }
+    if (gateBlocks[parent1].size() < gateBlocks[parent2].size()) {
+      std::swap(parent1, parent2);
+    }
+    parent[parent2] = parent1;
+    gateBlocks[parent1].insert(gateBlocks[parent1].end(),
+                               gateBlocks[parent2].begin(),
+                               gateBlocks[parent2].end());
+    bitBlocks[parent1].insert(bitBlocks[parent1].end(),
+                              bitBlocks[parent2].begin(),
+                              bitBlocks[parent2].end());
+    gateBlocks[parent2].clear();
+    bitBlocks[parent2].clear();
+  }
+};
+
+void CircuitOptimizer::collectBlocks(qc::QuantumComputation& qc,
+                                     const std::size_t maxBlockSize) {
+  if (qc.ops.size() <= 1) {
+    return;
+  }
+
+  // ensure canonical ordering and that measurements are as far back as possible
+  reorderOperations(qc);
+  deferMeasurements(qc);
+
+  // create an empty disjoint set union data structure
+  DSU dsu{};
+
+  // create a list for the gate blocks
+  std::vector<std::vector<QuantumComputation::iterator>> blockList{};
+
+  for (auto opIt = qc.begin(); opIt != qc.end(); ++opIt) {
+    auto& op = *opIt;
+    bool canProcess = true;
+    bool makesTooBig = false;
+
+    // check if the operation can be processed
+    if (!op->isUnitary()) {
+      canProcess = false;
+    }
+
+    const auto usedQubits = op->getUsedQubits();
+
+    if (canProcess) {
+      // check if grouping the operation with the current block would make the
+      // block too big
+      std::unordered_set<Qubit> blockQubits;
+      for (const auto& q : usedQubits) {
+        blockQubits.emplace(dsu.findBlock(q));
+      }
+      std::size_t totalSize = 0;
+      for (const auto& q : blockQubits) {
+        totalSize += dsu.bitBlocks[q].size();
+      }
+      if (totalSize > maxBlockSize) {
+        makesTooBig = true;
+      }
+    } else {
+      // resolve cases where an operation cannot be processed
+      for (const auto& q : usedQubits) {
+        const auto block = dsu.findBlock(q);
+        if (dsu.gateBlocks[block].empty()) {
+          continue;
+        }
+        blockList.emplace_back(std::move(dsu.gateBlocks[block]));
+        for (auto index : dsu.bitBlocks[block]) {
+          dsu.parent[index] = index;
+          dsu.bitBlocks[index] = {index};
+          dsu.gateBlocks[index] = {};
+        }
+      }
+    }
+
+    if (makesTooBig) {
+      // if the operation acts on more qubits than the maximum block size, all
+      // current blocks need to be finalized.
+      if (usedQubits.size() > maxBlockSize) {
+        // get all of the relevant blocks and check for the best way to combine
+        // them together.
+        std::unordered_map<Qubit, std::size_t> blocksAndSizes{};
+        for (const auto& q : usedQubits) {
+          const auto block = dsu.findBlock(q);
+          if (dsu.gateBlocks[block].empty() ||
+              blocksAndSizes.find(block) != blocksAndSizes.end()) {
+            continue;
+          }
+          blocksAndSizes[block] = dsu.bitBlocks[block].size();
+        }
+        // sort blocks in descending order
+        std::vector<std::pair<Qubit, std::size_t>> sortedBlocks(
+            blocksAndSizes.begin(), blocksAndSizes.end());
+        std::sort(
+            sortedBlocks.begin(), sortedBlocks.end(),
+            [](const auto& a, const auto& b) { return a.second > b.second; });
+        for (auto it = sortedBlocks.begin(); it != sortedBlocks.end(); ++it) {
+          auto& [block, size] = *it;
+          // maximally large block -> nothing to do
+          if (size == maxBlockSize) {
+            blockList.emplace_back(std::move(dsu.gateBlocks[block]));
+            for (auto index : dsu.bitBlocks[block]) {
+              dsu.parent[index] = index;
+              dsu.bitBlocks[index] = {index};
+              dsu.gateBlocks[index] = {};
+            }
+          }
+
+          // fill up with as many blocks as possible
+          auto nextIt = it + 1;
+          while (nextIt != sortedBlocks.end() && size < maxBlockSize) {
+            auto& [nextBlock, nextSize] = *nextIt;
+            if (size + nextSize <= maxBlockSize) {
+              dsu.unionBlock(block, nextBlock);
+              size += nextSize;
+              nextIt = sortedBlocks.erase(nextIt);
+            } else {
+              ++nextIt;
+            }
+          }
+
+          // just to be on the safe side, get the block again
+          block = dsu.findBlock(block);
+          if (!dsu.gateBlocks[block].empty()) {
+            blockList.emplace_back(std::move(dsu.gateBlocks[block]));
+          }
+          for (auto index : dsu.bitBlocks[block]) {
+            dsu.parent[index] = index;
+            dsu.bitBlocks[index] = {index};
+            dsu.gateBlocks[index] = {};
+          }
+        }
+      } else {
+        // otherwise, finalize blocks that would free up enough space.
+        // prioritize blocks that would free up the most space.
+        std::unordered_map<Qubit, std::size_t> savings{};
+        std::size_t totalSize = 0U;
+        for (const auto& q : usedQubits) {
+          const auto block = dsu.findBlock(q);
+          if (savings.find(block) != savings.end()) {
+            savings[block] -= 1;
+          } else {
+            savings[block] = dsu.bitBlocks[block].size() - 1;
+            totalSize += dsu.bitBlocks[block].size();
+          }
+        }
+        // sort savings in descending order
+        std::vector<std::pair<Qubit, std::size_t>> sortedSavings(
+            savings.begin(), savings.end());
+        std::sort(
+            sortedSavings.begin(), sortedSavings.end(),
+            [](const auto& a, const auto& b) { return a.second > b.second; });
+        auto savingsNeed = static_cast<std::int64_t>(totalSize - maxBlockSize);
+        for (const auto& [index, saving] : sortedSavings) {
+          if (savingsNeed > 0) {
+            savingsNeed -= static_cast<std::int64_t>(saving);
+            if (!dsu.gateBlocks[index].empty()) {
+              blockList.emplace_back(std::move(dsu.gateBlocks[index]));
+            }
+            for (auto j : dsu.bitBlocks[index]) {
+              dsu.parent[j] = j;
+              dsu.bitBlocks[j] = {j};
+              dsu.gateBlocks[j] = {};
+            }
+          }
+        }
+      }
+    }
+
+    if (canProcess) {
+      if (usedQubits.size() > maxBlockSize) {
+        continue;
+      }
+      std::int64_t prev = -1;
+      for (const auto& q : usedQubits) {
+        if (prev != -1) {
+          dsu.unionBlock(static_cast<Qubit>(prev), q);
+        }
+        prev = q;
+      }
+      dsu.gateBlocks[dsu.findBlock(static_cast<Qubit>(prev))].emplace_back(
+          opIt);
+    }
+  }
+
+  // convert remaining blocks to blockList
+  for (const auto& [q, index] : dsu.parent) {
+    if (q == index && !dsu.gateBlocks[q].empty()) {
+      blockList.emplace_back(std::move(dsu.gateBlocks[q]));
+    }
+  }
+
+  // Iterate over the blocks in reverse order and replace the first operation in
+  // each block with a compound operation containing all operations in the
+  // block. Then remove the remaining operations in the block.
+  for (auto it = blockList.rbegin(); it != blockList.rend(); ++it) {
+    auto& block = *it;
+    if (block.size() == 1U) {
+      continue;
+    }
+    std::vector<std::unique_ptr<Operation>> ops{};
+    ops.reserve(block.size());
+    for (auto& op : block) {
+      ops.emplace_back(std::move(*op));
+      *op = std::make_unique<StandardOperation>(0, I);
+    }
+    *block.front() = std::make_unique<CompoundOperation>(std::move(ops));
+  }
+
+  removeIdentities(qc);
+}
 } // namespace qc
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/QuantumComputation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/QuantumComputation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -242,19 +242,14 @@
 
   for (std::size_t i = 0; i < nq; ++i) {
     auto j = static_cast<Qubit>(nqubits + i);
     initialLayout.insert({j, j});
     outputPermutation.insert({j, j});
   }
   nqubits += nq;
-
-  for (auto& op : ops) {
-    op->setNqubits(nqubits + nancillae);
-  }
-
   ancillary.resize(nqubits + nancillae);
   garbage.resize(nqubits + nancillae);
 }
 
 void QuantumComputation::addClassicalRegister(std::size_t nc,
                                               const std::string& regName) {
   if (cregs.count(regName) != 0) {
@@ -291,18 +286,14 @@
   for (std::size_t i = 0; i < nq; ++i) {
     auto j = static_cast<Qubit>(totalqubits + i);
     initialLayout.insert({j, j});
     outputPermutation.insert({j, j});
     ancillary[j] = true;
   }
   nancillae += nq;
-
-  for (auto& op : ops) {
-    op->setNqubits(nqubits + nancillae);
-  }
 }
 
 void QuantumComputation::removeQubitfromQubitRegister(QuantumRegisterMap& regs,
                                                       const std::string& reg,
                                                       const Qubit idx) {
   if (idx == 0) {
     // last remaining qubit of register
@@ -399,21 +390,16 @@
   if (const auto it = outputPermutation.find(physicalQubitIndex);
       it != outputPermutation.end()) {
     outputQubitIndex = it->second;
     // erasing entry
     outputPermutation.erase(physicalQubitIndex);
   }
 
-  // update all operations
-  const auto totalQubits = nqubits + nancillae;
-  for (auto& op : ops) {
-    op->setNqubits(totalQubits);
-  }
-
   // update ancillary and garbage tracking
+  const auto totalQubits = nqubits + nancillae;
   for (std::size_t i = logicalQubitIndex; i < totalQubits; ++i) {
     ancillary[i] = ancillary[i + 1];
     garbage[i] = garbage[i + 1];
   }
   // unset last entry
   ancillary[totalQubits] = false;
   garbage[totalQubits] = false;
@@ -451,19 +437,14 @@
   // adjust output permutation
   if (outputQubitIndex.has_value()) {
     outputPermutation.insert({physicalQubitIndex, *outputQubitIndex});
   } else {
     // if a qubit is not relevant for the output, it is considered garbage
     garbage[logicalQubitIndex] = true;
   }
-
-  // update all operations
-  for (auto& op : ops) {
-    op->setNqubits(nqubits + nancillae);
-  }
 }
 
 void QuantumComputation::addQubit(const Qubit logicalQubitIndex,
                                   const Qubit physicalQubitIndex,
                                   const std::optional<Qubit> outputQubitIndex) {
   if (initialLayout.count(physicalQubitIndex) > 0 ||
       outputPermutation.count(physicalQubitIndex) > 0) {
@@ -487,22 +468,16 @@
   // adjust initial layout
   initialLayout.insert({physicalQubitIndex, logicalQubitIndex});
   if (outputQubitIndex.has_value()) {
     // adjust output permutation
     outputPermutation.insert({physicalQubitIndex, *outputQubitIndex});
   }
 
-  const auto totalQubits = nqubits + nancillae;
-
-  // update all operations
-  for (auto& op : ops) {
-    op->setNqubits(totalQubits);
-  }
-
   // update ancillary and garbage tracking
+  const auto totalQubits = nqubits + nancillae;
   ancillary.resize(totalQubits);
   garbage.resize(totalQubits);
   for (auto i = totalQubits - 1; i > logicalQubitIndex; --i) {
     ancillary[i] = ancillary[i - 1];
     garbage[i] = garbage[i - 1];
   }
   // unset new entry
@@ -523,24 +498,23 @@
     os << std::setw(4) << logical << "\033[0m";
   }
   os << "\n";
 
   size_t i = 0U;
   for (const auto& op : ops) {
     os << std::setw(width) << ++i << ":";
-    op->print(os, {}, static_cast<std::size_t>(width) + 1U);
+    op->print(os, {}, static_cast<std::size_t>(width) + 1U, nqubits);
     os << "\n";
   }
 
   os << std::setw(width + 1) << "o:";
   for (const auto& physicalQubit : initialLayout) {
     auto it = outputPermutation.find(physicalQubit.first);
     if (it == outputPermutation.end()) {
-      os << "\033[31m" << std::setw(4) << "|"
-         << "\033[0m";
+      os << "\033[31m" << std::setw(4) << "|" << "\033[0m";
     } else {
       os << std::setw(4) << it->second;
     }
   }
   os << "\n";
   return os;
 }
@@ -894,27 +868,41 @@
   }
 
   nqubits--;
   nancillae++;
   ancillary[logicalQubitIndex] = true;
 }
 
+void QuantumComputation::setLogicalQubitsAncillary(
+    const Qubit minLogicalQubitIndex, const Qubit maxLogicalQubitIndex) {
+  for (Qubit i = minLogicalQubitIndex; i <= maxLogicalQubitIndex; i++) {
+    setLogicalQubitAncillary(i);
+  }
+}
+
 void QuantumComputation::setLogicalQubitGarbage(const Qubit logicalQubitIndex) {
   garbage[logicalQubitIndex] = true;
   // setting a logical qubit garbage also means removing it from the output
   // permutation if it was present before
   for (auto it = outputPermutation.begin(); it != outputPermutation.end();
        ++it) {
     if (it->second == logicalQubitIndex) {
       outputPermutation.erase(it);
       break;
     }
   }
 }
 
+void QuantumComputation::setLogicalQubitsGarbage(
+    const Qubit minLogicalQubitIndex, const Qubit maxLogicalQubitIndex) {
+  for (Qubit i = minLogicalQubitIndex; i <= maxLogicalQubitIndex; i++) {
+    setLogicalQubitGarbage(i);
+  }
+}
+
 [[nodiscard]] std::pair<bool, std::optional<Qubit>>
 QuantumComputation::containsLogicalQubit(const Qubit logicalQubitIndex) const {
   if (const auto it = std::find_if(initialLayout.cbegin(), initialLayout.cend(),
                                    [&logicalQubitIndex](const auto& mapping) {
                                      return mapping.second == logicalQubitIndex;
                                    });
       it != initialLayout.cend()) {
@@ -1078,16 +1066,16 @@
     if (registerBit.second >= cRegister->second.second) {
       std::stringstream ss{};
       ss << "The classical register \"" << registerBit.first
          << "\" is too small! (" << registerBit.second
          << " >= " << cRegister->second.second << ")";
       throw QFRException(ss.str());
     }
-    emplace_back<NonUnitaryOperation>(
-        getNqubits(), qubit, cRegister->second.first + registerBit.second);
+    emplace_back<NonUnitaryOperation>(qubit, cRegister->second.first +
+                                                 registerBit.second);
 
   } else {
     std::stringstream ss{};
     ss << "The classical register \"" << registerBit.first
        << "\" does not exist!";
     throw QFRException(ss.str());
   }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/BernsteinVazirani.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/BernsteinVazirani.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 
 std::ostream& BernsteinVazirani::printStatistics(std::ostream& os) const {
   os << "BernsteinVazirani (" << bitwidth << ") Statistics:\n";
   os << "\tn: " << bitwidth + 1 << "\n";
   os << "\tm: " << getNindividualOps() << "\n";
   os << "\ts: " << expected << "\n";
   os << "\tdynamic: " << dynamic << "\n";
-  os << "--------------"
-     << "\n";
+  os << "--------------" << "\n";
   return os;
 }
 
 void BernsteinVazirani::createCircuit() {
   expected = s.to_string();
   std::reverse(expected.begin(), expected.end());
   while (expected.length() > bitwidth) {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/GoogleRandomCircuitSampling.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/GoogleRandomCircuitSampling.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -82,36 +82,35 @@
     }
 
     ss >> identifier;
     if (identifier == "cz") {
       ss >> control;
       ss >> target;
       cycles[cycle].emplace_back(std::make_unique<StandardOperation>(
-          nqubits, Control{static_cast<Qubit>(control)},
-          static_cast<Qubit>(target), Z));
+          Control{static_cast<Qubit>(control)}, static_cast<Qubit>(target), Z));
     } else if (identifier == "is") {
       ss >> control;
       ss >> target;
       cycles[cycle].emplace_back(std::make_unique<StandardOperation>(
-          nqubits, qc::Controls{}, static_cast<Qubit>(control),
+          qc::Controls{}, static_cast<Qubit>(control),
           static_cast<Qubit>(target), iSWAP));
     } else {
       ss >> target;
       if (identifier == "h") {
-        cycles[cycle].emplace_back(std::make_unique<StandardOperation>(
-            nqubits, static_cast<Qubit>(target), H));
+        cycles[cycle].emplace_back(
+            std::make_unique<StandardOperation>(static_cast<Qubit>(target), H));
       } else if (identifier == "t") {
-        cycles[cycle].emplace_back(std::make_unique<StandardOperation>(
-            nqubits, static_cast<Qubit>(target), T));
+        cycles[cycle].emplace_back(
+            std::make_unique<StandardOperation>(static_cast<Qubit>(target), T));
       } else if (identifier == "x_1_2") {
         cycles[cycle].emplace_back(std::make_unique<StandardOperation>(
-            nqubits, static_cast<Qubit>(target), RX, std::vector{PI_2}));
+            static_cast<Qubit>(target), RX, std::vector{PI_2}));
       } else if (identifier == "y_1_2") {
         cycles[cycle].emplace_back(std::make_unique<StandardOperation>(
-            nqubits, static_cast<Qubit>(target), RY, std::vector{PI_2}));
+            static_cast<Qubit>(target), RY, std::vector{PI_2}));
       } else {
         throw QFRException("Unknown gate '" + identifier);
       }
     }
   }
 }
 
@@ -127,28 +126,26 @@
   std::size_t i = 0;
   std::size_t j = 0;
   for (const auto& cycle : cycles) {
     os << "Cycle " << i++ << ":\n";
     for (const auto& op : cycle) {
       os << std::setw(static_cast<int>(std::log10(getNops()) + 1.)) << ++j
          << ": ";
-      op->print(os, initialLayout, 0U);
+      op->print(os, initialLayout, 0U, nqubits);
       os << "\n";
     }
   }
   return os;
 }
 
 std::ostream&
 GoogleRandomCircuitSampling::printStatistics(std::ostream& os) const {
   os << "GoogleRandomCircuitSampling Statistics:\n";
   os << "\tLayout: "
      << ((layout == Rectangular) ? "Rectangular" : "Bristlecone") << "\n";
   os << "\tn: " << static_cast<std::size_t>(nqubits) << "\n";
   os << "\tm: " << getNops() << "\n";
-  os << "\tc: 1 + " << cycles.size() - 2 << " + 1"
-     << "\n";
-  os << "--------------"
-     << "\n";
+  os << "\tc: 1 + " << cycles.size() - 2 << " + 1" << "\n";
+  os << "--------------" << "\n";
   return os;
 }
 } // namespace qc
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/Grover.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/Grover.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -106,12 +106,11 @@
 std::ostream& Grover::printStatistics(std::ostream& os) const {
   os << "Grover (" << nqubits - 1 << ") Statistics:\n";
   os << "\tn: " << nqubits << "\n";
   os << "\tm: " << getNindividualOps() << "\n";
   os << "\tseed: " << seed << "\n";
   os << "\tx: " << expected << "\n";
   os << "\ti: " << iterations << "\n";
-  os << "--------------"
-     << "\n";
+  os << "--------------" << "\n";
   return os;
 }
 } // namespace qc
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/QFT.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/QFT.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 }
 
 std::ostream& QFT::printStatistics(std::ostream& os) const {
   os << "QFT (" << precision << ") Statistics:\n";
   os << "\tn: " << nqubits << "\n";
   os << "\tm: " << getNindividualOps() << "\n";
   os << "\tdynamic: " << dynamic << "\n";
-  os << "--------------"
-     << "\n";
+  os << "--------------" << "\n";
   return os;
 }
 void QFT::createCircuit() {
   if (dynamic) {
     for (std::size_t i = 0; i < precision; i++) {
       // apply classically controlled phase rotations
       for (std::size_t j = 1; j <= i; ++j) {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/QPE.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/QPE.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -44,20 +44,18 @@
   createCircuit();
 }
 
 std::ostream& QPE::printStatistics(std::ostream& os) const {
   os << "QPE Statistics:\n";
   os << "\tn: " << nqubits + 1 << "\n";
   os << "\tm: " << getNindividualOps() << "\n";
-  os << "\tlambda: " << lambda << "π"
-     << "\n";
+  os << "\tlambda: " << lambda << "π" << "\n";
   os << "\tprecision: " << precision << "\n";
   os << "\titerative: " << iterative << "\n";
-  os << "--------------"
-     << "\n";
+  os << "--------------" << "\n";
   return os;
 }
 
 void QPE::createCircuit() {
   addQubitRegister(1, "psi");
 
   if (iterative) {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/RandomCliffordCircuit.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/RandomCliffordCircuit.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,15 @@
 
 std::ostream& RandomCliffordCircuit::printStatistics(std::ostream& os) const {
   os << "Random Clifford circuit statistics:\n";
   os << "\tn: " << nqubits << "\n";
   os << "\tm: " << getNindividualOps() << "\n";
   os << "\tdepth: " << depth << "\n";
   os << "\tseed: " << seed << "\n";
-  os << "--------------"
-     << "\n";
+  os << "--------------" << "\n";
   return os;
 }
 
 void RandomCliffordCircuit::append1QClifford(const std::uint16_t idx,
                                              const Qubit target) {
   const auto id = static_cast<std::uint8_t>(idx % 24);
   auto qc = QuantumComputation(nqubits);
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/algorithms/WState.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/algorithms/WState.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/Benchmark.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/Benchmark.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/CMakeLists.txt` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/CachedEdge.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/CachedEdge.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/Complex.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/Complex.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/ComplexNumbers.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/ComplexNumbers.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/ComplexValue.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/ComplexValue.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/Edge.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/Edge.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -22,39 +22,52 @@
 
 ///-----------------------------------------------------------------------------
 ///                      \n General purpose methods \n
 ///-----------------------------------------------------------------------------
 
 template <class Node>
 std::complex<fp>
-Edge<Node>::getValueByPath(const std::string& decisions) const {
+Edge<Node>::getValueByPath(const std::size_t numQubits,
+                           const std::string& decisions) const {
+  auto c = static_cast<std::complex<fp>>(w);
   if (isTerminal()) {
-    return static_cast<std::complex<fp>>(w);
+    return c;
   }
 
-  auto c = std::complex<fp>{1.0, 0.0};
   auto r = *this;
   if constexpr (std::is_same_v<Node, dNode>) {
     Edge<dNode>::applyDmChangesToEdge(r);
   }
-  while (!r.isTerminal()) {
-    c *= static_cast<std::complex<fp>>(r.w);
-    const auto tmp = static_cast<std::size_t>(decisions.at(r.p->v) - '0');
-    assert(tmp <= r.p->e.size());
 
+  auto level = numQubits;
+  while (level > 0U) {
+    const auto tmp = static_cast<std::size_t>(decisions.at(level - 1U) - '0');
+
+    // node is not at the expected level (skipped node)
+    if (r.isTerminal() || r.p->v != level - 1U) {
+      if (r.isZeroTerminal() || tmp == 1U || tmp == 2U) {
+        return 0.;
+      }
+      --level;
+      continue;
+    }
+
+    // node is at the expected level
+    assert(tmp <= r.p->e.size());
     if constexpr (std::is_same_v<Node, dNode>) {
       auto e = r;
       Edge<dNode>::applyDmChangesToEdge(r.p->e[tmp]);
       r = r.p->e[tmp];
       Edge<dNode>::revertDmChangesToEdge(e);
     } else {
       r = r.p->e[tmp];
     }
+    c *= static_cast<std::complex<fp>>(r.w);
+    --level;
   }
-  c *= static_cast<std::complex<fp>>(r.w);
   return c;
 }
 
 template <class Node> std::size_t Edge<Node>::size() const {
   static constexpr std::size_t NODECOUNT_BUCKETS = 200000U;
   static std::unordered_set<const Node*> visited{NODECOUNT_BUCKETS};
   visited.max_load_factor(10);
@@ -146,26 +159,28 @@
 
   return r;
 }
 
 template <class Node>
 template <typename T, isVector<T>>
 std::complex<fp> Edge<Node>::getValueByIndex(const std::size_t i) const {
-  if (isTerminal()) {
-    return static_cast<std::complex<fp>>(w);
+  auto bitwidth = static_cast<Qubit>(std::log2(i + 1U));
+
+  if (!isTerminal()) {
+    bitwidth = std::max(bitwidth, static_cast<Qubit>(p->v + 1U));
   }
 
-  auto decisions = std::string(p->v + 1U, '0');
-  for (auto j = 0U; j <= p->v; ++j) {
+  auto decisions = std::string(bitwidth, '0');
+  for (auto j = 0U; j < bitwidth; ++j) {
     if ((i & (1ULL << j)) != 0U) {
       decisions[j] = '1';
     }
   }
 
-  return getValueByPath(decisions);
+  return getValueByPath(bitwidth, decisions);
 }
 
 template <class Node>
 template <typename T, isVector<T>>
 CVec Edge<Node>::getVector(const fp threshold) const {
   if (isTerminal()) {
     return {static_cast<std::complex<fp>>(w)};
@@ -320,229 +335,245 @@
     }
   }
   return Edge<Node>{p, maxVal};
 }
 
 template <class Node>
 template <typename T, isMatrixVariant<T>>
-std::complex<fp> Edge<Node>::getValueByIndex(const std::size_t i,
+std::complex<fp> Edge<Node>::getValueByIndex(const std::size_t numQubits,
+                                             const std::size_t i,
                                              const std::size_t j) const {
   if (isTerminal()) {
     return static_cast<std::complex<fp>>(w);
   }
 
-  auto decisions = std::string(p->v + 1U, '0');
-  for (auto k = 0U; k <= p->v; ++k) {
+  auto decisions = std::string(numQubits, '0');
+  for (auto k = 0U; k < numQubits; ++k) {
     if ((i & (1ULL << k)) != 0U) {
       decisions[k] = '2';
     }
   }
-  for (auto k = 0U; k <= p->v; ++k) {
+  for (auto k = 0U; k < numQubits; ++k) {
     if ((j & (1ULL << k)) != 0U) {
       if (decisions[k] == '2') {
         decisions[k] = '3';
       } else {
         decisions[k] = '1';
       }
     }
   }
 
-  return getValueByPath(decisions);
+  return getValueByPath(numQubits, decisions);
 }
 
 template <class Node>
 template <typename T, isMatrixVariant<T>>
-CMat Edge<Node>::getMatrix(const fp threshold) const {
-  if (isTerminal()) {
+CMat Edge<Node>::getMatrix(const std::size_t numQubits,
+                           const fp threshold) const {
+  if (numQubits == 0U) {
     return CMat{1, {static_cast<std::complex<fp>>(w)}};
   }
 
   auto r = *this;
   if constexpr (std::is_same_v<Node, dNode>) {
     Edge<dNode>::applyDmChangesToEdge(r);
   }
-
-  const std::size_t dim = 2ULL << r.p->v;
-  auto mat = CMat(dim, CVec(dim, 0.0));
-
+  const std::size_t dim = 1ULL << numQubits;
+  auto mat = CMat(dim, CVec(dim, 0.));
   r.traverseMatrix(
       1, 0ULL, 0ULL,
       [&mat](const std::size_t i, const std::size_t j,
              const std::complex<fp>& c) { mat.at(i).at(j) = c; },
-      threshold);
-
+      numQubits, threshold);
   if constexpr (std::is_same_v<Node, dNode>) {
     Edge<dNode>::revertDmChangesToEdge(r);
   }
   return mat;
 }
 
 template <class Node>
 template <typename T, isMatrixVariant<T>>
-SparseCMat Edge<Node>::getSparseMatrix(const fp threshold) const {
-  if (isTerminal()) {
+SparseCMat Edge<Node>::getSparseMatrix(const std::size_t numQubits,
+                                       const fp threshold) const {
+  if (numQubits == 0U) {
     return {{{0U, 0U}, static_cast<std::complex<fp>>(w)}};
   }
 
   auto r = *this;
   if constexpr (std::is_same_v<Node, dNode>) {
     Edge<dNode>::applyDmChangesToEdge(r);
   }
 
   auto mat = SparseCMat{};
   r.traverseMatrix(
       1, 0ULL, 0ULL,
       [&mat](const std::size_t i, const std::size_t j,
-             const std::complex<fp>& c) {
-        mat[{i, j}] = c;
-      },
-      threshold);
+             const std::complex<fp>& c) { mat[{i, j}] = c; },
+      numQubits, threshold);
 
   if constexpr (std::is_same_v<Node, dNode>) {
     Edge<dNode>::revertDmChangesToEdge(r);
   }
 
   return mat;
 }
 
 template <class Node>
 template <typename T, isMatrixVariant<T>>
-void Edge<Node>::printMatrix() const {
+void Edge<Node>::printMatrix(const std::size_t numQubits) const {
   constexpr auto precision = 3;
   const auto oldPrecision = std::cout.precision();
   std::cout << std::setprecision(precision);
 
-  if (isTerminal()) {
+  if (numQubits == 0U) {
     std::cout << static_cast<std::complex<fp>>(w) << "\n";
     return;
   }
 
   auto r = *this;
   if constexpr (std::is_same_v<Node, dNode>) {
     Edge<dNode>::alignDensityEdge(r);
   }
 
-  const std::size_t element = 2ULL << r.p->v;
+  // total number of qubits should not be lower than the highest qubit index
+  assert(r.isTerminal() || numQubits >= r.p->v);
+  const std::size_t element = 1ULL << numQubits;
   for (auto i = 0ULL; i < element; ++i) {
     for (auto j = 0ULL; j < element; ++j) {
-      const auto amplitude = getValueByIndex(i, j);
+      const auto amplitude = getValueByIndex(numQubits, i, j);
       std::cout << amplitude << " ";
     }
     std::cout << "\n";
   }
   std::cout << std::setprecision(static_cast<int>(oldPrecision));
   std::cout << std::flush;
 }
 
 template <class Node>
 template <typename T, isMatrixVariant<T>>
 void Edge<Node>::traverseMatrix(const std::complex<fp>& amp,
                                 const std::size_t i, const std::size_t j,
-                                MatrixEntryFunc f, const fp threshold) const {
+                                MatrixEntryFunc f, const std::size_t level,
+                                const fp threshold) const {
   // calculate new accumulated amplitude
   const auto c = amp * static_cast<std::complex<fp>>(w);
 
   if (std::abs(c) < threshold) {
     return;
   }
 
-  if (isTerminal()) {
+  if (level == 0) {
+    assert(isTerminal());
     f(i, j, c);
     return;
   }
 
-  const std::size_t x = i | (1ULL << p->v);
-  const std::size_t y = j | (1ULL << p->v);
+  const auto nextLevel = static_cast<Qubit>(level - 1U);
+  const std::size_t x = i | (1ULL << nextLevel);
+  const std::size_t y = j | (1ULL << nextLevel);
+  if (isTerminal() || p->v < nextLevel) {
+    traverseMatrix(c, i, j, f, nextLevel, threshold);
+    traverseMatrix(c, x, y, f, nextLevel, threshold);
+    return;
+  }
+
   const auto coords = {std::pair{i, j}, {i, y}, {x, j}, {x, y}};
   std::size_t k = 0U;
   for (const auto& [a, b] : coords) {
     if (auto& e = p->e[k++]; !e.w.exactlyZero()) {
       if constexpr (std::is_same_v<Node, dNode>) {
         Edge<dNode>::applyDmChangesToEdge(e);
       }
-      e.traverseMatrix(c, a, b, f, threshold);
+      e.traverseMatrix(c, a, b, f, nextLevel, threshold);
       if constexpr (std::is_same_v<Node, dNode>) {
         Edge<dNode>::revertDmChangesToEdge(e);
       }
     }
   }
 }
 
 ///-----------------------------------------------------------------------------
 ///                   \n Methods for density matrix DDs \n
 ///-----------------------------------------------------------------------------
 
 template <class Node>
 template <typename T, isDensityMatrix<T>>
-SparsePVec Edge<Node>::getSparseProbabilityVector(const fp threshold) const {
-  if (isTerminal()) {
+SparsePVec Edge<Node>::getSparseProbabilityVector(const std::size_t numQubits,
+                                                  const fp threshold) const {
+  if (numQubits == 0U) {
     return {{0, static_cast<std::complex<fp>>(w).real()}};
   }
 
   auto e = *this;
   Edge<dNode>::alignDensityEdge(e);
 
   auto probabilities = SparsePVec{};
   e.traverseDiagonal(
       1, 0,
       [&probabilities](const std::size_t i, const fp& prob) {
         probabilities[i] = prob;
       },
-      threshold);
+      numQubits, threshold);
   return probabilities;
 }
 
 template <class Node>
 template <typename T, isDensityMatrix<T>>
 SparsePVecStrKeys
-Edge<Node>::getSparseProbabilityVectorStrKeys(const fp threshold) const {
-  if (isTerminal()) {
+Edge<Node>::getSparseProbabilityVectorStrKeys(const std::size_t numQubits,
+                                              const fp threshold) const {
+  if (numQubits == 0U) {
     return {{"0", static_cast<std::complex<fp>>(w).real()}};
   }
 
   auto e = *this;
   Edge<dNode>::alignDensityEdge(e);
   const auto nqubits = static_cast<std::size_t>(e.p->v) + 1U;
 
   auto probabilities = SparsePVecStrKeys{};
   e.traverseDiagonal(
       1, 0,
       [&probabilities, &nqubits](const std::size_t i, const fp& prob) {
         probabilities[intToBinaryString(i, nqubits)] = prob;
       },
-      threshold);
+      numQubits, threshold);
   return probabilities;
 }
 
 template <class Node>
 template <typename T, isDensityMatrix<T>>
 void Edge<Node>::traverseDiagonal(const fp& prob, const std::size_t i,
-                                  ProbabilityFunc f,
+                                  ProbabilityFunc f, const std::size_t level,
                                   const dd::fp threshold) const {
   // calculate new accumulated probability
   const auto c = static_cast<std::complex<fp>>(w);
-  assert(std::abs(c.imag()) < RealNumber::eps &&
-         "Density matrix diagonal must be real-valued.");
   const auto val = prob * c.real();
 
   if (val < threshold) {
     return;
   }
 
-  if (isTerminal()) {
+  if (level == 0) {
+    assert(isTerminal());
     f(i, val);
     return;
   }
 
-  // recursive case
+  const auto nextLevel = static_cast<Qubit>(level - 1U);
+  if (isTerminal() || p->v < nextLevel) {
+    traverseDiagonal(prob, i, f, nextLevel, threshold);
+    traverseDiagonal(prob, i | (1ULL << nextLevel), f, nextLevel, threshold);
+    return;
+  }
+
   if (auto& e = p->e[0]; !e.w.exactlyZero()) {
-    e.traverseDiagonal(val, i, f, threshold);
+    e.traverseDiagonal(val, i, f, nextLevel, threshold);
   }
   if (auto& e = p->e[3]; !e.w.exactlyZero()) {
-    e.traverseDiagonal(val, i | (1ULL << p->v), f, threshold);
+    e.traverseDiagonal(val, i | (1ULL << nextLevel), f, nextLevel, threshold);
   }
 }
 
 ///-----------------------------------------------------------------------------
 ///                      \n Explicit instantiations \n
 ///-----------------------------------------------------------------------------
 
@@ -565,43 +596,54 @@
                                          const std::size_t i, AmplitudeFunc f,
                                          const fp threshold) const;
 
 template Edge<mNode> Edge<mNode>::normalize<mNode, true>(
     mNode* p, const std::array<Edge<mNode>, NEDGE>& e, MemoryManager<mNode>& mm,
     ComplexNumbers& cn);
 template std::complex<fp>
-Edge<mNode>::getValueByIndex<mNode, true>(const std::size_t i,
+Edge<mNode>::getValueByIndex<mNode, true>(const std::size_t numQubits,
+                                          const std::size_t i,
                                           const std::size_t j) const;
-template CMat Edge<mNode>::getMatrix<mNode, true>(const fp threshold) const;
+template CMat Edge<mNode>::getMatrix<mNode, true>(const std::size_t numQubits,
+                                                  const fp threshold) const;
 template SparseCMat
-Edge<mNode>::getSparseMatrix<mNode, true>(const fp threshold) const;
-template void Edge<mNode>::printMatrix<mNode, true>() const;
+Edge<mNode>::getSparseMatrix<mNode, true>(const std::size_t numQubits,
+                                          const fp threshold) const;
+template void
+Edge<mNode>::printMatrix<mNode, true>(const std::size_t numQubits) const;
 template void Edge<mNode>::traverseMatrix<mNode, true>(
     const std::complex<fp>& amp, const std::size_t i, const std::size_t j,
-    MatrixEntryFunc f, const fp threshold) const;
+    MatrixEntryFunc f, const std::size_t level, const fp threshold) const;
 
 template Edge<dNode> Edge<dNode>::normalize<dNode, true>(
     dNode* p, const std::array<Edge<dNode>, NEDGE>& e, MemoryManager<dNode>& mm,
     ComplexNumbers& cn);
-template CMat Edge<dNode>::getMatrix<dNode, true>(const fp threshold) const;
+template CMat Edge<dNode>::getMatrix<dNode, true>(const std::size_t numQubits,
+                                                  const fp threshold) const;
 template SparseCMat
-Edge<dNode>::getSparseMatrix<dNode, true>(const fp threshold) const;
-template void Edge<dNode>::printMatrix<dNode, true>() const;
+Edge<dNode>::getSparseMatrix<dNode, true>(const std::size_t numQubits,
+                                          const fp threshold) const;
+template void
+Edge<dNode>::printMatrix<dNode, true>(const std::size_t numQubits) const;
 template SparsePVec
-Edge<dNode>::getSparseProbabilityVector(const fp threshold) const;
+Edge<dNode>::getSparseProbabilityVector(const std::size_t numQubits,
+                                        const fp threshold) const;
 template SparsePVecStrKeys
-Edge<dNode>::getSparseProbabilityVectorStrKeys(const fp threshold) const;
+Edge<dNode>::getSparseProbabilityVectorStrKeys(const std::size_t numQubits,
+                                               const fp threshold) const;
 template std::complex<fp>
-Edge<dNode>::getValueByIndex<dNode, true>(const std::size_t i,
+Edge<dNode>::getValueByIndex<dNode, true>(const std::size_t numQubits,
+                                          const std::size_t i,
                                           const std::size_t j) const;
 template void Edge<dNode>::traverseMatrix<dNode, true>(
     const std::complex<fp>& amp, const std::size_t i, const std::size_t j,
-    MatrixEntryFunc f, const fp threshold) const;
+    MatrixEntryFunc f, const std::size_t level, const fp threshold) const;
 template void Edge<dNode>::traverseDiagonal(const fp& prob, const std::size_t i,
                                             ProbabilityFunc f,
+                                            std::size_t level,
                                             const dd::fp threshold) const;
 
 } // namespace dd
 
 ///-----------------------------------------------------------------------------
 ///                         \n Hash related code \n
 ///-----------------------------------------------------------------------------
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/FunctionalityConstruction.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/FunctionalityConstruction.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   }
 
   if (const auto* grover = dynamic_cast<const qc::Grover*>(qc)) {
     return buildFunctionality(grover, dd);
   }
 
   auto permutation = qc->initialLayout;
-  auto e = dd.createInitialMatrix(nq, qc->ancillary);
+  auto e = dd.createInitialMatrix(qc->ancillary);
 
   for (const auto& op : *qc) {
     auto tmp = dd.multiply(getDD(op.get(), dd, permutation), e);
 
     dd.incRef(tmp);
     dd.decRef(e);
     e = tmp;
@@ -195,14 +195,21 @@
   e = tmp;
 
   return e;
 }
 
 template MatrixDD buildFunctionality(const qc::QuantumComputation* qc,
                                      Package<DDPackageConfig>& dd);
+template MatrixDD
+buildFunctionality(const qc::QuantumComputation* qc,
+                   Package<dd::DensityMatrixSimulatorDDPackageConfig>& dd);
+template MatrixDD
+buildFunctionality(const qc::QuantumComputation* qc,
+                   Package<dd::StochasticNoiseSimulatorDDPackageConfig>& dd);
+
 template MatrixDD buildFunctionalityRecursive(const qc::QuantumComputation* qc,
                                               Package<DDPackageConfig>& dd);
 template bool buildFunctionalityRecursive(const qc::QuantumComputation* qc,
                                           const std::size_t depth,
                                           const std::size_t opIdx,
                                           std::stack<MatrixDD>& s,
                                           qc::Permutation& permutation,
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/MemoryManager.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/MemoryManager.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/Node.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/Node.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/Operations.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/Operations.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 namespace dd {
 template <class Config>
 void dumpTensor(qc::Operation* op, std::ostream& of,
                 std::vector<std::size_t>& inds, size_t& gateIdx,
                 Package<Config>& dd) {
   const auto type = op->getType();
   if (op->isStandardOperation()) {
-    auto nqubits = op->getNqubits();
     const auto& controls = op->getControls();
     const auto& targets = op->getTargets();
 
     // start of tensor
     of << "[";
 
     // save tags including operation type, involved qubits, and gate index
@@ -51,15 +50,14 @@
       ssOut << ", \"q" << qubit << "_" << ind << "\"";
       ++iter;
     }
     of << "[" << ssIn.str() << ", " << ssOut.str() << "], ";
 
     // write tensor dimensions
     const std::size_t localQubits = targets.size() + controls.size();
-    const std::size_t globalQubits = nqubits;
     of << "[";
     for (std::size_t q = 0U; q < localQubits; ++q) {
       if (q != 0U) {
         of << ", ";
       }
       of << 2 << ", " << 2;
     }
@@ -74,28 +72,23 @@
         localTargets.emplace_back(localIdx);
       } else {
         const auto* control = std::get_if<qc::Control>(&var);
         localControls.emplace(localIdx, control->type);
       }
       ++localIdx;
     }
-    // temporarily change nqubits
-    op->setNqubits(localQubits);
 
     // get DD for local operation
     auto localOp = op->clone();
     localOp->setControls(localControls);
     localOp->setTargets(localTargets);
     const auto localDD = getDD(localOp.get(), dd);
 
     // translate local DD to matrix
-    const auto localMatrix = localDD.getMatrix();
-
-    // restore nqubits
-    op->setNqubits(globalQubits);
+    const auto localMatrix = localDD.getMatrix(localQubits);
 
     // set appropriate precision for dumping numbers
     const auto precision = of.precision();
     of.precision(std::numeric_limits<dd::fp>::max_digits10);
 
     // write tensor data
     of << "[";
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/RealNumber.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/RealNumber.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/RealNumberUniqueTable.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/RealNumberUniqueTable.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/Simulation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/Simulation.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,16 @@
         if (nonunitary->getType() == Reset) {
           const auto& qubits = nonunitary->getTargets();
           for (const auto& qubit : qubits) {
             auto bit = dd.measureOneCollapsing(
                 e, static_cast<Qubit>(permutation.at(qubit)), true, mt);
             // apply an X operation whenever the measured result is one
             if (bit == '1') {
-              const auto x = qc::StandardOperation(
-                  qc->getNqubits(), permutation.at(qubit), qc::X);
+              const auto x =
+                  qc::StandardOperation(permutation.at(qubit), qc::X);
               auto tmp = dd.multiply(getDD(&x, dd), e);
               dd.incRef(tmp);
               dd.decRef(e);
               e = tmp;
               dd.garbageCollect();
             }
           }
@@ -266,16 +266,15 @@
       // normalize probabilities
       const auto norm = pzero + pone;
       pzero /= norm;
       pone /= norm;
 
       if (RealNumber::approximatelyEquals(pone, 1.)) {
         const qc::MatrixDD xGate =
-            dd.makeGateDD(X_MAT, static_cast<std::size_t>(state.p->v) + 1U,
-                          static_cast<Qubit>(permutation.at(target)));
+            dd.makeGateDD(X_MAT, static_cast<Qubit>(permutation.at(target)));
         const qc::VectorDD resetState = dd.multiply(xGate, state);
         dd.incRef(resetState);
         dd.decRef(state);
         state = resetState;
         continue;
       }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/statistics/MemoryManagerStatistics.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/statistics/MemoryManagerStatistics.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/statistics/TableStatistics.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/statistics/TableStatistics.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/dd/statistics/UniqueTableStatistics.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/dd/statistics/UniqueTableStatistics.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/CMakeLists.txt` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Ecc.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Ecc.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q18Surface.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q18Surface.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q3Shor.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q3Shor.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -64,39 +64,36 @@
 }
 
 void Q3Shor::addOperation(const qc::Controls& controls,
                           const qc::Targets& targets, const qc::OpType type) {
   const auto numTargets = targets.size();
   const auto numControls = controls.size();
   const auto numQubits = qcOriginal->getNqubits();
-  const auto numMappedQubits = qcMapped->getNqubits();
   for (std::size_t j = 0; j < numTargets; j++) {
     auto i = targets[j];
     if (numControls > 0) {
-      qcMapped->emplace_back<qc::StandardOperation>(numMappedQubits, controls,
-                                                    i, type);
+      qcMapped->emplace_back<qc::StandardOperation>(controls, i, type);
       qc::Controls controls2;
       qc::Controls controls3;
       for (const auto& ct : controls) {
         controls2.insert(
             qc::Control{static_cast<Qubit>(ct.qubit + numQubits), ct.type});
         controls3.insert(
             qc::Control{static_cast<Qubit>(ct.qubit + 2 * numQubits), ct.type});
       }
       qcMapped->emplace_back<qc::StandardOperation>(
-          numMappedQubits, controls2, static_cast<Qubit>(i + numQubits), type);
+          controls2, static_cast<Qubit>(i + numQubits), type);
       qcMapped->emplace_back<qc::StandardOperation>(
-          numMappedQubits, controls3, static_cast<Qubit>(i + 2 * numQubits),
-          type);
+          controls3, static_cast<Qubit>(i + 2 * numQubits), type);
     } else {
-      qcMapped->emplace_back<qc::StandardOperation>(numMappedQubits, i, type);
+      qcMapped->emplace_back<qc::StandardOperation>(i, type);
       qcMapped->emplace_back<qc::StandardOperation>(
-          numMappedQubits, static_cast<Qubit>(i + numQubits), type);
+          static_cast<Qubit>(i + numQubits), type);
       qcMapped->emplace_back<qc::StandardOperation>(
-          numMappedQubits, static_cast<Qubit>(i + 2 * numQubits), type);
+          static_cast<Qubit>(i + 2 * numQubits), type);
     }
   }
 }
 
 void Q3Shor::mapGate(const qc::Operation& gate) {
   if (isDecoded && gate.getType() != qc::Measure && gate.getType() != qc::H) {
     writeEncoding();
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q5Laflamme.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q5Laflamme.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -133,16 +133,15 @@
     for (std::size_t t = 0; t < gate.getNtargets(); t++) {
       auto i = gate.getTargets().at(t);
       if (gate.getNcontrols() != 0U) {
         gateNotAvailableError(gate);
       } else {
         for (Qubit j = 0; j < N_REDUNDANT_QUBITS; j++) {
           qcMapped->emplace_back<qc::StandardOperation>(
-              qcMapped->getNqubits(), static_cast<Qubit>(i + j * nQubits),
-              gate.getType());
+              static_cast<Qubit>(i + j * nQubits), gate.getType());
         }
       }
     }
     break;
   case qc::Measure:
     if (!isDecoded) {
       measureAndCorrect();
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q7Steane.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q7Steane.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -112,43 +112,39 @@
 
 void Q7Steane::addSOperation(const qc::Controls& controls,
                              const qc::Targets& targets,
                              const qc::OpType type) {
   const auto numTargets = targets.size();
   const auto numControls = controls.size();
   const auto numQubits = qcOriginal->getNqubits();
-  const auto numMappedQubits = qcMapped->getNqubits();
 
   for (std::size_t k = 0; k < numTargets; k++) {
     auto i = targets[k];
     if (numControls > 0) {
       for (std::size_t j = 0; j < N_REDUNDANT_QUBITS; j++) {
         qc::Controls controls2;
         for (const auto& ct : controls) {
           controls2.emplace(static_cast<Qubit>(ct.qubit + j * numQubits),
                             ct.type);
         }
         qcMapped->emplace_back<qc::StandardOperation>(
-            numMappedQubits, controls2, static_cast<Qubit>(i + j * numQubits),
-            type);
+            controls2, static_cast<Qubit>(i + j * numQubits), type);
         qcMapped->emplace_back<qc::StandardOperation>(
-            numMappedQubits, controls2, static_cast<Qubit>(i + j * numQubits),
-            type);
+            controls2, static_cast<Qubit>(i + j * numQubits), type);
         qcMapped->emplace_back<qc::StandardOperation>(
-            numMappedQubits, controls2, static_cast<Qubit>(i + j * numQubits),
-            type);
+            controls2, static_cast<Qubit>(i + j * numQubits), type);
       }
     } else {
       for (std::size_t j = 0; j < N_REDUNDANT_QUBITS; j++) {
         qcMapped->emplace_back<qc::StandardOperation>(
-            numMappedQubits, static_cast<Qubit>(i + j * numQubits), type);
+            static_cast<Qubit>(i + j * numQubits), type);
         qcMapped->emplace_back<qc::StandardOperation>(
-            numMappedQubits, static_cast<Qubit>(i + j * numQubits), type);
+            static_cast<Qubit>(i + j * numQubits), type);
         qcMapped->emplace_back<qc::StandardOperation>(
-            numMappedQubits, static_cast<Qubit>(i + j * numQubits), type);
+            static_cast<Qubit>(i + j * numQubits), type);
       }
     }
   }
 }
 
 void Q7Steane::mapGate(const qc::Operation& gate) {
   if (isDecoded && gate.getType() != qc::Measure) {
@@ -169,22 +165,20 @@
         for (std::size_t j = 0; j < N_REDUNDANT_QUBITS; j++) {
           qc::Controls ctrls2;
           for (const auto& ct : ctrls) {
             ctrls2.insert(qc::Control{
                 static_cast<Qubit>(ct.qubit + j * nQubits), ct.type});
           }
           qcMapped->emplace_back<qc::StandardOperation>(
-              qcMapped->getNqubits(), ctrls2,
-              static_cast<Qubit>(i + j * nQubits), gate.getType());
+              ctrls2, static_cast<Qubit>(i + j * nQubits), gate.getType());
         }
       } else {
         for (std::size_t j = 0; j < N_REDUNDANT_QUBITS; j++) {
           qcMapped->emplace_back<qc::StandardOperation>(
-              qcMapped->getNqubits(), static_cast<Qubit>(i + j * nQubits),
-              gate.getType());
+              static_cast<Qubit>(i + j * nQubits), gate.getType());
         }
       }
     }
     break;
     // locigal S = 3 physical S's
   case qc::S:
   case qc::Sdg:
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q9Shor.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q9Shor.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -181,22 +181,21 @@
         qc::Controls controls2;
         for (const auto& ct : controls) {
           controls2.insert(
               qc::Control{static_cast<Qubit>(ct.qubit + j * nQubits), ct.type});
           qcMapped->h(static_cast<Qubit>(ct.qubit + j * nQubits));
         }
         qcMapped->emplace_back<qc::StandardOperation>(
-            qcMapped->getNqubits(), controls2,
-            static_cast<Qubit>(i + j * nQubits), type);
+            controls2, static_cast<Qubit>(i + j * nQubits), type);
         for (const auto& ct : controls) {
           qcMapped->h(static_cast<Qubit>(ct.qubit + j * nQubits));
         }
       }
     } else {
       for (size_t j = 0; j < N_REDUNDANT_QUBITS; j++) {
         qcMapped->emplace_back<qc::StandardOperation>(
-            qcMapped->getNqubits(), static_cast<Qubit>(i + j * nQubits), type);
+            static_cast<Qubit>(i + j * nQubits), type);
       }
     }
   }
 }
 } // namespace ecc
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/ecc/Q9Surface.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/ecc/Q9Surface.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/__init__.py` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/__main__.py` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/__main__.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_core/__init__.pyi` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_core/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,18 @@
     global_phase: float
 
     @property
     def num_qubits(self: Self) -> int: ...
     @property
     def num_ancilla_qubits(self: Self) -> int: ...
     @property
+    def num_garbage_qubits(self: Self) -> int: ...
+    @property
+    def num_measured_qubits(self: Self) -> int: ...
+    @property
     def num_qubits_without_ancilla_qubits(self: Self) -> int: ...
     @property
     def num_classical_bits(self: Self) -> int: ...
     @property
     def num_ops(self: Self) -> int: ...
     def num_single_qubit_ops(self: Self) -> int: ...
     @property
@@ -98,18 +102,20 @@
     # --------------------------------------------------------------------------
     #                       Ancilla and Garbage Handling
     # --------------------------------------------------------------------------
 
     @property
     def ancillary(self: Self) -> list[bool]: ...
     def set_circuit_qubit_ancillary(self: Self, q: int) -> None: ...
+    def set_circuit_qubits_ancillary(self: Self, q_min: int, q_max: int) -> None: ...
     def is_circuit_qubit_ancillary(self: Self, q: int) -> bool: ...
     @property
     def garbage(self: Self) -> list[bool]: ...
     def set_circuit_qubit_garbage(self: Self, q: int) -> None: ...
+    def set_circuit_qubits_garbage(self: Self, q_min: int, q_max: int) -> None: ...
     def is_circuit_qubit_garbage(self: Self, q: int) -> bool: ...
 
     # --------------------------------------------------------------------------
     #                        Symbolic Circuit Handling
     # --------------------------------------------------------------------------
 
     @property
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_core/operations.pyi` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_core/operations.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -89,15 +89,14 @@
     def __int__(self: Self) -> int: ...
     def __ne__(self: Self, other: object) -> bool: ...
     def __setstate__(self: Self, state: int) -> None: ...
 
 class Operation(ABC):
     type_: OpType
     controls: set[Control]
-    num_qubits: int
     targets: list[int]
     parameter: list[float]
     @property
     def name(self: Self) -> str: ...
     @property
     def num_targets(self: Self) -> int: ...
     @property
@@ -132,110 +131,94 @@
 
 class StandardOperation(Operation):
     @overload
     def __init__(self: Self) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         target: int,
         op_type: OpType,
         params: Sequence[float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         targets: Sequence[int],
         op_type: OpType,
         params: Sequence[float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         control: Control,
         target: int,
         op_type: OpType,
         params: Sequence[float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         control: Control,
         targets: Sequence[int],
         op_type: OpType,
         params: Sequence[float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         controls: set[Control],
         target: int,
         op_type: OpType,
         params: Sequence[float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         controls: set[Control],
         targets: Sequence[int],
         op_type: OpType,
         params: Sequence[float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
-    def __init__(self: Self, nq: int, controls: set[Control], target: int, starting_qubit: int = 0) -> None: ...
-    @overload
     def __init__(
         self: Self,
-        nq: int,
         controls: set[Control],
         target0: int,
         target1: int,
         op_type: OpType,
         params: Sequence[float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     def add_control(self: Self, control: Control) -> None: ...
     def clear_controls(self: Self) -> None: ...
     def remove_control(self: Self, control: Control) -> None: ...
     def invert(self: Self) -> None: ...
     def qasm2_str(self: Self, qreg: Sequence[tuple[str, str]], creg: Sequence[tuple[str, str]]) -> str: ...
     def qasm3_str(self: Self, qreg: Sequence[tuple[str, str]], creg: Sequence[tuple[str, str]]) -> str: ...
 
 class NonUnitaryOperation(Operation):
     @property
     def classics(self: Self) -> list[int]: ...
     @overload
-    def __init__(self: Self, nq: int, targets: Sequence[int], classics: Sequence[int]) -> None: ...
+    def __init__(self: Self, targets: Sequence[int], classics: Sequence[int]) -> None: ...
     @overload
-    def __init__(self: Self, nq: int, target: int, classic: int) -> None: ...
+    def __init__(self: Self, target: int, classic: int) -> None: ...
     @overload
-    def __init__(self: Self, nq: int, targets: Sequence[int], op_type: OpType = ...) -> None: ...
+    def __init__(self: Self, targets: Sequence[int], op_type: OpType = ...) -> None: ...
     def add_control(self: Self, control: Control) -> None: ...
     def clear_controls(self: Self) -> None: ...
     def remove_control(self: Self, control: Control) -> None: ...
     def invert(self: Self) -> None: ...
     def qasm2_str(self: Self, qreg: Sequence[tuple[str, str]], creg: Sequence[tuple[str, str]]) -> str: ...
     def qasm3_str(self: Self, qreg: Sequence[tuple[str, str]], creg: Sequence[tuple[str, str]]) -> str: ...
 
 class CompoundOperation(Operation):
     @overload
-    def __init__(self: Self, nq: int) -> None: ...
+    def __init__(self: Self) -> None: ...
     @overload
-    def __init__(self: Self, nq: int, ops: Sequence[Operation]) -> None: ...
+    def __init__(self: Self, ops: Sequence[Operation]) -> None: ...
     def __len__(self: Self) -> int: ...
     @overload
     def __getitem__(self: Self, idx: int) -> Operation: ...
     @overload
     def __getitem__(self: Self, idx: slice) -> list[Operation]: ...
     def append(self: Self, op: Operation) -> None: ...
     def empty(self: Self) -> bool: ...
@@ -248,79 +231,65 @@
 
 class SymbolicOperation(StandardOperation):
     @overload
     def __init__(self: Self) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         target: int,
         op_type: OpType,
         params: Sequence[Expression | float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         targets: Sequence[int],
         op_type: OpType,
         params: Sequence[Expression | float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         control: Control,
         target: int,
         op_type: OpType,
         params: Sequence[Expression | float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         control: Control,
         targets: Sequence[int],
         op_type: OpType,
         params: Sequence[Expression | float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         controls: set[Control],
         target: int,
         op_type: OpType,
         params: Sequence[Expression | float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         controls: set[Control],
         targets: Sequence[int],
         op_type: OpType,
         params: Sequence[Expression | float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     @overload
     def __init__(
         self: Self,
-        nq: int,
         controls: set[Control],
         target0: int,
         target1: int,
         op_type: OpType,
         params: Sequence[Expression | float] | None = None,
-        starting_qubit: int = 0,
     ) -> None: ...
     def get_parameter(self: Self, idx: int) -> Expression | float: ...
     def get_parameters(self: Self) -> list[Expression | float]: ...
     def get_instantiated_operation(self: Self, assignment: Mapping[Variable, float]) -> StandardOperation: ...
     def instantiate(self: Self, assignment: Mapping[Variable, float]) -> None: ...
 
 class ClassicControlledOperation(Operation):
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/_core/symbolic.pyi` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/_core/symbolic.pyi`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/commands.py` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/commands.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/evaluation.py` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/evaluation.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/io.py` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     from qiskit.circuit import QuantumCircuit
 
 
 def load(input_circuit: QuantumComputation | str | PathLike[str] | QuantumCircuit) -> QuantumComputation:
     """Load a quantum circuit from any supported format as a ``QuantumComputation``.
 
     Args:
-        input_circuit: The input circuit to translate to a ``QuantumComputation``.
-        This can be a `QuantumComputation` itself, a file name to any of the supported file formats,
-        an OpenQASM (2.0 or 3.0) string, or a Qiskit `QuantumCircuit`.
+        input_circuit: The input circuit to translate to a ``QuantumComputation``. This can be a `QuantumComputation` itself, a file name to any of the supported file formats, an OpenQASM (2.0 or 3.0) string, or a Qiskit `QuantumCircuit`.
 
     Returns:
         The ``QuantumComputation``.
 
     Raises:
         ValueError: If the input circuit is a Qiskit `QuantumCircuit` but the `qiskit` extra is not installed.
         FileNotFoundError: If the input circuit is a file name and the file does not exist.
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/operations.py` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/operations.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/mqt/core/plugins/qiskit.py` & `mqt_qmap-2.5.1/extern/mqt-core/src/mqt/core/plugins/qiskit.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,23 +160,23 @@
             msg = f"Unsupported gate {name} with definition {instr.definition}"
             raise NotImplementedError(msg) from ex
 
     qubits = [qubit_map[qubit] for qubit in qargs]
 
     if name == "measure":
         clbits = [clbit_map[clbit] for clbit in cargs]
-        qc.append(NonUnitaryOperation(qc.num_qubits, qubits, clbits))
+        qc.append(NonUnitaryOperation(qubits, clbits))
         return []
 
     if name == "reset":
-        qc.append(NonUnitaryOperation(qc.num_qubits, qubits))
+        qc.append(NonUnitaryOperation(qubits))
         return []
 
     if name == "barrier":
-        qc.append(StandardOperation(qc.num_qubits, qubits, OpType.barrier))
+        qc.append(StandardOperation(qubits, OpType.barrier))
         return []
 
     if name in {"i", "id", "iden"}:
         return _add_operation(qc, OpType.i, qargs, params, qubit_map)
 
     if name in {"x", "cx", "ccx", "mcx", "mcx_gray"}:
         return _add_operation(qc, OpType.x, qargs, params, qubit_map)
@@ -329,17 +329,17 @@
     qubit_map: Mapping[Qubit, int],
 ) -> list[float | ParameterExpression]:
     qubits = [qubit_map[qubit] for qubit in qargs]
     target = qubits.pop()
     controls = {Control(qubit) for qubit in qubits}
     parameters = [_parse_symbolic_expression(param) for param in params]
     if any(isinstance(parameter, Expression) for parameter in parameters):
-        qc.append(SymbolicOperation(qc.num_qubits, controls, target, type_, parameters))
+        qc.append(SymbolicOperation(controls, target, type_, parameters))
     else:
-        qc.append(StandardOperation(qc.num_qubits, controls, target, type_, cast(List[float], parameters)))
+        qc.append(StandardOperation(controls, target, type_, cast(List[float], parameters)))
     return parameters
 
 
 def _add_two_target_operation(
     qc: QuantumComputation | CompoundOperation,
     type_: OpType,
     qargs: Sequence[Qubit],
@@ -348,17 +348,17 @@
 ) -> list[float | ParameterExpression]:
     qubits = [qubit_map[qubit] for qubit in qargs]
     target2 = qubits.pop()
     target1 = qubits.pop()
     controls = {Control(qubit) for qubit in qubits}
     parameters = [_parse_symbolic_expression(param) for param in params]
     if any(isinstance(parameter, Expression) for parameter in parameters):
-        qc.append(SymbolicOperation(qc.num_qubits, controls, target1, target2, type_, parameters))
+        qc.append(SymbolicOperation(controls, target1, target2, type_, parameters))
     else:
-        qc.append(StandardOperation(qc.num_qubits, controls, target1, target2, type_, cast(List[float], parameters)))
+        qc.append(StandardOperation(controls, target1, target2, type_, cast(List[float], parameters)))
     return parameters
 
 
 def _import_layouts(qc: QuantumComputation, circ: QuantumCircuit) -> None:
     # qiskit-terra 0.24.0 added a (public) `layout` attribute
     layout = circ.layout if hasattr(circ, "layout") else circ._layout  # noqa: SLF001
 
@@ -403,15 +403,15 @@
     cargs: Sequence[Clbit],
     qubit_map: Mapping[Qubit, int],
     clbit_map: Mapping[Clbit, int],
 ) -> list[float | ParameterExpression]:
     qarg_map = dict(zip(circ.qubits, qargs))
     carg_map = dict(zip(circ.clbits, cargs))
 
-    qc.append(CompoundOperation(qc.num_qubits))
+    qc.append(CompoundOperation())
     comp_op = cast(CompoundOperation, qc[-1])
 
     params = []
     for instruction, q_args, c_args in circ.data:
         mapped_qargs = [qarg_map[qarg] for qarg in q_args]
         mapped_cargs = [carg_map[carg] for carg in c_args]
         instruction_params = instruction.params
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/operations/ClassicControlledOperation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/operations/ClassicControlledOperation.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/operations/CompoundOperation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/operations/CompoundOperation.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #include "operations/CompoundOperation.hpp"
 
 #include <algorithm>
 
 namespace qc {
-CompoundOperation::CompoundOperation(const std::size_t nq) {
+CompoundOperation::CompoundOperation() {
   name = "Compound operation:";
-  nqubits = nq;
   type = Compound;
 }
 
 CompoundOperation::CompoundOperation(
-    const std::size_t nq, std::vector<std::unique_ptr<Operation>>&& operations)
-    : CompoundOperation(nq) {
+    std::vector<std::unique_ptr<Operation>>&& operations)
+    : CompoundOperation() {
   // NOLINTNEXTLINE(cppcoreguidelines-prefer-member-initializer)
   ops = std::move(operations);
 }
 
 CompoundOperation::CompoundOperation(const CompoundOperation& co)
     : Operation(co), ops(co.ops.size()) {
   for (std::size_t i = 0; i < co.ops.size(); ++i) {
@@ -34,21 +33,14 @@
   return *this;
 }
 
 std::unique_ptr<Operation> CompoundOperation::clone() const {
   return std::make_unique<CompoundOperation>(*this);
 }
 
-void CompoundOperation::setNqubits(const std::size_t nq) {
-  nqubits = nq;
-  for (auto& op : ops) {
-    op->setNqubits(nq);
-  }
-}
-
 bool CompoundOperation::isNonUnitaryOperation() const {
   return std::any_of(ops.cbegin(), ops.cend(), [](const auto& op) {
     return op->isNonUnitaryOperation();
   });
 }
 
 bool CompoundOperation::isCompoundOperation() const { return true; }
@@ -114,20 +106,21 @@
 
 bool CompoundOperation::equals(const Operation& operation) const {
   return equals(operation, {}, {});
 }
 
 std::ostream& CompoundOperation::print(std::ostream& os,
                                        const Permutation& permutation,
-                                       const std::size_t prefixWidth) const {
+                                       const std::size_t prefixWidth,
+                                       const std::size_t nqubits) const {
   const auto prefix = std::string(prefixWidth - 1, ' ');
   os << std::string(4 * nqubits, '-') << "\n";
   for (const auto& op : ops) {
     os << prefix << ":";
-    op->print(os, permutation, prefixWidth);
+    op->print(os, permutation, prefixWidth, nqubits);
     os << "\n";
   }
   os << prefix << std::string(4 * nqubits + 1, '-');
   return os;
 }
 
 bool CompoundOperation::actsOn(const Qubit i) const {
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/operations/NonUnitaryOperation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/operations/NonUnitaryOperation.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -8,55 +8,50 @@
 
 #include <algorithm>
 #include <cassert>
 #include <utility>
 
 namespace qc {
 // Measurement constructor
-NonUnitaryOperation::NonUnitaryOperation(const std::size_t nq,
-                                         std::vector<Qubit> qubitRegister,
+NonUnitaryOperation::NonUnitaryOperation(std::vector<Qubit> qubitRegister,
                                          std::vector<Bit> classicalRegister)
     : classics(std::move(classicalRegister)) {
   type = Measure;
-  nqubits = nq;
   targets = std::move(qubitRegister);
   name = toString(type);
   if (targets.size() != classics.size()) {
     throw std::invalid_argument(
         "Sizes of qubit register and classical register do not match.");
   }
 }
-NonUnitaryOperation::NonUnitaryOperation(const std::size_t nq,
-                                         const Qubit qubit, const Bit cbit)
+NonUnitaryOperation::NonUnitaryOperation(const Qubit qubit, const Bit cbit)
     : classics({cbit}) {
   type = Measure;
-  nqubits = nq;
   targets = {qubit};
   name = toString(type);
 }
 
 // General constructor
-NonUnitaryOperation::NonUnitaryOperation(const std::size_t nq, Targets qubits,
-                                         OpType op) {
+NonUnitaryOperation::NonUnitaryOperation(Targets qubits, OpType op) {
   type = op;
-  nqubits = nq;
   targets = std::move(qubits);
   std::sort(targets.begin(), targets.end());
   name = toString(type);
 }
 
-std::ostream& NonUnitaryOperation::print(
-    std::ostream& os, const Permutation& permutation,
-    [[maybe_unused]] const std::size_t prefixWidth) const {
+std::ostream&
+NonUnitaryOperation::print(std::ostream& os, const Permutation& permutation,
+                           [[maybe_unused]] const std::size_t prefixWidth,
+                           const std::size_t nqubits) const {
   switch (type) {
   case Measure:
-    printMeasurement(os, targets, classics, permutation);
+    printMeasurement(os, targets, classics, permutation, nqubits);
     break;
   case Reset:
-    printReset(os, targets, permutation);
+    printReset(os, targets, permutation, nqubits);
     break;
   default:
     break;
   }
   return os;
 }
 
@@ -142,17 +137,19 @@
       return measurements1 == measurements2;
     }
     return Operation::equals(op, perm1, perm2);
   }
   return false;
 }
 
-void NonUnitaryOperation::printMeasurement(
-    std::ostream& os, const std::vector<Qubit>& q, const std::vector<Bit>& c,
-    const Permutation& permutation) const {
+void NonUnitaryOperation::printMeasurement(std::ostream& os,
+                                           const std::vector<Qubit>& q,
+                                           const std::vector<Bit>& c,
+                                           const Permutation& permutation,
+                                           const std::size_t nqubits) {
   auto qubitIt = q.cbegin();
   auto classicIt = c.cbegin();
   if (permutation.empty()) {
     for (std::size_t i = 0; i < nqubits; ++i) {
       if (qubitIt != q.cend() && *qubitIt == i) {
         os << "\033[34m" << std::setw(4) << *classicIt << "\033[0m";
         ++qubitIt;
@@ -172,15 +169,16 @@
       }
     }
   }
 }
 
 void NonUnitaryOperation::printReset(std::ostream& os,
                                      const std::vector<Qubit>& q,
-                                     const Permutation& permutation) const {
+                                     const Permutation& permutation,
+                                     const std::size_t nqubits) const {
   const auto actualTargets = permutation.apply(q);
   for (std::size_t i = 0; i < nqubits; ++i) {
     if (std::find(actualTargets.cbegin(), actualTargets.cend(), i) !=
         actualTargets.cend()) {
       os << "\033[31m" << std::setw(4) << shortName(type) << "\033[0m";
       continue;
     }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/operations/Operation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/operations/Operation.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
       os << "(" << parameter.at(j) << ") ";
     }
   }
 
   return os;
 }
 
-std::ostream&
-Operation::print(std::ostream& os, const Permutation& permutation,
-                 [[maybe_unused]] const std::size_t prefixWidth) const {
+std::ostream& Operation::print(std::ostream& os, const Permutation& permutation,
+                               [[maybe_unused]] const std::size_t prefixWidth,
+                               const std::size_t nqubits) const {
   const auto precBefore = std::cout.precision(20);
   const auto& actualControls = permutation.apply(getControls());
   const auto& actualTargets = permutation.apply(getTargets());
 
   for (std::size_t i = 0; i < nqubits; ++i) {
     const auto q = static_cast<Qubit>(i);
     if (std::find(actualTargets.cbegin(), actualTargets.cend(), q) !=
@@ -68,21 +68,19 @@
             std::find(actualControls.cbegin(), actualControls.cend(), q);
         it != actualControls.cend()) {
       if (it->type == Control::Type::Pos) {
         os << "\033[32m";
       } else {
         os << "\033[31m";
       }
-      os << std::setw(4) << "c"
-         << "\033[0m";
+      os << std::setw(4) << "c" << "\033[0m";
       continue;
     }
 
-    os << std::setw(4) << "|"
-       << "\033[0m";
+    os << std::setw(4) << "|" << "\033[0m";
   }
 
   printParameters(os);
 
   std::cout.precision(precBefore);
 
   return os;
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/operations/StandardOperation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/operations/StandardOperation.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -157,89 +157,71 @@
     type = parseU2(parameter.at(0), parameter.at(1));
   } else if (type == U) {
     assert(parameter.size() == 3);
     type = parseU3(parameter.at(0), parameter.at(1), parameter.at(2));
   }
 }
 
-void StandardOperation::setup(const std::size_t nq, const Qubit startingQubit) {
-  nqubits = nq;
-  startQubit = startingQubit;
+void StandardOperation::setup() {
   checkUgate();
   name = toString(type);
 }
 
 /***
  * Constructors
  ***/
-StandardOperation::StandardOperation(const std::size_t nq, const Qubit target,
-                                     const OpType g, std::vector<fp> params,
-                                     const Qubit startingQubit) {
+StandardOperation::StandardOperation(const Qubit target, const OpType g,
+                                     std::vector<fp> params) {
   type = g;
   parameter = std::move(params);
-  setup(nq, startingQubit);
+  setup();
   targets.emplace_back(target);
 }
 
-StandardOperation::StandardOperation(const std::size_t nq, const Targets& targ,
-                                     const OpType g, std::vector<fp> params,
-                                     const Qubit startingQubit) {
+StandardOperation::StandardOperation(const Targets& targ, const OpType g,
+                                     std::vector<fp> params) {
   type = g;
   parameter = std::move(params);
-  setup(nq, startingQubit);
+  setup();
   targets = targ;
 }
 
-StandardOperation::StandardOperation(const std::size_t nq,
-                                     const Control control, const Qubit target,
+StandardOperation::StandardOperation(const Control control, const Qubit target,
                                      const OpType g,
-                                     const std::vector<fp>& params,
-                                     const Qubit startingQubit)
-    : StandardOperation(nq, target, g, params, startingQubit) {
+                                     const std::vector<fp>& params)
+    : StandardOperation(target, g, params) {
   controls.insert(control);
 }
 
-StandardOperation::StandardOperation(const std::size_t nq,
-                                     const Control control, const Targets& targ,
+StandardOperation::StandardOperation(const Control control, const Targets& targ,
                                      const OpType g,
-                                     const std::vector<fp>& params,
-                                     const Qubit startingQubit)
-    : StandardOperation(nq, targ, g, params, startingQubit) {
+                                     const std::vector<fp>& params)
+    : StandardOperation(targ, g, params) {
   controls.insert(control);
 }
 
-StandardOperation::StandardOperation(const std::size_t nq, const Controls& c,
-                                     const Qubit target, const OpType g,
-                                     const std::vector<fp>& params,
-                                     const Qubit startingQubit)
-    : StandardOperation(nq, target, g, params, startingQubit) {
+StandardOperation::StandardOperation(const Controls& c, const Qubit target,
+                                     const OpType g,
+                                     const std::vector<fp>& params)
+    : StandardOperation(target, g, params) {
   controls = c;
 }
 
-StandardOperation::StandardOperation(const std::size_t nq, const Controls& c,
-                                     const Targets& targ, const OpType g,
-                                     const std::vector<fp>& params,
-                                     const Qubit startingQubit)
-    : StandardOperation(nq, targ, g, params, startingQubit) {
+StandardOperation::StandardOperation(const Controls& c, const Targets& targ,
+                                     const OpType g,
+                                     const std::vector<fp>& params)
+    : StandardOperation(targ, g, params) {
   controls = c;
 }
 
-// MCT Constructor
-StandardOperation::StandardOperation(const std::size_t nq, const Controls& c,
-                                     const Qubit target,
-                                     const Qubit startingQubit)
-    : StandardOperation(nq, c, target, X, {}, startingQubit) {}
-
 // MCF (cSWAP), Peres, parameterized two target Constructor
-StandardOperation::StandardOperation(const std::size_t nq, const Controls& c,
-                                     const Qubit target0, const Qubit target1,
-                                     const OpType g,
-                                     const std::vector<fp>& params,
-                                     const Qubit startingQubit)
-    : StandardOperation(nq, c, {target0, target1}, g, params, startingQubit) {}
+StandardOperation::StandardOperation(const Controls& c, const Qubit target0,
+                                     const Qubit target1, const OpType g,
+                                     const std::vector<fp>& params)
+    : StandardOperation(c, {target0, target1}, g, params) {}
 
 /***
  * Public Methods
  ***/
 void StandardOperation::dumpOpenQASM(std::ostream& of,
                                      const RegisterNames& qreg,
                                      [[maybe_unused]] const RegisterNames& creg,
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/operations/SymbolicOperation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/operations/SymbolicOperation.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -186,97 +186,83 @@
       type = parseU3(symbolicParameter[0].value(), symbolicParameter[1].value(),
                      parameter[2]);
     }
   }
   // NOLINTEND(bugprone-unchecked-optional-access)
 }
 
-void SymbolicOperation::setup(const std::size_t nq,
-                              const std::vector<SymbolOrNumber>& params,
-                              const Qubit startingQubit) {
-  nqubits = nq;
+void SymbolicOperation::setup(const std::vector<SymbolOrNumber>& params) {
   const auto numParams = params.size();
   parameter.resize(numParams);
   symbolicParameter.resize(numParams);
   for (std::size_t i = 0; i < numParams; ++i) {
     storeSymbolOrNumber(params[i], i);
   }
-  startQubit = startingQubit;
   checkSymbolicUgate();
   name = toString(type);
 }
 
 [[nodiscard]] fp
 SymbolicOperation::getInstantiation(const SymbolOrNumber& symOrNum,
                                     const VariableAssignment& assignment) {
   return std::visit(
       Overload{[&](const fp num) { return num; },
                [&](const Symbolic& sym) { return sym.evaluate(assignment); }},
       symOrNum);
 }
 
-SymbolicOperation::SymbolicOperation(const std::size_t nq, const Qubit target,
-                                     const OpType g,
-                                     const std::vector<SymbolOrNumber>& params,
-                                     const Qubit startingQubit) {
+SymbolicOperation::SymbolicOperation(
+    const Qubit target, const OpType g,
+    const std::vector<SymbolOrNumber>& params) {
   type = g;
-  setup(nq, params, startingQubit);
+  setup(params);
   targets.emplace_back(target);
 }
 
-SymbolicOperation::SymbolicOperation(const std::size_t nq, const Targets& targ,
-                                     const OpType g,
-                                     const std::vector<SymbolOrNumber>& params,
-                                     const Qubit startingQubit) {
+SymbolicOperation::SymbolicOperation(
+    const Targets& targ, const OpType g,
+    const std::vector<SymbolOrNumber>& params) {
   type = g;
-  setup(nq, params, startingQubit);
+  setup(params);
   targets = targ;
 }
 
-SymbolicOperation::SymbolicOperation(const std::size_t nq,
-                                     const Control control, const Qubit target,
+SymbolicOperation::SymbolicOperation(const Control control, const Qubit target,
                                      const OpType g,
-                                     const std::vector<SymbolOrNumber>& params,
-                                     const Qubit startingQubit)
-    : SymbolicOperation(nq, target, g, params, startingQubit) {
+                                     const std::vector<SymbolOrNumber>& params)
+    : SymbolicOperation(target, g, params) {
   controls.insert(control);
 }
 
-SymbolicOperation::SymbolicOperation(const std::size_t nq,
-                                     const Control control, const Targets& targ,
+SymbolicOperation::SymbolicOperation(const Control control, const Targets& targ,
                                      const OpType g,
-                                     const std::vector<SymbolOrNumber>& params,
-                                     const Qubit startingQubit)
-    : SymbolicOperation(nq, targ, g, params, startingQubit) {
+                                     const std::vector<SymbolOrNumber>& params)
+    : SymbolicOperation(targ, g, params) {
   controls.insert(control);
 }
 
-SymbolicOperation::SymbolicOperation(const std::size_t nq, const Controls& c,
-                                     const Qubit target, const OpType g,
-                                     const std::vector<SymbolOrNumber>& params,
-                                     const Qubit startingQubit)
-    : SymbolicOperation(nq, target, g, params, startingQubit) {
+SymbolicOperation::SymbolicOperation(const Controls& c, const Qubit target,
+                                     const OpType g,
+                                     const std::vector<SymbolOrNumber>& params)
+    : SymbolicOperation(target, g, params) {
   controls = c;
 }
 
-SymbolicOperation::SymbolicOperation(const std::size_t nq, const Controls& c,
-                                     const Targets& targ, const OpType g,
-                                     const std::vector<SymbolOrNumber>& params,
-                                     const Qubit startingQubit)
-    : SymbolicOperation(nq, targ, g, params, startingQubit) {
+SymbolicOperation::SymbolicOperation(const Controls& c, const Targets& targ,
+                                     const OpType g,
+                                     const std::vector<SymbolOrNumber>& params)
+    : SymbolicOperation(targ, g, params) {
   controls = c;
 }
 
 // MCF (cSWAP), Peres, parameterized two target Constructor
-SymbolicOperation::SymbolicOperation(const std::size_t nq, const Controls& c,
-                                     const Qubit target0, const Qubit target1,
-                                     const OpType g,
-                                     const std::vector<SymbolOrNumber>& params,
-                                     const Qubit startingQubit)
-    : SymbolicOperation(nq, c, {target0, target1}, g, params, startingQubit) {}
+SymbolicOperation::SymbolicOperation(const Controls& c, const Qubit target0,
+                                     const Qubit target1, const OpType g,
+                                     const std::vector<SymbolOrNumber>& params)
+    : SymbolicOperation(c, {target0, target1}, g, params) {}
 
 bool SymbolicOperation::equals(const Operation& op, const Permutation& perm1,
                                const Permutation& perm2) const {
   if (!op.isSymbolicOperation() && !isStandardOperation()) {
     return false;
   }
   if (isStandardOperation() &&
@@ -322,15 +308,15 @@
     const VariableAssignment& assignment) const {
   std::vector<fp> parameters;
   const auto size = symbolicParameter.size();
   parameters.reserve(size);
   for (std::size_t i = 0; i < size; ++i) {
     parameters.emplace_back(getInstantiation(getParameter(i), assignment));
   }
-  return {nqubits, targets, type, parameters, startQubit};
+  return {controls, targets, type, parameters};
 }
 
 // Instantiates this Operation
 // Afterwards casting to StandardOperation can be done if assignment is total
 void SymbolicOperation::instantiate(const VariableAssignment& assignment) {
   for (std::size_t i = 0; i < symbolicParameter.size(); ++i) {
     parameter.at(i) = getInstantiation(getParameter(i), assignment);
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/GRCSParser.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/GRCSParser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/QASM3Parser.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/QASM3Parser.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
     return constInt->getUInt();
   }
 
 public:
   explicit OpenQasm3Parser(qc::QuantumComputation* quantumComputation)
       : typeCheckPass(&constEvalPass), qc(quantumComputation) {
-    for (auto [identifier, builtin] : initializeBuiltins()) {
+    for (const auto& [identifier, builtin] : initializeBuiltins()) {
       constEvalPass.addConst(identifier, builtin.first);
       typeCheckPass.addBuiltin(identifier, builtin.second);
     }
   }
 
   ~OpenQasm3Parser() override = default;
 
@@ -526,15 +526,15 @@
     if (broadcastingWidth == 1) {
       return applyQuantumOperation(gate, targetBits, controlBits,
                                    evaluatedParameters, invertOperation,
                                    gateCallStatement->debugInfo);
     }
 
     // if we are broadcasting, we need to create a compound operation
-    auto op = std::make_unique<qc::CompoundOperation>(qc->getNqubits());
+    auto op = std::make_unique<qc::CompoundOperation>();
     for (size_t j = 0; j < broadcastingWidth; ++j) {
       // first we apply the operation
       auto nestedOp = applyQuantumOperation(
           gate, targetBits, controlBits, evaluatedParameters, invertOperation,
           gateCallStatement->debugInfo);
       if (nestedOp == nullptr) {
         return nullptr;
@@ -598,15 +598,15 @@
   std::unique_ptr<qc::Operation> applyQuantumOperation(
       const std::shared_ptr<Gate>& gate, qc::Targets targetBits,
       std::vector<qc::Control> controlBits,
       std::vector<qc::fp> evaluatedParameters, bool invertOperation,
       const std::shared_ptr<DebugInfo>& debugInfo) {
     if (auto* standardGate = dynamic_cast<StandardGate*>(gate.get())) {
       auto op = std::make_unique<qc::StandardOperation>(
-          qc->getNqubits(), qc::Controls{}, targetBits, standardGate->info.type,
+          qc::Controls{}, targetBits, standardGate->info.type,
           evaluatedParameters);
       if (invertOperation) {
         op->invert();
       }
       op->setControls(qc::Controls{controlBits.begin(), controlBits.end()});
       return op;
     }
@@ -623,15 +623,15 @@
       for (const auto& qubitIdentifier : compoundGate->targetNames) {
         auto qubit = std::pair{targetBits[index], 1};
 
         nestedQubits.emplace(qubitIdentifier, qubit);
         index++;
       }
 
-      auto op = std::make_unique<qc::CompoundOperation>(qc->getNqubits());
+      auto op = std::make_unique<qc::CompoundOperation>();
       for (const auto& nestedGate : compoundGate->body) {
         if (auto barrierStatement =
                 std::dynamic_pointer_cast<BarrierStatement>(nestedGate);
             barrierStatement != nullptr) {
           // nothing to do here for the simulator.
         } else if (auto resetStatement =
                        std::dynamic_pointer_cast<ResetStatement>(nestedGate);
@@ -708,16 +708,15 @@
                 identifier + "' has " + std::to_string(bits.size()) +
                 " bits, but quantum register '" +
                 measureExpression->gate->identifier + "' has " +
                 std::to_string(qubits.size()) + " qubits.",
             debugInfo);
     }
 
-    auto op = std::make_unique<qc::NonUnitaryOperation>(qc->getNqubits(),
-                                                        qubits, bits);
+    auto op = std::make_unique<qc::NonUnitaryOperation>(qubits, bits);
     qc->emplace_back(std::move(op));
   }
 
   void visitBarrierStatement(
       const std::shared_ptr<BarrierStatement> barrierStatement) override {
     qc->emplace_back(getBarrierOp(barrierStatement, qc->getQregs()));
   }
@@ -774,15 +773,15 @@
       qc->emplace_back(std::make_unique<qc::ClassicControlledOperation>(
           elseOps, creg->second, rhs->getUInt(), invertedComparsionKind));
     }
   }
 
   [[nodiscard]] std::unique_ptr<qc::Operation> translateBlockOperations(
       const std::vector<std::shared_ptr<Statement>>& statements) {
-    auto blockOps = std::make_unique<qc::CompoundOperation>(qc->getNqubits());
+    auto blockOps = std::make_unique<qc::CompoundOperation>();
     for (const auto& statement : statements) {
       auto gateCall = std::dynamic_pointer_cast<GateCallStatement>(statement);
       if (gateCall == nullptr) {
         error("Only quantum statements are supported in blocks.",
               statement->debugInfo);
       }
       const auto& qregs = qc->getQregs();
@@ -793,34 +792,32 @@
 
       blockOps->emplace_back(std::move(op));
     }
 
     return blockOps;
   }
 
-  [[nodiscard]] std::unique_ptr<qc::Operation>
+  [[nodiscard]] static std::unique_ptr<qc::Operation>
   getBarrierOp(const std::shared_ptr<BarrierStatement>& barrierStatement,
-               const qc::QuantumRegisterMap& qregs) const {
+               const qc::QuantumRegisterMap& qregs) {
     std::vector<qc::Qubit> qubits{};
     for (const auto& gate : barrierStatement->gates) {
       translateGateOperand(gate, qubits, qregs, barrierStatement->debugInfo);
     }
 
-    return std::make_unique<qc::StandardOperation>(qc->getNqubits(), qubits,
-                                                   qc::Barrier);
+    return std::make_unique<qc::StandardOperation>(qubits, qc::Barrier);
   }
 
-  [[nodiscard]] std::unique_ptr<qc::Operation>
+  [[nodiscard]] static std::unique_ptr<qc::Operation>
   getResetOp(const std::shared_ptr<ResetStatement>& resetStatement,
-             const qc::QuantumRegisterMap& qregs) const {
+             const qc::QuantumRegisterMap& qregs) {
     std::vector<qc::Qubit> qubits{};
     translateGateOperand(resetStatement->gate, qubits, qregs,
                          resetStatement->debugInfo);
-    return std::make_unique<qc::NonUnitaryOperation>(qc->getNqubits(), qubits,
-                                                     qc::Reset);
+    return std::make_unique<qc::NonUnitaryOperation>(qubits, qc::Reset);
   }
 
   std::pair<std::string, size_t>
   parseGateIdentifierCompatMode(const std::string& identifier) {
     // we need to copy as we modify the string and need to return the original
     // string if we don't find a match.
     std::string gateIdentifier = identifier;
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/QCParser.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/QCParser.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -289,23 +289,23 @@
       controls.pop_back();
       mcx(Controls{controls.cbegin(), controls.cend()}, target);
     } else if (gate == H || gate == Y || gate == Z || gate == S ||
                gate == Sdg || gate == T || gate == Tdg) {
       const Qubit target = controls.back().qubit;
       controls.pop_back();
       emplace_back<StandardOperation>(
-          nqubits, Controls{controls.cbegin(), controls.cend()}, target, gate);
+          Controls{controls.cbegin(), controls.cend()}, target, gate);
     } else if (gate == SWAP) {
       const Qubit target0 = controls.back().qubit;
       controls.pop_back();
       const Qubit target1 = controls.back().qubit;
       controls.pop_back();
       mcswap(Controls{controls.cbegin(), controls.cend()}, target0, target1);
     } else if (gate == RX || gate == RY || gate == RZ) {
       const Qubit target = controls.back().qubit;
       controls.pop_back();
       emplace_back<StandardOperation>(
-          nqubits, Controls{controls.cbegin(), controls.cend()}, target, gate,
+          Controls{controls.cbegin(), controls.cend()}, target, gate,
           std::vector{lambda});
     }
   }
 }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/RealParser.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/RealParser.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -224,36 +224,35 @@
     case S:
     case Sdg:
     case T:
     case Tdg:
     case V:
     case Vdg:
       emplace_back<StandardOperation>(
-          nqubits, Controls{controls.cbegin(), controls.cend()}, target, gate);
+          Controls{controls.cbegin(), controls.cend()}, target, gate);
       break;
     case X:
       mcx(Controls{controls.cbegin(), controls.cend()}, target);
       break;
     case RX:
     case RY:
     case RZ:
     case P:
       emplace_back<StandardOperation>(
-          nqubits, Controls{controls.cbegin(), controls.cend()}, target, gate,
+          Controls{controls.cbegin(), controls.cend()}, target, gate,
           std::vector{PI / (lambda)});
       break;
     case SWAP:
     case Peres:
     case Peresdg:
     case iSWAP: {
       const auto target1 = controls.back().qubit;
       controls.pop_back();
       emplace_back<StandardOperation>(
-          nqubits, Controls{controls.cbegin(), controls.cend()}, target1,
-          target, gate);
+          Controls{controls.cbegin(), controls.cend()}, target1, target, gate);
       break;
     }
     default:
       std::cerr << "Unsupported operation encountered:  " << gate << "!\n";
       break;
     }
   }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/TFCParser.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/TFCParser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Parser.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Parser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Scanner.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Scanner.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 #include "parsers/qasm3_parser/Scanner.hpp"
 
+#include <cstdint>
+#include <istream>
+#include <optional>
 #include <regex>
+#include <sstream>
+#include <stdexcept>
+#include <string>
 
 namespace qasm3 {
 char Scanner::readUtf8Codepoint(std::istream* in) {
   char c = 0;
   in->get(c);
   return c;
 }
@@ -182,20 +188,34 @@
   const auto valBeforeDecimalSeparator = consumeNumberLiteral(base);
 
   if (ch == '.' || ch == 'e' || ch == 'E') {
     if (base != 10) {
       error("Float literals are only allowed in base 10");
     }
 
-    char const sep = ch;
-    nextCh();
-    auto valAfterDecimalSeparator = consumeNumberLiteral(base);
+    std::stringstream ss{};
+    ss << valBeforeDecimalSeparator;
+
+    if (ch == '.') {
+      ss << ch;
+      nextCh();
+      const auto valAfterDecimalSeparator = consumeNumberLiteral(base);
+      ss << valAfterDecimalSeparator;
+    }
 
-    std::stringstream ss;
-    ss << valBeforeDecimalSeparator << sep << valAfterDecimalSeparator;
+    if (ch == 'e' || ch == 'E') {
+      ss << ch;
+      nextCh();
+      if (ch == '+' || ch == '-') {
+        ss << ch;
+        nextCh();
+      }
+      const auto valAfterExponent = consumeNumberLiteral(base);
+      ss << valAfterExponent;
+    }
 
     try {
       t.valReal = std::stod(ss.str());
     } catch (std::invalid_argument&) {
       error("Unable to parse float literal");
     }
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Statement.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Statement.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/Types.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/Types.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/CMakeLists.txt` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/module.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/module.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_classic_controlled_operation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_classic_controlled_operation.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,15 @@
       "Returns the classical register controlling the operation.");
   ccop.def_property_readonly(
       "expected_value", &qc::ClassicControlledOperation::getExpectedValue,
       "Returns the expected value of the classical register.");
   ccop.def("__repr__", [](const qc::ClassicControlledOperation& op) {
     std::stringstream ss;
     const auto& controlReg = op.getControlRegister();
-    ss << "ClassicControlledOperation(<...op...>, "
-       << "control_register=(" << controlReg.first << ", " << controlReg.second
-       << "), "
+    ss << "ClassicControlledOperation(<...op...>, " << "control_register=("
+       << controlReg.first << ", " << controlReg.second << "), "
        << "expected_value=" << op.getExpectedValue() << ")";
     return ss.str();
   });
 }
 
 } // namespace mqt
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_compound_operation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_compound_operation.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,24 @@
     }
     return i;
   };
 
   py::class_<qc::CompoundOperation, qc::Operation>(
       m, "CompoundOperation",
       "Quantum operation comprised of multiple sub-operations.")
-      .def(py::init<std::size_t>(), "nq"_a,
-           "Create an empty compound operation on `nq` qubits.")
-      .def(py::init([](std::size_t nq, std::vector<qc::Operation*>& ops) {
+      .def(py::init<>(), "Create an empty compound operation.")
+      .def(py::init([](std::vector<qc::Operation*>& ops) {
              std::vector<std::unique_ptr<qc::Operation>> uniqueOps;
              uniqueOps.reserve(ops.size());
              for (auto& op : ops) {
                uniqueOps.emplace_back(op->clone());
              }
-             return qc::CompoundOperation(nq, std::move(uniqueOps));
+             return qc::CompoundOperation(std::move(uniqueOps));
            }),
-           "nq"_a, "ops"_a,
-           "Create a compound operation from a list of operations.")
+           "ops"_a, "Create a compound operation from a list of operations.")
       .def("__len__", &qc::CompoundOperation::size,
            "Return number of sub-operations.")
       .def(
           "__getitem__",
           [&wrap](const qc::CompoundOperation& op, DiffType i) {
             i = wrap(i, op.size());
             return op.at(static_cast<SizeType>(i)).get();
@@ -68,12 +66,12 @@
           [](qc::CompoundOperation& compOp, const qc::Operation& op) {
             compOp.emplace_back(op.clone());
           },
           "op"_a, "Append operation op to the `CompoundOperation`.")
       .def("empty", &qc::CompoundOperation::empty)
       .def("__repr__", [](const qc::CompoundOperation& op) {
         std::stringstream ss;
-        ss << "CompoundOperation(" << op.getNqubits() << ", [...ops...])";
+        ss << "CompoundOperation([..." << op.size() << " ops...])";
         return ss.str();
       });
 }
 } // namespace mqt
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_control.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_control.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_non_unitary_operation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_non_unitary_operation.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 
 namespace mqt {
 
 void registerNonUnitaryOperation(py::module& m) {
   py::class_<qc::NonUnitaryOperation, qc::Operation>(
       m, "NonUnitaryOperation",
       "Non-unitary operations such as measurements and resets.")
-      .def(
-          py::init<std::size_t, std::vector<qc::Qubit>, std::vector<qc::Bit>>(),
-          "nq"_a, "targets"_a, "classics"_a,
-          "Create a multi-qubit measurement operation.")
-      .def(py::init<std::size_t, qc::Qubit, qc::Bit>(), "nq"_a, "target"_a,
-           "classic"_a,
+      .def(py::init<std::vector<qc::Qubit>, std::vector<qc::Bit>>(),
+           "targets"_a, "classics"_a,
+           "Create a multi-qubit measurement operation.")
+      .def(py::init<qc::Qubit, qc::Bit>(), "target"_a, "classic"_a,
            "Create a measurement operation that measures `target` into "
            "`classic`.")
-      .def(py::init<std::size_t, std::vector<qc::Qubit>, qc::OpType>(), "nq"_a,
-           "targets"_a, "op_type"_a = qc::OpType::Reset,
+      .def(py::init<std::vector<qc::Qubit>, qc::OpType>(), "targets"_a,
+           "op_type"_a = qc::OpType::Reset,
            "Create a multi-qubit reset operation.")
       .def_property_readonly(
           "classics",
           py::overload_cast<>(&qc::NonUnitaryOperation::getClassics,
                               py::const_),
           "Return the classical bits.")
       .def("__repr__", [](const qc::NonUnitaryOperation& op) {
         std::stringstream ss;
-        ss << "NonUnitaryOperation(" << op.getNqubits() << ", ";
+        ss << "NonUnitaryOperation(";
         const auto& targets = op.getTargets();
         if (targets.size() == 1U) {
           ss << "target=" << targets[0];
         } else {
           ss << "targets=[";
           for (const auto& target : targets) {
             ss << target << ", ";
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_operation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_operation.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,14 @@
            "Remove all controls from this operation.")
       .def(
           "remove_control",
           [](qc::Operation& op, const qc::Control& c) { op.removeControl(c); },
           "control"_a, "Remove a control from this operation.")
       .def("remove_controls", &qc::Operation::removeControls, "controls"_a,
            "Remove a list of controls from this operation.")
-      .def_property("num_qubits", &qc::Operation::getNqubits,
-                    &qc::Operation::setNqubits)
       .def("get_used_qubits", &qc::Operation::getUsedQubits,
            "Get the qubits used by the operation (both control and targets).")
       .def("acts_on", &qc::Operation::actsOn, "qubit"_a,
            "Check if the operation acts on the specified qubit.")
       .def_property(
           "parameter",
           [](const qc::Operation& op) { return op.getParameter(); },
@@ -73,20 +71,14 @@
                         const qc::Operation& other) { return op == other; })
       .def("__ne__", [](const qc::Operation& op,
                         const qc::Operation& other) { return op != other; })
       .def("__hash__",
            [](const qc::Operation& op) {
              return std::hash<qc::Operation>{}(op);
            })
-      .def("__str__",
-           [](const qc::Operation& op) {
-             std::ostringstream oss;
-             oss << op;
-             return oss.str();
-           })
       .def("__repr__", [](const qc::Operation& op) {
         std::ostringstream oss;
-        oss << op;
+        oss << "Operation(type=" << op.getType() << ", ...)";
         return oss.str();
       });
 }
 } // namespace mqt
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_optype.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_optype.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_standard_operation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_standard_operation.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -9,57 +9,50 @@
       "Standard quantum operation. "
       "This class is used to represent all standard operations, i.e. "
       "operations that can be represented by a single gate. "
       "This includes all single qubit gates, as well as multi-qubit gates like "
       "CNOT, SWAP, etc. as well primitives like barriers.")
       .def(py::init<>(), "Create an empty standard operation. This is "
                          "equivalent to the identity gate.")
-      .def(py::init<std::size_t, qc::Qubit, qc::OpType, std::vector<qc::fp>,
-                    qc::Qubit>(),
-           "nq"_a, "target"_a, "op_type"_a, "params"_a = std::vector<qc::fp>{},
-           "starting_qubit"_a = 0,
+      .def(py::init<qc::Qubit, qc::OpType, std::vector<qc::fp>>(), "target"_a,
+           "op_type"_a, "params"_a = std::vector<qc::fp>{},
            "Create a single-qubit standard operation of specified type.")
-      .def(py::init<std::size_t, const qc::Targets&, qc::OpType,
-                    std::vector<qc::fp>, qc::Qubit>(),
-           "nq"_a, "targets"_a, "op_type"_a, "params"_a = std::vector<qc::fp>{},
-           "starting_qubit"_a = 0,
+      .def(py::init<const qc::Targets&, qc::OpType, std::vector<qc::fp>>(),
+           "targets"_a, "op_type"_a, "params"_a = std::vector<qc::fp>{},
            "Create a multi-qubit standard operation of specified type.")
-      .def(py::init<std::size_t, qc::Control, qc::Qubit, qc::OpType,
-                    const std::vector<qc::fp>&, qc::Qubit>(),
-           "nq"_a, "control"_a, "target"_a, "op_type"_a,
-           "params"_a = std::vector<qc::fp>{}, "starting_qubit"_a = 0,
+      .def(py::init<qc::Control, qc::Qubit, qc::OpType,
+                    const std::vector<qc::fp>&>(),
+           "control"_a, "target"_a, "op_type"_a,
+           "params"_a = std::vector<qc::fp>{},
            "Create a controlled standard operation of specified type.")
-      .def(py::init<std::size_t, qc::Control, const qc::Targets&, qc::OpType,
-                    const std::vector<qc::fp>&, qc::Qubit>(),
-           "nq"_a, "control"_a, "targets"_a, "op_type"_a,
-           "params"_a = std::vector<qc::fp>{}, "starting_qubit"_a = 0,
+      .def(py::init<qc::Control, const qc::Targets&, qc::OpType,
+                    const std::vector<qc::fp>&>(),
+           "control"_a, "targets"_a, "op_type"_a,
+           "params"_a = std::vector<qc::fp>{},
            "Create a controlled multi-target standard operation of specified "
            "type.")
-      .def(py::init<std::size_t, const qc::Controls&, qc::Qubit, qc::OpType,
-                    const std::vector<qc::fp>&, qc::Qubit>(),
-           "nq"_a, "controls"_a, "target"_a, "op_type"_a,
-           "params"_a = std::vector<qc::fp>{}, "starting_qubit"_a = 0,
+      .def(py::init<const qc::Controls&, qc::Qubit, qc::OpType,
+                    const std::vector<qc::fp>&>(),
+           "controls"_a, "target"_a, "op_type"_a,
+           "params"_a = std::vector<qc::fp>{},
            "Create a multi-controlled standard operation of specified type.")
-      .def(py::init<std::size_t, const qc::Controls&, const qc::Targets&,
-                    qc::OpType, std::vector<qc::fp>, qc::Qubit>(),
-           "nq"_a, "controls"_a, "targets"_a, "op_type"_a,
-           "params"_a = std::vector<qc::fp>{}, "starting_qubit"_a = 0,
+      .def(py::init<const qc::Controls&, const qc::Targets&, qc::OpType,
+                    std::vector<qc::fp>>(),
+           "controls"_a, "targets"_a, "op_type"_a,
+           "params"_a = std::vector<qc::fp>{},
            "Create a multi-controlled multi-target standard operation of "
            "specified type.")
-      .def(py::init<std::size_t, const qc::Controls&, qc::Qubit, qc::Qubit>(),
-           "nq"_a, "controls"_a, "target"_a, "starting_qubit"_a = 0,
-           "Create a multi-controlled X operation.")
-      .def(py::init<std::size_t, const qc::Controls&, qc::Qubit, qc::Qubit,
-                    qc::OpType, std::vector<qc::fp>, qc::Qubit>(),
-           "nq"_a, "controls"_a, "target0"_a, "target1"_a, "op_type"_a,
-           "params"_a = std::vector<qc::fp>{}, "starting_qubit"_a = 0,
+      .def(py::init<const qc::Controls&, qc::Qubit, qc::Qubit, qc::OpType,
+                    std::vector<qc::fp>>(),
+           "controls"_a, "target0"_a, "target1"_a, "op_type"_a,
+           "params"_a = std::vector<qc::fp>{},
            "Create a multi-controlled two-target operation of specified type.")
       .def("__repr__", [](const qc::StandardOperation& op) {
         std::stringstream ss;
-        ss << "StandardOperation(" << op.getNqubits() << ", ";
+        ss << "StandardOperation(";
         const auto& controls = op.getControls();
         if (controls.size() == 1U) {
           ss << "control=";
           const auto& control = *controls.begin();
           ss << control.toString() << ", ";
         } else if (!controls.empty()) {
           ss << "controls={";
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/operations/register_symbolic_operation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/operations/register_symbolic_operation.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -6,69 +6,60 @@
 void registerSymbolicOperation(py::module& m) {
   py::class_<qc::SymbolicOperation, qc::StandardOperation>(
       m, "SymbolicOperation",
       "Class representing a symbolic operation."
       "This encompasses all symbolic versions of `StandardOperation` that "
       "involve (float) angle parameters.")
       .def(py::init<>(), "Create an empty symbolic operation.")
-      .def(py::init<std::size_t, qc::Qubit, qc::OpType,
-                    const std::vector<qc::SymbolOrNumber>&, qc::Qubit>(),
-           "nq"_a, "target"_a, "op_type"_a,
+      .def(py::init<qc::Qubit, qc::OpType,
+                    const std::vector<qc::SymbolOrNumber>&>(),
+           "target"_a, "op_type"_a,
            "params"_a = std::vector<qc::SymbolOrNumber>{},
-           "starting_qubit"_a = 0,
            "Create a symbolic operation acting on a single qubit."
            "Params is a list of parameters that can be either `Expression` or "
            "`float`.")
-      .def(py::init<std::size_t, const qc::Targets&, qc::OpType,
-                    const std::vector<qc::SymbolOrNumber>&, qc::Qubit>(),
-           "nq"_a, "targets"_a, "op_type"_a,
+      .def(py::init<const qc::Targets&, qc::OpType,
+                    const std::vector<qc::SymbolOrNumber>&>(),
+           "targets"_a, "op_type"_a,
            "params"_a = std::vector<qc::SymbolOrNumber>{},
-           "starting_qubit"_a = 0,
            "Create a symbolic operation acting on multiple qubits."
            "Params is a list of parameters that can be either `Expression` or "
            "`float`.")
-      .def(py::init<std::size_t, qc::Control, qc::Qubit, qc::OpType,
-                    const std::vector<qc::SymbolOrNumber>&, qc::Qubit>(),
-           "nq"_a, "control"_a, "target"_a, "op_type"_a,
+      .def(py::init<qc::Control, qc::Qubit, qc::OpType,
+                    const std::vector<qc::SymbolOrNumber>&>(),
+           "control"_a, "target"_a, "op_type"_a,
            "params"_a = std::vector<qc::SymbolOrNumber>{},
-           "starting_qubit"_a = 0,
            "Create a controlled symbolic operation."
            "Params is a list of parameters that can be either `Expression` or "
            "`float`.")
-      .def(py::init<std::size_t, qc::Control, const qc::Targets&, qc::OpType,
-                    const std::vector<qc::SymbolOrNumber>&, qc::Qubit>(),
-           "nq"_a, "control"_a, "targets"_a, "op_type"_a,
+      .def(py::init<qc::Control, const qc::Targets&, qc::OpType,
+                    const std::vector<qc::SymbolOrNumber>&>(),
+           "control"_a, "targets"_a, "op_type"_a,
            "params"_a = std::vector<qc::SymbolOrNumber>{},
-           "starting_qubit"_a = 0,
            "Create a controlled multi-target symbolic operation."
            "Params is a list of parameters that can be either `Expression` or "
            "`float`.")
-      .def(py::init<std::size_t, const qc::Controls&, qc::Qubit, qc::OpType,
-                    const std::vector<qc::SymbolOrNumber>&, qc::Qubit>(),
-           "nq"_a, "controls"_a, "target"_a, "op_type"_a,
+      .def(py::init<const qc::Controls&, qc::Qubit, qc::OpType,
+                    const std::vector<qc::SymbolOrNumber>&>(),
+           "controls"_a, "target"_a, "op_type"_a,
            "params"_a = std::vector<qc::SymbolOrNumber>{},
-           "starting_qubit"_a = 0,
            "Create a multi-controlled symbolic operation."
            "Params is a list of parameters that can be either `Expression` or "
            "`float`.")
-      .def(py::init<std::size_t, const qc::Controls&, const qc::Targets&,
-                    qc::OpType, const std::vector<qc::SymbolOrNumber>&,
-                    qc::Qubit>(),
-           "nq"_a, "controls"_a, "targets"_a, "op_type"_a,
+      .def(py::init<const qc::Controls&, const qc::Targets&, qc::OpType,
+                    const std::vector<qc::SymbolOrNumber>&>(),
+           "controls"_a, "targets"_a, "op_type"_a,
            "params"_a = std::vector<qc::SymbolOrNumber>{},
-           "starting_qubit"_a = 0,
            "Create a multi-controlled multi-target symbolic operation."
            "Params is a list of parameters that can be either `Expression` or "
            "`float`.")
-      .def(py::init<std::size_t, const qc::Controls&, qc::Qubit, qc::Qubit,
-                    qc::OpType, const std::vector<qc::SymbolOrNumber>&,
-                    qc::Qubit>(),
-           "nq"_a, "controls"_a, "target0"_a, "target1"_a, "op_type"_a,
+      .def(py::init<const qc::Controls&, qc::Qubit, qc::Qubit, qc::OpType,
+                    const std::vector<qc::SymbolOrNumber>&>(),
+           "controls"_a, "target0"_a, "target1"_a, "op_type"_a,
            "params"_a = std::vector<qc::SymbolOrNumber>{},
-           "starting_qubit"_a = 0,
            "Create a multi-controlled two-target symbolic operation."
            "Params is a list of parameters that can be either `Expression` or "
            "`float`.")
       .def("get_parameter", &qc::SymbolicOperation::getParameter)
       .def("get_parameters", &qc::SymbolicOperation::getParameters)
       .def("get_instantiated_operation",
            &qc::SymbolicOperation::getInstantiatedOperation,
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/qiskit/QuantumCircuit.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/qiskit/QuantumCircuit.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,22 @@
                             "rzx",        "rzz",      "xx_minus_yy",
                             "xx_plus_yy"};
 
   auto instructionName = instruction.attr("name").cast<std::string>();
   if (instructionName == "measure") {
     auto control = qubitMap[qargs[0]].cast<Qubit>();
     auto target = clbitMap[cargs[0]].cast<std::size_t>();
-    qc.emplace_back<NonUnitaryOperation>(qc.getNqubits(), control, target);
+    qc.emplace_back<NonUnitaryOperation>(control, target);
   } else if (instructionName == "barrier") {
     Targets targets{};
     for (const auto qubit : qargs) {
       auto target = qubitMap[qubit].cast<Qubit>();
       targets.emplace_back(target);
     }
-    qc.emplace_back<StandardOperation>(qc.getNqubits(), targets, Barrier);
+    qc.emplace_back<StandardOperation>(targets, Barrier);
   } else if (instructionName == "reset") {
     Targets targets{};
     for (const auto qubit : qargs) {
       auto target = qubitMap[qubit].cast<Qubit>();
       targets.emplace_back(target);
     }
     qc.reset(targets);
@@ -219,16 +219,16 @@
     }
   } else {
     try {
       importDefinition(qc, instruction.attr("definition"), qargs, cargs,
                        qubitMap, clbitMap);
     } catch (py::error_already_set& e) {
       std::cerr << "Failed to import instruction " << instructionName
-                << " from Qiskit QuantumCircuit" << std::endl;
-      std::cerr << e.what() << std::endl;
+                << " from Qiskit QuantumCircuit\n";
+      std::cerr << e.what() << "\n";
     }
   }
 }
 
 qc::SymbolOrNumber
 qc::qiskit::QuantumCircuit::parseSymbolicExpr(const py::object& pyExpr) {
   static const std::regex SUMMANDS("[+|-]?[^+-]+");
@@ -307,15 +307,15 @@
                                               qc::OpType type,
                                               const py::list& qargs,
                                               const py::list& params,
                                               const py::dict& qubitMap) {
   std::vector<Control> qubits{};
   for (const auto qubit : qargs) {
     auto target = qubitMap[qubit].cast<Qubit>();
-    qubits.emplace_back(Control{target});
+    qubits.emplace_back(target);
   }
   auto target = qubits.back().qubit;
   qubits.pop_back();
   std::vector<qc::SymbolOrNumber> parameters{};
   for (const auto& param : params) {
     parameters.emplace_back(
         parseParam(py::reinterpret_borrow<py::object>(param)));
@@ -324,32 +324,30 @@
   if (std::all_of(parameters.cbegin(), parameters.cend(), [](const auto& p) {
         return std::holds_alternative<fp>(p);
       })) {
     std::vector<fp> fpParams{};
     std::transform(parameters.cbegin(), parameters.cend(),
                    std::back_inserter(fpParams),
                    [](const auto& p) { return std::get<fp>(p); });
-    qc.emplace_back<StandardOperation>(qc.getNqubits(), controls, target, type,
-                                       fpParams);
+    qc.emplace_back<StandardOperation>(controls, target, type, fpParams);
   } else {
-    qc.emplace_back<SymbolicOperation>(qc.getNqubits(), controls, target, type,
-                                       parameters);
+    qc.emplace_back<SymbolicOperation>(controls, target, type, parameters);
     for (const auto& p : parameters) {
       qc.addVariables(p);
     }
   }
 }
 
 void qc::qiskit::QuantumCircuit::addTwoTargetOperation(
     qc::QuantumComputation& qc, qc::OpType type, const py::list& qargs,
     const py::list& params, const py::dict& qubitMap) {
   std::vector<Control> qubits{};
   for (const auto qubit : qargs) {
     auto target = qubitMap[qubit].cast<Qubit>();
-    qubits.emplace_back(Control{target});
+    qubits.emplace_back(target);
   }
   auto target1 = qubits.back().qubit;
   qubits.pop_back();
   auto target0 = qubits.back().qubit;
   qubits.pop_back();
   std::vector<qc::SymbolOrNumber> parameters{};
   for (const auto& param : params) {
@@ -360,19 +358,19 @@
   if (std::all_of(parameters.cbegin(), parameters.cend(), [](const auto& p) {
         return std::holds_alternative<fp>(p);
       })) {
     std::vector<fp> fpParams{};
     std::transform(parameters.cbegin(), parameters.cend(),
                    std::back_inserter(fpParams),
                    [](const auto& p) { return std::get<fp>(p); });
-    qc.emplace_back<StandardOperation>(qc.getNqubits(), controls, target0,
-                                       target1, type, fpParams);
+    qc.emplace_back<StandardOperation>(controls, target0, target1, type,
+                                       fpParams);
   } else {
-    qc.emplace_back<SymbolicOperation>(qc.getNqubits(), controls, target0,
-                                       target1, type, parameters);
+    qc.emplace_back<SymbolicOperation>(controls, target0, target1, type,
+                                       parameters);
     for (const auto& p : parameters) {
       qc.addVariables(p);
     }
   }
 }
 
 void qc::qiskit::QuantumCircuit::importDefinition(
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/register_operations.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/register_operations.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/register_permutation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/register_permutation.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/register_quantum_computation.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/register_quantum_computation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,18 @@
   ///---------------------------------------------------------------------------
 
   qc.def_property("name", &qc::QuantumComputation::getName,
                   &qc::QuantumComputation::setName);
   qc.def_property_readonly("num_qubits", &qc::QuantumComputation::getNqubits);
   qc.def_property_readonly("num_ancilla_qubits",
                            &qc::QuantumComputation::getNancillae);
+  qc.def_property_readonly("num_garbage_qubits",
+                           &qc::QuantumComputation::getNgarbageQubits);
+  qc.def_property_readonly("num_measured_qubits",
+                           &qc::QuantumComputation::getNmeasuredQubits);
   qc.def_property_readonly("num_qubits_without_ancilla_qubits",
                            &qc::QuantumComputation::getNqubitsWithoutAncillae);
   qc.def_property_readonly("num_classical_bits",
                            &qc::QuantumComputation::getNcbits);
   qc.def_property_readonly("num_ops", &qc::QuantumComputation::getNops);
   qc.def("num_single_qubit_ops", &qc::QuantumComputation::getNsingleQubitOps,
          "Returns the number of single-qubit operations.");
@@ -215,21 +219,30 @@
   ///                  \n Ancillary and Garbage Handling \n
   ///---------------------------------------------------------------------------
 
   qc.def_readonly("ancillary", &qc::QuantumComputation::ancillary);
   qc.def("set_circuit_qubit_ancillary",
          &qc::QuantumComputation::setLogicalQubitAncillary, "q"_a,
          "Set the circuit's (logical) qubit q to be an ancillary qubit.");
+  qc.def("se_circuit_qubits_ancillary",
+         &qc::QuantumComputation::setLogicalQubitsAncillary, "q_min"_a,
+         "q_max"_a,
+         "Set the circuit's (logical) qubits q_min to q_max to be ancillary "
+         "qubits.");
   qc.def("is_circuit_qubit_ancillary",
          &qc::QuantumComputation::logicalQubitIsAncillary, "q"_a,
          "Check if the circuit's (logical) qubit q is an ancillary qubit.");
   qc.def_readonly("garbage", &qc::QuantumComputation::garbage);
   qc.def("set_circuit_qubit_garbage",
          &qc::QuantumComputation::setLogicalQubitGarbage, "q"_a,
          "Set the circuit's (logical) qubit q to be a garbage output.");
+  qc.def("set_circuit_qubits_garbage",
+         &qc::QuantumComputation::setLogicalQubitsGarbage, "q_min"_a, "q_max"_a,
+         "Set the circuit's (logical) qubits q_min to q_max to be garbage "
+         "outputs.");
   qc.def("is_circuit_qubit_garbage",
          &qc::QuantumComputation::logicalQubitIsGarbage, "q"_a,
          "Check if the circuit's (logical) qubit q is a garbage output.");
 
   ///---------------------------------------------------------------------------
   ///                    \n Symbolic Circuit Handling \n
   ///---------------------------------------------------------------------------
```

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/symbolic/register_expression.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/symbolic/register_expression.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/symbolic/register_term.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/symbolic/register_term.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/python/symbolic/register_variable.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/python/symbolic/register_variable.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/zx/CMakeLists.txt` & `mqt_qmap-2.5.1/extern/mqt-core/src/zx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/zx/FunctionalityConstruction.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/zx/FunctionalityConstruction.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/zx/Rational.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/zx/Rational.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/zx/Rules.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/zx/Rules.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/zx/Simplify.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/zx/Simplify.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/zx/Utils.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/zx/Utils.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/extern/mqt-core/src/zx/ZXDiagram.cpp` & `mqt_qmap-2.5.1/extern/mqt-core/src/zx/ZXDiagram.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/Architecture.hpp` & `mqt_qmap-2.5.1/include/Architecture.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/DataLogger.hpp` & `mqt_qmap-2.5.1/include/DataLogger.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/Mapper.hpp` & `mqt_qmap-2.5.1/include/Mapper.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/MappingResults.hpp` & `mqt_qmap-2.5.1/include/MappingResults.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/CliffordSynthesizer.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/CliffordSynthesizer.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/Configuration.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/Configuration.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/Results.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/Results.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/Tableau.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/Tableau.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/TargetMetric.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/TargetMetric.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/GateEncoder.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/GateEncoder.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/MultiGateEncoder.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/MultiGateEncoder.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/ObjectiveEncoder.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/ObjectiveEncoder.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/SATEncoder.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/SATEncoder.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/SingleGateEncoder.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/SingleGateEncoder.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/cliffordsynthesis/encoding/TableauEncoder.hpp` & `mqt_qmap-2.5.1/include/cliffordsynthesis/encoding/TableauEncoder.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/AvailableArchitecture.hpp` & `mqt_qmap-2.5.1/include/configuration/AvailableArchitecture.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/CommanderGrouping.hpp` & `mqt_qmap-2.5.1/include/configuration/CommanderGrouping.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/Configuration.hpp` & `mqt_qmap-2.5.1/include/configuration/Configuration.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/EarlyTermination.hpp` & `mqt_qmap-2.5.1/include/configuration/EarlyTermination.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/Encoding.hpp` & `mqt_qmap-2.5.1/include/configuration/Encoding.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/Heuristic.hpp` & `mqt_qmap-2.5.1/include/configuration/Heuristic.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/InitialLayout.hpp` & `mqt_qmap-2.5.1/include/configuration/InitialLayout.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/Layering.hpp` & `mqt_qmap-2.5.1/include/configuration/Layering.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/LookaheadHeuristic.hpp` & `mqt_qmap-2.5.1/include/configuration/LookaheadHeuristic.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/Method.hpp` & `mqt_qmap-2.5.1/include/configuration/Method.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/configuration/SwapReduction.hpp` & `mqt_qmap-2.5.1/include/configuration/SwapReduction.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/exact/ExactMapper.hpp` & `mqt_qmap-2.5.1/include/exact/ExactMapper.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/heuristic/HeuristicMapper.hpp` & `mqt_qmap-2.5.1/include/heuristic/HeuristicMapper.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/heuristic/UniquePriorityQueue.hpp` & `mqt_qmap-2.5.1/include/heuristic/UniquePriorityQueue.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/Encodings.hpp` & `mqt_qmap-2.5.1/include/logicblocks/Encodings.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/Logic.hpp` & `mqt_qmap-2.5.1/include/logicblocks/Logic.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/LogicBlock.hpp` & `mqt_qmap-2.5.1/include/logicblocks/LogicBlock.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/LogicTerm.hpp` & `mqt_qmap-2.5.1/include/logicblocks/LogicTerm.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/Model.hpp` & `mqt_qmap-2.5.1/include/logicblocks/Model.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/Z3Logic.hpp` & `mqt_qmap-2.5.1/include/logicblocks/Z3Logic.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/Z3Model.hpp` & `mqt_qmap-2.5.1/include/logicblocks/Z3Model.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/logicblocks/util_logicblock.hpp` & `mqt_qmap-2.5.1/include/logicblocks/util_logicblock.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/include/utils.hpp` & `mqt_qmap-2.5.1/include/utils.hpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/noxfile.py` & `mqt_qmap-2.5.1/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Nox sessions."""
 
 from __future__ import annotations
 
 import argparse
 import os
+import shutil
 import sys
 from typing import TYPE_CHECKING
 
 import nox
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
+nox.needs_version = ">=2024.3.2"
+nox.options.default_venv_backend = "uv|virtualenv"
+
 nox.options.sessions = ["lint", "tests"]
 
 PYTHON_ALL_VERSIONS = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 BUILD_REQUIREMENTS = [
     "scikit-build-core[pyproject]>=0.8.1",
     "setuptools_scm>=7",
-    "pybind11>=2.11",
+    "pybind11>=2.12",
 ]
 
 if os.environ.get("CI", None):
     nox.options.error_on_missing_interpreters = True
 
 
 @nox.session(reuse_venv=True)
@@ -42,14 +46,19 @@
 ) -> None:
     posargs = list(session.posargs)
     env = {"PIP_DISABLE_PIP_VERSION_CHECK": "1"}
 
     if os.environ.get("CI", None) and sys.platform == "win32":
         env["SKBUILD_CMAKE_ARGS"] = "-T ClangCL"
 
+    if shutil.which("cmake") is None and shutil.which("cmake3") is None:
+        session.install("cmake")
+    if shutil.which("ninja") is None:
+        session.install("ninja")
+
     _extras = ["test", *extras]
     if "--cov" in posargs:
         _extras.append("coverage")
         posargs.append("--cov-config=pyproject.toml")
 
     session.install(*BUILD_REQUIREMENTS, *install_args, env=env)
     install_arg = f"-ve.[{','.join(_extras)}]"
@@ -59,37 +68,35 @@
 
 @nox.session(reuse_venv=True, python=PYTHON_ALL_VERSIONS)
 def tests(session: nox.Session) -> None:
     """Run the test suite."""
     _run_tests(session)
 
 
-@nox.session()
+@nox.session(reuse_venv=True, venv_backend="uv")
 def minimums(session: nox.Session) -> None:
     """Test the minimum versions of dependencies."""
     _run_tests(
         session,
-        install_args=["--constraint=test/python/constraints.txt"],
+        install_args=["--resolution=lowest-direct"],
         run_args=["-Wdefault"],
+        extras=["qiskit", "evaluation"],
     )
-    session.run("pip", "list")
+    session.run("uv", "pip", "list")
 
 
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
-    """Build the docs. Pass "--serve" to serve. Pass "-b linkcheck" to check links."""
+    """Build the docs. Use "--non-interactive" to avoid serving. Pass "-b linkcheck" to check links."""
     parser = argparse.ArgumentParser()
-    parser.add_argument("--serve", action="store_true", help="Serve after building")
     parser.add_argument("-b", dest="builder", default="html", help="Build target (default: html)")
     args, posargs = parser.parse_known_args(session.posargs)
 
-    if args.builder != "html" and args.serve:
-        session.error("Must not specify non-HTML builder with --serve")
-
-    extra_installs = ["sphinx-autobuild"] if args.serve else []
+    serve = args.builder == "html" and session.interactive
+    extra_installs = ["sphinx-autobuild"] if serve else []
     session.install(*BUILD_REQUIREMENTS, *extra_installs)
     session.install("--no-build-isolation", "-ve.[docs]")
     session.chdir("docs")
 
     if args.builder == "linkcheck":
         session.run("sphinx-build", "-b", "linkcheck", "source", "_build/linkcheck", *posargs)
         return
@@ -99,11 +106,11 @@
         "-T",  # full tracebacks
         f"-b={args.builder}",
         "source",
         f"_build/{args.builder}",
         *posargs,
     )
 
-    if args.serve:
+    if serve:
         session.run("sphinx-autobuild", *shared_args)
     else:
         session.run("sphinx-build", "--keep-going", *shared_args)
```

### Comparing `mqt_qmap-2.5.0/pyproject.toml` & `mqt_qmap-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["scikit-build-core>=0.8.1", "setuptools-scm>=7", "pybind11>=2.11"]
+requires = ["scikit-build-core>=0.8.1", "setuptools-scm>=7", "pybind11>=2.12"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "mqt.qmap"
 description = "A tool for Quantum Circuit Mapping"
 readme = "README.md"
 authors = [
@@ -35,21 +35,21 @@
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "qiskit[qasm3-import]>=1.0.0",
     "rustworkx[all]>=0.14.0",
     "importlib_resources>=5.0; python_version < '3.10'",
-    "typing_extensions>=4.2"
+    "typing_extensions>=4.6"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest>=7", "mqt.qcec>=2.4.5", "mqt.qmap[visualization]"]
-coverage = ["mqt.qmap[test]", "pytest-cov"]
+coverage = ["mqt.qmap[test]", "pytest-cov>=4"]
 docs = [
     "furo>=2023.08.17",
     "sphinx",
     "setuptools-scm>=7",
     "sphinxcontrib-bibtex>=2.4.2",
     "sphinx-copybutton",
     "sphinx-hoverxref",
@@ -215,15 +215,15 @@
     "T20",         # flake8-print
     "TCH",         # flake8-type-checking
     "TID",         # flake8-tidy-imports
     "TRY",         # tryceratops
     "UP",          # pyupgrade
     "YTT",         # flake8-2020
 ]
-extend-ignore = [
+ignore = [
     "ANN101",  # Missing type annotation for `self` in method
     "ANN102",  # Missing type annotation for `cls` in classmethod
     "ISC001",  # Conflicts with formatter
     "PLR09",   # Too many <...>
     "PLR2004", # Magic value used in comparison
     "PLC0415", # Import should be at top of file
     "PT004",   # Incorrect, just usefixtures instead.
```

### Comparing `mqt_qmap-2.5.0/src/Architecture.cpp` & `mqt_qmap-2.5.1/src/Architecture.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/CMakeLists.txt` & `mqt_qmap-2.5.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/DataLogger.cpp` & `mqt_qmap-2.5.1/src/DataLogger.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/Mapper.cpp` & `mqt_qmap-2.5.1/src/Mapper.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 // This file is part of the MQT QMAP library released under the MIT license.
 // See README.md or go to https://github.com/cda-tum/qmap for more information.
 //
 
 #include "Mapper.hpp"
 
 #include "CircuitOptimizer.hpp"
+#include "Definitions.hpp"
+#include "operations/CompoundOperation.hpp"
 
+#include <cassert>
+#include <cmath>
 #include <utility>
 
 void Mapper::initResults() {
   countGates(qc, results.input);
   results.input.name    = qc.getName();
   results.input.qubits  = static_cast<std::uint16_t>(qc.getNqubits());
   results.architecture  = architecture->getName();
```

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/CliffordSynthesizer.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/CliffordSynthesizer.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/Tableau.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/Tableau.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/GateEncoder.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/GateEncoder.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
   for (std::size_t q = 0U; q < N; ++q) {
     for (const auto gate : SINGLE_QUBIT_GATES) {
       if (gate == qc::OpType::None) {
         continue;
       }
       if (model.getBoolValue(singleQubitGates[gateToIndex(gate)][q],
                              lb.get())) {
-        qc.emplace_back<qc::StandardOperation>(N, q, gate);
+        qc.emplace_back<qc::StandardOperation>(q, gate);
         ++nSingleQubitGates;
         PLOG_DEBUG << toString(gate) << "(" << q << ")";
       }
     }
   }
 }
 
@@ -207,15 +207,15 @@
     for (std::size_t trgt = 0U; trgt < N; ++trgt) {
       if (ctrl == trgt) {
         continue;
       }
       const auto control =
           qc::Control{static_cast<qc::Qubit>(ctrl), qc::Control::Type::Pos};
       if (model.getBoolValue(twoQubitGates[ctrl][trgt], lb.get())) {
-        qc.emplace_back<qc::StandardOperation>(N, control, trgt, qc::OpType::X);
+        qc.cx(control, static_cast<qc::Qubit>(trgt));
         ++nTwoQubitGates;
         PLOG_DEBUG << "CX(" << ctrl << ", " << trgt << ")";
       }
     }
   }
 }
```

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/MultiGateEncoder.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/MultiGateEncoder.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/ObjectiveEncoder.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/ObjectiveEncoder.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/SATEncoder.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/SATEncoder.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/SingleGateEncoder.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/SingleGateEncoder.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/cliffordsynthesis/encoding/TableauEncoder.cpp` & `mqt_qmap-2.5.1/src/cliffordsynthesis/encoding/TableauEncoder.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/configuration/Configuration.cpp` & `mqt_qmap-2.5.1/src/configuration/Configuration.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/exact/ExactMapper.cpp` & `mqt_qmap-2.5.1/src/exact/ExactMapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 #include "exact/ExactMapper.hpp"
 
 #include "logicblocks/Encodings.hpp"
 #include "logicblocks/LogicBlock.hpp"
 #include "logicblocks/Model.hpp"
 #include "logicblocks/util_logicblock.hpp"
 
+#include <cassert>
+
 void ExactMapper::map(const Configuration& settings) {
   results.config     = settings;
   const auto& config = results.config;
 
   const std::chrono::high_resolution_clock::time_point start =
       std::chrono::high_resolution_clock::now();
   initResults();
@@ -275,16 +277,15 @@
       if (gate.singleQubit()) {
         if (settings.verbose) {
           std::cout << i << ": Added single qubit gate with target: "
                     << locations.at(gate.target) << "\n";
         }
 
         qcMapped.emplace_back<qc::StandardOperation>(
-            qcMapped.getNqubits(), locations.at(gate.target), op->getType(),
-            op->getParameter());
+            locations.at(gate.target), op->getType(), op->getParameter());
       } else {
         const Edge cnot = {locations.at(static_cast<std::size_t>(gate.control)),
                            locations.at(gate.target)};
 
         if (architecture->getCouplingMap().find(cnot) ==
             architecture->getCouplingMap().end()) {
           const Edge reverse = {cnot.second, cnot.first};
```

### Comparing `mqt_qmap-2.5.0/src/heuristic/HeuristicMapper.cpp` & `mqt_qmap-2.5.1/src/heuristic/HeuristicMapper.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 //
 // This file is part of the MQT QMAP library released under the MIT license.
 // See README.md or go to https://github.com/cda-tum/qmap for more information.
 //
 
 #include "heuristic/HeuristicMapper.hpp"
 
+#include "operations/StandardOperation.hpp"
 #include "utils.hpp"
 
 #include <algorithm>
+#include <cassert>
 #include <chrono>
 
 void HeuristicMapper::map(const Configuration& configuration) {
   if (configuration.dataLoggingEnabled()) {
     dataLogger = std::make_unique<DataLogger>(configuration.dataLoggingPath,
                                               *architecture, qc);
   }
@@ -39,28 +41,26 @@
   if (config.verbose) {
     printLocations(std::clog);
     printQubits(std::clog);
   }
 
   for (std::size_t i = 0; i < config.iterativeBidirectionalRoutingPasses; ++i) {
     if (config.verbose) {
-      std::clog << std::endl
-                << "Iterative bidirectional routing (forward pass " << i
-                << "):" << std::endl;
+      std::clog << "\nIterative bidirectional routing (forward pass " << i
+                << "):\n";
     }
     pseudoRouteCircuit(false);
     if (config.verbose) {
-      std::clog << std::endl
-                << "Iterative bidirectional routing (backward pass " << i
-                << "):" << std::endl;
+      std::clog << "\nIterative bidirectional routing (backward pass " << i
+                << "):\n";
     }
     pseudoRouteCircuit(true);
 
     if (config.verbose) {
-      std::clog << std::endl << "Main routing:" << std::endl;
+      std::clog << "\nMain routing:\n";
     }
   }
 
   routeCircuit();
 
   postMappingOptimizations(config);
   countGates(qcMapped, results.output);
@@ -384,15 +384,14 @@
           results.output.swaps++;
         } else if (swap.op == qc::Teleportation) {
           if (config.verbose) {
             std::clog << "TELE: " << swap.first << " <-> " << swap.second
                       << "\n";
           }
           qcMapped.emplace_back<qc::StandardOperation>(
-              qcMapped.getNqubits(),
               qc::Targets{static_cast<qc::Qubit>(swap.first),
                           static_cast<qc::Qubit>(swap.second),
                           static_cast<qc::Qubit>(swap.middleAncilla)},
               qc::Teleportation);
           results.output.teleportations++;
         }
         gateidx++;
@@ -407,22 +406,20 @@
             "Cast to StandardOperation not possible during mapping. Check that "
             "circuit contains only StandardOperations");
       }
 
       if (gate.singleQubit()) {
         if (locations.at(gate.target) == DEFAULT_POSITION) {
           qcMapped.emplace_back<qc::StandardOperation>(
-              qcMapped.getNqubits(), gate.target, op->getType(),
-              op->getParameter());
+              gate.target, op->getType(), op->getParameter());
           gatesToAdjust.push_back(gateidx);
           gateidx++;
         } else {
           qcMapped.emplace_back<qc::StandardOperation>(
-              qcMapped.getNqubits(), locations.at(gate.target), op->getType(),
-              op->getParameter());
+              locations.at(gate.target), op->getType(), op->getParameter());
           gateidx++;
         }
       } else {
         const Edge cnot = {
             locations.at(static_cast<std::uint16_t>(gate.control)),
             locations.at(gate.target)};
         if (!architecture->isEdgeConnected(cnot)) {
@@ -577,27 +574,27 @@
       config.automaticLayerSplits ? isLayerSplittable(layer) : false;
 
   while (!nodes.empty() &&
          (!validMapping ||
           nodes.top().getTotalCost() < bestDoneNode.getTotalFixedCost())) {
     if (splittable && expandedNodes >= config.automaticLayerSplitsNodeLimit) {
       if (config.dataLoggingEnabled()) {
-        qc::CompoundOperation compOp(architecture->getNqubits());
+        qc::CompoundOperation compOp{};
         for (const auto& gate : layers.at(layer)) {
           compOp.emplace_back(gate.op->clone());
         }
 
         dataLogger->logFinalizeLayer(layer, compOp, singleQubitMultiplicity,
                                      twoQubitMultiplicity, qubits, 0, 0, 0, 0,
                                      {}, {}, 0);
         dataLogger->splitLayer();
       }
       splitLayer(layer, *architecture);
       if (config.verbose) {
-        std::clog << "Split layer" << std::endl;
+        std::clog << "Split layer\n";
       }
       // recursively restart search with newly split layer
       // (step to the end of the circuit, if reverse mapping is active, since
       // the split layer is inserted in this direction, otherwise 1 layer would
       // be skipped)
       return aStarMap(reverse ? layer + 1 : layer, reverse);
     }
@@ -690,15 +687,15 @@
     }
 
     layerResultsIt->effectiveBranchingFactor = computeEffectiveBranchingRate(
         layerResultsIt->expandedNodes + 1, result.depth);
   }
 
   if (config.dataLoggingEnabled()) {
-    qc::CompoundOperation compOp(architecture->getNqubits());
+    qc::CompoundOperation compOp{};
     for (const auto& gate : layers.at(layer)) {
       compOp.emplace_back(gate.op->clone());
     }
 
     dataLogger->logFinalizeLayer(
         layer, compOp, singleQubitMultiplicities.at(layer),
         twoQubitMultiplicities.at(layer), qubits, result.id, result.costFixed,
```

### Comparing `mqt_qmap-2.5.0/src/logicblocks/CMakeLists.txt` & `mqt_qmap-2.5.1/src/logicblocks/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/logicblocks/Encodings.cpp` & `mqt_qmap-2.5.1/src/logicblocks/Encodings.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/logicblocks/LogicBlock.cpp` & `mqt_qmap-2.5.1/src/logicblocks/LogicBlock.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/logicblocks/LogicTerm.cpp` & `mqt_qmap-2.5.1/src/logicblocks/LogicTerm.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/logicblocks/Z3Logic.cpp` & `mqt_qmap-2.5.1/src/logicblocks/Z3Logic.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/logicblocks/Z3Model.cpp` & `mqt_qmap-2.5.1/src/logicblocks/Z3Model.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/__init__.py` & `mqt_qmap-2.5.1/src/mqt/qmap/__init__.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/clifford_synthesis.py` & `mqt_qmap-2.5.1/src/mqt/qmap/clifford_synthesis.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/compile.py` & `mqt_qmap-2.5.1/src/mqt/qmap/compile.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/libs/ibm_guadalupe_16.pickle` & `mqt_qmap-2.5.1/src/mqt/qmap/libs/ibm_guadalupe_16.pickle`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/libs/rigetti_16.pickle` & `mqt_qmap-2.5.1/src/mqt/qmap/libs/rigetti_16.pickle`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/load_architecture.py` & `mqt_qmap-2.5.1/src/mqt/qmap/load_architecture.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/load_calibration.py` & `mqt_qmap-2.5.1/src/mqt/qmap/load_calibration.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/pyqmap.pyi` & `mqt_qmap-2.5.1/src/mqt/qmap/pyqmap.pyi`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/qiskit/backend.py` & `mqt_qmap-2.5.1/src/mqt/qmap/qiskit/backend.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/subarchitectures.py` & `mqt_qmap-2.5.1/src/mqt/qmap/subarchitectures.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/visualization/search_visualizer.py` & `mqt_qmap-2.5.1/src/mqt/qmap/visualization/search_visualizer.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/mqt/qmap/visualization/visualize_search_graph.py` & `mqt_qmap-2.5.1/src/mqt/qmap/visualization/visualize_search_graph.py`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/python/CMakeLists.txt` & `mqt_qmap-2.5.1/src/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/python/bindings.cpp` & `mqt_qmap-2.5.1/src/python/bindings.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/src/utils.cpp` & `mqt_qmap-2.5.1/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `mqt_qmap-2.5.0/PKG-INFO` & `mqt_qmap-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.qmap
-Version: 2.5.0
+Version: 2.5.1
 Summary: A tool for Quantum Circuit Mapping
 Keywords: MQT quantum-computing design-automation compiler clifford-synthesis
 Author-Email: Lukas Burgholzer <lukas.burgholzer@tum.de>, Stefan Hillmich <stefan.hillmich@jku.at>, Tom Peham <tom.peham@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Chair for Design Automation, Technical University of Munich
         
@@ -47,20 +47,20 @@
 Project-URL: Documentation, https://mqt.readthedocs.io/projects/qmap
 Project-URL: Issues, https://github.com/cda-tum/mqt-qmap/issues
 Project-URL: Discussions, https://github.com/cda-tum/mqt-qmap/discussions
 Requires-Python: >=3.8
 Requires-Dist: qiskit[qasm3-import]>=1.0.0
 Requires-Dist: rustworkx[all]>=0.14.0
 Requires-Dist: importlib_resources>=5.0; python_version < "3.10"
-Requires-Dist: typing_extensions>=4.2
+Requires-Dist: typing_extensions>=4.6
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: mqt.qcec>=2.4.5; extra == "test"
 Requires-Dist: mqt.qmap[visualization]; extra == "test"
 Requires-Dist: mqt.qmap[test]; extra == "coverage"
-Requires-Dist: pytest-cov; extra == "coverage"
+Requires-Dist: pytest-cov>=4; extra == "coverage"
 Requires-Dist: furo>=2023.08.17; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: setuptools-scm>=7; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.4.2; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-hoverxref; extra == "docs"
 Requires-Dist: pybtex>=0.24; extra == "docs"
```

