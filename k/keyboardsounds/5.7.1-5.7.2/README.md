# Comparing `tmp/keyboardsounds-5.7.1.tar.gz` & `tmp/keyboardsounds-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyboardsounds-5.7.1.tar", last modified: Mon Apr 15 16:44:11 2024, max compression
+gzip compressed data, was "keyboardsounds-5.7.2.tar", last modified: Mon Apr 15 17:03:24 2024, max compression
```

## Comparing `keyboardsounds-5.7.1.tar` & `keyboardsounds-5.7.2.tar`

### file list

```diff
@@ -1,158 +1,162 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.771730 keyboardsounds-5.7.1/
--rw-rw-rw-   0        0        0     1074 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/LICENSE
--rw-rw-rw-   0        0        0    12639 2024-04-15 16:44:11.770730 keyboardsounds-5.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    11738 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.630010 keyboardsounds-5.7.1/keyboardsounds/
--rw-rw-rw-   0        0        0     5020 2024-02-27 16:21:44.000000 keyboardsounds-5.7.1/keyboardsounds/app_detector.py
--rw-rw-rw-   0        0        0     6278 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/app_rules.py
--rw-rw-rw-   0        0        0     9942 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/audio_manager.py
--rw-rw-rw-   0        0        0     4435 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/daemon.py
--rw-rw-rw-   0        0        0     9894 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/daemon_manager.py
--rw-rw-rw-   0        0        0    11909 2024-04-15 16:43:19.000000 keyboardsounds-5.7.1/keyboardsounds/main.py
--rw-rw-rw-   0        0        0      178 2024-02-23 15:27:38.000000 keyboardsounds-5.7.1/keyboardsounds/path_resolver.py
--rw-rw-rw-   0        0        0     3234 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profile.py
--rw-rw-rw-   0        0        0    18167 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profile_builder.py
--rw-rw-rw-   0        0        0     8802 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profile_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.614786 keyboardsounds-5.7.1/keyboardsounds/profiles/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.660677 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_space.mp3
--rw-rw-rw-   0        0        0      980 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.674914 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
--rw-rw-rw-   0        0        0      992 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/profile.yaml
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.689052 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2924 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
--rw-rw-rw-   0        0        0      988 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.702628 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/
--rw-rw-rw-   0        0        0     1099 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key5.mp3
--rw-rw-rw-   0        0        0     5850 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_space.mp3
--rw-rw-rw-   0        0        0      978 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_back.mp3
--rw-rw-rw-   0        0        0     1252 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_key.mp3
--rw-rw-rw-   0        0        0     1252 2024-04-14 23:03:15.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.705867 keyboardsounds-5.7.1/keyboardsounds/profiles/ios/
--rw-rw-rw-   0        0        0   740450 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/ios/ios-video-recording.mp4
--rw-rw-rw-   0        0        0      638 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/ios/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.718926 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_space.mp3
--rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_enter.mp3
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_key.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.726538 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key5.mp3
--rw-rw-rw-   0        0        0      504 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/release.mp3
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.740800 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/
--rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key5.mp3
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_space.mp3
--rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_back.mp3
--rw-rw-rw-   0        0        0     4596 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_key.mp3
--rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.747615 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/
--rw-rw-rw-   0        0        0    28336 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
--rw-rw-rw-   0        0        0    34328 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
--rw-rw-rw-   0        0        0    31488 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
--rw-rw-rw-   0        0        0    31176 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
--rw-rw-rw-   0        0        0    32228 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
--rw-rw-rw-   0        0        0    32016 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
--rw-rw-rw-   0        0        0      491 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.762572 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/
--rw-rw-rw-   0        0        0    28076 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/back.wav
--rw-rw-rw-   0        0        0    31916 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/caps.wav
--rw-rw-rw-   0        0        0    32812 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ctrl.wav
--rw-rw-rw-   0        0        0    22316 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ent.wav
--rw-rw-rw-   0        0        0    42540 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key1.wav
--rw-rw-rw-   0        0        0    26316 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key2.wav
--rw-rw-rw-   0        0        0    25516 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key3.wav
--rw-rw-rw-   0        0        0    25612 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key4.wav
--rw-rw-rw-   0        0        0    28300 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key5.wav
--rw-rw-rw-   0        0        0    26860 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key6.wav
--rw-rw-rw-   0        0        0      932 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/profile.yaml
--rw-rw-rw-   0        0        0    23596 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/shift.wav
--rw-rw-rw-   0        0        0    23212 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/space.wav
--rw-rw-rw-   0        0        0    38060 2024-04-14 23:03:27.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/tab.wav
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.768724 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/
--rw-rw-rw-   0        0        0    60204 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/delete.wav
--rw-rw-rw-   0        0        0   146204 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/enter.wav
--rw-rw-rw-   0        0        0    32664 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key.wav
--rw-rw-rw-   0        0        0    31588 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key2.wav
--rw-rw-rw-   0        0        0      579 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/profile.yaml
--rw-rw-rw-   0        0        0    35788 2024-04-14 23:03:42.000000 keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/space.wav
--rw-rw-rw-   0        0        0       60 2024-02-23 06:53:09.000000 keyboardsounds-5.7.1/keyboardsounds/root.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:44:11.770730 keyboardsounds-5.7.1/keyboardsounds.egg-info/
--rw-rw-rw-   0        0        0    12639 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6585 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 16:44:11.000000 keyboardsounds-5.7.1/keyboardsounds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      583 2024-04-15 16:43:29.000000 keyboardsounds-5.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 16:44:11.772729 keyboardsounds-5.7.1/setup.cfg
--rw-rw-rw-   0        0        0      997 2024-04-15 16:43:24.000000 keyboardsounds-5.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.584012 keyboardsounds-5.7.2/
+-rw-rw-rw-   0        0        0     1074 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/LICENSE
+-rw-rw-rw-   0        0        0    12639 2024-04-15 17:03:24.583376 keyboardsounds-5.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11738 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.412608 keyboardsounds-5.7.2/keyboardsounds/
+-rw-rw-rw-   0        0        0     5020 2024-02-27 16:21:44.000000 keyboardsounds-5.7.2/keyboardsounds/app_detector.py
+-rw-rw-rw-   0        0        0     6278 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/app_rules.py
+-rw-rw-rw-   0        0        0     9942 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/audio_manager.py
+-rw-rw-rw-   0        0        0     4435 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/daemon.py
+-rw-rw-rw-   0        0        0     9894 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/daemon_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.430087 keyboardsounds-5.7.2/keyboardsounds/external_api/
+-rw-rw-rw-   0        0        0     1987 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/external_api/__connection_handler.py
+-rw-rw-rw-   0        0        0     1826 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/external_api/__external_api.py
+-rw-rw-rw-   0        0        0       68 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/external_api/__init__.py
+-rw-rw-rw-   0        0        0    11909 2024-04-15 16:43:19.000000 keyboardsounds-5.7.2/keyboardsounds/main.py
+-rw-rw-rw-   0        0        0      178 2024-02-23 15:27:38.000000 keyboardsounds-5.7.2/keyboardsounds/path_resolver.py
+-rw-rw-rw-   0        0        0     3234 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profile.py
+-rw-rw-rw-   0        0        0    18167 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profile_builder.py
+-rw-rw-rw-   0        0        0     8802 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profile_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.395305 keyboardsounds-5.7.2/keyboardsounds/profiles/
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.446989 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_space.mp3
+-rw-rw-rw-   0        0        0      980 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.463568 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
+-rw-rw-rw-   0        0        0      992 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.480725 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2924 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
+-rw-rw-rw-   0        0        0      988 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.498815 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/
+-rw-rw-rw-   0        0        0     1099 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key5.mp3
+-rw-rw-rw-   0        0        0     5850 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_space.mp3
+-rw-rw-rw-   0        0        0      978 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_back.mp3
+-rw-rw-rw-   0        0        0     1252 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_key.mp3
+-rw-rw-rw-   0        0        0     1252 2024-04-14 23:03:15.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.503318 keyboardsounds-5.7.2/keyboardsounds/profiles/ios/
+-rw-rw-rw-   0        0        0   740450 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/ios/ios-video-recording.mp4
+-rw-rw-rw-   0        0        0      638 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/ios/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.522015 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_space.mp3
+-rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_enter.mp3
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_key.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.532526 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key5.mp3
+-rw-rw-rw-   0        0        0      504 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/release.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.548738 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/
+-rw-rw-rw-   0        0        0     1099 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key5.mp3
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_space.mp3
+-rw-rw-rw-   0        0        0      981 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_back.mp3
+-rw-rw-rw-   0        0        0     4596 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_key.mp3
+-rw-rw-rw-   0        0        0     1670 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.556140 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/
+-rw-rw-rw-   0        0        0    28336 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
+-rw-rw-rw-   0        0        0    34328 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
+-rw-rw-rw-   0        0        0    31488 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
+-rw-rw-rw-   0        0        0    31176 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
+-rw-rw-rw-   0        0        0    32228 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
+-rw-rw-rw-   0        0        0    32016 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
+-rw-rw-rw-   0        0        0      491 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.572040 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/
+-rw-rw-rw-   0        0        0    28076 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/back.wav
+-rw-rw-rw-   0        0        0    31916 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/caps.wav
+-rw-rw-rw-   0        0        0    32812 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/ctrl.wav
+-rw-rw-rw-   0        0        0    22316 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/ent.wav
+-rw-rw-rw-   0        0        0    42540 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key1.wav
+-rw-rw-rw-   0        0        0    26316 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key2.wav
+-rw-rw-rw-   0        0        0    25516 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key3.wav
+-rw-rw-rw-   0        0        0    25612 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key4.wav
+-rw-rw-rw-   0        0        0    28300 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key5.wav
+-rw-rw-rw-   0        0        0    26860 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key6.wav
+-rw-rw-rw-   0        0        0      932 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/profile.yaml
+-rw-rw-rw-   0        0        0    23596 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/shift.wav
+-rw-rw-rw-   0        0        0    23212 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/space.wav
+-rw-rw-rw-   0        0        0    38060 2024-04-14 23:03:27.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/tab.wav
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.580848 keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/
+-rw-rw-rw-   0        0        0    60204 2024-04-14 23:03:42.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/delete.wav
+-rw-rw-rw-   0        0        0   146204 2024-04-14 23:03:42.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/enter.wav
+-rw-rw-rw-   0        0        0    32664 2024-04-14 23:03:42.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/key.wav
+-rw-rw-rw-   0        0        0    31588 2024-04-14 23:03:42.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/key2.wav
+-rw-rw-rw-   0        0        0      579 2024-04-14 23:03:42.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/profile.yaml
+-rw-rw-rw-   0        0        0    35788 2024-04-14 23:03:42.000000 keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/space.wav
+-rw-rw-rw-   0        0        0       60 2024-02-23 06:53:09.000000 keyboardsounds-5.7.2/keyboardsounds/root.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:03:24.581852 keyboardsounds-5.7.2/keyboardsounds.egg-info/
+-rw-rw-rw-   0        0        0    12639 2024-04-15 17:03:24.000000 keyboardsounds-5.7.2/keyboardsounds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6723 2024-04-15 17:03:24.000000 keyboardsounds-5.7.2/keyboardsounds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:03:24.000000 keyboardsounds-5.7.2/keyboardsounds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-04-15 17:03:24.000000 keyboardsounds-5.7.2/keyboardsounds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 17:03:24.000000 keyboardsounds-5.7.2/keyboardsounds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      583 2024-04-15 17:02:32.000000 keyboardsounds-5.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:03:24.584012 keyboardsounds-5.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2024-04-15 17:02:29.000000 keyboardsounds-5.7.2/setup.py
```

### Comparing `keyboardsounds-5.7.1/LICENSE` & `keyboardsounds-5.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/PKG-INFO` & `keyboardsounds-5.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyboardsounds
-Version: 5.7.1
+Version: 5.7.2
 Summary: Adds the ability to play sounds while typing on any system.
 Author: Nathan Fiscaletti
 Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
 Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `keyboardsounds-5.7.1/README.md` & `keyboardsounds-5.7.2/README.md`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/app_detector.py` & `keyboardsounds-5.7.2/keyboardsounds/app_detector.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/app_rules.py` & `keyboardsounds-5.7.2/keyboardsounds/app_rules.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/audio_manager.py` & `keyboardsounds-5.7.2/keyboardsounds/audio_manager.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/daemon.py` & `keyboardsounds-5.7.2/keyboardsounds/daemon.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/daemon_manager.py` & `keyboardsounds-5.7.2/keyboardsounds/daemon_manager.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/main.py` & `keyboardsounds-5.7.2/keyboardsounds/main.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profile.py` & `keyboardsounds-5.7.2/keyboardsounds/profile.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profile_builder.py` & `keyboardsounds-5.7.2/keyboardsounds/profile_builder.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profile_validation.py` & `keyboardsounds-5.7.2/keyboardsounds/profile_validation.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/LICENSE` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key1.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key2.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key3.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key4.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_key5.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/press_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_key.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/alpaca/release_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/alpaca/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/LICENSE` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/press_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_key.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-black-ink/release_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-black-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/LICENSE` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/press_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_key.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/gateron-red-ink/release_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/gateron-red-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/LICENSE` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key1.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key2.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key3.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key4.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_key5.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/press_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_key.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/holy-panda/release_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/holy-panda/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/ios/ios-video-recording.mp4` & `keyboardsounds-5.7.2/keyboardsounds/profiles/ios/ios-video-recording.mp4`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/ios/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/ios/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/LICENSE` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key1.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key2.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key3.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key4.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_key5.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/press_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_key.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-black/release_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-black/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/LICENSE` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key1.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key2.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key3.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key4.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/press_key5.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-blue/release.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-blue/release.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/LICENSE` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key1.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key2.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key3.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key4.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_key5.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/press_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_back.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_enter.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_key.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-brown/release_space.mp3` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-brown/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/back.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/back.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/caps.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/caps.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ctrl.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/ctrl.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/ent.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/ent.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key1.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key2.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key3.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key4.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key5.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/key6.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/key6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/shift.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/shift.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/space.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/telios-v2/tab.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/telios-v2/tab.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/delete.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/delete.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/enter.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/enter.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/key.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/key2.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/profile.yaml` & `keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds/profiles/typewriter/space.wav` & `keyboardsounds-5.7.2/keyboardsounds/profiles/typewriter/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.1/keyboardsounds.egg-info/PKG-INFO` & `keyboardsounds-5.7.2/keyboardsounds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyboardsounds
-Version: 5.7.1
+Version: 5.7.2
 Summary: Adds the ability to play sounds while typing on any system.
 Author: Nathan Fiscaletti
 Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
 Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `keyboardsounds-5.7.1/keyboardsounds.egg-info/SOURCES.txt` & `keyboardsounds-5.7.2/keyboardsounds.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 keyboardsounds/profile_validation.py
 keyboardsounds/root.py
 keyboardsounds.egg-info/PKG-INFO
 keyboardsounds.egg-info/SOURCES.txt
 keyboardsounds.egg-info/dependency_links.txt
 keyboardsounds.egg-info/entry_points.txt
 keyboardsounds.egg-info/top_level.txt
+keyboardsounds/external_api/__connection_handler.py
+keyboardsounds/external_api/__external_api.py
+keyboardsounds/external_api/__init__.py
 keyboardsounds/profiles/alpaca/LICENSE
 keyboardsounds/profiles/alpaca/press_back.mp3
 keyboardsounds/profiles/alpaca/press_enter.mp3
 keyboardsounds/profiles/alpaca/press_key1.mp3
 keyboardsounds/profiles/alpaca/press_key2.mp3
 keyboardsounds/profiles/alpaca/press_key3.mp3
 keyboardsounds/profiles/alpaca/press_key4.mp3
```

### Comparing `keyboardsounds-5.7.1/pyproject.toml` & `keyboardsounds-5.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyboardsounds"
-version = "5.7.1"
+version = "5.7.2"
 authors = [
   { name="Nathan Fiscaletti", email="nate.fiscaletti@gmail.com" },
 ]
 description = "Adds the ability to play sounds while typing on any system."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `keyboardsounds-5.7.1/setup.py` & `keyboardsounds-5.7.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="keyboardsounds",
-    version="5.7.1",
+    version="5.7.2",
     description="Adds the ability to play sounds while typing on any system.",
     author="Nathan Fiscaletti",
     author_email="nate.fiscaletti@gmail.com",
     packages=["keyboardsounds"],
     install_requires=["pygame", "pynput", "psutil", "imageio-ffmpeg", "pyyaml"],
     package_data={
         "keyboardsounds": [
@@ -17,14 +17,15 @@
             "profiles/ios/*",
             "profiles/mx-black/*",
             "profiles/mx-blue/*",
             "profiles/mx-brown/*",
             "profiles/mx-speed-silver/*",
             "profiles/telios-v2/*",
             "profiles/typewriter/*",
+            "external_api/*",
         ],
     },
     entry_points={
         "console_scripts": [
             "keyboardsounds = keyboardsounds.main:main",
             "kbs = keyboardsounds.main:main",
         ],
```

