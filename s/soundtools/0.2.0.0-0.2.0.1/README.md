# Comparing `tmp/soundtools-0.2.0.0.tar.gz` & `tmp/soundtools-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.0.0.tar", last modified: Fri Apr 12 20:02:15 2024, max compression
+gzip compressed data, was "soundtools-0.2.0.1.tar", last modified: Mon Apr 15 02:09:38 2024, max compression
```

## Comparing `soundtools-0.2.0.0.tar` & `soundtools-0.2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 20:02:15.058745 soundtools-0.2.0.0/
--rw-rw-rw-   0        0        0      701 2024-04-12 20:02:15.057748 soundtools-0.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 20:02:15.058745 soundtools-0.2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-04-12 20:01:40.000000 soundtools-0.2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:02:15.055690 soundtools-0.2.0.0/soundtools/
--rw-rw-rw-   0        0        0      369 2024-04-07 11:11:28.000000 soundtools-0.2.0.0/soundtools/__init__.py
--rw-rw-rw-   0        0        0    36057 2024-04-12 19:59:12.000000 soundtools-0.2.0.0/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:02:15.057748 soundtools-0.2.0.0/soundtools.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 20:02:14.000000 soundtools-0.2.0.0/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 02:09:38.975987 soundtools-0.2.0.1/
+-rw-rw-rw-   0        0        0      705 2024-04-15 02:09:38.975987 soundtools-0.2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 02:09:38.975987 soundtools-0.2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      793 2024-04-15 02:08:58.000000 soundtools-0.2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:09:38.964952 soundtools-0.2.0.1/soundtools/
+-rw-rw-rw-   0        0        0      391 2024-04-12 20:06:10.000000 soundtools-0.2.0.1/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    35935 2024-04-15 02:07:19.000000 soundtools-0.2.0.1/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-15 02:09:38.974991 soundtools-0.2.0.1/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      705 2024-04-15 02:09:38.000000 soundtools-0.2.0.1/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-15 02:09:38.000000 soundtools-0.2.0.1/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 02:09:38.000000 soundtools-0.2.0.1/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 02:09:38.000000 soundtools-0.2.0.1/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.0.0/PKG-INFO` & `soundtools-0.2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
-made by Mohammad Erfan Karami
+### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.0
+version: 0.2.0.1
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.0.0/setup.py` & `soundtools-0.2.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.0.0',
+version='0.2.0.1',
 description="used to work with sounds waves",
-long_description="""made by Mohammad Erfan Karami
+long_description="""### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.0
+version: 0.2.0.1
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.0.0/soundtools/soundtools.py` & `soundtools-0.2.0.1/soundtools/soundtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,69 +42,61 @@
 
 #-- sound waves --#
 class Sounds:
     """has some basic sound waves and also caches the result of the functions for faster output"""
     def __init__(self, sample_rate: int=48000, dtype:np.float32|np.int16|np.uint8=np.float32) -> None:
         self.default_sample_rate: int = sample_rate
         self.existed_notes: dict[str, tuple] = {}
-        self.cache_at_dur: float = 1
         
         self.tau = 2*np.pi
         self.rev_pi = 1/np.pi
         self.two_oper_pi = 2/np.pi
         self.four_over_pi = 4/np.pi
         self.eight_over_pi_sqr = 8/np.pi**2
         
         self.change_dtype(dtype)
     
     
     def change_dtype(self, dtype: Dtype):
         self.dtype = dtype
         if self.dtype == np.float32:
-            self.min_amp = -1
-            self.max_amp = 1
+            self.min_amp = -0.95
+            self.max_amp = 0.95
         else:
             i = np.iinfo(self.dtype)
-            self.min_amp = i.min
-            self.max_amp = i.max
+            self.min_amp = i.min+1
+            self.max_amp = i.max-1
     
     
     # caches the waves so if you had to generate a note multiple times its not gonna take long to execute
     # you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable
     # so this decorator will save a tuple of that numpy array in self.existed_notes and convert it back to a numpy array each time you want to use that wave
     def cache_wave(wave_type: str) -> SoundBuffer:
         """caches the waves so if you had to generate a note multiple times it's gonna use the cached wave. 
         you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable, 
         so this decorator will store the numpy array as a tuple in "self.existed_notes" and convert it back to a numpy array each time you want to use that wave
         \nreturns the cached value if available, otherwise caches the returned wave"""
         def decorator(func: Wave) -> SoundBuffer:
             def wrapper(self, freq:float, dur:float, vol: float):
                 name = f"{wave_type}|{freq}"
                 if name in self.existed_notes.keys():
-                    wave = np.array(self.existed_notes[name], dtype=self.dtype)
-                    temp = wave.copy()
-                    mul = int(dur/self.cache_at_dur)
-                    if mul > 1:
-                        for _ in range(mul-1):
-                            wave = np.append(wave, temp)
-                    remainder = int((dur%self.cache_at_dur)*self.default_sample_rate)
-                    wave = vol * np.append(wave, wave[:remainder])
+                    wave = vol * np.array(self.existed_notes[name], dtype=self.dtype)
                     return wave
                 
-                temp = func(self, freq, self.cache_at_dur, 1)
+                temp = func(self, freq, dur, 1)
                 result: SoundBuffer = func(self, freq, dur, vol)
-                result[result > 1] = self.max_amp
-                result[result < -1] = self.min_amp
+                result[result > self.max_amp] = self.max_amp
+                result[result < self.min_amp] = self.min_amp
                 self.existed_notes[name] = self.array_to_tuple(temp)
                 
                 return result
             return wrapper
         return decorator
 
-    # @cache_wave("sine")
+    @cache_wave("sine")
     def sine_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a sine wave based on the given frequency, duration and amplituse or volume
         returns a numpy array"""
         
         wave = (vol * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)).astype(self.dtype)
         return wave
     
@@ -142,15 +134,15 @@
             if f > 20000:
                 break
             buf += (-1)**h * harmonic**(-2) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)
         
         wave = ((self.eight_over_pi_sqr)*vol*buf).astype(self.dtype)
         return wave
     
-    # @cache_wave("fast_tri")
+    @cache_wave("fast_tri")
     def fast_triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         return (self.two_oper_pi * vol * np.arcsin(np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate))).astype(self.dtype)
     
     @cache_wave("saw")
     def sawtooth_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """returns a numpy array,
         creates a sawtooth wave based on the given frequency, duration and amplitude or volume\n
@@ -299,14 +291,20 @@
     
     def fade_in_out(self, buffer: SoundBuffer, fadein_len:int = 1500, fadeout_len:int = 1500) -> SoundBuffer:
         buffer = self.fade_in(buffer, fadein_len)
         buffer = self.fade_out(buffer, fadeout_len)
         return buffer
     
     
+    def staccato(self, wave: SoundBuffer, dur: float, play_time: float=0.75) -> SoundBuffer:
+        playing = len(wave)*play_time
+        resting = (1-play_time)*dur
+        return np.append(wave[0:int(playing)], self.generate_note_buffer(0, self.sine_wave, resting))
+    
+    
     def array_to_tuple(self, np_array: SoundBuffer) -> tuple:
         """Iterates recursivelly."""
         try:
             return tuple(self.array_to_tuple(_) for _ in np_array)
         except TypeError:
             return np_array
```

### Comparing `soundtools-0.2.0.0/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.0.1/soundtools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.0.0
+Version: 0.2.0.1
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
-made by Mohammad Erfan Karami
+### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.0.0
+version: 0.2.0.1
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

