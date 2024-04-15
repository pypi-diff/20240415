# Comparing `tmp/diffCheck-0.0.7.tar.gz` & `tmp/diffCheck-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffCheck-0.0.7.tar", last modified: Fri Apr 12 15:03:04 2024, max compression
+gzip compressed data, was "diffCheck-0.0.8.tar", last modified: Mon Apr 15 09:10:11 2024, max compression
```

## Comparing `diffCheck-0.0.7.tar` & `diffCheck-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 15:03:04.495732 diffCheck-0.0.7/
--rw-rw-rw-   0        0        0      806 2024-04-12 15:03:04.495224 diffCheck-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 15:03:04.477727 diffCheck-0.0.7/diffCheck/
--rw-rw-rw-   0        0        0      142 2024-04-12 15:02:55.000000 diffCheck-0.0.7/diffCheck/__init__.py
--rw-rw-rw-   0        0        0     9504 2024-04-12 08:02:49.000000 diffCheck-0.0.7/diffCheck/df_geometries.py
--rw-rw-rw-   0        0        0     7812 2024-04-12 14:41:11.000000 diffCheck-0.0.7/diffCheck/df_joint_detector.py
--rw-rw-rw-   0        0        0     4604 2024-04-12 08:02:49.000000 diffCheck-0.0.7/diffCheck/df_transformations.py
--rw-rw-rw-   0        0        0     4166 2024-04-12 08:02:49.000000 diffCheck-0.0.7/diffCheck/df_util.py
-drwxrwxrwx   0        0        0        0 2024-04-12 15:03:04.493726 diffCheck-0.0.7/diffCheck.egg-info/
--rw-rw-rw-   0        0        0      806 2024-04-12 15:03:04.000000 diffCheck-0.0.7/diffCheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-04-12 15:03:04.000000 diffCheck-0.0.7/diffCheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 15:03:04.000000 diffCheck-0.0.7/diffCheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 15:03:04.000000 diffCheck-0.0.7/diffCheck.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 15:03:04.000000 diffCheck-0.0.7/diffCheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 15:03:04.495732 diffCheck-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      820 2024-04-12 15:02:55.000000 diffCheck-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:10:11.764436 diffCheck-0.0.8/
+-rw-rw-rw-   0        0        0      806 2024-04-15 09:10:11.763834 diffCheck-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 09:10:11.754010 diffCheck-0.0.8/diffCheck/
+-rw-rw-rw-   0        0        0       21 2024-04-15 09:09:27.000000 diffCheck-0.0.8/diffCheck/__init__.py
+-rw-rw-rw-   0        0        0     9419 2024-04-15 09:09:03.000000 diffCheck-0.0.8/diffCheck/df_geometries.py
+-rw-rw-rw-   0        0        0     7965 2024-04-15 09:09:08.000000 diffCheck-0.0.8/diffCheck/df_joint_detector.py
+-rw-rw-rw-   0        0        0     4700 2024-04-12 15:50:57.000000 diffCheck-0.0.8/diffCheck/df_transformations.py
+-rw-rw-rw-   0        0        0     4174 2024-04-12 15:49:55.000000 diffCheck-0.0.8/diffCheck/df_util.py
+-rw-rw-rw-   0        0        0      997 2024-04-15 09:07:29.000000 diffCheck-0.0.8/diffCheck/diffCheck_app.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:10:11.762274 diffCheck-0.0.8/diffCheck.egg-info/
+-rw-rw-rw-   0        0        0      806 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-15 09:10:11.000000 diffCheck-0.0.8/diffCheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 09:10:11.764971 diffCheck-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      824 2024-04-15 09:09:27.000000 diffCheck-0.0.8/setup.py
```

### Comparing `diffCheck-0.0.7/PKG-INFO` & `diffCheck-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.7
+Version: 0.0.8
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.7/diffCheck/df_geometries.py` & `diffCheck-0.0.8/diffCheck/df_geometries.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 
 
 @dataclass
 class DFVertex:
     """
     This class represents a vertex, a simple container with 3 coordinates
     """
-    x : float
-    y : float
-    z : float
+
+    x: float
+    y: float
+    z: float
+
     def __post_init__(self):
         self.x = self.x or 0.0
         self.y = self.y or 0.0
         self.z = self.z or 0.0
 
     def __repr__(self):
         return f"Vertex: X={self.x}, Y={self.y}, Z={self.z}"
@@ -57,54 +59,49 @@
 
 
 @dataclass
 class DFFace:
     """
     This class represents a face, in diffCheck, a face is a collection of vertices.
     """
+
     # just as breps a first outer loop and then inner loops of DFVertices
-    all_loops : typing.List[typing.List[DFVertex]]
-    joint_id : int
+    all_loops: typing.List[typing.List[DFVertex]]
+    joint_id: int = None
+
     def __post_init__(self):
         if len(self.all_loops[0]) < 3:
             raise ValueError("A face must have at least 3 vertices")
-        self.all_loops = self.all_loops or []
+        self.all_loops = self.all_loops
 
-        self.joint_id = self.joint_id or None
+        self.joint_id = self.joint_id
         self.__is_joint = False
         self.__id = uuid.uuid4().int
 
     def __repr__(self):
         return f"Face id: {len(self.id)}, IsJoint: {self.is_joint} Loops: {len(self.all_loops)}"
 
     def __hash__(self):
-        outer_loop = tuple(tuple(vertex.__dict__.values()) for vertex in self.all_loops[0])
-        inner_loops = tuple(tuple(vertex.__dict__.values()) for loop in self.all_loops[1:] for vertex in loop)
+        outer_loop = tuple(
+            tuple(vertex.__dict__.values()) for vertex in self.all_loops[0]
+        )
+        inner_loops = tuple(
+            tuple(vertex.__dict__.values())
+            for loop in self.all_loops[1:]
+            for vertex in loop
+        )
         return hash((outer_loop, inner_loops))
 
     def __eq__(self, other):
         if isinstance(other, DFFace):
             return self.all_loops == other.all_loops
         return False
 
-    @staticmethod
-    def compute_mass_center(face: rg.BrepFace) -> rg.Point3d:
-        """
-        Compute the mass center of a  face
-
-        :param face: The face to compute the mass center from
-        :return mass_center: The mass center of the face
-        """
-        amp = rg.AreaMassProperties.Compute(face)
-        if amp:
-            return amp.Centroid
-        return None
-
     @classmethod
-    def from_brep(cls, brep_face: rg.BrepFace, joint_id: int=None):
+    def from_brep(cls, brep_face: rg.BrepFace, joint_id: int = None):
         """
         Create a DFFace from a Rhino Brep face
 
         :param brep_face: The Rhino Brep face
         :param joint_id: The joint id
         :return face: The DFFace object
         """
@@ -131,20 +128,24 @@
         Convert the face to a Rhino Brep planar face
 
         :return brep_face: The Rhino Brep planar face
         """
         brep_curves = []
 
         for loop in self.all_loops:
-            inner_vertices = [rg.Point3d(vertex.x, vertex.y, vertex.z) for vertex in loop]
+            inner_vertices = [
+                rg.Point3d(vertex.x, vertex.y, vertex.z) for vertex in loop
+            ]
             inner_polyline = rg.Polyline(inner_vertices)
             inner_curve = inner_polyline.ToNurbsCurve()
             brep_curves.append(inner_curve)
 
-        brep = rg.Brep.CreatePlanarBreps(brep_curves, Rhino.RhinoDoc.ActiveDoc.ModelAbsoluteTolerance)[0]
+        brep = rg.Brep.CreatePlanarBreps(
+            brep_curves, Rhino.RhinoDoc.ActiveDoc.ModelAbsoluteTolerance
+        )[0]
 
         return brep
 
     def to_mesh(self):
         """
         Convert the face to a Rhino Mesh
 
@@ -167,32 +168,37 @@
 
 
 @dataclass
 class DFBeam:
     """
     This class represents a beam, in diffCheck, a beam is a collection of faces
     """
-    name : str
-    faces : typing.List[DFFace]
+
+    name: str
+    faces: typing.List[DFFace]
+
     def __post_init__(self):
         self.name = self.name or "Unnamed Beam"
         self.faces = self.faces or []
         self._joint_faces = []
         self._side_faces = []
 
         self.__id = uuid.uuid4().int
 
     @classmethod
     def from_brep(cls, brep):
         """
         Create a DFBeam from a RhinoBrep object.
         It also removes duplicates and creates a list of unique faces.
         """
-        faces = diffCheck.df_joint_detector.JointDetector(brep).run()
-        faces = list(set(faces))
+        faces : typing.List[DFFace] = []
+        data_faces = diffCheck.df_joint_detector.JointDetector(brep).run()
+        for data in data_faces:
+            face = DFFace.from_brep(data[0], data[1])
+            faces.append(face)
         beam = cls("Beam", faces)
         return beam
 
     def __repr__(self):
         return f"Beam: {self.name}, Faces: {len(self.faces)}"
 
     @property
@@ -209,16 +215,18 @@
 
 
 @dataclass
 class DFAssembly:
     """
     This class represents an assembly of beams
     """
-    beams : typing.List[DFBeam]
-    name : str
+
+    beams: typing.List[DFBeam]
+    name: str
+
     def __post_init__(self):
         self.beams = self.beams
         self.name = self.name or "Unnamed Assembly"
 
         self._all_jointfaces = []
         self._all_sidefaces = []
 
@@ -252,34 +260,36 @@
                 face_elem.set("is_joint", str(face.is_joint))
                 face_elem.set("joint_id", str(face.joint_id))
                 # export linked mesh
                 facerhmesh_elem = ET.SubElement(face_elem, "RhMesh")
                 mesh = face.to_mesh()
                 mesh_vertices = mesh.Vertices
                 for idx, vertex in enumerate(mesh_vertices):
-                    facerhmesh_vertex_elem = ET.SubElement(facerhmesh_elem, "RhMeshVertex")
+                    facerhmesh_vertex_elem = ET.SubElement(
+                        facerhmesh_elem, "RhMeshVertex"
+                    )
                     facerhmesh_vertex_elem.set("x", str(vertex.X))
                     facerhmesh_vertex_elem.set("y", str(vertex.Y))
                     facerhmesh_vertex_elem.set("z", str(vertex.Z))
                 mesh_faces = mesh.Faces
                 for idx, face in enumerate(mesh_faces):
                     facerhmesh_face_elem = ET.SubElement(facerhmesh_elem, "RhMeshFace")
                     facerhmesh_face_elem.set("v1", str(face.A))
                     facerhmesh_face_elem.set("v2", str(face.B))
                     facerhmesh_face_elem.set("v3", str(face.C))
                     facerhmesh_face_elem.set("v4", str(face.D))
 
         tree = ET.ElementTree(root)
-        xml_string = ET.tostring(root, encoding='unicode')
+        xml_string = ET.tostring(root, encoding="unicode")
         dom = parseString(xml_string)
         pretty_xml = dom.toprettyxml()
 
         return pretty_xml
 
-    def dump_xml(self, pretty_xml : str, dir: str):
+    def dump_xml(self, pretty_xml: str, dir: str):
         """
         Dump the pretty XML to a file
 
         :param pretty_xml: The pretty XML string
         :param dir: The directory to save the XML
         """
         timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
@@ -294,8 +304,8 @@
             self._all_jointfaces.extend(beam.joint_faces)
         return self._all_jointfaces
 
     @property
     def all_side_faces(self):
         for beam in self.beams:
             self._all_sidefaces.extend(beam.side_faces)
-        return self._all_sidefaces
+        return self._all_sidefaces
```

### Comparing `diffCheck-0.0.7/diffCheck/df_joint_detector.py` & `diffCheck-0.0.8/diffCheck/df_joint_detector.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,47 @@
 import Rhino.Geometry as rg
 
 import typing
 from dataclasses import dataclass
 
 import diffCheck.df_util
 import diffCheck.df_transformations
-import diffCheck.df_geometries
+
 
 @dataclass
-class JointDetector():
+class JointDetector:
     """
     This class is responsible for detecting joints in a brep
     """
     brep : Rhino.Geometry.Brep
     def __post_init__(self):
         self.brep = self.brep or None
         # list of straight cuts
         self._cuts : typing.List[rg.Brep] = []
         # list of holes
         self._holes : typing.List[rg.Brep] = []
         # list of mixed joints (cuts+holes)
         self._mix : typing.List[rg.Brep]= []
 
         # list of DFFaces from joints and sides
-        self._faces : typing.List[diffCheck.df_geometries.DFFace] = []
+        self._faces = []
+
+    def _compute_mass_center(self, b_face: rg.BrepFace) -> rg.Point3d:
+        """
+        Compute the mass center of a brep face
+
+        :param b_face: The brep face to compute the mass center from
+        :return mass_center: The mass center of the brep face
+        """
+        amp = rg.AreaMassProperties.Compute(b_face)
+        if amp:
+            return amp.Centroid
+        return None
 
-    def run(self) -> typing.List[diffCheck.df_geometries.DFFace]:
+    def run(self) :
         """
             Run the joint detector
 
             :return: a list of faces from joins and faces
         """
         ############################################################################
         # 1. Bring to XY, mamke AABB and get negative boolean difference
@@ -160,27 +172,27 @@
 
         # get all the medians of the faces of cuts only
         cuts_faces_centroids : typing.Dict[int, typing.List[rg.Point3d]] = {}
         for idx, b in enumerate(self._cuts):
             idx = idx + 1
             temp_face_centroids = []
             for f in b.Faces:
-                centroid = diffCheck.df_geometries.DFFace.compute_mass_center(f)
+                centroid = self._compute_mass_center(f)
                 temp_face_centroids.append(centroid)
             cuts_faces_centroids[idx] = temp_face_centroids
 
         # compare with the brep medians faces to get the joint/sides's faces
         for f in self.brep.Faces:
-            centroid_2test = diffCheck.df_geometries.DFFace.compute_mass_center(f)
+            centroid_2test = self._compute_mass_center(f)
             for key, centroids in cuts_faces_centroids.items():
                 is_joint = False
                 for centroid in centroids:
                     if centroid_2test.DistanceTo(centroid) < sc.doc.ModelAbsoluteTolerance:
-                        self._faces.append(diffCheck.df_geometries.DFFace.from_brep(f, key))
+                        self._faces.append([f, key])
                         is_joint = True
                         break
                 if is_joint:
                     break
             if not is_joint:
-                self._faces.append(diffCheck.df_geometries.DFFace.from_brep(f, None))
+                self._faces.append([f, None])
 
         return self._faces
```

### Comparing `diffCheck-0.0.7/diffCheck/df_transformations.py` & `diffCheck-0.0.8/diffCheck/df_transformations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 import Rhino
 import Rhino.Geometry as rg
 import scriptcontext as sc
 
 import numpy as np
 
-def get_inverse_transformation(x_form : Rhino.Geometry.Transform) -> Rhino.Geometry.Transform:
+
+def get_inverse_transformation(
+    x_form: Rhino.Geometry.Transform,
+) -> Rhino.Geometry.Transform:
     """
         Get the inverse of a transformation
         
         :param x_form: the transformation to get the inverse from
         :return: the inverse transformation
     """
-    transformation_matrix = np.array([
-        [x_form.M00, x_form.M01, x_form.M02, x_form.M03],
-        [x_form.M10, x_form.M11, x_form.M12, x_form.M13],
-        [x_form.M20, x_form.M21, x_form.M22, x_form.M23],
-        [x_form.M30, x_form.M31, x_form.M32, x_form.M33]
-    ])
+    transformation_matrix = np.array(
+        [
+            [x_form.M00, x_form.M01, x_form.M02, x_form.M03],
+            [x_form.M10, x_form.M11, x_form.M12, x_form.M13],
+            [x_form.M20, x_form.M21, x_form.M22, x_form.M23],
+            [x_form.M30, x_form.M31, x_form.M32, x_form.M33],
+        ]
+    )
     inverse_transformation_matrix = np.linalg.inv(transformation_matrix)
 
     x_form_back = Rhino.Geometry.Transform()
     for i in range(4):
         for j in range(4):
             x_form_back[i, j] = inverse_transformation_matrix[i, j]
 
     return x_form_back
 
-def pln_2_pln_world_transform(brep : Rhino.Geometry.Brep) -> Rhino.Geometry.Transform:
+
+def pln_2_pln_world_transform(brep: Rhino.Geometry.Brep) -> Rhino.Geometry.Transform:
     """
         Transform a brep (beam) to the world plane
         
         :param brep: the brep to transform
         :return: the transformation
     """
+
     def _get_lowest_brep_vertex(brep) -> Rhino.Geometry.Point3d:
         """
             Get the the vertex with the lowest y,x and z values
             
             :param brep: the brep to get the lowest vertex from
             :return: the lowest vertex
         """
@@ -67,15 +74,15 @@
     faces = [brep.Faces[face_index] for face_index in face_indices]
     biggest_face = None
     biggest_face_area = 0
     for face in faces:
         if rg.AreaMassProperties.Compute(face).Area > biggest_face_area:
             biggest_face_area = rg.AreaMassProperties.Compute(face).Area
             biggest_face = face
-    
+
     # get the plane of the biggest face
     if biggest_face.TryGetPlane()[0] is False:
         log.error("Could not find plane for longest edge. Exiting...")
         return
     plane_src = biggest_face.TryGetPlane()[1]
     plane_tgt = Rhino.Geometry.Plane.WorldXY
     print("Found plane for longest edge: " + str(plane_src))
@@ -101,23 +108,27 @@
     # check if a 90 deg rotation is needed (for the joint detector)
     x_form_transl_B = None
     x_form_rot90z = None
     if x_val_sum > y_val_sum:
         print("Bounding box is alligned to x axis. No rotation needed.")
     else:
         print("Bounding box is not alligned to y axis. A 90 deg rotation is needed.")
-        x_form_rot90z = Rhino.Geometry.Transform.Rotation(math.radians(90), rg.Vector3d.ZAxis, rg.Point3d.Origin)
+        x_form_rot90z = Rhino.Geometry.Transform.Rotation(
+            math.radians(90), rg.Vector3d.ZAxis, rg.Point3d.Origin
+        )
         brep.Transform(x_form_rot90z)
         lowest_vertex = _get_lowest_brep_vertex(brep)
 
-        x_form_transl_B = Rhino.Geometry.Transform.Translation(rg.Vector3d(-lowest_vertex))
+        x_form_transl_B = Rhino.Geometry.Transform.Translation(
+            rg.Vector3d(-lowest_vertex)
+        )
         brep.Transform(x_form_transl_B)
 
     # resume the transformations in one
     x_form = Rhino.Geometry.Transform.Identity
     if x_form_transl_B:
         Rhino.Geometry.Transform.TryGetInverse(x_form_transl_B)
         Rhino.Geometry.Transform.TryGetInverse(x_form_rot90z)
         x_form = x_form_transl_B * x_form_rot90z
     x_form = x_form * x_form_transl_A * x_form_pln2pln
 
-    return x_form
+    return x_form
```

### Comparing `diffCheck-0.0.7/diffCheck/df_util.py` & `diffCheck-0.0.8/diffCheck/df_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,23 @@
     else:
         for face in brep.Faces:
             face_brep = face.DuplicateFace(False)
             if face_brep:
                 exploded_objects.append(face_brep)
     return exploded_objects
 
+
 def get_crv_circle_center(crv) -> rg.Point3d:
     """ Get the center of a circle """
     bbox = crv.GetBoundingBox(True)
     bbox_b = bbox.ToBrep()
     center_point = bbox_b.GetBoundingBox(True).Center
     return center_point
 
+
 def is_pt_unique_in_dict(pt, pt_dict) -> bool:
     """
         Detect if the point exists in the dictionary, and if so, return the index
 
         :param pt: the point to check
         :param pt_dict: the dictionary to check
         :return: True if the point is unique, False otherwise
@@ -47,14 +49,15 @@
         Z_b = round(pt_dict.Z, 3)
 
         if X_a == X_b and Y_a == Y_b and Z_a == Z_b:
             is_unique = False
             break
     return is_unique
 
+
 def is_pt_unique_in_list(pt, list) -> bool:
     """
         Detect if the point exists in the list, and if so, return the index
 
         :param pt: the point to check
         :param list: the list to check
         :return: True if the point is unique, False otherwise
@@ -70,14 +73,15 @@
         Z_b = round(pt_list.Z, 3)
 
         if X_a == X_b and Y_a == Y_b and Z_a == Z_b:
             is_unique = False
             break
     return is_unique
 
+
 def detect_idx_pt_in_list(pt, list) -> int:
     """
         Detect the index of a point in a list
 
         :param pt: the point to check
         :param list: the list to check
         :return: the index of the point in the list
@@ -93,14 +97,15 @@
         Y_b = round(pt_list.Y, 3)
         Z_b = round(pt_list.Z, 3)
 
         if X_a == X_b and Y_a == Y_b and Z_a == Z_b:
             return idx
     return idx
 
+
 def compute_ordered_vertices(brep_face) -> typing.List[Rhino.Geometry.Point3d]:
     """ Retrieve the ordered vertices of a brep face """
     sorted_vertices = []
 
     edges = brep_face.DuplicateEdgeCurves()
     edges = list(set(edges))
 
@@ -123,12 +128,12 @@
                     edges_sorted.append(edge)
                     edges.pop(edges.index(edge))
                     break
                 elif edges_sorted[-1].PointAtEnd == edge.PointAtEnd:
                     edges_sorted.append(edge)
                     edges.pop(edges.index(edge))
                     break
-    
+
     for edge in edges_sorted:
         sorted_vertices.append(edge.PointAtStart)
 
-    return sorted_vertices
+    return sorted_vertices
```

### Comparing `diffCheck-0.0.7/diffCheck.egg-info/PKG-INFO` & `diffCheck-0.0.8/diffCheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.7
+Version: 0.0.8
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

