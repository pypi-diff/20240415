# Comparing `tmp/noteshrunk-1.2.0.tar.gz` & `tmp/noteshrunk-1.3.0.tar.gz`

## Comparing `noteshrunk-1.2.0.tar` & `noteshrunk-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/CHANGELOG.md
--rwxr-xr-x   0        0        0    23956 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/src/noteshrunk.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/LICENSE
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    45710 2020-02-02 00:00:00.000000 noteshrunk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/CHANGELOG.md
+-rwxr-xr-x   0        0        0    24255 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/src/noteshrunk.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    45903 2020-02-02 00:00:00.000000 noteshrunk-1.3.0/PKG-INFO
```

### Comparing `noteshrunk-1.2.0/CHANGELOG.md` & `noteshrunk-1.3.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.3] - 2024-04-15
+
+### Changed
+
+- Replaced `--global_palette` with `--local_palette` to make the global palette the default.
+
 ## [1.2] - 2024-04-13
 
 ### Added
 
 - This changelog file
 - Added a check for the existence of all input files so that the error is raised immediately and not halfway through processing.
```

### Comparing `noteshrunk-1.2.0/src/noteshrunk.py` & `noteshrunk-1.3.0/src/noteshrunk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
+VERSION = '1.3.0'
 
 import argparse
 from concurrent.futures import ThreadPoolExecutor
 import os
 from pathlib import Path
 import random
 import re
@@ -28,34 +29,31 @@
     Returns:
         argparse.Namespace: A namespace that holds the arguments as attributes.
     """
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description='Compress scanned documents')
 
-    parser.add_argument('files', nargs='+', help='Input image file paths.')
+    parser.add_argument(
+        'files',
+        nargs='+',
+        help='Input image file paths.')
     parser.add_argument(
         '-o',
         '--output',
         default='output.pdf',
         type=Path,
         help='Output PDF file path.')
     parser.add_argument(
         '-w',
         '--white_background',
         action='store_true',
         default=False,
         help='Use white background instead of dominant color.')
     parser.add_argument(
-        '-g',
-        '--global_palette',
-        action='store_true',
-        default=False,
-        help='Use the same color palette for all images by sampling -p percent of the pixels from every input image.')
-    parser.add_argument(
         '-s',
         '--saturate',
         action='store_true',
         default=False,
         help='Maximize saturation in the output image.')
     parser.add_argument(
         '-n',
@@ -72,27 +70,39 @@
     parser.add_argument(
         "-q",
         "--quality",
         type=int,
         default=75,
         choices=range(1, 101),  # Allow values between 1 and 100 (inclusive)
         metavar="[1-100]",
-        help="JPEG quality of the embedded images")
+        help='JPEG quality of the images embedded in the PDF')
+    parser.add_argument(
+        '-l',
+        '--local_palette',
+        action='store_true',
+        default=False,
+        help='Create an individual color palette for each image (by sampling a -p percentage of the pixels of that image) instead of a global palette (by sampling a -p percentage of the pixels of each input image).')
     parser.add_argument(
         "-p",
         "--percentage",
         type=float,
         default=10,
-        help="Percentage of pixels to sample from every image.")
+        help="Percentage of pixels to sample from each image.")
     parser.add_argument(
-        '-k',
-        '--keep_intermediate',
+        "-j",
+        "--jobs",
+        type=int,
+        default=os.cpu_count(),
+        help="Number of processes to use (default: number of CPU cores)")
+    parser.add_argument(
+        '-y',
+        '--overwrite',
         action='store_true',
         default=False,
-        help='Do not delete intermediate (single-page) PDFs afterwards.')
+        help='Overwrite existing files without asking.')
     parser.add_argument(
         "-ts",
         "--threshold_saturation",
         type=float,
         default=15,
         help="HSV saturation threshold (in percent) used for the background detection.")
     parser.add_argument(
@@ -119,43 +129,42 @@
     parser.add_argument(
         "-ms",
         "--median_strength",
         type=int,
         default=3,
         help="Strength of median filtering")
     parser.add_argument(
-        "-os",
-        "--opening_strength",
-        type=float,
-        default=3,
-        help="Strength of opening filtering / radius of the structuring element (disk)")
-    parser.add_argument(
         "-cs",
         "--closing_strength",
         type=float,
         default=3,
         help="Strength of closing filtering / radius of the structuring element (disk)")
     parser.add_argument(
-        "-j",
-        "--jobs",
-        type=int,
-        default=os.cpu_count(),
-        help="Number of processes to use (default: number of CPU cores)")
+        "-os",
+        "--opening_strength",
+        type=float,
+        default=3,
+        help="Strength of opening filtering / radius of the structuring element (disk)")
+    parser.add_argument(
+        '-k',
+        '--keep_intermediate',
+        action='store_true',
+        default=False,
+        help='Do not delete intermediate (single-page) PDFs afterwards.')
     parser.add_argument(
         '-v',
         '--verbose',
         action='store_true',
         default=False,
         help='Verbose output')
     parser.add_argument(
-        '-y',
-        '--overwrite',
-        action='store_true',
-        default=False,
-        help='Overwrite existing files without asking.')
+        '--version',
+        action='version',
+        version=VERSION,
+        help='Show program version and exit')
 
     argcomplete.autocomplete(parser)
     return parser.parse_args()
 
 
 def sort_filenames(filenames):
     """
@@ -678,18 +687,18 @@
     """
     image = io.imread(file)
 
     processed_images = []
 
     verbose_print(args, 'Processing image {}'.format(idx + 1))
 
-    if args.global_palette:
-        color_palette, kmeans_model = global_palette
-    else:
+    if args.local_palette:
         color_palette, kmeans_model = create_palette(image, args)
+    else:
+        color_palette, kmeans_model = global_palette
 
     image = apply_color_palette(image, color_palette, kmeans_model, args)
 
     save_as_pdf(image, output_filename, args)
 
 
 def check_file_existence(files):
@@ -714,40 +723,41 @@
 
 
 def main():
     """
     The main function of the program.
     """
     args = parse_args()
+
     file_paths = sort_filenames(args.files)
     check_file_existence(file_paths)
 
     # Create a temporary folder at the output file location for storing intermediate PDFs.
     # This way the intermediate files are automatically deleted upon program exit.
     # Each image is converted to a single-page PDF before concatenation
     # afterwards, which reduces the memory footprint.
     with tempfile.TemporaryDirectory(dir=os.getcwd(), prefix='tmp_pdfs-', delete=(not args.keep_intermediate)) as temp_dir:
 
         intermediate_pdf_paths = []
 
-        if args.global_palette:
+        if not args.local_palette:
             color_palette, kmeans_model = create_palette(file_paths, args, use_global_palette=True)
 
         with ThreadPoolExecutor(max_workers=args.jobs) as executor:
 
             for idx, file in enumerate(file_paths):
 
                 output_filename = args.output.parent / temp_dir / Path(file.name).with_suffix('.pdf')
 
                 # E.g. the same input file multiple times
                 if output_filename in intermediate_pdf_paths or output_filename.exists():
                     output_filename = rename_with_random_string(output_filename)
 
                 executor.submit(process_image, file=file, output_filename=output_filename, idx=idx, args=args,
-                                 global_palette=(color_palette, kmeans_model) if args.global_palette else None)
+                                 global_palette=(color_palette, kmeans_model) if not args.local_palette else None)
 
                 intermediate_pdf_paths.append(output_filename)
 
             executor.shutdown(wait=True)
 
         verbose_print(
             args,
```

### Comparing `noteshrunk-1.2.0/.gitignore` & `noteshrunk-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.2.0/LICENSE` & `noteshrunk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noteshrunk-1.2.0/README.md` & `noteshrunk-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,65 +14,68 @@
 * **Customizable Palette:** Allows you to specify the number of colors in the output palette and choose between a global palette for all pages or individual palettes for each page.
 * **Color Control:** Offers the option to maximize saturation in the output image as well as to remove the background (replace with white), enhancing visual clarity.
 * **Denoising Options:** Provides median filtering and morphological operations to reduce noise and improve image quality.
 * **Parallel processing:** Utilizes multiple CPU cores for faster processing of multiple images.
 
 ## Requirements
 
+### Python Packages
+
 - argcomplete
 - NumPy
 - Pillow (PIL Fork)
 - Python 3
 - scikit-image
 - scikit-learn
 - SciPy
 
-### Optional
+### Other
 
-- Ghostscript (for PDF merging; otherwise you need to use the `-k` flag)
+- Ghostscript (executable `gs` in PATH - for PDF merging)
 
 ## Installation
 
 ```bash
 pipx install noteshrunk
 ```
 
 ## Usage
 
 ```
-noteshrunk [-h] [-o OUTPUT] [-w] [-g] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]]
-           [-p PERCENTAGE] [-k] [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
-           [--denoise_median] [--denoise_closing] [--denoise_opening] [-ms MEDIAN_STRENGTH]
-           [-os OPENING_STRENGTH] [-cs CLOSING_STRENGTH] [-j JOBS] [-v] [-y]
-           files [files ...]
+noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]] [-l]
+           [-p PERCENTAGE] [-j JOBS] [-y] [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
+           [--denoise_median] [--denoise_closing] [--denoise_opening]
+           [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH] [-os OPENING_STRENGTH]
+           [-k] [-v] [--version] files [files ...]
 ```
 
 ### Arguments
 
 * `files`: A list of paths to the input image files.
 * `-o`, `--output`: Path to the output PDF file (default: `output.pdf`).
 * `-w`, `--white_background`: Use white background instead of dominant color.
-* `-g`, `--global_palette`: Use the same color palette for all images by sampling a percentage of the pixels from every input image.
 * `-s`, `--saturate`: Maximize saturation in the output image.
 * `-n`, `--n_colors`: Number of colors in the palette (default: 8).
 * `-d`, `--dpi`: DPI value of the input images (default: 300).
-* `-q`, `--quality`: JPEG quality of the embedded images (1-100, default: 75).
-* `-p`, `--percentage`: Percentage of pixels to sample from every image for global palette creation (default: 10).
-* `-k`, `--keep_intermediate`: Keep the intermediate single-page PDFs.
+* `-q`, `--quality`: JPEG quality of the images embedded in the PDF (1-100, default: 75).
+* `-l`, `--local_palette`: Create an individual color palette for each image (by sampling a -p percentage of the pixels of that image) instead of a global palette (by sampling a -p percentage of the pixels of each input image).
+* `-p`, `--percentage`: Percentage of pixels to sample from each input image for color palette creation (default: 10).
+* `-j`, `--jobs`: Number of threads to use for multi-threading (default: number of CPU cores).
+* `-y`, `--overwrite`: Overwrite existing files without asking.
 * `-ts`, `--threshold_saturation`: HSV saturation threshold (in percent) used for background detection (default: 15).
 * `-tv`, `--threshold_value`: HSV value threshold (in percent) used for background detection (default: 25).
 * `--denoise_median`: Apply median denoising.
 * `--denoise_closing`: Apply morphological closing on the background mask.
 * `--denoise_opening`: Apply morphological opening on the background mask.
 * `-ms`, `--median_strength`: Strength of median filtering (default: 3).
-* `-os`, `--opening_strength`: Strength of opening filtering / radius of the structuring element (disk, default: 3).
 * `-cs`, `--closing_strength`: Strength of closing filtering / radius of the structuring element (disk, default: 3).
-* `-j`, `--jobs`: Number of processes to use (default: number of CPU cores).
+* `-os`, `--opening_strength`: Strength of opening filtering / radius of the structuring element (disk, default: 3).
+* `-k`, `--keep_intermediate`: Keep the intermediate single-page PDFs.
 * `-v`, `--verbose`: Verbose output.
-* `-y`, `--overwrite`: Overwrite existing files without asking.
+* `--version`: Show program version and exit.
 
 ## Examples
 
 1.  Compress a single image with default settings:
 
     ```bash
     noteshrunk input.png
@@ -80,17 +83,17 @@
 
 2.  Compress multiple images with a white background and 16 colors:
 
     ```bash
     noteshrunk -w -n 16 image1.jpg image2.png
     ```
 
-3.  Compress images using a global palette and keep intermediate files while disabling multi-processing:
+3.  Compress images using a local color palette and keep intermediate files while disabling multi-threading:
     ```bash
-    noteshrunk -g -j 1 -k *.jpg
+    noteshrunk -l -j 1 -k *.jpg
     ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues or pull requests on the GitHub repository.
 
 ## Acknowledgements
```

### Comparing `noteshrunk-1.2.0/pyproject.toml` & `noteshrunk-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "noteshrunk"
-version = "1.2.0"
+version = "1.3.0"
 description = "Document Color Palette Compression"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 authors = [
     {name = "suuuehgi"}
 ]
```

### Comparing `noteshrunk-1.2.0/PKG-INFO` & `noteshrunk-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: noteshrunk
-Version: 1.2.0
+Version: 1.3.0
 Summary: Document Color Palette Compression
 Project-URL: Homepage, https://github.com/suuuehgi/noteshrunk
 Project-URL: Issues, https://github.com/suuuehgi/noteshrunk/issues
 Author: suuuehgi
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -708,65 +708,68 @@
 * **Customizable Palette:** Allows you to specify the number of colors in the output palette and choose between a global palette for all pages or individual palettes for each page.
 * **Color Control:** Offers the option to maximize saturation in the output image as well as to remove the background (replace with white), enhancing visual clarity.
 * **Denoising Options:** Provides median filtering and morphological operations to reduce noise and improve image quality.
 * **Parallel processing:** Utilizes multiple CPU cores for faster processing of multiple images.
 
 ## Requirements
 
+### Python Packages
+
 - argcomplete
 - NumPy
 - Pillow (PIL Fork)
 - Python 3
 - scikit-image
 - scikit-learn
 - SciPy
 
-### Optional
+### Other
 
-- Ghostscript (for PDF merging; otherwise you need to use the `-k` flag)
+- Ghostscript (executable `gs` in PATH - for PDF merging)
 
 ## Installation
 
 ```bash
 pipx install noteshrunk
 ```
 
 ## Usage
 
 ```
-noteshrunk [-h] [-o OUTPUT] [-w] [-g] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]]
-           [-p PERCENTAGE] [-k] [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
-           [--denoise_median] [--denoise_closing] [--denoise_opening] [-ms MEDIAN_STRENGTH]
-           [-os OPENING_STRENGTH] [-cs CLOSING_STRENGTH] [-j JOBS] [-v] [-y]
-           files [files ...]
+noteshrunk [-h] [-o OUTPUT] [-w] [-s] [-n N_COLORS] [-d DPI] [-q [1-100]] [-l]
+           [-p PERCENTAGE] [-j JOBS] [-y] [-ts THRESHOLD_SATURATION] [-tv THRESHOLD_VALUE]
+           [--denoise_median] [--denoise_closing] [--denoise_opening]
+           [-ms MEDIAN_STRENGTH] [-cs CLOSING_STRENGTH] [-os OPENING_STRENGTH]
+           [-k] [-v] [--version] files [files ...]
 ```
 
 ### Arguments
 
 * `files`: A list of paths to the input image files.
 * `-o`, `--output`: Path to the output PDF file (default: `output.pdf`).
 * `-w`, `--white_background`: Use white background instead of dominant color.
-* `-g`, `--global_palette`: Use the same color palette for all images by sampling a percentage of the pixels from every input image.
 * `-s`, `--saturate`: Maximize saturation in the output image.
 * `-n`, `--n_colors`: Number of colors in the palette (default: 8).
 * `-d`, `--dpi`: DPI value of the input images (default: 300).
-* `-q`, `--quality`: JPEG quality of the embedded images (1-100, default: 75).
-* `-p`, `--percentage`: Percentage of pixels to sample from every image for global palette creation (default: 10).
-* `-k`, `--keep_intermediate`: Keep the intermediate single-page PDFs.
+* `-q`, `--quality`: JPEG quality of the images embedded in the PDF (1-100, default: 75).
+* `-l`, `--local_palette`: Create an individual color palette for each image (by sampling a -p percentage of the pixels of that image) instead of a global palette (by sampling a -p percentage of the pixels of each input image).
+* `-p`, `--percentage`: Percentage of pixels to sample from each input image for color palette creation (default: 10).
+* `-j`, `--jobs`: Number of threads to use for multi-threading (default: number of CPU cores).
+* `-y`, `--overwrite`: Overwrite existing files without asking.
 * `-ts`, `--threshold_saturation`: HSV saturation threshold (in percent) used for background detection (default: 15).
 * `-tv`, `--threshold_value`: HSV value threshold (in percent) used for background detection (default: 25).
 * `--denoise_median`: Apply median denoising.
 * `--denoise_closing`: Apply morphological closing on the background mask.
 * `--denoise_opening`: Apply morphological opening on the background mask.
 * `-ms`, `--median_strength`: Strength of median filtering (default: 3).
-* `-os`, `--opening_strength`: Strength of opening filtering / radius of the structuring element (disk, default: 3).
 * `-cs`, `--closing_strength`: Strength of closing filtering / radius of the structuring element (disk, default: 3).
-* `-j`, `--jobs`: Number of processes to use (default: number of CPU cores).
+* `-os`, `--opening_strength`: Strength of opening filtering / radius of the structuring element (disk, default: 3).
+* `-k`, `--keep_intermediate`: Keep the intermediate single-page PDFs.
 * `-v`, `--verbose`: Verbose output.
-* `-y`, `--overwrite`: Overwrite existing files without asking.
+* `--version`: Show program version and exit.
 
 ## Examples
 
 1.  Compress a single image with default settings:
 
     ```bash
     noteshrunk input.png
@@ -774,17 +777,17 @@
 
 2.  Compress multiple images with a white background and 16 colors:
 
     ```bash
     noteshrunk -w -n 16 image1.jpg image2.png
     ```
 
-3.  Compress images using a global palette and keep intermediate files while disabling multi-processing:
+3.  Compress images using a local color palette and keep intermediate files while disabling multi-threading:
     ```bash
-    noteshrunk -g -j 1 -k *.jpg
+    noteshrunk -l -j 1 -k *.jpg
     ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues or pull requests on the GitHub repository.
 
 ## Acknowledgements
```

