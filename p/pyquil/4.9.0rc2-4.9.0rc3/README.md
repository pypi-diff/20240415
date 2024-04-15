# Comparing `tmp/pyquil-4.9.0rc2.tar.gz` & `tmp/pyquil-4.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquil-4.9.0rc2.tar", max compression
+gzip compressed data, was "pyquil-4.9.0rc3.tar", max compression
```

## Comparing `pyquil-4.9.0rc2.tar` & `pyquil-4.9.0rc3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    11358 2024-04-11 15:07:19.134930 pyquil-4.9.0rc2/LICENSE
--rw-r--r--   0        0        0     1779 2024-04-11 15:07:19.134930 pyquil-4.9.0rc2/NOTICE.md
--rw-r--r--   0        0        0     8944 2024-04-11 15:07:19.134930 pyquil-4.9.0rc2/README.md
--rw-r--r--   0        0        0     2781 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0      159 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/_version.py
--rw-r--r--   0        0        0     2129 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_abstract_compiler.py
--rw-r--r--   0        0        0     7377 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_benchmark.py
--rw-r--r--   0        0        0     9942 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_compiler.py
--rw-r--r--   0        0        0     5554 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_compiler_client.py
--rw-r--r--   0        0        0     4265 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_errors.py
--rw-r--r--   0        0        0     1010 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_logger.py
--rw-r--r--   0        0        0     7568 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_qam.py
--rw-r--r--   0        0        0    11336 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_qpu.py
--rw-r--r--   0        0        0    55258 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_quantum_computer.py
--rw-r--r--   0        0        0     8637 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_qvm.py
--rw-r--r--   0        0        0     5562 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_rewrite_arithmetic.py
--rw-r--r--   0        0        0    10749 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/api/_wavefunction_simulator.py
--rw-r--r--   0        0        0      369 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/diagnostics.py
--rw-r--r--   0        0        0     1371 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/__init__.py
--rw-r--r--   0        0        0      896 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_calibration.py
--rw-r--r--   0        0        0    15705 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_group.py
--rw-r--r--   0        0        0    22783 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_main.py
--rw-r--r--   0        0        0     8213 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_memory.py
--rw-r--r--   0        0        0     5547 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_program.py
--rw-r--r--   0        0        0     9047 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_result.py
--rw-r--r--   0        0        0     7469 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_setting.py
--rw-r--r--   0        0        0      934 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/experiment/_symmetrization.py
--rw-r--r--   0        0        0      282 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/external/README.md
--rw-r--r--   0        0        0        0 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/external/__init__.py
--rw-r--r--   0        0        0     9858 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/external/rpcq.py
--rw-r--r--   0        0        0    42387 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/gates.py
--rw-r--r--   0        0        0      201 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/latex/__init__.py
--rw-r--r--   0        0        0    18720 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/latex/_diagram.py
--rw-r--r--   0        0        0     3452 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/latex/_ipython.py
--rw-r--r--   0        0        0     4041 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/latex/_main.py
--rw-r--r--   0        0        0     1266 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/latex/latex_generation.py
--rw-r--r--   0        0        0    31958 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/noise.py
--rw-r--r--   0        0        0     3346 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/noise_gates.py
--rw-r--r--   0        0        0    15865 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/operator_estimation.py
--rw-r--r--   0        0        0    42454 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/paulis.py
--rw-r--r--   0        0        0        0 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/py.typed
--rw-r--r--   0        0        0    19676 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/pyqvm.py
--rw-r--r--   0        0        0      336 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/__init__.py
--rw-r--r--   0        0        0     1662 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/_base.py
--rw-r--r--   0        0        0        0 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/_isa.py
--rw-r--r--   0        0        0      774 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/compiler.py
--rw-r--r--   0        0        0     1856 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/graph.py
--rw-r--r--   0        0        0     2714 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/qcs.py
--rw-r--r--   0        0        0      417 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/transformers/__init__.py
--rw-r--r--   0        0        0      331 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
--rw-r--r--   0        0        0     5279 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
--rw-r--r--   0        0        0    11791 2024-04-11 15:07:19.374931 pyquil-4.9.0rc2/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
--rw-r--r--   0        0        0      224 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
--rw-r--r--   0        0        0    48378 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/quil.py
--rw-r--r--   0        0        0    42707 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/quilatom.py
--rw-r--r--   0        0        0   103651 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/quilbase.py
--rw-r--r--   0        0        0     4191 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/quiltcalibrations.py
--rw-r--r--   0        0        0    10338 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/quiltwaveforms.py
--rw-r--r--   0        0        0      511 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/simulation/__init__.py
--rw-r--r--   0        0        0    13329 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/simulation/_numpy.py
--rw-r--r--   0        0        0    15815 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/simulation/_reference.py
--rw-r--r--   0        0        0    14218 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/simulation/matrices.py
--rw-r--r--   0        0        0    19105 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/simulation/tools.py
--rw-r--r--   0        0        0     8766 2024-04-11 15:07:19.378931 pyquil-4.9.0rc2/pyquil/wavefunction.py
--rw-r--r--   0        0        0    11060 1970-01-01 00:00:00.000000 pyquil-4.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-12 19:00:24.226325 pyquil-4.9.0rc3/LICENSE
+-rw-r--r--   0        0        0     1779 2024-04-12 19:00:24.226325 pyquil-4.9.0rc3/NOTICE.md
+-rw-r--r--   0        0        0     8944 2024-04-12 19:00:24.226325 pyquil-4.9.0rc3/README.md
+-rw-r--r--   0        0        0     2781 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      159 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/_version.py
+-rw-r--r--   0        0        0     2129 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/api/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/api/_abstract_compiler.py
+-rw-r--r--   0        0        0     7377 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/api/_benchmark.py
+-rw-r--r--   0        0        0     9942 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/api/_compiler.py
+-rw-r--r--   0        0        0     5554 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/api/_compiler_client.py
+-rw-r--r--   0        0        0     4265 2024-04-12 19:00:24.462327 pyquil-4.9.0rc3/pyquil/api/_errors.py
+-rw-r--r--   0        0        0     1010 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/api/_logger.py
+-rw-r--r--   0        0        0     7568 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/api/_qam.py
+-rw-r--r--   0        0        0    11336 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/api/_qpu.py
+-rw-r--r--   0        0        0    55258 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/api/_quantum_computer.py
+-rw-r--r--   0        0        0     8637 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/api/_qvm.py
+-rw-r--r--   0        0        0     5562 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/api/_rewrite_arithmetic.py
+-rw-r--r--   0        0        0    10749 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/api/_wavefunction_simulator.py
+-rw-r--r--   0        0        0      369 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/diagnostics.py
+-rw-r--r--   0        0        0     1371 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_calibration.py
+-rw-r--r--   0        0        0    15705 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_group.py
+-rw-r--r--   0        0        0    22783 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_main.py
+-rw-r--r--   0        0        0     8213 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_memory.py
+-rw-r--r--   0        0        0     5547 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_program.py
+-rw-r--r--   0        0        0     9047 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_result.py
+-rw-r--r--   0        0        0     7469 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_setting.py
+-rw-r--r--   0        0        0      934 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/experiment/_symmetrization.py
+-rw-r--r--   0        0        0      282 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/external/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/external/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/external/rpcq.py
+-rw-r--r--   0        0        0    42387 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/gates.py
+-rw-r--r--   0        0        0      201 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/latex/__init__.py
+-rw-r--r--   0        0        0    18720 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/latex/_diagram.py
+-rw-r--r--   0        0        0     3452 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/latex/_ipython.py
+-rw-r--r--   0        0        0     4041 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/latex/_main.py
+-rw-r--r--   0        0        0     1266 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/latex/latex_generation.py
+-rw-r--r--   0        0        0    31958 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/noise.py
+-rw-r--r--   0        0        0     3346 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/noise_gates.py
+-rw-r--r--   0        0        0    15865 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/operator_estimation.py
+-rw-r--r--   0        0        0    42310 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/paulis.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/py.typed
+-rw-r--r--   0        0        0    19676 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/pyqvm.py
+-rw-r--r--   0        0        0      336 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/__init__.py
+-rw-r--r--   0        0        0     1662 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/_base.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/_isa.py
+-rw-r--r--   0        0        0      774 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/compiler.py
+-rw-r--r--   0        0        0     1856 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/graph.py
+-rw-r--r--   0        0        0     2714 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/qcs.py
+-rw-r--r--   0        0        0      417 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/transformers/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
+-rw-r--r--   0        0        0     5279 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
+-rw-r--r--   0        0        0    11791 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
+-rw-r--r--   0        0        0      224 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
+-rw-r--r--   0        0        0    48378 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quil.py
+-rw-r--r--   0        0        0    44767 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quilatom.py
+-rw-r--r--   0        0        0   103651 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quilbase.py
+-rw-r--r--   0        0        0     4191 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quiltcalibrations.py
+-rw-r--r--   0        0        0    10338 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/quiltwaveforms.py
+-rw-r--r--   0        0        0      511 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/simulation/__init__.py
+-rw-r--r--   0        0        0    13329 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/simulation/_numpy.py
+-rw-r--r--   0        0        0    15815 2024-04-12 19:00:24.466327 pyquil-4.9.0rc3/pyquil/simulation/_reference.py
+-rw-r--r--   0        0        0    14218 2024-04-12 19:00:24.470327 pyquil-4.9.0rc3/pyquil/simulation/matrices.py
+-rw-r--r--   0        0        0    19105 2024-04-12 19:00:24.470327 pyquil-4.9.0rc3/pyquil/simulation/tools.py
+-rw-r--r--   0        0        0     8766 2024-04-12 19:00:24.470327 pyquil-4.9.0rc3/pyquil/wavefunction.py
+-rw-r--r--   0        0        0    11060 1970-01-01 00:00:00.000000 pyquil-4.9.0rc3/PKG-INFO
```

### Comparing `pyquil-4.9.0rc2/LICENSE` & `pyquil-4.9.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/NOTICE.md` & `pyquil-4.9.0rc3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/README.md` & `pyquil-4.9.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyproject.toml` & `pyquil-4.9.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyquil"
-version = "4.9.0-rc.2"
+version = "4.9.0-rc.3"
 description = "A Python library for creating Quantum Instruction Language (Quil) programs."
 authors = ["Rigetti Computing <softapps@rigetti.com>"]
 readme = "README.md"
 repository = "https://github.com/rigetti/pyquil.git"
 documentation = "https://pyquil-docs.rigetti.com"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `pyquil-4.9.0rc2/pyquil/_version.py` & `pyquil-4.9.0rc3/pyquil/_version.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/__init__.py` & `pyquil-4.9.0rc3/pyquil/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_abstract_compiler.py` & `pyquil-4.9.0rc3/pyquil/api/_abstract_compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_benchmark.py` & `pyquil-4.9.0rc3/pyquil/api/_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_compiler.py` & `pyquil-4.9.0rc3/pyquil/api/_compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_compiler_client.py` & `pyquil-4.9.0rc3/pyquil/api/_compiler_client.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_errors.py` & `pyquil-4.9.0rc3/pyquil/api/_errors.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_logger.py` & `pyquil-4.9.0rc3/pyquil/api/_logger.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_qam.py` & `pyquil-4.9.0rc3/pyquil/api/_qam.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_qpu.py` & `pyquil-4.9.0rc3/pyquil/api/_qpu.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_quantum_computer.py` & `pyquil-4.9.0rc3/pyquil/api/_quantum_computer.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_qvm.py` & `pyquil-4.9.0rc3/pyquil/api/_qvm.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_rewrite_arithmetic.py` & `pyquil-4.9.0rc3/pyquil/api/_rewrite_arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/api/_wavefunction_simulator.py` & `pyquil-4.9.0rc3/pyquil/api/_wavefunction_simulator.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/__init__.py` & `pyquil-4.9.0rc3/pyquil/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_calibration.py` & `pyquil-4.9.0rc3/pyquil/experiment/_calibration.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_group.py` & `pyquil-4.9.0rc3/pyquil/experiment/_group.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_main.py` & `pyquil-4.9.0rc3/pyquil/experiment/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_memory.py` & `pyquil-4.9.0rc3/pyquil/experiment/_memory.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_program.py` & `pyquil-4.9.0rc3/pyquil/experiment/_program.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_result.py` & `pyquil-4.9.0rc3/pyquil/experiment/_result.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_setting.py` & `pyquil-4.9.0rc3/pyquil/experiment/_setting.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/experiment/_symmetrization.py` & `pyquil-4.9.0rc3/pyquil/experiment/_symmetrization.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/external/rpcq.py` & `pyquil-4.9.0rc3/pyquil/external/rpcq.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/gates.py` & `pyquil-4.9.0rc3/pyquil/gates.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/latex/_diagram.py` & `pyquil-4.9.0rc3/pyquil/latex/_diagram.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/latex/_ipython.py` & `pyquil-4.9.0rc3/pyquil/latex/_ipython.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/latex/_main.py` & `pyquil-4.9.0rc3/pyquil/latex/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/latex/latex_generation.py` & `pyquil-4.9.0rc3/pyquil/latex/latex_generation.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/noise.py` & `pyquil-4.9.0rc3/pyquil/noise.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/noise_gates.py` & `pyquil-4.9.0rc3/pyquil/noise_gates.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/operator_estimation.py` & `pyquil-4.9.0rc3/pyquil/operator_estimation.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/paulis.py` & `pyquil-4.9.0rc3/pyquil/paulis.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, (PauliTerm, PauliSum)):
             raise TypeError("Can't compare PauliTerm with object of type {}.".format(type(other)))
         elif isinstance(other, PauliSum):
             return other == self
         else:
             return self.operations_as_set() == other.operations_as_set() and np.allclose(
-                self.coefficient, other.coefficient  # type: ignore
+                self.coefficient, other.coefficient
             )
 
     def __hash__(self) -> int:
         assert isinstance(self.coefficient, Complex)
         return hash(
             (
                 round(self.coefficient.real * HASH_PRECISION),
@@ -821,19 +821,19 @@
             like_terms[key].append(term)
         else:
             like_terms[key] = [term]
 
     terms = []
     for term_list in like_terms.values():
         first_term = term_list[0]
-        if len(term_list) == 1 and not np.isclose(first_term.coefficient, 0.0):  # type: ignore
+        if len(term_list) == 1 and not np.isclose(first_term.coefficient, 0.0):
             terms.append(first_term)
         else:
             coeff = sum(t.coefficient for t in term_list)
-            if not np.isclose(coeff, 0.0):  # type: ignore
+            if not np.isclose(coeff, 0.0):
                 terms.append(term_with_coeff(term_list[0], coeff))
     return PauliSum(terms)
 
 
 def check_commutation(pauli_list: Sequence[PauliTerm], pauli_two: PauliTerm) -> bool:
     """
     Check if commuting a PauliTerm commutes with a list of other terms by natural calculation.
@@ -892,21 +892,17 @@
     """
     Tests to see if a PauliTerm or PauliSum is a scalar multiple of identity
 
     :param term: Either a PauliTerm or PauliSum
     :returns: True if the PauliTerm or PauliSum is a scalar multiple of identity, False otherwise
     """
     if isinstance(term, PauliTerm):
-        return (len(term) == 0) and (not np.isclose(term.coefficient, 0))  # type: ignore
+        return (len(term) == 0) and (not np.isclose(term.coefficient, 0))
     elif isinstance(term, PauliSum):
-        return (
-            (len(term.terms) == 1)
-            and (len(term.terms[0]) == 0)
-            and (not np.isclose(term.terms[0].coefficient, 0))  # type: ignore
-        )
+        return (len(term.terms) == 1) and (len(term.terms[0]) == 0) and (not np.isclose(term.terms[0].coefficient, 0))
     else:
         raise TypeError("is_identity only checks PauliTerms and PauliSum objects!")
 
 
 def exponentiate(term: PauliTerm) -> Program:
     """
     Creates a pyQuil program that simulates the unitary evolution exp(-1j * term)
@@ -1020,15 +1016,15 @@
 
     matrices = []
     for term in pauli_sum.terms:
         coeff = term.coefficient
         assert isinstance(coeff, Number)
         qubit_paulis = {qubit: pauli for qubit, pauli in term.operations_as_set()}
         paulis = [qubit_paulis[q] if q in qubit_paulis else "I" for q in qubits]
-        matrix = float(np.real(coeff)) * reduce(np.kron, [pauli_matrices[p] for p in paulis])  # type: ignore
+        matrix = float(np.real(coeff)) * reduce(np.kron, [pauli_matrices[p] for p in paulis])
         matrices.append(matrix)
     generated_unitary = expm(-1j * np.pi * sum(matrices))
     phase = np.exp(-1j * np.angle(generated_unitary[0, 0]))
     return np.asarray(phase * generated_unitary, dtype=np.complex_)
 
 
 def _exponentiate_general_case(pauli_term: PauliTerm, param: float) -> Program:
```

### Comparing `pyquil-4.9.0rc2/pyquil/pyqvm.py` & `pyquil-4.9.0rc3/pyquil/pyqvm.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quantum_processor/_base.py` & `pyquil-4.9.0rc3/pyquil/quantum_processor/_base.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quantum_processor/compiler.py` & `pyquil-4.9.0rc3/pyquil/quantum_processor/compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quantum_processor/graph.py` & `pyquil-4.9.0rc3/pyquil/quantum_processor/graph.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quantum_processor/qcs.py` & `pyquil-4.9.0rc3/pyquil/quantum_processor/qcs.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py` & `pyquil-4.9.0rc3/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py` & `pyquil-4.9.0rc3/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quil.py` & `pyquil-4.9.0rc3/pyquil/quil.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quilatom.py` & `pyquil-4.9.0rc3/pyquil/quilatom.py`

 * *Files 5% similar despite different names*

```diff
@@ -533,14 +533,59 @@
 
     def __neg__(self) -> "Mul":
         return Mul(-1, self)
 
     def _substitute(self, d: Any) -> ExpressionDesignator:
         return self
 
+    def _evaluate(self) -> np.complex128:
+        """
+        Attempts to evaluate the expression to by simplifying it to a complex number.
+
+        Expression simplification can be slow, especially for large recursive expressions.
+        This method will raise a ValueError if the expression cannot be simplified to a complex
+        number.
+        """
+        expr = quil_rs_expr.Expression.parse(str(self))
+        expr.simplify()  # type: ignore[no-untyped-call]
+        if not expr.is_number():
+            raise ValueError(f"Cannot evaluate expression {self} to a number. Got {expr}.")
+        return np.complex128(expr.to_number())
+
+    def __float__(self) -> float:
+        """
+        Returns a copy of the expression as a float by attempting to simplify the expression.
+
+        Expression simplification can be slow, especially for large recursive expressions.
+        This cast will raise a ValueError if simplification doesn't result in a real number.
+        """
+        value = self._evaluate()
+        if value.imag != 0:
+            raise ValueError(f"Cannot convert complex value with non-zero imaginary value to float: {value}")
+        return float(value.real)
+
+    def __array__(self, dtype: Optional[np.dtype] = None) -> np.ndarray:
+        """
+        Implements the numpy array protocol for this expression.
+
+        If the dtype is not object, then there will be an attempt to simplify the expression to a
+        complex number. If the expression cannot be simplified to one, then fallback to the
+        object representation of the expression.
+
+        Note that expression simplification can be slow for large recursive expressions.
+        """
+        try:
+            if dtype != object:
+                return np.asarray(self._evaluate(), dtype=dtype)
+            raise ValueError
+        except ValueError:
+            # Note: The `None` here is a placeholder for the expression in the numpy array.
+            # The expression instance will still be accessible in the array.
+            return np.array(None, dtype=object)
+
 
 ParameterSubstitutionsMapDesignator = Mapping[Union["Parameter", "MemoryReference"], ExpressionValueDesignator]
 
 
 def substitute(expr: ExpressionDesignator, d: ParameterSubstitutionsMapDesignator) -> ExpressionDesignator:
     """
     Using a dictionary of substitutions ``d``, try and explicitly evaluate as much of ``expr`` as
```

### Comparing `pyquil-4.9.0rc2/pyquil/quilbase.py` & `pyquil-4.9.0rc3/pyquil/quilbase.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quiltcalibrations.py` & `pyquil-4.9.0rc3/pyquil/quiltcalibrations.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/quiltwaveforms.py` & `pyquil-4.9.0rc3/pyquil/quiltwaveforms.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/simulation/_numpy.py` & `pyquil-4.9.0rc3/pyquil/simulation/_numpy.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/simulation/_reference.py` & `pyquil-4.9.0rc3/pyquil/simulation/_reference.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/simulation/matrices.py` & `pyquil-4.9.0rc3/pyquil/simulation/matrices.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/simulation/tools.py` & `pyquil-4.9.0rc3/pyquil/simulation/tools.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/pyquil/wavefunction.py` & `pyquil-4.9.0rc3/pyquil/wavefunction.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.9.0rc2/PKG-INFO` & `pyquil-4.9.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquil
-Version: 4.9.0rc2
+Version: 4.9.0rc3
 Summary: A Python library for creating Quantum Instruction Language (Quil) programs.
 Home-page: https://github.com/rigetti/pyquil.git
 License: Apache-2.0
 Keywords: quantum,quil,programming,hybrid
 Author: Rigetti Computing
 Author-email: softapps@rigetti.com
 Requires-Python: >=3.8,<=3.12
```
