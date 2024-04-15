# Comparing `tmp/artscraper-0.2.0.tar.gz` & `tmp/artscraper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artscraper-0.2.0.tar", last modified: Tue May 30 08:39:31 2023, max compression
+gzip compressed data, was "artscraper-0.3.1.tar", last modified: Mon Apr 15 09:42:03 2024, max compression
```

## Comparing `artscraper-0.2.0.tar` & `artscraper-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:39:31.452521 artscraper-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 08:39:17.000000 artscraper-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-30 08:39:31.452521 artscraper-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-30 08:39:17.000000 artscraper-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:39:31.452521 artscraper-0.2.0/artscraper/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/find_artists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/find_artworks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5688 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/googleart.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7634 2023-05-30 08:39:17.000000 artscraper-0.2.0/artscraper/wikiart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:39:31.452521 artscraper-0.2.0/artscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 08:39:31.000000 artscraper-0.2.0/artscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 08:39:31.452521 artscraper-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-30 08:39:17.000000 artscraper-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:42:03.618903 artscraper-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-15 09:41:58.000000 artscraper-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-15 09:42:03.618903 artscraper-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-15 09:41:58.000000 artscraper-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:42:03.618903 artscraper-0.3.1/artscraper/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-15 09:41:58.000000 artscraper-0.3.1/artscraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-15 09:41:58.000000 artscraper-0.3.1/artscraper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-15 09:41:58.000000 artscraper-0.3.1/artscraper/find_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-15 09:41:58.000000 artscraper-0.3.1/artscraper/find_artworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 09:41:58.000000 artscraper-0.3.1/artscraper/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8226 2024-04-15 09:41:58.000000 artscraper-0.3.1/artscraper/googleart.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7634 2024-04-15 09:41:58.000000 artscraper-0.3.1/artscraper/wikiart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:42:03.618903 artscraper-0.3.1/artscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-15 09:42:03.000000 artscraper-0.3.1/artscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-15 09:42:03.000000 artscraper-0.3.1/artscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:42:03.000000 artscraper-0.3.1/artscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 09:42:03.000000 artscraper-0.3.1/artscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 09:42:03.000000 artscraper-0.3.1/artscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 09:42:03.618903 artscraper-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 09:41:58.000000 artscraper-0.3.1/setup.py
```

### Comparing `artscraper-0.2.0/LICENSE` & `artscraper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `artscraper-0.2.0/README.md` & `artscraper-0.3.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 
 # ArtScraper
 
 ArtScraper is a tool to download images and metadata for artworks available on
 WikiArt (www.wikiart.org/) and Google Arts & Culture
 (artsandculture.google.com/).
 
+Functionality:
+- `WikiArt` and `Google Arts & Culture`: Download images and metadata from a list of artworks' urls
+- `Google Arts & Culture`: Download all images and metadata in the site, or from specific artists
 
-## Installation and setup
+## 1. Installation and setup
 
 The ArtScraper package can be installed with pip, which automatically installs
 the python dependencies:
 
 ```
 pip install artscraper
 ```
 
 
-### WikiArt
+## 2. Downloading art from WikiArt
 
 To download data from WikiArt it is necessary to obtain
 [API](https://www.wikiart.org/en/App/GetApi) keys. After obtaining them, you
 can put them in a file called `.wiki_api` in the working directory for your
 script. The format is: the API access key, a new line, the API secret key, and
 a new line, e.g.:
 
@@ -28,155 +31,113 @@
 7e57a60844
 3defc62d8f
 ```
 
 Alternatively, when ArtScraper doesn't detect the file `.wiki_api`, it will
 ask for the API keys.
 
-### Google Arts & Culture
+An example of fetching data is shown below and in the [notebook](examples/example_artscraper.ipynb). 
 
-To download data from GoogleArt it is necessary to install 
-[Firefox](https://www.mozilla.org/en-US/firefox/new/) and `geckodriver`. 
-
-There are two options to download the geckodriver.
-- Using a package manager (recommended on Linux/OS X): On Linux, geckodriver 
-is most likely available through the package manager for your distribution
-(e.g. on Ubuntu `sudo apt install firefox-geckodriver`. On OS X, it is the 
-easiest to install it through either [brew](https://formulae.brew.sh/formula/geckodriver#default) or [macports](https://ports.macports.org/port/geckodriver/) (e.g. `brew install geckodriver`). Depending on your settings, you might need to add the directory where the geckodriver resides to the PATH variable. 
-- Downloading it [from here](https://github.com/mozilla/geckodriver/releases) and making it available to the code. For example in Windows you can download the file `geckodriver-v0.31.0-win64.zip`, place the driver in the directory of your code, and specify the path when you initialize the GoogleArtScraper. For example:
 ```python
-with GoogleArtScraper(geckodriver_path="./geckodriver.exe") as scraper:
-    ...
-```
-
-Make sure that you have a recent version of geckodriver, because selenium (a non-python dependency used in the GoogleArt scraper) uses features that were only recently introduced 
-in geckodriver. We have only tested the scraping on Linux/Firefox and OSX/Firefox.
 
+from artscraper import WikiArtScraper
 
-## Download images and metadata (interactive)
-
-An example of fetching data is shown in an
-[example](examples/example_artscraper.ipynb) notebook. 
+art_url = "https://www.wikiart.org/en/edvard-munch/anxiety-1894"
 
-Assuming the WikiArtScraper
-is used, we can download the data from a link with:
+with WikiArtScraper(output_dir="data") as scraper:
+    scraper.load_link(art_url)
+    scraper.save_metadata() 
+    scraper.save_image()
 
-```python
+```
 
-from artscraper import WikiArtScraper
+This will store both the image itself and the metadata in separate folders. If
+you use ArtScraper in this way, it will skip images/metadata that is already
+present. Remove the directory to force it to redownload it. 
 
-scraper = WikiArtScraper()
+Results:
 
-# Load the URL into the scraper.
-scraper.load_link("some URL")
+[<img src="https://uploads5.wikiart.org/images/edvard-munch/anxiety-1894.jpg" weight="20">](https://www.wikiart.org/en/edvard-munch/anxiety-1894)
 
-# Get the metadata
-metadata = scraper.get_metadata()
 
-# Save the image to some local file
-scraper.save_image("wiki.jpg")
+## 3. Downloading art from Google Arts & Culture
 
-# Release resources
-scraper.close()
-```
+To download data from GoogleArt it is necessary to install 
+[Firefox](https://www.mozilla.org/en-US/firefox/new/).
 
-We can see that every time we want to download either images or metadata, we
-first load the URL into the scraper. For the GoogleArt implementation,
-releasing the resources with `scraper.close` will ensure that the browser is
-closed. The scraper should not be used after that.
+ArtScraper will open a new Firefox window, navigate to the image, zoom on it and take a screenshot of it. It will take a few seconds. Do not minimize that browser, and do not let the screensaver go on.
 
-## Download images and metadata (automatic)
 
-An example of fetching data is shown in an
-[example](examples/example_artscraper.ipynb) notebook.
+### 3.1 Downloading art from Google Arts & Culture using artworks' urls
 
-For many use cases it might be useful to download a series of links and store
-them in a consistent way.
+An example of fetching data is shown below and in the [notebook](examples/example_artscraper.ipynb). 
 
 ```python
-
 from artscraper import GoogleArtScraper
 
-with GoogleArtScraper("data/output/googlearts") as scraper:
-    for url in some_links:
-        scraper.load_link(url)
-        scraper.save_metadata()
-        scraper.save_image()
+art_url = "https://artsandculture.google.com/asset/anxiety-edvard-munch/JgE_nwHHS7wTPw"
+
+with GoogleArtScraper() as scraper:
+    scraper.load_link(art_url)
+    metadata = scraper.get_metadata() #or scraper.save_metadata()
+    scraper.save_image("data/anxiety_munch.jpg")
+    print(metadata) 
+
 ```
 
-This will store both the image itself and the metadata in separate folders. If
-you use ArtScraper in this way, it will skip images/metadata that is already
-present. Remove the directory to force it to redownload it.
 
-## Get list of all artists from Google Arts & Culture website
+### 3.2 Downloading all art from Google Arts & Culture 
 
-See [example notebook](examples/example_collect_all_artworks.ipynb). A list with the Google Arts& Culture web addresses of all artists is returned.
-```python
-from artscraper import get_artist_links
+See [example notebook](examples/example_collect_all_artworks.ipynb).
 
-# Get links for all artists, as a list. The links are also saved in a file.
-artist_urls = get_artist_links(executable_path='geckodriver', min_wait_time=1, output_file='artist_links.txt')
-```
+The final structure of the results will be
+- data
+  - artist_links.txt (All artists, with one url per line) 
+  - Artist_1
+    - description.txt (Description of artist, from wikidata)
+    - metadata.json (Metadata of arist, from wikidata)
+    - works.txt (All artworks, with one url per line)
+    - works 
+      - work1
+        - artwork.png (Artwork image)
+        - metadata.json (Metadata of artwork, from Google Art and Culture)
+      - work2
+        - ...
+  - Artist_2
+    - ... 
 
-## Get links to an artist's works
-A list of all works by a particular artist, specified by the address of their Google Arts & Culture webpage, is returned.
-  
-```python
-# Find links to artworks for a particular artist, from their Google Arts & Culture webpage url
-    with FindArtworks(artist_link=artist_url, output_dir=output_dir, min_wait_time=1) as scraper:
-		    # Get list of artist's works
-            artwork_links = scraper.get_artist_works()
-```
 
-## Get metadata about an artist
-Metadata for the artist is returned.
-```python
-# Get metadata for a particular artist, from their Google Arts & Culture webpage url
-    with FindArtworks(artist_link=artist_url, output_dir=output_dir, min_wait_time=1) as scraper:
-		    # Get list of artist's works
-            artwork_links = scraper.get_artist_metadata()
-```
+A full example (but please check the [example notebook](examples/example_collect_all_artworks.ipynb) to add retries):
 
-## Collect data about all artists, and all their artworks
-From a list containing links to all the artists, the following are saved, for each artist:
-1. List containing all works by the artist
-2. Description of the artist
-3. Metadata of the artist
-4. Image and metadata of each artwork by the artist
 ```python
+from artscraper.find_artists import get_artist_links
+# Get links for all artists, as a list
+output_dir = "data"
+artist_urls = get_artist_links(min_wait_time=1, output_file=f'{output_dir}/artist_links.txt')
+
+# Find_artworks for each artist
 for artist_url in artist_urls:
-    with FindArtworks(artist_link=artist_url, output_dir=output_dir, min_wait_time=1) as scraper:
-            # Save list of works, description, and metadata for an artist
+    with FindArtworks(artist_link=artist_url, output_dir=output_dir, 
+                      min_wait_time=min_wait_time) as scraper:
+            # Save list of artworks, the description, and metadata for an artist
             scraper.save_artist_information()
-            # Get list of links to this artist's works 
-            artwork_links = scraper.get_artist_works()
-            # Create directory for this artist
-            artist_dir = output_dir + '/' + scraper.get_wikipedia_article_title()
+            # Find artist directory
+            artist_dir = output_dir + '/' + scraper.get_artist_name() 
+
     # Scrape artworks
-    with GoogleArtScraper(artist_dir + '/' + 'works', min_wait=1) as subscraper:
-        # Go through each artwork link
+    with GoogleArtScraper(artist_dir + '/' + 'works', min_wait=min_wait_time) as subscraper:
+        # Get list of links to this artist's works 
+        with open(artist_dir+'/'+'works.txt', 'r') as file:
+            artwork_links = [line.rstrip() for line in file]  
+        # Download all artwork link (slow)
         for url in artwork_links:
-            subscraper.load_link(url)
-            subscraper.save_metadata()
-            subscraper.save_image()
-```
-
-## Troubleshooting
-
-Sometimes the `GoogleArtScraper` returns white images (tested on OS X), which
-is most likely due to the screensaver kicking in. Apart from disabling the
-screensaver, the following shell command might be useful to remove most of the
-white images (if the data is in `data/output/google_arts`:
-
-```
-sh for F in $(find data/output/google_arts/ -iname painting.png -size -55k); do rm -r $(dirname $F); done
+            print(f'artwork URL: {url}')
+            subscraper.save_artwork_information()
 ```
 
-Be careful with bash scripts like these and makes sure you are in the right
-directory.
 
 ## Contributing
 
 Contributions are what make the open source community an amazing place
 to learn, inspire, and create. Any contributions you make are **greatly
 appreciated**.
 
@@ -184,15 +145,15 @@
 [CONTRIBUTING](https://github.com/sodascience/artscraper/blob/main/CONTRIBUTING.md)
 file for more information on issues and pull requests.
 
 ## License and citation
 
 The package `artscraper` is published under an MIT license. When using `artscraper` for academic work, please cite:
 
-    Schram, Raoul, Garcia-Bernardo, Javier, van Kesteren, Erik-Jan, de Bruin, Jonathan, & Stamkou, Eftychia. (2022). 
+    Schram, Raoul, Mitra, Modhurita, Garcia-Bernardo, Javier, van Kesteren, Erik-Jan, de Bruin, Jonathan, & Stamkou, Eftychia. (2022). 
     ArtScraper: A Python library to scrape online artworks (0.1.1). Zenodo. https://doi.org/10.5281/zenodo.7129975
 
 
 ## Contact
 
 This project is developed and maintained by the [ODISSEI Social Data
 Science (SoDa)](https://odissei-data.nl/nl/soda/) team.
```

### Comparing `artscraper-0.2.0/artscraper/base.py` & `artscraper-0.3.1/artscraper/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,17 @@
         """
         if meta_fp is None:
             meta_fp = self.meta_fp
         if meta_fp.is_file():
             return
         metadata = self.get_metadata()
         self.paint_dir.mkdir(exist_ok=True)
-        with open(meta_fp, "w", encoding="utf-8") as f:  # pylint: disable=invalid-name
-            json.dump(metadata, f)
+        with open(meta_fp, "w", encoding='utf-8') as f:
+            # pylint: disable=invalid-name
+            json.dump(metadata, f, ensure_ascii=False)
 
     @abstractmethod
     def save_image(self, img_fp=None, link=None):
         """Abstract method to save the image to a file.
 
         Arguments
         ---------
```

### Comparing `artscraper-0.2.0/artscraper/find_artists.py` & `artscraper-0.3.1/artscraper/find_artists.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 '''
 Get artist links from Google Arts & Culture webpage
 '''
 
 import time
+
 from selenium import webdriver
+from selenium.webdriver.firefox.service import Service as FirefoxService
+from webdriver_manager.firefox import GeckoDriverManager
+
 from artscraper.functions import random_wait_time
 
 def get_artist_links(webpage='https://artsandculture.google.com/category/artist',
-                     executable_path='geckodriver',
                      min_wait_time=5, output_file=None):
     '''
     Parameters
     ----------
     webpage : Web address of Google Arts & Culture artists page
     executable_path: Path to geckodriver
     output_file: File to which the list of links is to be written
 
     Returns
     -------
     list_links : List with Google Arts & Culture web addresses for all artists
     '''
 
     # Launch Firefox browser
-    driver = webdriver.Firefox(executable_path=executable_path)
-
-    # Get Google Arts & Culture webpage listing all artists
-    driver.get(webpage)
-
-    # Get scroll height after first time page load
-    last_height = driver.execute_script("return document.body.scrollHeight")
-    while True:
-        # Scroll down to bottom
-        driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
-        # Wait to load page
-        time.sleep(random_wait_time(min_wait=min_wait_time))
-        # Calculate new scroll height and compare with last scroll height
-        new_height = driver.execute_script("return document.body.scrollHeight")
-        if new_height == last_height:
-            break
-        last_height = new_height
-
-    # Find xpaths containing artist links
-    elements = driver.find_elements('xpath', '//*[contains(@href,"categoryId=artist")]')
-
-    # List to store artist links
-    list_links = []
-    # Go through each xpath containing an artist link
-    for element in elements:
-        # Extract link to webpage
-        link = element.get_attribute('href')
-        # Remove trailing text
-        link = link.replace('?categoryId=artist', '')
-        # Append to list
-        list_links.append(link)
+    with webdriver.Firefox(service=FirefoxService(GeckoDriverManager().install())) as driver:
+        # Get Google Arts & Culture webpage listing all artists
+        driver.get(webpage)
+
+        # Get scroll height after first time page load
+        last_height = driver.execute_script("return document.body.scrollHeight")
+        while True:
+            # Scroll down to bottom
+            driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
+            # Wait to load page
+            time.sleep(random_wait_time(min_wait=min_wait_time))
+            # Calculate new scroll height and compare with last scroll height
+            new_height = driver.execute_script("return document.body.scrollHeight")
+            if new_height == last_height:
+                break
+            last_height = new_height
+
+        # Find xpaths containing artist links
+        elements = driver.find_elements('xpath', '//*[contains(@href,"categoryId=artist")]')
+
+        # List to store artist links
+        list_links = []
+        # Go through each xpath containing an artist link
+        for element in elements:
+            # Extract link to webpage
+            link = element.get_attribute('href')
+            # Remove trailing text
+            link = link.replace('?categoryId=artist', '')
+            # Append to list
+            list_links.append(link)
 
-    # Close driver
-    driver.close()
 
     if output_file:
         with open(output_file, 'w', encoding='utf-8') as file:
             for link in list_links:
                 file.write(link)
                 file.write('\n')
```

### Comparing `artscraper-0.2.0/artscraper/find_artworks.py` & `artscraper-0.3.1/artscraper/find_artworks.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,42 +3,45 @@
 
 get_artist_works: Get links to the artist's works, from Google Arts & Culture webpage
 get_artist_description: Get description of the artist, from Wikipedia
 get_artist_metadata: Get metadata of the artist, from Wikidata
 
 '''
 
-# Allow __init__ function to have more than 5 arguments
-#pylint: disable-msg=too-many-arguments
-
 from pathlib import Path
 
 import time
 import re
+from urllib.parse import urlparse
+from urllib.parse import unquote
+import json
 import requests
 
 from selenium import webdriver
+from selenium.webdriver.firefox.service import Service as FirefoxService
+from webdriver_manager.firefox import GeckoDriverManager
 
 import wikipediaapi
 
 from artscraper.functions import random_wait_time
 
 class FindArtworks:
     '''
     Class for finding artworks and metadata for an artist,
     given the link to their Google Arts & Culture webpage
-    '''
+    unquote   '''
 
-    def __init__(self, artist_link, executable_path='geckodriver',
+    # Allow __init__ function to have more than 5 arguments
+    # pylint: disable-msg=too-many-arguments
+
+    def __init__(self, artist_link,
                  output_dir='./data', sparql_query= None, min_wait_time=5):
 
         # Link to artist's Google Arts & Culture webpage
         self.artist_link = artist_link
-        # Path to geckodriver
-        self.executable_path = executable_path
         # Directory to which the data is to be written
         # Create it if it doesn't exist
         Path(output_dir).mkdir(parents=True, exist_ok=True)
         # Directory to which the data is to be written
         self.output_dir = output_dir
         # Minimum wait time between two clicks while scrolling a webpage
         self.min_wait_time = min_wait_time
@@ -46,65 +49,69 @@
         # SPARQL query to fetch metadata from wikidata
         if sparql_query is None:
             # Default SPARQL query
             self.sparql_query = '''
                 SELECT
                 ?familyName ?familyNameLabel
                 ?givenName ?givenNameLabel
+                ?pseudonym ?pseudonymLabel
                 ?sexOrGender ?sexOrGenderLabel
                 ?dateOfBirth ?dateOfBirthLabel
                 ?placeOfBirth ?placeOfBirthLabel
                 ?latitudeOfPlaceOfBirth ?latitudeOfPlaceOfBirthLabel
                 ?longitudeOfPlaceOfBirth ?longitudeOfPlaceOfBirthLabel
                 ?dateOfDeath ?dateOfDeathLabel
                 ?placeOfDeath ?placeOfDeathLabel
                 ?latitudeOfPlaceOfDeath ?latitudeOfPlaceOfDeathLabel
                 ?longitudeOfPlaceOfDeath ?longitudeOfPlaceOfDeathLabel
                 ?countryOfCitizenship ?countryOfCitizenshipLabel
                 ?residence ?residenceLabel
                 ?workLocation ?workLocationLabel
                 ?genre ?genreLabel
                 ?movement ?movementLabel
+                ?occupation ?occupationLabel
                 WHERE {
                   OPTIONAL { wd:person_id wdt:P734 ?familyName. }
                   OPTIONAL { wd:person_id wdt:P735 ?givenName. }
+                  OPTIONAL { wd:person_id wdt:P742 ?pseudonym. }
                   OPTIONAL { wd:person_id wdt:P21 ?sexOrGender. }
                   OPTIONAL {
                       wd:person_id wdt:P569 ?dateTimeOfBirth.
                       BIND (xsd:date(?dateTimeOfBirth) AS ?dateOfBirth)
                   }
-                  OPTIONAL { wd:person_id wdt:P19 ?placeOfBirth. }
                   OPTIONAL {
-                    ?placeOfBirth wdt:P625 ?coordinatesBirth.
-                    BIND(geof:latitude(?coordinatesBirth) AS ?latitudeOfPlaceOfBirth)
-                    BIND(geof:longitude(?coordinatesBirth) AS ?longitudeOfPlaceOfBirth)
+                      wd:person_id wdt:P19 ?placeOfBirth.
+                      ?placeOfBirth wdt:P625 ?coordinatesBirth.
+                      BIND(geof:latitude(?coordinatesBirth) AS ?latitudeOfPlaceOfBirth)
+                      BIND(geof:longitude(?coordinatesBirth) AS ?longitudeOfPlaceOfBirth)
                   }
                   OPTIONAL {
-                      wd:person_id wdt:P569 ?dateTimeOfDeath.
+                      wd:person_id wdt:P570 ?dateTimeOfDeath.
                       BIND (xsd:date(?dateTimeOfDeath) AS ?dateOfDeath)
                   }
-                  OPTIONAL { wd:person_id wdt:P20 ?placeOfDeath. }
                   OPTIONAL {
-                    ?placeOfDeath wdt:P625 ?coordinatesDeath.
-                    BIND(geof:latitude(?coordinatesDeath) AS ?latitudeOfPlaceOfDeath)
-                    BIND(geof:longitude(?coordinatesDeath) AS ?longitudeOfPlaceOfDeath)
+                      wd:person_id wdt:P20 ?placeOfDeath.
+                      ?placeOfDeath wdt:P625 ?coordinatesDeath.
+                      BIND(geof:latitude(?coordinatesDeath) AS ?latitudeOfPlaceOfDeath)
+                      BIND(geof:longitude(?coordinatesDeath) AS ?longitudeOfPlaceOfDeath)
                   }
                   OPTIONAL { wd:person_id wdt:P27 ?countryOfCitizenship. }
                   OPTIONAL { wd:person_id wdt:P551 ?residence. }
                   OPTIONAL { wd:person_id wdt:P937 ?workLocation. }
                   OPTIONAL { wd:person_id wdt:P136 ?genre. }
                   OPTIONAL { wd:person_id wdt:P135 ?movement. }
+                  OPTIONAL { wd:person_id wdt:P106 ?occupation. }
                   SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
                 }
                 '''
         else:
             self.sparql_query = sparql_query
 
         # Open web browser
-        self.driver = webdriver.Firefox(executable_path=self.executable_path)
+        self.driver = webdriver.Firefox(service=FirefoxService(GeckoDriverManager().install()))
 
 
     def __enter__(self):
         return self
 
 
     def __exit__(self, _exc_type, _exc_val, _exc_tb):
@@ -132,35 +139,61 @@
 
         '''
         Save information (artist_works, artist_description, artist_metadata) about the artist
 
         '''
 
         artist_works, artist_description, artist_metadata = self.get_artist_information()
-        artist_name = self.get_wikipedia_article_title()
-
+        artist_name = self.get_artist_name()
         # Create directory for artist
         pathname_directory = self.output_dir + '/' + artist_name
         Path(pathname_directory).mkdir(parents=True, exist_ok=True)
-
         # Filenames for artist's works, description, metadata
         artist_works_file = pathname_directory + '/' + 'works.txt'
         artist_description_file = pathname_directory + '/' + 'description.txt'
-        artist_metadata_file = pathname_directory + '/' + 'metadata.txt'
-
+        artist_metadata_file = pathname_directory + '/' + 'metadata.json'
         # Save artist's works, description, metadata
         with open(artist_works_file, 'w', encoding='utf-8') as file:
             for link in artist_works:
                 file.write(f'{link}\n')
         with open(artist_description_file, 'w', encoding='utf-8') as file:
-            file.write(artist_description)
+            if artist_description is not None:
+                file.write(artist_description)
         with open(artist_metadata_file, 'w', encoding='utf-8') as file:
-            for key,value in artist_metadata.items():
-                file.write(f'{key} : {value}\n')
+            if artist_metadata is not None:
+                json.dump(artist_metadata, file, ensure_ascii=False)
+
+
+    def get_artist_name(self):
+
+        '''
+        Return artist's name, with parts thereof being separated by underscores
+        '''
+
+        # Artist link
+        artist_link = self.artist_link
+
+        # Split the link by forward slashes
+        parts = artist_link.split('/')
+        # Extract the artist's name (separated by dashes)
+        artist_name_string = parts[4]
+        artist_name_string = unquote(artist_name_string)
 
+        # Split the artist's name into component parts
+        artist_name_parts = artist_name_string.split('-')
+        # Capitalize each component
+        artist_name_capitalized_parts = []
+        for part in artist_name_parts:
+            part = part.capitalize()
+            artist_name_capitalized_parts.append(part)
+
+        # Artist's name, separated by underscores
+        artist_name = ('_').join(artist_name_capitalized_parts)
+
+        return artist_name
 
     def get_artist_works(self):
 
         '''
         Returns
         -------
         list_links: List with web addresses of the artist's works on Google Arts & Culture
@@ -172,34 +205,91 @@
 
         # Locate the section on the page containing the artworks, by searching for the text heading
         element = self.driver.find_element('xpath', '//*[contains(text(), "Discover this artist")]')
 
         # Find the parent element corresponding to the text heading
         parent_element = element.find_element('xpath', '../..')
 
-        # Find right arrow button
-        right_arrow_element = parent_element.find_element('xpath', \
-            './/*[contains(@data-gaaction,"rightArrow")]')
+        # Initialize total number of artworks
+        # (set to number of artworks by artist with the most artworks)
+        total_num_artworks = 200000
+
+        # Find number of artists
+        # Find elements with tag name 'h3'
+        items_elements = parent_element.find_elements('tag name', 'h3')
+        for element in items_elements:
+            if 'items' in element.text:
+                match = re.search(r'\d+', element.text)
+                if match:
+                    total_num_artworks = int(match.group())
+                    break
+
+        # Find right arrow element
+        def _find_right_arrow_element(parent_element):
+
+            right_arrow_element = parent_element.find_element('xpath', \
+                './/*[contains(@data-gaaction,"rightArrow")]')
+
+            return right_arrow_element
+
+        # Get list of artwork links
+        def _get_list_links(parent_element):
+
+            # Find right arrow button
+            right_arrow_element = parent_element.find_element('xpath', \
+                './/*[contains(@data-gaaction,"rightArrow")]')
+
+            # List of all elements with links to artworks
+            elements = right_arrow_element.find_elements('xpath', \
+                '//*[contains(@href,"/asset/")]')
+
+            # Get the links from the XPath elements
+            list_links = [element.get_attribute('href') for element in elements]
+
+            return list_links
+
+        # Click on right arrow
+        def _click_on_right_arrow(parent_element):
 
-        # Check if right arrow button can still be clicked
-        while right_arrow_element.get_attribute('tabindex') is not None:
             # Find right arrow button
             right_arrow_element = parent_element.find_element('xpath', \
                 './/*[contains(@data-gaaction,"rightArrow")]')
             # Click on right arrow button
             self.driver.execute_script("arguments[0].click();", right_arrow_element)
-            # Wait for page to load
-            time.sleep(random_wait_time(min_wait=self.min_wait_time))
 
-        # List of all elements with links to artworks
-        elements = right_arrow_element.find_elements('xpath', \
-                '//*[contains(@href,"/asset/")]')
+        list_links = _get_list_links(parent_element)
+
+        # Initialize count of number of iterations for which the number of artworks remains the same
+        n_tries = 0
+
+        while (len(list_links) < total_num_artworks and n_tries < 3):
+
+            # Save current number of artworks
+            old_num_artworks = len(list_links)
+
+            # Find right arrow element
+            right_arrow_element =  _find_right_arrow_element(parent_element)
+
+            # Check if right arrow button can still be clicked
+            if right_arrow_element.get_attribute('tabindex') is not None:
+
+                # Click on right arrow
+                _click_on_right_arrow(parent_element)
+
+                # Wait for page to load
+                time.sleep(random_wait_time(min_wait=self.min_wait_time))
+
+                # Obtain new list of artworks
+                list_links = _get_list_links(parent_element)
 
-        # Get the links from the XPath elements
-        list_links = [element.get_attribute('href') for element in elements]
+            if len(list_links) == old_num_artworks:
+                # Count number of iterations for which the number of artworks remains the same
+                n_tries = n_tries + 1
+            else:
+                n_tries = 0
 
         return list_links
 
 
     def get_artist_description(self):
 
         '''
@@ -207,43 +297,60 @@
         -------
         description : String containing description of artist (lead section of Wikipedia article)
 
         '''
 
         # Get title of artist's Wikipedia article
         title = self.get_wikipedia_article_title()
-        # Choose the English Wikipedia
-        wiki = wikipediaapi.Wikipedia('en')
+
+        # Return None if no Wikipedia article exists
+        if title is None:
+            return None
+
+        # Get link to Wikipedia article
+        wikipedia_article_link = self.get_wikipedia_article_link()
+        # Parse the URL
+        parsed_url = urlparse(wikipedia_article_link)
+        # Find the language of the Wikipedia article
+        language_code = parsed_url.netloc.split('.')[0]
+
+        # Choose the Wikipedia corresponding to the language code
+        wiki = wikipediaapi.Wikipedia(language_code)
         # Get the Wikipedia page
         page = wiki.page(title)
         # Get summary of the page (lead section of the Wikipedia article)
         description = page.summary
 
+        description = unquote(description)
+
         return description
 
     def get_artist_metadata(self):
 
         '''
         Returns
         -------
         metadata: Dictionary containing metadata about the artist
 
         '''
 
         # Get Wikidata ID of artist
         artist_id = self.get_artist_wikidata_id()
+        if artist_id is None:
+            return None
 
         # Wikidata database to query
         url = 'https://query.wikidata.org/sparql'
 
         # Replace person_id in SPARQL query with the wikidata ID of the artist
         query = self.sparql_query.replace('person_id', artist_id)
 
         # Send query request
-        request = requests.get(url, params= {'format': 'json', 'query': ''.join(query)}, timeout=30)
+        request = requests.get(url, params={'format': 'json', \
+                            'query': ''.join(query)}, timeout=120)
 
         # Convert response to dictionary
         data = request.json()
 
         # Extract properties searched by the SPARQL query
         properties_query = re.findall(r"\?[^\s]*Label\b", self.sparql_query)
 
@@ -265,17 +372,22 @@
         -------
         wikipedia_link : Web address of the artist's Wikipedia article'
 
         '''
 
         # Get Google Arts & Culture webpage for the artist
         self.driver.get(self.artist_link)
+        # Allow bare-except
+        # pylint: disable=W0702
+        try:
+            # Locate the element containing the link to the artist's Wikipedia article
+            element = self.driver.find_element('xpath','//*[contains(@href,"wikipedia")]')
+        except:
+            return None
 
-        # Locate the element containing the link to the artist's Wikipedia article
-        element = self.driver.find_element('xpath','//*[contains(@href,"wikipedia")]')
         # Extract the link to the Wikipedia article
         wikipedia_link = element.get_attribute('href')
 
         return wikipedia_link
 
     def get_wikipedia_article_title(self):
 
@@ -285,45 +397,49 @@
         title : String containing the title of the artist's Wikipedia article
 
         '''
 
         # Get the link to the artist's Wikipedia article
         wikipedia_link = self.get_wikipedia_article_link()
 
-        # Get title of artist's Wikipedia article
-        title = wikipedia_link.rsplit('/')[-1]
+        if wikipedia_link is not None:
+            # Get title of artist's Wikipedia article
+            title = wikipedia_link.rsplit('/')[-1]
+            title = unquote(title)
+            return title
 
-        return title
+        return None
 
     def get_artist_wikidata_id(self):
 
         '''
         Returns
         -------
         wikidata_id: Wikidata ID of the artist
         '''
 
-        # Get Google Arts & Culture webpage for the artist
-        self.driver.get(self.artist_link)
-
-        # Locate the element containing the link to the artist's Wikipedia article
-        element = self.driver.find_element('xpath','//*[contains(@href,"wikipedia")]')
-        # Extract the link to the Wikipedia article
-        wikipedia_link = element.get_attribute('href')
+        # Get the link to the Wikipedia article
+        wikipedia_link = self.get_wikipedia_article_link()
 
         # Get Wikipedia page for the artist
-        self.driver.get(wikipedia_link)
-        # Find element containing text about Wikidata
-        element = self.driver.find_element('xpath','//*[contains(text(),"Wikidata item")]')
-        # Find parent element of this element
-        parent_element = element.find_element('xpath', '..')
+        if wikipedia_link is not None:
+            self.driver.get(wikipedia_link)
+        else:
+            return None
+
+        # Find element containing the link to the Wikidata page
+        element = self.driver.find_element('xpath','//*[contains(@href,"www.wikidata.org")]')
         # Extract the link to the Wikidata page
-        wikidata_link = parent_element.get_attribute('href')
+        wikidata_link = element.get_attribute('href')
+        # Specify pattern of Wikidata ID
+        pattern = r'Q\d+'
+        # Search for pattern in the Wikidata link
+        match = re.search(pattern, wikidata_link)
         # Find the Wikidata ID of the artist
-        wikidata_id = wikidata_link.rsplit('/')[-1]
+        wikidata_id = match.group(0)
 
         return wikidata_id
 
 
     def _get_property(self, data, query_property):
 
         '''
@@ -336,14 +452,15 @@
         output_property_list : Value(s) of extracted property
         '''
 
         output_property_list = []
         if query_property+'Label' in data['results']['bindings'][0].keys():
             for element in data['results']['bindings']:
                 output_property = element[query_property+'Label']['value']
+                output_property = unquote(output_property)
                 # Avoid duplicates
                 if output_property not in output_property_list:
                     output_property_list.append(output_property)
             if len(output_property_list)==1:
                 output_property_list = output_property_list[0]
             return output_property_list
```

### Comparing `artscraper-0.2.0/artscraper/wikiart.py` & `artscraper-0.3.1/artscraper/wikiart.py`

 * *Files identical despite different names*

### Comparing `artscraper-0.2.0/setup.py` & `artscraper-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
     
 setup(
     name='artscraper',
-    version='0.2.0',
+    version='0.3.1',
     author='ODISSEI Social Data Science Team',
     description='Package for scraping artworks from WikiArt and GoogleArt',
     long_description='See https://github.com/sodascience/artscraper for examples and usage',
     keywords='artscraper wikiart artsandculture',
     license='MIT',
     url='https://github.com/sodascience/artscraper',
     packages=find_packages(exclude=['data', 'docs', 'tests', 'examples']),
     python_requires='~=3.6',
     install_requires=[
         "requests",
         "selenium",
         "beautifulsoup4",
-        "wikipedia-api"
+        "wikipedia-api",
+        "webdriver-manager",
     ]
 )
```

