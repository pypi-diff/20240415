# Comparing `tmp/asyncpow-0.3.0.tar.gz` & `tmp/asyncpow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpow-0.3.0.tar", max compression
+gzip compressed data, was "asyncpow-0.4.0.tar", max compression
```

## Comparing `asyncpow-0.3.0.tar` & `asyncpow-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     6694 2024-04-08 18:04:56.762812 asyncpow-0.3.0/README.md
--rw-r--r--   0        0        0     1187 2024-04-08 18:04:56.762812 asyncpow-0.3.0/asyncpow/__init__.py
--rw-r--r--   0        0        0     4916 2024-04-08 18:04:56.762812 asyncpow-0.3.0/asyncpow/apis/media.py
--rw-r--r--   0        0        0     2768 2024-04-08 18:04:56.762812 asyncpow-0.3.0/asyncpow/apis/movie.py
--rw-r--r--   0        0        0     5237 2024-04-08 18:04:56.762812 asyncpow-0.3.0/asyncpow/apis/search.py
--rw-r--r--   0        0        0     2977 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/apis/status.py
--rw-r--r--   0        0        0     2825 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/apis/tv.py
--rw-r--r--   0        0        0     1148 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/const.py
--rw-r--r--   0        0        0     1753 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/exceptions.py
--rw-r--r--   0        0        0     5055 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/models/common.py
--rw-r--r--   0        0        0     1790 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/models/media.py
--rw-r--r--   0        0        0     3787 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/models/movie.py
--rw-r--r--   0        0        0     5011 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/models/search.py
--rw-r--r--   0        0        0     1517 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/models/status.py
--rw-r--r--   0        0        0     3136 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/models/tv.py
--rw-r--r--   0        0        0     4340 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/overseerr.py
--rw-r--r--   0        0        0        0 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/py.typed
--rw-r--r--   0        0        0     4067 2024-04-08 18:04:56.766812 asyncpow-0.3.0/asyncpow/utils/http.py
--rw-r--r--   0        0        0     2919 2024-04-08 18:05:46.803256 asyncpow-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6694 2024-04-15 09:02:51.667383 asyncpow-0.4.0/README.md
+-rw-r--r--   0        0        0     1215 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/__init__.py
+-rw-r--r--   0        0        0     4908 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/media.py
+-rw-r--r--   0        0        0     2781 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/movie.py
+-rw-r--r--   0        0        0     5779 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/request.py
+-rw-r--r--   0        0        0     5290 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/search.py
+-rw-r--r--   0        0        0     3006 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/status.py
+-rw-r--r--   0        0        0     2854 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/apis/tv.py
+-rw-r--r--   0        0        0     1176 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/const.py
+-rw-r--r--   0        0        0     1781 2024-04-15 09:02:51.667383 asyncpow-0.4.0/asyncpow/exceptions.py
+-rw-r--r--   0        0        0     4981 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/common.py
+-rw-r--r--   0        0        0     4210 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/media.py
+-rw-r--r--   0        0        0     3815 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/movie.py
+-rw-r--r--   0        0        0     1574 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/request.py
+-rw-r--r--   0        0        0     5039 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/search.py
+-rw-r--r--   0        0        0     1546 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/status.py
+-rw-r--r--   0        0        0     3085 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/models/tv.py
+-rw-r--r--   0        0        0     4502 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/overseerr.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/py.typed
+-rw-r--r--   0        0        0     4096 2024-04-15 09:02:51.671383 asyncpow-0.4.0/asyncpow/utils/http.py
+-rw-r--r--   0        0        0     2919 2024-04-15 09:03:36.367846 asyncpow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 asyncpow-0.4.0/PKG-INFO
```

### Comparing `asyncpow-0.3.0/README.md` & `asyncpow-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `asyncpow-0.3.0/asyncpow/__init__.py` & `asyncpow-0.4.0/asyncpow/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
-
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 from .overseerr import Overseerr
 
 __all__ = ["Overseerr"]
```

### Comparing `asyncpow-0.3.0/asyncpow/apis/media.py` & `asyncpow-0.4.0/asyncpow/apis/media.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 from typing import Optional
 
 from aiohttp import ClientSession, hdrs
 from yarl import URL
 
 from asyncpow.models.common import SortOptions
@@ -64,16 +63,16 @@
     ) -> dict | MediaModel:
         """
         Get media items based on specified parameters.
 
         Args:
             take (int): The number of items to retrieve (default is 20).
             skip (int): The number of items to skip (default is 0).
-            filter (MediaFilterOptions): The filter option for media items (default is MediaFilterOptions.AVAILABLE).
-            sort (SortOptions): The sorting option for media items (default is SortOptions.ADDED).
+            filter (MediaFilterOptions): The filter option for media items (default is None).
+            sort (SortOptions): The sorting option for media items (default is None).
             raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
 
         Returns:
             dict | MediaModel: The media model object retrieved based on the parameters.
         """
         params: dict = {"take": take, "skip": skip}
         if filter:
```

### Comparing `asyncpow-0.3.0/asyncpow/apis/movie.py` & `asyncpow-0.4.0/asyncpow/apis/movie.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
-
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 from aiohttp import ClientSession
 from yarl import URL
 
 from asyncpow.models.movie import MovieDetailsModel
 from asyncpow.utils.http import request
 
@@ -46,27 +44,27 @@
             None
         """
         self.media_url = base_url.joinpath("movie")
         self.api_key = api_key
         self.session = session
 
     async def async_get_movie(
-        self, movieId: int, lang: str = "en", raw_response: bool = False
+        self, id: int, lang: str = "en", raw_response: bool = False
     ) -> dict | MovieDetailsModel:
         """
         Retrieves movie details by ID asynchronously.
 
         Args:
-            movieId (int): The ID of the movie.
+            id (int): The ID of the movie.
             lang (str): The language for the response (default is "en").
             raw_response (bool): Flag to return raw response or MovieDetailsModel (default is False).
 
         Returns:
             dict | MovieDetailsModel: The raw response or MovieDetailsModel object based on the raw_response flag.
         """
 
         params = {"language": lang}
-        url = self.media_url.joinpath(str(movieId))
+        url = self.media_url.joinpath(str(id))
 
         headers = {"X-Api-Key": self.api_key}
         response = await request(self.session, url, params=params, headers=headers)
         return response if raw_response else MovieDetailsModel(**response)
```

### Comparing `asyncpow-0.3.0/asyncpow/apis/search.py` & `asyncpow-0.4.0/asyncpow/apis/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
-
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 from aiohttp import ClientSession
 from yarl import URL
 
 from asyncpow.models.search import DiscoverWatchlistModel, SearchResultModel
 from asyncpow.utils.http import request
 
@@ -52,14 +50,15 @@
 
     async def async_get_search(
         self, query: str, raw_response: bool = False, page: int = 1, lang: str = "en"
     ) -> dict | SearchResultModel:
         """Search for Movies, TV or Person
 
         Args:
+            query (str):
             raw_response (bool): Flag to determine whether to return the raw response (True) or an object (False). Default is False.
             page (int): The page number for items (default is 1).
             lang (str): The language for items (default is "en").
 
         Returns:
             _type_: _description_
         """
```

### Comparing `asyncpow-0.3.0/asyncpow/apis/status.py` & `asyncpow-0.4.0/asyncpow/apis/status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 from aiohttp import ClientSession
 from yarl import URL
 
 from asyncpow.models.status import StatusAppDataModel, StatusModel
 from asyncpow.utils.http import request
```

### Comparing `asyncpow-0.3.0/asyncpow/apis/tv.py` & `asyncpow-0.4.0/asyncpow/apis/tv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 from aiohttp import ClientSession
 from yarl import URL
 
 from asyncpow.models.tv import TvDetailsModel
 from asyncpow.utils.http import request
```

### Comparing `asyncpow-0.3.0/asyncpow/const.py` & `asyncpow-0.4.0/asyncpow/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
-
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 API_URI = "api/v1"
```

### Comparing `asyncpow-0.3.0/asyncpow/exceptions.py` & `asyncpow-0.4.0/asyncpow/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
-
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 class POWException(Exception):
     """The base AsyncPOW Exception that all other exception classes extend."""
 
 
 class POWTimeoutException(POWException):
```

### Comparing `asyncpow-0.3.0/asyncpow/models/common.py` & `asyncpow-0.4.0/asyncpow/models/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,89 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 from typing import Literal
 
 from pydantic import BaseModel
 
 SortOptions = Literal["added", "modified", "mediaAdded"]
+MediaType = Literal["movie", "tv"]
 
 
 class UserModel(BaseModel):
     """
     Data class representing a user model.
     """
 
+    displayName: str
     id: int
     email: str
-    username: str
-    plexToken: str
-    plexUsername: str
+    username: str | None = None
+    password: str | None = None
+    resetPasswordGuid: str | None = None
+    recoveryLinkExpirationDate: str | None = None
     userType: int
+    plexId: int | None = None
+    plexToken: str | None = None
+    plexUsername: str | None = None
     permissions: int
     avatar: str
     createdAt: str
     updatedAt: str
-    requestCount: str
+    requestCount: int
+    requests: list | None = None  # TODO: Requests
+    movieQuotaLimit: int | None = None
+    movieQuotaDays: int | None = None
+    tvQuotaLimit: int | None = None
+    tvQuotaDays: int | None = None
+    settings: dict | None = None  # TODO: UserSettingsModel
+    pushSubscriptions: list | None = None  # TODO: UserPushSubscriptionModel
+    createdIssues: list | None = None  # TODO: IssueModel
 
 
 class PageInfoModel(BaseModel):
     """
     Data class representing page information.
+
+    As per code
     """
 
     page: int
     pages: int
     results: int
+    pageSize: int
+
+
+class PaginatedResponseModel(BaseModel):
+    """
+    Data class representing page information.
+
+    As per code
+    """
+
+    pageInfo: PageInfoModel
 
 
 class CastModel(BaseModel):
     """
     Data class representing a cast member.
     """
 
@@ -181,56 +207,19 @@
     Data class representing a production country.
     """
 
     iso_3166_1: str
     name: str
 
 
-class MediaRequestModel(BaseModel):
+class SeasonModel(BaseModel):
     """
-    Data class representing a media request model.
+    Data class representing a Season.
     """
 
+    airDate: str
     id: int
-    status: int
-    media: dict
-    createdAt: str
-    updatedAt: str
-    requestedBy: UserModel
-    modifiedBy: list[UserModel]
-    is4k: bool
-    serverId: int
-    profileId: int
-    rootFolder: str
-
-
-class MediaInfoModel(BaseModel):
-    """
-    Data class representing media information model.
-    """
-
-    id: int
-    mediaType: str
-    tmdbId: int
-    status: int
-    status4k: int
-    createdAt: str
-    updatedAt: str
-    lastSeasonChange: str
-    mediaAddedAt: str
-    serviceId: int
-    externalServiceId: int
-    externalServiceSlug: int
-    ratingKey: int
-    requests: MediaRequestModel | None = None
-    plexUrl: str | None = None
-    iOSPlexUrl: str | None = None
-    serviceUrl: str | None = None
-    serviceId4k: int | None = None
-    externalServiceId4k: int | None = None
-    externalServiceSlug4k: int | None = None
-    ratingKey4k: int | None = None
-    tvdbId: int | None = None
-    imdbId: int | None = None
-    downloadStatus: list | None = None
-    downloadStatus4k: list | None = None
-    seasons: list | None = None
+    episodeCount: int
+    name: str
+    overview: str
+    posterPath: str | None = None
+    seasonNumber: int
```

### Comparing `asyncpow-0.3.0/asyncpow/models/media.py` & `asyncpow-0.4.0/asyncpow/models/status.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,44 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
-
-from typing import Literal
 
 from pydantic import BaseModel
 
-from asyncpow.models.common import MediaInfoModel, PageInfoModel
-
-MediaFilterOptions = Literal["all", "available", "partial", "allavailable", "pending", "processing"]
-
-MediaStatusOptions = Literal["available", "partial", "pending", "processing", "unknown"]
-
 
-class MediaModel(BaseModel):
+class StatusModel(BaseModel):
     """
-    Data class representing a media model.
+    Data class representing the status model.
     """
 
-    pageInfo: PageInfoModel
-    results: MediaInfoModel
+    version: str
+    commitTag: str
+    updateAvailable: bool
+    commitsBehind: int
+    restartRequired: bool
 
 
-class MediaModel2(BaseModel):
+class StatusAppDataModel(BaseModel):
     """
-    Data class representing a secondary media model.
+    Data class representing the status of the app data.
     """
 
-    id: int
-    tmdbId: int
-    tvdbId: int
-    status: int
-    requests: list[MediaInfoModel]
+    appData: bool
+    appDataPath: str
```

### Comparing `asyncpow-0.3.0/asyncpow/models/movie.py` & `asyncpow-0.4.0/asyncpow/models/movie.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
-
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 from typing import Literal
 
 from pydantic import BaseModel
 
 from asyncpow.models.common import (
     CreditModel,
```

### Comparing `asyncpow-0.3.0/asyncpow/models/search.py` & `asyncpow-0.4.0/asyncpow/models/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 from pydantic import BaseModel, validator
 
 from asyncpow.exceptions import POWMediaTypeException
-from asyncpow.models.common import MediaInfoModel
+from asyncpow.models.media import MediaInfoModel
 
 
 class MovieResultModel(BaseModel):
     """
     Data class representing a movie search result.
     """
```

### Comparing `asyncpow-0.3.0/asyncpow/models/tv.py` & `asyncpow-0.4.0/asyncpow/models/tv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
+from typing import Literal
 
 from pydantic import BaseModel
 
 from asyncpow.models.common import (
     CreditModel,
     ExternalIdsModel,
     GenreModel,
     KeywordModel,
     ProductionCompanyModel,
     ProductionCountryModel,
+    SeasonModel,
     SpokenLanguagesModelTv,
     WatchProviderModel,
 )
 
+MediaRequestStatus = Literal["1"]  # TODO: Look into this more
+
 
 class EpisodeModel(BaseModel):
     """TV Episode model"""
 
     id: int
     name: str
     airDate: str | None
@@ -47,26 +51,14 @@
     seasonNumber: int
     showId: int
     stillPath: str | None
     voteAverage: float
     voteCount: int | None = None
 
 
-class SeasonModel(BaseModel):
-    """Model for TV Seasons"""
-
-    id: int
-    airDate: str | None = None
-    episodeCount: int
-    name: str
-    overview: str
-    posterPath: str | None = None
-    seasonNumber: int
-
-
 class CreatedByModel(BaseModel):
     """Model for Created by"""
 
     id: int
     name: str
     gender: int
     profilePath: str | None = None
@@ -74,15 +66,15 @@
 
 class TvDetailsModel(BaseModel):
     """TV Details model"""
 
     id: int
     backdropPath: str
     posterPath: str
-    contentRatings: dict
+    contentRatings: dict  # TODO: TmdbTvRatingResult
     createdBy: list[CreatedByModel]
     episodeRunTime: list[int]
     firstAirDate: str
     genres: list[GenreModel]
     homepage: str
     inProduction: bool
     languages: list[str]
```

### Comparing `asyncpow-0.3.0/asyncpow/overseerr.py` & `asyncpow-0.4.0/asyncpow/overseerr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 import aiohttp
 from cachetools import TTLCache
 from yarl import URL
 
 from asyncpow.apis.media import Media
 from asyncpow.apis.movie import Movie
+from asyncpow.apis.request import Request
 from asyncpow.apis.search import Discover, Search
 from asyncpow.apis.status import Status
 from asyncpow.apis.tv import Tv
 from asyncpow.const import API_URI
 
 VERSION_CACHE: TTLCache[str, str | None] = TTLCache(maxsize=16, ttl=7200)
 
@@ -93,14 +93,15 @@
         # Initialize instances of API classes
         self.status = Status(self.url, self.api_key, self._session)
         self.search = Search(self.url, self.api_key, self._session)
         self.discover = Discover(self.url, self.api_key, self._session)
         self.media = Media(self.url, self.api_key, self._session)
         self.movie = Movie(self.url, self.api_key, self._session)
         self.tv = Tv(self.url, self.api_key, self._session)
+        self.request = Request(self.url, self.api_key, self._session, self.tv, self.movie)
 
     async def __aenter__(self):
         """
         Enter method for asynchronous context manager.
 
         Returns:
             self
```

### Comparing `asyncpow-0.3.0/asyncpow/utils/http.py` & `asyncpow-0.4.0/asyncpow/utils/http.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-"""
-AsyncPOW - https://github.com/totaldebug/asyncpow
+# AsyncPOW - https://github.com/totaldebug/asyncpow
+#
+# Copyright (c) 2024 Steven Marks, Total Debug
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of
+# this software and associated documentation files (the "Software"), to deal in
+# the Software without restriction, including without limitation the rights to
+# use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+# the Software, and to permit persons to whom the Software is furnished to do so,
+# subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+# FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+# COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+# IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-Copyright (c) 2024 Steven Marks, Total Debug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
 
 import asyncio
 import json
 from typing import Any, Mapping, Optional
 
 from aiohttp import ClientError, ClientSession, hdrs
 import backoff
```

### Comparing `asyncpow-0.3.0/pyproject.toml` & `asyncpow-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpow"
-version = "0.3.0"
+version = "0.4.0"
 description = "Asynchronous Python Overseerr Wrapper"
 authors = ["Steven Marks - TotalDebug"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/totaldebug/asyncpow"
 repository = "https://github.com/totaldebug/asyncpow"
 classifiers = [
```

### Comparing `asyncpow-0.3.0/PKG-INFO` & `asyncpow-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpow
-Version: 0.3.0
+Version: 0.4.0
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
-Metadata-Version: 2.1 Name: asyncpow Version: 0.3.0 Summary: Asynchronous
+Metadata-Version: 2.1 Name: asyncpow Version: 0.4.0 Summary: Asynchronous
 Python Overseerr Wrapper Home-page: https://github.com/totaldebug/asyncpow
 License: MIT Keywords: wled,api,async,client Author: Steven Marks - TotalDebug
 Maintainer: Steven Marks - TotalDebug Requires-Python: >=3.12,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.12
```

