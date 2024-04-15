# Comparing `tmp/ktoolbox_pure_py-0.5.1.tar.gz` & `tmp/ktoolbox_pure_py-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktoolbox_pure_py-0.5.1.tar", max compression
+gzip compressed data, was "ktoolbox_pure_py-0.5.2.tar", max compression
```

## Comparing `ktoolbox_pure_py-0.5.1.tar` & `ktoolbox_pure_py-0.5.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1533 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/LICENSE
--rw-r--r--   0        0        0     4796 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/README.md
--rw-r--r--   0        0        0      166 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/__init__.py
--rw-r--r--   0        0        0      475 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/__main__.py
--rw-r--r--   0        0        0      949 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/_enum.py
--rw-r--r--   0        0        0      103 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/action/__init__.py
--rw-r--r--   0        0        0      192 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/action/base.py
--rw-r--r--   0        0        0     1187 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/action/fetch.py
--rw-r--r--   0        0        0     6745 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/action/job.py
--rw-r--r--   0        0        0     3233 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/action/search.py
--rw-r--r--   0        0        0     3024 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/action/utils.py
--rw-r--r--   0        0        0      172 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/__init__.py
--rw-r--r--   0        0        0     4163 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/base.py
--rw-r--r--   0        0        0       31 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/misc/__init__.py
--rw-r--r--   0        0        0      480 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/misc/get_app_version.py
--rw-r--r--   0        0        0       71 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/model/__init__.py
--rw-r--r--   0        0        0      405 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/model/announcement.py
--rw-r--r--   0        0        0      581 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/model/creator.py
--rw-r--r--   0        0        0      831 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/model/post.py
--rw-r--r--   0        0        0      116 2024-03-30 06:47:08.679419 ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/__init__.py
--rw-r--r--   0        0        0      789 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_announcement.py
--rw-r--r--   0        0        0      997 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_creator_post.py
--rw-r--r--   0        0        0      629 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_creators.py
--rw-r--r--   0        0        0      761 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_post.py
--rw-r--r--   0        0        0      836 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/api/utils.py
--rw-r--r--   0        0        0    10238 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/cli.py
--rw-r--r--   0        0        0     7572 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/configuration.py
--rw-r--r--   0        0        0       46 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/downloader/__init__.py
--rw-r--r--   0        0        0      200 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/downloader/base.py
--rw-r--r--   0        0        0     9043 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/downloader/downloader.py
--rw-r--r--   0        0        0       43 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/job/__init__.py
--rw-r--r--   0        0        0     1656 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/job/model.py
--rw-r--r--   0        0        0     6810 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/job/runner.py
--rw-r--r--   0        0        0      882 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/model.py
--rw-r--r--   0        0        0     5467 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/ktoolbox/utils.py
--rw-r--r--   0        0        0     1978 2024-03-30 06:47:08.683419 ktoolbox_pure_py-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 ktoolbox_pure_py-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/LICENSE
+-rw-r--r--   0        0        0     5054 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/README.md
+-rw-r--r--   0        0        0      166 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/__main__.py
+-rw-r--r--   0        0        0      949 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/_enum.py
+-rw-r--r--   0        0        0      103 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/base.py
+-rw-r--r--   0        0        0     1187 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/fetch.py
+-rw-r--r--   0        0        0     6803 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/job.py
+-rw-r--r--   0        0        0     3233 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/search.py
+-rw-r--r--   0        0        0     3079 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/action/utils.py
+-rw-r--r--   0        0        0      172 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/__init__.py
+-rw-r--r--   0        0        0     4163 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/base.py
+-rw-r--r--   0        0        0       31 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/misc/__init__.py
+-rw-r--r--   0        0        0      480 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/misc/get_app_version.py
+-rw-r--r--   0        0        0       71 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/announcement.py
+-rw-r--r--   0        0        0      581 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/creator.py
+-rw-r--r--   0        0        0      831 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/model/post.py
+-rw-r--r--   0        0        0      116 2024-04-15 15:56:50.450143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_announcement.py
+-rw-r--r--   0        0        0      997 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creator_post.py
+-rw-r--r--   0        0        0      629 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creators.py
+-rw-r--r--   0        0        0      761 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_post.py
+-rw-r--r--   0        0        0      836 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/api/utils.py
+-rw-r--r--   0        0        0    10238 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/cli.py
+-rw-r--r--   0        0        0     7572 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/configuration.py
+-rw-r--r--   0        0        0       67 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/base.py
+-rw-r--r--   0        0        0     9705 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/downloader.py
+-rw-r--r--   0        0        0     2913 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/downloader/utils.py
+-rw-r--r--   0        0        0       43 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/job/__init__.py
+-rw-r--r--   0        0        0     1656 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/job/model.py
+-rw-r--r--   0        0        0     6817 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/job/runner.py
+-rw-r--r--   0        0        0      882 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/model.py
+-rw-r--r--   0        0        0     3701 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/ktoolbox/utils.py
+-rw-r--r--   0        0        0     1978 2024-04-15 15:56:50.454143 ktoolbox_pure_py-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6408 1970-01-01 00:00:00.000000 ktoolbox_pure_py-0.5.2/PKG-INFO
```

### Comparing `ktoolbox_pure_py-0.5.1/LICENSE` & `ktoolbox_pure_py-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/README.md` & `ktoolbox_pure_py-0.5.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -98,14 +98,20 @@
 the downloaded files will be **skipped**.
   
 #### ⬇️🖌️ Download posts from a creator
 ```bash
 # Download all posts of the creator/artist
 ktoolbox sync-creator https://kemono.su/fanbox/user/9016
 
+# Download latest 10 posts of the creator/artist
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --length=10
+
+# Download latest No.11-No.15 posts of the creator/artist
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --offset=10 --length=5
+
 # Download posts from the creator/artist from 2024-1-1 to 2024-3-1
 ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --start-time=2024-1-1 --end-time=2024-3-1
 ```
 
 ### iOS Shortcuts
 
 Goto [Shortcuts for iOS](https://ktoolbox.readthedocs.io/latest/shortcut/) page for more details.
```

#### html2text {}

```diff
@@ -21,29 +21,32 @@
 ktoolbox.readthedocs.io/latest/commands/guide) page. #### â Get general help
 ```bash ktoolbox -h ``` #### â Get help of a command ```bash ktoolbox
 download-post -h ``` #### â¬ï¸ð¼ï¸ Download a specific post ```bash
 ktoolbox download-post https://kemono.su/fanbox/user/49494721/post/6608808 ```
 If some files failed to download, you can try to execute the command line
 again, the downloaded files will be **skipped**. #### â¬ï¸ðï¸ Download
 posts from a creator ```bash # Download all posts of the creator/artist
-ktoolbox sync-creator https://kemono.su/fanbox/user/9016 # Download posts from
-the creator/artist from 2024-1-1 to 2024-3-1 ktoolbox sync-creator https://
-kemono.su/fanbox/user/9016 --start-time=2024-1-1 --end-time=2024-3-1 ``` ###
-iOS Shortcuts Goto [Shortcuts for iOS](https://ktoolbox.readthedocs.io/latest/
-shortcut/) page for more details. ### Configuration - Download 10 files at the
-same time - Rename attachments in numerical order - Prefix the post directory
-name with its release/publish date - ... Goto [Configuration-Guide](https://
-ktoolbox.readthedocs.io/latest/configuration/guide/) page for more details. ##
-Other Branches - Pure Python branch: [ðpure-py](https://github.com/Ljzd-PRO/
-KToolBox/tree/pure-py) - Use pydantic v1 so that cargo is not needed for
-installation - For example, you can use it on iOS terminal App [a-Shell](https:
-//github.com/holzschu/a-shell) - ð[PyPI](https://pypi.org/project/ktoolbox-
-pure-py/) - Development branch: [ðdevel](https://github.com/Ljzd-PRO/
-KToolBox/tree/devel) ## About Kemono Description from https://kemono.su : >
-Kemono is a public archiver for: > > - Patreon > - Pixiv Fanbox > - Discord > -
-Fantia > - Afdian > - Boosty > - DLsite > - Gumroad > - SubscribeStar > >
-Contributors here upload content and share it here for easy searching and
-organization. \ > To get started viewing content, either search for creators on
-the artists page, or search for content on the posts page. ## Code Coverage !
-[codecov.io](https://codecov.io/gh/Ljzd-PRO/KToolBox/graphs/
-sunburst.svg?token=5XK9CYQHQN) ## License KToolBox is licensed under BSD 3-
-Clause. Copyright Â© 2023 by Ljzd-PRO.
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 # Download latest 10
+posts of the creator/artist ktoolbox sync-creator https://kemono.su/fanbox/
+user/9016 --length=10 # Download latest No.11-No.15 posts of the creator/artist
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --offset=10 --length=5
+# Download posts from the creator/artist from 2024-1-1 to 2024-3-1 ktoolbox
+sync-creator https://kemono.su/fanbox/user/9016 --start-time=2024-1-1 --end-
+time=2024-3-1 ``` ### iOS Shortcuts Goto [Shortcuts for iOS](https://
+ktoolbox.readthedocs.io/latest/shortcut/) page for more details. ###
+Configuration - Download 10 files at the same time - Rename attachments in
+numerical order - Prefix the post directory name with its release/publish date
+- ... Goto [Configuration-Guide](https://ktoolbox.readthedocs.io/latest/
+configuration/guide/) page for more details. ## Other Branches - Pure Python
+branch: [ðpure-py](https://github.com/Ljzd-PRO/KToolBox/tree/pure-py) - Use
+pydantic v1 so that cargo is not needed for installation - For example, you can
+use it on iOS terminal App [a-Shell](https://github.com/holzschu/a-shell) -
+ð[PyPI](https://pypi.org/project/ktoolbox-pure-py/) - Development branch:
+[ðdevel](https://github.com/Ljzd-PRO/KToolBox/tree/devel) ## About Kemono
+Description from https://kemono.su : > Kemono is a public archiver for: > > -
+Patreon > - Pixiv Fanbox > - Discord > - Fantia > - Afdian > - Boosty > -
+DLsite > - Gumroad > - SubscribeStar > > Contributors here upload content and
+share it here for easy searching and organization. \ > To get started viewing
+content, either search for creators on the artists page, or search for content
+on the posts page. ## Code Coverage ![codecov.io](https://codecov.io/gh/Ljzd-
+PRO/KToolBox/graphs/sunburst.svg?token=5XK9CYQHQN) ## License KToolBox is
+licensed under BSD 3-Clause. Copyright Â© 2023 by Ljzd-PRO.
```

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/_enum.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/_enum.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/action/fetch.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/action/fetch.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/action/job.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/action/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import aiofiles
 from loguru import logger
 from pathvalidate import sanitize_filename, is_valid_filename
 
 from ktoolbox._enum import PostFileTypeEnum, DataStorageNameEnum
 from ktoolbox.action import ActionRet, fetch_creator_posts, FetchInterruptError
-from ktoolbox.action.utils import generate_post_path_name, filter_posts_by_time
+from ktoolbox.action.utils import generate_post_path_name, filter_posts_by_date
 from ktoolbox.api.model import Post, Attachment
 from ktoolbox.configuration import config, PostStructureConfiguration
 from ktoolbox.job import Job, CreatorIndices
 
 __all__ = ["create_job_from_post", "create_job_from_creator"]
 
 
@@ -25,15 +25,15 @@
         post_structure: Union[PostStructureConfiguration, bool] = None,
         dump_post_data: bool = True
 ) -> List[Job]:
     """
     Create a list of download job from a post data
 
     :param post: post data
-    :param post_path: Path of the post directory
+    :param post_path: Path of the post directory, which needs to be sanitized
     :param post_structure: post path structure, ``False`` -> disable, \
      ``True`` & ``None`` -> ``config.job.post_structure``
     :param dump_post_data: Whether to dump post data (post.json) in post directory
     """
     post_path.mkdir(exist_ok=True)
 
     # Load ``PostStructureConfiguration``
@@ -105,15 +105,15 @@
         end_time: Optional[datetime]
 ) -> ActionRet[List[Job]]:
     """
     Create a list of download job from a creator
 
     :param service: The service where the post is located
     :param creator_id: The ID of the creator
-    :param path: The path for posts to download
+    :param path: The path for downloading posts, which needs to be sanitized
     :param all_pages: Fetch all posts, ``offset`` and ``length`` will be ignored if enabled
     :param offset: Result offset (or start offset)
     :param length: The number of posts to fetch
     :param save_creator_indices: Record ``CreatorIndices`` data for update posts from current creator directory
     :param mix_posts: Save all files from different posts at same path, \
      ``update_from``, ``save_creator_indices`` will be ignored if enabled
     :param start_time: Start time of the time range
@@ -143,15 +143,15 @@
     if not all_pages:
         post_list = post_list[offset % 50:][:length]
     else:
         post_list = post_list[offset % 50:]
 
     # Filter posts by publish time
     if start_time or end_time:
-        post_list = list(filter_posts_by_time(post_list, start_time, end_time))
+        post_list = list(filter_posts_by_date(post_list, start_time, end_time))
     logger.info(f"Get {len(post_list)} posts, start creating jobs")
 
     # Filter posts and generate ``CreatorIndices``
     if not mix_posts:
         if save_creator_indices:  # It's unnecessary to create indices again when ``update_from`` was provided
             indices = CreatorIndices(
                 creator_id=creator_id,
```

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/action/search.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/action/search.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/action/utils.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/action/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from loguru import logger
 from pathvalidate import sanitize_filename
 
 from ktoolbox.api.model import Post
 from ktoolbox.configuration import config
 from ktoolbox.job import CreatorIndices
 
-__all__ = ["generate_post_path_name", "filter_posts_by_time", "filter_posts_by_indices"]
+__all__ = ["generate_post_path_name", "filter_posts_by_date", "filter_posts_by_indices"]
 
 
 def generate_post_path_name(post: Post) -> str:
     """Generate directory name for post to save."""
     if config.job.post_id_as_path or not post.title:
         return post.id
     else:
@@ -30,47 +30,48 @@
                 )
             )
         except KeyError as e:
             logger.error(f"`JobConfiguration.post_dirname_format` contains invalid key: {e}")
             exit(1)
 
 
-def _match_post_time(
+def _match_post_date(
         post: Post,
-        start_time: Optional[datetime],
-        end_time: Optional[datetime]
+        start_date: Optional[datetime],
+        end_date: Optional[datetime]
 ) -> bool:
     """
-    Check if the post publish date match the time range.
+    Check if the post date match the time range.
 
     :param post: Target post object
-    :param start_time: Start time of the time range
-    :param end_time: End time of the time range
+    :param start_date: Start time of the time range
+    :param end_date: End time of the time range
     :return: Whether if the post publish date match the time range
     """
-    if start_time and post.published < start_time:
+    post_date = post.published or post.added
+    if start_date and post_date and post_date < start_date:
         return False
-    if end_time and post.published > end_time:
+    if end_date and post_date and post_date > end_date:
         return False
     return True
 
 
-def filter_posts_by_time(
+def filter_posts_by_date(
         post_list: List[Post],
-        start_time: Optional[datetime],
-        end_time: Optional[datetime]
+        start_date: Optional[datetime],
+        end_date: Optional[datetime]
 ) -> Generator[Post, Any, Any]:
     """
-    Filter posts by publish time range
+    Filter posts by publish date range
 
     :param post_list: List of posts
-    :param start_time: Start time of the time range
-    :param end_time: End time of the time range
+    :param start_date: Start time of the time range
+    :param end_date: End time of the time range
     """
-    post_filter = filter(lambda x: _match_post_time(x, start_time, end_time), post_list)
+    post_filter = filter(lambda x: _match_post_date(x, start_date, end_date), post_list)
     yield from post_filter
 
 
 def filter_posts_by_indices(posts: List[Post], indices: CreatorIndices) -> Tuple[List[Post], CreatorIndices]:
     """
     Compare and filter posts by ``CreatorIndices`` data
```

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/base.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/base.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/model/creator.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/model/creator.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/model/post.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/model/post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_announcement.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_announcement.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_creator_post.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creator_post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_creators.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_creators.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/posts/get_post.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/posts/get_post.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/api/utils.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/api/utils.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/cli.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/configuration.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/configuration.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/downloader/downloader.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/downloader/downloader.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,63 +7,68 @@
 from urllib.parse import urlparse, unquote
 
 import aiofiles
 import httpx
 import tenacity
 import tqdm.asyncio
 from loguru import logger
+from pathvalidate import sanitize_filename
 from tenacity import wait_fixed, retry_if_result, retry_if_exception
 from tenacity.stop import stop_after_attempt, stop_never
 from tqdm import tqdm as std_tqdm
 
 from ktoolbox._enum import RetCodeEnum
 from ktoolbox.configuration import config
-from ktoolbox.downloader import DownloaderRet
-from ktoolbox.utils import filename_from_headers, generate_msg
+from ktoolbox.downloader.base import DownloaderRet
+from ktoolbox.downloader.utils import filename_from_headers, duplicate_file_check
+from ktoolbox.utils import generate_msg
 
 __all__ = ["Downloader"]
 
 
 class Downloader:
+    """
+    :ivar _save_filename: The actual filename for saving.
+    """
+
     def __init__(
             self,
             url: str,
             path: Path,
             *,
             buffer_size: int = None,
             chunk_size: int = None,
-            alt_filename: str = None,
+            designated_filename: str = None,
             server_path: str = None
     ):
         # noinspection GrazieInspection
         """
         Initialize a file downloader
 
         - About filename:
-            * If ``alt_filename`` parameter is set, use it.
-            * Else if ``Content-Disposition`` is set in headers, use filename from it.
-            * Else use filename from URL 'path' part.
+            1. If ``designated_filename`` parameter is set, use it.
+            2. Else if ``Content-Disposition`` is set in headers, use filename from it.
+            3. Else use filename from 'file' part of ``server_path``.
 
         :param url: Download URL
-        :param path: Directory path to save the file
+        :param path: Directory path to save the file, which needs to be sanitized
         :param buffer_size: Number of bytes for file I/O buffer
         :param chunk_size: Number of bytes for chunk of download stream
-        :param alt_filename: Use this name if no filename given by the server
-        :param server_path: Server path of the file. if config.use_bucket is True, \
-        it will be used as save the path to the file
+        :param designated_filename: Manually specify the filename for saving, which needs to be sanitized
+        :param server_path: Server path of the file. if ``DownloaderConfiguration.use_bucket`` enabled, \
+        it will be used as the save path.
         """
 
         self._url = url
         self._path = path
         self._buffer_size = buffer_size or config.downloader.buffer_size
         self._chunk_size = chunk_size or config.downloader.chunk_size
-        # _alt_filename 是用于下载的文件名
-        self._alt_filename = alt_filename  # 用于下载的文件名
-        self._server_path = server_path  # 服务器文件路径 /hash[:1]/hash2[1:3]/hash
-        self._filename = alt_filename  # 保留用做实际文件名
+        self._designated_filename = designated_filename
+        self._server_path = server_path  # /hash[:1]/hash2[1:3]/hash
+        self._save_filename = designated_filename  # Prioritize the manually specified filename
 
         self._lock = asyncio.Lock()
         self._stop: bool = False
 
     @cached_property
     def url(self) -> str:
         """Download URL"""
@@ -83,15 +88,15 @@
     def chunk_size(self) -> int:
         """Number of bytes for chunk of download stream"""
         return self._chunk_size
 
     @property
     def filename(self) -> Optional[str]:
         """Actual filename of the download file"""
-        return self._filename
+        return self._save_filename
 
     @property
     def finished(self) -> bool:
         """
         Check if the download finished
 
         :return: ``False`` if the download **in process**, ``True`` otherwise
@@ -137,42 +142,35 @@
         :param sync_callable: Sync callable for download finished
         :param async_callable: Async callable for download finished
         :param tqdm_class: ``tqdm`` class to replace default ``tqdm.asyncio.tqdm``
         :param progress: Show progress bar
         :return: ``DownloaderRet`` which contain the actual output filename
         :raise CancelledError
         """
-        # Get filename to check if file exists
+        # Get filename to check if file exists (First-time duplicate file check)
         # Check it before request to make progress more efficiency
         server_relpath = self._server_path[1:]
         server_relpath_without_params = urlparse(server_relpath).path
         server_path_filename = unquote(Path(server_relpath_without_params).name)
-        art_file_path = self._path / (self._filename or server_path_filename)
-        check_path = art_file_path
+        # Priority order can be referenced from the constructor's documentation
+        save_filepath = self._path / (self._save_filename or server_path_filename)
 
         # Get bucket file path
-        art_bucket_file_path: Optional[Path] = None
+        bucket_file_path: Optional[Path] = None
         if config.downloader.use_bucket:
-            art_bucket_file_path = config.downloader.bucket_path / server_relpath
-            check_path = art_bucket_file_path
+            bucket_file_path = config.downloader.bucket_path / server_relpath
 
         # Check if the file exists
-        if check_path.is_file():
-            if config.downloader.use_bucket:
-                ret_msg = "Download file already exists in both bucket and local, skipping"
-                if not art_file_path.is_file():
-                    ret_msg = "Download file already exists in bucket, linking to target path"
-                    check_path.hardlink_to(art_file_path)
-            else:
-                ret_msg = "Download file already exists, skipping"
+        file_existed, ret_msg = duplicate_file_check(save_filepath, bucket_file_path)
+        if file_existed:
             return DownloaderRet(
                 code=RetCodeEnum.FileExisted,
                 message=generate_msg(
                     ret_msg,
-                    path=art_file_path
+                    path=save_filepath
                 )
             )
 
         tqdm_class: Type[std_tqdm] = tqdm_class or tqdm.asyncio.tqdm
         async with self._lock:
             async with httpx.AsyncClient(verify=config.ssl_verify) as client:
                 async with client.stream(
@@ -183,55 +181,69 @@
                 ) as res:  # type: httpx.Response
                     if res.status_code != httpx.codes.OK:
                         return DownloaderRet(
                             code=RetCodeEnum.GeneralFailure,
                             message=generate_msg(
                                 "Download failed",
                                 status_code=res.status_code,
-                                filename=art_file_path
+                                filename=save_filepath
                             )
                         )
 
-                    # Get filename
-                    filename = self._alt_filename or filename_from_headers(res.headers) or server_path_filename
-                    self._filename = filename
+                    # Get filename for saving and check if file exists (Second-time duplicate file check)
+                    # Priority order can be referenced from the constructor's documentation
+                    self._save_filename = self._designated_filename or sanitize_filename(
+                        filename_from_headers(res.headers)
+                    ) or server_path_filename
+                    save_filepath = self._path / self._save_filename
+                    file_existed, ret_msg = duplicate_file_check(save_filepath, bucket_file_path)
+                    if file_existed:
+                        return DownloaderRet(
+                            code=RetCodeEnum.FileExisted,
+                            message=generate_msg(
+                                ret_msg,
+                                path=save_filepath
+                            )
+                        )
 
                     # Download
-                    temp_filepath = Path(f"{(self._path / server_path_filename)}.{config.downloader.temp_suffix}")
+                    temp_filepath = Path(f"{save_filepath}.{config.downloader.temp_suffix}")
                     total_size = int(length_str) if (length_str := res.headers.get("Content-Length")) else None
                     async with aiofiles.open(str(temp_filepath), "wb", self._buffer_size) as f:
                         chunk_iterator = res.aiter_bytes(self._chunk_size)
                         t = tqdm_class(
-                            desc=filename,
+                            desc=self._save_filename,
                             total=total_size,
                             disable=not progress,
                             unit="iB",
                             unit_scale=True,
                             unit_divisor=1024
                         )
                         async for chunk in chunk_iterator:
                             if self._stop:
                                 raise CancelledError
                             await f.write(chunk)
                             t.update(len(chunk))  # Update progress bar
 
             # Download finished
             if config.downloader.use_bucket:
-                art_bucket_file_path.parent.mkdir(parents=True, exist_ok=True)
-                os.link(temp_filepath, art_bucket_file_path)
+                bucket_file_path.parent.mkdir(parents=True, exist_ok=True)
+                os.link(temp_filepath, bucket_file_path)
+            temp_filepath.rename(self._path / self._save_filename)
 
-            temp_filepath.rename(self._path / filename)
+            # Callbacks
             if sync_callable:
                 sync_callable(self)
             if async_callable:
                 await async_callable(self)
+
             return DownloaderRet(
-                data=filename
-            ) if filename else DownloaderRet(
+                data=self._save_filename
+            ) if self._save_filename else DownloaderRet(
                 code=RetCodeEnum.GeneralFailure,
                 message=generate_msg(
                     "Download failed",
-                    filename=self._alt_filename
+                    filename=self._designated_filename
                 )
             )
 
     __call__ = run
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/job/model.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/job/model.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/job/runner.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/job/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
             # Create downloader
             url_parts = [config.downloader.scheme, config.api.files_netloc, job.server_path, '', '', '']
             url = str(urlunparse(url_parts))
             downloader = Downloader(
                 url=url,
                 path=job.path,
-                alt_filename=job.alt_filename,
+                designated_filename=job.alt_filename,
                 server_path=job.server_path
             )
 
             # Create task
             task = asyncio.create_task(
                 downloader.run(
                     tqdm_class=self._tqdm_class,
```

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/model.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/model.py`

 * *Files identical despite different names*

### Comparing `ktoolbox_pure_py-0.5.1/ktoolbox/utils.py` & `ktoolbox_pure_py-0.5.2/ktoolbox/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import asyncio
-import cgi
 import logging
 import sys
-import urllib.parse
 from pathlib import Path
-from typing import Generic, TypeVar, Optional, Dict, List, Tuple
+from typing import Generic, TypeVar, Optional, List, Tuple
 
 import aiofiles
 from loguru import logger
 from pydantic import BaseModel
 
 from ktoolbox._enum import RetCodeEnum, DataStorageNameEnum
 from ktoolbox.configuration import config
 from ktoolbox.model import SearchResult
 
 __all__ = [
     "BaseRet",
-    "filename_from_headers",
     "generate_msg",
     "logger_init",
     "dump_search",
     "parse_webpage_url",
     "uvloop_init"
 ]
 
@@ -37,76 +34,14 @@
     class Config(BaseModel.Config):
         arbitrary_types_allowed = True
 
     def __bool__(self):
         return self.code == RetCodeEnum.Success
 
 
-def parse_header(line: str) -> Dict[str, Optional[str]]:
-    """
-    Alternative resolution for parsing header line.
-
-    Apply when ``cgi.parse_header`` is unable to use due to the deprecation of `cgi` module.
-
-    https://peps.python.org/pep-0594/#cgi
-
-    - Example:
-    ```
-    parse_header("text/html; charset=utf-8")
-    ```
-
-    - Return:
-    ```
-    {'text/html': None, 'charset': 'utf-8'}
-    ```
-
-    :param line: Header line
-    :return: Dict of header line
-    """
-    dict_value: Dict[str, Optional[str]] = {}
-    for item in line.split(";"):
-        if len(pair := item.split("=")) == 1:
-            dict_value[pair[0]] = None
-        else:
-            dict_value.setdefault(*pair)
-    return dict_value
-
-
-def filename_from_headers(headers: Dict[str, str]) -> Optional[str]:
-    """
-    Get file name from headers.
-
-    Parse from ``Content-Disposition``.
-
-    - Example:
-    ```
-    filename_from_headers('attachment;filename*=utf-8\\'\\'README%2Emd;filename="README.md"')
-    ```
-
-    - Return:
-    ```
-    README.md
-    ```
-
-    :param headers: HTTP headers
-    :return: File name
-    """
-    if not (disposition := headers.get("Content-Disposition")):
-        if not (disposition := headers.get("content-disposition")):
-            return None
-    _, options = cgi.parse_header(disposition)  # alternative: `parse_header` in `utils.py`
-    if filename := options.get("filename*"):
-        if len(name_with_charset := filename.split("''")) == 2:
-            charset, name = name_with_charset
-            return urllib.parse.unquote(name, charset)
-    if filename := options.get("filename"):
-        return urllib.parse.unquote(filename, config.downloader.encoding)
-    return None
-
-
 def generate_msg(title: str = None, **kwargs):
     """
     Generate message for ``BaseRet`` and logger
 
     :param title: Message title
     :param kwargs: Extra data
     """
```

### Comparing `ktoolbox_pure_py-0.5.1/pyproject.toml` & `ktoolbox_pure_py-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ktoolbox-pure-py"
-version = "0.5.1"
+version = "0.5.2"
 description = "A useful CLI tool for downloading posts in Kemono.party / .su (Pure Python version)"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.asia>"]
 readme = "README.md"
 homepage = "https://ktoolbox.readthedocs.io/"
 repository = "https://github.com/Ljzd-PRO/KToolBox"
 documentation = "https://ktoolbox.readthedocs.io/"
```

### Comparing `ktoolbox_pure_py-0.5.1/PKG-INFO` & `ktoolbox_pure_py-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktoolbox-pure-py
-Version: 0.5.1
+Version: 0.5.2
 Summary: A useful CLI tool for downloading posts in Kemono.party / .su (Pure Python version)
 Home-page: https://ktoolbox.readthedocs.io/
 Keywords: kemono,kemono.party,cli-app,downloader,os-independent
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.asia
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -129,14 +129,20 @@
 the downloaded files will be **skipped**.
   
 #### ⬇️🖌️ Download posts from a creator
 ```bash
 # Download all posts of the creator/artist
 ktoolbox sync-creator https://kemono.su/fanbox/user/9016
 
+# Download latest 10 posts of the creator/artist
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --length=10
+
+# Download latest No.11-No.15 posts of the creator/artist
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --offset=10 --length=5
+
 # Download posts from the creator/artist from 2024-1-1 to 2024-3-1
 ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --start-time=2024-1-1 --end-time=2024-3-1
 ```
 
 ### iOS Shortcuts
 
 Goto [Shortcuts for iOS](https://ktoolbox.readthedocs.io/latest/shortcut/) page for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ktoolbox-pure-py Version: 0.5.1 Summary: A useful
+Metadata-Version: 2.1 Name: ktoolbox-pure-py Version: 0.5.2 Summary: A useful
 CLI tool for downloading posts in Kemono.party / .su (Pure Python version)
 Home-page: https://ktoolbox.readthedocs.io/ Keywords: kemono,kemono.party,cli-
 app,downloader,os-independent Author: Ljzd-PRO Author-email: ljzd@office.ljzd-
 pro.asia Requires-Python: >=3.8,<3.12 Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -39,29 +39,32 @@
 ktoolbox.readthedocs.io/latest/commands/guide) page. #### â Get general help
 ```bash ktoolbox -h ``` #### â Get help of a command ```bash ktoolbox
 download-post -h ``` #### â¬ï¸ð¼ï¸ Download a specific post ```bash
 ktoolbox download-post https://kemono.su/fanbox/user/49494721/post/6608808 ```
 If some files failed to download, you can try to execute the command line
 again, the downloaded files will be **skipped**. #### â¬ï¸ðï¸ Download
 posts from a creator ```bash # Download all posts of the creator/artist
-ktoolbox sync-creator https://kemono.su/fanbox/user/9016 # Download posts from
-the creator/artist from 2024-1-1 to 2024-3-1 ktoolbox sync-creator https://
-kemono.su/fanbox/user/9016 --start-time=2024-1-1 --end-time=2024-3-1 ``` ###
-iOS Shortcuts Goto [Shortcuts for iOS](https://ktoolbox.readthedocs.io/latest/
-shortcut/) page for more details. ### Configuration - Download 10 files at the
-same time - Rename attachments in numerical order - Prefix the post directory
-name with its release/publish date - ... Goto [Configuration-Guide](https://
-ktoolbox.readthedocs.io/latest/configuration/guide/) page for more details. ##
-Other Branches - Pure Python branch: [ðpure-py](https://github.com/Ljzd-PRO/
-KToolBox/tree/pure-py) - Use pydantic v1 so that cargo is not needed for
-installation - For example, you can use it on iOS terminal App [a-Shell](https:
-//github.com/holzschu/a-shell) - ð[PyPI](https://pypi.org/project/ktoolbox-
-pure-py/) - Development branch: [ðdevel](https://github.com/Ljzd-PRO/
-KToolBox/tree/devel) ## About Kemono Description from https://kemono.su : >
-Kemono is a public archiver for: > > - Patreon > - Pixiv Fanbox > - Discord > -
-Fantia > - Afdian > - Boosty > - DLsite > - Gumroad > - SubscribeStar > >
-Contributors here upload content and share it here for easy searching and
-organization. \ > To get started viewing content, either search for creators on
-the artists page, or search for content on the posts page. ## Code Coverage !
-[codecov.io](https://codecov.io/gh/Ljzd-PRO/KToolBox/graphs/
-sunburst.svg?token=5XK9CYQHQN) ## License KToolBox is licensed under BSD 3-
-Clause. Copyright Â© 2023 by Ljzd-PRO.
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 # Download latest 10
+posts of the creator/artist ktoolbox sync-creator https://kemono.su/fanbox/
+user/9016 --length=10 # Download latest No.11-No.15 posts of the creator/artist
+ktoolbox sync-creator https://kemono.su/fanbox/user/9016 --offset=10 --length=5
+# Download posts from the creator/artist from 2024-1-1 to 2024-3-1 ktoolbox
+sync-creator https://kemono.su/fanbox/user/9016 --start-time=2024-1-1 --end-
+time=2024-3-1 ``` ### iOS Shortcuts Goto [Shortcuts for iOS](https://
+ktoolbox.readthedocs.io/latest/shortcut/) page for more details. ###
+Configuration - Download 10 files at the same time - Rename attachments in
+numerical order - Prefix the post directory name with its release/publish date
+- ... Goto [Configuration-Guide](https://ktoolbox.readthedocs.io/latest/
+configuration/guide/) page for more details. ## Other Branches - Pure Python
+branch: [ðpure-py](https://github.com/Ljzd-PRO/KToolBox/tree/pure-py) - Use
+pydantic v1 so that cargo is not needed for installation - For example, you can
+use it on iOS terminal App [a-Shell](https://github.com/holzschu/a-shell) -
+ð[PyPI](https://pypi.org/project/ktoolbox-pure-py/) - Development branch:
+[ðdevel](https://github.com/Ljzd-PRO/KToolBox/tree/devel) ## About Kemono
+Description from https://kemono.su : > Kemono is a public archiver for: > > -
+Patreon > - Pixiv Fanbox > - Discord > - Fantia > - Afdian > - Boosty > -
+DLsite > - Gumroad > - SubscribeStar > > Contributors here upload content and
+share it here for easy searching and organization. \ > To get started viewing
+content, either search for creators on the artists page, or search for content
+on the posts page. ## Code Coverage ![codecov.io](https://codecov.io/gh/Ljzd-
+PRO/KToolBox/graphs/sunburst.svg?token=5XK9CYQHQN) ## License KToolBox is
+licensed under BSD 3-Clause. Copyright Â© 2023 by Ljzd-PRO.
```

