# Comparing `tmp/tuduam-2024.8-py3-none-any.whl.zip` & `tmp/tuduam-2024.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 33666 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      262 b- defN 24-Feb-13 07:26 tuduam/__init__.py
--rw-rw-rw-  2.0 fat    12019 b- defN 24-Feb-13 07:26 tuduam/aerodynamics.py
--rw-rw-rw-  2.0 fat     6696 b- defN 24-Feb-13 07:26 tuduam/data_structures.py
--rw-rw-rw-  2.0 fat     2434 b- defN 24-Feb-13 07:26 tuduam/performance.py
--rw-rw-rw-  2.0 fat    42292 b- defN 24-Feb-13 07:26 tuduam/propulsion.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-13 07:26 tuduam/sim_ctrl.py
--rw-rw-rw-  2.0 fat    51051 b- defN 24-Feb-13 07:26 tuduam/structures.py
--rw-rw-rw-  2.0 fat       23 b- defN 24-Feb-13 07:30 tuduam/version.py
--rw-rw-rw-  2.0 fat     1548 b- defN 24-Feb-13 07:26 tuduam-2024.8.data/data/LICENSE
--rw-rw-rw-  2.0 fat      783 b- defN 24-Feb-13 07:26 tuduam-2024.8.data/data/README.md
--rw-rw-rw-  2.0 fat     1548 b- defN 24-Feb-13 07:30 tuduam-2024.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2085 b- defN 24-Feb-13 07:30 tuduam-2024.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-13 07:30 tuduam-2024.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Feb-13 07:30 tuduam-2024.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1176 b- defN 24-Feb-13 07:30 tuduam-2024.8.dist-info/RECORD
-15 files, 122016 bytes uncompressed, 31736 bytes compressed:  74.0%
+Zip file size: 42023 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat      262 b- defN 24-Apr-15 12:05 tuduam/__init__.py
+-rw-rw-rw-  2.0 fat    12019 b- defN 24-Apr-15 12:05 tuduam/aerodynamics.py
+-rw-rw-rw-  2.0 fat     6692 b- defN 24-Apr-15 12:05 tuduam/data_structures.py
+-rw-rw-rw-  2.0 fat     2434 b- defN 24-Apr-15 12:05 tuduam/performance.py
+-rw-rw-rw-  2.0 fat    42608 b- defN 24-Apr-15 12:05 tuduam/propulsion.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-15 12:05 tuduam/sim_ctrl.py
+-rw-rw-rw-  2.0 fat    85384 b- defN 24-Apr-15 12:05 tuduam/structures.py
+-rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-15 12:09 tuduam/version.py
+-rw-rw-rw-  2.0 fat     1548 b- defN 24-Apr-15 12:05 tuduam-2024.9.data/data/LICENSE
+-rw-rw-rw-  2.0 fat      783 b- defN 24-Apr-15 12:05 tuduam-2024.9.data/data/README.md
+-rw-rw-rw-  2.0 fat     1548 b- defN 24-Apr-15 12:09 tuduam-2024.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2085 b- defN 24-Apr-15 12:09 tuduam-2024.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 12:09 tuduam-2024.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-15 12:09 tuduam-2024.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1176 b- defN 24-Apr-15 12:09 tuduam-2024.9.dist-info/RECORD
+15 files, 156661 bytes uncompressed, 40093 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -18,29 +18,29 @@
 
 Filename: tuduam/structures.py
 Comment: 
 
 Filename: tuduam/version.py
 Comment: 
 
-Filename: tuduam-2024.8.data/data/LICENSE
+Filename: tuduam-2024.9.data/data/LICENSE
 Comment: 
 
-Filename: tuduam-2024.8.data/data/README.md
+Filename: tuduam-2024.9.data/data/README.md
 Comment: 
 
-Filename: tuduam-2024.8.dist-info/LICENSE
+Filename: tuduam-2024.9.dist-info/LICENSE
 Comment: 
 
-Filename: tuduam-2024.8.dist-info/METADATA
+Filename: tuduam-2024.9.dist-info/METADATA
 Comment: 
 
-Filename: tuduam-2024.8.dist-info/WHEEL
+Filename: tuduam-2024.9.dist-info/WHEEL
 Comment: 
 
-Filename: tuduam-2024.8.dist-info/top_level.txt
+Filename: tuduam-2024.9.dist-info/top_level.txt
 Comment: 
 
-Filename: tuduam-2024.8.dist-info/RECORD
+Filename: tuduam-2024.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tuduam/data_structures.py

```diff
@@ -106,16 +106,18 @@
     cd0: Optional[float] = None
     """"Zero lift drag coefficient"""
     spanwise_points: Optional[int] = None
     """"The spanwise points used in the Weissinger-L/Lifiting line method.
     Odd integer"""
 
 class Material(Parent):
+    safety_factor: float
+    load_factor: float
     young_modulus: Optional[float] = None
-    safety_factor: Optional[float] = None
+    load_factor: Optional[float] = None
     shear_modulus: Optional[float] = None
     poisson: Optional[float] = None
     density: Optional[float] = None
     sigma_yield: Optional[float] = None
     sigma_ultimate: Optional[float] = None
     shear_strength: Optional[float] = None
     beta_crippling: Optional[float] = None 
@@ -152,14 +154,11 @@
     t_sk_cell:list
     """The thickness of the skin in each cell, length should be equal to n_cell"""
     t_sp: float
     """The thickness of the spars"""
     area_str:float
     """"Area of the stringer"""
     str_cell: list
-    """"List of stringers (both top and bottom) per cell. Length should be n_cell"""
-    booms_sk: int
-    """"Amount of booms on the skin """
-    booms_spar: int
-    """"Amount of booms on each spar"""
+    """"List of stringers (both top and bottom) per cell. Length should be n_cell. Due to the discretization
+    it also required to be an even number"""
```

## tuduam/propulsion.py

```diff
@@ -1,42 +1,52 @@
 import re
+from typing import List
 import plotly.graph_objs as go
 import numpy as np
 import os
 import pdb
 from tuduam.data_structures import Propeller
 import matplotlib.pyplot as plt
 import scipy.integrate as spint
 from scipy.interpolate import NearestNDInterpolator
 from warnings import warn
 
 
 def extract_data_dir(dir_path:str) -> np.ndarray:
     """ This function pulls data from multiple files within a directory as outputted by Xfoil and puts them in one array. Information on how to do this can be found in the notebooks. 
 
+    **Assumptions**
+
+
+    1. The function expects the name to atleast have Rexxxx where the x's represent the Reynolds number
+
+
+
     :param dir_path: The path of the directory to read from can be absolute or relative
     :type dir_path: str
     :return: An  m x 8 array where the colums are the following: [alpha, CL, CD, CDp, CM, Top_xtr, bot_xtr, Reynolds number]
     :rtype: np.ndarray
     """    
-    data_points = list()
+    data_points: List[List[float]] = list()
 
     for file in os.listdir(dir_path):
         try:
             reyn = float(re.findall(r'Re(\d+)', file, re.IGNORECASE)[0])
         except IndexError:
             raise Exception("One of the files is likely in the incorrect format. Please check wheter the Reynolds number has Re infront of it")
         with open(os.path.join(dir_path,file), "r") as f:
             write = False
             for line in f.readlines():
-                if  line.count("-") > 3:
+                if  line.count("-") > 10:  # increase the threshold to a number larger than the number of columns in the file
                     write = True
                     continue
+                if line == '\n': # skip any empty line
+                    continue
                 if write:
-                    value_lst = [float(value) for value in line.split()]
+                    value_lst: List[float]  = [float(value) for value in line.split()]
                     value_lst.append(reyn)
                     data_points.append(value_lst)
     return np.array(data_points)
 
 
 def alpha_xfoil_interp(dir_path:str) -> NearestNDInterpolator:
     """ summary
@@ -123,15 +133,15 @@
             airfoil_coord.append(new_line)
 
         airfoil_coord = np.array(airfoil_coord)
         airfoil_coord = airfoil_coord.T
 
         return airfoil_coord
 
-    def plot_blade(self,tst=False):
+    def plot_blade(self,tst=False) -> None:
         """ Returns two plots, one top down view of the propeller showing the amount of twist and the various chords
         and one plot showing a side view of the propeller
 
         :param tst: A boolean which is used for testing to surpess the output, defaults to False
         :type tst: bool, optional
         """        
         # Create figures
@@ -665,28 +675,27 @@
             zeta = zeta_new
         #
         design = self.run_BEM(zeta)
         return design
 
 
 class OffDesignAnalysisBEM:
-    """
+    r"""
     A class encapsulating the arbitrary analysis of a propeller blade as described in Adkins and Liebeck (1994).
 
-    General notes
-    ----------------------
-    -  Interferences factors were clipped to -0.7 and 0.7. Viterna and Janetzke11 give empirical arguments 
+    **General notes**
+
+    1. Interferences factors were clipped to -0.7 and 0.7. Viterna and Janetzke11 give empirical arguments 
        for clipping the magnitude of a and a' at the value of 0.7 in order to better convergence.  See a_fac and a_prime_fac
 
-    Future improvement
-    -----------------------------
-    -  TODO: Also compare to sample example in original paper of Adkins and Liebeck (1994)
-    - TODO: Refactor such that rpm and V can be changed in the  self.analyse_propeller method. Reinstantiating the class would not be
-            necessary in that case
-    - TODO: Make the off design analysis robust enough so a scipy.optimize could perhaps be used in the future.
+    **Future improvement**
+    
+    1. TODO: Also compare to sample example in original paper of Adkins and Liebeck (1994)
+    2. TODO: Refactor such that rpm and V can be changed in the  self.analyse_propeller method. Reinstantiating the class would not be necessary in that case
+    3. TODO: Make the off design analysis robust enough so a scipy.optimize could perhaps be used in the future.
 
     """    
     def __init__(self, dir_path:str, propclass: Propeller, V: float,
                   rpm: float, rho: float, dyn_vis: float, a: float) -> None:
         self.V = V
         self.B = propclass.n_blades
         self.R = propclass.r_prop
```

## tuduam/structures.py

```diff
@@ -1,22 +1,37 @@
 import numpy  as np
-import random
-import plotly.graph_objs as go
-import plotly.express as px
-import plotly.figure_factory as ff
 from typing import Tuple, List
-import matplotlib.pyplot as plt
 from scipy.interpolate import CubicSpline
+import scipy.optimize as sop
 import scipy.constants as const
-from .data_structures import Wingbox
+from .data_structures import Wingbox, Material
 from math import ceil
-from shapely.geometry import Polygon, Point
+from shapely.geometry import Polygon
 from warnings import warn
+import random
 import pdb
 
+# Pymoo relevant imports
+from pymoo.core.problem import Problem, ElementwiseProblem
+from pymoo.core.problem import StarmapParallelization
+from pymoo.operators.crossover.sbx import SBX
+from pymoo.operators.mutation.pm import PM
+from pymoo.operators.repair.rounding import RoundingRepair
+from pymoo.operators.sampling.rnd import IntegerRandomSampling
+import multiprocessing
+from pymoo.algorithms.soo.nonconvex.ga import GA
+from pymoo.optimize import minimize
+
+# grahphing import
+import plotly.graph_objs as go
+import plotly.express as px
+import plotly.figure_factory as ff
+import matplotlib.pyplot as plt
+
+
 class Boom:
     """ A class to represent an idealized boom
     """
     def __init__(self) -> None:
         self.bid = None #  Boom ID
         self.A = None  # Area boom
         self.x = None # X location
@@ -38,15 +53,16 @@
             cell_idx = 0
         else:
             cell_idx = cell_idx.nonzero()[0][-1]
         return cell_idx
 
 
 class IdealPanel:
-    """_summary_
+    """
+    A class representing a panel in an idealized wingbox
     """
     def __init__(self):
         self.pid = None # Panel ID
         self.bid1 = None  # The boom id of its corresponding first boom id
         self.bid2 = None # The boom id of its corresponding second boom id
         self.b1 = None
         self.b2  = None
@@ -97,21 +113,20 @@
         except AttributeError as err:
             raise err("The boom instance has not been assigned yet or is missing the attribute x and y")
         self.dir_vec =  [x_comp, y_comp]
 
 class IdealWingbox():
     """ A class representing an idealized wingbox, containing methods to perform computations
     on that instants and some accessed methods. It is not recommended to use as a standalone tool but should 
-    be using in conjunction with the discretize_airfoil function.
+    be using in conjunction with the :func:`discretize_airfoil` function.
 
-    Assumptions
-    --------------------------------------------------------------------------------
-    - The x datum of the coordinate system should be attached to the leading edge of the 
+    **Assumptions**
+    1. The x datum of the coordinate system should be attached to the leading edge of the 
     wingbox
-    - Some methods such as the read_cell_area expect the first and last to begin and end on a vertex.
+    2. Some methods such as the read_cell_area expect the first and last to begin and end on a vertex.
 
 
     """    
     def __init__(self, wingbox: Wingbox, chord:float) -> None:
         self.wingbox_struct = wingbox
         self.chord = chord
         self.x_centroid = None # datum attached to leading edge
@@ -141,31 +156,42 @@
         for idx, spar_loc in enumerate(spar_loc_arr):
             if idx != len(spar_loc_arr) - 1:
                 panel_lst.append([i for i in self.panel_dict.values() if (spar_loc <= (i.b1.x + i.b2.x)/2 < spar_loc_arr[idx + 1]) and i.b1.x != i.b2.x])
             else:
                 panel_lst.append([i for i in self.panel_dict.values() if  (i.b1.x + i.b2.x)/2 >= spar_loc and i.b1.x != i.b2.x])
         return panel_lst
 
+    def get_total_area(self) -> float:
+        """ Returns the total area of all the booms. These booms also contain the addition of the skin thicknesses. This function in the library is used 
+        for the optimizatio of a wingbox.
 
-    def _get_polygon_of_cells(self, validate=False) -> List[float]:
-        """ Compute the area of each cell with the help of the shapely.geometry.Polygon class. The function expects a fully loaded airfoil to be in the 
+        :return: The total area of all the booms combined
+        :rtype: float
+        """        
+
+        tot_area = 0
+        for boom in self.boom_dict.values():
+            tot_area += boom.A
+        return tot_area
+
+
+    def get_polygon_cells(self, validate=False) -> List[float]:
+        """ 
+        Compute the area of each cell with the help of the shapely.geometry.Polygon class. The function expects a fully loaded airfoil to be in the 
         class using the idealized_airfoil function. Errenous results or an error will be given in case this is not the case! When using this function for the first time
         with a new airfoil it is advised to run it once with validate= True to see if the resulting areas are trustworthy. This will
         show you n plots of the cell polygon where n is the amount of cells.
 
-        Assumptions
-        -----------------------------------------------------------------------------
-        - Function is built for a object built with the discretize airfoil, that is cell 0 has a singular point as a leading edge, that is one
-        point is the furthest ahead. The same goes for cell n but with the trailing edge
+        **Assumptions**
+
+        1. Function is built for a object built with the discretize airfoil, that is cell 0 has a singular point as a leading edge, that is one point is the furthest ahead. The same goes for cell n but with the trailing edge
 
         :param validate: When True will show the 3 plots described above, defaults to False
         :type validate: bool, optional
-        :param validate:
-        :return: A list whic is m long where m is the amount of cells. Each element is the area
-        of the respective cell.
+        :return: A list whic is m long where m is the amount of cells. Each element is the area of the respective cell.
         :rtype: List[float]
         """        
         bm_per_cell_lst =  []
         polygon_lst =  []
 
         # Get all the booms per cell
         spar_loc_arr = np.insert(self.wingbox_struct.spar_loc_nondim, 0,0)*self.chord
@@ -251,33 +277,34 @@
                 x,y = poly.exterior.xy
                 plt.hlines([bnd], np.min(x_lst), np.max(x_lst), "r")
                 plt.plot(x,y)
                 plt.show()
 
         return polygon_lst
 
-    def read_cell_areas(self, validate= False):
-        polygon_lst = self._get_polygon_of_cells(validate)
+    def get_cell_areas(self, validate= False) -> List[float]:
+        polygon_lst = self.get_polygon_cells(validate)
         return [i.area for i in polygon_lst]
 
+
     def _compute_boom_areas(self, chord) -> None:
         """ Function that creates all boom areas, program assumes a fully functional panel and boom
         dictionary where all values have the full classes assigned. Function can be used by user manually
         but it is generall advised to use the discretize_airfoil function to create a wingbox.
 
-        Assumptions
-        --------------------------
-        - The idealizatin only takes into account a force in the vertical direction (that is tip-deflection path)
-        - The area of the stringers is smeared acrossed all skin booms in the respective cell
+        **Assumptions**
+
+        #. The idealizatin only takes into account a force in the vertical direction (that is tip-deflection path)
+        #. 
         """        
 
         # Find stringer area to add per cell
-        str_contrib = []
-        for idx, n_str in enumerate(self.wingbox_struct.str_cell):
-            str_contrib.append(n_str*self.wingbox_struct.area_str/len(self._read_skin_panels_per_cell[idx]))
+        # str_contrib = []
+        # for idx, n_str in enumerate(self.wingbox_struct.str_cell):
+        #     str_contrib.append(n_str*self.wingbox_struct.area_str/len(self._read_skin_panels_per_cell[idx]))
 
         # Define absolute spar location for use within the loop
         spar_loc_abs = np.array(self.wingbox_struct.spar_loc_nondim)*chord
         # Per boom find all the panel in which the boom is found and add skin contribution
         for boom in self.boom_dict.values():
             boom_area = boom.A =  0
             # Retrieve all panel where boom is a part of
@@ -285,35 +312,39 @@
             for pnl in pnl_lst:
                 if boom.bid == pnl.bid1:
                     boom_area += pnl.t_pnl*pnl.length()/6*(2 + (pnl.b2.y - self.y_centroid )/(boom.y - self.y_centroid))
                 else:
                     boom_area += pnl.t_pnl*pnl.length()/6*(2 + (pnl.b1.y - self.y_centroid)/(boom.y - self.y_centroid))
 
             boom.A = boom_area
+            # check if it is not a spar boom, this will get a flange addition in the future maybe
+            if not any(np.isclose(boom.x, spar_loc_abs )):
+                boom.A += self.wingbox_struct.area_str
+            if boom.A < 0: 
+                warn("Negative boom areas encountered this is currently a bug, temporary fix takes the absolute value")
+                boom.A = np.abs(boom.A)
 
-            if len(str_contrib) != 0 and not any(np.isclose(boom.x, spar_loc_abs )):
-                boom.A += str_contrib[boom.get_cell_idx(self.wingbox_struct, chord )]
 
-    def stress_analysis(self,  intern_shear:float, internal_mz:float, shear_centre_rel : float, shear_mod:float, validate=False) ->  Tuple[float, dict]:
+    def stress_analysis(self,  intern_shear:float, internal_mz:float, shear_centre_rel : float, shear_mod: float, validate=False) ->  Tuple[list,list]:
         """ 
         Perform stress analysis on  a wingbox section 
 
         List of assumptions (Most made in Megson, some for simplificatoin of code)
-        ---------------------------------------
+        ---------------------------------------------------------------------------
         - The effect of taper are not included see 21.2 (See megson) TODO: future implementation
         - Lift acts through the shear centre (no torque is created) TODO: future implementation
         - Stresses due to drag are not considered. 
 
 
 
         :param intern_shear: _description_
         :type intern_shear: float
         :param internal_mz: _description_
         :type internal_mz: float
-        :param shear_mod: _description_
+        :param shear_mod: shear_modulus
         :type shear_mod: float
         :return: _description_
         :rtype: Tuple[float, dict]
         """    
 
         # Ensure all shear flows are set to none because the function relies on it
         for pnl in self.panel_dict.values():
@@ -344,15 +375,15 @@
                     if cond1 and cond2 and cond3 and cond4: # Combine all statements
                         pnl.q_basic = 0 # Cut this panel
                         cut_lst.append(pnl) 
             # If are at the last cell cut both the left and right panel connected to the spar
             elif idx ==  len(self.wingbox_struct.spar_loc_nondim) - 1:
                 for pnl in self.panel_dict.values():
                     cond1 = pnl.b1.x != pnl.b2.x
-                    cond2 = pnl.b2.y >= self.y_centroid and pnl.b1.y >= self.y_centroid
+                    cond2 = (pnl.b2.y + pnl.b1.y)/2 >= self.y_centroid 
                     cond3 = pnl.b1.x == spar_loc or pnl.b2.x == spar_loc
                     if cond1 and cond2 and cond3:
                         pnl.q_basic = 0
                         cut_lst.append(pnl)
             # In case something goes wrong with the previous statements
             else:
                 raise Exception(f"Something went wrong, more iterations were made than there are cells")
@@ -419,16 +450,16 @@
                 else: 
                     raise Exception("No connecting panel was found")
 
 
         #=========================================================================
         # Now Compute the complementary shear flows and the twist per unit lengt   
         #========================================================================
-        area_lst = self.read_cell_areas() # Get the area per cell
-        centroid_lst = [np.array(poly.centroid.xy).flatten() for poly in self._get_polygon_of_cells()] # get the centroid of each cell
+        area_lst = self.get_cell_areas() # Get the area per cell
+        centroid_lst = [np.array(poly.centroid.xy).flatten() for poly in self.get_polygon_cells()] # get the centroid of each cell
 
         # Get the panel per cell, that is the fully defined cell. 
         pnl_per_cell_lst2 = []
         spar_loc_arr = np.insert(self.wingbox_struct.spar_loc_nondim, 0,0)*self.chord # dimensionalize and insert a zero
         for idx, spar_loc in enumerate(spar_loc_arr):
             # conditions for any cell except the last
             if idx != len(spar_loc_arr) - 1:
@@ -479,18 +510,18 @@
 
         # Set up eqautions for twist per unit legnth but in b array
         for idx, cell in enumerate(pnl_per_cell_lst2):
             b_ele = 0
             for pnl in cell:
                 r_abs_vec = np.array([(pnl.b1.x + pnl.b2.x)/2 , (pnl.b1.y + pnl.b2.y)/2])
                 r_rel_vec = r_abs_vec - centroid_lst[idx]
-                # When we have a panel that was not cut (they do not have a defined direction yet)
                 if pnl.q_basic != 0: 
                     sign = np.sign(np.cross(r_rel_vec, pnl.dir_vec))
                     b_ele += sign*pnl.q_basic*pnl.length()/pnl.t_pnl
+                # When we have a panel that was not cut, they do not have a defined direction yet and it does not matter since magnitude is 0
                 elif pnl.q_basic == 0:
                     b_ele += pnl.q_basic*pnl.length()/pnl.t_pnl
                 else:
                     raise Exception(f"Line should not have been reached")
             b_arr[idx,0] = b_ele
 
 
@@ -586,15 +617,15 @@
                             raise Exception(f"Line should not have been reached")
                 elif idx == len(pnl_per_cell_lst2) - 1:
                     # If it is on the left spar
                     if (pnl.b1.x == pnl.b2.x == x_min) :
                         sign = np.sign(np.cross(r_rel_vec, pnl.dir_vec))
                         pnl.q_tot  = pnl.q_basic + sign*qs_lst[idx] - sign*qs_lst[idx - 1]
                         pnl.tau = pnl.q_tot/pnl.t_pnl
-                    # Else if it not on the right spar just add qs,n
+                    # Else if  just add qs,n. As no other influece needs to be taken into account
                     else:
                         # Check if it was not the cut panel
                         if pnl.q_basic != 0: 
                             sign = np.sign(np.cross(r_rel_vec, pnl.dir_vec))
                             pnl.q_tot  = pnl.q_basic + sign*qs_lst[idx]
                             pnl.tau = pnl.q_tot/pnl.t_pnl
                         # if it is a cut panel
@@ -704,16 +735,14 @@
         # Create quiver figure
         fig = ff.create_quiver(x, y, u, v,
                             scale= scale,
                             arrow_scale= arrow_scale,
                             line= dict(color="red", width = 3),
                             name='Direction of shear flows',
                             line_width=1)
-
-
         fig.show()
 
 
 
 
     def plot_geometry(self) -> None:
 
@@ -744,31 +773,33 @@
 
             # For colorbar
             colorbar_trace_x.extend(x)
             colorbar_trace_y.extend(y)
 
         # Layout configuration
         layout = go.Layout(
-            title='Panel Stress Visualization',
+            title='Discretization of airfoil',
             xaxis=dict(title='X-axis'),
             yaxis=dict(title='Y-axis'),
         )
 
         # Create figure and add traces
         fig = go.Figure(data=traces, layout=layout)
         fig.show()
 
 
 def read_coord(path_coord:str) -> np.ndarray:
-    """ Returns an  m x 2 array of the airfoil coordinates based on a Selig formatted dat file.
+    """
+    Returns an  m x 2 array of the airfoil coordinates based on a Selig formatted dat file.
 
-    :return: An m x 2 array with the airfoil coordinates where x goes top trailing edge to top leading edge and then back to 
-    lower trailing edge. I.e it keeps the Selig format
+    :param path_coord: m x 2 array with the airfoil coordinates where x goes top trailing edge to top leading edge and then back to  lower trailing edge. I.e it keeps the Selig format
+    :type path_coord: str
+    :return: _description_
     :rtype: np.ndarray
-    """        
+    """    
     # List to save formatted coordinates
     airfoil_coord = []
 
     with open(path_coord) as f:
         for line in f.readlines():
             if any([i.isalpha() for i in line]):
                 continue
@@ -793,25 +824,25 @@
     bot_coord =  coord_scaled[np.argmin(coord_scaled[:,0]):, :] # coordinates of bottom skin
 
     top_interp = CubicSpline(top_coord[:,0], top_coord[:,1])
     bot_interp = CubicSpline(bot_coord[:,0], bot_coord[:,1])
     return top_interp, bot_interp
 
 def get_centroids(path_coord:str) -> Tuple[float, float]:
-    """ Compute the nondimensional x and y centroid based on the coordinate file of an airfoil.
+    r""" Compute the nondimensional x and y centroid based on the coordinate file of an airfoil.
     The centroids are computing assuming the following:
      
-     Assumptions
-     -----------------------------
-     - It is only based on the skin, i.e  the spar webs and stringers are ignored. Additionally the different thickness of the skin are not taken into account 
+     **Assumptions**
+
+     1. It is only based on the skin, i.e  the spar webs and stringers are ignored. Additionally the different thickness of the skin are not taken into account 
      The implication being that the x centroid should be at x/c = 0.5. Unless there was a bias in the sampling points
 
-    Future improvement
-     -----------------------------
-     - Take into account the spar webs for a better x centroid. However irrelevant for now as we only
+    **Future improvement** 
+
+     1. Take into account the spar webs for a better x centroid. However irrelevant for now as we only
      take into account forces in the vertical directoin
     
 
     :param path_coord: Path to the geometry file using the Selig format
     :type path_coord: str
     :return: The nondimensional x and y centroid of the airfoil
     :rtype: Tuple[float, float]
@@ -819,33 +850,37 @@
     coord = read_coord(path_coord)
     y_centroid_dimless = np.sum(coord[:,1])/coord.shape[0]
     x_centroid_dimless = np.sum(coord[:,0])/coord.shape[0]
     return x_centroid_dimless, y_centroid_dimless
 
 
 def discretize_airfoil(path_coord:str, chord:float, wingbox_struct:Wingbox) -> IdealWingbox:
-    """ Create a discretized airfoil according to the principles of Megson based on a path to a txt file containing
+    r""" Create a discretized airfoil according to the principles of Megson based on a path to a txt file containing
     the non-dimensional coordinates of the airfoil, the corresonding chord and the wingbox data structure fully filled in.
 
-    Assumptions
-    -------------------------------------
-    - Airfoil is idealized according Megson ch. 20
-    - The stringers are modeled by equally smearing the total area of the combined 
-    stringers in a certain cell  to all booms attached to the skin in that cell 
-    - The ratio of $\frac{\sigma_1}{\sigma_2}$  required for the boom size based on the skin is 
-    determined by the ratio of their y positin thus $\frac{y_1}{y_2}$.
-
-    General Procedure
-    -----------------------------------------------
-    1. Create a spline of the top and bottom airfoil
-    2. Create array along which to sample this spline to create the booms, creating specific samples for the spar positions
-    3. Move over top surface creating booms and panel as we go
-    4. Do the same for the bottom surface moving in a circle like motion
-    5. Move over all the spars and create booms and panels as we go.
-    6. Iterate over all booms and add skin contribution and stringer contribution to all their areas
+    **Assumptions**
+
+    #. Airfoil is idealized according Megson ch. 20 
+    #. Each stringer will form one boom in the discretized airfoil 
+    #. Only an equal amount of stringers can be specified per cell, if that is not the case a warning is issued however. (due to the method of discretization)
+    #. The ratio of :math:`\frac{\sigma_1}{\sigma_2}` required for the skin contribution to the  boom size based on the skin is determined by the ratio of their y positin thus :math:`\frac{y_1}{y_2}`. \n
+    
+
+    **General Procedure**
+
+    #. Create a spline of the top and bottom airfoil
+    #. Create array along which to sample this spline to create the booms, creating specific samples for the spar positions
+    #. Move over top surface creating booms and panel as we go
+    #. Do the same for the bottom surface moving in a circle like motion
+    #. Move over all the spars and create booms and panels as we go.
+    #. Iterate over all booms and add skin contribution and stringer contribution to all their areas
+
+    **Future Improvements**
+
+    #. Add contribution of spar caps (For now as been left out as I did not see the value of it at the time)
 
 
     :param path_coord: _description_
     :type path_coord: str
     :param chord: _description_
     :type chord: float
     :param wingbox_struct: _description_
@@ -854,31 +889,61 @@
     :rtype: IdealWingbox
     """    
     
     # Check  wingbox data structure
     assert len(wingbox_struct.t_sk_cell) == wingbox_struct.n_cell, "Length of t_sk_cell should be equal to the amount of cells"
     assert len(wingbox_struct.str_cell) == wingbox_struct.n_cell, "Length of str_cell should be equal to the amount of cells"
     assert len(wingbox_struct.spar_loc_nondim) == wingbox_struct.n_cell - 1, "Length of spar_loc should be equal to the amount of cells - 1"
-    assert wingbox_struct.booms_spar > 4, "Length of spar_loc should be equal to the amount of cells - 1"
+    assert all(np.round(wingbox_struct.str_cell,0) > 4), "Each cell must have atleast five stringers. The following configuration would results in an error during runtime"
 
     top_interp, bot_interp = spline_airfoil_coord(path_coord, chord)
     x_centr, y_centr = get_centroids(path_coord)
 
     wingbox = IdealWingbox(wingbox_struct, chord)
     wingbox.x_centroid =  x_centr*chord
     wingbox.y_centroid =  y_centr*chord
 
 
-    x_boom_loc = np.linspace(0, chord, ceil(wingbox_struct.booms_sk/2 + 2))
+    spar_loc_lst: list = np.insert(wingbox_struct.spar_loc_nondim, [0, wingbox_struct.n_cell - 1], [0, 1])*chord
+    str_lst: list = wingbox_struct.str_cell # list with the amount of stringers per cell
+
+    x_boom_loc = np.array([])
+
+    #TODO create a new x_boom_loc 
+    for idx, loc in enumerate(spar_loc_lst): 
+        if idx != len(spar_loc_lst) - 1:
+            len_cell = spar_loc_lst[idx + 1] - loc
+            # A 0.1 starting point is chosen to avoid 
+            str_tot = str_lst[idx] 
+            
+            # See assumptions, the following make sure any float get rounded since
+            # the optimizer usually does not return nice integers. It then also gives a warning
+            # if the value was not an integer
+            if isinstance(str_tot, int):
+                if str_tot % 2 != 0:
+                    warn(f"{str_lst[idx]} was not an even number and will be floored for conservative reasons")
+                    n_str = np.floor(str_lst[idx]/2)
+                else: 
+                    n_str = str_lst[idx]/2
+            else: 
+                str_tot = np.round(str_tot,0)
+                if str_tot % 2 != 0:
+                    warn(f"{str_lst[idx]} was not an even number and will be floored for conservative reasons")
+                    n_str = np.floor(str_lst[idx]/2)
+                else: 
+                    n_str = str_lst[idx]/2
+
+            if idx != 0:
+                loc_cell =  np.linspace(loc , spar_loc_lst[idx + 1], int(n_str + 1))[1:]
+            else:
+                loc_cell =  np.linspace(loc , spar_loc_lst[idx + 1], int(n_str + 1))
+            x_boom_loc = np.append(x_boom_loc, loc_cell)
+        else: 
+            pass
 
-    # Put booms at the spar locations
-    for spar_loc in wingbox_struct.spar_loc_nondim:
-        spar_loc *= chord
-        idx = np.argmin(np.abs(x_boom_loc - spar_loc))
-        x_boom_loc[idx] = spar_loc
 
     boom_dict = {}
     panel_dict = {}
     bid = 0 # set bid to zero
     pid = 0  # set panel counter to zero
     # create the upper booms and panels from leading edge to trailing edge
     for idx, x_boom in enumerate(x_boom_loc, start=0):
@@ -958,66 +1023,26 @@
         if spar_booms[0].y > spar_booms[1].y:
             upper_b = spar_booms[0]
             lower_b = spar_booms[1]
         else:
             upper_b = spar_booms[1]
             lower_b = spar_booms[0]
 
-        y_locations = np.delete(np.linspace(upper_b.y, lower_b.y, wingbox_struct.booms_spar), [0,-1]) # delete padding as they already have booms
-
-        # Loop over the spar to create the booms
-        for idx, y_loc in enumerate(y_locations, start=0):
-            # Create boom
-            boom = Boom()
-            boom.bid = bid
-            boom.x =  spar_loc
-            boom.y = y_loc
-            if boom.bid not in boom_dict.keys():
-                boom_dict[boom.bid] = boom
-            else:
-                raise RuntimeError(f"Boom id {boom.bid} already exists in variable boom dictionary")
 
-            if idx == 0:
-                pnl = IdealPanel()
-                pnl.pid = pid
-                pnl.bid1 = upper_b.bid 
-                pnl.bid2 = bid
-                pnl.t_pnl = wingbox_struct.t_sp
-                pnl.b1 =  boom_dict[pnl.bid1]
-                pnl.b2 =  boom_dict[pnl.bid2]
-                if pnl.pid not in panel_dict.keys():
-                    panel_dict[pid] = pnl
-                else:
-                    raise RuntimeError(f"Boom id {boom.bid} already exists in variable boom dictionary")
-            else: 
-                pnl = IdealPanel()
-                pnl.pid = pid
-                pnl.bid1 = bid - 1
-                pnl.bid2 = bid
-                pnl.t_pnl = wingbox_struct.t_sp
-                pnl.b1 =  boom_dict[pnl.bid1]
-                pnl.b2 =  boom_dict[pnl.bid2]
-
-                if pnl.pid not in panel_dict.keys():
-                    panel_dict[pid] = pnl
-                else:
-                    raise RuntimeError(f"Boom id {boom.bid} already exists in variable boom dictionary")
-
-            bid += 1
-            pid += 1
-
-        # Connect the last panel to the lower boom
+        # Create panel connecting upper boom and lower boom
         pnl = IdealPanel()
         pnl.pid = pid
-        pnl.bid1 = bid - 1
+        pnl.bid1 = upper_b.bid 
         pnl.bid2 = lower_b.bid
         pnl.t_pnl = wingbox_struct.t_sp
         pnl.b1 =  boom_dict[pnl.bid1]
         pnl.b2 =  boom_dict[pnl.bid2]
 
+
+
         if pnl.pid not in panel_dict.keys():
             panel_dict[pid] = pnl
         else:
             raise RuntimeError(f"Boom id {boom.bid} already exists in variable boom dictionary")
         pid += 1
 
 
@@ -1025,14 +1050,718 @@
     wingbox.panel_dict.update(panel_dict)
 
     wingbox._compute_boom_areas(chord)
 
     return wingbox
 
 
+class ProblemFreePanel(ElementwiseProblem):
+    """ The following problem sets up Discrete variable problem which optimises the amount of stringers per cell. This was done 
+    in a separate problem as changing the amount of stringers changes the amount of panels and hence the amount of constraints. Most optimizers
+    do not allow this, hence the following problem uses the output of the :class:`WingboxFixedPanel` to abide by the constraints.
+    """    
+
+    def __init__(self, shear: float, moment: float, applied_loc: float, chord: float, len_sec: float, box_struct: Wingbox, mat_struct: Material,
+                 path_coord: str, **kwargs_intern ):
+
+        self.box_params: list =  list()
+        self.shear = shear
+        self.moment = moment
+        self.applied_loc = applied_loc
+        self.chord = chord
+        self.len_sec = len_sec
+        self.box_struct = box_struct
+        self.mat_struct = mat_struct
+        self.path_coord = path_coord
+        self.kwargs_intern = kwargs_intern #  Used to pass any settings to GA_optimize functions
+
+        super().__init__(n_var= box_struct.n_cell, n_obj=1, n_ieq_constr=0, xl=5, xu=40, vtype= int, **kwargs_intern)
+
+    def _evaluate(self, x, out, *args, **kwargs) -> None:
+        """ This function get evaluated for each 'element', where an element in this case is a single sequence of n_var long. For more info
+        please see the documentation of the pymoo library.
+
+        :param x: A list of n_var long containing the amount of stringers per cell
+        :type x: np.ndarray
+        :param out: A dictionary containing the constraitns and objective
+        :type out: dict
+        """        
+
+        
+        n_cell = self.box_struct.n_cell
+
+        if len(x) != n_cell:
+            raise RuntimeError("The flattened  design vector received does not match the wingbox properties")
+        
+        sec_opt =  SectionOptimization(self.path_coord, self.chord, self.len_sec,  self.box_struct, self.mat_struct)
+
+        try:
+            self.kwargs_intern.pop("elementwise_runner")
+        except KeyError:
+            pass
+
+        GA_res = sec_opt.GA_optimize(self.shear, self.moment, self.applied_loc, **self.kwargs_intern)
+
+        if GA_res.X is None:
+            raise ValueError(f"Internal optimization for stringers {x} was not successful and the outer optimization could not continue")
+
+        # Discretize airfoil from new given parameters
+        wingbox_obj = discretize_airfoil(self.path_coord, self.chord, self.box_struct)
+
+        out["F"] = wingbox_obj.get_total_area() 
+
+class ProblemFixedPanel(ElementwiseProblem):
+    """
+        The followinng problem sets up an exploration of a wingbox for a fixed amount of stringers per cell. Since it is difficult for an optimizer
+        like COBYLA to find a global minimum a genetica algorith is set up first to explore the design space. This problem sets up this search.
+    """    
+
+    def __init__(self, shear: float, moment: float, applied_loc: float, chord: float, len_sec: float,
+                 box_struct: Wingbox, mat_struct: Material, path_coord: str, **kwargs):
+
+        self.shear = shear
+        self.moment = moment
+        self.applied_loc = applied_loc
+        self.chord = chord
+        self.len_sec = len_sec
+        self.box_struct = box_struct
+        self.mat_struct = mat_struct
+        self.path_coord = path_coord
+        sample = discretize_airfoil(self.path_coord, self.chord, self.box_struct)
+
+        super().__init__(n_var= box_struct.n_cell + 2, n_obj=1, n_ieq_constr= 2*len(sample.panel_dict), xl=np.ones(self.box_struct.n_cell + 2)*1e-8, xu=np.ones(self.box_struct.n_cell + 2), **kwargs)
+
+    def _evaluate(self, x, out, *args, **kwargs):
+        """
+        The function is excecuted at each element in the optimization. The arguments that are passed should be in the following 
+        order t_sk_cell, t_sp, area_str. Together given a total length of N + 2 where N is the amount of cells.
+        This interally checked if it is not the case a runtime error will be raised
+
+        :param x: The design variable vector which is in the following format [t_sk_cell, t_sp, area_str, str_cell]
+        :type x: list
+        :param shear: The shear force for which we're optimizing
+        :type shear: float
+        :param moment: The moment for which we're optimizing
+        :type moment: float
+        :param applied_loc: The applied location of the shear force on the wingbox.
+        :type applied_loc: float
+        :param str_lst: A list with the amount of stringers per cell.
+        :type str_lst: list
+        :raises RuntimeError: when the flattened design vector does not match the specified wingbox properties.
+        """        
+        
+        n_cell = self.box_struct.n_cell
+
+        if len(x) != n_cell + 2:
+            raise RuntimeError("The flattened  design vector received does not match the wingbox properties")
+        
+        
+        # Assing new properties to the wingbox struct assuming the specified length
+        t_sk_cell =  x[:n_cell]
+        t_sp = x[n_cell]
+        area_str = x[n_cell + 1]
+
+        self.box_struct.t_sk_cell = t_sk_cell
+        self.box_struct.t_sp = t_sp
+        self.box_struct.area_str =  area_str
+
+        # Discretize airfoil from new given parameters
+        wingbox_obj = discretize_airfoil(self.path_coord, self.chord, self.box_struct)
+
+        # Perform stress analysis
+        wingbox_obj.stress_analysis(self.shear, self.moment, self.applied_loc, self.mat_struct.shear_modulus)
+
+        #================ Get constraints ======================================
+        constr_cls = IsotropicWingboxConstraints(wingbox_obj, self.mat_struct, self.len_sec)
+        out["F"] = wingbox_obj.get_total_area() 
+        out["G"] = np.negative(np.concatenate((constr_cls.interaction_curve(), constr_cls.von_Mises()))) # negative is necessary because pymoo handles inequality constraints differently
+
+class SectionOptimization:
+    """
+    The following class allows for the optimization of a single airfoil section. The clas assumes that the correct material properties
+     have been embedded in :class:`Material` has been chosen, an initial estimate should be embedded in the :class:`Wingbox` class.
+
+    **Attributes**
+
+    :param path_coord: The path to the coordinate file of the airfoil that is used
+    :type path_coord: string
+    :param chord: The chord size
+    :type chord: float
+    :param len_sec: The length of the section, that is the length to the next rib
+    :type len_sec: float
+    :param box_struct: The wingbox structure
+    :type box_struct: wingbox
+    :param mat_struct: The Material  data structure
+    :type box_struct: Material
+    """    
+    def __init__(self, path_coord: str, chord: float, len_sec: float, wingbox_struct: Wingbox, material_struct: Material) -> None:
+        """Constructor method
+
+        :param path_coord: The path to the coordinate file of the airfoil that is used
+        :type path_coord: str
+        :param chord: The chord size
+        :type chord: float
+        :param len_sec: The length of the section, that is the lengt to the next rib
+        :type len_sec: float
+        :param wingbox_struct: THe wingbox datastructure
+        :type wingbox_struct: Wingbox
+        :param material_struct: _description_
+        :type material_struct: Material
+        """        
+
+        self.path_coord = path_coord
+        self.chord = chord
+        self.len_sec =  len_sec
+        self.box_struct: Wingbox = wingbox_struct
+        self.mat_struct: Material  = material_struct
+
+        # Required Overhead
+        self.wingbox_obj: None | IdealWingbox = None
+
+    def GA_optimize(self, shear: float, moment: float, applied_loc: float,
+                     n_gen: int = 50, # Possible keywords
+                     pop: int = 100,
+                     verbose: bool = True,
+                     seed: int = 1,
+                     multiprocess: bool =  False,
+                     cores: int = multiprocessing.cpu_count(),
+                     save_hist: bool = True):
+        
+        """ The following function executes the Genetic Algorithm (`GA <https://pymoo.org/algorithms/soo/ga.html>`_) to optimize the wingbox given to the overarching class
+        and with the loads fed to the function. Additionally there are some keywords which are explained below.
+
+        :param shear: The internal shear force acting at the section
+        :type shear: float
+        :param moment: The internal moment acting at the section
+        :type moment: float
+        :param applied_loc: The position of the internal shear force given as a ratio to the chord.
+        :type applied_loc: float
+        :param n_gen: The amount of generations allowed before termination, defaults to 50
+        :type n_gen: int, optional
+        :param pop: The generation size, defaults to 50
+        :type pop: int, optional
+        :param verbose: If true will print the results of all generations, defaults to True
+        :type verbose: bool, optional
+        :param seed: The seed for the random generations of the samples, defaults to 1
+        :type seed: int, optional
+        :param cores: The amount of cores used for the parallelization of the evaluations , defaults to multiprocesing.cpu_count()
+        :type cores: int, optional 
+        :param save_hist: Saves the history in the result object if true, defaults to True
+        :type save_hist: bool, optional
+        :return: Returns the result class from pymoo, which will also contain the history if specified true. Please see the example for use cases (`example <https://pymoo.org/getting_started/part_4.html>`_) .
+        :rtype: pymoo.core.result.Result
+        """        
+
+        # initialize the thread pool and create the runner
+        if multiprocess:
+            n_proccess =  cores
+            pool = multiprocessing.Pool(n_proccess)
+            runner = StarmapParallelization(pool.starmap)
+
+            problem = ProblemFixedPanel(shear, moment, applied_loc, self.chord,  self.len_sec, 
+                                        self.box_struct, self.mat_struct, self.path_coord, elementwise_runner=runner)
+        else:
+            problem = ProblemFixedPanel(shear, moment, applied_loc, self.chord,  self.len_sec, 
+                                        self.box_struct, self.mat_struct, self.path_coord)
+
+        method = GA(pop_size=pop, eliminate_duplicates=True)
+        resGA = minimize(problem, method, termination=('n_gen', n_gen), seed= seed,
+                        save_history=save_hist, verbose=verbose)
+        return resGA
+
+    def _obj_func_cobyla(self, x: list, shear: float, moment: float, applied_loc: float, str_lst: list):
+        """
+        This function is not to be intended by the user hence it is hinted to be a private method. The function passed to the scip.optimize.minmize function. The arguments that are passed should be in the following 
+        order t_sk_cell, t_sp, area_str. Together given a total length of N + 2 where N is the amount of cells.
+        This interally checked if it is not the case a runtime error will be raised
+
+        :param x: The design variable vector which is in the following format [t_sk_cell, t_sp, area_str, str_cell]
+        :type x: list
+        :param shear: The shear force for which we're optimizing
+        :type shear: float
+        :param moment: The moment for which we're optimizing
+        :type moment: float
+        :param applied_loc: The applied location of the shear force on the wingbox.
+        :type applied_loc: float
+        :param str_lst: A list with the amount of stringers per cell.
+        :type str_lst: list
+        :raises RuntimeError: when the flattened design vector does not match the specified wingbox properties.
+        """        
+        
+        n_cell = self.box_struct.n_cell
+
+        if len(x) != n_cell + 2:
+            raise RuntimeError("The flattened  design vector received does not match the wingbox properties")
+        
+        
+        # Assing new properties to the wingbox struct assuming the specified length
+        t_sk_cell =  x[:n_cell]
+        t_sp = x[n_cell]
+        area_str = x[n_cell + 1]
+
+        self.box_struct.t_sk_cell = t_sk_cell
+        self.box_struct.t_sp = t_sp
+        self.box_struct.area_str =  area_str
+        self.box_struct.str_cell = str_lst
+
+        # Discretize airfoil from new given parameters
+        self.wingbox_obj = discretize_airfoil(self.path_coord, self.chord, self.box_struct)
+
+        # Perform stress analysis
+        self.wingbox_obj.stress_analysis(shear, moment, applied_loc, self.mat_struct.shear_modulus)
+
+        return self.wingbox_obj.get_total_area() 
+
+
+    def optimize_cobyla(self, shear: float, moment: float, applied_loc: float, str_lst: list,
+                        bnd_mult: int = 1e3, 
+                        x0: list | None = None) -> sop._optimize.OptimizeResult:
+        """ Optimizes the design using the COBYLA optimizers with the constraints defined in :class:` IsotropicWingboxConstraints`.  The optimization parameters
+        are the skin thickness in each cell, the spar thickness and the area of the stringers. Hence the resulting design vector is x = [] The amount of stringers is not a optimization parameter here
+        as this would results in a varying amount of constraints which is not supported by COBYLA. Hence, the result of this will be fed to a different 
+        optimizer.
+
+        :param shear: _description_
+        :type shear: float
+        :param moment: _description_
+        :type moment: float
+        :param applied_loc: _description_
+        :type applied_loc: float
+        :param str_list: List of the amount of stringers per cell
+        :type str_list: list
+        :param bnd_mult: A multiplier to increase the enforcement of the boudns on the variables, default to 1000
+        :type bnd_mult: int, optional
+        :param x0: A more explicit way to define the intial estimate instead of taking it from the wingbox struct, default to None
+        :type x0: list, optional
+        :return: _description_
+        :rtype: sop._optimize.OptimizeResult
+        """        
+
+        n = self.box_struct.n_cell # quick reference to number of cells
+        # Whatever parameters were given in the datastrucrtre are used as inital estimate
+        if x0 is None:
+            x0 = self.box_struct.t_sk_cell + [self.box_struct.t_sp] + [self.box_struct.area_str] 
+        else:
+            pass
+
+        constr_lst: List[dict] = [
+            {'type': 'ineq', 'fun': self._get_constraint_vector, "args": [shear, moment, applied_loc]},
+                ]
+
+        #FIXME Cobyla does not take bounds class
+        lb_lst = []
+        ub_lst = []
+
+        for i in range(len(x0)):
+            if i <= n-1:
+                lb_lst.append(1e-5)
+                ub_lst.append(0.3)
+            elif i == n :
+                lb_lst.append(1e-5)
+                ub_lst.append(0.5)
+            elif i  ==  n + 1: 
+                lb_lst.append(1e-8)
+                ub_lst.append(1)
+        
+        # Apply bounds through constraints manually so we can penalize them with a greater quantity
+        # Otherwise they migt be ignored compared to other constraints
+        for i in range(len(lb_lst)):
+            def upper_constraint(x, idx):
+                return 1e3*(ub_lst[idx] - x[idx])
+
+            def lower_constraint(x, idx):
+                return 1e3*(x[idx] - lb_lst[idx])
+
+            constr_lst.append({'type':'ineq', 'args': [i], 'fun':upper_constraint})
+            constr_lst.append({'type':'ineq', 'args':[i], 'fun':lower_constraint})
+
+        res = sop.minimize(self._obj_func_cobyla, x0, args=(shear, moment, applied_loc, str_lst), method="COBYLA" , constraints= constr_lst)
+        return res
+    
+    def full_section_opt(self, shear: float, moment: float, applied_loc: float,
+                     n_gen_full: int = 50, # Possible keywords
+                     pop_full: int = 100,
+                     verbose_full: bool = True,
+                     cores: int = multiprocessing.cpu_count(),
+                     seed: int = 1,
+                     save_hist_full: bool = True, **kwargs):
+        """ 
+        The following functions handles the full optimization of the wingbox. Compared to the func:`GA_optimize` the following functions also varies
+        the amount of stringers per cell to find the optimum design. In order to do this it utlizes all previously defined optimization in combination 
+        with a discrete Geentic algoirth variabled optimization. 
+
+        :param shear: _description_
+        :type shear: float
+        :param moment: _description_
+        :type moment: float
+        :param applied_loc: _description_
+        :type applied_loc: float
+        :param n_gen_full: _description_, defaults to 50
+        :type n_gen_full: int, optional
+        :param verbose_full: _description_, defaults to True
+        :type verbose_full: bool, optional
+        :param seed: _description_, defaults to 1
+        :type seed: int, optional
+        :param save_hist_full: _description_, defaults to True
+        :type save_hist_full: bool, optional
+        """        
+
+        n_proccess =  cores
+        pool = multiprocessing.Pool(n_proccess)
+        runner = StarmapParallelization(pool.starmap)
+        prob = ProblemFreePanel(shear, moment, applied_loc, self.chord, self.len_sec, self.box_struct, self.mat_struct, 
+                                self.path_coord, elementwise_runner=runner, **kwargs)
+        
+
+        method = GA(pop_size=pop_full,
+                    sampling=IntegerRandomSampling(),
+                    crossover=SBX(prob=1.0, eta=3.0, vtype=float, repair=RoundingRepair()),
+                    mutation=PM(prob=1.0, eta=3.0, vtype=float, repair=RoundingRepair()),
+                    eliminate_duplicates=True,
+                    )
+
+        res = minimize(prob,
+                    method,
+                    termination=('n_gen', n_gen_full),
+                    seed=seed,
+                    save_history= save_hist_full,
+                    verbose= verbose_full
+                    )
+        return res
+
+
+
+
+
+    def _get_constraint_vector(self, x: list, shear: float, moment: float, applied_loc: float) -> list:
+        r""" 
+        The following function utilizes all other constraints and wraps their results into one vector. Where each 
+        element represents one  of the inequality constraints. The reasons we utilize this method instead of just passing each function as their own constraint
+        has to do with the overhead that would be incurred. Since scipy.optimize.minimize can only take a flattened array, I can not pass the actual discretized
+        airfoil around. Hence, if I want to get the discretize airfoil from the flattened array I have to run the  :func:`discretize_airfoil` again.  To avoid
+        doing this a multitude times all constraints are wrapped into one function.
+
+        :param x: The flattened array received from the scipy.optimize.minimize function.
+        :type x: list
+        :param wingbox_struct: The wingbox struct from the  data structures module        
+        :param shear: The applied shear force on the wingbox.
+        :type shear: float
+        :param moment: The applied moment on the wingbox
+        :type moment: float
+        :param applied_loc: The applied location of the shear force on the wingbox
+        :type applied_loc: float
+        :return: All constraints appended to each other into one constraints
+        :rtype: list
+        """ 
+
+        n_cell = self.box_struct.n_cell
+        t_sk_cell =  x[:n_cell]
+        t_sp = x[n_cell]
+        area_str = x[n_cell + 1]
+
+        self.box_struct.t_sk_cell = t_sk_cell
+        self.box_struct.t_sp = t_sp
+        self.box_struct.area_str =  area_str 
+
+        ideal_wingbox: IdealWingbox = discretize_airfoil(self.path_coord, self.chord, self.box_struct)
+        ideal_wingbox.stress_analysis(shear, moment, applied_loc, self.mat_struct.shear_modulus)
+        constr_cls = IsotropicWingboxConstraints(ideal_wingbox, self.mat_struct, self.len_sec)
+        return np.concatenate((constr_cls.interaction_curve(), constr_cls.von_Mises()))
+
+
+class IsotropicWingboxConstraints:
+    def __init__(self, wingbox:IdealWingbox, material_struct: Material, len_to_rib: float) -> None:
+        self.wingbox = wingbox
+        self.material_struct = material_struct
+        self.len_to_rib = len_to_rib
+        self.pnl_lst =  [i for i in self.wingbox.panel_dict.values()] 
+        self.tens_pnl_idx =  [idx for idx, i in enumerate(self.wingbox.panel_dict.values()) if (i.b1.sigma > 0) and (i.b2.sigma > 0)] # Panel which are in tension since for some of the constraints it is not relevant here
+
+        # Value used for the interpolation to get Kb
+        x = [1. , 1.5, 2. , 2.5, 3. , 3.5, 4. , 4.5, 5. ]
+        y = [9.5, 7.2, 6.4, 6, 5.8, 5.9, 5.8, 5.6, 5.4]
+
+        # Interpolator for critical shear function
+        self.kb_spline = CubicSpline(x,y, extrapolate=False) 
+    
+    def _kb_interp(self, ar_lst: list):
+        res = self.kb_spline(ar_lst)
+        res = np.nan_to_num(res, nan= 5.) # Set values that were outside of the interpolation range to 5.
+        return res
+
+
+    def _crit_instability_compr(self) -> list:#TODO
+        r""" 
+        Compute the elastic instability of a flat sheet in compression for each panel in the idealized wingbox using 
+        the equation shown below.
+
+
+        .. math::
+            \sigma_{cr} = k_c  \frac{pi^2 E}{12(1 - \nu)} \left(\frac{t_{sk}}{b}\right)^2
+
+        Where b is the short dimension of plate or loaded edge. For :math:`K_c` a value of 4 was chosen. Please see the figure below for the reasoning.
+        Since all edges are considerded simpy supported from either the stringer or the ribs it is conservative to go for a value of 4.
+        For any other information please see source 1.
+
+        .. image:: ../_static/buckle_coef.png
+            :width: 300
+        
+        **Future improvements**
+        1.  compute the proper buckling coefficient in real time using the sheet aspect ratio (or just check for aspect ratio's smaller than 1. These seem to be the most relevant to catch)
+        2. A plasticity factor could be implemented (see source 1, equation C5.2)
+
+        **Bibliography**
+
+        1. Chapter C5.2, Bruhn, Analysis & Design of Flight Vehicle Structures
+
+        :param wingbox: Ideal wingbox class which is utilized to create constraints per panel 
+        :type wingbox: IdealWingbox
+        :param material_struct: Data structure containing all material propertie
+        :type material_struct: Material
+        :param len_to_rib: The  distance to the next rib
+        :type len_to_rib: float
+        :return: The critical buckling stress due to compression
+        :rtype: float
+        """    
+        kc = 4 # buckling coefficient (currently very conservative but should be computed in real time using)
+        t_arr = np.array([i.t_pnl for i in self.pnl_lst])  # thickness array of all the panels
+        b = np.array([min(i.length(), self.len_to_rib) for i in self.pnl_lst])
+        res = kc*np.pi**2*self.material_struct.young_modulus/(12*(1 - self.material_struct.poisson ** 2)) * (t_arr/b) ** 2
+        # res[self.tens_pnl_idx] = 1
+        return res
+
+
+    def _crit_instability_shear(self) -> list:#TODO
+        r""" 
+        Compute the elastic instability of a flat sheet in shear for each panel in the idealized wingbox using  
+        the equation shown below. Very similar for the case in compression (see :func:`crit_instability_compr`) except for the shear buckling coefficient.
+
+
+        .. math::
+            \sigma_{cr} = k_b  \frac{pi^2 E}{12(1 - \nu)} \left(\frac{t_{sk}}{b}\right)^2
+
+        Where b is the short dimension of plate or loaded edge. For :math:`K_b`, the shear buckling coefficient, 
+        the figure below was used to make a polynomial fit of the 3rd degree. The dataset used was as follows:
+
+        x = [1. , 1.5, 2. , 2.5, 3. , 3.5, 4. , 4.5, 5. ] 
+        y = [9.5, 7.2, 6.4, 6, 5.8, 5.9, 5.8, 5.6, 5.4]
+
+
+        The interpolator was created in the initilisation of the class. For any other information please see source 1.
+
+        .. image:: ../_static/shear_buck_coef.png
+            :width: 300
+        
+        **Future improvements**
+        1. A plasticity factor could be implemented (see source 1, equation C5.2)
+
+        **Bibliography**
+
+        1. Chapter C5.7, Bruhn, Analysis & Design of Flight Vehicle Structures
+
+        :param wingbox: Ideal wingbox class which is utilized to create constraints per panel 
+        :type wingbox: IdealWingbox
+        :param material_struct: Data structure containing all material propertie
+        :type material_struct: Material
+        :param len_to_rib: The length to the next rib, thus the length to the next simply supported edge in the spanwise direction.
+        :type len_to_rib: float
+        :return: The critical buckling stress due to compression
+        :rtype: float
+        """    
+        t_arr = np.array([i.t_pnl for i in self.pnl_lst])  # thickness array of all the panels
+
+        # For the length of each panel we must look at the stringers 
+
+        asp_lst = [] # Aspect ratio list
+        b_lst = []
+        for pnl in self.pnl_lst:
+            len_pnl: float = pnl.length()
+            # Make sure to divide by the shortest side
+            if self.len_to_rib < len_pnl:
+                asp_lst.append(len_pnl/self.len_to_rib)
+                b_lst.append(self.len_to_rib)
+            else: 
+                asp_lst.append(self.len_to_rib/len_pnl)
+                b_lst.append(len_pnl)
+
+        asp_lst = np.array(asp_lst)
+        b_lst = np.array(b_lst)
+
+        # Compute the shear buckling coefficient using poly fit described in the docstring
+        kb_vec: np.ndarray =  self._kb_interp(asp_lst)
+
+        res = kb_vec* np.pi ** 2 * self.material_struct.young_modulus/(12*(1 - self.material_struct.poisson**2)) * (t_arr/ b_lst)**2
+        return res
+
+    # def flange_buckling(t_st, w_st):#TODO
+    #     buck = 2 * np.pi ** 2 * material_struct.young_modulus / (12 * (1 - material_struct.poisson ** 2)) * (t_st / w_st) ** 2
+    #     return buck
+
+
+    # def web_buckling(t_st, h_st):#TODO
+    #     buck = 4 * np.pi ** 2 *material.young_modulus / (12 * (1 -material.poisson ** 2)) * (t_st / h_st) ** 2
+    #     return buck0
+
+
+    # def global_buckling( h_st, t_st, t):#TODO
+    #     # n = n_st(c_r, b_st)
+    #     tsmr = (t *pitch_str + t_st *wing.n_str * (h_st - t)) /pitch_str
+    #     return 4 * np.pi ** 2 * self.material.young_modulus / (12 * (1 - self.material.poisson ** 2)) * (tsmr / self.pitch_str) ** 2
+
+
+    # def shear_buckling(self,t_sk):#TODO
+    #     buck = 5.35 * pi ** 2 * self.material.young_modulus / (12 * (1 - self.material.poisson)) * (t_sk / self.pitch_str) ** 2
+    #     return buck
+
+
+
+    def interaction_curve(self):
+        r""" The following function ensures the panel remains below the interaction curve of a composite panel
+        under combined compression and shear forces. This function is designed to be used with the :func:`SectionOptimization._get_constraint_vector` however it
+        can also be used to check this specific constraints for any given design. The following equation is used for the 
+        interaction curve which has been rewritten from equation 6.38, page 144 in source [1]:
+
+        .. math::
+            -\frac{N_x}{N_{x,crit}} - \left(\frac{N_{xy}}{N_{xy,crit}}\right) + 1 > 0
+
+
+
+        **Bibliography**
+        [1] Kassapoglou. Design and Analysis of Composite Structures. 2nd Edition. John Wiley & Sons Ltd, 2013.
+
+        :param wingbox: _description_
+        :type wingbox: IdealWingbox
+        :param material_struct: _description_
+        :type material_struct: Material
+        :param len_to_rib: _description_
+        :type len_to_rib: float
+        :return: _description_
+        :rtype: _type_
+        """    
+
+        
+        area_pnl: list = [pnl.t_pnl*pnl.length() for pnl in self.pnl_lst]
+        Nx_crit = self._crit_instability_compr()*area_pnl
+        Nxy_crit = self._crit_instability_shear()*area_pnl
+
+        Nx: list = np.abs([min(pnl.b1.sigma*pnl.b1.A, pnl.b2.sigma*pnl.b2.A) for pnl in self.pnl_lst]) # Take the maximum of the two booms
+        Nxy: list = np.abs([pnl.q_tot*pnl.length() for pnl in self.pnl_lst])
+
+        interaction_constr = -Nx/ Nx_crit - (Nxy/Nxy_crit) ** 2 + 1
+        interaction_constr[self.tens_pnl_idx] = 1
+
+
+        return interaction_constr
+
+
+    # def column_st(self, h_st, w_st, t_st, t_sk):#
+    #     #Lnew=new_L(b,L)
+    #     Ist = t_st * h_st ** 3 / 12 + (w_st - t_st) * t_st ** 3 / 12 + t_sk**3*w_st/12+t_sk*w_st*(0.5*h_st)**2
+    #     i= pi ** 2 * self.material.young_modulus * Ist / (2*w_st* self.rib_pitch ** 2)#TODO IF HE FAILS REPLACE SPAN WITH RIB PITCH
+    #     return i
+
+
+    # def f_ult(self, h_st,w_st,t_st,t_sk,y):#TODO
+    #     A_st = self.get_area_str(h_st,w_st,t_st)
+    #     # n=n_st(c_r,b_st)
+    #     A=self.wing.n_str*A_st+self.width_wingbox*self.chord(y)*t_sk
+    #     f_uts=self.sigma_uts*A
+    #     return f_uts
+
+
+    # def buckling_constr(self, x):
+    #     buck = self.buckling(x)
+    #     return -1*(buck - 1)
+
+
+    # def global_local(self, x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     glob = self.global_buckling(h_st, t_st, t_sk)
+    #     loc = self.local_buckling(t_sk)
+    #     diff = glob - loc
+    #     return diff
+
+
+    # def local_column(self, x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     col = self.column_st(h_st,w_st,t_st, t_sk)
+    #     loc = self.local_buckling(t_sk)
+    #     # print("col=",col/1e6)
+    #     # print("loc=",loc/1e6)
+    #     diff = col - loc
+    #     return diff
+
+
+    # def flange_loc_loc(self, x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     flange = self.flange_buckling(t_st,w_st)
+    #     loc = self.local_buckling(t_sk)
+    #     diff = flange - loc
+    #     return diff
+
+
+    # def web_flange(self, x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     web = self.web_buckling(t_st, h_st)
+    #     loc = self.local_buckling(t_sk)
+    #     diff =web-loc
+    #     return diff
+
+
+    def von_Mises(self):
+        r""" THe following constraint implemetns the von mises failure criterion which is defined as follows for the case where only a direct stress
+        in the y axis occurs and one shear stress is present.
+
+        .. math::
+             \sigma_y & \geq  \sigma_v \\
+              \sigma_y  - \sqrt{\sigma_{11}^2 + 3\tau^2} & \geq  0 \\
+
+
+        :return: _description_
+        :rtype: _type_
+        """        
+
+        shear_arr = np.array([i.tau for i in  self.pnl_lst])
+        direct_stress_arr = np.array([(i.b1.sigma + i.b2.sigma)/2 for i in  self.pnl_lst])
+        return self.material_struct.sigma_yield - np.sqrt(direct_stress_arr**2 + 3*shear_arr**2)
+
+
+    # def crippling(self, x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     A = self.get_area_str(h_st,w_st,t_st)
+    #     col = self.column_st( h_st,w_st,t_st,t_sk)
+    #     crip = t_st * self.material.beta_crippling * self.material.sigma_yield* ((self.material.g_crippling * t_st ** 2 / A) * np.sqrt(self.material.young_modulus / self.material.sigma_yield)) ** self.m_crip
+    #     return crip
+
+    # #----OWN CONSTRAINTS-----
+    # def str_buckling_constr(self,x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     Ist = t_st * h_st ** 3 / 12 + (w_st - t_st) * t_st ** 3 / 12 + t_sk**3*w_st/12+t_sk*w_st*(0.5*h_st)**2
+    #     i= pi ** 2 * self.material.young_modulus * Ist / (self.rib_pitch ** 2)#TODO IF HE FAILS REPLACE SPAN WITH RIB PITCH
+    #     i_sigma = (i/self.get_area_str(h_st,w_st,t_st))#convert to stress
+    #     return -1*(self.material.safety_factor*self.bending_stress_y_from_tip(x)/(i_sigma) - 1)
+
+    # def f_ult_constr(self,x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     return -1*(self.material.safety_factor*self.bending_stress_y_from_tip(x)/self.material.sigma_ultimate - 1)
+    # def flange_buckling_constr(self,x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     return -1*(self.material.safety_factor*self.bending_stress_y_from_tip(x)/self.flange_buckling(t_st,w_st) - 1)
+
+    # def web_buckling_constr(self,x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     return -1*(self.material.safety_factor*self.bending_stress_y_from_tip(x)/self.web_buckling(t_st,h_st) - 1)
+
+    # def global_buckling_constr(self,x):
+    #     t_sp, h_st, w_st, t_st, t_sk = x
+    #     return -1*(self.material.safety_factor*self.bending_stress_y_from_tip(x)/self.global_buckling(h_st,t_st,t_sk) - 1)
+
+ 
+
+
 
 def class2_wing_mass(vtol, flight_perf, wing ):
         """ Returns the structural weight of both wings 
 
         :param vtol: VTOL data structure
         :type vtol: VTOL
         :param flight_perf: FlightPerformance data structure
```

## tuduam/version.py

```diff
@@ -1 +1 @@
-__version__ = "2024.8"
+__version__ = "2024.9"
```

## Comparing `tuduam-2024.8.data/data/LICENSE` & `tuduam-2024.9.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `tuduam-2024.8.data/data/README.md` & `tuduam-2024.9.data/data/README.md`

 * *Files identical despite different names*

## Comparing `tuduam-2024.8.dist-info/LICENSE` & `tuduam-2024.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tuduam-2024.8.dist-info/METADATA` & `tuduam-2024.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuduam
-Version: 2024.8
+Version: 2024.9
 Summary: Python module related to the course on Urban Air Mobility at the faculty of Aeropsace Engineering, TU Delft
 Home-page: https://github.com/saullocastro/tuduam
 Author: Saullo G. P. Castro, Damien Keijzer
 Author-email: S.G.P.Castro@tudelft.nl
 License: 3-Clause BSD
 Keywords: eVTOL design
 Classifier: Development Status :: 1 - Planning
```

## Comparing `tuduam-2024.8.dist-info/RECORD` & `tuduam-2024.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 tuduam/__init__.py,sha256=Fy4no3CeW2pJ6bbZTORiyBG5_exr7AzzOQJt1ogVw7I,262
 tuduam/aerodynamics.py,sha256=ad00L6DKI9Z7f5cbC096gGAEZLByQO_tdIE47oOkeYk,12019
-tuduam/data_structures.py,sha256=heDHhukzmfVgMcvFetahlmOyq6iPBKFor0Ot58iZHDA,6696
+tuduam/data_structures.py,sha256=MKM1Lxpg5jYwhlnd9i6s9x1fsdGxcKGEYnu4d62LXlw,6692
 tuduam/performance.py,sha256=l3Nt8WJcdDdb6lr8INcRnnYdiQD1ZAjbc0RoCEprte0,2434
-tuduam/propulsion.py,sha256=6RPMhkCiuXPf1VeLdgfboyg7nwxd3-OqhhRJSiMJdek,42292
+tuduam/propulsion.py,sha256=nKn_DjrbYpL_D02MZVilTTh8Zjnh0dO79tcAHPU02IM,42608
 tuduam/sim_ctrl.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tuduam/structures.py,sha256=o9qq8R0HYYqAmYzo-02fnYXSPlGfEiLtFkRtH2jP2ls,51051
-tuduam/version.py,sha256=gG0-bMJjTIpymOBuckmceGCbMzCMxGOAWi7qDm4CRXQ,23
-tuduam-2024.8.data/data/LICENSE,sha256=XkhI_IVX8YUvsk_QQq2CRhL69BLVH5KXYG1Zfr2RFR8,1548
-tuduam-2024.8.data/data/README.md,sha256=UQYWheb4XnKKFNENoCO9qbESgH5Pjm0s8Y26vA8MmrY,783
-tuduam-2024.8.dist-info/LICENSE,sha256=XkhI_IVX8YUvsk_QQq2CRhL69BLVH5KXYG1Zfr2RFR8,1548
-tuduam-2024.8.dist-info/METADATA,sha256=fflbcx3PdxIqyWZlVuJojhsMR4dD_qH8InZqykCz2QA,2085
-tuduam-2024.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-tuduam-2024.8.dist-info/top_level.txt,sha256=0Yb2AC_j5u9HlDnp0wIL_EVFKvGJKuj_K5v_xzkDiAs,7
-tuduam-2024.8.dist-info/RECORD,,
+tuduam/structures.py,sha256=nfLLvd70b9Nx6vyHxbbHaWeGsp72Erdzg0I4dbeAYSQ,85384
+tuduam/version.py,sha256=3qebckGu0HHMiTghIrnH1iuqvQpjA-5FcHHZflj4ih0,23
+tuduam-2024.9.data/data/LICENSE,sha256=XkhI_IVX8YUvsk_QQq2CRhL69BLVH5KXYG1Zfr2RFR8,1548
+tuduam-2024.9.data/data/README.md,sha256=UQYWheb4XnKKFNENoCO9qbESgH5Pjm0s8Y26vA8MmrY,783
+tuduam-2024.9.dist-info/LICENSE,sha256=XkhI_IVX8YUvsk_QQq2CRhL69BLVH5KXYG1Zfr2RFR8,1548
+tuduam-2024.9.dist-info/METADATA,sha256=rRtnQnsn3tfrIdPz69TliiKtbKJh_2D3Oq1cVO97FtU,2085
+tuduam-2024.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tuduam-2024.9.dist-info/top_level.txt,sha256=0Yb2AC_j5u9HlDnp0wIL_EVFKvGJKuj_K5v_xzkDiAs,7
+tuduam-2024.9.dist-info/RECORD,,
```

