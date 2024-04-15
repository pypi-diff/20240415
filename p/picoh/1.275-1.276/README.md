# Comparing `tmp/picoh-1.275.tar.gz` & `tmp/picoh-1.276.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/picoh-python/picoh-python/dist/tmpagpqzx11/picoh-1.275.tar", last modified: Wed Apr 14 13:13:04 2021, max compression
+gzip compressed data, was "picoh-1.276.tar", last modified: Mon Apr 15 18:40:56 2024, max compression
```

## Comparing `picoh-1.275.tar` & `picoh-1.276.tar`

### file list

```diff
@@ -1,14 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-14 13:13:04.000000 picoh-1.275/
--rw-r--r--   0 runner    (1001) docker     (116)      344 2021-04-14 13:13:04.000000 picoh-1.275/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    11480 2021-04-14 13:12:53.000000 picoh-1.275/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-14 13:13:04.000000 picoh-1.275/picoh/
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-04-14 13:12:53.000000 picoh-1.275/picoh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    43226 2021-04-14 13:12:53.000000 picoh-1.275/picoh/picoh.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-14 13:13:04.000000 picoh-1.275/picoh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      344 2021-04-14 13:13:04.000000 picoh-1.275/picoh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      205 2021-04-14 13:13:04.000000 picoh-1.275/picoh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-04-14 13:13:04.000000 picoh-1.275/picoh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       39 2021-04-14 13:13:04.000000 picoh-1.275/picoh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-04-14 13:13:04.000000 picoh-1.275/picoh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2021-04-14 13:13:04.000000 picoh-1.275/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1446 2021-04-14 13:12:53.000000 picoh-1.275/setup.py
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-04-15 18:40:56.052105 picoh-1.276/
+-rw-r--r--   0 georgewalker   (501) staff       (20)      426 2024-04-15 18:40:56.050080 picoh-1.276/PKG-INFO
+-rw-r--r--   0 georgewalker   (501) staff       (20)    11480 2024-04-15 18:36:49.000000 picoh-1.276/README.md
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-04-15 18:40:55.931746 picoh-1.276/picoh/
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-04-15 18:40:55.986086 picoh-1.276/picoh/Images/
+-rw-r--r--   0 georgewalker   (501) staff       (20)  1852007 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/calibrate2400.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)  1787784 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/calibrate400.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      856 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/logoPT.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)      874 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/movedown.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)      877 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/moveright.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)       90 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/off.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)       74 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/offsmaller.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)       90 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/on.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)       74 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/onsmaller.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)     2002 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/picohlogo.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)     2002 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/picohlogoOn.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)     1314 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/picohlogoSmall.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)      807 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/pixel.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)      875 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/plus.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)      633 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/resetIcon.gif
+-rwxr-xr-x   0 georgewalker   (501) staff       (20)     2486 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Images/savebutton.gif
+-rw-r--r--   0 georgewalker   (501) staff       (20)     1228 2024-04-15 18:36:49.000000 picoh-1.276/picoh/MotorDefinitionsPicoh.omd
+-rw-r--r--   0 georgewalker   (501) staff       (20)      459 2024-04-15 18:36:49.000000 picoh-1.276/picoh/PicohSettings.xml
+-rw-r--r--   0 georgewalker   (501) staff       (20)      221 2024-04-15 18:36:49.000000 picoh-1.276/picoh/PicohSpeech.csv
+-rw-r--r--   0 georgewalker   (501) staff       (20)    88134 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Silence1.wav
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-04-15 18:40:56.040917 picoh-1.276/picoh/Sounds/
+-rw-r--r--   0 georgewalker   (501) staff       (20)  1206224 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Sounds/fanfare.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)  1619014 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Sounds/loop.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)   234489 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Sounds/ohbot.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)   103760 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Sounds/smash.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)   287760 2024-04-15 18:36:49.000000 picoh-1.276/picoh/Sounds/spring.wav
+-rw-r--r--   0 georgewalker   (501) staff       (20)        6 2024-04-15 18:36:49.000000 picoh-1.276/picoh/__init__.py
+-rw-r--r--   0 georgewalker   (501) staff       (20)     4998 2024-04-15 18:36:49.000000 picoh-1.276/picoh/ohbot.obe
+-rw-r--r--   0 georgewalker   (501) staff       (20)    43540 2024-04-15 18:36:49.000000 picoh-1.276/picoh/picoh.py
+drwxr-xr-x   0 georgewalker   (501) staff       (20)        0 2024-04-15 18:40:56.049201 picoh-1.276/picoh.egg-info/
+-rw-r--r--   0 georgewalker   (501) staff       (20)      426 2024-04-15 18:40:55.000000 picoh-1.276/picoh.egg-info/PKG-INFO
+-rw-r--r--   0 georgewalker   (501) staff       (20)      857 2024-04-15 18:40:55.000000 picoh-1.276/picoh.egg-info/SOURCES.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)        1 2024-04-15 18:40:55.000000 picoh-1.276/picoh.egg-info/dependency_links.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)       48 2024-04-15 18:40:55.000000 picoh-1.276/picoh.egg-info/requires.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)        6 2024-04-15 18:40:55.000000 picoh-1.276/picoh.egg-info/top_level.txt
+-rw-r--r--   0 georgewalker   (501) staff       (20)       79 2024-04-15 18:40:56.052485 picoh-1.276/setup.cfg
+-rw-r--r--   0 georgewalker   (501) staff       (20)     1437 2024-04-15 18:40:19.000000 picoh-1.276/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `picoh-1.275/README.md` & `picoh-1.276/README.md`

 * *Files identical despite different names*

### Comparing `picoh-1.275/picoh/picoh.py` & `picoh-1.276/picoh/picoh.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,98 +5,108 @@
 import serial.tools.list_ports
 import time
 import threading
 import os
 import os.path
 from os import path
 import shutil
+import sys
 import wave
 import subprocess
 from lxml import etree
 import random
 import re
 import csv
 import requests
 
 AccessUri = "https://westeurope.api.cognitive.microsoft.com/sts/v1.0/issueToken"
 SynthesizeUri = "https://westeurope.tts.speech.microsoft.com/cognitiveservices/v1"
 
-sapivoice = ""
-sapistream = ""
+sapivoice = ''
+sapistream = ''
 
 # Import the correct sound library depending on platform.
 if platform.system() == "Windows":
     import winsound
     # For SAPI speech
     from comtypes.client import CreateObject
 
 if platform.system() == "Darwin":
     from playsound import playsound
 if platform.system() == "Linux":
     from playsound import playsound
     from gtts import gTTS
     from pydub import AudioSegment
-# Variables to hold name of settings
 
+# Variables to hold name of settings
 speechDatabaseFile = ''
 defaultEyeShape = ''
 eyeShapeLeft = ''
 eyeShapeRight = ''
 eyeShapeFile = ''
 speechAudioFile = 'picohData/picohspeech.wav'
 picohMotorDefFile = 'picohData/MotorDefinitonsPicoh.omd'
 soundFolder = 'picohData/Sounds'
 synthesizer = ''
 voice = ''
 language = 'en-GB' # Language/Accent for GTTS web text to speech.
 settingsFile = 'picohData/PicohSettings.xml' # String to hold location of settings file
 speechGender = "Female"
+# This is passed in to setsynthesizer
 cogServicesID = ''
 
 # Variable to hold the location of the picoh library folder.
 directory = os.path.dirname(os.path.abspath(__file__))
 
 # name of directory that holds eye shape, motor definition and speech db files.
 dirName = 'picohData'
 
 # Global variable to turn on and off printing debug info.
 debug = False
 
+# define constants for waits in seconds
+WAITSHORT = 0.01
+WAITMEDIUM = 0.05
+WAITLONG = 0.1
+
 # define constants for motors
 HEADNOD = 0
 HEADTURN = 1
 EYETURN = 2
 LIDBLINK = 3
 TOPLIP = 4
 BOTTOMLIP = 5
 EYETILT = 6
+HEADROLL = 7
 
 # array to hold sensor values.
 sensors = [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
 
 # Put motor ranges into lists
 motorPos = [11, 11, 11, 11, 11, 11, 11, 11]
 motorMins = [0, 0, 0, 0, 0, 0, 0, 0]
 motorMaxs = [0, 0, 0, 0, 0, 0, 0, 0]
 motorSpeeds = [0, 0, 0, 0, 0, 0, 0, 0]
 motorAccels = [0, 0, 0, 0, 0, 0, 0, 0]
 motorRev = [False, False, False, False, False, False, False, False]
 restPos = [0, 0, 0, 0, 0, 0, 0, 0]
 isAttached = [False, False, False, False, False, False, False, False]
 motorType = ["", "", "", "", "", "", "", ""]
+lipTopPos = 5
+lipBottomPos = 5
 
 # empty lists to hold eye shapes and phrases from speech databa se.
 shapeList = []
 phraseList = []
 
 # define a module level variable for the serial port
 port = ""
 
 # define library version
-version = "1.275"
+version = "1.276"
 
 # flag to stop writing when writing for threading
 writing = False
 
 # flag to allow the library to run when not connected
 connected = False
 
@@ -218,16 +228,14 @@
 lastfexr = 5
 lastfeyl = 5
 lastfeyr = 5
 
 blinkl = 10
 blinkr = 10
 
-bottomLipPos = 5
-
 baseR = 0
 baseG = 0
 baseB = 0
 
 ser = None
 
 # A class that defines eye shape objects.
@@ -363,15 +371,15 @@
         val = voice[pos + 2:]
         pos = val.find(" ")
         if ((pos != None) and (pos > 0)):
             val = val[:pos]
     return val
 
 
-# generate speech file depending on platform and sythensizer.
+# generate speech file depending on platform and synthesizer.
 def _generateSpeechFile(text):
     # Pick up the global variable that defines the language. This is only used in GTTS speech.
     global language
     file = speechAudioFile
 
     if synthesizer.lower() == 'azure':
 
@@ -743,25 +751,25 @@
 
     # Write message to serial port
     _serwrite(msg)
 
     # Update motor positions list
     motorPos[m] = pos
 
-  # Function to write to serial port
+# Function to write to serial port
 def _serwrite(s):
     global connected, writing
 
     if debug:
         print("Serial command sent to Picoh:")
         print(s)
     if platform.system() == "Windows" or platform.system() == "Linux":
-        # wait until previous write is finished
+        # wait until previous write is finished without blocking other threads
         while (writing):
-            pass
+            wait(WAITSHORT)
         # print ('waiting on write')
 
     if connected:
         writing = True
         ser.write(s.encode('latin-1'))
         writing = False
 
@@ -788,35 +796,42 @@
 
 # Function to find the scaled position of a given motor. Arguments | m (motor) → int (0-6) | pos (position) → int (0-10) | Returns a position
 def _getPos(m, pos):
     mRange = motorMaxs[m] - motorMins[m]
     scaledPos = (mRange / 10) * pos
     return scaledPos + motorMins[m]
 
+# Function to return the current lip position for speech
+def getTopLip ():
+    return lipTopPos
+
+# Function to return the bottom lip position for speech
+def getBottomLip ():
+    return lipBottomPos
 
 # Function to set the language used by gTTS web speech synthesizer
 # name - run 'say -v ?' in terminal to find available names.
 def setLanguage(params=language):
     global language
     language = params
 
 # Function to set the voice used by the synthesiser
 # name - run 'say -v ?' in terminal to find available names.
 # speed - speech rate in words per min.
 # This override will stay in use until it's next called
 def setVoice(params=voice,language = "en-GB", gender = 'Female'):
-    global voice, speech_config, audio_config,azureSynthesizer, speechGender
+    global voice, speechGender
     voice = params
     speechGender = gender
     setLanguage(language)
     
 
 # Function to set a different speech synthesizer - defaults to sapi
 def setSynthesizer(params=synthesizer,ID = "",region ='westeurope'):
-    global synthesizer, speech_config, audio_config,azureSynthesizer, voice, cogServicesID
+    global synthesizer, voice, cogServicesID
     synthesizer = params
     voice = ""
     cogServicesID = ID
     if params.lower() == 'azure':
         setVoice("LibbyNeural")
     
 # Set the speed of the speech in words per min.
@@ -939,41 +954,34 @@
             if phonemes[i] > max:
                 max = phonemes[i]
 
         for i in range(0, len(phonemes) - 1):
             phonemes[i] = phonemes[i] * 10 / max
             # print ('visnorm', i, ":", times[i], ':', phonemes[i])
     
-    # Use the bottom lip to push the top lip above the centre point if it is below
-       
-    if lipSync:
-        if soundDelay > 0:
-            # Set up a thread for the speech sound synthesis, delay start by soundDelay
-            t = threading.Timer(soundDelay, _playSpeech, args=(hdmiAudio,), kwargs=None)
-            # Set up a thread for the speech movement
-            t2 = threading.Thread(target=_moveSpeech, args=(phonemes, times,True))
-        else:
-            # Set up a thread for the speech sound synthesis
-            t = threading.Thread(target=_playSpeech, args=(hdmiAudio,))
-            # Set up a thread for the speech movement, delay start by - soundDelay
-            t2 = threading.Timer(-soundDelay, _moveSpeech, args=(phonemes, times,True), kwargs=None)
-        t2.start()
+    if soundDelay > 0:
+        # Set up a thread for the speech sound synthesis, delay start by soundDelay
+        t = threading.Timer(soundDelay, _playSpeech, args=(hdmiAudio,), kwargs=None)
+        # Set up a thread for the speech movement
+        t2 = threading.Thread(target=_moveSpeech, args=(phonemes, times, lipSync))
     else:
         # Set up a thread for the speech sound synthesis
         t = threading.Thread(target=_playSpeech, args=(hdmiAudio,))
-        t2 = threading.Timer(-soundDelay, _moveSpeech, args=(phonemes, times,False), kwargs=None)
-        t2.start()
+        # Set up a thread for the speech movement, delay start by - soundDelay
+        t2 = threading.Timer(-soundDelay, _moveSpeech, args=(phonemes, times, lipSync), kwargs=None)
+    t2.start()
     t.start()
 
     # if untilDone, keep running until speech has finished
     if untilDone:
         totalTime = times[len(times) - 1]
         startTime = time.time()
         while time.time() - startTime < totalTime:
-            continue
+            # wait to prevent blocking of other threads
+            wait (WAITLONG)
                 
 # Function to play back the speech wav file, if hmdi audio is being used play silence before speech sound
 def _playSpeech(addSilence):
     dir = os.path.dirname(os.path.abspath(__file__))
     silenceFile = os.path.join(dir, 'Silence1.wav')
 
     speechFile = speechAudioFile
@@ -992,43 +1000,49 @@
         if addSilence:
             commandString = 'aplay -D plug:default ' + silenceFile + '\naplay picohData/picohspeech.wav'
             os.system(commandString)
         else:
             os.system('aplay -D plug:default picohData/picohspeech.wav')
 
 
-# Function to move Picoh's lips in time with speech. Arguments | phonemes → list of phonemes[] | waits → list of waits[]
-def _moveSpeech(phonemes, times,autoSync = True):
-    global bottomLipPos
+# Function to set lipTopPos and lipBottomPos global variables to lip positions
+# Optionally moves Picoh's lips to these positions
+# Arguments | phonemes → list of phonemes[] | waits → list of waits[] | flag to do the physical move
+def _moveSpeech(phonemes, times, doMove):
+    global lipTopPos, lipBottomPos
     startTime = time.time()
     timeNow = 0
     totalTime = times[len(times) - 1]
     currentX = -1
     while timeNow < totalTime:
         timeNow = time.time() - startTime
         for x in range(0, len(times)):
             if timeNow > times[x] and x > currentX:
                 if synthesizer.upper() == "FESTIVAL":
-                    #posTop = _phonememapTopFest(phonemes[x])
-                    posBottom = _phonememapBottomFest(phonemes[x])
+                    lipTopPos = _phonememapTopFest(phonemes[x])
+                    lipBottomPos = _phonememapBottomFest(phonemes[x])
                 else:
-                    #posTop = _phonememapTop(phonemes[x])
-                    posBottom = _phonememapBottom(phonemes[x])
-                # move(TOPLIP, posTop, 10)
-
-                #posBottom = (((posBottom-5)/5)*3)+5
-                if autoSync:
-                    move(BOTTOMLIP, posBottom, 10)
-                bottomLipPos = posBottom
+                    lipTopPos = _phonememapTop(phonemes[x])
+                    lipBottomPos = _phonememapBottom(phonemes[x])
+
+                if (doMove):
+                    #move(TOPLIP, lipTopPos, 10)
+                    move(BOTTOMLIP, lipBottomPos, 10)
 
                 currentX = x
+        # wait to prevent blocking of other threads
+        wait(WAITLONG)
+                
     # move(TOPLIP, 5)
-    if autoSync:
+    if (doMove):
+        #move(TOPLIP, 5)
         move(BOTTOMLIP, 5)
-    bottomLipPos = posBottom
+        
+    lipTopPos = 5
+    lipBottomPos = 5
 
 # Function to limit values so they are between 0 - 10    
 def _limit(val):
     if val > 10:
         return 10
     elif val < 0:
         return 0
@@ -1128,23 +1142,27 @@
         'v': 5
     }.get(val, 5)
 
 # Function mapping phonemes to top lip positions.
 def _phonememapTop(val):
     return 5 + (_limit(val) / 2)
 
-# Function mapping phonemes to top lip positions.
+# Function mapping phonemes to bottom lip positions.
 # Bottom lip never goes over 9
 def _phonememapBottom(val):
     return 5 + (_limit(val) * 3 / 10)
 
-# Legacy function to support Ohbot programs with eyeColour. Passes onto baseColour.
+# Function to support Ohbot programs with eyeColour. Passes onto baseColour.
 def eyeColour(r, g, b, swapRandG=False):
     baseColour(r, g, b, swapRandG)
 
+# Function to support Ohbot programs with eyeColour, mirrors eyeColour().
+def setEyeColour(r, g, b, swapRandG=False):
+    eyeColour(r, g, b, swapRandG)
+
 # Clone of base colour to keep consitency with set eyeShape etc.
 def setBaseColour(r, g, b, swapRandG=False):
     baseColour(r, g, b, swapRandG)
 
 # US Spelling
 def setBaseColor(r, g, b, swapRandG=False):
     baseColour(r, g, b, swapRandG)
@@ -1219,15 +1237,15 @@
 
     # Reset Picoh back to start position
 def reset():
     baseColour(0, 0, 0)
     setEyeShape(defaultEyeShape, defaultEyeShape)
     for x in range(len(restPos) - 1,-1,-1):
         move(x, restPos[x])
-        wait(0.1)
+        wait(WAITLONG)
     close()
 
 # Return the sensor value between 0-10 for a given sensor number. Values stored in sensors[] array.
 def readSensor(index):
     ser.flushInput()
 
     msg = "i0" + str(index) + "\n"
@@ -1357,15 +1375,15 @@
     # Send hex to Picoh.
 
     if leftHex == '':
         print(str(shapeNameLeft) + " Eyeshape Not Found")
         return
     if connected:
         _setEyes(rightHex, leftHex, autoMirrorVar)
-        wait(0.05)
+        wait(WAITMEDIUM)
         move(EYETILT, lastfeyl,1)
         move(EYETILT, lastfeyr,2)
 
         move(EYETURN, lastfexl,1)
         move(EYETURN, lastfexr,2)
```

### Comparing `picoh-1.275/setup.py` & `picoh-1.276/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from distutils.core import setup
 
 import platform
 
 if platform.system() == "Darwin":
-    includes =['pyserial','lxml','playsound','pyobjc','numpy','comtypes','requests']
+    includes =['pyserial','lxml','playsound','numpy','comtypes','requests']
 
 if platform.system() == "Windows":
     includes =['pyserial','lxml','playsound','numpy','comtypes','requests']
 
 if platform.system() == "Linux":
     includes =['pyserial','playsound','gTTS','pydub','requests']
 
 setup(
     name = 'picoh',
     packages = ['picoh'],
       package_data={'': ['PicohSettings.xml','Silence1.wav','picohspeech.wav','PicohSpeech.csv','ohbot.obe','phonemes.txt','Images/movedown.gif','Images/moveright.gif','Images/off.gif','Images/offsmaller.gif','Images/on.gif','Images/onsmaller.gif','Images/picohlogo.gif','Images/picohlogoOn.gif','Images/picohlogoSmall.gif','Images/calibrate400.gif','Images/calibrate2400.gif','Images/plus.gif','Images/resetIcon.gif','Images/savebutton.gif','Images/logoPT.gif','MotorDefinitionsPicoh.omd','Images/pixel.gif','Sounds/fanfare.wav','Sounds/loop.wav','Sounds/ohbot.wav','Sounds/smash.wav','Sounds/spring.wav']},
     include_package_data=True,
-    version = '1.275',
+    version = '1.276',
     description = 'Python library for controlling Picoh Robot',
     author = 'ohbot',
     author_email = 'info@ohbot.co.uk',
     url = 'https://github.com/ohbot/picoh',
     download_url = 'https://github.com/ohbot/picoh-python/archive/1.26.tar.gz',
     keywords = ['ohbot', 'robot','picoh'],
     classifiers = [],
```

