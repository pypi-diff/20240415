# Comparing `tmp/uploadgram-0.2.3.tar.gz` & `tmp/uploadgram-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadgram-0.2.3.tar", max compression
+gzip compressed data, was "uploadgram-0.3.1.tar", max compression
```

## Comparing `uploadgram-0.2.3.tar` & `uploadgram-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    34522 2022-07-29 15:24:39.869046 uploadgram-0.2.3/LICENSE
--rw-r--r--   0        0        0      389 2022-07-29 15:24:39.869046 uploadgram-0.2.3/README.md
--rw-r--r--   0        0        0     1755 2022-07-29 15:24:39.869046 uploadgram-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      878 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/__init__.py
--rw-r--r--   0        0        0     1920 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/config.py
--rw-r--r--   0        0        0     1167 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/get_config.py
--rw-r--r--   0        0        0     1208 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/humanbytes.py
--rw-r--r--   0        0        0     2782 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/progress.py
--rw-r--r--   0        0        0     1390 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/run_shell_command.py
--rw-r--r--   0        0        0     4285 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/shell.py
--rw-r--r--   0        0        0     1558 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/take_screen_shot.py
--rw-r--r--   0        0        0     1239 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/time_formatter.py
--rw-r--r--   0        0        0     7828 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/upload.py
--rw-r--r--   0        0        0     1533 2022-07-29 15:24:39.869046 uploadgram-0.2.3/uploadgram/uploadgram.py
--rw-r--r--   0        0        0     1281 2022-07-29 15:25:09.688958 uploadgram-0.2.3/setup.py
--rw-r--r--   0        0        0     1747 2022-07-29 15:25:09.689266 uploadgram-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-04-15 13:05:00.860704 uploadgram-0.3.1/LICENSE
+-rw-r--r--   0        0        0      412 2024-04-15 13:05:00.860704 uploadgram-0.3.1/README.md
+-rw-r--r--   0        0        0     1757 2024-04-15 13:05:00.860704 uploadgram-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      878 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/__init__.py
+-rw-r--r--   0        0        0     1920 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/config.py
+-rw-r--r--   0        0        0     1167 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/get_config.py
+-rw-r--r--   0        0        0     1208 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/humanbytes.py
+-rw-r--r--   0        0        0     2772 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/progress.py
+-rw-r--r--   0        0        0     1390 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/run_shell_command.py
+-rw-r--r--   0        0        0     4292 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/shell.py
+-rw-r--r--   0        0        0     1586 2024-04-15 13:05:00.860704 uploadgram-0.3.1/uploadgram/take_screen_shot.py
+-rw-r--r--   0        0        0     1239 2024-04-15 13:05:00.864704 uploadgram-0.3.1/uploadgram/time_formatter.py
+-rw-r--r--   0        0        0     7920 2024-04-15 13:05:00.864704 uploadgram-0.3.1/uploadgram/upload.py
+-rw-r--r--   0        0        0     2083 2024-04-15 13:05:00.864704 uploadgram-0.3.1/uploadgram/uploadgram.py
+-rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 uploadgram-0.3.1/PKG-INFO
```

### Comparing `uploadgram-0.2.3/LICENSE` & `uploadgram-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uploadgram-0.2.3/pyproject.toml` & `uploadgram-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uploadgram"
-version = "0.2.3"
+version = "0.3.1"
 description ="Upload files to Telegram upto 4 GiB, from the Terminal"
 authors = ["Shrimadhav U K <uploADGRam@shrimadhavUK.me>"]
 homepage = "https://github.com/SpEcHiDe/UploadGram"
 repository = "https://github.com/SpEcHiDe/UploadGram"
 keywords = ["telegram-upload", "telegram", "upload", "video", "audio"]
 license = "AGPLv3"
 readme = "README.md"
@@ -23,16 +23,16 @@
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.7,<4"
 python-dotenv = "0.10"
-Pyrogram = "2.0.35"
-TgCrypto = "1.2.3"
+pyrotgfork = "2.1.17"
+TgCrypto = "1.2.5"
 hachoir = "3.1.1"
 tqdm = "4.62.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 isort = "^5.7.0"
 black = "^20.8b1"
```

### Comparing `uploadgram-0.2.3/uploadgram/__init__.py` & `uploadgram-0.3.1/uploadgram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """Top-level package for Uploadgram."""
 
 __author__ = """SpEcHIDe"""
 __email__ = "uploADGRam@shrimadhavUK.me"
-__version__ = "0.2.3"
+__version__ = "0.3.1"
```

### Comparing `uploadgram-0.2.3/uploadgram/config.py` & `uploadgram-0.3.1/uploadgram/config.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.2.3/uploadgram/get_config.py` & `uploadgram-0.3.1/uploadgram/get_config.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.2.3/uploadgram/humanbytes.py` & `uploadgram-0.3.1/uploadgram/humanbytes.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.2.3/uploadgram/progress.py` & `uploadgram-0.3.1/uploadgram/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,12 +66,12 @@
                 humanbytes(total),
                 humanbytes(speed),
                 estimated_total_time
                 if estimated_total_time != ""
                 else "0 seconds",
             )
             try:
-                await message.edit_text(text="{}\n {}".format(ud_type, tmp))
+                await message.edit_text(text=f"{ud_type}\n {tmp}")
             except FloodWait as e:
                 await sleep(e.value)
             except:  # noqa: E722
                 pass
```

### Comparing `uploadgram-0.2.3/uploadgram/run_shell_command.py` & `uploadgram-0.3.1/uploadgram/run_shell_command.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.2.3/uploadgram/shell.py` & `uploadgram-0.3.1/uploadgram/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         )
     if (
         dest_chat.isnumeric() or
         dest_chat.startswith("-100")
     ):
         dest_chat = int(dest_chat)
     dest_chat = (
-        await uploadgram.get_chat(dest_chat)
+        await uploadgram.get_chat(dest_chat, False)
     ).id
 
     dir_path = args.dir_path
     if not dir_path:
         dir_path = input(
             "enter path to upload to Telegram: "
         )
```

### Comparing `uploadgram-0.2.3/uploadgram/take_screen_shot.py` & `uploadgram-0.3.1/uploadgram/take_screen_shot.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     out_put_file_name = os.path.join(
         output_directory,
         str(time()) + ".jpg"
     )
     if video_file.upper().endswith(TG_VIDEO_TYPES):
         file_genertor_command = [
             "ffmpeg",
+            "-hide_banner",
             "-ss",
             str(ttl),
             "-i",
             video_file,
             "-vframes",
             "1",
             out_put_file_name
```

### Comparing `uploadgram-0.2.3/uploadgram/time_formatter.py` & `uploadgram-0.3.1/uploadgram/time_formatter.py`

 * *Files identical despite different names*

### Comparing `uploadgram-0.2.3/uploadgram/upload.py` & `uploadgram-0.3.1/uploadgram/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,26 +143,26 @@
     file_path: str,
     caption_rts: str,
     thumbnail_file: str,
     start_time: int,
     pbar: tqdm,
 ):
 
-    return await usr_sent_message._client.send_document(
-        chat_id=usr_sent_message.chat.id,
+    return await usr_sent_message.reply_document(
         document=file_path,
+        quote=True,
         caption=caption_rts,
-        force_document=True,
+        disable_content_type_detection=True,
         thumb=thumbnail_file,
         progress=progress_for_pyrogram,
         progress_args=(
             bot_sent_message,
             start_time,
             pbar,
-            "UpLoading to Telegram",
+            f"Uploading {os.path.basename(file_path)} as <b>DOCUMENT</b>"
         ),
     )
 
 
 async def upload_as_video(
     usr_sent_message: Message,
     bot_sent_message: Message,
@@ -212,15 +212,15 @@
         supports_streaming=True,
         caption=caption_rts,
         progress=progress_for_pyrogram,
         progress_args=(
             bot_sent_message,
             start_time,
             pbar,
-            "UpLoading to Telegram",
+            f"Uploading {os.path.basename(file_path)} as <b>VIDEO</b>"
         ),
     )
     if thumb_nail_img and os.path.exists(thumb_nail_img):
         os.remove(thumb_nail_img)
     return _tmp_m
 
 
@@ -263,10 +263,10 @@
         title=title,
         thumb=thumbnail_file,
         progress=progress_for_pyrogram,
         progress_args=(
             bot_sent_message,
             start_time,
             pbar,
-            "UpLoading to Telegram",
+            f"Uploading {os.path.basename(file_path)} as <b>AUDIO</b>"
         ),
     )
```

### Comparing `uploadgram-0.2.3/uploadgram/uploadgram.py` & `uploadgram-0.3.1/uploadgram/uploadgram.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,34 +10,45 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Affero General Public License for more details.
 #  You should have received a copy of the GNU Affero General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from pyrogram import Client, __version__
-from pyrogram.enums import ParseMode
+from pyrogram.enums import ParseMode, ClientPlatform
 from .get_config import get_config
 
 
 class Uploadgram(Client):
     """ modded client """
 
     def __init__(self):
         super().__init__(
             name="UploadGram",
             api_id=int(get_config("UG_TG_APP_ID")),
             api_hash=get_config("UG_TG_API_HASH"),
             parse_mode=ParseMode.HTML,
             sleep_threshold=int(get_config("UG_TG_ST", 10)),
-            no_updates=True
+            workers=int(get_config("UG_TG_WS", 10)),
+            max_concurrent_transmissions=int(get_config("UG_TG_MCTS", 4))
+            no_updates=True,
+            device_model="Samsung SM-G998B",
+            app_version="8.4.1 (2522)",
+            system_version="SDK 31",
+            lang_pack="",
+            lang_code="en",
+            system_lang_code="en",
+            max_message_cache_size=int(get_config("UG_TG_MMC", 0)),
+            max_business_user_connection_cache_size=int(get_config("UG_TG_MBUC", 0)),
+            client_platform=ClientPlatform.ANDROID
         )
 
     async def start(self):
         await super().start()
-        usr_bot_me = self.me
         print(
-            f"@{usr_bot_me.username} based on Pyrogram v{__version__} started."
+            f"{self.me} based on Pyrogram v{__version__} started."
         )
 
     async def stop(self, *args):
+        usr_bot_me = self.me
         await super().stop()
-        print("UploadGram stopped. Bye.")
+        print(f"{usr_bot_me} stopped. Bye.")
```

### Comparing `uploadgram-0.2.3/PKG-INFO` & `uploadgram-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 Metadata-Version: 2.1
 Name: uploadgram
-Version: 0.2.3
+Version: 0.3.1
 Summary: Upload files to Telegram upto 4 GiB, from the Terminal
 Home-page: https://github.com/SpEcHiDe/UploadGram
 License: AGPLv3
 Keywords: telegram-upload,telegram,upload,video,audio
 Author: Shrimadhav U K
 Author-email: uploADGRam@shrimadhavUK.me
 Requires-Python: >=3.7.7,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Pyrogram (==2.0.35)
-Requires-Dist: TgCrypto (==1.2.3)
+Requires-Dist: TgCrypto (==1.2.5)
 Requires-Dist: hachoir (==3.1.1)
+Requires-Dist: pyrotgfork (==2.1.17)
 Requires-Dist: python-dotenv (==0.10)
 Requires-Dist: tqdm (==4.62.3)
 Project-URL: Repository, https://github.com/SpEcHiDe/UploadGram
 Description-Content-Type: text/markdown
 
 ## uploadgram
 
 uploadgram uses your Telegram account to upload files up to 2GiB, from the Terminal.
 
 - Heavily inspired by the [telegram-upload](https://github.com/Nekmo/telegram-upload)
 
 - Installing:
+
 `pip install uploadgram`
 
 - Requirements:
-`pyrogram`
+
+a customized fork of `pyrogram`
 
 
 # Sample Usage
 
 ```sh
 $ uploadgram 7351948 /path/to/dir/or/file --delete_on_success True --fd True -t /path/to/custom/thumbnail
 ```
```

