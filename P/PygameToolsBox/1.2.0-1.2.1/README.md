# Comparing `tmp/PygameToolsBox-1.2.0.tar.gz` & `tmp/pygametoolsbox-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.2.0.tar", last modified: Mon Apr  8 02:35:59 2024, max compression
+gzip compressed data, was "pygametoolsbox-1.2.1.tar", last modified: Sun Apr 14 23:28:00 2024, max compression
```

## Comparing `PygameToolsBox-1.2.0.tar` & `pygametoolsbox-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 02:35:59.101176 PygameToolsBox-1.2.0/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3717 2024-04-08 02:35:59.100175 PygameToolsBox-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-08 02:35:59.070180 PygameToolsBox-1.2.0/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-08 02:35:44.000000 PygameToolsBox-1.2.0/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     4376 2024-04-08 02:27:26.000000 PygameToolsBox-1.2.0/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      327 2024-04-08 02:08:23.000000 PygameToolsBox-1.2.0/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 PygameToolsBox-1.2.0/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.2.0/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-08 02:35:59.089179 PygameToolsBox-1.2.0/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3717 2024-04-08 02:35:59.000000 PygameToolsBox-1.2.0/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-08 02:35:59.000000 PygameToolsBox-1.2.0/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 02:35:59.000000 PygameToolsBox-1.2.0/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-08 02:35:59.000000 PygameToolsBox-1.2.0/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-08 02:35:59.000000 PygameToolsBox-1.2.0/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3111 2024-04-08 02:33:17.000000 PygameToolsBox-1.2.0/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 02:35:59.102175 PygameToolsBox-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 23:28:00.965778 pygametoolsbox-1.2.1/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 pygametoolsbox-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3717 2024-04-14 23:28:00.965778 pygametoolsbox-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 23:28:00.934502 pygametoolsbox-1.2.1/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-14 23:27:49.000000 pygametoolsbox-1.2.1/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     4513 2024-04-11 01:18:52.000000 pygametoolsbox-1.2.1/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      327 2024-04-08 02:08:23.000000 pygametoolsbox-1.2.1/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 pygametoolsbox-1.2.1/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3891 2024-04-11 00:36:46.000000 pygametoolsbox-1.2.1/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-14 23:28:00.950246 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3717 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-14 23:28:00.000000 pygametoolsbox-1.2.1/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3111 2024-04-08 02:33:17.000000 pygametoolsbox-1.2.1/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 pygametoolsbox-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 23:28:00.965778 pygametoolsbox-1.2.1/setup.cfg
```

### Comparing `PygameToolsBox-1.2.0/LICENSE` & `pygametoolsbox-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.2.0/PKG-INFO` & `pygametoolsbox-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.2.0/PygameToolsBox/animated_object.py` & `pygametoolsbox-1.2.1/PygameToolsBox/animated_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,38 +20,41 @@
                           specified more than one time the image will be showed
                           multiple time.
         """
         self.name = name
         self.repeat = repeat
         self.images_index = images_index
         self.iteration = 0
-        self.repeated = 0
+        self.repeat_pending = 0
+        self.stopped = True
 
     def start(self):
         """
         Initialize sequence animation. Start from initial settings
         """
-        self.repeated = self.repeat
+        self.repeat_pending = self.repeat
         self.iteration = 0
+        self.stopped = False
 
     def get_next(self) -> int:
         """
         Go to next index image
         """
         self.iteration += 1
 
         if self.iteration >= len(self.images_index):
-            if self.repeated > 0:
-                self.repeated -= 1
+            if self.repeat_pending > 0:
+                self.repeat_pending -= 1
                 self.iteration = 0
-            elif self.repeated < 0:
+            elif self.repeat_pending < 0:
                 self.iteration = 0
             else:
                 pygame.event.post(Event(ANIMATION_END))
-                self.iteration = len(self.images_index) - 1
+                self.stopped = True
+                self.iteration = -1
 
         return self.images_index[self.iteration]
 
 
 class AnimatedObject(Sprite):
     def __init__(self, images: [Surface], cooling: int):
         """
@@ -107,19 +110,18 @@
     def update(self):
         """
         Call every frame for adjust animation and object position
         :param pos: New position for the sprite
         """
         if self._cool_down > 0:
             self._cool_down -= 1
-        else:
+        elif not self._current_action.stopped:
             self._cool_down = self._cooling
             self._image_index = self._current_action.get_next()
-
-        self._set_image()
+            self._set_image()
 
     def draw(self, win: Surface):
         """
         Display object to the screen
         :param win: Surface to draw
         """
         win.blit(self.image, self.rect)
```

### Comparing `PygameToolsBox-1.2.0/PygameToolsBox/parallax_bg.py` & `pygametoolsbox-1.2.1/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.2.0/PygameToolsBox/spritesheet.py` & `pygametoolsbox-1.2.1/PygameToolsBox/spritesheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 class SpriteSheet:
     def __init__(self,
                  sprite_sheet_path: Path,
                  sprite_size_x: float,
                  sprite_size_y: float,
                  nb_rows: int,
                  nb_cols: int,
-                 alpha: bool = True):
+                 alpha: bool = True,
+                 scale: float = 1):
         """
         :param sprite_sheet_path:
             Path and file of the spead sheet
             All sprites of the sprite sheet must be relative to same purpose.
             N.B. Each instance of the image must have sames sizes. Each instance
             may have different height and width. Each sub-sprites is delimited by this width and height.
             It's possible in case you have multiples sprites to make many rows, in this case each rows must have the
@@ -28,20 +29,25 @@
             How many rows of the sub sprite, sprite sheet contains
         :param nb_cols:
             How many cols of the sub sprite, sprite sheet contains
         :param alpha:
             Is the sprite sheet contains a canal alpha for transparency. Otherwise,
             you may use the property "set_colorkey" from the sub image
         """
+        self.scale = scale
         if alpha:
             self._sprite_sheet = pygame.image.load(sprite_sheet_path).convert_alpha()
         else:
             self._sprite_sheet = pygame.image.load(sprite_sheet_path).convert()
-        self._sprite_size_x = sprite_size_x
-        self._sprite_size_y = sprite_size_y
+
+        if scale != 1:
+            self._sprite_sheet = pygame.transform.scale_by(self._sprite_sheet, scale)
+
+        self._sprite_size_x = sprite_size_x * scale
+        self._sprite_size_y = sprite_size_y * scale
         self._rows = nb_rows
         self._cols = nb_cols
         self._alpha = alpha
 
     def get_sprite(self, row: int, col: int) -> Surface | None:
         """
         :param row:
```

### Comparing `PygameToolsBox-1.2.0/PygameToolsBox.egg-info/PKG-INFO` & `pygametoolsbox-1.2.1/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.2.0/README.md` & `pygametoolsbox-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.2.0/pyproject.toml` & `pygametoolsbox-1.2.1/pyproject.toml`

 * *Files identical despite different names*

