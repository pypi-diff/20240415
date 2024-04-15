# Comparing `tmp/eyegestures-1.3.3.tar.gz` & `tmp/eyegestures-1.3.4.tar.gz`

## Comparing `eyegestures-1.3.3.tar` & `eyegestures-1.3.4.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/Fixation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/calibration.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/eye.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/eyegestures.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/face.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/gazeContexter.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/gazeEstimator.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/gevent.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/nose.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/processing.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/pupil.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/scalling_test.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/screenTracker_test.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/utils.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/screenTracker/clusters.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/screenTracker/dataPoints.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/screenTracker/heatmap.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 eyegestures-1.3.3/eyeGestures/screenTracker/screenTracker.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 eyegestures-1.3.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eyegestures-1.3.3/LICENSE
--rw-r--r--   0        0        0     9866 2020-02-02 00:00:00.000000 eyegestures-1.3.3/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 eyegestures-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    51138 2020-02-02 00:00:00.000000 eyegestures-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/Fixation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/__init__.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/calibration.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/eye.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/eyegestures.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/face.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/gazeContexter.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/gazeEstimator.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/gevent.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/processing.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/scalling_test.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker_test.py
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/utils.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/clusters.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/dataPoints.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/heatmap.py
+-rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 eyegestures-1.3.4/eyeGestures/screenTracker/screenTracker.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 eyegestures-1.3.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 eyegestures-1.3.4/LICENSE
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 eyegestures-1.3.4/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 eyegestures-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0    51549 2020-02-02 00:00:00.000000 eyegestures-1.3.4/PKG-INFO
```

### Comparing `eyegestures-1.3.3/eyeGestures/calibration.py` & `eyegestures-1.3.4/eyeGestures/screenTracker/dataPoints.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,62 @@
-
-import time 
 import math
 import numpy as np
-from sklearn.model_selection import train_test_split
-from sklearn.linear_model import LinearRegression
-from sklearn.metrics import mean_squared_error, r2_score
 
-class Calibrator:
+from scipy import signal
+
+class Center():
+    """Helper representing Center of object with x,y,width,height"""
+
+    def __init__(self,x,y,width,height):
+        self.x = (x + width)/2
+        self.y = (y + height)/2
+
+class Screen():
+    """Helper representing screen by making box of width,height"""
 
-    def __init__(self,width,height,time = 60):
+    def __init__(self,width,height):
+        self.x = 0
+        self.y = 0
         self.width = width
-        self.height = height
-        self.time = time
+        self.height= height
+
+    def getCenter(self):
+        """Function returnig center of the screen"""
+        return Center(self.x,self.y,self.width, self.height)
+
+class ScreenROI():
+    """Helper representing ROI by making box of width,height with x and y offset"""
+
+    def __init__(self,x,y,width,height):
+        self.x = x 
+        self.y = y
+        self.width = width
+        self.height= height
 
-        self.run = False
-        self.t_start = 0
+    def setCenter(self,x, y):
+        """Function allowing to move ROI by changing its center"""
+        self.x = x - self.width/2
+        self.y = y - self.height/2
 
-        self.onFinish = None
+    def getCenter(self):
+        """Function returnig center of the ROI"""
+        return Center(self.x, self.y, self.width, self.height)
+
+    def getBoundaries(self):
+        """Function returnig boundaries of the ROI"""
+        return (self.x,self.y,self.width, self.height)
+
+
+class Display():
+    """Helper representing Display by making box of width,height with x and y offset"""
+
+    def __init__(self,width,height,offset_x,offset_y):
+        self.width = width
+        self.height = height
+        self.offset_x = offset_x
+        self.offset_y = offset_y
 
-    def start(self,onFinish):
-        self.t_start = time.time()
-        self.run = True
-
-        self.onFinish = onFinish
-
-    def getTrainingPoint(self):
-
-        if not self.run:
-            return self.points[0]
-        
-        else:
-            time_step = self.time/len(self.points)
-            index = int((time.time() - self.t_start)/time_step) * ((time.time() - self.t_start) > 0)
-            
-            if(index < 0 or index >= len(self.points)):
-                self.run = False
-
-                if not self.onFinish is None:
-                    self.onFinish()
-                    return self.points[0]
-                
-            return self.points[index]
+        # self.buffor = Buffor(20)
 
-    def inProgress(self):
-        return self.run 
+    def getCenter(self):
+        """Function returnig center of the Display"""
+        return self.__center
```

### Comparing `eyegestures-1.3.3/eyeGestures/eye.py` & `eyegestures-1.3.4/eyeGestures/eye.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,180 +1,177 @@
+"""Module providing a extraction of eye from face object."""
+
 import cv2
-import math
 import numpy as np
 import mediapipe as mp
-import eyeGestures.pupil as pupil
-from scipy.optimize import fsolve
-from eyeGestures.utils import Buffor
-
-# Function to fit a quadratic curve and find intersections
-def fit_curve(p1, p2):
-    # Fit a quadratic curve (ax^2 + bx + c) through the points
-    coefficients = np.polyfit([p1[0], p2[0]], [p1[1], p2[1]], 2)
-    curve = np.poly1d(coefficients)
-
-    return curve
-
-# Function to find intersections with y = 0
-def find_intersections(curve, points):
-    def intersection(x):
-        return curve(x)
-
-    intersection_points = fsolve(intersection, 0)
-    return (intersection_points,0)
-
-def getCurves(points, reference_point):
-    segments = []
-    intersection_points = []
-    for i in range(len(points)):
-        p1, p2 = points[i], points[(i + 1 ) % len(points)]
-        if (p1[1] - reference_point) * (p2[1] - reference_point) < 0:
-            curve = fit_curve(p1, p2)
-            
-            segment_x_range = np.linspace(p1[0], p2[0], 100)
-            segments.append((curve,segment_x_range))
-            x = find_intersections(curve,np.array([p1, p2]))
-            intersection_points.append(x)
-
-    return segments,intersection_points
-
-def getIntersections(points, reference_point):
-    _, intersetions = getCurves(points, reference_point)
-    return np.array(intersetions)
-
-class Eye:    
-    LEFT_EYE_KEYPOINTS  = np.array(list(mp.solutions.face_mesh.FACEMESH_LEFT_EYE))[:,0]
-    RIGHT_EYE_KEYPOINTS = np.array(list(mp.solutions.face_mesh.FACEMESH_RIGHT_EYE))[:,0]
-    LEFT_EYE_IRIS_KEYPOINT  = []
+
+
+class Eye:
+    """Class storing data related and representing a eye"""
+    LEFT_EYE_KEYPOINTS = np.array(
+        list(mp.solutions.face_mesh.FACEMESH_LEFT_EYE))[:, 0]
+    RIGHT_EYE_KEYPOINTS = np.array(
+        list(mp.solutions.face_mesh.FACEMESH_RIGHT_EYE))[:, 0]
+    LEFT_EYE_IRIS_KEYPOINT = []
     RIGHT_EYE_IRIS_KEYPOINT = []
-    LEFT_EYE_PUPIL_KEYPOINT  = [473]
+    LEFT_EYE_PUPIL_KEYPOINT = [473]
     RIGHT_EYE_PUPIL_KEYPOINT = [468]
-        
+
     # LEFT_EYE_KEYPOINTS = [36, 37, 38, 39, 40, 41] # keypoint indices for left eye
     # RIGHT_EYE_KEYPOINTS = [42, 43, 44, 45, 46, 47] # keypoint indices for right eye
 
-    scale = (150,100)
+    scale = (150, 100)
+
+    def __init__(self, side: int):
 
-    def __init__(self, side : int):
-        
         # check if eye is left or right
         if side == 1:
             self.side = "right"
             self.pupil_index = self.RIGHT_EYE_PUPIL_KEYPOINT
         elif side == 0:
             self.side = "left"
             self.pupil_index = self.LEFT_EYE_PUPIL_KEYPOINT
-        
+
+        self.x = 0
+        self.y = 0
+        self.width = 0
+        self.height = 0
+        self.center_x = 0
+        self.center_y = 0
+        self.image = None
+        self.pupil = None
+        self.offset = None
+        self.region = None
+        self.cut_image = None
+        self.landmarks = None
+
         # self._process(self.image,self.region)
 
-    def update(self,image : np.ndarray, landmarks : list, offset : np.ndarray):
+    def update(self, image: np.ndarray, landmarks: list, offset: np.ndarray):
+        """function updating data stored inside eye object"""
+
         self.image = image
         self.offset = offset
         self.landmarks = landmarks
 
         # check if eye is left or right
         if self.side == "right":
-            self.region = np.array(landmarks[self.RIGHT_EYE_KEYPOINTS], dtype=np.int32)
-        
+            self.region = np.array(
+                landmarks[self.RIGHT_EYE_KEYPOINTS], dtype=np.int32)
+
         elif self.side == "left":
-            self.region = np.array(landmarks[self.LEFT_EYE_KEYPOINTS], dtype=np.int32)
-        
+            self.region = np.array(
+                landmarks[self.LEFT_EYE_KEYPOINTS], dtype=np.int32)
+
         self.pupil = landmarks[self.pupil_index][0]
-        self._process(self.image,self.region)
+        self._process(self.image, self.region)
 
     def getCenter(self):
-        return (self.center_x,self.center_y)
+        """function returning center of eye"""
+
+        return (self.center_x, self.center_y)
 
     def getPos(self):
-        return (self.x,self.y)
+        """function returning position of eye in the image"""
+
+        return (self.x, self.y)
 
     def getPupil(self):
+        """function returning pupil object"""
+
         # return self.pupil.getCoords()
         return self.pupil
-    
+
     def getBlink(self):
+        """function returning blink event"""
         # return self.pupil.getCoords()
-        return (self.height) <= 3 # 2x margin 
+        return (self.height) <= 3  # 2x margin
 
     def getImage(self):
+        """function returning image of the eye cut from the entire face image"""
+
         # TODO: draw additional parameters
         return self.cut_image
 
-    def getGaze(self,gaze_buffor,y_correction=0,x_correction=0):
+    def getGaze(self, gaze_buffor, y_correction=0, x_correction=0):
+        """function returning gaze position"""
+
         # pupilCoords = self.pupil.getCoords()
-        center = np.array((self.center_x,self.center_y)) - self.offset
-        
+        center = np.array((self.center_x, self.center_y)) - self.offset
+
         region_corrected = self.region - self.offset
         pupil_corrected = self.pupil - self.offset
 
-        vectors = region_corrected  - center
+        vectors = region_corrected - center
         pupil = pupil_corrected - center
-        
+
         vectors = vectors - pupil
         gaze_vector = np.zeros((2))
-        
+
         gaze_vector[1] = np.sum(vectors, axis=0)[1] * 10 - y_correction
         gaze_vector[0] = -np.sum(vectors, axis=0)[0] * 10 - x_correction
-        
+
         # print("gaze_vector: ",gaze_vector)
-        gaze_buffor.add(gaze_vector)   
+        gaze_buffor.add(gaze_vector)
         return gaze_buffor.getAvg()
-        
+
     def getOpenness(self):
-        return self.height/2 
+        """function returning eye openness"""
+
+        return self.height/2
 
     def getLandmarks(self):
-        return self.region 
+        """function returning eye landmarks"""
 
-    def _process(self,image,region):
+        return self.region
+
+    def _process(self, image, region):
         h, w, _ = image.shape
 
-        mask = np.full((h, w), 0, dtype=np.uint8) 
+        mask = np.full((h, w), 0, dtype=np.uint8)
         background = np.zeros((h, w), dtype=np.uint8)
         cv2.fillPoly(mask, [region], 0)
 
-        masked_image = cv2.bitwise_not(background, cv2.cvtColor(image.copy(), cv2.COLOR_BGR2GRAY), mask=mask)
-        
+        masked_image = cv2.bitwise_not(background, cv2.cvtColor(
+            image.copy(), cv2.COLOR_BGR2GRAY), mask=mask)
+
         margin = 2
-        min_x = np.min(region[:,0]) - margin
-        max_x = np.max(region[:,0]) + margin
-        min_y = np.min(region[:,1]) - margin
-        max_y = np.max(region[:,1]) + margin
-        
+        min_x = np.min(region[:, 0]) - margin
+        max_x = np.max(region[:, 0]) + margin
+        min_y = np.min(region[:, 1]) - margin
+        max_y = np.max(region[:, 1]) + margin
+
         self.x = min_x
         self.y = min_y
-        
-        self.width  = np.max(region[:,0]) - np.min(region[:,0])
-        self.height = np.max(region[:,1]) - np.min(region[:,1])
-        
+
+        self.width = np.max(region[:, 0]) - np.min(region[:, 0])
+        self.height = np.max(region[:, 1]) - np.min(region[:, 1])
+
         self.center_x = (min_x + max_x)/2
         self.center_y = (min_y + max_y)/2
 
-        # HACKETY_HACK: 
-        self.pupil[1] = np.min(region[:,1])
-    
-        # self.intersection = getIntersections(region,self.center_y)
-        self.cut_image = masked_image[min_y:max_y,min_x:max_x]
+        # HACKETY_HACK:
+        self.pupil[1] = np.min(region[:, 1])
+
+        self.cut_image = masked_image[min_y:max_y, min_x:max_x]
         # print(f"here: {self.cut_image.shape,min_y,max_y,min_x,max_x}")
         self.cut_image = cv2.cvtColor(self.cut_image, cv2.COLOR_GRAY2BGR)
-        
+
         for point in self.region:
-            point = point - (min_x,min_y)
-            cv2.circle(self.cut_image,point.astype(int),1,(255,0,0,150),1)
+            point = point - (min_x, min_y)
+            cv2.circle(self.cut_image, point.astype(
+                int), 1, (255, 0, 0, 150), 1)
 
-        pupil = self.pupil - (min_x,min_y)
+        pupil = self.pupil - (min_x, min_y)
 
         # print(f"pupil: {pupil}")
-        cv2.circle(self.cut_image,pupil.astype(int),1,(0,255,0,150),1)
+        cv2.circle(self.cut_image, pupil.astype(int), 1, (0, 255, 0, 150), 1)
+
+        self.cut_image = cv2.resize(self.cut_image, self.scale)
 
-        self.cut_image = cv2.resize(self.cut_image,self.scale)
-        
-        # save cut_image to buffor and get avg from previous buffors 
+        # save cut_image to buffor and get avg from previous buffors
         # self.eyeBuffer.add(self.cut_image)
-        # self.cut_image = np.array(self.eyeBuffer.getAvg(), dtype=np.uint8) 
-            
+        # self.cut_image = np.array(self.eyeBuffer.getAvg(), dtype=np.uint8)
+
         # LEGACY
         # org_scale = (max_x - min_x,max_y - min_y)
         # self.pupil = pupil.Pupil(self.cut_image, min_x, min_y, self.scale, org_scale)
-        
-
-
```

### Comparing `eyegestures-1.3.3/eyeGestures/face.py` & `eyegestures-1.3.4/eyeGestures/face.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,88 @@
+"""Module providing finding and extraction of face from image."""
+
 import cv2
 import numpy as np
 import mediapipe as mp
 import eyeGestures.eye as eye
-import eyeGestures.nose as nose
+
 
 class FaceFinder:
 
-    def __init__(self, static_image_mode = True):
+    def __init__(self, static_image_mode=True):
         self.mp_face_mesh = mp.solutions.face_mesh.FaceMesh(
             refine_landmarks=True,
             static_image_mode=static_image_mode,
             min_detection_confidence=0.5,
             min_tracking_confidence=0.5
         )
 
-    def find(self,image):
+    def find(self, image):
 
-        assert(len(image.shape) > 2)
+        assert (len(image.shape) > 2)
 
         try:
-            face_mesh = self.mp_face_mesh.process(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
- 
+            face_mesh = self.mp_face_mesh.process(
+                cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
+
             return face_mesh
         except Exception as e:
             print(f"Exception in FaceFinder: {e}")
             return None
 
+
 class Face:
 
     def __init__(self):
-        self.eyeLeft  = eye.Eye(0)
+        self.eyeLeft = eye.Eye(0)
         self.eyeRight = eye.Eye(1)
 
     def getBoundingBox(self):
         margin = 0
-        min_x = np.min(self.landmarks[:,0]) - margin
-        max_x = np.max(self.landmarks[:,0]) + margin
-        min_y = np.min(self.landmarks[:,1]) - margin
-        max_y = np.max(self.landmarks[:,1]) + margin
-        
-        width  = int((max_x - min_x))
+        min_x = np.min(self.landmarks[:, 0]) - margin
+        max_x = np.max(self.landmarks[:, 0]) + margin
+        min_y = np.min(self.landmarks[:, 1]) - margin
+        max_y = np.max(self.landmarks[:, 1]) + margin
+
+        width = int((max_x - min_x))
         height = int((max_y - min_y))
         x = int(min_x)
-        y = int(min_y) 
-        return (x,y,width,height)
+        y = int(min_y)
+        return (x, y, width, height)
 
     def getLeftEye(self):
         return self.eyeLeft
 
     def getRightEye(self):
         return self.eyeRight
 
     def getLandmarks(self):
         return self.landmarks
-        
-    def _landmarks(self,face):
-                   
+
+    def _landmarks(self, face):
+
         __complex_landmark_points = face.multi_face_landmarks
         __complex_landmarks = __complex_landmark_points[0].landmark
 
         __face_landmarks = []
         for landmark in __complex_landmarks:
             __face_landmarks.append((
                 landmark.x * self.image_w,
                 landmark.y * self.image_h))
 
         return np.array(__face_landmarks)
 
-    def process(self,image,face):
+    def process(self, image, face):
         try:
             self.face = face
             self.image_h, self.image_w, _ = image.shape
             self.landmarks = self._landmarks(self.face)
             # self.nose = nose.Nose(image,self.landmarks,self.getBoundingBox())
-            
+
             x, y, _, _ = self.getBoundingBox()
-            offset = np.array((x,y))
+            offset = np.array((x, y))
             # offset = offset - self.nose.getHeadTiltOffset()
 
-            self.eyeLeft.update(image ,self.landmarks,offset)
-            self.eyeRight.update(image,self.landmarks,offset)
+            self.eyeLeft.update(image, self.landmarks, offset)
+            self.eyeRight.update(image, self.landmarks, offset)
         except Exception as e:
             return None
-
```

### Comparing `eyegestures-1.3.3/eyeGestures/gazeEstimator.py` & `eyegestures-1.3.4/eyeGestures/gazeEstimator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,215 @@
 
 import numpy as np
 from eyeGestures.gevent import Gevent
-from eyeGestures.nose import NoseDirection
 from eyeGestures.face import FaceFinder, Face
-from eyeGestures.Fixation import Fixation 
-from eyeGestures.processing    import EyeProcessor
-from eyeGestures.gazeContexter import GazeContext 
+from eyeGestures.Fixation import Fixation
+from eyeGestures.processing import EyeProcessor
+from eyeGestures.gazeContexter import GazeContext
 from eyeGestures.screenTracker.screenTracker import ScreenManager
 import eyeGestures.screenTracker.dataPoints as dp
 from eyeGestures.utils import Buffor
 
 
-def isInside(circle_x, circle_y, r, x, y):     
+def isInside(circle_x, circle_y, r, x, y):
+    """Function checking if points are inside the circle"""
+
     # Compare radius of circle
     # with distance of its center
     # from given point
     if ((x - circle_x) * (x - circle_x) +
-        (y - circle_y) * (y - circle_y) <= r * r):
+            (y - circle_y) * (y - circle_y) <= r * r):
         return True
     else:
         return False
 
+
 class GazeTracker:
+    """Class processing images and returning gaze tracker"""
 
     N_FEATURES = 16
 
-    def __init__(self,screen_width,screen_heigth,
-                 eye_screen_w,eye_screen_h,
-                 roi_x,roi_y,
+    def __init__(self, screen_width, screen_heigth,
+                 eye_screen_w, eye_screen_h,
+                 roi_x, roi_y,
                  roi_width, roi_height,
-                 monitor_offset_x = 0,
-                 monitor_offset_y = 0):
+                 monitor_offset_x=0,
+                 monitor_offset_y=0):
 
-        self.screen = dp.Screen(screen_width,screen_heigth)
+        self.screen = dp.Screen(screen_width, screen_heigth)
 
-        self.roi_x = roi_x 
+        self.roi_x = roi_x
         self.roi_y = roi_y
-        self.roi_width = roi_width 
+        self.roi_width = roi_width
         self.roi_height = roi_height
-        
+
         self.eye_screen_w = eye_screen_w
         self.eye_screen_h = eye_screen_h
 
-        self.eyeProcessorLeft  = EyeProcessor(eye_screen_w,eye_screen_h)
-        self.eyeProcessorRight = EyeProcessor(eye_screen_w,eye_screen_h)
+        self.eyeProcessorLeft = EyeProcessor(eye_screen_w, eye_screen_h)
+        self.eyeProcessorRight = EyeProcessor(eye_screen_w, eye_screen_h)
 
         self.screen_man = ScreenManager()
 
         self.finder = FaceFinder()
 
         # those are used for analysis
-        self.__headDir = [0.5,0.5]
+        self.__headDir = [0.5, 0.5]
 
-        self.point_screen = [0.0,0.0]
-        self.freezed_point = [0.0,0.0]
+        self.point_screen = [0.0, 0.0]
+        self.freezed_point = [0.0, 0.0]
 
         self.face = Face()
         self.GContext = GazeContext()
     #     self.calibration = False
 
-    def __gaze_intersection(self,l_eye,r_eye, l_buff, r_buff):
+    def __gaze_intersection(self, l_eye, r_eye, l_buff, r_buff):
         l_pupil = l_eye.getPupil()
-        l_gaze  = l_eye.getGaze(l_buff)
-        
-        r_pupil = r_eye.getPupil()        
-        r_gaze  = r_eye.getGaze(r_buff)
+        l_gaze = l_eye.getGaze(l_buff)
+
+        r_pupil = r_eye.getPupil()
+        r_gaze = r_eye.getGaze(r_buff)
 
         l_end = l_gaze + l_pupil
         r_end = r_gaze + r_pupil
 
         l_m = (l_end[1] - l_pupil[1])/(l_end[0] - l_pupil[0])
         r_m = (r_end[1] - r_pupil[1])/(r_end[0] - r_pupil[0])
 
         l_b = l_end[1] - l_m * l_end[0]
         r_b = r_end[1] - r_m * r_end[0]
 
         i_x = (r_b - l_b)/(l_m - r_m)
         i_y = r_m * i_x + r_b
-        return (i_x,i_y)
-    
+        return (i_x, i_y)
+
     def __pupil(self, eye, eyeProcessor, intersection_x, buffor):
 
-        eyeProcessor.append( eye.getPupil(), eye.getLandmarks(), buffor)
-        point = eyeProcessor.getAvgPupil(self.eye_screen_w,self.eye_screen_h,buffor)
-        point = np.array((int(intersection_x),point[1]))
-        
+        eyeProcessor.append(eye.getPupil(), eye.getLandmarks(), buffor)
+        point = eyeProcessor.getAvgPupil(
+            self.eye_screen_w, self.eye_screen_h, buffor)
+        point = np.array((int(intersection_x), point[1]))
+
         return point, buffor
-    
+
     def estimate(self,
                  image,
                  display,
                  context_id,
                  calibration,
-                 fixation_freeze = 0.7, 
+                 fixation_freeze=0.7,
                  freeze_radius=20,
-                 offset_x = 0,
-                 offset_y = 0):
+                 offset_x=0,
+                 offset_y=0):
+        """Function estimating gaze and returning gaze event based on image"""
 
         event = None
         face_mesh = self.getFeatures(image)
         if not face_mesh:
-            return None 
+            return None
 
         self.face.process(image, face_mesh)
 
-        context = self.GContext.get(context_id,display,roi = dp.ScreenROI(
+        context = self.GContext.get(context_id, display, roi=dp.ScreenROI(
             self.roi_x,
             self.roi_y,
             self.roi_width,
             self.roi_height),
-            edges = dp.ScreenROI(285,105,80,15),
-            cluster_boundaries = dp.ScreenROI(225,125,20,20),
-            buffor  = Buffor(200),
-            l_pupil = Buffor(20),
-            r_pupil = Buffor(20),
-            l_eye_buff = Buffor(20),
-            r_eye_buff = Buffor(20),
-            fixation=Fixation(0,0,100))
+            edges=dp.ScreenROI(285, 105, 80, 15),
+            cluster_boundaries=dp.ScreenROI(225, 125, 20, 20),
+            buffor=Buffor(200),
+            l_pupil=Buffor(20),
+            r_pupil=Buffor(20),
+            l_eye_buff=Buffor(20),
+            r_eye_buff=Buffor(20),
+            fixation=Fixation(0, 0, 100))
         context.calibration = calibration
-        
+
         if not self.face is None:
-            
-            l_eye   = self.face.getLeftEye()
-            r_eye   = self.face.getRightEye()
+
+            l_eye = self.face.getLeftEye()
+            r_eye = self.face.getRightEye()
 
             # TODO: check what happens here before with l_pupil
-            intersection_x,_ = self.__gaze_intersection(l_eye,r_eye, context.l_eye_buff, context.r_eye_buff)
-            l_point, l_buffor = self.__pupil(l_eye, self.eyeProcessorLeft,  intersection_x, context.l_pupil)
-            r_point, r_buffor = self.__pupil(r_eye, self.eyeProcessorRight, intersection_x, context.r_pupil)
-            
+            intersection_x, _ = self.__gaze_intersection(
+                l_eye, r_eye, context.l_eye_buff, context.r_eye_buff)
+            l_point, l_buffor = self.__pupil(
+                l_eye, self.eyeProcessorLeft,  intersection_x, context.l_pupil)
+            r_point, r_buffor = self.__pupil(
+                r_eye, self.eyeProcessorRight, intersection_x, context.r_pupil)
+
             context.l_pupil = l_buffor
             context.r_pupil = r_buffor
 
-            compound_point = np.array(((l_point + r_point)/2),dtype=np.uint32)
-        
+            compound_point = np.array(((l_point + r_point)/2), dtype=np.uint32)
+
             blink = l_eye.getBlink() or r_eye.getBlink()
             if blink != True:
                 context.gazeBuffor.add(compound_point)
-    
+
             self.point_screen, roi, cluster = self.screen_man.process(context.gazeBuffor,
-                                                        context.roi,
-                                                        context.edges,
-                                                        self.screen,
-                                                        context.display,
-                                                        context.calibration,
-                                                        (offset_x,offset_y)
-                                                        )
-            
+                                                                      context.roi,
+                                                                      context.edges,
+                                                                      self.screen,
+                                                                      context.display,
+                                                                      context.calibration,
+                                                                      (offset_x,
+                                                                       offset_y)
+                                                                      )
+
             context.roi = roi
             if cluster:
-                x,y,width,height = cluster.getBoundaries()
+                x, y, width, height = cluster.getBoundaries()
                 context.cluster_boundaries.x = x
                 context.cluster_boundaries.y = y
                 context.cluster_boundaries.width = width
                 context.cluster_boundaries.height = height
 
-            self.GContext.update(context_id,context)
+            self.GContext.update(context_id, context)
 
             ###########################################################
-            
-            fix = context.fixation.process(self.point_screen[0],self.point_screen[1])
+
+            fix = context.fixation.process(
+                self.point_screen[0], self.point_screen[1])
             # this should prevent of sudden movement down when blinking - not perfect yet
-            
+
             if fix > fixation_freeze:
                 r = freeze_radius
-                if not isInside(self.freezed_point[0],self.freezed_point[1],r,self.point_screen[0],self.point_screen[1]):
+                if not isInside(self.freezed_point[0], self.freezed_point[1], r, self.point_screen[0], self.point_screen[1]):
                     self.freezed_point = self.point_screen
 
                 event = Gevent(compound_point,
-                        self.freezed_point,
-                        blink,
-                        fix,
-                        l_eye,
-                        r_eye,
-                        context,
-                        context_id)
+                               self.freezed_point,
+                               blink,
+                               fix,
+                               l_eye,
+                               r_eye,
+                               display,
+                               context_id)
             else:
                 self.freezed_point = self.point_screen
                 event = Gevent(compound_point,
-                            self.point_screen,
-                            blink,
-                            fix,
-                            l_eye,
-                            r_eye,
-                            context,
-                            context_id)
+                               self.point_screen,
+                               blink,
+                               fix,
+                               l_eye,
+                               r_eye,
+                               display,
+                               context_id)
 
         return event
-    
-    def get_contextes(self):
-        return self.finder.get_contextes()
 
-    def add_offset(self,x,y):
-        self.screen_man.push_window(x,y)
+    # def get_contextes(self):
+    #     """Function returning contextes"""
+
+    #     return self.GContext.get_contextes()
+
+    # def add_offset(self,x,y):
+    #     """Function adding offsets to tracker"""
+
+    #     self.screen_man.push_window(x,y)
+
+    def getFeatures(self, image):
+        """Function returning face landmarks"""
 
-    def getFeatures(self,image):
         face_mesh = self.finder.find(image)
         return face_mesh
-        
-    def getHeadDirection(self):
-        return self.__headDir
```

### Comparing `eyegestures-1.3.3/eyeGestures/gevent.py` & `eyegestures-1.3.4/eyeGestures/gevent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
- 
+"""Module providing a Gaze Events."""
+
+
 class Gevent:
+    """Class representing gaze event, with tracked points scaled to screen, blink and fixation."""
 
     def __init__(self,
                  point,
                  point_screen,
                  blink,
                  fixation,
                  l_eye,
@@ -12,12 +15,12 @@
                  context):
 
         self.point = point
         self.blink = blink
         self.fixation = fixation
         self.point_screen = point_screen
 
-        ## ALL DEBUG DATA
+        # ALL DEBUG DATA
         self.l_eye = l_eye
         self.r_eye = r_eye
         self.screen_man = screen_man
-        self.context = context
+        self.context = context
```

### Comparing `eyegestures-1.3.3/eyeGestures/processing.py` & `eyegestures-1.3.4/eyeGestures/processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,65 @@
+"""Module providing a processing pupil position to gaze direction."""
 
 import numpy as np
-from eyeGestures.utils import Buffor
+
 
 class EyeProcessor:
+    """Class providing processing for eye to obtain gaze direction."""
 
-    def __init__(self,scale_w=250,scale_h=250):
+    def __init__(self, scale_w=250, scale_h=250):
         self.scale_w = scale_w
         self.scale_h = scale_h
+        self.min_x = 0
+        self.max_x = 0
+        self.min_y = 0
+        self.max_y = 0
+        self.pupil = None
+        self.landmarks = None
 
+    def append(self, pupil: (int, int), landmarks: np.ndarray, pupilBuffor):
+        """Function appending new pupil point to tracker."""
 
-    def append(self,pupil : (int,int) ,landmarks : np.ndarray, pupilBuffor):
         self.pupil = pupil
         self.landmarks = landmarks
 
-        # get center: 
+        # get center:
         margin = 5
-        self.min_x = np.min(self.landmarks[:,0]) - margin
-        self.max_x = np.max(self.landmarks[:,0]) + margin
-        self.min_y = np.min(self.landmarks[:,1]) - margin
-        self.max_y = np.max(self.landmarks[:,1]) + margin
-        
-        assert(self.pupil[0] > self.min_x)
-        assert(self.pupil[1] > self.min_y)
+        self.min_x = np.min(self.landmarks[:, 0]) - margin
+        self.max_x = np.max(self.landmarks[:, 0]) + margin
+        self.min_y = np.min(self.landmarks[:, 1]) - margin
+        self.max_y = np.max(self.landmarks[:, 1]) + margin
+
+        assert self.pupil[0] > self.min_x
+        assert self.pupil[1] > self.min_y
 
-        width  = self.max_x - self.min_x
+        width = self.max_x - self.min_x
         height = (self.max_y - self.min_y)/2
 
-        
         pupilBuffor.add(
             self.__convertPoint(self.pupil,
-                        width = self.scale_w, height = self.scale_h,
-                        scale_w = width, scale_h = height,
-                        offset = (self.min_x, self.min_y)))
-
-    def getWidth(self):
-        return self.width
-
-    def getHeight(self):
-        return self.height
-
-    def __convertPoint(self, point, width=1.0, height=1.0, scale_w = 1.0, scale_h = 1.0, offset = (0.0,0.0)):
+                                width=self.scale_w, height=self.scale_h,
+                                scale_w=width, scale_h=height,
+                                offset=(self.min_x, self.min_y)))
+
+    def __convertPoint(self, point,
+                       width=1.0,
+                       height=1.0,
+                       scale_w=1.0,
+                       scale_h=1.0,
+                       offset=(0.0, 0.0)):
         (min_x, min_y) = offset
         x = int(((point[0]-min_x)/scale_w)*width)
         y = int(((point[1]-min_y)/scale_h)*height)
-        return (x,y)
+        return (x, y)
 
     def getAvgPupil(self, width, height, pupilBuffor):
+        """Function returning average point based on tracked."""
+
         if not width is None and not height is None:
             _retPupil = self.__convertPoint(pupilBuffor.getAvg(),
-                            width = width,height = height,
-                            scale_w = self.scale_w, scale_h = self.scale_h)
+                                            width=width, height=height,
+                                            scale_w=self.scale_w, scale_h=self.scale_h)
         else:
             _retPupil = pupilBuffor.getAvg()
-        
+
         return _retPupil
```

### Comparing `eyegestures-1.3.3/eyeGestures/scalling_test.py` & `eyegestures-1.3.4/eyeGestures/scalling_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,54 +4,58 @@
 
 # region of interest inside the virtual screen
 ROI_WIDTH = 30
 ROI_HEIGHT = 20
 
 ####################### screen 2 display Tests #################################
 
+
 def test_scaleUpTest():
-    pos = (50,50)
+    pos = (50, 50)
     BIGGER = 10
 
-    roi = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH,ROI_HEIGHT)
-    roi2 = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH+BIGGER,ROI_HEIGHT+BIGGER)
-    
-    bigger_roi = scrtr.scaleUp(roi,roi2,0.1)
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    roi2 = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH+BIGGER, ROI_HEIGHT+BIGGER)
+
+    bigger_roi = scrtr.scaleUp(roi, roi2, 0.1)
 
     assert bigger_roi.width > roi.width
     assert bigger_roi.height > roi.height
 
+
 def test_scaleUpTest_known():
-    pos = (50,50)
+    pos = (50, 50)
     BIGGER = 10
 
-    roi = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH,ROI_HEIGHT)
-    roi2 = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH+BIGGER,ROI_HEIGHT+BIGGER)
-    
-    bigger_roi = scrtr.scaleUp(roi,roi2,0.1)
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    roi2 = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH+BIGGER, ROI_HEIGHT+BIGGER)
+
+    bigger_roi = scrtr.scaleUp(roi, roi2, 0.1)
 
     assert int(bigger_roi.width) == int(ROI_WIDTH*1.1)
     assert int(bigger_roi.height) == int(ROI_HEIGHT*1.1)
 
+
 def test_scaleDownTest():
-    pos = (50,50)
+    pos = (50, 50)
     SMALLER = 10
 
-    roi = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH,ROI_HEIGHT)
-    roi2 = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH-SMALLER,ROI_HEIGHT-SMALLER)
-    
-    smaller_roi = scrtr.scaleDown(roi,roi2,-0.1)
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    roi2 = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH-SMALLER, ROI_HEIGHT-SMALLER)
+
+    smaller_roi = scrtr.scaleDown(roi, roi2, -0.1)
 
-    assert smaller_roi.width  < roi.width
+    assert smaller_roi.width < roi.width
     assert smaller_roi.height < roi.height
 
+
 def test_scaleUpTest_known():
-    pos = (50,50)
+    pos = (50, 50)
     SMALLER = 10
 
-    roi = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH,ROI_HEIGHT)
-    roi2 = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH-SMALLER,ROI_HEIGHT-SMALLER)
-    
-    smaller_roi = scrtr.scaleDown(roi,roi2,-0.1)
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    roi2 = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH-SMALLER, ROI_HEIGHT-SMALLER)
+
+    smaller_roi = scrtr.scaleDown(roi, roi2, -0.1)
 
     assert int(smaller_roi.width) == int(ROI_WIDTH*0.9)
     assert int(smaller_roi.height) == int(ROI_HEIGHT*0.9)
```

### Comparing `eyegestures-1.3.3/eyeGestures/screenTracker_test.py` & `eyegestures-1.3.4/eyeGestures/screenTracker_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import pytest
-import eyeGestures.screenTracker.screenTracker as scrtr
 import eyeGestures.screenTracker.dataPoints as dp
+import eyeGestures.screenTracker.screenTracker as scrtr
 
 # virtual tracking ScreenProcessor
 SCREEN_WIDTH = 500
 SCREEN_HEIGHT = 500
 
 # region of interest inside the virtual ScreenProcessor
 ROI_WIDTH = 50
@@ -12,98 +11,105 @@
 
 # size of real display
 DISPLAY_WIDTH = 1200
 DISPLAY_HEIGHT = 1800
 
 ####################### ScreenProcessor 2 display Tests #################################
 
+
 def test_screen2display_1_1():
-    point = (1,1)
+    """[TEST]"""
+    point = (1, 1)
 
-    roi = dp.ScreenROI(0,0,ROI_WIDTH,ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH,DISPLAY_HEIGHT,0,0)
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
 
     tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point,roi,display)
-    
+    p = tracker.screen2display(point, roi, display)
+
     assert p == (point[0]/ROI_WIDTH * DISPLAY_WIDTH,
                  point[1]/ROI_HEIGHT * DISPLAY_HEIGHT)
 
+
 def test_screen2display_55_1():
-    point = (55,1)
+    """[TEST]"""
+    point = (55, 1)
 
-    roi = dp.ScreenROI(0,0,ROI_WIDTH,ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH,DISPLAY_HEIGHT,0,0)
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
 
     tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point,roi,display)
-    
-    assert p == (DISPLAY_WIDTH, 
+    p = tracker.screen2display(point, roi, display)
+
+    assert p == (DISPLAY_WIDTH,
                  point[1]/ROI_HEIGHT * DISPLAY_HEIGHT)
 
+
 def test_screen2display_55_55():
-    point = (55,55)
+    """[TEST]"""
+    point = (55, 55)
 
-    roi = dp.ScreenROI(0,0,ROI_WIDTH,ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH,DISPLAY_HEIGHT,0,0)
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
 
     tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point,roi,display)
-    
+    p = tracker.screen2display(point, roi, display)
+
     assert p == (DISPLAY_WIDTH,
-                DISPLAY_HEIGHT)
+                 DISPLAY_HEIGHT)
 
 
 def test_screen2display_0_0():
-    point = (0,0)
+    """[TEST]"""
+    point = (0, 0)
 
-    roi = dp.ScreenROI(0,0,ROI_WIDTH,ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH,DISPLAY_HEIGHT,0,0)
+    roi = dp.ScreenROI(0, 0, ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
 
     tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point,roi,display)
-    
+    p = tracker.screen2display(point, roi, display)
+
     assert p == (0, 0)
 
+
 def test_screen2display_1_1_pos_50_50():
-    point = (51,51)
-    pos = (50,50)
+    """[TEST]"""
+    point = (51, 51)
+    pos = (50, 50)
 
-    roi = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH,ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH,DISPLAY_HEIGHT,0,0)
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
 
     tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point,roi,display)
-    
+    p = tracker.screen2display(point, roi, display)
+
     assert p == ((point[0] - pos[0])/ROI_WIDTH * DISPLAY_WIDTH,
                  (point[1] - pos[1])/ROI_HEIGHT * DISPLAY_HEIGHT)
 
 
 def test_screen2display_55_55_pos_50_50():
-    point = (105,105) 
-    pos = (50,50)
+    """[TEST]"""
+    point = (105, 105)
+    pos = (50, 50)
 
-    roi = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH,ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH,DISPLAY_HEIGHT,0,0)
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
 
     tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point,roi,display)
-    
+    p = tracker.screen2display(point, roi, display)
+
     assert p == (DISPLAY_WIDTH,
                  DISPLAY_HEIGHT)
 
 
 def test_screen2display_0_0_pos_50_50():
-    point = (0,0)
-    pos = (50,50)
+    """[TEST]"""
+    point = (0, 0)
+    pos = (50, 50)
 
-    roi = dp.ScreenROI(pos[0],pos[1],ROI_WIDTH,ROI_HEIGHT)
-    display = dp.Display(DISPLAY_WIDTH,DISPLAY_HEIGHT,0,0)
+    roi = dp.ScreenROI(pos[0], pos[1], ROI_WIDTH, ROI_HEIGHT)
+    display = dp.Display(DISPLAY_WIDTH, DISPLAY_HEIGHT, 0, 0)
 
     tracker = scrtr.ScreenProcessor()
-    p = tracker.screen2display(point,roi,display)
-    
-    assert p == (0, 0)
-
-
-    
+    p = tracker.screen2display(point, roi, display)
 
+    assert p == (0, 0)
```

### Comparing `eyegestures-1.3.3/eyeGestures/utils.py` & `eyegestures-1.3.4/eyeGestures/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,44 @@
-import cv2
 import time
-import pickle
-import numpy as np
 import queue
+import pickle
 import platform
 import threading
-from typing import Callable, Tuple
+
+import cv2
+import numpy as np
 
 # Make predictions for new data points
 
+
 def timeit(func):
+    """
+    timeit
+    """
     def inner(*args, **kwargs):
+        """
+        inner
+        """
         start = time.time()
         ret = func(*args, **kwargs)
         print(f"Elapsed time: {time.time() - start}")
-        return ret 
+        return ret
     return inner
 
+
 def shape_to_np(shape, dtype="int"):
+    """
+    shape_to_np
+    """
     coords = np.zeros((68, 2), dtype=dtype)
     for i in range(0, 68):
         coords[i] = (shape.part(i).x, shape.part(i).y)
     return coords
 
+
 def make_image_grid(images, rows, cols):
     """
     Make a grid of images.
 
     Parameters:
     - images: list of images to form the grid (all images must be of the same size and type)
     - rows, cols: number of rows and columns in the grid
@@ -39,78 +51,84 @@
     # assert len(images) >= rows * cols, "Not enough images to fill the grid"
 
     # Get image dimensions
     img_h, img_w = images[0].shape[:2]
 
     if len(images[0].shape) > 2:
         # Create a black canvas to draw the grid on
-        grid_image = np.zeros((img_h * rows, img_w * cols, images[0].shape[2]), dtype=np.uint8)
+        grid_image = np.zeros(
+            (img_h * rows, img_w * cols, images[0].shape[2]), dtype=np.uint8)
     else:
         grid_image = np.zeros((img_h * rows, img_w * cols), dtype=np.uint8)
 
     # Copy images to the grid
     for i, img in enumerate(images):
         if i >= rows * cols:
             break  # Stop if we have filled the grid
         row = i // cols
         col = i % cols
-        grid_image[row * img_h:(row + 1) * img_h, col * img_w:(col + 1) * img_w] = img
+        grid_image[row * img_h:(row + 1) * img_h, col *
+                   img_w:(col + 1) * img_w] = img
 
     return grid_image
 
 
 class var:
 
-    def __init__(self,var):
+    def __init__(self, var):
         self.__var = var
 
-    def set(self,var):
+    def set(self, var):
         self.__var = var
 
     def get(self):
         return self.__var
 
+
 class Buffor:
 
     def __init__(self, length):
         self.length = length
         self.__buffor = []
 
-    def add(self,var):
+    def add(self, var):
         if len(self.__buffor) >= self.length:
             self.__buffor.pop(0)
 
         self.__buffor.append(var)
 
-    def getAvg(self,lenght=0):
+    def getAvg(self, lenght=0):
         return np.sum(self.__buffor[-lenght:], axis=0) / len(self.__buffor[-lenght:])
 
     def getBuffor(self):
         return self.__buffor
-    
+
     def loadBuffor(self, buffor):
         self.__buffor = buffor
 
     def getLast(self):
         return self.__buffor[0]
 
     def getFirst(self):
         return self.__buffor[len(self.__buffor) - 1]
 
     def getLen(self):
         return len(self.__buffor)
 
 # Bufforless
+
+
 class VideoCapture:
+    """Wrapper on openCV2 stream making it bufforless and adding camera search"""
 
-    def __init__(self, name, bufforless = True):
+    def __init__(self, name, bufforless=True):
         self.bufforless = bufforless
         self.run = True
 
-        if isinstance(name,str):
+        if isinstance(name, str):
             if ".pkl" in name:
                 self.stream = False
             else:
                 self.stream = True
         else:
             self.stream = True
 
@@ -122,16 +140,16 @@
             self.q = queue.Queue()
             self.t = threading.Thread(target=self.__reader).start()
         else:
             self.frames = []
             with open(name, 'rb') as file:
                 self.frames = pickle.load(file)
 
-    def __openCam(self,name):
-        if isinstance(name,int):
+    def __openCam(self, name):
+        if isinstance(name, int):
             if "Windows" in platform.system():
                 self.cap = cv2.VideoCapture(name, cv2.CAP_DSHOW)
             else:
                 self.cap = cv2.VideoCapture(name)
 
             if self.cap is None or not self.cap.isOpened():
                 print(f"Was unable to open camera: {name}.")
@@ -147,21 +165,23 @@
             if not ret:
                 break
             if not self.q.empty() and self.bufforless:
                 try:
                     self.q.get_nowait()
                 except queue.Empty:
                     pass
-            self.q.put((ret,frame))
+            self.q.put((ret, frame))
 
         self.run = False
 
     def read(self):
+        """Function returning latest frame"""
         if self.stream:
             return self.q.get()
         else:
             frame = self.frames.pop(0)
             self.frames.pop(0)
             return ((len(self.frames) >= 1), frame)
 
     def close(self):
-        self.run = False
+        """Function closing stream"""
+        self.run = False
```

### Comparing `eyegestures-1.3.3/eyeGestures/screenTracker/heatmap.py` & `eyegestures-1.3.4/eyeGestures/screenTracker/heatmap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 class Heatmap():
+    """Helper representing Heatmap of tracked points"""
 
     def __init__(self,width,height,buffor):
         self.inc_step = 10
         self.step = 10
         bars = self.step
 
         self.width = width
@@ -27,35 +28,39 @@
         self.max_x = self.__getParam((self.axis_x > self.inc_step*4),last=True)
         self.min_y = self.__getParam((self.axis_y > self.inc_step*4),last=False)
         self.max_y = self.__getParam((self.axis_y > self.inc_step*4),last=True)
 
     def __getParam(self,param,last : bool = False):
         ret = 0
         retArray = np.where(param)
-        
+
         if len(retArray[0]) > 0:
             ret = retArray[0][- int(last)] * self.step
 
             if not ret == np.NAN:
                 ret = int(ret)
-        
+
         return ret
-        
+
     def getBoundaries(self):
+        """Function returning boundaries of heatmap"""
         x = self.min_x
         y = self.min_y
         w = self.max_x - self.min_x
-        h = self.max_y - self.min_y 
+        h = self.max_y - self.min_y
         return (x,y,w,h)
 
     def getCenter(self):
+        """Function returning center of heatmap"""
         center_x = int((self.max_x - self.min_x)/2 + self.min_x)
         center_y = int((self.max_y - self.min_y)/2 + self.min_y)
         return (center_x,center_y)
-    
+
     def getPeak(self):
+        """Function returning peak of heatmap"""
         x = int(np.argmax(self.axis_x)*self.inc_step)
         y = int(np.argmax(self.axis_y)*self.inc_step)
         return (x,y)
 
     def getHist(self):
+        """Function returning histogram of the heatmap. This heatmap is simply 2d histogram, so this function returns values for each axis."""
         return (self.axis_x/self.inc_step,self.axis_y/self.inc_step)
```

### Comparing `eyegestures-1.3.3/eyeGestures/screenTracker/screenTracker.py` & `eyegestures-1.3.4/eyeGestures/screenTracker/screenTracker.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,186 +7,200 @@
 import eyeGestures.screenTracker.dataPoints as dp
 from eyeGestures.screenTracker.clusters import Clusters
 from eyeGestures.screenTracker.heatmap import Heatmap
 
 # THIS FILE IS SLOWLY BECOMING BLACK MAGIC
 
 def detect_edges(roi, display, point_on_screen, point_on_display):
+    """Function performing edge detection based on point, screen and display sizes"""
     (s_x,s_y) = point_on_screen 
     (d_x,d_y) = point_on_display
 
     x,y,width,height = roi.getBoundaries() 
     new_roi = dp.ScreenROI(x,y,width,height)
-    
+
     # new_w = screen.width
     # margin = 5
     # TODO: fix this to estimate w and h
-    if(d_x <= 0):
+    if d_x <= 0 :
         new_roi.width = new_roi.width + abs(new_roi.x - s_x)
         new_roi.x = s_x
-        
-    if(d_x >= display.width):
+
+    if d_x >= display.width :
         new_roi.width = abs(new_roi.x - s_x)
 
-    if(d_y <= 0):
+    if d_y <= 0 :
         new_roi.height = new_roi.height + abs(new_roi.y - s_y)
         new_roi.y = s_y
-        
-    if(d_y >= display.height):
+
+    if d_y >= display.height :
         new_roi.height = abs(new_roi.y - s_y)
-    
-    return new_roi 
+
+    return new_roi
 
 def rescale_h(roi, scale_h, change = 0.5):
+    """change size on height"""
     scale_diff_h = abs(1.0 - scale_h)
-    
+
     ret_heigth  = roi.height
-    
+
     if scale_diff_h > change: 
         ret_heigth = roi.height/1.0 * scale_h
 
     return ret_heigth
-    
+
 def rescale_w(roi, scale_w, change = 0.5):
+    """change size on width"""
     scale_diff_w = abs(1.0 - scale_w)
-    
+
     ret_width   = roi.width
 
     if scale_diff_w > change: 
         ret_width = roi.width/1.0 * scale_w
 
     return ret_width
 
 
 def scaleDown(roi, edge, scale):
-    
+    """Function scalling down one roi till edges are met"""
+
     (_,_,cluster_w,cluster_h) = edge.getBoundaries()
 
     new_roi = dp.ScreenROI(roi.x,roi.y,roi.width,roi.height)
-    if(cluster_w < roi.width):
+    if cluster_w < roi.width :
         new_scale_w = 1.0 + scale
         new_w = rescale_w(roi,new_scale_w,scale)
         new_roi.width = new_w
-    
-    if(cluster_h < roi.height):
+
+    if cluster_h < roi.height :
         new_scale_h = 1.0 + scale
         new_h = rescale_h(roi,new_scale_h,scale)
         new_roi.height = new_h
 
     return new_roi
 
 def scaleUp(roi, roi2, scale):
-    
+    """Function scalling up one roi into another roi, second roi is for limiting scaling operation and scale is telling how much you can scale"""
+
     (_,_,roi2_w,roi2_h) = roi2.getBoundaries()
 
     new_roi = dp.ScreenROI(roi.x,roi.y,roi.width,roi.height)
 
-    if(roi2_w > roi.width):
+    if roi2_w > roi.width :
         new_scale_w = 1.0 + scale
         new_w = rescale_w(roi,new_scale_w,scale)
         new_roi.width = new_w
-       
-    if(roi2_h > roi.height):
+
+    if roi2_h > roi.height :
         new_scale_h = 1.0 + scale
         new_h = rescale_h(roi,new_scale_h,scale)
         new_roi.height = new_h
 
     return new_roi
 
 
 class ScreenProcessor:
+    """Class for doing tracking and converting screen to display and display to screen"""
 
     def __init__(self):
         pass
 
     # RUN FEATURE
     def process(self,point,point_offset,buffor_length,roi,edges,screen,display,heatmap):
-        
+        """Function performing main processing for screen processor. Tons of parameters doing brrrr"""
+
         s_point_offset = self.display2screen(point_offset,screen,display)
         p_on_display = self.screen2display([point[0] + s_point_offset[0],point[1] + s_point_offset[1]],roi,display)
         # p_on_display = self.screen2display(point,roi,display)
-        
+
         if buffor_length > 20:
             new_edges = detect_edges(roi, display, point, p_on_display)
             edges.x      = new_edges.x
             edges.y      = new_edges.y
             edges.width  = new_edges.width
             edges.height = new_edges.height
-        
+
         p_on_display = (p_on_display[0] + display.offset_x, p_on_display[1] + display.offset_y)
-        
+
         # return how close that is hist region
         (_,_,roi_w,roi_h) = heatmap.getBoundaries()
         closeness_percentage = (roi_w * roi_h)/(screen.width * screen.height)
         return (p_on_display,closeness_percentage)
 
     # CALIBRATION FEATURE
     # it should not affect objects but produce new ones
     def update(self, roi, edges, cluster, heatmap):
+        """Function to update screen processor with new clusters and heatmaps"""
 
         (x,y) = heatmap.getCenter()
         # =====================================
-        # ---------histogram obtained---------- 
+        # ---------histogram obtained----------
         # =====================================
         new_roi = dp.ScreenROI(roi.x,roi.y,roi.width,roi.height)
         new_roi.setCenter(x,y)
         edges.setCenter(x,y)
         # self.eyeScreen.setCenter(x,y) 
         new_roi = scaleUp(new_roi, edges, scale = 0.1)
 
         # =====================================
         # if screen is bigger than edges make it smaller
         # =====================================
         new_roi = scaleDown(new_roi, cluster, scale = -0.1)
         return new_roi
-        
-    
+
+
     def screen2display(self, screen_point, screen, display):
+        """Function converting screen points to display points"""
+
         s_x,s_y = screen_point[0],screen_point[1]
 
         d_x = int((s_x - screen.x)/screen.width * display.width)
         d_y = int((s_y - screen.y)/screen.height * display.height)
 
         d_x = max(d_x,0)
         d_y = max(d_y,0)
         d_x = min(d_x,display.width)
         d_y = min(d_y,display.height)
 
         return (d_x,d_y)
-    
+
     def display2screen(self, display_point, screen, display):
+        """Function converting display points to screen points"""
+
         d_x,d_y = display_point[0],display_point[1]
 
         s_x = int((d_x)/display.width  * screen.width)
         s_y = int((d_y)/display.height * screen.height)
 
 
         return (s_x,s_y)
 
 class ScreenManager:
+    """Class performing most of tracking after estimating position of gaze"""
 
-    def __init__(self,):     
+    def __init__(self,):
         self.screen_processor = ScreenProcessor()
-   
+
 
     def process(self, buffor, roi, edges, screen, display, calibration, offset):
+        """Function doing processing and tracking and calibration of tracker"""
 
         heatmap = Heatmap(screen.width,screen.height,buffor.getBuffor())
         cluster = Clusters(buffor.getBuffor()).getMainCluster()
 
         if cluster is not None:
-            
+   
             if calibration:
                 roi = self.screen_processor.update(roi, edges, cluster, heatmap)
 
             p, percentage = self.screen_processor.process(
                 buffor.getAvg(20),
                 (offset[0],offset[1]),
                 len(buffor.getBuffor()),
                 roi,
                 edges,
                 screen,
                 display,
                 heatmap)
-               
+
             return (p, roi, cluster)
         return ([0,0], roi, cluster)
```

### Comparing `eyegestures-1.3.3/LICENSE` & `eyegestures-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eyegestures-1.3.3/README.md` & `eyegestures-1.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,617 +1,643 @@
-00000000: 6060 600a 466f 7220 656e 7465 7270 7269  ```.For enterpri
-00000010: 7365 2061 766f 6964 696e 6720 4750 4c33  se avoiding GPL3
-00000020: 206c 6963 656e 7369 6e67 2074 6865 7265   licensing there
-00000030: 2069 7320 636f 6d6d 6572 6369 616c 206c   is commercial l
-00000040: 6963 656e 7365 210a 6060 600a 2323 20f0  icense!.```.## .
-00000050: 9f91 81ef b88f 2045 7965 4765 7374 7572  ...... EyeGestur
-00000060: 6573 0a0a 4579 6547 6573 7475 7265 7320  es..EyeGestures 
-00000070: 6973 206f 7065 6e20 736f 7572 6365 2065  is open source e
-00000080: 7965 7472 6163 6b69 6e67 2073 6f66 7477  yetracking softw
-00000090: 6172 652f 6c69 6272 6172 7920 7573 696e  are/library usin
-000000a0: 6720 6e61 7469 7665 2077 6562 6361 6d73  g native webcams
-000000b0: 2061 6e64 2070 686f 6e65 2063 616d 6572   and phone camer
-000000c0: 7320 666f 7220 6163 6869 6576 696e 6720  s for achieving 
-000000d0: 6974 7320 676f 616c 2e20 5468 6520 6169  its goal. The ai
-000000e0: 6d20 6f66 206c 6962 7261 7279 2069 7320  m of library is 
-000000f0: 746f 2062 7269 6e67 2061 6363 6573 7369  to bring accessi
-00000100: 6269 6c69 7479 206f 6620 6579 6574 7261  bility of eyetra
-00000110: 636b 696e 6720 616e 6420 6579 6564 7269  cking and eyedri
-00000120: 7665 6e20 696e 7465 7266 6163 6573 2077  ven interfaces w
-00000130: 6974 686f 7574 2072 6571 7569 7265 6d65  ithout requireme
-00000140: 6e74 206f 6620 6f62 7461 696e 696e 6720  nt of obtaining 
-00000150: 6578 7065 6e73 6976 6520 6861 7264 7761  expensive hardwa
-00000160: 7265 2e0a 0a3c 7020 616c 6967 6e3d 2263  re...<p align="c
-00000170: 656e 7465 7222 3e0a 2020 3c69 6d67 2073  enter">.  <img s
-00000180: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
-00000190: 7562 2e63 6f6d 2f50 6574 6572 5761 4949  ub.com/PeterWaII
-000001a0: 6163 652f 5065 7465 7257 6149 4961 6365  ace/PeterWaIIace
-000001b0: 2f61 7373 6574 732f 3430 3737 3335 3530  /assets/40773550
-000001c0: 2f32 6164 3235 3235 322d 6539 3665 2d34  /2ad25252-e96e-4
-000001d0: 3764 342d 6232 3566 2d63 3437 6261 3766  7d4-b25f-c47ba7f
-000001e0: 3066 3466 3322 2077 6964 7468 3d22 3330  0f4f3" width="30
-000001f0: 3022 2068 6569 6768 743d 2231 3530 223e  0" height="150">
-00000200: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
-00000210: 3a2f 2f67 6974 6875 622e 636f 6d2f 5065  ://github.com/Pe
-00000220: 7465 7257 6149 4961 6365 2f50 6574 6572  terWaIIace/Peter
-00000230: 5761 4949 6163 652f 6173 7365 7473 2f34  WaIIace/assets/4
-00000240: 3037 3733 3535 302f 6633 3133 3238 3433  0773550/f3132843
-00000250: 2d30 3633 612d 3433 3961 2d38 6531 632d  -063a-439a-8e1c-
-00000260: 3233 3835 6464 6664 6363 6461 2220 7769  2385ddfdccda" wi
-00000270: 6474 683d 2233 3030 0a22 2068 6569 6768  dth="300." heigh
-00000280: 743d 2231 3530 223e 0a3c 2f70 3e0a 3c70  t="150">.</p>.<p
-00000290: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000002a0: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
-000002b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e61  ://github.com/Na
-000002c0: 7469 7665 5365 6e73 6f72 732f 4579 6547  tiveSensors/EyeG
-000002d0: 6573 7475 7265 732f 6173 7365 7473 2f34  estures/assets/4
-000002e0: 3037 3733 3535 302f 3834 6161 3734 3336  0773550/84aa7436
-000002f0: 2d36 3135 332d 3439 6263 2d62 3865 362d  -6153-49bc-b8e6-
-00000300: 6363 6461 3533 3566 3235 6536 2922 2077  ccda535f25e6)" w
-00000310: 6964 7468 3d22 3630 300a 2220 6865 6967  idth="600." heig
-00000320: 6874 3d22 3330 3022 3e0a 3c2f 703e 0a0a  ht="300">.</p>..
-00000330: 2323 2320 e2ad 9020 4d69 7373 696f 6e20  ### ... Mission 
-00000340: 0a0a 5468 6572 6520 6973 206e 6f20 6f6e  ..There is no on
-00000350: 6520 7369 7a65 2d66 6974 7320 616c 6c20  e size-fits all 
-00000360: 736f 6c75 7469 6f6e 2c20 616e 6420 7765  solution, and we
-00000370: 2062 656c 6965 7665 2074 6861 7420 6469   believe that di
-00000380: 6666 6572 656e 7469 6174 696e 6720 696e  fferentiating in
-00000390: 7465 7266 6163 6573 2062 7269 6e67 7320  terfaces brings 
-000003a0: 6163 6365 7373 6962 696c 6974 7920 746f  accessibility to
-000003b0: 2064 6967 6974 616c 2073 7061 6365 732e   digital spaces.
-000003c0: 2044 6573 6967 6e69 6e67 2065 7965 2d64   Designing eye-d
-000003d0: 7269 7665 6e20 696e 7465 7266 6163 6573  riven interfaces
-000003e0: 2067 6976 6573 206d 6f72 6520 636f 6e74   gives more cont
-000003f0: 726f 6c20 6f76 6572 2063 6f6d 7075 7465  rol over compute
-00000400: 7273 2074 6f20 7468 6f73 6520 7768 6f20  rs to those who 
-00000410: 6361 6e6e 6f74 2066 756c 6c79 2065 6e6a  cannot fully enj
-00000420: 6f79 2074 6865 6972 2063 6170 6162 696c  oy their capabil
-00000430: 6974 6965 7320 6475 6520 746f 2064 6966  ities due to dif
-00000440: 6665 7265 6e74 2064 6973 6162 696c 6974  ferent disabilit
-00000450: 6965 732c 2061 7320 7765 6c6c 2061 7320  ies, as well as 
-00000460: 616e 2061 6464 6974 696f 6e61 6c20 7761  an additional wa
-00000470: 7920 746f 2063 6f6e 7472 6f6c 2063 6f6d  y to control com
-00000480: 7075 7465 7220 746f 2072 6573 7473 2e20  puter to rests. 
-00000490: 0a0a 5375 6368 2074 6563 686e 6f6c 6f67  ..Such technolog
-000004a0: 7920 7368 6f75 6c64 206e 6f74 2062 6520  y should not be 
-000004b0: 7061 7977 616c 6c65 6420 6279 2065 7870  paywalled by exp
-000004c0: 656e 7369 7665 2065 7965 2d74 7261 636b  ensive eye-track
-000004d0: 696e 6720 6861 7264 7761 7265 2c20 6573  ing hardware, es
-000004e0: 7065 6369 616c 6c79 2069 6e20 6361 7365  pecially in case
-000004f0: 2077 6865 6e20 6974 2069 7320 6e65 6564   when it is need
-00000500: 6564 2074 6f20 6578 6973 7420 696e 2074  ed to exist in t
-00000510: 6865 2064 6967 6974 616c 2077 6f72 6c64  he digital world
-00000520: 2061 6e64 206f 7065 7261 7465 2079 6f75   and operate you
-00000530: 7220 636f 6d70 7574 6572 2e20 4d6f 7374  r computer. Most
-00000540: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
-00000550: 636f 6e73 756d 6572 2065 6c65 6374 726f  consumer electro
-00000560: 6e69 6373 2064 6576 6963 6573 2068 6176  nics devices hav
-00000570: 6520 6275 696c 742d 696e 206e 6174 6976  e built-in nativ
-00000580: 6520 6361 6d65 7261 732c 2061 6e64 2074  e cameras, and t
-00000590: 6865 2063 7572 7265 6e74 2073 7461 7465  he current state
-000005a0: 206f 6620 7265 7365 6172 6368 2069 6e64   of research ind
-000005b0: 6963 6174 6573 2074 6861 7420 6974 2069  icates that it i
-000005c0: 7320 6163 6869 6576 6162 6c65 2074 6f20  s achievable to 
-000005d0: 6861 7665 2065 7965 2074 7261 636b 696e  have eye trackin
-000005e0: 6720 6174 2072 6561 736f 6e61 626c 6520  g at reasonable 
-000005f0: 6163 6375 7261 6379 2062 6173 6564 206f  accuracy based o
-00000600: 6e20 7468 6f73 6520 6e61 7469 7665 2063  n those native c
-00000610: 616d 6572 6173 2e20 0a0a 4f75 7220 6d69  ameras. ..Our mi
-00000620: 7373 696f 6e20 6973 2074 6f20 6272 696e  ssion is to brin
-00000630: 6720 6579 652d 7472 6163 6b69 6e67 2074  g eye-tracking t
-00000640: 6563 686e 6f6c 6f67 7920 746f 2061 7320  echnology to as 
-00000650: 6d61 6e79 2070 656f 706c 6520 6173 2070  many people as p
-00000660: 6f73 7369 626c 652e 200a 0a4f 7572 2074  ossible. ..Our t
-00000670: 6563 686e 6f6c 6f67 7920 6973 206e 6f74  echnology is not
-00000680: 2070 6572 6665 6374 2c20 6275 7420 7765   perfect, but we
-00000690: 2073 7472 6976 6520 746f 2062 652e 0a0a   strive to be...
-000006a0: 2323 2320 f09f 9387 2046 696e 6420 7573  ### .... Find us
-000006b0: 3a0a 2d20 5b52 5353 5d28 6874 7470 733a  :.- [RSS](https:
-000006c0: 2f2f 706f 6c61 722e 7368 2f4e 6174 6976  //polar.sh/Nativ
-000006d0: 6553 656e 736f 7273 2f72 7373 3f61 7574  eSensors/rss?aut
-000006e0: 683d 6579 4a68 6247 6369 4f69 4a49 557a  h=eyJhbGciOiJIUz
-000006f0: 4931 4e69 4973 496e 5235 6343 4936 496b  I1NiIsInR5cCI6Ik
-00000700: 7058 5643 4a39 2e65 794a 7759 5852 6661  pXVCJ9.eyJwYXRfa
-00000710: 5751 694f 694a 6b4d 4459 784d 4446 694f  WQiOiJkMDYxMDFiO
-00000720: 4330 7859 7a59 794c 5451 314d 5459 7459  C0xYzYyLTQ1MTYtY
-00000730: 6a67 3359 5330 334e 5446 684f 544d 334f  jg3YS03NTFhOTM3O
-00000740: 5449 785a 6d55 694c 434a 7a59 3239 775a  TIxZmUiLCJzY29wZ
-00000750: 584d 694f 694a 6863 6e52 7059 3278 6c63  XMiOiJhcnRpY2xlc
-00000760: 7a70 795a 5746 6b49 6977 6964 486c 775a  zpyZWFkIiwidHlwZ
-00000770: 5349 3649 6d46 3164 4767 694c 434a 6c65  SI6ImF1dGgiLCJle
-00000780: 4841 694f 6a45 334e 444d 784e 6a67 334f  HAiOjE3NDMxNjg3O
-00000790: 4468 392e 646a 6f69 3541 5257 4872 2d78  Dh9.djoi5ARWHr-x
-000007a0: 4657 5f58 4a36 4677 616c 334a 5554 3166  FW_XJ6Fwal3JUT1f
-000007b0: 4162 7678 344e 706c 2d64 6142 4335 5529  Abvx4Npl-daBC5U)
-000007c0: 0a2d 205b 6469 7363 6f72 645d 2868 7474  .- [discord](htt
-000007d0: 7073 3a2f 2f64 6973 636f 7264 2e67 672f  ps://discord.gg/
-000007e0: 4656 3352 5954 7556 290a 2d20 5b74 7769  FV3RYTuV).- [twi
-000007f0: 7474 6572 5d28 6874 7470 733a 2f2f 7477  tter](https://tw
-00000800: 6974 7465 722e 636f 6d2f 5057 346c 747a  itter.com/PW4ltz
-00000810: 290a 2d20 656d 6169 6c3a 2063 6f6e 7461  ).- email: conta
-00000820: 6374 4065 7965 6765 7374 7572 6573 2e63  ct@eyegestures.c
-00000830: 6f6d 0a0a 466f 6c6c 6f77 2075 7320 6f6e  om..Follow us on
-00000840: 2070 6f6c 6172 2028 6974 2063 6f73 7473   polar (it costs
-00000850: 206e 6f74 6869 6e67 2062 7574 2079 6f75   nothing but you
-00000860: 2068 656c 7020 7072 6f6a 6563 7421 293a   help project!):
-00000870: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000880: 3a2f 2f70 6f6c 6172 2e73 682f 4e61 7469  ://polar.sh/Nati
-00000890: 7665 5365 6e73 6f72 7322 3e3c 7069 6374  veSensors"><pict
-000008a0: 7572 653e 3c73 6f75 7263 6520 6d65 6469  ure><source medi
-000008b0: 613d 2228 7072 6566 6572 732d 636f 6c6f  a="(prefers-colo
-000008c0: 722d 7363 6865 6d65 3a20 6461 726b 2922  r-scheme: dark)"
-000008d0: 2073 7263 7365 743d 2268 7474 7073 3a2f   srcset="https:/
-000008e0: 2f70 6f6c 6172 2e73 682f 656d 6265 642f  /polar.sh/embed/
-000008f0: 7375 6273 6372 6962 652e 7376 673f 6f72  subscribe.svg?or
-00000900: 673d 4e61 7469 7665 5365 6e73 6f72 7326  g=NativeSensors&
-00000910: 6c61 6265 6c3d 5375 6273 6372 6962 6526  label=Subscribe&
-00000920: 6461 726b 6d6f 6465 223e 3c69 6d67 2061  darkmode"><img a
-00000930: 6c74 3d22 5375 6273 6372 6962 6520 6f6e  lt="Subscribe on
-00000940: 2050 6f6c 6172 2220 7372 633d 2268 7474   Polar" src="htt
-00000950: 7073 3a2f 2f70 6f6c 6172 2e73 682f 656d  ps://polar.sh/em
-00000960: 6265 642f 7375 6273 6372 6962 652e 7376  bed/subscribe.sv
-00000970: 673f 6f72 673d 4e61 7469 7665 5365 6e73  g?org=NativeSens
-00000980: 6f72 7326 6c61 6265 6c3d 5375 6273 6372  ors&label=Subscr
-00000990: 6962 6522 3e3c 2f70 6963 7475 7265 3e3c  ibe"></picture><
-000009a0: 2f61 3e0a 0a23 2323 20f0 9f92 9c20 5370  /a>..### .... Sp
-000009b0: 6f6e 736f 7273 3a20 0a0a 6060 600a 5370  onsors: ..```.Sp
-000009c0: 6f6e 736f 7220 7573 2061 6e64 2077 6520  onsor us and we 
-000009d0: 6361 6e20 6164 6420 796f 7572 206c 696e  can add your lin
-000009e0: 6b2c 2062 616e 6e65 7220 6f72 206f 7468  k, banner or oth
-000009f0: 6572 2070 726f 6d6f 206d 6174 6572 6961  er promo materia
-00000a00: 6c73 210a 6060 600a 0a23 2323 20f0 9f93  ls!.```..### ...
-00000a10: a220 416e 6e6f 756e 6365 6d65 6e74 733a  . Announcements:
-00000a20: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000a30: 3a2f 2f70 6f6c 6172 2e73 682f 4e61 7469  ://polar.sh/Nati
-00000a40: 7665 5365 6e73 6f72 732f 706f 7374 7322  veSensors/posts"
-00000a50: 3e3c 7069 6374 7572 653e 3c73 6f75 7263  ><picture><sourc
-00000a60: 6520 6d65 6469 613d 2228 7072 6566 6572  e media="(prefer
-00000a70: 732d 636f 6c6f 722d 7363 6865 6d65 3a20  s-color-scheme: 
-00000a80: 6461 726b 2922 2073 7263 7365 743d 2268  dark)" srcset="h
-00000a90: 7474 7073 3a2f 2f70 6f6c 6172 2e73 682f  ttps://polar.sh/
-00000aa0: 656d 6265 642f 706f 7374 732e 7376 673f  embed/posts.svg?
-00000ab0: 6f72 673d 4e61 7469 7665 5365 6e73 6f72  org=NativeSensor
-00000ac0: 7326 6461 726b 6d6f 6465 223e 3c69 6d67  s&darkmode"><img
-00000ad0: 2061 6c74 3d22 506f 7374 7320 6f6e 2050   alt="Posts on P
-00000ae0: 6f6c 6172 2220 7372 633d 2268 7474 7073  olar" src="https
-00000af0: 3a2f 2f70 6f6c 6172 2e73 682f 656d 6265  ://polar.sh/embe
-00000b00: 642f 706f 7374 732e 7376 673f 6f72 673d  d/posts.svg?org=
-00000b10: 4e61 7469 7665 5365 6e73 6f72 7322 3e3c  NativeSensors"><
-00000b20: 2f70 6963 7475 7265 3e3c 2f61 3e0a 0a23  /picture></a>..#
-00000b30: 2323 20f0 9f94 a520 5765 6220 4465 6d6f  ## .... Web Demo
-00000b40: 733a 0a0a 2d20 5b4d 6169 6e20 7061 6765  s:..- [Main page
-00000b50: 5d28 6874 7470 733a 2f2f 6579 6567 6573  ](https://eyeges
-00000b60: 7475 7265 732e 636f 6d2f 290a 2d20 5b47  tures.com/).- [G
-00000b70: 616d 6520 6465 6d6f 5d28 6874 7470 733a  ame demo](https:
-00000b80: 2f2f 6579 6567 6573 7475 7265 732e 636f  //eyegestures.co
-00000b90: 6d2f 6761 6d65 290a 2d20 5b43 696e 656d  m/game).- [Cinem
-00000ba0: 6120 6465 6d6f 5d28 6874 7470 733a 2f2f  a demo](https://
-00000bb0: 6579 6567 6573 7475 7265 732e 636f 6d2f  eyegestures.com/
-00000bc0: 6369 6e65 6d61 290a 0a23 2323 20f0 9f92  cinema)..### ...
-00000bd0: bb20 496e 7374 616c 6c0a 6060 600a 7079  . Install.```.py
-00000be0: 6275 696c 642e 7368 203b 2070 7974 686f  build.sh ; pytho
-00000bf0: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
-00000c00: 6c20 6469 7374 2f65 7965 6765 7374 7572  l dist/eyegestur
-00000c10: 6573 2d31 2e32 2e32 2d70 7933 2d6e 6f6e  es-1.2.2-py3-non
-00000c20: 652d 616e 792e 7768 6c0a 6060 600a 0a4e  e-any.whl.```..N
-00000c30: 6f74 653a 2079 6f75 206d 6179 206e 6565  ote: you may nee
-00000c40: 6420 746f 2063 6861 6e67 6520 7665 7273  d to change vers
-00000c50: 696f 6e20 6f66 2070 6163 6b61 6765 2060  ion of package `
-00000c60: 6579 6567 6573 7475 7265 732d 582e 582e  eyegestures-X.X.
-00000c70: 5860 2e0a 0a23 2323 20e2 9a99 efb8 8f20  X`...### ...... 
-00000c80: 5275 6e20 0a60 6060 0a70 7974 686f 6e33  Run .```.python3
-00000c90: 2065 7861 6d70 6c65 732f 7369 6d70 6c65   examples/simple
-00000ca0: 5f65 7861 6d70 6c65 2e70 790a 6060 600a  _example.py.```.
-00000cb0: 0a23 2323 20f0 9f94 a720 4465 7665 6c6f  .### .... Develo
-00000cc0: 7020 0a0a 546f 2062 6567 696e 2c20 796f  p ..To begin, yo
-00000cd0: 7520 696e 7374 616e 7469 6174 6520 616e  u instantiate an
-00000ce0: 2045 7965 4765 7374 7572 6573 206f 626a   EyeGestures obj
-00000cf0: 6563 7420 7769 7468 2069 6e69 7469 616c  ect with initial
-00000d00: 2052 6567 696f 6e20 6f66 2049 6e74 6572   Region of Inter
-00000d10: 6573 7420 2852 6f49 2920 7061 7261 6d65  est (RoI) parame
-00000d20: 7465 7273 2e20 5468 6573 6520 7061 7261  ters. These para
-00000d30: 6d65 7465 7273 2064 6566 696e 6520 6120  meters define a 
-00000d40: 7072 656c 696d 696e 6172 7920 666f 6375  preliminary focu
-00000d50: 7320 6172 6561 2066 6f72 2074 6865 2074  s area for the t
-00000d60: 7261 636b 6572 2077 6974 6869 6e20 6120  racker within a 
-00000d70: 7669 7274 7561 6c20 3530 3078 3530 3020  virtual 500x500 
-00000d80: 7363 7265 656e 2073 7061 6365 2c20 7768  screen space, wh
-00000d90: 6963 6820 6865 6c70 7320 696e 206c 6f63  ich helps in loc
-00000da0: 6174 696e 6720 7468 6520 7573 6572 2773  ating the user's
-00000db0: 2067 617a 6520 6d6f 7265 2065 6666 6963   gaze more effic
-00000dc0: 6965 6e74 6c79 2e0a 0a4d 6169 6e20 6045  iently...Main `E
-00000dd0: 7965 4765 7374 7572 6560 206f 626a 6563  yeGesture` objec
-00000de0: 7420 7072 6f76 6964 6573 2067 656e 6572  t provides gener
-00000df0: 616c 2063 6f6e 6669 6775 7261 7469 6f6e  al configuration
-00000e00: 2069 6e69 7469 616c 2063 6f6e 6469 7469   initial conditi
-00000e10: 6f6e 733a 200a 0a60 6060 7079 7468 6f6e  ons: ..```python
-00000e20: 0a45 7965 4765 7374 7572 6573 2820 200a  .EyeGestures(  .
-00000e30: 2020 726f 695f 7820 3d20 3238 350a 2020    roi_x = 285.  
-00000e40: 726f 695f 7920 3d20 3131 350a 2020 726f  roi_y = 115.  ro
-00000e50: 695f 7769 6474 6820 3d20 3830 0a20 2072  i_width = 80.  r
-00000e60: 6f69 5f68 6569 6768 7420 3d20 3135 0a29  oi_height = 15.)
-00000e70: 0a60 6060 2020 0a0a 5468 6520 7472 6163  .```  ..The trac
-00000e80: 6b65 7220 6f70 6572 6174 6573 2077 6974  ker operates wit
-00000e90: 6869 6e20 6120 7669 7274 7561 6c20 7363  hin a virtual sc
-00000ea0: 7265 656e 206d 6561 7375 7269 6e67 2035  reen measuring 5
-00000eb0: 3030 7835 3030 2c20 7768 6572 6520 6974  00x500, where it
-00000ec0: 206d 6170 7320 7468 6520 706f 7369 7469   maps the positi
-00000ed0: 6f6e 7320 6f66 2074 6865 2070 7570 696c  ons of the pupil
-00000ee0: 7320 616e 6420 6f74 6865 7220 6372 6974  s and other crit
-00000ef0: 6963 616c 2066 6163 6961 6c20 6665 6174  ical facial feat
-00000f00: 7572 6573 2074 6f20 6465 6475 6365 2074  ures to deduce t
-00000f10: 6865 2075 7365 7227 7320 6761 7a65 2064  he user's gaze d
-00000f20: 6972 6563 7469 6f6e 2e20 5769 7468 696e  irection. Within
-00000f30: 2074 6869 7320 7370 6163 652c 2074 6865   this space, the
-00000f40: 2052 6567 696f 6e20 6f66 2049 6e74 6572   Region of Inter
-00000f50: 6573 7420 2852 6f49 2920 7365 7276 6573  est (RoI) serves
-00000f60: 2061 7320 6120 7265 7072 6573 656e 7461   as a representa
-00000f70: 7469 6f6e 206f 6620 7468 6520 7573 6572  tion of the user
-00000f80: 2773 2064 6973 706c 6179 2c20 696e 6665  's display, infe
-00000f90: 7272 6564 2074 6872 6f75 6768 2061 2063  rred through a c
-00000fa0: 6f6d 6269 6e61 7469 6f6e 206f 6620 6579  ombination of ey
-00000fb0: 6520 6d6f 7665 6d65 6e74 2061 6e64 2065  e movement and e
-00000fc0: 6467 6520 6465 7465 6374 696f 6e20 6475  dge detection du
-00000fd0: 7269 6e67 2063 616c 6962 7261 7469 6f6e  ring calibration
-00000fe0: 2e0a 0a41 6674 6572 206c 6f63 6174 696e  ...After locatin
-00000ff0: 6720 7468 6520 526f 4920 7769 7468 696e  g the RoI within
-00001000: 2074 6865 2035 3030 7835 3030 2073 7061   the 500x500 spa
-00001010: 6365 2c20 6974 7320 6469 6d65 6e73 696f  ce, its dimensio
-00001020: 6e73 2061 7265 2061 646a 7573 7465 6420  ns are adjusted 
-00001030: 746f 2066 6974 2074 6865 2072 6573 6f6c  to fit the resol
-00001040: 7574 696f 6e20 7573 6564 2069 6e20 7468  ution used in th
-00001050: 6520 6573 7469 6d61 7465 2066 756e 6374  e estimate funct
-00001060: 696f 6e2c 2074 7970 6963 616c 6c79 2064  ion, typically d
-00001070: 6573 6372 6962 6564 2061 7320 6064 6973  escribed as `dis
-00001080: 706c 6179 5f77 6964 7468 6020 6279 2060  play_width` by `
-00001090: 6469 7370 6c61 795f 6865 6967 6874 602e  display_height`.
-000010a0: 0a0a 4361 6c69 6272 6174 696f 6e20 6169  ..Calibration ai
-000010b0: 6d73 2074 6f20 7072 6563 6973 656c 7920  ms to precisely 
-000010c0: 6465 7465 726d 696e 6520 7468 6520 526f  determine the Ro
-000010d0: 4927 7320 6469 6d65 6e73 696f 6e73 2e20  I's dimensions. 
-000010e0: 5072 696f 7220 746f 2063 616c 6962 7261  Prior to calibra
-000010f0: 7469 6f6e 2c20 7468 6520 7472 6163 6b65  tion, the tracke
-00001100: 7220 7265 6c69 6573 206f 6e20 696e 6974  r relies on init
-00001110: 6961 6c20 6f70 7469 6f6e 616c 2070 6172  ial optional par
-00001120: 616d 6574 6572 732c 2069 6e63 6c75 6469  ameters, includi
-00001130: 6e67 3a0a 0a2d 2060 726f 695f 7860 3a20  ng:..- `roi_x`: 
-00001140: 5468 6520 696e 6974 6961 6c20 782d 636f  The initial x-co
-00001150: 6f72 6469 6e61 7465 206f 6620 7468 6520  ordinate of the 
-00001160: 526f 4920 2872 616e 6769 6e67 2066 726f  RoI (ranging fro
-00001170: 6d20 3020 746f 2035 3030 292e 0a2d 2060  m 0 to 500)..- `
-00001180: 726f 695f 7960 3a20 5468 6520 696e 6974  roi_y`: The init
-00001190: 6961 6c20 792d 636f 6f72 6469 6e61 7465  ial y-coordinate
-000011a0: 206f 6620 7468 6520 526f 4920 2872 616e   of the RoI (ran
-000011b0: 6769 6e67 2066 726f 6d20 3020 746f 2035  ging from 0 to 5
-000011c0: 3030 292e 0a2d 2060 726f 695f 7769 6474  00)..- `roi_widt
-000011d0: 6860 3a20 5468 6520 696e 6974 6961 6c20  h`: The initial 
-000011e0: 7769 6474 6820 6f66 2074 6865 2052 6f49  width of the RoI
-000011f0: 2062 6566 6f72 6520 6361 6c69 6272 6174   before calibrat
-00001200: 696f 6e20 2872 616e 6769 6e67 2066 726f  ion (ranging fro
-00001210: 6d20 3020 746f 2035 3030 202d 2078 292e  m 0 to 500 - x).
-00001220: 0a2d 2060 726f 695f 6865 6967 6874 603a  .- `roi_height`:
-00001230: 2054 6865 2069 6e69 7469 616c 2068 6569   The initial hei
-00001240: 6768 7420 6f66 2074 6865 2052 6f49 2062  ght of the RoI b
-00001250: 6566 6f72 6520 6361 6c69 6272 6174 696f  efore calibratio
-00001260: 6e20 2872 616e 6769 6e67 2066 726f 6d20  n (ranging from 
-00001270: 3020 746f 2035 3030 202d 2078 292e 0a0a  0 to 500 - x)...
-00001280: 4e65 7874 2070 6172 7420 6973 206f 6274  Next part is obt
-00001290: 6169 6e69 6e67 2065 7374 696d 6174 696f  aining estimatio
-000012a0: 6e73 2066 726f 6d20 6361 6d65 7261 2066  ns from camera f
-000012b0: 7261 6d65 7320 2869 6620 796f 7520 6361  rames (if you ca
-000012c0: 6e6e 6f74 2067 6574 2065 7374 696d 6174  nnot get estimat
-000012d0: 696f 6e73 2c20 796f 7520 6d61 7920 7472  ions, you may tr
-000012e0: 7920 746f 2063 6861 6e67 6520 636f 6c6f  y to change colo
-000012f0: 7220 636f 6469 6e67 206f 7220 726f 7461  r coding or rota
-00001300: 7469 6f6e 206f 6620 696d 6167 6520 2d20  tion of image - 
-00001310: 6368 6563 6b20 6073 696d 706c 655f 6578  check `simple_ex
-00001320: 616d 706c 652e 7079 6029 2e0a 0a60 6060  ample.py`)...```
-00001330: 7079 7468 6f6e 0a65 7665 6e74 203d 2067  python.event = g
-00001340: 6573 7475 7265 732e 6573 7469 6d61 7465  estures.estimate
-00001350: 280a 2020 2020 696d 6167 6520 3d20 6672  (.    image = fr
-00001360: 616d 652c 0a20 2020 2063 6f6e 7465 7874  ame,.    context
-00001370: 203d 2022 6d61 696e 222c 0a20 2020 2063   = "main",.    c
-00001380: 616c 6962 7261 7469 6f6e 203d 2054 7275  alibration = Tru
-00001390: 652c 2023 2073 6574 2063 616c 6962 7261  e, # set calibra
-000013a0: 7469 6f6e 202d 2073 7769 7463 6820 746f  tion - switch to
-000013b0: 2046 616c 7365 2074 6f20 7374 6f70 2063   False to stop c
-000013c0: 616c 6962 7261 7469 6f6e 0a20 2020 2064  alibration.    d
-000013d0: 6973 706c 6179 5f77 6964 7468 203d 2073  isplay_width = s
-000013e0: 6372 6565 6e5f 7769 6474 682c 0a20 2020  creen_width,.   
-000013f0: 2064 6973 706c 6179 5f68 6569 6768 7420   display_height 
-00001400: 3d20 7363 7265 656e 5f68 6569 6768 742c  = screen_height,
-00001410: 0a20 2020 2064 6973 706c 6179 5f6f 6666  .    display_off
-00001420: 7365 745f 7820 3d20 302c 200a 2020 2020  set_x = 0, .    
-00001430: 6469 7370 6c61 795f 6f66 6673 6574 5f79  display_offset_y
-00001440: 203d 2030 2c20 0a20 2020 2066 6978 6174   = 0, .    fixat
-00001450: 696f 6e5f 6672 6565 7a65 203d 2030 2e38  ion_freeze = 0.8
-00001460: 2c0a 2020 2020 6672 6565 7a65 5f72 6164  ,.    freeze_rad
-00001470: 6975 7320 3d20 3130 290a 6060 600a 0a2d  ius = 10).```..-
-00001480: 2060 696d 6167 6560 202d 2069 7320 6376   `image` - is cv
-00001490: 3220 696d 6167 6520 6672 616d 650a 2d20  2 image frame.- 
-000014a0: 6063 6f6e 7465 7874 6020 2d20 6973 206e  `context` - is n
-000014b0: 616d 6520 6769 7665 6e20 746f 2063 6f6e  ame given to con
-000014c0: 7465 6374 2e20 4966 206e 616d 6520 6368  tect. If name ch
-000014d0: 616e 6765 7320 7468 656e 2064 6966 6665  anges then diffe
-000014e0: 7265 6e74 2074 7261 636b 6572 2063 6f6e  rent tracker con
-000014f0: 7465 7874 2069 7320 7573 6564 2e20 5472  text is used. Tr
-00001500: 6163 6b65 7220 7265 6d62 6572 7320 7072  acker rembers pr
-00001510: 6576 696f 7573 2070 6f69 6e74 7320 746f  evious points to
-00001520: 2065 7374 696d 6174 6520 6e65 7720 6f6e   estimate new on
-00001530: 652c 2062 7574 2074 686f 7365 2070 6f69  e, but those poi
-00001540: 6e74 7320 6172 6520 6173 7369 6e67 6564  nts are assinged
-00001550: 2074 6f20 7369 6e67 6c65 2063 6f6e 7465   to single conte
-00001560: 7874 2e20 4279 2063 6861 6e67 696e 6720  xt. By changing 
-00001570: 6e61 6d65 7320 6f72 2070 6173 7369 6e67  names or passing
-00001580: 206e 6577 206f 6e65 7320 796f 7520 6361   new ones you ca
-00001590: 6e20 7377 6974 6368 2061 6e64 2063 7265  n switch and cre
-000015a0: 6174 6520 636f 6e74 6578 7465 732e 0a2d  ate contextes..-
-000015b0: 2060 6361 6c69 6272 6174 696f 6e60 202d   `calibration` -
-000015c0: 2069 6620 6054 7275 6560 2074 6865 6e20   if `True` then 
-000015d0: 6576 6572 7920 6665 7720 7365 636f 6e64  every few second
-000015e0: 7320 7472 6163 6b65 7220 6973 2072 6563  s tracker is rec
-000015f0: 616c 6962 7261 7469 6e67 2c20 6966 2060  alibrating, if `
-00001600: 4661 6c73 6560 2074 6865 6e20 7472 6163  False` then trac
-00001610: 6b65 7220 7365 7474 696e 6720 6973 2066  ker setting is f
-00001620: 726f 7a65 6e2e 2054 6865 2062 6573 7420  rozen. The best 
-00001630: 6170 7072 6f61 6368 2069 7320 746f 2065  approach is to e
-00001640: 6e61 626c 6520 6361 6c69 6272 6174 696f  nable calibratio
-00001650: 6e20 7768 656e 206f 6e65 206f 6620 7468  n when one of th
-00001660: 6520 6564 6765 7320 6973 2072 6561 6368  e edges is reach
-00001670: 6564 2e20 0a2d 2060 6469 7370 6c61 795f  ed. .- `display_
-00001680: 7769 6474 6860 202d 2077 6964 7468 206f  width` - width o
-00001690: 6620 6469 7370 6c61 792f 7363 7265 656e  f display/screen
-000016a0: 2075 7365 642e 0a2d 2060 6469 7370 6c61   used..- `displa
-000016b0: 795f 6865 6967 6874 6020 2d20 6865 6967  y_height` - heig
-000016c0: 6874 206f 6620 6469 7370 6c61 792f 7363  ht of display/sc
-000016d0: 7265 656e 2075 7365 642e 0a2d 2060 6469  reen used..- `di
-000016e0: 7370 6c61 795f 6f66 6673 6574 5f78 6020  splay_offset_x` 
-000016f0: 2d20 6f66 6673 6574 206f 6620 7820 666f  - offset of x fo
-00001700: 7220 6469 7370 6c61 792f 7363 7265 656e  r display/screen
-00001710: 2075 7365 642e 2055 7365 2069 7420 7768   used. Use it wh
-00001720: 656e 2068 6176 696e 6720 7477 6f20 6469  en having two di
-00001730: 7370 6c61 7973 2061 6e64 2061 7070 2069  splays and app i
-00001740: 7320 636f 7665 7269 6e67 2061 6c6c 2073  s covering all s
-00001750: 6372 6565 6e73 2c20 6275 7420 796f 7520  creens, but you 
-00001760: 7761 6e74 2074 6f20 6c69 6d69 7420 796f  want to limit yo
-00001770: 7572 2063 7572 736f 7220 7472 6163 6b65  ur cursor tracke
-00001780: 7220 746f 206f 6e6c 7920 7370 6563 6966  r to only specif
-00001790: 6963 2064 6973 706c 6179 2e0a 2d20 6064  ic display..- `d
-000017a0: 6973 706c 6179 5f6f 6666 7365 745f 7960  isplay_offset_y`
-000017b0: 202d 206f 6666 7365 7420 6f66 2079 2066   - offset of y f
-000017c0: 6f72 2064 6973 706c 6179 2f73 6372 6565  or display/scree
-000017d0: 6e20 7573 6564 2e20 5573 6520 6974 2077  n used. Use it w
-000017e0: 6865 6e20 6861 7669 6e67 2074 776f 2064  hen having two d
-000017f0: 6973 706c 6179 7320 616e 6420 6170 7020  isplays and app 
-00001800: 6973 2063 6f76 6572 696e 6720 616c 6c20  is covering all 
-00001810: 7363 7265 656e 732c 2062 7574 2079 6f75  screens, but you
-00001820: 2077 616e 7420 746f 206c 696d 6974 2079   want to limit y
-00001830: 6f75 7220 6375 7273 6f72 2074 7261 636b  our cursor track
-00001840: 6572 2074 6f20 6f6e 6c79 2073 7065 6369  er to only speci
-00001850: 6669 6320 6469 7370 6c61 792e 0a2d 2060  fic display..- `
-00001860: 6669 7861 7469 6f6e 5f66 7265 657a 6560  fixation_freeze`
-00001870: 202d 2074 6872 6573 686f 6c64 206f 6620   - threshold of 
-00001880: 7573 6572 2066 6978 6174 696f 6e20 6f6e  user fixation on
-00001890: 206f 6e65 2070 6f69 6e74 2028 6974 2067   one point (it g
-000018a0: 6f65 7320 6672 6f6d 2030 2e30 2074 6f20  oes from 0.0 to 
-000018b0: 312e 3029 2e20 4966 2074 6872 6573 686f  1.0). If thresho
-000018c0: 6c64 2069 7320 6372 6f73 7365 6420 706f  ld is crossed po
-000018d0: 696e 7420 6973 2066 726f 7a65 6e20 7469  int is frozen ti
-000018e0: 6c6c 2075 7365 7220 6272 6561 6b73 2060  ll user breaks `
-000018f0: 6672 6565 7a65 5f72 6164 6975 7360 2069  freeze_radius` i
-00001900: 6e20 7069 7865 6c73 2e0a 2d20 6066 7265  n pixels..- `fre
-00001910: 657a 655f 7261 6469 7573 6020 2d20 6469  eze_radius` - di
-00001920: 7374 616e 6365 2063 7572 736f 7220 6361  stance cursor ca
-00001930: 6e20 6d6f 7665 2074 6f20 7265 6163 6820  n move to reach 
-00001940: 6669 7861 7469 6f6e 2061 6e64 2066 7265  fixation and fre
-00001950: 657a 696e 672c 2069 6620 6375 7273 6f72  ezing, if cursor
-00001960: 206d 6f76 656d 656e 7473 2061 7265 2067   movements are g
-00001970: 7265 6174 6572 2074 6861 6e20 6469 7374  reater than dist
-00001980: 616e 6365 2074 6865 6e20 6669 7861 7469  ance then fixati
-00001990: 6f6e 206d 6561 7375 7265 6d65 6e74 2067  on measurement g
-000019a0: 6f65 7320 646f 776e 2074 6f20 6030 2e30  oes down to `0.0
-000019b0: 602e 0a0a 6060 600a 4765 7665 6e74 2065  `...```.Gevent e
-000019c0: 7665 6e74 0a60 6060 0a0a 6047 6576 656e  vent.```..`Geven
-000019d0: 7460 2069 7320 7265 7475 726e 6564 2065  t` is returned e
-000019e0: 6c65 6d65 6e74 2068 6176 696e 6720 616c  lement having al
-000019f0: 6c20 6461 7461 206e 6563 6573 7361 7279  l data necessary
-00001a00: 2074 6f20 7573 6520 7472 6163 6b65 723a   to use tracker:
-00001a10: 0a20 0a2d 2060 706f 696e 745f 7363 7265  . .- `point_scre
-00001a20: 656e 6020 6973 2070 6f69 6e74 2063 6f6f  en` is point coo
-00001a30: 7264 696e 6174 6573 206f 6e20 7363 7265  rdinates on scre
-00001a40: 656e 0a2d 2060 626c 696e 6b60 2069 7320  en.- `blink` is 
-00001a50: 626f 6f6c 6561 6e20 7661 6c75 6520 6465  boolean value de
-00001a60: 7363 7269 6269 6e67 2062 6c69 6e6b 2065  scribing blink e
-00001a70: 7665 6e74 2e20 4966 2060 3060 206e 6f20  vent. If `0` no 
-00001a80: 626c 696e 6b20 6f63 6375 7265 642c 2069  blink occured, i
-00001a90: 6620 6031 6020 626c 696e 6b20 6f63 6375  f `1` blink occu
-00001aa0: 7265 642e 0a2d 2060 6669 7861 7469 6f6e  red..- `fixation
-00001ab0: 6020 7661 6c75 6520 6672 6f6d 2060 302e  ` value from `0.
-00001ac0: 3060 2074 6f20 6031 2e30 6020 6465 7363  0` to `1.0` desc
-00001ad0: 7269 6269 6e67 206c 6576 656c 206f 6620  ribing level of 
-00001ae0: 7573 6572 2066 6978 6174 696f 6e2e 0a0a  user fixation...
-00001af0: 456e 7469 7265 2070 726f 6772 616d 3a20  Entire program: 
-00001b00: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-00001b10: 7274 2056 6964 656f 4361 7074 7572 6520  rt VideoCapture 
-00001b20: 2363 6861 6e67 6520 6974 2074 6f20 6f70  #change it to op
-00001b30: 656e 6376 2066 6f72 2072 6561 6c20 6170  encv for real ap
-00001b40: 706c 6963 6174 696f 6e73 0a66 726f 6d20  plications.from 
-00001b50: 6579 6547 6573 7475 7265 732e 7574 696c  eyeGestures.util
-00001b60: 7320 696d 706f 7274 2056 6964 656f 4361  s import VideoCa
-00001b70: 7074 7572 650a 6672 6f6d 2065 7965 4765  pture.from eyeGe
-00001b80: 7374 7572 6573 2e65 7965 6765 7374 7572  stures.eyegestur
-00001b90: 6573 2069 6d70 6f72 7420 4579 6547 6573  es import EyeGes
-00001ba0: 7475 7265 730a 0a67 6573 7475 7265 7320  tures..gestures 
-00001bb0: 3d20 4579 6547 6573 7475 7265 7328 0a20  = EyeGestures(. 
-00001bc0: 2072 6f69 5f78 203d 2032 3835 0a20 2072   roi_x = 285.  r
-00001bd0: 6f69 5f79 203d 2031 3135 0a20 2072 6f69  oi_y = 115.  roi
-00001be0: 5f77 6964 7468 203d 2038 300a 2020 726f  _width = 80.  ro
-00001bf0: 695f 6865 6967 6874 203d 2031 350a 290a  i_height = 15.).
-00001c00: 0a63 6170 203d 2056 6964 656f 4361 7074  .cap = VideoCapt
-00001c10: 7572 6528 3029 2020 0a0a 2320 4d61 696e  ure(0)  ..# Main
-00001c20: 2067 616d 6520 6c6f 6f70 0a72 756e 6e69   game loop.runni
-00001c30: 6e67 203d 2054 7275 650a 7768 696c 6520  ng = True.while 
-00001c40: 7275 6e6e 696e 673a 0a0a 2020 2020 2320  running:..    # 
-00001c50: 4765 6e65 7261 7465 206e 6577 2072 616e  Generate new ran
-00001c60: 646f 6d20 706f 7369 7469 6f6e 2066 6f72  dom position for
-00001c70: 2074 6865 2063 7572 736f 720a 2020 2020   the cursor.    
-00001c80: 7265 742c 2066 7261 6d65 203d 2063 6170  ret, frame = cap
-00001c90: 2e72 6561 6428 2920 2020 2020 0a0a 2020  .read()     ..  
-00001ca0: 2020 6576 656e 7420 3d20 6765 7374 7572    event = gestur
-00001cb0: 6573 2e65 7374 696d 6174 6528 0a20 2020  es.estimate(.   
-00001cc0: 2020 2020 2066 7261 6d65 2c0a 2020 2020       frame,.    
-00001cd0: 2020 2020 226d 6169 6e22 2c0a 2020 2020      "main",.    
-00001ce0: 2020 2020 5472 7565 2c20 2320 7365 7420      True, # set 
-00001cf0: 6361 6c69 6272 6174 696f 6e20 2d20 7377  calibration - sw
-00001d00: 6974 6368 2074 6f20 4661 6c73 6520 746f  itch to False to
-00001d10: 2073 746f 7020 6361 6c69 6272 6174 696f   stop calibratio
-00001d20: 6e0a 2020 2020 2020 2020 7363 7265 656e  n.        screen
-00001d30: 5f77 6964 7468 2c0a 2020 2020 2020 2020  _width,.        
-00001d40: 7363 7265 656e 5f68 6569 6768 742c 0a20  screen_height,. 
-00001d50: 2020 2020 2020 2030 2c20 302c 2030 2e38         0, 0, 0.8
-00001d60: 2c31 3029 0a0a 2020 2020 6375 7273 6f72  ,10)..    cursor
-00001d70: 5f78 2c20 6375 7273 6f72 5f79 203d 2065  _x, cursor_y = e
-00001d80: 7665 6e74 2e70 6f69 6e74 5f73 6372 6565  vent.point_scree
-00001d90: 6e5b 305d 2c65 7665 6e74 2e70 6f69 6e74  n[0],event.point
-00001da0: 5f73 6372 6565 6e5b 315d 0a0a 6060 600a  _screen[1]..```.
-00001db0: 0a0a 2323 2320 f09f 8c90 2057 6562 2045  ..### .... Web E
-00001dc0: 6d62 6564 6420 5b50 6169 6420 4150 495d  mbedd [Paid API]
-00001dd0: 0a0a 466f 7220 6e6f 7720 6d6f 7265 2069  ..For now more i
-00001de0: 6e66 6f20 6361 6e20 6265 2066 6f75 6e64  nfo can be found
-00001df0: 2068 6572 653a 2068 7474 7073 3a2f 2f65   here: https://e
-00001e00: 7965 6765 7374 7572 6573 2e63 6f6d 2f75  yegestures.com/u
-00001e10: 7365 725f 706f 7274 616c 0a0a 6060 6068  ser_portal..```h
-00001e20: 746d 6c0a 2f2f 202e 2e2e 2072 6573 7420  tml.// ... rest 
-00001e30: 6f66 2068 746d 6c20 636c 6965 6e74 202e  of html client .
-00001e40: 2e2e 0a0a 3c73 6372 6970 743e 0a2f 2f20  ....<script>.// 
-00001e50: 2e2e 2e20 796f 7572 2063 6f64 6520 2e2e  ... your code ..
-00001e60: 2e0a 0a66 756e 6374 696f 6e20 6f6e 5469  ...function onTi
-00001e70: 6c65 2869 642c 2066 6978 2c20 626c 696e  le(id, fix, blin
-00001e80: 6b29 207b 0a20 202f 2f20 2e2e 2e20 646f  k) {.  // ... do
-00001e90: 2073 6f6d 6574 6869 6e67 2068 6572 6520   something here 
-00001ea0: 2e2e 2e0a 7d0a 0a66 756e 6374 696f 6e20  ....}..function 
-00001eb0: 6f6e 4361 6c69 6272 6174 696f 6e28 2920  onCalibration() 
-00001ec0: 7b0a 2020 2f2f 202e 2e2e 2064 6f20 736f  {.  // ... do so
-00001ed0: 6d65 7468 696e 6720 6865 7265 202e 2e2e  mething here ...
-00001ee0: 0a7d 0a3c 2f73 6372 6970 743e 0a3c 7363  .}.</script>.<sc
-00001ef0: 7269 7074 2073 7263 3d22 6874 7470 733a  ript src="https:
-00001f00: 2f2f 6364 6e6a 732e 636c 6f75 6466 6c61  //cdnjs.cloudfla
-00001f10: 7265 2e63 6f6d 2f61 6a61 782f 6c69 6273  re.com/ajax/libs
-00001f20: 2f73 6f63 6b65 742e 696f 2f34 2e30 2e30  /socket.io/4.0.0
-00001f30: 2f73 6f63 6b65 742e 696f 2e6a 7322 3e3c  /socket.io.js"><
-00001f40: 2f73 6372 6970 743e 0a3c 7363 7269 7074  /script>.<script
-00001f50: 2073 7263 3d22 6874 7470 733a 2f2f 6579   src="https://ey
-00001f60: 6567 6573 7475 7265 732e 636f 6d2f 6579  egestures.com/ey
-00001f70: 6554 696c 6573 2e6d 696e 2e6a 7322 3e3c  eTiles.min.js"><
-00001f80: 2f73 6372 6970 743e 0a3c 7363 7269 7074  /script>.<script
-00001f90: 3e0a 2020 4579 6554 696c 6573 4150 4928  >.  EyeTilesAPI(
-00001fa0: 0a20 2020 206b 6579 203d 2022 594f 5552  .    key = "YOUR
-00001fb0: 5f41 5049 5f4b 4559 222c 0a20 2020 2074  _API_KEY",.    t
-00001fc0: 696c 6573 203d 205b 312c 2032 2c20 315d  iles = [1, 2, 1]
-00001fd0: 2c0a 2020 2020 6669 7854 6872 6573 6820  ,.    fixThresh 
-00001fe0: 3d20 302e 312c 0a20 2020 2066 6978 5261  = 0.1,.    fixRa
-00001ff0: 6469 7573 203d 2035 3030 2c0a 2020 2020  dius = 500,.    
-00002000: 7369 6768 7447 7269 6420 3d20 7472 7565  sightGrid = true
-00002010: 2c0a 2020 2020 6f6e 5469 6c65 203d 206f  ,.    onTile = o
-00002020: 6e54 696c 652c 0a20 2020 206f 6e43 616c  nTile,.    onCal
-00002030: 6962 7261 7469 6f6e 203d 206f 6e43 616c  ibration = onCal
-00002040: 6962 7261 7469 6f6e 2c0a 2020 293b 0a3c  ibration,.  );.<
-00002050: 2f73 6372 6970 743e 2020 2020 0a60 6060  /script>    .```
-00002060: 0a0a 2323 2320 7275 6c65 7320 6f66 2075  ..### rules of u
-00002070: 7369 6e67 0a0a 4966 2079 6f75 2061 7265  sing..If you are
-00002080: 2062 7569 6c64 696e 6720 7075 626c 6963   building public
-00002090: 6c79 2061 7661 696c 6162 6c65 2070 726f  ly available pro
-000020a0: 6475 6374 2c20 616e 6420 6861 7665 206e  duct, and have n
-000020b0: 6f20 636f 6d6d 6572 6369 616c 206c 6963  o commercial lic
-000020c0: 656e 7365 2c20 706c 6561 7365 206d 656e  ense, please men
-000020d0: 7469 6f6e 2075 7320 736f 6d65 7768 6572  tion us somewher
-000020e0: 6520 696e 2079 6f75 7220 696e 7465 7266  e in your interf
-000020f0: 6163 652e 200a 0a2a 2a50 726f 6d6f 204d  ace. ..**Promo M
-00002100: 6174 6572 6961 6c73 3a2a 2a0a 0a68 7474  aterials:**..htt
-00002110: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002120: 4e61 7469 7665 5365 6e73 6f72 732f 4579  NativeSensors/Ey
-00002130: 6547 6573 7475 7265 732f 6173 7365 7473  eGestures/assets
-00002140: 2f34 3037 3733 3535 302f 3463 6138 3432  /40773550/4ca842
-00002150: 6239 2d62 6133 322d 3466 6664 2d62 3265  b9-ba32-4ffd-b2e
-00002160: 342d 3137 3966 6636 3765 6534 3766 0a0a  4-179ff67ee47f..
-00002170: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00002180: 2f2f 6769 7468 7562 2e63 6f6d 2f4e 6174  //github.com/Nat
-00002190: 6976 6553 656e 736f 7273 2f45 7965 4765  iveSensors/EyeGe
-000021a0: 7374 7572 6573 2f61 7373 6574 732f 3430  stures/assets/40
-000021b0: 3737 3335 3530 2f34 6361 3834 3262 392d  773550/4ca842b9-
-000021c0: 6261 3332 2d34 6666 642d 6232 6534 2d31  ba32-4ffd-b2e4-1
-000021d0: 3739 6666 3637 6565 3437 6622 2077 6964  79ff67ee47f" wid
-000021e0: 7468 3d22 3330 300a 223e 0a0a 6874 7470  th="300.">..http
-000021f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
-00002200: 6174 6976 6553 656e 736f 7273 2f45 7965  ativeSensors/Eye
-00002210: 4765 7374 7572 6573 2f61 7373 6574 732f  Gestures/assets/
-00002220: 3430 3737 3335 3530 2f36 6137 6337 3462  40773550/6a7c74b
-00002230: 352d 6230 3639 2d34 6565 632d 6263 3936  5-b069-4eec-bc96
-00002240: 2d33 6136 6262 3431 3539 6233 370a 0a3c  -3a6bb4159b37..<
-00002250: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00002260: 2f67 6974 6875 622e 636f 6d2f 4e61 7469  /github.com/Nati
-00002270: 7665 5365 6e73 6f72 732f 4579 6547 6573  veSensors/EyeGes
-00002280: 7475 7265 732f 6173 7365 7473 2f34 3037  tures/assets/407
-00002290: 3733 3535 302f 3661 3763 3734 6235 2d62  73550/6a7c74b5-b
-000022a0: 3036 392d 3465 6563 2d62 6339 362d 3361  069-4eec-bc96-3a
-000022b0: 3662 6234 3135 3962 3337 2220 7769 6474  6bb4159b37" widt
-000022c0: 683d 2232 3030 0a22 3e0a 0a0a 2323 2320  h="200.">...### 
-000022d0: f09f 92bb 2043 6f6e 7472 6962 7574 6f72  .... Contributor
-000022e0: 730a 0a3c 6120 6872 6566 3d22 6874 7470  s..<a href="http
-000022f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4f  s://github.com/O
-00002300: 574e 4552 2f52 4550 4f2f 6772 6170 6873  WNER/REPO/graphs
-00002310: 2f63 6f6e 7472 6962 7574 6f72 7322 3e0a  /contributors">.
-00002320: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00002330: 733a 2f2f 636f 6e74 7269 622e 726f 636b  s://contrib.rock
-00002340: 732f 696d 6167 653f 7265 706f 3d4e 6174  s/image?repo=Nat
-00002350: 6976 6553 656e 736f 7273 2f45 7965 4765  iveSensors/EyeGe
-00002360: 7374 7572 6573 2220 2f3e 0a3c 2f61 3e0a  stures" />.</a>.
-00002370: 0a23 2323 20f0 9f92 b520 5375 7070 6f72  .### .... Suppor
-00002380: 7420 7468 6520 7072 6f6a 6563 7420 0a0a  t the project ..
-00002390: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000023a0: 2f70 6f6c 6172 2e73 682f 4e61 7469 7665  /polar.sh/Native
-000023b0: 5365 6e73 6f72 732f 7375 6273 6372 6970  Sensors/subscrip
-000023c0: 7469 6f6e 7322 3e3c 7069 6374 7572 653e  tions"><picture>
-000023d0: 3c73 6f75 7263 6520 6d65 6469 613d 2228  <source media="(
-000023e0: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
-000023f0: 6865 6d65 3a20 6461 726b 2922 2073 7263  heme: dark)" src
-00002400: 7365 743d 2268 7474 7073 3a2f 2f70 6f6c  set="https://pol
-00002410: 6172 2e73 682f 656d 6265 642f 7469 6572  ar.sh/embed/tier
-00002420: 732e 7376 673f 6f72 673d 4e61 7469 7665  s.svg?org=Native
-00002430: 5365 6e73 6f72 7326 6461 726b 6d6f 6465  Sensors&darkmode
-00002440: 223e 3c69 6d67 2061 6c74 3d22 5375 6273  "><img alt="Subs
-00002450: 6372 6970 7469 6f6e 2054 6965 7273 206f  cription Tiers o
-00002460: 6e20 506f 6c61 7222 2073 7263 3d22 6874  n Polar" src="ht
-00002470: 7470 733a 2f2f 706f 6c61 722e 7368 2f65  tps://polar.sh/e
-00002480: 6d62 6564 2f74 6965 7273 2e73 7667 3f6f  mbed/tiers.svg?o
-00002490: 7267 3d4e 6174 6976 6553 656e 736f 7273  rg=NativeSensors
-000024a0: 223e 3c2f 7069 6374 7572 653e 3c2f 613e  "></picture></a>
-000024b0: 0a0a 3c70 6963 7475 7265 3e0a 2020 3c73  ..<picture>.  <s
-000024c0: 6f75 7263 650a 2020 2020 6d65 6469 613d  ource.    media=
-000024d0: 2228 7072 6566 6572 732d 636f 6c6f 722d  "(prefers-color-
-000024e0: 7363 6865 6d65 3a20 6461 726b 2922 0a20  scheme: dark)". 
-000024f0: 2020 2073 7263 7365 743d 220a 2020 2020     srcset=".    
-00002500: 2020 6874 7470 733a 2f2f 6170 692e 7374    https://api.st
-00002510: 6172 2d68 6973 746f 7279 2e63 6f6d 2f73  ar-history.com/s
-00002520: 7667 3f72 6570 6f73 3d4e 6174 6976 6553  vg?repos=NativeS
-00002530: 656e 736f 7273 2f45 7965 4765 7374 7572  ensors/EyeGestur
-00002540: 6573 2674 7970 653d 4461 7465 2674 6865  es&type=Date&the
-00002550: 6d65 3d64 6172 6b0a 2020 2020 220a 2020  me=dark.    ".  
-00002560: 2f3e 0a20 203c 736f 7572 6365 0a20 2020  />.  <source.   
-00002570: 206d 6564 6961 3d22 2870 7265 6665 7273   media="(prefers
-00002580: 2d63 6f6c 6f72 2d73 6368 656d 653a 206c  -color-scheme: l
-00002590: 6967 6874 2922 0a20 2020 2073 7263 7365  ight)".    srcse
-000025a0: 743d 220a 2020 2020 2020 6874 7470 733a  t=".      https:
-000025b0: 2f2f 6170 692e 7374 6172 2d68 6973 746f  //api.star-histo
-000025c0: 7279 2e63 6f6d 2f73 7667 3f72 6570 6f73  ry.com/svg?repos
-000025d0: 3d4e 6174 6976 6553 656e 736f 7273 2f45  =NativeSensors/E
-000025e0: 7965 4765 7374 7572 6573 2674 7970 653d  yeGestures&type=
-000025f0: 4461 7465 0a20 2020 2022 0a20 202f 3e0a  Date.    ".  />.
-00002600: 2020 3c69 6d67 0a20 2020 2061 6c74 3d22    <img.    alt="
-00002610: 5374 6172 2048 6973 746f 7279 2043 6861  Star History Cha
-00002620: 7274 220a 2020 2020 7372 633d 2268 7474  rt".    src="htt
-00002630: 7073 3a2f 2f61 7069 2e73 7461 722d 6869  ps://api.star-hi
-00002640: 7374 6f72 792e 636f 6d2f 7376 673f 7265  story.com/svg?re
-00002650: 706f 733d 4e61 7469 7665 5365 6e73 6f72  pos=NativeSensor
-00002660: 732f 4579 6547 6573 7475 7265 7326 7479  s/EyeGestures&ty
-00002670: 7065 3d44 6174 6522 0a20 202f 3e0a 3c2f  pe=Date".  />.</
-00002680: 7069 6374 7572 653e 0a0a                 picture>..
+00000000: 0a0a 215b 5079 5049 202d 2044 6f77 6e6c  ..![PyPI - Downl
+00000010: 6f61 6473 5d28 6874 7470 733a 2f2f 696d  oads](https://im
+00000020: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000030: 692f 646d 2f65 7965 4765 7374 7572 6573  i/dm/eyeGestures
+00000040: 290a 0a60 6060 0a46 6f72 2065 6e74 6572  )..```.For enter
+00000050: 7072 6973 6520 6176 6f69 6469 6e67 2047  prise avoiding G
+00000060: 504c 3320 6c69 6365 6e73 696e 6720 7468  PL3 licensing th
+00000070: 6572 6520 6973 2063 6f6d 6d65 7263 6961  ere is commercia
+00000080: 6c20 6c69 6365 6e73 6521 0a60 6060 0a57  l license!.```.W
+00000090: 6520 6f66 6665 7220 6375 7374 6f6d 2069  e offer custom i
+000000a0: 6e74 6567 7261 7469 6f6e 2061 6e64 206d  ntegration and m
+000000b0: 616e 6167 6564 2073 6572 7669 6365 732e  anaged services.
+000000c0: 2046 6f72 2062 7573 696e 6573 7365 7320   For businesses 
+000000d0: 7265 7175 6972 696e 6720 696e 766f 6963  requiring invoic
+000000e0: 6573 206d 6573 7361 6765 2075 7320 6063  es message us `c
+000000f0: 6f6e 7461 6374 4065 7965 6765 7374 7572  ontact@eyegestur
+00000100: 6573 2e63 6f6d 602e 0a0a 2323 20f0 9f91  es.com`...## ...
+00000110: 81ef b88f 2045 7965 4765 7374 7572 6573  .... EyeGestures
+00000120: 0a0a 4579 6547 6573 7475 7265 7320 6973  ..EyeGestures is
+00000130: 206f 7065 6e20 736f 7572 6365 2065 7965   open source eye
+00000140: 7472 6163 6b69 6e67 2073 6f66 7477 6172  tracking softwar
+00000150: 652f 6c69 6272 6172 7920 7573 696e 6720  e/library using 
+00000160: 6e61 7469 7665 2077 6562 6361 6d73 2061  native webcams a
+00000170: 6e64 2070 686f 6e65 2063 616d 6572 7320  nd phone camers 
+00000180: 666f 7220 6163 6869 6576 696e 6720 6974  for achieving it
+00000190: 7320 676f 616c 2e20 5468 6520 6169 6d20  s goal. The aim 
+000001a0: 6f66 206c 6962 7261 7279 2069 7320 746f  of library is to
+000001b0: 2062 7269 6e67 2061 6363 6573 7369 6269   bring accessibi
+000001c0: 6c69 7479 206f 6620 6579 6574 7261 636b  lity of eyetrack
+000001d0: 696e 6720 616e 6420 6579 6564 7269 7665  ing and eyedrive
+000001e0: 6e20 696e 7465 7266 6163 6573 2077 6974  n interfaces wit
+000001f0: 686f 7574 2072 6571 7569 7265 6d65 6e74  hout requirement
+00000200: 206f 6620 6f62 7461 696e 696e 6720 6578   of obtaining ex
+00000210: 7065 6e73 6976 6520 6861 7264 7761 7265  pensive hardware
+00000220: 2e0a 0a3c 7020 616c 6967 6e3d 2263 656e  ...<p align="cen
+00000230: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
+00000240: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000250: 2e63 6f6d 2f50 6574 6572 5761 4949 6163  .com/PeterWaIIac
+00000260: 652f 5065 7465 7257 6149 4961 6365 2f61  e/PeterWaIIace/a
+00000270: 7373 6574 732f 3430 3737 3335 3530 2f32  ssets/40773550/2
+00000280: 6164 3235 3235 322d 6539 3665 2d34 3764  ad25252-e96e-47d
+00000290: 342d 6232 3566 2d63 3437 6261 3766 3066  4-b25f-c47ba7f0f
+000002a0: 3466 3322 2077 6964 7468 3d22 3330 3022  4f3" width="300"
+000002b0: 2068 6569 6768 743d 2231 3530 223e 0a3c   height="150">.<
+000002c0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000002d0: 2f67 6974 6875 622e 636f 6d2f 5065 7465  /github.com/Pete
+000002e0: 7257 6149 4961 6365 2f50 6574 6572 5761  rWaIIace/PeterWa
+000002f0: 4949 6163 652f 6173 7365 7473 2f34 3037  IIace/assets/407
+00000300: 3733 3535 302f 6633 3133 3238 3433 2d30  73550/f3132843-0
+00000310: 3633 612d 3433 3961 2d38 6531 632d 3233  63a-439a-8e1c-23
+00000320: 3835 6464 6664 6363 6461 2220 7769 6474  85ddfdccda" widt
+00000330: 683d 2233 3030 0a22 2068 6569 6768 743d  h="300." height=
+00000340: 2231 3530 223e 0a3c 2f70 3e0a 3c70 2061  "150">.</p>.<p a
+00000350: 6c69 676e 3d22 6365 6e74 6572 223e 0a3c  lign="center">.<
+00000360: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000370: 2f67 6974 6875 622e 636f 6d2f 4e61 7469  /github.com/Nati
+00000380: 7665 5365 6e73 6f72 732f 4579 6547 6573  veSensors/EyeGes
+00000390: 7475 7265 732f 6173 7365 7473 2f34 3037  tures/assets/407
+000003a0: 3733 3535 302f 3834 6161 3734 3336 2d36  73550/84aa7436-6
+000003b0: 3135 332d 3439 6263 2d62 3865 362d 6363  153-49bc-b8e6-cc
+000003c0: 6461 3533 3566 3235 6536 2922 2077 6964  da535f25e6)" wid
+000003d0: 7468 3d22 3630 300a 2220 6865 6967 6874  th="600." height
+000003e0: 3d22 3330 3022 3e0a 3c2f 703e 0a0a 2323  ="300">.</p>..##
+000003f0: 2320 e2ad 9020 4d69 7373 696f 6e20 0a0a  # ... Mission ..
+00000400: 5468 6572 6520 6973 206e 6f20 6f6e 6520  There is no one 
+00000410: 7369 7a65 2d66 6974 7320 616c 6c20 736f  size-fits all so
+00000420: 6c75 7469 6f6e 2c20 616e 6420 7765 2062  lution, and we b
+00000430: 656c 6965 7665 2074 6861 7420 6469 6666  elieve that diff
+00000440: 6572 656e 7469 6174 696e 6720 696e 7465  erentiating inte
+00000450: 7266 6163 6573 2062 7269 6e67 7320 6163  rfaces brings ac
+00000460: 6365 7373 6962 696c 6974 7920 746f 2064  cessibility to d
+00000470: 6967 6974 616c 2073 7061 6365 732e 2044  igital spaces. D
+00000480: 6573 6967 6e69 6e67 2065 7965 2d64 7269  esigning eye-dri
+00000490: 7665 6e20 696e 7465 7266 6163 6573 2067  ven interfaces g
+000004a0: 6976 6573 206d 6f72 6520 636f 6e74 726f  ives more contro
+000004b0: 6c20 6f76 6572 2063 6f6d 7075 7465 7273  l over computers
+000004c0: 2074 6f20 7468 6f73 6520 7768 6f20 6361   to those who ca
+000004d0: 6e6e 6f74 2066 756c 6c79 2065 6e6a 6f79  nnot fully enjoy
+000004e0: 2074 6865 6972 2063 6170 6162 696c 6974   their capabilit
+000004f0: 6965 7320 6475 6520 746f 2064 6966 6665  ies due to diffe
+00000500: 7265 6e74 2064 6973 6162 696c 6974 6965  rent disabilitie
+00000510: 732c 2061 7320 7765 6c6c 2061 7320 616e  s, as well as an
+00000520: 2061 6464 6974 696f 6e61 6c20 7761 7920   additional way 
+00000530: 746f 2063 6f6e 7472 6f6c 2063 6f6d 7075  to control compu
+00000540: 7465 7220 746f 2072 6573 7473 2e20 0a0a  ter to rests. ..
+00000550: 5375 6368 2074 6563 686e 6f6c 6f67 7920  Such technology 
+00000560: 7368 6f75 6c64 206e 6f74 2062 6520 7061  should not be pa
+00000570: 7977 616c 6c65 6420 6279 2065 7870 656e  ywalled by expen
+00000580: 7369 7665 2065 7965 2d74 7261 636b 696e  sive eye-trackin
+00000590: 6720 6861 7264 7761 7265 2c20 6573 7065  g hardware, espe
+000005a0: 6369 616c 6c79 2069 6e20 6361 7365 2077  cially in case w
+000005b0: 6865 6e20 6974 2069 7320 6e65 6564 6564  hen it is needed
+000005c0: 2074 6f20 6578 6973 7420 696e 2074 6865   to exist in the
+000005d0: 2064 6967 6974 616c 2077 6f72 6c64 2061   digital world a
+000005e0: 6e64 206f 7065 7261 7465 2079 6f75 7220  nd operate your 
+000005f0: 636f 6d70 7574 6572 2e20 4d6f 7374 206f  computer. Most o
+00000600: 6620 7468 6520 6375 7272 656e 7420 636f  f the current co
+00000610: 6e73 756d 6572 2065 6c65 6374 726f 6e69  nsumer electroni
+00000620: 6373 2064 6576 6963 6573 2068 6176 6520  cs devices have 
+00000630: 6275 696c 742d 696e 206e 6174 6976 6520  built-in native 
+00000640: 6361 6d65 7261 732c 2061 6e64 2074 6865  cameras, and the
+00000650: 2063 7572 7265 6e74 2073 7461 7465 206f   current state o
+00000660: 6620 7265 7365 6172 6368 2069 6e64 6963  f research indic
+00000670: 6174 6573 2074 6861 7420 6974 2069 7320  ates that it is 
+00000680: 6163 6869 6576 6162 6c65 2074 6f20 6861  achievable to ha
+00000690: 7665 2065 7965 2074 7261 636b 696e 6720  ve eye tracking 
+000006a0: 6174 2072 6561 736f 6e61 626c 6520 6163  at reasonable ac
+000006b0: 6375 7261 6379 2062 6173 6564 206f 6e20  curacy based on 
+000006c0: 7468 6f73 6520 6e61 7469 7665 2063 616d  those native cam
+000006d0: 6572 6173 2e20 0a0a 4f75 7220 6d69 7373  eras. ..Our miss
+000006e0: 696f 6e20 6973 2074 6f20 6272 696e 6720  ion is to bring 
+000006f0: 6579 652d 7472 6163 6b69 6e67 2074 6563  eye-tracking tec
+00000700: 686e 6f6c 6f67 7920 746f 2061 7320 6d61  hnology to as ma
+00000710: 6e79 2070 656f 706c 6520 6173 2070 6f73  ny people as pos
+00000720: 7369 626c 652e 200a 0a4f 7572 2074 6563  sible. ..Our tec
+00000730: 686e 6f6c 6f67 7920 6973 206e 6f74 2070  hnology is not p
+00000740: 6572 6665 6374 2c20 6275 7420 7765 2073  erfect, but we s
+00000750: 7472 6976 6520 746f 2062 652e 0a0a 2323  trive to be...##
+00000760: 2320 f09f 9387 2046 696e 6420 7573 3a0a  # .... Find us:.
+00000770: 2d20 5b52 5353 5d28 6874 7470 733a 2f2f  - [RSS](https://
+00000780: 706f 6c61 722e 7368 2f4e 6174 6976 6553  polar.sh/NativeS
+00000790: 656e 736f 7273 2f72 7373 3f61 7574 683d  ensors/rss?auth=
+000007a0: 6579 4a68 6247 6369 4f69 4a49 557a 4931  eyJhbGciOiJIUzI1
+000007b0: 4e69 4973 496e 5235 6343 4936 496b 7058  NiIsInR5cCI6IkpX
+000007c0: 5643 4a39 2e65 794a 7759 5852 6661 5751  VCJ9.eyJwYXRfaWQ
+000007d0: 694f 694a 6b4d 4459 784d 4446 694f 4330  iOiJkMDYxMDFiOC0
+000007e0: 7859 7a59 794c 5451 314d 5459 7459 6a67  xYzYyLTQ1MTYtYjg
+000007f0: 3359 5330 334e 5446 684f 544d 334f 5449  3YS03NTFhOTM3OTI
+00000800: 785a 6d55 694c 434a 7a59 3239 775a 584d  xZmUiLCJzY29wZXM
+00000810: 694f 694a 6863 6e52 7059 3278 6c63 7a70  iOiJhcnRpY2xlczp
+00000820: 795a 5746 6b49 6977 6964 486c 775a 5349  yZWFkIiwidHlwZSI
+00000830: 3649 6d46 3164 4767 694c 434a 6c65 4841  6ImF1dGgiLCJleHA
+00000840: 694f 6a45 334e 444d 784e 6a67 334f 4468  iOjE3NDMxNjg3ODh
+00000850: 392e 646a 6f69 3541 5257 4872 2d78 4657  9.djoi5ARWHr-xFW
+00000860: 5f58 4a36 4677 616c 334a 5554 3166 4162  _XJ6Fwal3JUT1fAb
+00000870: 7678 344e 706c 2d64 6142 4335 5529 0a2d  vx4Npl-daBC5U).-
+00000880: 205b 6469 7363 6f72 645d 2868 7474 7073   [discord](https
+00000890: 3a2f 2f64 6973 636f 7264 2e67 672f 4656  ://discord.gg/FV
+000008a0: 3352 5954 7556 290a 2d20 5b74 7769 7474  3RYTuV).- [twitt
+000008b0: 6572 5d28 6874 7470 733a 2f2f 7477 6974  er](https://twit
+000008c0: 7465 722e 636f 6d2f 5057 346c 747a 290a  ter.com/PW4ltz).
+000008d0: 2d20 656d 6169 6c3a 2063 6f6e 7461 6374  - email: contact
+000008e0: 4065 7965 6765 7374 7572 6573 2e63 6f6d  @eyegestures.com
+000008f0: 0a0a 466f 6c6c 6f77 2075 7320 6f6e 2070  ..Follow us on p
+00000900: 6f6c 6172 2028 6974 2063 6f73 7473 206e  olar (it costs n
+00000910: 6f74 6869 6e67 2062 7574 2079 6f75 2068  othing but you h
+00000920: 656c 7020 7072 6f6a 6563 7421 293a 0a0a  elp project!):..
+00000930: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000940: 2f70 6f6c 6172 2e73 682f 4e61 7469 7665  /polar.sh/Native
+00000950: 5365 6e73 6f72 7322 3e3c 7069 6374 7572  Sensors"><pictur
+00000960: 653e 3c73 6f75 7263 6520 6d65 6469 613d  e><source media=
+00000970: 2228 7072 6566 6572 732d 636f 6c6f 722d  "(prefers-color-
+00000980: 7363 6865 6d65 3a20 6461 726b 2922 2073  scheme: dark)" s
+00000990: 7263 7365 743d 2268 7474 7073 3a2f 2f70  rcset="https://p
+000009a0: 6f6c 6172 2e73 682f 656d 6265 642f 7375  olar.sh/embed/su
+000009b0: 6273 6372 6962 652e 7376 673f 6f72 673d  bscribe.svg?org=
+000009c0: 4e61 7469 7665 5365 6e73 6f72 7326 6c61  NativeSensors&la
+000009d0: 6265 6c3d 5375 6273 6372 6962 6526 6461  bel=Subscribe&da
+000009e0: 726b 6d6f 6465 223e 3c69 6d67 2061 6c74  rkmode"><img alt
+000009f0: 3d22 5375 6273 6372 6962 6520 6f6e 2050  ="Subscribe on P
+00000a00: 6f6c 6172 2220 7372 633d 2268 7474 7073  olar" src="https
+00000a10: 3a2f 2f70 6f6c 6172 2e73 682f 656d 6265  ://polar.sh/embe
+00000a20: 642f 7375 6273 6372 6962 652e 7376 673f  d/subscribe.svg?
+00000a30: 6f72 673d 4e61 7469 7665 5365 6e73 6f72  org=NativeSensor
+00000a40: 7326 6c61 6265 6c3d 5375 6273 6372 6962  s&label=Subscrib
+00000a50: 6522 3e3c 2f70 6963 7475 7265 3e3c 2f61  e"></picture></a
+00000a60: 3e0a 0a23 2323 20f0 9f92 9c20 5370 6f6e  >..### .... Spon
+00000a70: 736f 7273 3a20 0a0a 6060 600a 5370 6f6e  sors: ..```.Spon
+00000a80: 736f 7220 7573 2061 6e64 2077 6520 6361  sor us and we ca
+00000a90: 6e20 6164 6420 796f 7572 206c 696e 6b2c  n add your link,
+00000aa0: 2062 616e 6e65 7220 6f72 206f 7468 6572   banner or other
+00000ab0: 2070 726f 6d6f 206d 6174 6572 6961 6c73   promo materials
+00000ac0: 210a 6060 600a 3c21 2d2d 2050 4f4c 4152  !.```.<!-- POLAR
+00000ad0: 2074 7970 653d 6164 7320 6964 3d65 697a   type=ads id=eiz
+00000ae0: 6465 6c77 7520 7375 6273 6372 6970 7469  delwu subscripti
+00000af0: 6f6e 5f62 656e 6566 6974 5f69 643d 6262  on_benefit_id=bb
+00000b00: 3237 3262 3664 2d66 3639 382d 3434 6533  272b6d-f698-44e3
+00000b10: 2d61 3431 372d 3336 6136 6661 3230 3362  -a417-36a6fa203b
+00000b20: 6265 2077 6964 7468 3d32 3430 2068 6569  be width=240 hei
+00000b30: 6768 743d 3130 3020 2d2d 3e0a 0a0a 0a3c  ght=100 -->....<
+00000b40: 212d 2d20 504f 4c41 522d 454e 4420 6964  !-- POLAR-END id
+00000b50: 3d65 697a 6465 6c77 7520 2d2d 3e0a 0a23  =eizdelwu -->..#
+00000b60: 2323 20f0 9f93 a220 416e 6e6f 756e 6365  ## .... Announce
+00000b70: 6d65 6e74 733a 0a0a 3c61 2068 7265 663d  ments:..<a href=
+00000b80: 2268 7474 7073 3a2f 2f70 6f6c 6172 2e73  "https://polar.s
+00000b90: 682f 4e61 7469 7665 5365 6e73 6f72 732f  h/NativeSensors/
+00000ba0: 706f 7374 7322 3e3c 7069 6374 7572 653e  posts"><picture>
+00000bb0: 3c73 6f75 7263 6520 6d65 6469 613d 2228  <source media="(
+00000bc0: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
+00000bd0: 6865 6d65 3a20 6461 726b 2922 2073 7263  heme: dark)" src
+00000be0: 7365 743d 2268 7474 7073 3a2f 2f70 6f6c  set="https://pol
+00000bf0: 6172 2e73 682f 656d 6265 642f 706f 7374  ar.sh/embed/post
+00000c00: 732e 7376 673f 6f72 673d 4e61 7469 7665  s.svg?org=Native
+00000c10: 5365 6e73 6f72 7326 6461 726b 6d6f 6465  Sensors&darkmode
+00000c20: 223e 3c69 6d67 2061 6c74 3d22 506f 7374  "><img alt="Post
+00000c30: 7320 6f6e 2050 6f6c 6172 2220 7372 633d  s on Polar" src=
+00000c40: 2268 7474 7073 3a2f 2f70 6f6c 6172 2e73  "https://polar.s
+00000c50: 682f 656d 6265 642f 706f 7374 732e 7376  h/embed/posts.sv
+00000c60: 673f 6f72 673d 4e61 7469 7665 5365 6e73  g?org=NativeSens
+00000c70: 6f72 7322 3e3c 2f70 6963 7475 7265 3e3c  ors"></picture><
+00000c80: 2f61 3e0a 0a23 2323 20f0 9f94 a520 5765  /a>..### .... We
+00000c90: 6220 4465 6d6f 733a 0a0a 2d20 5b4d 6169  b Demos:..- [Mai
+00000ca0: 6e20 7061 6765 5d28 6874 7470 733a 2f2f  n page](https://
+00000cb0: 6579 6567 6573 7475 7265 732e 636f 6d2f  eyegestures.com/
+00000cc0: 290a 2d20 5b47 616d 6520 6465 6d6f 5d28  ).- [Game demo](
+00000cd0: 6874 7470 733a 2f2f 6579 6567 6573 7475  https://eyegestu
+00000ce0: 7265 732e 636f 6d2f 6761 6d65 290a 2d20  res.com/game).- 
+00000cf0: 5b43 696e 656d 6120 6465 6d6f 5d28 6874  [Cinema demo](ht
+00000d00: 7470 733a 2f2f 6579 6567 6573 7475 7265  tps://eyegesture
+00000d10: 732e 636f 6d2f 6369 6e65 6d61 290a 2d20  s.com/cinema).- 
+00000d20: 5b52 6573 7461 7572 616e 745d 2868 7474  [Restaurant](htt
+00000d30: 7073 3a2f 2f65 7965 6765 7374 7572 6573  ps://eyegestures
+00000d40: 2e63 6f6d 2f72 6573 7461 7572 616e 7429  .com/restaurant)
+00000d50: 0a0a 2323 2320 f09f 92bb 2049 6e73 7461  ..### .... Insta
+00000d60: 6c6c 0a60 6060 0a70 7974 686f 6e33 202d  ll.```.python3 -
+00000d70: 6d20 7069 7020 696e 7374 616c 6c20 6579  m pip install ey
+00000d80: 6547 6573 7475 7265 730a 6060 600a 0a4e  eGestures.```..N
+00000d90: 6f74 653a 2079 6f75 206d 6179 206e 6565  ote: you may nee
+00000da0: 6420 746f 2063 6861 6e67 6520 7665 7273  d to change vers
+00000db0: 696f 6e20 6f66 2070 6163 6b61 6765 2060  ion of package `
+00000dc0: 6579 6567 6573 7475 7265 732d 582e 582e  eyegestures-X.X.
+00000dd0: 5860 2e0a 0a23 2323 20e2 9a99 efb8 8f20  X`...### ...... 
+00000de0: 5275 6e20 0a60 6060 0a70 7974 686f 6e33  Run .```.python3
+00000df0: 2065 7861 6d70 6c65 732f 7369 6d70 6c65   examples/simple
+00000e00: 5f65 7861 6d70 6c65 2e70 790a 6060 600a  _example.py.```.
+00000e10: 0a23 2323 20f0 9faa 9f20 5275 6e20 5769  .### .... Run Wi
+00000e20: 6e64 6f77 7320 4170 7020 0a60 6060 0a70  ndows App .```.p
+00000e30: 7974 686f 6e33 2061 7070 732f 7769 6e5f  ython3 apps/win_
+00000e40: 6170 702e 7079 0a60 6060 0a0a 2323 2320  app.py.```..### 
+00000e50: f09f 94a7 2044 6576 656c 6f70 200a 0a54  .... Develop ..T
+00000e60: 6f20 6265 6769 6e2c 2079 6f75 2069 6e73  o begin, you ins
+00000e70: 7461 6e74 6961 7465 2061 6e20 4579 6547  tantiate an EyeG
+00000e80: 6573 7475 7265 7320 6f62 6a65 6374 2077  estures object w
+00000e90: 6974 6820 696e 6974 6961 6c20 5265 6769  ith initial Regi
+00000ea0: 6f6e 206f 6620 496e 7465 7265 7374 2028  on of Interest (
+00000eb0: 526f 4929 2070 6172 616d 6574 6572 732e  RoI) parameters.
+00000ec0: 2054 6865 7365 2070 6172 616d 6574 6572   These parameter
+00000ed0: 7320 6465 6669 6e65 2061 2070 7265 6c69  s define a preli
+00000ee0: 6d69 6e61 7279 2066 6f63 7573 2061 7265  minary focus are
+00000ef0: 6120 666f 7220 7468 6520 7472 6163 6b65  a for the tracke
+00000f00: 7220 7769 7468 696e 2061 2076 6972 7475  r within a virtu
+00000f10: 616c 2035 3030 7835 3030 2073 6372 6565  al 500x500 scree
+00000f20: 6e20 7370 6163 652c 2077 6869 6368 2068  n space, which h
+00000f30: 656c 7073 2069 6e20 6c6f 6361 7469 6e67  elps in locating
+00000f40: 2074 6865 2075 7365 7227 7320 6761 7a65   the user's gaze
+00000f50: 206d 6f72 6520 6566 6669 6369 656e 746c   more efficientl
+00000f60: 792e 0a0a 4d61 696e 2060 4579 6547 6573  y...Main `EyeGes
+00000f70: 7475 7265 6020 6f62 6a65 6374 2070 726f  ture` object pro
+00000f80: 7669 6465 7320 6765 6e65 7261 6c20 636f  vides general co
+00000f90: 6e66 6967 7572 6174 696f 6e20 696e 6974  nfiguration init
+00000fa0: 6961 6c20 636f 6e64 6974 696f 6e73 3a20  ial conditions: 
+00000fb0: 0a0a 6060 6070 7974 686f 6e0a 4579 6547  ..```python.EyeG
+00000fc0: 6573 7475 7265 7328 2020 0a20 2072 6f69  estures(  .  roi
+00000fd0: 5f78 203d 2032 3835 0a20 2072 6f69 5f79  _x = 285.  roi_y
+00000fe0: 203d 2031 3135 0a20 2072 6f69 5f77 6964   = 115.  roi_wid
+00000ff0: 7468 203d 2038 300a 2020 726f 695f 6865  th = 80.  roi_he
+00001000: 6967 6874 203d 2031 350a 290a 6060 6020  ight = 15.).``` 
+00001010: 200a 0a54 6865 2074 7261 636b 6572 206f   ..The tracker o
+00001020: 7065 7261 7465 7320 7769 7468 696e 2061  perates within a
+00001030: 2076 6972 7475 616c 2073 6372 6565 6e20   virtual screen 
+00001040: 6d65 6173 7572 696e 6720 3530 3078 3530  measuring 500x50
+00001050: 302c 2077 6865 7265 2069 7420 6d61 7073  0, where it maps
+00001060: 2074 6865 2070 6f73 6974 696f 6e73 206f   the positions o
+00001070: 6620 7468 6520 7075 7069 6c73 2061 6e64  f the pupils and
+00001080: 206f 7468 6572 2063 7269 7469 6361 6c20   other critical 
+00001090: 6661 6369 616c 2066 6561 7475 7265 7320  facial features 
+000010a0: 746f 2064 6564 7563 6520 7468 6520 7573  to deduce the us
+000010b0: 6572 2773 2067 617a 6520 6469 7265 6374  er's gaze direct
+000010c0: 696f 6e2e 2057 6974 6869 6e20 7468 6973  ion. Within this
+000010d0: 2073 7061 6365 2c20 7468 6520 5265 6769   space, the Regi
+000010e0: 6f6e 206f 6620 496e 7465 7265 7374 2028  on of Interest (
+000010f0: 526f 4929 2073 6572 7665 7320 6173 2061  RoI) serves as a
+00001100: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00001110: 6f66 2074 6865 2075 7365 7227 7320 6469  of the user's di
+00001120: 7370 6c61 792c 2069 6e66 6572 7265 6420  splay, inferred 
+00001130: 7468 726f 7567 6820 6120 636f 6d62 696e  through a combin
+00001140: 6174 696f 6e20 6f66 2065 7965 206d 6f76  ation of eye mov
+00001150: 656d 656e 7420 616e 6420 6564 6765 2064  ement and edge d
+00001160: 6574 6563 7469 6f6e 2064 7572 696e 6720  etection during 
+00001170: 6361 6c69 6272 6174 696f 6e2e 0a0a 4166  calibration...Af
+00001180: 7465 7220 6c6f 6361 7469 6e67 2074 6865  ter locating the
+00001190: 2052 6f49 2077 6974 6869 6e20 7468 6520   RoI within the 
+000011a0: 3530 3078 3530 3020 7370 6163 652c 2069  500x500 space, i
+000011b0: 7473 2064 696d 656e 7369 6f6e 7320 6172  ts dimensions ar
+000011c0: 6520 6164 6a75 7374 6564 2074 6f20 6669  e adjusted to fi
+000011d0: 7420 7468 6520 7265 736f 6c75 7469 6f6e  t the resolution
+000011e0: 2075 7365 6420 696e 2074 6865 2065 7374   used in the est
+000011f0: 696d 6174 6520 6675 6e63 7469 6f6e 2c20  imate function, 
+00001200: 7479 7069 6361 6c6c 7920 6465 7363 7269  typically descri
+00001210: 6265 6420 6173 2060 6469 7370 6c61 795f  bed as `display_
+00001220: 7769 6474 6860 2062 7920 6064 6973 706c  width` by `displ
+00001230: 6179 5f68 6569 6768 7460 2e0a 0a43 616c  ay_height`...Cal
+00001240: 6962 7261 7469 6f6e 2061 696d 7320 746f  ibration aims to
+00001250: 2070 7265 6369 7365 6c79 2064 6574 6572   precisely deter
+00001260: 6d69 6e65 2074 6865 2052 6f49 2773 2064  mine the RoI's d
+00001270: 696d 656e 7369 6f6e 732e 2050 7269 6f72  imensions. Prior
+00001280: 2074 6f20 6361 6c69 6272 6174 696f 6e2c   to calibration,
+00001290: 2074 6865 2074 7261 636b 6572 2072 656c   the tracker rel
+000012a0: 6965 7320 6f6e 2069 6e69 7469 616c 206f  ies on initial o
+000012b0: 7074 696f 6e61 6c20 7061 7261 6d65 7465  ptional paramete
+000012c0: 7273 2c20 696e 636c 7564 696e 673a 0a0a  rs, including:..
+000012d0: 2d20 6072 6f69 5f78 603a 2054 6865 2069  - `roi_x`: The i
+000012e0: 6e69 7469 616c 2078 2d63 6f6f 7264 696e  nitial x-coordin
+000012f0: 6174 6520 6f66 2074 6865 2052 6f49 2028  ate of the RoI (
+00001300: 7261 6e67 696e 6720 6672 6f6d 2030 2074  ranging from 0 t
+00001310: 6f20 3530 3029 2e0a 2d20 6072 6f69 5f79  o 500)..- `roi_y
+00001320: 603a 2054 6865 2069 6e69 7469 616c 2079  `: The initial y
+00001330: 2d63 6f6f 7264 696e 6174 6520 6f66 2074  -coordinate of t
+00001340: 6865 2052 6f49 2028 7261 6e67 696e 6720  he RoI (ranging 
+00001350: 6672 6f6d 2030 2074 6f20 3530 3029 2e0a  from 0 to 500)..
+00001360: 2d20 6072 6f69 5f77 6964 7468 603a 2054  - `roi_width`: T
+00001370: 6865 2069 6e69 7469 616c 2077 6964 7468  he initial width
+00001380: 206f 6620 7468 6520 526f 4920 6265 666f   of the RoI befo
+00001390: 7265 2063 616c 6962 7261 7469 6f6e 2028  re calibration (
+000013a0: 7261 6e67 696e 6720 6672 6f6d 2030 2074  ranging from 0 t
+000013b0: 6f20 3530 3020 2d20 7829 2e0a 2d20 6072  o 500 - x)..- `r
+000013c0: 6f69 5f68 6569 6768 7460 3a20 5468 6520  oi_height`: The 
+000013d0: 696e 6974 6961 6c20 6865 6967 6874 206f  initial height o
+000013e0: 6620 7468 6520 526f 4920 6265 666f 7265  f the RoI before
+000013f0: 2063 616c 6962 7261 7469 6f6e 2028 7261   calibration (ra
+00001400: 6e67 696e 6720 6672 6f6d 2030 2074 6f20  nging from 0 to 
+00001410: 3530 3020 2d20 7829 2e0a 0a4e 6578 7420  500 - x)...Next 
+00001420: 7061 7274 2069 7320 6f62 7461 696e 696e  part is obtainin
+00001430: 6720 6573 7469 6d61 7469 6f6e 7320 6672  g estimations fr
+00001440: 6f6d 2063 616d 6572 6120 6672 616d 6573  om camera frames
+00001450: 2028 6966 2079 6f75 2063 616e 6e6f 7420   (if you cannot 
+00001460: 6765 7420 6573 7469 6d61 7469 6f6e 732c  get estimations,
+00001470: 2079 6f75 206d 6179 2074 7279 2074 6f20   you may try to 
+00001480: 6368 616e 6765 2063 6f6c 6f72 2063 6f64  change color cod
+00001490: 696e 6720 6f72 2072 6f74 6174 696f 6e20  ing or rotation 
+000014a0: 6f66 2069 6d61 6765 202d 2063 6865 636b  of image - check
+000014b0: 2060 7369 6d70 6c65 5f65 7861 6d70 6c65   `simple_example
+000014c0: 2e70 7960 292e 0a0a 6060 6070 7974 686f  .py`)...```pytho
+000014d0: 6e0a 6576 656e 7420 3d20 6765 7374 7572  n.event = gestur
+000014e0: 6573 2e65 7374 696d 6174 6528 0a20 2020  es.estimate(.   
+000014f0: 2069 6d61 6765 203d 2066 7261 6d65 2c0a   image = frame,.
+00001500: 2020 2020 636f 6e74 6578 7420 3d20 226d      context = "m
+00001510: 6169 6e22 2c0a 2020 2020 6361 6c69 6272  ain",.    calibr
+00001520: 6174 696f 6e20 3d20 5472 7565 2c20 2320  ation = True, # 
+00001530: 7365 7420 6361 6c69 6272 6174 696f 6e20  set calibration 
+00001540: 2d20 7377 6974 6368 2074 6f20 4661 6c73  - switch to Fals
+00001550: 6520 746f 2073 746f 7020 6361 6c69 6272  e to stop calibr
+00001560: 6174 696f 6e0a 2020 2020 6469 7370 6c61  ation.    displa
+00001570: 795f 7769 6474 6820 3d20 7363 7265 656e  y_width = screen
+00001580: 5f77 6964 7468 2c0a 2020 2020 6469 7370  _width,.    disp
+00001590: 6c61 795f 6865 6967 6874 203d 2073 6372  lay_height = scr
+000015a0: 6565 6e5f 6865 6967 6874 2c0a 2020 2020  een_height,.    
+000015b0: 6469 7370 6c61 795f 6f66 6673 6574 5f78  display_offset_x
+000015c0: 203d 2030 2c20 0a20 2020 2064 6973 706c   = 0, .    displ
+000015d0: 6179 5f6f 6666 7365 745f 7920 3d20 302c  ay_offset_y = 0,
+000015e0: 200a 2020 2020 6669 7861 7469 6f6e 5f66   .    fixation_f
+000015f0: 7265 657a 6520 3d20 302e 382c 0a20 2020  reeze = 0.8,.   
+00001600: 2066 7265 657a 655f 7261 6469 7573 203d   freeze_radius =
+00001610: 2031 3029 0a60 6060 0a0a 2d20 6069 6d61   10).```..- `ima
+00001620: 6765 6020 2d20 6973 2063 7632 2069 6d61  ge` - is cv2 ima
+00001630: 6765 2066 7261 6d65 0a2d 2060 636f 6e74  ge frame.- `cont
+00001640: 6578 7460 202d 2069 7320 6e61 6d65 2067  ext` - is name g
+00001650: 6976 656e 2074 6f20 636f 6e74 6563 742e  iven to contect.
+00001660: 2049 6620 6e61 6d65 2063 6861 6e67 6573   If name changes
+00001670: 2074 6865 6e20 6469 6666 6572 656e 7420   then different 
+00001680: 7472 6163 6b65 7220 636f 6e74 6578 7420  tracker context 
+00001690: 6973 2075 7365 642e 2054 7261 636b 6572  is used. Tracker
+000016a0: 2072 656d 6265 7273 2070 7265 7669 6f75   rembers previou
+000016b0: 7320 706f 696e 7473 2074 6f20 6573 7469  s points to esti
+000016c0: 6d61 7465 206e 6577 206f 6e65 2c20 6275  mate new one, bu
+000016d0: 7420 7468 6f73 6520 706f 696e 7473 2061  t those points a
+000016e0: 7265 2061 7373 696e 6765 6420 746f 2073  re assinged to s
+000016f0: 696e 676c 6520 636f 6e74 6578 742e 2042  ingle context. B
+00001700: 7920 6368 616e 6769 6e67 206e 616d 6573  y changing names
+00001710: 206f 7220 7061 7373 696e 6720 6e65 7720   or passing new 
+00001720: 6f6e 6573 2079 6f75 2063 616e 2073 7769  ones you can swi
+00001730: 7463 6820 616e 6420 6372 6561 7465 2063  tch and create c
+00001740: 6f6e 7465 7874 6573 2e0a 2d20 6063 616c  ontextes..- `cal
+00001750: 6962 7261 7469 6f6e 6020 2d20 6966 2060  ibration` - if `
+00001760: 5472 7565 6020 7468 656e 2065 7665 7279  True` then every
+00001770: 2066 6577 2073 6563 6f6e 6473 2074 7261   few seconds tra
+00001780: 636b 6572 2069 7320 7265 6361 6c69 6272  cker is recalibr
+00001790: 6174 696e 672c 2069 6620 6046 616c 7365  ating, if `False
+000017a0: 6020 7468 656e 2074 7261 636b 6572 2073  ` then tracker s
+000017b0: 6574 7469 6e67 2069 7320 6672 6f7a 656e  etting is frozen
+000017c0: 2e20 5468 6520 6265 7374 2061 7070 726f  . The best appro
+000017d0: 6163 6820 6973 2074 6f20 656e 6162 6c65  ach is to enable
+000017e0: 2063 616c 6962 7261 7469 6f6e 2077 6865   calibration whe
+000017f0: 6e20 6f6e 6520 6f66 2074 6865 2065 6467  n one of the edg
+00001800: 6573 2069 7320 7265 6163 6865 642e 200a  es is reached. .
+00001810: 2d20 6064 6973 706c 6179 5f77 6964 7468  - `display_width
+00001820: 6020 2d20 7769 6474 6820 6f66 2064 6973  ` - width of dis
+00001830: 706c 6179 2f73 6372 6565 6e20 7573 6564  play/screen used
+00001840: 2e0a 2d20 6064 6973 706c 6179 5f68 6569  ..- `display_hei
+00001850: 6768 7460 202d 2068 6569 6768 7420 6f66  ght` - height of
+00001860: 2064 6973 706c 6179 2f73 6372 6565 6e20   display/screen 
+00001870: 7573 6564 2e0a 2d20 6064 6973 706c 6179  used..- `display
+00001880: 5f6f 6666 7365 745f 7860 202d 206f 6666  _offset_x` - off
+00001890: 7365 7420 6f66 2078 2066 6f72 2064 6973  set of x for dis
+000018a0: 706c 6179 2f73 6372 6565 6e20 7573 6564  play/screen used
+000018b0: 2e20 5573 6520 6974 2077 6865 6e20 6861  . Use it when ha
+000018c0: 7669 6e67 2074 776f 2064 6973 706c 6179  ving two display
+000018d0: 7320 616e 6420 6170 7020 6973 2063 6f76  s and app is cov
+000018e0: 6572 696e 6720 616c 6c20 7363 7265 656e  ering all screen
+000018f0: 732c 2062 7574 2079 6f75 2077 616e 7420  s, but you want 
+00001900: 746f 206c 696d 6974 2079 6f75 7220 6375  to limit your cu
+00001910: 7273 6f72 2074 7261 636b 6572 2074 6f20  rsor tracker to 
+00001920: 6f6e 6c79 2073 7065 6369 6669 6320 6469  only specific di
+00001930: 7370 6c61 792e 0a2d 2060 6469 7370 6c61  splay..- `displa
+00001940: 795f 6f66 6673 6574 5f79 6020 2d20 6f66  y_offset_y` - of
+00001950: 6673 6574 206f 6620 7920 666f 7220 6469  fset of y for di
+00001960: 7370 6c61 792f 7363 7265 656e 2075 7365  splay/screen use
+00001970: 642e 2055 7365 2069 7420 7768 656e 2068  d. Use it when h
+00001980: 6176 696e 6720 7477 6f20 6469 7370 6c61  aving two displa
+00001990: 7973 2061 6e64 2061 7070 2069 7320 636f  ys and app is co
+000019a0: 7665 7269 6e67 2061 6c6c 2073 6372 6565  vering all scree
+000019b0: 6e73 2c20 6275 7420 796f 7520 7761 6e74  ns, but you want
+000019c0: 2074 6f20 6c69 6d69 7420 796f 7572 2063   to limit your c
+000019d0: 7572 736f 7220 7472 6163 6b65 7220 746f  ursor tracker to
+000019e0: 206f 6e6c 7920 7370 6563 6966 6963 2064   only specific d
+000019f0: 6973 706c 6179 2e0a 2d20 6066 6978 6174  isplay..- `fixat
+00001a00: 696f 6e5f 6672 6565 7a65 6020 2d20 7468  ion_freeze` - th
+00001a10: 7265 7368 6f6c 6420 6f66 2075 7365 7220  reshold of user 
+00001a20: 6669 7861 7469 6f6e 206f 6e20 6f6e 6520  fixation on one 
+00001a30: 706f 696e 7420 2869 7420 676f 6573 2066  point (it goes f
+00001a40: 726f 6d20 302e 3020 746f 2031 2e30 292e  rom 0.0 to 1.0).
+00001a50: 2049 6620 7468 7265 7368 6f6c 6420 6973   If threshold is
+00001a60: 2063 726f 7373 6564 2070 6f69 6e74 2069   crossed point i
+00001a70: 7320 6672 6f7a 656e 2074 696c 6c20 7573  s frozen till us
+00001a80: 6572 2062 7265 616b 7320 6066 7265 657a  er breaks `freez
+00001a90: 655f 7261 6469 7573 6020 696e 2070 6978  e_radius` in pix
+00001aa0: 656c 732e 0a2d 2060 6672 6565 7a65 5f72  els..- `freeze_r
+00001ab0: 6164 6975 7360 202d 2064 6973 7461 6e63  adius` - distanc
+00001ac0: 6520 6375 7273 6f72 2063 616e 206d 6f76  e cursor can mov
+00001ad0: 6520 746f 2072 6561 6368 2066 6978 6174  e to reach fixat
+00001ae0: 696f 6e20 616e 6420 6672 6565 7a69 6e67  ion and freezing
+00001af0: 2c20 6966 2063 7572 736f 7220 6d6f 7665  , if cursor move
+00001b00: 6d65 6e74 7320 6172 6520 6772 6561 7465  ments are greate
+00001b10: 7220 7468 616e 2064 6973 7461 6e63 6520  r than distance 
+00001b20: 7468 656e 2066 6978 6174 696f 6e20 6d65  then fixation me
+00001b30: 6173 7572 656d 656e 7420 676f 6573 2064  asurement goes d
+00001b40: 6f77 6e20 746f 2060 302e 3060 2e0a 0a60  own to `0.0`...`
+00001b50: 6060 0a47 6576 656e 7420 6576 656e 740a  ``.Gevent event.
+00001b60: 6060 600a 0a60 4765 7665 6e74 6020 6973  ```..`Gevent` is
+00001b70: 2072 6574 7572 6e65 6420 656c 656d 656e   returned elemen
+00001b80: 7420 6861 7669 6e67 2061 6c6c 2064 6174  t having all dat
+00001b90: 6120 6e65 6365 7373 6172 7920 746f 2075  a necessary to u
+00001ba0: 7365 2074 7261 636b 6572 3a0a 200a 2d20  se tracker:. .- 
+00001bb0: 6070 6f69 6e74 5f73 6372 6565 6e60 2069  `point_screen` i
+00001bc0: 7320 706f 696e 7420 636f 6f72 6469 6e61  s point coordina
+00001bd0: 7465 7320 6f6e 2073 6372 6565 6e0a 2d20  tes on screen.- 
+00001be0: 6062 6c69 6e6b 6020 6973 2062 6f6f 6c65  `blink` is boole
+00001bf0: 616e 2076 616c 7565 2064 6573 6372 6962  an value describ
+00001c00: 696e 6720 626c 696e 6b20 6576 656e 742e  ing blink event.
+00001c10: 2049 6620 6030 6020 6e6f 2062 6c69 6e6b   If `0` no blink
+00001c20: 206f 6363 7572 6564 2c20 6966 2060 3160   occured, if `1`
+00001c30: 2062 6c69 6e6b 206f 6363 7572 6564 2e0a   blink occured..
+00001c40: 2d20 6066 6978 6174 696f 6e60 2076 616c  - `fixation` val
+00001c50: 7565 2066 726f 6d20 6030 2e30 6020 746f  ue from `0.0` to
+00001c60: 2060 312e 3060 2064 6573 6372 6962 696e   `1.0` describin
+00001c70: 6720 6c65 7665 6c20 6f66 2075 7365 7220  g level of user 
+00001c80: 6669 7861 7469 6f6e 2e0a 0a45 6e74 6972  fixation...Entir
+00001c90: 6520 7072 6f67 7261 6d3a 200a 0a60 6060  e program: ..```
+00001ca0: 7079 7468 6f6e 0a69 6d70 6f72 7420 5669  python.import Vi
+00001cb0: 6465 6f43 6170 7475 7265 2023 6368 616e  deoCapture #chan
+00001cc0: 6765 2069 7420 746f 206f 7065 6e63 7620  ge it to opencv 
+00001cd0: 666f 7220 7265 616c 2061 7070 6c69 6361  for real applica
+00001ce0: 7469 6f6e 730a 6672 6f6d 2065 7965 4765  tions.from eyeGe
+00001cf0: 7374 7572 6573 2e75 7469 6c73 2069 6d70  stures.utils imp
+00001d00: 6f72 7420 5669 6465 6f43 6170 7475 7265  ort VideoCapture
+00001d10: 0a66 726f 6d20 6579 6547 6573 7475 7265  .from eyeGesture
+00001d20: 732e 6579 6567 6573 7475 7265 7320 696d  s.eyegestures im
+00001d30: 706f 7274 2045 7965 4765 7374 7572 6573  port EyeGestures
+00001d40: 0a0a 6765 7374 7572 6573 203d 2045 7965  ..gestures = Eye
+00001d50: 4765 7374 7572 6573 280a 2020 726f 695f  Gestures(.  roi_
+00001d60: 7820 3d20 3238 350a 2020 726f 695f 7920  x = 285.  roi_y 
+00001d70: 3d20 3131 350a 2020 726f 695f 7769 6474  = 115.  roi_widt
+00001d80: 6820 3d20 3830 0a20 2072 6f69 5f68 6569  h = 80.  roi_hei
+00001d90: 6768 7420 3d20 3135 0a29 0a0a 6361 7020  ght = 15.)..cap 
+00001da0: 3d20 5669 6465 6f43 6170 7475 7265 2830  = VideoCapture(0
+00001db0: 2920 200a 0a23 204d 6169 6e20 6761 6d65  )  ..# Main game
+00001dc0: 206c 6f6f 700a 7275 6e6e 696e 6720 3d20   loop.running = 
+00001dd0: 5472 7565 0a77 6869 6c65 2072 756e 6e69  True.while runni
+00001de0: 6e67 3a0a 0a20 2020 2023 2047 656e 6572  ng:..    # Gener
+00001df0: 6174 6520 6e65 7720 7261 6e64 6f6d 2070  ate new random p
+00001e00: 6f73 6974 696f 6e20 666f 7220 7468 6520  osition for the 
+00001e10: 6375 7273 6f72 0a20 2020 2072 6574 2c20  cursor.    ret, 
+00001e20: 6672 616d 6520 3d20 6361 702e 7265 6164  frame = cap.read
+00001e30: 2829 2020 2020 200a 0a20 2020 2065 7665  ()     ..    eve
+00001e40: 6e74 203d 2067 6573 7475 7265 732e 6573  nt = gestures.es
+00001e50: 7469 6d61 7465 280a 2020 2020 2020 2020  timate(.        
+00001e60: 6672 616d 652c 0a20 2020 2020 2020 2022  frame,.        "
+00001e70: 6d61 696e 222c 0a20 2020 2020 2020 2054  main",.        T
+00001e80: 7275 652c 2023 2073 6574 2063 616c 6962  rue, # set calib
+00001e90: 7261 7469 6f6e 202d 2073 7769 7463 6820  ration - switch 
+00001ea0: 746f 2046 616c 7365 2074 6f20 7374 6f70  to False to stop
+00001eb0: 2063 616c 6962 7261 7469 6f6e 0a20 2020   calibration.   
+00001ec0: 2020 2020 2073 6372 6565 6e5f 7769 6474       screen_widt
+00001ed0: 682c 0a20 2020 2020 2020 2073 6372 6565  h,.        scree
+00001ee0: 6e5f 6865 6967 6874 2c0a 2020 2020 2020  n_height,.      
+00001ef0: 2020 302c 2030 2c20 302e 382c 3130 290a    0, 0, 0.8,10).
+00001f00: 0a20 2020 2063 7572 736f 725f 782c 2063  .    cursor_x, c
+00001f10: 7572 736f 725f 7920 3d20 6576 656e 742e  ursor_y = event.
+00001f20: 706f 696e 745f 7363 7265 656e 5b30 5d2c  point_screen[0],
+00001f30: 6576 656e 742e 706f 696e 745f 7363 7265  event.point_scre
+00001f40: 656e 5b31 5d0a 0a60 6060 0a0a 0a23 2323  en[1]..```...###
+00001f50: 20f0 9f8c 9020 5765 6220 456d 6265 6464   .... Web Embedd
+00001f60: 205b 5061 6964 2041 5049 5d0a 0a46 6f72   [Paid API]..For
+00001f70: 206e 6f77 206d 6f72 6520 696e 666f 2063   now more info c
+00001f80: 616e 2062 6520 666f 756e 6420 6865 7265  an be found here
+00001f90: 3a20 6874 7470 733a 2f2f 6579 6567 6573  : https://eyeges
+00001fa0: 7475 7265 732e 636f 6d2f 7573 6572 5f70  tures.com/user_p
+00001fb0: 6f72 7461 6c0a 0a60 6060 6874 6d6c 0a2f  ortal..```html./
+00001fc0: 2f20 2e2e 2e20 7265 7374 206f 6620 6874  / ... rest of ht
+00001fd0: 6d6c 2063 6c69 656e 7420 2e2e 2e0a 0a3c  ml client .....<
+00001fe0: 7363 7269 7074 3e0a 2f2f 202e 2e2e 2079  script>.// ... y
+00001ff0: 6f75 7220 636f 6465 202e 2e2e 0a0a 6675  our code .....fu
+00002000: 6e63 7469 6f6e 206f 6e54 696c 6528 6964  nction onTile(id
+00002010: 2c20 6669 782c 2062 6c69 6e6b 2920 7b0a  , fix, blink) {.
+00002020: 2020 2f2f 202e 2e2e 2064 6f20 736f 6d65    // ... do some
+00002030: 7468 696e 6720 6865 7265 202e 2e2e 0a7d  thing here ....}
+00002040: 0a0a 6675 6e63 7469 6f6e 206f 6e43 616c  ..function onCal
+00002050: 6962 7261 7469 6f6e 2829 207b 0a20 202f  ibration() {.  /
+00002060: 2f20 2e2e 2e20 646f 2073 6f6d 6574 6869  / ... do somethi
+00002070: 6e67 2068 6572 6520 2e2e 2e0a 7d0a 3c2f  ng here ....}.</
+00002080: 7363 7269 7074 3e0a 3c73 6372 6970 7420  script>.<script 
+00002090: 7372 633d 2268 7474 7073 3a2f 2f63 646e  src="https://cdn
+000020a0: 6a73 2e63 6c6f 7564 666c 6172 652e 636f  js.cloudflare.co
+000020b0: 6d2f 616a 6178 2f6c 6962 732f 736f 636b  m/ajax/libs/sock
+000020c0: 6574 2e69 6f2f 342e 302e 302f 736f 636b  et.io/4.0.0/sock
+000020d0: 6574 2e69 6f2e 6a73 223e 3c2f 7363 7269  et.io.js"></scri
+000020e0: 7074 3e0a 3c73 6372 6970 7420 7372 633d  pt>.<script src=
+000020f0: 2268 7474 7073 3a2f 2f65 7965 6765 7374  "https://eyegest
+00002100: 7572 6573 2e63 6f6d 2f65 7965 5469 6c65  ures.com/eyeTile
+00002110: 732e 6d69 6e2e 6a73 223e 3c2f 7363 7269  s.min.js"></scri
+00002120: 7074 3e0a 3c73 6372 6970 743e 0a20 2045  pt>.<script>.  E
+00002130: 7965 5469 6c65 7341 5049 280a 2020 2020  yeTilesAPI(.    
+00002140: 6b65 7920 3d20 2259 4f55 525f 4150 495f  key = "YOUR_API_
+00002150: 4b45 5922 2c0a 2020 2020 7469 6c65 7320  KEY",.    tiles 
+00002160: 3d20 5b31 2c20 322c 2031 5d2c 0a20 2020  = [1, 2, 1],.   
+00002170: 2066 6978 5468 7265 7368 203d 2030 2e31   fixThresh = 0.1
+00002180: 2c0a 2020 2020 6669 7852 6164 6975 7320  ,.    fixRadius 
+00002190: 3d20 3530 302c 0a20 2020 2073 6967 6874  = 500,.    sight
+000021a0: 4772 6964 203d 2074 7275 652c 0a20 2020  Grid = true,.   
+000021b0: 206f 6e54 696c 6520 3d20 6f6e 5469 6c65   onTile = onTile
+000021c0: 2c0a 2020 2020 6f6e 4361 6c69 6272 6174  ,.    onCalibrat
+000021d0: 696f 6e20 3d20 6f6e 4361 6c69 6272 6174  ion = onCalibrat
+000021e0: 696f 6e2c 0a20 2029 3b0a 3c2f 7363 7269  ion,.  );.</scri
+000021f0: 7074 3e20 2020 200a 6060 600a 0a23 2323  pt>    .```..###
+00002200: 2072 756c 6573 206f 6620 7573 696e 670a   rules of using.
+00002210: 0a49 6620 796f 7520 6172 6520 6275 696c  .If you are buil
+00002220: 6469 6e67 2070 7562 6c69 636c 7920 6176  ding publicly av
+00002230: 6169 6c61 626c 6520 7072 6f64 7563 742c  ailable product,
+00002240: 2061 6e64 2068 6176 6520 6e6f 2063 6f6d   and have no com
+00002250: 6d65 7263 6961 6c20 6c69 6365 6e73 652c  mercial license,
+00002260: 2070 6c65 6173 6520 6d65 6e74 696f 6e20   please mention 
+00002270: 7573 2073 6f6d 6577 6865 7265 2069 6e20  us somewhere in 
+00002280: 796f 7572 2069 6e74 6572 6661 6365 2e20  your interface. 
+00002290: 0a0a 2a2a 5072 6f6d 6f20 4d61 7465 7269  ..**Promo Materi
+000022a0: 616c 733a 2a2a 0a0a 6874 7470 733a 2f2f  als:**..https://
+000022b0: 6769 7468 7562 2e63 6f6d 2f4e 6174 6976  github.com/Nativ
+000022c0: 6553 656e 736f 7273 2f45 7965 4765 7374  eSensors/EyeGest
+000022d0: 7572 6573 2f61 7373 6574 732f 3430 3737  ures/assets/4077
+000022e0: 3335 3530 2f34 6361 3834 3262 392d 6261  3550/4ca842b9-ba
+000022f0: 3332 2d34 6666 642d 6232 6534 2d31 3739  32-4ffd-b2e4-179
+00002300: 6666 3637 6565 3437 660a 0a3c 696d 6720  ff67ee47f..<img 
+00002310: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00002320: 6875 622e 636f 6d2f 4e61 7469 7665 5365  hub.com/NativeSe
+00002330: 6e73 6f72 732f 4579 6547 6573 7475 7265  nsors/EyeGesture
+00002340: 732f 6173 7365 7473 2f34 3037 3733 3535  s/assets/4077355
+00002350: 302f 3463 6138 3432 6239 2d62 6133 322d  0/4ca842b9-ba32-
+00002360: 3466 6664 2d62 3265 342d 3137 3966 6636  4ffd-b2e4-179ff6
+00002370: 3765 6534 3766 2220 7769 6474 683d 2233  7ee47f" width="3
+00002380: 3030 0a22 3e0a 0a68 7474 7073 3a2f 2f67  00.">..https://g
+00002390: 6974 6875 622e 636f 6d2f 4e61 7469 7665  ithub.com/Native
+000023a0: 5365 6e73 6f72 732f 4579 6547 6573 7475  Sensors/EyeGestu
+000023b0: 7265 732f 6173 7365 7473 2f34 3037 3733  res/assets/40773
+000023c0: 3535 302f 3661 3763 3734 6235 2d62 3036  550/6a7c74b5-b06
+000023d0: 392d 3465 6563 2d62 6339 362d 3361 3662  9-4eec-bc96-3a6b
+000023e0: 6234 3135 3962 3337 0a0a 3c69 6d67 2073  b4159b37..<img s
+000023f0: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00002400: 7562 2e63 6f6d 2f4e 6174 6976 6553 656e  ub.com/NativeSen
+00002410: 736f 7273 2f45 7965 4765 7374 7572 6573  sors/EyeGestures
+00002420: 2f61 7373 6574 732f 3430 3737 3335 3530  /assets/40773550
+00002430: 2f36 6137 6337 3462 352d 6230 3639 2d34  /6a7c74b5-b069-4
+00002440: 6565 632d 6263 3936 2d33 6136 6262 3431  eec-bc96-3a6bb41
+00002450: 3539 6233 3722 2077 6964 7468 3d22 3230  59b37" width="20
+00002460: 300a 223e 0a0a 0a23 2323 20f0 9f92 bb20  0.">...### .... 
+00002470: 436f 6e74 7269 6275 746f 7273 0a0a 3c61  Contributors..<a
+00002480: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00002490: 6974 6875 622e 636f 6d2f 4f57 4e45 522f  ithub.com/OWNER/
+000024a0: 5245 504f 2f67 7261 7068 732f 636f 6e74  REPO/graphs/cont
+000024b0: 7269 6275 746f 7273 223e 0a20 203c 696d  ributors">.  <im
+000024c0: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
+000024d0: 6f6e 7472 6962 2e72 6f63 6b73 2f69 6d61  ontrib.rocks/ima
+000024e0: 6765 3f72 6570 6f3d 4e61 7469 7665 5365  ge?repo=NativeSe
+000024f0: 6e73 6f72 732f 4579 6547 6573 7475 7265  nsors/EyeGesture
+00002500: 7322 202f 3e0a 3c2f 613e 0a0a 2323 2320  s" />.</a>..### 
+00002510: f09f 92b5 2053 7570 706f 7274 2074 6865  .... Support the
+00002520: 2070 726f 6a65 6374 200a 0a3c 6120 6872   project ..<a hr
+00002530: 6566 3d22 6874 7470 733a 2f2f 706f 6c61  ef="https://pola
+00002540: 722e 7368 2f4e 6174 6976 6553 656e 736f  r.sh/NativeSenso
+00002550: 7273 2f73 7562 7363 7269 7074 696f 6e73  rs/subscriptions
+00002560: 223e 3c70 6963 7475 7265 3e3c 736f 7572  "><picture><sour
+00002570: 6365 206d 6564 6961 3d22 2870 7265 6665  ce media="(prefe
+00002580: 7273 2d63 6f6c 6f72 2d73 6368 656d 653a  rs-color-scheme:
+00002590: 2064 6172 6b29 2220 7372 6373 6574 3d22   dark)" srcset="
+000025a0: 6874 7470 733a 2f2f 706f 6c61 722e 7368  https://polar.sh
+000025b0: 2f65 6d62 6564 2f74 6965 7273 2e73 7667  /embed/tiers.svg
+000025c0: 3f6f 7267 3d4e 6174 6976 6553 656e 736f  ?org=NativeSenso
+000025d0: 7273 2664 6172 6b6d 6f64 6522 3e3c 696d  rs&darkmode"><im
+000025e0: 6720 616c 743d 2253 7562 7363 7269 7074  g alt="Subscript
+000025f0: 696f 6e20 5469 6572 7320 6f6e 2050 6f6c  ion Tiers on Pol
+00002600: 6172 2220 7372 633d 2268 7474 7073 3a2f  ar" src="https:/
+00002610: 2f70 6f6c 6172 2e73 682f 656d 6265 642f  /polar.sh/embed/
+00002620: 7469 6572 732e 7376 673f 6f72 673d 4e61  tiers.svg?org=Na
+00002630: 7469 7665 5365 6e73 6f72 7322 3e3c 2f70  tiveSensors"></p
+00002640: 6963 7475 7265 3e3c 2f61 3e0a 0a3c 7069  icture></a>..<pi
+00002650: 6374 7572 653e 0a20 203c 736f 7572 6365  cture>.  <source
+00002660: 0a20 2020 206d 6564 6961 3d22 2870 7265  .    media="(pre
+00002670: 6665 7273 2d63 6f6c 6f72 2d73 6368 656d  fers-color-schem
+00002680: 653a 2064 6172 6b29 220a 2020 2020 7372  e: dark)".    sr
+00002690: 6373 6574 3d22 0a20 2020 2020 2068 7474  cset=".      htt
+000026a0: 7073 3a2f 2f61 7069 2e73 7461 722d 6869  ps://api.star-hi
+000026b0: 7374 6f72 792e 636f 6d2f 7376 673f 7265  story.com/svg?re
+000026c0: 706f 733d 4e61 7469 7665 5365 6e73 6f72  pos=NativeSensor
+000026d0: 732f 4579 6547 6573 7475 7265 7326 7479  s/EyeGestures&ty
+000026e0: 7065 3d44 6174 6526 7468 656d 653d 6461  pe=Date&theme=da
+000026f0: 726b 0a20 2020 2022 0a20 202f 3e0a 2020  rk.    ".  />.  
+00002700: 3c73 6f75 7263 650a 2020 2020 6d65 6469  <source.    medi
+00002710: 613d 2228 7072 6566 6572 732d 636f 6c6f  a="(prefers-colo
+00002720: 722d 7363 6865 6d65 3a20 6c69 6768 7429  r-scheme: light)
+00002730: 220a 2020 2020 7372 6373 6574 3d22 0a20  ".    srcset=". 
+00002740: 2020 2020 2068 7474 7073 3a2f 2f61 7069       https://api
+00002750: 2e73 7461 722d 6869 7374 6f72 792e 636f  .star-history.co
+00002760: 6d2f 7376 673f 7265 706f 733d 4e61 7469  m/svg?repos=Nati
+00002770: 7665 5365 6e73 6f72 732f 4579 6547 6573  veSensors/EyeGes
+00002780: 7475 7265 7326 7479 7065 3d44 6174 650a  tures&type=Date.
+00002790: 2020 2020 220a 2020 2f3e 0a20 203c 696d      ".  />.  <im
+000027a0: 670a 2020 2020 616c 743d 2253 7461 7220  g.    alt="Star 
+000027b0: 4869 7374 6f72 7920 4368 6172 7422 0a20  History Chart". 
+000027c0: 2020 2073 7263 3d22 6874 7470 733a 2f2f     src="https://
+000027d0: 6170 692e 7374 6172 2d68 6973 746f 7279  api.star-history
+000027e0: 2e63 6f6d 2f73 7667 3f72 6570 6f73 3d4e  .com/svg?repos=N
+000027f0: 6174 6976 6553 656e 736f 7273 2f45 7965  ativeSensors/Eye
+00002800: 4765 7374 7572 6573 2674 7970 653d 4461  Gestures&type=Da
+00002810: 7465 220a 2020 2f3e 0a3c 2f70 6963 7475  te".  />.</pictu
+00002820: 7265 3e0a 0a                             re>..
```

### Comparing `eyegestures-1.3.3/pyproject.toml` & `eyegestures-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "test_app.py",
   "test.py",
   "tools/*"
 ]
 
 [project]
 name = "eyeGestures"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
   { name="Piotr Walas", email="piotr.walas@eyegestures.com" },
 ]
 maintainers = [
   { name="Piotr Walas", email="piotr.walas@eyegestures.com" }
 ]
 description = "Package for eye tracking algorithm allowing for development of gaze controlled computer interface"
```

### Comparing `eyegestures-1.3.3/PKG-INFO` & `eyegestures-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: eyeGestures
-Version: 1.3.3
+Version: 1.3.4
 Summary: Package for eye tracking algorithm allowing for development of gaze controlled computer interface
 Project-URL: Homepage, https://github.com/NativeSensors/EyeGestures
 Project-URL: Issues, https://github.com/NativeSensors/EyeGestures/Issues
 Author-email: Piotr Walas <piotr.walas@eyegestures.com>
 Maintainer-email: Piotr Walas <piotr.walas@eyegestures.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -684,17 +684,23 @@
 Keywords: eye,eyetracking,gaze,gazetracking,tracking
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
+
+
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eyeGestures)
+
 ```
 For enterprise avoiding GPL3 licensing there is commercial license!
 ```
+We offer custom integration and managed services. For businesses requiring invoices message us `contact@eyegestures.com`.
+
 ## 👁️ EyeGestures
 
 EyeGestures is open source eyetracking software/library using native webcams and phone camers for achieving its goal. The aim of library is to bring accessibility of eyetracking and eyedriven interfaces without requirement of obtaining expensive hardware.
 
 <p align="center">
   <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/2ad25252-e96e-47d4-b25f-c47ba7f0f4f3" width="300" height="150">
 <img src="https://github.com/PeterWaIIace/PeterWaIIace/assets/40773550/f3132843-063a-439a-8e1c-2385ddfdccda" width="300
@@ -726,37 +732,48 @@
 <a href="https://polar.sh/NativeSensors"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe&darkmode"><img alt="Subscribe on Polar" src="https://polar.sh/embed/subscribe.svg?org=NativeSensors&label=Subscribe"></picture></a>
 
 ### 💜 Sponsors: 
 
 ```
 Sponsor us and we can add your link, banner or other promo materials!
 ```
+<!-- POLAR type=ads id=eizdelwu subscription_benefit_id=bb272b6d-f698-44e3-a417-36a6fa203bbe width=240 height=100 -->
+
+
+
+<!-- POLAR-END id=eizdelwu -->
 
 ### 📢 Announcements:
 
 <a href="https://polar.sh/NativeSensors/posts"><picture><source media="(prefers-color-scheme: dark)" srcset="https://polar.sh/embed/posts.svg?org=NativeSensors&darkmode"><img alt="Posts on Polar" src="https://polar.sh/embed/posts.svg?org=NativeSensors"></picture></a>
 
 ### 🔥 Web Demos:
 
 - [Main page](https://eyegestures.com/)
 - [Game demo](https://eyegestures.com/game)
 - [Cinema demo](https://eyegestures.com/cinema)
+- [Restaurant](https://eyegestures.com/restaurant)
 
 ### 💻 Install
 ```
-pybuild.sh ; python3 -m pip install dist/eyegestures-1.2.2-py3-none-any.whl
+python3 -m pip install eyeGestures
 ```
 
 Note: you may need to change version of package `eyegestures-X.X.X`.
 
 ### ⚙️ Run 
 ```
 python3 examples/simple_example.py
 ```
 
+### 🪟 Run Windows App 
+```
+python3 apps/win_app.py
+```
+
 ### 🔧 Develop 
 
 To begin, you instantiate an EyeGestures object with initial Region of Interest (RoI) parameters. These parameters define a preliminary focus area for the tracker within a virtual 500x500 screen space, which helps in locating the user's gaze more efficiently.
 
 Main `EyeGesture` object provides general configuration initial conditions: 
 
 ```python
```

