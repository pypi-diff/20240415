# Comparing `tmp/deezer_downloader-2.0.7.tar.gz` & `tmp/deezer_downloader-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_downloader-2.0.7.tar", max compression
+gzip compressed data, was "deezer_downloader-2.0.8.tar", max compression
```

## Comparing `deezer_downloader-2.0.7.tar` & `deezer_downloader-2.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.7/LICENSE
--rw-r--r--   0        0        0     9283 2023-12-20 22:16:07.508244 deezer_downloader-2.0.7/README.md
--rw-r--r--   0        0        0     1423 2023-12-05 12:49:21.783881 deezer_downloader-2.0.7/deezer_downloader/cli/deezer-downloader.ini.template
--rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.7/deezer_downloader/cli/runner.py
--rw-r--r--   0        0        0     1497 2023-05-01 07:47:26.683606 deezer_downloader-2.0.7/deezer_downloader/configuration.py
--rw-r--r--   0        0        0    20834 2024-03-05 13:13:07.555845 deezer_downloader-2.0.7/deezer_downloader/deezer.py
--rw-r--r--   0        0        0     5031 2023-04-29 16:38:19.755822 deezer_downloader-2.0.7/deezer_downloader/spotify.py
--rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.7/deezer_downloader/threadpool_queue.py
--rw-r--r--   0        0        0    10201 2023-04-10 17:34:44.980270 deezer_downloader-2.0.7/deezer_downloader/web/app.py
--rw-r--r--   0        0        0    11048 2023-04-29 16:16:41.814433 deezer_downloader-2.0.7/deezer_downloader/web/music_backend.py
--rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
--rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/css/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/css/bootstrap.min.css
--rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/css/font-awesome.min.css
--rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/css/jquery.jgrowl.min.css
--rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/favicon.ico
--rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.7/deezer_downloader/web/static/js/bootstrap.min.js
--rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.7/deezer_downloader/web/static/js/custom.js
--rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.7/deezer_downloader/web/static/js/jquery.jgrowl.min.js
--rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.7/deezer_downloader/web/static/js/jquery.min.js
--rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.7/deezer_downloader/web/static/js/popper.min.js
--rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.7/deezer_downloader/web/templates/autoindex.html
--rw-r--r--   0        0        0     8735 2023-04-10 10:27:40.860066 deezer_downloader-2.0.7/deezer_downloader/web/templates/index.html
--rw-r--r--   0        0        0     2309 2023-04-29 15:45:57.946045 deezer_downloader-2.0.7/deezer_downloader/youtubedl.py
--rw-r--r--   0        0        0      977 2024-03-05 13:23:49.691019 deezer_downloader-2.0.7/pyproject.toml
--rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 deezer_downloader-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-09 20:20:53.021110 deezer_downloader-2.0.8/LICENSE
+-rw-r--r--   0        0        0     9423 2024-03-17 16:29:53.492476 deezer_downloader-2.0.8/README.md
+-rw-r--r--   0        0        0     1423 2023-12-05 12:49:21.783881 deezer_downloader-2.0.8/deezer_downloader/cli/deezer-downloader.ini.template
+-rw-r--r--   0        0        0     1738 2023-04-09 20:56:59.983157 deezer_downloader-2.0.8/deezer_downloader/cli/runner.py
+-rw-r--r--   0        0        0     1497 2023-05-01 07:47:26.683606 deezer_downloader-2.0.8/deezer_downloader/configuration.py
+-rw-r--r--   0        0        0    20834 2024-03-05 13:13:07.555845 deezer_downloader-2.0.8/deezer_downloader/deezer.py
+-rw-r--r--   0        0        0     5031 2023-04-29 16:38:19.755822 deezer_downloader-2.0.8/deezer_downloader/spotify.py
+-rw-r--r--   0        0        0     3382 2023-04-09 20:20:53.021110 deezer_downloader-2.0.8/deezer_downloader/threadpool_queue.py
+-rw-r--r--   0        0        0    10201 2023-04-10 17:34:44.980270 deezer_downloader-2.0.8/deezer_downloader/web/app.py
+-rw-r--r--   0        0        0    11048 2023-04-29 16:16:41.814433 deezer_downloader-2.0.8/deezer_downloader/web/music_backend.py
+-rw-r--r--   0        0        0   623500 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip
+-rw-r--r--   0        0        0    70682 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/css/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   155758 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0    31000 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/css/font-awesome.min.css
+-rw-r--r--   0        0        0     1515 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/css/jquery.jgrowl.min.css
+-rw-r--r--   0        0        0      327 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/favicon.ico
+-rw-r--r--   0        0        0    77160 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    58072 2023-04-09 20:20:53.024443 deezer_downloader-2.0.8/deezer_downloader/web/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0    11064 2023-04-09 20:20:53.027777 deezer_downloader-2.0.8/deezer_downloader/web/static/js/custom.js
+-rw-r--r--   0        0        0     5476 2023-04-09 20:20:53.027777 deezer_downloader-2.0.8/deezer_downloader/web/static/js/jquery.jgrowl.min.js
+-rw-r--r--   0        0        0    89795 2023-04-09 20:20:53.027777 deezer_downloader-2.0.8/deezer_downloader/web/static/js/jquery.min.js
+-rw-r--r--   0        0        0    21004 2023-04-09 20:20:53.027777 deezer_downloader-2.0.8/deezer_downloader/web/static/js/popper.min.js
+-rw-r--r--   0        0        0      194 2023-04-09 20:20:53.027777 deezer_downloader-2.0.8/deezer_downloader/web/templates/autoindex.html
+-rw-r--r--   0        0        0     8735 2023-04-10 10:27:40.860066 deezer_downloader-2.0.8/deezer_downloader/web/templates/index.html
+-rw-r--r--   0        0        0     2309 2023-04-29 15:45:57.946045 deezer_downloader-2.0.8/deezer_downloader/youtubedl.py
+-rw-r--r--   0        0        0      977 2024-04-15 10:53:51.640401 deezer_downloader-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10407 1970-01-01 00:00:00.000000 deezer_downloader-2.0.8/PKG-INFO
```

### Comparing `deezer_downloader-2.0.7/LICENSE` & `deezer_downloader-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/README.md` & `deezer_downloader-2.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 ## Music Downloader 🎶 🎧 💃 🦄
 [![tests](https://github.com/kmille/deezer-downloader/actions/workflows/tests.yaml/badge.svg)](https://github.com/kmille/deezer-downloader/actions/workflows/tests.yaml)
 ![latest tag](https://img.shields.io/github/v/tag/kmille/deezer-downloader?sort=semver) ![Python 3.6](https://img.shields.io/badge/python-%3E=3.6-blue.svg) ![pypi-version](https://img.shields.io/pypi/v/deezer-downloader) ![pypi-downloads](https://img.shields.io/pypi/dm/deezer-downloader)
 
-
-
 ### Features
 
 - download songs, albums, public playlists from Deezer.com (account is required, free plan is enough)
 - download Spotify playlists (by parsing the Spotify website and download the songs from Deezer)
 - download as zip file (including m3u8 playlist file)
-- 320 kbit/s mp3s with ID3-Tags and album cover (UPDATE: right now only 128bkit/s mp3 works, see #66)
+- ~~320 kbit/s~~ (currently only 128 kbit/s, see [this issue](https://github.com/kmille/deezer-downloader/issues/66#issuecomment-2002309521)) mp3s with ID3-Tags and album cover
 - download songs via yt-dlp
 - KISS (keep it simple and stupid) front end
 - MPD integration (use it on a Raspberry Pi!)
 - simple REST api
 - proxy support (https/socks5)
 
 
 ### How to use it
 
 There is a settings file template called `settings.ini.example`. You can specify the download directory with  `download_dir`. Pressing the download button only downloads the song/album/playlist. If you set `use_mpd=True` in the `settings.ini` the backend will connect to mpd (localhost:6600) and update the music database. Pressing the play button will download the music. If `use_mpd=True`  is set the mpd database will be updated and the song/album/playlist will be added to the playlist. In `settings.ini` `music_dir` should be the music root location of mpd. The `download_dir` must be a subdirectory of `music_dir`. 
 
-As Deezer sometimes requires a captcha to login the auto login features was removed. Instead you have to manually insert a valid Deezer cookie to the `settings.ini`. The relevant cookie is the `arl` cookie. 
+As Deezer sometimes requires a captcha to login the auto login features was removed. Instead you have to manually insert a valid Deezer cookie to the `settings.ini`. The relevant cookie is the `arl` cookie. **Important: The ARL cookie must be of a non-premium account!**
 
 ```bash
 kmille@linbox:deezer-downloader poetry run deezer-downloader --help
 usage: deezer-downloader [-h] [-v] [-t] [-c CONFIG]
 
 Download music from Deezer with a nice front end
 
@@ -55,15 +53,15 @@
 
 
 ### How to get it up and running
 #### with pip
 You can run `pip install --user deezer-downloader`. Then you can run `~/.local/bin/deezer-downloader --help`
 
 #### with Docker
-You can use the Docker image hosted on [hub.docker.com](https://hub.docker.com/r/kmille2/deezer-downloader). Login into your free Deezer account and grab the `arl` cookie. Then:
+You can use the Docker image hosted on [hub.docker.com](https://hub.docker.com/r/kmille2/deezer-downloader). Login into your **free** Deezer account and grab the `arl` cookie. Then:
 
 ```bash
 mkdir downloads
 sudo docker run -p 5000:5000 --volume $(pwd)/downloads/:/mnt/deezer-downloader --env DEEZER_COOKIE_ARL=changeme kmille2/deezer-downloader:latest 
 xdg-open http://localhost:5000
 ```
```

### Comparing `deezer_downloader-2.0.7/deezer_downloader/cli/deezer-downloader.ini.template` & `deezer_downloader-2.0.8/deezer_downloader/cli/deezer-downloader.ini.template`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/cli/runner.py` & `deezer_downloader-2.0.8/deezer_downloader/cli/runner.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/configuration.py` & `deezer_downloader-2.0.8/deezer_downloader/configuration.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/deezer.py` & `deezer_downloader-2.0.8/deezer_downloader/deezer.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/spotify.py` & `deezer_downloader-2.0.8/deezer_downloader/spotify.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/threadpool_queue.py` & `deezer_downloader-2.0.8/deezer_downloader/threadpool_queue.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/app.py` & `deezer_downloader-2.0.8/deezer_downloader/web/app.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/music_backend.py` & `deezer_downloader-2.0.8/deezer_downloader/web/music_backend.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip` & `deezer_downloader-2.0.8/deezer_downloader/web/static/css/bootstrap-4.1.3-dist.zip`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/css/bootstrap.bundle.min.js` & `deezer_downloader-2.0.8/deezer_downloader/web/static/css/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/css/bootstrap.min.css` & `deezer_downloader-2.0.8/deezer_downloader/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/css/font-awesome.min.css` & `deezer_downloader-2.0.8/deezer_downloader/web/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/css/jquery.jgrowl.min.css` & `deezer_downloader-2.0.8/deezer_downloader/web/static/css/jquery.jgrowl.min.css`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2` & `deezer_downloader-2.0.8/deezer_downloader/web/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/js/bootstrap.min.js` & `deezer_downloader-2.0.8/deezer_downloader/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/js/custom.js` & `deezer_downloader-2.0.8/deezer_downloader/web/static/js/custom.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/js/jquery.jgrowl.min.js` & `deezer_downloader-2.0.8/deezer_downloader/web/static/js/jquery.jgrowl.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/js/jquery.min.js` & `deezer_downloader-2.0.8/deezer_downloader/web/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/static/js/popper.min.js` & `deezer_downloader-2.0.8/deezer_downloader/web/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/web/templates/index.html` & `deezer_downloader-2.0.8/deezer_downloader/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/deezer_downloader/youtubedl.py` & `deezer_downloader-2.0.8/deezer_downloader/youtubedl.py`

 * *Files identical despite different names*

### Comparing `deezer_downloader-2.0.7/pyproject.toml` & `deezer_downloader-2.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-downloader"
-version = "2.0.7"
+version = "2.0.8"
 description = "download music from Deezer with a nice front end"
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "deezer_downloader"}]
 repository = "https://github.com/kmille/deezer-downloader"
 homepage = "https://github.com/kmille/deezer-downloader"
```

### Comparing `deezer_downloader-2.0.7/PKG-INFO` & `deezer_downloader-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deezer-downloader
-Version: 2.0.7
+Version: 2.0.8
 Summary: download music from Deezer with a nice front end
 Home-page: https://github.com/kmille/deezer-downloader
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,34 +23,32 @@
 Project-URL: Repository, https://github.com/kmille/deezer-downloader
 Description-Content-Type: text/markdown
 
 ## Music Downloader 🎶 🎧 💃 🦄
 [![tests](https://github.com/kmille/deezer-downloader/actions/workflows/tests.yaml/badge.svg)](https://github.com/kmille/deezer-downloader/actions/workflows/tests.yaml)
 ![latest tag](https://img.shields.io/github/v/tag/kmille/deezer-downloader?sort=semver) ![Python 3.6](https://img.shields.io/badge/python-%3E=3.6-blue.svg) ![pypi-version](https://img.shields.io/pypi/v/deezer-downloader) ![pypi-downloads](https://img.shields.io/pypi/dm/deezer-downloader)
 
-
-
 ### Features
 
 - download songs, albums, public playlists from Deezer.com (account is required, free plan is enough)
 - download Spotify playlists (by parsing the Spotify website and download the songs from Deezer)
 - download as zip file (including m3u8 playlist file)
-- 320 kbit/s mp3s with ID3-Tags and album cover (UPDATE: right now only 128bkit/s mp3 works, see #66)
+- ~~320 kbit/s~~ (currently only 128 kbit/s, see [this issue](https://github.com/kmille/deezer-downloader/issues/66#issuecomment-2002309521)) mp3s with ID3-Tags and album cover
 - download songs via yt-dlp
 - KISS (keep it simple and stupid) front end
 - MPD integration (use it on a Raspberry Pi!)
 - simple REST api
 - proxy support (https/socks5)
 
 
 ### How to use it
 
 There is a settings file template called `settings.ini.example`. You can specify the download directory with  `download_dir`. Pressing the download button only downloads the song/album/playlist. If you set `use_mpd=True` in the `settings.ini` the backend will connect to mpd (localhost:6600) and update the music database. Pressing the play button will download the music. If `use_mpd=True`  is set the mpd database will be updated and the song/album/playlist will be added to the playlist. In `settings.ini` `music_dir` should be the music root location of mpd. The `download_dir` must be a subdirectory of `music_dir`. 
 
-As Deezer sometimes requires a captcha to login the auto login features was removed. Instead you have to manually insert a valid Deezer cookie to the `settings.ini`. The relevant cookie is the `arl` cookie. 
+As Deezer sometimes requires a captcha to login the auto login features was removed. Instead you have to manually insert a valid Deezer cookie to the `settings.ini`. The relevant cookie is the `arl` cookie. **Important: The ARL cookie must be of a non-premium account!**
 
 ```bash
 kmille@linbox:deezer-downloader poetry run deezer-downloader --help
 usage: deezer-downloader [-h] [-v] [-t] [-c CONFIG]
 
 Download music from Deezer with a nice front end
 
@@ -80,15 +78,15 @@
 
 
 ### How to get it up and running
 #### with pip
 You can run `pip install --user deezer-downloader`. Then you can run `~/.local/bin/deezer-downloader --help`
 
 #### with Docker
-You can use the Docker image hosted on [hub.docker.com](https://hub.docker.com/r/kmille2/deezer-downloader). Login into your free Deezer account and grab the `arl` cookie. Then:
+You can use the Docker image hosted on [hub.docker.com](https://hub.docker.com/r/kmille2/deezer-downloader). Login into your **free** Deezer account and grab the `arl` cookie. Then:
 
 ```bash
 mkdir downloads
 sudo docker run -p 5000:5000 --volume $(pwd)/downloads/:/mnt/deezer-downloader --env DEEZER_COOKIE_ARL=changeme kmille2/deezer-downloader:latest 
 xdg-open http://localhost:5000
 ```
```

