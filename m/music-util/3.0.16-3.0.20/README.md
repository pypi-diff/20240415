# Comparing `tmp/music_util-3.0.16.tar.gz` & `tmp/music_util-3.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music_util-3.0.16.tar", last modified: Mon Dec 18 18:21:08 2023, max compression
+gzip compressed data, was "music_util-3.0.20.tar", last modified: Mon Apr 15 01:28:59 2024, max compression
```

## Comparing `music_util-3.0.16.tar` & `music_util-3.0.20.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 18:21:08.058863 music_util-3.0.16/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-18 18:20:59.000000 music_util-3.0.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-18 18:21:08.058863 music_util-3.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-18 18:20:59.000000 music_util-3.0.16/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-18 18:21:01.000000 music_util-3.0.16/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-18 18:20:59.000000 music_util-3.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 18:21:08.058863 music_util-3.0.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 18:21:08.054862 music_util-3.0.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 18:21:08.054862 music_util-3.0.16/src/music_util/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-18 18:20:59.000000 music_util-3.0.16/src/music_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-12-18 18:20:59.000000 music_util-3.0.16/src/music_util/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-18 18:20:59.000000 music_util-3.0.16/src/music_util/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-18 18:20:59.000000 music_util-3.0.16/src/music_util/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-12-18 18:20:59.000000 music_util-3.0.16/src/music_util/transcr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-12-18 18:20:59.000000 music_util-3.0.16/src/music_util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-12-18 18:20:59.000000 music_util-3.0.16/src/music_util/voc_rem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 18:21:08.058863 music_util-3.0.16/src/music_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-18 18:21:08.000000 music_util-3.0.16/src/music_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-18 18:21:08.000000 music_util-3.0.16/src/music_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 18:21:08.000000 music_util-3.0.16/src/music_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-18 18:21:08.000000 music_util-3.0.16/src/music_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-18 18:21:08.000000 music_util-3.0.16/src/music_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-18 18:21:08.000000 music_util-3.0.16/src/music_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:28:59.780914 music_util-3.0.20/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 01:28:55.000000 music_util-3.0.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 01:28:59.780914 music_util-3.0.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-15 01:28:55.000000 music_util-3.0.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 01:28:57.000000 music_util-3.0.20/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-15 01:28:55.000000 music_util-3.0.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:28:59.780914 music_util-3.0.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:28:59.772914 music_util-3.0.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:28:59.776914 music_util-3.0.20/src/music_util/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 01:28:55.000000 music_util-3.0.20/src/music_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-15 01:28:55.000000 music_util-3.0.20/src/music_util/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 01:28:55.000000 music_util-3.0.20/src/music_util/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-15 01:28:55.000000 music_util-3.0.20/src/music_util/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-15 01:28:55.000000 music_util-3.0.20/src/music_util/transcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 01:28:55.000000 music_util-3.0.20/src/music_util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-15 01:28:55.000000 music_util-3.0.20/src/music_util/voc_rem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:28:59.776914 music_util-3.0.20/src/music_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-15 01:28:59.000000 music_util-3.0.20/src/music_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 01:28:59.000000 music_util-3.0.20/src/music_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:28:59.000000 music_util-3.0.20/src/music_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 01:28:59.000000 music_util-3.0.20/src/music_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 01:28:59.000000 music_util-3.0.20/src/music_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 01:28:59.000000 music_util-3.0.20/src/music_util.egg-info/top_level.txt
```

### Comparing `music_util-3.0.16/PKG-INFO` & `music_util-3.0.20/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music_util
-Version: 3.0.16
+Version: 3.0.20
 Summary: Collection of utilities for musicians
 Author-email: Maoserr <maoserr@gmail.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/maoserr/music-util/issues
 Project-URL: Source, https://github.com/maoserr/music-util
 Keywords: music, utility
 Requires-Python: >=3.7
@@ -30,13 +30,29 @@
 
 [Demucs](https://github.com/facebookresearch/demucs)
 
 ![Voc](https://raw.githubusercontent.com/maoserr/music-util/develop/doc/voc_remover.png?raw=true "Vocals")
 
 ## Transcription
 
-Attempts to generate note graph using MP3 file. 
+Attempts to generate sheet music using MP3 file.
 This only works if there's one note per time, and not on chords.
+(Mostly as a starting point for manual transcription, and not an accurate solution.)
+
+MP3 is converted into a Lilypond file (.ly). You can then compile into PDFs.
 
 [Crepe](https://github.com/marl/crepe)
 
 ![Tra](https://raw.githubusercontent.com/maoserr/music-util/develop/doc/trans.png?raw=true "Transcription")
+
+Sample Lilypond results:
+```
+{
+r1 r1 ais2 cis'1 cis'1 f'8 gis'8 
+ r4 gis'1 fis'2 dis'1 r2 ais8 cis'4 
+ ais8 cis'4 r16 dis'2 fis'1 r16 ais4 
+ b16 r1 gis2 r1 cis'1 dis'4 f'2 
+ gis'1 gis'1 dis'2 r1 f'4 r1 r1 
+ cis'1 cis'1 r8 ais16 a2 r4 cis'4 
+ ...
+}
+```
```

### Comparing `music_util-3.0.16/pyproject.toml` & `music_util-3.0.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `music_util-3.0.16/src/music_util/icon.png` & `music_util-3.0.20/src/music_util/icon.png`

 * *Files identical despite different names*

### Comparing `music_util-3.0.16/src/music_util/main.py` & `music_util-3.0.20/src/music_util/main.py`

 * *Files identical despite different names*

### Comparing `music_util-3.0.16/src/music_util/pipe.py` & `music_util-3.0.20/src/music_util/pipe.py`

 * *Files identical despite different names*

### Comparing `music_util-3.0.16/src/music_util/transcr.py` & `music_util-3.0.20/src/music_util/voc_rem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,105 @@
 import os
 import sys
 import tkinter as tk
 from tkinter import ttk, filedialog
+from collections import OrderedDict
 from multiprocessing import Process, Queue
 
-import librosa
-import pandas as pd
+model_list = OrderedDict([
+    ("HT Demucs (fine-tuned)", "htdemucs_ft"),
+    ("HT Demucs", "htdemucs"),
+    ("HT Demucs + Guitar & Piano", "htdemucs_6s"),
+])
+
+default_opts = {
+    "HT Demucs (fine-tuned)": "--two-stems vocals --mp3",
+}
 
 
-def get_notes(notes: pd.DataFrame, outfile: str, tempo: float, beats: list):
-    beat_len_ms = (60 * 1000) / tempo
-    min_note_len = beat_len_ms / 16
-
-    notes['chg'] = notes.note.ne(notes.note.shift())
-    notes['not_rest'] = notes.confidence.gt(0.6)
-    notes['notes_chg'] = notes['chg'] & notes['not_rest']
-    notes['notes_size'] = notes['notes_chg'].cumsum()
-
-    notes_uniq = notes.groupby('notes_size').agg({
-        'pitch': 'first',
-        'confidence': 'first',
-        'note': 'first',
-        'chg': 'count',
-        'not_rest': 'first',
-        'notes_chg': 'first'
-    })
-    outdf = notes
-    outdf.to_csv(outfile)
-
-
-def crepe_exe(args: list, q: Queue):
+def demucs_exec(args: list, q: Queue):
     from music_util.utils import StdoutProcRedirect
     sys.stdout = StdoutProcRedirect(q)
     sys.stderr = StdoutProcRedirect(q)
 
     try:
-        import torchcrepe
-        import numpy as np
         import torch
-        import os
+        from demucs import separate
+        if torch.cuda.is_available():
+            device = "cuda"
+        else:
+            device = "cpu"
+        print(f"GPU acceleration: {device}")
 
-        infiles = args[0]
-        for file in infiles:
-            audio_rosa, sr = librosa.load(file, sr=16000, mono=True)
-            tempo, beats = librosa.beat.beat_track(y=audio_rosa, sr=sr)
-            if audio_rosa.dtype == np.int16:
-                audio_rosa = audio_rosa.astype(np.float32) / np.iinfo(np.int16).max
-
-            audio = torch.tensor(np.copy(audio_rosa.transpose()))[None]
-            pitch, confidence = torchcrepe.predict(audio, sr, return_periodicity=True, model="tiny")
-            notes = pd.DataFrame({"pitch": pitch.numpy().squeeze(), "confidence": confidence.numpy().squeeze()})
-            notes['note'] = librosa.hz_to_note(notes['pitch'])
-            get_notes(notes, args[1], tempo, beats)
+        separate.main(args)
         print("Processing complete")
     except:
         import traceback
         traceback.print_exc()
 
 
-class Transcript(tk.Frame):
+class VocalRemover(tk.Frame):
     def __init__(self, root: ttk.Notebook, q: Queue, *args, **kwargs):
         tk.Frame.__init__(self, root, *args, **kwargs)
         self.grid()
         self.q = q
 
+        default_model = list(model_list.keys())[0]
+
         self.outfile = tk.StringVar(root, os.path.join(os.getcwd(), "out"))
-        self.inpfile = tk.StringVar(root, "")
+        self.model = tk.StringVar(root, list(model_list.keys())[0])
+        self.adv_opt = tk.StringVar(root, default_opts.get(default_model, ""))
         r = 0
 
         # Input row
-        ttk.Label(self, text="Input").grid(row=r, column=0, sticky="n")
+        ttk.Label(self, text="Inputs").grid(row=r, column=0, sticky="n")
         self.inp_list = ttk.Treeview(self, columns=('file',), show='headings')
         self.inp_list.column('file')
         self.inp_list.heading('file', text="MP3 Input Files")
         self.inp_list.grid(row=r, column=1, sticky="nsew")
-        ttk.Button(self, text="+", command=self.set_infile).grid(row=r, column=2, sticky="new")
+        ttk.Button(self, text="+", command=self.set_file).grid(row=r, column=2, sticky="new")
         r = r + 1
 
         # Output row
         ttk.Label(self, text="Output").grid(row=r, column=0)
         ttk.Entry(self, textvariable=self.outfile).grid(row=r, column=1, sticky="ew")
         ttk.Button(self, text="...", command=self.set_outfile).grid(row=r, column=2, sticky="new")
         r = r + 1
 
+        # Model selection row
+        ttk.Label(self, text="Model").grid(row=r, column=0)
+        ttk.Combobox(self, textvariable=self.model, state="readonly",
+                     values=list(model_list.keys())).grid(row=r, column=1, sticky="we")
+        r = r + 1
+
         # Run row
-        ttk.Button(self, text="Run", command=self.run_transcipt).grid(row=r, column=2, sticky="e")
+        ttk.Label(self, text="Advanced").grid(row=r, column=0)
+        ttk.Entry(self, textvariable=self.adv_opt).grid(row=r, column=1, sticky="ew")
+        ttk.Button(self, text="Run", command=self.run_demucs).grid(row=r, column=2, sticky="e")
+        r = r + 1
 
         self.grid_columnconfigure(1, weight=4)
+        self.grid_rowconfigure(1, weight=4)
         for child in self.winfo_children():
             child.grid_configure(padx=5, pady=5)
 
-    def set_outfile(self):
-        self.outfile.set(tk.filedialog.asksaveasfilename(title='Select output location',
-                                                         filetypes=(("CSV file", "*.csv"),)))
-
-    def set_infile(self):
+    def set_file(self):
         files = tk.filedialog.askopenfilenames(title='Select MP3',
                                                initialdir='/',
                                                filetypes=(("MP3", "*.mp3"), ("All files", "*.*")))
         for i in files:
             self.inp_list.insert('', tk.END, values=(i,))
 
-    def run_transcipt(self):
+    def set_outfile(self):
+        self.outfile.set(tk.filedialog.asksaveasfilename(title='Select output location',
+                                                         filetypes=(("Folder", "*.*"),)))
+
+    def run_demucs(self):
         in_files = [self.inp_list.item(i)['values'][0] for i in self.inp_list.get_children()]
-        outfile = self.outfile.get()
-        print("Starting crepes...")
-        all_args = [in_files, outfile]
-        p = Process(target=crepe_exe, args=(all_args, self.q))
+        mod = model_list[self.model.get()]
+        args = self.adv_opt.get().split()
+        out = self.outfile.get()
+        print("Starting demucs...")
+        all_args = ["-n", mod, "--out", out] + args + in_files
+        print("All args: " + " ".join(all_args))
+        p = Process(target=demucs_exec, args=(all_args, self.q))
         p.start()
```

### Comparing `music_util-3.0.16/src/music_util.egg-info/PKG-INFO` & `music_util-3.0.20/src/music_util.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: music-util
-Version: 3.0.16
+Name: music_util
+Version: 3.0.20
 Summary: Collection of utilities for musicians
 Author-email: Maoserr <maoserr@gmail.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/maoserr/music-util/issues
 Project-URL: Source, https://github.com/maoserr/music-util
 Keywords: music, utility
 Requires-Python: >=3.7
@@ -30,13 +30,29 @@
 
 [Demucs](https://github.com/facebookresearch/demucs)
 
 ![Voc](https://raw.githubusercontent.com/maoserr/music-util/develop/doc/voc_remover.png?raw=true "Vocals")
 
 ## Transcription
 
-Attempts to generate note graph using MP3 file. 
+Attempts to generate sheet music using MP3 file.
 This only works if there's one note per time, and not on chords.
+(Mostly as a starting point for manual transcription, and not an accurate solution.)
+
+MP3 is converted into a Lilypond file (.ly). You can then compile into PDFs.
 
 [Crepe](https://github.com/marl/crepe)
 
 ![Tra](https://raw.githubusercontent.com/maoserr/music-util/develop/doc/trans.png?raw=true "Transcription")
+
+Sample Lilypond results:
+```
+{
+r1 r1 ais2 cis'1 cis'1 f'8 gis'8 
+ r4 gis'1 fis'2 dis'1 r2 ais8 cis'4 
+ ais8 cis'4 r16 dis'2 fis'1 r16 ais4 
+ b16 r1 gis2 r1 cis'1 dis'4 f'2 
+ gis'1 gis'1 dis'2 r1 f'4 r1 r1 
+ cis'1 cis'1 r8 ais16 a2 r4 cis'4 
+ ...
+}
+```
```

