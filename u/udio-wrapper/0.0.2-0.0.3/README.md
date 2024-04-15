# Comparing `tmp/udio_wrapper-0.0.2.tar.gz` & `tmp/udio_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udio_wrapper-0.0.2.tar", last modified: Sat Apr 13 15:12:12 2024, max compression
+gzip compressed data, was "udio_wrapper-0.0.3.tar", last modified: Mon Apr 15 15:33:15 2024, max compression
```

## Comparing `udio_wrapper-0.0.2.tar` & `udio_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2024-04-13 15:12:12.480425 udio_wrapper-0.0.2/
--rw-r--r--   0 marc       (501) staff       (20)     1063 2024-04-12 14:51:54.000000 udio_wrapper-0.0.2/LICENSE
--rw-r--r--   0 marc       (501) staff       (20)     7451 2024-04-13 15:12:12.480145 udio_wrapper-0.0.2/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)     6921 2024-04-13 15:09:07.000000 udio_wrapper-0.0.2/README.md
--rw-r--r--   0 marc       (501) staff       (20)       38 2024-04-13 15:12:12.480501 udio_wrapper-0.0.2/setup.cfg
--rw-r--r--   0 marc       (501) staff       (20)      865 2024-04-13 15:11:48.000000 udio_wrapper-0.0.2/setup.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2024-04-13 15:12:12.477924 udio_wrapper-0.0.2/udio_wrapper/
--rw-r--r--   0 marc       (501) staff       (20)     4456 2024-04-13 15:08:37.000000 udio_wrapper-0.0.2/udio_wrapper/__init__.py
-drwxr-xr-x   0 marc       (501) staff       (20)        0 2024-04-13 15:12:12.479438 udio_wrapper-0.0.2/udio_wrapper.egg-info/
--rw-r--r--   0 marc       (501) staff       (20)     7451 2024-04-13 15:12:12.000000 udio_wrapper-0.0.2/udio_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 marc       (501) staff       (20)      230 2024-04-13 15:12:12.000000 udio_wrapper-0.0.2/udio_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 marc       (501) staff       (20)        1 2024-04-13 15:12:12.000000 udio_wrapper-0.0.2/udio_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 marc       (501) staff       (20)       17 2024-04-13 15:12:12.000000 udio_wrapper-0.0.2/udio_wrapper.egg-info/requires.txt
--rw-r--r--   0 marc       (501) staff       (20)       13 2024-04-13 15:12:12.000000 udio_wrapper-0.0.2/udio_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2024-04-15 15:33:15.551318 udio_wrapper-0.0.3/
+-rw-r--r--   0 marc       (501) staff       (20)     1063 2024-04-12 14:51:54.000000 udio_wrapper-0.0.3/LICENSE
+-rw-r--r--   0 marc       (501) staff       (20)     7649 2024-04-15 15:33:15.551146 udio_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)     7119 2024-04-15 15:32:06.000000 udio_wrapper-0.0.3/README.md
+-rw-r--r--   0 marc       (501) staff       (20)       38 2024-04-15 15:33:15.551385 udio_wrapper-0.0.3/setup.cfg
+-rw-r--r--   0 marc       (501) staff       (20)      865 2024-04-15 15:32:10.000000 udio_wrapper-0.0.3/setup.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2024-04-15 15:33:15.550098 udio_wrapper-0.0.3/udio_wrapper/
+-rw-r--r--   0 marc       (501) staff       (20)     9391 2024-04-15 15:31:40.000000 udio_wrapper-0.0.3/udio_wrapper/__init__.py
+drwxr-xr-x   0 marc       (501) staff       (20)        0 2024-04-15 15:33:15.550907 udio_wrapper-0.0.3/udio_wrapper.egg-info/
+-rw-r--r--   0 marc       (501) staff       (20)     7649 2024-04-15 15:33:15.000000 udio_wrapper-0.0.3/udio_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 marc       (501) staff       (20)      230 2024-04-15 15:33:15.000000 udio_wrapper-0.0.3/udio_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 marc       (501) staff       (20)        1 2024-04-15 15:33:15.000000 udio_wrapper-0.0.3/udio_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 marc       (501) staff       (20)       17 2024-04-15 15:33:15.000000 udio_wrapper-0.0.3/udio_wrapper.egg-info/requires.txt
+-rw-r--r--   0 marc       (501) staff       (20)       13 2024-04-15 15:33:15.000000 udio_wrapper-0.0.3/udio_wrapper.egg-info/top_level.txt
```

### Comparing `udio_wrapper-0.0.2/LICENSE` & `udio_wrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `udio_wrapper-0.0.2/PKG-INFO` & `udio_wrapper-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udio_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generates songs using the Udio API using textual prompts.
 Home-page: https://github.com/flowese/UdioWrapper
 Author: Flowese
 Author-email: flowese@gmail.com
 Keywords: audio,music,generation,API,AI,Udio
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,14 +46,20 @@
 
 To install the package from PyPI, run the following command:
 
 ```bash
 pip install udio_wrapper
 ```
 
+To upgrade the package from PyPI, run the following command:
+```bash
+pip install --upgrade --no-cache-dir udio_wrapper
+```
+
+
 ### From GitHub Repository
 
 To install the package directly from the GitHub repository, run:
 
 ```bash
 pip install git+https://github.com/flowese/UdioWrapper.git
 ```
@@ -76,106 +82,96 @@
 
 To use `udio_wrapper`, import the `UdioWrapper` class and provide the necessary parameters.
 
 ## Usage Examples
 
 The following examples demonstrate various ways to use the `UdioWrapper` to generate music based on different scenarios:
 
-Generating a Complete Song with Automatically Generated Lyrics
 ```python
-from udio_wrapper import UdioWrapper
-
-udio = UdioWrapper(auth_token="your_auth_token_here")
-auto_song_url = udio.inference(
-    original_prompt="A song about the wonders of nature",
-    number_of_extensions=1,
-    extend_prompt="Keep singing about the beauty of the forest",
-    outro_prompt="Concluding with the serene sunset",
-    save_to_disk=True
-)
-print(f"URL of the complete song with automatic lyrics: {auto_song_url}")
-
+auth_token = "your-auth-token-here"  # Replace this with your actual authentication token
+udio_wrapper = UdioWrapper(auth_token)
 ```
 
-Generating a Complete Instrumental Song
+1. Creating a Short Song
+You can specify the prompt, seed, custom lyrics.
 ```python
-instrumental_song_url = udio.inference(
-    original_prompt="Smooth jazz instrumental music",
-    original_lyric_input="",
-    number_of_extensions=1,
-    extend_prompt="Continue the smooth jazz vibe",
-    extend_lyric_input="",
-    outro_prompt="Finish with a calming jazz outro",
-    outro_lyric_input="",
-    save_to_disk=True
-)
-print(f"URL of the complete instrumental song: {instrumental_song_url}")
 
+short_song_no_download = udio_wrapper.create_song(
+    prompt="Relaxing jazz and soulful music",
+    seed=-1,
+    custom_lyrics="Short song lyrics here"
+)
+print("Short song generated without downloading:", short_song_no_download)
 ```
-
-Generating a Complete Song with Custom Lyrics
+2. Extending a Song
+Extend a previously created song by providing its path and ID for conditioning. This method also allows for lyric customization.
 ```python
-custom_lyric_song_url = udio.inference(
-    original_prompt="A ballad about lost love",
-    original_lyric_input="Here under the moonlight, I remember your smile",
-    number_of_extensions=1,
-    extend_prompt="Continuing the tale of our summer love",
-    extend_lyric_input="Now all I have is the echo of your laughter",
-    outro_prompt="Ending our story as the leaves begin to fall",
-    outro_lyric_input="Farewell my love, until we meet again",
-    save_to_disk=True
-)
-print(f"URL of the complete song with custom lyrics: {custom_lyric_song_url}")
 
+extend_song_download = udio_wrapper.extend(
+    prompt="A dynamic version of relaxing jazz and soulful music",
+    seed=-1,
+    audio_conditioning_path="url-generated-song",
+    audio_conditioning_song_id="previous-song-id",
+    custom_lyrics="Extended version lyrics"
+)
+print("Extended song generated and downloaded:", extend_song_download)
 ```
 
-Generating a Simple Song with Custom Lyrics (No Extensions or Outro)
+3. Adding an Outro
+Generate an outro for your music sequence using the last song as a base. This includes custom lyrics.
 ```python
-simple_custom_lyric_song_url = udio.inference(
-    original_prompt="A pop song about bright city nights",
-    original_lyric_input="Neon lights and lonely hearts",
-    save_to_disk=True
-)
-print(f"URL of the simple song with custom lyrics: {simple_custom_lyric_song_url}")
 
+outro_song_download = udio_wrapper.add_outro(
+    prompt="A smooth ending to our jazz session",
+    seed=-1,
+    audio_conditioning_path="url-generated-song",
+    audio_conditioning_song_id="last-extended-song-id",
+    custom_lyrics="Outro lyrics here"
+)
+print("Outro song generated and downloaded:", outro_song_download)
 ```
 
-Generating a Simple Instrumental Song (No Extensions or Outro)
+4. Creating a Complete Song Sequence
+Generate a full sequence of songs, including multiple extensions and an outro. This process involves defining prompts and lyrics for each part of the sequence.
 ```python
-simple_instrumental_song_url = udio.inference(
-    original_prompt="Classical piano piece in minor key",
-    original_lyric_input="",
-    save_to_disk=True
+complete_song_sequence = udio_wrapper.create_complete_song(
+    short_prompt="On a full moon night",
+    extend_prompts=["the soft sound of the saxophone fills the air", "creating an atmosphere of mystery and romance"],
+    outro_prompt="Thus ends this melody, leaving an echo of emotions in the heart",
+    num_extensions=2,
+    custom_lyrics_short="Short song lyrics here",
+    custom_lyrics_extend=["Lyrics for first extension", "Lyrics for second extension"],
+    custom_lyrics_outro="Outro lyrics here"
 )
-print(f"URL of the simple instrumental song: {simple_instrumental_song_url}")
-
+print("Complete song sequence generated and downloaded:", complete_song_sequence)
 ```
 
-
 #### Parameters
 
-Each parameter in the `UdioWrapper` inference method has a specific purpose for creating customized music tracks:
-
 - **`auth_token`** *(Required)*: The authorization token you obtained from Udio, which is necessary for authenticating and making API requests.
 
-- **`original_prompt`** *(Required)*: The initial textual prompt that sets the thematic direction for generating the first track. This is the creative seed from which the song is grown.
 
-- **`original_lyric_input`** *(Optional)*: Specifies the lyrics for the initial track. If provided as an empty string (`""`), the resulting song will be purely instrumental. If omitted, Udio's API will automatically generate lyrics based on the `original_prompt`.
+Each method in the `UdioWrapper` class can take several parameters to control song generation and processing. Below is a breakdown of the parameters and their usage:
+
+- **prompt** *(str)*: A text prompt describing the theme or emotion of the song. This is the creative input from which the song generation is based.
+
+- **seed** *(int, optional)*: A seed number to ensure the reproducibility of the song generation. Using the same seed with the same parameters will generate the same audio output. Default is `-1`, which results in random generation each time.
+
+- **custom_lyrics** *(str, optional)*: Lyrics written by the user to be included in the song. If no lyrics are provided, the generation relies solely on the musical style implied by the prompt.
 
-- **`number_of_extensions`** *(Optional)*: The number of times the initial track should be extended. Each extension will be based on the last segment of the music generated in the previous step. The default value is 0, which means no extensions.
+- **audio_conditioning_path** *(str, optional)*: The file path to an audio file that will serve as a base or influence for the song being generated. This is used primarily for extending songs or generating outros based on a previous song.
 
-- **`extend_prompt`** *(Optional)*: The textual prompt for each extension phase. This prompt should ideally continue the theme or style set by the `original_prompt`.
+- **audio_conditioning_song_id** *(str, optional)*: The identifier of a previously generated song that will be used to influence the current song generation. This is necessary when creating extended songs or outros that are meant to follow a specific musical piece.
 
-- **`extend_lyric_input`** *(Optional)*: Custom lyrics for each extension phase. If this parameter is set to an empty string, the extension will be instrumental. If omitted, the API will automatically generate lyrics that attempt to continue the thematic content of the song.
+- **num_extensions** *(int, optional)*: Specifies the number of extended songs to generate in a sequence. This parameter is only used in the method that generates a complete song sequence. Default is `1`.
 
-- **`outro_prompt`** *(Optional)*: The textual prompt for the outro of the song, providing a thematic and musical conclusion.
+- **extend_prompts** *(list of str, optional)*: A list of prompts for generating each extension in a sequence. Each prompt should ideally reflect a progression or variation in style or theme from the previous song.
 
-- **`outro_lyric_input`** *(Optional)*: Custom lyrics for the outro. If provided as an empty string, the outro will be instrumental. If omitted, the API will generate lyrics that cap off the song's narrative.
+- **outro_prompt** *(str, optional)*: A prompt specifically for generating an outro. This should convey a sense of conclusion or finale relative to the musical sequence.
 
-- **`save_to_disk`** *(Optional)*: A boolean indicating whether to save the generated tracks to the disk. The default is `True`, which means the tracks will be saved.
 
 These parameters allow full customization of the music generation process, from the initial creation through extensions to the final outro, giving users the ability to tailor both the music and lyrics to fit their specific needs or artistic vision.
 
 
 ## License
 
 This project is licensed under the MIT License.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: udio_wrapper Version: 0.0.2 Summary: Generates
+Metadata-Version: 2.1 Name: udio_wrapper Version: 0.0.3 Summary: Generates
 songs using the Udio API using textual prompts. Home-page: https://github.com/
 flowese/UdioWrapper Author: Flowese Author-email: flowese@gmail.com Keywords:
 audio,music,generation,API,AI,Udio Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: requests==2.31.0 # Udio Wrapper !
 [Udio Wrapper](banner.jpeg) Written by @Flowese _[_O_p_e_n_ _D_e_m_o_ _I_n_ _C_o_l_a_b_]##
@@ -12,82 +12,86 @@
 Over Other Models Unlike other music generation models, Udio offers a unique
 feature of extending or conditioning new tracks based on existing ones, making
 it ideal for iterative and creative music production processes. ## Legal
 Disclaimer This package is created for educational and research purposes. By
 using this package, you agree to do so at your own risk. This package is not
 affiliated, endorsed, or sponsored by Udio in any way. ## Requirements - Python
 3.x - pip ## Installation ### From PyPI To install the package from PyPI, run
-the following command: ```bash pip install udio_wrapper ``` ### From GitHub
-Repository To install the package directly from the GitHub repository, run:
-```bash pip install git+https://github.com/flowese/UdioWrapper.git ``` ##
-Configuration ### Obtaining the Authorization Token 1. Sign up at [Udio](https:
-//www.udio.com/). 2. Once registered, open your browser's inspector: - In
-Chrome: `Ctrl+Shift+I` or `F12` on Windows, `Cmd+Option+I` on Mac. 3. Go to the
-`Application` tab. 4. On the left panel, locate and click on `Cookies`, then
-select the Ideogram website. 5. Find the cookie named `sb-api-auth-token`. 6.
-Click on `sb-api-auth-token` and copy the value in the `Value` field. ![Udio
-Wrapper](screen_cookies.jpeg) ### Usage To use `udio_wrapper`, import the
-`UdioWrapper` class and provide the necessary parameters. ## Usage Examples The
-following examples demonstrate various ways to use the `UdioWrapper` to
-generate music based on different scenarios: Generating a Complete Song with
-Automatically Generated Lyrics ```python from udio_wrapper import UdioWrapper
-udio = UdioWrapper(auth_token="your_auth_token_here") auto_song_url =
-udio.inference( original_prompt="A song about the wonders of nature",
-number_of_extensions=1, extend_prompt="Keep singing about the beauty of the
-forest", outro_prompt="Concluding with the serene sunset", save_to_disk=True )
-print(f"URL of the complete song with automatic lyrics: {auto_song_url}") ```
-Generating a Complete Instrumental Song ```python instrumental_song_url =
-udio.inference( original_prompt="Smooth jazz instrumental music",
-original_lyric_input="", number_of_extensions=1, extend_prompt="Continue the
-smooth jazz vibe", extend_lyric_input="", outro_prompt="Finish with a calming
-jazz outro", outro_lyric_input="", save_to_disk=True ) print(f"URL of the
-complete instrumental song: {instrumental_song_url}") ``` Generating a Complete
-Song with Custom Lyrics ```python custom_lyric_song_url = udio.inference
-( original_prompt="A ballad about lost love", original_lyric_input="Here under
-the moonlight, I remember your smile", number_of_extensions=1,
-extend_prompt="Continuing the tale of our summer love", extend_lyric_input="Now
-all I have is the echo of your laughter", outro_prompt="Ending our story as the
-leaves begin to fall", outro_lyric_input="Farewell my love, until we meet
-again", save_to_disk=True ) print(f"URL of the complete song with custom
-lyrics: {custom_lyric_song_url}") ``` Generating a Simple Song with Custom
-Lyrics (No Extensions or Outro) ```python simple_custom_lyric_song_url =
-udio.inference( original_prompt="A pop song about bright city nights",
-original_lyric_input="Neon lights and lonely hearts", save_to_disk=True ) print
-(f"URL of the simple song with custom lyrics: {simple_custom_lyric_song_url}")
-``` Generating a Simple Instrumental Song (No Extensions or Outro) ```python
-simple_instrumental_song_url = udio.inference( original_prompt="Classical piano
-piece in minor key", original_lyric_input="", save_to_disk=True ) print(f"URL
-of the simple instrumental song: {simple_instrumental_song_url}") ``` ####
-Parameters Each parameter in the `UdioWrapper` inference method has a specific
-purpose for creating customized music tracks: - **`auth_token`** *(Required)*:
-The authorization token you obtained from Udio, which is necessary for
-authenticating and making API requests. - **`original_prompt`** *(Required)*:
-The initial textual prompt that sets the thematic direction for generating the
-first track. This is the creative seed from which the song is grown. -
-**`original_lyric_input`** *(Optional)*: Specifies the lyrics for the initial
-track. If provided as an empty string (`""`), the resulting song will be purely
-instrumental. If omitted, Udio's API will automatically generate lyrics based
-on the `original_prompt`. - **`number_of_extensions`** *(Optional)*: The number
-of times the initial track should be extended. Each extension will be based on
-the last segment of the music generated in the previous step. The default value
-is 0, which means no extensions. - **`extend_prompt`** *(Optional)*: The
-textual prompt for each extension phase. This prompt should ideally continue
-the theme or style set by the `original_prompt`. - **`extend_lyric_input`** *
-(Optional)*: Custom lyrics for each extension phase. If this parameter is set
-to an empty string, the extension will be instrumental. If omitted, the API
-will automatically generate lyrics that attempt to continue the thematic
-content of the song. - **`outro_prompt`** *(Optional)*: The textual prompt for
-the outro of the song, providing a thematic and musical conclusion. -
-**`outro_lyric_input`** *(Optional)*: Custom lyrics for the outro. If provided
-as an empty string, the outro will be instrumental. If omitted, the API will
-generate lyrics that cap off the song's narrative. - **`save_to_disk`** *
-(Optional)*: A boolean indicating whether to save the generated tracks to the
-disk. The default is `True`, which means the tracks will be saved. These
-parameters allow full customization of the music generation process, from the
-initial creation through extensions to the final outro, giving users the
-ability to tailor both the music and lyrics to fit their specific needs or
-artistic vision. ## License This project is licensed under the MIT License. ##
-Contributing If you'd like to contribute to this project, feel free to fork the
-repository and send a pull request, or open an issue to discuss what you'd like
-to change. All contributions are welcome! ## TODO ### Pending Tasks and
-Features - Improve error handling and response validation. - Implement a user-
-friendly web interface for easier interaction with the API. -----
+the following command: ```bash pip install udio_wrapper ``` To upgrade the
+package from PyPI, run the following command: ```bash pip install --upgrade --
+no-cache-dir udio_wrapper ``` ### From GitHub Repository To install the package
+directly from the GitHub repository, run: ```bash pip install git+https://
+github.com/flowese/UdioWrapper.git ``` ## Configuration ### Obtaining the
+Authorization Token 1. Sign up at [Udio](https://www.udio.com/). 2. Once
+registered, open your browser's inspector: - In Chrome: `Ctrl+Shift+I` or `F12`
+on Windows, `Cmd+Option+I` on Mac. 3. Go to the `Application` tab. 4. On the
+left panel, locate and click on `Cookies`, then select the Ideogram website. 5.
+Find the cookie named `sb-api-auth-token`. 6. Click on `sb-api-auth-token` and
+copy the value in the `Value` field. ![Udio Wrapper](screen_cookies.jpeg) ###
+Usage To use `udio_wrapper`, import the `UdioWrapper` class and provide the
+necessary parameters. ## Usage Examples The following examples demonstrate
+various ways to use the `UdioWrapper` to generate music based on different
+scenarios: ```python auth_token = "your-auth-token-here" # Replace this with
+your actual authentication token udio_wrapper = UdioWrapper(auth_token) ``` 1.
+Creating a Short Song You can specify the prompt, seed, custom lyrics.
+```python short_song_no_download = udio_wrapper.create_song( prompt="Relaxing
+jazz and soulful music", seed=-1, custom_lyrics="Short song lyrics here" )
+print("Short song generated without downloading:", short_song_no_download) ```
+2. Extending a Song Extend a previously created song by providing its path and
+ID for conditioning. This method also allows for lyric customization. ```python
+extend_song_download = udio_wrapper.extend( prompt="A dynamic version of
+relaxing jazz and soulful music", seed=-1, audio_conditioning_path="url-
+generated-song", audio_conditioning_song_id="previous-song-id",
+custom_lyrics="Extended version lyrics" ) print("Extended song generated and
+downloaded:", extend_song_download) ``` 3. Adding an Outro Generate an outro
+for your music sequence using the last song as a base. This includes custom
+lyrics. ```python outro_song_download = udio_wrapper.add_outro( prompt="A
+smooth ending to our jazz session", seed=-1, audio_conditioning_path="url-
+generated-song", audio_conditioning_song_id="last-extended-song-id",
+custom_lyrics="Outro lyrics here" ) print("Outro song generated and downloaded:
+", outro_song_download) ``` 4. Creating a Complete Song Sequence Generate a
+full sequence of songs, including multiple extensions and an outro. This
+process involves defining prompts and lyrics for each part of the sequence.
+```python complete_song_sequence = udio_wrapper.create_complete_song
+( short_prompt="On a full moon night", extend_prompts=["the soft sound of the
+saxophone fills the air", "creating an atmosphere of mystery and romance"],
+outro_prompt="Thus ends this melody, leaving an echo of emotions in the heart",
+num_extensions=2, custom_lyrics_short="Short song lyrics here",
+custom_lyrics_extend=["Lyrics for first extension", "Lyrics for second
+extension"], custom_lyrics_outro="Outro lyrics here" ) print("Complete song
+sequence generated and downloaded:", complete_song_sequence) ``` ####
+Parameters - **`auth_token`** *(Required)*: The authorization token you
+obtained from Udio, which is necessary for authenticating and making API
+requests. Each method in the `UdioWrapper` class can take several parameters to
+control song generation and processing. Below is a breakdown of the parameters
+and their usage: - **prompt** *(str)*: A text prompt describing the theme or
+emotion of the song. This is the creative input from which the song generation
+is based. - **seed** *(int, optional)*: A seed number to ensure the
+reproducibility of the song generation. Using the same seed with the same
+parameters will generate the same audio output. Default is `-1`, which results
+in random generation each time. - **custom_lyrics** *(str, optional)*: Lyrics
+written by the user to be included in the song. If no lyrics are provided, the
+generation relies solely on the musical style implied by the prompt. -
+**audio_conditioning_path** *(str, optional)*: The file path to an audio file
+that will serve as a base or influence for the song being generated. This is
+used primarily for extending songs or generating outros based on a previous
+song. - **audio_conditioning_song_id** *(str, optional)*: The identifier of a
+previously generated song that will be used to influence the current song
+generation. This is necessary when creating extended songs or outros that are
+meant to follow a specific musical piece. - **num_extensions** *(int,
+optional)*: Specifies the number of extended songs to generate in a sequence.
+This parameter is only used in the method that generates a complete song
+sequence. Default is `1`. - **extend_prompts** *(list of str, optional)*: A
+list of prompts for generating each extension in a sequence. Each prompt should
+ideally reflect a progression or variation in style or theme from the previous
+song. - **outro_prompt** *(str, optional)*: A prompt specifically for
+generating an outro. This should convey a sense of conclusion or finale
+relative to the musical sequence. These parameters allow full customization of
+the music generation process, from the initial creation through extensions to
+the final outro, giving users the ability to tailor both the music and lyrics
+to fit their specific needs or artistic vision. ## License This project is
+licensed under the MIT License. ## Contributing If you'd like to contribute to
+this project, feel free to fork the repository and send a pull request, or open
+an issue to discuss what you'd like to change. All contributions are welcome!
+## TODO ### Pending Tasks and Features - Improve error handling and response
+validation. - Implement a user-friendly web interface for easier interaction
+with the API. -----
```

### Comparing `udio_wrapper-0.0.2/README.md` & `udio_wrapper-0.0.3/udio_wrapper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: udio-wrapper
+Version: 0.0.3
+Summary: Generates songs using the Udio API using textual prompts.
+Home-page: https://github.com/flowese/UdioWrapper
+Author: Flowese
+Author-email: flowese@gmail.com
+Keywords: audio,music,generation,API,AI,Udio
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests==2.31.0
+
 
 # Udio Wrapper
 
 ![Udio Wrapper](banner.jpeg)
 
 Written by @Flowese
 
@@ -30,14 +46,20 @@
 
 To install the package from PyPI, run the following command:
 
 ```bash
 pip install udio_wrapper
 ```
 
+To upgrade the package from PyPI, run the following command:
+```bash
+pip install --upgrade --no-cache-dir udio_wrapper
+```
+
+
 ### From GitHub Repository
 
 To install the package directly from the GitHub repository, run:
 
 ```bash
 pip install git+https://github.com/flowese/UdioWrapper.git
 ```
@@ -60,106 +82,96 @@
 
 To use `udio_wrapper`, import the `UdioWrapper` class and provide the necessary parameters.
 
 ## Usage Examples
 
 The following examples demonstrate various ways to use the `UdioWrapper` to generate music based on different scenarios:
 
-Generating a Complete Song with Automatically Generated Lyrics
 ```python
-from udio_wrapper import UdioWrapper
-
-udio = UdioWrapper(auth_token="your_auth_token_here")
-auto_song_url = udio.inference(
-    original_prompt="A song about the wonders of nature",
-    number_of_extensions=1,
-    extend_prompt="Keep singing about the beauty of the forest",
-    outro_prompt="Concluding with the serene sunset",
-    save_to_disk=True
-)
-print(f"URL of the complete song with automatic lyrics: {auto_song_url}")
-
+auth_token = "your-auth-token-here"  # Replace this with your actual authentication token
+udio_wrapper = UdioWrapper(auth_token)
 ```
 
-Generating a Complete Instrumental Song
+1. Creating a Short Song
+You can specify the prompt, seed, custom lyrics.
 ```python
-instrumental_song_url = udio.inference(
-    original_prompt="Smooth jazz instrumental music",
-    original_lyric_input="",
-    number_of_extensions=1,
-    extend_prompt="Continue the smooth jazz vibe",
-    extend_lyric_input="",
-    outro_prompt="Finish with a calming jazz outro",
-    outro_lyric_input="",
-    save_to_disk=True
-)
-print(f"URL of the complete instrumental song: {instrumental_song_url}")
 
+short_song_no_download = udio_wrapper.create_song(
+    prompt="Relaxing jazz and soulful music",
+    seed=-1,
+    custom_lyrics="Short song lyrics here"
+)
+print("Short song generated without downloading:", short_song_no_download)
 ```
-
-Generating a Complete Song with Custom Lyrics
+2. Extending a Song
+Extend a previously created song by providing its path and ID for conditioning. This method also allows for lyric customization.
 ```python
-custom_lyric_song_url = udio.inference(
-    original_prompt="A ballad about lost love",
-    original_lyric_input="Here under the moonlight, I remember your smile",
-    number_of_extensions=1,
-    extend_prompt="Continuing the tale of our summer love",
-    extend_lyric_input="Now all I have is the echo of your laughter",
-    outro_prompt="Ending our story as the leaves begin to fall",
-    outro_lyric_input="Farewell my love, until we meet again",
-    save_to_disk=True
-)
-print(f"URL of the complete song with custom lyrics: {custom_lyric_song_url}")
 
+extend_song_download = udio_wrapper.extend(
+    prompt="A dynamic version of relaxing jazz and soulful music",
+    seed=-1,
+    audio_conditioning_path="url-generated-song",
+    audio_conditioning_song_id="previous-song-id",
+    custom_lyrics="Extended version lyrics"
+)
+print("Extended song generated and downloaded:", extend_song_download)
 ```
 
-Generating a Simple Song with Custom Lyrics (No Extensions or Outro)
+3. Adding an Outro
+Generate an outro for your music sequence using the last song as a base. This includes custom lyrics.
 ```python
-simple_custom_lyric_song_url = udio.inference(
-    original_prompt="A pop song about bright city nights",
-    original_lyric_input="Neon lights and lonely hearts",
-    save_to_disk=True
-)
-print(f"URL of the simple song with custom lyrics: {simple_custom_lyric_song_url}")
 
+outro_song_download = udio_wrapper.add_outro(
+    prompt="A smooth ending to our jazz session",
+    seed=-1,
+    audio_conditioning_path="url-generated-song",
+    audio_conditioning_song_id="last-extended-song-id",
+    custom_lyrics="Outro lyrics here"
+)
+print("Outro song generated and downloaded:", outro_song_download)
 ```
 
-Generating a Simple Instrumental Song (No Extensions or Outro)
+4. Creating a Complete Song Sequence
+Generate a full sequence of songs, including multiple extensions and an outro. This process involves defining prompts and lyrics for each part of the sequence.
 ```python
-simple_instrumental_song_url = udio.inference(
-    original_prompt="Classical piano piece in minor key",
-    original_lyric_input="",
-    save_to_disk=True
+complete_song_sequence = udio_wrapper.create_complete_song(
+    short_prompt="On a full moon night",
+    extend_prompts=["the soft sound of the saxophone fills the air", "creating an atmosphere of mystery and romance"],
+    outro_prompt="Thus ends this melody, leaving an echo of emotions in the heart",
+    num_extensions=2,
+    custom_lyrics_short="Short song lyrics here",
+    custom_lyrics_extend=["Lyrics for first extension", "Lyrics for second extension"],
+    custom_lyrics_outro="Outro lyrics here"
 )
-print(f"URL of the simple instrumental song: {simple_instrumental_song_url}")
-
+print("Complete song sequence generated and downloaded:", complete_song_sequence)
 ```
 
-
 #### Parameters
 
-Each parameter in the `UdioWrapper` inference method has a specific purpose for creating customized music tracks:
-
 - **`auth_token`** *(Required)*: The authorization token you obtained from Udio, which is necessary for authenticating and making API requests.
 
-- **`original_prompt`** *(Required)*: The initial textual prompt that sets the thematic direction for generating the first track. This is the creative seed from which the song is grown.
 
-- **`original_lyric_input`** *(Optional)*: Specifies the lyrics for the initial track. If provided as an empty string (`""`), the resulting song will be purely instrumental. If omitted, Udio's API will automatically generate lyrics based on the `original_prompt`.
+Each method in the `UdioWrapper` class can take several parameters to control song generation and processing. Below is a breakdown of the parameters and their usage:
+
+- **prompt** *(str)*: A text prompt describing the theme or emotion of the song. This is the creative input from which the song generation is based.
+
+- **seed** *(int, optional)*: A seed number to ensure the reproducibility of the song generation. Using the same seed with the same parameters will generate the same audio output. Default is `-1`, which results in random generation each time.
+
+- **custom_lyrics** *(str, optional)*: Lyrics written by the user to be included in the song. If no lyrics are provided, the generation relies solely on the musical style implied by the prompt.
 
-- **`number_of_extensions`** *(Optional)*: The number of times the initial track should be extended. Each extension will be based on the last segment of the music generated in the previous step. The default value is 0, which means no extensions.
+- **audio_conditioning_path** *(str, optional)*: The file path to an audio file that will serve as a base or influence for the song being generated. This is used primarily for extending songs or generating outros based on a previous song.
 
-- **`extend_prompt`** *(Optional)*: The textual prompt for each extension phase. This prompt should ideally continue the theme or style set by the `original_prompt`.
+- **audio_conditioning_song_id** *(str, optional)*: The identifier of a previously generated song that will be used to influence the current song generation. This is necessary when creating extended songs or outros that are meant to follow a specific musical piece.
 
-- **`extend_lyric_input`** *(Optional)*: Custom lyrics for each extension phase. If this parameter is set to an empty string, the extension will be instrumental. If omitted, the API will automatically generate lyrics that attempt to continue the thematic content of the song.
+- **num_extensions** *(int, optional)*: Specifies the number of extended songs to generate in a sequence. This parameter is only used in the method that generates a complete song sequence. Default is `1`.
 
-- **`outro_prompt`** *(Optional)*: The textual prompt for the outro of the song, providing a thematic and musical conclusion.
+- **extend_prompts** *(list of str, optional)*: A list of prompts for generating each extension in a sequence. Each prompt should ideally reflect a progression or variation in style or theme from the previous song.
 
-- **`outro_lyric_input`** *(Optional)*: Custom lyrics for the outro. If provided as an empty string, the outro will be instrumental. If omitted, the API will generate lyrics that cap off the song's narrative.
+- **outro_prompt** *(str, optional)*: A prompt specifically for generating an outro. This should convey a sense of conclusion or finale relative to the musical sequence.
 
-- **`save_to_disk`** *(Optional)*: A boolean indicating whether to save the generated tracks to the disk. The default is `True`, which means the tracks will be saved.
 
 These parameters allow full customization of the music generation process, from the initial creation through extensions to the final outro, giving users the ability to tailor both the music and lyrics to fit their specific needs or artistic vision.
 
 
 ## License
 
 This project is licensed under the MIT License.
```

#### html2text {}

```diff
@@ -1,86 +1,97 @@
-# Udio Wrapper ![Udio Wrapper](banner.jpeg) Written by @Flowese _[_O_p_e_n_ _D_e_m_o_ _I_n
-_C_o_l_a_b_]## Description `udio_wrapper` is a Python package that allows you to
-generate music tracks from Udio's API using textual prompts. This package is
-designed to interact with Udio's API and is not officially endorsed by Udio. ##
-Advantages Over Other Models Unlike other music generation models, Udio offers
-a unique feature of extending or conditioning new tracks based on existing
-ones, making it ideal for iterative and creative music production processes. ##
-Legal Disclaimer This package is created for educational and research purposes.
-By using this package, you agree to do so at your own risk. This package is not
+Metadata-Version: 2.1 Name: udio-wrapper Version: 0.0.3 Summary: Generates
+songs using the Udio API using textual prompts. Home-page: https://github.com/
+flowese/UdioWrapper Author: Flowese Author-email: flowese@gmail.com Keywords:
+audio,music,generation,API,AI,Udio Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: requests==2.31.0 # Udio Wrapper !
+[Udio Wrapper](banner.jpeg) Written by @Flowese _[_O_p_e_n_ _D_e_m_o_ _I_n_ _C_o_l_a_b_]##
+Description `udio_wrapper` is a Python package that allows you to generate
+music tracks from Udio's API using textual prompts. This package is designed to
+interact with Udio's API and is not officially endorsed by Udio. ## Advantages
+Over Other Models Unlike other music generation models, Udio offers a unique
+feature of extending or conditioning new tracks based on existing ones, making
+it ideal for iterative and creative music production processes. ## Legal
+Disclaimer This package is created for educational and research purposes. By
+using this package, you agree to do so at your own risk. This package is not
 affiliated, endorsed, or sponsored by Udio in any way. ## Requirements - Python
 3.x - pip ## Installation ### From PyPI To install the package from PyPI, run
-the following command: ```bash pip install udio_wrapper ``` ### From GitHub
-Repository To install the package directly from the GitHub repository, run:
-```bash pip install git+https://github.com/flowese/UdioWrapper.git ``` ##
-Configuration ### Obtaining the Authorization Token 1. Sign up at [Udio](https:
-//www.udio.com/). 2. Once registered, open your browser's inspector: - In
-Chrome: `Ctrl+Shift+I` or `F12` on Windows, `Cmd+Option+I` on Mac. 3. Go to the
-`Application` tab. 4. On the left panel, locate and click on `Cookies`, then
-select the Ideogram website. 5. Find the cookie named `sb-api-auth-token`. 6.
-Click on `sb-api-auth-token` and copy the value in the `Value` field. ![Udio
-Wrapper](screen_cookies.jpeg) ### Usage To use `udio_wrapper`, import the
-`UdioWrapper` class and provide the necessary parameters. ## Usage Examples The
-following examples demonstrate various ways to use the `UdioWrapper` to
-generate music based on different scenarios: Generating a Complete Song with
-Automatically Generated Lyrics ```python from udio_wrapper import UdioWrapper
-udio = UdioWrapper(auth_token="your_auth_token_here") auto_song_url =
-udio.inference( original_prompt="A song about the wonders of nature",
-number_of_extensions=1, extend_prompt="Keep singing about the beauty of the
-forest", outro_prompt="Concluding with the serene sunset", save_to_disk=True )
-print(f"URL of the complete song with automatic lyrics: {auto_song_url}") ```
-Generating a Complete Instrumental Song ```python instrumental_song_url =
-udio.inference( original_prompt="Smooth jazz instrumental music",
-original_lyric_input="", number_of_extensions=1, extend_prompt="Continue the
-smooth jazz vibe", extend_lyric_input="", outro_prompt="Finish with a calming
-jazz outro", outro_lyric_input="", save_to_disk=True ) print(f"URL of the
-complete instrumental song: {instrumental_song_url}") ``` Generating a Complete
-Song with Custom Lyrics ```python custom_lyric_song_url = udio.inference
-( original_prompt="A ballad about lost love", original_lyric_input="Here under
-the moonlight, I remember your smile", number_of_extensions=1,
-extend_prompt="Continuing the tale of our summer love", extend_lyric_input="Now
-all I have is the echo of your laughter", outro_prompt="Ending our story as the
-leaves begin to fall", outro_lyric_input="Farewell my love, until we meet
-again", save_to_disk=True ) print(f"URL of the complete song with custom
-lyrics: {custom_lyric_song_url}") ``` Generating a Simple Song with Custom
-Lyrics (No Extensions or Outro) ```python simple_custom_lyric_song_url =
-udio.inference( original_prompt="A pop song about bright city nights",
-original_lyric_input="Neon lights and lonely hearts", save_to_disk=True ) print
-(f"URL of the simple song with custom lyrics: {simple_custom_lyric_song_url}")
-``` Generating a Simple Instrumental Song (No Extensions or Outro) ```python
-simple_instrumental_song_url = udio.inference( original_prompt="Classical piano
-piece in minor key", original_lyric_input="", save_to_disk=True ) print(f"URL
-of the simple instrumental song: {simple_instrumental_song_url}") ``` ####
-Parameters Each parameter in the `UdioWrapper` inference method has a specific
-purpose for creating customized music tracks: - **`auth_token`** *(Required)*:
-The authorization token you obtained from Udio, which is necessary for
-authenticating and making API requests. - **`original_prompt`** *(Required)*:
-The initial textual prompt that sets the thematic direction for generating the
-first track. This is the creative seed from which the song is grown. -
-**`original_lyric_input`** *(Optional)*: Specifies the lyrics for the initial
-track. If provided as an empty string (`""`), the resulting song will be purely
-instrumental. If omitted, Udio's API will automatically generate lyrics based
-on the `original_prompt`. - **`number_of_extensions`** *(Optional)*: The number
-of times the initial track should be extended. Each extension will be based on
-the last segment of the music generated in the previous step. The default value
-is 0, which means no extensions. - **`extend_prompt`** *(Optional)*: The
-textual prompt for each extension phase. This prompt should ideally continue
-the theme or style set by the `original_prompt`. - **`extend_lyric_input`** *
-(Optional)*: Custom lyrics for each extension phase. If this parameter is set
-to an empty string, the extension will be instrumental. If omitted, the API
-will automatically generate lyrics that attempt to continue the thematic
-content of the song. - **`outro_prompt`** *(Optional)*: The textual prompt for
-the outro of the song, providing a thematic and musical conclusion. -
-**`outro_lyric_input`** *(Optional)*: Custom lyrics for the outro. If provided
-as an empty string, the outro will be instrumental. If omitted, the API will
-generate lyrics that cap off the song's narrative. - **`save_to_disk`** *
-(Optional)*: A boolean indicating whether to save the generated tracks to the
-disk. The default is `True`, which means the tracks will be saved. These
-parameters allow full customization of the music generation process, from the
-initial creation through extensions to the final outro, giving users the
-ability to tailor both the music and lyrics to fit their specific needs or
-artistic vision. ## License This project is licensed under the MIT License. ##
-Contributing If you'd like to contribute to this project, feel free to fork the
-repository and send a pull request, or open an issue to discuss what you'd like
-to change. All contributions are welcome! ## TODO ### Pending Tasks and
-Features - Improve error handling and response validation. - Implement a user-
-friendly web interface for easier interaction with the API. -----
+the following command: ```bash pip install udio_wrapper ``` To upgrade the
+package from PyPI, run the following command: ```bash pip install --upgrade --
+no-cache-dir udio_wrapper ``` ### From GitHub Repository To install the package
+directly from the GitHub repository, run: ```bash pip install git+https://
+github.com/flowese/UdioWrapper.git ``` ## Configuration ### Obtaining the
+Authorization Token 1. Sign up at [Udio](https://www.udio.com/). 2. Once
+registered, open your browser's inspector: - In Chrome: `Ctrl+Shift+I` or `F12`
+on Windows, `Cmd+Option+I` on Mac. 3. Go to the `Application` tab. 4. On the
+left panel, locate and click on `Cookies`, then select the Ideogram website. 5.
+Find the cookie named `sb-api-auth-token`. 6. Click on `sb-api-auth-token` and
+copy the value in the `Value` field. ![Udio Wrapper](screen_cookies.jpeg) ###
+Usage To use `udio_wrapper`, import the `UdioWrapper` class and provide the
+necessary parameters. ## Usage Examples The following examples demonstrate
+various ways to use the `UdioWrapper` to generate music based on different
+scenarios: ```python auth_token = "your-auth-token-here" # Replace this with
+your actual authentication token udio_wrapper = UdioWrapper(auth_token) ``` 1.
+Creating a Short Song You can specify the prompt, seed, custom lyrics.
+```python short_song_no_download = udio_wrapper.create_song( prompt="Relaxing
+jazz and soulful music", seed=-1, custom_lyrics="Short song lyrics here" )
+print("Short song generated without downloading:", short_song_no_download) ```
+2. Extending a Song Extend a previously created song by providing its path and
+ID for conditioning. This method also allows for lyric customization. ```python
+extend_song_download = udio_wrapper.extend( prompt="A dynamic version of
+relaxing jazz and soulful music", seed=-1, audio_conditioning_path="url-
+generated-song", audio_conditioning_song_id="previous-song-id",
+custom_lyrics="Extended version lyrics" ) print("Extended song generated and
+downloaded:", extend_song_download) ``` 3. Adding an Outro Generate an outro
+for your music sequence using the last song as a base. This includes custom
+lyrics. ```python outro_song_download = udio_wrapper.add_outro( prompt="A
+smooth ending to our jazz session", seed=-1, audio_conditioning_path="url-
+generated-song", audio_conditioning_song_id="last-extended-song-id",
+custom_lyrics="Outro lyrics here" ) print("Outro song generated and downloaded:
+", outro_song_download) ``` 4. Creating a Complete Song Sequence Generate a
+full sequence of songs, including multiple extensions and an outro. This
+process involves defining prompts and lyrics for each part of the sequence.
+```python complete_song_sequence = udio_wrapper.create_complete_song
+( short_prompt="On a full moon night", extend_prompts=["the soft sound of the
+saxophone fills the air", "creating an atmosphere of mystery and romance"],
+outro_prompt="Thus ends this melody, leaving an echo of emotions in the heart",
+num_extensions=2, custom_lyrics_short="Short song lyrics here",
+custom_lyrics_extend=["Lyrics for first extension", "Lyrics for second
+extension"], custom_lyrics_outro="Outro lyrics here" ) print("Complete song
+sequence generated and downloaded:", complete_song_sequence) ``` ####
+Parameters - **`auth_token`** *(Required)*: The authorization token you
+obtained from Udio, which is necessary for authenticating and making API
+requests. Each method in the `UdioWrapper` class can take several parameters to
+control song generation and processing. Below is a breakdown of the parameters
+and their usage: - **prompt** *(str)*: A text prompt describing the theme or
+emotion of the song. This is the creative input from which the song generation
+is based. - **seed** *(int, optional)*: A seed number to ensure the
+reproducibility of the song generation. Using the same seed with the same
+parameters will generate the same audio output. Default is `-1`, which results
+in random generation each time. - **custom_lyrics** *(str, optional)*: Lyrics
+written by the user to be included in the song. If no lyrics are provided, the
+generation relies solely on the musical style implied by the prompt. -
+**audio_conditioning_path** *(str, optional)*: The file path to an audio file
+that will serve as a base or influence for the song being generated. This is
+used primarily for extending songs or generating outros based on a previous
+song. - **audio_conditioning_song_id** *(str, optional)*: The identifier of a
+previously generated song that will be used to influence the current song
+generation. This is necessary when creating extended songs or outros that are
+meant to follow a specific musical piece. - **num_extensions** *(int,
+optional)*: Specifies the number of extended songs to generate in a sequence.
+This parameter is only used in the method that generates a complete song
+sequence. Default is `1`. - **extend_prompts** *(list of str, optional)*: A
+list of prompts for generating each extension in a sequence. Each prompt should
+ideally reflect a progression or variation in style or theme from the previous
+song. - **outro_prompt** *(str, optional)*: A prompt specifically for
+generating an outro. This should convey a sense of conclusion or finale
+relative to the musical sequence. These parameters allow full customization of
+the music generation process, from the initial creation through extensions to
+the final outro, giving users the ability to tailor both the music and lyrics
+to fit their specific needs or artistic vision. ## License This project is
+licensed under the MIT License. ## Contributing If you'd like to contribute to
+this project, feel free to fork the repository and send a pull request, or open
+an issue to discuss what you'd like to change. All contributions are welcome!
+## TODO ### Pending Tasks and Features - Improve error handling and response
+validation. - Implement a user-friendly web interface for easier interaction
+with the API. -----
```

### Comparing `udio_wrapper-0.0.2/setup.py` & `udio_wrapper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='udio_wrapper',
-    version='0.0.2',
+    version='0.0.3',
     author='Flowese',
     author_email='flowese@gmail.com',
     description='Generates songs using the Udio API using textual prompts.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/flowese/UdioWrapper',
     packages=find_packages(),
```

### Comparing `udio_wrapper-0.0.2/udio_wrapper.egg-info/PKG-INFO` & `udio_wrapper-0.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: udio_wrapper
-Version: 0.0.2
-Summary: Generates songs using the Udio API using textual prompts.
-Home-page: https://github.com/flowese/UdioWrapper
-Author: Flowese
-Author-email: flowese@gmail.com
-Keywords: audio,music,generation,API,AI,Udio
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests==2.31.0
-
 
 # Udio Wrapper
 
 ![Udio Wrapper](banner.jpeg)
 
 Written by @Flowese
 
@@ -46,14 +30,20 @@
 
 To install the package from PyPI, run the following command:
 
 ```bash
 pip install udio_wrapper
 ```
 
+To upgrade the package from PyPI, run the following command:
+```bash
+pip install --upgrade --no-cache-dir udio_wrapper
+```
+
+
 ### From GitHub Repository
 
 To install the package directly from the GitHub repository, run:
 
 ```bash
 pip install git+https://github.com/flowese/UdioWrapper.git
 ```
@@ -76,106 +66,96 @@
 
 To use `udio_wrapper`, import the `UdioWrapper` class and provide the necessary parameters.
 
 ## Usage Examples
 
 The following examples demonstrate various ways to use the `UdioWrapper` to generate music based on different scenarios:
 
-Generating a Complete Song with Automatically Generated Lyrics
 ```python
-from udio_wrapper import UdioWrapper
-
-udio = UdioWrapper(auth_token="your_auth_token_here")
-auto_song_url = udio.inference(
-    original_prompt="A song about the wonders of nature",
-    number_of_extensions=1,
-    extend_prompt="Keep singing about the beauty of the forest",
-    outro_prompt="Concluding with the serene sunset",
-    save_to_disk=True
-)
-print(f"URL of the complete song with automatic lyrics: {auto_song_url}")
-
+auth_token = "your-auth-token-here"  # Replace this with your actual authentication token
+udio_wrapper = UdioWrapper(auth_token)
 ```
 
-Generating a Complete Instrumental Song
+1. Creating a Short Song
+You can specify the prompt, seed, custom lyrics.
 ```python
-instrumental_song_url = udio.inference(
-    original_prompt="Smooth jazz instrumental music",
-    original_lyric_input="",
-    number_of_extensions=1,
-    extend_prompt="Continue the smooth jazz vibe",
-    extend_lyric_input="",
-    outro_prompt="Finish with a calming jazz outro",
-    outro_lyric_input="",
-    save_to_disk=True
-)
-print(f"URL of the complete instrumental song: {instrumental_song_url}")
 
+short_song_no_download = udio_wrapper.create_song(
+    prompt="Relaxing jazz and soulful music",
+    seed=-1,
+    custom_lyrics="Short song lyrics here"
+)
+print("Short song generated without downloading:", short_song_no_download)
 ```
-
-Generating a Complete Song with Custom Lyrics
+2. Extending a Song
+Extend a previously created song by providing its path and ID for conditioning. This method also allows for lyric customization.
 ```python
-custom_lyric_song_url = udio.inference(
-    original_prompt="A ballad about lost love",
-    original_lyric_input="Here under the moonlight, I remember your smile",
-    number_of_extensions=1,
-    extend_prompt="Continuing the tale of our summer love",
-    extend_lyric_input="Now all I have is the echo of your laughter",
-    outro_prompt="Ending our story as the leaves begin to fall",
-    outro_lyric_input="Farewell my love, until we meet again",
-    save_to_disk=True
-)
-print(f"URL of the complete song with custom lyrics: {custom_lyric_song_url}")
 
+extend_song_download = udio_wrapper.extend(
+    prompt="A dynamic version of relaxing jazz and soulful music",
+    seed=-1,
+    audio_conditioning_path="url-generated-song",
+    audio_conditioning_song_id="previous-song-id",
+    custom_lyrics="Extended version lyrics"
+)
+print("Extended song generated and downloaded:", extend_song_download)
 ```
 
-Generating a Simple Song with Custom Lyrics (No Extensions or Outro)
+3. Adding an Outro
+Generate an outro for your music sequence using the last song as a base. This includes custom lyrics.
 ```python
-simple_custom_lyric_song_url = udio.inference(
-    original_prompt="A pop song about bright city nights",
-    original_lyric_input="Neon lights and lonely hearts",
-    save_to_disk=True
-)
-print(f"URL of the simple song with custom lyrics: {simple_custom_lyric_song_url}")
 
+outro_song_download = udio_wrapper.add_outro(
+    prompt="A smooth ending to our jazz session",
+    seed=-1,
+    audio_conditioning_path="url-generated-song",
+    audio_conditioning_song_id="last-extended-song-id",
+    custom_lyrics="Outro lyrics here"
+)
+print("Outro song generated and downloaded:", outro_song_download)
 ```
 
-Generating a Simple Instrumental Song (No Extensions or Outro)
+4. Creating a Complete Song Sequence
+Generate a full sequence of songs, including multiple extensions and an outro. This process involves defining prompts and lyrics for each part of the sequence.
 ```python
-simple_instrumental_song_url = udio.inference(
-    original_prompt="Classical piano piece in minor key",
-    original_lyric_input="",
-    save_to_disk=True
+complete_song_sequence = udio_wrapper.create_complete_song(
+    short_prompt="On a full moon night",
+    extend_prompts=["the soft sound of the saxophone fills the air", "creating an atmosphere of mystery and romance"],
+    outro_prompt="Thus ends this melody, leaving an echo of emotions in the heart",
+    num_extensions=2,
+    custom_lyrics_short="Short song lyrics here",
+    custom_lyrics_extend=["Lyrics for first extension", "Lyrics for second extension"],
+    custom_lyrics_outro="Outro lyrics here"
 )
-print(f"URL of the simple instrumental song: {simple_instrumental_song_url}")
-
+print("Complete song sequence generated and downloaded:", complete_song_sequence)
 ```
 
-
 #### Parameters
 
-Each parameter in the `UdioWrapper` inference method has a specific purpose for creating customized music tracks:
-
 - **`auth_token`** *(Required)*: The authorization token you obtained from Udio, which is necessary for authenticating and making API requests.
 
-- **`original_prompt`** *(Required)*: The initial textual prompt that sets the thematic direction for generating the first track. This is the creative seed from which the song is grown.
 
-- **`original_lyric_input`** *(Optional)*: Specifies the lyrics for the initial track. If provided as an empty string (`""`), the resulting song will be purely instrumental. If omitted, Udio's API will automatically generate lyrics based on the `original_prompt`.
+Each method in the `UdioWrapper` class can take several parameters to control song generation and processing. Below is a breakdown of the parameters and their usage:
+
+- **prompt** *(str)*: A text prompt describing the theme or emotion of the song. This is the creative input from which the song generation is based.
+
+- **seed** *(int, optional)*: A seed number to ensure the reproducibility of the song generation. Using the same seed with the same parameters will generate the same audio output. Default is `-1`, which results in random generation each time.
+
+- **custom_lyrics** *(str, optional)*: Lyrics written by the user to be included in the song. If no lyrics are provided, the generation relies solely on the musical style implied by the prompt.
 
-- **`number_of_extensions`** *(Optional)*: The number of times the initial track should be extended. Each extension will be based on the last segment of the music generated in the previous step. The default value is 0, which means no extensions.
+- **audio_conditioning_path** *(str, optional)*: The file path to an audio file that will serve as a base or influence for the song being generated. This is used primarily for extending songs or generating outros based on a previous song.
 
-- **`extend_prompt`** *(Optional)*: The textual prompt for each extension phase. This prompt should ideally continue the theme or style set by the `original_prompt`.
+- **audio_conditioning_song_id** *(str, optional)*: The identifier of a previously generated song that will be used to influence the current song generation. This is necessary when creating extended songs or outros that are meant to follow a specific musical piece.
 
-- **`extend_lyric_input`** *(Optional)*: Custom lyrics for each extension phase. If this parameter is set to an empty string, the extension will be instrumental. If omitted, the API will automatically generate lyrics that attempt to continue the thematic content of the song.
+- **num_extensions** *(int, optional)*: Specifies the number of extended songs to generate in a sequence. This parameter is only used in the method that generates a complete song sequence. Default is `1`.
 
-- **`outro_prompt`** *(Optional)*: The textual prompt for the outro of the song, providing a thematic and musical conclusion.
+- **extend_prompts** *(list of str, optional)*: A list of prompts for generating each extension in a sequence. Each prompt should ideally reflect a progression or variation in style or theme from the previous song.
 
-- **`outro_lyric_input`** *(Optional)*: Custom lyrics for the outro. If provided as an empty string, the outro will be instrumental. If omitted, the API will generate lyrics that cap off the song's narrative.
+- **outro_prompt** *(str, optional)*: A prompt specifically for generating an outro. This should convey a sense of conclusion or finale relative to the musical sequence.
 
-- **`save_to_disk`** *(Optional)*: A boolean indicating whether to save the generated tracks to the disk. The default is `True`, which means the tracks will be saved.
 
 These parameters allow full customization of the music generation process, from the initial creation through extensions to the final outro, giving users the ability to tailor both the music and lyrics to fit their specific needs or artistic vision.
 
 
 ## License
 
 This project is licensed under the MIT License.
```

#### html2text {}

```diff
@@ -1,93 +1,90 @@
-Metadata-Version: 2.1 Name: udio_wrapper Version: 0.0.2 Summary: Generates
-songs using the Udio API using textual prompts. Home-page: https://github.com/
-flowese/UdioWrapper Author: Flowese Author-email: flowese@gmail.com Keywords:
-audio,music,generation,API,AI,Udio Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: requests==2.31.0 # Udio Wrapper !
-[Udio Wrapper](banner.jpeg) Written by @Flowese _[_O_p_e_n_ _D_e_m_o_ _I_n_ _C_o_l_a_b_]##
-Description `udio_wrapper` is a Python package that allows you to generate
-music tracks from Udio's API using textual prompts. This package is designed to
-interact with Udio's API and is not officially endorsed by Udio. ## Advantages
-Over Other Models Unlike other music generation models, Udio offers a unique
-feature of extending or conditioning new tracks based on existing ones, making
-it ideal for iterative and creative music production processes. ## Legal
-Disclaimer This package is created for educational and research purposes. By
-using this package, you agree to do so at your own risk. This package is not
+# Udio Wrapper ![Udio Wrapper](banner.jpeg) Written by @Flowese _[_O_p_e_n_ _D_e_m_o_ _I_n
+_C_o_l_a_b_]## Description `udio_wrapper` is a Python package that allows you to
+generate music tracks from Udio's API using textual prompts. This package is
+designed to interact with Udio's API and is not officially endorsed by Udio. ##
+Advantages Over Other Models Unlike other music generation models, Udio offers
+a unique feature of extending or conditioning new tracks based on existing
+ones, making it ideal for iterative and creative music production processes. ##
+Legal Disclaimer This package is created for educational and research purposes.
+By using this package, you agree to do so at your own risk. This package is not
 affiliated, endorsed, or sponsored by Udio in any way. ## Requirements - Python
 3.x - pip ## Installation ### From PyPI To install the package from PyPI, run
-the following command: ```bash pip install udio_wrapper ``` ### From GitHub
-Repository To install the package directly from the GitHub repository, run:
-```bash pip install git+https://github.com/flowese/UdioWrapper.git ``` ##
-Configuration ### Obtaining the Authorization Token 1. Sign up at [Udio](https:
-//www.udio.com/). 2. Once registered, open your browser's inspector: - In
-Chrome: `Ctrl+Shift+I` or `F12` on Windows, `Cmd+Option+I` on Mac. 3. Go to the
-`Application` tab. 4. On the left panel, locate and click on `Cookies`, then
-select the Ideogram website. 5. Find the cookie named `sb-api-auth-token`. 6.
-Click on `sb-api-auth-token` and copy the value in the `Value` field. ![Udio
-Wrapper](screen_cookies.jpeg) ### Usage To use `udio_wrapper`, import the
-`UdioWrapper` class and provide the necessary parameters. ## Usage Examples The
-following examples demonstrate various ways to use the `UdioWrapper` to
-generate music based on different scenarios: Generating a Complete Song with
-Automatically Generated Lyrics ```python from udio_wrapper import UdioWrapper
-udio = UdioWrapper(auth_token="your_auth_token_here") auto_song_url =
-udio.inference( original_prompt="A song about the wonders of nature",
-number_of_extensions=1, extend_prompt="Keep singing about the beauty of the
-forest", outro_prompt="Concluding with the serene sunset", save_to_disk=True )
-print(f"URL of the complete song with automatic lyrics: {auto_song_url}") ```
-Generating a Complete Instrumental Song ```python instrumental_song_url =
-udio.inference( original_prompt="Smooth jazz instrumental music",
-original_lyric_input="", number_of_extensions=1, extend_prompt="Continue the
-smooth jazz vibe", extend_lyric_input="", outro_prompt="Finish with a calming
-jazz outro", outro_lyric_input="", save_to_disk=True ) print(f"URL of the
-complete instrumental song: {instrumental_song_url}") ``` Generating a Complete
-Song with Custom Lyrics ```python custom_lyric_song_url = udio.inference
-( original_prompt="A ballad about lost love", original_lyric_input="Here under
-the moonlight, I remember your smile", number_of_extensions=1,
-extend_prompt="Continuing the tale of our summer love", extend_lyric_input="Now
-all I have is the echo of your laughter", outro_prompt="Ending our story as the
-leaves begin to fall", outro_lyric_input="Farewell my love, until we meet
-again", save_to_disk=True ) print(f"URL of the complete song with custom
-lyrics: {custom_lyric_song_url}") ``` Generating a Simple Song with Custom
-Lyrics (No Extensions or Outro) ```python simple_custom_lyric_song_url =
-udio.inference( original_prompt="A pop song about bright city nights",
-original_lyric_input="Neon lights and lonely hearts", save_to_disk=True ) print
-(f"URL of the simple song with custom lyrics: {simple_custom_lyric_song_url}")
-``` Generating a Simple Instrumental Song (No Extensions or Outro) ```python
-simple_instrumental_song_url = udio.inference( original_prompt="Classical piano
-piece in minor key", original_lyric_input="", save_to_disk=True ) print(f"URL
-of the simple instrumental song: {simple_instrumental_song_url}") ``` ####
-Parameters Each parameter in the `UdioWrapper` inference method has a specific
-purpose for creating customized music tracks: - **`auth_token`** *(Required)*:
-The authorization token you obtained from Udio, which is necessary for
-authenticating and making API requests. - **`original_prompt`** *(Required)*:
-The initial textual prompt that sets the thematic direction for generating the
-first track. This is the creative seed from which the song is grown. -
-**`original_lyric_input`** *(Optional)*: Specifies the lyrics for the initial
-track. If provided as an empty string (`""`), the resulting song will be purely
-instrumental. If omitted, Udio's API will automatically generate lyrics based
-on the `original_prompt`. - **`number_of_extensions`** *(Optional)*: The number
-of times the initial track should be extended. Each extension will be based on
-the last segment of the music generated in the previous step. The default value
-is 0, which means no extensions. - **`extend_prompt`** *(Optional)*: The
-textual prompt for each extension phase. This prompt should ideally continue
-the theme or style set by the `original_prompt`. - **`extend_lyric_input`** *
-(Optional)*: Custom lyrics for each extension phase. If this parameter is set
-to an empty string, the extension will be instrumental. If omitted, the API
-will automatically generate lyrics that attempt to continue the thematic
-content of the song. - **`outro_prompt`** *(Optional)*: The textual prompt for
-the outro of the song, providing a thematic and musical conclusion. -
-**`outro_lyric_input`** *(Optional)*: Custom lyrics for the outro. If provided
-as an empty string, the outro will be instrumental. If omitted, the API will
-generate lyrics that cap off the song's narrative. - **`save_to_disk`** *
-(Optional)*: A boolean indicating whether to save the generated tracks to the
-disk. The default is `True`, which means the tracks will be saved. These
-parameters allow full customization of the music generation process, from the
-initial creation through extensions to the final outro, giving users the
-ability to tailor both the music and lyrics to fit their specific needs or
-artistic vision. ## License This project is licensed under the MIT License. ##
-Contributing If you'd like to contribute to this project, feel free to fork the
-repository and send a pull request, or open an issue to discuss what you'd like
-to change. All contributions are welcome! ## TODO ### Pending Tasks and
-Features - Improve error handling and response validation. - Implement a user-
-friendly web interface for easier interaction with the API. -----
+the following command: ```bash pip install udio_wrapper ``` To upgrade the
+package from PyPI, run the following command: ```bash pip install --upgrade --
+no-cache-dir udio_wrapper ``` ### From GitHub Repository To install the package
+directly from the GitHub repository, run: ```bash pip install git+https://
+github.com/flowese/UdioWrapper.git ``` ## Configuration ### Obtaining the
+Authorization Token 1. Sign up at [Udio](https://www.udio.com/). 2. Once
+registered, open your browser's inspector: - In Chrome: `Ctrl+Shift+I` or `F12`
+on Windows, `Cmd+Option+I` on Mac. 3. Go to the `Application` tab. 4. On the
+left panel, locate and click on `Cookies`, then select the Ideogram website. 5.
+Find the cookie named `sb-api-auth-token`. 6. Click on `sb-api-auth-token` and
+copy the value in the `Value` field. ![Udio Wrapper](screen_cookies.jpeg) ###
+Usage To use `udio_wrapper`, import the `UdioWrapper` class and provide the
+necessary parameters. ## Usage Examples The following examples demonstrate
+various ways to use the `UdioWrapper` to generate music based on different
+scenarios: ```python auth_token = "your-auth-token-here" # Replace this with
+your actual authentication token udio_wrapper = UdioWrapper(auth_token) ``` 1.
+Creating a Short Song You can specify the prompt, seed, custom lyrics.
+```python short_song_no_download = udio_wrapper.create_song( prompt="Relaxing
+jazz and soulful music", seed=-1, custom_lyrics="Short song lyrics here" )
+print("Short song generated without downloading:", short_song_no_download) ```
+2. Extending a Song Extend a previously created song by providing its path and
+ID for conditioning. This method also allows for lyric customization. ```python
+extend_song_download = udio_wrapper.extend( prompt="A dynamic version of
+relaxing jazz and soulful music", seed=-1, audio_conditioning_path="url-
+generated-song", audio_conditioning_song_id="previous-song-id",
+custom_lyrics="Extended version lyrics" ) print("Extended song generated and
+downloaded:", extend_song_download) ``` 3. Adding an Outro Generate an outro
+for your music sequence using the last song as a base. This includes custom
+lyrics. ```python outro_song_download = udio_wrapper.add_outro( prompt="A
+smooth ending to our jazz session", seed=-1, audio_conditioning_path="url-
+generated-song", audio_conditioning_song_id="last-extended-song-id",
+custom_lyrics="Outro lyrics here" ) print("Outro song generated and downloaded:
+", outro_song_download) ``` 4. Creating a Complete Song Sequence Generate a
+full sequence of songs, including multiple extensions and an outro. This
+process involves defining prompts and lyrics for each part of the sequence.
+```python complete_song_sequence = udio_wrapper.create_complete_song
+( short_prompt="On a full moon night", extend_prompts=["the soft sound of the
+saxophone fills the air", "creating an atmosphere of mystery and romance"],
+outro_prompt="Thus ends this melody, leaving an echo of emotions in the heart",
+num_extensions=2, custom_lyrics_short="Short song lyrics here",
+custom_lyrics_extend=["Lyrics for first extension", "Lyrics for second
+extension"], custom_lyrics_outro="Outro lyrics here" ) print("Complete song
+sequence generated and downloaded:", complete_song_sequence) ``` ####
+Parameters - **`auth_token`** *(Required)*: The authorization token you
+obtained from Udio, which is necessary for authenticating and making API
+requests. Each method in the `UdioWrapper` class can take several parameters to
+control song generation and processing. Below is a breakdown of the parameters
+and their usage: - **prompt** *(str)*: A text prompt describing the theme or
+emotion of the song. This is the creative input from which the song generation
+is based. - **seed** *(int, optional)*: A seed number to ensure the
+reproducibility of the song generation. Using the same seed with the same
+parameters will generate the same audio output. Default is `-1`, which results
+in random generation each time. - **custom_lyrics** *(str, optional)*: Lyrics
+written by the user to be included in the song. If no lyrics are provided, the
+generation relies solely on the musical style implied by the prompt. -
+**audio_conditioning_path** *(str, optional)*: The file path to an audio file
+that will serve as a base or influence for the song being generated. This is
+used primarily for extending songs or generating outros based on a previous
+song. - **audio_conditioning_song_id** *(str, optional)*: The identifier of a
+previously generated song that will be used to influence the current song
+generation. This is necessary when creating extended songs or outros that are
+meant to follow a specific musical piece. - **num_extensions** *(int,
+optional)*: Specifies the number of extended songs to generate in a sequence.
+This parameter is only used in the method that generates a complete song
+sequence. Default is `1`. - **extend_prompts** *(list of str, optional)*: A
+list of prompts for generating each extension in a sequence. Each prompt should
+ideally reflect a progression or variation in style or theme from the previous
+song. - **outro_prompt** *(str, optional)*: A prompt specifically for
+generating an outro. This should convey a sense of conclusion or finale
+relative to the musical sequence. These parameters allow full customization of
+the music generation process, from the initial creation through extensions to
+the final outro, giving users the ability to tailor both the music and lyrics
+to fit their specific needs or artistic vision. ## License This project is
+licensed under the MIT License. ## Contributing If you'd like to contribute to
+this project, feel free to fork the repository and send a pull request, or open
+an issue to discuss what you'd like to change. All contributions are welcome!
+## TODO ### Pending Tasks and Features - Improve error handling and response
+validation. - Implement a user-friendly web interface for easier interaction
+with the API. -----
```

