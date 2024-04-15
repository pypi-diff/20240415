# Comparing `tmp/pa_dlna-0.8.tar.gz` & `tmp/pa_dlna-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pa_dlna-0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pa_dlna-0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pa_dlna-0.8.tar` & `pa_dlna-0.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0       94 2023-02-22 15:13:35.485494 pa_dlna-0.8/.coveragerc
--rw-r--r--   0        0        0       20 2023-10-24 08:47:40.338190 pa_dlna-0.8/.dockerignore
--rw-r--r--   0        0        0       53 2023-03-11 14:12:56.457976 pa_dlna-0.8/.gitignore
--rw-r--r--   0        0        0     1871 2024-03-24 08:08:30.875378 pa_dlna-0.8/.gitlab-ci.yml
--rw-r--r--   0        0        0      567 2024-03-24 08:08:30.875378 pa_dlna-0.8/.gitlab/issue_templates/Default.md
--rw-r--r--   0        0        0      372 2023-01-02 10:51:58.608445 pa_dlna-0.8/.readthedocs.yaml
--rw-r--r--   0        0        0      923 2023-10-24 08:28:26.899933 pa_dlna-0.8/Dockerfile.pipewire
--rw-r--r--   0        0        0     1409 2023-10-24 08:49:57.739331 pa_dlna-0.8/Dockerfile.pulse
--rw-r--r--   0        0        0     1081 2022-03-09 16:46:11.925010 pa_dlna-0.8/LICENSE
--rw-r--r--   0        0        0     4970 2023-10-29 13:29:31.842958 pa_dlna-0.8/README.rst
--rw-r--r--   0        0        0      638 2023-04-13 13:35:50.730833 pa_dlna-0.8/docs/Makefile
--rw-r--r--   0        0        0       38 2023-01-02 11:02:52.279913 pa_dlna-0.8/docs/requirements.txt
--rw-r--r--   0        0        0      945 2023-10-31 08:32:05.344108 pa_dlna-0.8/docs/source/_static/coverage.svg
--rw-r--r--   0        0        0      681 2022-12-29 10:19:08.013752 pa_dlna-0.8/docs/source/common.txt
--rw-r--r--   0        0        0     1595 2023-04-20 10:04:24.742324 pa_dlna-0.8/docs/source/conf.py
--rw-r--r--   0        0        0     9516 2024-03-12 15:45:51.278290 pa_dlna-0.8/docs/source/configuration.rst
--rw-r--r--   0        0        0     4777 2024-03-24 09:04:58.665998 pa_dlna-0.8/docs/source/default-config.rst
--rw-r--r--   0        0        0    10080 2024-03-12 16:06:47.344424 pa_dlna-0.8/docs/source/development.rst
--rw-r--r--   0        0        0     4501 2024-03-24 08:20:38.095616 pa_dlna-0.8/docs/source/history.rst
--rw-r--r--   0        0        0      608 2023-04-14 07:08:07.571321 pa_dlna-0.8/docs/source/index.rst
--rw-r--r--   0        0        0     2573 2023-10-26 13:47:32.528529 pa_dlna-0.8/docs/source/pa-dlna.rst
--rw-r--r--   0        0        0     1506 2023-04-20 10:04:24.742324 pa_dlna-0.8/docs/source/upnp-cmd.rst
--rw-r--r--   0        0        0     8303 2023-10-28 14:48:08.364436 pa_dlna-0.8/docs/source/usage.rst
--rw-r--r--   0        0        0     2766 2023-10-29 13:29:31.846292 pa_dlna-0.8/examples/libpulse.py
--rw-r--r--   0        0        0      304 2024-03-24 09:03:15.006933 pa_dlna-0.8/pa_dlna/__init__.py
--rw-r--r--   0        0        0    10365 2023-09-13 15:15:43.834929 pa_dlna-0.8/pa_dlna/config.py
--rw-r--r--   0        0        0    11883 2023-09-13 15:15:43.834929 pa_dlna-0.8/pa_dlna/encoders.py
--rw-r--r--   0        0        0    20954 2024-03-09 13:44:04.324380 pa_dlna-0.8/pa_dlna/http_server.py
--rw-r--r--   0        0        0    11073 2023-10-26 08:43:01.639143 pa_dlna-0.8/pa_dlna/init.py
--rw-r--r--   0        0        0      332 2023-10-29 13:29:31.846292 pa_dlna-0.8/pa_dlna/libpulse/__init__.py
--rw-r--r--   0        0        0    25381 2024-03-17 20:51:57.617327 pa_dlna-0.8/pa_dlna/libpulse/libpulse.py
--rw-r--r--   0        0        0    11986 2023-10-29 13:29:31.846292 pa_dlna-0.8/pa_dlna/libpulse/mainloop.py
--rw-r--r--   0        0        0     6354 2023-10-29 13:29:31.846292 pa_dlna-0.8/pa_dlna/libpulse/prototypes.py
--rw-r--r--   0        0        0     2929 2023-10-29 13:29:31.846292 pa_dlna-0.8/pa_dlna/libpulse/pulseaudio_h.py
--rw-r--r--   0        0        0     4924 2023-10-29 13:29:31.846292 pa_dlna-0.8/pa_dlna/libpulse/structures.py
--rw-r--r--   0        0        0        0 2023-10-29 13:29:31.846292 pa_dlna-0.8/pa_dlna/libpulse/tests/__init__.py
--rw-r--r--   0        0        0    10129 2023-10-29 13:29:31.846292 pa_dlna-0.8/pa_dlna/libpulse/tests/test_libpulse.py
--rw-r--r--   0        0        0    31494 2024-03-24 08:25:41.384944 pa_dlna-0.8/pa_dlna/pa_dlna.py
--rw-r--r--   0        0        0    10780 2024-03-24 08:25:41.384944 pa_dlna-0.8/pa_dlna/pulseaudio.py
--rw-r--r--   0        0        0     2221 2023-10-21 14:54:41.117483 pa_dlna-0.8/pa_dlna/tests/__init__.py
-lrwxr-xr-x   0        0        0        0 2023-02-23 08:02:35.850765 pa_dlna-0.8/pa_dlna/tests/encoder.py -> streams.py
--rw-r--r--   0        0        0     6279 2024-03-24 08:20:38.095616 pa_dlna-0.8/pa_dlna/tests/libpulse.py
-lrwxr-xr-x   0        0        0        0 2023-02-23 08:46:33.657873 pa_dlna-0.8/pa_dlna/tests/parec.py -> streams.py
--rwxr-xr-x   0        0        0    12201 2024-03-21 19:14:57.543919 pa_dlna-0.8/pa_dlna/tests/streams.py
--rw-r--r--   0        0        0    13572 2023-09-13 15:15:43.834929 pa_dlna-0.8/pa_dlna/tests/test_config.py
--rw-r--r--   0        0        0    13140 2024-03-09 13:44:04.324380 pa_dlna-0.8/pa_dlna/tests/test_http_server.py
--rw-r--r--   0        0        0    11007 2023-10-26 09:33:36.792676 pa_dlna-0.8/pa_dlna/tests/test_init.py
--rw-r--r--   0        0        0    30145 2024-03-22 08:53:55.174040 pa_dlna-0.8/pa_dlna/tests/test_pa_dlna.py
--rw-r--r--   0        0        0    11230 2024-03-24 08:20:38.095616 pa_dlna-0.8/pa_dlna/tests/test_pulseaudio.py
--rw-r--r--   0        0        0      568 2023-04-20 10:04:24.742324 pa_dlna-0.8/pa_dlna/upnp/__init__.py
--rw-r--r--   0        0        0    15351 2023-10-28 14:35:32.338240 pa_dlna-0.8/pa_dlna/upnp/network.py
--rw-r--r--   0        0        0     4677 2023-04-20 10:04:24.742324 pa_dlna-0.8/pa_dlna/upnp/tests/__init__.py
--rw-r--r--   0        0        0     4444 2023-01-30 09:51:40.021976 pa_dlna-0.8/pa_dlna/upnp/tests/device_resps.py
--rw-r--r--   0        0        0    15906 2023-10-26 09:46:05.153433 pa_dlna-0.8/pa_dlna/upnp/tests/test_network.py
--rw-r--r--   0        0        0    22638 2024-03-09 13:44:04.324380 pa_dlna-0.8/pa_dlna/upnp/tests/test_upnp.py
--rw-r--r--   0        0        0     3617 2023-06-14 13:37:47.247900 pa_dlna-0.8/pa_dlna/upnp/tests/test_util.py
--rw-r--r--   0        0        0     5073 2023-01-29 08:56:25.682591 pa_dlna-0.8/pa_dlna/upnp/tests/test_xml.py
--rw-r--r--   0        0        0    31416 2024-03-14 10:10:28.955299 pa_dlna-0.8/pa_dlna/upnp/upnp.py
--rw-r--r--   0        0        0     2806 2023-06-14 13:37:47.247900 pa_dlna-0.8/pa_dlna/upnp/util.py
--rw-r--r--   0        0        0     7571 2023-01-27 11:19:33.383315 pa_dlna-0.8/pa_dlna/upnp/xml.py
--rw-r--r--   0        0        0    20287 2024-03-09 13:44:04.324380 pa_dlna-0.8/pa_dlna/upnp_cmd.py
--rw-r--r--   0        0        0      954 2023-10-23 14:19:59.578760 pa_dlna-0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-05 15:19:20.393000 pa_dlna-0.8/tools/__init__.py
--rw-r--r--   0        0        0     1554 2022-11-05 15:19:20.393000 pa_dlna-0.8/tools/build_didl_lite.py
--rw-r--r--   0        0        0      416 2023-10-25 12:42:54.490838 pa_dlna-0.8/tools/docker-pipewire.sh
--rw-r--r--   0        0        0     1790 2023-01-02 08:45:32.674009 pa_dlna-0.8/tools/gendoc_default_config.py
--rw-r--r--   0        0        0     9383 2023-10-29 13:29:31.849625 pa_dlna-0.8/tools/parse_libpulse.py
--rw-r--r--   0        0        0      740 2023-04-20 10:04:24.745657 pa_dlna-0.8/tools/set_devpt_version_name.py
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 pa_dlna-0.8/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-02-22 15:13:35.485494 pa_dlna-0.9/.coveragerc
+-rw-r--r--   0        0        0       20 2023-10-24 08:47:40.338190 pa_dlna-0.9/.dockerignore
+-rw-r--r--   0        0        0       53 2023-03-11 14:12:56.457976 pa_dlna-0.9/.gitignore
+-rw-r--r--   0        0        0     1871 2024-03-24 08:08:30.875378 pa_dlna-0.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0      567 2024-03-24 08:08:30.875378 pa_dlna-0.9/.gitlab/issue_templates/Default.md
+-rw-r--r--   0        0        0      372 2023-01-02 10:51:58.608445 pa_dlna-0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      923 2023-10-24 08:28:26.899933 pa_dlna-0.9/Dockerfile.pipewire
+-rw-r--r--   0        0        0     1409 2023-10-24 08:49:57.739331 pa_dlna-0.9/Dockerfile.pulse
+-rw-r--r--   0        0        0     1081 2022-03-09 16:46:11.925010 pa_dlna-0.9/LICENSE
+-rw-r--r--   0        0        0     4970 2023-10-29 13:29:31.842958 pa_dlna-0.9/README.rst
+-rw-r--r--   0        0        0      638 2023-04-13 13:35:50.730833 pa_dlna-0.9/docs/Makefile
+-rw-r--r--   0        0        0       38 2023-01-02 11:02:52.279913 pa_dlna-0.9/docs/requirements.txt
+-rw-r--r--   0        0        0      945 2024-03-27 09:13:25.961385 pa_dlna-0.9/docs/source/_static/coverage.svg
+-rw-r--r--   0        0        0      681 2022-12-29 10:19:08.013752 pa_dlna-0.9/docs/source/common.txt
+-rw-r--r--   0        0        0     1595 2023-04-20 10:04:24.742324 pa_dlna-0.9/docs/source/conf.py
+-rw-r--r--   0        0        0     9516 2024-03-12 15:45:51.278290 pa_dlna-0.9/docs/source/configuration.rst
+-rw-r--r--   0        0        0     4777 2024-03-27 09:13:12.768199 pa_dlna-0.9/docs/source/default-config.rst
+-rw-r--r--   0        0        0    10080 2024-03-12 16:06:47.344424 pa_dlna-0.9/docs/source/development.rst
+-rw-r--r--   0        0        0     4631 2024-03-27 09:05:37.756207 pa_dlna-0.9/docs/source/history.rst
+-rw-r--r--   0        0        0      608 2023-04-14 07:08:07.571321 pa_dlna-0.9/docs/source/index.rst
+-rw-r--r--   0        0        0     2573 2023-10-26 13:47:32.528529 pa_dlna-0.9/docs/source/pa-dlna.rst
+-rw-r--r--   0        0        0     1506 2023-04-20 10:04:24.742324 pa_dlna-0.9/docs/source/upnp-cmd.rst
+-rw-r--r--   0        0        0     8303 2023-10-28 14:48:08.364436 pa_dlna-0.9/docs/source/usage.rst
+-rw-r--r--   0        0        0     2766 2023-10-29 13:29:31.846292 pa_dlna-0.9/examples/libpulse.py
+-rw-r--r--   0        0        0      304 2024-03-27 09:12:36.035267 pa_dlna-0.9/pa_dlna/__init__.py
+-rw-r--r--   0        0        0    10365 2023-09-13 15:15:43.834929 pa_dlna-0.9/pa_dlna/config.py
+-rw-r--r--   0        0        0    11883 2023-09-13 15:15:43.834929 pa_dlna-0.9/pa_dlna/encoders.py
+-rw-r--r--   0        0        0    20954 2024-03-09 13:44:04.324380 pa_dlna-0.9/pa_dlna/http_server.py
+-rw-r--r--   0        0        0    11073 2023-10-26 08:43:01.639143 pa_dlna-0.9/pa_dlna/init.py
+-rw-r--r--   0        0        0      332 2023-10-29 13:29:31.846292 pa_dlna-0.9/pa_dlna/libpulse/__init__.py
+-rw-r--r--   0        0        0    25577 2024-03-27 08:36:19.753051 pa_dlna-0.9/pa_dlna/libpulse/libpulse.py
+-rw-r--r--   0        0        0    11986 2023-10-29 13:29:31.846292 pa_dlna-0.9/pa_dlna/libpulse/mainloop.py
+-rw-r--r--   0        0        0     6354 2023-10-29 13:29:31.846292 pa_dlna-0.9/pa_dlna/libpulse/prototypes.py
+-rw-r--r--   0        0        0     2929 2023-10-29 13:29:31.846292 pa_dlna-0.9/pa_dlna/libpulse/pulseaudio_h.py
+-rw-r--r--   0        0        0     4924 2023-10-29 13:29:31.846292 pa_dlna-0.9/pa_dlna/libpulse/structures.py
+-rw-r--r--   0        0        0        0 2023-10-29 13:29:31.846292 pa_dlna-0.9/pa_dlna/libpulse/tests/__init__.py
+-rw-r--r--   0        0        0    10146 2024-03-27 08:35:43.836677 pa_dlna-0.9/pa_dlna/libpulse/tests/test_libpulse.py
+-rw-r--r--   0        0        0    30568 2024-03-26 19:44:12.210110 pa_dlna-0.9/pa_dlna/pa_dlna.py
+-rw-r--r--   0        0        0    10206 2024-03-26 19:44:12.210110 pa_dlna-0.9/pa_dlna/pulseaudio.py
+-rw-r--r--   0        0        0     2221 2023-10-21 14:54:41.117483 pa_dlna-0.9/pa_dlna/tests/__init__.py
+lrwxr-xr-x   0        0        0        0 2023-02-23 08:02:35.850765 pa_dlna-0.9/pa_dlna/tests/encoder.py -> streams.py
+-rw-r--r--   0        0        0     6248 2024-03-26 19:44:12.210110 pa_dlna-0.9/pa_dlna/tests/libpulse.py
+lrwxr-xr-x   0        0        0        0 2023-02-23 08:46:33.657873 pa_dlna-0.9/pa_dlna/tests/parec.py -> streams.py
+-rwxr-xr-x   0        0        0    12201 2024-03-21 19:14:57.543919 pa_dlna-0.9/pa_dlna/tests/streams.py
+-rw-r--r--   0        0        0    13572 2023-09-13 15:15:43.834929 pa_dlna-0.9/pa_dlna/tests/test_config.py
+-rw-r--r--   0        0        0    13140 2024-03-09 13:44:04.324380 pa_dlna-0.9/pa_dlna/tests/test_http_server.py
+-rw-r--r--   0        0        0    11007 2023-10-26 09:33:36.792676 pa_dlna-0.9/pa_dlna/tests/test_init.py
+-rw-r--r--   0        0        0    31239 2024-03-26 19:44:12.210110 pa_dlna-0.9/pa_dlna/tests/test_pa_dlna.py
+-rw-r--r--   0        0        0    11230 2024-03-24 08:20:38.095616 pa_dlna-0.9/pa_dlna/tests/test_pulseaudio.py
+-rw-r--r--   0        0        0      568 2023-04-20 10:04:24.742324 pa_dlna-0.9/pa_dlna/upnp/__init__.py
+-rw-r--r--   0        0        0    15351 2023-10-28 14:35:32.338240 pa_dlna-0.9/pa_dlna/upnp/network.py
+-rw-r--r--   0        0        0     4677 2023-04-20 10:04:24.742324 pa_dlna-0.9/pa_dlna/upnp/tests/__init__.py
+-rw-r--r--   0        0        0     4444 2023-01-30 09:51:40.021976 pa_dlna-0.9/pa_dlna/upnp/tests/device_resps.py
+-rw-r--r--   0        0        0    15906 2023-10-26 09:46:05.153433 pa_dlna-0.9/pa_dlna/upnp/tests/test_network.py
+-rw-r--r--   0        0        0    22638 2024-03-09 13:44:04.324380 pa_dlna-0.9/pa_dlna/upnp/tests/test_upnp.py
+-rw-r--r--   0        0        0     3617 2023-06-14 13:37:47.247900 pa_dlna-0.9/pa_dlna/upnp/tests/test_util.py
+-rw-r--r--   0        0        0     5073 2023-01-29 08:56:25.682591 pa_dlna-0.9/pa_dlna/upnp/tests/test_xml.py
+-rw-r--r--   0        0        0    31416 2024-03-14 10:10:28.955299 pa_dlna-0.9/pa_dlna/upnp/upnp.py
+-rw-r--r--   0        0        0     2806 2023-06-14 13:37:47.247900 pa_dlna-0.9/pa_dlna/upnp/util.py
+-rw-r--r--   0        0        0     7571 2023-01-27 11:19:33.383315 pa_dlna-0.9/pa_dlna/upnp/xml.py
+-rw-r--r--   0        0        0    20287 2024-03-09 13:44:04.324380 pa_dlna-0.9/pa_dlna/upnp_cmd.py
+-rw-r--r--   0        0        0      954 2023-10-23 14:19:59.578760 pa_dlna-0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-05 15:19:20.393000 pa_dlna-0.9/tools/__init__.py
+-rw-r--r--   0        0        0     1554 2022-11-05 15:19:20.393000 pa_dlna-0.9/tools/build_didl_lite.py
+-rw-r--r--   0        0        0      416 2023-10-25 12:42:54.490838 pa_dlna-0.9/tools/docker-pipewire.sh
+-rw-r--r--   0        0        0     1790 2023-01-02 08:45:32.674009 pa_dlna-0.9/tools/gendoc_default_config.py
+-rw-r--r--   0        0        0     9383 2023-10-29 13:29:31.849625 pa_dlna-0.9/tools/parse_libpulse.py
+-rw-r--r--   0        0        0      740 2023-04-20 10:04:24.745657 pa_dlna-0.9/tools/set_devpt_version_name.py
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 pa_dlna-0.9/PKG-INFO
```

### Comparing `pa_dlna-0.8/.gitlab-ci.yml` & `pa_dlna-0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/.gitlab/issue_templates/Default.md` & `pa_dlna-0.9/.gitlab/issue_templates/Default.md`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/Dockerfile.pipewire` & `pa_dlna-0.9/Dockerfile.pipewire`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/Dockerfile.pulse` & `pa_dlna-0.9/Dockerfile.pulse`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/LICENSE` & `pa_dlna-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/README.rst` & `pa_dlna-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/Makefile` & `pa_dlna-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/_static/coverage.svg` & `pa_dlna-0.9/docs/source/_static/coverage.svg`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/common.txt` & `pa_dlna-0.9/docs/source/common.txt`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/conf.py` & `pa_dlna-0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/configuration.rst` & `pa_dlna-0.9/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/default-config.rst` & `pa_dlna-0.9/docs/source/default-config.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/development.rst` & `pa_dlna-0.9/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/history.rst` & `pa_dlna-0.9/docs/source/history.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Release history
 ===============
 
+Version 0.9
+  - Support Pipewire version 1.0 and the previous version 0.3.
+  - Log the name of the sound server and its version.
+
 Version 0.8
   - Changing the volume level with ``pavucontrol`` does not interfere with the
     current audio stream.
   - Support multiple embedded MediaRenderers in a DLNA device.
   - The ``deviceList`` attribute of UPnPDevice is now a list instead of a
     dictionary.
   - Do not age an UPnP root device upon receiving a ``CACHE-CONTROL`` header
```

### Comparing `pa_dlna-0.8/docs/source/index.rst` & `pa_dlna-0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/pa-dlna.rst` & `pa_dlna-0.9/docs/source/pa-dlna.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/upnp-cmd.rst` & `pa_dlna-0.9/docs/source/upnp-cmd.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/docs/source/usage.rst` & `pa_dlna-0.9/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/examples/libpulse.py` & `pa_dlna-0.9/examples/libpulse.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/config.py` & `pa_dlna-0.9/pa_dlna/config.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/encoders.py` & `pa_dlna-0.9/pa_dlna/encoders.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/http_server.py` & `pa_dlna-0.9/pa_dlna/http_server.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/init.py` & `pa_dlna-0.9/pa_dlna/init.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/libpulse/libpulse.py` & `pa_dlna-0.9/pa_dlna/libpulse/libpulse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The ctypes interface to the libpulse library."""
 
 import asyncio
 import logging
+import re
 import ctypes as ct
 from ctypes.util import find_library
 
 from .pulseaudio_h import *
 from .mainloop import MainLoop, get_ctype, CALLBACK_TYPES, callback_func_ptr
 from .prototypes import PROTOTYPES
 from .structures import (PA_SAMPLE_SPEC, PA_CHANNEL_MAP, PA_CVOLUME,
@@ -486,27 +487,30 @@
             raise PulseOperationError(errmsg)
         return server_info
 
     async def log_server_info(self):
         if self.state[0] != 'PA_CONTEXT_READY':
             raise PulseStateError(self.state)
 
+        server_info = await self.pa_context_get_server_info()
+        server_name = server_info.server_name
+        if re.match(r'.*\d+\.\d', server_name):
+            # Pipewire includes the server version in the server name.
+            logger.info(f'Server: {server_name}')
+        else:
+            logger.info(f'Server: {server_name} {server_info.server_version}')
+
         version = pa_context_get_protocol_version(self.c_context)
         server_ver = pa_context_get_server_protocol_version(self.c_context)
         logger.debug(f'libpulse library/server versions: '
                      f'{version}/{server_ver}')
 
-        server_info = await self.pa_context_get_server_info()
-        logger.info(f'Server version: {server_info.server_version}')
-
         # 'server' is the name of the socket libpulse is connected to.
-        server_name = server_info.server_name
         server = pa_context_get_server(self.c_context)
-        logger.info(f"Connected to '{server_name}' at '{server.decode()}'")
-
+        logger.debug(f'{server_name} connected to {server.decode()}')
 
     # Private methods.
     @staticmethod
     def _success_callback(func_name, future, success):
         # 'success' may be PA_OPERATION_DONE or PA_OPERATION_CANCELLED.
         # PA_OPERATION_CANCELLED occurs "as a result of the context getting
         # disconnected while the operation is pending". We just log this event as
```

### Comparing `pa_dlna-0.8/pa_dlna/libpulse/mainloop.py` & `pa_dlna-0.9/pa_dlna/libpulse/mainloop.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/libpulse/prototypes.py` & `pa_dlna-0.9/pa_dlna/libpulse/prototypes.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/libpulse/pulseaudio_h.py` & `pa_dlna-0.9/pa_dlna/libpulse/pulseaudio_h.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/libpulse/structures.py` & `pa_dlna-0.9/pa_dlna/libpulse/structures.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/libpulse/tests/test_libpulse.py` & `pa_dlna-0.9/pa_dlna/libpulse/tests/test_libpulse.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 class LibPulseTestCase(IsolatedAsyncioTestCase):
     async def test_log_server_info(self):
         with self.assertLogs(level=logging.DEBUG) as m_logs:
             async with LibPulse('libpulse-test') as lib_pulse:
                 await lib_pulse.log_server_info()
 
         self.assertTrue(search_in_logs(m_logs.output, 'libpuls',
-                    re.compile(f'Connected to .* at')))
+                    re.compile(fr'Server: [Pp]ulse[Aa]udio.* \d+\.\d')))
 
     async def test_load_module(self):
         with self.assertLogs(level=logging.DEBUG) as m_logs:
             async with LibPulse('libpulse-test') as lib_pulse:
                 async with LoadModule(lib_pulse, 'module-null-sink',
                                       MODULE_ARG) as loaded_module:
                     pass
```

### Comparing `pa_dlna-0.8/pa_dlna/pa_dlna.py` & `pa_dlna-0.9/pa_dlna/pa_dlna.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 AUDIO_URI_PREFIX = '/audio-content'
 MEDIARENDERER = 'urn:schemas-upnp-org:device:MediaRenderer:'
 AVTRANSPORT = 'urn:upnp-org:serviceId:AVTransport'
 RENDERINGCONTROL = 'urn:upnp-org:serviceId:RenderingControl'
 CONNECTIONMANAGER = 'urn:upnp-org:serviceId:ConnectionManager'
 IGNORED_SOAPFAULTS = {'701': 'Transition not available',
                       '715': "Content 'BUSY'"}
+# Maximum time before starting a new session while waiting for the second
+# pulse event.
+NEW_SESSION_MAX_DELAY = 1
 
-UPnPAction = namedtuple('UPnPAction', ['action', 'state'])
 def get_udn(data):
     """Build an UPnP udn."""
 
     # 'hexdigest' length is 40, we will use the first 32 characters.
     hexdigest = hashlib.sha1(data).hexdigest()
     p = 0
     udn = ['uuid:']
@@ -92,15 +94,16 @@
         self.name = f'{self.getattr("modelName")}-{udn_tail}'
         self.description = f'{self.getattr("friendlyName")} - {udn_tail}'
         self.root_device_name = (f'{self.root_device.modelName}-'
                                  f'{self.root_device.udn[-5:]}')
         self.curtask = None             # Renderer.run() task
         self.closing = False
         self.nullsink = None            # NullSink instance
-        self.previous_idx = None        # index of previous sink input
+        self.previous_idx = None        # previous sink input index
+        self.exit_metadata = None       # sink input meta data at exit
         self.encoder = None
         self.mime_type = None
         self.protocol_info = None
         self.current_uri = None
         self.new_pulse_session = False
         self.suspended_state = False
         self.stream_sessions = StreamSessions(self)
@@ -180,54 +183,33 @@
 
     def match(self, uri_path):
         return uri_path == f'{AUDIO_URI_PREFIX}/{self.upnp_device.UDN}'
 
     async def start_track(self, writer):
         await self.stream_sessions.start_track(writer)
 
-    def sink_states(self, sink):
-        if sink is None:
-            sink = self.nullsink.sink
-            prev_state = sink.state
-            new_state = None
-        else:
-            prev_sink = self.nullsink.sink
-            prev_state = (prev_sink.state
-                          if prev_sink is not None else None)
-            new_state = sink.state
-        return prev_state, new_state
-
-    def log_pulse_event(self, event, prev_state, new_state, sink_input):
-        if new_state is None:
-            sink_state = f'previous state: {prev_state}'
-        else:
-            sink_state = f'prev/new state: {prev_state}/{new_state}'
+    async def push_second_event_at(self, delay, event, sink, sink_input):
+        """Push the first pulse event a second time to start a new session.
+
+        Handle the case where the second pulse event is missing.
+        """
 
+        await asyncio.sleep(delay)
+        if self.new_pulse_session:
+            self.pulse_queue.put_nowait((event, sink, sink_input))
+
+    def log_pulse_event(self, event, sink_input):
         sink_input_index = 'unknown'
         if sink_input is None:
             sink_input = self.nullsink.sink_input
         if sink_input is not None:
             sink_input_index = sink_input.index
 
         logger.debug(f"'{event}' pulse event [{self.name} "
-                     f'sink-input: idx {sink_input_index}, {sink_state}]')
-
-        if new_state == 'suspended' and not self.suspended_state:
-            self.suspended_state = True
-            logger.warning(f"'{event}' pulse event {self.name} sink-input: "
-                           f"{sink_input_index}, entering 'suspended' state")
-        elif new_state != 'suspended' and self.suspended_state:
-            self.suspended_state = False
-            logger.info(f"'{event}' pulse event {self.name} sink-input: "
-                        f"{sink_input_index}, leaving 'suspended' state")
-
-        for state in (prev_state, new_state):
-            if state not in (None, 'idle', 'running', 'suspended'):
-                logger.info(f"Expecting 'idle', 'running' or 'suspended'"
-                            f" state but found '{state}'")
+                     f'sink-input index {sink_input_index}]')
 
     def sink_input_meta(self, sink_input):
         if sink_input is None:
             return None
 
         proplist = sink_input.proplist
         publisher = proplist.get('application.name', '')
@@ -236,145 +218,132 @@
 
         if not self.encoder.track_metadata:
             title = publisher
             artist = ''
 
         return MetaData(publisher, artist, title)
 
-    async def new_session(self, metadata, state):
-        await self.set_avtransporturi(metadata, state)
-        log_action(self.name, 'Play', state)
-        await self.play()
-
     async def handle_action(self, action):
-        """An action is either 'Stop', 'Pause' or an instance of MetaData.
+        """An action is either 'Stop' or an instance of MetaData.
 
         DLNA TransportStates are 'NO_MEDIA_PRESENT', 'STOPPED' or
         'PLAYING', the other states are silently ignored.
         """
 
         # Get the stream state.
         state = await self.get_transport_state()
 
         # Space out SOAP actions that start or stop a stream.
-        if action != 'Pause' and self.encoder.soap_minimum_interval != 0:
+        if self.encoder.soap_minimum_interval != 0:
             await self.soap_spacer.wait()
 
         # Run an AVTransport action if needed.
         try:
             if state not in ('STOPPED', 'NO_MEDIA_PRESENT'):
                 if isinstance(action, MetaData):
                     if self.encoder.track_metadata:
                         await self.set_nextavtransporturi(action, state)
-                    else:
-                        await self.stop()
-                        log_action(self.name, 'Stop', state)
-                        await self.new_session(action, state)
                     return
                 elif action == 'Stop':
                     # Do not use the corresponding soap action. Let the
                     # HTTP 1.1 chunked transfer encoding handles the closing
                     # of the stream.
                     log_action(self.name, 'Closing-Stop', state)
                     await self.stream_sessions.close_session()
                     return
-                # Ignore 'Pause' events as it does not work well with
-                # streaming because of the DLNA buffering the stream.
-                # Also pulseaudio generate very short lived 'Pause'
-                # events that are annoying.
-                elif action == 'Pause':
-                    pass
-            else:
-                if isinstance(action, MetaData):
-                    await self.new_session(action, state)
-                    return
+            elif isinstance(action, MetaData):
+                await self.set_avtransporturi(action, state)
+                log_action(self.name, 'Play', state)
+                await self.play()
+                return
         except UPnPSoapFaultError as e:
             error_code = e.args[0].errorCode
             if error_code in IGNORED_SOAPFAULTS:
                 error_msg = IGNORED_SOAPFAULTS[error_code]
                 logger.warning(f"Ignoring SOAP error '{error_msg}'")
             else:
                 raise
 
         log_action(self.name, action, state, ignored=True)
 
     async def handle_pulse_event(self):
-        try:
-            handling_event = False
-            event, sink, sink_input = await self.pulse_queue.get()
-            handling_event = True
-            await self._handle_pulse_event(event, sink, sink_input)
-        finally:
-            if handling_event:
-                self.pulse_queue.task_done()
-
-    async def _handle_pulse_event(self, event, sink, sink_input):
         """Handle a PulseAudio event.
 
-        Known pulseaudio states are 'idle', 'running'.
         An event is either 'new', 'change', 'remove' or 'exit'.
-        An action is either 'Stop', 'Pause' or an instance of MetaData.
+        An action is either 'Stop' or an instance of MetaData.
         """
 
-        # The 'sink' and 'sink_input' variables define the new state.
-        # 'self.nullsink' holds the state prior to this event.
         if self.nullsink is None:
             # The Renderer instance is now temporarily disabled.
             return
 
-        prev_state, new_state = self.sink_states(sink)
-        self.log_pulse_event(event, prev_state, new_state, sink_input)
+        event, sink, sink_input = await self.pulse_queue.get()
+        self.log_pulse_event(event, sink_input)
 
         # Note that, at each pulseaudio event, a new instance of sink and
         # sink_input is generated by the libpulse library.
         if (sink_input is not None and
                 self.nullsink.sink_input is not None  and
                 sink_input.index != self.nullsink.sink_input.index):
             self.previous_idx = self.nullsink.sink_input.index
 
         # Process the event and set the new attributes values of nullsink.
         if event in ('remove', 'exit'):
-            self.nullsink.sink_input = None
-            await self.handle_action('Stop')
+            if self.nullsink.sink_input is not None:
+                if event == 'exit':
+                    self.exit_metadata = self.sink_input_meta(
+                                                    self.nullsink.sink_input)
+                self.nullsink.sink_input = None
+                await self.handle_action('Stop')
             return
 
         assert sink is not None and sink_input is not None
-        cur_metadata = self.sink_input_meta(sink_input)
-
-        # A new pulse session.
-        if (self.nullsink.sink_input is None or
-                prev_state == 'suspended' or
-                (event == 'new' and new_state == 'idle')):
-            self.new_pulse_session = True
+        try:
+            cur_metadata = self.sink_input_meta(sink_input)
+            if self.nullsink.sink_input is None:
+                self.new_pulse_session = True
+                # The reconnection of a sink-input after an exit is signaled
+                # by only one 'change' event, while a new session is signaled
+                # by two events in both PulseAudio and Pipewire, the track
+                # meta data (if any) being only available in the second one.
+                #
+                # push_second_event_at() handles the case where the second
+                # event is missing after a NEW_SESSION_MAX_DELAY delay.
+                if cur_metadata == self.exit_metadata:
+                    self.exit_metadata = None
+                else:
+                    self.control_point.cp_tasks.create_task(
+                        self.push_second_event_at(NEW_SESSION_MAX_DELAY,
+                                                  event, sink, sink_input),
+                        name='new_session_max_delay')
+                    return
 
-        if self.new_pulse_session:
-            if new_state == 'running':
+            if self.new_pulse_session:
+                self.new_pulse_session = False
                 # So that the device may display at least some useful info.
                 if not cur_metadata.title:
                     cur_metadata = cur_metadata._replace(
                                             title=cur_metadata.publisher)
-                self.new_pulse_session = False
-                await self.handle_action(cur_metadata)
-
-        elif (cur_metadata.title != '' and
-                (prev_state, new_state) == ('running', 'running')):
-            prev_metadata = self.sink_input_meta(self.nullsink.sink_input)
-            if (prev_metadata is not None and
-                    cur_metadata.title != prev_metadata.title):
                 await self.handle_action(cur_metadata)
 
-        elif (prev_state, new_state) == ('running', 'idle'):
-            await self.handle_action('Pause')
+            # A new track.
+            elif 'media.title' in sink_input.proplist:
+                prev_metadata = self.sink_input_meta(self.nullsink.sink_input)
+                # Note that if self.encoder.track_metadata is false, then
+                # cur_metadata.title == prev_metadata.title since 'title'
+                # value is 'publisher' value.
+                if (prev_metadata is not None and
+                        cur_metadata.title != prev_metadata.title):
+                    await self.handle_action(cur_metadata)
 
-        if self.nullsink is None:
-            # The Renderer instance is now temporarily disabled.
-            return
-
-        self.nullsink.sink = sink
-        self.nullsink.sink_input = sink_input
+        finally:
+            # If the Renderer instance is not temporarily disabled.
+            if self.nullsink is not None:
+                self.nullsink.sink = sink
+                self.nullsink.sink_input = sink_input
 
     async def soap_action(self, serviceId, action, args={}):
         """Send a SOAP action.
 
         Return the dict {argumentName: out arg value} if successfull,
         otherwise an instance of the upnp.xml.SoapFault namedtuple defined by
         field names in ('errorCode', 'errorDescription').
@@ -477,14 +446,16 @@
             if not await self.select_encoder(self.upnp_device.UDN):
                 return
             self.set_current_uri()
             logger.info(f'New {self.name} renderer with {self.encoder}'
                         f" handling '{self.mime_type}'"
                         f'{NL_INDENT}URL: {self.current_uri}')
 
+            # Handle the case where pa-dlna is started after streaming has
+            # started (no pulse event).
             sink_input = await self.control_point.pulse.get_sink_input(self)
             if sink_input is not None:
                 logger.info(f"Streaming '{sink_input.name}' on {self.name}")
                 self.nullsink.sink_input = sink_input
                 cur_metadata = self.sink_input_meta(sink_input)
                 if not cur_metadata.title:
                     cur_metadata = cur_metadata._replace(
```

### Comparing `pa_dlna-0.8/pa_dlna/pulseaudio.py` & `pa_dlna-0.9/pa_dlna/pulseaudio.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,17 +160,16 @@
         """Dispatch the event to a renderer.
 
         event.type is either 'new', 'change' or 'remove'.
         A new event.index is generated by pulseaudio for each 'new' event. The
         index of a 'remove' event refers to the index of a previous 'new'
         event.
 
-        A 'new' event establishes an association between a sink-input and (to)
-        a sink. A 'change' event signals a change in the metadata of the
-        stream.
+        A 'new' event establishes an association between a sink-input and
+        a sink.
 
         IMPORTANT:
         'nullsink.sink' and 'nullsink.sink_input' are the renderer's instances
         built from one of the previous events. They are stale instances.
         'sink' and 'sink_input' returned by find_renderer() and
         get_sink_by_name() are the current instances as set by pulseaudio.
         """
@@ -194,33 +193,26 @@
                 return
 
             # 'renderer.nullsink.sink' is the stale sink from the previous
             # event, we need to fetch the 'sink' correponding to this event.
             sink = await self.lib_pulse.pa_context_get_sink_info_by_name(
                                                 renderer.nullsink.sink.name)
             if sink is not None:
-                prev_state, new_state = renderer.sink_states(sink)
-                no_change = self.is_ignored_event(sink_input, event)
-                if no_change and prev_state == new_state:
+                if (self.is_ignored_event(sink_input, event) and
+                        event.type not in ('new', 'remove')):
                     # Ignore a SinkInputEvent with no changes from the
                     # previous one (or if the previous one does not exist) and
-                    # the sink state has not changed.
+                    # the event type is `change`.
                     pass
                 elif sink_input.index == renderer.previous_idx:
                     # Ignore event related to the previous sink-input.
                     pass
                 else:
                     renderer.pulse_queue.put_nowait(
                                                 (evt_type, sink, sink_input))
-                    # Upon stopping a stream, libpulse emits a batch of weird
-                    # sink state changes and sometimes a batch of them for the
-                    # same change. This is the reason why we have to wait
-                    # for the change to be fully handled by the Renderer.
-                    if no_change and prev_state != new_state:
-                        await renderer.pulse_queue.join()
 
         prev_renderer = self.find_previous_renderer(event)
         # The sink_input has been re-routed to another sink.
         if prev_renderer is not None and prev_renderer is not renderer:
             # Build our own 'exit' event (pulseaudio does not provide one)
             # for the sink that had been previously connected to this
             # sink_input.
```

### Comparing `pa_dlna-0.8/pa_dlna/tests/__init__.py` & `pa_dlna-0.9/pa_dlna/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/tests/libpulse.py` & `pa_dlna-0.9/pa_dlna/tests/libpulse.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 
 class Sink:
     index = 0
 
     def __init__(self, name, owner_module=None):
         self.name = name
         self.owner_module = owner_module
-        self.state = 'ignored'
         self.sink_input = None
 
         self.index = Sink.index
         Sink.index += 1
 
     def __str__(self):
         return self.name
```

### Comparing `pa_dlna-0.8/pa_dlna/tests/streams.py` & `pa_dlna-0.9/pa_dlna/tests/streams.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/tests/test_config.py` & `pa_dlna-0.9/pa_dlna/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/tests/test_http_server.py` & `pa_dlna-0.9/pa_dlna/tests/test_http_server.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/tests/test_init.py` & `pa_dlna-0.9/pa_dlna/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/tests/test_pa_dlna.py` & `pa_dlna-0.9/pa_dlna/tests/test_pa_dlna.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,16 +92,15 @@
             self.deviceType = 'some device type'
 
         loopback = '127.0.0.1'
         super().__init__(upnp_control_point, self.udn, loopback, loopback,
                          None, 3600)
 
 class Sink:
-    def __init__(self, state):
-        self.state = state
+    pass
 
 class SinkInput:
     def __init__(self, index=0, proplist=None):
         self.index = index
         self.proplist = proplist if proplist is not None else PROPLIST.copy()
 
 class PaDlnaTestCase(IsolatedAsyncioTestCase):
@@ -400,61 +399,63 @@
                                 re.compile('Ignore disabled UPnPRootDevice')))
 
 class PulseEventContext:
     """The context set before running handle_pulse_event() tests.
 
     The context is made of 'renderer', 'sink' and 'sink_input'.
     'sink' and 'sink_input' are either both None or both not None.
-    In the last case, this is interpreted as a change of the pulseaudio state.
     """
 
     def __init__(self,
-                 previous_idx=None,
-                 prev_sink_state='idle',
+                 sink=None,
                  prev_sink_input_index = None,
-                 sink_state=None,
                  sink_input_index=None,
                  sink_input_proplist=None):
 
-        is_index = isinstance(sink_input_index, int)
-        assert (all((sink_state, is_index)) or
-                all((not sink_state, not is_index)))
+        assert ((sink is None and sink_input_index is None) or
+                (sink is not None and sink_input_index is not None))
 
         # Build the renderer.
         upnp_control_point = UPnPControlPoint(nics=[], msearch_interval=60)
         control_point = AVControlPoint()
         control_point.upnp_control_point = upnp_control_point
         _set_control_point(control_point)
 
         root_device = RootDevice(upnp_control_point)
         renderers_list = RenderersList(control_point, root_device)
 
         # Note that self.renderer is not appended to renderers_list as this is
         # not needed.
         self.renderer = Renderer(control_point, root_device, renderers_list)
-        self.renderer.previous_idx = previous_idx
 
         # Set the value of Renderer.nullsink.
-        prev_sink = Sink(prev_sink_state)
+        prev_sink = Sink()
         nullsink = pulseaudio.NullSink(prev_sink)
         if prev_sink_input_index is not None:
             nullsink.sink_input = SinkInput(prev_sink_input_index)
         self.renderer.nullsink = nullsink
 
         # Build the sink.
-        self.sink = Sink(sink_state) if sink_state is not None else None
+        self.sink = sink
 
         # Build the sink_input.
         self.sink_input = (SinkInput(sink_input_index, sink_input_proplist) if
-                           is_index else None)
+                           sink_input_index is not None else None)
 
 class PatchSoapActionTests(IsolatedAsyncioTestCase):
     """Test cases using patch_soap_action()."""
 
-    async def patch_soap_action(self, event, ctx, transport_state='PLAYING',
+    @staticmethod
+    async def select_encoder(ctx):
+        if ctx.renderer.encoder is None:
+            await ctx.renderer.select_encoder(ctx.renderer.root_device.udn)
+        else:
+            ctx.renderer.encoder.soap_minimum_interval = 0
+
+    async def patch_soap_action(self, event, ctx, transport_state='STOPPED',
                                 track_metadata=True,
                                 soap_minimum_interval=None):
         async def soap_action(renderer, serviceId, action, args={}):
             if action == 'GetProtocolInfo':
                 return {'Source': None,
                         'Sink': 'http-get:*:audio/mp3:*'
                         }
@@ -464,144 +465,216 @@
                 result.append((serviceId, action, args))
 
         result = []
         with mock.patch.object(Renderer, 'soap_action', soap_action),\
                 self.assertLogs(level=logging.DEBUG) as m_logs:
             # Select the encoder: Renderer.sink_input_meta() needs
             # to read the Renderer.encoder.track_metadata attribute.
-            await ctx.renderer.select_encoder(ctx.renderer.root_device.udn)
-            ctx.renderer.encoder.track_metadata = track_metadata
+            await self.select_encoder(ctx)
+            renderer = ctx.renderer
+            renderer.encoder.track_metadata = track_metadata
             if soap_minimum_interval is not None:
-                ctx.renderer.soap_spacer.next_soap_at = (time.monotonic() +
-                                                         soap_minimum_interval)
+                renderer.encoder.soap_minimum_interval = soap_minimum_interval
+                renderer.soap_spacer.next_soap_at = (time.monotonic() +
+                                                     soap_minimum_interval)
 
-            ctx.renderer.pulse_queue.put_nowait((event, ctx.sink,
+            renderer.pulse_queue.put_nowait((event, ctx.sink,
                                                  ctx.sink_input))
-            await ctx.renderer.handle_pulse_event()
+            await renderer.handle_pulse_event()
 
         return result, m_logs
 
     async def test_remove_event(self):
-        ctx = PulseEventContext(prev_sink_state='running',
-                                prev_sink_input_index=0)
+        index = 999
+        ctx = PulseEventContext(prev_sink_input_index=index)
         self.assertEqual(ctx.sink, None)
         self.assertTrue(ctx.renderer.nullsink.sink_input is not None)
         self.assertEqual(ctx.sink_input, None)
 
-        result, logs = await self.patch_soap_action('remove', ctx)
+        result, logs = await self.patch_soap_action('remove', ctx,
+                                                    transport_state='PLAYING')
 
         self.assertEqual(len(result), 0)
         self.assertEqual(ctx.renderer.nullsink.sink_input, None)
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile("'remove' pulse event .*previous state: running")))
+            re.compile(f"'remove' pulse event .* index {index}")))
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
             re.compile(
                 "'Closing-Stop' UPnP action .* device prev state: PLAYING")))
 
+    async def test_exit_metadata(self):
+        ctx = PulseEventContext(prev_sink_input_index=0)
+        self.assertEqual(ctx.sink, None)
+        self.assertTrue(ctx.renderer.nullsink.sink_input is not None)
+        self.assertEqual(ctx.sink_input, None)
+
+        await self.patch_soap_action('exit', ctx, transport_state='PLAYING')
+        self.assertTrue(ctx.renderer.exit_metadata is not None)
+
+        ctx.sink = Sink()
+        ctx.sink_input = SinkInput(1)
+        result, logs = await self.patch_soap_action('change', ctx)
+
+        self.assertEqual(ctx.renderer.exit_metadata, None)
+        self.assertEqual(len(result), 2)
+        self.assertEqual(result[0][1], 'SetAVTransportURI')
+        self.assertEqual(result[1][1], 'Play')
+
     async def test_first_track(self):
-        ctx = PulseEventContext(sink_state='running', sink_input_index=0)
+        ctx = PulseEventContext(sink=Sink(), sink_input_index=0)
         self.assertEqual(ctx.renderer.nullsink.sink_input, None)
-        del ctx.sink_input.proplist['media.title']
 
-        result, logs = await self.patch_soap_action('new', ctx,
-                                                    transport_state='STOPPED')
+        await self.patch_soap_action('new', ctx)
+        result, logs = await self.patch_soap_action('change', ctx)
 
         self.assertTrue(ctx.renderer.nullsink.sink is ctx.sink)
         self.assertTrue(ctx.renderer.nullsink.sink_input is ctx.sink_input)
         self.assertEqual(len(result), 2)
         self.assertEqual(result[0][1], 'SetAVTransportURI')
         self.assertEqual(result[1][1], 'Play')
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-                re.compile('new.* event .* prev/new state: idle/running')))
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-                re.compile("MetaData\(.* artist='Ziggy Stardust'")))
-
-    async def test_soap_minimum_interval(self):
-        ctx = PulseEventContext(sink_state='running', sink_input_index=0)
-
-        with mock.patch.object(asyncio, 'sleep') as sleep:
-            result, logs = await self.patch_soap_action('new', ctx,
-                        transport_state='STOPPED', soap_minimum_interval=5)
-        sleep.assert_called_once()
+                re.compile("MetaData\(.*artist='Ziggy Stardust'")))
 
     async def test_next_track(self):
+        index = 999
         proplist = PROPLIST.copy()
         proplist['media.title'] = 'Sticky Fingers'
-        ctx = PulseEventContext(prev_sink_state='running',
+        ctx = PulseEventContext(sink=Sink(),
                                 prev_sink_input_index=0,
-                                sink_state='running',
-                                sink_input_index=1,
+                                sink_input_index=index,
                                 sink_input_proplist=proplist)
         self.assertTrue(ctx.renderer.nullsink.sink_input is not None)
 
-        result, logs = await self.patch_soap_action('change', ctx)
+        result, logs = await self.patch_soap_action('change', ctx,
+                                                    transport_state='PLAYING')
 
         self.assertTrue(ctx.renderer.nullsink.sink is ctx.sink)
         self.assertTrue(ctx.renderer.nullsink.sink_input is ctx.sink_input)
         self.assertEqual(len(result), 1)
         self.assertEqual(result[0][1], 'SetNextAVTransportURI')
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile('change.* event .* prev/new state: running/running')))
+            re.compile(f'change.* event .* sink-input index {index}')))
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-                re.compile("MetaData\(.* artist='Ziggy Stardust'")))
+                re.compile("MetaData\(.* title='Sticky Fingers'\)")))
+
+    async def test_no_title(self):
+        # Test that an empty 'title' is replaced by the 'publisher'.
+        ctx = PulseEventContext(sink=Sink(), sink_input_index=0)
+        self.assertEqual(ctx.renderer.nullsink.sink_input, None)
+
+        await self.patch_soap_action('new', ctx)
+        proplist = PROPLIST.copy()
+        application_name = 'foo'
+        proplist['application.name'] = application_name
+        proplist['media.title'] = ''
+        ctx.sink_input.proplist = proplist
+        result, logs = await self.patch_soap_action('change', ctx)
+
+        self.assertEqual(len(result), 2)
+        self.assertEqual(result[0][1], 'SetAVTransportURI')
+        self.assertEqual(result[1][1], 'Play')
+        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
+                re.compile(f"MetaData\(.*, title='{application_name}'\)")))
 
     async def test_no_track_metadata(self):
+        # Ignore change event when:
+        #   - not new_session
+        #   - renderer.encoder.track_metadata is false
+        ctx = PulseEventContext(sink=Sink(),
+                                prev_sink_input_index=0,
+                                sink_input_index=1)
+        self.assertTrue(ctx.renderer.nullsink.sink_input is not None)
+
+        # A dummy 'change' event to select the encoder.
+        await self.patch_soap_action('change', ctx, transport_state='PLAYING')
+
+
+        ctx.renderer.encoder.track_metadata = False
+        sink_input_meta = ctx.renderer.sink_input_meta
         proplist = PROPLIST.copy()
         proplist['media.title'] = 'Sticky Fingers'
-        ctx = PulseEventContext(prev_sink_state='running',
-                                sink_state='running',
-                                sink_input_index=1,
-                                sink_input_proplist=proplist)
-        self.assertTrue(ctx.renderer.nullsink.sink_input is None)
+        ctx.renderer.nullsink.sink_input.proplist = proplist
 
+        # See the comment in the code.
+        self.assertTrue(sink_input_meta(ctx.sink_input) ==
+                   sink_input_meta(ctx.renderer.nullsink.sink_input))
         result, logs = await self.patch_soap_action('change', ctx,
-                                                    track_metadata=False)
+                                                    transport_state='PLAYING')
+        self.assertEqual(len(result), 0)
 
-        self.assertTrue(ctx.renderer.nullsink.sink is ctx.sink)
-        self.assertTrue(ctx.renderer.nullsink.sink_input is ctx.sink_input)
-        self.assertEqual(len(result), 3)
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile('change.* event .* prev/new state: running/running')))
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile("'Stop' UPnP action .* PLAYING")))
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile("'SetAVTransportURI' UPnP action .* PLAYING")))
+    async def test_change_same_metadata(self):
+        # Ignore change event when:
+        #   - not new_session
+        #   - no change in metadata
+        ctx = PulseEventContext(sink=Sink(),
+                                prev_sink_input_index=0,
+                                sink_input_index=1)
+        self.assertTrue(ctx.renderer.nullsink.sink_input is not None)
+
+        result, logs = await self.patch_soap_action('change', ctx,
+                                                    transport_state='PLAYING')
+
+        self.assertEqual(len(result), 0)
+
+    async def test_new_session_max_delay(self):
+        # Test that after Renderer.new_pulse_session is set to True, if the
+        # second event is missing, the first event event is pushed again by
+        # the 'new_session_max_delay' task.
+        async def soap_action(renderer, serviceId, action, args={}):
+            if action == 'GetProtocolInfo':
+                return {'Source': None,
+                        'Sink': 'http-get:*:audio/mp3:*'
+                        }
+            elif action == 'GetTransportInfo':
+                return {'CurrentTransportState': 'STOPPED'}
+            else:
+                result.append((serviceId, action, args))
+
+        ctx = PulseEventContext(sink=Sink(), sink_input_index=0)
+        self.assertEqual(ctx.renderer.nullsink.sink_input, None)
+
+        with mock.patch.object(pa_dlna, 'NEW_SESSION_MAX_DELAY', 0) as delay:
+            await self.patch_soap_action('new', ctx)
+            self.assertTrue(ctx.renderer.new_pulse_session)
+            await asyncio.sleep(0)
+
+            # Handle the event pushed by the 'new_session_max_delay' task.
+            result = []
+            with mock.patch.object(Renderer, 'soap_action', soap_action),\
+                    self.assertLogs(level=logging.DEBUG) as logs:
+                await ctx.renderer.handle_pulse_event()
+
+        self.assertEqual(len(result), 2)
+        self.assertEqual(result[0][1], 'SetAVTransportURI')
+        self.assertEqual(result[1][1], 'Play')
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile("'Play' UPnP action .* PLAYING")))
+                re.compile("MetaData\(.*artist='Ziggy Stardust'")))
+
+    async def test_soap_minimum_interval(self):
+        ctx = PulseEventContext(sink=Sink(), sink_input_index=0)
+
+        with mock.patch.object(asyncio, 'sleep') as sleep:
+            await self.patch_soap_action('new', ctx)
+            result, logs = await self.patch_soap_action('change', ctx,
+                                                    soap_minimum_interval=5)
+        sleep.assert_called_once()
 
     async def test_soap_fault(self):
-        ctx = PulseEventContext(sink_state='running', sink_input_index=0)
+        ctx = PulseEventContext(sink=Sink(), sink_input_index=0)
         self.assertEqual(ctx.renderer.nullsink.sink_input, None)
 
         with mock.patch.object(Renderer, 'play') as play:
             play.side_effect = UPnPSoapFaultError(SoapFault('701'))
-            result, logs = await self.patch_soap_action('new', ctx,
-                                                    transport_state='STOPPED')
+            await self.patch_soap_action('new', ctx)
+            result, logs = await self.patch_soap_action('change', ctx)
 
         play.assert_called_once()
         self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
             re.compile("Ignoring SOAP error 'Transition not available'")))
 
-    async def test_pause(self):
-        ctx = PulseEventContext(prev_sink_state='running',
-                                prev_sink_input_index=1,
-                                sink_state='idle',
-                                sink_input_index=1)
-        self.assertTrue(ctx.renderer.nullsink.sink_input is not None)
-
-        result, logs = await self.patch_soap_action('change', ctx)
-
-        self.assertTrue(ctx.renderer.nullsink.sink is ctx.sink)
-        self.assertTrue(ctx.renderer.nullsink.sink_input is ctx.sink_input)
-        self.assertEqual(len(result), 0)
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile('change.* event .* prev/new state: running/idle')))
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-            re.compile("'Pause' ignored UPnP action")))
-
     async def test_start_streaming(self):
         # Test that streaming starts when pa-dlna is started while the track
         # is already playing.
         sink_input_name = 'Orcas Ibericas'
         sink_input = LibPulseSinkInput(sink_input_name, [])
         sink_input.proplist = PROPLIST
         upnp_control_point, control_point = get_control_point([sink_input])
@@ -627,37 +700,7 @@
             await renderer.pulse_register()
             await renderer.run()
             handle_action.assert_called_once_with(
                                         renderer.sink_input_meta(sink_input))
 
         self.assertTrue(search_in_logs(m_logs.output, 'pa-dlna',
                                 re.compile(f"Streaming '{sink_input_name}'")))
-
-    async def test_in_suspended_state(self):
-        ctx = PulseEventContext(sink_state='suspended', sink_input_index=0)
-        self.assertEqual(ctx.renderer.nullsink.sink_input, None)
-
-        result, logs = await self.patch_soap_action('change', ctx,
-                                                    transport_state='STOPPED')
-
-        self.assertTrue(ctx.renderer.nullsink.sink is ctx.sink)
-        self.assertTrue(ctx.renderer.nullsink.sink_input is ctx.sink_input)
-        self.assertEqual(result, [])
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-                                    re.compile("entering 'suspended' state")))
-
-    async def test_out_suspended_state(self):
-        ctx = PulseEventContext(prev_sink_state='suspended',
-                                sink_state='running', sink_input_index=0)
-        ctx.renderer.suspended_state = 'suspended'
-        self.assertEqual(ctx.renderer.nullsink.sink_input, None)
-
-        result, logs = await self.patch_soap_action('change', ctx,
-                                                    transport_state='STOPPED')
-
-        self.assertTrue(ctx.renderer.nullsink.sink is ctx.sink)
-        self.assertTrue(ctx.renderer.nullsink.sink_input is ctx.sink_input)
-        self.assertEqual(len(result), 2)
-        self.assertEqual(result[0][1], 'SetAVTransportURI')
-        self.assertEqual(result[1][1], 'Play')
-        self.assertTrue(search_in_logs(logs.output, 'pa-dlna',
-                                    re.compile("leaving 'suspended' state")))
```

### Comparing `pa_dlna-0.8/pa_dlna/tests/test_pulseaudio.py` & `pa_dlna-0.9/pa_dlna/tests/test_pulseaudio.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/__init__.py` & `pa_dlna-0.9/pa_dlna/upnp/__init__.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/network.py` & `pa_dlna-0.9/pa_dlna/upnp/network.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/tests/__init__.py` & `pa_dlna-0.9/pa_dlna/upnp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/tests/device_resps.py` & `pa_dlna-0.9/pa_dlna/upnp/tests/device_resps.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/tests/test_network.py` & `pa_dlna-0.9/pa_dlna/upnp/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/tests/test_upnp.py` & `pa_dlna-0.9/pa_dlna/upnp/tests/test_upnp.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/tests/test_util.py` & `pa_dlna-0.9/pa_dlna/upnp/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/tests/test_xml.py` & `pa_dlna-0.9/pa_dlna/upnp/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/upnp.py` & `pa_dlna-0.9/pa_dlna/upnp/upnp.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/util.py` & `pa_dlna-0.9/pa_dlna/upnp/util.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp/xml.py` & `pa_dlna-0.9/pa_dlna/upnp/xml.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pa_dlna/upnp_cmd.py` & `pa_dlna-0.9/pa_dlna/upnp_cmd.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/pyproject.toml` & `pa_dlna-0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/tools/build_didl_lite.py` & `pa_dlna-0.9/tools/build_didl_lite.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/tools/gendoc_default_config.py` & `pa_dlna-0.9/tools/gendoc_default_config.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/tools/parse_libpulse.py` & `pa_dlna-0.9/tools/parse_libpulse.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/tools/set_devpt_version_name.py` & `pa_dlna-0.9/tools/set_devpt_version_name.py`

 * *Files identical despite different names*

### Comparing `pa_dlna-0.8/PKG-INFO` & `pa_dlna-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pa-dlna
-Version: 0.8
+Version: 0.9
 Summary: Forward pulseaudio streams to DLNA devices.
 Keywords: pulseaudio,pipewire,DLNA,UPnP,asyncio,ctypes
 Author-email: Xavier de Gaye <xdegaye@gmail.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: AsyncIO
```

