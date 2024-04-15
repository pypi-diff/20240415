# Comparing `tmp/brickbundles-0.5.0-py3-none-any.whl.zip` & `tmp/brickbundles-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,20 @@
-Zip file size: 107724 bytes, number of entries: 274
+Zip file size: 109995 bytes, number of entries: 278
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Actuator.brick
 -rw-r--r--  2.0 unx      742 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Differential.brick
+-rw-r--r--  2.0 unx     3717 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/EmpiricalTorqueConverter.brick
 -rw-r--r--  2.0 unx      675 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Engine.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Gear.brick
--rw-r--r--  2.0 unx      112 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/HingeActuator.brick
--rw-r--r--  2.0 unx      281 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/PrismaticActuator.brick
+-rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/HingeActuator.brick
+-rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/PrismaticActuator.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Shaft.brick
 -rw-r--r--  2.0 unx      201 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/GearTorqueOutput.brick
+-rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueConverterLockUpStateInput.brick
+-rw-r--r--  2.0 unx      168 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueConverterPumpTorqueOutput.brick
+-rw-r--r--  2.0 unx      171 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueConverterTurbineTorqueOutput.brick
 -rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Signals/TorqueMotorInput.brick
 -rw-r--r--  2.0 unx     1193 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick
 -rw-r--r--  2.0 unx       53 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/TorqueMotor.brick
 -rw-r--r--  2.0 unx      112 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/config.brick
 -rw-r--r--  2.0 unx      420 b- defN 80-Jan-01 00:00 brickbundles/Math/AffineTransform.brick
 -rw-r--r--  2.0 unx      141 b- defN 80-Jan-01 00:00 brickbundles/Math/Constants.brick
 -rw-r--r--  2.0 unx      285 b- defN 80-Jan-01 00:00 brickbundles/Math/Functions.brick
@@ -266,11 +270,11 @@
 -rw-r--r--  2.0 unx      234 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick
 -rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Geometry.brick
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Sphere.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/TriMeshGeometry.brick
 -rw-r--r--  2.0 unx       10 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Materials/Material.brick
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 brickbundles/Visuals/config.brick
 -rw-r--r--  2.0 unx     1346 b- defN 80-Jan-01 00:00 brickbundles/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.5.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    30405 b- defN 16-Jan-01 00:00 brickbundles-0.5.0.dist-info/RECORD
-274 files, 127932 bytes uncompressed, 56568 bytes compressed:  55.8%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.6.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    30893 b- defN 16-Jan-01 00:00 brickbundles-0.6.0.dist-info/RECORD
+278 files, 132570 bytes uncompressed, 58007 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: brickbundles/DriveTrain/Actuator.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Differential.brick
 Comment: 
 
+Filename: brickbundles/DriveTrain/EmpiricalTorqueConverter.brick
+Comment: 
+
 Filename: brickbundles/DriveTrain/Engine.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Gear.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/HingeActuator.brick
@@ -18,14 +21,23 @@
 
 Filename: brickbundles/DriveTrain/Shaft.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/Signals/GearTorqueOutput.brick
 Comment: 
 
+Filename: brickbundles/DriveTrain/Signals/TorqueConverterLockUpStateInput.brick
+Comment: 
+
+Filename: brickbundles/DriveTrain/Signals/TorqueConverterPumpTorqueOutput.brick
+Comment: 
+
+Filename: brickbundles/DriveTrain/Signals/TorqueConverterTurbineTorqueOutput.brick
+Comment: 
+
 Filename: brickbundles/DriveTrain/Signals/TorqueMotorInput.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick
 Comment: 
 
 Filename: brickbundles/DriveTrain/TorqueMotor.brick
@@ -807,17 +819,17 @@
 
 Filename: brickbundles/Visuals/config.brick
 Comment: 
 
 Filename: brickbundles/__init__.py
 Comment: 
 
-Filename: brickbundles-0.5.0.dist-info/METADATA
+Filename: brickbundles-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: brickbundles-0.5.0.dist-info/WHEEL
+Filename: brickbundles-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: brickbundles-0.5.0.dist-info/RECORD
+Filename: brickbundles-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## brickbundles/DriveTrain/HingeActuator.brick

```diff
@@ -1,4 +1,3 @@
 
-HingeActuator:
-    connector_1d is Physics1D.Charges.MateConnector
-    mate_3d is Physics3D.Interactions.Hinge
+HingeActuator is Actuator:
+    mate_3d becomes Physics3D.Interactions.Hinge
```

## brickbundles/DriveTrain/PrismaticActuator.brick

```diff
@@ -1,8 +1,7 @@
 
-PrismaticActuator:
+PrismaticActuator is Actuator:
     .doc: """
     Actuation of the linear degree of freedom of the 3D Prismatic
     by rotaional to translational conversion from a 1D rotational shaft.
     """
-    connector_1d is Physics1D.Charges.MateConnector
-    mate_3d is Physics3D.Interactions.Prismatic
+    mate_3d becomes Physics3D.Interactions.Prismatic
```

## Comparing `brickbundles-0.5.0.dist-info/METADATA` & `brickbundles-0.6.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrickBundles
-Version: 0.5.0
+Version: 0.6.0
 Summary: Brick Bundles package, i.e. all Brick sourcefiles and convenience access method in a package
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `brickbundles-0.5.0.dist-info/RECORD` & `brickbundles-0.6.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 brickbundles/DriveTrain/Actuator.brick,sha256=x2MlOtidmaIG8Q0FWMu5piL5R9OQMOmD7VIMC9Z3CNM,106
 brickbundles/DriveTrain/Differential.brick,sha256=0wcO8TMm85pxdDeQfNCq75BO7V85jpcYyFdfiCPyB5A,742
+brickbundles/DriveTrain/EmpiricalTorqueConverter.brick,sha256=Dsm0NY3fK1ivflaFViEHI72oQR0GaUAhSb9om9WydYE,3717
 brickbundles/DriveTrain/Engine.brick,sha256=Is3sdxaZfoGcV5D45wSgSN0puv_6cIV1VUUkyt0HSTU,675
 brickbundles/DriveTrain/Gear.brick,sha256=zlJtK6Ii-t08ZXLTZ38lGZlp3_qi8C-8GN5cwTfrbu8,133
-brickbundles/DriveTrain/HingeActuator.brick,sha256=A1eSKcju316hLDp4jZ5MsnKZsbmQXUZIAlHuy0vX7Ro,112
-brickbundles/DriveTrain/PrismaticActuator.brick,sha256=Cu0E814_u5OVhf6iAjzXi0R-qW86f0l5MBvMLfFiVow,281
+brickbundles/DriveTrain/HingeActuator.brick,sha256=8-8on4lblbEYqyggeL1oJaS9j69zCEAPTEy2WRHuX-o,77
+brickbundles/DriveTrain/PrismaticActuator.brick,sha256=V6w4GIamptmkQDK97VMN2tlMznv1Bmr6iQAw8ckzqyg,246
 brickbundles/DriveTrain/Shaft.brick,sha256=5IwBB9q-73xngtKf3cLJt09lD-QoelUQYZ2miMzFZdw,133
 brickbundles/DriveTrain/Signals/GearTorqueOutput.brick,sha256=Asi_heEYQ5C7aS3a4KUSyM6VxPBhnBZ0Etfm34PrhhU,201
+brickbundles/DriveTrain/Signals/TorqueConverterLockUpStateInput.brick,sha256=42E3R72GzNBxdazIgAEojdt1fYlVjATD6bTtHVY0UCY,164
+brickbundles/DriveTrain/Signals/TorqueConverterPumpTorqueOutput.brick,sha256=t86UmbtYuJBfqoPpR2Qe3a9zKhfrc9nGRSr2SgSWPro,168
+brickbundles/DriveTrain/Signals/TorqueConverterTurbineTorqueOutput.brick,sha256=JHOvw6eYe0lGO7rx5DanAX1W1KnLjUo3xbz0NAHYtfg,171
 brickbundles/DriveTrain/Signals/TorqueMotorInput.brick,sha256=cUOqFfihVtsq2ZSLq_bDKb6Nl0BOI9zUknnhnFV5SR8,128
 brickbundles/DriveTrain/TorqueLimitedSlipDifferential.brick,sha256=rDsDLx-93miXe4vGLukv7zMU9YGlZywUDk73oAGQ34Q,1193
 brickbundles/DriveTrain/TorqueMotor.brick,sha256=eUs07jvCdqwdJiUdiXDmANVAnW1kYNtmwuxuBSUycRM,53
 brickbundles/DriveTrain/config.brick,sha256=v4CrbDzcvkJqxfoLuApV8NC7f1JxJW8F6haJiym0e90,112
 brickbundles/Math/AffineTransform.brick,sha256=YrFSwBjhHoLf72D2OawtrKYCFjp7aqVe8BTnv3aUSx8,420
 brickbundles/Math/Constants.brick,sha256=lripEIYTI9AkFuln4alNrGrsUA0U2i21Q5HZplTn38E,141
 brickbundles/Math/Functions.brick,sha256=ofmSeTWw8ppjOKG6WGkcMhl-WRqIeDWiFMZlQTZ8sX0,285
@@ -265,10 +269,10 @@
 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick,sha256=0cEEaVuE72vhJvAv6J1guVo6yZVOCf7Q4gFP9KvElGQ,234
 brickbundles/Visuals/Geometries/Geometry.brick,sha256=-tiwTgsHtKnrPvaPO6kj5LG_gfF0csLAxdJUXJJzywg,90
 brickbundles/Visuals/Geometries/Sphere.brick,sha256=K3DerE_AE6EnHc_2GmT1e9sYrCMUosmUlTXIcqYapBg,39
 brickbundles/Visuals/Geometries/TriMeshGeometry.brick,sha256=qctdVQYflyKPuuX6HK8QvTgRbKNYlI5JAB82UNmKTZs,96
 brickbundles/Visuals/Materials/Material.brick,sha256=hVvFGaQhcFJblZ1R0SLDhWjIY6lSKC84i9hBwmA3sq8,10
 brickbundles/Visuals/config.brick,sha256=Z7y-m-8BN9N4V0OvqKp8BKivcspo8_-IpA2xA5xvf80,72
 brickbundles/__init__.py,sha256=VC7H2Q-oD1kqfe06eBZdgPlW8tC1kzBRQXWHkOIYk24,1346
-brickbundles-0.5.0.dist-info/METADATA,sha256=7k4V8mNlCYDuMTlJsMGZWkbY6hc4bsKhpZqRa2d9aTQ,1066
-brickbundles-0.5.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-brickbundles-0.5.0.dist-info/RECORD,,
+brickbundles-0.6.0.dist-info/METADATA,sha256=xF_W6UX1VA9rt5cTmb9Vcp5bzxKlsL6EjbuxF1s_dsQ,1066
+brickbundles-0.6.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+brickbundles-0.6.0.dist-info/RECORD,,
```

