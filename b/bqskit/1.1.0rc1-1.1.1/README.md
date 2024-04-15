# Comparing `tmp/bqskit-1.1.0rc1.tar.gz` & `tmp/bqskit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqskit-1.1.0rc1.tar", last modified: Wed Sep 13 21:53:13 2023, max compression
+gzip compressed data, was "bqskit-1.1.1.tar", last modified: Mon Dec 11 17:19:18 2023, max compression
```

## Comparing `bqskit-1.1.0rc1.tar` & `bqskit-1.1.1.tar`

### file list

```diff
@@ -1,359 +1,358 @@
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.161696 bqskit-1.1.0rc1/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2527 2022-09-19 11:52:09.000000 bqskit-1.1.0rc1/LICENSE
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4207 2023-09-13 21:53:29.161696 bqskit-1.1.0rc1/PKG-INFO
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2695 2023-09-10 23:46:44.000000 bqskit-1.1.0rc1/README.md
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.765023 bqskit-1.1.0rc1/bqskit/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2954 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.788357 bqskit-1.1.0rc1/bqskit/compiler/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1568 2023-09-08 14:08:35.000000 bqskit-1.1.0rc1/bqskit/compiler/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6212 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/compiler/basepass.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    61967 2023-09-13 13:30:17.000000 bqskit-1.1.0rc1/bqskit/compiler/compile.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    19188 2023-09-09 00:39:20.000000 bqskit-1.1.0rc1/bqskit/compiler/compiler.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8330 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/compiler/gateset.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4208 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/compiler/machine.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9072 2023-09-07 00:16:47.000000 bqskit-1.1.0rc1/bqskit/compiler/passdata.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      242 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/compiler/status.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1796 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/compiler/task.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3840 2023-09-13 01:56:41.000000 bqskit-1.1.0rc1/bqskit/compiler/workflow.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.791690 bqskit-1.1.0rc1/bqskit/exec/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1085 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/exec/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      685 2023-01-19 22:11:21.000000 bqskit-1.1.0rc1/bqskit/exec/results.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      575 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/exec/runner.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.795024 bqskit-1.1.0rc1/bqskit/exec/runners/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      461 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/exec/runners/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1238 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/exec/runners/ibmq.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12733 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/exec/runners/quest.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      675 2022-09-19 11:52:09.000000 bqskit-1.1.0rc1/bqskit/exec/runners/sim.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.801690 bqskit-1.1.0rc1/bqskit/ext/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1925 2023-09-11 14:08:52.000000 bqskit-1.1.0rc1/bqskit/ext/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.805024 bqskit-1.1.0rc1/bqskit/ext/cirq/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      256 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ext/cirq/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2221 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ext/cirq/models.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1208 2023-01-23 16:58:30.000000 bqskit-1.1.0rc1/bqskit/ext/cirq/translate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      810 2023-09-11 14:08:48.000000 bqskit-1.1.0rc1/bqskit/ext/honeywell.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.808357 bqskit-1.1.0rc1/bqskit/ext/pytket/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      270 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ext/pytket/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1269 2023-01-23 16:58:30.000000 bqskit-1.1.0rc1/bqskit/ext/pytket/translate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.811690 bqskit-1.1.0rc1/bqskit/ext/qiskit/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      348 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ext/qiskit/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1923 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ext/qiskit/models.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1219 2023-01-23 16:58:30.000000 bqskit-1.1.0rc1/bqskit/ext/qiskit/translate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      573 2023-09-11 14:05:02.000000 bqskit-1.1.0rc1/bqskit/ext/quantinuum.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.815024 bqskit-1.1.0rc1/bqskit/ext/qutip/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      263 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ext/qutip/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1279 2023-01-23 16:58:30.000000 bqskit-1.1.0rc1/bqskit/ext/qutip/translate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2281 2023-09-12 21:36:31.000000 bqskit-1.1.0rc1/bqskit/ext/rigetti.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1951 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ext/supermarq.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.828357 bqskit-1.1.0rc1/bqskit/ir/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2161 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)   113551 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/ir/circuit.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2845 2023-09-05 03:06:24.000000 bqskit-1.1.0rc1/bqskit/ir/gate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.841691 bqskit-1.1.0rc1/bqskit/ir/gates/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3222 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/ir/gates/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1158 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/barrier.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5017 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/circuitgate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.851691 bqskit-1.1.0rc1/bqskit/ir/gates/composed/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      595 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composed/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    17293 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composed/controlled.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3646 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composed/daggergate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12811 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composed/embedded.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7242 2023-09-11 14:11:23.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composed/frozenparam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3144 2023-01-19 20:43:03.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composed/tagged.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7673 2022-10-27 12:13:07.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composed/vlg.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2308 2023-08-31 14:34:47.000000 bqskit-1.1.0rc1/bqskit/ir/gates/composedgate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.895025 bqskit-1.1.0rc1/bqskit/ir/gates/constant/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2838 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      915 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/b.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1260 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/ccx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      915 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/ch.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1451 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/clock.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1313 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/cpi.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      748 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/cs.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2360 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/csum.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      812 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/ct.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      798 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/cx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      751 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/cy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      749 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/cz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2654 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/h.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2299 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/identity.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1126 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/iswap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1472 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/itoffoli.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2036 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/pd.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1463 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/permutation.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2093 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/rccx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      561 2023-08-30 12:25:06.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/s.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      576 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/sdg.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1812 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/shift.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      922 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/sqrtcnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      952 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/sqrtiswap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4827 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/subswap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1715 2023-01-23 16:58:30.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/swap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      786 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/sx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      845 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/sycamore.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      620 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/t.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      635 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/tdg.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1163 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/unitary.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      604 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/x.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1076 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/xx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      608 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/y.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1072 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/yy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      606 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/z.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1100 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constant/zz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1816 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/constantgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1355 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/generalgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2420 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/measure.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.925026 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2033 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2518 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ccp.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3335 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ckm.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3356 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ckmd.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1820 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cp.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2524 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cphase.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2005 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/crx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1998 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cry.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1970 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/crz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3439 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cu.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2444 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/fsim.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3411 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/pauli.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2772 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/phasedxz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5347 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rsu3.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2415 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2903 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rxx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2402 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ry.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2239 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ryy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1754 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2052 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rzz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2212 2023-03-22 18:11:26.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u1.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2276 2023-09-11 14:08:08.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u1q.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2118 2022-08-31 17:16:53.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u2.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3997 2023-09-05 03:06:24.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u3.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7452 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u8.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3135 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/unitary.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      354 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/qubitgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      532 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/gates/quditgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      357 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/gates/qutritgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6710 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/interval.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13048 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/iterator.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.928359 bqskit-1.1.0rc1/bqskit/ir/lang/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      517 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/lang/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      615 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/lang/language.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.935026 bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      344 2022-08-17 01:47:54.000000 bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2666 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/parser.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1194 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/qasm2.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    31359 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/visitor.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7090 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/location.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5179 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/ir/operation.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.938359 bqskit-1.1.0rc1/bqskit/ir/opt/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1501 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/opt/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.945026 bqskit-1.1.0rc1/bqskit/ir/opt/cost/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1108 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2284 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/differentiable.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1147 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/function.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.948359 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      563 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.948359 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/cost/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      288 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/cost/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1541 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.951692 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/residuals/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      318 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/residuals/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1602 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2258 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/generator.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1391 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/cost/residual.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6696 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/instantiater.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.955026 bqskit-1.1.0rc1/bqskit/ir/opt/instantiaters/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      382 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/instantiaters/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3027 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/instantiaters/minimization.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2763 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/ir/opt/instantiaters/qfactor.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1048 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/minimizer.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.961693 bqskit-1.1.0rc1/bqskit/ir/opt/minimizers/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      339 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/opt/minimizers/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1802 2023-02-28 01:32:46.000000 bqskit-1.1.0rc1/bqskit/ir/opt/minimizers/ceres.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      471 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/minimizers/lbfgs.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1020 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/minimizers/scipy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1217 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/multistartgen.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.965026 bqskit-1.1.0rc1/bqskit/ir/opt/multistartgens/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      293 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/opt/multistartgens/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1953 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/multistartgens/diagonal.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1826 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/ir/opt/multistartgens/random.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3477 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/point.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    14991 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/ir/region.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1828 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/ir/structure.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.971693 bqskit-1.1.0rc1/bqskit/passes/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    11915 2023-09-05 23:29:53.000000 bqskit-1.1.0rc1/bqskit/passes/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      790 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/alias.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.981693 bqskit-1.1.0rc1/bqskit/passes/control/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1900 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/control/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2346 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/dothendecide.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1681 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/dowhileloop.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    19272 2023-09-10 14:11:27.000000 bqskit-1.1.0rc1/bqskit/passes/control/foreach.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1960 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/ifthenelse.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3330 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/paralleldo.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1012 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.995026 bqskit-1.1.0rc1/bqskit/passes/control/predicates/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1505 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1201 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/andpredicate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1984 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/change.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2948 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/count.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2217 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/many.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1013 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/multi.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1027 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/notpredicate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1196 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/orpredicate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      739 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/physical.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2930 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/single.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1073 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/predicates/width.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1516 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/control/whileloop.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      919 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/passes/group.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.998360 bqskit-1.1.0rc1/bqskit/passes/io/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      466 2022-08-13 15:35:15.000000 bqskit-1.1.0rc1/bqskit/passes/io/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1740 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/io/checkpoint.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7234 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/io/intermediate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.008360 bqskit-1.1.0rc1/bqskit/passes/mapping/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1050 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1083 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/apply.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8564 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/embed.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.011693 bqskit-1.1.0rc1/bqskit/passes/mapping/layout/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      385 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/layout/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3220 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/layout/pam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2781 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/layout/sabre.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13590 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/pam.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.015027 bqskit-1.1.0rc1/bqskit/passes/mapping/placement/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      402 2023-07-13 16:33:54.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/placement/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2170 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/placement/greedy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1046 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/placement/trivial.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.021694 bqskit-1.1.0rc1/bqskit/passes/mapping/routing/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      367 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/routing/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1682 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/routing/pam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1297 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/routing/sabre.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    18683 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/sabre.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1214 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/setmodel.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9823 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/mapping/topology.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2310 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/measure.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      456 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/noop.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.028360 bqskit-1.1.0rc1/bqskit/passes/partitioning/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      641 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/passes/partitioning/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3250 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/partitioning/cluster.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8805 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/partitioning/greedy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13917 2023-09-05 23:29:53.000000 bqskit-1.1.0rc1/bqskit/passes/partitioning/quick.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13619 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/partitioning/scan.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1786 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/partitioning/single.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.038360 bqskit-1.1.0rc1/bqskit/passes/processing/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      632 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/processing/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6356 2023-09-10 16:02:02.000000 bqskit-1.1.0rc1/bqskit/passes/processing/exhaustive.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3388 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/passes/processing/iterative.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      413 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/processing/rebase.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5280 2023-09-10 16:02:07.000000 bqskit-1.1.0rc1/bqskit/passes/processing/scan.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5141 2023-09-10 16:02:13.000000 bqskit-1.1.0rc1/bqskit/passes/processing/substitute.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.041694 bqskit-1.1.0rc1/bqskit/passes/retarget/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      396 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/retarget/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6740 2023-09-10 16:02:19.000000 bqskit-1.1.0rc1/bqskit/passes/retarget/auto.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1421 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/retarget/general.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12903 2023-09-10 16:02:27.000000 bqskit-1.1.0rc1/bqskit/passes/retarget/two.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.058361 bqskit-1.1.0rc1/bqskit/passes/rules/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      710 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/passes/rules/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/rules/ch2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/rules/cnot2ch.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/rules/cnot2cy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/rules/cnot2cz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/rules/cy2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/rules/cz2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1567 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/rules/swap2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1018 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/rules/u3.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3421 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/rules/zxzxz.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.061694 bqskit-1.1.0rc1/bqskit/passes/search/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      731 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/passes/search/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2425 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/search/frontier.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      926 2023-08-30 13:33:56.000000 bqskit-1.1.0rc1/bqskit/passes/search/generator.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.075028 bqskit-1.1.0rc1/bqskit/passes/search/generators/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      810 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4173 2023-09-06 12:17:45.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/fourparam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2606 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/middleout.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8173 2023-09-05 23:29:53.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/seed.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7161 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/simple.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4850 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/single.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2358 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/stair.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5474 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/search/generators/wide.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1287 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/search/heuristic.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.081694 bqskit-1.1.0rc1/bqskit/passes/search/heuristics/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      368 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/passes/search/heuristics/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2737 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/search/heuristics/astar.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1115 2023-08-30 12:18:37.000000 bqskit-1.1.0rc1/bqskit/passes/search/heuristics/dijkstra.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1617 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/search/heuristics/greedy.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.095028 bqskit-1.1.0rc1/bqskit/passes/synthesis/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      771 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13559 2023-09-10 16:02:33.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/leap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4677 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/pas.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    10758 2023-09-10 16:02:50.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/qfast.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12979 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/qpredict.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9680 2023-09-10 16:02:58.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/qsearch.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1729 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/synthesis.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1230 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/synthesis/target.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.115028 bqskit-1.1.0rc1/bqskit/passes/util/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1104 2023-09-05 23:29:53.000000 bqskit-1.1.0rc1/bqskit/passes/util/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      618 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/compress.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5023 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/conversion.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1553 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/converttou3.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1759 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/converttovar.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4163 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/passes/util/extend.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2716 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/fill.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1940 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/log.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1019 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/random.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1403 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/record.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2024 2023-09-05 23:29:53.000000 bqskit-1.1.0rc1/bqskit/passes/util/structure.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      635 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/unfold.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1091 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/passes/util/update.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.118362 bqskit-1.1.0rc1/bqskit/qis/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2190 2023-09-10 15:21:26.000000 bqskit-1.1.0rc1/bqskit/qis/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    20134 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/qis/graph.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8060 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/qis/pauli.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4959 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/qis/permutation.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.125028 bqskit-1.1.0rc1/bqskit/qis/state/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      462 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/qis/state/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    14052 2023-09-05 03:06:24.000000 bqskit-1.1.0rc1/bqskit/qis/state/state.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      660 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/qis/state/statemap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3719 2023-09-04 21:07:24.000000 bqskit-1.1.0rc1/bqskit/qis/state/system.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.135028 bqskit-1.1.0rc1/bqskit/qis/unitary/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      808 2023-08-31 13:38:05.000000 bqskit-1.1.0rc1/bqskit/qis/unitary/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2310 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/qis/unitary/differentiable.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1282 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/qis/unitary/meta.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1739 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/qis/unitary/optimizable.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4714 2023-09-05 03:06:24.000000 bqskit-1.1.0rc1/bqskit/qis/unitary/unitary.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12154 2023-01-19 20:43:03.000000 bqskit-1.1.0rc1/bqskit/qis/unitary/unitarybuilder.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    15716 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/bqskit/qis/unitary/unitarymatrix.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.148362 bqskit-1.1.0rc1/bqskit/runtime/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6364 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      551 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/address.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3319 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/attached.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    22189 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/base.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    15713 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/detached.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      530 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/direction.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1659 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/future.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    11817 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/manager.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      441 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/message.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      379 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/result.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3734 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/task.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    25392 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/runtime/worker.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.155029 bqskit-1.1.0rc1/bqskit/utils/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      593 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/utils/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2342 2022-09-19 11:52:10.000000 bqskit-1.1.0rc1/bqskit/utils/cachedclass.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      408 2023-01-19 20:43:03.000000 bqskit-1.1.0rc1/bqskit/utils/docs.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5890 2023-09-07 00:24:46.000000 bqskit-1.1.0rc1/bqskit/utils/math.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      525 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/utils/random.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.158362 bqskit-1.1.0rc1/bqskit/utils/test/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      371 2022-08-13 15:35:16.000000 bqskit-1.1.0rc1/bqskit/utils/test/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13812 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/utils/test/strategies.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    20931 2023-09-10 16:15:26.000000 bqskit-1.1.0rc1/bqskit/utils/test/types.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5284 2023-08-30 12:18:38.000000 bqskit-1.1.0rc1/bqskit/utils/typing.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      217 2023-09-13 21:52:40.000000 bqskit-1.1.0rc1/bqskit/version.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:28.775023 bqskit-1.1.0rc1/bqskit.egg-info/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4207 2023-09-13 21:53:28.000000 bqskit-1.1.0rc1/bqskit.egg-info/PKG-INFO
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9924 2023-09-13 21:53:28.000000 bqskit-1.1.0rc1/bqskit.egg-info/SOURCES.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)        1 2023-09-13 21:53:28.000000 bqskit-1.1.0rc1/bqskit.egg-info/dependency_links.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      181 2023-09-13 21:53:28.000000 bqskit-1.1.0rc1/bqskit.egg-info/entry_points.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      142 2023-09-13 21:53:28.000000 bqskit-1.1.0rc1/bqskit.egg-info/requires.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)        7 2023-09-13 21:53:28.000000 bqskit-1.1.0rc1/bqskit.egg-info/top_level.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1090 2023-09-10 00:52:30.000000 bqskit-1.1.0rc1/pyproject.toml
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)       38 2023-09-13 21:53:29.161696 bqskit-1.1.0rc1/setup.cfg
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3027 2023-09-08 13:17:49.000000 bqskit-1.1.0rc1/setup.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-09-13 21:53:29.161696 bqskit-1.1.0rc1/tests/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6031 2022-09-19 11:52:11.000000 bqskit-1.1.0rc1/tests/test_conftest.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.327680 bqskit-1.1.1/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2527 2023-12-11 17:17:54.000000 bqskit-1.1.1/LICENSE
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4255 2023-12-11 17:20:13.324347 bqskit-1.1.1/PKG-INFO
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2695 2023-12-11 17:17:54.000000 bqskit-1.1.1/README.md
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:12.987677 bqskit-1.1.1/bqskit/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2954 2023-12-11 17:17:54.000000 bqskit-1.1.1/bqskit/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.007677 bqskit-1.1.1/bqskit/compiler/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1568 2023-12-11 17:17:54.000000 bqskit-1.1.1/bqskit/compiler/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     6212 2023-12-11 17:17:54.000000 bqskit-1.1.1/bqskit/compiler/basepass.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    65291 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/compile.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    19638 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/compiler.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     8330 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/gateset.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4214 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/machine.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     9542 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/passdata.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      242 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/status.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1796 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/task.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3835 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/compiler/workflow.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.011010 bqskit-1.1.1/bqskit/exec/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1085 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/exec/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      685 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/exec/results.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      575 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/exec/runner.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.017677 bqskit-1.1.1/bqskit/exec/runners/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      461 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/exec/runners/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1238 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/exec/runners/ibmq.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    12733 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/exec/runners/quest.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      675 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/exec/runners/sim.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.024344 bqskit-1.1.1/bqskit/ext/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2774 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.027677 bqskit-1.1.1/bqskit/ext/cirq/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      256 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/cirq/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2221 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/cirq/models.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1208 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/cirq/translate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      810 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/honeywell.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.031010 bqskit-1.1.1/bqskit/ext/pytket/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      270 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/pytket/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1269 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/pytket/translate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.034344 bqskit-1.1.1/bqskit/ext/qiskit/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      348 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/qiskit/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1923 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/qiskit/models.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1219 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/qiskit/translate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      573 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/quantinuum.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.034344 bqskit-1.1.1/bqskit/ext/qutip/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      263 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/qutip/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1279 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/qutip/translate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2281 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/rigetti.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1951 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ext/supermarq.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.047677 bqskit-1.1.1/bqskit/ir/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2161 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)   114034 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/circuit.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2845 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.057677 bqskit-1.1.1/bqskit/ir/gates/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3222 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1158 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/barrier.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5017 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/circuitgate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.064344 bqskit-1.1.1/bqskit/ir/gates/composed/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      595 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composed/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    17293 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composed/controlled.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3646 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composed/daggergate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    13455 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composed/embedded.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     7242 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composed/frozenparam.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3246 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composed/tagged.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     7673 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composed/vlg.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2308 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/composedgate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.104344 bqskit-1.1.1/bqskit/ir/gates/constant/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2838 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      915 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/b.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1260 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/ccx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      915 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/ch.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1421 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/clock.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1313 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/cpi.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      748 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/cs.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2330 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/csum.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      812 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/ct.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      798 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/cx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      751 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/cy.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      749 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/cz.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2631 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/h.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2299 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/identity.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1126 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/iswap.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1472 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/itoffoli.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2006 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/pd.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1463 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/permutation.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2093 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/rccx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      561 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/s.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      576 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/sdg.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1812 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/shift.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      922 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/sqrtcnot.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      952 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/sqrtiswap.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4827 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/subswap.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1715 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/swap.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      786 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/sx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      845 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/sycamore.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      620 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/t.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      635 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/tdg.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1163 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/unitary.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      604 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/x.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1076 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/xx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      608 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/y.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1072 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/yy.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      606 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/z.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1100 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constant/zz.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1816 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/constantgate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1355 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/generalgate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2420 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/measure.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.134345 bqskit-1.1.1/bqskit/ir/gates/parameterized/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2033 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2518 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/ccp.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3335 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/ckm.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3356 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/ckmd.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1820 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/cp.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2524 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/cphase.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2005 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/crx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1998 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/cry.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1970 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/crz.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3439 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/cu.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2389 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/fsim.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3411 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/pauli.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2772 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/phasedxz.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5347 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/rsu3.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2415 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/rx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2903 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/rxx.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2402 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/ry.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2239 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/ryy.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1754 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/rz.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2052 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/rzz.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2212 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/u1.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2276 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/u1q.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2118 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/u2.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3997 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/u3.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     7452 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/u8.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3135 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/parameterized/unitary.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      354 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/qubitgate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      532 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/quditgate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      357 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/gates/qutritgate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     6710 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/interval.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    13048 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/iterator.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.137678 bqskit-1.1.1/bqskit/ir/lang/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      517 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/lang/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      615 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/lang/language.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.141012 bqskit-1.1.1/bqskit/ir/lang/qasm2/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      344 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/lang/qasm2/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2666 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/lang/qasm2/parser.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1194 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/lang/qasm2/qasm2.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    31359 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/lang/qasm2/visitor.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     7090 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/location.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5179 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/operation.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.144345 bqskit-1.1.1/bqskit/ir/opt/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1501 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.151012 bqskit-1.1.1/bqskit/ir/opt/cost/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1108 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2284 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/differentiable.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1147 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/function.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.151012 bqskit-1.1.1/bqskit/ir/opt/cost/functions/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      563 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/functions/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.154345 bqskit-1.1.1/bqskit/ir/opt/cost/functions/cost/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      288 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/functions/cost/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1541 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.157678 bqskit-1.1.1/bqskit/ir/opt/cost/functions/residuals/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      318 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/functions/residuals/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1602 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2258 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/generator.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1391 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/cost/residual.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     6696 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/instantiater.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.161012 bqskit-1.1.1/bqskit/ir/opt/instantiaters/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      382 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/instantiaters/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4837 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/instantiaters/minimization.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2763 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/instantiaters/qfactor.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1048 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/minimizer.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.164345 bqskit-1.1.1/bqskit/ir/opt/minimizers/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      339 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/minimizers/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1802 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/minimizers/ceres.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      471 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/minimizers/lbfgs.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1020 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/minimizers/scipy.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1217 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/multistartgen.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.167678 bqskit-1.1.1/bqskit/ir/opt/multistartgens/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      293 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/multistartgens/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1953 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/multistartgens/diagonal.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1826 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/opt/multistartgens/random.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3477 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/point.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    14991 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/region.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1828 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/ir/structure.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.174345 bqskit-1.1.1/bqskit/passes/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    12894 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      790 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/alias.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.181012 bqskit-1.1.1/bqskit/passes/control/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1985 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2346 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/dothendecide.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1681 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/dowhileloop.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    20602 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/foreach.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1960 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/ifthenelse.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3330 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/paralleldo.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1012 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.194345 bqskit-1.1.1/bqskit/passes/control/predicates/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1505 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1201 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/andpredicate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1984 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/change.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2948 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/count.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2217 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/many.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1013 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/multi.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1027 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/notpredicate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1196 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/orpredicate.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      739 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/physical.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2930 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/single.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1073 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/predicates/width.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1516 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/control/whileloop.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      919 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/group.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.197679 bqskit-1.1.1/bqskit/passes/io/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      466 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/io/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1740 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/io/checkpoint.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     7234 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/io/intermediate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.207679 bqskit-1.1.1/bqskit/passes/mapping/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1060 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/apply.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     8646 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/embed.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.211012 bqskit-1.1.1/bqskit/passes/mapping/layout/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      385 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/layout/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3278 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/layout/pam.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2796 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/layout/sabre.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    15244 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/pam.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.214346 bqskit-1.1.1/bqskit/passes/mapping/placement/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      402 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/placement/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2170 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/placement/greedy.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1046 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/placement/trivial.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.217679 bqskit-1.1.1/bqskit/passes/mapping/routing/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      367 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/routing/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1458 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/routing/pam.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1116 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/routing/sabre.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    19281 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/sabre.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2500 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/setmodel.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     9823 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/topology.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4781 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/mapping/verify.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2310 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/measure.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      456 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/noop.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.221012 bqskit-1.1.1/bqskit/passes/partitioning/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      641 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/partitioning/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3250 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/partitioning/cluster.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     8805 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/partitioning/greedy.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    13917 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/partitioning/quick.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    13623 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/partitioning/scan.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1786 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/partitioning/single.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.227679 bqskit-1.1.1/bqskit/passes/processing/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      632 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/processing/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     6356 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/processing/exhaustive.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3388 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/processing/iterative.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      413 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/processing/rebase.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5280 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/processing/scan.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5141 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/processing/substitute.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.234346 bqskit-1.1.1/bqskit/passes/retarget/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      396 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/retarget/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     6740 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/retarget/auto.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1421 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/retarget/general.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    12903 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/retarget/two.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.244346 bqskit-1.1.1/bqskit/passes/rules/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      710 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/rules/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/rules/ch2cnot.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-12-11 17:17:55.000000 bqskit-1.1.1/bqskit/passes/rules/cnot2ch.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/rules/cnot2cy.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/rules/cnot2cz.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/rules/cy2cnot.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/rules/cz2cnot.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1567 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/rules/swap2cnot.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1018 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/rules/u3.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3421 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/rules/zxzxz.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.247679 bqskit-1.1.1/bqskit/passes/search/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      731 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2425 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/frontier.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      926 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generator.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.257679 bqskit-1.1.1/bqskit/passes/search/generators/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      810 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4292 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/fourparam.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2606 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/middleout.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     8173 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/seed.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     7161 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/simple.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4850 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/single.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2358 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/stair.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5474 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/generators/wide.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1287 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/heuristic.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.261013 bqskit-1.1.1/bqskit/passes/search/heuristics/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      368 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/heuristics/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2737 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/heuristics/astar.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1115 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/heuristics/dijkstra.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1617 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/search/heuristics/greedy.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.271013 bqskit-1.1.1/bqskit/passes/synthesis/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      771 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    13559 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/leap.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4677 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/pas.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    10758 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/qfast.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    12979 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/qpredict.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     9680 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/qsearch.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1729 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/synthesis.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1230 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/synthesis/target.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.284346 bqskit-1.1.1/bqskit/passes/util/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1104 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      618 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/compress.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5023 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/conversion.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1553 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/converttou3.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1759 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/converttovar.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4163 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/extend.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2716 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/fill.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1940 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/log.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1019 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/random.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1403 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/record.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2024 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/structure.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      635 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/unfold.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1091 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/passes/util/update.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.287680 bqskit-1.1.1/bqskit/qis/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2190 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    20134 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/graph.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     8060 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/pauli.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4959 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/permutation.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.294346 bqskit-1.1.1/bqskit/qis/state/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      462 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/state/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    14052 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/state/state.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      660 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/state/statemap.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3719 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/state/system.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.301013 bqskit-1.1.1/bqskit/qis/unitary/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      808 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/unitary/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2310 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/unitary/differentiable.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1282 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/unitary/meta.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1739 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/unitary/optimizable.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     4714 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/unitary/unitary.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    12154 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/unitary/unitarybuilder.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    16289 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/qis/unitary/unitarymatrix.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.314347 bqskit-1.1.1/bqskit/runtime/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     6409 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      551 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/address.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3332 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/attached.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    22194 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/base.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    15713 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/detached.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      530 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/direction.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1659 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/future.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    11828 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/manager.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      441 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/message.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      379 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/result.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3734 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/task.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    25392 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/runtime/worker.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.321013 bqskit-1.1.1/bqskit/utils/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      593 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     2342 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/cachedclass.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      408 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/docs.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     7056 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/math.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      525 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/random.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:13.324347 bqskit-1.1.1/bqskit/utils/test/
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      371 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/test/__init__.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    13812 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/test/strategies.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)    20931 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/test/types.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     5284 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/utils/typing.py
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)      210 2023-12-11 17:17:56.000000 bqskit-1.1.1/bqskit/version.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-12-11 17:20:12.994343 bqskit-1.1.1/bqskit.egg-info/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4255 2023-12-11 17:20:12.000000 bqskit-1.1.1/bqskit.egg-info/PKG-INFO
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9933 2023-12-11 17:20:12.000000 bqskit-1.1.1/bqskit.egg-info/SOURCES.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)        1 2023-12-11 17:20:12.000000 bqskit-1.1.1/bqskit.egg-info/dependency_links.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      181 2023-12-11 17:20:12.000000 bqskit-1.1.1/bqskit.egg-info/entry_points.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      142 2023-12-11 17:20:12.000000 bqskit-1.1.1/bqskit.egg-info/requires.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)        7 2023-12-11 17:20:12.000000 bqskit-1.1.1/bqskit.egg-info/top_level.txt
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     1096 2023-12-11 17:17:56.000000 bqskit-1.1.1/pyproject.toml
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)       38 2023-12-11 17:20:13.327680 bqskit-1.1.1/setup.cfg
+-rw-rw-r--   0 edyounis  (1000) edyounis  (1000)     3077 2023-12-11 17:17:56.000000 bqskit-1.1.1/setup.py
```

### Comparing `bqskit-1.1.0rc1/LICENSE` & `bqskit-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/PKG-INFO` & `bqskit-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqskit
-Version: 1.1.0rc1
+Version: 1.1.1
 Summary: Berkeley Quantum Synthesis Toolkit
 Home-page: https://github.com/BQSKit/bqskit
 Author: LBNL - BQSKit developers
 Author-email: edyounis@lbl.gov
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/BQSKit/bqskit/issues
 Project-URL: Source Code, https://github.com/BQSKit/bqskit
@@ -20,14 +20,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Typing :: Typed
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
```

### Comparing `bqskit-1.1.0rc1/README.md` & `bqskit-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/__init__.py` & `bqskit-1.1.1/bqskit/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/__init__.py` & `bqskit-1.1.1/bqskit/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/basepass.py` & `bqskit-1.1.1/bqskit/compiler/basepass.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/compile.py` & `bqskit-1.1.1/bqskit/compiler/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,19 @@
 from bqskit.passes.mapping.apply import ApplyPlacement
 from bqskit.passes.mapping.embed import EmbedAllPermutationsPass
 from bqskit.passes.mapping.layout.pam import PAMLayoutPass
 from bqskit.passes.mapping.layout.sabre import GeneralizedSabreLayoutPass
 from bqskit.passes.mapping.placement.greedy import GreedyPlacementPass
 from bqskit.passes.mapping.routing.pam import PAMRoutingPass
 from bqskit.passes.mapping.routing.sabre import GeneralizedSabreRoutingPass
+from bqskit.passes.mapping.setmodel import ExtractModelConnectivityPass
+from bqskit.passes.mapping.setmodel import RestoreModelConnevtivityPass
 from bqskit.passes.mapping.setmodel import SetModelPass
 from bqskit.passes.mapping.topology import SubtopologySelectionPass
+from bqskit.passes.mapping.verify import PAMVerificationSequence
 from bqskit.passes.measure import ExtractMeasurements
 from bqskit.passes.measure import RestoreMeasurements
 from bqskit.passes.noop import NOOPPass
 from bqskit.passes.partitioning.quick import QuickPartitioner
 from bqskit.passes.partitioning.single import GroupSingleQuditGatePass
 from bqskit.passes.processing.scan import ScanningGateRemovalPass
 from bqskit.passes.retarget.auto import AutoRebase2QuditGatePass
@@ -318,14 +321,23 @@
         >>> from bqskit import compile, Circuit, MachineModel
         >>> from bqskit.ir.gates import CZGate, RZGate, SqrtXGate
         >>> target_gate_set = {CZGate(), RZGate(), SqrtXGate()}
         >>> circuit = Circuit.from_file('input.qasm')
         >>> model = MachineModel(circuit.num_qudits, gate_set=target_gate_set)
         >>> compiled_circuit = compile(circuit, model, optimization_level=2)
 
+        You can also use pre-built models from the :obj:`~bqskit.ext` package
+        for common hardware. For example, to compile to the H1-1 machine
+        from Quantinuum:
+
+        >>> from bqskit import compile, Circuit
+        >>> from bqskit.ext import H1_1Model
+        >>> circuit = Circuit.from_file('input.qasm')
+        >>> compiled_circuit = compile(circuit, H1_1Model)
+
     Raises:
         ValueError: If the input is an empty iterable.
 
         ValueError: If the input (or any input) is larger than the model.
 
         ValueError: If either the input or the model has mixed radixes.
 
@@ -973,45 +985,57 @@
     max_synthesis_size: int = 3,
     error_threshold: float | None = None,
     error_sim_size: int = 8,
 ) -> Workflow:
     """
     Build standard workflow for circuit multi-qudit gate set retargeting.
 
-    This workflow assumes that SetModelPass will be run earlier in the full
-    workflow and doesn't add it in here.
+    Notes:
+        - This workflow assumes that SetModelPass will be run earlier in the
+          full workflow and doesn't add it in here.
+
+        - For the most part, circuit connectivity isn't a concern during
+          retargeting. However, if the circuit contains many-qudit (>= 3)
+          gates, then the workflow will not preserve connectivity during
+          the decomposition of those gates. If your input contains many-qudit
+          gates, consider following this with a mapping workflow.
     """
+
+    core_retarget_workflow = [
+        FillSingleQuditGatesPass(),
+        IfThenElsePass(
+            NotPredicate(MultiPhysicalPredicate()),
+            IfThenElsePass(
+                ManyQuditGatesPredicate(),
+                [
+                    ExtractModelConnectivityPass(),
+                    build_standard_search_synthesis_workflow(
+                        optimization_level,
+                        synthesis_epsilon,
+                    ),
+                    RestoreModelConnevtivityPass(),
+                ],
+                AutoRebase2QuditGatePass(3, 5),
+            ),
+            ScanningGateRemovalPass(
+                success_threshold=synthesis_epsilon,
+                collection_filter=_mq_gate_collection_filter,
+                instantiate_options=get_instantiate_options(optimization_level),
+            ),
+        ),
+    ]
+
     return Workflow(
         [
             IfThenElsePass(
                 NotPredicate(WidthPredicate(2)),
                 [
                     LogPass('Retargeting multi-qudit gates.'),
                     build_partitioning_workflow(
-                        [
-                            FillSingleQuditGatesPass(),
-                            IfThenElsePass(
-                                NotPredicate(MultiPhysicalPredicate()),
-                                IfThenElsePass(
-                                    ManyQuditGatesPredicate(),
-                                    build_standard_search_synthesis_workflow(
-                                        optimization_level,
-                                        synthesis_epsilon,
-                                    ),
-                                    AutoRebase2QuditGatePass(3, 5),
-                                ),
-                                ScanningGateRemovalPass(
-                                    success_threshold=synthesis_epsilon,
-                                    collection_filter=_mq_gate_collection_filter,  # noqa: E501
-                                    instantiate_options=get_instantiate_options(
-                                        optimization_level,
-                                    ),
-                                ),
-                            ),
-                        ],
+                        core_retarget_workflow,
                         max_synthesis_size,
                         None if error_threshold is None else error_sim_size,
                     ),
                 ],
             ),
         ], name='Multi Qudit Retargeting',
     )
@@ -1124,14 +1148,154 @@
             GreedyPlacementPass(),
             GeneralizedSabreLayoutPass(),
             GeneralizedSabreRoutingPass(),
         ], name='SABRE Mapping',
     )
 
 
+def build_seqpam_mapping_optimization_workflow(
+    optimization_level: int = 4,
+    synthesis_epsilon: float = 1e-8,
+    num_layout_passes: int = 3,
+    block_size: int = 3,
+    error_sim_size: int | None = None,
+) -> Workflow:
+    """
+    Build a Sequential-Permutation-Aware Mapping and Optimizing Workflow.
+
+    Note:
+        - This workflow assumes that SetModelPass will be run earlier in the
+          full workflow and doesn't add it in here.
+
+        - This will apply the placement found during the workflow. The
+        resulting circuit will be physically mapped.
+
+    Args:
+        optimization_level (int): The optimization level. See :func:`compile`
+            for more information.
+
+        synthesis_epsilon (float): The maximum distance between target
+            and circuit unitary allowed to declare successful synthesis.
+            Set to 0 for exact synthesis. (Default: 1e-8)
+
+        num_layout_passes (int): The number of layout forward and backward
+            passes to run. See :class:`PamLayoutPass` for more information.
+            (Default: 3)
+
+        block_size (int): The size of the blocks to partition into.
+            Warning, the number of permutation evaluated increases
+            factorially and the difficulty of each permutation increases
+            exponentially with this. (Default: 3)
+
+        error_sim_size (int | None): The size of the blocks to simulate
+            errors on. If None, then no error analysis is performed.
+            (Default: None)
+
+    Raises:
+        ValueError: If block_size < 2.
+
+        ValueError: If error_sim_size < block_size.
+    """
+    if not is_integer(block_size):
+        raise TypeError(
+            f'Expected block_size to be int, got {type(block_size)}.',
+        )
+
+    if block_size < 2:
+        raise ValueError(f'Expected block_size > 1, got {block_size}.')
+
+    if error_sim_size is not None and not is_integer(block_size):
+        raise TypeError(
+            f'Expected int for error_sim_size, got {type(error_sim_size)}.',
+        )
+
+    if error_sim_size is not None and error_sim_size < block_size:
+        raise ValueError(
+            f'Expected error_sim_size >= block_size, got {error_sim_size}.',
+        )
+
+    qsearch = QSearchSynthesisPass(
+        success_threshold=synthesis_epsilon,
+        instantiate_options=get_instantiate_options(optimization_level),
+    )
+
+    leap = LEAPSynthesisPass(
+        success_threshold=synthesis_epsilon,
+        min_prefix_size=9,
+        instantiate_options=get_instantiate_options(optimization_level),
+    )
+
+    if error_sim_size is not None:
+        post_pam_seq: BasePass = PAMVerificationSequence(error_sim_size)
+    else:
+        post_pam_seq = NOOPPass()
+
+    return Workflow(
+        IfThenElsePass(
+            NotPredicate(WidthPredicate(2)),
+            [
+                LogPass('Caching permutation-aware synthesis results.'),
+                ExtractModelConnectivityPass(),
+                QuickPartitioner(block_size),
+                ForEachBlockPass(
+                    IfThenElsePass(
+                        WidthPredicate(4),
+                        EmbedAllPermutationsPass(
+                            inner_synthesis=qsearch,
+                            input_perm=True,
+                            output_perm=False,
+                            vary_topology=False,
+                        ),
+                        EmbedAllPermutationsPass(
+                            inner_synthesis=leap,
+                            input_perm=True,
+                            output_perm=False,
+                            vary_topology=False,
+                        ),
+                    ),
+                ),
+                LogPass('Preoptimizing with permutation-aware mapping.'),
+                PAMRoutingPass(),
+                post_pam_seq,
+                UnfoldPass(),
+                RestoreModelConnevtivityPass(),
+
+                LogPass('Recaching permutation-aware synthesis results.'),
+                SubtopologySelectionPass(block_size),
+                QuickPartitioner(block_size),
+                ForEachBlockPass(
+                    IfThenElsePass(
+                        WidthPredicate(4),
+                        EmbedAllPermutationsPass(
+                            inner_synthesis=qsearch,
+                            input_perm=False,
+                            output_perm=True,
+                            vary_topology=True,
+                        ),
+                        EmbedAllPermutationsPass(
+                            inner_synthesis=leap,
+                            input_perm=False,
+                            output_perm=True,
+                            vary_topology=True,
+                        ),
+                    ),
+                ),
+                LogPass('Performing permutation-aware mapping.'),
+                ApplyPlacement(),
+                PAMLayoutPass(num_layout_passes),
+                PAMRoutingPass(0.1),
+                post_pam_seq,
+                ApplyPlacement(),
+                UnfoldPass(),
+            ],
+        ),
+        name='SeqPAM Mapping',
+    )
+
+
 def build_gate_deletion_optimization_workflow(
     optimization_level: int = 1,
     synthesis_epsilon: float = 1e-8,
     max_synthesis_size: int = 3,
     error_threshold: float | None = None,
     error_sim_size: int = 8,
     iterative: bool = False,
@@ -1366,97 +1530,28 @@
     model: MachineModel,
     synthesis_epsilon: float = 1e-8,
     max_synthesis_size: int = 3,
     error_threshold: float | None = None,
     error_sim_size: int = 8,
 ) -> list[BasePass]:
     """Build optimization Level 4 workflow for circuit compilation."""
-    if error_threshold is not None:
-        _logger.warning(
-            'Automated error upper bound calculated is not yet'
-            ' ready for opt level 4.',
-        )
-
     if max_synthesis_size > 3:
         _logger.warning(
             'It is currently recommended to set max_synthesis_size to 3'
             ' for optimization level 4. This may change in the future.',
         )
 
-    qsearch = QSearchSynthesisPass(
-        success_threshold=synthesis_epsilon,
-        instantiate_options=get_instantiate_options(4),
-    )
-    leap = LEAPSynthesisPass(
-        success_threshold=synthesis_epsilon,
-        min_prefix_size=9,
-        instantiate_options=get_instantiate_options(4),
-    )
-
     return [
-        SetModelPass(
-            MachineModel(
-                model.num_qudits,
-                None,
-                model.gate_set,
-                model.radixes,
-            ),
-        ),
-        Workflow(
-            IfThenElsePass(
-                NotPredicate(WidthPredicate(2)),
-                [
-                    QuickPartitioner(3),
-                    ForEachBlockPass(
-                        IfThenElsePass(
-                            WidthPredicate(4),
-                            EmbedAllPermutationsPass(
-                                inner_synthesis=qsearch,
-                                input_perm=True,
-                                output_perm=False,
-                                vary_topology=False,
-                            ),
-                            EmbedAllPermutationsPass(
-                                inner_synthesis=leap,
-                                input_perm=True,
-                                output_perm=False,
-                                vary_topology=False,
-                            ),
-                        ),
-                    ),
-                    PAMRoutingPass(),
-                    UnfoldPass(),
+        SetModelPass(model),
 
-                    SetModelPass(model),
-                    SubtopologySelectionPass(3),
-                    QuickPartitioner(3),
-                    ForEachBlockPass(
-                        IfThenElsePass(
-                            WidthPredicate(4),
-                            EmbedAllPermutationsPass(
-                                inner_synthesis=qsearch,
-                                input_perm=False,
-                                output_perm=True,
-                                vary_topology=True,
-                            ),
-                            EmbedAllPermutationsPass(
-                                inner_synthesis=leap,
-                                input_perm=False,
-                                output_perm=True,
-                                vary_topology=True,
-                            ),
-                        ),
-                    ),
-                    ApplyPlacement(),
-                    PAMLayoutPass(3),
-                    PAMRoutingPass(0.1),
-                    UnfoldPass(),
-                ],
-            ),
-            name='SeqPAM Mapping',
+        build_seqpam_mapping_optimization_workflow(
+            4,
+            synthesis_epsilon,
+            block_size=max_synthesis_size,
+            error_sim_size=None if error_threshold is None else error_sim_size,
         ),
 
         build_multi_qudit_retarget_workflow(
             4,
             synthesis_epsilon,
             max_synthesis_size,
             error_threshold,
```

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/compiler.py` & `bqskit-1.1.1/bqskit/compiler/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module implements the Compiler class."""
 from __future__ import annotations
 
 import atexit
 import functools
 import logging
-import os
 import signal
+import subprocess
 import sys
 import time
 import uuid
 import warnings
 from multiprocessing.connection import Client
 from multiprocessing.connection import Connection
 from subprocess import Popen
@@ -121,20 +121,24 @@
         Start an attached serer with `num_workers` workers.
 
         See :obj:`~bqskit.runtime.attached.AttachedServer` for more info.
         """
         params = f'{num_workers}, {runtime_log_level}, {worker_port=}'
         import_str = 'from bqskit.runtime.attached import start_attached_server'
         launch_str = f'{import_str}; start_attached_server({params})'
-        self.p = Popen([sys.executable, '-c', launch_str])
+        if sys.platform == 'win32':
+            flags = subprocess.CREATE_NEW_PROCESS_GROUP
+        else:
+            flags = 0
+        self.p = Popen([sys.executable, '-c', launch_str], creationflags=flags)
         _logger.debug('Starting runtime server process.')
 
     def _connect_to_server(self, ip: str, port: int) -> None:
         """Connect to a runtime server at `ip` and `port`."""
-        max_retries = 7
+        max_retries = 8
         wait_time = .25
         for _ in range(max_retries):
             try:
                 family = 'AF_INET' if sys.platform == 'win32' else None
                 conn = Client((ip, port), family)
             except ConnectionRefusedError:
                 time.sleep(wait_time)
@@ -179,34 +183,43 @@
                 _logger.debug('Disconnected from runtime server.')
             finally:
                 self.conn = None
 
         # Shutdown server if attached
         if self.p is not None and self.p.pid is not None:
             try:
-                os.kill(self.p.pid, signal.SIGINT)
-                _logger.debug('Interrupted attached runtime server.')
-
+                if sys.platform == 'win32':
+                    self.p.send_signal(signal.CTRL_C_EVENT)
+                else:
+                    self.p.send_signal(signal.SIGINT)
+                _logger.debug('Interrupting attached runtime server.')
                 self.p.communicate(timeout=1)
-                if self.p.returncode is None:
-                    if sys.platform == 'win32':
-                        self.p.terminate()
-                    else:
-                        os.kill(self.p.pid, signal.SIGKILL)
-                    _logger.debug('Killed attached runtime server.')
+
+            except subprocess.TimeoutExpired:
+                self.p.kill()
+                _logger.debug('Killing attached runtime server.')
+                try:
+                    self.p.communicate(timeout=30)
+                except subprocess.TimeoutExpired:
+                    _logger.warning(
+                        'Failed to kill attached runtime server.'
+                        ' It may still be running as a zombie process.',
+                    )
+                else:
+                    _logger.debug('Attached runtime server is down.')
 
             except Exception as e:
-                _logger.debug(
+                _logger.warning(
                     f'Error while shuting down attached runtime server: {e}.',
                 )
+
             else:
                 _logger.debug('Successfully shutdown attached runtime server.')
+
             finally:
-                self.p.communicate()
-                _logger.debug('Attached runtime server is down.')
                 self.p = None
 
         # Reset interrupt signal handler and remove exit handler
         if hasattr(self, 'old_signal'):
             signal.signal(signal.SIGINT, self.old_signal)
 
     def __del__(self) -> None:
```

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/gateset.py` & `bqskit-1.1.1/bqskit/compiler/gateset.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/machine.py` & `bqskit-1.1.1/bqskit/compiler/machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
                 to `num_qudits`. Each element specifies the base of a
                 qudit. Defaults to qubits.
 
         Raises:
             ValueError: If `num_qudits` is nonpositive.
 
         Note:
-            Pre-built models for many active QPUs exist in the `bqskit.ext`
-            package.
+            Pre-built models for many active QPUs exist in the
+            :obj:`~bqskit.ext` package.
         """
 
         if not is_integer(num_qudits):
             raise TypeError(
                 f'Expected integer num_qudits, got {type(num_qudits)}.',
             )
```

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/passdata.py` & `bqskit-1.1.1/bqskit/compiler/passdata.py`

 * *Files 9% similar despite different names*

```diff
@@ -142,15 +142,20 @@
                 'Cannot set placement. Expected a sequence of integers.',
             )
 
         self._placement = list(int(x) for x in _val)
 
     @property
     def initial_mapping(self) -> list[int]:
-        """Return the initial mapping of logical to physical qudits."""
+        """
+        Return the initial mapping of logical to physical qudits.
+
+        This always maps how the logical qudits from the original circuit start
+        on the physical qudits of the current circuit.
+        """
         return self._initial_mapping
 
     @initial_mapping.setter
     def initial_mapping(self, _val: Sequence[int]) -> None:
         if not is_sequence(_val):
             raise TypeError(
                 f'Cannot set initial_mapping to {type(_val)}.'
@@ -162,15 +167,20 @@
                 'Cannot set initial_mapping. Expected a sequence of integers.',
             )
 
         self._initial_mapping = list(int(x) for x in _val)
 
     @property
     def final_mapping(self) -> list[int]:
-        """Return the final mapping of logical to physical qudits."""
+        """
+        Return the final mapping of logical to physical qudits.
+
+        This always maps how the logical qudits from the original circuit end on
+        the physical qudits of the current circuit.
+        """
         return self._final_mapping
 
     @final_mapping.setter
     def final_mapping(self, _val: Sequence[int]) -> None:
         if not is_sequence(_val):
             raise TypeError(
                 f'Cannot set final_mapping to {type(_val)}.'
@@ -258,7 +268,11 @@
         else:
             self._target = copy.copy(other._target)
             self._error = copy.copy(other._error)
             self._model = copy.copy(other._model)
             self._placement = copy.copy(other._placement)
             self._data = copy.copy(other._data)
             self._seed = copy.copy(other._seed)
+
+    def update_error_mul(self, error: float) -> None:
+        """Update the error multiplicatively."""
+        self.error = (1 - ((1 - self.error) * (1 - error)))
```

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/task.py` & `bqskit-1.1.1/bqskit/compiler/task.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/compiler/workflow.py` & `bqskit-1.1.1/bqskit/compiler/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     def name(self) -> str:
         """The name of the pass."""
         return self._name or self.__class__.__name__
 
     def __str__(self) -> str:
         name_seq = f'Workflow: {self.name}\n\t'
         pass_strs = [
-            f'{i}. {"Workflow: " + p.name if isinstance(p, Workflow) else p}'
+            f'{i}. Workflow: {p.name if isinstance(p, Workflow) else p}'
             for i, p in enumerate(self._passes)
         ]
         return name_seq + '\n\t'.join(pass_strs)
 
     def __add__(self, other: WorkflowLike) -> Workflow:
         return Workflow(self._passes + Workflow(other)._passes)
```

### Comparing `bqskit-1.1.0rc1/bqskit/exec/__init__.py` & `bqskit-1.1.1/bqskit/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/exec/results.py` & `bqskit-1.1.1/bqskit/exec/results.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/exec/runner.py` & `bqskit-1.1.1/bqskit/exec/runner.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/exec/runners/ibmq.py` & `bqskit-1.1.1/bqskit/exec/runners/ibmq.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/exec/runners/quest.py` & `bqskit-1.1.1/bqskit/exec/runners/quest.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/exec/runners/sim.py` & `bqskit-1.1.1/bqskit/exec/runners/sim.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/cirq/models.py` & `bqskit-1.1.1/bqskit/ext/cirq/models.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/cirq/translate.py` & `bqskit-1.1.1/bqskit/ext/cirq/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/honeywell.py` & `bqskit-1.1.1/bqskit/ext/honeywell.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/pytket/translate.py` & `bqskit-1.1.1/bqskit/ext/pytket/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/qiskit/models.py` & `bqskit-1.1.1/bqskit/ext/qiskit/models.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/qiskit/translate.py` & `bqskit-1.1.1/bqskit/ext/qiskit/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/quantinuum.py` & `bqskit-1.1.1/bqskit/ext/quantinuum.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/qutip/translate.py` & `bqskit-1.1.1/bqskit/ext/qutip/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/rigetti.py` & `bqskit-1.1.1/bqskit/ext/rigetti.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ext/supermarq.py` & `bqskit-1.1.1/bqskit/ext/supermarq.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/__init__.py` & `bqskit-1.1.1/bqskit/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/circuit.py` & `bqskit-1.1.1/bqskit/ir/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1031,21 +1031,24 @@
             for i, cycle in enumerate(self._circuit[start[0]:end[0] + 1]):
                 for q, _op in enumerate(cycle[start[1]:end[1] + 1]):
                     if _op is not None and _op.gate == op:
                         return CircuitPoint(start[0] + i, start[1] + q)
 
         raise ValueError('No such operation exists in the circuit.')
 
-    def append(self, op: Operation) -> None:
+    def append(self, op: Operation) -> int:
         """
-        Append `op` to the end of the circuit.
+        Append `op` to the end of the circuit and return its cycle index.
 
         Args:
             op (Operation): The operation to append.
 
+        Returns:
+            int: The cycle index of the appended operation.
+
         Raises:
             ValueError: If `op` cannot be placed on the circuit due to
                 either an invalid location or gate radix mismatch.
 
         Notes:
             Due to the circuit being represented as a matrix,
             `circuit.append(op)` does not imply `op` is last in simulation
@@ -1089,49 +1092,54 @@
             self._graph_info[pair] += 1
 
         # Update _gate_info
         if op.gate not in self._gate_info:
             self._gate_info[op.gate] = 0
         self._gate_info[op.gate] += 1
 
+        return cycle_index
+
     def append_gate(
         self,
         gate: Gate,
         location: CircuitLocationLike,
         params: RealVector = [],
-    ) -> None:
+    ) -> int:
         """
         Append the gate object to the circuit on the qudits in location.
 
         Args:
             gate (Gate): The gate to append.
 
             location (CircuitLocationLike): Apply the gate to these qudits.
 
             params (RealVector): The gate's parameters.
                 (Default: all zeros)
 
+        Returns:
+            int: The cycle index of the appended gate.
+
         Examples:
             >>> from bqskit.ir.gates import HGate
             >>> circ = Circuit(1)
             >>> # Append a Hadamard gate to qudit 0.
             >>> circ.append_gate(HGate(), 0)
 
         See Also:
             :func:`append`
         """
-        self.append(Operation(gate, location, params))
+        return self.append(Operation(gate, location, params))
 
     def append_circuit(
         self,
         circuit: Circuit,
         location: CircuitLocationLike,
         as_circuit_gate: bool = False,
         move: bool = False,
-    ) -> None:
+    ) -> int:
         """
         Append `circuit` at the qudit location specified.
 
         Args:
             circuit (Circuit): The circuit to append.
 
             location (CircuitLocationLike): Apply the circuit to these qudits.
@@ -1139,14 +1147,18 @@
             as_circuit_gate (bool): If true, append `circuit` as a unit
                 block (CircuitGate) rather than each operation in `circuit`
                 individually. (Default: False)
 
             move (bool): Move circuit into circuit gate rather than copy.
                 (Default: False)
 
+        Returns:
+            int: The starting cycle index of the appended circuit. If the
+                appended circuit is empty, then this will be -1.
+
         Raises:
             ValueError: If `circuit` is not the same size as `location`.
 
         See Also:
             :func:`append`
         """
         if not isinstance(circuit, Circuit):
@@ -1161,20 +1173,25 @@
             raise TypeError(f'Expected bool, got: {type(as_circuit_gate)}.')
 
         if circuit.num_qudits != len(location):
             raise ValueError('Circuit and location size mismatch.')
 
         if as_circuit_gate:
             op = Operation(CircuitGate(circuit, move), location, circuit.params)
-            self.append(op)
-            return
+            return self.append(op)
+
+        cycle_index = -1
 
         for op in circuit:
             mapped_location = [location[q] for q in op.location]
-            self.append(Operation(op.gate, mapped_location, op.params))
+            ci = self.append(Operation(op.gate, mapped_location, op.params))
+            if cycle_index is None:
+                cycle_index = ci
+
+        return cycle_index
 
     def extend(self, ops: Iterable[Operation]) -> None:
         """
         Append all operations in `ops` to the circuit.
 
         Args:
             ops (Operation): The operations to append.
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gate.py` & `bqskit-1.1.1/bqskit/ir/gate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/__init__.py` & `bqskit-1.1.1/bqskit/ir/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/barrier.py` & `bqskit-1.1.1/bqskit/ir/gates/barrier.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/circuitgate.py` & `bqskit-1.1.1/bqskit/ir/gates/circuitgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composed/__init__.py` & `bqskit-1.1.1/bqskit/ir/gates/composed/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composed/controlled.py` & `bqskit-1.1.1/bqskit/ir/gates/composed/controlled.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composed/daggergate.py` & `bqskit-1.1.1/bqskit/ir/gates/composed/daggergate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composed/embedded.py` & `bqskit-1.1.1/bqskit/ir/gates/composed/embedded.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,50 +46,60 @@
             a & 0 & b \\\\
             0 & 1 & 0 \\\\
             c & 0 & d \\\\
         \\end{pmatrix}
 
     This concept can be generalized to multiple qudits and even
     mixed-radix systems.
+
+    Note:
+        - Global phase inconsistencies in gates will become local phase
+            inconsistencies in the embedded gate. For example, if the
+            global phase difference between the U1Gate and the RZGate
+            will become local phase differences in the corresponding
+            subspaces when embedded into a higher-dimensional qudit.
     """
 
     def __init__(
         self,
         gate: Gate,
         radixes: Sequence[int] | int,
-        level_maps: Sequence[int] | Sequence[Sequence[int]],
+        level_maps: None | Sequence[int] | Sequence[Sequence[int]] = None,
     ) -> None:
         """
         Construct an EmbeddedGate.
 
         Args:
             gate (Gate): The gate to embed in a higher-dimensional qudit
                 gate.
 
             radixes (Sequence[int] | int): The target radixes of the higher-
                 dimensional system. If an integer is given, then the radixes
                 are assumed to be the same for all qudits. For example,
                 if `radixes = 3`, then the gate will be embedded into a
                 qutrit gate.
 
-            level_maps (Sequence[int] | Sequence[Sequence[int]]): The level
-                map for the embedding for each qudit. If a sequence of
-                integers is given, then the level map is assumed to be
-                the same for all qudits. For example, if `radixes = 3`
-                and `level_maps = [0, 2]`, then the gate will be
-                embedded into a qutrit gate by mapping the qubit levels
-                0 and 1 to the qutrit levels 0 and 2, respectively. If a
-                sequence of sequences is given, then the level map is
-                assumed to be different for each qudit. For example, if
-                `radixes = [3, 3]` and `level_maps = [[0, 2], [1, 2]]`,
-                then the gate will be embedded into a two-qudit gate by
-                mapping the first qubit's 0 and 1 levels to the first
-                qutrit's 0 and 2 levels, respectively, and by mapping
-                the second qubit's 0 and 1 levels to the second qutrit's
-                1 and 2 levels, respectively.
+             level_maps (None | Sequence[int] | Sequence[Sequence[int]]):
+                 The level map for the embedding for each qudit. If a
+                 sequence of integers is given, then the level map is
+                 assumed to be the same for all qudits. For example, if
+                 `radixes = 3` and `level_maps = [0, 2]`, then the gate
+                 will be embedded into a qutrit gate by mapping the qubit
+                 levels 0 and 1 to the qutrit levels 0 and 2,
+                 respectively. If a sequence of sequences is given, then
+                 the level map is assumed to be different for each qudit.
+                 For example, if `radixes = [3, 3]` and `level_maps =
+                 [[0, 2], [1, 2]]`, then the gate will be embedded into a
+                 two-qudit gate by mapping the first qubit's 0 and 1
+                 levels to the first qutrit's 0 and 2 levels,
+                 respectively, and by mapping the second qubit's 0 and 1
+                 levels to the second qutrit's 1 and 2 levels,
+                 respectively. This can also be set to `None`, which will
+                 embed the lower dimension gate in the lowest levels of
+                 the new radixes.
 
         Raises:
 
             ValueError: If any radix is less than 2.
 
             ValueError: If radixes is given as a sequence and its length
                 is not equal to the number of qudits in the gate.
@@ -134,14 +144,17 @@
                 'Given target radixes was not valid. Either invalid type,'
                 ' invalid length, or invalid radix. Expected target radixes'
                 ' to be a single integer or sequence of integers with length'
                 f' equal to {gate.num_qudits=}. Also expected every radix'
                 f' to be greater than 2, got {radixes=}.',
             )
 
+        if level_maps is None:
+            level_maps = [list(range(levels)) for levels in gate.radixes]
+
         if not is_sequence(level_maps):
             raise TypeError(
                 'Expected level_maps to be a sequence of integers or a '
                 f'sequence of sequences of integers, got {level_maps}.',
             )
 
         if is_sequence_of_int(level_maps):
@@ -189,17 +202,17 @@
         if any(len(lmap) != len(set(lmap)) for lmap in level_maps):
             raise ValueError(
                 'Given level_maps was not valid. Expected every level_map'
                 f' to be one-to-one, got duplicate levels: {level_maps=}.',
             )
 
         self.gate = gate
-        self.level_maps = [list(lmap) for lmap in level_maps]
+        self.level_maps = tuple([tuple(list(lmap)) for lmap in level_maps])
         self._num_qudits = gate._num_qudits
-        self._name = 'Embedded(%s)' % self.gate.name  # TODO: include radixes and level maps  # noqa: E501
+        self._name = f'Embedded({self.gate.name}){self.level_maps}'
         self._num_params = self.gate._num_params
         self._radixes = tuple(radixes)
         self._dim = int(np.prod(self.radixes))
 
         # If input is a constant gate, we can cache the unitary.
         if self.num_params == 0 and not building_docs():
             U = self.gate.get_unitary()
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composed/frozenparam.py` & `bqskit-1.1.1/bqskit/ir/gates/composed/frozenparam.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composed/tagged.py` & `bqskit-1.1.1/bqskit/ir/gates/composed/tagged.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,8 +98,11 @@
         return (
             isinstance(other, TaggedGate)
             and self.gate == other.gate
             and self.tag == other.tag
         )
 
     def __hash__(self) -> int:
+        if isinstance(self.tag, dict):
+            return hash((self.gate, tuple(self.tag.items())))
+
         return hash((self.gate, self.tag))
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composed/vlg.py` & `bqskit-1.1.1/bqskit/ir/gates/composed/vlg.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/composedgate.py` & `bqskit-1.1.1/bqskit/ir/gates/composedgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/__init__.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/b.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/b.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/ccx.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/ccx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/ch.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/ch.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/clock.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/clock.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 class ClockGate(ConstantGate, QuditGate):
     """
     The one-qudit clock (Z) gate. This is a Weyl-Heisenberg gate.
 
     The clock gate is given by the following formula:
 
     .. math::
-        \\begin{equation}
-            Z = \\sum_a \\exp(2\\pi ia/d) |a><a|
-        \\end{equation}
+        Z = \\sum_a \\exp(\\frac{2\\pi ai}{d}) |a\\rangle\\langle a|
 
     where d is the number of levels (2 levels is a qubit,
     3 levels is a qutrit, etc.)
 
     References:
         - https://arxiv.org/pdf/2302.07966.pdf
     """
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/cpi.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/cpi.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/cs.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/cs.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/csum.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/csum.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 class CSUMGate(ConstantGate, QuditGate):
     """
     The two-qudit Conditional-SUM gate.
 
     The CSUM gate is given by the following formula:
 
     .. math::
-        \\begin{equation}
-            CSUM |i,j> = |i, i + j mod d>
-        \\end{equation}
+        CSUM |i,j\\rangle = |i, i + j \\mathrm{mod} d\\rangle
 
     where d is the number of levels (2 levels is a qubit,
     3 levels is a qutrit, etc.)
 
 
     For qutrits the CSUMGate is represented by the following matrix:
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/ct.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/ct.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/cx.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/cx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/cy.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/cy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/cz.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/cz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/h.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/h.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,22 +24,20 @@
         \\frac{\\sqrt{2}}{2} & \\frac{\\sqrt{2}}{2} \\\\
         \\frac{\\sqrt{2}}{2} & -\\frac{\\sqrt{2}}{2} \\\\
         \\end{pmatrix}
 
     However, generally it is given by the following formula:
 
     .. math::
-        \\begin{equation}
-            H = 1/\\sqrt(d) \\sum_{ij} \\omega_d^{ij} |i >< j|
-        \\end{equation}
+        H = \\frac{1}{\\sqrt(d)} \\sum_{ij} \\omega_d^{ij} |i\\rangle\\langle j|
 
     where
 
     .. math::
-        \\omega = \\exp(2\\pi*i/d)
+        \\omega = \\exp(\\frac{2\\pi i}{d})
 
     and `d` is the number of levels (2 levels is a qubit,
     3 levels is a qutrit, etc.)
 
     References:
         - https://www.frontiersin.org/articles/10.3389/fphy.2020.589504/full
         - https://pubs.aip.org/aip/jmp/article-abstract/56/3/032202/763827
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/identity.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/identity.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/iswap.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/iswap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/itoffoli.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/itoffoli.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/pd.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/pd.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 class PDGate(ConstantGate, QuditGate):
     """
     The one-qudit P[i] gate.
 
     The clock gate is given by the following formula:
 
     .. math::
-        \\begin{equation}
-            P[i]_d = \\sum_{j} (-\\omega^2)^{\\delta_{ij}} |j><j|
-        \\end{equation}
+        P[i]_d = \\sum_{j} (-\\omega^2)^{\\delta_{ij}} |j\\rangle\\langle j|
 
     where
 
     .. math::
-        \\omega = \\exp(2\\pi*i/d)
+        \\omega = \\exp(\\frac{2\\pi i}{d})
 
     and d is the number of levels (2 levels is a qubit,
     3 levels is a qutrit, etc.)
 
     References:
         - https://pubs.aip.org/aip/jmp/article-abstract/56/3/032202/763827
     """
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/permutation.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/permutation.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/rccx.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/rccx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/s.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/s.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/sdg.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/sdg.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/shift.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/shift.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/sqrtcnot.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/sqrtcnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/sqrtiswap.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/sqrtiswap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/subswap.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/subswap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/swap.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/swap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/sx.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/sx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/sycamore.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/sycamore.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/t.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/t.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/tdg.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/tdg.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/unitary.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/unitary.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/x.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/x.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/xx.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/xx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/y.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/y.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/yy.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/yy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/z.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/z.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constant/zz.py` & `bqskit-1.1.1/bqskit/ir/gates/constant/zz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/constantgate.py` & `bqskit-1.1.1/bqskit/ir/gates/constantgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/generalgate.py` & `bqskit-1.1.1/bqskit/ir/gates/generalgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/measure.py` & `bqskit-1.1.1/bqskit/ir/gates/measure.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/__init__.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ccp.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/ccp.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ckm.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/ckm.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ckmd.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/ckmd.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cp.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/cp.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cphase.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/cphase.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/crx.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/crx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cry.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/cry.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/crz.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/crz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/cu.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/cu.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/fsim.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/fsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,29 @@
     QubitGate,
     DifferentiableUnitary,
     CachedClass,
 ):
     """
     Google's FSIM Gate.
 
-        Contains all two qubit interactions that preserve excitations,
-        up to single-qubit rotations and global phase.
+    Contains all two qubit interactions that preserve excitations,
+    up to single-qubit rotations and global phase.
 
-        It is given by the following parameterized unitary:
+    It is given by the following parameterized unitary:
 
-        .. math::
+    .. math::
+        \\begin{pmatrix}
+        1 & 0 & 0 & 0 \\\\
+        0 & \\cos{\\theta} & -i\\sin{\\theta} & 0 \\\\
+        0 & -i\\sin{\\theta} & \\cos{\\theta} & 0 \\\\
+        0 & 0 & 0 & e^{-i\\phi} \\\\
+        \\end{pmatrix}
 
-    $
-            \\begin{pmatrix}
-            1 & 0 & 0 & 0 \\\\
-            0 & \\cos{\\theta} & -i\\sin{\\theta} & 0 \\\\
-            0 & -i\\sin{\\theta} & \\cos{\\theta} & 0 \\\\
-            0 & 0 & 0 & e^{-i\\phi} \\\\
-            \\end{pmatrix}
-
-        References:
-            https://quantumai.google/reference/python/cirq/ops/FSimGate
+    References:
+        https://quantumai.google/reference/python/cirq/ops/FSimGate
     """
 
     _num_qudits = 2
     _num_params = 2
     _qasm_name = 'fsim'
 
     def get_unitary(self, params: RealVector = []) -> UnitaryMatrix:
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/pauli.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/pauli.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/phasedxz.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/phasedxz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rsu3.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/rsu3.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rx.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/rx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rxx.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/rxx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ry.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/ry.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/ryy.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/ryy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rz.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/rz.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     A gate representing an arbitrary rotation around the Z axis.
 
     It is given by the following parameterized unitary:
 
     .. math::
 
         \\begin{pmatrix}
-        \\exp({i\\frac{\\theta}{2}}) & 0 \\\\
-        0 & \\exp({-i\\frac{\\theta}{2}}) \\\\
+        \\exp({-i\\frac{\\theta}{2}}) & 0 \\\\
+        0 & \\exp({i\\frac{\\theta}{2}}) \\\\
         \\end{pmatrix}
     """
 
     _num_qudits = 1
     _num_params = 1
     _qasm_name = 'rz'
```

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/rzz.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/rzz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u1.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/u1.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u1q.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/u1q.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u2.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/u2.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u3.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/u3.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/u8.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/u8.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/parameterized/unitary.py` & `bqskit-1.1.1/bqskit/ir/gates/parameterized/unitary.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/gates/quditgate.py` & `bqskit-1.1.1/bqskit/ir/gates/quditgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/interval.py` & `bqskit-1.1.1/bqskit/ir/interval.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/iterator.py` & `bqskit-1.1.1/bqskit/ir/iterator.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/lang/__init__.py` & `bqskit-1.1.1/bqskit/ir/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/lang/language.py` & `bqskit-1.1.1/bqskit/ir/lang/language.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/parser.py` & `bqskit-1.1.1/bqskit/ir/lang/qasm2/parser.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/qasm2.py` & `bqskit-1.1.1/bqskit/ir/lang/qasm2/qasm2.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/lang/qasm2/visitor.py` & `bqskit-1.1.1/bqskit/ir/lang/qasm2/visitor.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/location.py` & `bqskit-1.1.1/bqskit/ir/location.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/operation.py` & `bqskit-1.1.1/bqskit/ir/operation.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/__init__.py` & `bqskit-1.1.1/bqskit/ir/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/__init__.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/differentiable.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/differentiable.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/function.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/function.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/__init__.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/generator.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/generator.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/cost/residual.py` & `bqskit-1.1.1/bqskit/ir/opt/cost/residual.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/instantiater.py` & `bqskit-1.1.1/bqskit/ir/opt/instantiater.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/instantiaters/qfactor.py` & `bqskit-1.1.1/bqskit/ir/opt/instantiaters/qfactor.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/minimizer.py` & `bqskit-1.1.1/bqskit/ir/opt/minimizer.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/minimizers/ceres.py` & `bqskit-1.1.1/bqskit/ir/opt/minimizers/ceres.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/minimizers/scipy.py` & `bqskit-1.1.1/bqskit/ir/opt/minimizers/scipy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/multistartgen.py` & `bqskit-1.1.1/bqskit/ir/opt/multistartgen.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/multistartgens/diagonal.py` & `bqskit-1.1.1/bqskit/ir/opt/multistartgens/diagonal.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/opt/multistartgens/random.py` & `bqskit-1.1.1/bqskit/ir/opt/multistartgens/random.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/point.py` & `bqskit-1.1.1/bqskit/ir/point.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/region.py` & `bqskit-1.1.1/bqskit/ir/region.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/ir/structure.py` & `bqskit-1.1.1/bqskit/ir/structure.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/__init__.py` & `bqskit-1.1.1/bqskit/passes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,26 @@
     GeneralizedSabreRoutingPass
     SetModelPass
     ApplyPlacement
     SubtopologySelectionPass
     PAMLayoutPass
     PAMRoutingPass
     EmbedAllPermutationsPass
+    ExtractModelConnectivityPass
+    RestoreModelConnevtivityPass
+
+
+.. rubric:: PAM Verification Passes
+
+These passes either perform upper-bound error analysis of the PAM process.
+
+    TagPAMBlockDataPass
+    CalculatePAMErrorsPass
+    UnTagPAMBlockDataPass
+    PAMVerificationSequence
 
 .. rubric:: Utility Passes
 
 .. autosummary::
     :toctree: autogen
     :recursive:
 
@@ -144,14 +156,15 @@
     ToVariablePass
     BlockConversionPass
     LogPass
     ExtendBlockSizePass
     LogErrorPass
     FillSingleQuditGatesPass
     StructureAnalysisPass
+    ClearAllBlockData
 
 .. rubric:: IO Passes
 
 .. autosummary::
     :toctree: autogen
     :recursive:
 
@@ -189,14 +202,15 @@
     WideLayerGenerator
 """
 from __future__ import annotations
 
 from bqskit.passes.alias import PassAlias
 from bqskit.passes.control.dothendecide import DoThenDecide
 from bqskit.passes.control.dowhileloop import DoWhileLoopPass
+from bqskit.passes.control.foreach import ClearAllBlockData
 from bqskit.passes.control.foreach import ForEachBlockPass
 from bqskit.passes.control.ifthenelse import IfThenElsePass
 from bqskit.passes.control.paralleldo import ParallelDo
 from bqskit.passes.control.predicate import PassPredicate
 from bqskit.passes.control.predicates.change import ChangePredicate
 from bqskit.passes.control.predicates.count import GateCountPredicate
 from bqskit.passes.control.predicates.many import ManyQuditGatesPredicate
@@ -219,16 +233,22 @@
 from bqskit.passes.mapping.embed import EmbedAllPermutationsPass
 from bqskit.passes.mapping.layout.pam import PAMLayoutPass
 from bqskit.passes.mapping.layout.sabre import GeneralizedSabreLayoutPass
 from bqskit.passes.mapping.placement.greedy import GreedyPlacementPass
 from bqskit.passes.mapping.placement.trivial import TrivialPlacementPass
 from bqskit.passes.mapping.routing.pam import PAMRoutingPass
 from bqskit.passes.mapping.routing.sabre import GeneralizedSabreRoutingPass
+from bqskit.passes.mapping.setmodel import ExtractModelConnectivityPass
+from bqskit.passes.mapping.setmodel import RestoreModelConnevtivityPass
 from bqskit.passes.mapping.setmodel import SetModelPass
 from bqskit.passes.mapping.topology import SubtopologySelectionPass
+from bqskit.passes.mapping.verify import CalculatePAMErrorsPass
+from bqskit.passes.mapping.verify import PAMVerificationSequence
+from bqskit.passes.mapping.verify import TagPAMBlockDataPass
+from bqskit.passes.mapping.verify import UnTagPAMBlockDataPass
 from bqskit.passes.measure import ExtractMeasurements
 from bqskit.passes.measure import RestoreMeasurements
 from bqskit.passes.noop import NOOPPass
 from bqskit.passes.partitioning.cluster import ClusteringPartitioner
 from bqskit.passes.partitioning.greedy import GreedyPartitioner
 from bqskit.passes.partitioning.quick import QuickPartitioner
 from bqskit.passes.partitioning.scan import ScanPartitioner
@@ -281,14 +301,15 @@
 from bqskit.passes.util.structure import StructureAnalysisPass
 from bqskit.passes.util.unfold import UnfoldPass
 from bqskit.passes.util.update import UpdateDataPass
 
 
 __all__ = [
     'DoWhileLoopPass',
+    'ClearAllBlockData',
     'ForEachBlockPass',
     'IfThenElsePass',
     'PassPredicate',
     'ChangePredicate',
     'GateCountPredicate',
     'NotPredicate',
     'WhileLoopPass',
@@ -372,8 +393,14 @@
     'ManyQuditGatesPredicate',
     'NoSingleQuditGatesInModel',
     'HasGeneralSingleQuditGate',
     'ZXGatePredicate',
     'AllConstantSingleQuditGates',
     'GeneralSQDecomposition',
     'StructureAnalysisPass',
+    'ExtractModelConnectivityPass',
+    'RestoreModelConnevtivityPass',
+    'TagPAMBlockDataPass',
+    'CalculatePAMErrorsPass',
+    'UnTagPAMBlockDataPass',
+    'PAMVerificationSequence',
 ]
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/alias.py` & `bqskit-1.1.1/bqskit/passes/alias.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/__init__.py` & `bqskit-1.1.1/bqskit/passes/control/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This package defines passes and objects that control pass execution flow."""
 from __future__ import annotations
 
 from bqskit.passes.control.dothendecide import DoThenDecide
 from bqskit.passes.control.dowhileloop import DoWhileLoopPass
+from bqskit.passes.control.foreach import ClearAllBlockData
 from bqskit.passes.control.foreach import ForEachBlockPass
 from bqskit.passes.control.ifthenelse import IfThenElsePass
 from bqskit.passes.control.paralleldo import ParallelDo
 from bqskit.passes.control.predicate import PassPredicate
 from bqskit.passes.control.predicates.change import ChangePredicate
 from bqskit.passes.control.predicates.count import GateCountPredicate
 from bqskit.passes.control.predicates.many import ManyQuditGatesPredicate
@@ -20,14 +21,15 @@
 from bqskit.passes.control.predicates.single import ZXGatePredicate
 from bqskit.passes.control.predicates.width import WidthPredicate
 from bqskit.passes.control.whileloop import WhileLoopPass
 
 __all__ = [
     'DoWhileLoopPass',
     'ForEachBlockPass',
+    'ClearAllBlockData',
     'IfThenElsePass',
     'PassPredicate',
     'ChangePredicate',
     'GateCountPredicate',
     'ManyQuditGatesPredicate',
     'NotPredicate',
     'WhileLoopPass',
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/dothendecide.py` & `bqskit-1.1.1/bqskit/passes/control/dothendecide.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/dowhileloop.py` & `bqskit-1.1.1/bqskit/passes/control/dowhileloop.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/foreach.py` & `bqskit-1.1.1/bqskit/passes/control/foreach.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,32 @@
 
     key = 'ForEachBlockPass_data'
     """The key in data, where block data will be put."""
 
     pass_down_key_prefix = 'ForEachBlockPass_pass_down_'
     """If a key exists in the pass data with this prefix, pass it to blocks."""
 
+    pass_down_block_specific_key_prefix = (
+        'ForEachBlockPass_specific_pass_down_'
+    )
+    """
+    Data specific to the processing of individual blocks in a partitioned
+    circuit can be injected into the `PassData` in `run` by using this prefix.
+
+    The expected type of the associated value is `dict[int, Any]`, where
+    integer (sub-)keys correspond to block numbers in a partitioned quantum
+    circuit.
+
+    Pseudocode example for seed circuits:
+        seeds = {block_id: [seed_circuit_a, seed_circuit_b, ...], ...}
+        key = self.pass_down_block_specific_key_prefix + 'seed_circuits'
+        seed_updater = UpdateDataPass(key, seeds)
+        workflow = Workflow([..., seed_updater, ForEachBlockPass(...), ...])
+    """
+
     def __init__(
         self,
         loop_body: WorkflowLike,
         calculate_error_bound: bool = False,
         collection_filter: Callable[[Operation], bool] | None = None,
         replace_filter: ReplaceFilterFn | str = 'always',
         batch_size: int | None = None,
@@ -193,14 +211,18 @@
             block_data['subnumbering'] = subnumbering
             block_data['model'] = submodel
             block_data['point'] = CircuitPoint(cycle, op.location[0])
             block_data['calculate_error_bound'] = self.calculate_error_bound
             for key in data:
                 if key.startswith(self.pass_down_key_prefix):
                     block_data[key] = data[key]
+                elif key.startswith(
+                    self.pass_down_block_specific_key_prefix,
+                ) and i in data[key]:
+                    block_data[key] = data[key][i]
             block_data.seed = data.seed
 
             subcircuits.append(subcircuit)
             block_datas.append(block_data)
 
         # Do the work
         results = await get_runtime().map(
@@ -231,28 +253,27 @@
                         op.location,
                         subcircuit.params,
                     ),
                 )
                 block_data['replaced'] = True
 
                 # Calculate Error
-                if self.calculate_error_bound:
-                    error_sum += block_data.error
+                error_sum += block_data.error
             else:
                 block_data['replaced'] = False
 
         # Replace blocks
         circuit.batch_replace(points, ops)
 
         # Record block data into pass data
         data[self.key].append(completed_block_datas)
 
         # Record error
+        data.update_error_mul(error_sum)
         if self.calculate_error_bound:
-            data.error = (1 - ((1 - data.error) * (1 - error_sum)))
             _logger.debug(f'New circuit error is {data.error}.')
 
 
 def default_collection_filter(op: Operation) -> bool:
     return isinstance(
         op.gate, (
             CircuitGate,
@@ -502,7 +523,19 @@
     if method not in replace_filters:
         raise ValueError(f'Unknown replace filter method {method}.')
 
     return replace_filters[method](model)
 
 
 ReplaceFilterFn = Callable[[Circuit, Operation], bool]
+
+
+class ClearAllBlockData(BasePass):
+    """Clear all block data and passed down data from the pass data."""
+
+    async def run(self, circuit: Circuit, data: PassData) -> None:
+        """Perform the pass's operation, see :class:`BasePass` for more."""
+        for key in list(data.keys()):
+            if key.startswith(ForEachBlockPass.key):
+                del data[key]
+            elif key.startswith(ForEachBlockPass.pass_down_key_prefix):
+                del data[key]
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/ifthenelse.py` & `bqskit-1.1.1/bqskit/passes/control/ifthenelse.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/paralleldo.py` & `bqskit-1.1.1/bqskit/passes/control/paralleldo.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicate.py` & `bqskit-1.1.1/bqskit/passes/control/predicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/__init__.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/andpredicate.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/andpredicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/change.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/change.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/count.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/count.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/many.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/many.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/multi.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/multi.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/notpredicate.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/notpredicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/orpredicate.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/orpredicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/physical.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/physical.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/single.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/single.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/predicates/width.py` & `bqskit-1.1.1/bqskit/passes/control/predicates/width.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/control/whileloop.py` & `bqskit-1.1.1/bqskit/passes/control/whileloop.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/group.py` & `bqskit-1.1.1/bqskit/passes/group.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/io/checkpoint.py` & `bqskit-1.1.1/bqskit/passes/io/checkpoint.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/io/intermediate.py` & `bqskit-1.1.1/bqskit/passes/io/intermediate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/embed.py` & `bqskit-1.1.1/bqskit/passes/mapping/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,18 @@
             graphs = data[SubtopologySelectionPass.key][width]
 
         else:
             graphs = [CouplingGraph.all_to_all(width)]
 
         datas = []
         for graph in graphs:
-            model = MachineModel(circuit.num_qudits, graph)
+            model = MachineModel(
+                circuit.num_qudits, graph,
+                data.gate_set, data.model.radixes,
+            )
             target_data = copy.deepcopy(data)
             target_data.model = model
             datas.append(target_data)
 
         # Create parallel arrays for map
         extended_targets = []
         extended_datas = []
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/layout/pam.py` & `bqskit-1.1.1/bqskit/passes/mapping/layout/pam.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         block_datas = data[ForEachBlockPass.key][-1]
         for block_data in block_datas:
             perm_data[block_data['point']] = block_data['permutation_data']
 
         if not subgraph.is_fully_connected():
             raise RuntimeError('Cannot route circuit on disconnected qudits.')
 
-        pi = data.initial_mapping
+        pi = [i for i in range(circuit.num_qudits)]
+
         for _ in range(self.total_passes):
             self.forward_pass(circuit, pi, subgraph, perm_data)
             self.backward_pass(circuit, pi, subgraph)
 
-        data.initial_mapping = pi
-        _logger.info(f'Found layout: {str(pi)}')
+        self._apply_perm(pi, data.placement)
+        _logger.info(f'Found layout: {pi}, new placement: {data.placement}')
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/layout/sabre.py` & `bqskit-1.1.1/bqskit/passes/mapping/layout/sabre.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,19 +65,19 @@
             decay_reset_on_gate,
             extended_set_size,
             extended_set_weight,
         )
 
     async def run(self, circuit: Circuit, data: PassData) -> None:
         """Perform the pass's operation, see :class:`BasePass` for more."""
-        subgraph = self.get_connectivity(circuit, data)
+        subgraph = data.connectivity
         if not subgraph.is_fully_connected():
             raise RuntimeError('Cannot layout circuit on disconnected qudits.')
 
-        pi = data.initial_mapping
+        pi = [i for i in range(circuit.num_qudits)]
+
         for _ in range(self.total_passes):
             self.forward_pass(circuit, pi, subgraph)
             self.backward_pass(circuit, pi, subgraph)
 
-        # select qubits
-        data.initial_mapping = pi
-        _logger.info(f'Found layout: {str(pi)}')
+        self._apply_perm(pi, data.placement)
+        _logger.info(f'Found layout: {pi}, new placement: {data.placement}')
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/pam.py` & `bqskit-1.1.1/bqskit/passes/mapping/pam.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 """This module implements the PAMRoutingPass class."""
 from __future__ import annotations
 
 import itertools as it
 import logging
 from typing import Dict
+from typing import Literal
+from typing import overload
 from typing import Sequence
 from typing import Tuple
+from typing import TypedDict
 
 import numpy as np
 
 from bqskit.ir.circuit import Circuit
+from bqskit.ir.gates.barrier import BarrierPlaceholder
 from bqskit.ir.gates.constant.swap import SwapGate
 from bqskit.ir.point import CircuitPoint
 from bqskit.passes.mapping.sabre import GeneralizedSabreAlgorithm
 from bqskit.qis.graph import CouplingGraph
+from bqskit.qis.unitary.unitarymatrix import UnitaryMatrix
 
 _logger = logging.getLogger(__name__)
 
 
 PAMBlockPermData = Dict[Tuple[Tuple[int, ...], Tuple[int, ...]], Circuit]
 PAMBlockTAPermData = Dict[CouplingGraph, PAMBlockPermData]
 
 
+class PAMBlockResultData(TypedDict):
+    pre_perm: tuple[int, ...]
+    post_perm: tuple[int, ...]
+    original_utry: UnitaryMatrix
+
+
+PAMBlockResultDict = Dict[CircuitPoint, PAMBlockResultData]
+
+
 class PermutationAwareMappingAlgorithm(GeneralizedSabreAlgorithm):
     """Route the circuit with permutation awareness."""
 
     def __init__(
         self,
         gate_count_weight: float = 0.1,
         decay_delta: float = 0.001,
@@ -68,22 +82,44 @@
             decay_delta,
             decay_reset_interval,
             decay_reset_on_gate,
             extended_set_size,
             extended_set_weight,
         )
 
+    @overload  # type: ignore
+    def forward_pass(
+        self,
+        circuit: Circuit,
+        pi: list[int],
+        cg: CouplingGraph,
+        perm_data: dict[CircuitPoint, PAMBlockTAPermData],
+        modify_circuit: Literal[False] = False,
+    ) -> None:
+        ...
+
+    @overload
+    def forward_pass(
+        self,
+        circuit: Circuit,
+        pi: list[int],
+        cg: CouplingGraph,
+        perm_data: dict[CircuitPoint, PAMBlockTAPermData],
+        modify_circuit: Literal[True],
+    ) -> PAMBlockResultDict:
+        ...
+
     def forward_pass(  # type: ignore
         self,
         circuit: Circuit,
         pi: list[int],
         cg: CouplingGraph,
         perm_data: dict[CircuitPoint, PAMBlockTAPermData],
         modify_circuit: bool = False,
-    ) -> None:
+    ) -> PAMBlockResultDict | None:
         """
         Apply a forward pass of the PAM algorithm to `pi`.
 
         Args:
             circuit (Circuit): The circuit to pass over.
 
             pi (list[int]): The input logical-to-physical mapping. This
@@ -105,14 +141,15 @@
         iter_count = 0
         prev_executed_counts: dict[CircuitPoint, int] = {n: 0 for n in F}
         leading_swaps: list[tuple[int, int]] = []
         _logger.debug(f'Starting forward pam pass with pi: {pi}.')
 
         if modify_circuit:
             mapped_circuit = Circuit(circuit.num_qudits, circuit.radixes)
+            out_data: PAMBlockResultDict = {}
 
         # Main Loop
         while len(F) > 0:
 
             # Retrieve executable gates giving the current mapping `pi`
             execute_list = [n for n in F if self._can_exe(circuit[n], pi, cg)]
 
@@ -135,14 +172,21 @@
                         if num_prev_executed == total_num_prev:
                             F.add(successor)
 
                 # Permute the qubits on the just executed gates
                 E = self._calc_extended_set(circuit, F)
                 for n in execute_list:
                     op = circuit[n]
+
+                    if isinstance(op.gate, BarrierPlaceholder):
+                        if modify_circuit:
+                            physical_location = [pi[q] for q in op.location]
+                            mapped_circuit.append_gate(op.gate, op.location)
+                        continue
+
                     p1, circ, p2 = self._get_best_perm(
                         circuit,
                         perm_data[n],
                         cg,
                         F,
                         pi,
                         D,
@@ -150,19 +194,25 @@
                         op.location,
                     )
 
                     self._apply_perm(p1, pi)
 
                     if modify_circuit:
                         physical_location = [pi[q] for q in op.location]
-                        mapped_circuit.append_circuit(
+                        cycle = mapped_circuit.append_circuit(
                             circ,
                             physical_location,
                             True,
                         )
+                        new_point = CircuitPoint(cycle, physical_location[0])
+                        out_data[new_point] = {
+                            'pre_perm': self._global_to_local_perm(p1),
+                            'post_perm': self._global_to_local_perm(p2),
+                            'original_utry': op.get_unitary(),
+                        }
 
                     self._apply_perm(p2, pi)
 
                 # Reset decay if necessary
                 if self.decay_reset_on_gate:
                     iter_count = 0
                     for i in range(circuit.num_qudits):
@@ -209,14 +259,20 @@
             iter_count += 1
             if iter_count % self.decay_reset_interval == 0:
                 for i in range(circuit.num_qudits):
                     decay[i] = 1.0
 
         if modify_circuit:
             circuit.become(mapped_circuit)
+            return out_data
+
+    def _global_to_local_perm(self, gperm: Sequence[int]) -> tuple[int, ...]:
+        """Return the local permutation from a global permutation."""
+        global_to_local_map = {q: i for i, q in enumerate(sorted(gperm))}
+        return tuple(global_to_local_map[i] for i in gperm)
 
     def _get_best_perm(
         self,
         circuit: Circuit,
         perm_data: PAMBlockTAPermData,
         cg: CouplingGraph,
         F: set[CircuitPoint],
@@ -351,14 +407,7 @@
                     min_term = min(term, min_term)
                 extend += min_term
             extend /= len(E)
             extend *= self.extended_set_weight
 
         pi[:] = pi_bkp[:]
         return front + extend
-
-    def _apply_perm(self, perm: Sequence[int], pi: list[int]) -> None:
-        """Apply the `perm` permutation to the current mapping `pi`."""
-        _logger.debug('applying permutation %s' % str(perm))
-        pi_c = {q: pi[perm[i]] for i, q in enumerate(sorted(perm))}
-        for q in perm:
-            pi[q] = pi_c[q]
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/placement/greedy.py` & `bqskit-1.1.1/bqskit/passes/mapping/placement/greedy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/placement/trivial.py` & `bqskit-1.1.1/bqskit/passes/mapping/placement/trivial.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/routing/pam.py` & `bqskit-1.1.1/bqskit/passes/mapping/routing/pam.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 """This module implements the PAMRoutingPass."""
 from __future__ import annotations
 
-import copy
 import logging
 
 from bqskit.compiler.basepass import BasePass
 from bqskit.compiler.passdata import PassData
 from bqskit.ir.circuit import Circuit
 from bqskit.ir.point import CircuitPoint
 from bqskit.passes.control.foreach import ForEachBlockPass
 from bqskit.passes.mapping.pam import PAMBlockTAPermData
 from bqskit.passes.mapping.pam import PermutationAwareMappingAlgorithm
 
 _logger = logging.getLogger(__name__)
 
 
 class PAMRoutingPass(PermutationAwareMappingAlgorithm, BasePass):
+
+    out_data_key = '_pam_routing_block_out_data'
+
     async def run(self, circuit: Circuit, data: PassData) -> None:
         """Perform the pass's operation, see :class:`BasePass` for more."""
-        model = self.get_model(circuit, data)
-        placement = self.get_placement(circuit, data)
-        subgraph = model.coupling_graph.get_subgraph(placement)
+        subgraph = data.connectivity
+        if not subgraph.is_fully_connected():
+            raise RuntimeError('Cannot route circuit on disconnected qudits.')
 
         perm_data: dict[CircuitPoint, PAMBlockTAPermData] = {}
         block_datas = data[ForEachBlockPass.key][-1]
         for block_data in block_datas:
             perm_data[block_data['point']] = block_data['permutation_data']
 
-        if not subgraph.is_fully_connected():
-            raise RuntimeError('Cannot route circuit on disconnected qudits.')
+        pi = [i for i in range(circuit.num_qudits)]
+        out_data = self.forward_pass(circuit, pi, subgraph, perm_data, True)
+        data.final_mapping = [pi[x] for x in data.final_mapping]
 
-        if 'initial_mapping' in data:
-            pi = copy.deepcopy(data['initial_mapping'])
-        else:
-            pi = [i for i in range(circuit.num_qudits)]
-
-        self.forward_pass(circuit, pi, subgraph, perm_data, modify_circuit=True)
-        if 'final_mapping' in data:
-            self._apply_perm(data['final_mapping'], pi)
-        data['final_mapping'] = pi
         _logger.info(f'Finished routing with layout: {str(pi)}')
+        data[self.out_data_key] = out_data
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/routing/sabre.py` & `bqskit-1.1.1/bqskit/passes/mapping/routing/sabre.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """This module implements the GeneralizedSabreRoutingPass class."""
 from __future__ import annotations
 
-import copy
 import logging
 
 from bqskit.compiler.basepass import BasePass
 from bqskit.compiler.passdata import PassData
 from bqskit.ir.circuit import Circuit
 from bqskit.passes.mapping.sabre import GeneralizedSabreAlgorithm
 
@@ -18,20 +17,16 @@
     Uses the Sabre algorithm to route the circuit.
 
     See :class:`GeneralizedSabreAlgorithm` for more info.
     """
 
     async def run(self, circuit: Circuit, data: PassData) -> None:
         """Perform the pass's operation, see :class:`BasePass` for more."""
-        subgraph = self.get_connectivity(circuit, data)
+        subgraph = data.connectivity
         if not subgraph.is_fully_connected():
             raise RuntimeError('Cannot route circuit on disconnected qudits.')
 
-        if 'initial_mapping' in data:
-            pi = copy.deepcopy(data['initial_mapping'])
-        else:
-            pi = [i for i in range(circuit.num_qudits)]
-
+        pi = [i for i in range(circuit.num_qudits)]
         self.forward_pass(circuit, pi, subgraph, modify_circuit=True)
-        # TODO: if final_mapping is already in data, apply it first
-        data['final_mapping'] = pi
+        data.final_mapping = [pi[x] for x in data.final_mapping]
+
         _logger.info(f'Finished routing with layout: {str(pi)}')
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/sabre.py` & `bqskit-1.1.1/bqskit/passes/mapping/sabre.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import logging
 from typing import Iterator
 from typing import Sequence
 
 import numpy as np
 
 from bqskit.ir.circuit import Circuit
+from bqskit.ir.gates.barrier import BarrierPlaceholder
+from bqskit.ir.gates.circuitgate import CircuitGate
 from bqskit.ir.gates.constant.swap import SwapGate
 from bqskit.ir.operation import Operation
 from bqskit.ir.point import CircuitPoint
 from bqskit.qis.graph import CouplingGraph
 
 
 _logger = logging.getLogger(__name__)
@@ -325,17 +327,24 @@
             iter_count += 1
             if iter_count % self.decay_reset_interval == 0:
                 for i in range(circuit.num_qudits):
                     decay[i] = 1.0
 
     def _can_exe(self, op: Operation, pi: list[int], cg: CouplingGraph) -> bool:
         """Return true if `op` is executable given the current mapping `pi`."""
-        # TODO: check if circuitgate of only 1-qubit gates
+        if isinstance(op.gate, BarrierPlaceholder):
+            return True
+
+        if isinstance(op.gate, CircuitGate):
+            if all(g.num_qudits == 1 for g in op.gate._circuit.gate_set):
+                return True
+
         if op.num_qudits == 1:
             return True
+
         physical_qudits = [pi[i] for i in op.location]
         return cg.get_subgraph(physical_qudits).is_fully_connected()
 
     def _calc_extended_set(
         self,
         circuit: Circuit,
         F: set[CircuitPoint],
@@ -506,7 +515,14 @@
 
             _logger.debug(f'Moving {q} to {center_qudit} via {path}.')
 
             for p1, p2 in zip(path, path[1:]):
                 if pi[center_qudit] == p1 or pi[center_qudit] == p2:
                     continue
                 yield (p1, p2)
+
+    def _apply_perm(self, perm: Sequence[int], pi: list[int]) -> None:
+        """Apply the `perm` permutation to the current mapping `pi`."""
+        _logger.debug('applying permutation %s' % str(perm))
+        pi_c = {q: pi[perm[i]] for i, q in enumerate(sorted(perm))}
+        for q in perm:
+            pi[q] = pi_c[q]
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/setmodel.py` & `bqskit-1.1.1/bqskit/passes/util/update.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,41 @@
-"""This module implements the SetModelPass class."""
+"""This module implements the UpdateDataPass class."""
 from __future__ import annotations
 
 import logging
+from typing import Any
 
 from bqskit.compiler.basepass import BasePass
-from bqskit.compiler.machine import MachineModel
 from bqskit.compiler.passdata import PassData
 from bqskit.ir.circuit import Circuit
 
+
 _logger = logging.getLogger(__name__)
 
 
-class SetModelPass(BasePass):
-    """Sets a target machine model for future passes to target."""
+class UpdateDataPass(BasePass):
+    """
+    The UpdateDataPass class.
+
+    The UpdateDataPass adds a key-value pair to data dictionary.
+    """
 
-    def __init__(self, model: MachineModel) -> None:
+    def __init__(self, key: str, val: Any) -> None:
         """
-        Construct a SetModelPass.
+        Construct a UpdateDataPass.
 
         Args:
-            model (MachineModel | None): The machine model to encode
-                into the compilation workflow.
+            key (str): The key to add.
+
+            val (Any): The value to associate with the key.
         """
-        if not isinstance(model, MachineModel):
-            raise TypeError(f'Expected MachineModel, got: {type(model)}.')
 
-        self.model = model
+        if not isinstance(key, str):
+            raise TypeError('Expected string for key, got %s.' % type(key))
+
+        self.key = key
+        self.val = val
 
     async def run(self, circuit: Circuit, data: PassData) -> None:
         """Perform the pass's operation, see :class:`BasePass` for more."""
-        if self.model.num_qudits < circuit.num_qudits:
-            raise RuntimeError('Machine model is too small for circuit.')
-
-        data.model = self.model  # Update Model
-        data.placement = list(range(circuit.num_qudits))  # Reset placement
+        _logger.debug(f'Injecting {self.key}:{self.val} into the data dict.')
+        data[self.key] = self.val
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/mapping/topology.py` & `bqskit-1.1.1/bqskit/passes/mapping/topology.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/measure.py` & `bqskit-1.1.1/bqskit/passes/measure.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/partitioning/__init__.py` & `bqskit-1.1.1/bqskit/passes/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/partitioning/cluster.py` & `bqskit-1.1.1/bqskit/passes/partitioning/cluster.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/partitioning/greedy.py` & `bqskit-1.1.1/bqskit/passes/partitioning/greedy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/partitioning/quick.py` & `bqskit-1.1.1/bqskit/passes/partitioning/quick.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/partitioning/scan.py` & `bqskit-1.1.1/bqskit/passes/partitioning/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         if self.block_size > circuit.num_qudits:
             _logger.warning(
                 'Configured block size is greater than circuit size; '
                 'blocking entire circuit.',
             )
             circuit.fold({
-                qudit_index: (0, circuit.num_cycles)
+                qudit_index: (0, circuit.num_cycles - 1)
                 for qudit_index in range(circuit.num_qudits)
             })
             return
 
         # Cache maximum cycles in circuit
         num_cycles = circuit.num_cycles
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/partitioning/single.py` & `bqskit-1.1.1/bqskit/passes/partitioning/single.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/processing/__init__.py` & `bqskit-1.1.1/bqskit/passes/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/processing/exhaustive.py` & `bqskit-1.1.1/bqskit/passes/processing/exhaustive.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/processing/iterative.py` & `bqskit-1.1.1/bqskit/passes/processing/iterative.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/processing/scan.py` & `bqskit-1.1.1/bqskit/passes/processing/scan.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/processing/substitute.py` & `bqskit-1.1.1/bqskit/passes/processing/substitute.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/retarget/auto.py` & `bqskit-1.1.1/bqskit/passes/retarget/auto.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/retarget/general.py` & `bqskit-1.1.1/bqskit/passes/retarget/general.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/retarget/two.py` & `bqskit-1.1.1/bqskit/passes/retarget/two.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/__init__.py` & `bqskit-1.1.1/bqskit/passes/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/ch2cnot.py` & `bqskit-1.1.1/bqskit/passes/rules/ch2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/cnot2ch.py` & `bqskit-1.1.1/bqskit/passes/rules/cnot2ch.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/cnot2cy.py` & `bqskit-1.1.1/bqskit/passes/rules/cnot2cy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/cnot2cz.py` & `bqskit-1.1.1/bqskit/passes/rules/cnot2cz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/cy2cnot.py` & `bqskit-1.1.1/bqskit/passes/rules/cy2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/cz2cnot.py` & `bqskit-1.1.1/bqskit/passes/rules/cz2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/swap2cnot.py` & `bqskit-1.1.1/bqskit/passes/rules/swap2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/u3.py` & `bqskit-1.1.1/bqskit/passes/rules/u3.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/rules/zxzxz.py` & `bqskit-1.1.1/bqskit/passes/rules/zxzxz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/__init__.py` & `bqskit-1.1.1/bqskit/passes/search/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/frontier.py` & `bqskit-1.1.1/bqskit/passes/search/frontier.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generator.py` & `bqskit-1.1.1/bqskit/passes/search/generator.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/__init__.py` & `bqskit-1.1.1/bqskit/passes/search/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/fourparam.py` & `bqskit-1.1.1/bqskit/passes/search/generators/fourparam.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,17 @@
 
         # Generate successors
         successors = []
         for edge in coupling_graph:
 
             if self.count_outer_cnots(circuit, edge) >= 3:
                 # No need to build circuits with more than 3 cnots in a row
-                continue
+                if circuit.num_qudits != 2:
+                    # Guard on >2 qubit to prevent high-error glitches
+                    continue
 
             successor = circuit.copy()
             successor.append_gate(CNOTGate(), edge)
             successor.append_gate(RYGate(), edge[0])
             successor.append_gate(RZGate(), edge[0])
             successor.append_gate(RYGate(), edge[1])
             successor.append_gate(RXGate(), edge[1])
```

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/middleout.py` & `bqskit-1.1.1/bqskit/passes/search/generators/middleout.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/seed.py` & `bqskit-1.1.1/bqskit/passes/search/generators/seed.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/simple.py` & `bqskit-1.1.1/bqskit/passes/search/generators/simple.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/single.py` & `bqskit-1.1.1/bqskit/passes/search/generators/single.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/stair.py` & `bqskit-1.1.1/bqskit/passes/search/generators/stair.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/generators/wide.py` & `bqskit-1.1.1/bqskit/passes/search/generators/wide.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/heuristic.py` & `bqskit-1.1.1/bqskit/passes/search/heuristic.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/heuristics/astar.py` & `bqskit-1.1.1/bqskit/passes/search/heuristics/astar.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/heuristics/dijkstra.py` & `bqskit-1.1.1/bqskit/passes/search/heuristics/dijkstra.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/search/heuristics/greedy.py` & `bqskit-1.1.1/bqskit/passes/search/heuristics/greedy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/__init__.py` & `bqskit-1.1.1/bqskit/passes/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/leap.py` & `bqskit-1.1.1/bqskit/passes/synthesis/leap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/pas.py` & `bqskit-1.1.1/bqskit/passes/synthesis/pas.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/qfast.py` & `bqskit-1.1.1/bqskit/passes/synthesis/qfast.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/qpredict.py` & `bqskit-1.1.1/bqskit/passes/synthesis/qpredict.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/qsearch.py` & `bqskit-1.1.1/bqskit/passes/synthesis/qsearch.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/synthesis.py` & `bqskit-1.1.1/bqskit/passes/synthesis/synthesis.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/synthesis/target.py` & `bqskit-1.1.1/bqskit/passes/synthesis/target.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/__init__.py` & `bqskit-1.1.1/bqskit/passes/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/compress.py` & `bqskit-1.1.1/bqskit/passes/util/compress.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/conversion.py` & `bqskit-1.1.1/bqskit/passes/util/conversion.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/converttou3.py` & `bqskit-1.1.1/bqskit/passes/util/converttou3.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/converttovar.py` & `bqskit-1.1.1/bqskit/passes/util/converttovar.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/extend.py` & `bqskit-1.1.1/bqskit/passes/util/extend.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/fill.py` & `bqskit-1.1.1/bqskit/passes/util/fill.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/log.py` & `bqskit-1.1.1/bqskit/passes/util/log.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/random.py` & `bqskit-1.1.1/bqskit/passes/util/random.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/record.py` & `bqskit-1.1.1/bqskit/passes/util/record.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/structure.py` & `bqskit-1.1.1/bqskit/passes/util/structure.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/passes/util/unfold.py` & `bqskit-1.1.1/bqskit/passes/util/unfold.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/__init__.py` & `bqskit-1.1.1/bqskit/qis/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/graph.py` & `bqskit-1.1.1/bqskit/qis/graph.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/pauli.py` & `bqskit-1.1.1/bqskit/qis/pauli.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/permutation.py` & `bqskit-1.1.1/bqskit/qis/permutation.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/state/state.py` & `bqskit-1.1.1/bqskit/qis/state/state.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/state/statemap.py` & `bqskit-1.1.1/bqskit/qis/state/statemap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/state/system.py` & `bqskit-1.1.1/bqskit/qis/state/system.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/unitary/__init__.py` & `bqskit-1.1.1/bqskit/qis/unitary/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/unitary/differentiable.py` & `bqskit-1.1.1/bqskit/qis/unitary/differentiable.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/unitary/meta.py` & `bqskit-1.1.1/bqskit/qis/unitary/meta.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/unitary/optimizable.py` & `bqskit-1.1.1/bqskit/qis/unitary/optimizable.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/unitary/unitary.py` & `bqskit-1.1.1/bqskit/qis/unitary/unitary.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/unitary/unitarybuilder.py` & `bqskit-1.1.1/bqskit/qis/unitary/unitarybuilder.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/qis/unitary/unitarymatrix.py` & `bqskit-1.1.1/bqskit/qis/unitary/unitarymatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,27 @@
         return UnitaryMatrix(self._utry.T, self.radixes, False)
 
     @property
     def dagger(self) -> UnitaryMatrix:
         """The conjugate transpose of the unitary."""
         return self.conj().T
 
+    def to_special(self) -> UnitaryMatrix:
+        """Return a special unitary matrix verson of this one."""
+        determinant = np.linalg.det(self)
+        dimension = len(self)
+        global_phase = np.angle(determinant) / dimension
+        global_phase = global_phase % (2 * np.pi / dimension)
+        global_phase_factor = np.exp(-1j * global_phase)
+        return global_phase_factor * self
+
+    def is_special(self) -> bool:
+        """Return true if this unitary is special."""
+        return 1 - np.abs(np.linalg.det(self)) < 1e-8
+
     def __len__(self) -> int:
         """The dimension of the square unitary matrix."""
         return self.shape[0]
 
     def __iter__(self) -> int:
         """An iterator that iterates through the rows of the matrix."""
         return self._utry.__iter__()
@@ -208,15 +221,15 @@
             degree (int): The degree of the distance metric.
 
         Returns:
             float: A value between 1 and 0, where 0 means the two unitaries
             are equal up to global phase and 1 means the two unitaries are
             very unsimilar or far apart.
         """
-        other = UnitaryMatrix(other)
+        other = UnitaryMatrix(other, check_arguments=False)
         num = np.abs(np.trace(self.conj().T @ other))
         dem = self.dim
         frac = min(num / dem, 1)
         dist = np.power(1 - (frac ** degree), 1.0 / degree)
         return dist if dist > 0.0 else 0.0
 
     def get_statevector(self, in_state: StateLike) -> StateVector:
@@ -471,15 +484,15 @@
                     np.abs(np.abs(input) - 1) <= 1e-14
                     for input in inputs if np.isscalar(input)
                 )
             )
         )
 
         if convert_back:
-            return UnitaryMatrix(out, self.radixes)
+            return UnitaryMatrix(out, self.radixes, False)
 
         return out
 
     def __str__(self) -> str:
         """Return the string representation of the unitary."""
         return str(self._utry)
```

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/__init__.py` & `bqskit-1.1.1/bqskit/runtime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     :recursive:
 
     ~bqskit.runtime.attached.AttachedServer
     ~bqskit.runtime.detached.DetachedServer
     ~bqskit.runtime.manager.Manager
     ~bqskit.runtime.detached.start_server
     ~bqskit.runtime.manager.start_manager
+    ~bqskit.runtime.worker.start_worker_rank
 
 Parallelize Pass Computation
 ############################
 
 When developing a BQSKit compiler pass, you can hook into the active
 runtime server through the :func:`get_runtime` function. This returns a
 :class:`RuntimeHandle`, which you can use to submit, map, wait on, and
```

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/address.py` & `bqskit-1.1.1/bqskit/runtime/address.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/attached.py` & `bqskit-1.1.1/bqskit/runtime/attached.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.mailboxes: dict[int, ServerMailbox] = {}
         self.mailbox_counter = 0
 
         # Start workers
         self.spawn_workers(num_workers, worker_port)
 
         # Connect to client
-        client_conn = self.listen_once(port)
+        client_conn = self.listen_once('localhost', port)
         self.clients[client_conn] = set()
         self.sel.register(
             client_conn,
             selectors.EVENT_READ,
             MessageDirection.CLIENT,
         )
         self.logger.info('Connected to client.')
```

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/base.py` & `bqskit-1.1.1/bqskit/runtime/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             self.employees.append(RuntimeEmployee(conn, num_workers))
             self.conn_to_employee_dict[conn] = self.employees[-1]
             self.sel.register(
                 conn,
                 selectors.EVENT_READ,
                 MessageDirection.BELOW,
             )
-            self.logger.info(f'Registered manager {i} with {num_workers = }.')
+            self.logger.info(f'Registered manager {i} with {num_workers=}.')
             self.total_workers += num_workers
         self.num_idle_workers = self.total_workers
 
         self.logger.info(f'Node has {self.total_workers} total workers.')
 
     def connect_to_manager(
         self,
@@ -328,18 +328,18 @@
             self.logger.info(f'Registered worker {i}.')
 
         self.step_size = 1
         self.total_workers = num_workers
         self.num_idle_workers = num_workers
         self.logger.info(f'Node has connected to {num_workers} workers.')
 
-    def listen_once(self, port: int) -> Connection:
-        """Listen on `port` for a connection and return on first one."""
+    def listen_once(self, ip: str, port: int) -> Connection:
+        """Listen on `ip`:`port` for a connection and return on first one."""
         family = 'AF_INET' if sys.platform == 'win32' else None
-        listener = Listener(('0.0.0.0', port), family)
+        listener = Listener((ip, port), family)
         conn = listener.accept()
         listener.close()
         return conn
 
     def run(self) -> None:
         """Main loop."""
         self.logger.info(f'{self.__class__.__name__} running...')
```

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/detached.py` & `bqskit-1.1.1/bqskit/runtime/detached.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/direction.py` & `bqskit-1.1.1/bqskit/runtime/direction.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/future.py` & `bqskit-1.1.1/bqskit/runtime/future.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/manager.py` & `bqskit-1.1.1/bqskit/runtime/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
             only_connect (bool): If true, do not spawn workers, only connect
                 to already spawned workers.
         """
         super().__init__()
 
         # Connect upstream
-        self.upstream = self.listen_once(port)
+        self.upstream = self.listen_once('0.0.0.0', port)
 
         # Handshake with upstream
         msg, payload = self.upstream.recv()
         assert msg == RuntimeMessage.CONNECT
         self.lower_id_bound = payload[0]
         self.upper_id_bound = payload[1]
         self.sel.register(
```

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/task.py` & `bqskit-1.1.1/bqskit/runtime/task.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/runtime/worker.py` & `bqskit-1.1.1/bqskit/runtime/worker.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/utils/__init__.py` & `bqskit-1.1.1/bqskit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/utils/cachedclass.py` & `bqskit-1.1.1/bqskit/utils/cachedclass.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/utils/math.py` & `bqskit-1.1.1/bqskit/utils/math.py`

 * *Files 19% similar despite different names*

```diff
@@ -219,7 +219,41 @@
             generators.append(t2)
 
         t3 = np.eye(n)
         t3[n - 1, n - 1] = -n + 1
         t3 *= np.sqrt(2 / (n * (n - 1)))
         generators.append(t3)
         return np.array(generators, dtype=np.complex128)
+
+
+def canonical_unitary(
+    unitary: npt.NDArray[np.complex128],
+) -> npt.NDArray[np.complex128]:
+    """
+    Computes a canonical form for the provided unitary.
+
+    If unitary matrices V, W differ only by a global phase, then
+    canonical_unitary(V) == canonical_unitary(W).
+
+    Args:
+        unitary (npt.NDArray[np.complex128]): A unitary matrix.
+
+    Returns:
+        npt.NDArray[np.complex128]: A unitary matrix.
+
+    References:
+        https://arxiv.org/abs/2306.05622
+    """
+    determinant = np.linalg.det(unitary)
+    dimension = len(unitary)
+    # Compute special unitary
+    global_phase = np.angle(determinant) / dimension
+    global_phase = global_phase % (2 * np.pi / dimension)
+    global_phase_factor = np.exp(-1j * global_phase)
+    special_unitary = global_phase_factor * unitary
+    # Standardize speical unitary to account for exp(-i2pi/N) differences
+    first_row_mags = np.linalg.norm(special_unitary[0, :], ord=2)
+    index = np.argmax(first_row_mags)
+    std_phase = np.angle(special_unitary[0, index])
+    correction_phase = 0 - std_phase
+    std_correction = np.exp(1j * correction_phase)
+    return std_correction * special_unitary
```

### Comparing `bqskit-1.1.0rc1/bqskit/utils/random.py` & `bqskit-1.1.1/bqskit/utils/random.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/utils/test/strategies.py` & `bqskit-1.1.1/bqskit/utils/test/strategies.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/utils/test/types.py` & `bqskit-1.1.1/bqskit/utils/test/types.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit/utils/typing.py` & `bqskit-1.1.1/bqskit/utils/typing.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0rc1/bqskit.egg-info/PKG-INFO` & `bqskit-1.1.1/bqskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqskit
-Version: 1.1.0rc1
+Version: 1.1.1
 Summary: Berkeley Quantum Synthesis Toolkit
 Home-page: https://github.com/BQSKit/bqskit
 Author: LBNL - BQSKit developers
 Author-email: edyounis@lbl.gov
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/BQSKit/bqskit/issues
 Project-URL: Source Code, https://github.com/BQSKit/bqskit
@@ -20,14 +20,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Typing :: Typed
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
```

### Comparing `bqskit-1.1.0rc1/bqskit.egg-info/SOURCES.txt` & `bqskit-1.1.1/bqskit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
 bqskit/passes/mapping/__init__.py
 bqskit/passes/mapping/apply.py
 bqskit/passes/mapping/embed.py
 bqskit/passes/mapping/pam.py
 bqskit/passes/mapping/sabre.py
 bqskit/passes/mapping/setmodel.py
 bqskit/passes/mapping/topology.py
+bqskit/passes/mapping/verify.py
 bqskit/passes/mapping/layout/__init__.py
 bqskit/passes/mapping/layout/pam.py
 bqskit/passes/mapping/layout/sabre.py
 bqskit/passes/mapping/placement/__init__.py
 bqskit/passes/mapping/placement/greedy.py
 bqskit/passes/mapping/placement/trivial.py
 bqskit/passes/mapping/routing/__init__.py
@@ -299,9 +300,8 @@
 bqskit/utils/cachedclass.py
 bqskit/utils/docs.py
 bqskit/utils/math.py
 bqskit/utils/random.py
 bqskit/utils/typing.py
 bqskit/utils/test/__init__.py
 bqskit/utils/test/strategies.py
-bqskit/utils/test/types.py
-tests/test_conftest.py
+bqskit/utils/test/types.py
```

### Comparing `bqskit-1.1.0rc1/pyproject.toml` & `bqskit-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "oldest-supported-numpy",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 minversion = 3.3.0
-envlist = pre-commit,py38,py39,py310,py311
+envlist = pre-commit,py38,py39,py310,py311,py312
 skip_missing_interpreters = true
 
 [testenv]
 passenv =
     TERM
 deps =
     numpy>=1.22
@@ -28,15 +28,15 @@
 commands =
     pytest {posargs}
 
 [testenv:pre-commit]
 skip_install = true
 deps = pre-commit
 commands = pre-commit run --all-files --show-diff-on-failure
-basepython=py311
+basepython=py312
 """
 
 [tool.pytest.ini_options]
 minversion = "2.8"
 testpaths = ["tests/"]
 python_files = "test*.py"
 norecursedirs = ".env"
```

### Comparing `bqskit-1.1.0rc1/setup.py` & `bqskit-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Software Development :: Compilers',
         'Typing :: Typed',
     ],
     keywords=[
@@ -61,15 +62,15 @@
     project_urls={
         'Bug Tracker': 'https://github.com/BQSKit/bqskit/issues',
         'Source Code': 'https://github.com/BQSKit/bqskit',
         'Documentation': 'https://bqskit.readthedocs.io/en/latest',
     },
     packages=find_packages(exclude=['examples*', 'test*']),
     install_requires=[
-        'bqskitrs>=0.4.0',
+        'bqskitrs>=0.4.1',
         'lark-parser',
         'numpy>=1.22.0',
         'scipy>=1.8.0',
         'typing-extensions>=4.0.0',
     ],
     python_requires='>=3.8, <4',
     entry_points={
```

