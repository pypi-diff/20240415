# Comparing `tmp/oqtant-1.8.2.tar.gz` & `tmp/oqtant-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqtant-1.8.2.tar", max compression
+gzip compressed data, was "oqtant-1.9.0.tar", max compression
```

## Comparing `oqtant-1.8.2.tar` & `oqtant-1.9.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0    10930 2024-01-29 19:46:03.120936 oqtant-1.8.2/LICENSE
--rw-r--r--   0        0        0     2983 2024-01-09 22:05:44.730365 oqtant-1.8.2/README.md
--rw-r--r--   0        0        0     7917 2024-01-09 22:05:44.730982 oqtant-1.8.2/documentation/INSTALL.md
--rw-r--r--   0        0        0     7188 2024-01-29 19:46:03.121430 oqtant-1.8.2/documentation/api/oqtant_api_overview.md
--rw-r--r--   0        0        0    19458 2024-01-29 19:46:03.121876 oqtant-1.8.2/documentation/api/oqtant_client.md
--rw-r--r--   0        0        0     2709 2024-01-23 17:19:43.220631 oqtant-1.8.2/documentation/api/schemas.interpolation.md
--rw-r--r--   0        0        0     3848 2024-01-29 19:46:03.122281 oqtant-1.8.2/documentation/api/schemas.job.md
--rw-r--r--   0        0        0      330 2024-01-29 18:52:40.972974 oqtant-1.8.2/documentation/api/schemas.md
--rw-r--r--   0        0        0    16430 2024-01-29 19:46:03.122577 oqtant-1.8.2/documentation/api/schemas.optical.md
--rw-r--r--   0        0        0    31762 2024-01-29 19:46:03.122834 oqtant-1.8.2/documentation/api/schemas.output.md
--rw-r--r--   0        0        0    29164 2024-01-29 19:46:03.123139 oqtant-1.8.2/documentation/api/schemas.quantum_matter.md
--rw-r--r--   0        0        0    11498 2024-01-29 19:46:03.123389 oqtant-1.8.2/documentation/api/schemas.rf.md
--rw-r--r--   0        0        0     2157 2024-01-29 19:46:03.123663 oqtant-1.8.2/documentation/api/simulator.md
--rw-r--r--   0        0        0     2415 2024-01-29 19:46:03.123871 oqtant-1.8.2/documentation/api/simulator.qm_potential.md
--rw-r--r--   0        0        0    17587 2024-01-29 19:46:03.124097 oqtant-1.8.2/documentation/api/simulator.simulator.md
--rw-r--r--   0        0        0     1109 2024-01-29 19:46:03.124426 oqtant-1.8.2/documentation/api/simulator.three_dim.md
--rw-r--r--   0        0        0     4890 2024-01-29 19:46:03.124684 oqtant-1.8.2/documentation/api/simulator.wave_function.md
--rw-r--r--   0        0        0     4257 2024-01-29 18:52:41.200756 oqtant-1.8.2/documentation/api/util.auth.md
--rw-r--r--   0        0        0     7658 2024-01-29 19:46:03.124939 oqtant-1.8.2/documentation/api/util.exceptions.md
--rw-r--r--   0        0        0      324 2024-01-29 18:52:41.197420 oqtant-1.8.2/documentation/api/util.md
--rw-r--r--   0        0        0     8142 2024-01-12 14:07:03.322403 oqtant-1.8.2/documentation/examples/demos/demo_1_quantum_interference.ipynb
--rw-r--r--   0        0        0    11924 2024-01-29 22:20:40.116543 oqtant-1.8.2/documentation/examples/demos/demo_2_multiple_slit_interference.ipynb
--rw-r--r--   0        0        0     6851 2024-01-29 19:45:56.705976 oqtant-1.8.2/documentation/examples/hello_world.ipynb
--rw-r--r--   0        0        0     6949 2024-01-29 19:46:03.125260 oqtant-1.8.2/documentation/examples/walkthroughs/images/benchmark_machine.png
--rw-r--r--   0        0        0    43511 2024-01-29 19:46:03.125803 oqtant-1.8.2/documentation/examples/walkthroughs/images/sim_vs_TOF.png
--rw-r--r--   0        0        0    42865 2024-01-29 19:46:03.126220 oqtant-1.8.2/documentation/examples/walkthroughs/images/sim_vs_lifetime.png
--rw-r--r--   0        0        0    20741 2024-01-30 19:43:25.257985 oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_1_introduction.ipynb
--rw-r--r--   0        0        0    20051 2024-01-12 14:07:03.323268 oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_2_making_quantum_matter.ipynb
--rw-r--r--   0        0        0    25419 2024-01-29 19:45:56.706371 oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_3_optical_barriers.ipynb
--rw-r--r--   0        0        0    15228 2024-01-12 14:07:03.323908 oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_4_optical_landscapes.ipynb
--rw-r--r--   0        0        0    11039 2024-01-25 15:21:26.072997 oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_5_experimentation_and_batch_jobs.ipynb
--rw-r--r--   0        0        0    18589 2024-01-29 19:46:03.126450 oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_6_simulator.ipynb
--rw-r--r--   0        0        0     1385 2023-12-07 19:27:02.465324 oqtant-1.8.2/documentation/oqtant_client_docs.md
--rw-r--r--   0        0        0     4656 2023-12-26 15:29:02.506066 oqtant-1.8.2/documentation/oqtant_rest_api_docs.md
--rw-r--r--   0        0        0      575 2024-01-29 19:46:03.126740 oqtant-1.8.2/oqtant/__init__.py
--rw-r--r--   0        0        0      575 2024-01-29 19:46:03.126891 oqtant-1.8.2/oqtant/fixtures/__init__.py
--rw-r--r--   0        0        0     4391 2024-01-29 19:46:03.127155 oqtant-1.8.2/oqtant/fixtures/jobs.py
--rw-r--r--   0        0        0    33806 2024-01-29 19:46:03.127453 oqtant-1.8.2/oqtant/oqtant_client.py
--rw-r--r--   0        0        0      575 2024-01-29 19:46:03.127591 oqtant-1.8.2/oqtant/schemas/__init__.py
--rw-r--r--   0        0        0     4426 2024-01-29 19:46:03.127888 oqtant-1.8.2/oqtant/schemas/job.py
--rw-r--r--   0        0        0    16976 2024-01-29 19:46:03.128240 oqtant-1.8.2/oqtant/schemas/optical.py
--rw-r--r--   0        0        0    25214 2024-01-30 19:41:21.702082 oqtant-1.8.2/oqtant/schemas/output.py
--rw-r--r--   0        0        0    39855 2024-01-29 19:46:03.128840 oqtant-1.8.2/oqtant/schemas/quantum_matter.py
--rw-r--r--   0        0        0    10157 2024-01-29 19:46:03.129106 oqtant-1.8.2/oqtant/schemas/rf.py
--rw-r--r--   0        0        0     1106 2024-01-30 19:43:15.221388 oqtant-1.8.2/oqtant/settings.py
--rw-r--r--   0        0        0      766 2024-01-29 19:46:03.129709 oqtant-1.8.2/oqtant/simulator/__init__.py
--rw-r--r--   0        0        0     5176 2024-01-29 19:46:03.129978 oqtant-1.8.2/oqtant/simulator/qm_potential.py
--rw-r--r--   0        0        0    56602 2024-01-29 19:46:03.130337 oqtant-1.8.2/oqtant/simulator/simulator.py
--rw-r--r--   0        0        0     2328 2024-01-29 19:46:03.130586 oqtant-1.8.2/oqtant/simulator/three_dim.py
--rw-r--r--   0        0        0    10854 2024-01-29 19:46:03.130851 oqtant-1.8.2/oqtant/simulator/wave_function.py
--rw-r--r--   0        0        0      575 2024-01-29 19:46:03.132478 oqtant-1.8.2/oqtant/util/__init__.py
--rw-r--r--   0        0        0     5774 2024-01-29 19:46:03.132726 oqtant-1.8.2/oqtant/util/auth.py
--rw-r--r--   0        0        0     1961 2024-01-29 19:46:03.132883 oqtant-1.8.2/oqtant/util/exceptions.py
--rw-r--r--   0        0        0     1176 2024-01-29 19:46:03.133180 oqtant-1.8.2/oqtant/util/server.py
--rw-r--r--   0        0        0     3777 2024-01-30 19:43:36.942033 oqtant-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 oqtant-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0    10930 2024-01-31 19:29:20.906275 oqtant-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2983 2024-01-08 16:15:02.965361 oqtant-1.9.0/README.md
+-rw-r--r--   0        0        0     7917 2024-01-08 16:15:02.965361 oqtant-1.9.0/documentation/INSTALL.md
+-rw-r--r--   0        0        0     7154 2024-02-07 21:23:06.819000 oqtant-1.9.0/documentation/api/oqtant_api_overview.md
+-rw-r--r--   0        0        0    19458 2024-02-06 19:08:32.146097 oqtant-1.9.0/documentation/api/oqtant_client.md
+-rw-r--r--   0        0        0     2709 2023-11-30 20:46:15.013365 oqtant-1.9.0/documentation/api/schemas.interpolation.md
+-rw-r--r--   0        0        0     3848 2024-02-06 19:08:32.156097 oqtant-1.9.0/documentation/api/schemas.job.md
+-rw-r--r--   0        0        0      330 2024-02-06 19:08:32.146097 oqtant-1.9.0/documentation/api/schemas.md
+-rw-r--r--   0        0        0    11289 2024-02-07 21:23:06.819000 oqtant-1.9.0/documentation/api/schemas.optical.md
+-rw-r--r--   0        0        0    31734 2024-02-07 21:23:06.819000 oqtant-1.9.0/documentation/api/schemas.output.md
+-rw-r--r--   0        0        0    29415 2024-02-07 21:23:06.819000 oqtant-1.9.0/documentation/api/schemas.quantum_matter.md
+-rw-r--r--   0        0        0    11498 2024-02-06 19:08:32.356098 oqtant-1.9.0/documentation/api/schemas.rf.md
+-rw-r--r--   0        0        0     2157 2024-02-06 19:08:32.359431 oqtant-1.9.0/documentation/api/simulator.md
+-rw-r--r--   0        0        0     2415 2024-02-06 19:08:32.362764 oqtant-1.9.0/documentation/api/simulator.qm_potential.md
+-rw-r--r--   0        0        0    17587 2024-02-06 19:08:32.482765 oqtant-1.9.0/documentation/api/simulator.simulator.md
+-rw-r--r--   0        0        0     1109 2024-02-06 19:08:32.486098 oqtant-1.9.0/documentation/api/simulator.three_dim.md
+-rw-r--r--   0        0        0     4890 2024-02-06 19:08:32.496098 oqtant-1.9.0/documentation/api/simulator.wave_function.md
+-rw-r--r--   0        0        0     4257 2024-02-06 19:08:32.502765 oqtant-1.9.0/documentation/api/util.auth.md
+-rw-r--r--   0        0        0     7658 2024-02-06 19:08:32.516098 oqtant-1.9.0/documentation/api/util.exceptions.md
+-rw-r--r--   0        0        0      324 2024-02-06 19:08:32.496098 oqtant-1.9.0/documentation/api/util.md
+-rw-r--r--   0        0        0     8142 2024-01-18 14:17:22.033599 oqtant-1.9.0/documentation/examples/demos/demo_1_quantum_interference.ipynb
+-rw-r--r--   0        0        0    11924 2024-01-31 19:29:20.906275 oqtant-1.9.0/documentation/examples/demos/demo_2_multiple_slit_interference.ipynb
+-rw-r--r--   0        0        0     6851 2024-01-24 20:15:13.422798 oqtant-1.9.0/documentation/examples/hello_world.ipynb
+-rw-r--r--   0        0        0     6949 2024-01-31 19:29:20.906275 oqtant-1.9.0/documentation/examples/walkthroughs/images/benchmark_machine.png
+-rw-r--r--   0        0        0    43511 2024-01-31 19:29:20.906275 oqtant-1.9.0/documentation/examples/walkthroughs/images/sim_vs_TOF.png
+-rw-r--r--   0        0        0    42865 2024-01-31 19:29:20.906275 oqtant-1.9.0/documentation/examples/walkthroughs/images/sim_vs_lifetime.png
+-rw-r--r--   0        0        0    20741 2024-01-23 21:11:09.267467 oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_1_introduction.ipynb
+-rw-r--r--   0        0        0    20051 2024-01-23 21:11:09.267467 oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_2_making_quantum_matter.ipynb
+-rw-r--r--   0        0        0    25419 2024-01-18 14:17:22.040266 oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_3_optical_barriers.ipynb
+-rw-r--r--   0        0        0    15228 2024-01-18 14:17:22.040266 oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_4_optical_landscapes.ipynb
+-rw-r--r--   0        0        0    11424 2024-02-06 19:07:39.806006 oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_5_experimentation_and_batch_jobs.ipynb
+-rw-r--r--   0        0        0    18514 2024-01-31 19:29:20.906275 oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_6_simulator.ipynb
+-rw-r--r--   0        0        0     1385 2023-11-27 20:53:39.840317 oqtant-1.9.0/documentation/oqtant_client_docs.md
+-rw-r--r--   0        0        0     4656 2023-11-09 14:54:30.299653 oqtant-1.9.0/documentation/oqtant_rest_api_docs.md
+-rw-r--r--   0        0        0      575 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/__init__.py
+-rw-r--r--   0        0        0      575 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/fixtures/__init__.py
+-rw-r--r--   0        0        0     4391 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/fixtures/jobs.py
+-rw-r--r--   0        0        0    33806 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/oqtant_client.py
+-rw-r--r--   0        0        0      575 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/schemas/__init__.py
+-rw-r--r--   0        0        0     4426 2024-02-05 18:48:02.323389 oqtant-1.9.0/oqtant/schemas/job.py
+-rw-r--r--   0        0        0    13636 2024-02-07 21:23:06.819000 oqtant-1.9.0/oqtant/schemas/optical.py
+-rw-r--r--   0        0        0    25222 2024-02-06 19:07:39.809339 oqtant-1.9.0/oqtant/schemas/output.py
+-rw-r--r--   0        0        0    40352 2024-02-07 21:23:06.819000 oqtant-1.9.0/oqtant/schemas/quantum_matter.py
+-rw-r--r--   0        0        0    10157 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/schemas/rf.py
+-rw-r--r--   0        0        0     1106 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/settings.py
+-rw-r--r--   0        0        0     2821 2024-02-06 19:07:39.809339 oqtant-1.9.0/oqtant/simulator/README.md
+-rw-r--r--   0        0        0      766 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/simulator/__init__.py
+-rw-r--r--   0        0        0     5176 2024-01-31 19:29:20.906275 oqtant-1.9.0/oqtant/simulator/qm_potential.py
+-rw-r--r--   0        0        0    56602 2024-01-31 19:29:20.909608 oqtant-1.9.0/oqtant/simulator/simulator.py
+-rw-r--r--   0        0        0     2328 2024-01-31 19:29:20.909608 oqtant-1.9.0/oqtant/simulator/three_dim.py
+-rw-r--r--   0        0        0    10854 2024-01-31 19:29:20.909608 oqtant-1.9.0/oqtant/simulator/wave_function.py
+-rw-r--r--   0        0        0      575 2024-01-31 19:29:20.909608 oqtant-1.9.0/oqtant/util/__init__.py
+-rw-r--r--   0        0        0     5774 2024-01-31 19:29:20.909608 oqtant-1.9.0/oqtant/util/auth.py
+-rw-r--r--   0        0        0     1961 2024-01-31 19:29:20.909608 oqtant-1.9.0/oqtant/util/exceptions.py
+-rw-r--r--   0        0        0     1176 2024-01-31 19:29:20.909608 oqtant-1.9.0/oqtant/util/server.py
+-rw-r--r--   0        0        0     3776 2024-02-07 21:38:40.638649 oqtant-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4624 1970-01-01 00:00:00.000000 oqtant-1.9.0/PKG-INFO
```

### Comparing `oqtant-1.8.2/LICENSE` & `oqtant-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/README.md` & `oqtant-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/INSTALL.md` & `oqtant-1.9.0/documentation/INSTALL.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/oqtant_api_overview.md` & `oqtant-1.9.0/documentation/api/oqtant_api_overview.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 ## Classes
 
 - [`oqtant_client.OqtantClient`](./oqtant_client.md#class-oqtantclient): Python class for interacting with Oqtant
 - [`job.OqtantJob`](./schemas.job.md#class-oqtantjob): A class that represents a job submitted to Oqtant
 - [`optical.Barrier`](./schemas.optical.md#class-barrier): Class that represents a painted optical barrier.
 - [`optical.Landscape`](./schemas.optical.md#class-landscape): Class that represents a dynamic painted-potential optical landscape constructed
 - [`optical.Snapshot`](./schemas.optical.md#class-snapshot): A class that represents a painted optical landscape/potential at a single
-- [`output.AxisType`](./schemas.output.md#class-axistype): An enumeration.
+- [`output.AxisType`](./schemas.output.md#class-axistype)
 - [`output.OqtantNonPlotOutput`](./schemas.output.md#class-oqtantnonplotoutput)
 - [`output.OqtantOutput`](./schemas.output.md#class-oqtantoutput): A class that represents the output of a job submitted to Oqtant
 - [`output.OqtantPlotOutput`](./schemas.output.md#class-oqtantplotoutput)
-- [`output.OutputImageType`](./schemas.output.md#class-outputimagetype): An enumeration.
+- [`output.OutputImageType`](./schemas.output.md#class-outputimagetype)
 - [`quantum_matter.QuantumMatter`](./schemas.quantum_matter.md#class-quantummatter): A class that represents user inputs to create and manipulate quantum matter
 - [`quantum_matter.QuantumMatterFactory`](./schemas.quantum_matter.md#class-quantummatterfactory): An abstract factory for creating instances of the QuantumMatter schema classes
 - [`rf.ConversionError`](./schemas.rf.md#class-conversionerror)
 - [`rf.RfEvap`](./schemas.rf.md#class-rfevap): A class that represents the forced RF evaporation that cools atoms to quantum degeneracy.
 - [`rf.RfSequence`](./schemas.rf.md#class-rfsequence): A class that represents a sequence of radio frequency powers/frequencies in time
 - [`rf.RfShield`](./schemas.rf.md#class-rfshield): A class that represents an RF shield (at fixed frequency and power)
 - [`qm_potential.QMPotential`](./simulator.qm_potential.md#class-qmpotential): 'QMPotential' represents the quantum matter object potential (combination of magnetic trap/snapshot/barriers)
```

### Comparing `oqtant-1.8.2/documentation/api/oqtant_client.md` & `oqtant-1.9.0/documentation/api/oqtant_client.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/schemas.interpolation.md` & `oqtant-1.9.0/documentation/api/schemas.interpolation.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/schemas.job.md` & `oqtant-1.9.0/documentation/api/schemas.job.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/schemas.optical.md` & `oqtant-1.9.0/documentation/api/simulator.simulator.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,617 +1,648 @@
 <!-- markdownlint-disable -->
 
-<a href="../../oqtant/schemas/optical.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-# <kbd>module</kbd> `schemas.optical`
+# <kbd>module</kbd> `simulator.simulator`
 
 
 
 
 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L32"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L34"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+## <kbd>class</kbd> `TimeSpan`
+TimeSpan(start: float, end: float) 
+
+<a href="../../<string>"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `__init__`
+
+```python
+__init__(start: float, end: float) → None
+```
 
-## <kbd>class</kbd> `Snapshot`
-A class that represents a painted optical landscape/potential at a single point in (manipulation stage) time 
 
 
----
 
-#### <kbd>property</kbd> interpolation_kind
 
 
 
 
 
 ---
 
-#### <kbd>property</kbd> model_computed_fields
+<a href="../../oqtant/simulator/simulator.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-Get the computed fields of this model instance. 
+## <kbd>class</kbd> `Simulator`
+'Simulator' Defines methods for evolution and plotting of the system described by the Oqtant simulator. The Oqtant simulator is constantly in evolution and the inteface should not be relied upon for use external to the Oqtant API. 
 
+<a href="../../oqtant/simulator/simulator.py#L55"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `__init__`
+
+```python
+__init__(potential: QMPotential)
+```
+
+Creates Three Wavefunctions: 
+- One is In-Trap (IT) 
+- One is Time of Flight Far Field (tof_ff) 
+- One is Time of Flight Near Field (tof_nf) 
+
+
+
+**Args:**
+ potential: Defined with QMPotential object. 
 
-**Returns:**
-  A dictionary of computed field names and their corresponding `ComputedFieldInfo` objects. 
 
 ---
 
-#### <kbd>property</kbd> model_extra
+#### <kbd>property</kbd> it_plot
 
-Get extra fields set during validation. 
+Generate a simulation analog to an in-trap image from the Oqtant hardware. 
 
 
 
 **Returns:**
-  A dictionary of extra fields, or `None` if `config.extra` is not set to `"allow"`. 
+ 
+ - <b>`dict`</b>:  data for generating an Image object(pixels, pixcal, rows, columns) 
 
 ---
 
-#### <kbd>property</kbd> model_fields_set
+#### <kbd>property</kbd> tof_output
 
-Returns the set of fields that have been explicitly set on this model instance. 
+Generate an simulation analog to a TOF image from the Oqtant hardware. 
 
 
 
 **Returns:**
-  A set of strings representing the fields that have been set,  i.e. that were not filled from defaults. 
+ 
+ - <b>`dict`</b>:  data for generating an Image object(pixels, pixcal, rows, columns) 
 
 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L64"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L1187"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>classmethod</kbd> `from_input`
+### <kbd>method</kbd> `animate_current`
 
 ```python
-from_input(landscape: 'Landscape') → Snapshot
+animate_current(frame_interval: int = 1) → FuncAnimation
 ```
 
-Method to create a Snapshot object from an existing jobs input 
-
-
+Animates the density profiles and change in potentials over time.  This is an integrated profile along the x-direction and is different from a single slice. 
 
 **Args:**
  
- - <b>`landscape`</b> (bert_schemas.job.Landscape):  The input values 
-
-
+ - <b>`frame_interval`</b> (int):  number of frames to skip each interval, determines smoothness. default =1 
 
 **Returns:**
  
- - <b>`Snapshot`</b>:  A new Snapshot object created using the input data 
+ - <b>`FuncAnimation`</b>:  an animation of the profile along the x-direction. 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L76"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L1374"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `get_ideal_potential`
+### <kbd>method</kbd> `animate_density`
 
 ```python
-get_ideal_potential(
-    time=0.0,
-    positions: 'list' = array([-60., -59., -58., -57., -56., -55., -54., -53., -52., -51., -50.,
-       -49., -48., -47., -46., -45., -44., -43., -42., -41., -40., -39.,
-       -38., -37., -36., -35., -34., -33., -32., -31., -30., -29., -28.,
-       -27., -26., -25., -24., -23., -22., -21., -20., -19., -18., -17.,
-       -16., -15., -14., -13., -12., -11., -10.,  -9.,  -8.,  -7.,  -6.,
-        -5.,  -4.,  -3.,  -2.,  -1.,   0.,   1.,   2.,   3.,   4.,   5.,
-         6.,   7.,   8.,   9.,  10.,  11.,  12.,  13.,  14.,  15.,  16.,
-        17.,  18.,  19.,  20.,  21.,  22.,  23.,  24.,  25.,  26.,  27.,
-        28.,  29.,  30.,  31.,  32.,  33.,  34.,  35.,  36.,  37.,  38.,
-        39.,  40.,  41.,  42.,  43.,  44.,  45.,  46.,  47.,  48.,  49.,
-        50.,  51.,  52.,  53.,  54.,  55.,  56.,  57.,  58.,  59.,  60.])
-) → list[float]
+animate_density(frame_interval=1, figsize=(8, 3), show_potential=True)
 ```
 
-Method to get the ideal potential energy at the specified positions 
+Animates the change in density and potential over time 
 
 
 
 **Args:**
  
- - <b>`positions`</b> (list, optional):  List of positions in microns 
+ - <b>`frame_interval`</b> (int):  number of frames to skip each interval, determines smoothness. default = 1 
+ - <b>`show_potential`</b> (bool):  whether or not to show the potential on the animation. default = True 
+ - <b>`figsize`</b> (tuple):  size of the output figure. default = (8,3) 
 
 
 
 **Returns:**
  
- - <b>`list[float]`</b>:  Potential energies, in kHz, at the specified positions 
+ - <b>`FuncAnimation`</b>:  an animation of the profile along the x-direction. 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L95"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L1254"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `get_potential`
+### <kbd>method</kbd> `animate_phase`
 
 ```python
-get_potential(positions: 'list[float]') → list[float]
+animate_phase(
+    frame_interval: int = 1,
+    show_potential: bool = True,
+    figsize=(8, 3)
+)
 ```
 
-Method to calculate the optical potential associated with a Landscape object, taking into account the actual implementation of the Oqtant projection system, at the given time 
+Animate the change in phase 
 
 
 
 **Args:**
  
- - <b>`positions`</b> (list[float]):  Positions, in microns, where the potential should be evaluated 
+ - <b>`frame_interval`</b> (int):  number of frames to skip each interval, determines smoothness. default =1 
+ - <b>`show_potential`</b> (bool):  whether or not to show the potential on the animation. default = True 
+ - <b>`figsize`</b> (tuple):  size of the output figure. default = (8,3) 
 
 
 
 **Returns:**
  
- - <b>`list[float]`</b>:  Potential energies, in kHz, at the specified positions 
+ - <b>`FuncAnimation`</b>:  an animation of the profile along the x-direction. 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L37"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L1471"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>classmethod</kbd> `new`
+### <kbd>method</kbd> `animate_profiles`
 
 ```python
-new(
-    time: 'float' = 0,
-    positions: 'list' = [-10, 10],
-    potentials: 'list' = [0, 0],
-    interpolation: 'InterpolationType' = 'LINEAR'
-) → Snapshot
+animate_profiles(frame_interval=1)
 ```
 
-Method to create a new Snapshot object 
+Animates the density profiles and change in potentials over time.  This is an integrated profile along the x-direction and is different from a single slice(!). 
 
 
 
 **Args:**
  
- - <b>`time`</b> (float, optional):  Time associated with the snapshot 
- - <b>`positions`</b> (list, optional):  Position list for the snapshot 
- - <b>`potentials`</b> (list, optional):  Potential energies corresponding to the list of positions 
- - <b>`interpolation`</b> (bert_schemas.job.InterpolationType, optional):  How to connect the object's  (positions, potentials) data in space. 
+ - <b>`frame_interval`</b> (int):  number of frames to skip each interval, determines smoothness. default = 1 
+ - <b>`show_potential`</b> (bool):  whether or not to show the potential on the animation. default = True 
+ - <b>`figsize`</b> (tuple):  size of the output figure. default = (8,3) 
 
 
 
 **Returns:**
  
- - <b>`Snapshot`</b>:  a new Snapshot object 
+ - <b>`FuncAnimation`</b>:  an animation of the profile along the x-direction. 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L110"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L216"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `show_potential`
+### <kbd>method</kbd> `convert_intrap_to_nearfield`
 
 ```python
-show_potential(
-    xlimits: 'list[float]' = [-61.0, 61],
-    ylimits: 'list[float]' = [-1.0, 101],
-    include_ideal: 'bool' = False
-) → None
+convert_intrap_to_nearfield(psi: ndarray) → ndarray
 ```
 
-Method to plot the potential energy as a function of position for a Landscape object at the given times 
+Performs interpolation of wave function between IT and TOF grids For handoff between evolve IT and in TOF modes. 
 
 
 
 **Args:**
  
- - <b>`xlimits`</b> (list[float], optional):  Plot limits for x axis 
- - <b>`ylimits`</b> (list[float], optional):  Plot limits for y axis 
- - <b>`include_ideal`</b> (bool, optional):  Flag for including target potential in plot 
+ - <b>`psi`</b> (ndarray):   a wave function of the IT grid (self.wavefunction.three_d_grid) 
 
+**Returns:**
+ 
+ - <b>`ndarray`</b>:   psi interpolated onto the TOF nearfield grid (self.wavefunction_tof_nf.three_d_grid) 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L154"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
-
-## <kbd>class</kbd> `Landscape`
-Class that represents a dynamic painted-potential optical landscape constructed from individual (instantaneous time) Snapshots 
+<a href="../../oqtant/simulator/simulator.py#L254"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `convert_nearfield_to_farfield`
 
----
+```python
+convert_nearfield_to_farfield(psi_tof_nf: ndarray) → ndarray
+```
 
-#### <kbd>property</kbd> interpolation_kind
+Interpolation of wave function between NF and FF grids For handoff between evolve NF and in FF modes. 
 
 
 
+**Args:**
+ 
+ - <b>`psi_tof_nf`</b> (ndarray):   a wave function of the NF grid (self.wavefunction_tof_nf.three_d_grid) 
 
+**Returns:**
+ 
+ - <b>`ndarray`</b>:   psi interpolated onto the TOF grid (self.wavefunction_tof_ff.three_d_grid) 
 
 ---
 
-#### <kbd>property</kbd> model_computed_fields
-
-Get the computed fields of this model instance. 
+<a href="../../oqtant/simulator/simulator.py#L848"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `convert_timesteps`
 
+```python
+convert_timesteps(timesteps: list) → ndarray
+```
 
-**Returns:**
-  A dictionary of computed field names and their corresponding `ComputedFieldInfo` objects. 
+Convert a list of arbitrary times (in oqtant units) to a list of simulator timestep indices. Simulation must already have been evaluated. 
 
----
 
-#### <kbd>property</kbd> model_extra
 
-Get extra fields set during validation. 
+**Args:**
+ 
+ - <b>`timesteps`</b> (list):  list of times in oqtant units 
 
 
 
 **Returns:**
-  A dictionary of extra fields, or `None` if `config.extra` is not set to `"allow"`. 
+ 
+ - <b>`ndarray `</b>:  array of simulator timestep indexes (not the values of the timesteps) 
 
 ---
 
-#### <kbd>property</kbd> model_fields_set
-
-Returns the set of fields that have been explicitly set on this model instance. 
-
+<a href="../../oqtant/simulator/simulator.py#L898"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `get_column_densities`
 
-**Returns:**
-  A set of strings representing the fields that have been set,  i.e. that were not filled from defaults. 
-
----
+```python
+get_column_densities(time_ms: float) → tuple
+```
 
-#### <kbd>property</kbd> snapshots
+Returns the column densities and slices of the condensate in cartesian coordinates for an arbitrary time. In correct coordinates to be returned to the user. 
 
-Property to get a list of Snapshot objects associated to a Landscape object 
 
 
+**Args:**
+ 
+ - <b>`time_ms`</b> (float):   time (in milliseconds) 
 
 **Returns:**
  
- - <b>`list[Snapshot]`</b>:  List of Snapshot objects 
-
-
+ - <b>`tuple (column_zy, column_zx, slice_y, slice_x) `</b>:  the column densitites and slices at the desired time 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L187"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L353"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>classmethod</kbd> `from_input`
+### <kbd>method</kbd> `get_gpe`
 
 ```python
-from_input(landscape: 'OpticalLandscape') → Landscape
+get_gpe(psi: ndarray) → ndarray
 ```
 
-Method to create a Landscape object from an existing jobs input 
+Implementation of the Gross-Pitaevskii Equation w/Neumann boundary conditions at r = 0 and Dirichlet at large x and r. If self.tof_nf or self.tof_ff == True, the external potential is ignored. 
 
 
 
 **Args:**
  
- - <b>`landscape`</b> (job_schema.OpticalLandscape):  The input values 
+ - <b>`psi`</b> (ndarray):  the current timestep wavefunction 
 
 
 
 **Returns:**
  
- - <b>`Landscape`</b>:  A new Landscape object 
+ - <b>`ndarray`</b>:  wavefunction calculated by the Gross-Pitaevskii Equation 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L209"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L292"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `get_ideal_potential`
+### <kbd>method</kbd> `get_laplacian`
 
 ```python
-get_ideal_potential(
-    time: 'float',
-    positions: 'list[float]' = array([-60., -59., -58., -57., -56., -55., -54., -53., -52., -51., -50.,
-       -49., -48., -47., -46., -45., -44., -43., -42., -41., -40., -39.,
-       -38., -37., -36., -35., -34., -33., -32., -31., -30., -29., -28.,
-       -27., -26., -25., -24., -23., -22., -21., -20., -19., -18., -17.,
-       -16., -15., -14., -13., -12., -11., -10.,  -9.,  -8.,  -7.,  -6.,
-        -5.,  -4.,  -3.,  -2.,  -1.,   0.,   1.,   2.,   3.,   4.,   5.,
-         6.,   7.,   8.,   9.,  10.,  11.,  12.,  13.,  14.,  15.,  16.,
-        17.,  18.,  19.,  20.,  21.,  22.,  23.,  24.,  25.,  26.,  27.,
-        28.,  29.,  30.,  31.,  32.,  33.,  34.,  35.,  36.,  37.,  38.,
-        39.,  40.,  41.,  42.,  43.,  44.,  45.,  46.,  47.,  48.,  49.,
-        50.,  51.,  52.,  53.,  54.,  55.,  56.,  57.,  58.,  59.,  60.])
-) → list[float]
+get_laplacian(y: ndarray) → ndarray
 ```
 
-Method to calculate ideal object potential energy at the specified time and positions 
+Implementation of the second derivatives in x and r including forward, central, and backward formulas to second order accuracy 
 
 
 
 **Args:**
  
- - <b>`time`</b> (float):  Time, in ms, at which the potential energy is calculated 
- - <b>`positions`</b> (list[float], optional):  Positions at which the potential energy is calculated 
+ - <b>`y`</b> (ndarray):  function for which we calculate the laplacian 
 
 
 
 **Returns:**
  
- - <b>`list[float]`</b>:  Potential energies, in kHz, at specified time and positions 
+ - <b>`ndarray`</b>:  The laplacian of the function 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L240"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L785"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `get_potential`
+### <kbd>method</kbd> `is_time_far_field`
 
 ```python
-get_potential(
-    time: 'float',
-    positions: 'list' = array([-60., -59., -58., -57., -56., -55., -54., -53., -52., -51., -50.,
-       -49., -48., -47., -46., -45., -44., -43., -42., -41., -40., -39.,
-       -38., -37., -36., -35., -34., -33., -32., -31., -30., -29., -28.,
-       -27., -26., -25., -24., -23., -22., -21., -20., -19., -18., -17.,
-       -16., -15., -14., -13., -12., -11., -10.,  -9.,  -8.,  -7.,  -6.,
-        -5.,  -4.,  -3.,  -2.,  -1.,   0.,   1.,   2.,   3.,   4.,   5.,
-         6.,   7.,   8.,   9.,  10.,  11.,  12.,  13.,  14.,  15.,  16.,
-        17.,  18.,  19.,  20.,  21.,  22.,  23.,  24.,  25.,  26.,  27.,
-        28.,  29.,  30.,  31.,  32.,  33.,  34.,  35.,  36.,  37.,  38.,
-        39.,  40.,  41.,  42.,  43.,  44.,  45.,  46.,  47.,  48.,  49.,
-        50.,  51.,  52.,  53.,  54.,  55.,  56.,  57.,  58.,  59.,  60.])
-) → list[float]
+is_time_far_field(time: float) → bool
 ```
 
-Method to calculate the optical potential associated with a Landscape object, taking into account the actual implementation of the Oqtant projection system, at the given time 
+Checks if the time is when the condensate is in far-field part of TOF. 
 
 
 
 **Args:**
  
- - <b>`time`</b> (float):  Time, in ms, at which to sample the potential energy 
- - <b>`positions`</b> (list[float], optional):  Positions, in microns, where the potential should be evaluated 
-
-
+ - <b>`time`</b> (float):    time in simulation (!) units. 
 
 **Returns:**
  
- - <b>`list[float]`</b>:  Potential energies, in kHz, at the requested positions and time 
+ - <b>`Bool`</b>:   True means the system is in FF of TOF mode at that time. 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L159"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L756"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>classmethod</kbd> `new`
+### <kbd>method</kbd> `is_time_intrap`
 
 ```python
-new(
-    snapshots: 'list[Snapshot]' = [Snapshot(time_ms=0.0, potentials_khz=[0.0, 0.0], positions_um=[-10.0, 10.0], spatial_interpolation=<InterpolationType.LINEAR: 'LINEAR'>, interpolation_kind='linear'), Snapshot(time_ms=2.0, potentials_khz=[0.0, 0.0], positions_um=[-10.0, 10.0], spatial_interpolation=<InterpolationType.LINEAR: 'LINEAR'>, interpolation_kind='linear')]
-) → Landscape
+is_time_intrap(time: float) → bool
 ```
 
-Method to create a new Landscape object 
+Checks if the time is when the condensate is still in trap. 
 
 
 
 **Args:**
  
- - <b>`snapshots`</b> (list[Snapshot], optional):  A list of Snapshot objects 
-
-
+ - <b>`time`</b> (float):    time in simulation units. 
 
 **Returns:**
  
- - <b>`Landscape`</b>:  A new Landscape object 
+ - <b>`Bool`</b>:   True means the system is in IT mode at that time.  False means it is not (it is in TOF mode). 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L258"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L769"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `show_potential`
+### <kbd>method</kbd> `is_time_near_field`
 
 ```python
-show_potential(
-    times: 'list' = [0.0],
-    xlimits: 'list' = [-61.0, 61],
-    ylimits: 'list' = [-1.0, 101],
-    include_ideal: 'bool' = False
-)
+is_time_near_field(time: float) → bool
 ```
 
-Method to plot the potential energy as a function of position for a Landscape object at the given times 
+Checks if the time is when the condensate is in near-field part of TOF. 
 
 
 
 **Args:**
  
- - <b>`times`</b> (list[float], optional):  Times, in ms, at which to evaluate and plot the potential 
- - <b>`xlimits`</b> (list[float], optional):  Plot limits for x axis 
- - <b>`ylimits`</b> (list[float], optional):  Plot limits for y axis 
- - <b>`include_ideal`</b> (bool, optional):  Flag for including target potential in plot 
+ - <b>`time`</b> (float):    time in simulation (!) units. 
 
+**Returns:**
+ 
+ - <b>`Bool`</b>:   True means the system is in NF of TOF mode at that time. 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L303"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L484"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-## <kbd>class</kbd> `Barrier`
-Class that represents a painted optical barrier. 
+### <kbd>method</kbd> `is_wavefunction_at_boundary`
+
+```python
+is_wavefunction_at_boundary(psi: ndarray) → None
+```
 
+Warn user if the condensate is hitting the edge of the simulation. 
+
+
+
+**Args:**
+ 
+ - <b>`psi`</b> (ndarray):  the wave function 
 
 ---
 
-#### <kbd>property</kbd> birth
+<a href="../../oqtant/simulator/simulator.py#L135"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `run_TOF`
+
+```python
+run_TOF() → None
+```
 
-Property to get the (manipulation stage) time that the Barrier object will be created 
+This function runs the TOF evolution and turns on/off the far field grid as needed 
 
 
 
 **Returns:**
- 
- - <b>`float`</b>:  The time, in ms, at which the barrier will start being projected 
+  None 
 
 ---
 
-#### <kbd>property</kbd> death
+<a href="../../oqtant/simulator/simulator.py#L184"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `run_TOF_farField`
+
+```python
+run_TOF_farField() → None
+```
 
-Property to get the (manipulation stage) time that the Barrier object will cease to exist 
+This function evolves the condensate with ground = False, with no trapping potentials or optical potentials. It runs for the remaining time of flight of the quantum_matter object, beginning with the result wavefunction of run_TOF_nearField at 6ms. It uses the far field TOF grid: self.wavefunction_tof_ff.three_d_grid is created with argument FF = True 
 
 
 
 **Returns:**
- 
- - <b>`float`</b>:  The time, in ms, at which the barrier will stop being projected 
+  None 
 
 ---
 
-#### <kbd>property</kbd> interpolation_kind
+<a href="../../oqtant/simulator/simulator.py#L149"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `run_TOF_nearField`
 
+```python
+run_TOF_nearField() → None
+```
+
+This function evolves the condensate with ground = False, with no trapping potentials or optical potentials. It runs for up to 6ms of the quantum_matter object, beginning with the result wavefunction of run_evolution It uses the near field TOF grid: self.wavefunction_tof_nf.three_d_grid is created with argument NF = True 
 
 
 
+**Returns:**
+  None 
+
 ---
 
-#### <kbd>property</kbd> lifetime
+<a href="../../oqtant/simulator/simulator.py#L113"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `run_evolution`
+
+```python
+run_evolution() → None
+```
 
-Property to get the lifetime value of a Barrier object 
+Run the simulation in In-Trap (IT) mode. This function evolves the condensate with ground = False. It is done at positive times during the "experiment" stage (t=0). Optical potentials may be applied during this stage. It runs for the lifetime of the quantum_matter object It starts from the end result of running get_ground_state 
 
 
 
 **Returns:**
- 
- - <b>`float`</b>:  The amount of time, in ms, that the barrier will exist 
+  None 
 
 ---
 
-#### <kbd>property</kbd> model_computed_fields
+<a href="../../oqtant/simulator/simulator.py#L382"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `run_rk4`
 
-Get the computed fields of this model instance. 
+```python
+run_rk4(time_span: TimeSpan, stage_name: str = '') → None
+```
 
+Implementation of the Runge-Kutta 4th order method to evolve in time. Depends on if the simulation is in IT mode, tof_nf or tof_ff mode. 
 
 
+
+**Args:**
+ 
+ - <b>`time_span`</b> (TimeSpan):   a list of times (in milliseconds) 
+ - <b>`stage_name`</b> (str):  name for the evolving stage. default = "" 
+
 **Returns:**
-  A dictionary of computed field names and their corresponding `ComputedFieldInfo` objects. 
+ None 
 
 ---
 
-#### <kbd>property</kbd> model_extra
+<a href="../../oqtant/simulator/simulator.py#L90"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+
+### <kbd>method</kbd> `set_ground_state`
+
+```python
+set_ground_state() → None
+```
 
-Get extra fields set during validation. 
+This function evolves the condensate with ground = True. It is done at negative times before the barriers are switched on. 2.5 simulation units of time is sufficient to settle down to the ground state. 
 
 
 
 **Returns:**
-  A dictionary of extra fields, or `None` if `config.extra` is not set to `"allow"`. 
+  None 
 
 ---
 
-#### <kbd>property</kbd> model_fields_set
+<a href="../../oqtant/simulator/simulator.py#L985"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-Returns the set of fields that have been explicitly set on this model instance. 
+### <kbd>method</kbd> `show_column_densities`
 
+```python
+show_column_densities(times_ms: list, slices: bool = True, figsize=(15, 7))
+```
 
+Plots the column densities and slices of the condensate in cartesian coordinates for an input array of times. In correct coordinates to be returned to the user. 
 
-**Returns:**
-  A set of strings representing the fields that have been set,  i.e. that were not filled from defaults. 
 
 
+**Args:**
+ 
+ - <b>`times_ms`</b> (list):   a list of times (in milliseconds) 
+ - <b>`slices`</b> (bool):  plot or not to plot slices 
+ - <b>`figsize`</b> (tuple):  size of output figure. default = (15,7) 
+
+**Returns:**
+ None 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L348"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L1153"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>classmethod</kbd> `from_input`
+### <kbd>method</kbd> `show_current`
 
 ```python
-from_input(barrier: 'Barrier') → Barrier
+show_current(times_ms: list, figsize=(10, 7)) → None
 ```
 
-Method to create a Barrier object using the input values of a job 
+Plot the flow for a given list of timesteps two separate subplots 
 
 
 
 **Args:**
  
- - <b>`barrier`</b> (job_schema.Barrier):  The input values 
+ - <b>`times_ms`</b> (list):  List of times (ms) at which to display current 
+ - <b>`figsize`</b> (tuple):  size of output figure. default = (10,7) 
 
 
 
 **Returns:**
- 
- - <b>`Barrier`</b>:  A new Barrier object created using the input data 
+ None 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L306"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L931"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>classmethod</kbd> `new`
+### <kbd>method</kbd> `show_density_cylindrical`
 
 ```python
-new(
-    positions: 'list[float]' = [0.0, 0.0],
-    heights: 'list[float]' = [0.0, 0.0],
-    widths: 'list[float]' = [1.0, 1.0],
-    times: 'list[float]' = [0.0, 10.0],
-    shape: 'ShapeType' = <ShapeType.GAUSSIAN: 'GAUSSIAN'>,
-    interpolation: 'InterpolationType' = <InterpolationType.LINEAR: 'LINEAR'>
-) → Barrier
+show_density_cylindrical(times_ms: list, figsize=(15, 7)) → None
 ```
 
-Method to create a new Barrier object 
+Plots the density profile of the condensate in cylindrical coordinates for an input array of times. Useful coordinates for diagonising issues but not to be returned to the user. 
 
 
 
 **Args:**
  
- - <b>`positions`</b> (list[float], optional):  Positions for the barrier 
- - <b>`heights`</b> (list[float], optional):  Heights for the barrier 
- - <b>`widths`</b> (list[float], optional):  Widths for the barrier 
- - <b>`times`</b> (list[float], optional):  Times for the barrier 
- - <b>`shape`</b> (bert_schemas.job.ShapeType, optional):  Shape of the barrier 
- - <b>`interpolation`</b> (bert_schemas.job.InterpolationType, optional):  Interpolation type of the barrier 
+ - <b>`times_ms`</b> (list):   a list of times (in milliseconds/oqtant units) 
+ - <b>`figsize`</b> (tuple):  size of output figure. default = (15,7) 
 
+**Returns:**
+ None 
 
+---
 
-**Returns:**
- 
- - <b>`Barrier`</b>:  A new Barrier object 
+<a href="../../oqtant/simulator/simulator.py#L825"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
+### <kbd>method</kbd> `show_final_result`
 
+```python
+show_final_result() → None
+```
 
-**Raises:**
- 
- - <b>`ValueError`</b>:  if data lists are not of equal length 
+Plot the density at the end of the simulation in cylindrical coordinates. Useful coordinates for diagonising issues but not to be returned to the user. 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L360"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L1106"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `show_dynamics`
+### <kbd>method</kbd> `show_phase`
 
 ```python
-show_dynamics() → None
+show_phase(times_ms: list, figsize=(10, 7)) → None
 ```
 
-Method to plot the position, width and height of a Barrier object over time 
+Plot the phase for a given list of timesteps This can only be displayed in cylindrical coordinates. It is a helpful tool still for the user.  The aspect ratio is still a bit weird. 
+
+
+
+**Args:**
+ 
+ - <b>`times_ms`</b> (list):  List of times to display 
+ - <b>`figsize`</b> (tuple):  size of output figure. default = (10,7) 
+
+**Returns:**
+ None 
 
 ---
 
-<a href="../../oqtant/schemas/optical.py#L407"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/simulator/simulator.py#L797"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
-### <kbd>method</kbd> `show_potential`
+### <kbd>method</kbd> `which_wavefunction_mode`
 
 ```python
-show_potential(
-    times: 'list[float]' = [0.0],
-    xlimits: 'list[float]' = [-61.0, 61],
-    ylimits: 'list[float]' = [-1.0, 101],
-    include_ideal: 'bool' = False
-) → None
+which_wavefunction_mode(time: float) → WaveFunction
 ```
 
-Method to plot the potential energy as a function of position for a Barrier object 
+Checks which mode the time corresponds to and returns the correct wavefunction class. 
 
 
 
 **Args:**
  
- - <b>`times`</b> (list[float], optional):  The times, in ms, at which the potential is evaluated 
- - <b>`xlimits`</b> (list[float], optional):  Plot limits for x axis 
- - <b>`ylimits`</b> (list[float], optional):  Plot limits for y axis 
- - <b>`include_ideal`</b> (bool, optional):  Flag for including target potential in plot 
+ - <b>`time`</b> (float):    time in simulation (!) units. 
+
+**Returns:**
+ 
+ - <b>`WaveFunction`</b>:   instance of the wavefunction class in the correct mode 
 
 
 
 
 ---
 
 _This file was automatically generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
```

#### html2text {}

```diff
@@ -1,170 +1,176 @@
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]# module
-`schemas.optical` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]## class `Snapshot` A class that represents a painted optical landscape/
-potential at a single point in (manipulation stage) time --- #### property
-interpolation_kind --- #### property model_computed_fields Get the computed
-fields of this model instance. **Returns:** A dictionary of computed field
-names and their corresponding `ComputedFieldInfo` objects. --- #### property
-model_extra Get extra fields set during validation. **Returns:** A dictionary
-of extra fields, or `None` if `config.extra` is not set to `"allow"`. --- ####
-property model_fields_set Returns the set of fields that have been explicitly
-set on this model instance. **Returns:** A set of strings representing the
-fields that have been set, i.e. that were not filled from defaults. --- _[_h_t_t_p_s_:
-_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### classmethod
-`from_input` ```python from_input(landscape: 'Landscape') â Snapshot ```
-Method to create a Snapshot object from an existing jobs input **Args:** -
-``llaannddssccaappee`` (bert_schemas.job.Landscape): The input values **Returns:** -
-``SSnnaappsshhoott``: A new Snapshot object created using the input data --- _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`get_ideal_potential` ```python get_ideal_potential( time=0.0, positions:
-'list' = array([-60., -59., -58., -57., -56., -55., -54., -53., -52., -51., -
-50., -49., -48., -47., -46., -45., -44., -43., -42., -41., -40., -39., -38., -
-37., -36., -35., -34., -33., -32., -31., -30., -29., -28., -27., -26., -25., -
-24., -23., -22., -21., -20., -19., -18., -17., -16., -15., -14., -13., -12., -
-11., -10., -9., -8., -7., -6., -5., -4., -3., -2., -1., 0., 1., 2., 3., 4., 5.,
-6., 7., 8., 9., 10., 11., 12., 13., 14., 15., 16., 17., 18., 19., 20., 21.,
-22., 23., 24., 25., 26., 27., 28., 29., 30., 31., 32., 33., 34., 35., 36., 37.,
-38., 39., 40., 41., 42., 43., 44., 45., 46., 47., 48., 49., 50., 51., 52., 53.,
-54., 55., 56., 57., 58., 59., 60.]) ) â list[float] ``` Method to get the
-ideal potential energy at the specified positions **Args:** - ``ppoossiittiioonnss``
-(list, optional): List of positions in microns **Returns:** - ``lliisstt[[ffllooaatt]]``:
-Potential energies, in kHz, at the specified positions --- _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`get_potential` ```python get_potential(positions: 'list[float]') â list
-[float] ``` Method to calculate the optical potential associated with a
-Landscape object, taking into account the actual implementation of the Oqtant
-projection system, at the given time **Args:** - ``ppoossiittiioonnss`` (list[float]):
-Positions, in microns, where the potential should be evaluated **Returns:** -
-``lliisstt[[ffllooaatt]]``: Potential energies, in kHz, at the specified positions ---
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### classmethod
-`new` ```python new( time: 'float' = 0, positions: 'list' = [-10, 10],
-potentials: 'list' = [0, 0], interpolation: 'InterpolationType' = 'LINEAR' )
-â Snapshot ``` Method to create a new Snapshot object **Args:** - ``ttiimmee``
-(float, optional): Time associated with the snapshot - ``ppoossiittiioonnss`` (list,
-optional): Position list for the snapshot - ``ppootteennttiiaallss`` (list, optional):
-Potential energies corresponding to the list of positions - ``iinntteerrppoollaattiioonn``
-(bert_schemas.job.InterpolationType, optional): How to connect the object's
-(positions, potentials) data in space. **Returns:** - ``SSnnaappsshhoott``: a new
-Snapshot object --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### method `show_potential` ```python show_potential( xlimits: 'list
-[float]' = [-61.0, 61], ylimits: 'list[float]' = [-1.0, 101], include_ideal:
-'bool' = False ) â None ``` Method to plot the potential energy as a function
-of position for a Landscape object at the given times **Args:** - ``xxlliimmiittss``
-(list[float], optional): Plot limits for x axis - ``yylliimmiittss`` (list[float],
-optional): Plot limits for y axis - ``iinncclluuddee__iiddeeaall`` (bool, optional): Flag for
-including target potential in plot --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `Landscape` Class that represents a dynamic
-painted-potential optical landscape constructed from individual (instantaneous
-time) Snapshots --- #### property interpolation_kind --- #### property
-model_computed_fields Get the computed fields of this model instance.
-**Returns:** A dictionary of computed field names and their corresponding
-`ComputedFieldInfo` objects. --- #### property model_extra Get extra fields set
-during validation. **Returns:** A dictionary of extra fields, or `None` if
-`config.extra` is not set to `"allow"`. --- #### property model_fields_set
-Returns the set of fields that have been explicitly set on this model instance.
-**Returns:** A set of strings representing the fields that have been set, i.e.
-that were not filled from defaults. --- #### property snapshots Property to get
-a list of Snapshot objects associated to a Landscape object **Returns:** -
-``lliisstt[[SSnnaappsshhoott]]``: List of Snapshot objects --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### classmethod `from_input` ```python
-from_input(landscape: 'OpticalLandscape') â Landscape ``` Method to create a
-Landscape object from an existing jobs input **Args:** - ``llaannddssccaappee``
-(job_schema.OpticalLandscape): The input values **Returns:** - ``LLaannddssccaappee``: A
-new Landscape object --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `get_ideal_potential` ```python
-get_ideal_potential( time: 'float', positions: 'list[float]' = array([-60., -
-59., -58., -57., -56., -55., -54., -53., -52., -51., -50., -49., -48., -47., -
-46., -45., -44., -43., -42., -41., -40., -39., -38., -37., -36., -35., -34., -
-33., -32., -31., -30., -29., -28., -27., -26., -25., -24., -23., -22., -21., -
-20., -19., -18., -17., -16., -15., -14., -13., -12., -11., -10., -9., -8., -7.,
--6., -5., -4., -3., -2., -1., 0., 1., 2., 3., 4., 5., 6., 7., 8., 9., 10., 11.,
-12., 13., 14., 15., 16., 17., 18., 19., 20., 21., 22., 23., 24., 25., 26., 27.,
-28., 29., 30., 31., 32., 33., 34., 35., 36., 37., 38., 39., 40., 41., 42., 43.,
-44., 45., 46., 47., 48., 49., 50., 51., 52., 53., 54., 55., 56., 57., 58., 59.,
-60.]) ) â list[float] ``` Method to calculate ideal object potential energy
-at the specified time and positions **Args:** - ``ttiimmee`` (float): Time, in ms, at
-which the potential energy is calculated - ``ppoossiittiioonnss`` (list[float], optional):
-Positions at which the potential energy is calculated **Returns:** - ``lliisstt
-[[ffllooaatt]]``: Potential energies, in kHz, at specified time and positions ---
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`get_potential` ```python get_potential( time: 'float', positions: 'list' =
-array([-60., -59., -58., -57., -56., -55., -54., -53., -52., -51., -50., -49.,
--48., -47., -46., -45., -44., -43., -42., -41., -40., -39., -38., -37., -36., -
-35., -34., -33., -32., -31., -30., -29., -28., -27., -26., -25., -24., -23., -
-22., -21., -20., -19., -18., -17., -16., -15., -14., -13., -12., -11., -10., -
-9., -8., -7., -6., -5., -4., -3., -2., -1., 0., 1., 2., 3., 4., 5., 6., 7., 8.,
-9., 10., 11., 12., 13., 14., 15., 16., 17., 18., 19., 20., 21., 22., 23., 24.,
-25., 26., 27., 28., 29., 30., 31., 32., 33., 34., 35., 36., 37., 38., 39., 40.,
-41., 42., 43., 44., 45., 46., 47., 48., 49., 50., 51., 52., 53., 54., 55., 56.,
-57., 58., 59., 60.]) ) â list[float] ``` Method to calculate the optical
-potential associated with a Landscape object, taking into account the actual
-implementation of the Oqtant projection system, at the given time **Args:** -
-``ttiimmee`` (float): Time, in ms, at which to sample the potential energy -
-``ppoossiittiioonnss`` (list[float], optional): Positions, in microns, where the potential
-should be evaluated **Returns:** - ``lliisstt[[ffllooaatt]]``: Potential energies, in kHz,
-at the requested positions and time --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### classmethod `new` ```python new( snapshots: 'list
-[Snapshot]' = [Snapshot(time_ms=0.0, potentials_khz=[0.0, 0.0], positions_um=[-
-10.0, 10.0], spatial_interpolation=
-LINEAR'>, interpolation_kind='linear'), Snapshot(time_ms=2.0, potentials_khz=
-[0.0, 0.0], positions_um=[-10.0, 10.0], spatial_interpolation=
-LINEAR'>, interpolation_kind='linear')] ) â Landscape ``` Method to create a
-new Landscape object **Args:** - ``ssnnaappsshhoottss`` (list[Snapshot], optional): A list
-of Snapshot objects **Returns:** - ``LLaannddssccaappee``: A new Landscape object ---
+`simulator.simulator` --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `TimeSpan` TimeSpan(start: float, end: float)
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`show_potential` ```python show_potential( times: 'list' = [0.0], xlimits:
-'list' = [-61.0, 61], ylimits: 'list' = [-1.0, 101], include_ideal: 'bool' =
-False ) ``` Method to plot the potential energy as a function of position for a
-Landscape object at the given times **Args:** - ``ttiimmeess`` (list[float],
-optional): Times, in ms, at which to evaluate and plot the potential -
-``xxlliimmiittss`` (list[float], optional): Plot limits for x axis - ``yylliimmiittss`` (list
-[float], optional): Plot limits for y axis - ``iinncclluuddee__iiddeeaall`` (bool, optional):
-Flag for including target potential in plot --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `Barrier` Class that represents a
-painted optical barrier. --- #### property birth Property to get the
-(manipulation stage) time that the Barrier object will be created **Returns:**
-- ``ffllooaatt``: The time, in ms, at which the barrier will start being projected --
-- #### property death Property to get the (manipulation stage) time that the
-Barrier object will cease to exist **Returns:** - ``ffllooaatt``: The time, in ms, at
-which the barrier will stop being projected --- #### property
-interpolation_kind --- #### property lifetime Property to get the lifetime
-value of a Barrier object **Returns:** - ``ffllooaatt``: The amount of time, in ms,
-that the barrier will exist --- #### property model_computed_fields Get the
-computed fields of this model instance. **Returns:** A dictionary of computed
-field names and their corresponding `ComputedFieldInfo` objects. --- ####
-property model_extra Get extra fields set during validation. **Returns:** A
-dictionary of extra fields, or `None` if `config.extra` is not set to
-`"allow"`. --- #### property model_fields_set Returns the set of fields that
-have been explicitly set on this model instance. **Returns:** A set of strings
-representing the fields that have been set, i.e. that were not filled from
-defaults. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### classmethod `from_input` ```python from_input(barrier: 'Barrier')
-â Barrier ``` Method to create a Barrier object using the input values of a
-job **Args:** - ``bbaarrrriieerr`` (job_schema.Barrier): The input values **Returns:** -
-``BBaarrrriieerr``: A new Barrier object created using the input data --- _[_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### classmethod `new`
-```python new( positions: 'list[float]' = [0.0, 0.0], heights: 'list[float]' =
-[0.0, 0.0], widths: 'list[float]' = [1.0, 1.0], times: 'list[float]' = [0.0,
-10.0], shape: 'ShapeType' =
-GAUSSIAN'>, interpolation: 'InterpolationType' =
-LINEAR'> ) â Barrier ``` Method to create a new Barrier object **Args:** -
-``ppoossiittiioonnss`` (list[float], optional): Positions for the barrier - ``hheeiigghhttss``
-(list[float], optional): Heights for the barrier - ``wwiiddtthhss`` (list[float],
-optional): Widths for the barrier - ``ttiimmeess`` (list[float], optional): Times for
-the barrier - ``sshhaappee`` (bert_schemas.job.ShapeType, optional): Shape of the
-barrier - ``iinntteerrppoollaattiioonn`` (bert_schemas.job.InterpolationType, optional):
-Interpolation type of the barrier **Returns:** - ``BBaarrrriieerr``: A new Barrier
-object **Raises:** - ``VVaalluueeEErrrroorr``: if data lists are not of equal length ---
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`show_dynamics` ```python show_dynamics() â None ``` Method to plot the
-position, width and height of a Barrier object over time --- _[_h_t_t_p_s_:_/_/
+`__init__` ```python __init__(start: float, end: float) â None ``` ---
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
+`Simulator` 'Simulator' Defines methods for evolution and plotting of the
+system described by the Oqtant simulator. The Oqtant simulator is constantly in
+evolution and the inteface should not be relied upon for use external to the
+Oqtant API. _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
+method `__init__` ```python __init__(potential: QMPotential) ``` Creates Three
+Wavefunctions: - One is In-Trap (IT) - One is Time of Flight Far Field (tof_ff)
+- One is Time of Flight Near Field (tof_nf) **Args:** potential: Defined with
+QMPotential object. --- #### property it_plot Generate a simulation analog to
+an in-trap image from the Oqtant hardware. **Returns:** - ``ddiicctt``: data for
+generating an Image object(pixels, pixcal, rows, columns) --- #### property
+tof_output Generate an simulation analog to a TOF image from the Oqtant
+hardware. **Returns:** - ``ddiicctt``: data for generating an Image object(pixels,
+pixcal, rows, columns) --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `animate_current` ```python animate_current
+(frame_interval: int = 1) â FuncAnimation ``` Animates the density profiles
+and change in potentials over time. This is an integrated profile along the x-
+direction and is different from a single slice. **Args:** - ``ffrraammee__iinntteerrvvaall``
+(int): number of frames to skip each interval, determines smoothness. default
+=1 **Returns:** - ``FFuunnccAAnniimmaattiioonn``: an animation of the profile along the x-
+direction. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `animate_density` ```python animate_density(frame_interval=1,
+figsize=(8, 3), show_potential=True) ``` Animates the change in density and
+potential over time **Args:** - ``ffrraammee__iinntteerrvvaall`` (int): number of frames to
+skip each interval, determines smoothness. default = 1 - ``sshhooww__ppootteennttiiaall``
+(bool): whether or not to show the potential on the animation. default = True -
+``ffiiggssiizzee`` (tuple): size of the output figure. default = (8,3) **Returns:** -
+``FFuunnccAAnniimmaattiioonn``: an animation of the profile along the x-direction. --- _[_h_t_t_p_s_:
+_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`animate_phase` ```python animate_phase( frame_interval: int = 1,
+show_potential: bool = True, figsize=(8, 3) ) ``` Animate the change in phase
+**Args:** - ``ffrraammee__iinntteerrvvaall`` (int): number of frames to skip each interval,
+determines smoothness. default =1 - ``sshhooww__ppootteennttiiaall`` (bool): whether or not to
+show the potential on the animation. default = True - ``ffiiggssiizzee`` (tuple): size
+of the output figure. default = (8,3) **Returns:** - ``FFuunnccAAnniimmaattiioonn``: an
+animation of the profile along the x-direction. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `animate_profiles` ```python
+animate_profiles(frame_interval=1) ``` Animates the density profiles and change
+in potentials over time. This is an integrated profile along the x-direction
+and is different from a single slice(!). **Args:** - ``ffrraammee__iinntteerrvvaall`` (int):
+number of frames to skip each interval, determines smoothness. default = 1 -
+``sshhooww__ppootteennttiiaall`` (bool): whether or not to show the potential on the animation.
+default = True - ``ffiiggssiizzee`` (tuple): size of the output figure. default = (8,3)
+**Returns:** - ``FFuunnccAAnniimmaattiioonn``: an animation of the profile along the x-
+direction. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `convert_intrap_to_nearfield` ```python
+convert_intrap_to_nearfield(psi: ndarray) â ndarray ``` Performs
+interpolation of wave function between IT and TOF grids For handoff between
+evolve IT and in TOF modes. **Args:** - ``ppssii`` (ndarray): a wave function of the
+IT grid (self.wavefunction.three_d_grid) **Returns:** - ``nnddaarrrraayy``: psi
+interpolated onto the TOF nearfield grid
+(self.wavefunction_tof_nf.three_d_grid) --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
+_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `convert_nearfield_to_farfield`
+```python convert_nearfield_to_farfield(psi_tof_nf: ndarray) â ndarray ```
+Interpolation of wave function between NF and FF grids For handoff between
+evolve NF and in FF modes. **Args:** - ``ppssii__ttooff__nnff`` (ndarray): a wave function
+of the NF grid (self.wavefunction_tof_nf.three_d_grid) **Returns:** -
+``nnddaarrrraayy``: psi interpolated onto the TOF grid
+(self.wavefunction_tof_ff.three_d_grid) --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
+_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `convert_timesteps` ```python
+convert_timesteps(timesteps: list) â ndarray ``` Convert a list of arbitrary
+times (in oqtant units) to a list of simulator timestep indices. Simulation
+must already have been evaluated. **Args:** - ``ttiimmeesstteeppss`` (list): list of times
+in oqtant units **Returns:** - ``nnddaarrrraayy ``: array of simulator timestep indexes
+(not the values of the timesteps) --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `get_column_densities` ```python
+get_column_densities(time_ms: float) â tuple ``` Returns the column densities
+and slices of the condensate in cartesian coordinates for an arbitrary time. In
+correct coordinates to be returned to the user. **Args:** - ``ttiimmee__mmss`` (float):
+time (in milliseconds) **Returns:** - ``ttuuppllee ((ccoolluummnn__zzyy,, ccoolluummnn__zzxx,, sslliiccee__yy,,
+sslliiccee__xx)) ``: the column densitites and slices at the desired time --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `get_gpe`
+```python get_gpe(psi: ndarray) â ndarray ``` Implementation of the Gross-
+Pitaevskii Equation w/Neumann boundary conditions at r = 0 and Dirichlet at
+large x and r. If self.tof_nf or self.tof_ff == True, the external potential is
+ignored. **Args:** - ``ppssii`` (ndarray): the current timestep wavefunction
+**Returns:** - ``nnddaarrrraayy``: wavefunction calculated by the Gross-Pitaevskii
+Equation --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
+method `get_laplacian` ```python get_laplacian(y: ndarray) â ndarray ```
+Implementation of the second derivatives in x and r including forward, central,
+and backward formulas to second order accuracy **Args:** - ``yy`` (ndarray):
+function for which we calculate the laplacian **Returns:** - ``nnddaarrrraayy``: The
+laplacian of the function --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `is_time_far_field` ```python
+is_time_far_field(time: float) â bool ``` Checks if the time is when the
+condensate is in far-field part of TOF. **Args:** - ``ttiimmee`` (float): time in
+simulation (!) units. **Returns:** - ``BBooooll``: True means the system is in FF of
+TOF mode at that time. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `is_time_intrap` ```python is_time_intrap
+(time: float) â bool ``` Checks if the time is when the condensate is still
+in trap. **Args:** - ``ttiimmee`` (float): time in simulation units. **Returns:** -
+``BBooooll``: True means the system is in IT mode at that time. False means it is not
+(it is in TOF mode). --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `is_time_near_field` ```python
+is_time_near_field(time: float) â bool ``` Checks if the time is when the
+condensate is in near-field part of TOF. **Args:** - ``ttiimmee`` (float): time in
+simulation (!) units. **Returns:** - ``BBooooll``: True means the system is in NF of
+TOF mode at that time. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `is_wavefunction_at_boundary` ```python
+is_wavefunction_at_boundary(psi: ndarray) â None ``` Warn user if the
+condensate is hitting the edge of the simulation. **Args:** - ``ppssii`` (ndarray):
+the wave function --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `run_TOF` ```python run_TOF() â None ``` This function runs
+the TOF evolution and turns on/off the far field grid as needed **Returns:**
+None --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]###
+method `run_TOF_farField` ```python run_TOF_farField() â None ``` This
+function evolves the condensate with ground = False, with no trapping
+potentials or optical potentials. It runs for the remaining time of flight of
+the quantum_matter object, beginning with the result wavefunction of
+run_TOF_nearField at 6ms. It uses the far field TOF grid:
+self.wavefunction_tof_ff.three_d_grid is created with argument FF = True
+**Returns:** None --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `run_TOF_nearField` ```python run_TOF_nearField() â None
+``` This function evolves the condensate with ground = False, with no trapping
+potentials or optical potentials. It runs for up to 6ms of the quantum_matter
+object, beginning with the result wavefunction of run_evolution It uses the
+near field TOF grid: self.wavefunction_tof_nf.three_d_grid is created with
+argument NF = True **Returns:** None --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `run_evolution` ```python run_evolution()
+â None ``` Run the simulation in In-Trap (IT) mode. This function evolves the
+condensate with ground = False. It is done at positive times during the
+"experiment" stage (t=0). Optical potentials may be applied during this stage.
+It runs for the lifetime of the quantum_matter object It starts from the end
+result of running get_ground_state **Returns:** None --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `run_rk4`
+```python run_rk4(time_span: TimeSpan, stage_name: str = '') â None ```
+Implementation of the Runge-Kutta 4th order method to evolve in time. Depends
+on if the simulation is in IT mode, tof_nf or tof_ff mode. **Args:** -
+``ttiimmee__ssppaann`` (TimeSpan): a list of times (in milliseconds) - ``ssttaaggee__nnaammee`` (str):
+name for the evolving stage. default = "" **Returns:** None --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`set_ground_state` ```python set_ground_state() â None ``` This function
+evolves the condensate with ground = True. It is done at negative times before
+the barriers are switched on. 2.5 simulation units of time is sufficient to
+settle down to the ground state. **Returns:** None --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `show_column_densities`
+```python show_column_densities(times_ms: list, slices: bool = True, figsize=
+(15, 7)) ``` Plots the column densities and slices of the condensate in
+cartesian coordinates for an input array of times. In correct coordinates to be
+returned to the user. **Args:** - ``ttiimmeess__mmss`` (list): a list of times (in
+milliseconds) - ``sslliicceess`` (bool): plot or not to plot slices - ``ffiiggssiizzee``
+(tuple): size of output figure. default = (15,7) **Returns:** None --- _[_h_t_t_p_s_:_/
+_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`show_current` ```python show_current(times_ms: list, figsize=(10, 7)) â None
+``` Plot the flow for a given list of timesteps two separate subplots **Args:**
+- ``ttiimmeess__mmss`` (list): List of times (ms) at which to display current - ``ffiiggssiizzee``
+(tuple): size of output figure. default = (10,7) **Returns:** None --- _[_h_t_t_p_s_:_/
+_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`show_density_cylindrical` ```python show_density_cylindrical(times_ms: list,
+figsize=(15, 7)) â None ``` Plots the density profile of the condensate in
+cylindrical coordinates for an input array of times. Useful coordinates for
+diagonising issues but not to be returned to the user. **Args:** - ``ttiimmeess__mmss``
+(list): a list of times (in milliseconds/oqtant units) - ``ffiiggssiizzee`` (tuple):
+size of output figure. default = (15,7) **Returns:** None --- _[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`show_potential` ```python show_potential( times: 'list[float]' = [0.0],
-xlimits: 'list[float]' = [-61.0, 61], ylimits: 'list[float]' = [-1.0, 101],
-include_ideal: 'bool' = False ) â None ``` Method to plot the potential
-energy as a function of position for a Barrier object **Args:** - ``ttiimmeess`` (list
-[float], optional): The times, in ms, at which the potential is evaluated -
-``xxlliimmiittss`` (list[float], optional): Plot limits for x axis - ``yylliimmiittss`` (list
-[float], optional): Plot limits for y axis - ``iinncclluuddee__iiddeeaall`` (bool, optional):
-Flag for including target potential in plot --- _This file was automatically
-generated via [lazydocs](https://github.com/ml-tooling/lazydocs)._
+`show_final_result` ```python show_final_result() â None ``` Plot the density
+at the end of the simulation in cylindrical coordinates. Useful coordinates for
+diagonising issues but not to be returned to the user. --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `show_phase`
+```python show_phase(times_ms: list, figsize=(10, 7)) â None ``` Plot the
+phase for a given list of timesteps This can only be displayed in cylindrical
+coordinates. It is a helpful tool still for the user. The aspect ratio is still
+a bit weird. **Args:** - ``ttiimmeess__mmss`` (list): List of times to display -
+``ffiiggssiizzee`` (tuple): size of output figure. default = (10,7) **Returns:** None --
+- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`which_wavefunction_mode` ```python which_wavefunction_mode(time: float) â
+WaveFunction ``` Checks which mode the time corresponds to and returns the
+correct wavefunction class. **Args:** - ``ttiimmee`` (float): time in simulation (!)
+units. **Returns:** - ``WWaavveeFFuunnccttiioonn``: instance of the wavefunction class in the
+correct mode --- _This file was automatically generated via [lazydocs](https://
+github.com/ml-tooling/lazydocs)._
```

### Comparing `oqtant-1.8.2/documentation/api/schemas.output.md` & `oqtant-1.9.0/documentation/api/schemas.output.md`

 * *Files 1% similar despite different names*

```diff
@@ -173,26 +173,30 @@
 
 
 ---
 
 <a href="../../oqtant/schemas/output.py#L33"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `OutputImageType`
-An enumeration. 
+
+
+
 
 
 
 
 
 ---
 
 <a href="../../oqtant/schemas/output.py#L40"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `AxisType`
-An enumeration. 
+
+
+
 
 
 
 
 
 ---
```

#### html2text {}

```diff
@@ -40,23 +40,23 @@
 the y direction (along gravity) - ``TTFFppOODD`` (float): Thomas-Fermi peak optical
 density - ``rrxx`` (float): Thomas-Fermi radius along the x direction - ``rryy``
 (float): Thomas-Fermi radius along the y direction (along gravity) - ``xxcc``
 (float): Cloud center along the x direction (along gravity) - ``yycc`` (float):
 Cloud center along the y direction - ``ooss`` (float): Constant offset **Returns:**
 - ``nnuummppyy..nnddaarrrraayy``: a 2D array of samples from a bimodal (Thomas-Fermi +
 Gaussian) distribution --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `OutputImageType` An enumeration. --- _[_h_t_t_p_s_:
-_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `AxisType` An
-enumeration. --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]## class `OqtantOutput` A class that represents the output of a job
-submitted to Oqtant --- #### property IT Property that returns the shaped in-
-trap (IT) image of a job's output if it exists **Returns:** - ``nnuummppyy..nnddaarrrraayy``:
-The reshaped pixels of the IT image --- #### property TOF Property that returns
-the shaped time of flight (TOF) image of a job's output if it exists **Returns:
-** - ``nnuummppyy..nnddaarrrraayy``: The reshaped pixels of the TOF image --- #### property
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `OutputImageType` --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class `AxisType` ---
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]## class
+`OqtantOutput` A class that represents the output of a job submitted to Oqtant
+--- #### property IT Property that returns the shaped in-trap (IT) image of a
+job's output if it exists **Returns:** - ``nnuummppyy..nnddaarrrraayy``: The reshaped pixels
+of the IT image --- #### property TOF Property that returns the shaped time of
+flight (TOF) image of a job's output if it exists **Returns:** -
+``nnuummppyy..nnddaarrrraayy``: The reshaped pixels of the TOF image --- #### property
 atom_statistics Property that prints out the atom statistics of a
 TIME_OF_FLIGHT image job's output --- #### property condensed_fraction --- ####
 property condensed_population --- #### property fields Method to print out the
 output fields for an OqtantOutput --- #### property get_bimodal_fit_parameters
 --- #### property image_type --- #### property model_computed_fields Get the
 computed fields of this model instance. **Returns:** A dictionary of computed
 field names and their corresponding `ComputedFieldInfo` objects. --- ####
```

### Comparing `oqtant-1.8.2/documentation/api/schemas.quantum_matter.md` & `oqtant-1.9.0/documentation/api/schemas.quantum_matter.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - **DEFAULT_LIFETIME**
 - **DEFAULT_TOF**
 - **TEMPERATURE_TO_EVAP_FREQUENCY**
 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L53"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L54"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `QuantumMatter`
 A class that represents user inputs to create and manipulate quantum matter 
 
 
 ---
 
@@ -165,15 +165,15 @@
  
  - <b>`str`</b>:  The time the current job was submitted 
 
 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L381"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L387"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `corrected_rf_power`
 
 ```python
 corrected_rf_power(frequency_mhz: 'float', power_mw: 'float') → float
 ```
 
@@ -190,15 +190,15 @@
 
 **Returns:**
  
  - <b>`float`</b>:  The corrected RF power in mW 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L405"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L411"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `corrected_rf_powers`
 
 ```python
 corrected_rf_powers(
     frequencies: 'list[float]',
     powers: 'list[float]'
@@ -218,45 +218,47 @@
 
 **Returns:**
  
  - <b>`list[float]`</b>:  The corrected list of RF powers in mW 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L210"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L211"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>classmethod</kbd> `from_input`
 
 ```python
 from_input(
     name: 'str',
     input: 'InputValues',
+    note: 'JobNote | None' = None,
     client: 'OqtantClient | None' = None
 ) → QuantumMatter
 ```
 
 Method to create a new QuantumMatter object using the input values of an existing job 
 
 
 
 **Args:**
  
  - <b>`name`</b> (str):  Name of the quantum matter 
  - <b>`input`</b> (bert_schemas.job.InputValues):  The input values 
+ - <b>`note`</b> (bert_schemas.job.JobNote | None):  The notes for the input, can be None 
  - <b>`client`</b> (oqtant.oqtant_client.OqtantClient | None, optional):  An instance of OqtantClient 
 
 
 
 **Returns:**
  
  - <b>`QuantumMatter`</b>:  A new QuantumMatter object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L259"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L263"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>classmethod</kbd> `from_oqtant_job`
 
 ```python
 from_oqtant_job(
     job: 'OqtantJob',
     client: 'OqtantClient',
@@ -278,15 +280,15 @@
 
 **Returns:**
  
  - <b>`QuantumMatter`</b>:  A new QuantumMatter object created using the OqtantJob data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L527"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L533"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_ideal_optical_potential`
 
 ```python
 get_ideal_optical_potential(
     time: 'float',
     positions: 'list[float]'
@@ -306,15 +308,15 @@
 
 **Returns:**
  
  - <b>`list[float]`</b>:  list of potential energies, in kHz, at the request time and positions 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L505"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L511"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_magnetic_potential`
 
 ```python
 get_magnetic_potential(positions: 'list[float]') → list[float]
 ```
 
@@ -330,15 +332,15 @@
 
 **Returns:**
  
  - <b>`list[float]`</b>:  List of magnetic potentials in kHz corresponding to the given positions 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L551"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L557"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_potential`
 
 ```python
 get_potential(
     time: 'float',
     positions: 'list[float]',
@@ -358,15 +360,15 @@
 
 **Returns:**
  
  - <b>`list[float]`</b>:  List of potential energy corresponding to each request position 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L365"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L371"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_result`
 
 ```python
 get_result(run: 'int' = 1) → None
 ```
 
@@ -376,41 +378,41 @@
 
 **Args:**
  
  - <b>`run`</b> (int, optional):  The specific run to get 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L332"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L338"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_sim_result`
 
 ```python
 get_sim_result() → None
 ```
 
 Method to get the results of a simulator job. Alerts the user if simulation results are invalid due to boundary collision. 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L74"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L75"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `model_post_init`
 
 ```python
 model_post_init(*args) → None
 ```
 
 
 
 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L284"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L290"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `output_values_to_oqtant_output`
 
 ```python
 output_values_to_oqtant_output(
     output_values: 'PlotOutput | NonPlotOutput'
 ) → OqtantPlotOutput | OqtantNonPlotOutput
@@ -427,27 +429,27 @@
 
 
 **Returns:**
  (oqtant.schemas.output.OqtantPlotOutput | oqtant.schemas.output.OqtantNonPlotOutput): The converted output values 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L622"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L628"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `show_barrier_dynamics`
 
 ```python
 show_barrier_dynamics() → None
 ```
 
 Method to plot the time dynamics of every Barrier object within a QuantumMatter object 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L572"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L578"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `show_potential`
 
 ```python
 show_potential(
     times: 'list' = [0.0],
     xlimits: 'list' = [-61.0, 61],
@@ -467,15 +469,15 @@
  - <b>`xlimits`</b> (list[float], optional):  The plot limits for the x axis 
  - <b>`ylimits`</b> (list[float], optional):  The plot limits for the y axis 
  - <b>`include_ideal`</b> (bool, optional):  Flag for including target potential in plot 
  - <b>`include_magnetic`</b> (bool, optional):  Flag to include contributions from magnetic trap 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L421"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L427"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `show_rf_dynamics`
 
 ```python
 show_rf_dynamics(corrected: 'bool' = False) → None
 ```
 
@@ -485,15 +487,15 @@
 
 **Args:**
  
  - <b>`corrected`</b> (bool, optional):  Flag to correct the RF power 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L316"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L322"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `submit`
 
 ```python
 submit(track: 'bool' = False, sim: 'bool' = False) → None
 ```
 
@@ -504,45 +506,45 @@
 **Args:**
  
  - <b>`track`</b> (bool, optional):  Flag to poll for job updates after submission 
  - <b>`sim`</b> (bool, optional):  Flag to use the simulator backend instead of real hardware 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L309"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L315"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `submit_sim`
 
 ```python
 submit_sim() → None
 ```
 
 Method to submit a QuantumMatter object to be run as a simulation 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L303"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L309"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `write_to_file`
 
 ```python
 write_to_file(*args, **kwargs) → None
 ```
 
 Method to write the results of a submitted QuantumMatter object to a file. Wrapper for OqtantClient.write_job_to_file 
 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L674"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L680"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ## <kbd>class</kbd> `QuantumMatterFactory`
 An abstract factory for creating instances of the QuantumMatter schema classes 
 
-<a href="../../oqtant/schemas/quantum_matter.py#L677"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L683"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `__init__`
 
 ```python
 __init__()
 ```
 
@@ -551,15 +553,15 @@
 
 
 
 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L918"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L930"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_barrier`
 
 ```python
 create_barrier(
     positions: 'list[float]' = [0.0, 0.0],
     heights: 'list[float]' = [0.0, 0.0],
@@ -593,15 +595,15 @@
 
 **Raises:**
  
  - <b>`ValueError`</b>:  if data lists are not of equal length 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L959"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L971"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_barrier_from_input`
 
 ```python
 create_barrier_from_input(input: 'Barrier') → Barrier
 ```
 
@@ -617,15 +619,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.optical.Barrier`</b>:  A new Barrier object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L882"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L894"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_landscape`
 
 ```python
 create_landscape(
     snapshots: 'list[Snapshot]' = [Snapshot(time_ms=0.0, potentials_khz=[0.0, 0.0], positions_um=[-10.0, 10.0], spatial_interpolation=<InterpolationType.LINEAR: 'LINEAR'>, interpolation_kind='linear'), Snapshot(time_ms=2.0, potentials_khz=[0.0, 0.0], positions_um=[-10.0, 10.0], spatial_interpolation=<InterpolationType.LINEAR: 'LINEAR'>, interpolation_kind='linear')]
 ) → Landscape
@@ -643,15 +645,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.optical.Landscape`</b>:  A new Landscape object 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L906"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L918"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_landscape_from_input`
 
 ```python
 create_landscape_from_input(input: 'OpticalLandscape') → Landscape
 ```
 
@@ -667,15 +669,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.optical.Landscape`</b>:  A new Landscape object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L791"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L799"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_quantum_matter`
 
 ```python
 create_quantum_matter(
     name: 'str | None' = None,
     temperature: 'float | None' = None,
@@ -713,43 +715,45 @@
 
 **Returns:**
  
  - <b>`QuantumMatter`</b>:  A new QuantumMatter object 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L830"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L838"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_quantum_matter_from_input`
 
 ```python
 create_quantum_matter_from_input(
     name: 'str',
-    input: 'InputValues'
+    input: 'InputValues',
+    note: 'JobNote | None' = None
 ) → QuantumMatter
 ```
 
 Method to create a QuantumMatter object using the input values of a job. Wrapper for QuantumMatter.from_input 
 
 
 
 **Args:**
  
  - <b>`name`</b> (str):  The name of the quantum matter 
  - <b>`input`</b> (bert_schemas.job.InputValues):  The input values 
+ - <b>`note`</b> (job_schema.job.JobNote | None):  The notes for the input, can be None 
 
 
 
 **Returns:**
  
  - <b>`QuantumMatter`</b>:  A new QuantumMatter object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L1008"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L1020"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_rf_evap`
 
 ```python
 create_rf_evap(
     times: 'list' = [0],
     powers: 'list' = [0],
@@ -773,15 +777,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.rf.RfEvap`</b>:  A new RfEvap object 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L1033"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L1045"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_rf_evap_from_input`
 
 ```python
 create_rf_evap_from_input(input: 'RfEvaporation') → RfEvap
 ```
 
@@ -797,15 +801,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.rf.RfEvap`</b>:  A new RfEvap object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L971"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L983"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_rf_sequence`
 
 ```python
 create_rf_sequence(
     times: 'list' = [0],
     powers: 'list' = [0],
@@ -829,15 +833,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.rf.RfSequence`</b>:  A new RfSequence object 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L996"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L1008"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_rf_sequence_from_input`
 
 ```python
 create_rf_sequence_from_input(input: 'RfEvaporation') → RfSequence
 ```
 
@@ -853,15 +857,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.rf.RfSequence`</b>:  A new RfSequence object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L1045"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L1057"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_rf_shield`
 
 ```python
 create_rf_shield(
     power: 'float' = 0,
     frequency: 'float' = 0,
@@ -883,15 +887,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.rf.RfShield`</b>:  A new RfShield object 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L1066"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L1078"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_rf_shield_from_input`
 
 ```python
 create_rf_shield_from_input(input: 'RfEvaporation') → RfShield
 ```
 
@@ -907,15 +911,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.rf.RfShield`</b>:  A new RfShield object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L845"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L857"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_snapshot`
 
 ```python
 create_snapshot(
     time: 'float' = 0,
     positions: 'list' = [-10, 10],
@@ -939,15 +943,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.optical.Snapshot`</b>:  A new Snapshot object 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L870"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L882"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `create_snapshot_from_input`
 
 ```python
 create_snapshot_from_input(input: 'Landscape') → Snapshot
 ```
 
@@ -963,15 +967,15 @@
 
 **Returns:**
  
  - <b>`oqtant.schemas.optical.Snapshot`</b>:  A new Snapshot object created using the input data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L767"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L775"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_batch_result`
 
 ```python
 get_batch_result(matter: 'QuantumMatter', run: 'int') → QuantumMatter
 ```
 
@@ -988,15 +992,15 @@
 
 **Returns:**
  
  - <b>`QuantumMatter`</b>:  A new QuantumMatter object created using the jobs data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L689"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L695"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_client`
 
 ```python
 get_client(token: 'str | None' = None) → None
 ```
 
@@ -1006,15 +1010,15 @@
 
 **Args:**
  
  - <b>`token`</b> (str | None, optional):  Token to use when working outside of a notebook 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L681"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L687"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `get_login`
 
 ```python
 get_login() → Auth
 ```
 
@@ -1024,15 +1028,15 @@
 
 **Returns:**
  
  - <b>`ipyauth.Auth`</b>:  The authentication widget 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L725"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L731"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `load_matter_from_file`
 
 ```python
 load_matter_from_file(*args, **kwargs) → QuantumMatter
 ```
 
@@ -1042,15 +1046,15 @@
 
 **Returns:**
  
  - <b>`QuantumMatter`</b>:  A new QuantumMatter object created using the file data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L735"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L741"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `load_matter_from_job_id`
 
 ```python
 load_matter_from_job_id(job_id: 'str', run: 'int' = 1) → QuantumMatter
 ```
 
@@ -1067,15 +1071,15 @@
 
 **Returns:**
  
  - <b>`QuantumMatter`</b>:  A new QuantumMatter object created using the jobs data 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L698"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L704"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `search_jobs`
 
 ```python
 search_jobs(*args, **kwargs) → list[dict]
 ```
 
@@ -1085,15 +1089,15 @@
 
 **Returns:**
  
  - <b>`list[dict]`</b>:  The jobs found for the search criteria 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L716"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L722"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `show_job_limits`
 
 ```python
 show_job_limits() → dict
 ```
 
@@ -1103,15 +1107,15 @@
 
 **Returns:**
  
  - <b>`dict`</b>:  The job limit information for the authenticated user 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L707"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L713"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `show_queue_status`
 
 ```python
 show_queue_status(*args, **kwargs) → list[dict]
 ```
 
@@ -1121,15 +1125,15 @@
 
 **Returns:**
  
  - <b>`list[dict]`</b>:  The jobs found for the search criteria along with their queue status 
 
 ---
 
-<a href="../../oqtant/schemas/quantum_matter.py#L758"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
+<a href="../../oqtant/schemas/quantum_matter.py#L766"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>
 
 ### <kbd>method</kbd> `submit_list_as_batch`
 
 ```python
 submit_list_as_batch(*args, **kwargs) → str
 ```
```

#### html2text {}

```diff
@@ -40,19 +40,20 @@
 `corrected_rf_powers` ```python corrected_rf_powers( frequencies: 'list
 [float]', powers: 'list[float]' ) â list[float] ``` Method to calculate the
 corrected RF powers based on the given lists of frequencies and powers **Args:
 ** - ``ffrreeqquueenncciieess`` (list[float]): The frequencies in MHz - ``ppoowweerrss`` (list
 [float]): The powers in mW **Returns:** - ``lliisstt[[ffllooaatt]]``: The corrected list of
 RF powers in mW --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
 _s_q_u_a_r_e_]### classmethod `from_input` ```python from_input( name: 'str', input:
-'InputValues', client: 'OqtantClient | None' = None ) â QuantumMatter ```
-Method to create a new QuantumMatter object using the input values of an
-existing job **Args:** - ``nnaammee`` (str): Name of the quantum matter - ``iinnppuutt``
-(bert_schemas.job.InputValues): The input values - ``cclliieenntt``
-(oqtant.oqtant_client.OqtantClient | None, optional): An instance of
+'InputValues', note: 'JobNote | None' = None, client: 'OqtantClient | None' =
+None ) â QuantumMatter ``` Method to create a new QuantumMatter object using
+the input values of an existing job **Args:** - ``nnaammee`` (str): Name of the
+quantum matter - ``iinnppuutt`` (bert_schemas.job.InputValues): The input values -
+``nnoottee`` (bert_schemas.job.JobNote | None): The notes for the input, can be None
+- ``cclliieenntt`` (oqtant.oqtant_client.OqtantClient | None, optional): An instance of
 OqtantClient **Returns:** - ``QQuuaannttuummMMaatttteerr``: A new QuantumMatter object created
 using the input data --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
 _c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### classmethod `from_oqtant_job` ```python
 from_oqtant_job( job: 'OqtantJob', client: 'OqtantClient', run: 'int' = 1 ) â
 QuantumMatter ``` Method to create a new QuantumMatter object using an existing
 OqtantJob **Args:** - ``jjoobb`` (oqtant.schemas.job.OqtantJob): The OqtantJob
 object to create from - ``cclliieenntt`` (oqtant.oqtant_client.OqtantClient): An
@@ -182,44 +183,46 @@
 RF shield - ``bbaarrrriieerrss`` (list[oqtant.schemas.optical.Barrier] | None, optional):
 The quantum matter barriers - ``llaannddssccaappee`` (oqtant.schemas.optical.Landscape |
 None, optional): The quantum matter landscape - ``llaasseerrss`` (list
 [bert_schemas.job.Lasers] | None, optional): The quantum matter lasers - ``nnoottee``
 (str | None, optional): A note about the quantum matter **Returns:** -
 ``QQuuaannttuummMMaatttteerr``: A new QuantumMatter object --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-
 _s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `create_quantum_matter_from_input`
-```python create_quantum_matter_from_input( name: 'str', input: 'InputValues' )
-â QuantumMatter ``` Method to create a QuantumMatter object using the input
-values of a job. Wrapper for QuantumMatter.from_input **Args:** - ``nnaammee`` (str):
-The name of the quantum matter - ``iinnppuutt`` (bert_schemas.job.InputValues): The
-input values **Returns:** - ``QQuuaannttuummMMaatttteerr``: A new QuantumMatter object created
-using the input data --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `create_rf_evap` ```python create_rf_evap
-( times: 'list' = [0], powers: 'list' = [0], frequencies: 'list' = [0],
-interpolation: 'str' = 'LINEAR' ) â RfEvap ``` Method to create a RfEvap
-object **Args:** - ``ttiimmeess`` (list[int], optional): The time values in
-milliseconds - ``ppoowweerrss`` (list[list[float], optional): The power values in
-milliwatts - ``ffrreeqquueenncciieess`` (list[float], optional): The frequency values in
-megahertz - ``iinntteerrppoollaattiioonn`` (bert_schemas.job.InterpolationType, optional): The
-interpolation type to be used **Returns:** - ``ooqqttaanntt..sscchheemmaass..rrff..RRffEEvvaapp``: A new
-RfEvap object --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_]### method `create_rf_evap_from_input` ```python
-create_rf_evap_from_input(input: 'RfEvaporation') â RfEvap ``` Method to
-create a RfEvap object from the input values of a job **Args:** - ``iinnppuutt``
-(bert_schemas.job.RfEvaporation): The input values **Returns:** -
-``ooqqttaanntt..sscchheemmaass..rrff..RRffEEvvaapp``: A new RfEvap object created using the input data --
-- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
-`create_rf_sequence` ```python create_rf_sequence( times: 'list' = [0], powers:
-'list' = [0], frequencies: 'list' = [0], interpolation: 'str' = 'LINEAR' ) â
-RfSequence ``` Method to create a RfSequence object **Args:** - ``ttiimmeess`` (list
-[int], optional): The time values in milliseconds - ``ppoowweerrss`` (list[list[float],
-optional): The power values in milliwatts - ``ffrreeqquueenncciieess`` (list[float],
-optional): The frequency values in megahertz - ``iinntteerrppoollaattiioonn``
+```python create_quantum_matter_from_input( name: 'str', input: 'InputValues',
+note: 'JobNote | None' = None ) â QuantumMatter ``` Method to create a
+QuantumMatter object using the input values of a job. Wrapper for
+QuantumMatter.from_input **Args:** - ``nnaammee`` (str): The name of the quantum
+matter - ``iinnppuutt`` (bert_schemas.job.InputValues): The input values - ``nnoottee``
+(job_schema.job.JobNote | None): The notes for the input, can be None
+**Returns:** - ``QQuuaannttuummMMaatttteerr``: A new QuantumMatter object created using the
+input data --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-
+_s_q_u_a_r_e_]### method `create_rf_evap` ```python create_rf_evap( times: 'list' =
+[0], powers: 'list' = [0], frequencies: 'list' = [0], interpolation: 'str' =
+'LINEAR' ) â RfEvap ``` Method to create a RfEvap object **Args:** - ``ttiimmeess``
+(list[int], optional): The time values in milliseconds - ``ppoowweerrss`` (list[list
+[float], optional): The power values in milliwatts - ``ffrreeqquueenncciieess`` (list
+[float], optional): The frequency values in megahertz - ``iinntteerrppoollaattiioonn``
 (bert_schemas.job.InterpolationType, optional): The interpolation type to be
-used **Returns:** - ``ooqqttaanntt..sscchheemmaass..rrff..RRffSSeeqquueennccee``: A new RfSequence object --
-- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+used **Returns:** - ``ooqqttaanntt..sscchheemmaass..rrff..RRffEEvvaapp``: A new RfEvap object --- _[_h_t_t_p_s_:
+_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
+`create_rf_evap_from_input` ```python create_rf_evap_from_input(input:
+'RfEvaporation') â RfEvap ``` Method to create a RfEvap object from the input
+values of a job **Args:** - ``iinnppuutt`` (bert_schemas.job.RfEvaporation): The input
+values **Returns:** - ``ooqqttaanntt..sscchheemmaass..rrff..RRffEEvvaapp``: A new RfEvap object created
+using the input data --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-
+_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `create_rf_sequence` ```python
+create_rf_sequence( times: 'list' = [0], powers: 'list' = [0], frequencies:
+'list' = [0], interpolation: 'str' = 'LINEAR' ) â RfSequence ``` Method to
+create a RfSequence object **Args:** - ``ttiimmeess`` (list[int], optional): The time
+values in milliseconds - ``ppoowweerrss`` (list[list[float], optional): The power
+values in milliwatts - ``ffrreeqquueenncciieess`` (list[float], optional): The frequency
+values in megahertz - ``iinntteerrppoollaattiioonn`` (bert_schemas.job.InterpolationType,
+optional): The interpolation type to be used **Returns:** -
+``ooqqttaanntt..sscchheemmaass..rrff..RRffSSeeqquueennccee``: A new RfSequence object --- _[_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method
 `create_rf_sequence_from_input` ```python create_rf_sequence_from_input(input:
 'RfEvaporation') â RfSequence ``` Method to create a RfSequence object from
 the input values of a job **Args:** - ``iinnppuutt ((bbeerrtt__sscchheemmaass..jjoobb..RRffEEvvaappoorraattiioonn``:
 The input values **Returns:** - ``ooqqttaanntt..sscchheemmaass..rrff..RRffSSeeqquueennccee``: A new
 RfSequence object created using the input data --- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_-_s_o_u_r_c_e_-_c_c_c_c_c_c_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]### method `create_rf_shield` ```python
 create_rf_shield( power: 'float' = 0, frequency: 'float' = 0, lifetime: 'float'
```

### Comparing `oqtant-1.8.2/documentation/api/schemas.rf.md` & `oqtant-1.9.0/documentation/api/schemas.rf.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/simulator.md` & `oqtant-1.9.0/documentation/api/simulator.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/simulator.qm_potential.md` & `oqtant-1.9.0/documentation/api/simulator.qm_potential.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/simulator.three_dim.md` & `oqtant-1.9.0/documentation/api/simulator.three_dim.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/simulator.wave_function.md` & `oqtant-1.9.0/documentation/api/simulator.wave_function.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/util.auth.md` & `oqtant-1.9.0/documentation/api/util.auth.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/api/util.exceptions.md` & `oqtant-1.9.0/documentation/api/util.exceptions.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/demos/demo_1_quantum_interference.ipynb` & `oqtant-1.9.0/documentation/examples/demos/demo_1_quantum_interference.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/demos/demo_2_multiple_slit_interference.ipynb` & `oqtant-1.9.0/documentation/examples/demos/demo_2_multiple_slit_interference.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/hello_world.ipynb` & `oqtant-1.9.0/documentation/examples/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/images/benchmark_machine.png` & `oqtant-1.9.0/documentation/examples/walkthroughs/images/benchmark_machine.png`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/images/sim_vs_TOF.png` & `oqtant-1.9.0/documentation/examples/walkthroughs/images/sim_vs_TOF.png`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/images/sim_vs_lifetime.png` & `oqtant-1.9.0/documentation/examples/walkthroughs/images/sim_vs_lifetime.png`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_1_introduction.ipynb` & `oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_1_introduction.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_2_making_quantum_matter.ipynb` & `oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_2_making_quantum_matter.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_3_optical_barriers.ipynb` & `oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_3_optical_barriers.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_4_optical_landscapes.ipynb` & `oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_4_optical_landscapes.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_5_experimentation_and_batch_jobs.ipynb` & `oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_5_experimentation_and_batch_jobs.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995273109243697%*

 * *Differences: {"'cells'": "{19: {'source': {insert: [(7, '        note=str(n + 1)\\n'), (8, '        + "*

 * *            '"/"\\n\'), (9, \'        + str(N),  # notes persist in batches and will remain tied '*

 * *            'to each matter object\\n\')], delete: [7]}}, 26: {\'source\': [\'print(f"Run: '*

 * *            '{first_run.run} of {len(matters)}")\\n\', \'print(f"Job Name: '*

 * *            '{first_run.name}")\\n\', \'print(f"Job Note: {first_run.note}")\\n\', \'print(f"Input '*

 * *            'Values: {first_run.input}")\\n\', \'pr […]*

```diff
@@ -200,15 +200,17 @@
                 "# create a list of QuantumMatter objects\n",
                 "N = 2\n",
                 "matters = [\n",
                 "    qmf.create_quantum_matter(\n",
                 "        temperature=50 * (n + 1),\n",
                 "        lifetime=20 + (n * 2),\n",
                 "        time_of_flight=3 + (n * 2),\n",
-                "        name=str(n + 1) + \"/\" + str(N),\n",
+                "        note=str(n + 1)\n",
+                "        + \"/\"\n",
+                "        + str(N),  # notes persist in batches and will remain tied to each matter object\n",
                 "    )\n",
                 "    for n in range(N)\n",
                 "]"
             ]
         },
         {
             "cell_type": "markdown",
@@ -266,20 +268,25 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(\"run\", first_run.run, \"of\", first_run.run_count)\n",
-                "print(second_run.run, \"of\", second_run.run_count)\n",
-                "print(first_run.input)\n",
-                "print(second_run.input)\n",
-                "print(first_run.output.temperature_nk)\n",
-                "print(second_run.output.temperature_nk)"
+                "print(f\"Run: {first_run.run} of {len(matters)}\")\n",
+                "print(f\"Job Name: {first_run.name}\")\n",
+                "print(f\"Job Note: {first_run.note}\")\n",
+                "print(f\"Input Values: {first_run.input}\")\n",
+                "print(f\"Temperature: {first_run.output.temperature_nk}\")\n",
+                "\n",
+                "print(f\"\\nRun: {second_run.run} of {len(matters)}\")\n",
+                "print(f\"Job Name: {second_run.name}\")\n",
+                "print(f\"Job Note: {first_run.note}\")\n",
+                "print(f\"Input Values: {second_run.input}\")\n",
+                "print(f\"Temperature: {second_run.output.temperature_nk}\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Plot the results together as above, but augment our approach at extracting the data:"
```

### Comparing `oqtant-1.8.2/documentation/examples/walkthroughs/walkthrough_6_simulator.ipynb` & `oqtant-1.9.0/documentation/examples/walkthroughs/walkthrough_6_simulator.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999245169082125%*

 * *Differences: {"'cells'": "{43: {'source': {insert: [(9, "*

 * *            "'![benchmark_machine](images/benchmark_machine.png)\\n')], delete: [12, 11, 10, 7]}}}"}*

```diff
@@ -532,18 +532,15 @@
                 "The available memory and time required to evaluate an Oqtant simulator job depend principally on the length of the different experimental stages specified. Memory and time do not scale significantly with experiment complexity (i.e. number of snapshots or barriers). TOF stage duration dominates evaluation time due to the larger grid size. For more information about grid size, see the [simulator technical note](https://www.oqtant.com/technical/simulator.md). \n",
                 "\n",
                 "### Benchmarking of the simulator\n",
                 "\n",
                 "Initial benchmarking was performed on simulation (```.get_result()```) only. Generating simulation outputs using access or plotting methods (```get_column_densities```, ```show_column_densities```) or any animations will incur additional processing time and memory usage. Benchmarking performed on the the following machine:\n",
                 "\n",
                 "\n",
-                "\n",
-                "<div>\n",
-                "<img            src=\"images/benchmark_machine.png\" alight=\"left\" width=\"500\"/>\n",
-                "</div>\n",
+                "![benchmark_machine](images/benchmark_machine.png)\n",
                 "\n",
                 "\n",
                 "\n",
                 "![lifetime profile results](images/sim_vs_lifetime.png)\n",
                 "\n",
                 "![TOF profile results](images/sim_vs_TOF.png)\n",
                 "\n",
```

### Comparing `oqtant-1.8.2/documentation/oqtant_client_docs.md` & `oqtant-1.9.0/documentation/oqtant_client_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/documentation/oqtant_rest_api_docs.md` & `oqtant-1.9.0/documentation/oqtant_rest_api_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/__init__.py` & `oqtant-1.9.0/oqtant/__init__.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/fixtures/__init__.py` & `oqtant-1.9.0/oqtant/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/fixtures/jobs.py` & `oqtant-1.9.0/oqtant/fixtures/jobs.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/oqtant_client.py` & `oqtant-1.9.0/oqtant/oqtant_client.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/schemas/__init__.py` & `oqtant-1.9.0/oqtant/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/schemas/job.py` & `oqtant-1.9.0/oqtant/schemas/job.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/schemas/optical.py` & `oqtant-1.9.0/oqtant/schemas/optical.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 
 import json
 
 import matplotlib.pyplot as plt
 import numpy as np
 from bert_schemas import job as job_schema
-from bert_schemas.job import Projected, interpolate_1d, interpolate_1d_list
+from bert_schemas import projected
 
 # Module containing methods and classes for abstractions of quasi-1D "painted" light Oqtant object
 
 # "ideal" optical potentials are those specified by the user using included objects
 # "actual" optical potentials include implementation and hardware realities
 # such as objects being projected as a sum of gaussians on a pre-defined position grid
 # with dynamic weights recalculated on a periodic basis
@@ -69,65 +69,31 @@
             landscape (bert_schemas.job.Landscape): The input values
 
         Returns:
             Snapshot: A new Snapshot object created using the input data
         """
         return cls(**landscape.model_dump())
 
-    def get_ideal_potential(
-        self, time=0.0, positions: list = Projected.PROJECTED_SPOTS
-    ) -> list[float]:
-        """Method to get the ideal potential energy at the specified positions
-
-        Args:
-            positions (list, optional): List of positions in microns
-
-        Returns:
-            list[float]: Potential energies, in kHz, at the specified positions
-        """
-        potentials = interpolate_1d_list(
-            self.positions_um,
-            self.potentials_khz,
-            positions,
-            self.spatial_interpolation,
-        )
-        return potentials
-
-    def get_potential(self, positions: list[float]) -> list[float]:
-        """Method to calculate the optical potential associated with a Landscape object,
-        taking into account the actual implementation of the Oqtant projection system,
-        at the given time
-
-        Args:
-            positions (list[float]): Positions, in microns, where the potential should be evaluated
-
-        Returns:
-            list[float]: Potential energies, in kHz, at the specified positions
-        """
-        return Projected.get_actual_potential(
-            self.get_ideal_potential, positions=positions
-        )
-
     def show_potential(
         self,
-        xlimits: list[float] = [Projected.POSITION_MIN - 1, Projected.POSITION_MAX + 1],
-        ylimits: list[float] = [Projected.ENERGY_MIN - 1, Projected.ENERGY_MAX + 1],
+        xlimits: list[float] = [projected.POSITION_MIN - 1, projected.POSITION_MAX + 1],
+        ylimits: list[float] = [projected.ENERGY_MIN - 1, projected.ENERGY_MAX + 1],
         include_ideal: bool = False,
     ) -> None:
         """Method to plot the potential energy as a function of position for a Landscape
         object at the given times
 
         Args:
             xlimits (list[float], optional): Plot limits for x axis
             ylimits (list[float], optional): Plot limits for y axis
             include_ideal (bool, optional): Flag for including target potential in plot
         """
 
         positions = np.arange(
-            Projected.POSITION_MIN, Projected.POSITION_MAX + 0.1, 0.1, dtype=float
+            projected.POSITION_MIN, projected.POSITION_MAX + 0.1, 0.1, dtype=float
         )
 
         _, ax = plt.subplots()
         color = next(ax._get_lines.prop_cycler)["color"]
         (ln,) = plt.plot(
             positions, self.get_potential(positions=positions), color=color
         )
@@ -202,80 +168,31 @@
         """Property to get a list of Snapshot objects associated to a Landscape object
 
         Returns:
             list[Snapshot]: List of Snapshot objects
         """
         return [Snapshot(**landscape.model_dump()) for landscape in self.landscapes]
 
-    def get_ideal_potential(
-        self, time: float, positions: list[float] = Projected.PROJECTED_SPOTS
-    ) -> list[float]:
-        """Method to calculate ideal object potential energy at the specified time and positions
-
-        Args:
-            time (float): Time, in ms, at which the potential energy is calculated
-            positions (list[float], optional): Positions at which the potential energy is calculated
-
-        Returns:
-            list[float]: Potential energies, in kHz, at specified time and positions
-        """
-        potential = [0] * len(positions)
-        snaps = self.snapshots
-        if len(snaps) < 2:
-            return potential
-        snap_times = [snap.time_ms for snap in snaps]
-        if time >= min(snap_times) and time <= max(snap_times):
-            pre = next(snap for snap in reversed(snaps) if snap.time_ms <= time)
-            nex = next(snap for snap in snaps if snap.time_ms >= time)
-            potential = [
-                interpolate_1d(
-                    [pre.time_ms, nex.time_ms], [p1, p2], time, self.interpolation
-                )
-                for p1, p2 in zip(
-                    pre.get_ideal_potential(positions=positions),
-                    nex.get_ideal_potential(positions=positions),
-                )
-            ]
-        return potential
-
-    def get_potential(
-        self, time: float, positions: list = Projected.PROJECTED_SPOTS
-    ) -> list[float]:
-        """Method to calculate the optical potential associated with a Landscape object,
-        taking into account the actual implementation of the Oqtant projection system,
-        at the given time
-
-        Args:
-            time (float): Time, in ms, at which to sample the potential energy
-            positions (list[float], optional): Positions, in microns, where the potential should be evaluated
-
-        Returns:
-            list[float]: Potential energies, in kHz, at the requested positions and time
-        """
-        return Projected.get_actual_potential(
-            self.get_ideal_potential, time=time, positions=positions
-        )
-
     def show_potential(
         self,
         times: list = [0.0],
-        xlimits: list = [Projected.POSITION_MIN - 1, Projected.POSITION_MAX + 1],
-        ylimits: list = [Projected.ENERGY_MIN - 1, Projected.ENERGY_MAX + 1],
+        xlimits: list = [projected.POSITION_MIN - 1, projected.POSITION_MAX + 1],
+        ylimits: list = [projected.ENERGY_MIN - 1, projected.ENERGY_MAX + 1],
         include_ideal: bool = False,
     ):
         """Method to plot the potential energy as a function of position for a Landscape object at the given times
 
         Args:
             times (list[float], optional): Times, in ms, at which to evaluate and plot the potential
             xlimits (list[float], optional): Plot limits for x axis
             ylimits (list[float], optional): Plot limits for y axis
             include_ideal (bool, optional): Flag for including target potential in plot
         """
         positions = np.arange(
-            Projected.POSITION_MIN, Projected.POSITION_MAX + 0.1, 0.1, dtype=float
+            projected.POSITION_MIN, projected.POSITION_MAX + 0.1, 0.1, dtype=float
         )
 
         fig, ax = plt.subplots()
         lns = []
         labs = []
         for time in times:
             potentials = self.get_potential(time, positions)
@@ -360,26 +277,26 @@
     def show_dynamics(self) -> None:
         """Method to plot the position, width and height of a Barrier object over time"""
         tstart = min(self.times_ms)
         tstop = max(self.times_ms)
         times = np.linspace(
             tstart,
             tstop,
-            num=int((tstop - tstart) / Projected.UPDATE_PERIOD),
+            num=int((tstop - tstart) / projected.UPDATE_PERIOD),
             endpoint=True,
         )
         fig, ax1 = plt.subplots()
 
         # plot position and width vs time
         style = "steps-pre"
         color = next(ax1._get_lines.prop_cycler)["color"]
         ax1.set_xlabel("time (ms)")
         ax1.set_ylabel("position or width (microns)")
         ax1.set_xlim([-1, self.times_ms[-1] + 1])
-        ax1.set_ylim([Projected.POSITION_MIN - 1, Projected.POSITION_MAX + 1])
+        ax1.set_ylim([projected.POSITION_MIN - 1, projected.POSITION_MAX + 1])
         (ln1,) = plt.plot(
             times, self.get_positions(times), color=color, drawstyle=style
         )
         plt.plot(
             self.times_ms,
             self.get_positions(self.times_ms),
             ".",
@@ -403,16 +320,16 @@
         plt.title("Barrier dynamics")
         fig.tight_layout()
         plt.show()
 
     def show_potential(
         self,
         times: list[float] = [0.0],
-        xlimits: list[float] = [Projected.POSITION_MIN - 1, Projected.POSITION_MAX + 1],
-        ylimits: list[float] = [Projected.ENERGY_MIN - 1, Projected.ENERGY_MAX + 1],
+        xlimits: list[float] = [projected.POSITION_MIN - 1, projected.POSITION_MAX + 1],
+        ylimits: list[float] = [projected.ENERGY_MIN - 1, projected.ENERGY_MAX + 1],
         include_ideal: bool = False,
     ) -> None:
         """Method to plot the potential energy as a function of position for a Barrier object
 
         Args:
             times (list[float], optional): The times, in ms, at which the potential is evaluated
             xlimits (list[float], optional): Plot limits for x axis
```

### Comparing `oqtant-1.8.2/oqtant/schemas/output.py` & `oqtant-1.9.0/oqtant/schemas/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -618,18 +618,20 @@
         ax.view_init(30, view_angle)
 
         if file_name:
             self._save_plot_file(plt, file_name)
         plt.show()
 
 
-class OqtantPlotOutput(OqtantOutput, job_schema.PlotOutput): ...
+class OqtantPlotOutput(OqtantOutput, job_schema.PlotOutput):
+    ...
 
 
-class OqtantNonPlotOutput(OqtantOutput, job_schema.NonPlotOutput): ...
+class OqtantNonPlotOutput(OqtantOutput, job_schema.NonPlotOutput):
+    ...
 
 
 def round_sig(x: float, sig: int = 2) -> float:
     """Method to round a number to a specified number of significant digits
 
     Args:
         x (float): The number to be rounded
@@ -665,15 +667,15 @@
         numpy.ndarray: a 2D array of samples from a Thomas Fermi distribution
     """
 
     # unpack 1D list into 2D x and y coords
     (x, y) = xy_mesh
 
     # Simplify Thomas-Fermi expression
-    A = 1 - ((y - yc) / rx) ** 2 - ((x - xc) / ry) ** 2
+    A = 1 - ((y - yc) / ry) ** 2 - ((x - xc) / rx) ** 2
 
     # make 2D Thomas-Fermi distribution
     OD = np.real(TFpOD * np.maximum(np.sign(A) * (np.abs(A)) ** (3 / 2), 0)) + os
 
     # flatten the 2D Gaussian down to 1D
     return OD.ravel()
```

### Comparing `oqtant-1.8.2/oqtant/schemas/quantum_matter.py` & `oqtant-1.9.0/oqtant/schemas/quantum_matter.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 import warnings
 from copy import deepcopy
 from typing import TYPE_CHECKING
 
 import matplotlib.pyplot as plt
 import numpy as np
 from bert_schemas import job as job_schema
+from bert_schemas import projected
 from bert_schemas.job import NonPlotOutput, PlotOutput
 from ipyauth import Auth
 from pydantic import BaseModel, confloat, conint
 
 from oqtant import oqtant_client as oq
 from oqtant.schemas.job import OqtantJob
-from oqtant.schemas.optical import Barrier, Landscape, Projected, Snapshot
+from oqtant.schemas.optical import Barrier, Landscape, Snapshot
 from oqtant.schemas.output import OqtantNonPlotOutput, OqtantPlotOutput
 from oqtant.schemas.rf import ConversionError, RfEvap, RfSequence, RfShield
 from oqtant.simulator import Simulator
 from oqtant.util.auth import notebook_login
 
 if TYPE_CHECKING:
     from oqtant.oqtant_client import OqtantClient
@@ -59,15 +60,15 @@
     image: job_schema.ImageType | None = DEFAULT_IMAGE
     time_of_flight: confloat(ge=2, le=20) | None = DEFAULT_TOF
     rf_evap: RfEvap | None = None
     rf_shield: RfShield | None = None
     barriers: list[Barrier | job_schema.Barrier] | None = None
     landscape: Landscape | job_schema.OpticalLandscape | None = None
     lasers: list[job_schema.Laser] | None = None
-    note: str | None = None
+    note: job_schema.JobNote | None = None
     client: object | None = None
     result: object | None = None
     job_id: str | None = None
     output: object | None = None
     is_sim: bool = False
     sim: Simulator | None = None
 
@@ -208,21 +209,23 @@
         return rf_evaporation
 
     @classmethod
     def from_input(
         cls,
         name: str,
         input: job_schema.InputValues,
+        note: job_schema.JobNote | None = None,
         client: OqtantClient | None = None,
     ) -> QuantumMatter:
         """Method to create a new QuantumMatter object using the input values of an existing job
 
         Args:
             name (str): Name of the quantum matter
             input (bert_schemas.job.InputValues): The input values
+            note (bert_schemas.job.JobNote | None): The notes for the input, can be None
             client (oqtant.oqtant_client.OqtantClient | None, optional): An instance of OqtantClient
 
         Returns:
             QuantumMatter: A new QuantumMatter object created using the input data
         """
         try:
             evap = RfEvap.from_input(input.rf_evaporation)
@@ -250,14 +253,15 @@
             time_of_flight=input.time_of_flight_ms,
             rf_evap=evap,
             rf_shield=shield,
             barriers=barriers,
             landscape=landscape,
             lasers=input.lasers,
             client=client,
+            note=note,
         )
 
     @classmethod
     def from_oqtant_job(
         cls, job: OqtantJob, client: OqtantClient, run: int = 1
     ) -> QuantumMatter:
         """Method to create a new QuantumMatter object using an existing OqtantJob
@@ -267,15 +271,17 @@
             client (oqtant.oqtant_client.OqtantClient): An instance of OqtantClient
             run (int, optional): The specific run to use
 
         Returns:
             QuantumMatter: A new QuantumMatter object created using the OqtantJob data
         """
         inputs = job.inputs[run - 1]
-        qm = QuantumMatter.from_input(name=job.name, input=inputs.values, client=client)
+        qm = QuantumMatter.from_input(
+            name=job.name, input=inputs.values, note=inputs.notes, client=client
+        )
         qm.job_id = str(job.external_id)
         qm.result = job
 
         if inputs.output:
             qm.output = QuantumMatter.output_values_to_oqtant_output(
                 inputs.output.values
             )
@@ -557,41 +563,41 @@
             time (float): The time at which to calculate the potential
             positions (list[float]): The positions at which to calculate the potential
             include_magnetic (bool, optional): Flag to include contributions from magnetic trap
         Returns:
             list[float]: List of potential energy corresponding to each request position
         """
         potential = np.asarray(
-            Projected.get_actual_potential(
+            projected.get_actual_potential(
                 self.get_ideal_optical_potential, time=time, positions=positions
             )
         )
         if include_magnetic:
             potential += np.asarray(self.get_magnetic_potential(positions=positions))
         return list(potential)
 
     def show_potential(
         self,
         times: list = [0.0],
-        xlimits: list = [Projected.POSITION_MIN - 1, Projected.POSITION_MAX + 1],
-        ylimits: list = [Projected.ENERGY_MIN - 1, Projected.ENERGY_MAX + 1],
+        xlimits: list = [projected.POSITION_MIN - 1, projected.POSITION_MAX + 1],
+        ylimits: list = [projected.ENERGY_MIN - 1, projected.ENERGY_MAX + 1],
         include_ideal: bool = False,
         include_magnetic: bool = True,
     ) -> None:
         """Method to plot the (optical) potential energy surface at the specified times
 
         Args:
             times (list[float], optional): The times for which to display the potential energy
             xlimits (list[float], optional): The plot limits for the x axis
             ylimits (list[float], optional): The plot limits for the y axis
             include_ideal (bool, optional): Flag for including target potential in plot
             include_magnetic (bool, optional): Flag to include contributions from magnetic trap
         """
         positions = np.arange(
-            Projected.POSITION_MIN, Projected.POSITION_MAX + 0.1, 0.1, dtype=float
+            projected.POSITION_MIN, projected.POSITION_MAX + 0.1, 0.1, dtype=float
         )
         fig, ax = plt.subplots()
         lns = []
         labs = []
         for time in times:
             color = next(ax._get_lines.prop_cycler)["color"]
             (ln,) = plt.plot(
@@ -742,17 +748,19 @@
         Returns:
             QuantumMatter: A new QuantumMatter object created using the jobs data
         """
         result = self.client.get_job(job_id, run)
         if result.status == job_schema.JobStatus.COMPLETE:
             output_values = result.inputs[0].output.values
             output = QuantumMatter.output_values_to_oqtant_output(output_values)
+        else:
+            output = None
 
         matter = self.create_quantum_matter_from_input(
-            name=result.name, input=result.inputs[0].values
+            name=result.name, input=result.inputs[0].values, note=result.inputs[0].notes
         )
         matter.output = output
         matter.job_id = job_id
         matter.result = result
         return matter
 
     def submit_list_as_batch(self, *args, **kwargs) -> str:
@@ -772,15 +780,15 @@
             run (int, optional): The specific run to get
 
         Returns:
             QuantumMatter: A new QuantumMatter object created using the jobs data
         """
         result = self.client.get_job(matter.job_id, run)
         new_matter = self.create_quantum_matter_from_input(
-            name=result.name, input=result.inputs[0].values
+            name=result.name, note=result.inputs[0].notes, input=result.inputs[0].values
         )
         new_matter.job_id = matter.job_id
         new_matter.result = result
         if result.status == job_schema.JobStatus.COMPLETE:
             output_values = result.inputs[0].output.values
             new_matter.output = QuantumMatter.output_values_to_oqtant_output(
                 output_values
@@ -824,27 +832,31 @@
         for k, v in locals().items():
             if v is not None:
                 kwargs[k] = v
 
         return QuantumMatter(**kwargs)
 
     def create_quantum_matter_from_input(
-        self, name: str, input: job_schema.InputValues
+        self,
+        name: str,
+        input: job_schema.InputValues,
+        note: job_schema.JobNote | None = None,
     ) -> QuantumMatter:
         """Method to create a QuantumMatter object using the input values of a job.
         Wrapper for QuantumMatter.from_input
 
         Args:
             name (str): The name of the quantum matter
             input (bert_schemas.job.InputValues): The input values
+            note (job_schema.job.JobNote | None): The notes for the input, can be None
 
         Returns:
             QuantumMatter: A new QuantumMatter object created using the input data
         """
-        return QuantumMatter.from_input(name, input, self.client)
+        return QuantumMatter.from_input(name, input, note, self.client)
 
     @staticmethod
     def create_snapshot(
         time: float = 0,
         positions: list = [-10, 10],
         potentials: list = [0, 0],
         interpolation: job_schema.InterpolationType = "LINEAR",
@@ -877,15 +889,15 @@
         Returns:
             oqtant.schemas.optical.Snapshot: A new Snapshot object created using the input data
         """
         return Snapshot(**input.model_dump())
 
     @staticmethod
     def create_landscape(
-        snapshots: list[Snapshot] = [Snapshot.new(time=0), Snapshot.new(time=2)]
+        snapshots: list[Snapshot] = [Snapshot.new(time=0), Snapshot.new(time=2)],
     ) -> Landscape:
         """Method to create a Landscape object from a list Snapshot objects
 
         Args:
             snapshots (list[oqtant.schemas.optical.Snapshot], optional): List of snapshots, defaults if not provided
 
         Returns:
```

### Comparing `oqtant-1.8.2/oqtant/schemas/rf.py` & `oqtant-1.9.0/oqtant/schemas/rf.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/settings.py` & `oqtant-1.9.0/oqtant/settings.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/simulator/__init__.py` & `oqtant-1.9.0/oqtant/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/simulator/qm_potential.py` & `oqtant-1.9.0/oqtant/simulator/qm_potential.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/simulator/simulator.py` & `oqtant-1.9.0/oqtant/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/simulator/three_dim.py` & `oqtant-1.9.0/oqtant/simulator/three_dim.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/simulator/wave_function.py` & `oqtant-1.9.0/oqtant/simulator/wave_function.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/util/__init__.py` & `oqtant-1.9.0/oqtant/util/__init__.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/util/auth.py` & `oqtant-1.9.0/oqtant/util/auth.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/util/exceptions.py` & `oqtant-1.9.0/oqtant/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/oqtant/util/server.py` & `oqtant-1.9.0/oqtant/util/server.py`

 * *Files identical despite different names*

### Comparing `oqtant-1.8.2/pyproject.toml` & `oqtant-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqtant"
-version = "1.8.2"
+version = "1.9.0"
 description = "Oqtant Desktop Suite"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Hannah North <hannah.north@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
   "Noah Fitch <noah.fitch@coldquanta.com>",
 ]
@@ -47,15 +47,15 @@
 ipyauth = "^0.2.6"
 ipywidgets = "^7.6.5"
 python-dateutil = "^2.8.2"
 fastapi = "^0.103.1"
 pydantic = "^2.3.0"
 email-validator = "^2.0.0.post2"
 pydantic-settings = "^2.0.3"
-bert-schemas = {version = "^2.5.0", source = "bert-packages"}
+bert-schemas = {version = "2.6.0", source = "bert-packages"}
 traitlets = "5.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-xdist = "^3.2.0"
 pytest-ordering = "^0.6"
 pytest-cov = "^4.0.0"
```

### Comparing `oqtant-1.8.2/PKG-INFO` & `oqtant-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: oqtant
-Version: 1.8.2
+Version: 1.9.0
 Summary: Oqtant Desktop Suite
 Home-page: https://oqtant.infleqtion.com/
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bert-schemas (>=2.5.0,<3.0.0)
+Requires-Dist: bert-schemas (==2.6.0)
 Requires-Dist: email-validator (>=2.0.0.post2,<3.0.0)
 Requires-Dist: fastapi (>=0.103.1,<0.104.0)
 Requires-Dist: ipyauth (>=0.2.6,<0.3.0)
 Requires-Dist: ipykernel (>=6.23.1,<7.0.0)
 Requires-Dist: ipywidgets (>=7.6.5,<8.0.0)
 Requires-Dist: lmfit (>=1.0.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<3.7.0)
```

