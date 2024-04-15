# Comparing `tmp/playwrightcapture-1.24.3.tar.gz` & `tmp/playwrightcapture-1.24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.24.3.tar", max compression
+gzip compressed data, was "playwrightcapture-1.24.4.tar", max compression
```

## Comparing `playwrightcapture-1.24.3.tar` & `playwrightcapture-1.24.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/LICENSE
--rw-r--r--   0        0        0     1441 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/README.md
--rw-r--r--   0        0        0      511 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    61485 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1764 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1487 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.3/PKG-INFO
+-rw-r--r--   0        0        0     1775 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/LICENSE
+-rw-r--r--   0        0        0     1441 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/README.md
+-rw-r--r--   0        0        0      511 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    62432 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1764 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1487 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/pyproject.toml
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.4/PKG-INFO
```

### Comparing `playwrightcapture-1.24.3/LICENSE` & `playwrightcapture-1.24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.3/README.md` & `playwrightcapture-1.24.4/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.3/playwrightcapture/capture.py` & `playwrightcapture-1.24.4/playwrightcapture/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -677,15 +677,18 @@
                             if not error_msg:
                                 raise e
                             to_return['error'] = f"Error while downloading: {error_msg}"
                             self.logger.info(to_return['error'])
                             self.should_retry = True
                         except Exception:
                             raise e
-                elif self._exception_is_network_error(initial_error):
+                else:
+                    if not self._exception_is_network_error(initial_error):
+                        # TODO: Do something?
+                        self.logger.warning(f'Unexpected error: {initial_error}')
                     raise initial_error
             else:
                 await page.bring_to_front()
                 self.logger.debug('Page moved to front.')
 
                 # page instrumentation
                 await self._wait_for_random_timeout(page, 5)  # Wait 5 sec after document loaded
@@ -714,16 +717,16 @@
 
                 # check if we have anything on the page. If we don't, the page is not working properly.
                 if await self._failsafe_get_content(page):
                     self.logger.debug('Got rendered content')
                     if allow_tracking:
                         await self._wait_for_random_timeout(page, 2)
                         # This event is required trigger the add_locator_handler
-                        if await page.locator("body").is_visible():
-                            await page.locator("body").click(button="right", timeout=2000)
+                        if await page.locator("body").first.is_visible():
+                            await page.locator("body").first.click(button="right", timeout=2000)
 
                     # move mouse
                     await page.mouse.move(x=random.uniform(300, 800), y=random.uniform(200, 500))
                     self.logger.debug('Moved mouse.')
                     await self._wait_for_random_timeout(page, 2)
                     self.logger.debug('Keep going after moving mouse.')
 
@@ -860,22 +863,27 @@
                 # this one sounds like something we can retry...
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Download is starting',
                             'Connection closed',
                             'Navigation interrupted by another one',
                             'Navigation failed because page was closed!',
-                            'Protocol error (Page.bringToFront): Not attached to an active page']:
+                            'Protocol error (Page.bringToFront): Not attached to an active page',
+                            'Peer failed to perform TLS handshake: The TLS connection was non-properly terminated.',
+                            'Load cannot follow more than 20 redirections']:
                 # Other errors, let's give it another shot
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Target page, context or browser has been closed']:
                 # The browser barfed, let's try again
                 self.logger.info(f'Browser barfed on {url} (retrying): {e.message}')
                 self.should_retry = True
+            elif e.name in ['net::ERR_INVALID_AUTH_CREDENTIALS']:
+                # No need to retry, the credentials are wrong/missing.
+                pass
             else:
                 # Unexpected ones
                 self.logger.exception(f'Something went poorly with {url}: {e.message}')
         except Exception as e:
             # we may get a non-playwright exception to.
             # The ones we try to handle here should be treated as if they were.
             to_return['error'] = str(e)
@@ -928,16 +936,16 @@
     async def _safe_wait(self, page: Page, force_max_wait_in_sec: int | None=None) -> None:
         max_wait: float
         try:
             if force_max_wait_in_sec is not None:
                 max_wait = force_max_wait_in_sec
             else:
                 max_wait = self._capture_timeout / self.__network_not_idle
-            max_wait *= 1000
             self.logger.debug(f'Waiting for network idle, max wait: {max_wait}s')
+            max_wait *= 1000
             # If we don't have networkidle relatively quick, it's probably because we're playing a video.
             await page.wait_for_load_state('networkidle', timeout=max_wait)
         except PlaywrightTimeoutError:
             # Network never idle, keep going
             self.__network_not_idle += 1
             self.logger.debug(f'Timed out - Waiting for network idle, max wait: {max_wait}s')
 
@@ -1099,16 +1107,19 @@
                 'NS_ERROR_UNKNOWN_HOST',
                 'NS_ERROR_UNKNOWN_PROTOCOL',
                 'net::ERR_ABORTED',
                 'net::ERR_ADDRESS_UNREACHABLE',
                 'net::ERR_CONNECTION_CLOSED',
                 'net::ERR_CONNECTION_REFUSED',
                 'net::ERR_CONNECTION_RESET',
+                'net::ERR_CONNECTION_TIMED_OUT',
                 'net::ERR_EMPTY_RESPONSE',
+                'net::ERR_HTTP_RESPONSE_CODE_FAILURE',
                 'net::ERR_HTTP2_PROTOCOL_ERROR',
+                'net::ERR_INVALID_RESPONSE',
                 'net::ERR_NAME_NOT_RESOLVED',
                 'net::ERR_SOCKS_CONNECTION_FAILED',
                 'net::ERR_SSL_UNRECOGNIZED_NAME_ALERT',
                 'net::ERR_SSL_VERSION_OR_CIPHER_MISMATCH',
                 'net::ERR_SSL_PROTOCOL_ERROR',
                 'net::ERR_TIMED_OUT',
                 'net::ERR_TOO_MANY_REDIRECTS',
@@ -1247,16 +1258,22 @@
                 if favicon:
                     try:
                         mimetype = from_string(favicon, mime=True)
                     except PureError:
                         # unable to identify the mimetype
                         self.logger.debug(f'Unable to identify the mimetype for favicon from {u}')
                     else:
-                        if mimetype.startswith('image'):
+                        if not mimetype:
+                            # empty, ignore
+                            pass
+                        elif mimetype.startswith('image'):
                             to_return.add(favicon)
+                        elif mimetype.startswith('text'):
+                            # Just ignore, it's probably a 404 page
+                            pass
                         else:
                             self.logger.warning(f'Unexpected mimetype for favicon from {u}: {mimetype}')
                 self.logger.debug(f'Done with favicon from {u}.')
             except requests.HTTPError as e:
                 self.logger.debug(f'Unable to fetch favicon from {u}: {e}')
             except Exception as e:
                 self.logger.info(f'Unexpectedly unable to fetch favicon from {u}: {e}')
```

### Comparing `playwrightcapture-1.24.3/playwrightcapture/helpers.py` & `playwrightcapture-1.24.4/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.3/pyproject.toml` & `playwrightcapture-1.24.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.24.3"
+version = "1.24.4"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -25,15 +25,15 @@
 w3lib = "^2.1.2"
 requests = {extras = ["socks"], version = "^2.31.0"}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.3", optional = true}
 pytz = {"version" = "^2024.1", python = "<3.9"}
 tzdata = "^2024.1"
 playwright-stealth = "^1.0.6"
-setuptools = "^69.2.0"
+setuptools = "^69.5.1"
 puremagic = "^1.21"
 
 [tool.poetry.extras]
 recaptcha = ["requests", "pydub", "SpeechRecognition"]
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `playwrightcapture-1.24.3/PKG-INFO` & `playwrightcapture-1.24.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightCapture
-Version: 1.24.3
+Version: 1.24.4
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 Requires-Dist: dateparser (>=1.2.0,<2.0.0)
 Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: playwright-stealth (>=1.0.6,<2.0.0)
 Requires-Dist: puremagic (>=1.21,<2.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2024.1,<2025.0) ; python_version < "3.9"
 Requires-Dist: requests[socks] (>=2.31.0,<3.0.0) ; extra == "recaptcha"
-Requires-Dist: setuptools (>=69.2.0,<70.0.0)
+Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Requires-Dist: tzdata (>=2024.1,<2025.0)
 Requires-Dist: w3lib (>=2.1.2,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
 Description-Content-Type: text/markdown
 
 # Playwright Capture
```

