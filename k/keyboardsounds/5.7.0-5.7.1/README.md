# Comparing `tmp/keyboardsounds-5.7.0.tar.gz` & `tmp/keyboardsounds-5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyboardsounds-5.7.0.tar", last modified: Tue Feb 27 16:18:06 2024, max compression
+gzip compressed data, was "keyboardsounds-5.7.1.tar", last modified: Mon Apr 15 16:44:11 2024, max compression
```

## Comparing `keyboardsounds-5.7.0.tar` & `keyboardsounds-5.7.1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.948368 keyboardsounds-5.7.0/
--rw-rw-rw-   0        0        0     1074 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/LICENSE
--rw-rw-rw-   0        0        0    13236 2024-02-27 16:18:06.947242 keyboardsounds-5.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    12307 2024-02-27 15:44:20.000000 keyboardsounds-5.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.841077 keyboardsounds-5.7.0/keyboardsounds/
--rw-rw-rw-   0        0        0     5020 2024-02-23 18:48:21.000000 keyboardsounds-5.7.0/keyboardsounds/app_detector.py
--rw-rw-rw-   0        0        0     5854 2024-02-23 19:57:34.000000 keyboardsounds-5.7.0/keyboardsounds/app_rules.py
--rw-rw-rw-   0        0        0     9517 2024-02-23 19:17:48.000000 keyboardsounds-5.7.0/keyboardsounds/audio_manager.py
--rw-rw-rw-   0        0        0     3266 2024-02-23 20:03:20.000000 keyboardsounds-5.7.0/keyboardsounds/daemon.py
--rw-rw-rw-   0        0        0     7994 2024-02-23 19:26:53.000000 keyboardsounds-5.7.0/keyboardsounds/daemon_manager.py
--rw-rw-rw-   0        0        0    10014 2024-02-27 15:49:12.000000 keyboardsounds-5.7.0/keyboardsounds/main.py
--rw-rw-rw-   0        0        0      178 2024-02-23 15:27:38.000000 keyboardsounds-5.7.0/keyboardsounds/path_resolver.py
--rw-rw-rw-   0        0        0     3234 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profile.py
--rw-rw-rw-   0        0        0    18167 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profile_builder.py
--rw-rw-rw-   0        0        0     8802 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profile_validation.py
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.829525 keyboardsounds-5.7.0/keyboardsounds/profiles/
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.862645 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_space.mp3
--rw-rw-rw-   0        0        0      980 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.873935 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
--rw-rw-rw-   0        0        0      992 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/profile.yaml
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.884826 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2924 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
--rw-rw-rw-   0        0        0      988 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.895801 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key5.mp3
--rw-rw-rw-   0        0        0     5850 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_space.mp3
--rw-rw-rw-   0        0        0      978 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_back.mp3
--rw-rw-rw-   0        0        0     1252 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_key.mp3
--rw-rw-rw-   0        0        0     1252 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.896877 keyboardsounds-5.7.0/keyboardsounds/profiles/ios/
--rw-rw-rw-   0        0        0   740450 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/ios/ios-video-recording.mp4
--rw-rw-rw-   0        0        0      638 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/ios/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.907284 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_space.mp3
--rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_enter.mp3
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_key.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.913876 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key5.mp3
--rw-rw-rw-   0        0        0      504 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/release.mp3
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.923762 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key5.mp3
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_space.mp3
--rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_back.mp3
--rw-rw-rw-   0        0        0     4596 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_key.mp3
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.928958 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/
--rw-rw-rw-   0        0        0    28336 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
--rw-rw-rw-   0        0        0    34328 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
--rw-rw-rw-   0        0        0    31488 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
--rw-rw-rw-   0        0        0    31176 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
--rw-rw-rw-   0        0        0    32228 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
--rw-rw-rw-   0        0        0    32016 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
--rw-rw-rw-   0        0        0      491 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.939364 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/
--rw-rw-rw-   0        0        0    28076 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/back.wav
--rw-rw-rw-   0        0        0    31916 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/caps.wav
--rw-rw-rw-   0        0        0    32812 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/ctrl.wav
--rw-rw-rw-   0        0        0    22316 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/ent.wav
--rw-rw-rw-   0        0        0    42540 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key1.wav
--rw-rw-rw-   0        0        0    26316 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key2.wav
--rw-rw-rw-   0        0        0    25516 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key3.wav
--rw-rw-rw-   0        0        0    25612 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key4.wav
--rw-rw-rw-   0        0        0    28300 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key5.wav
--rw-rw-rw-   0        0        0    26860 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key6.wav
--rw-rw-rw-   0        0        0      932 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/profile.yaml
--rw-rw-rw-   0        0        0    23596 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/shift.wav
--rw-rw-rw-   0        0        0    23212 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/space.wav
--rw-rw-rw-   0        0        0    38060 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/tab.wav
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.945237 keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/
--rw-rw-rw-   0        0        0    60204 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/delete.wav
--rw-rw-rw-   0        0        0   146204 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/enter.wav
--rw-rw-rw-   0        0        0    32664 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/key.wav
--rw-rw-rw-   0        0        0    31588 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/key2.wav
--rw-rw-rw-   0        0        0      579 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/profile.yaml
--rw-rw-rw-   0        0        0    35788 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/space.wav
--rw-rw-rw-   0        0        0       60 2024-02-23 06:53:09.000000 keyboardsounds-5.7.0/keyboardsounds/root.py
-drwxrwxrwx   0        0        0        0 2024-02-27 16:18:06.946241 keyboardsounds-5.7.0/keyboardsounds.egg-info/
--rw-rw-rw-   0        0        0    13236 2024-02-27 16:18:06.000000 keyboardsounds-5.7.0/keyboardsounds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6585 2024-02-27 16:18:06.000000 keyboardsounds-5.7.0/keyboardsounds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 16:18:06.000000 keyboardsounds-5.7.0/keyboardsounds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-02-27 16:18:06.000000 keyboardsounds-5.7.0/keyboardsounds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-02-27 16:18:06.000000 keyboardsounds-5.7.0/keyboardsounds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      583 2024-02-23 07:23:02.000000 keyboardsounds-5.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-27 16:18:06.948368 keyboardsounds-5.7.0/setup.cfg
--rw-rw-rw-   0        0        0      918 2024-02-23 07:23:02.000000 keyboardsounds-5.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.771730 keyboardsounds-5.7.1/
+-rw-rw-rw-   0        0        0     1074 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/LICENSE
+-rw-rw-rw-   0        0        0    12639 2024-04-15 16:44:11.770730 keyboardsounds-5.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11738 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.630010 keyboardsounds-5.7.1/keyboardsounds/
+-rw-rw-rw-   0        0        0     5020 2024-02-27 16:21:44.000000 keyboardsounds-5.7.1/keyboardsounds/app_detector.py
+-rw-rw-rw-   0        0        0     6278 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/app_rules.py
+-rw-rw-rw-   0        0        0     9942 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/audio_manager.py
+-rw-rw-rw-   0        0        0     4435 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/daemon.py
+-rw-rw-rw-   0        0        0     9894 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/daemon_manager.py
+-rw-rw-rw-   0        0        0    11909 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/main.py
+-rw-rw-rw-   0        0        0      178 2024-02-23 15:27:38.000000 keyboardsounds-5.7.1/keyboardsounds/path_resolver.py
+-rw-rw-rw-   0        0        0     3234 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profile.py
+-rw-rw-rw-   0        0        0    18167 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profile_builder.py
+-rw-rw-rw-   0        0        0     8802 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profile_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.614786 keyboardsounds-5.7.1/keyboardsounds/profiles/
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.660677 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_space.mp3
+-rw-rw-rw-   0        0        0      980 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.674914 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
+-rw-rw-rw-   0        0        0      992 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.689052 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2924 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
+-rw-rw-rw-   0        0        0      988 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.702628 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/
+-rw-rw-rw-   0        0        0     1099 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key5.mp3
+-rw-rw-rw-   0        0        0     5850 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_space.mp3
+-rw-rw-rw-   0        0        0      978 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_back.mp3
+-rw-rw-rw-   0        0        0     1252 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_key.mp3
+-rw-rw-rw-   0        0        0     1252 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.705867 keyboardsounds-5.7.1/keyboardsounds/profiles/ios/
+-rw-rw-rw-   0        0        0   740450 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/ios/ios-video-recording.mp4
+-rw-rw-rw-   0        0        0      638 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/ios/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.718926 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_space.mp3
+-rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_enter.mp3
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_key.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.726538 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key5.mp3
+-rw-rw-rw-   0        0        0      504 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/release.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.740800 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key5.mp3
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_space.mp3
+-rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_back.mp3
+-rw-rw-rw-   0        0        0     4596 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_key.mp3
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.747615 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/
+-rw-rw-rw-   0        0        0    28336 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
+-rw-rw-rw-   0        0        0    34328 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
+-rw-rw-rw-   0        0        0    31488 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
+-rw-rw-rw-   0        0        0    31176 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
+-rw-rw-rw-   0        0        0    32228 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
+-rw-rw-rw-   0        0        0    32016 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
+-rw-rw-rw-   0        0        0      491 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.762572 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/
+-rw-rw-rw-   0        0        0    28076 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/back.wav
+-rw-rw-rw-   0        0        0    31916 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/caps.wav
+-rw-rw-rw-   0        0        0    32812 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ctrl.wav
+-rw-rw-rw-   0        0        0    22316 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ent.wav
+-rw-rw-rw-   0        0        0    42540 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key1.wav
+-rw-rw-rw-   0        0        0    26316 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key2.wav
+-rw-rw-rw-   0        0        0    25516 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key3.wav
+-rw-rw-rw-   0        0        0    25612 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key4.wav
+-rw-rw-rw-   0        0        0    28300 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key5.wav
+-rw-rw-rw-   0        0        0    26860 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key6.wav
+-rw-rw-rw-   0        0        0      932 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/profile.yaml
+-rw-rw-rw-   0        0        0    23596 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/shift.wav
+-rw-rw-rw-   0        0        0    23212 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/space.wav
+-rw-rw-rw-   0        0        0    38060 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/tab.wav
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.768724 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/
+-rw-rw-rw-   0        0        0    60204 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/delete.wav
+-rw-rw-rw-   0        0        0   146204 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/enter.wav
+-rw-rw-rw-   0        0        0    32664 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key.wav
+-rw-rw-rw-   0        0        0    31588 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key2.wav
+-rw-rw-rw-   0        0        0      579 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/profile.yaml
+-rw-rw-rw-   0        0        0    35788 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/space.wav
+-rw-rw-rw-   0        0        0       60 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/root.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.770730 keyboardsounds-5.7.1/keyboardsounds.egg-info/
+-rw-rw-rw-   0        0        0    12639 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6585 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      583 2024-04-15 16:43:29.000000 keyboardsounds-5.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 16:44:11.772729 keyboardsounds-5.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      997 2024-04-15 16:43:24.000000 keyboardsounds-5.7.1/setup.py
```

### Comparing `keyboardsounds-5.7.0/LICENSE` & `keyboardsounds-5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/PKG-INFO` & `keyboardsounds-5.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyboardsounds
-Version: 5.7.0
+Version: 5.7.1
 Summary: Adds the ability to play sounds while typing on any system.
 Author: Nathan Fiscaletti
 Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
 Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 [![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
 [![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
 
 This python package will add the ability to play sounds while typing anywhere on your system. You can also create [Custom Profiles](#custom-profiles) for customized audio when typing.
 
+[Work in Progress Desktop Application](https://github.com/nathan-fiscaletti/keyboardsounds-desktop)
+
 ## Preview Video
 
 > Click to view a preview of the application.
 
 [![Preview Video](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/video-preview.png?raw=true)](https://www.youtube.com/watch?v=sWAj8zEk7sQ)
 
 ## Installation
@@ -293,24 +295,14 @@
       # sound will be mapped to.
       keys: [ backspace, delete ]
 
 ```
 
 ## Development
 
-To install the package in development mode, run the following commands.
-
-```bash
-$ git clone git@github.com:nathan-fiscaletti/keyboardsounds.git
-$ cd keyboardsounds
-$ pip install -e .
-```
-
-## Development
-
 This section is intended for developers who wish to contribute to this project. Follow the steps below to set up your development environment and start contributing.
 
 ### Prerequisites
 
 - [Git](https://git-scm.com/downloads)
 - [Python](https://www.python.org/) (version 3.7 or higher)
 - [pip](https://pip.pypa.io/en/stable/installing/) (Python package installer)
@@ -319,23 +311,23 @@
 ### Setting Up the Development Environment
 
 1. **Clone the Repository**
 
    Begin by cloning the repository to your local machine using Git:
 
    ```bash
-   git clone https://github.com/yourusername/yourprojectname.git
+   git clone https://github.com/nathan-fiscaletti/keyboardsounds.git
    ```
 
 2. **Navigate to the Project Directory**
 
    Change to the project directory:
 
    ```bash
-   cd yourprojectname
+   cd keyboardsounds
    ```
 
 3. **Create a Virtual Environment (Optional)**
 
    It's recommended to create a virtual environment to keep dependencies required by different projects separate. If you have `virtualenv` installed, create a virtual environment:
 
    ```bash
@@ -359,50 +351,31 @@
 
    ```bash
    pip install -r requirements.txt
    ```
 
 ### Running the Project Locally
 
-- To run the project, use the following command:
-
-  ```bash
-  python main.py
-  ```
-
-  Replace `main.py` with the script you wish to run. This command will execute the script and start your application.
-
-### Running Tests
+It is recommended that you install the package in editable mode to allow you to make changes to the code and see the changes reflected in the application.
 
-- Ensure that your changes do not break any existing functionality by running the tests. If the project uses a test framework (like `pytest`), you can run tests using:
+- To install the package in editable mode, use the following command:
 
   ```bash
-  pytest
+  pip install -e .
   ```
 
-  or if tests are set up with `unittest`:
-
-  ```bash
-  python -m unittest discover
-  ```
+  This command will install the package in editable mode, allowing you to make changes to the code and see the changes reflected in the application.
 
 ### Contributing
 
 Contributions are what make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 #### Submitting Pull Requests
 
-1. Fork the repository and create your branch from `main`.
-2. If you've added code, write tests for it and make sure existing tests pass.
-3. Ensure your code adheres to the project's coding conventions.
+1. Fork the repository and create your branch from `master`.
+2. If you've added code, ensure your code adheres to the project's coding conventions.
 4. Update documentation as necessary.
 5. Submit your pull request with a detailed description of your changes.
 
-Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests to us.
-
 ### Getting Help
 
-Should you have any questions or encounter issues, feel free to open an issue on the repository, and we'll do our best to address it.
-
----
-
-Make sure to adjust the content to reflect your project's specific requirements, such as the main script name, the use of a different test framework, or additional setup steps.
+Should you have any questions or encounter issues, feel free to open an issue on the repository, and I'll do my best to address it.
```

### Comparing `keyboardsounds-5.7.0/README.md` & `keyboardsounds-5.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 [![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
 [![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
 
 This python package will add the ability to play sounds while typing anywhere on your system. You can also create [Custom Profiles](#custom-profiles) for customized audio when typing.
 
+[Work in Progress Desktop Application](https://github.com/nathan-fiscaletti/keyboardsounds-desktop)
+
 ## Preview Video
 
 > Click to view a preview of the application.
 
 [![Preview Video](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/video-preview.png?raw=true)](https://www.youtube.com/watch?v=sWAj8zEk7sQ)
 
 ## Installation
@@ -279,24 +281,14 @@
       # sound will be mapped to.
       keys: [ backspace, delete ]
 
 ```
 
 ## Development
 
-To install the package in development mode, run the following commands.
-
-```bash
-$ git clone git@github.com:nathan-fiscaletti/keyboardsounds.git
-$ cd keyboardsounds
-$ pip install -e .
-```
-
-## Development
-
 This section is intended for developers who wish to contribute to this project. Follow the steps below to set up your development environment and start contributing.
 
 ### Prerequisites
 
 - [Git](https://git-scm.com/downloads)
 - [Python](https://www.python.org/) (version 3.7 or higher)
 - [pip](https://pip.pypa.io/en/stable/installing/) (Python package installer)
@@ -305,23 +297,23 @@
 ### Setting Up the Development Environment
 
 1. **Clone the Repository**
 
    Begin by cloning the repository to your local machine using Git:
 
    ```bash
-   git clone https://github.com/yourusername/yourprojectname.git
+   git clone https://github.com/nathan-fiscaletti/keyboardsounds.git
    ```
 
 2. **Navigate to the Project Directory**
 
    Change to the project directory:
 
    ```bash
-   cd yourprojectname
+   cd keyboardsounds
    ```
 
 3. **Create a Virtual Environment (Optional)**
 
    It's recommended to create a virtual environment to keep dependencies required by different projects separate. If you have `virtualenv` installed, create a virtual environment:
 
    ```bash
@@ -345,50 +337,31 @@
 
    ```bash
    pip install -r requirements.txt
    ```
 
 ### Running the Project Locally
 
-- To run the project, use the following command:
-
-  ```bash
-  python main.py
-  ```
-
-  Replace `main.py` with the script you wish to run. This command will execute the script and start your application.
-
-### Running Tests
+It is recommended that you install the package in editable mode to allow you to make changes to the code and see the changes reflected in the application.
 
-- Ensure that your changes do not break any existing functionality by running the tests. If the project uses a test framework (like `pytest`), you can run tests using:
+- To install the package in editable mode, use the following command:
 
   ```bash
-  pytest
+  pip install -e .
   ```
 
-  or if tests are set up with `unittest`:
-
-  ```bash
-  python -m unittest discover
-  ```
+  This command will install the package in editable mode, allowing you to make changes to the code and see the changes reflected in the application.
 
 ### Contributing
 
 Contributions are what make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 #### Submitting Pull Requests
 
-1. Fork the repository and create your branch from `main`.
-2. If you've added code, write tests for it and make sure existing tests pass.
-3. Ensure your code adheres to the project's coding conventions.
+1. Fork the repository and create your branch from `master`.
+2. If you've added code, ensure your code adheres to the project's coding conventions.
 4. Update documentation as necessary.
 5. Submit your pull request with a detailed description of your changes.
 
-Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests to us.
-
 ### Getting Help
 
-Should you have any questions or encounter issues, feel free to open an issue on the repository, and we'll do our best to address it.
-
----
-
-Make sure to adjust the content to reflect your project's specific requirements, such as the main script name, the use of a different test framework, or additional setup steps.
+Should you have any questions or encounter issues, feel free to open an issue on the repository, and I'll do my best to address it.
```

### Comparing `keyboardsounds-5.7.0/keyboardsounds/app_detector.py` & `keyboardsounds-5.7.1/keyboardsounds/app_detector.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/app_rules.py` & `keyboardsounds-5.7.1/keyboardsounds/app_rules.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,34 +5,38 @@
 
 from typing import List, Optional
 
 from keyboardsounds.root import ROOT
 
 RULES_PATH = f"{ROOT}/rules.json"
 
+
 class Action(Enum):
     EXCLUSIVE = "exclusive"
     DISABLE = "disable"
     ENABLE = "enable"
 
+
 class GlobalAction(Enum):
     DISABLE = "disable"
     ENABLE = "enable"
 
+
 class Rule:
     def __init__(self, app_path: str, action: Action) -> None:
         """
         Initializes a new Rule instance.
 
         :param app_path: Path of the app the rule applies to.
         :param action: Action (from Action enum) for the app.
         """
         self.app_path = app_path
         self.action = action
 
+
 class Rules:
     def __init__(self, global_action: GlobalAction, rules: List[Rule]) -> None:
         """
         Initializes Rules instance managing app-specific rules and a global
         action.
 
         :param global_action: Default action for all apps.
@@ -59,15 +63,15 @@
         """
         # Check if the rule exists
         existing_rule = None
         for rule in self.rules:
             if rule.app_path == app_path:
                 existing_rule = rule
                 break
-        
+
         # If the rule exists, update its action
         if existing_rule:
             existing_rule.action = action
         else:
             # Otherwise, add a new rule
             self.rules.append(Rule(app_path, action))
 
@@ -83,23 +87,23 @@
         """
         Checks if a rule exists for a specific application.
 
         :param app_path: Application path to check for a rule.
         :return: True if a rule exists for the application, False otherwise.
         """
         return any(r.app_path == app_path for r in self.rules)
-    
+
     def has_exclusive_rule(self) -> bool:
         """
         Checks if there is an exclusive rule in the rules.
 
         :return: True if an exclusive rule exists, False otherwise.
         """
         return any(r.action == Action.EXCLUSIVE for r in self.rules)
-    
+
     def get_exclusive_rule(self) -> Optional[Rule]:
         """
         Retrieves the exclusive rule from the rules.
 
         :return: Rule with an exclusive action.
         """
         for r in self.rules:
@@ -110,38 +114,51 @@
     def get_action(self, app_path: str) -> Action:
         """
         Retrieves the action for a specific application.
 
         :param app_path: Application path to retrieve the action for.
         :return: Action applicable to the application.
         """
+        if self.global_action == GlobalAction.DISABLE.value:
+            for r in self.rules:
+                if r.app_path == app_path:
+                    if r.action == Action.ENABLE:
+                        return Action.ENABLE
+            return Action.DISABLE
+
         for r in self.rules:
             if r.app_path == app_path:
                 return r.action
         return Action(self.global_action.value)
-    
+
     def save(self) -> None:
         """
         Saves the current rules to the database.
 
         This function may raise exceptions related to file operations, such as
         IOError for I/O operation failures, PermissionError for insufficient
         permissions, and FileNotFoundError if the rules file is not found.
 
         Exceptions:
         - IOError: If an I/O operation fails.
         - PermissionError: If there are insufficient permissions.
         - FileNotFoundError: If the rules file does not exist.
         """
-        with open(RULES_PATH, 'w') as f:
-            json.dump({
-                "global_action": self.global_action.value,
-                "rules": [{"app_path": r.app_path, "action": r.action.value}
-                      for r in self.rules]
-            }, f)
+        with open(RULES_PATH, "w") as f:
+            json.dump(
+                {
+                    "global_action": self.global_action.value,
+                    "rules": [
+                        {"app_path": r.app_path, "action": r.action.value}
+                        for r in self.rules
+                    ],
+                },
+                f,
+            )
+
 
 def get_rules() -> Rules:
     """
     Loads and returns the rules from the database.
 
     This function may raise exceptions related to file operations, such as:
     - IOError: If an I/O operation fails.
@@ -150,27 +167,30 @@
 
     :raises IOError: If an I/O operation fails.
     :raises PermissionError: If there are insufficient permissions.
     :raises FileNotFoundError: If the file path does not exist.
     """
     __safe_create_rules()
 
-    with open(RULES_PATH, 'r') as f:
+    with open(RULES_PATH, "r") as f:
         data = json.load(f)
         return Rules(
             global_action=GlobalAction(data["global_action"]),
-            rules=[Rule(r["app_path"], Action(r["action"]))
-                   for r in data["rules"]]
+            rules=[Rule(r["app_path"], Action(r["action"])) for r in data["rules"]],
         )
 
+
 def __safe_create_rules() -> None:
     """
     Ensures the rules file exists, creating it with defaults if not.
 
     Used internally to avoid errors when file is absent.
     """
     if not os.path.exists(RULES_PATH):
-        with open(RULES_PATH, 'w') as f:
-            json.dump({
-                "global_action": GlobalAction.ENABLE.value,
-                "rules": [],
-            }, f)
+        with open(RULES_PATH, "w") as f:
+            json.dump(
+                {
+                    "global_action": GlobalAction.ENABLE.value,
+                    "rules": [],
+                },
+                f,
+            )
```

### Comparing `keyboardsounds-5.7.0/keyboardsounds/audio_manager.py` & `keyboardsounds-5.7.1/keyboardsounds/audio_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 
 from imageio_ffmpeg import get_ffmpeg_exe
 from pynput.keyboard import Key, KeyCode
 
 from keyboardsounds.profile import Profile
 
+
 class AudioManager:
     def __init__(self, profile: Profile) -> None:
         """
         Initializes the AudioManager with a given profile.
 
         Parameters:
         - profile (Profile): The profile object containing configuration
@@ -24,43 +25,56 @@
         based on the provided profile, and sets up the audio manager.
         """
         self.sounds = {}
         self.profile = profile
         self.__prime_audio_clips()
         self.__enabled = True
 
+    def set_profile(self, profile: Profile):
+        """
+        Sets a new profile for the AudioManager.
+
+        Parameters:
+        - profile (Profile): The new profile to be set for the AudioManager.
+
+        This method allows for changing the profile associated with the
+        AudioManager instance, updating the sound clips and key mappings
+        accordingly.
+        """
+        self.sounds = {}
+        self.profile = profile
+        self.__prime_audio_clips()
+
     def __prime_audio_clips(self):
         """
         Primes audio clips based on the profile configuration.
 
         This private method reads the profile configuration to determine the
         type of audio sources (e.g., video files, individual audio files) and
         prepares the audio clips accordingly. It might involve converting video
         files to audio, extracting specific segments from audio files, and
         organizing them for playback.
 
         No parameters or return values as it modifies the internal state of the
         AudioManager instance.
         """
-        if self.profile.value('profile.type') == "video-extract":
+        if self.profile.value("profile.type") == "video-extract":
             ffmpeg_exe = get_ffmpeg_exe()
-            V_FILE = self.profile.get_file_path(
-                self.profile.value('profile.video')
-            )
+            V_FILE = self.profile.get_file_path(self.profile.value("profile.video"))
             A_FILE = f"{V_FILE}.wav"
             subprocess.run(
                 [ffmpeg_exe, "-y", "-i", V_FILE, "-f", "wav", "-vn", A_FILE],
-                stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
             )
-            for source in self.profile.value('sources'):
-                self.__extract(source["id"], A_FILE,
-                               source["start"], source["end"])
+            for source in self.profile.value("sources"):
+                self.__extract(source["id"], A_FILE, source["start"], source["end"])
             os.unlink(A_FILE)
-        elif self.profile.value('profile.type') == "files":
-            for source in self.profile.value('sources'):
+        elif self.profile.value("profile.type") == "files":
+            for source in self.profile.value("sources"):
                 if isinstance(source["source"], dict):
                     source_id = source["id"]
                     press_loc = source["source"]["press"]
                     press_path = self.profile.get_file_path(press_loc)
                     release_loc = source["source"]["release"]
                     release_path = self.profile.get_file_path(release_loc)
                     press_id = f"{source_id}__press"
@@ -70,15 +84,15 @@
                     self.__extract(release_id, release_path)
 
                     press_snd = self.sounds[press_id].getbuffer().tobytes()
                     release_snd = self.sounds[release_id].getbuffer().tobytes()
 
                     self.sounds[source_id] = {
                         "press": io.BytesIO(press_snd),
-                        "release": io.BytesIO(release_snd)
+                        "release": io.BytesIO(release_snd),
                     }
                     del self.sounds[press_id]
                     del self.sounds[release_id]
                 elif type(source["source"]) == str:
                     source_id = source["id"]
                     path = self.profile.get_file_path(source["source"])
                     self.__extract(source_id, path)
@@ -97,26 +111,26 @@
                                    clip should be extracted. If None, the clip
                                    is extracted till the end of the file.
 
         This method handles both audio and video files, extracting the required
         segment and storing it in memory for quick access. The extracted audio
         clip is associated with the provided id.
         """
-        if input.endswith(('mp3', 'MP3')):
-            source = open(input, 'rb')
+        if input.endswith(("mp3", "MP3")):
+            source = open(input, "rb")
             data = source.read()
             source.close()
             self.sounds[id] = io.BytesIO(data)
         else:
-            source = wave.open(input, 'rb')
+            source = wave.open(input, "rb")
             source.setpos(int(start * source.getframerate()))
             end = end or source.getnframes() / source.getframerate()
             frames = int((end - start) * source.getframerate())
             self.sounds[id] = io.BytesIO()
-            dest = wave.open(self.sounds[id], 'wb')
+            dest = wave.open(self.sounds[id], "wb")
             dest.setparams(source.getparams())
             dest.writeframes(source.readframes(frames))
             source.close()
             self.sounds[id].seek(0)
 
     def get_sound(self, key, action: str = "press") -> Optional[io.BytesIO]:
         """
@@ -139,25 +153,25 @@
         action, taking into account any custom mappings defined in the profile.
         If no specific sound is mapped for the key, a default or random sound
         might be returned based on the profile configuration.
         """
         if not self.__enabled:
             return None
 
-        if self.profile.value('keys') is not None:
-            if self.profile.value('keys.other') is not None:
-                for mapping in self.profile.value('keys.other'):
+        if self.profile.value("keys") is not None:
+            if self.profile.value("keys.other") is not None:
+                for mapping in self.profile.value("keys.other"):
                     k_val = key.name if isinstance(key, Key) else key.char
                     if k_val in mapping["keys"]:
                         return self.__get_sound(mapping["sound"], action)
-            if self.profile.value('keys.default') is not None:
-                default_key = self.profile.value('keys.default')
+            if self.profile.value("keys.default") is not None:
+                default_key = self.profile.value("keys.default")
                 return self.__get_sound(default_key, action)
         return self.__get_sound(key=None, action=action)
-    
+
     def set_enabled(self, enabled: bool) -> None:
         """
         Enables or disables the AudioManager.
 
         Parameters:
         - enabled (bool): A boolean flag to enable (True) or disable (False)
                           the AudioManager.
@@ -186,15 +200,15 @@
         sound selection.
         """
         if key is None:
             key = list(self.sounds.keys())
         if type(key) is list:
             return self.__parse_sound(self.sounds[random.choice(key)], action)
         return self.__parse_sound(self.sounds[key], action)
-    
+
     def __parse_sound(self, sound, action: str = "press") -> io.BytesIO:
         """
         Converts a sound clip into a BytesIO object suitable for playback.
 
         Parameters:
         - sound:                  The sound clip to be parsed. Can be a direct
                                   audio clip or a dictionary containing 'press'
```

### Comparing `keyboardsounds-5.7.0/keyboardsounds/daemon_manager.py` & `keyboardsounds-5.7.1/keyboardsounds/daemon_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import sys
 import psutil
 import subprocess
 import time
 import json
+import socket
 
 import keyboardsounds.daemon as daemon
 from keyboardsounds.profile import Profile
+from keyboardsounds.external_api import ExternalAPI
+
 
 class DaemonManager:
     def __init__(self, lock_file) -> None:
         """
         Initializes the DaemonManager object with a specified lock file.
 
         Parameters:
@@ -21,14 +24,15 @@
         - None
         """
         self.__lock_file = lock_file
         self.__proc_info = None
         self.__lock_exists = False
         self.__is_daemon_process = False
         self.__proc = None
+        self.__api = None
         self.__load_status()
 
     def __load_status(self):
         """
         Loads the daemon's current status from the lock file, if it exists, and
         updates internal state accordingly. This includes checking if the lock
         file exists, reading process information, and determining if the current
@@ -66,41 +70,68 @@
                 current_name = psutil.Process().name()
                 self.__is_daemon_process = proc_name == current_name
             except ValueError:
                 pass
         else:
             self.__is_daemon_process = False
 
-    def status(self, full=False) -> str:
+    def status(self, full=False, short=False) -> str:
         """
         Returns the current status of the daemon process. Can provide a simple
         status or a full status with additional details.
 
         Parameters:
         - full (bool): If True, returns a detailed status string including
                        volume, PID, and profile. If False, returns a simple
                        status string.
+        - short (bool): If True, returns a JSON string with the status details.
 
         Returns:
         - str: The status of the daemon, which can be 'running', 'stale', or
-               'free'. If 'full' is True, additional details are included in the
-               returned string.
+               'free'. If 'full' or 'short' is True, returns a detailed status
+                string or JSON string, respectively.
         """
         if full:
             volume = self.get_volume()
             volume_status = f", Volume: {volume}%" if volume is not None else ""
             pid = self.get_pid()
             pid_status = f", PID: {pid}" if pid is not None else ""
             prof = self.get_profile()
             profile_status = f", Profile: {prof}" if prof is not None else ""
             status_text = {"running": "Running", "stale": "Stale"}.get(
                 self.status(), "Not running"
             )
             status = f"{status_text}{volume_status}{pid_status}{profile_status}"
             return f"Status: {status}"
+        elif short:
+            volume = self.get_volume()
+            pid = self.get_pid()
+            prof = self.get_profile()
+            daemon_status = self.status()
+            api_port = self.get_api_port()
+
+            user_status = None
+            if daemon_status == "running":
+                user_status = "Running"
+            else:
+                user_status = "Not running"
+
+            status = {
+                "status": daemon_status,
+                "user_status": user_status,
+                "volume": volume,
+                "pid": pid,
+                "profile": prof,
+                "api_port": api_port,
+                "lock": {
+                    "active": self.__lock_exists,
+                    "file": os.path.abspath(self.__lock_file),
+                },
+            }
+            return json.dumps(status)
         else:
             self.__load_status()
             if self.__lock_exists:
                 if self.__is_daemon_process:
                     return "running"
                 else:
                     return "stale"
@@ -153,14 +184,30 @@
         """
         self.__load_status()
         status = self.status()
         if status == "running":
             return self.__proc_info["profile"]
         return None
 
+    def get_api_port(self) -> int | None:
+        """
+        Retrieves the API port used by the daemon if it is running.
+
+        Parameters:
+        - None
+
+        Returns:
+        - str or None: The API port, or None if the daemon is not running.
+        """
+        self.__load_status()
+        status = self.status()
+        if status == "running":
+            return int(self.__proc_info["api_port"])
+        return None
+
     def try_stop(self) -> None:
         """
         Attempts to stop the daemon process if it is running or stale. Cleans up
         the lock file if necessary.
 
         Parameters:
         - None
@@ -199,33 +246,45 @@
         Returns:
         - bool: True if the daemon was started successfully, False if there was
                 an error during startup.
         """
         try:
             Profile(profile)
         except ValueError as err:
-            print(F"Error: {err}")
+            print(f"Error: {err}")
             return False
 
         status = self.status()
         if status == "running":
             self.try_stop()
             status = self.status()
 
         if status == "stale":
             self.try_stop()
 
         subprocess.Popen(
             [sys.argv[0], "start-daemon", str(volume), profile],
             creationflags=subprocess.CREATE_NO_WINDOW if os.name == "nt" else 0,
-            start_new_session=True
+            start_new_session=True,
         )
         time.sleep(1.0)
         return True
 
+    def update_lock_file(self, volume: int, profile: str):
+        with open(self.__lock_file, "w") as f:
+            json.dump(
+                {
+                    "pid": os.getpid(),
+                    "volume": volume,
+                    "profile": profile,
+                    "api_port": self.__api.port(),
+                },
+                f,
+            )
+
     def capture_daemon_initialization(self):
         """
         Captures and initializes the daemon process based on command-line
         arguments. This method is intended to be called at the start of the
         program.
 
         Parameters:
@@ -247,22 +306,21 @@
 
             profile = "ios"
             try:
                 profile = sys.argv[3]
             except:
                 pass
 
-            with open(self.__lock_file, 'w') as f:
-                json.dump({
-                    "pid": os.getpid(),
-                    "volume": volume,
-                    "profile": profile,
-                }, f)
+            api_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            api_socket.bind(("localhost", 0))
+            self.__api = ExternalAPI(api_socket, daemon.on_command)
+            self.__api.listen()
+
+            self.update_lock_file(volume, profile)
 
             LINE_BUFFERED = 1
-            f = open(os.devnull, 'w', buffering=LINE_BUFFERED)
+            f = open(os.devnull, "w", buffering=LINE_BUFFERED)
             sys.stdout = f
             sys.stderr = f
-            daemon.run(volume, profile)
+            daemon.run(self, volume, profile)
             return True
         return False
-
```

### Comparing `keyboardsounds-5.7.0/keyboardsounds/main.py` & `keyboardsounds-5.7.1/keyboardsounds/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import argparse
 import os
-import sys
-import time
+import json
 
 from sys import platform
 
-LINUX=platform.lower().startswith("linux")
-WIN32=platform.lower().startswith("win")
+LINUX = platform.lower().startswith("linux")
+WIN32 = platform.lower().startswith("win")
 
-os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
+os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
 import pygame
 
 from importlib.metadata import version
 
 from keyboardsounds.root import ROOT
 
 from keyboardsounds.daemon_manager import DaemonManager
 
 from keyboardsounds.profile import Profile
 from keyboardsounds.profile_builder import CliProfileBuilder
 
 from keyboardsounds.app_rules import Action, GlobalAction
 from keyboardsounds.app_rules import get_rules
 
+
 def main():
     if LINUX:
         if os.geteuid() != 0:
             print(
-                "warning: it is recommended that you run this program " +
-                "as root on Linux systems."
+                "warning: it is recommended that you run this program "
+                + "as root on Linux systems."
             )
 
     LOCK_FILE = f"{ROOT}/.lock"
 
     # Work around to get pygame to load mp3 files on windows
     # see https://github.com/pygame/pygame/issues/2647
     if os.name == "nt":
@@ -46,61 +46,126 @@
 
     win_messages = []
     if WIN32:
         win_messages = (
             f"  manage rules:{os.linesep * 2}"
             f"    %(prog)s <ar|add-rule> -r <rule> -a <app>{os.linesep}"
             f"    %(prog)s <rr|remove-rule> -a <app>{os.linesep}"
-            f"    %(prog)s <lr|list-rules>{os.linesep}"
+            f"    %(prog)s <lr|list-rules> [-s]{os.linesep}"
             f"    %(prog)s <sr|set-global-rule> -r <rule>{os.linesep}"
-            f"    %(prog)s <gr|get-global-rule>{os.linesep * 2}"
+            f"    %(prog)s <gr|get-global-rule> [-s]{os.linesep * 2}"
         )
 
     usage = (
-        f"usage: %(prog)s <action> [params]{os.linesep *2}"
-        f"  manage daemon:{os.linesep * 2}"
-        f"    %(prog)s start [-v <volume>] [-p <profile>]{os.linesep}"
-        f"    %(prog)s stop{os.linesep}"
-        f"    %(prog)s status{os.linesep * 2}"
-        f"  manage profiles:{os.linesep * 2}"
-        f"    %(prog)s <ap|add-profile> -z <zipfile>{os.linesep}"
-        f"    %(prog)s <rp|remove-profile> -n <profile>{os.linesep}"
-        f"    %(prog)s <lp|list-profiles>{os.linesep}"
-        f"    %(prog)s <bp|build-profile> -d <sound_dir> -o <zip_file>{os.linesep * 2}"
-    ) + win_messages + (
-        f"  other:{os.linesep * 2}"
-        f"    %(prog)s [--version|-V]{os.linesep}"
+        (
+            f"usage: %(prog)s <action> [params]{os.linesep *2}"
+            f"  manage daemon:{os.linesep * 2}"
+            f"    %(prog)s start [-v <volume>] [-p <profile>]{os.linesep}"
+            f"    %(prog)s stop{os.linesep}"
+            f"    %(prog)s status [-s]{os.linesep * 2}"
+            f"  manage profiles:{os.linesep * 2}"
+            f"    %(prog)s <ap|add-profile> -z <zipfile>{os.linesep}"
+            f"    %(prog)s <rp|remove-profile> -n <profile>{os.linesep}"
+            f"    %(prog)s <lp|list-profiles> [-s]{os.linesep}"
+            f"    %(prog)s <bp|build-profile> -d <sound_dir> -o <zip_file>{os.linesep * 2}"
+        )
+        + win_messages
+        + (f"  other:{os.linesep * 2}" f"    %(prog)s [--version|-V]{os.linesep}")
     )
 
     parser = argparse.ArgumentParser(
         prog=f"<keyboardsounds|kbs>",
         usage=argparse.SUPPRESS,
         description=f"Keyboard Sounds v{version_number}{os.linesep * 2}{usage}{os.linesep}",
-        formatter_class=argparse.RawDescriptionHelpFormatter
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
 
     parser.add_argument("action", help="The action to perform")
-    
+
     # Start Action
-    parser.add_argument("-v", "--volume", type=int, default=100, metavar="volume", help="volume of the sound effects (0-100), default 100")
-    parser.add_argument("-p", "--profile", type=str, default="ios", metavar="profile", help="sound profile to use, default 'ios'")
+    parser.add_argument(
+        "-v",
+        "--volume",
+        type=int,
+        default=100,
+        metavar="volume",
+        help="volume of the sound effects (0-100), default 100",
+    )
+    parser.add_argument(
+        "-p",
+        "--profile",
+        type=str,
+        default="ios",
+        metavar="profile",
+        help="sound profile to use, default 'ios'",
+    )
+
+    # Status Action
+    parser.add_argument(
+        "-s",
+        "--short",
+        action="store_true",
+        help="consolidate output to a single line for scripting",
+    )
 
     # Profiles
-    parser.add_argument("-n", "--name", type=str, default=None, metavar="name", help="name of the profile remove")
-    parser.add_argument("-z", "--zip", type=str, default=None, metavar="file", help="path to the zip file containing the profile to add")
+    parser.add_argument(
+        "-n",
+        "--name",
+        type=str,
+        default=None,
+        metavar="name",
+        help="name of the profile remove",
+    )
+    parser.add_argument(
+        "-z",
+        "--zip",
+        type=str,
+        default=None,
+        metavar="file",
+        help="path to the zip file containing the profile to add",
+    )
     parser.add_argument("-V", "--version", action="version", version=version_number)
 
     # Profile Builder
-    parser.add_argument("-d", "--directory", type=str, default=None, metavar="directory", help="path to the directory containing the sounds to use for the profile")
-    parser.add_argument("-o", "--output", type=str, default=None, metavar="file", help="path to the zip file to create")
+    parser.add_argument(
+        "-d",
+        "--directory",
+        type=str,
+        default=None,
+        metavar="directory",
+        help="path to the directory containing the sounds to use for the profile",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=str,
+        default=None,
+        metavar="file",
+        help="path to the zip file to create",
+    )
 
     # Rules
     if WIN32:
-        parser.add_argument("-a", "--app", type=str, default=None, metavar="app", help="absolute path to the application to add the rule for")
-        parser.add_argument("-r", "--rule", type=str, default=None, metavar="rule", help="rule to apply. must be one of 'enable', 'disable', or 'exclusive'")
+        parser.add_argument(
+            "-a",
+            "--app",
+            type=str,
+            default=None,
+            metavar="app",
+            help="absolute path to the application to add the rule for",
+        )
+        parser.add_argument(
+            "-r",
+            "--rule",
+            type=str,
+            default=None,
+            metavar="rule",
+            help="rule to apply. must be one of 'enable', 'disable', or 'exclusive'",
+        )
 
     args = parser.parse_args()
 
     if args.action == "start":
         status = dm.status()
         if status == "running":
             print("Re-configuring running instance of Keyboard Sounds daemon...")
@@ -108,17 +173,21 @@
             print("Starting Keyboard Sounds daemon...")
         if not dm.try_start(volume=args.volume, profile=args.profile):
             print("Failed to start.")
             return
         print(f"Started Keyboard Sounds.")
     elif args.action == "stop":
         stopped = dm.try_stop()
-        print("Stopped Keyboard Sounds daemon." if stopped else "Failed to stop Keyboard Sounds daemon. Is it running?")
+        print(
+            "Stopped Keyboard Sounds daemon."
+            if stopped
+            else "Failed to stop Keyboard Sounds daemon. Is it running?"
+        )
     elif args.action == "status":
-        status = dm.status(full=True)
+        status = dm.status(full=not args.short, short=args.short)
         print(f"{status}")
     elif args.action == "add-profile" or args.action == "ap":
         if args.zip is None:
             print("Please specify a zip file for the profile to add.")
             return
         Profile.add_profile(args.zip)
         return
@@ -127,78 +196,118 @@
             print("Please specify a name for the profile to remove.")
             return
         Profile.remove_profile(args.name)
         return
     elif args.action == "list-profiles" or args.action == "lp":
         profiles = [profile.metadata() for profile in Profile.list()]
 
+        if args.short:
+            print(
+                json.dumps(
+                    [
+                        {
+                            "name": profile["name"],
+                            "author": profile["author"],
+                            "description": profile["description"],
+                        }
+                        for profile in profiles
+                    ]
+                )
+            )
+            return
+
         names = [profile["name"] for profile in profiles]
-        names.append('Name')
+        names.append("Name")
         authors = [profile["author"] for profile in profiles]
-        authors.append('Author')
+        authors.append("Author")
         name_len = len(max(names, key=len))
         auth_len = len(max(authors, key=len))
 
         print(f"{os.linesep} Available profiles{os.linesep}")
         print(f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description")
         print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
         for profile in profiles:
-            print(f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}")
+            print(
+                f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
+            )
         print(os.linesep)
-
         return
     elif args.action == "build-profile" or args.action == "bp":
         if args.directory is None:
-            print("Please specify a directory containing the sounds to use for the profile.")
+            print(
+                "Please specify a directory containing the sounds to use for the profile."
+            )
             return
         if args.output is None:
             print("Please specify a zip file to create.")
             return
-        
+
         builder = CliProfileBuilder(args.directory, args.output)
         builder.start()
 
     # Rules are only available on windows
     elif WIN32 and (args.action == "list-rules" or args.action == "lr"):
+        rules = get_rules()
+
+        if args.short:
+            print(
+                json.dumps(
+                    [
+                        {"app_path": rule.app_path, "action": rule.action.value}
+                        for rule in rules.rules
+                    ]
+                )
+            )
+            return
+
         print(f"Keyboard Sounds v{version_number} - Application Rules{os.linesep}")
 
-        print(f"Use 'keyboardsounds add-rule' to add a rule for a specific application.")
-        print(f"Use 'keyboardsounds remove-rule' to remove a rule for a specific application.")
+        print(
+            f"Use 'keyboardsounds add-rule' to add a rule for a specific application."
+        )
+        print(
+            f"Use 'keyboardsounds remove-rule' to remove a rule for a specific application."
+        )
         print(f"Use 'keyboardsounds set-global-rule' to set the global rule.")
 
-        rules = get_rules()
-
         print(f"{os.linesep}Configured Rules:{os.linesep}")
 
         print(f" - Application : Global")
         print(f"   Action      : {rules.global_action.value.upper()}")
 
-        
         for rule in rules.rules:
             print("")
             print(f" - Application : {rule.app_path}")
             print(f"   Action      : {rule.action.value.upper()}")
         print("")
     elif WIN32 and (args.action == "add-rule" or args.action == "ar"):
         if args.app is None:
             print("Please specify an application to add the rule for.")
             return
         if args.rule is None:
-            print("Please specify a rule to apply. Must be one of 'enable', 'disable', or 'exclusive'.")
+            print(
+                "Please specify a rule to apply. Must be one of 'enable', 'disable', or 'exclusive'."
+            )
             return
-        
+
         args.rule = args.rule.lower()
 
         rules = get_rules()
-        if args.rule.lower() not in [Action.ENABLE.value, Action.DISABLE.value, Action.EXCLUSIVE.value]:
+        if args.rule.lower() not in [
+            Action.ENABLE.value,
+            Action.DISABLE.value,
+            Action.EXCLUSIVE.value,
+        ]:
             print("Invalid rule. Must be one of 'enable', 'disable', or 'exclusive'.")
             return
         if args.rule.lower() == Action.EXCLUSIVE.value:
             if rules.has_exclusive_rule():
-                print("Exclusive rule already exists. Only one exclusive rule can be set.")
+                print(
+                    "Exclusive rule already exists. Only one exclusive rule can be set."
+                )
                 return
         rules.set_rule(args.app, Action(args.rule))
         try:
             rules.save()
             print(f"Rule '{args.rule.upper()}' added for {args.app}.")
         except Exception as e:
             print(f"Failed to save rules: {e}")
@@ -216,15 +325,17 @@
         try:
             rules.save()
             print(f"Rule removed for {args.app}.")
         except Exception as e:
             print(f"Failed to save rules: {e}")
     elif WIN32 and (args.action == "set-global-rule" or args.action == "sr"):
         if args.rule is None:
-            print("Please specify a rule to apply. Must be one of 'enable' or 'disable'.")
+            print(
+                "Please specify a rule to apply. Must be one of 'enable' or 'disable'."
+            )
             return
 
         args.rule = args.rule.lower()
 
         if args.rule not in [Action.ENABLE.value, Action.DISABLE.value]:
             print("Invalid rule. Must be one of 'enable' or 'disable'.")
             return
@@ -241,14 +352,18 @@
         except Exception as e:
             print(f"Failed to save rules: {e}")
             return
 
         print(f"Global rule set to '{args.rule.upper()}'.")
     elif WIN32 and (args.action == "get-global-rule" or args.action == "gr"):
         rules = get_rules()
+        if args.short:
+            print(json.dumps({"global_action": rules.global_action.value}))
+            return
         print(f"Global rule is set to '{rules.global_action.value.upper()}'.")
 
     else:
         parser.print_usage()
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profile.py` & `keyboardsounds-5.7.1/keyboardsounds/profile.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profile_builder.py` & `keyboardsounds-5.7.1/keyboardsounds/profile_builder.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profile_validation.py` & `keyboardsounds-5.7.1/keyboardsounds/profile_validation.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/LICENSE` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key1.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key2.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key3.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key4.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_key5.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/press_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_key.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/alpaca/release_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/LICENSE` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/press_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_key.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-black-ink/release_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/LICENSE` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/press_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_key.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/gateron-red-ink/release_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/LICENSE` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key1.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key2.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key3.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key4.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_key5.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/press_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_key.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/holy-panda/release_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/ios/ios-video-recording.mp4` & `keyboardsounds-5.7.1/keyboardsounds/profiles/ios/ios-video-recording.mp4`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/ios/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/ios/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/LICENSE` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key1.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key2.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key3.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key4.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_key5.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/press_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_key.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-black/release_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/LICENSE` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key1.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key2.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key3.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key4.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/press_key5.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-blue/release.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/release.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/LICENSE` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key1.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key2.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key3.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key4.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_key5.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/press_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_back.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_enter.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_key.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-brown/release_space.mp3` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/back.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/back.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/caps.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/caps.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/ctrl.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ctrl.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/ent.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ent.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key1.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key2.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key3.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key4.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key5.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/key6.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/shift.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/shift.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/space.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/telios-v2/tab.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/tab.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/delete.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/delete.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/enter.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/enter.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/key.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/key2.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/profile.yaml` & `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds/profiles/typewriter/space.wav` & `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/keyboardsounds.egg-info/PKG-INFO` & `keyboardsounds-5.7.1/keyboardsounds.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyboardsounds
-Version: 5.7.0
+Version: 5.7.1
 Summary: Adds the ability to play sounds while typing on any system.
 Author: Nathan Fiscaletti
 Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
 Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,16 @@
 [![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
 [![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
 
 This python package will add the ability to play sounds while typing anywhere on your system. You can also create [Custom Profiles](#custom-profiles) for customized audio when typing.
 
+[Work in Progress Desktop Application](https://github.com/nathan-fiscaletti/keyboardsounds-desktop)
+
 ## Preview Video
 
 > Click to view a preview of the application.
 
 [![Preview Video](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/video-preview.png?raw=true)](https://www.youtube.com/watch?v=sWAj8zEk7sQ)
 
 ## Installation
@@ -293,24 +295,14 @@
       # sound will be mapped to.
       keys: [ backspace, delete ]
 
 ```
 
 ## Development
 
-To install the package in development mode, run the following commands.
-
-```bash
-$ git clone git@github.com:nathan-fiscaletti/keyboardsounds.git
-$ cd keyboardsounds
-$ pip install -e .
-```
-
-## Development
-
 This section is intended for developers who wish to contribute to this project. Follow the steps below to set up your development environment and start contributing.
 
 ### Prerequisites
 
 - [Git](https://git-scm.com/downloads)
 - [Python](https://www.python.org/) (version 3.7 or higher)
 - [pip](https://pip.pypa.io/en/stable/installing/) (Python package installer)
@@ -319,23 +311,23 @@
 ### Setting Up the Development Environment
 
 1. **Clone the Repository**
 
    Begin by cloning the repository to your local machine using Git:
 
    ```bash
-   git clone https://github.com/yourusername/yourprojectname.git
+   git clone https://github.com/nathan-fiscaletti/keyboardsounds.git
    ```
 
 2. **Navigate to the Project Directory**
 
    Change to the project directory:
 
    ```bash
-   cd yourprojectname
+   cd keyboardsounds
    ```
 
 3. **Create a Virtual Environment (Optional)**
 
    It's recommended to create a virtual environment to keep dependencies required by different projects separate. If you have `virtualenv` installed, create a virtual environment:
 
    ```bash
@@ -359,50 +351,31 @@
 
    ```bash
    pip install -r requirements.txt
    ```
 
 ### Running the Project Locally
 
-- To run the project, use the following command:
-
-  ```bash
-  python main.py
-  ```
-
-  Replace `main.py` with the script you wish to run. This command will execute the script and start your application.
-
-### Running Tests
+It is recommended that you install the package in editable mode to allow you to make changes to the code and see the changes reflected in the application.
 
-- Ensure that your changes do not break any existing functionality by running the tests. If the project uses a test framework (like `pytest`), you can run tests using:
+- To install the package in editable mode, use the following command:
 
   ```bash
-  pytest
+  pip install -e .
   ```
 
-  or if tests are set up with `unittest`:
-
-  ```bash
-  python -m unittest discover
-  ```
+  This command will install the package in editable mode, allowing you to make changes to the code and see the changes reflected in the application.
 
 ### Contributing
 
 Contributions are what make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
 
 #### Submitting Pull Requests
 
-1. Fork the repository and create your branch from `main`.
-2. If you've added code, write tests for it and make sure existing tests pass.
-3. Ensure your code adheres to the project's coding conventions.
+1. Fork the repository and create your branch from `master`.
+2. If you've added code, ensure your code adheres to the project's coding conventions.
 4. Update documentation as necessary.
 5. Submit your pull request with a detailed description of your changes.
 
-Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests to us.
-
 ### Getting Help
 
-Should you have any questions or encounter issues, feel free to open an issue on the repository, and we'll do our best to address it.
-
----
-
-Make sure to adjust the content to reflect your project's specific requirements, such as the main script name, the use of a different test framework, or additional setup steps.
+Should you have any questions or encounter issues, feel free to open an issue on the repository, and I'll do my best to address it.
```

### Comparing `keyboardsounds-5.7.0/keyboardsounds.egg-info/SOURCES.txt` & `keyboardsounds-5.7.1/keyboardsounds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.0/pyproject.toml` & `keyboardsounds-5.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyboardsounds"
-version = "5.7.0"
+version = "5.7.1"
 authors = [
   { name="Nathan Fiscaletti", email="nate.fiscaletti@gmail.com" },
 ]
 description = "Adds the ability to play sounds while typing on any system."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `keyboardsounds-5.7.0/setup.py` & `keyboardsounds-5.7.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from setuptools import setup
 
 setup(
-   name='keyboardsounds',
-   version='5.7.0',
-   description='Adds the ability to play sounds while typing on any system.',
-   author='Nathan Fiscaletti',
-   author_email='nate.fiscaletti@gmail.com',
-   packages=['keyboardsounds'],
-   install_requires=['pygame', 'pynput', 'psutil', 'imageio-ffmpeg', 'pyyaml'],
-   package_data={
-    'keyboardsounds': [
-      'profiles/alpaca/*',
-      'profiles/gateron-black-ink/*',
-      'profiles/gateron-red-ink/*',
-      'profiles/holy-panda/*',
-      'profiles/ios/*',
-      'profiles/mx-black/*',
-      'profiles/mx-blue/*',
-      'profiles/mx-brown/*',
-      'profiles/mx-speed-silver/*',
-      'profiles/telios-v2/*',
-      'profiles/typewriter/*',
-    ],
-   },
-   entry_points={
-         'console_scripts': [
-              'keyboardsounds = keyboardsounds.main:main',
-              'kbs = keyboardsounds.main:main',
-         ],
-   },
+    name="keyboardsounds",
+    version="5.7.1",
+    description="Adds the ability to play sounds while typing on any system.",
+    author="Nathan Fiscaletti",
+    author_email="nate.fiscaletti@gmail.com",
+    packages=["keyboardsounds"],
+    install_requires=["pygame", "pynput", "psutil", "imageio-ffmpeg", "pyyaml"],
+    package_data={
+        "keyboardsounds": [
+            "profiles/alpaca/*",
+            "profiles/gateron-black-ink/*",
+            "profiles/gateron-red-ink/*",
+            "profiles/holy-panda/*",
+            "profiles/ios/*",
+            "profiles/mx-black/*",
+            "profiles/mx-blue/*",
+            "profiles/mx-brown/*",
+            "profiles/mx-speed-silver/*",
+            "profiles/telios-v2/*",
+            "profiles/typewriter/*",
+        ],
+    },
+    entry_points={
+        "console_scripts": [
+            "keyboardsounds = keyboardsounds.main:main",
+            "kbs = keyboardsounds.main:main",
+        ],
+    },
 )
```

