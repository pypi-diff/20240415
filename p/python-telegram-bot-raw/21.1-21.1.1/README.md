# Comparing `tmp/python-telegram-bot-raw-21.1.tar.gz` & `tmp/python-telegram-bot-raw-21.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-bot-raw-21.1.tar", last modified: Fri Apr 12 10:41:16 2024, max compression
+gzip compressed data, was "python-telegram-bot-raw-21.1.1.tar", last modified: Mon Apr 15 15:01:10 2024, max compression
```

## Comparing `python-telegram-bot-raw-21.1.tar` & `python-telegram-bot-raw-21.1.1.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/LICENSE
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/LICENSE.dual
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/LICENSE.lesser
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/MANIFEST.in
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12539 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12714 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/README.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10852 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/README_RAW.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3686 2024-04-12 10:02:06.000000 python-telegram-bot-raw-21.1/pyproject.toml
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.346938 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12539 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5123 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/SOURCES.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/dependency_links.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      203 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/requires.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2024-04-12 10:41:16.000000 python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/top_level.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1/requirements-opts.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      484 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1/requirements.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      235 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/setup.cfg
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5073 2024-04-12 10:34:12.000000 python-telegram-bot-raw-21.1/setup.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.354938 python-telegram-bot-raw-21.1/telegram/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15285 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1820 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/__main__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2861 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_birthdate.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   379065 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_bot.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3273 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botcommand.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10380 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botcommandscope.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2511 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botdescription.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1805 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_botname.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15745 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_business.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    33026 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_callbackquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   147253 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11366 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatadministratorrights.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15478 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatboost.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6764 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatinvitelink.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8746 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatjoinrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3296 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26788 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatmember.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7991 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatmemberupdated.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10917 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_chatpermissions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4274 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_choseninlineresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6956 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_dice.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.358938 python-telegram-bot-raw-21.1/telegram/_files/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3536 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/_basemedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3836 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/_basethumbedmedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4272 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/animation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4497 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/audio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7096 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/chatphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2720 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/contact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3552 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/document.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14644 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/file.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4191 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/inputfile.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26864 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/inputmedia.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5621 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/inputsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4762 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/location.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2826 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/photosize.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17443 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/sticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4466 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/venue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4114 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/video.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3516 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/videonote.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3031 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_files/voice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4383 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_forcereply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6965 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_forumtopic.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.358938 python-telegram-bot-raw-21.1/telegram/_games/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1309 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/callbackgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8114 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/game.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2518 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_games/gamehighscore.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14854 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_giveaway.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.362939 python-telegram-bot-raw-21.1/telegram/_inline/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15174 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5601 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9211 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2838 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5274 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultarticle.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5695 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5138 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5666 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcacheddocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5423 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5514 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5679 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3659 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5586 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5351 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5530 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcontact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7143 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultdocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2735 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7814 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9328 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7919 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7128 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5353 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultsbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7172 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvenue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8610 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5587 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2746 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputcontactmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12830 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputinvoicemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6586 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputlocationmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1567 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4804 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputtextmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4561 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_inline/inputvenuemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9168 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_keyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2547 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_keyboardbuttonpolltype.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12851 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_keyboardbuttonrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4498 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_linkpreviewoptions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5134 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_loginurl.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6856 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_menubutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   202095 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_message.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2015 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageautodeletetimerchanged.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8934 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageentity.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1704 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageid.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10097 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messageorigin.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7958 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_messagereactionupdated.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.362939 python-telegram-bot-raw-21.1/telegram/_passport/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22748 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/credentials.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6373 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/data.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12726 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/encryptedpassportelement.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5171 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/passportdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18799 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/passportelementerrors.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7157 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_passport/passportfile.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.362939 python-telegram-bot-raw-21.1/telegram/_payment/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5012 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/invoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2703 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/labeledprice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3118 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/orderinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5904 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/precheckoutquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2977 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/shippingaddress.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2502 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/shippingoption.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/shippingquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4939 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_payment/successfulpayment.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17858 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_poll.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2864 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_proximityalerttriggered.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6543 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_reaction.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20722 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_reply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16464 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_replykeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3251 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_replykeyboardremove.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2199 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_sentwebappmessage.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13120 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_shared.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2551 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_story.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4136 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_switchinlinequerychosenchat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27782 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_telegramobject.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    34486 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_update.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    80314 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_user.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2907 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_userprofilephotos.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/telegram/_utils/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2310 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/argumentparsing.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8924 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/datetime.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4305 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/defaultvalue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2641 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/enum.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5747 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/files.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1970 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/logging.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/markup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1833 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/repr.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1441 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/strings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3641 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/types.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1989 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/warnings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3863 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_utils/warnings_transition.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2234 2024-04-12 10:35:28.000000 python-telegram-bot-raw-21.1/telegram/_version.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6022 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_videochat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2444 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_webappdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2124 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_webappinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7720 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_webhookinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3585 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/_writeaccessallowed.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   106661 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/constants.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7574 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/error.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7252 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/helpers.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1/telegram/py.typed
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-12 10:41:16.366938 python-telegram-bot-raw-21.1/telegram/request/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20478 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_baserequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12968 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_httpxrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5204 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_requestdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7408 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/request/_requestparameter.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1899 2024-04-12 10:34:13.000000 python-telegram-bot-raw-21.1/telegram/warnings.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/LICENSE
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/LICENSE.dual
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/LICENSE.lesser
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/MANIFEST.in
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12541 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12714 2024-04-15 14:54:41.000000 python-telegram-bot-raw-21.1.1/README.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10852 2024-04-15 14:54:41.000000 python-telegram-bot-raw-21.1.1/README_RAW.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3686 2024-04-15 14:50:11.000000 python-telegram-bot-raw-21.1.1/pyproject.toml
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.058611 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12541 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5123 2024-04-15 15:01:10.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/SOURCES.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/dependency_links.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      203 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/requires.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2024-04-15 15:01:09.000000 python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/top_level.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1.1/requirements-opts.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      484 2024-03-06 19:36:26.000000 python-telegram-bot-raw-21.1.1/requirements.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      235 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/setup.cfg
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5073 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/setup.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.066611 python-telegram-bot-raw-21.1.1/telegram/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15285 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1820 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/__main__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2861 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_birthdate.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   379065 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_bot.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3273 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botcommand.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10380 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botcommandscope.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2511 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botdescription.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1805 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_botname.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15745 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_business.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    33026 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_callbackquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   147253 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11366 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatadministratorrights.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15478 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatboost.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6764 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatinvitelink.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8746 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatjoinrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3296 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26788 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatmember.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7991 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatmemberupdated.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10917 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_chatpermissions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4274 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_choseninlineresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6956 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_dice.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.070611 python-telegram-bot-raw-21.1.1/telegram/_files/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3536 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/_basemedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3836 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/_basethumbedmedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4272 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/animation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4497 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/audio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7096 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/chatphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2720 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/contact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3552 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/document.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14644 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/file.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4191 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/inputfile.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26864 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/inputmedia.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5621 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/inputsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4762 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/location.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2826 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/photosize.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17443 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/sticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4466 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/venue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4114 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/video.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3516 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/videonote.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3031 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_files/voice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4383 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_forcereply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6965 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_forumtopic.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.070611 python-telegram-bot-raw-21.1.1/telegram/_games/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1309 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/callbackgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8114 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/game.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2518 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_games/gamehighscore.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14854 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_giveaway.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.074610 python-telegram-bot-raw-21.1.1/telegram/_inline/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15174 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5601 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9211 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2838 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5274 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultarticle.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5695 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5138 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5666 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcacheddocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5423 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5514 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5679 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3659 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5586 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5351 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5530 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcontact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7143 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultdocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2735 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7814 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9328 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7919 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7128 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5353 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultsbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7172 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvenue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8610 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5587 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2746 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputcontactmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12830 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputinvoicemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6586 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputlocationmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1567 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4804 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputtextmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4561 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_inline/inputvenuemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9168 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_keyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2547 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonpolltype.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12851 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4498 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_linkpreviewoptions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5134 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_loginurl.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6856 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_menubutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   202907 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_message.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2015 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageautodeletetimerchanged.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8934 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageentity.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1704 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageid.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10097 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messageorigin.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7958 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_messagereactionupdated.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.074610 python-telegram-bot-raw-21.1.1/telegram/_passport/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22754 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/credentials.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6373 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/data.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12726 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/encryptedpassportelement.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5171 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/passportdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18799 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/passportelementerrors.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7157 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_passport/passportfile.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.074610 python-telegram-bot-raw-21.1.1/telegram/_payment/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5012 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/invoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2703 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/labeledprice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3118 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/orderinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5904 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/precheckoutquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2977 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/shippingaddress.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2502 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/shippingoption.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/shippingquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4939 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_payment/successfulpayment.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17858 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_poll.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2864 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_proximityalerttriggered.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6543 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_reaction.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20722 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_reply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16464 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_replykeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3251 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_replykeyboardremove.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2199 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_sentwebappmessage.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13120 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_shared.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2551 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_story.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4136 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_switchinlinequerychosenchat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    27782 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_telegramobject.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    34486 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_update.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    80314 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_user.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2907 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_userprofilephotos.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/telegram/_utils/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2310 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/argumentparsing.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8924 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/datetime.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4305 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/defaultvalue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2641 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/enum.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5747 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/files.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1970 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/logging.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/markup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1833 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/repr.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1441 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/strings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3641 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/types.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1989 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/warnings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3863 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_utils/warnings_transition.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2234 2024-04-15 14:56:01.000000 python-telegram-bot-raw-21.1.1/telegram/_version.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6022 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_videochat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2444 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_webappdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2124 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_webappinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7720 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_webhookinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3585 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/_writeaccessallowed.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   106661 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/constants.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7574 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/error.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7252 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/helpers.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-21.1.1/telegram/py.typed
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2024-04-15 15:01:10.078610 python-telegram-bot-raw-21.1.1/telegram/request/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    20478 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_baserequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12968 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_httpxrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5204 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_requestdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7408 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/request/_requestparameter.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1899 2024-04-15 14:54:39.000000 python-telegram-bot-raw-21.1.1/telegram/warnings.py
```

### Comparing `python-telegram-bot-raw-21.1/LICENSE` & `python-telegram-bot-raw-21.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/LICENSE.dual` & `python-telegram-bot-raw-21.1.1/LICENSE.dual`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/LICENSE.lesser` & `python-telegram-bot-raw-21.1.1/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/PKG-INFO` & `python-telegram-bot-raw-21.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 21.1
+Version: 21.1.1
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
```

### Comparing `python-telegram-bot-raw-21.1/README.rst` & `python-telegram-bot-raw-21.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/README_RAW.rst` & `python-telegram-bot-raw-21.1.1/README_RAW.rst`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/pyproject.toml` & `python-telegram-bot-raw-21.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/PKG-INFO` & `python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 21.1
+Version: 21.1.1
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
```

### Comparing `python-telegram-bot-raw-21.1/python_telegram_bot_raw.egg-info/SOURCES.txt` & `python-telegram-bot-raw-21.1.1/python_telegram_bot_raw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/requirements-opts.txt` & `python-telegram-bot-raw-21.1.1/requirements-opts.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/setup.py` & `python-telegram-bot-raw-21.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/__init__.py` & `python-telegram-bot-raw-21.1.1/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/__main__.py` & `python-telegram-bot-raw-21.1.1/telegram/__main__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_birthdate.py` & `python-telegram-bot-raw-21.1.1/telegram/_birthdate.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_bot.py` & `python-telegram-bot-raw-21.1.1/telegram/_bot.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_botcommand.py` & `python-telegram-bot-raw-21.1.1/telegram/_botcommand.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_botcommandscope.py` & `python-telegram-bot-raw-21.1.1/telegram/_botcommandscope.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_botdescription.py` & `python-telegram-bot-raw-21.1.1/telegram/_botdescription.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_botname.py` & `python-telegram-bot-raw-21.1.1/telegram/_botname.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_business.py` & `python-telegram-bot-raw-21.1.1/telegram/_business.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_callbackquery.py` & `python-telegram-bot-raw-21.1.1/telegram/_callbackquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chat.py` & `python-telegram-bot-raw-21.1.1/telegram/_chat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatadministratorrights.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatadministratorrights.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatboost.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatboost.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatinvitelink.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatinvitelink.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatjoinrequest.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatjoinrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatlocation.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatlocation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatmember.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatmember.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatmemberupdated.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatmemberupdated.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_chatpermissions.py` & `python-telegram-bot-raw-21.1.1/telegram/_chatpermissions.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_choseninlineresult.py` & `python-telegram-bot-raw-21.1.1/telegram/_choseninlineresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_dice.py` & `python-telegram-bot-raw-21.1.1/telegram/_dice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/_basemedium.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/_basemedium.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/_basethumbedmedium.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/_basethumbedmedium.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/animation.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/animation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/audio.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/audio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/chatphoto.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/chatphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/contact.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/contact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/document.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/document.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/file.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/file.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/inputfile.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/inputfile.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/inputmedia.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/inputmedia.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/inputsticker.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/inputsticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/location.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/location.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/photosize.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/photosize.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/sticker.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/sticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/venue.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/venue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/video.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/video.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/videonote.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/videonote.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_files/voice.py` & `python-telegram-bot-raw-21.1.1/telegram/_files/voice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_forcereply.py` & `python-telegram-bot-raw-21.1.1/telegram/_forcereply.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_forumtopic.py` & `python-telegram-bot-raw-21.1.1/telegram/_forumtopic.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_games/callbackgame.py` & `python-telegram-bot-raw-21.1.1/telegram/_games/callbackgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_games/game.py` & `python-telegram-bot-raw-21.1.1/telegram/_games/game.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_games/gamehighscore.py` & `python-telegram-bot-raw-21.1.1/telegram/_games/gamehighscore.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_giveaway.py` & `python-telegram-bot-raw-21.1.1/telegram/_giveaway.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardbutton.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinekeyboardmarkup.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinekeyboardmarkup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequery.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresult.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultarticle.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultarticle.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultaudio.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedaudio.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcacheddocument.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcacheddocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedgif.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedphoto.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedsticker.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedsticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvideo.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcachedvoice.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcachedvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultcontact.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultcontact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultdocument.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultdocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgame.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultgif.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultlocation.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultlocation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultmpeg4gif.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultphoto.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultsbutton.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultsbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvenue.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvenue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvideo.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inlinequeryresultvoice.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inlinequeryresultvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inputcontactmessagecontent.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inputcontactmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inputinvoicemessagecontent.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inputinvoicemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inputlocationmessagecontent.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inputlocationmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inputmessagecontent.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inputmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inputtextmessagecontent.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inputtextmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_inline/inputvenuemessagecontent.py` & `python-telegram-bot-raw-21.1.1/telegram/_inline/inputvenuemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_keyboardbutton.py` & `python-telegram-bot-raw-21.1.1/telegram/_keyboardbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_keyboardbuttonpolltype.py` & `python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonpolltype.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_keyboardbuttonrequest.py` & `python-telegram-bot-raw-21.1.1/telegram/_keyboardbuttonrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_linkpreviewoptions.py` & `python-telegram-bot-raw-21.1.1/telegram/_linkpreviewoptions.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_loginurl.py` & `python-telegram-bot-raw-21.1.1/telegram/_loginurl.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_menubutton.py` & `python-telegram-bot-raw-21.1.1/telegram/_menubutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_message.py` & `python-telegram-bot-raw-21.1.1/telegram/_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1458,15 +1458,15 @@
 
     def build_reply_arguments(
         self,
         quote: Optional[str] = None,
         quote_index: Optional[int] = None,
         target_chat_id: Optional[Union[int, str]] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
     ) -> _ReplyKwargs:
         """
         Builds a dictionary with the keys ``chat_id`` and ``reply_parameters``. This dictionary can
         be used to reply to a message with the given quote and target chat.
 
         Examples:
 
@@ -1583,29 +1583,40 @@
             effective_reply_parameters = self._quote(effective_do_quote)
 
         return chat_id, effective_reply_parameters
 
     def _parse_message_thread_id(
         self,
         chat_id: Union[str, int],
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
     ) -> Optional[int]:
-        return message_thread_id or (
-            self.message_thread_id if chat_id in {self.chat_id, self.chat.username} else None
-        )
+        # values set by user have the highest priority
+        if not isinstance(message_thread_id, DefaultValue):
+            return message_thread_id
+
+        # self.message_thread_id can be used for send_*.param.message_thread_id only if the
+        # thread is a forum topic. It does not work if the thread is a chain of replies to a
+        # message in a normal group. In that case, self.message_thread_id is just the message_id
+        # of the first message in the chain.
+        if not self.is_topic_message:
+            return None
+
+        # Setting message_thread_id=self.message_thread_id only makes sense if we're replying in
+        # the same chat.
+        return self.message_thread_id if chat_id in {self.chat_id, self.chat.username} else None
 
     async def reply_text(
         self,
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         link_preview_options: ODVInput["LinkPreviewOptions"] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         disable_web_page_preview: Optional[bool] = None,
         quote: Optional[bool] = None,
@@ -1673,15 +1684,15 @@
     async def reply_markdown(
         self,
         text: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         link_preview_options: ODVInput["LinkPreviewOptions"] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         disable_web_page_preview: Optional[bool] = None,
         quote: Optional[bool] = None,
@@ -1755,15 +1766,15 @@
     async def reply_markdown_v2(
         self,
         text: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         link_preview_options: ODVInput["LinkPreviewOptions"] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         disable_web_page_preview: Optional[bool] = None,
         quote: Optional[bool] = None,
@@ -1833,15 +1844,15 @@
     async def reply_html(
         self,
         text: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         link_preview_options: ODVInput["LinkPreviewOptions"] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         disable_web_page_preview: Optional[bool] = None,
         quote: Optional[bool] = None,
@@ -1911,15 +1922,15 @@
     async def reply_media_group(
         self,
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -1990,15 +2001,15 @@
         photo: Union[FileInput, "PhotoSize"],
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         has_spoiler: Optional[bool] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         quote: Optional[bool] = None,
@@ -2072,15 +2083,15 @@
         title: Optional[str] = None,
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         quote: Optional[bool] = None,
@@ -2155,15 +2166,15 @@
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_content_type_detection: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         quote: Optional[bool] = None,
@@ -2238,15 +2249,15 @@
         height: Optional[int] = None,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
@@ -2319,15 +2330,15 @@
 
     async def reply_sticker(
         self,
         sticker: Union[FileInput, "Sticker"],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         emoji: Optional[str] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
@@ -2397,15 +2408,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         supports_streaming: Optional[bool] = None,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         has_spoiler: Optional[bool] = None,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
@@ -2481,15 +2492,15 @@
         self,
         video_note: Union[FileInput, "VideoNote"],
         duration: Optional[int] = None,
         length: Optional[int] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         thumbnail: Optional[FileInput] = None,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         quote: Optional[bool] = None,
@@ -2560,15 +2571,15 @@
         duration: Optional[int] = None,
         caption: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         filename: Optional[str] = None,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
@@ -2640,15 +2651,15 @@
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         live_period: Optional[int] = None,
         horizontal_accuracy: Optional[float] = None,
         heading: Optional[int] = None,
         proximity_alert_radius: Optional[int] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         location: Optional[Location] = None,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
@@ -2723,15 +2734,15 @@
         foursquare_id: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         foursquare_type: Optional[str] = None,
         google_place_id: Optional[str] = None,
         google_place_type: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         venue: Optional[Venue] = None,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
@@ -2804,15 +2815,15 @@
         phone_number: Optional[str] = None,
         first_name: Optional[str] = None,
         last_name: Optional[str] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         vcard: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         contact: Optional[Contact] = None,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
@@ -2889,15 +2900,15 @@
         reply_markup: Optional[ReplyMarkup] = None,
         explanation: Optional[str] = None,
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
         open_period: Optional[int] = None,
         close_date: Optional[Union[int, datetime.datetime]] = None,
         explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -2969,15 +2980,15 @@
 
     async def reply_dice(
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         emoji: Optional[str] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3035,15 +3046,15 @@
             message_thread_id=message_thread_id,
             business_connection_id=self.business_connection_id,
         )
 
     async def reply_chat_action(
         self,
         action: str,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
@@ -3082,15 +3093,15 @@
 
     async def reply_game(
         self,
         game_short_name: str,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3173,15 +3184,15 @@
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         provider_data: Optional[Union[str, object]] = None,
         send_phone_number_to_provider: Optional[bool] = None,
         send_email_to_provider: Optional[bool] = None,
         max_tip_amount: Optional[int] = None,
         suggested_tip_amounts: Optional[Sequence[int]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3383,15 +3394,15 @@
         message_id: int,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: Optional[int] = None,
+        message_thread_id: ODVInput[int] = DEFAULT_NONE,
         reply_parameters: Optional["ReplyParameters"] = None,
         *,
         reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         quote: Optional[bool] = None,
         do_quote: Optional[Union[bool, _ReplyKwargs]] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
```

### Comparing `python-telegram-bot-raw-21.1/telegram/_messageautodeletetimerchanged.py` & `python-telegram-bot-raw-21.1.1/telegram/_messageautodeletetimerchanged.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_messageentity.py` & `python-telegram-bot-raw-21.1.1/telegram/_messageentity.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_messageid.py` & `python-telegram-bot-raw-21.1.1/telegram/_messageid.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_messageorigin.py` & `python-telegram-bot-raw-21.1.1/telegram/_messageorigin.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_messagereactionupdated.py` & `python-telegram-bot-raw-21.1.1/telegram/_messagereactionupdated.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_passport/credentials.py` & `python-telegram-bot-raw-21.1.1/telegram/_passport/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,23 +149,23 @@
         # Required
         self.data: str = data
         self.hash: str = hash
         self.secret: str = secret
 
         self._id_attrs = (self.data, self.hash, self.secret)
 
-        self._decrypted_secret: Optional[str] = None
+        self._decrypted_secret: Optional[bytes] = None
         self._decrypted_data: Optional[Credentials] = None
 
         self._freeze()
 
     @property
-    def decrypted_secret(self) -> str:
+    def decrypted_secret(self) -> bytes:
         """
-        :obj:`str`: Lazily decrypt and return secret.
+        :obj:`bytes`: Lazily decrypt and return secret.
 
         Raises:
             telegram.error.PassportDecryptionError: Decryption failed. Usually due to bad
                 private/public key but can also suggest malformed/tampered data.
         """
         if self._decrypted_secret is None:
             if not CRYPTO_INSTALLED:
```

### Comparing `python-telegram-bot-raw-21.1/telegram/_passport/data.py` & `python-telegram-bot-raw-21.1.1/telegram/_passport/data.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_passport/encryptedpassportelement.py` & `python-telegram-bot-raw-21.1.1/telegram/_passport/encryptedpassportelement.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_passport/passportdata.py` & `python-telegram-bot-raw-21.1.1/telegram/_passport/passportdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_passport/passportelementerrors.py` & `python-telegram-bot-raw-21.1.1/telegram/_passport/passportelementerrors.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_passport/passportfile.py` & `python-telegram-bot-raw-21.1.1/telegram/_passport/passportfile.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/invoice.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/invoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/labeledprice.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/labeledprice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/orderinfo.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/orderinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/precheckoutquery.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/precheckoutquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/shippingaddress.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/shippingaddress.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/shippingoption.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/shippingoption.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/shippingquery.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/shippingquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_payment/successfulpayment.py` & `python-telegram-bot-raw-21.1.1/telegram/_payment/successfulpayment.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_poll.py` & `python-telegram-bot-raw-21.1.1/telegram/_poll.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_proximityalerttriggered.py` & `python-telegram-bot-raw-21.1.1/telegram/_proximityalerttriggered.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_reaction.py` & `python-telegram-bot-raw-21.1.1/telegram/_reaction.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_reply.py` & `python-telegram-bot-raw-21.1.1/telegram/_reply.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_replykeyboardmarkup.py` & `python-telegram-bot-raw-21.1.1/telegram/_replykeyboardmarkup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_replykeyboardremove.py` & `python-telegram-bot-raw-21.1.1/telegram/_replykeyboardremove.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_sentwebappmessage.py` & `python-telegram-bot-raw-21.1.1/telegram/_sentwebappmessage.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_shared.py` & `python-telegram-bot-raw-21.1.1/telegram/_shared.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_story.py` & `python-telegram-bot-raw-21.1.1/telegram/_story.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_switchinlinequerychosenchat.py` & `python-telegram-bot-raw-21.1.1/telegram/_switchinlinequerychosenchat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_telegramobject.py` & `python-telegram-bot-raw-21.1.1/telegram/_telegramobject.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_update.py` & `python-telegram-bot-raw-21.1.1/telegram/_update.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_user.py` & `python-telegram-bot-raw-21.1.1/telegram/_user.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_userprofilephotos.py` & `python-telegram-bot-raw-21.1.1/telegram/_userprofilephotos.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/argumentparsing.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/argumentparsing.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/datetime.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/defaultvalue.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/defaultvalue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/enum.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/enum.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/files.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/files.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/logging.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/logging.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/markup.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/markup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/repr.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/repr.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/strings.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/strings.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/types.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/types.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/warnings.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_utils/warnings_transition.py` & `python-telegram-bot-raw-21.1.1/telegram/_utils/warnings_transition.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_version.py` & `python-telegram-bot-raw-21.1.1/telegram/_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         if self.releaselevel != "final":
             version = f"{version}{self._rl_shorthand()}{self.serial}"
 
         return version
 
 
 __version_info__: Final[Version] = Version(
-    major=21, minor=1, micro=0, releaselevel="final", serial=0
+    major=21, minor=1, micro=1, releaselevel="final", serial=0
 )
 __version__: Final[str] = str(__version_info__)
 
 # # SETUP.PY MARKER
 # Lines above this line will be `exec`-cuted in setup.py. Make sure that this only contains
 # std-lib imports!
```

### Comparing `python-telegram-bot-raw-21.1/telegram/_videochat.py` & `python-telegram-bot-raw-21.1.1/telegram/_videochat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_webappdata.py` & `python-telegram-bot-raw-21.1.1/telegram/_webappdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_webappinfo.py` & `python-telegram-bot-raw-21.1.1/telegram/_webappinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_webhookinfo.py` & `python-telegram-bot-raw-21.1.1/telegram/_webhookinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/_writeaccessallowed.py` & `python-telegram-bot-raw-21.1.1/telegram/_writeaccessallowed.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/constants.py` & `python-telegram-bot-raw-21.1.1/telegram/constants.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/error.py` & `python-telegram-bot-raw-21.1.1/telegram/error.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/helpers.py` & `python-telegram-bot-raw-21.1.1/telegram/helpers.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/request/__init__.py` & `python-telegram-bot-raw-21.1.1/telegram/request/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/request/_baserequest.py` & `python-telegram-bot-raw-21.1.1/telegram/request/_baserequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/request/_httpxrequest.py` & `python-telegram-bot-raw-21.1.1/telegram/request/_httpxrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/request/_requestdata.py` & `python-telegram-bot-raw-21.1.1/telegram/request/_requestdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/request/_requestparameter.py` & `python-telegram-bot-raw-21.1.1/telegram/request/_requestparameter.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-21.1/telegram/warnings.py` & `python-telegram-bot-raw-21.1.1/telegram/warnings.py`

 * *Files identical despite different names*

