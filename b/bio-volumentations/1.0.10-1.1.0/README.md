# Comparing `tmp/bio_volumentations-1.0.10.tar.gz` & `tmp/bio_volumentations-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio_volumentations-1.0.10.tar", last modified: Wed Feb 14 12:18:06 2024, max compression
+gzip compressed data, was "bio_volumentations-1.1.0.tar", last modified: Mon Apr 15 09:39:58 2024, max compression
```

## Comparing `bio_volumentations-1.0.10.tar` & `bio_volumentations-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,32 @@
-drwxrwxr-x   0 michelkiwi  (1000) michelkiwi  (1000)        0 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)      401 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/PKG-INFO
-drwxrwxr-x   0 michelkiwi  (1000) michelkiwi  (1000)        0 2024-02-14 12:18:06.479941 bio_volumentations-1.0.10/bio_volumentations/
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     3889 2024-02-14 12:17:00.000000 bio_volumentations-1.0.10/bio_volumentations/__init__.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)       22 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/__version__.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     2541 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/demo.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     5819 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/devel.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)      840 2024-02-14 12:17:07.000000 bio_volumentations-1.0.10/bio_volumentations/setup.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     3898 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/speed_test.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     1345 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/tst_volumentations_speed.py
-drwxrwxr-x   0 michelkiwi  (1000) michelkiwi  (1000)        0 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     3781 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/__init__.py
-drwxrwxr-x   0 michelkiwi  (1000) michelkiwi  (1000)        0 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/augmentations/
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     3712 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/augmentations/__init__.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)    27936 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/augmentations/functional.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)    60764 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/augmentations/transforms.py
-drwxrwxr-x   0 michelkiwi  (1000) michelkiwi  (1000)        0 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/conversion/
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     3669 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/conversion/__init__.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     3830 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/conversion/functional.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     6470 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/conversion/transforms.py
-drwxrwxr-x   0 michelkiwi  (1000) michelkiwi  (1000)        0 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/core/
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     3631 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/core/__init__.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     4786 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/core/composition.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     6745 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/core/transforms_interface.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     4916 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/random_utils.py
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)      784 2024-02-14 12:08:10.000000 bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/setup.py
-drwxrwxr-x   0 michelkiwi  (1000) michelkiwi  (1000)        0 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/bio_volumentations.egg-info/
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)      401 2024-02-14 12:18:06.000000 bio_volumentations-1.0.10/bio_volumentations.egg-info/PKG-INFO
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)     1300 2024-02-14 12:18:06.000000 bio_volumentations-1.0.10/bio_volumentations.egg-info/SOURCES.txt
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)        1 2024-02-14 12:18:06.000000 bio_volumentations-1.0.10/bio_volumentations.egg-info/dependency_links.txt
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)       65 2024-02-14 12:18:06.000000 bio_volumentations-1.0.10/bio_volumentations.egg-info/entry_points.txt
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)       39 2024-02-14 12:18:06.000000 bio_volumentations-1.0.10/bio_volumentations.egg-info/requires.txt
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)       19 2024-02-14 12:18:06.000000 bio_volumentations-1.0.10/bio_volumentations.egg-info/top_level.txt
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)       38 2024-02-14 12:18:06.483941 bio_volumentations-1.0.10/setup.cfg
--rw-rw-r--   0 michelkiwi  (1000) michelkiwi  (1000)      840 2024-02-14 12:16:40.000000 bio_volumentations-1.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/
+-rw-rw-rw-   0        0        0     1120 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    11364 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9047 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.300001 bio_volumentations-1.1.0/bio_volumentations/
+-rw-rw-rw-   0        0        0     4025 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.316562 bio_volumentations-1.1.0/bio_volumentations/augmentations/
+-rw-rw-rw-   0        0        0     3953 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/__init__.py
+-rw-rw-rw-   0        0        0    25874 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/functional.py
+-rw-rw-rw-   0        0        0     6343 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/spatial_funcional.py
+-rw-rw-rw-   0        0        0    63200 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/transforms.py
+-rw-rw-rw-   0        0        0     7379 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/bio_volumentations/conversion/
+-rw-rw-rw-   0        0        0     3910 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/conversion/__init__.py
+-rw-rw-rw-   0        0        0     4070 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/conversion/functional.py
+-rw-rw-rw-   0        0        0     7095 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/conversion/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/bio_volumentations/core/
+-rw-rw-rw-   0        0        0     3869 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/core/__init__.py
+-rw-rw-rw-   0        0        0     6040 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/core/composition.py
+-rw-rw-rw-   0        0        0     6382 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/core/transforms_interface.py
+-rw-rw-rw-   0        0        0     5558 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/random_utils.py
+-rw-rw-rw-   0        0        0     2557 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/typing.py
+drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/bio_volumentations.egg-info/
+-rw-rw-rw-   0        0        0    11364 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2686 2024-04-15 09:39:45.000000 bio_volumentations-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/tests/
+-rw-rw-rw-   0        0        0      204 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/tests/test_random_utils.py
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/__init__.py` & `bio_volumentations-1.1.0/bio_volumentations/augmentations/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-from .volumentations_biomedicine.augmentations.transforms import *
-from .volumentations_biomedicine.conversion.transforms import *
-from .volumentations_biomedicine.core.composition import *
-from .volumentations_biomedicine.core.transforms_interface import *
-
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+from ..augmentations.functional import *
+from ..augmentations.transforms import *
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/__init__.py` & `bio_volumentations-1.1.0/bio_volumentations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-from .augmentations.transforms import *
-from .conversion.transforms import *
-from .core.composition import *
-from .core.transforms_interface import *
-
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+from .augmentations.transforms import *
+from .conversion.transforms import *
+from .core.composition import *
+from .core.transforms_interface import *
+
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/augmentations/transforms.py` & `bio_volumentations-1.1.0/bio_volumentations/augmentations/transforms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1200 +1,1415 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-from warnings import warn
-
-import random
-import numpy as np
-from ..core.transforms_interface import *
-from ..augmentations import functional as F
-from ..random_utils import *
-from typing import Any, Dict, List, Sequence, Tuple, Union
-
-# TODO apply_mask/float - ine spravanie? zatial vsade to iste
-
-#Potentional upgrade : different sigmas for different channels
-class GaussianNoise(ImageOnlyTransform):
-    """Adds gaussian noise to the image.
-
-        Noise is drawn from the normal distribution. 
-
-        Args:
-            var_limit (tuple, optional): variance of normal distribution is randomly chosen from this interval. Defaults to (0.001, 0.1).
-            mean (float, optional): mean of normal distribution. Defaults to 0.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-
-
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, var_limit: tuple = (0.001, 0.1), mean: float = 0,
-                 always_apply: bool = False, p: float = 0.5):
-        super().__init__(always_apply, p)
-        self.var_limit = var_limit
-        self.mean = mean
-
-    def apply(self, img, gauss=None):
-        return F.gaussian_noise(img, gauss=gauss)
-
-    def get_params(self, **data):
-        image = data["image"]
-        var = uniform(self.var_limit[0], self.var_limit[1])
-        sigma = var ** 0.5
-        gauss = normal(self.mean, sigma, image.shape)
-        return {"gauss": gauss}
-
-    def __repr__(self):
-        return f'GaussianNoise({self.var_limit}, {self.mean}, {self.always_apply}, {self.p})'
-
-#TODO anti_aliasing_downsample keep parameter or remove?
-class Resize(DualTransform):
-    """Resize input to the given shape.
-
-        Resize input using skimage resize function. Shape is expected without channel dimensions. If there is one less dimension,
-        than expected then size of last dimension(time) is unchanged. Interpolation, border_mode, ival, mval and anti_aliasing_downsample
-        are arguments for https://scikit-image.org/docs/stable/api/skimage.transform.html#skimage.transform.resize 
-
-        Args:
-            shape (tuple of ints): shape of desired image without channel dimension. If inputed with one less dimensions,
-                it is expected that it is time dimensions and is copied from image.
-            interpolation (int, optional): order of spline interpolation for image. Defaults to 1.
-            border_mode (string, optional): points outside image are filled according to the this mode. Defaults to 'reflect'.
-            ival (float, optional): value outside of image when the border_mode is chosen to be "constant". Defaults to 0.
-            mval (float, optional): value outside of mask when the border_mode is chosen to be "constant". Defaults to 0.
-            anti_aliasing_downsample (bool, optional): controls if the gaussian filter should be used on image before downsampling, recommended. Defaults to True.
-            ignore_index (float | None, optional): If ignore_index is float, then transformation of mask is done with 
-                border_mode = "constant" and mval = ignore_index. If ignore_index is None, then it does nothing. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, shape: tuple, interpolation: int = 1, border_mode: str = 'reflect', ival: float = 0, mval: float = 0,
-                 anti_aliasing_downsample: bool = True, ignore_index : Union[float, None] = None, always_apply: bool = False, p: float = 1):
-        
-        super().__init__(always_apply, p)
-        self.shape = shape
-        self.interpolation = interpolation
-        self.border_mode = border_mode
-        self.mask_mode = border_mode
-        self.ival = ival
-        self.mval = mval
-        self.anti_aliasing_downsample = anti_aliasing_downsample
-        if not (ignore_index is None):
-            self.mask_mode = "constant"
-            self.mval = ignore_index
-
-    def apply(self, img):
-        return F.resize(img, input_new_shape=self.shape, interpolation=self.interpolation,
-                        border_mode=self.border_mode, cval=self.ival, anti_aliasing_downsample=self.anti_aliasing_downsample)
-
-    def apply_to_mask(self, mask):
-        return F.resize(mask, input_new_shape=self.shape, interpolation=0,
-                        border_mode=self.mask_mode, cval=self.mval, anti_aliasing_downsample=False,
-                        mask=True)
-        
-    def __repr__(self):
-        return f'Resize({self.shape}, {self.interpolation}, {self.border_mode} , {self.ival}, {self.mval}, {self.anti_aliasing_downsample},   {self.always_apply}, {self.p})'
-
-class Scale(DualTransform):
-    """Rescale input by the given scale.
-
-        Rescaling is done by function zoom from scipy. If scale_factor is float, spatial dimensions are scaled by this number.
-        If it is list, then it is expected without channel dimensions. If there is one less dimension, than expected then size of last dimensions(time) is unchanged.
-        Check https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.zoom.html for additional arguments.
-
-        Args:
-            scale_factor (float|List[float], optional): Value by which the input should be scaled. If 
-                there is single value, then all spatial dimensions are scaled by it. If 
-                input is list then all dimensions except for channel one are scaled by it. If 
-                there is one less dimensions then last dimension(time) is not scaled. Defaults to 1.
-            interpolation (int, optional): order of spline interpolation for image.. Defaults to 1.
-            border_mode (str, optional): points outside image are filled according to the this mode. Defaults to 'reflect'.
-            ival (float, optional): value outside of image when the border_mode is chosen to be "constant". Defaults to 0.
-            mval (float, optional): value outside of mask when the border_mode is chosen to be "constant". Defaults to 0.
-            ignore_index (float | None, optional): If ignore_index is float, then transformation of mask is done with 
-                border_mode = "constant" and mval = ignore_index. If ignore_index is None, then it does nothing. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, scale_factor: Union[float, List[float]] = 1, interpolation: int = 1, border_mode: str = 'reflect',
-                 ival: float = 0, mval: float = 0, ignore_index : Union[float, None] = None, always_apply: bool = False, p: int = 1):
-        super().__init__(always_apply, p)
-        self.scale_factor = scale_factor
-        self.interpolation = interpolation
-        self.border_mode = border_mode
-        self.mask_mode = border_mode
-        self.ival = ival
-        self.mval = mval
-        if not (ignore_index is None):
-            self.mask_mode = "constant"
-            self.mval = ignore_index
-
-    def apply(self, img):
-        return F.scale(img, input_scale_factor=self.scale_factor, interpolation=self.interpolation,
-                       border_mode=self.border_mode, cval=self.ival, mask=False)
-
-    def apply_to_mask(self, mask):
-        return F.scale(mask, input_scale_factor=self.scale_factor, interpolation=0,
-                       border_mode=self.mask_mode, cval=self.mval, mask=True)
-
-    def __repr__(self):
-        return f'Scale({self.scale_factor}, {self.interpolation}, {self.border_mode}, {self.ival}, {self.mval}, {self.always_apply}, {self.p})'
-
-class RandomScale(DualTransform):
-    """Randomly rescale input by the given scale.
-
-        Under the hood, https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.zoom.html is being used.
-
-        Args:
-            scale_limit (float | Tuple[float] | List[Tuple[float]], optional): Value by which the input should be scaled. 
-                If there is single value, then all spatial dimensions are scaled by it. 
-                If input is tuple, it creates interval from which the single value for scaling will be chosen. 
-                If input is list it should have length of number axes of input - 1 (- channel dimension) and 
-                contains tuple of 2 elements. All dimensions except for channel one 
-                are scaled by the number from the interval given by tuple. If there is one less dimensions then
-                last dimension(time) is not scaled. Defaults to (0.9, 1.1).
-            interpolation (int, optional): order of spline interpolation for image. Defaults to 1.
-            border_mode (str, optional): points outside image are filled according to the this mode.. Defaults to 'reflect'.
-            ival (float, optional): value outside of image when the border_mode is chosen to be "constant". Defaults to 0.
-            mval (float, optional): value outside of mask when the border_mode is chosen to be "constant". Defaults to 0.
-            ignore_index (float | None, optional): If ignore_index is float, then transformation of mask is done with 
-                border_mode = "constant" and mval = ignore_index. If ignore_index is None, then it does nothing. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """      
-    def __init__(self, scale_limit: Union[float,Tuple[float], List[Tuple[float]]] = (0.9, 1.1), interpolation: int = 1,
-                 border_mode: str = 'reflect', ival: float = 0, mval: float = 0, ignore_index : Union[float, None] = None,
-                 always_apply: bool = False, p: float = 0.5):  
-        super().__init__(always_apply, p)
-        self.scale_limit = scale_limit
-        self.interpolation = interpolation
-        self.border_mode = border_mode
-        self.mask_mode = border_mode
-        self.ival = ival
-        self.mval = mval
-        if not (ignore_index is None):
-            self.mask_mode = "constant"
-            self.mval = ignore_index
-
-    def get_params(self, **data):
-        scale = None
-        if isinstance(self.scale_limit, (float, int)):
-             tuple_scale_limit = to_tuple(self.scale_limit, bias=1)
-             scale = random.uniform(tuple_scale_limit[0], tuple_scale_limit[1])
-
-        elif isinstance(self.scale_limit, tuple):
-            if len(self.scale_limit) != 2:
-                warn(f"RandomScale(): scale_limit : {self.scale_limit} tuple should contain exactly 2 elements. ", UserWarning)    
-            scale = random.uniform(self.scale_limit[0], self.scale_limit[1])
-
-        elif isinstance(self.scale_limit, list):
-            scale = []
-            for dimension in self.scale_limit:
-                if isinstance(dimension, tuple):
-                    if len(dimension) != 2:
-                        warn(f"RandomScale(): scale_limit : {dimension} tuple should contain exactly 2 elements. ", UserWarning)
-                    scale.append(random.uniform(dimension[0], dimension[1]))
-                elif isinstance(dimension, (float, int)):
-                    tuple_scale =  to_tuple(dimension, bias=1)
-                    scale.append(random.uniform(tuple_scale[0], tuple_scale[1]))
-
-                else:
-                    warn(f"RandomScale(): scale_limit : {self.scale_limit} List contains something different than float or tuple. Scaling with 1. ", UserWarning)
-                    scale.append(1)
-
-        if scale is None:
-            warn(f"RandomScale(): scale_limit : {self.scale_limit} is not a tuple or List. ", UserWarning)
-        #Negative scaling factor check
-        if isinstance(scale, (float,int)):
-            if scale <= 0:
-                warn(f"RandomScale(): scaling factor: {scale} would be negative or zero, changing it to 1. ", UserWarning)
-                scale = 1
-        elif isinstance(scale, List):
-            for i,dimension  in enumerate(scale):
-                if dimension <= 0:
-                    warn(f"RandomScale(): Part of scaling factor: {scale} would be negative, changing it to 1. ", UserWarning)
-                    scale[i] = 1
-        
-        return {"scale": scale}
-
-    def apply(self, img, scale):
-        return F.scale(img, input_scale_factor=scale, interpolation=self.interpolation, border_mode=self.border_mode, cval=self.ival,
-                       mask=False)
-
-    def apply_to_mask(self, mask, scale):
-        return F.scale(mask, input_scale_factor=scale, interpolation=0, border_mode=self.mask_mode, cval=self.mval,
-                       mask=True)
-
-    def __repr__(self):
-        return f'RandomScale({self.scale_limit}, {self.interpolation}, {self.always_apply}, {self.p})'
-
-class RandomRotate90(DualTransform):
-    """Rotation of input by 0/90/180/270 degrees in spatial dimensions.
-
-        Input is being rotated around the specified axes. For example if axes = [3,2], 
-        then input is rotated around 3 axis (1 and 2 axes are changing)
-        and afterwards it is rotated around 2 axis(1 and 3 axes are changing).
-
-        Args:
-            axes (List[int], optional): list of axes around which input is rotated and also determines 
-                order if shuffle_axis is false. Ignoring axes which are not in this list [1,2,3]. 
-                Number in axes do not need to be unique. Defaults to [1, 2, 3].
-            shuffle_axis (bool, optional): If set to True, order of rotations is random. Defaults to False.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, axes: List[int] = [1, 2, 3], shuffle_axis : bool = False,  
-                 always_apply: bool = False, p: float = 0.5):
-        super().__init__(always_apply, p)
-        self.axes = axes
-        self.shuffle_axis = shuffle_axis
-
-    def apply(self, img, rotation_around, factor):
-        for i in range(len(rotation_around)):
-            img = np.rot90(img, factor[i], axes=rotation_around[i])
-        return img
-
-    def apply_to_mask(self, mask, rotation_around, factor):
-        for i in range(len(rotation_around)):
-            mask = np.rot90(mask, factor[i], axes=(
-                rotation_around[i][0] - 1, rotation_around[i][1] - 1))
-        return mask
-
-    def get_params(self, **data):
-        # Create all combinations for rotating + randomly shuffle
-        # TODO what if self.axes == None
-        # TODO add check if the axes are not exceeding dimensions + are they rotating channels?
-        if self.axes is None:
-            self.axes = [1,2,3]
-        axes_to_rotate = {1 : (2,3), 2: (1,3), 3 : (1,2)}
-        rotation_around = []
-        allowed_axes = [1,2,3]
-        for i in self.axes:
-            if i in allowed_axes:
-                rotation_around.append(axes_to_rotate[i])
-        if self.shuffle_axis:
-            random.shuffle(rotation_around)
-        factor = [random.randint(0, 3) for i in range(len(rotation_around))]
-        return {"factor": factor,
-                "rotation_around": rotation_around}
-
-    def __repr__(self):
-        return f'RandomRotate90({self.axes}, {self.always_apply}, {self.p})'
-
-class Flip(DualTransform):
-    """Flips input around specified axes. 
-
-        Args:
-            axes (List[int], optional): List of axes around which is flip done. Defaults to [1,2,3].
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, axes: List[int] = [1,2,3], always_apply=False, p=1):
-        super().__init__(always_apply, p)
-        self.axes = axes
-
-    def apply(self, img, axes):
-        return np.flip(img, axes)
-
-    def apply_to_mask(self, mask, axes):
-        # Mask has no dimension channel
-        return np.flip(mask, axis=[item - 1 for item in axes])
-
-    def get_params(self, **data):
-        if self.axes is None:
-            axes = [1,2,3]
-        else:
-            axes = self.axes
-        return {"axes": axes}
-
-    def __repr__(self):
-        return f'Flip({self.axes}, {self.always_apply}, {self.p})'
-
-class RandomFlip(DualTransform):
-    """Flips a input around a tuple of axes randomly chosen from the input list of axis combinations.
-
-        If axes_to_choose to choose is None, random subset of spatial axes is chosen.
-
-        Args:
-        
-            axes_to_choose (List[Tuple[int]] or None, optional): Randomly chooses tuple of axes from list around 
-                which to flip input. If None then a random subset of spatial axes is chosen. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, axes_to_choose: Union[None, List[Tuple[int]]] = None, always_apply=False, p=0.5):
-        super().__init__(always_apply, p)
-        self.axes = axes_to_choose
-
-    def apply(self, img, axes):
-        return np.flip(img, axes)
-
-    def apply_to_mask(self, mask, axes):
-        # Mask has no dimension channel
-        return np.flip(mask, axis=[item - 1 for item in axes])
-
-    def get_params(self, **data):
-        
-        if self.axes is None or len(self.axes) == 0:
-            # Pick random combination of axes to flip
-            combinations = [(1,), (2,), (3,), (1, 2),
-                            (1, 3), (2, 3), (1, 2, 3)]
-            axes = random.choice(combinations)
-        else:
-            # Pick a random choice from input
-            axes = random.choice(self.axes)
-        return {"axes": axes}
-
-    def __repr__(self):
-        return f'Flip({self.axes}, {self.always_apply}, {self.p})'
-
-class CenterCrop(DualTransform):
-    """Crops center region of the input. Size of this crop is given by shape.
-          
-        Unlike CenterCrop from Albumentations, this transform pads the input in dimensions 
-        where the input is smaller than the crop-shape with numpy.pad, for which are border_mode, ival and mval.
-
-        https://numpy.org/doc/stable/reference/generated/numpy.pad.html
-
-        Args:
-            shape (Tuple[int]) Final shape of input, expected without first axis of image (representing channels): 
-            border_mode (str, optional): border mode used for numpy.pad. Defaults to "reflect".
-            ival (Tuple[float], optional): values used for 'constant' or 'linear_ramp' for image. Defaults to (0, 0).
-            mval (Tuple[float], optional): values used for 'constant' or 'linear_ramp' for mask. Defaults to (0, 0).
-            ignore_index (float | None, optional): If ignore_index is float, then transformation of mask is done with 
-                border_mode = "constant" and mval = ignore_index. If ignore_index is None, then it does nothing. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, shape: Tuple[int], border_mode: str = "reflect", ival: Union[Sequence[float], float] = (0, 0),
-                 mval: Union[Sequence[float], float] = (0, 0), ignore_index : Union[float, None] = None,
-                 always_apply: bool = False, p: float = 1.0):
-        super().__init__(always_apply, p)
-        self.shape = np.asarray(shape, dtype=np.intc)
-        self.border_mode = border_mode
-        self.mask_mode = border_mode
-        self.ival = ival
-        self.mval = mval
-        
-        if not (ignore_index is None):
-            self.mask_mode = "constant"
-            self.mval = ignore_index
-        
-
-    def apply(self, img):
-        return F.center_crop(img, self.shape, self.border_mode, self.ival, False)
-
-    def apply_to_mask(self, mask):
-        return F.center_crop(mask, self.shape, self.mask_mode, self.mval, True)
-
-    def __repr__(self):
-        return f'CenterCrop({self.shape}, {self.always_apply}, {self.p})'
-
-class RandomCrop(DualTransform):
-    """Randomly crops region from input. Size of this crop is given by shape.
-
-        Unlike RandomCrop from Albumentations, this transform pads the input in dimensions 
-        where the input is smaller than the crop-shape with numpy.pad, for which are border_mode, ival and mval.
-
-
-
-        Args:
-            shape (Tuple[int]) Final shape of input, expected without first axis of image (representing channels): 
-            border_mode (str, optional): border mode used for numpy.pad. Defaults to "reflect".
-            ival (Tuple[float], optional): values used for 'constant' or 'linear_ramp' for image. Defaults to (0, 0).
-            mval (Tuple[float], optional): values used for 'constant' or 'linear_ramp' for mask. Defaults to (0, 0).
-            ignore_index (float | None, optional): If ignore_index is float, then transformation of mask is done with 
-                border_mode = "constant" and mval = ignore_index. If ignore_index is None, then it does nothing. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, shape: tuple, border_mode: str = "reflect", ival: Union[Sequence[float], float] = (0, 0),
-                 mval: Union[Sequence[float], float] = (0, 0), ignore_index : Union[float, None] = None,  
-                 always_apply: bool = False, p: float = 1.0):
-        super().__init__(always_apply, p)
-        self.shape = np.asarray(shape, dtype=np.intc)
-        self.border_mode = border_mode
-        self.mask_mode = border_mode
-        self.ival = ival
-        self.mval = mval
-
-        if not (ignore_index is None):
-            self.mask_mode = "constant"
-            self.mval = ignore_index
-
-    def apply(self, img, crop_start=np.array((0, 0, 0))):
-        return F.random_crop(img, self.shape, crop_start, self.border_mode, self.ival, mask = False)
-
-    def apply_to_mask(self, mask, crop_start=np.array((0, 0, 0))):
-        return F.random_crop(mask, self.shape, crop_start, self.mask_mode, self.mval, mask = True)
-
-    def get_params(self, **data):
-
-        return {
-            "crop_start": [random.random() for i in range(len(self.shape))]
-        }
-
-    def __repr__(self):
-        return f'RandomCrop({self.shape}, {self.always_apply}, {self.p})'
-
-#TODO translate, posuva aj cez casovu dimenziu. Pricom scaling_coef nie. Preto otázka ci to omezit or not.
-class AffineTransform(DualTransform):
-    """Rotation around spatial axes.
-
-        Rotation around each axis is chosen randomly from given interval in angle_limit. If a float X is given instead of 
-        for given axis then it becomes interval [-X, X]. If scaling_coef is used, it should be list with length equal 3. 
-        For closer clook at the interpolation, border_mode, ival and mval take a look at the scipy.ndimage.affine_transform.
-
-        Args:
-            angle_limit (List[Tuple[float] | float], optional): Contains intervals in degrees from which angle of rotation is 
-                chosen, for corresponding axis. Defaults to [(-15, 15),(-15, 15),(-15, 15)].
-            translantion_limit (List[Tuple[int], | int] | None, optional): List of length equal to the number of axes -1
-                (minus channel), each element controls translation in this axis. This list consists of intervals,
-                from which, it is then randomly chosen the translation vector. Defaults to None.
-            scaling_coef (List[float] | None, optional): List which contains scaling coefficients to make 
-                the image data isotropic in spatial dimensions. Length of list needs to be 3(number of spatial axes)
-                as only spatial dimensions are scaled. If scaling_coef is set to None, there is no scalling.
-                Recommended for anisotropic data and if one of spatial axis have significantly lower amount of
-                samples. Defaults to None.
-            scale_back (bool, optional): If scaling_coef is not None, then image is scaled back, to be anisotropic. Defaults to True.
-            interpolation (Int, optional): The order of spline interpolation. Defaults to 1.
-            border_mode (str, optional): The mode parameter determines how the input array is extended beyond its boundaries. Defaults to 'constant'.
-            ival (float, optional): Value to fill past edges of image if mode is 'constant'. Defaults to 0.
-            mval (float, optional): Value to fill past edges of mask if mode is 'constant'. Defaults to 0.
-            ignore_index ( float | None, optional): If ignore_index is float, then transformation of mask is done with 
-                border_mode = "constant" and mval = ignore_index. If ignore_index is None, then it does nothing. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, angle_limit : List[ Union[Tuple[float] , float]] = [15,15,15] , 
-                 translantion_limit : Union[List[Union[Tuple[int], int]], None] = None,
-                 scaling_coef: Union[List, None] = None, scale_back : bool = True, interpolation: int = 1, 
-                 border_mode: str = 'reflect', ival: float = 0, mval: float = 0, 
-                 ignore_index : Union[float, None] = None, always_apply: bool = False, p: float = 0.5):
-        super().__init__(always_apply, p)
-        self.translantion_limit = translantion_limit
-        self.scaling_coef = scaling_coef
-        self.interpolation = interpolation
-        self.border_mode = border_mode
-        self.mask_mode = border_mode
-        self.ival = ival
-        self.mval = mval
-        self.scale_back = scale_back
-
-        if not (ignore_index is None):
-            self.mask_mode = "constant"
-            self.mval = ignore_index
-
-        #if user adds tuple instead of list.
-        if isinstance(angle_limit, tuple):
-            self.angle_limit = list(angle_limit)
-        else:
-            self.angle_limit = angle_limit
-
-
-
-    def apply(self, img, x, y, z, translate):
-        return F.affine_transform(img, x, y, z, translate,  interpolation=self.interpolation, border_mode=self.border_mode,
-                              value=self.ival, input_scaling_coef=self.scaling_coef, scale_back= self.scale_back)
-
-    def apply_to_mask(self, mask, x, y, z, translate):
-        return F.affine_transform(mask, x, y, z, translate, interpolation=0, border_mode=self.mask_mode, value=self.mval, 
-                              input_scaling_coef=self.scaling_coef, scale_back= self.scale_back, mask=True)
-
-    def get_params(self, **data):
-        for number,axis in enumerate(self.angle_limit):
-            if isinstance(axis, (float,int)):
-                self.angle_limit[number] = to_tuple(axis) 
-        if self.translantion_limit is None:
-            translate = None
-        else:
-            translate = [random.randint(self.translantion_limit[i][0], self.translantion_limit[i][1]) 
-                         if isinstance(self.translantion_limit[i],(tuple,list))
-                         else self.translantion_limit[i] for i in range(len(self.translantion_limit))]
-        return {
-            "x": random.uniform(self.angle_limit[0][0], self.angle_limit[0][1]),
-            "y": random.uniform(self.angle_limit[1][0], self.angle_limit[1][1]),
-            "z": random.uniform(self.angle_limit[2][0], self.angle_limit[2][1]),
-            "translate" : translate
-        }
-
-# TODO create checks (mean, std, got good shape, and etc.), what if given list but only one channel, and reverse.
-class NormalizeMeanStd(ImageOnlyTransform):
-    """Normalization of image by given mean and std.
-
-        For a single channel image normalization is applied by the formula :math:`img = (img - mean) / std`.
-        
-        If image contains more channels, then for each channel previous formula is used.
-
-        Args:
-            mean (float | List[float]): Mean of image. If there are more channels, then it should be list of means for each channel.
-            std (float | List[float]): Std of image. If there are more channels, then it should be list of stds for each channel.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, mean: Union[List[float], float], std: Union[List[float], float],
-                 always_apply: bool = True, p: float = 1.0):
-        super(NormalizeMeanStd, self).__init__(always_apply, p)
-        self.mean = np.array(mean, dtype=np.float32) 
-        self.std = np.array(std, dtype=np.float32) 
-        self.denominator = np.reciprocal(self.std, dtype=np.float32)
-
-    def apply(self, image, **params):
-        return F.normalize_mean_std(image, self.mean, self.denominator)
-
-    def __repr__(self):
-        return f'NormalizeMeanStd({self.mean}, {self.std}, ' \
-               f' {self.always_apply}, {self.p})'
-
-class GaussianBlur(ImageOnlyTransform):
-    """Performs gaussian blur on the image.
-
-        Sigma parameter determines the strength of gaussian blur. There is no blurring between channels. 
-        By default there is no blurring also on time dimension. If given single number, channels and axes are blurred 
-        with same strength. If given tuple, blurring is performed with same effect over channels, but on each axis differently.
-        If given List, each channel is blurred differently, according to the element inside list.
-
-        For more information about border_mode and cval check scipy.ndimage.gaussian_filter.
-
-        Args:
-            sigma (float, Tuple(float), List[Tuple(float) | float] , optional): Determines strength of the blurring. 
-                List must have length equal to the number of channels. Tuple should have same number elements as number of axes - 1. Defaults to 0.8.
-            border_mode (str, optional): The mode parameter determines how the input array is extended beyond its boundaries. Defaults to "reflect".
-            cval (float, optional):  Value to fill past edges of image if mode is 'constant'. Defaults to 0.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, sigma: Union[float , Tuple[float], List[ Union[Tuple[float], float]]] = 0.8, border_mode: str = "reflect", cval: float = 0,
-                 always_apply: bool = False, p: float = 0.5):
-        
-        super(GaussianBlur, self).__init__(always_apply, p)
-        self.sigma = sigma
-        self.border_mode = border_mode
-        self.cval = cval
-
-    def apply(self, img, **params):
-        return F.gaussian_blur(img, self.sigma, self.border_mode, self.cval)
-
-class RandomGaussianBlur(ImageOnlyTransform):
-    """Performs gaussian blur on the image with a random strength blurring.
-
-        Behaves similarly to GaussianBlur, sigma has same format, but each number in sigma creates 
-        interval [start_of_interval, sigma_number], from which random number is chosen. 
-
-        Args:
-            sigma (float, Tuple(float), List[Tuple(float) | float, optional): Determines end of interval from which strength of blurring is chosen. Defaults to 0.8.
-            start_of_interval (float, optional): Determines start of interval from which strength of blurring is chosen. Defaults to 0.
-            border_mode (str, optional): The mode parameter determines how the input array is extended beyond its boundaries. Defaults to "reflect".
-            cval (float, optional):  Value to fill past edges of image if mode is 'constant'. Defaults to 0.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, max_sigma: Union[float , Tuple[float], List[ Union[Tuple[float], float]]] = 0.8, start_of_interval : float = 0 , border_mode: str = "reflect", cval: float = 0,
-                 always_apply: bool = False, p: float = 0.5):
-        super(RandomGaussianBlur, self).__init__(always_apply, p)
-        self.sigma = max_sigma
-        self.start_of_interval = start_of_interval
-        self.border_mode = border_mode
-        self.cval = cval
-
-    def apply(self, img, sigma, **params):
-        return F.gaussian_blur(img, sigma, self.border_mode, self.cval)
-
-    def get_params(self, **data):
-        if isinstance(self.sigma, (float,int)):
-            sigma = random.uniform(self.start_of_interval, self.sigma)
-        elif isinstance(self.sigma, tuple):
-            sigma = tuple([random.uniform(self.start_of_interval, self.sigma[i]) for i in range(len(self.sigma))])
-        else:
-            sigma = []
-            for channel in self.sigma:
-                if isinstance(channel, (float,int)):
-                    sigma.append(random.uniform(self.start_of_interval, channel))
-                else:
-                    sigma.append( tuple([random.uniform(self.start_of_interval, channel) for i in range(len(channel))]))
-        return {"sigma": sigma}
-
-class RandomGamma(ImageOnlyTransform):
-    """Performs gamma transform with a randomly selected gamma.
-
-        Gamma is randomly selected from interval given by gamma_limit. If the values in image are not in [0,1] interval
-        then this transformation is skipped.
-
-
-        Args:
-            gamma_limit (Tuple(float), optional): Interval from which gamma is selected. Defaults to (0.8, 1.20).
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, gamma_limit: Tuple[float] = (0.8, 1.20),
-                 always_apply: bool = False, p: float = 0.5):
-        super(RandomGamma, self).__init__(always_apply, p)
-        self.gamma_limit = gamma_limit
-
-    def apply(self, img, gamma=1, **params):
-        return F.gamma_transform(img, gamma=gamma)
-
-    def get_params(self, **data):
-        return {"gamma": random.uniform(self.gamma_limit[0], self.gamma_limit[1])}
-
-    def get_transform_init_args_names(self):
-        return ("gamma_limit", "eps")
-
-    def __repr__(self):
-        return f'RandomGamma({self.gamma_limit}, {self.eps}, {self.always_apply}, {self.p})'
-
-class RandomBrightnessContrast(ImageOnlyTransform):
-    """Randomly change brightness and contrast of the input image.
-
-        Unlike RandomBrightnessContrast from Albumentations, this transform is using
-        formula  :math:`f(a) = (c+1) * a + b`, where c is contrast and b is brightness.
-
-        Args:
-            brightness_limit ((float, float) | float, optional): Interval from which change in brightness is taken.
-                If limit is a single float, the interval will be (-limit, limit). If change in brightness is 0,
-                brightness won`t change. Defaults to 0.2.
-            contrast_limit ((float, float) | float, optional): Interval from which change in contrast is taken.
-                If limit is a single float, the interval will be (-limit, limit). If change in contrast is 0,
-                contrast won`t change. Defaults to 0.2.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, brightness_limit=0.2, contrast_limit=0.2, always_apply=False, p=0.5,):
-        super(RandomBrightnessContrast, self).__init__(always_apply, p)
-        self.brightness_limit = to_tuple(brightness_limit)
-        self.contrast_limit = to_tuple(contrast_limit)
-
-    def apply(self, img, alpha=1.0, beta=0.0, **params):
-        return F.brightness_contrast_adjust(img, alpha, beta)
-
-    def get_params(self, **data):
-        return {
-            "alpha": 1.0 + random.uniform(self.contrast_limit[0], self.contrast_limit[1]),
-            "beta": 0.0 + random.uniform(self.brightness_limit[0], self.brightness_limit[1]),
-        }
-
-    def get_transform_init_args_names(self):
-        return ("brightness_limit", "contrast_limit")
-
-    def __repr__(self):
-        return f'RandomBrightnessContrast({self.brightness_limit}, {self.contrast_limit},  ' \
-               f'{self.always_apply}, {self.p})'
-
-class HistogramEqualization(ImageOnlyTransform):
-    """Performs equalization of histogram.
-
-        This equalization is done channel-wise, meaning that each channel is equalized separately. 
-        Images are normalized over both spatial and temporal domains together. The output is in the range [0,1].
-
-        This transformation is performed with https://scikit-image.org/docs/stable/api/skimage.exposure.html#skimage.exposure.equalize_hist
-
-        Args:
-            bins (int, optional): Number of bins for image histogram. Defaults to 256.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, bins : int = 256, always_apply: bool = False, p: float = 1):
-        super(HistogramEqualization, self).__init__(always_apply, p)
-        self.bins = bins
-
-    def apply(self, img, **params):
-        return F.histogram_equalization(img, self.bins)
-
-class Pad(DualTransform):
-    """Pads the input.
-
-        Input is padded based on pad_size. If pad_size is only one number, all spatial axes are padded on both sides
-        with this number. If it is tuple, then it has same behaviour as pad_size except sides are padded with different 
-        number of pixels. If it is List, then it must have 3 items, which define padding for each spatial dimension
-        separately (in either of the ways described above). If the List is shorter, remaining axes are padded with 0. 
-
-        For other parameters check https://numpy.org/doc/stable/reference/generated/numpy.pad.html    
-
-        Args:
-            pad_size (int | Tuple[int] | List[int | Tuple[int]]): Determines number of pixels to be padded. Tuple should be of size 2. 
-                List should be of size equal to the image axes - 1 (channel axis).  
-            border_mode (str, optional): numpy.pad parameter . Defaults to 'constant'.
-            value (float | Sequence, optional): value for image if needed by chosen border_mode. Defaults to 0.
-            mask_value (float | Sequence, optional): value for mask if needed by chosen border_mode. Defaults to 0.
-            ignore_index ( float | None, optional): If ignore_index is float, then transformation of mask is done with 
-                border_mode = "constant" and mval = ignore_index. If ignore_index is None, then it does nothing. Defaults to None.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 0.5.
-        Targets:
-            image, mask
-        Image types:
-            float32
-    """
-    def __init__(self, pad_size : Union[int, Tuple[int],  List[ Union[int, Tuple[int]]]], border_mode : str = 'constant',
-                ival : Union[float, Sequence] = 0, mval : Union[float, Sequence] = 0,
-                ignore_index : Union[float, None] = None, always_apply : bool = False, p : float = 1):
-        super().__init__(always_apply, p)
-        self.pad_size = pad_size
-        self.border_mode = border_mode
-        self.mask_mode = border_mode 
-        self.ival = ival
-        self.mval = mval
-                   
-
-        if not (ignore_index is None):
-            self.mask_mode = "constant"
-            self.mval = ignore_index
-
-
-    def apply(self, img):
-        return F.pad_pixels(img, self.pad_size, self.border_mode, self.ival)
-
-    def apply_to_mask(self, mask):
-        return F.pad_pixels(mask, self.pad_size, self.mask_mode, self.mval, True)
-
-    def __repr__(self):
-        return f'Pad({self.pad_size}, {self.border_mode}, {self.ival}, {self.mval}, {self.always_apply}, ' \
-               f'{self.p})'
-
-class Normalize(ImageOnlyTransform):
-    """Normalize image channels to the given mean and std.
-
-        Normalization is performed channel-wise. 
-
-        Args:
-            mean (float | List[float], optional): Value of desired mean. If it is list, then it should have
-             same length as number of channels, and each value corresponds to the desired mean in respective channel. Defaults to 0.
-            std (float | List[float], optional): Value of desired std. If it is list, then it should have
-             same length as number of channels, and each value corresponds to the desired std in respective channel. Defaults to 1.
-            always_apply (bool, optional): always apply transformation in composition. Defaults to False.
-            p (float, optional): chance of applying transformation in composition. Defaults to 1.
-        Targets:
-            image
-        Image types:
-            float32
-    """
-    def __init__(self, mean : Union[float,List[float]] = 0, std : Union[float, List[float]] = 1,
-                 always_apply : bool = True, p : float = 1.0):
-        super().__init__(always_apply, p)
-        self.mean = mean
-        self.std = std
-
-
-    def apply(self, img):
-        return F.normalize(img, self.mean, self.std)
-
-    def __repr__(self):
-        return f'Normalize({self.range_norm}, {self.always_apply}, {self.p})'
-
-class Contiguous(DualTransform):
-    def apply(self, image):
-        return np.ascontiguousarray(image)
-
-    def __repr__(self):
-        return f'Contiguous()'
-
-
-
-####################################################################
-####################################################################
-####################################################################
-####################################################################
-####################################################################
-# taken transforms from forks, not implemented #####################
-# shouldnt work, except for Float() ################################
-####################################################################
-####################################################################
-####################################################################
-
-
-
-# not sure what should be end goal for this transformation 
-# but currecntly used as a transform which is always called at the start of Compose
-class Float(DualTransform):
-    def apply(self, image):
-        # TODO this should change value range to (0,1) from the original dtype' value range. Have a look at the code
-        #  below and function F.to_float(), F.from_float()
-
-        # if isinstance(image, np.float32):
-        #     # assume the image already has correct value range (0,1)
-        #     return image
-        #
-        # # change value range to (0,1)
-        # if issubclass(image.dtype.type, numbers.Integral):
-        #     dtype_info = np.iinfo(image.dtype)
-        # else:
-        #     dtype_info = np.finfo(image.dtype)
-        #
-        # if dtype_info.min == 0:
-        #     return image.astype(np.float32) / dtype_info.max
-        #
-        # return ((image.astype(np.float32) / (-dtype_info.min)) / 2) + 0.5
-
-        return image.astype(np.float32)
-
-    def __repr__(self):
-        return f'Float()'
-
-
-
-
-
-class ElasticTransform(DualTransform):
-    def __init__(self, deformation_limits=(0, 0.25), interpolation=1, border_mode='constant', value=0, mask_value=0,
-                 always_apply=False, p=0.5):
-        super().__init__(always_apply, p)
-        self.deformation_limits = deformation_limits
-        self.interpolation = interpolation
-        self.border_mode = border_mode
-        self.value = value
-        self.mask_value = mask_value
-
-    def apply(self, img, sigmas, alphas, random_state=None):
-        return F.elastic_transform(img, sigmas, alphas, interpolation=self.interpolation, random_state=random_state,
-                                   border_mode=self.border_mode, value=self.value)
-
-    def apply_to_mask(self, img, sigmas, alphas, random_state=None):
-        return F.elastic_transform(img, sigmas, alphas, interpolation=0, random_state=random_state,
-                                   border_mode=self.border_mode, value=self.mask_value)
-
-    def get_params(self, **data):
-        image = data["image"]  # [H, W, D]
-        random_state = random.randint(0, 10000)
-        deformation = random.uniform(*self.deformation_limits)
-        sigmas = [deformation * x for x in image.shape[:3]]
-        alphas = [random.uniform(x / 8, x / 2) for x in sigmas]
-        return {
-            "random_state": random_state,
-            "sigmas": sigmas,
-            "alphas": alphas,
-        }
-
-    def __repr__(self):
-        return f'ElasticTransform({self.deformation_limits}, {self.interpolation}, {self.border_mode}, {self.value}, ' \
-               f'{self.mask_value}, {self.always_apply}, {self.p})'
-
-
-# TODO from shape variables to shape arrays
-
-
-
-
-
-#Its here, so it wont show in documentation.
-
-    """GridDropout, drops out rectangular regions of an image and the corresponding mask in a grid fashion.
-        Args:
-        ratio (float): the ratio of the mask holes to the unit_size (same for horizontal and vertical directions).
-            Must be between 0 and 1. Default: 0.5.
-        unit_size_min (int): minimum size of the grid unit. Must be between 2 and the image shorter edge.
-            If 'None', holes_number_x and holes_number_y are used to setup the grid. Default: `None`.
-        unit_size_max (int): maximum size of the grid unit. Must be between 2 and the image shorter edge.
-            If 'None', holes_number_x and holes_number_y are used to setup the grid. Default: `None`.
-        holes_number_x (int): the number of grid units in x direction. Must be between 1 and image width//2.
-            If 'None', grid unit width is set as image_width//10. Default: `None`.
-        holes_number_y (int): the number of grid units in y direction. Must be between 1 and image height//2.
-            If `None`, grid unit height is set equal to the grid unit width or image height, whatever is smaller.
-        holes_number_z (int): the number of grid units in z direction. Must be between 1 and image depth//2.
-            If `None`, grid unit depth is set equal to the grid unit width or image height, whatever is smaller.
-        shift_x (int): offsets of the grid start in x direction from (0,0) coordinate.
-            Clipped between 0 and grid unit_width - hole_width. Default: 0.
-        shift_y (int): offsets of the grid start in y direction from (0,0) coordinate.
-            Clipped between 0 and grid unit height - hole_height. Default: 0.
-        shift_z (int): offsets of the grid start in z direction from (0,0) coordinate.
-            Clipped between 0 and grid unit depth - hole_depth. Default: 0.
-        random_offset (boolean): weather to offset the grid randomly between 0 and grid unit size - hole size
-            If 'True', entered shift_x, shift_y, shift_z are ignored and set randomly. Default: `False`.
-        fill_value (int): value for the dropped pixels. Default = 0
-        mask_fill_value (int): value for the dropped pixels in mask.
-            If `None`, tranformation is not applied to the mask. Default: `None`.
-    Targets:
-        image, mask
-    Image types:
-        uint8, float32
-    References:
-        https://arxiv.org/abs/2001.04086
-    """
-
-class GridDropout(DualTransform):
-
-    def __init__(
-            self,
-            ratio: float = 0.5,
-            unit_size_min: int = None,
-            unit_size_max: int = None,
-            holes_number_x: int = None,
-            holes_number_y: int = None,
-            holes_number_z: int = None,
-            shift_x: int = 0,
-            shift_y: int = 0,
-            shift_z: int = 0,
-            random_offset: bool = False,
-            fill_value: int = 0,
-            mask_fill_value: int = None,
-            always_apply: bool = False,
-            p: float = 0.5,
-    ):
-        super(GridDropout, self).__init__(always_apply, p)
-        self.ratio = ratio
-        self.unit_size_min = unit_size_min
-        self.unit_size_max = unit_size_max
-        self.holes_number_x = holes_number_x
-        self.holes_number_y = holes_number_y
-        self.holes_number_z = holes_number_z
-        self.shift_x = shift_x
-        self.shift_y = shift_y
-        self.shift_z = shift_z
-        self.random_offset = random_offset
-        self.fill_value = fill_value
-        self.mask_fill_value = mask_fill_value
-        if not 0 < self.ratio <= 1:
-            raise ValueError("ratio must be between 0 and 1.")
-
-    def apply(self, image, holes=(), **params):
-        return F.cutout(image, holes, self.fill_value)
-
-    def apply_to_mask(self, image, holes=(), **params):
-        if self.mask_fill_value is None:
-            return image
-
-        return F.cutout(image, holes, self.mask_fill_value)
-
-    def get_params(self, **data):
-        img = data["image"]
-        height, width, depth = img.shape[:3]
-        # set grid using unit size limits
-        if self.unit_size_min and self.unit_size_max:
-            if not 2 <= self.unit_size_min <= self.unit_size_max:
-                raise ValueError(
-                    "Max unit size should be >= min size, both at least 2 pixels.")
-            if self.unit_size_max > min(height, width):
-                raise ValueError(
-                    "Grid size limits must be within the shortest image edge.")
-            unit_width = random.randint(
-                self.unit_size_min, self.unit_size_max + 1)
-            unit_height = unit_width
-            unit_depth = unit_width
-        else:
-            # set grid using holes numbers
-            if self.holes_number_x is None:
-                unit_width = max(2, width // 10)
-            else:
-                if not 1 <= self.holes_number_x <= width // 2:
-                    raise ValueError(f"The hole_number_x must be between 1 and image width//2 ({width//2}), "
-                                     f"but was {self.holes_number_x}.")
-                unit_width = width // self.holes_number_x
-            if self.holes_number_y is None:
-                unit_height = max(min(unit_width, height), 2)
-            else:
-                if not 1 <= self.holes_number_y <= height // 2:
-                    raise ValueError(f"The hole_number_y must be between 1 and image height//2 ({height//2}), "
-                                     f"but was {self.holes_number_y}.")
-                unit_height = height // self.holes_number_y
-            if self.holes_number_z is None:
-                unit_depth = max(min(unit_height, depth), 2)
-            else:
-                if not 1 <= self.holes_number_z <= depth // 2:
-                    raise ValueError(f"The hole_number_z must be between 1 and image depth//2 ({depth//2}), "
-                                     f"but was {self.holes_number_z}.")
-                unit_depth = depth // self.holes_number_z
-
-        hole_width = int(unit_width * self.ratio)
-        hole_height = int(unit_height * self.ratio)
-        hole_depth = int(unit_depth * self.ratio)
-        # min 1 pixel and max unit length - 1
-        hole_width = min(max(hole_width, 1), unit_width - 1)
-        hole_height = min(max(hole_height, 1), unit_height - 1)
-        hole_depth = min(max(hole_depth, 1), unit_depth - 1)
-        # set offset of the grid
-        if self.shift_x is None:
-            shift_x = 0
-        else:
-            shift_x = min(max(0, self.shift_x), unit_width - hole_width)
-        if self.shift_y is None:
-            shift_y = 0
-        else:
-            shift_y = min(max(0, self.shift_y), unit_height - hole_height)
-        if self.shift_z is None:
-            shift_z = 0
-        else:
-            shift_z = min(max(0, self.shift_z), unit_depth - hole_depth)
-        if self.random_offset:
-            shift_x = random.randint(0, unit_width - hole_width)
-            shift_y = random.randint(0, unit_height - hole_height)
-            shift_z = random.randint(0, unit_depth - hole_depth)
-        holes = []
-        for i in range(width // unit_width + 1):
-            for j in range(height // unit_height + 1):
-                for k in range(depth // unit_depth + 1):
-                    x1 = min(shift_x + unit_width * i, width)
-                    y1 = min(shift_y + unit_height * j, height)
-                    z1 = min(shift_z + unit_depth * j, depth)
-                    x2 = min(x1 + hole_width, width)
-                    y2 = min(y1 + hole_height, height)
-                    z2 = min(z1 + hole_depth, depth)
-                    holes.append((x1, y1, z1, x2, y2, z2))
-
-        return {"holes": holes}
-
-    def get_transform_init_args_names(self):
-        return (
-            "ratio",
-            "unit_size_min",
-            "unit_size_max",
-            "holes_number_x",
-            "holes_number_y",
-            "shift_x",
-            "shift_y",
-            "mask_fill_value",
-            "random_offset",
-        )
-
-    def __repr__(self):
-        return f'GridDropout({self.ratio}, {self.unit_size_min}, {self.unit_size_max}, {self.holes_number_x}, ' \
-               f'{self.holes_number_y}, {self.holes_number_z}, {self.shift_x}, {self.shift_y}, {self.shift_z}, ' \
-               f'{self.random_offset}, {self.fill_value}, {self.mask_fill_value}, {self.always_apply}, {self.p})'
-
-
-class RandomDropPlane(DualTransform):
-    """Randomly drop some planes in axis randomly chosen from 'axes' input array.
-
-    Args:
-        plane_drop_prob (float): float value in (0.0, 1.0) range. Default: 0.1
-        axes (tuple). Default: 0
-        p (float): probability of applying the transform. Default: 1.
-
-    Targets:
-        image, mask
-
-    Image types:
-        uint8, float32
-    """
-
-    def __init__(
-            self,
-            plane_drop_prob=0.1,
-            axes=(0,),
-            always_apply=False,
-            p=1.0
-    ):
-        super(RandomDropPlane, self).__init__(always_apply, p)
-        self.plane_drop_prob = plane_drop_prob
-        self.axes = axes
-
-    def get_params(self, **data):
-        img = data["image"]
-        # TODO add choosing axis randomly from all spatial axes like in flip if axes is initially None
-        axis = random.choice(self.axes)
-        r = img.shape[axis]
-        indexes = []
-        for i in range(r):
-            if random.uniform(0, 1) > self.plane_drop_prob:
-                indexes.append(i)
-        if len(indexes) == 0:
-            indexes.append(0)
-
-        return {
-            "indexes": indexes, "axis": axis,
-        }
-
-    def apply(self, img, indexes=(), axis=0, **params):
-        return np.take(img, indexes, axis=axis)
-
-    def apply_to_mask(self, mask, indexes=(), axis=0, **params):
-        return np.take(mask, indexes, axis=axis)
-
-    def __repr__(self):
-        return f'RandomDropPlane({self.plane_drop_prob}, {self.axes}, {self.always_apply}, {self.p})'
-
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+import random
+import numpy as np
+from ..core.transforms_interface import DualTransform, ImageOnlyTransform
+from ..augmentations import functional as F
+from ..random_utils import uniform, sample_range_uniform
+from typing import List, Sequence, Tuple, Union
+from ..typing import TypeSextetFloat, TypeTripletFloat, TypePairFloat
+from .utils import parse_limits, parse_coefs, to_tuple
+
+
+# TODO potential upgrade : different sigmas for different channels
+class GaussianNoise(ImageOnlyTransform):
+    """Adds Gaussian noise to the image. The noise is drawn from normal distribution with given parameters.
+
+        Args:
+            var_limit (tuple, optional): Variance of normal distribution is randomly chosen from this interval.
+
+                Defaults to ``(0.001, 0.1)``.
+            mean (float, optional): Mean of normal distribution.
+
+                Defaults to ``0``.
+            always_apply (bool, optional): Always apply this transformation in composition.
+
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition.
+
+                Defaults to ``0.5``.
+
+        Targets:
+            image
+    """
+    def __init__(self, var_limit: tuple = (0.001, 0.1), mean: float = 0,
+                 always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.var_limit = var_limit
+        self.mean = mean
+
+    def apply(self, img, **params):
+        return F.gaussian_noise(img, sigma=params['sigma'], mean=self.mean)
+
+    def get_params(self, **params):
+        var = uniform(self.var_limit[0], self.var_limit[1])
+        sigma = var ** 0.5
+        return {"sigma": sigma}
+
+    def __repr__(self):
+        return f'GaussianNoise({self.var_limit}, {self.mean}, {self.always_apply}, {self.p})'
+
+
+class PoissonNoise(ImageOnlyTransform):
+    """Adds Poisson noise to the image.
+
+        Args:
+            intensity_limit (tuple): Range to sample the expected intensity of Poisson noise.
+
+                Defaults to ``(1, 10)``.
+            always_apply (bool, optional): Always apply this transformation in composition.
+
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition.
+
+                Defaults to ``0.5``.
+
+        Targets:
+            image
+    """
+    def __init__(self,
+                 intensity_limit=(1, 10),
+                 always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.intensity_limit = intensity_limit
+
+    def apply(self, img, **params):
+        return F.poisson_noise(img, intensity=params['intensity'])
+
+    def get_params(self, **params):
+        intensity = uniform(self.intensity_limit[0], self.intensity_limit[1])
+        return {"intensity": intensity}
+
+    def __repr__(self):
+        return f'PoissonNoise({self.always_apply}, {self.p})'
+
+
+# TODO anti_aliasing_downsample keep parameter or remove?
+class Resize(DualTransform):
+    """Resize input to the given shape.
+
+        Internally, the ``skimage.transform.resize`` function is used.
+        The ``interpolation``, ``border_mode``, ``ival``, ``mval``,
+        and ``anti_aliasing_downsample`` arguments are forwarded to it. More details at:
+        https://scikit-image.org/docs/stable/api/skimage.transform.html#skimage.transform.resize.
+
+        Args:
+            shape (tuple of ints): The desired image shape.
+
+                Must be of either of: ``(Z, Y, X)`` or ``(Z, Y, X, T)``.
+
+                The unspecified dimensions (C and possibly T) are not affected.
+            interpolation (int, optional): Order of spline interpolation.
+
+                Defaults to ``1``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'reflect'``.
+            ival (float, optional): Value of `image` voxels outside of the `image` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            mval (float, optional): Value of `mask` voxels outside of the `mask` domain. Only applied when ``border_mode = 'constant'``.
+            
+                Defaults to ``0``.
+            anti_aliasing_downsample (bool, optional): Controls if the Gaussian filter should be applied before
+                downsampling. Recommended. 
+                
+                Defaults to ``True``.
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+                
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, shape: tuple, interpolation: int = 1, border_mode: str = 'reflect', ival: float = 0,
+                 mval: float = 0, anti_aliasing_downsample: bool = True, ignore_index: Union[float, None] = None,
+                 always_apply: bool = False, p: float = 1):
+        
+        super().__init__(always_apply, p)
+        self.shape = shape
+        self.interpolation = interpolation
+        self.border_mode = border_mode
+        self.mask_mode = border_mode
+        self.ival = ival
+        self.mval = mval
+        self.anti_aliasing_downsample = anti_aliasing_downsample
+        if not (ignore_index is None):
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def apply(self, img, **params):
+        return F.resize(img, input_new_shape=self.shape, interpolation=self.interpolation,
+                        border_mode=self.border_mode, cval=self.ival,
+                        anti_aliasing_downsample=self.anti_aliasing_downsample)
+
+    def apply_to_mask(self, mask, **params):
+        return F.resize(mask, input_new_shape=self.shape, interpolation=0,
+                        border_mode=self.mask_mode, cval=self.mval, anti_aliasing_downsample=False,
+                        mask=True)
+
+    def apply_to_float_mask(self, mask, **params):
+        return F.resize(mask, input_new_shape=self.shape, interpolation=self.interpolation,
+                        border_mode=self.mask_mode, cval=self.mval, anti_aliasing_downsample=False,
+                        mask=True)
+        
+    def __repr__(self):
+        return f'Resize({self.shape}, {self.interpolation}, {self.border_mode} , {self.ival}, {self.mval},' \
+               f'{self.anti_aliasing_downsample},   {self.always_apply}, {self.p})'
+
+
+class Scale(DualTransform):
+    """Rescale input by the given scale.
+
+        Args:
+            scales (float|List[float], optional): Value by which the input should be scaled.
+
+                Must be either of: ``S``, ``[S_Z, S_Y, S_X]``, or ``[S_Z, S_Y, S_X, S_T]``.
+
+                If a float, then all spatial dimensions are scaled by it (equivalent to ``[S, S, S]``).
+
+                The unspecified dimensions (C and possibly T) are not affected.
+
+                Defaults to ``1``.
+            interpolation (int, optional): Order of spline interpolation.
+
+                Defaults to ``1``.
+            spacing (float | Tuple[float, float, float] | None, optional): Voxel spacing for individual spatial dimensions.
+
+                Must be either of: ``S``, ``(S1, S2, S3)``, or ``None``.
+
+                If ``None``, equivalent to ``(1, 1, 1)``.
+
+                If a float ``S``, equivalent to ``(S, S, S)``.
+
+                Otherwise, a scale for each spatial dimension must be given.
+
+                Defaults to ``None``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'constant'``.
+            ival (float, optional): Value of `image` voxels outside of the `image` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            mval (float, optional): Value of `mask` voxels outside of the `mask` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, scales: Union[float, TypeTripletFloat] = 1,
+                 interpolation: int = 1, spacing: Union[float, TypeTripletFloat] = None,
+                 border_mode: str = 'constant', ival: float = 0, mval: float = 0,
+                 ignore_index: Union[float, None] = None, always_apply: bool = False, p: float = 1):
+        super().__init__(always_apply, p)
+        self.scale = parse_coefs(scales, identity_element=1.)
+        self.interpolation: int = interpolation
+        self.spacing: TypeTripletFloat = parse_coefs(spacing, identity_element=1.)
+        self.border_mode = border_mode              # not implemented
+        self.mask_mode = border_mode                # not implemented
+        self.ival = ival
+        self.mval = mval
+        if not (ignore_index is None):
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def apply(self, img, **params):
+        return F.affine(img,
+                        scales=self.scale,
+                        interpolation=self.interpolation,
+                        border_mode=self.border_mode,
+                        value=self.ival,
+                        spacing=self.spacing)
+
+    def apply_to_mask(self, mask, **params):
+        interpolation = 0   # refers to 'sitkNearestNeighbor'
+        return F.affine(mask,
+                        scales=self.scale,
+                        interpolation=interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+    def apply_to_float_mask(self, mask, **params):
+        return F.affine(mask,
+                        scales=self.scale,
+                        interpolation=self.interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+    def __repr__(self):
+        return f'Scale({self.scale}, {self.interpolation}, {self.border_mode}, {self.ival}, {self.mval},' \
+               f'{self.always_apply}, {self.p})'
+
+
+# TODO cannot rescale T dimension
+class RandomScale(DualTransform):
+    """Randomly rescale input.
+
+        Args:
+            scaling_limit (float | Tuple[float] | List[Tuple[float]], optional): Limits of scaling factors.
+
+                Must be either of: ``S``, ``(S1, S2)``, ``(S_Z, S_Y, S_X)``, or ``(S_Z1, S_Z2, S_Y1, S_Y2, S_X1, S_X2)``.
+
+                If a float ``S``, then all spatial dimensions are scaled by a random number drawn uniformly from
+                the interval [1-S, 1+S] (equivalent to inputting ``(1-S, 1+S, 1-S, 1+S, 1-S, 1+S)``).
+
+                If a tuple of 2 floats, then all spatial dimensions are scaled by a random number drawn uniformly
+                from the interval [S1, S2] (equivalent to inputting ``(S1, S2, S1, S2, S1, S2)``).
+
+                If a tuple of 3 floats, then an interval [1-S_a, 1+S_a] is constructed for each spatial
+                dimension and the scale is randomly drawn from it
+                (equivalent to inputting ``(1-S_Z, 1+S_Z, 1-S_Y, 1+S_Y, 1-S_X, 1+S_X)``).
+
+                If a tuple of 6 floats, the scales for individual spatial dimensions are randomly drawn from the
+                respective intervals [S_Z1, S_Z2], [S_Y1, S_Y2], [S_X1, S_X2].
+
+                The unspecified dimensions (C and T) are not affected.
+
+                Defaults to ``(0.9, 1.1)``.
+
+            interpolation (int, optional): Order of spline interpolation.
+
+                Defaults to ``1``.
+
+            spacing (float | Tuple[float, float, float] | None, optional): Voxel spacing for individual spatial dimensions.
+
+                Must be either of: ``S``, ``(S1, S2, S3)``, or ``None``.
+
+                If ``None``, equivalent to ``(1, 1, 1)``.
+
+                If a float ``S``, equivalent to ``(S, S, S)``.
+
+                Otherwise, a scale for each spatial dimension must be given.
+
+                Defaults to ``None``.
+
+            border_mode (str, optional): Values outside image domain are filled according to the mode.
+
+                Defaults to ``'constant'``.
+
+            ival (float, optional): Value of `image` voxels outside of the `image` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+
+            mval (float, optional): Value of `mask` voxels outside of the `mask` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+
+                Defaults to ``None``.
+
+            always_apply (bool, optional): Always apply this transformation in composition.
+
+                Defaults to ``False``.
+
+            p (float, optional): Chance of applying this transformation in composition.
+
+                Defaults to ``0.5``.
+
+        Targets:
+            image, mask, float_mask
+    """      
+    def __init__(self, scaling_limit: Union[float, TypePairFloat, TypeTripletFloat, TypeSextetFloat] = (0.9, 1.1),
+                 interpolation: int = 1, spacing: Union[float, TypeTripletFloat] = None,
+                 border_mode: str = 'constant', ival: float = 0, mval: float = 0,
+                 ignore_index: Union[float, None] = None, always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.scaling_limit: TypeSextetFloat = parse_limits(scaling_limit)
+        self.interpolation: int = interpolation
+        self.spacing: TypeTripletFloat = parse_coefs(spacing, identity_element=1.)
+        self.border_mode = border_mode
+        self.mask_mode = border_mode
+        self.ival: float = ival
+        self.mval: float = mval
+        if not (ignore_index is None):
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def get_params(self, **data):
+        # set parameters of the transform
+        scale = sample_range_uniform(self.scaling_limit)
+
+        return {
+            "scale": scale,
+        }
+
+    def apply(self, img, **params):
+        return F.affine(img,
+                        scales=params["scale"],
+                        interpolation=self.interpolation,
+                        border_mode=self.border_mode,
+                        value=self.ival,
+                        spacing=self.spacing)
+
+    def apply_to_mask(self, mask, **params):
+        interpolation = 0   # refers to 'sitkNearestNeighbor'
+        return F.affine(mask,
+                        scales=params["scale"],
+                        interpolation=interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+    def apply_to_float_mask(self, mask, **params):
+        return F.affine(mask,
+                        scales=params["scale"],
+                        interpolation=self.interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+    def __repr__(self):
+        return f'RandomScale({self.scaling_limit}, {self.interpolation}, {self.always_apply}, {self.p})'
+
+
+class RandomRotate90(DualTransform):
+    """Rotation of input by 0, 90, 180, or 270 degrees around the specified spatial axes.
+
+        Args:
+            axes (List[int], optional): List of axes around which the input is rotated. Recognised axis symbols are
+                ``1`` for Z, ``2`` for Y, and ``3`` for X. A single axis can occur multiple times in the list.
+                If ``shuffle_axis = False``, the order of axes determines the order of transformations.
+
+                Defaults to ``[1, 2, 3]``.
+            shuffle_axis (bool, optional): If set to ``True``, the order of rotations is random.
+
+                Defaults to ``False``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, axes: List[int] = None, shuffle_axis: bool = False,
+                 always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.axes = axes
+        self.shuffle_axis = shuffle_axis
+
+    def apply(self, img, **params):
+        for factor, axes in zip(params["factor"], params["rotation_around"]):
+            img = np.rot90(img, factor, axes=axes)
+        return img
+
+    def apply_to_mask(self, mask, **params):
+        for i in range(len(params["rotation_around"])):
+            mask = np.rot90(mask, params["factor"][i], axes=(
+                params["rotation_around"][i][0] - 1, params["rotation_around"][i][1] - 1))
+        return mask
+
+    def get_params(self, **data):
+
+        # Rotate by all axis by default
+        if self.axes is None:
+            self.axes = [1, 2, 3]
+
+        # Create all combinations for rotating
+        axes_to_rotate = {1: (2, 3), 2: (1, 3), 3: (1, 2)}
+        rotation_around = []
+        for i in self.axes:
+            if i in axes_to_rotate.keys():
+                rotation_around.append(axes_to_rotate[i])
+
+        # shuffle order of axis
+        if self.shuffle_axis:
+            random.shuffle(rotation_around)
+
+        # choose angle to rotate
+        factor = [random.randint(0, 3) for _ in range(len(rotation_around))]
+        return {"factor": factor,
+                "rotation_around": rotation_around}
+
+    def __repr__(self):
+        return f'RandomRotate90({self.axes}, {self.always_apply}, {self.p})'
+
+
+class Flip(DualTransform):
+    """Flip input around the specified spatial axes.
+
+        Args:
+            axes (List[int], optional): List of axes around which is flip done. Recognised axis symbols are
+                ``1`` for Z, ``2`` for Y, and ``3`` for X.
+
+                Defaults to ``[1,2,3]``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, axes: List[int] = None, always_apply=False, p=1):
+        super().__init__(always_apply, p)
+        self.axes = axes
+
+    def apply(self, img, **params):
+        return np.flip(img, params["axes"])
+
+    def apply_to_mask(self, mask, **params):
+        # Mask has no dimension channel
+        return np.flip(mask, axis=[item - 1 for item in params["axes"]])
+
+    def get_params(self, **data):
+        if self.axes is None:
+            axes = [1, 2, 3]
+        else:
+            axes = self.axes
+        return {"axes": axes}
+
+    def __repr__(self):
+        return f'Flip({self.axes}, {self.always_apply}, {self.p})'
+
+
+# TODO include possibility to pick empty combination = no flipping
+class RandomFlip(DualTransform):
+    """Flip input around a set of axes randomly chosen from the input list of axis combinations.
+
+        Args:
+            axes_to_choose (List[Tuple[int]] or None, optional): List of axis combinations from which one option
+                is randomly chosen. Recognised axis symbols are ``1`` for Z, ``2`` for Y, and ``3`` for X.
+                The image will be flipped around all axes in the chosen combination.
+
+                If ``None``, a random subset of spatial axes is chosen, corresponding to inputting
+                ``[(1,), (2,), (3,), (1, 2), (1, 3), (2, 3), (1, 2, 3)]``.
+
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, axes_to_choose: Union[None, List[Tuple[int]]] = None, always_apply=False, p=0.5):
+        super().__init__(always_apply, p)
+        self.axes = axes_to_choose
+
+    def apply(self, img, **params):
+        return np.flip(img, params["axes"])
+
+    def apply_to_mask(self, mask, **params):
+        # Mask has no dimension channel
+        return np.flip(mask, axis=[item - 1 for item in params["axes"]])
+
+    def get_params(self, **data):
+        
+        if self.axes is None or len(self.axes) == 0:
+            # Pick random combination of axes to flip
+            # TODO include possibility to pick empty combination = no flipping
+            combinations = [(1,), (2,), (3,), (1, 2),
+                            (1, 3), (2, 3), (1, 2, 3)]
+            axes = random.choice(combinations)
+        else:
+            # Pick a random choice from input
+            axes = random.choice(self.axes)
+        return {"axes": axes}
+
+    def __repr__(self):
+        return f'Flip({self.axes}, {self.always_apply}, {self.p})'
+
+
+class CenterCrop(DualTransform):
+    """Crops the central region of the input of given size.
+          
+        Unlike ``CenterCrop`` from `Albumentations`, this transform pads the input in dimensions
+        where the input is smaller than the ``shape`` with ``numpy.pad``. The ``border_mode``, ``ival`` and ``mval``
+        arguments are forwarded to ``numpy.pad`` if padding is necessary. More details at:
+        https://numpy.org/doc/stable/reference/generated/numpy.pad.html.
+
+        Args:
+            shape (Tuple[int]): The desired shape of input.
+
+                Must be either of: ``[Z, Y, X]`` or ``[Z, Y, X, T]``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'reflect'``.
+            ival (float | Sequence, optional): Values of `image` voxels outside of the `image` domain.
+                Only applied when ``border_mode = 'constant'`` or ``border_mode = 'linear_ramp'``.
+
+                Defaults to ``(0, 0)``.
+            mval (float | Sequence, optional): Values of `mask` voxels outside of the `mask` domain.
+                Only applied when ``border_mode = 'constant'`` or ``border_mode = 'linear_ramp'``.
+
+                Defaults to ``(0, 0)``.
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, shape: Tuple[int], border_mode: str = "reflect", ival: Union[Sequence[float], float] = (0, 0),
+                 mval: Union[Sequence[float], float] = (0, 0), ignore_index: Union[float, None] = None,
+                 always_apply: bool = False, p: float = 1.0):
+        super().__init__(always_apply, p)
+        self.shape = np.asarray(shape, dtype=np.intc)
+        self.border_mode = border_mode
+        self.mask_mode = border_mode
+        self.ival = ival
+        self.mval = mval
+        
+        if not (ignore_index is None):
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def apply(self, img, **params):
+        return F.center_crop(img, self.shape, self.border_mode, self.ival, False)
+
+    def apply_to_mask(self, mask, **params):
+        return F.center_crop(mask, self.shape, self.mask_mode, self.mval, True)
+
+    def __repr__(self):
+        return f'CenterCrop({self.shape}, {self.always_apply}, {self.p})'
+
+
+class RandomCrop(DualTransform):
+    """Randomly crops a region of given size from the input.
+
+        Unlike ``RandomCrop`` from `Albumentations`, this transform pads the input in dimensions
+        where the input is smaller than the ``shape`` with ``numpy.pad``. The ``border_mode``, ``ival`` and ``mval``
+        arguments are forwarded to ``numpy.pad`` if padding is necessary. More details at:
+        https://numpy.org/doc/stable/reference/generated/numpy.pad.html.
+
+        Args:
+            shape (Tuple[int]): The desired shape of input.
+
+                Must be either of: ``[Z, Y, X]`` or ``[Z, Y, X, T]``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'reflect'``.
+            ival (float | Sequence, optional): Values of `image` voxels outside of the `image` domain.
+                Only applied when ``border_mode = 'constant'`` or ``border_mode = 'linear_ramp'``.
+
+                Defaults to ``(0, 0)``.
+            mval (float | Sequence, optional): Values of `mask` voxels outside of the `mask` domain.
+                Only applied when ``border_mode = 'constant'`` or ``border_mode = 'linear_ramp'``.
+
+                Defaults to ``(0, 0)``.
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, shape: tuple, border_mode: str = "reflect", ival: Union[Sequence[float], float] = (0, 0),
+                 mval: Union[Sequence[float], float] = (0, 0), ignore_index: Union[float, None] = None,
+                 always_apply: bool = False, p: float = 1.0):
+        super().__init__(always_apply, p)
+        self.shape = np.asarray(shape, dtype=np.intc)
+        self.border_mode = border_mode
+        self.mask_mode = border_mode
+        self.ival = ival
+        self.mval = mval
+
+        if not (ignore_index is None):
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def apply(self, img, crop_start=np.array((0, 0, 0))):
+        return F.random_crop(img, self.shape, crop_start, self.border_mode, self.ival, mask=False)
+
+    def apply_to_mask(self, mask, crop_start=np.array((0, 0, 0))):
+        return F.random_crop(mask, self.shape, crop_start, self.mask_mode, self.mval, mask=True)
+
+    def get_params(self, **data):
+
+        return {
+            "crop_start": [random.random() for _ in range(len(self.shape))]
+        }
+
+    def __repr__(self):
+        return f'RandomCrop({self.shape}, {self.always_apply}, {self.p})'
+
+
+class RandomAffineTransform(DualTransform):
+    """Affine transformation of the input image with randomly chosen parameters.
+
+        Args:
+            angle_limit (Tuple[float] | float, optional): Intervals in degrees from which angles of
+                rotation for the spatial axes are chosen.
+
+                Must be either of: ``A``, ``(A1, A2)``, or ``(A_Z1, A_Z2, A_Y1, A_Y2, A_X1, A_X2)``.
+
+                If a float, equivalent to ``(-A, A, -A, A, -A, A)``.
+
+                If a tuple with 2 items, equivalent to ``(A1, A2, A1, A2, A1, A2)``.
+
+                If a tuple with 6 items, angle of rotation is randomly chosen from an interval [A_a1, A_a2] for each
+                spatial axis.
+
+                Defaults to ``(15, 15, 15)``.
+            translation_limit (Tuple[int] | int | None, optional): Intervals from which the translation parameters
+                for the spatial axes are chosen.
+
+                Must be either of: ``T``, ``(T1, T2)``, or ``(T_Z1, T_Z2, T_Y1, T_Y2, T_X1, T_X2)``.
+
+                If a float, equivalent to ``(-T, T, -T, T, -T, T)``.
+
+                If a tuple with 2 items, equivalent to ``(T1, T2, T1, T2, T1, T2)``.
+
+                If a tuple with 6 items, the translation parameter is randomly chosen from an interval [T_a1, T_a2] for
+                each spatial axis.
+
+                Defaults to ``(0, 0, 0)``.
+            scaling_limit (Tuple[float] | float, optional): Intervals from which the scales for the spatial axes are chosen.
+
+                Must be either of: ``S``, ``(S1, S2)``, or ``(S_Z1, S_Z2, S_Y1, S_Y2, S_X1, S_X2)``.
+
+                If a float, equivalent to ``(1-S, 1+S, 1-S, 1+S, 1-S, 1+S)``.
+
+                If a tuple with 2 items, equivalent to ``(S1, S2, S1, S2, S1, S2)``.
+
+                If a tuple with 6 items, the scale is randomly chosen from an interval [S_a1, S_a2] for
+                each spatial axis.
+
+                Defaults to ``(0.2, 0.2, 0.2)``.
+            spacing (float | Tuple[float, float, float] | None, optional): Voxel spacing for individual spatial dimensions.
+
+                Must be either of: ``S``, ``(S1, S2, S3)``, or ``None``.
+
+                If ``None``, equivalent to ``(1, 1, 1)``.
+
+                If a float ``S``, equivalent to ``(S, S, S)``.
+
+                Otherwise, a scale for each spatial dimension must be given.
+
+                Defaults to ``None``.
+            change_to_isotropic (bool, optional): Change data from anisotropic to isotropic.
+
+                Defaults to ``False``.
+            interpolation (int, optional): Order of spline interpolation.
+
+                Defaults to ``1``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'constant'``.
+            ival (float, optional): Value of `image` voxels outside of the `image` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            mval (float, optional): Value of `mask` voxels outside of the `mask` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, angle_limit: Union[float, TypePairFloat, TypeSextetFloat] = (15, 15, 15),
+                 translation_limit: Union[float, TypePairFloat, TypeSextetFloat] = (0, 0, 0),
+                 scaling_limit: Union[float, TypePairFloat, TypeSextetFloat] = (0.2, 0.2, 0.2),
+                 spacing: Union[float, TypeTripletFloat] = None,
+                 change_to_isotropic: bool = False,
+                 interpolation: int = 1,
+                 border_mode: str = 'constant', ival: float = 0, mval: float = 0,
+                 ignore_index: Union[float, None] = None, always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.angle_limit: TypeSextetFloat = parse_limits(angle_limit, identity_element=0)
+        self.translation_limit: TypeSextetFloat = parse_limits(translation_limit, identity_element=0)
+        self.scaling_limit: TypeSextetFloat = parse_limits(scaling_limit, identity_element=1)
+        self.spacing: TypeTripletFloat = parse_coefs(spacing, identity_element=1)
+        self.interpolation: int = interpolation
+        self.border_mode = border_mode                 # not used
+        self.mask_mode = border_mode                   # not used
+        self.ival = ival
+        self.mval = mval
+        self.keep_scale = not change_to_isotropic
+
+        if ignore_index is not None:
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def apply(self, img, **params):
+        return F.affine(img,
+                        scales=params["scale"],
+                        degrees=params["angles"],
+                        translation=params["translation"],
+                        interpolation=self.interpolation,
+                        border_mode=self.border_mode,
+                        value=self.ival,
+                        spacing=self.spacing)
+
+    def apply_to_mask(self, mask, **params):
+        interpolation = 0   # refers to 'sitkNearestNeighbor'
+        return F.affine(mask,
+                        scales=params["scale"],
+                        degrees=params["angles"],
+                        translation=params["translation"],
+                        interpolation=interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+    def apply_to_float_mask(self, mask, **params):
+        return F.affine(mask,
+                        scales=params["scale"],
+                        degrees=params["angles"],
+                        translation=params["translation"],
+                        interpolation=self.interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+    def get_params(self, **data):
+
+        # set parameters of the transform
+        scales = sample_range_uniform(self.scaling_limit)
+        angles = sample_range_uniform(self.angle_limit)
+        translation = sample_range_uniform(self.translation_limit)
+
+        return {
+            "scale": scales,
+            "angles": angles,
+            "translation": translation
+        }
+
+
+class AffineTransform(DualTransform):
+    """Affine transformation of the input image with given parameters.
+
+        Args:
+            angles (Tuple[float], optional): Angles of rotation for the spatial axes.
+
+                Must be: ``(A_Z, A_Y, A_X)``.
+
+                Defaults to ``(0, 0, 0)``.
+            translation (Tuple[float], optional): Translation vector for the spatial axes.
+
+                Must be: ``(T_Z, T_Y, T_X)``.
+
+                Defaults to ``(0, 0, 0)``.
+            scale (Tuple[float], optional): Scales for the spatial axes.
+
+                Must be: ``(S_Z, S_Y, S_X)``.
+
+                Defaults to ``(1, 1, 1)``.
+            spacing (Tuple[float, float, float], optional): Voxel spacing for individual spatial dimensions.
+
+                Must be: ``(S1, S2, S3)`` (a scale for each spatial dimension must be given).
+
+                Defaults to ``(1, 1, 1)``.
+            change_to_isotropic (bool, optional): Change data from anisotropic to isotropic.
+
+                Defaults to ``False``.
+            interpolation (int, optional): Order of spline interpolation.
+
+                Defaults to ``1``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'constant'``.
+            ival (float, optional): Value of `image` voxels outside of the `image` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            mval (float, optional): Value of `mask` voxels outside of the `mask` domain. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, angles: TypeTripletFloat = (0, 0, 0),
+                 translation: TypeTripletFloat = (0, 0, 0),
+                 scale: TypeTripletFloat = (1, 1, 1),
+                 spacing: TypeTripletFloat = (1, 1, 1),
+                 change_to_isotropic: bool = False,
+                 interpolation: int = 1,
+                 border_mode: str = 'constant', ival: float = 0, mval: float = 0,
+                 ignore_index: Union[float, None] = None, always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.angles: TypeTripletFloat = parse_coefs(angles, identity_element=0)
+        self.translation: TypeTripletFloat = parse_coefs(translation, identity_element=0)
+        self.scale: TypeTripletFloat = parse_coefs(scale, identity_element=1)
+        self.spacing: TypeTripletFloat = parse_coefs(spacing, identity_element=1)
+        self.interpolation: int = interpolation
+        self.border_mode = border_mode                 # not used
+        self.mask_mode = border_mode                   # not used
+        self.ival = ival
+        self.mval = mval
+        self.keep_scale = not change_to_isotropic
+
+        if ignore_index is not None:
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def apply(self, img, **params):
+        return F.affine(img,
+                        scales=self.scale,
+                        degrees=self.angles,
+                        translation=self.translation,
+                        interpolation=self.interpolation,
+                        border_mode=self.border_mode,
+                        value=self.ival,
+                        spacing=self.spacing)
+
+    def apply_to_mask(self, mask, **params):
+        interpolation = 0   # refers to 'sitkNearestNeighbor'
+        return F.affine(mask,
+                        scales=self.scale,
+                        degrees=self.angles,
+                        translation=self.translation,
+                        interpolation=interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+    def apply_to_float_mask(self, mask, **params):
+        return F.affine(mask,
+                        scales=self.scale,
+                        degrees=self.angles,
+                        translation=self.translation,
+                        interpolation=self.interpolation,
+                        border_mode=self.mask_mode,
+                        value=self.mval,
+                        spacing=self.spacing)
+
+
+# TODO create checks (mean, std, got good shape, and etc.), what if given list but only one channel, and reverse.
+class NormalizeMeanStd(ImageOnlyTransform):
+    """Normalize image values to have mean 0 and standard deviation 1, given channel-wise means and standard deviations.
+
+        For a single-channel image, the normalization is applied by the formula: :math:`img = (img - mean) / std`.
+        If the image contains more channels, then the previous formula is used for each channel separately.
+
+        It is recommended to input dataset-wide means and standard deviations.
+
+        Args:
+            mean (float | List[float]): Channel-wise image mean.
+
+                Must be either of: ``M``, ``(M_1, M_2, ..., M_C)``.
+            std (float | List[float]): Channel-wise image standard deviation.
+
+                Must be either of: ``S``, ``(S_1, S_2, ..., S_C)``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``True``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image
+    """
+    def __init__(self, mean: Union[List[float], float], std: Union[List[float], float],
+                 always_apply: bool = True, p: float = 1.0):
+        super().__init__(always_apply, p)
+        self.mean = np.array(mean, dtype=np.float32) 
+        self.std = np.array(std, dtype=np.float32) 
+        self.denominator = np.reciprocal(self.std, dtype=np.float32)
+
+    def apply(self, image, **params):
+        return F.normalize_mean_std(image, self.mean, self.denominator)
+
+    def __repr__(self):
+        return f'NormalizeMeanStd({self.mean}, {self.std}, ' \
+               f' {self.always_apply}, {self.p})'
+
+
+class GaussianBlur(ImageOnlyTransform):
+    """Performs Gaussian blurring of the image. In case of a multi-channel image, individual channels are blured separately.
+
+        Internally, the ``scipy.ndimage.gaussian_filter`` function is used. The ``border_mode`` and ``cval``
+        arguments are forwarded to it. More details at:
+        https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.gaussian_filter.html.
+
+        Args:
+            sigma (float, Tuple(float), List[Tuple(float) | float] , optional): Gaussian sigma.
+
+                Must be either of: ``S``, ``(S_Z, S_Y, S_X)``, ``(S_Z, S_Y, S_X, S_T)``, ``[S_1, S_2, ..., S_C]``,
+                ``[(S_Z1, S_Y1, S_X1), (S_Z2, S_Y2, S_X2), ..., (S_ZC, S_YC, S_XC)]``, or
+                ``[(S_Z1, S_Y1, S_X1, S_T1), (S_Z2, S_Y2, S_X2, S_T2), ..., (S_ZC, S_YC, S_XC, S_TC)]``.
+
+                If a float, the spatial dimensions are blurred with the same strength (equivalent to ``(S, S, S)``).
+
+                If a tuple, the sigmas for spatial dimensions and possibly the time dimension must be specified.
+
+                If a list, sigmas for each channel must be specified either as a single number or as a tuple.
+
+                Defaults to ``0.8``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'reflect'``.
+            cval (float, optional): Value to fill past edges of image. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image
+    """
+    def __init__(self, sigma: Union[float , Tuple[float], List[ Union[Tuple[float], float]]] = 0.8,
+                 border_mode: str = "reflect", cval: float = 0,
+                 always_apply: bool = False, p: float = 0.5):
+        
+        super().__init__(always_apply, p)
+        self.sigma = sigma
+        self.border_mode = border_mode
+        self.cval = cval
+
+    def apply(self, img, **params):
+        return F.gaussian_blur(img, self.sigma, self.border_mode, self.cval)
+
+
+class RandomGaussianBlur(ImageOnlyTransform):
+    """Performs Gaussian blur on the image with a random strength blurring.
+        In case of a multi-channel image, individual channels are blured separately.
+
+        Behaves similarly to GaussianBlur. The Gaussian sigma is randomly drawn from
+        the interval [min_sigma, s] for the respective s from ``max_sigma`` for each channel and dimension.
+
+        Internally, the ``scipy.ndimage.gaussian_filter`` function is used. The ``border_mode`` and ``cval``
+        arguments are forwarded to it. More details at:
+        https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.gaussian_filter.html.
+
+        Args:
+            max_sigma (float, Tuple(float), List[Tuple(float) | float] , optional): Maximum Gaussian sigma.
+
+                Must be either of: ``S``, ``(S_Z, S_Y, S_X)``, ``(S_Z, S_Y, S_X, S_T)``, ``[S_1, S_2, ..., S_C]``,
+                ``[(S_Z1, S_Y1, S_X1), (S_Z2, S_Y2, S_X2), ..., (S_ZC, S_YC, S_XC)]``, or
+                ``[(S_Z1, S_Y1, S_X1, S_T1), (S_Z2, S_Y2, S_X2, S_T2), ..., (S_ZC, S_YC, S_XC, S_TC)]``.
+
+                If a float, the spatial dimensions are blurred equivalently (equivalent to ``(S, S, S)``).
+
+                If a tuple, the sigmas for spatial dimensions and possibly the time dimension must be specified.
+
+                If a list, sigmas for each channel must be specified either as a single number or as a tuple.
+
+                Defaults to ``0.8``.
+            min_sigma (float, optional): Minimum Gaussian sigma for all channels and dimensions.
+
+                Defaults to ``0``.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'reflect'``.
+            cval (float, optional): Value to fill past edges of image. Only applied when ``border_mode = 'constant'``.
+
+                Defaults to ``0``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image
+    """
+    def __init__(self, max_sigma: Union[float, TypeTripletFloat] = 0.8,
+                 min_sigma: float = 0, border_mode: str = "reflect", cval: float = 0,
+                 always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.max_sigma = parse_coefs(max_sigma)
+        self.min_sigma = min_sigma
+        self.border_mode = border_mode
+        self.cval = cval
+
+    def apply(self, img, **params):
+        return F.gaussian_blur(img, params["sigma"], self.border_mode, self.cval)
+
+    def get_params(self, **data):
+        if isinstance(self.max_sigma, (float, int)):
+            sigma = random.uniform(self.min_sigma, self.max_sigma)
+        elif isinstance(self.max_sigma, tuple):
+            sigma = tuple([random.uniform(self.min_sigma, self.max_sigma[i]) for i in range(len(self.max_sigma))])
+        else:
+            sigma = []
+            for channel in self.max_sigma:
+                if isinstance(channel, (float, int)):
+                    sigma.append(random.uniform(self.min_sigma, channel))
+                else:
+                    sigma.append(tuple([random.uniform(self.min_sigma, channel) for i in range(len(channel))]))
+        return {"sigma": sigma}
+
+
+class RandomGamma(ImageOnlyTransform):
+    """Performs the gamma transformation with a randomly chosen gamma. If image values (in any channel) are outside
+        the [0,1] interval, this transformation is not performed.
+
+        Args:
+            gamma_limit (Tuple(float), optional): Interval from which gamma is selected.
+
+                Defaults to ``(0.8, 1.2)``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image
+    """
+    def __init__(self, gamma_limit: Tuple[float] = (0.8, 1.2),
+                 always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply, p)
+        self.gamma_limit = gamma_limit
+
+    def apply(self, img, gamma=1, **params):
+        return F.gamma_transform(img, gamma=gamma)
+
+    def get_params(self, **data):
+        return {"gamma": random.uniform(self.gamma_limit[0], self.gamma_limit[1])}
+
+    def __repr__(self):
+        return f'RandomGamma({self.gamma_limit}, {self.always_apply}, {self.p})'
+
+
+class RandomBrightnessContrast(ImageOnlyTransform):
+    """Randomly change brightness and contrast of the input image.
+
+        Unlike ``RandomBrightnessContrast`` from `Albumentations`, this transform is using the
+        formula :math:`f(a) = (c+1) * a + b`, where :math:`c` is contrast and :math:`b` is brightness.
+
+        Args:
+            brightness_limit ((float, float) | float, optional): Interval from which the change in brightness is
+                randomly drawn. If the change in brightness is 0, the brightness will not change.
+
+                Must be either of: ``B``, ``(B1, B2)``.
+
+                If a float, the interval will be ``(-B, B)``.
+
+                Defaults to ``0.2``.
+            contrast_limit ((float, float) | float, optional): Interval from which the change in contrast is
+                randomly drawn. If the change in contrast is 1, the contrast will not change.
+
+                Must be either of: ``C``, ``(C1, C2)``.
+
+                If a float, the interval will be ``(-C, C)``.
+
+                Defaults to ``0.2``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``0.5``.
+
+        Targets:
+            image
+    """
+    def __init__(self, brightness_limit=0.2, contrast_limit=0.2, always_apply=False, p=0.5,):
+        super().__init__(always_apply, p)
+        self.brightness_limit = to_tuple(brightness_limit)
+        self.contrast_limit = to_tuple(contrast_limit)
+
+    def apply(self, img, **params):
+        return F.brightness_contrast_adjust(img, params['alpha'], params['beta'])
+
+    def get_params(self, **data):
+        return {
+            "alpha": 1.0 + random.uniform(self.contrast_limit[0], self.contrast_limit[1]),
+            "beta": 0.0 + random.uniform(self.brightness_limit[0], self.brightness_limit[1]),
+        }
+
+    def __repr__(self):
+        return f'RandomBrightnessContrast({self.brightness_limit}, {self.contrast_limit},  ' \
+               f'{self.always_apply}, {self.p})'
+
+
+class HistogramEqualization(ImageOnlyTransform):
+    """Performs equalization of histogram. The equalization is done channel-wise, meaning that each channel is equalized
+        separately.
+
+        **Warning! Images are normalized over both spatial and temporal domains together. The output is in the range [0, 1].**
+
+        Args:
+            bins (int, optional): Number of bins for image histogram.
+
+                Defaults to ``256``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``False``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image
+    """
+    def __init__(self, bins: int = 256, always_apply: bool = False, p: float = 1):
+        super().__init__(always_apply, p)
+        self.bins = bins
+
+    def apply(self, img, **params):
+        return F.histogram_equalization(img, self.bins)
+
+
+class Pad(DualTransform):
+    """Pads the input.
+
+        Args:
+            pad_size (int | Tuple[int] | List[int | Tuple[int]]): Number of pixels padded to the edges of each axis.
+
+                Must be either of: ``P``, ``(P1, P2)``, ``[P_Z, P_Y, P_X]``, ``[P_Z, P_Y, P_X, P_T]``,
+                ``[(P_Z1, P_Z2), (P_Y1, P_Y2), (P_X1, P_X2)]``, or
+                ``[(P_Z1, P_Z2), (P_Y1, P_Y2), (P_X1, P_X2), (P_T1, P_T2)]``.
+
+                If an integer, it is equivalent to ``[(P, P), (P, P), (P, P)]``.
+
+                If a tuple, it is equivalent to ``[(P1, P2), (P1, P2), (P1, P2)]``.
+
+                If a list, it must specify padding for all spatial dimensions and possibly also for the time dimension.
+
+                The unspecified dimensions (C and possibly T) are not affected.
+            border_mode (str, optional): Values outside image domain are filled according to this mode.
+
+                Defaults to ``'constant'``.
+            ival (float | Sequence, optional): Values of `image` voxels outside of the `image` domain.
+                Only applied when ``border_mode = 'constant'`` or ``border_mode = 'linear_ramp'``.
+
+                Defaults to ``0``.
+            mval (float | Sequence, optional): Values of `mask` voxels outside of the `mask` domain.
+                Only applied when ``border_mode = 'constant'`` or ``border_mode = 'linear_ramp'``.
+
+                Defaults to ``0``.
+            ignore_index (float | None, optional): If a float, then transformation of `mask` is done with 
+                ``border_mode = 'constant'`` and ``mval = ignore_index``. 
+                
+                If ``None``, this argument is ignored.
+
+                Defaults to ``None``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``True``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, pad_size: Union[int, Tuple[int],  List[Union[int, Tuple[int]]]], border_mode: str = 'constant',
+                 ival: Union[float, Sequence] = 0, mval: Union[float, Sequence] = 0,
+                 ignore_index: Union[float, None] = None, always_apply: bool = True, p : float = 1):
+        super().__init__(always_apply, p)
+        self.pad_size = pad_size
+        self.border_mode = border_mode
+        self.mask_mode = border_mode 
+        self.ival = ival
+        self.mval = mval
+
+        if not (ignore_index is None):
+            self.mask_mode = "constant"
+            self.mval = ignore_index
+
+    def apply(self, img, **params):
+        return F.pad_pixels(img, self.pad_size, self.border_mode, self.ival)
+
+    def apply_to_mask(self, mask, **params):
+        return F.pad_pixels(mask, self.pad_size, self.mask_mode, self.mval, True)
+
+    def __repr__(self):
+        return f'Pad({self.pad_size}, {self.border_mode}, {self.ival}, {self.mval}, {self.always_apply}, ' \
+               f'{self.p})'
+
+
+class Normalize(ImageOnlyTransform):
+    """Change image mean and standard deviation to the given values (channel-wise).
+
+        Args:
+            mean (float | List[float], optional): The desired channel-wise means.
+
+                Must be either of: ``M``, ``[M_1, M_2, ..., M_C]``.
+
+                Defaults to ``0``.
+            std (float | List[float], optional): The desired channel-wise standard deviations.
+
+                Must be either of: ``S``, ``[S_1, S_2, ..., S_C]``.
+
+                Defaults to ``1``.
+            always_apply (bool, optional): Always apply this transformation in composition. 
+            
+                Defaults to ``True``.
+            p (float, optional): Chance of applying this transformation in composition. 
+            
+                Defaults to ``1``.
+
+        Targets:
+            image
+    """
+    def __init__(self, mean: Union[float, List[float]] = 0, std: Union[float, List[float]] = 1,
+                 always_apply: bool = True, p: float = 1.0):
+        super().__init__(always_apply, p)
+        self.mean = mean
+        self.std = std
+
+    def apply(self, img, **params):
+        return F.normalize(img, self.mean, self.std)
+
+    def __repr__(self):
+        return f'Normalize({self.mean}, {self.std}, {self.always_apply}, {self.p})'
+
+
+class Contiguous(DualTransform):
+    """Transform the image data to a contiguous array.
+
+        Args:
+            always_apply (bool, optional): Always apply this transformation in composition.
+
+                Defaults to ``True``.
+            p (float, optional): Chance of applying this transformation in composition.
+
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, always_apply: bool = True, p: float = 1.0):
+        super().__init__(always_apply, p)
+
+    def apply(self, image, **params):
+        return np.ascontiguousarray(image)
+
+    def apply_to_mask(self, mask, **params):
+        return np.ascontiguousarray(mask)
+
+    def __repr__(self):
+        return f'Contiguous({self.always_apply}, {self.p})'
+
+
+class Float(DualTransform):
+    """Change datatype to ``np.float32`` without changing intensities.
+
+        Args:
+            always_apply (bool, optional): Always apply this transformation in composition.
+
+                Defaults to ``True``.
+            p (float, optional): Chance of applying this transformation in composition.
+
+                Defaults to ``1``.
+
+        Targets:
+            image, mask, float_mask
+    """
+    def __init__(self, always_apply: bool = True, p: float = 1.0):
+        super().__init__(always_apply, p)
+
+    def apply(self, image, **params):
+        return image.astype(np.float32)
+
+    def apply_to_mask(self, mask, **params):
+        return mask.astype(np.float32)
+
+    def __repr__(self):
+        return f'Float({self.always_apply}, {self.p})'
+
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/conversion/__init__.py` & `bio_volumentations-1.1.0/bio_volumentations/conversion/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-from ..conversion.transforms import *
-
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+from ..conversion.transforms import *
+
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/conversion/functional.py` & `bio_volumentations-1.1.0/bio_volumentations/conversion/functional.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-
-
-
-def check_dimensions(list_of_shapes : list):
-    for i in range(1,len(list_of_shapes)):
-        if len(list_of_shapes[i]) != len(list_of_shapes[i - 1]):
-            return True    
-    return False
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+
+def check_dimensions(list_of_shapes: list):
+    for i in range(1, len(list_of_shapes)):
+        if len(list_of_shapes[i]) != len(list_of_shapes[i - 1]):
+            return True
+    return False
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/conversion/transforms.py` & `bio_volumentations-1.1.0/bio_volumentations/conversion/transforms.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,138 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-import torch
-from ..core.transforms_interface import *
-from ..conversion import functional as FCT
-from warnings import warn
-
-
-class ConversionToFormat(DualTransform):
-    def __init__(self, always_apply: bool = False, p: float = 1):
-        """Adds channel dimension to the 3D images without it"""
-        super().__init__(always_apply,p)
-
-    def __call__(self, force_apply, targets, **data):
-        if force_apply or self.always_apply or random.random() < self.p:
-            params = self.get_params(**data)
-
-            if VERBOSE:
-                print('RUN', self.__class__.__name__, params)
-            img_shape = []
-            mask_shape = []
-            float_shape = []
-            for k, v in data.items():
-                if k in targets[0]:
-                    img_shape.append(v.shape) 
-                elif k in targets[1]:
-                    mask_shape.append(v.shape) 
-                elif k in targets[2]:
-                    float_shape.append(v.shape) 
-            
-            if FCT.check_dimensions(img_shape):
-                warn(f"Input images shapes do not have same length,", UserWarning)
-            elif FCT.check_dimensions(mask_shape):
-                warn(f"Input masks shapes do not have same length,", UserWarning)
-            elif FCT.check_dimensions(float_shape):
-                warn(f"Float masks shapes do not have same length,", UserWarning)
-
-            for k, v in data.items():
-                if k in targets[0]:
-                    if len(v.shape) == 3:
-                        warn(f"Adding channel dimension to the image", UserWarning)
-                        data[k] = v[None, ...]
-
-        return data
-
-    def apply(self, volume, **params):
-        return volume
-
-    def apply_to_mask(self, mask, **params):
-        return mask
-
-    def __repr__(self):
-        return f'ConversionToFormat()'
-
-
-class NoConversion(DualTransform):
-    def __init__(self):
-        super().__init__()
-
-    def apply(self, volume, **params):
-        return volume
-
-    def apply_to_mask(self, mask, **params):
-        return mask
-
-    def __repr__(self):
-        return f'NoConversion()'
-
-
-
-class ToTensor(DualTransform):
-    """Convert image and masks to `torch.Tensor` with standard pytorch format: `CDHW(T)` for images, 'DHW(T)' for masks.
-    Args:
-        always_apply (bool): Indicates whether this transformation should be always applied. Default: True.
-        p (float): Probability of applying the transform. Default: 1.0.
-    """
-
-    def __init__(self, always_apply=True, p=1.0):
-        super(ToTensor, self).__init__(always_apply=always_apply, p=p)
-
-    def apply(self, img, **params):
-        return torch.from_numpy(img)
-
-    def apply_to_mask(self, mask, **params):
-        return torch.from_numpy(mask)
-
-    def __repr__(self):
-        return f'ToTensor({self.always_apply}, {self.p})'
-
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+
+import random
+from ..core.transforms_interface import DualTransform
+from ..conversion import functional as FCT
+from warnings import warn
+
+
+class ConversionToFormat(DualTransform):
+    """Check the very basic assumptions about the input images.
+
+        Adds channel dimension to the 3D images without it. Checks that shapes of individual target types are
+        consistent (to some extent).
+
+        Args:
+            always_apply (bool, optional): Always apply this transformation in composition.
+
+                Defaults to ``True``.
+            p (float, optional): Chance of applying this transformation in composition.
+
+                Defaults to ``1``.
+
+        Targets:
+            image, mask
+    """
+    def __init__(self, always_apply: bool = True, p: float = 1):
+        super().__init__(always_apply, p)
+
+    def __call__(self, force_apply, targets, **data):
+        if force_apply or self.always_apply or random.random() < self.p:
+            # params = self.get_params(**data)
+
+            img_shape = []
+            mask_shape = []
+            float_shape = []
+            for k, v in data.items():
+                if k in targets[0]:
+                    img_shape.append(v.shape) 
+                elif k in targets[1]:
+                    mask_shape.append(v.shape) 
+                elif k in targets[2]:
+                    float_shape.append(v.shape) 
+            
+            if FCT.check_dimensions(img_shape):
+                warn(f"Input images shapes do not have same length,", UserWarning)
+            elif FCT.check_dimensions(mask_shape):
+                warn(f"Input masks shapes do not have same length,", UserWarning)
+            elif FCT.check_dimensions(float_shape):
+                warn(f"Float masks shapes do not have same length,", UserWarning)
+
+            for k, v in data.items():
+                if k in targets[0]:
+                    if len(v.shape) == 3:
+                        warn(f"Adding channel dimension to the image", UserWarning)
+                        data[k] = v[None, ...]
+
+        return data
+
+    def apply(self, volume, **params):
+        return volume
+
+    def apply_to_mask(self, mask, **params):
+        return mask
+
+    def apply_to_float_mask(self, mask, **params):
+        return mask
+
+    def __repr__(self):
+        return f'ConversionToFormat({self.always_apply}, {self.p})'
+
+
+class NoConversion(DualTransform):
+    """An identity transform.
+
+        Args:
+            always_apply (bool, optional): Always apply this transformation in composition.
+
+                Defaults to ``True``.
+            p (float, optional): Chance of applying this transformation in composition.
+
+                Defaults to ``1``.
+
+        Targets:
+            image, mask
+    """
+    def __init__(self, always_apply: bool = True, p: float = 1):
+        super().__init__(always_apply, p)
+
+    def apply(self, volume, **params):
+        return volume
+
+    def apply_to_mask(self, mask, **params):
+        return mask
+
+    def apply_to_float_mask(self, mask, **params):
+        return mask
+
+    def __repr__(self):
+        return f'NoConversion({self.always_apply}, {self.p})'
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/core/composition.py` & `bio_volumentations-1.1.0/bio_volumentations/core/composition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,96 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-import random
-from ..augmentations import transforms as T
-from ..conversion import transforms as CT
-
-
-class Compose:
-    def __init__(self, transforms, p=1.0, targets=[['image'], ['mask'], ['float_mask']], conversion=None):
-        assert 0 <= p <= 1
-        self.transforms = [T.Float(always_apply=True), CT.ConversionToFormat(always_apply= True)] +  transforms + [T.Contiguous(always_apply=True)] + \
-                          [CT.NoConversion() if conversion is None else conversion]
-        self.p = p
-        self.targets = targets
-
-    def get_always_apply_transforms(self):
-        res = []
-        for tr in self.transforms:
-            if tr.always_apply:
-                res.append(tr)
-        return res
-
-    def __call__(self, force_apply=False, **data):
-        need_to_run = force_apply or random.random() < self.p
-        transforms = self.transforms if need_to_run else self.get_always_apply_transforms()
-
-        for tr in transforms:
-            data = tr(force_apply, self.targets, **data)
-
-        return data
-
-    def __repr__(self):
-        return f'Compose({self.transforms[1:-2]}, {self.p}, {self.targets}, {self.transforms[-1]})'
-
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+
+import random
+from ..augmentations import transforms as T
+from ..conversion import transforms as CT
+
+
+class Compose:
+    """Compose a list of transformations into a callable transformation pipeline.
+
+    **It is strongly recommended to use** ``Compose`` **to define and use the transformation pipeline.**
+
+    In addition, basic input image checks and conversions are performed. Optionally, datatype conversion
+    (e.g. from ``numpy.ndarray`` to ``torch.Tensor``) is performed.
+
+    Args:
+        transforms (List[Transform]): List of transforms (objects of type ``Transform``).
+
+        p (float, optional): Chance of applying the whole pipeline.
+
+            Defaults to ``1``.
+        targets (Tuple[List[str]] | List[List[str]], optional): List of targets.
+
+            Defaults to ``(['image'], ['mask'], ['float_mask'])``.
+        conversion (Transform | None, optional): Image datatype conversion transform, applied after the transformations.
+
+            Defaults to ``None``.
+    """
+    def __init__(self, transforms, p=1.0, targets=(['image'], ['mask'], ['float_mask']), conversion=None):
+        assert 0 <= p <= 1
+        self.transforms = ([T.Float(always_apply=True),
+                            CT.ConversionToFormat(always_apply=True)] +
+                           transforms +
+                           [T.Contiguous(always_apply=True)] +
+                           [CT.NoConversion() if conversion is None else conversion])
+        self.p = p
+        self.targets = targets
+
+    def get_always_apply_transforms(self):
+        res = []
+        for tr in self.transforms:
+            if tr.always_apply:
+                res.append(tr)
+        return res
+
+    def __call__(self, force_apply=False, **data):
+        need_to_run = force_apply or random.random() < self.p
+        transforms = self.transforms if need_to_run else self.get_always_apply_transforms()
+
+        for tr in transforms:
+            data = tr(force_apply, self.targets, **data)
+
+        return data
+
+    def __repr__(self):
+        return f'Compose({self.transforms[1:-2]}, {self.p}, {self.targets}, {self.transforms[-1]})'
+
```

### Comparing `bio_volumentations-1.0.10/bio_volumentations/volumentations_biomedicine/random_utils.py` & `bio_volumentations-1.1.0/bio_volumentations/random_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,93 @@
-# ============================================================================================= #
-#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller, Lucia Hradecká           #
-#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
-#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
-#                ZFTurbo            : https://github.com/ZFTurbo                                #
-#                ashawkey           : https://github.com/ashawkey                               #
-#                Dominik Müller     : https://github.com/muellerdo                              #
-#                Lucia Hradecká     : https://gitlab.fi.muni.cz/xdupkan/                        #
-#                                                                                               #
-#  Volumentations History:                                                                      #
-#       - Original:                 https://github.com/albumentations-team/albumentations       #
-#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
-#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
-#       - Enhancements:             https://github.com/qubvel/volumentations                    #
-#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
-#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/xdupkan/volumentations/           #
-#                                                                                               #
-#  MIT License.                                                                                 #
-#                                                                                               #
-#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
-#  of this software and associated documentation files (the "Software"), to deal                #
-#  in the Software without restriction, including without limitation the rights                 #
-#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
-#  copies of the Software, and to permit persons to whom the Software is                        #
-#  furnished to do so, subject to the following conditions:                                     #
-#                                                                                               #
-#  The above copyright notice and this permission notice shall be included in all               #
-#  copies or substantial portions of the Software.                                              #
-#                                                                                               #
-#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
-#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
-#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
-#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
-#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
-#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
-#  SOFTWARE.                                                                                    #
-# ============================================================================================= #
-import numpy as np
-from typing import Optional, Sequence, Union, Type, Any
-import random as py_random
-
-NumType = Union[int, float, np.ndarray]
-IntNumType = Union[int, np.ndarray]
-Size = Union[int, Sequence[int]]
-
-
-def get_random_state() -> np.random.RandomState:
-    return np.random.RandomState(py_random.randint(0, (1 << 32) - 1))
-
-
-def randint(
-        low: IntNumType,
-        high: Optional[IntNumType] = None,
-        size: Optional[Size] = None,
-        dtype: Type = np.int32,
-        random_state: Optional[np.random.RandomState] = None,
-) -> Any:
-    if random_state is None:
-        random_state = get_random_state()
-    return random_state.randint(low, high, size, dtype)
-
-
-def uniform(
-        low: NumType = 0.0,
-        high: NumType = 1.0,
-        size: Optional[Size] = None,
-        random_state: Optional[np.random.RandomState] = None,
-) -> Any:
-    if random_state is None:
-        random_state = get_random_state()
-    return random_state.uniform(low, high, size)
-
-
-def normal(
-        loc: NumType = 0.0,
-        scale: NumType = 1.0,
-        size: Optional[Size] = None,
-        random_state: Optional[np.random.RandomState] = None,
-) -> Any:
-    if random_state is None:
-        random_state = get_random_state()
-    return random_state.normal(loc, scale, size)
+# ============================================================================================= #
+#  Author:       Pavel Iakubovskii, ZFTurbo, ashawkey, Dominik Müller,                          #
+#                Samuel Šuľan, Lucia Hradecká, Filip Lux                                        #
+#  Copyright:    albumentations:    : https://github.com/albumentations-team                    #
+#                Pavel Iakubovskii  : https://github.com/qubvel                                 #
+#                ZFTurbo            : https://github.com/ZFTurbo                                #
+#                ashawkey           : https://github.com/ashawkey                               #
+#                Dominik Müller     : https://github.com/muellerdo                              #
+#                Lucia Hradecká     : lucia.d.hradecka@gmail.com                                #
+#                Filip Lux          : lux.filip@gmail.com                                       #
+#                                                                                               #
+#  Volumentations History:                                                                      #
+#       - Original:                 https://github.com/albumentations-team/albumentations       #
+#       - 3D Conversion:            https://github.com/ashawkey/volumentations                  #
+#       - Continued Development:    https://github.com/ZFTurbo/volumentations                   #
+#       - Enhancements:             https://github.com/qubvel/volumentations                    #
+#       - Further Enhancements:     https://github.com/muellerdo/volumentations                 #
+#       - Biomedical Enhancements:  https://gitlab.fi.muni.cz/cbia/bio-volumentations           #
+#                                                                                               #
+#  MIT License.                                                                                 #
+#                                                                                               #
+#  Permission is hereby granted, free of charge, to any person obtaining a copy                 #
+#  of this software and associated documentation files (the "Software"), to deal                #
+#  in the Software without restriction, including without limitation the rights                 #
+#  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell                    #
+#  copies of the Software, and to permit persons to whom the Software is                        #
+#  furnished to do so, subject to the following conditions:                                     #
+#                                                                                               #
+#  The above copyright notice and this permission notice shall be included in all               #
+#  copies or substantial portions of the Software.                                              #
+#                                                                                               #
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR                   #
+#  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,                     #
+#  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE                  #
+#  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER                       #
+#  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,                #
+#  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE                #
+#  SOFTWARE.                                                                                    #
+# ============================================================================================= #
+
+import numpy as np
+from typing import Optional, Sequence, Union, Type, Any
+from .typing import TypeSextetFloat, TypeTripletFloat
+import random as random
+
+NumType = Union[int, float, np.ndarray]
+IntNumType = Union[int, np.ndarray]
+Size = Union[int, Sequence[int]]
+
+
+def get_random_state() -> np.random.RandomState:
+    return np.random.RandomState(random.randint(0, (1 << 32) - 1))
+
+
+def randint(
+        low: IntNumType,
+        high: Optional[IntNumType] = None,
+        size: Optional[Size] = None,
+        dtype: Type = np.int32,
+        random_state: Optional[np.random.RandomState] = None,
+) -> Any:
+    if random_state is None:
+        random_state = get_random_state()
+    return random_state.randint(low, high, size, dtype)
+
+
+def uniform(
+        low: NumType = 0.0,
+        high: NumType = 1.0,
+        size: Optional[Size] = None,
+        random_state: Optional[np.random.RandomState] = None,
+) -> Any:
+    if random_state is None:
+        random_state = get_random_state()
+    return random_state.uniform(low, high, size)
+
+
+def normal(
+        loc: NumType = 0.0,
+        scale: NumType = 1.0,
+        size: Optional[Size] = None,
+        random_state: Optional[np.random.RandomState] = None,
+) -> Any:
+    if random_state is None:
+        random_state = get_random_state()
+    return random_state.normal(loc, scale, size)
+
+
+def sample_range_uniform(limits: TypeSextetFloat,
+                         random_state: Optional[np.random.RandomState] = None) -> TypeTripletFloat:
+    return (random.uniform(limits[0], limits[1]),
+            random.uniform(limits[2], limits[3]),
+            random.uniform(limits[4], limits[5]))
```

