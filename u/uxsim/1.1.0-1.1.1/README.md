# Comparing `tmp/uxsim-1.1.0.tar.gz` & `tmp/uxsim-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxsim-1.1.0.tar", last modified: Mon Apr  1 12:21:14 2024, max compression
+gzip compressed data, was "uxsim-1.1.1.tar", last modified: Mon Apr 15 10:46:50 2024, max compression
```

## Comparing `uxsim-1.1.0.tar` & `uxsim-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.674981 uxsim-1.1.0/
--rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    14009 2024-04-01 12:21:14.673967 uxsim-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    13108 2024-04-01 11:09:22.000000 uxsim-1.1.0/README.md
--rw-rw-rw-   0        0        0     1132 2024-03-26 09:57:16.000000 uxsim-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 12:21:14.674981 uxsim-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.609380 uxsim-1.1.0/tests/
--rw-rw-rw-   0        0        0     1523 2024-03-26 09:57:16.000000 uxsim-1.1.0/tests/test_examples.py
--rw-rw-rw-   0        0        0     1682 2024-03-26 03:14:04.000000 uxsim-1.1.0/tests/test_result_gui_viewer.py
--rw-rw-rw-   0        0        0     3326 2024-03-26 04:14:08.000000 uxsim-1.1.0/tests/test_verification_exceptional.py
--rw-rw-rw-   0        0        0    69316 2024-04-01 11:10:22.000000 uxsim-1.1.0/tests/test_verification_multilane.py
--rw-rw-rw-   0        0        0    42414 2024-03-29 08:55:07.000000 uxsim-1.1.0/tests/test_verification_node.py
--rw-rw-rw-   0        0        0    22326 2024-03-31 13:21:16.000000 uxsim-1.1.0/tests/test_verification_route_choice.py
--rw-rw-rw-   0        0        0     3784 2024-03-22 02:43:13.000000 uxsim-1.1.0/tests/test_verification_sioux_falls.py
--rw-rw-rw-   0        0        0    39162 2024-03-26 04:14:43.000000 uxsim-1.1.0/tests/test_verification_straight_road.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.614969 uxsim-1.1.0/uxsim/
-drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.642968 uxsim-1.1.0/uxsim/OSMImporter/
--rw-rw-rw-   0        0        0    16170 2024-04-01 09:24:47.000000 uxsim-1.1.0/uxsim/OSMImporter/OSMImporter.py
--rw-rw-rw-   0        0        0       26 2024-03-26 02:31:54.000000 uxsim-1.1.0/uxsim/OSMImporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.646971 uxsim-1.1.0/uxsim/ResultGUIViewer/
--rw-rw-rw-   0        0        0    17979 2024-03-27 03:42:24.000000 uxsim-1.1.0/uxsim/ResultGUIViewer/ResultGUIViewer.py
--rw-rw-rw-   0        0        0       30 2024-03-25 09:10:21.000000 uxsim-1.1.0/uxsim/ResultGUIViewer/__init__.py
--rw-rw-rw-   0        0        0      193 2024-04-01 07:03:19.000000 uxsim-1.1.0/uxsim/__init__.py
--rw-rw-rw-   0        0        0    53987 2024-03-29 05:21:02.000000 uxsim-1.1.0/uxsim/analyzer.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.671935 uxsim-1.1.0/uxsim/files/
--rw-rw-rw-   0        0        0 10695124 2023-05-03 08:50:59.000000 uxsim-1.1.0/uxsim/files/HackGen-Regular.ttf
--rw-rw-rw-   0        0        0    58464 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/Inconsolata.otf
--rw-rw-rw-   0        0        0     5826 2024-03-27 03:00:30.000000 uxsim-1.1.0/uxsim/files/LICENSE_of_HackGen-Regular
--rw-rw-rw-   0        0        0     4486 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/Licence_of_Inconsolata.otf.txt
--rw-rw-rw-   0        0        0       47 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/README.md
--rw-rw-rw-   0        0        0        0 2024-03-26 09:57:16.000000 uxsim-1.1.0/uxsim/files/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-03-22 02:43:13.000000 uxsim-1.1.0/uxsim/utils.py
--rw-rw-rw-   0        0        0    77449 2024-04-01 10:29:15.000000 uxsim-1.1.0/uxsim/uxsim.py
-drwxrwxrwx   0        0        0        0 2024-04-01 12:21:14.672953 uxsim-1.1.0/uxsim.egg-info/
--rw-rw-rw-   0        0        0    14009 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      863 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-01 12:21:14.000000 uxsim-1.1.0/uxsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 10:46:50.003897 uxsim-1.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12181 2024-04-15 10:46:50.002899 uxsim-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11281 2024-04-08 12:09:02.000000 uxsim-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1123 2024-04-06 11:27:18.000000 uxsim-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 10:46:50.003897 uxsim-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.949399 uxsim-1.1.1/tests/
+-rw-rw-rw-   0        0        0     1523 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_examples.py
+-rw-rw-rw-   0        0        0     6650 2024-04-10 07:28:00.000000 uxsim-1.1.1/tests/test_other_functions.py
+-rw-rw-rw-   0        0        0     1682 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_result_gui_viewer.py
+-rw-rw-rw-   0        0        0     3326 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_verification_exceptional.py
+-rw-rw-rw-   0        0        0    69316 2024-04-01 12:42:58.000000 uxsim-1.1.1/tests/test_verification_multilane.py
+-rw-rw-rw-   0        0        0    42414 2024-04-01 12:42:58.000000 uxsim-1.1.1/tests/test_verification_node.py
+-rw-rw-rw-   0        0        0    26886 2024-04-15 10:46:18.000000 uxsim-1.1.1/tests/test_verification_route_choice.py
+-rw-rw-rw-   0        0        0     3784 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_verification_sioux_falls.py
+-rw-rw-rw-   0        0        0    39162 2024-04-01 12:42:22.000000 uxsim-1.1.1/tests/test_verification_straight_road.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.953878 uxsim-1.1.1/uxsim/
+drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.974900 uxsim-1.1.1/uxsim/OSMImporter/
+-rw-rw-rw-   0        0        0    16334 2024-04-09 08:40:41.000000 uxsim-1.1.1/uxsim/OSMImporter/OSMImporter.py
+-rw-rw-rw-   0        0        0       26 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/OSMImporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:46:49.977899 uxsim-1.1.1/uxsim/ResultGUIViewer/
+-rw-rw-rw-   0        0        0    16823 2024-04-09 09:16:07.000000 uxsim-1.1.1/uxsim/ResultGUIViewer/ResultGUIViewer.py
+-rw-rw-rw-   0        0        0       30 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/ResultGUIViewer/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/__init__.py
+-rw-rw-rw-   0        0        0    55213 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/analyzer.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:46:50.000899 uxsim-1.1.1/uxsim/files/
+-rw-rw-rw-   0        0        0 10695124 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/HackGen-Regular.ttf
+-rw-rw-rw-   0        0        0    58464 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/Inconsolata.otf
+-rw-rw-rw-   0        0        0     5951 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/LICENSE_of_HackGen-Regular
+-rw-rw-rw-   0        0        0     4486 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/Licence_of_Inconsolata.otf.txt
+-rw-rw-rw-   0        0        0       47 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/README.md
+-rw-rw-rw-   0        0        0        0 2024-04-01 12:42:22.000000 uxsim-1.1.1/uxsim/files/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/utils.py
+-rw-rw-rw-   0        0        0    80146 2024-04-15 10:46:18.000000 uxsim-1.1.1/uxsim/uxsim.py
+drwxrwxrwx   0        0        0        0 2024-04-15 10:46:50.001896 uxsim-1.1.1/uxsim.egg-info/
+-rw-rw-rw-   0        0        0    12181 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      893 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 10:46:49.000000 uxsim-1.1.1/uxsim.egg-info/top_level.txt
```

### Comparing `uxsim-1.1.0/LICENSE` & `uxsim-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/PKG-INFO` & `uxsim-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uxsim
-Version: 1.1.0
+Version: 1.1.1
 Summary: UXsim: traffic flow simulator
 Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
 License: MIT License
 Project-URL: Homepage, https://github.com/toruseo/UXsim
-Project-URL: Download, https://github.com/toruseo/UXsim
-Project-URL: Bug Tracker, https://github.com/toruseo/UXsim/issues
+Project-URL: Documentation, https://toruseo.jp/UXsim/docs
+Project-URL: Issues, https://github.com/toruseo/UXsim/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -31,75 +31,76 @@
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
 [![Static Badge](https://img.shields.io/badge/readme-%E6%97%A5%E6%9C%AC%E8%AA%9E%20%F0%9F%87%AF%F0%9F%87%B5%20-pink)](https://github.com/toruseo/UXsim/blob/main/README.jp.md)
 
 *UXsim* is a free, open-source macroscopic and mesoscopic network traffic flow simulator written in Python.
 It simulates the movements of car travelers and traffic congestion in road networks.
-It is suitable for simulating large-scale (e.g. city-scale) traffic phenomena.
-UXsim would be especially useful for scientific and educational purposes because of its simple, lightweight, and customizable features, but of course users are free to use UXsim for any purpose.
+It is suitable for simulating large-scale (e.g., city-scale) traffic phenomena.
+UXsim is especially useful for scientific and educational purposes because of its simple, lightweight, and customizable features, but users are free to use UXsim for any purpose.
 
-If you are interested in, please see
+If you are interested, please see:
 
 - [Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations and tutorials
 - [Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 
 ## Main Features
 
-- Simple, lightweight, and easy-to-use Python implementation of the modern standard models of dynamic network traffic flow.
-- Macroscopic traffic simulation: Simulating over 60000 vehicles in 30 seconds in a city.
-- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand.
-- Implementation of traffic control/management schemes such as traffic signals and road pricing.
-- Basic analysis of simulation results and their export to pandas.DataFrame and CSV files.
-- Visualization of simulation results using matplotlib. Interactive GUI is available.
-- Flexible and customizable thanks to pure Python implementation. Can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control.
+- Simple, lightweight, and easy-to-use Python implementation of modern standard models of dynamic network traffic flow
+- Macroscopic traffic simulation: Simulating over 60000 vehicles in a city in 30 seconds
+- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand
+- Theoretically valid models commonly used in academic/professional transportation research
+- Implementation of traffic control/management schemes such as traffic signals and road pricing
+- Basic analysis of simulation results and their export to pandas.DataFrame and CSV files
+- Visualization of simulation results using matplotlib; interactive GUI is available
+- Flexible and customizable thanks to pure Python implementation; can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
-Belows are simulation result where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
+Below are simulation results where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
 
 Visualization of link traffic states (thicker lines mean more vehicles, darker colors mean slower speeds) and some vehicle trajectories:
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/gridnetwork_macro.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/gridnetwork_fancy.gif" width="400"/>
 </p>
 
 Vehicle trajectory diagram on a corridor of the above network:
 <img src="https://github.com/toruseo/UXsim/blob/images/tsd_traj_links_grid.png" width="600">
 
 ### Deep reinforcement learning signal control using PyTorch
 
-Traffic signal controller is trained by deep reinforcement learning (DRL) of [PyTorch](https://pytorch.org/).
-The left (or upper) is no control scenario with fixed signal timing; the traffic demand exceeds the network capacity with naive signal setting, and a gridlock occurs.
-The right (or bottom) is with DRL control scenario, where traffic signal can be changed by observing queue length; although the demand level is the same, traffic is smoothly flowing.
-[Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
+A traffic signal controller is trained by deep reinforcement learning (DRL) using [PyTorch](https://pytorch.org/).
+The left (or upper) scenario shows no control with fixed signal timing; the traffic demand exceeds the network capacity with the naive signal setting, and a gridlock occurs.
+The right (or bottom) scenario shows DRL control, where the traffic signal can be changed by observing queue length; although the demand level is the same, traffic flows smoothly.
+A [Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
 
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_nocontrol.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_DQL.gif" width="400"/>
 </p>
 
 ### Interactive GUI for exploring a simulation result
 
 https://github.com/toruseo/UXsim/assets/34780089/ec780a33-d9ba-4068-a005-0b06127196d9
 
 ## Install
 
 ### Using pip
 
-The simplest way is using pip to install from PyPI.
+The simplest way is to use pip to install from PyPI:
 
 ```
 pip install uxsim
 ```
 
 <details>
-<summary>Alternative methods (click to see)</summary>
+<summary>Alternative methods for advanced users (click to see)</summary>
 	
 ### Using pip with custom configuration
 
 You can also use `pip` to install the GitHub version:
 
 ```
 pip install -U -e git+https://github.com/toruseo/uxsim@main#egg=uxsim
@@ -110,39 +111,29 @@
 ```
 pip install -U -e git+https://github.com/YOUR_FORK/uxsim@YOUR_BRANCH#egg=uxsim
 ```
 
 	
 ### Manual install
 
-Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it to your local directory as follows:
+Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it in your local directory as follows:
 ```
 your_project_directory/
 ├── uxsim/ 	# The uxsim directory
 │ ├── uxsim.py 	# The main code of UXsim. You can customize this as you wish
 │ └── ... 	# Other files and directories in uxsim
-├── your_simulation_code.py 		# Your code if nessesary
-├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if nessesary
-├── ... 	# Other files if nessesary
+├── your_simulation_code.py 		# Your code if necessary
+├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if necessary
+├── ... 	# Other files if necessary
 ```
-In this way, you can flexibly customize UXsim by your own.
+This way, you can flexibly customize UXsim on your own.
 
 </details>
 
-## Usage
-
-Import the module using:
-```python
-from uxsim import *
-```
-and then define your simulation scenario.
-
-The [Jupyter Notebook Demo](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) summarizes the basic usage and features.
-You can also test [Google Colab demo](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb).
-For the further details, please see [demos_and_examples](https://github.com/toruseo/UXsim/tree/main/demos_and_examples) and [UXsim technical documentation](https://toruseo.jp/UXsim/docs/index.html).
+## Getting Started
 
 As a simple example, the following code will simulate traffic flow in a Y-shaped network. 
 ```python
 from uxsim import *
 
 # Define the main simulation
 # Units are standardized to seconds (s) and meters (m)
@@ -173,15 +164,15 @@
 
 # Visualize snapshots of network traffic state for several timesteps
 W.analyzer.network(100, detailed=1, network_font_size=12)
 W.analyzer.network(600, detailed=1, network_font_size=12)
 W.analyzer.network(800, detailed=1, network_font_size=12)
 ```
 
-It would output text to the terminal and images to `out` directory like below:
+It will output text to the terminal and images to the `out` directory like below:
 ```
 simulation setting:
  scenario name:
  simulation duration:    1200 s
  number of vehicles:     810 veh
  total road length:      3000 m
  time discret. width:    5 s
@@ -206,65 +197,54 @@
 ```
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_100.png" width="250"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_600.png" width="250"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_800.png" width="250"/>
 </p>
 
-## Main Files
-
-- `uxsim` directory: UXsim main package
-	- `uxsim/uxsim.py`: UXsim main code
-	- `uxsim/analyzer.py`: Simulation result analysis code
-	- `uxsim/utils.py`: UXsim utilities code
-	- `uxsim/ResultGUIViewer/ResultGUIViewer.py`: Submodule on GUI for visualizing simulation results
-	- `uxsim/OSMImporter/OSMImporter.py`: Submodule on road network import from OpenStreetMap (experimental)
- 	- `uxsim/files` directory: UXsim utilities files
-- `demos_and_examples` directory: Tutorials and examples of UXsim
-- `dat` directory: Sample scenario files
-- `tests`, `.github` directories: Development-related files
-
 ## Further Reading
 
-If you want to know the details of UXsim, please see
+To learn more about UXsim, please see:
 
 - [Simple demo in Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations
-- [UXsim Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 - [Demos and examples](https://github.com/toruseo/UXsim/tree/main/demos_and_examples): Various examples using Jupyter Notebooks and Python codes
+- [UXsim Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 - [arXiv preprint](https://arxiv.org/abs/2309.17114): Scientific overview
 
+## Main Files
+
+- `uxsim` directory: UXsim main package
+	- `uxsim/uxsim.py`: UXsim main code
+- `demos_and_examples` directory: Tutorials and examples of UXsim
+- `dat` directory: Sample scenario files
+
 ## Terms of Use & License
 
 UXsim is released under the MIT License. You are free to use it as long as the source is acknowledged.
 
-When publishing works based on from UXsim, please cite:
+When publishing works based on UXsim, please cite:
 
 - Toru Seo. Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation. Corona Publishing Co., Ltd., 2023.
 - Toru Seo. UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview. arXiv preprint arXiv: 2309.17114, 2023
 
 ## Contributing and Discussion
 
-Contribution is welcome!
-For minor changes including bug fixes, please submit a pull request.
-Please make sure that your codes pass the automatic tests in Github Action.
-If you want a major change, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page first.
+Contributions are welcome!
+Please see the [Contributing Guideline](https://github.com/toruseo/UXsim/blob/main/.github/CONTRIBUTING.md).
 
-If you have any questions or suggestions, please start a discussion at [Discussions](https://github.com/toruseo/UXsim/discussions) page (in English or Japanese).
+If you have any questions or suggestions, please post them to the [Issues](https://github.com/toruseo/UXsim/issues) or [Discussions](https://github.com/toruseo/UXsim/discussions) (in English or Japanese).
 
 I (Toru Seo) work on this project in my spare time. Please understand that my response may be delayed.
 
 ## Acknowledgments
 
-UXsim is based on various works in traffic flow theory and related fields. We would like to acknowledge the contributions of the research community in advancing this field.
-Especially, UXsim directly uses the following works:
+UXsim is based on various works in traffic flow theory and related fields. We acknowledge the contributions of the research community in advancing this field.
+Specifically, UXsim directly uses the following works:
 
-- [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extention [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
+- [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extension [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
 - [Incremental Node Model](https://doi.org/10.1016/j.trb.2011.04.001) and its [mesoscopic version](https://ubiquitypress.com/site/chapters/e/10.5334/baw.50/)
 - [Dynamic User Optimum](https://doi.org/10.1016/S0191-2615(00)00005-9)-type Route Choice Model
 
 ## Related Links
 
 - [Toru Seo (Author)](https://toruseo.jp/index_en.html)
-- [Collection of related simulators by Seo](https://toruseo.jp/uxsim/index_en.html)
-- Japanese book "[Macroscopic Traffic Simulation: Fundamental Mathematical Theory and Python Implementation](https://www.coronasha.co.jp/np/isbn/9784339052794/)" (Author: [Toru Seo](https://toruseo.jp/), Publisher: [Corona Publishing Co., Ltd.](https://www.coronasha.co.jp/)): UXsim is a significant expansion of the traffic flow simulator *UroborosX* described in this book.
 - [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/en/)
-- [Interactive Traffic Flow Simulator that Runs on a Web Browser](http://seo.cv.ens.titech.ac.jp/traffic-flow-demo/bottleneck.html): Play with the same link traffic flow model used in this simulator interactively, and learn the basics of traffic flow and its simulation.
```

### Comparing `uxsim-1.1.0/README.md` & `uxsim-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,75 +6,76 @@
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
 [![Static Badge](https://img.shields.io/badge/readme-%E6%97%A5%E6%9C%AC%E8%AA%9E%20%F0%9F%87%AF%F0%9F%87%B5%20-pink)](https://github.com/toruseo/UXsim/blob/main/README.jp.md)
 
 *UXsim* is a free, open-source macroscopic and mesoscopic network traffic flow simulator written in Python.
 It simulates the movements of car travelers and traffic congestion in road networks.
-It is suitable for simulating large-scale (e.g. city-scale) traffic phenomena.
-UXsim would be especially useful for scientific and educational purposes because of its simple, lightweight, and customizable features, but of course users are free to use UXsim for any purpose.
+It is suitable for simulating large-scale (e.g., city-scale) traffic phenomena.
+UXsim is especially useful for scientific and educational purposes because of its simple, lightweight, and customizable features, but users are free to use UXsim for any purpose.
 
-If you are interested in, please see
+If you are interested, please see:
 
 - [Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations and tutorials
 - [Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 
 ## Main Features
 
-- Simple, lightweight, and easy-to-use Python implementation of the modern standard models of dynamic network traffic flow.
-- Macroscopic traffic simulation: Simulating over 60000 vehicles in 30 seconds in a city.
-- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand.
-- Implementation of traffic control/management schemes such as traffic signals and road pricing.
-- Basic analysis of simulation results and their export to pandas.DataFrame and CSV files.
-- Visualization of simulation results using matplotlib. Interactive GUI is available.
-- Flexible and customizable thanks to pure Python implementation. Can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control.
+- Simple, lightweight, and easy-to-use Python implementation of modern standard models of dynamic network traffic flow
+- Macroscopic traffic simulation: Simulating over 60000 vehicles in a city in 30 seconds
+- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand
+- Theoretically valid models commonly used in academic/professional transportation research
+- Implementation of traffic control/management schemes such as traffic signals and road pricing
+- Basic analysis of simulation results and their export to pandas.DataFrame and CSV files
+- Visualization of simulation results using matplotlib; interactive GUI is available
+- Flexible and customizable thanks to pure Python implementation; can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
-Belows are simulation result where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
+Below are simulation results where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
 
 Visualization of link traffic states (thicker lines mean more vehicles, darker colors mean slower speeds) and some vehicle trajectories:
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/gridnetwork_macro.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/gridnetwork_fancy.gif" width="400"/>
 </p>
 
 Vehicle trajectory diagram on a corridor of the above network:
 <img src="https://github.com/toruseo/UXsim/blob/images/tsd_traj_links_grid.png" width="600">
 
 ### Deep reinforcement learning signal control using PyTorch
 
-Traffic signal controller is trained by deep reinforcement learning (DRL) of [PyTorch](https://pytorch.org/).
-The left (or upper) is no control scenario with fixed signal timing; the traffic demand exceeds the network capacity with naive signal setting, and a gridlock occurs.
-The right (or bottom) is with DRL control scenario, where traffic signal can be changed by observing queue length; although the demand level is the same, traffic is smoothly flowing.
-[Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
+A traffic signal controller is trained by deep reinforcement learning (DRL) using [PyTorch](https://pytorch.org/).
+The left (or upper) scenario shows no control with fixed signal timing; the traffic demand exceeds the network capacity with the naive signal setting, and a gridlock occurs.
+The right (or bottom) scenario shows DRL control, where the traffic signal can be changed by observing queue length; although the demand level is the same, traffic flows smoothly.
+A [Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
 
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_nocontrol.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_DQL.gif" width="400"/>
 </p>
 
 ### Interactive GUI for exploring a simulation result
 
 https://github.com/toruseo/UXsim/assets/34780089/ec780a33-d9ba-4068-a005-0b06127196d9
 
 ## Install
 
 ### Using pip
 
-The simplest way is using pip to install from PyPI.
+The simplest way is to use pip to install from PyPI:
 
 ```
 pip install uxsim
 ```
 
 <details>
-<summary>Alternative methods (click to see)</summary>
+<summary>Alternative methods for advanced users (click to see)</summary>
 	
 ### Using pip with custom configuration
 
 You can also use `pip` to install the GitHub version:
 
 ```
 pip install -U -e git+https://github.com/toruseo/uxsim@main#egg=uxsim
@@ -85,39 +86,29 @@
 ```
 pip install -U -e git+https://github.com/YOUR_FORK/uxsim@YOUR_BRANCH#egg=uxsim
 ```
 
 	
 ### Manual install
 
-Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it to your local directory as follows:
+Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it in your local directory as follows:
 ```
 your_project_directory/
 ├── uxsim/ 	# The uxsim directory
 │ ├── uxsim.py 	# The main code of UXsim. You can customize this as you wish
 │ └── ... 	# Other files and directories in uxsim
-├── your_simulation_code.py 		# Your code if nessesary
-├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if nessesary
-├── ... 	# Other files if nessesary
+├── your_simulation_code.py 		# Your code if necessary
+├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if necessary
+├── ... 	# Other files if necessary
 ```
-In this way, you can flexibly customize UXsim by your own.
+This way, you can flexibly customize UXsim on your own.
 
 </details>
 
-## Usage
-
-Import the module using:
-```python
-from uxsim import *
-```
-and then define your simulation scenario.
-
-The [Jupyter Notebook Demo](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) summarizes the basic usage and features.
-You can also test [Google Colab demo](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb).
-For the further details, please see [demos_and_examples](https://github.com/toruseo/UXsim/tree/main/demos_and_examples) and [UXsim technical documentation](https://toruseo.jp/UXsim/docs/index.html).
+## Getting Started
 
 As a simple example, the following code will simulate traffic flow in a Y-shaped network. 
 ```python
 from uxsim import *
 
 # Define the main simulation
 # Units are standardized to seconds (s) and meters (m)
@@ -148,15 +139,15 @@
 
 # Visualize snapshots of network traffic state for several timesteps
 W.analyzer.network(100, detailed=1, network_font_size=12)
 W.analyzer.network(600, detailed=1, network_font_size=12)
 W.analyzer.network(800, detailed=1, network_font_size=12)
 ```
 
-It would output text to the terminal and images to `out` directory like below:
+It will output text to the terminal and images to the `out` directory like below:
 ```
 simulation setting:
  scenario name:
  simulation duration:    1200 s
  number of vehicles:     810 veh
  total road length:      3000 m
  time discret. width:    5 s
@@ -181,65 +172,54 @@
 ```
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_100.png" width="250"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_600.png" width="250"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_800.png" width="250"/>
 </p>
 
-## Main Files
-
-- `uxsim` directory: UXsim main package
-	- `uxsim/uxsim.py`: UXsim main code
-	- `uxsim/analyzer.py`: Simulation result analysis code
-	- `uxsim/utils.py`: UXsim utilities code
-	- `uxsim/ResultGUIViewer/ResultGUIViewer.py`: Submodule on GUI for visualizing simulation results
-	- `uxsim/OSMImporter/OSMImporter.py`: Submodule on road network import from OpenStreetMap (experimental)
- 	- `uxsim/files` directory: UXsim utilities files
-- `demos_and_examples` directory: Tutorials and examples of UXsim
-- `dat` directory: Sample scenario files
-- `tests`, `.github` directories: Development-related files
-
 ## Further Reading
 
-If you want to know the details of UXsim, please see
+To learn more about UXsim, please see:
 
 - [Simple demo in Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations
-- [UXsim Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 - [Demos and examples](https://github.com/toruseo/UXsim/tree/main/demos_and_examples): Various examples using Jupyter Notebooks and Python codes
+- [UXsim Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 - [arXiv preprint](https://arxiv.org/abs/2309.17114): Scientific overview
 
+## Main Files
+
+- `uxsim` directory: UXsim main package
+	- `uxsim/uxsim.py`: UXsim main code
+- `demos_and_examples` directory: Tutorials and examples of UXsim
+- `dat` directory: Sample scenario files
+
 ## Terms of Use & License
 
 UXsim is released under the MIT License. You are free to use it as long as the source is acknowledged.
 
-When publishing works based on from UXsim, please cite:
+When publishing works based on UXsim, please cite:
 
 - Toru Seo. Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation. Corona Publishing Co., Ltd., 2023.
 - Toru Seo. UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview. arXiv preprint arXiv: 2309.17114, 2023
 
 ## Contributing and Discussion
 
-Contribution is welcome!
-For minor changes including bug fixes, please submit a pull request.
-Please make sure that your codes pass the automatic tests in Github Action.
-If you want a major change, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page first.
+Contributions are welcome!
+Please see the [Contributing Guideline](https://github.com/toruseo/UXsim/blob/main/.github/CONTRIBUTING.md).
 
-If you have any questions or suggestions, please start a discussion at [Discussions](https://github.com/toruseo/UXsim/discussions) page (in English or Japanese).
+If you have any questions or suggestions, please post them to the [Issues](https://github.com/toruseo/UXsim/issues) or [Discussions](https://github.com/toruseo/UXsim/discussions) (in English or Japanese).
 
 I (Toru Seo) work on this project in my spare time. Please understand that my response may be delayed.
 
 ## Acknowledgments
 
-UXsim is based on various works in traffic flow theory and related fields. We would like to acknowledge the contributions of the research community in advancing this field.
-Especially, UXsim directly uses the following works:
+UXsim is based on various works in traffic flow theory and related fields. We acknowledge the contributions of the research community in advancing this field.
+Specifically, UXsim directly uses the following works:
 
-- [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extention [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
+- [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extension [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
 - [Incremental Node Model](https://doi.org/10.1016/j.trb.2011.04.001) and its [mesoscopic version](https://ubiquitypress.com/site/chapters/e/10.5334/baw.50/)
 - [Dynamic User Optimum](https://doi.org/10.1016/S0191-2615(00)00005-9)-type Route Choice Model
 
 ## Related Links
 
 - [Toru Seo (Author)](https://toruseo.jp/index_en.html)
-- [Collection of related simulators by Seo](https://toruseo.jp/uxsim/index_en.html)
-- Japanese book "[Macroscopic Traffic Simulation: Fundamental Mathematical Theory and Python Implementation](https://www.coronasha.co.jp/np/isbn/9784339052794/)" (Author: [Toru Seo](https://toruseo.jp/), Publisher: [Corona Publishing Co., Ltd.](https://www.coronasha.co.jp/)): UXsim is a significant expansion of the traffic flow simulator *UroborosX* described in this book.
-- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/en/)
-- [Interactive Traffic Flow Simulator that Runs on a Web Browser](http://seo.cv.ens.titech.ac.jp/traffic-flow-demo/bottleneck.html): Play with the same link traffic flow model used in this simulator interactively, and learn the basics of traffic flow and its simulation.
+- [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/en/)
```

### Comparing `uxsim-1.1.0/pyproject.toml` & `uxsim-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     "scipy>=1.9.1",
     "pandas>=1.4.4",
     "PyQt5>=5.15.7"
 ]
 dynamic = ["version"] # Version is read from uxsim/__init__.py
 
 [project.urls]
-"Homepage" = "https://github.com/toruseo/UXsim"
-"Download" = "https://github.com/toruseo/UXsim"
-"Bug Tracker" = "https://github.com/toruseo/UXsim/issues"
+Homepage = "https://github.com/toruseo/UXsim"
+Documentation = "https://toruseo.jp/UXsim/docs"
+Issues = "https://github.com/toruseo/UXsim/issues"
 
 [tool.setuptools]
 packages = {find = {include = ["uxsim", "uxsim.*"]}}
 
 [tool.setuptools.dynamic]
 version = {attr = "uxsim.__version__"}
```

### Comparing `uxsim-1.1.0/tests/test_examples.py` & `uxsim-1.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/tests/test_result_gui_viewer.py` & `uxsim-1.1.1/tests/test_result_gui_viewer.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/tests/test_verification_exceptional.py` & `uxsim-1.1.1/tests/test_verification_exceptional.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/tests/test_verification_multilane.py` & `uxsim-1.1.1/tests/test_verification_multilane.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/tests/test_verification_node.py` & `uxsim-1.1.1/tests/test_verification_node.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/tests/test_verification_route_choice.py` & `uxsim-1.1.1/tests/test_verification_route_choice.py`

 * *Files 10% similar despite different names*

```diff
@@ -547,8 +547,122 @@
     assert equal_tolerance(np.average(tt2s), ttave, rel_tol=0.2)
     assert equal_tolerance(np.average(tt3s), ttave, rel_tol=0.2)
     assert equal_tolerance(np.average(tt4s), ttave, rel_tol=0.2)
     assert equal_tolerance(np.average(vol1s), volave, rel_tol=0.2)
     assert equal_tolerance(np.average(vol2s), volave, rel_tol=0.2)
     assert equal_tolerance(np.average(vol3s), volave, rel_tol=0.2)
     assert equal_tolerance(np.average(vol4s), volave, rel_tol=0.2)
-    assert equal_tolerance(volave*4, 2000*0.8)
+    assert equal_tolerance(volave*4, 2000*0.8)
+
+def test_route_links_prefer():     
+    W = World(
+        name="",
+        deltan=5,
+        tmax=2000,
+        print_mode=1, save_mode=1, show_mode=1,
+        random_seed=None
+    )
+
+    W.addNode("orig", 0, 0)
+    W.addNode("mid1",0,0)
+    W.addNode("mid2",0,0)
+    W.addNode("dest", 0, 0)
+    link11 = W.addLink("link11", "orig", "mid1", length=1000, free_flow_speed=20)
+    link12 = W.addLink("link12", "orig", "mid1", length=1000, free_flow_speed=10)
+    link21 = W.addLink("link21", "mid1", "mid2", length=1000, free_flow_speed=20)
+    link22 = W.addLink("link22", "mid1", "mid2", length=1000, free_flow_speed=10)
+    link31 = W.addLink("link31", "mid2", "dest", length=1000, free_flow_speed=20)
+    link32 = W.addLink("link32", "mid2", "dest", length=1000, free_flow_speed=10)
+
+    for t in range(0,1000, 10):
+        W.addVehicle("orig", "dest", links_prefer=[link12, link21, link32], departure_time=t)
+
+    W.exec_simulation()
+
+    W.analyzer.print_simple_stats()
+
+    df = W.analyzer.link_to_pandas()
+
+    assert equal_tolerance(df[df["link"]=="link12"]["traffic_volume"].values[0], 500)
+    assert equal_tolerance(df[df["link"]=="link21"]["traffic_volume"].values[0], 500)
+    assert equal_tolerance(df[df["link"]=="link32"]["traffic_volume"].values[0], 500)
+
+def test_route_links_avoid():
+    W = World(
+        name="",
+        deltan=5,
+        tmax=2000,
+        print_mode=1, save_mode=1, show_mode=1,
+        random_seed=None
+    )
+
+    W.addNode("orig", 0, 0)
+    W.addNode("mid1",0,0)
+    W.addNode("mid2",0,0)
+    W.addNode("dest", 0, 0)
+    link11 = W.addLink("link11", "orig", "mid1", length=1000, free_flow_speed=20)
+    link12 = W.addLink("link12", "orig", "mid1", length=1000, free_flow_speed=10)
+    link21 = W.addLink("link21", "mid1", "mid2", length=1000, free_flow_speed=20)
+    link22 = W.addLink("link22", "mid1", "mid2", length=1000, free_flow_speed=10)
+    link31 = W.addLink("link31", "mid2", "dest", length=1000, free_flow_speed=20)
+    link32 = W.addLink("link32", "mid2", "dest", length=1000, free_flow_speed=10)
+
+    for t in range(0,1000, 10):
+        W.addVehicle("orig", "dest", links_avoid=[link12, link21, link32], departure_time=t)
+
+    W.exec_simulation()
+
+    W.analyzer.print_simple_stats()
+
+    df = W.analyzer.link_to_pandas()
+
+    assert equal_tolerance(df[df["link"]=="link11"]["traffic_volume"].values[0], 500)
+    assert equal_tolerance(df[df["link"]=="link22"]["traffic_volume"].values[0], 500)
+    assert equal_tolerance(df[df["link"]=="link31"]["traffic_volume"].values[0], 500)
+
+@pytest.mark.flaky(reruns=5)
+def test_route_multiple_links_between_same_nodes():    
+    vol11s = []
+    vol12s = []
+    vol21s = []
+    vol22s = []
+
+    for i in range(10):
+
+        W = World(
+            name="",
+            deltan=5,
+            tmax=2000,
+            print_mode=0, save_mode=1, show_mode=1,
+            random_seed=None,
+            duo_update_time=100
+        )
+
+        W.addNode("orig", 0, 0)
+        W.addNode("mid1",0,0)
+        W.addNode("mid2",0,0)
+        W.addNode("dest", 0, 0)
+        link11 = W.addLink("link11", "orig", "mid1", length=1000, free_flow_speed=20)
+        link12 = W.addLink("link12", "orig", "mid1", length=1000, free_flow_speed=10)
+        link21 = W.addLink("link21", "orig", "mid2", length=1000, free_flow_speed=20)
+        link22 = W.addLink("link22", "orig", "mid2", length=1000, free_flow_speed=10)
+        link31 = W.addLink("link31", "mid1", "dest", length=1000, free_flow_speed=20)
+        link32 = W.addLink("link32", "mid2", "dest", length=1000, free_flow_speed=20)
+
+        W.adddemand("orig", "dest", 0, 1000, 0.8)
+
+        W.exec_simulation()
+
+        W.analyzer.print_simple_stats()
+
+        df = W.analyzer.link_to_pandas()
+        #display(df)
+
+        vol11s.append(df[df["link"]=="link11"]["traffic_volume"].values[0])
+        vol12s.append(df[df["link"]=="link12"]["traffic_volume"].values[0])
+        vol21s.append(df[df["link"]=="link21"]["traffic_volume"].values[0])
+        vol22s.append(df[df["link"]=="link22"]["traffic_volume"].values[0])
+
+    print(f"{np.average(vol11s) = }\n{np.average(vol12s) = }\n{np.average(vol21s) = }\n{np.average(vol22s) = }")
+    assert equal_tolerance(np.average(vol11s), np.average(vol12s), rel_tol=0.2)
+    assert equal_tolerance(np.average(vol21s), np.average(vol22s), rel_tol=0.2)
+    assert equal_tolerance(np.average(vol11s)+np.average(vol12s), np.average(vol21s)+np.average(vol22s), rel_tol=0.2)
```

### Comparing `uxsim-1.1.0/tests/test_verification_sioux_falls.py` & `uxsim-1.1.1/tests/test_verification_sioux_falls.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/tests/test_verification_straight_road.py` & `uxsim-1.1.1/tests/test_verification_straight_road.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/uxsim/OSMImporter/OSMImporter.py` & `uxsim-1.1.1/uxsim/OSMImporter/OSMImporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         
         print("aggregated network size:")
         print(" number of links:", len(links))
         print(" number of nodes:", len(nodes))
 
         return nodes, links
 
-    def osm_network_visualize(nodes, links, figsize=(12,12), xlim=[None,None], ylim=[None,None], show_link_name=False): 
+    def osm_network_visualize(nodes, links, figsize=(12,12), xlim=[None,None], ylim=[None,None], show_link_name=False, show_mode=1, save_mode=0, save_fname="osm_network.png"): 
         """
         Visualize the imported network. Mainly for test purpose.
         """
         node_positions = {node[0]: (node[1], node[2]) for node in nodes}
 
         # グラフを描画
         plt.figure(figsize=figsize)
@@ -309,15 +309,19 @@
             xmid2, ymid2 = (x1+2*x2)/3+vx, (y1+2*y2)/3+vy
             plt.plot([x1, xmid1, xmid2, x2], [y1, ymid1, ymid2, y2], 'b-', linewidth=1)
             if show_link_name:
                 plt.text((x1+x2)/2, (y1+y2)/2, link[0], fontsize=8)
         
         plt.xlim(xlim)
         plt.ylim(ylim)
-        plt.show()
+        if show_mode:
+            plt.show()
+        if save_mode:
+            plt.savefig(save_fname)
+        plt.close()
 
     def osm_network_to_World(W, nodes, links, default_jam_density=0.2, coef_degree_to_meter=111000):
         """
         Load the imported network to the World object of UXsim.
 
         Parameters
         ----------
```

### Comparing `uxsim-1.1.0/uxsim/ResultGUIViewer/ResultGUIViewer.py` & `uxsim-1.1.1/uxsim/ResultGUIViewer/ResultGUIViewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,53 +428,7 @@
 
     app = QApplication(sys.argv)
     window = MainWindow(W, nodes, edges, vehicle_list, tmax)
     window.show()
     if return_app_window:
         return app, window
     sys.exit(app.exec_())
-
-
-if __name__ == "__main__":
-    #this is just a test
-    tmax = 5
-    nodes = [
-        ("A", 100, 100, {"attr1": 1, "attr2": "foo"}),
-        ("B", 300, 200, {"attr1": 2, "attr2": "bar"}),
-        ("C", 200, 400, {"attr1": 3, "attr2": "baz"})
-    ]
-
-    e1data = [
-        [1,0,0,0,0],
-        [0,1,0,0,0],
-        [0,0,1,0,0],
-        [0,0,0,1,0],
-        [0,0,0,0,1],
-    ]
-    e3data = [
-        [1,1,0.5,0,0],
-        [0,1,1,0.5,0],
-        [0,0,1,1,0.5],
-        [0.5,0,0,1,1],
-        [1,0.5,0,0,1],
-    ]
-
-    edges = [
-        ("Edge1", "A", "B", np.array(e1data), {"attr1": 10, "attr2": "edge1"}),
-        ("Edge2", "B", "C", np.array(e1data), {"attr1": 20, "attr2": "edge2"}),
-        ("Edge3", "C", "B", np.array(e3data), {"attr1": 20, "attr2": "edge2"})
-    ]
-
-    vehicle_list = None
-
-    # vehicle_list = [
-    #     (0, "Edge1", 0.1),
-    #     (1, "Edge1", 0.5),
-    #     (2, "Edge2", 0.2),
-    #     (3, "Edge2", 0.8),
-    #     (4, "Edge3", 0.6),
-    # ]
-
-    app = QApplication(sys.argv)
-    window = MainWindow(nodes, edges, vehicle_list, tmax)
-    window.show()
-    sys.exit(app.exec_())
```

### Comparing `uxsim-1.1.0/uxsim/analyzer.py` & `uxsim-1.1.1/uxsim/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 from collections import defaultdict as ddict
 from importlib.resources import read_binary #according to official doc, this is also not recommended
 import io
 from scipy.sparse.csgraph import floyd_warshall
 
 from .utils  import *
 
-plt.rcParams["font.family"] = "monospace"
-if "MS Gothic" in plt.rcParams["font.family"]:
-    plt.rcParams["font.family"] = "MS Gothic"
-
+plt.rcParams["font.family"] = get_font_for_matplotlib()
 
 class Analyzer:
     """
     Class for analyzing and visualizing a simulation result.
     """
 
     def __init__(s, W):
@@ -135,14 +132,17 @@
                 s.linkc_tt_ave[l] = np.average([t for t in l.traveltime_actual if t>0])
                 s.linkc_tt_std[l] = np.std([t for t in l.traveltime_actual if t>0])
 
     def compute_accurate_traj(s):
         """
         Generate more complete vehicle trajectories for each link by extrapolating recorded trajectories. It is assumed that vehicles are in free-flow travel at the end of the link.
         """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The trajecotries are not exactly accurate.", LoggingWarning)
+
         if s.flag_trajectory_computed:
             return 0
         else:
             s.flag_trajectory_computed = 1
 
         for veh in s.W.VEHICLES.values():
             l_old = None
@@ -299,14 +299,16 @@
             The names of the links for which the time-space diagram is to be plotted.
             If None, the diagram is plotted for all links in the network. Default is None.
         figsize : tuple of int, optional
             The size of the figure to be plotted, default is (12,4).
         plot_signal : bool, optional
             Plot the downstream signal red light.
         """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The plot is not exactly accurate.", LoggingWarning)
 
         #リンク車両軌跡の時空間図
         s.W.print(" drawing trajectories...")
         s.compute_accurate_traj()
 
         #対象がlistであればOKで，単一な場合にはlistに変換する．未指定であれば全部にする．
         if links == None:
@@ -358,14 +360,16 @@
             The names of the links for which the time-space diagram is to be plotted.
             If None, the diagram is plotted for all links in the network. Default is None.
         figsize : tuple of int, optional
             The size of the figure to be plotted, default is (12,4).
         plot_signal : bool, optional
             Plot the downstream signal red light.
         """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The plot is not exactly accurate.", LoggingWarning)
 
         #リンク密度の時空間図
         s.W.print(" drawing traffic states...")
         s.compute_edie_state()
 
         #対象がlistであればOKで，単一な場合にはlistに変換する．未指定であれば全部にする．
         if links == None:
@@ -420,14 +424,17 @@
         linkslist : list of link or list of list of link
             The names of the concective links for which the time-space diagram is to be plotted.
         figsize : tuple of int, optional
             The size of the figure to be plotted, default is (12,4).
         plot_signal : bool, optional
             Plot the signal red light.
         """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The plot is not exactly accurate.", LoggingWarning)
+            
         #複数リンクの連続した車両軌跡の時空間図
         s.W.print(" drawing trajectories in consecutive links...")
         s.compute_accurate_traj()
 
         #リンクリストのリストであればそのまま，そうでなければリスト化
         try:
             iter(linkslist[0])
@@ -841,14 +848,16 @@
         -----
         This method generates a visually appealing animation that visualizes vehicles' trajectories across the transportation network over time.
         The animation provides information on vehicle positions, speeds, link names, node locations, and more, with Bezier curves used for smooth transitions.
         The generated animation is saved to the directory `out<W.name>` with a filename `anim_network_fancy.gif`.
 
         Temporary images used to create the animation are removed after the animation is generated.
         """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The animation is not exactly accurate.", LoggingWarning)
 
         s.W.print(" generating animation...")
 
         # ベジエ補間
         from scipy.interpolate import make_interp_spline
 
         #{t: ["xs":[], "ys":[], "v": v, "c":c]}
@@ -1055,14 +1064,17 @@
 
         Notes
         -----
         This method visualizes the speed profile and the links traversed by a specific vehicle over time.
         The speed is plotted on the primary y-axis, and the links are plotted on the secondary y-axis.
         The plot is saved to the directory `out<W.name>` with the filename `vehicle_<vehname>.png`.
         """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The plot is not exactly accurate.", LoggingWarning)
+        
         veh = s.W.VEHICLES[vehname]
 
         fig, ax1 = plt.subplots()
         plt.title(f"vehicle: {veh.name}")
         ax1.fill_between(veh.log_t, 0, veh.log_v, color="c", zorder=10)
         ax1.set_ylabel('speed (m/s)', color='c')
         plt.ylim([0, None])
@@ -1098,14 +1110,17 @@
             - 'dest': the destination node of the vehicle's trip.
             - 't': the timestep.
             - 'link': the link the vehicle is on (or relevant status).
             - 'x': the position of the vehicle on the link.
             - 's': the spacing of the vehicle.
             - 'v': the speed of the vehicle.
         """
+        if s.W.vehicle_logging_timestep_interval != 1:
+            warnings.warn("vehicle_logging_timestep_interval is not 1. The output data is not exactly accurate.", LoggingWarning)
+
         if s.flag_pandas_convert == 0:
             s.flag_pandas_convert = 1
 
             out = [["name", "dn", "orig", "dest", "t", "link", "x", "s", "v"]]
             for veh in s.W.VEHICLES.values():
                 for i in range(len(veh.log_t)):
                     if veh.log_state[i] in ("wait", "run", "end", "abort"):
```

### Comparing `uxsim-1.1.0/uxsim/files/HackGen-Regular.ttf` & `uxsim-1.1.1/uxsim/files/HackGen-Regular.ttf`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/uxsim/files/Inconsolata.otf` & `uxsim-1.1.1/uxsim/files/Inconsolata.otf`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/uxsim/files/LICENSE_of_HackGen-Regular` & `uxsim-1.1.1/uxsim/files/LICENSE_of_HackGen-Regular`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-# Licensing
-
-- Source fonts are licensed under SIL OPEN FONT LICENSE Version 1.1.
-  For more information, see "LICENSE_<FontName>" file contained in the "source" directory.
-- "白源/HackGen" are licensed under SIL OPEN FONT LICENSE Version 1.1.
-- Other source code, such as generating scripts, will use the MIT license.
-
-## "白源/HackGen" licensing
-
-Copyright (c) 2019, Yuko OTAWARA. with Reserved Font Name "白源", "HackGen"
-
-This Font Software is licensed under the SIL Open Font License, Version 1.1.
-This license is copied below, and is also available with a FAQ at:
-https://scripts.sil.org/OFL
-
-
------------------------------------------------------------
-SIL OPEN FONT LICENSE Version 1.1 - 26 February 2007
------------------------------------------------------------
-
-PREAMBLE
-The goals of the Open Font License (OFL) are to stimulate worldwide
-development of collaborative font projects, to support the font creation
-efforts of academic and linguistic communities, and to provide a free and
-open framework in which fonts may be shared and improved in partnership
-with others.
-
-The OFL allows the licensed fonts to be used, studied, modified and
-redistributed freely as long as they are not sold by themselves. The
-fonts, including any derivative works, can be bundled, embedded, 
-redistributed and/or sold with any software provided that any reserved
-names are not used by derivative works. The fonts and derivatives,
-however, cannot be released under any other type of license. The
-requirement for fonts to remain under this license does not apply
-to any document created using the fonts or their derivatives.
-
-DEFINITIONS
-"Font Software" refers to the set of files released by the Copyright
-Holder(s) under this license and clearly marked as such. This may
-include source files, build scripts and documentation.
-
-"Reserved Font Name" refers to any names specified as such after the
-copyright statement(s).
-
-"Original Version" refers to the collection of Font Software components as
-distributed by the Copyright Holder(s).
-
-"Modified Version" refers to any derivative made by adding to, deleting,
-or substituting -- in part or in whole -- any of the components of the
-Original Version, by changing formats or by porting the Font Software to a
-new environment.
-
-"Author" refers to any designer, engineer, programmer, technical
-writer or other person who contributed to the Font Software.
-
-PERMISSION & CONDITIONS
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of the Font Software, to use, study, copy, merge, embed, modify,
-redistribute, and sell modified and unmodified copies of the Font
-Software, subject to the following conditions:
-
-1) Neither the Font Software nor any of its individual components,
-in Original or Modified Versions, may be sold by itself.
-
-2) Original or Modified Versions of the Font Software may be bundled,
-redistributed and/or sold with any software, provided that each copy
-contains the above copyright notice and this license. These can be
-included either as stand-alone text files, human-readable headers or
-in the appropriate machine-readable metadata fields within text or
-binary files as long as those fields can be easily viewed by the user.
-
-3) No Modified Version of the Font Software may use the Reserved Font
-Name(s) unless explicit written permission is granted by the corresponding
-Copyright Holder. This restriction only applies to the primary font name as
-presented to the users.
-
-4) The name(s) of the Copyright Holder(s) or the Author(s) of the Font
-Software shall not be used to promote, endorse or advertise any
-Modified Version, except to acknowledge the contribution(s) of the
-Copyright Holder(s) and the Author(s) or with their explicit written
-permission.
-
-5) The Font Software, modified or unmodified, in part or in whole,
-must be distributed entirely under this license, and must not be
-distributed under any other license. The requirement for fonts to
-remain under this license does not apply to any document created
-using the Font Software.
-
-TERMINATION
-This license becomes null and void if any of the above conditions are
-not met.
-
-DISCLAIMER
-THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT
-OF COPYRIGHT, PATENT, TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL THE
-COPYRIGHT HOLDER BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
-INCLUDING ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL
-DAMAGES, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM
-OTHER DEALINGS IN THE FONT SOFTWARE.
-
-## Other source licensing (MIT)
-
-Copyright (c) 2019 Yuko OTAWARA
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
+# Licensing
+
+- Source fonts are licensed under SIL OPEN FONT LICENSE Version 1.1.
+  For more information, see "LICENSE_<FontName>" file contained in the "source" directory.
+- "白源/HackGen" are licensed under SIL OPEN FONT LICENSE Version 1.1.
+- Other source code, such as generating scripts, will use the MIT license.
+
+## "白源/HackGen" licensing
+
+Copyright (c) 2019, Yuko OTAWARA. with Reserved Font Name "白源", "HackGen"
+
+This Font Software is licensed under the SIL Open Font License, Version 1.1.
+This license is copied below, and is also available with a FAQ at:
+https://scripts.sil.org/OFL
+
+
+-----------------------------------------------------------
+SIL OPEN FONT LICENSE Version 1.1 - 26 February 2007
+-----------------------------------------------------------
+
+PREAMBLE
+The goals of the Open Font License (OFL) are to stimulate worldwide
+development of collaborative font projects, to support the font creation
+efforts of academic and linguistic communities, and to provide a free and
+open framework in which fonts may be shared and improved in partnership
+with others.
+
+The OFL allows the licensed fonts to be used, studied, modified and
+redistributed freely as long as they are not sold by themselves. The
+fonts, including any derivative works, can be bundled, embedded, 
+redistributed and/or sold with any software provided that any reserved
+names are not used by derivative works. The fonts and derivatives,
+however, cannot be released under any other type of license. The
+requirement for fonts to remain under this license does not apply
+to any document created using the fonts or their derivatives.
+
+DEFINITIONS
+"Font Software" refers to the set of files released by the Copyright
+Holder(s) under this license and clearly marked as such. This may
+include source files, build scripts and documentation.
+
+"Reserved Font Name" refers to any names specified as such after the
+copyright statement(s).
+
+"Original Version" refers to the collection of Font Software components as
+distributed by the Copyright Holder(s).
+
+"Modified Version" refers to any derivative made by adding to, deleting,
+or substituting -- in part or in whole -- any of the components of the
+Original Version, by changing formats or by porting the Font Software to a
+new environment.
+
+"Author" refers to any designer, engineer, programmer, technical
+writer or other person who contributed to the Font Software.
+
+PERMISSION & CONDITIONS
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of the Font Software, to use, study, copy, merge, embed, modify,
+redistribute, and sell modified and unmodified copies of the Font
+Software, subject to the following conditions:
+
+1) Neither the Font Software nor any of its individual components,
+in Original or Modified Versions, may be sold by itself.
+
+2) Original or Modified Versions of the Font Software may be bundled,
+redistributed and/or sold with any software, provided that each copy
+contains the above copyright notice and this license. These can be
+included either as stand-alone text files, human-readable headers or
+in the appropriate machine-readable metadata fields within text or
+binary files as long as those fields can be easily viewed by the user.
+
+3) No Modified Version of the Font Software may use the Reserved Font
+Name(s) unless explicit written permission is granted by the corresponding
+Copyright Holder. This restriction only applies to the primary font name as
+presented to the users.
+
+4) The name(s) of the Copyright Holder(s) or the Author(s) of the Font
+Software shall not be used to promote, endorse or advertise any
+Modified Version, except to acknowledge the contribution(s) of the
+Copyright Holder(s) and the Author(s) or with their explicit written
+permission.
+
+5) The Font Software, modified or unmodified, in part or in whole,
+must be distributed entirely under this license, and must not be
+distributed under any other license. The requirement for fonts to
+remain under this license does not apply to any document created
+using the Font Software.
+
+TERMINATION
+This license becomes null and void if any of the above conditions are
+not met.
+
+DISCLAIMER
+THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT
+OF COPYRIGHT, PATENT, TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL THE
+COPYRIGHT HOLDER BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
+INCLUDING ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL
+DAMAGES, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM
+OTHER DEALINGS IN THE FONT SOFTWARE.
+
+## Other source licensing (MIT)
+
+Copyright (c) 2019 Yuko OTAWARA
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
```

### Comparing `uxsim-1.1.0/uxsim/files/Licence_of_Inconsolata.otf.txt` & `uxsim-1.1.1/uxsim/files/Licence_of_Inconsolata.otf.txt`

 * *Files identical despite different names*

### Comparing `uxsim-1.1.0/uxsim/uxsim.py` & `uxsim-1.1.1/uxsim/uxsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,19 +145,26 @@
         Departs vehicles from the waiting queue.
 
         Notes
         -----
         If there are vehicles in the generation queue of the node, this method attempts to depart a vehicle to one of the outgoing links.
         The choice of the outgoing link is based on the vehicle's route preference for each link. Once a vehicle is departed, it is removed from the generation queue, added to the list of vehicles on the chosen link, and its state is set to "run".
         """
-        outlinks = list(s.outlinks.values())
-        if len(outlinks):
-            for i in range(sum([l.lanes for l in outlinks])):
-                if len(s.generation_queue) > 0:
+        outlinks0 = list(s.outlinks.values())
+        if len(outlinks0):
+            for i in range(sum([l.lanes for l in outlinks0])):
+                if len(s.generation_queue) > 0:                    
                     veh = s.generation_queue[0]
+
+                    #consider the link preferences
+                    outlinks = list(s.outlinks.values())
+                    if set(outlinks) & set(veh.links_prefer): 
+                        outlinks = list(set(outlinks) & set(veh.links_prefer))
+                    if set(outlinks) & set(veh.links_avoid):
+                        outlinks = list(set(outlinks) - set(veh.links_avoid))
                     
                     preference = [veh.route_pref[l] for l in outlinks]
                     if sum(preference) > 0:
                         outlink = random.choices(outlinks, preference)[0]
                     else:
                         outlink = random.choices(outlinks)[0]
 
@@ -367,14 +374,18 @@
         Notes
         -----
         Traffic Flow Model:
         - The link model follows a multi-lane, single-pipe approach where FIFO is guaranteed per link and no lane changing occurs.
         - Fundamental diagram parameters such as free_flow_speed, jam_density (or jam_density_per_lane), and number_of_lanes determine the link's flow characteristics. Reaction time of drivers `REACTION_TIME` is a grobal parameter.
         - Real-time link status for external reference is maintained with attributes `speed`, `density`, `flow`, `num_vehicles`, and `num_vehicles_queue`.
 
+        Traffic Flow Model Parameters:
+        - Their definition is illustrated as https://toruseo.jp/UXsim/docs/_images/fundamental_diagram.png
+        - If you are not familiar to the traffic flow theory, it is recommended that you adjust only `free_flow_speed` and `number_of_lanes` for the traffic flow model parameters, leaving the other parameters at their default values.
+
         Capacity and Bottlenecks:
         - The `capacity_out` and `capacity_in` parameters set the outflow and inflow capacities of the link. If not provided, the capacities are unlimited.
         - These capacities can represent bottlenecks at the beginning or end of the link.
 
         Connection to Node Model:
         - At the downstream end of a sending link, vehicles in all lanes have the right to be sent out, but FIFO order is maintained.
         - At the upstream end of a receiving link, all lanes can accept vehicles.
@@ -917,15 +928,15 @@
         s.W.VEHICLES_LIVING.pop(s.name)
 
         if s.flag_trip_aborted:
             s.state = "abort"
             s.arrival_time = -1
             s.travel_time = -1
 
-        s.record_log()
+        s.record_log(enforce_log=1)
 
     def carfollow(s):
         """
         Drive withing a link.
         """
         s.x_next = s.x + s.link.u*s.W.DELTAT
         if s.leader != None:
@@ -950,15 +961,15 @@
             Should be in the range [0, 1], where 0 means the old preferences are fully retained and 1 means the preferences are completely updated.
 
         Notes
         -----
         This method updates the link preferences used by the vehicle to select its route based on its current understanding of the system.
 
         - If the vehicle's route choice principle is "homogeneous_DUO", it will update its preferences based on a global, homogenous dynamic user optimization (DUO) model.
-        - If the route choice principle is "heterogeneous_DUO", it will update its preferences based on a heterogeneous DUO model, considering both its past preferences and the system's current state.
+        - If the route choice principle is "heterogeneous_DUO", it will update its preferences based on a heterogeneous DUO model, considering both its past preferences and the system's current state. This is imcomplete feature. Not recommended.
 
         The updated preferences guide the vehicle's decisions in subsequent route choices.
         """
         if s.route_choice_principle == "homogeneous_DUO":
             s.route_pref = s.W.ROUTECHOICE.route_pref[s.dest.id]
         elif s.route_choice_principle == "heterogeneous_DUO":
             route_pref_new = {l:0 for l in s.W.LINKS}
@@ -1011,48 +1022,55 @@
             if link_old != link:
                 route.append(link)
                 ts.append(s.log_t[i])
                 link_old = link
 
         return Route(s.W, route[:-1]), ts
 
-    def record_log(s):
+    def record_log(s, enforce_log=0):
         """
         Record travel logs.
+
+        Parameters
+        ----------
+        enforce_log : bool, optional
+            Record log regardless of the logging interval, default is 0.
         """
-        if s.state != "run":
-            if s.state == "end" and s.log_t_link[-1][1] != "end":
-                s.log_t_link.append([s.W.T*s.W.DELTAT, "end"])
-
-            s.log_t.append(s.W.T*s.W.DELTAT)
-            s.log_state.append(s.state)
-            s.log_link.append(-1)
-            s.log_x.append(-1)
-            s.log_s.append(-1)
-            s.log_v.append(-1)
-
-            if s.state == "wait":
-                s.W.analyzer.average_speed_count += 1
-                s.W.analyzer.average_speed += 0
-        else:
-            if len(s.log_link) == 0 or s.log_link[-1] != s.link:
-                s.log_t_link.append([s.W.T*s.W.DELTAT, s.link])
+        if s.W.vehicle_logging_timestep_interval != -1:
+            if (s.W.T%s.W.vehicle_logging_timestep_interval == 0 or enforce_log):
+                if s.state != "run":
+                    if s.state == "end" and s.log_t_link[-1][1] != "end":
+                        s.log_t_link.append([s.W.T*s.W.DELTAT, "end"])
+
+                    s.log_t.append(s.W.T*s.W.DELTAT)
+                    s.log_state.append(s.state)
+                    s.log_link.append(-1)
+                    s.log_x.append(-1)
+                    s.log_s.append(-1)
+                    s.log_v.append(-1)
+
+                    if s.state == "wait":
+                        s.W.analyzer.average_speed_count += 1
+                        s.W.analyzer.average_speed += 0
+                else:
+                    if len(s.log_link) == 0 or s.log_link[-1] != s.link:
+                        s.log_t_link.append([s.W.T*s.W.DELTAT, s.link])
 
-            s.log_t.append(s.W.T*s.W.DELTAT)
-            s.log_state.append(s.state)
-            s.log_link.append(s.link)
-            s.log_x.append(s.x)
-            s.log_v.append(s.v)
-            if s.leader != None and s.link == s.leader.link:
-                s.log_s.append(s.leader.x-s.x)
-            else:
-                s.log_s.append(-1)
+                    s.log_t.append(s.W.T*s.W.DELTAT)
+                    s.log_state.append(s.state)
+                    s.log_link.append(s.link)
+                    s.log_x.append(s.x)
+                    s.log_v.append(s.v)
+                    if s.leader != None and s.link == s.leader.link:
+                        s.log_s.append(s.leader.x-s.x)
+                    else:
+                        s.log_s.append(-1)
 
-            s.W.analyzer.average_speed_count += 1
-            s.W.analyzer.average_speed += (s.v - s.W.analyzer.average_speed)/s.W.analyzer.average_speed_count
+                    s.W.analyzer.average_speed_count += 1
+                    s.W.analyzer.average_speed += (s.v - s.W.analyzer.average_speed)/s.W.analyzer.average_speed_count
 
 
 class RouteChoice:
     """
     Class for computing shortest path for all vehicles.
     """
 
@@ -1085,20 +1103,27 @@
         Parameters
         ----------
         infty : float
             value representing infinity.
         noise : float
             very small noise to slightly randomize route choice. useful to eliminate strange results at an initial stage of simulation where many routes has identical travel time.
         """
+        s.adj_mat_time = np.zeros([len(s.W.NODES), len(s.W.NODES)])
+        adj_mat_link_count = np.zeros([len(s.W.NODES), len(s.W.NODES)])
+
         for link in s.W.LINKS:
             i = link.start_node.id
             j = link.end_node.id
             if s.W.ADJ_MAT[i,j]:
-                s.adj_mat_time[i,j] = link.traveltime_instant[-1]*random.uniform(1, 1+noise) + link.route_choice_penalty
-                if link.capacity_in == 0: #流入禁止の場合は通行不可
+                new_link_tt = link.traveltime_instant[-1]*random.uniform(1, 1+noise) + link.route_choice_penalty
+                n = adj_mat_link_count[i,j]
+                s.adj_mat_time[i,j] = s.adj_mat_time[i,j]*n/(n+1) + new_link_tt/(n+1) # if there are multiple links between the same nodes, average the travel time
+                # s.adj_mat_time[i,j] = new_link_tt #if there is only one link between the nodes, this line is fine, but for generality we use the above line
+                adj_mat_link_count[i,j] += 1
+                if link.capacity_in == 0: #if the inflow is profibited, travel time is assumed to be infinite
                     s.adj_mat_time[i,j] = np.inf
             else:
                 s.adj_mat_time[i,j] = np.inf
 
         s.dist, s.pred = floyd_warshall(s.adj_mat_time, return_predecessors=True)
 
         n_vertices = s.pred.shape[0]
@@ -1108,56 +1133,56 @@
                 # iからjへの最短経路を逆にたどる．．． -> todo: 起終点を逆にした最短経路探索にすればよい
                 if i != j:
                     prev = j
                     while s.pred[i, prev] != i and s.pred[i, prev] != -9999:
                         prev = s.pred[i, prev]
                     s.next[i, j] = prev
 
-    def route_search_all_old(s, infty=9999999999999999999, noise=0):
-        """
-        Compute the current shortest path based on instantanious travel time. Old version, slow for large networks.
-
-        Parameters
-        ----------
-        infty : float
-            value representing infinity.
-        noise : float
-            very small noise to slightly randomize route choice. useful to eliminate strange results at an initial stage of simulation where many routes has identical travel time.
-        """
-        for link in s.W.LINKS:
-            i = link.start_node.id
-            j = link.end_node.id
-            if s.W.ADJ_MAT[i,j]:
-                s.adj_mat_time[i,j] = link.traveltime_instant[-1]*random.uniform(1, 1+noise) + link.route_choice_penalty
-                if link.capacity_in == 0: #流入禁止の場合は通行不可
-                    s.adj_mat_time[i,j] = 0
-            else:
-                s.adj_mat_time[i,j] = 0
-
-        dist = np.zeros([len(s.W.NODES), len(s.W.NODES)])
-        next = np.zeros([len(s.W.NODES), len(s.W.NODES)])
-        for i in range(len(s.W.NODES)):
-            for j in range(len(s.W.NODES)):
-                if s.adj_mat_time[i,j] > 0:
-                    dist[i,j] = s.adj_mat_time[i,j]
-                    next[i,j] = j
-                elif i == j:
-                    next[i,j] = j
-                else:
-                    dist[i,j] = infty
-                    next[i,j] = -1
-
-        for k in range(len(s.W.NODES)):
-            for i in range(len(s.W.NODES)):
-                for j in range(len(s.W.NODES)):
-                    if dist[i,j] > dist[i,k]+dist[k,j]:
-                        dist[i,j] = dist[i,k]+dist[k,j]
-                        next[i,j] = next[i,k]
-        s.dist = dist
-        s.next = next
+    # def route_search_all_old(s, infty=9999999999999999999, noise=0):
+    #     """
+    #     Compute the current shortest path based on instantanious travel time. Old version, slow for large networks.
+
+    #     Parameters
+    #     ----------
+    #     infty : float
+    #         value representing infinity.
+    #     noise : float
+    #         very small noise to slightly randomize route choice. useful to eliminate strange results at an initial stage of simulation where many routes has identical travel time.
+    #     """
+    #     for link in s.W.LINKS:
+    #         i = link.start_node.id
+    #         j = link.end_node.id
+    #         if s.W.ADJ_MAT[i,j]:
+    #             s.adj_mat_time[i,j] = link.traveltime_instant[-1]*random.uniform(1, 1+noise) + link.route_choice_penalty
+    #             if link.capacity_in == 0: #流入禁止の場合は通行不可
+    #                 s.adj_mat_time[i,j] = 0
+    #         else:
+    #             s.adj_mat_time[i,j] = 0
+
+    #     dist = np.zeros([len(s.W.NODES), len(s.W.NODES)])
+    #     next = np.zeros([len(s.W.NODES), len(s.W.NODES)])
+    #     for i in range(len(s.W.NODES)):
+    #         for j in range(len(s.W.NODES)):
+    #             if s.adj_mat_time[i,j] > 0:
+    #                 dist[i,j] = s.adj_mat_time[i,j]
+    #                 next[i,j] = j
+    #             elif i == j:
+    #                 next[i,j] = j
+    #             else:
+    #                 dist[i,j] = infty
+    #                 next[i,j] = -1
+
+    #     for k in range(len(s.W.NODES)):
+    #         for i in range(len(s.W.NODES)):
+    #             for j in range(len(s.W.NODES)):
+    #                 if dist[i,j] > dist[i,k]+dist[k,j]:
+    #                     dist[i,j] = dist[i,k]+dist[k,j]
+    #                     next[i,j] = next[i,k]
+    #     s.dist = dist
+    #     s.next = next
 
     def homogeneous_DUO_update(s):
         """
         Update link preference of all homogeneous travelers based on DUO principle.
         """
         for dest in s.W.NODES:
             k = dest.id
@@ -1175,15 +1200,15 @@
 
 
 class World:
     """
     World (i.e., simulation environment). A World object is consistently referred to as `W` in this code.
     """
 
-    def __init__(W, name="", deltan=5, reaction_time=1, duo_update_time=600, duo_update_weight=0.5, duo_noise=0.01, eular_dt=120, eular_dx=100, random_seed=None, print_mode=1, save_mode=1, show_mode=0, route_choice_principle="homogeneous_DUO", show_progress=1, show_progress_deltat=600, tmax=None):
+    def __init__(W, name="", deltan=5, reaction_time=1, duo_update_time=600, duo_update_weight=0.5, duo_noise=0.01, eular_dt=120, eular_dx=100, random_seed=None, print_mode=1, save_mode=1, show_mode=0, route_choice_principle="homogeneous_DUO", show_progress=1, show_progress_deltat=600, tmax=None, vehicle_logging_timestep_interval=1):
         """
         Create a World.
 
         Parameters
         ----------
         name : str, optional
             The name of the world, default is an empty string.
@@ -1211,14 +1236,17 @@
             The route choice principle, default is "homogeneous_DUO".
         show_progress : int, optional
             Whether show network progress, default is 1 (enabled).
         show_progress_deltat : float, optional
             The time interval for showing network progress, default is 600 seconds.
         tmax : float or None, optional
             The simulation duration, default is None (automatically determined).
+        vehicle_logging_timestep_interval : int, optional
+            The interval for logging vehicle data, default is 1. Logging is off if set to -1.
+            Setting large intervel (2 or more) or turn off the logging makes the simulation significantly faster in large-scale scenarios without loosing simulation internal accuracy, but outputed vehicle trajecotry and other related data will become inaccurate.
 
         Notes
         -----
         A World object must be defined firstly to initiate simulation.
         """
 
         ## パラメータ設定
@@ -1241,14 +1269,16 @@
         ## データ格納先定義
         W.VEHICLES = OrderedDict()            #home, wait, run, end
         W.VEHICLES_LIVING = OrderedDict()     #home, wait, run
         W.VEHICLES_RUNNING = OrderedDict()    #run
         W.NODES = []
         W.LINKS = []
 
+        W.vehicle_logging_timestep_interval = vehicle_logging_timestep_interval
+
         W.route_choice_principle = route_choice_principle
 
         ## リアルタイム経過表示
         W.show_progress = show_progress
         W.show_progress_deltat_timestep = int(show_progress_deltat/W.DELTAT)
 
         ## システム設定
@@ -1644,15 +1674,15 @@
 
             for name in list(W.VEHICLES_LIVING.keys()):
                 W.VEHICLES_LIVING[name].update()
 
             if W.T % W.DELTAT_ROUTE == 0:
                 W.ROUTECHOICE.route_search_all(noise=W.DUO_NOISE)
                 W.ROUTECHOICE.homogeneous_DUO_update()
-                for veh in W.VEHICLES_LIVING.values():
+                for veh in W.VEHICLES_LIVING.values():  #TODO: this is redundant. To be moved to the previous for-loop.
                     veh.route_pref_update(weight=W.DUO_UPDATE_WEIGHT)
 
             W.TIME = W.T*W.DELTAT
 
             if W.print_mode and W.show_progress and W.T%W.show_progress_deltat_timestep == 0 and W.T > 0:
                 W.analyzer.show_simulation_progress()
 
@@ -1876,17 +1906,15 @@
             return False
 
     @catch_exceptions_and_warn()
     def show_network(W, width=1, left_handed=1, figsize=(6,6), network_font_size=10, node_size=6):
         """
         Visualizes the entire transportation network shape.
         """
-        plt.rcParams["font.family"] = "monospace"
-        if "MS Gothic" in plt.rcParams["font.family"]:
-            plt.rcParams["font.family"] = "MS Gothic"
+        plt.rcParams["font.family"] = get_font_for_matplotlib()
 
         plt.figure(figsize=figsize)
         plt.subplot(111, aspect="equal")
         for n in W.NODES:
             plt.plot(n.x, n.y, "o", c="gray", ms=node_size, zorder=10)
             if network_font_size > 0:
                 plt.text(n.x, n.y, n.name, c="g", horizontalalignment="center", verticalalignment="top", zorder=20, fontsize=network_font_size)
@@ -1910,15 +1938,20 @@
         if buffx == 0:
             buffx = buffy
         if buffy == 0:
             buffy = buffx
         plt.xlim([minx-buffx, maxx+buffx])
         plt.ylim([miny-buffy, maxy+buffy])
         plt.tight_layout()
-        plt.show()
+        if W.save_mode:
+            plt.savefig(f"out{W.name}/network.png")
+        if W.show_mode:
+            plt.show()
+        else:
+            plt.close("all")
 
 
 class Route:
     """
     Class for a route that store concective links.
     """
     def __init__(s, W, links, name="", trust_input=False):
```

### Comparing `uxsim-1.1.0/uxsim.egg-info/PKG-INFO` & `uxsim-1.1.1/uxsim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uxsim
-Version: 1.1.0
+Version: 1.1.1
 Summary: UXsim: traffic flow simulator
 Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
 License: MIT License
 Project-URL: Homepage, https://github.com/toruseo/UXsim
-Project-URL: Download, https://github.com/toruseo/UXsim
-Project-URL: Bug Tracker, https://github.com/toruseo/UXsim/issues
+Project-URL: Documentation, https://toruseo.jp/UXsim/docs
+Project-URL: Issues, https://github.com/toruseo/UXsim/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -31,75 +31,76 @@
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
 [![Static Badge](https://img.shields.io/badge/readme-%E6%97%A5%E6%9C%AC%E8%AA%9E%20%F0%9F%87%AF%F0%9F%87%B5%20-pink)](https://github.com/toruseo/UXsim/blob/main/README.jp.md)
 
 *UXsim* is a free, open-source macroscopic and mesoscopic network traffic flow simulator written in Python.
 It simulates the movements of car travelers and traffic congestion in road networks.
-It is suitable for simulating large-scale (e.g. city-scale) traffic phenomena.
-UXsim would be especially useful for scientific and educational purposes because of its simple, lightweight, and customizable features, but of course users are free to use UXsim for any purpose.
+It is suitable for simulating large-scale (e.g., city-scale) traffic phenomena.
+UXsim is especially useful for scientific and educational purposes because of its simple, lightweight, and customizable features, but users are free to use UXsim for any purpose.
 
-If you are interested in, please see
+If you are interested, please see:
 
 - [Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations and tutorials
 - [Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 
 ## Main Features
 
-- Simple, lightweight, and easy-to-use Python implementation of the modern standard models of dynamic network traffic flow.
-- Macroscopic traffic simulation: Simulating over 60000 vehicles in 30 seconds in a city.
-- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand.
-- Implementation of traffic control/management schemes such as traffic signals and road pricing.
-- Basic analysis of simulation results and their export to pandas.DataFrame and CSV files.
-- Visualization of simulation results using matplotlib. Interactive GUI is available.
-- Flexible and customizable thanks to pure Python implementation. Can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control.
+- Simple, lightweight, and easy-to-use Python implementation of modern standard models of dynamic network traffic flow
+- Macroscopic traffic simulation: Simulating over 60000 vehicles in a city in 30 seconds
+- Dynamic traffic assignment: Traffic flow simulation with a given network and time-dependent OD demand
+- Theoretically valid models commonly used in academic/professional transportation research
+- Implementation of traffic control/management schemes such as traffic signals and road pricing
+- Basic analysis of simulation results and their export to pandas.DataFrame and CSV files
+- Visualization of simulation results using matplotlib; interactive GUI is available
+- Flexible and customizable thanks to pure Python implementation; can also be directly integrated with other Python-based frameworks, such as PyTorch for deep reinforcement learning traffic control
 
 ## Simulation Examples
 
 ### Large-scale scenario
 
-Belows are simulation result where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
+Below are simulation results where approximately 60000 vehicles pass through a 10km x 10km grid network in 2 hours. The computation time was about 30 seconds on a standard desktop PC.
 
 Visualization of link traffic states (thicker lines mean more vehicles, darker colors mean slower speeds) and some vehicle trajectories:
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/gridnetwork_macro.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/gridnetwork_fancy.gif" width="400"/>
 </p>
 
 Vehicle trajectory diagram on a corridor of the above network:
 <img src="https://github.com/toruseo/UXsim/blob/images/tsd_traj_links_grid.png" width="600">
 
 ### Deep reinforcement learning signal control using PyTorch
 
-Traffic signal controller is trained by deep reinforcement learning (DRL) of [PyTorch](https://pytorch.org/).
-The left (or upper) is no control scenario with fixed signal timing; the traffic demand exceeds the network capacity with naive signal setting, and a gridlock occurs.
-The right (or bottom) is with DRL control scenario, where traffic signal can be changed by observing queue length; although the demand level is the same, traffic is smoothly flowing.
-[Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
+A traffic signal controller is trained by deep reinforcement learning (DRL) using [PyTorch](https://pytorch.org/).
+The left (or upper) scenario shows no control with fixed signal timing; the traffic demand exceeds the network capacity with the naive signal setting, and a gridlock occurs.
+The right (or bottom) scenario shows DRL control, where the traffic signal can be changed by observing queue length; although the demand level is the same, traffic flows smoothly.
+A [Jupyter Notebook of this example](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_03en_pytorch.ipynb) is available.
 
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_nocontrol.gif" width="400"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/anim_network1_0.22_DQL.gif" width="400"/>
 </p>
 
 ### Interactive GUI for exploring a simulation result
 
 https://github.com/toruseo/UXsim/assets/34780089/ec780a33-d9ba-4068-a005-0b06127196d9
 
 ## Install
 
 ### Using pip
 
-The simplest way is using pip to install from PyPI.
+The simplest way is to use pip to install from PyPI:
 
 ```
 pip install uxsim
 ```
 
 <details>
-<summary>Alternative methods (click to see)</summary>
+<summary>Alternative methods for advanced users (click to see)</summary>
 	
 ### Using pip with custom configuration
 
 You can also use `pip` to install the GitHub version:
 
 ```
 pip install -U -e git+https://github.com/toruseo/uxsim@main#egg=uxsim
@@ -110,39 +111,29 @@
 ```
 pip install -U -e git+https://github.com/YOUR_FORK/uxsim@YOUR_BRANCH#egg=uxsim
 ```
 
 	
 ### Manual install
 
-Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it to your local directory as follows:
+Download the `uxsim` directory from this Github repo or [the latest release](https://github.com/toruseo/UXsim/releases/latest/download/uxsim.zip) and place it in your local directory as follows:
 ```
 your_project_directory/
 ├── uxsim/ 	# The uxsim directory
 │ ├── uxsim.py 	# The main code of UXsim. You can customize this as you wish
 │ └── ... 	# Other files and directories in uxsim
-├── your_simulation_code.py 		# Your code if nessesary
-├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if nessesary
-├── ... 	# Other files if nessesary
+├── your_simulation_code.py 		# Your code if necessary
+├── your_simulation_notebook.ipynb 	# Your Jupyter notebook if necessary
+├── ... 	# Other files if necessary
 ```
-In this way, you can flexibly customize UXsim by your own.
+This way, you can flexibly customize UXsim on your own.
 
 </details>
 
-## Usage
-
-Import the module using:
-```python
-from uxsim import *
-```
-and then define your simulation scenario.
-
-The [Jupyter Notebook Demo](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) summarizes the basic usage and features.
-You can also test [Google Colab demo](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb).
-For the further details, please see [demos_and_examples](https://github.com/toruseo/UXsim/tree/main/demos_and_examples) and [UXsim technical documentation](https://toruseo.jp/UXsim/docs/index.html).
+## Getting Started
 
 As a simple example, the following code will simulate traffic flow in a Y-shaped network. 
 ```python
 from uxsim import *
 
 # Define the main simulation
 # Units are standardized to seconds (s) and meters (m)
@@ -173,15 +164,15 @@
 
 # Visualize snapshots of network traffic state for several timesteps
 W.analyzer.network(100, detailed=1, network_font_size=12)
 W.analyzer.network(600, detailed=1, network_font_size=12)
 W.analyzer.network(800, detailed=1, network_font_size=12)
 ```
 
-It would output text to the terminal and images to `out` directory like below:
+It will output text to the terminal and images to the `out` directory like below:
 ```
 simulation setting:
  scenario name:
  simulation duration:    1200 s
  number of vehicles:     810 veh
  total road length:      3000 m
  time discret. width:    5 s
@@ -206,65 +197,54 @@
 ```
 <p float="left">
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_100.png" width="250"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_600.png" width="250"/>
 <img src="https://github.com/toruseo/UXsim/blob/images/network1_800.png" width="250"/>
 </p>
 
-## Main Files
-
-- `uxsim` directory: UXsim main package
-	- `uxsim/uxsim.py`: UXsim main code
-	- `uxsim/analyzer.py`: Simulation result analysis code
-	- `uxsim/utils.py`: UXsim utilities code
-	- `uxsim/ResultGUIViewer/ResultGUIViewer.py`: Submodule on GUI for visualizing simulation results
-	- `uxsim/OSMImporter/OSMImporter.py`: Submodule on road network import from OpenStreetMap (experimental)
- 	- `uxsim/files` directory: UXsim utilities files
-- `demos_and_examples` directory: Tutorials and examples of UXsim
-- `dat` directory: Sample scenario files
-- `tests`, `.github` directories: Development-related files
-
 ## Further Reading
 
-If you want to know the details of UXsim, please see
+To learn more about UXsim, please see:
 
 - [Simple demo in Jupyter Notebook](https://github.com/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_01en.ipynb) or [Google Colab](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb): Interactive demonstrations
-- [UXsim Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 - [Demos and examples](https://github.com/toruseo/UXsim/tree/main/demos_and_examples): Various examples using Jupyter Notebooks and Python codes
+- [UXsim Technical Documentation](https://toruseo.jp/UXsim/docs/index.html): Detailed documents on tutorials, simulation mechanism, and specifications of modules/functions
 - [arXiv preprint](https://arxiv.org/abs/2309.17114): Scientific overview
 
+## Main Files
+
+- `uxsim` directory: UXsim main package
+	- `uxsim/uxsim.py`: UXsim main code
+- `demos_and_examples` directory: Tutorials and examples of UXsim
+- `dat` directory: Sample scenario files
+
 ## Terms of Use & License
 
 UXsim is released under the MIT License. You are free to use it as long as the source is acknowledged.
 
-When publishing works based on from UXsim, please cite:
+When publishing works based on UXsim, please cite:
 
 - Toru Seo. Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation. Corona Publishing Co., Ltd., 2023.
 - Toru Seo. UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview. arXiv preprint arXiv: 2309.17114, 2023
 
 ## Contributing and Discussion
 
-Contribution is welcome!
-For minor changes including bug fixes, please submit a pull request.
-Please make sure that your codes pass the automatic tests in Github Action.
-If you want a major change, please start a discussion at [Issues](https://github.com/toruseo/UXsim/issues) page first.
+Contributions are welcome!
+Please see the [Contributing Guideline](https://github.com/toruseo/UXsim/blob/main/.github/CONTRIBUTING.md).
 
-If you have any questions or suggestions, please start a discussion at [Discussions](https://github.com/toruseo/UXsim/discussions) page (in English or Japanese).
+If you have any questions or suggestions, please post them to the [Issues](https://github.com/toruseo/UXsim/issues) or [Discussions](https://github.com/toruseo/UXsim/discussions) (in English or Japanese).
 
 I (Toru Seo) work on this project in my spare time. Please understand that my response may be delayed.
 
 ## Acknowledgments
 
-UXsim is based on various works in traffic flow theory and related fields. We would like to acknowledge the contributions of the research community in advancing this field.
-Especially, UXsim directly uses the following works:
+UXsim is based on various works in traffic flow theory and related fields. We acknowledge the contributions of the research community in advancing this field.
+Specifically, UXsim directly uses the following works:
 
-- [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extention [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
+- [Newell's simplified car-following model](https://doi.org/10.1016/S0191-2615(00)00044-8) and its extension [X-model](https://doi.org/10.1016/j.trb.2013.02.008)
 - [Incremental Node Model](https://doi.org/10.1016/j.trb.2011.04.001) and its [mesoscopic version](https://ubiquitypress.com/site/chapters/e/10.5334/baw.50/)
 - [Dynamic User Optimum](https://doi.org/10.1016/S0191-2615(00)00005-9)-type Route Choice Model
 
 ## Related Links
 
 - [Toru Seo (Author)](https://toruseo.jp/index_en.html)
-- [Collection of related simulators by Seo](https://toruseo.jp/uxsim/index_en.html)
-- Japanese book "[Macroscopic Traffic Simulation: Fundamental Mathematical Theory and Python Implementation](https://www.coronasha.co.jp/np/isbn/9784339052794/)" (Author: [Toru Seo](https://toruseo.jp/), Publisher: [Corona Publishing Co., Ltd.](https://www.coronasha.co.jp/)): UXsim is a significant expansion of the traffic flow simulator *UroborosX* described in this book.
 - [Seo Laboratory, Tokyo Institute of Technology](http://seo.cv.ens.titech.ac.jp/en/)
-- [Interactive Traffic Flow Simulator that Runs on a Web Browser](http://seo.cv.ens.titech.ac.jp/traffic-flow-demo/bottleneck.html): Play with the same link traffic flow model used in this simulator interactively, and learn the basics of traffic flow and its simulation.
```

### Comparing `uxsim-1.1.0/uxsim.egg-info/SOURCES.txt` & `uxsim-1.1.1/uxsim.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 tests/test_examples.py
+tests/test_other_functions.py
 tests/test_result_gui_viewer.py
 tests/test_verification_exceptional.py
 tests/test_verification_multilane.py
 tests/test_verification_node.py
 tests/test_verification_route_choice.py
 tests/test_verification_sioux_falls.py
 tests/test_verification_straight_road.py
```

