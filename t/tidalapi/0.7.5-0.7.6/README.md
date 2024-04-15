# Comparing `tmp/tidalapi-0.7.5.tar.gz` & `tmp/tidalapi-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidalapi-0.7.5.tar", max compression
+gzip compressed data, was "tidalapi-0.7.6.tar", max compression
```

## Comparing `tidalapi-0.7.5.tar` & `tidalapi-0.7.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     7134 2024-03-01 23:34:43.165755 tidalapi-0.7.5/HISTORY.rst
--rw-r--r--   0        0        0     7651 2023-05-21 21:11:51.414585 tidalapi-0.7.5/LICENSE
--rw-r--r--   0        0        0     1031 2024-02-29 21:48:37.241858 tidalapi-0.7.5/README.rst
--rw-r--r--   0        0        0     1605 2024-02-29 20:56:20.813312 tidalapi-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      639 2024-02-20 21:04:43.647386 tidalapi-0.7.5/tidalapi/__init__.py
--rw-r--r--   0        0        0    11879 2024-02-29 20:03:52.950514 tidalapi-0.7.5/tidalapi/album.py
--rw-r--r--   0        0        0     9403 2024-02-29 19:53:37.085762 tidalapi-0.7.5/tidalapi/artist.py
--rw-r--r--   0        0        0      476 2024-02-29 18:29:10.719189 tidalapi-0.7.5/tidalapi/exceptions.py
--rw-r--r--   0        0        0     2833 2024-02-28 21:50:59.760790 tidalapi-0.7.5/tidalapi/genre.py
--rw-r--r--   0        0        0    28341 2024-02-29 20:03:52.450513 tidalapi-0.7.5/tidalapi/media.py
--rw-r--r--   0        0        0     9480 2024-03-01 19:30:14.696611 tidalapi-0.7.5/tidalapi/mix.py
--rw-r--r--   0        0        0    13926 2024-02-28 20:27:10.490674 tidalapi-0.7.5/tidalapi/page.py
--rw-r--r--   0        0        0    10971 2024-03-01 23:02:56.287584 tidalapi-0.7.5/tidalapi/playlist.py
--rw-r--r--   0        0        0     8508 2024-02-29 22:00:15.174912 tidalapi-0.7.5/tidalapi/request.py
--rw-r--r--   0        0        0    39253 2024-02-29 22:39:11.189544 tidalapi-0.7.5/tidalapi/session.py
--rw-r--r--   0        0        0      127 2024-01-28 13:24:55.354259 tidalapi-0.7.5/tidalapi/types.py
--rw-r--r--   0        0        0    14687 2024-02-28 18:38:57.564864 tidalapi-0.7.5/tidalapi/user.py
--rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 tidalapi-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     7411 2024-04-15 17:13:23.762864 tidalapi-0.7.6/HISTORY.rst
+-rw-r--r--   0        0        0     7651 2023-05-21 21:11:51.414585 tidalapi-0.7.6/LICENSE
+-rw-r--r--   0        0        0     1031 2024-02-29 21:48:37.241858 tidalapi-0.7.6/README.rst
+-rw-r--r--   0        0        0     1610 2024-04-15 17:13:23.734864 tidalapi-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      639 2024-04-15 17:13:23.734864 tidalapi-0.7.6/tidalapi/__init__.py
+-rw-r--r--   0        0        0    11879 2024-04-15 17:13:53.398951 tidalapi-0.7.6/tidalapi/album.py
+-rw-r--r--   0        0        0    10128 2024-04-08 19:44:24.168437 tidalapi-0.7.6/tidalapi/artist.py
+-rw-r--r--   0        0        0      476 2024-02-29 18:29:10.719189 tidalapi-0.7.6/tidalapi/exceptions.py
+-rw-r--r--   0        0        0     2833 2024-02-28 21:50:59.760790 tidalapi-0.7.6/tidalapi/genre.py
+-rw-r--r--   0        0        0    28953 2024-04-08 19:39:35.354927 tidalapi-0.7.6/tidalapi/media.py
+-rw-r--r--   0        0        0     9480 2024-03-01 19:30:14.696611 tidalapi-0.7.6/tidalapi/mix.py
+-rw-r--r--   0        0        0    13926 2024-02-28 20:27:10.490674 tidalapi-0.7.6/tidalapi/page.py
+-rw-r--r--   0        0        0    10971 2024-03-01 23:02:56.287584 tidalapi-0.7.6/tidalapi/playlist.py
+-rw-r--r--   0        0        0     8508 2024-02-29 22:00:15.174912 tidalapi-0.7.6/tidalapi/request.py
+-rw-r--r--   0        0        0    39506 2024-04-15 17:15:23.983392 tidalapi-0.7.6/tidalapi/session.py
+-rw-r--r--   0        0        0      127 2024-01-28 13:24:55.354259 tidalapi-0.7.6/tidalapi/types.py
+-rw-r--r--   0        0        0    14687 2024-02-28 18:38:57.564864 tidalapi-0.7.6/tidalapi/user.py
+-rw-r--r--   0        0        0     9788 1970-01-01 00:00:00.000000 tidalapi-0.7.6/PKG-INFO
```

### Comparing `tidalapi-0.7.5/HISTORY.rst` & `tidalapi-0.7.6/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 =======
 
+v0.7.6
+------
+* Fix: Set token type correctly for OAuth/PKCE authentication - tehkillerbee_
+* Revert to using enums with str support for relevant classes - tehkillerbee_, exislow_
+* Removed return types from method names for consistency, added deprecation warnings - exislow_
+
 v0.7.5
 ------
 * Fix: Use wide image when no square picture is available. - tehkillerbee_
 * Feat.: Added HiRes page. - tehkillerbee_
 * Feat.: Handle missing Stream fields gracefully. Get stream audio resolution (bit depth, rate) as tuple. - tehkillerbee_
 * Feat.: Added misc helper functions for audio mode, get available audio mode for media. - tehkillerbee_
 * Feat.: Added misc. fields to album. Get audio resolution for album + individual tracks. - tehkillerbee_
```

### Comparing `tidalapi-0.7.5/LICENSE` & `tidalapi-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/README.rst` & `tidalapi-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/pyproject.toml` & `tidalapi-0.7.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tidalapi"
-version = "0.7.5"
+version = "0.7.6"
 description = "Unofficial API for TIDAL music streaming service."
 authors = ["Thomas Amland <thomas.amland@googlemail.com>"]
 maintainers = ["tehkillerbee <tehkillerbee@users.noreply.github.com>"]
 license = "LGPL-3.0-or-later"
 readme = ["README.rst", "HISTORY.rst"]
 homepage = "https://tidalapi.netlify.app"
 repository = "https://github.com/tamland/python-tidal"
@@ -34,15 +34,15 @@
 types-requests = "^2.31.0.1"
 types-urllib3 = "^1.26.25.13"
 pytest = "^7.4.0"
 keyring = "^24.2.0"
 pillow = "^10.0.0"
 tox = "^4.6.4"
 ffmpeg-python = "^0.2.0"
-black = "^23.3.0"
+black = ">=23.3,<25.0"
 isort = "^5.12.0"
 ruff = "^0.0.277"
 docformatter = {extras = ["tomli"], version = "^1.7.3"}
 pytest-mock = "^3.11.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `tidalapi-0.7.5/tidalapi/__init__.py` & `tidalapi-0.7.6/tidalapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     Favorites,
     FetchedUser,
     LoggedInUser,
     PlaylistCreator,
     User,
 )
 
-__version__ = "0.7.5"
+__version__ = "0.7.6"
```

### Comparing `tidalapi-0.7.5/tidalapi/album.py` & `tidalapi-0.7.6/tidalapi/album.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/tidalapi/artist.py` & `tidalapi-0.7.6/tidalapi/artist.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """A module containing information and functions related to TIDAL artists."""
 
 import copy
 from datetime import datetime
 from enum import Enum
 from typing import TYPE_CHECKING, List, Mapping, Optional, Union, cast
+from warnings import warn
 
 import dateutil.parser
 from typing_extensions import NoReturn
 
 from tidalapi.exceptions import ObjectNotFound, TooManyRequests
 from tidalapi.types import JsonObj
 
@@ -124,24 +125,44 @@
         """
         params = {"limit": limit, "offset": offset}
         return self._get_albums(params)
 
     def get_albums_ep_singles(
         self, limit: Optional[int] = None, offset: int = 0
     ) -> List["Album"]:
+        warn(
+            "This method is deprecated an will be removed in a future release. Use instead `get_ep_singles`",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+        return self.get_ep_singles(limit=limit, offset=offset)
+
+    def get_ep_singles(
+        self, limit: Optional[int] = None, offset: int = 0
+    ) -> List["Album"]:
         """Queries TIDAL for the artists extended plays and singles.
 
         :return: A list of :class:`Albums <tidalapi.album.Album>`
         """
         params = {"filter": "EPSANDSINGLES", "limit": limit, "offset": offset}
         return self._get_albums(params)
 
     def get_albums_other(
         self, limit: Optional[int] = None, offset: int = 0
     ) -> List["Album"]:
+        warn(
+            "This method is deprecated an will be removed in a future release. Use instead `get_other`",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
+        return self.get_other(limit=limit, offset=offset)
+
+    def get_other(self, limit: Optional[int] = None, offset: int = 0) -> List["Album"]:
         """Queries TIDAL for albums the artist has appeared on as a featured artist.
 
         :return: A list of :class:`Albums <tidalapi.album.Album>`
         """
         params = {"filter": "COMPILATIONS", "limit": limit, "offset": offset}
         return self._get_albums(params)
```

### Comparing `tidalapi-0.7.5/tidalapi/genre.py` & `tidalapi-0.7.6/tidalapi/genre.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/tidalapi/media.py` & `tidalapi-0.7.6/tidalapi/media.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,76 +49,100 @@
     TooManyRequests,
     UnknownManifestFormat,
     URLNotAvailable,
 )
 from tidalapi.types import JsonObj
 
 
-class Quality:
+class Quality(str, Enum):
     low_96k: str = "LOW"
     low_320k: str = "HIGH"
     high_lossless: str = "LOSSLESS"
     hi_res: str = "HI_RES"
     hi_res_lossless: str = "HI_RES_LOSSLESS"
 
+    def __str__(self) -> str:
+        return self.value
 
-class VideoQuality:
+
+class VideoQuality(str, Enum):
     high: str = "HIGH"
     medium: str = "MEDIUM"
     low: str = "LOW"
     audio_only: str = "AUDIO_ONLY"
 
+    def __str__(self) -> str:
+        return self.value
+
 
-class AudioMode:
+class AudioMode(str, Enum):
     stereo: str = "STEREO"
     sony_360: str = "SONY_360RA"
     dolby_atmos: str = "DOLBY_ATMOS"
 
+    def __str__(self) -> str:
+        return self.value
+
 
-class MediaMetadataTags:
+class MediaMetadataTags(str, Enum):
     mqa: str = "MQA"
     hires_lossless: str = "HIRES_LOSSLESS"
     lossless: str = "LOSSLESS"
     sony_360: str = "SONY_360RA"
     dolby_atmos: str = "DOLBY_ATMOS"
 
+    def __str__(self) -> str:
+        return self.value
 
-class AudioExtensions:
+
+class AudioExtensions(str, Enum):
     FLAC: str = ".flac"
     M4A: str = ".m4a"
     MP4: str = ".mp4"
 
+    def __str__(self) -> str:
+        return self.value
+
 
-class VideoExtensions:
+class VideoExtensions(str, Enum):
     TS: str = ".ts"
 
+    def __str__(self) -> str:
+        return self.value
 
-class ManifestMimeType:
+
+class ManifestMimeType(str, Enum):
     # EMU: str = "application/vnd.tidal.emu"
     # APPL: str = "application/vnd.apple.mpegurl"
     MPD: str = "application/dash+xml"
     BTS: str = "application/vnd.tidal.bts"
     VIDEO: str = "video/mp2t"
 
+    def __str__(self) -> str:
+        return self.value
+
 
-class Codec:
+class Codec(str, Enum):
     MP3: str = "MP3"
     AAC: str = "AAC"
     M4A: str = "MP4A"
     FLAC: str = "FLAC"
     MQA: str = "MQA"
     Atmos: str = "EAC3"
     AC4: str = "AC4"
     SONY360RA: str = "MHA1"
     LowResCodecs: [str] = [MP3, AAC, M4A]
     PremiumCodecs: [str] = [MQA, Atmos, AC4]
     HQCodecs: [str] = PremiumCodecs + [FLAC]
 
+    def __str__(self) -> str:
+        return self.value
 
-class MimeType:
+
+class MimeType(str, Enum):
     audio_mpeg = "audio/mpeg"
     audio_mp3 = "audio/mp3"
     audio_m4a = "audio/m4a"
     audio_flac = "audio/flac"
     audio_xflac = "audio/x-flac"
     audio_eac3 = "audio/eac3"
     audio_ac4 = "audio/mp4"
@@ -131,14 +155,17 @@
         Codec.M4A: audio_m4a,
         Codec.FLAC: audio_xflac,
         Codec.MQA: audio_xflac,
         Codec.Atmos: audio_eac3,
         Codec.AC4: audio_ac4,
     }
 
+    def __str__(self) -> str:
+        return self.value
+
     @staticmethod
     def from_audio_codec(codec):
         return MimeType.audio_map.get(codec, MimeType.audio_m4a)
 
     @staticmethod
     def is_FLAC(mime_type):
         return (
```

### Comparing `tidalapi-0.7.5/tidalapi/mix.py` & `tidalapi-0.7.6/tidalapi/mix.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/tidalapi/page.py` & `tidalapi-0.7.6/tidalapi/page.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/tidalapi/playlist.py` & `tidalapi-0.7.6/tidalapi/playlist.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/tidalapi/request.py` & `tidalapi-0.7.6/tidalapi/request.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/tidalapi/session.py` & `tidalapi-0.7.6/tidalapi/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,15 +494,15 @@
 
         # Get redirect URL from user input.
         url_redirect: str = input("Paste 'Ooops' page URL here and press <ENTER>:")
         # Query for auth tokens
         json: dict[str, Union[str, int]] = self.pkce_get_auth_token(url_redirect)
 
         # Parse and set tokens.
-        self.process_auth_token(json)
+        self.process_auth_token(json, is_pkce_token=True)
 
         # Swap the client_id and secret
         # self.client_enable_hires()
 
     def client_enable_hires(self):
         self.config.client_id = self.config.client_id_pkce
         self.config.client_secret = self.config.client_secret_pkce
@@ -643,36 +643,40 @@
 
         json = request.json()
         executor = concurrent.futures.ThreadPoolExecutor()
         return LinkLogin(json), executor.submit(self._process_link_login, json)
 
     def _process_link_login(self, json: JsonObj) -> None:
         json = self._wait_for_link_login(json)
-        self.process_auth_token(json)
+        self.process_auth_token(json, is_pkce_token=False)
 
-    def process_auth_token(self, json: dict[str, Union[str, int]]) -> None:
+    def process_auth_token(
+        self, json: dict[str, Union[str, int]], is_pkce_token: bool = True
+    ) -> None:
         """Parses the authorization response and sets the token values to the specific
         variables for further usage.
 
         :param json: Parsed JSON response after login / authorization.
         :type json: dict[str, str | int]
+        :param is_pkce_token: Set true if current token is obtained using PKCE
+        :type is_pkce_token: bool
         :return: None
         """
         self.access_token = json["access_token"]
         self.expiry_time = datetime.datetime.utcnow() + datetime.timedelta(
             seconds=json["expires_in"]
         )
         self.refresh_token = json["refresh_token"]
         self.token_type = json["token_type"]
         session = self.request.request("GET", "sessions")
         json = session.json()
         self.session_id = json["sessionId"]
         self.country_code = json["countryCode"]
         self.user = user.User(self, user_id=json["userId"]).factory()
-        self.is_pkce = True
+        self.is_pkce = is_pkce_token
 
     def _wait_for_link_login(self, json: JsonObj) -> Any:
         expiry = float(json["expiresIn"])
         interval = float(json["interval"])
         device_code = json["deviceCode"]
         url = self.config.api_oauth2_token
         params = {
@@ -703,20 +707,22 @@
         :return: True if we believe the token was successfully refreshed, otherwise
             False
         """
         url = self.config.api_oauth2_token
         params = {
             "grant_type": "refresh_token",
             "refresh_token": refresh_token,
-            "client_id": self.config.client_id_pkce
-            if self.is_pkce
-            else self.config.client_id,
-            "client_secret": self.config.client_secret_pkce
-            if self.is_pkce
-            else self.config.client_secret,
+            "client_id": (
+                self.config.client_id_pkce if self.is_pkce else self.config.client_id
+            ),
+            "client_secret": (
+                self.config.client_secret_pkce
+                if self.is_pkce
+                else self.config.client_secret
+            ),
         }
 
         request = self.request_session.post(url, params)
         json = request.json()
         if request.status_code != 200:
             raise AuthenticationError("Authentication failed")
             # raise AuthenticationError(Authentication failed json["error"], json["error_description"])
```

### Comparing `tidalapi-0.7.5/tidalapi/user.py` & `tidalapi-0.7.6/tidalapi/user.py`

 * *Files identical despite different names*

### Comparing `tidalapi-0.7.5/PKG-INFO` & `tidalapi-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidalapi
-Version: 0.7.5
+Version: 0.7.6
 Summary: Unofficial API for TIDAL music streaming service.
 Home-page: https://tidalapi.netlify.app
 License: LGPL-3.0-or-later
 Author: Thomas Amland
 Author-email: thomas.amland@googlemail.com
 Maintainer: tehkillerbee
 Maintainer-email: tehkillerbee@users.noreply.github.com
@@ -73,14 +73,20 @@
         $ poetry install --no-root
 
 .. :changelog:
 
 History
 =======
 
+v0.7.6
+------
+* Fix: Set token type correctly for OAuth/PKCE authentication - tehkillerbee_
+* Revert to using enums with str support for relevant classes - tehkillerbee_, exislow_
+* Removed return types from method names for consistency, added deprecation warnings - exislow_
+
 v0.7.5
 ------
 * Fix: Use wide image when no square picture is available. - tehkillerbee_
 * Feat.: Added HiRes page. - tehkillerbee_
 * Feat.: Handle missing Stream fields gracefully. Get stream audio resolution (bit depth, rate) as tuple. - tehkillerbee_
 * Feat.: Added misc helper functions for audio mode, get available audio mode for media. - tehkillerbee_
 * Feat.: Added misc. fields to album. Get audio resolution for album + individual tracks. - tehkillerbee_
```

