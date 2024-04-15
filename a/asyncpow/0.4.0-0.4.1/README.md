# Comparing `tmp/asyncpow-0.4.0.tar.gz` & `tmp/asyncpow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpow-0.4.0.tar", max compression
+gzip compressed data, was "asyncpow-0.4.1.tar", max compression
```

## Comparing `asyncpow-0.4.0.tar` & `asyncpow-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6694 2024-04-15 09:02:51.667383 asyncpow-0.4.0/README.md
--rw-r--r--   0        0        0     1215 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/__init__.py
--rw-r--r--   0        0        0     4908 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/media.py
--rw-r--r--   0        0        0     2781 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/movie.py
--rw-r--r--   0        0        0     5779 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/request.py
--rw-r--r--   0        0        0     5290 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/search.py
--rw-r--r--   0        0        0     3006 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/status.py
--rw-r--r--   0        0        0     2854 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/tv.py
--rw-r--r--   0        0        0     1176 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/const.py
--rw-r--r--   0        0        0     1781 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/exceptions.py
--rw-r--r--   0        0        0     4981 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/common.py
--rw-r--r--   0        0        0     4210 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/media.py
--rw-r--r--   0        0        0     3815 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/movie.py
--rw-r--r--   0        0        0     1574 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/request.py
--rw-r--r--   0        0        0     5039 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/search.py
--rw-r--r--   0        0        0     1546 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/status.py
--rw-r--r--   0        0        0     3085 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/tv.py
--rw-r--r--   0        0        0     4502 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/overseerr.py
--rw-r--r--   0        0        0        0 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/py.typed
--rw-r--r--   0        0        0     4096 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/utils/http.py
--rw-r--r--   0        0        0     2919 2024-04-15 09:03:36.367846 asyncpow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6694 2024-04-15 14:57:21.205706 asyncpow-0.4.1/README.md
+-rw-r--r--   0        0        0     1215 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/__init__.py
+-rw-r--r--   0        0        0     4908 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/apis/media.py
+-rw-r--r--   0        0        0     2781 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/apis/movie.py
+-rw-r--r--   0        0        0     6053 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/apis/request.py
+-rw-r--r--   0        0        0     5290 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/apis/search.py
+-rw-r--r--   0        0        0     3006 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/apis/status.py
+-rw-r--r--   0        0        0     2848 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/apis/tv.py
+-rw-r--r--   0        0        0     1176 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/const.py
+-rw-r--r--   0        0        0     1781 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/exceptions.py
+-rw-r--r--   0        0        0     4981 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/models/common.py
+-rw-r--r--   0        0        0     4026 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/models/media.py
+-rw-r--r--   0        0        0     3815 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/models/movie.py
+-rw-r--r--   0        0        0     1574 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/models/request.py
+-rw-r--r--   0        0        0     5039 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/models/search.py
+-rw-r--r--   0        0        0     1546 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/models/status.py
+-rw-r--r--   0        0        0     3085 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/models/tv.py
+-rw-r--r--   0        0        0     4502 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/overseerr.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/py.typed
+-rw-r--r--   0        0        0     4096 2024-04-15 14:57:21.205706 asyncpow-0.4.1/asyncpow/utils/http.py
+-rw-r--r--   0        0        0     2919 2024-04-15 14:58:09.201548 asyncpow-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.4.1/PKG-INFO
```

### Comparing `asyncpow-0.4.0/README.md` & `asyncpow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/__init__.py` & `asyncpow-0.4.1/asyncpow/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/apis/media.py` & `asyncpow-0.4.1/asyncpow/apis/media.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/apis/movie.py` & `asyncpow-0.4.1/asyncpow/apis/movie.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/apis/request.py` & `asyncpow-0.4.1/asyncpow/apis/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 from typing import Literal
 
 from aiohttp import ClientSession, hdrs
 from yarl import URL
 
 from asyncpow.apis.movie import Movie
 from asyncpow.apis.tv import Tv
-from asyncpow.exceptions import POWMediaTypeException
+from asyncpow.exceptions import POWException, POWMediaTypeException
 from asyncpow.models.common import SortOptions
 from asyncpow.models.media import MediaRequestModel
 from asyncpow.models.request import RequestFilterOptions, RequestResultsResponseModel
+from asyncpow.models.tv import TvDetailsModel
 from asyncpow.utils.http import request
 
 
 class Request:
     """
     Class to interact with request-related endpoints.
 
@@ -122,32 +123,34 @@
 
         if type == "movie":
             req_data = {
                 "mediaType": "movie",
                 "mediaId": id,
             }
         elif type == "tv":
-            data = self.tv.async_get_tv(id=id)
-
-            if series == "all":
-                seasons_array = [
-                    season.seasonNumber for season in data.seasons if season.seasonNumber != 0
-                ]
-            elif series == "first":
-                seasons_array = [1]
-
-            elif series == "latest":
-                for season in data.seasons:
-                    seasons_array = [season.seasonNumber]
-            req_data = {
-                "mediaType": "tv",
-                "mediaId": id,
-                "tvdbId": data.externalIds.tvdbId,
-                "seasons": seasons_array,
-            }
+            data = await self.tv.async_get_tv(id=id)
+            if isinstance(data, TvDetailsModel):
+                if series == "all":
+                    seasons_array = [
+                        season.seasonNumber for season in data.seasons if season.seasonNumber != 0
+                    ]
+                elif series == "first":
+                    seasons_array = [1]
+
+                elif series == "latest":
+                    for season in data.seasons:
+                        seasons_array = [season.seasonNumber]
+                req_data = {
+                    "mediaType": "tv",
+                    "mediaId": id,
+                    "tvdbId": data.externalIds.tvdbId,
+                    "seasons": seasons_array,
+                }
+            else:
+                raise POWException(f"Expecting TvDetailsModel, got {type(data)}")
         else:
             raise POWMediaTypeException("Unknown media type, use either movie or tv")
 
         headers = {"X-Api-Key": self.api_key, "Content-Type": "application/json"}
         response = await request(
             self.session,
             self.request_url,
```

### Comparing `asyncpow-0.4.0/asyncpow/apis/search.py` & `asyncpow-0.4.1/asyncpow/apis/search.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/apis/status.py` & `asyncpow-0.4.1/asyncpow/apis/status.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/apis/tv.py` & `asyncpow-0.4.1/asyncpow/apis/tv.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,29 +45,29 @@
             None
         """
         self.media_url = base_url.joinpath("tv")
         self.api_key = api_key
         self.session = session
 
     async def async_get_tv(
-        self, tvId: int, lang: str = "en", raw_response: bool = False
+        self, id: int, lang: str = "en", raw_response: bool = False
     ) -> dict | TvDetailsModel:
         """
         Retrieves TV details by ID asynchronously.
 
         Args:
-            tvId (int): The ID of the TV show.
+            id (int): The ID of the TV show.
             lang (str): The language for the response (default is "en").
             raw_response (bool): Flag to return raw response or TvDetailsModel (default is False).
 
         Returns:
             dict | TvDetailsModel: The raw response or TvDetailsModel object based on the raw_response flag.
 
         Examples:
             tv_details = await async_get_tv(12345, lang="en", raw_response=False)
         """
         params = {"language": lang}
-        url = self.media_url.joinpath(str(tvId))
+        url = self.media_url.joinpath(str(id))
 
         headers = {"X-Api-Key": self.api_key}
         response = await request(self.session, url, params=params, headers=headers)
         return response if raw_response else TvDetailsModel(**response)
```

### Comparing `asyncpow-0.4.0/asyncpow/const.py` & `asyncpow-0.4.1/asyncpow/const.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/exceptions.py` & `asyncpow-0.4.1/asyncpow/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/models/common.py` & `asyncpow-0.4.1/asyncpow/models/common.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/models/media.py` & `asyncpow-0.4.1/asyncpow/models/media.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,25 +16,49 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from typing import ForwardRef, Literal
+from typing import Literal
 
 from pydantic import BaseModel
 
 from asyncpow.models.common import MediaType, PaginatedResponseModel, SeasonModel, UserModel
 
 MediaFilterOptions = Literal["all", "available", "partial", "allavailable", "pending", "processing"]
 
 MediaStatusOptions = Literal["available", "partial", "pending", "processing", "unknown"]
 
-MediaRequestModel = ForwardRef("MediaRequestModel")
+
+class MediaRequestModel(BaseModel):
+    """
+    Data class representing a media request model.
+
+    As per code
+    """
+
+    id: int
+    status: int  # 1 = PENDING APPROVAL, 2 = APPROVED, 3 = DECLINED
+    media: "MediaInfoModel"
+    requestedBy: UserModel
+    modifiedBy: UserModel | None = None
+    createdAt: str
+    updatedAt: str
+    type: MediaType
+    is4k: bool
+    serverId: int | None = None
+    profileId: int | None = None
+    rootFolder: str | None = None
+    languageProfileId: int | None = None
+    tags: list | None = None
+    isAutoRequest: bool = False
+    seasonCount: int | None = None
+    seasons: list["SeasonRequestModel"] | None = None
 
 
 class MediaInfoModel(BaseModel):
     """
     Data class representing media information model.
     """
 
@@ -62,17 +86,14 @@
     plexUrl4k: str | None = None
     iOSPlexUrl: str | None = None
     iOSPlexUrl4k: str | None = None
     tautulliUrl: str | None = None
     tautulliUrl4k: str | None = None
     serviceUrl: str | None = None
     serviceUrl4k: int | None = None
-    externalServiceId4k: int | None = None
-    externalServiceSlug4k: int | None = None
-    ratingKey4k: int | None = None
     tvdbId: int | None = None
     imdbId: int | None = None
     downloadStatus: list | None = None
     downloadStatus4k: list | None = None
     seasons: list[SeasonModel] | list | None = None
 
 
@@ -83,40 +104,14 @@
     seasonNumber: int
     status: int = 1  # PENDING = 1, APPROVED = 2, DECLINED = 3, FAILED = 4
     request: MediaRequestModel | None = None
     createdAt: str
     updatedAt: str
 
 
-class MediaRequestModel(BaseModel):
-    """
-    Data class representing a media request model.
-
-    As per code
-    """
-
-    id: int
-    status: int  # 1 = PENDING APPROVAL, 2 = APPROVED, 3 = DECLINED
-    media: MediaInfoModel
-    requestedBy: UserModel
-    modifiedBy: UserModel | None = None
-    createdAt: str
-    updatedAt: str
-    type: MediaType
-    is4k: bool
-    serverId: int | None = None
-    profileId: int | None = None
-    rootFolder: str | None = None
-    languageProfileId: int | None = None
-    tags: list | None = None
-    isAutoRequest: bool = False
-    seasonCount: int | None = None
-    seasons: list[SeasonRequestModel] | None = None
-
-
 class MediaModel(PaginatedResponseModel):
     """
     Data class representing a media model.
     """
 
     results: MediaInfoModel
```

### Comparing `asyncpow-0.4.0/asyncpow/models/movie.py` & `asyncpow-0.4.1/asyncpow/models/movie.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/models/request.py` & `asyncpow-0.4.1/asyncpow/models/request.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/models/search.py` & `asyncpow-0.4.1/asyncpow/models/search.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/models/status.py` & `asyncpow-0.4.1/asyncpow/models/status.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/models/tv.py` & `asyncpow-0.4.1/asyncpow/models/tv.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/overseerr.py` & `asyncpow-0.4.1/asyncpow/overseerr.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/asyncpow/utils/http.py` & `asyncpow-0.4.1/asyncpow/utils/http.py`

 * *Files identical despite different names*

### Comparing `asyncpow-0.4.0/pyproject.toml` & `asyncpow-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpow"
-version = "0.4.0"
+version = "0.4.1"
 description = "Asynchronous Python Overseerr Wrapper"
 authors = ["Steven Marks - TotalDebug"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/totaldebug/asyncpow"
 repository = "https://github.com/totaldebug/asyncpow"
 classifiers = [
```

### Comparing `asyncpow-0.4.0/PKG-INFO` & `asyncpow-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Asynchronous Python Overseerr Wrapper
 Home-page: https://github.com/totaldebug/asyncpow
 License: MIT
 Keywords: wled,api,async,client
 Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug
 Requires-Python: >=3.12,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asyncpow Version: 0.4.0 Summary: Asynchronous
+Metadata-Version: 2.1 Name: asyncpow Version: 0.4.1 Summary: Asynchronous
 Python Overseerr Wrapper Home-page: https://github.com/totaldebug/asyncpow
 License: MIT Keywords: wled,api,async,client Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug Requires-Python: >=3.12,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.12
```

