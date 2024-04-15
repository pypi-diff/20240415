# Comparing `tmp/codeframe-0.5.3.tar.gz` & `tmp/codeframe-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeframe-0.5.3.tar", last modified: Thu Mar 21 09:32:25 2024, max compression
+gzip compressed data, was "codeframe-0.5.4.tar", last modified: Mon Apr 15 08:56:30 2024, max compression
```

## Comparing `codeframe-0.5.3.tar` & `codeframe-0.5.4.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.340504 codeframe-0.5.3/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-03-21 09:32:25.340504 codeframe-0.5.3/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2025 2024-03-21 09:32:21.000000 codeframe-0.5.3/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.336504 codeframe-0.5.3/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    10064 2024-03-21 09:32:23.000000 codeframe-0.5.3/bin/codeframe
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.336504 codeframe-0.5.3/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-01-17 17:42:18.000000 codeframe-0.5.3/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6895 2024-03-20 08:17:13.000000 codeframe-0.5.3/codeframe/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.340504 codeframe-0.5.3/codeframe/data/
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.340504 codeframe-0.5.3/codeframe/data/installation_files/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      461 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/.bumpversion.cfg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       83 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/.gitignore
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1845 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/README.org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-03-19 15:01:37.000000 codeframe-0.5.3/codeframe/data/installation_files/__init__.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.340504 codeframe-0.5.3/codeframe/data/installation_files/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9911 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/bin/codeframe
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    10064 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/bin_codeframe.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.340504 codeframe-0.5.3/codeframe/data/installation_files/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3944 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/distcheck.sh
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      291 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/requirements.txt
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-03-21 09:32:17.000000 codeframe-0.5.3/codeframe/data/installation_files/setup.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2024-03-19 14:47:38.000000 codeframe-0.5.3/codeframe/data/testing
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4075 2024-03-20 08:16:36.000000 codeframe-0.5.3/codeframe/df_table.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9251 2024-03-21 09:08:32.000000 codeframe-0.5.3/codeframe/installation.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4325 2024-03-21 09:31:22.000000 codeframe-0.5.3/codeframe/interpreter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8610 2024-03-19 13:03:28.000000 codeframe-0.5.3/codeframe/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4971 2024-03-19 13:03:28.000000 codeframe-0.5.3/codeframe/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2897 2024-01-23 13:00:22.000000 codeframe-0.5.3/codeframe/topbar.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-03-21 09:32:24.000000 codeframe-0.5.3/codeframe/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-21 09:32:25.340504 codeframe-0.5.3/codeframe.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-03-21 09:32:25.000000 codeframe-0.5.3/codeframe.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      945 2024-03-21 09:32:25.000000 codeframe-0.5.3/codeframe.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-03-21 09:32:25.000000 codeframe-0.5.3/codeframe.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       76 2024-03-21 09:32:25.000000 codeframe-0.5.3/codeframe.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2024-03-21 09:32:25.000000 codeframe-0.5.3/codeframe.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-03-21 09:32:25.340504 codeframe-0.5.3/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-03-19 15:48:21.000000 codeframe-0.5.3/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.485666 codeframe-0.5.4/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 08:56:30.485666 codeframe-0.5.4/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2025 2024-04-15 08:56:24.000000 codeframe-0.5.4/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.481665 codeframe-0.5.4/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 08:56:26.000000 codeframe-0.5.4/bin/codeframe
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.481665 codeframe-0.5.4/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-01-17 17:42:18.000000 codeframe-0.5.4/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    10240 2024-04-09 08:16:32.000000 codeframe-0.5.4/codeframe/cmd_parser.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6895 2024-03-20 08:17:13.000000 codeframe-0.5.4/codeframe/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.481665 codeframe-0.5.4/codeframe/data/
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.485666 codeframe-0.5.4/codeframe/data/installation_files/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      461 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/.bumpversion.cfg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       83 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/.gitignore
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1845 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/README.org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-03-19 15:01:37.000000 codeframe-0.5.4/codeframe/data/installation_files/__init__.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.485666 codeframe-0.5.4/codeframe/data/installation_files/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    10064 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/bin/codeframe
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/bin_codeframe.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.485666 codeframe-0.5.4/codeframe/data/installation_files/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3944 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/distcheck.sh
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      291 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/requirements.txt
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-04-15 08:56:20.000000 codeframe-0.5.4/codeframe/data/installation_files/setup.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2024-03-19 14:47:38.000000 codeframe-0.5.4/codeframe/data/testing
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4075 2024-03-20 08:16:36.000000 codeframe-0.5.4/codeframe/df_table.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      633 2024-04-09 08:07:38.000000 codeframe-0.5.4/codeframe/fn_load.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9251 2024-03-21 09:08:32.000000 codeframe-0.5.4/codeframe/installation.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9460 2024-04-08 14:32:43.000000 codeframe-0.5.4/codeframe/interpreter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8898 2024-04-15 08:51:16.000000 codeframe-0.5.4/codeframe/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5127 2024-04-03 05:16:15.000000 codeframe-0.5.4/codeframe/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2897 2024-01-23 13:00:22.000000 codeframe-0.5.4/codeframe/topbar.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-15 08:56:29.000000 codeframe-0.5.4/codeframe/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 08:56:30.485666 codeframe-0.5.4/codeframe.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 08:56:30.000000 codeframe-0.5.4/codeframe.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      990 2024-04-15 08:56:30.000000 codeframe-0.5.4/codeframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-15 08:56:30.000000 codeframe-0.5.4/codeframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       76 2024-04-15 08:56:30.000000 codeframe-0.5.4/codeframe.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2024-04-15 08:56:30.000000 codeframe-0.5.4/codeframe.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-15 08:56:30.485666 codeframe-0.5.4/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-03-19 15:48:21.000000 codeframe-0.5.4/setup.py
```

### Comparing `codeframe-0.5.3/PKG-INFO` & `codeframe-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.5.3
+Version: 0.5.4
 Summary: Automatically created environment for python package
 Home-page: https://gitlab.com/jaromrax/codeframe
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `codeframe-0.5.3/README.md` & `codeframe-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/bin/codeframe` & `codeframe-0.5.4/codeframe/data/installation_files/bin/codeframe`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe/config.py` & `codeframe-0.5.4/codeframe/config.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe/data/installation_files/README.org` & `codeframe-0.5.4/codeframe/data/installation_files/README.org`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe/data/installation_files/bin/codeframe` & `codeframe-0.5.4/bin/codeframe`

 * *Files 12% similar despite different names*

```diff
@@ -31,19 +31,22 @@
 from pyfiglet import Figlet
 import signal
 
 # ====================== for separate terminal keyboard using mmap
 
 from prompt_toolkit import PromptSession, prompt
 from prompt_toolkit.history import FileHistory
+
 from prompt_toolkit.completion import WordCompleter
+from prompt_toolkit.completion import NestedCompleter
+
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 
 # ========================
-SHOW_LOGO_TABLE = False
+SHOW_LOGO_TABLE = True
 SHOW_TIME = True
 SHOW_COMMAND_LINE = True
 RUN_MMAP_INPUT = True  #  INTERACTIVE MMAP-INTERACTIVE
 RUN_SELECT_FROM_TABLE = False
 
 termsize = os.get_terminal_size().columns
 
@@ -97,26 +100,26 @@
         print("i... RESET TERMINAL")
         os.system("reset")
         #terminal.clear()
         termsize = termsize2
         move_cursor(3, 1)
         #print("X")
 
-def main(projectname=None, debug=False, keyboard_remote_start = False, interactive = False):
+def main(projectname=None, debug=False, keyboard_remote_start = False, servermode = False):
     """
     Main function of the project. When 'projectname' given: new project is created
 
     Parameters:
     projectname: THIS WILL GENERATE NEW PROJECT with these modules
     keyboard_remote_start: just start a standalone prompt
-    interactive: keyboard input is taken in the main terminal window
+    servermode: wait for commands via mmap... to be used with -k
     """
     global RUN_SELECT_FROM_TABLE, SHOW_LOGO_TABLE, SHOW_TIME, RUN_MMAP_INPUT
 
-    if interactive: RUN_MMAP_INPUT = False
+    if not servermode: RUN_MMAP_INPUT = False
     # GLobal clear terminal
     if debug:
         print(__version__)
     #else:
 
     signal.signal(signal.SIGWINCH, handle_sigwinch)
 
@@ -126,18 +129,22 @@
     config.CONFIG["history"] = "~/.config/codeframe/history"
     # solely LOAD will create ....from_memory files
     # config.load_config()
     # solely  SAVE will create cfg.json only
     # config.save_config()
 
     # ==================================================== #########################
-    # ==================================================== ######################### standalone
+    # ==================================================== ######################### remote
     # ==================================================== #########################
+    #               command prompt - separate thread
+    # ==============================================================================
     if keyboard_remote_start:
-        prompt_completer = WordCompleter( interpreter.KNOWN_COMMANDS )
+        #prompt_completer = WordCompleter( interpreter.KNOWN_COMMANDS )
+        prompt_completer = NestedCompleter.from_nested_dict( interpreter.KNOWN_COMMANDS_DICT )
+
         multilineinput = False
         config.myPromptSession = PromptSession(
             history=FileHistory( os.path.expanduser(config.CONFIG["history"]) )
         ) #, multiline=Trueinp
         inp = ""
         myname = os.path.splitext(os.path.basename(__file__))[0]
 
@@ -153,19 +160,44 @@
                                                 )
             if inp==".h":
                 print("H...  HELP:")
                 print("H...  .t   table+logo")
                 print("H...  .d   disable logo and time")
                 print("H...  .r   reset terminal")
                 print("H... known commands: ", "  ".join(interpreter.KNOWN_COMMANDS )  )
+            elif inp==".q":
+                mmapwr.mmwrite(inp)
             else:
+                # print(f" >>>Write {inp} to the")
                 mmapwr.mmwrite(inp)
+                done = False
+                ii = 1
+                while not done:
+                    # res = mmapwr.mmread(  ) # read response
+                    ii+=1
+                    res = mmapwr.mmread_n_clear( mmapwr.MMAPRESP  )
+                    res = res.strip() # strin newline
+                    if ii%2==0:
+                        print("w", end="\r", flush=True)
+                    else:
+                        print("W", end="\r", flush=True)
+                    #print(f"... input was /{inp}/==/{res}/..result of read   len(inp):", len(inp), "  ...res:",len(res) )
+                    if res.strip()==inp.strip():
+                        #print(f" YES::::.../{inp}/==/{res}/.. ?")
+                        done = True
+                    #else:
+                    #    print(f" NONO:::.../{inp}/==/{res}/.. ?")
+                    time.sleep(0.25)
+                #print("... konec prikazu")
+
+
         # print(inp)
         return
     # ==================================================== #########################
+    #           command prompt - separate thread
     # ==================================================== #########################
     # ==================================================== #########################
 
 
     if projectname is None:
         print()
     elif projectname == "usage":
@@ -177,14 +209,16 @@
         sys.exit(0)
     # ----------------------- installation with this name ----------
     else:
         installation.main(projectname)
         sys.exit(0)
 
     # ===================== top bar and commads from kdb ==========
+    os.system("reset")
+    # when I put reset later, it occludes the 1st red inpput command
     top = topbar.Topbar(bgcolor=bg.blue)
     top2 = top.add(bgcolor=bg.black)
 
     top.print_to(
         10,
         f" {fg.white}{fx.bold}{dt.datetime.now().strftime('%H:%M:%S')}\
 {fx.default}{fg.default} ",
@@ -199,26 +233,27 @@
     a, b = (" ", " ")
 
     # KEYTHREAD THIS MUST BE HERE.....toi catch 1st letter
     #   only return         key, enter, abc = kthread.get_global_key()
     #                       key:mayreact on q;     enter==hit ; abc=>(a,b) for display.
     kthread = None
     if RUN_MMAP_INPUT:
+        # THis goes when mmap active
+        #print("i...   MMAP ACTIVE ...........................")
         kthread = key_enter.MmapSimulatedKeyboard(ending=".q")
     else:
+        #print("D...    MMAP NOT ACTIVE, using SSHKEYB.............")
         kthread = key_enter.KeyboardThreadSsh(ending=".q")
-    #
     # whatabout to have other terminal feeding mmapfile
     #
 
     df = create_dummy_df()
     terminal = Terminal()
     selection = None
     #terminal.clear()
-    os.system("reset")
     move_cursor(3, 1)
 #################################################################
     #          L O O P
     #################################################################
     while True:  # ================================= LOOP
 
         autoreset_terminal()
@@ -252,23 +287,27 @@
                     SHOW_LOGO_TABLE = not SHOW_LOGO_TABLE
                 elif cmd==".d":
                     SHOW_TIME = not SHOW_TIME
                 elif cmd==".r":
                     os.system("reset")
                     move_cursor(3,1)
                 else:
+                    print("...calling interpreter")
                     interpreter.main( cmd )
                 if RUN_SELECT_FROM_TABLE:
                     # list of row numbers from column 'n' :  assume whole word is list of rows:
                     if selection is not None and selection != "":
                         selection = ""
                     else:
                         selection = cmd
                 # ======================================================== INTERPRETER
             #print(f"----------- {cmd}; table_selection:{selection}--------------------- ***")
+            #print("...writeback try", key)
+            mmapwr.mmwrite( key , mmapwr.MMAPRESP)
+            #print("...writeback done",key)
         else:
             cmd = ""
 
         top.print_to(
             10,
             f" {fg.white}{fx.bold}{dt.datetime.now().strftime('%H:%M:%S')}\
 {fx.default}{fg.default}",
```

### Comparing `codeframe-0.5.3/codeframe/data/installation_files/bin_codeframe.py` & `codeframe-0.5.4/codeframe/data/installation_files/bin_codeframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.completion import NestedCompleter
 
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 
 # ========================
-SHOW_LOGO_TABLE = False
+SHOW_LOGO_TABLE = True
 SHOW_TIME = True
 SHOW_COMMAND_LINE = True
 RUN_MMAP_INPUT = True  #  INTERACTIVE MMAP-INTERACTIVE
 RUN_SELECT_FROM_TABLE = False
 
 termsize = os.get_terminal_size().columns
 
@@ -100,26 +100,26 @@
         print("i... RESET TERMINAL")
         os.system("reset")
         #terminal.clear()
         termsize = termsize2
         move_cursor(3, 1)
         #print("X")
 
-def main(projectname=None, debug=False, keyboard_remote_start = False, interactive = False):
+def main(projectname=None, debug=False, keyboard_remote_start = False, servermode = False):
     """
     Main function of the project. When 'projectname' given: new project is created
 
     Parameters:
     projectname: THIS WILL GENERATE NEW PROJECT with these modules
     keyboard_remote_start: just start a standalone prompt
-    interactive: keyboard input is taken in the main terminal window
+    servermode: wait for commands via mmap... to be used with -k
     """
     global RUN_SELECT_FROM_TABLE, SHOW_LOGO_TABLE, SHOW_TIME, RUN_MMAP_INPUT
 
-    if interactive: RUN_MMAP_INPUT = False
+    if not servermode: RUN_MMAP_INPUT = False
     # GLobal clear terminal
     if debug:
         print(__version__)
     #else:
 
     signal.signal(signal.SIGWINCH, handle_sigwinch)
 
@@ -129,16 +129,18 @@
     config.CONFIG["history"] = "~/.config/codeframe/history"
     # solely LOAD will create ....from_memory files
     # config.load_config()
     # solely  SAVE will create cfg.json only
     # config.save_config()
 
     # ==================================================== #########################
-    # ==================================================== ######################### standalone
+    # ==================================================== ######################### remote
     # ==================================================== #########################
+    #               command prompt - separate thread
+    # ==============================================================================
     if keyboard_remote_start:
         #prompt_completer = WordCompleter( interpreter.KNOWN_COMMANDS )
         prompt_completer = NestedCompleter.from_nested_dict( interpreter.KNOWN_COMMANDS_DICT )
 
         multilineinput = False
         config.myPromptSession = PromptSession(
             history=FileHistory( os.path.expanduser(config.CONFIG["history"]) )
@@ -158,19 +160,44 @@
                                                 )
             if inp==".h":
                 print("H...  HELP:")
                 print("H...  .t   table+logo")
                 print("H...  .d   disable logo and time")
                 print("H...  .r   reset terminal")
                 print("H... known commands: ", "  ".join(interpreter.KNOWN_COMMANDS )  )
+            elif inp==".q":
+                mmapwr.mmwrite(inp)
             else:
+                # print(f" >>>Write {inp} to the")
                 mmapwr.mmwrite(inp)
+                done = False
+                ii = 1
+                while not done:
+                    # res = mmapwr.mmread(  ) # read response
+                    ii+=1
+                    res = mmapwr.mmread_n_clear( mmapwr.MMAPRESP  )
+                    res = res.strip() # strin newline
+                    if ii%2==0:
+                        print("w", end="\r", flush=True)
+                    else:
+                        print("W", end="\r", flush=True)
+                    #print(f"... input was /{inp}/==/{res}/..result of read   len(inp):", len(inp), "  ...res:",len(res) )
+                    if res.strip()==inp.strip():
+                        #print(f" YES::::.../{inp}/==/{res}/.. ?")
+                        done = True
+                    #else:
+                    #    print(f" NONO:::.../{inp}/==/{res}/.. ?")
+                    time.sleep(0.25)
+                #print("... konec prikazu")
+
+
         # print(inp)
         return
     # ==================================================== #########################
+    #           command prompt - separate thread
     # ==================================================== #########################
     # ==================================================== #########################
 
 
     if projectname is None:
         print()
     elif projectname == "usage":
@@ -182,14 +209,16 @@
         sys.exit(0)
     # ----------------------- installation with this name ----------
     else:
         installation.main(projectname)
         sys.exit(0)
 
     # ===================== top bar and commads from kdb ==========
+    os.system("reset")
+    # when I put reset later, it occludes the 1st red inpput command
     top = topbar.Topbar(bgcolor=bg.blue)
     top2 = top.add(bgcolor=bg.black)
 
     top.print_to(
         10,
         f" {fg.white}{fx.bold}{dt.datetime.now().strftime('%H:%M:%S')}\
 {fx.default}{fg.default} ",
@@ -204,26 +233,27 @@
     a, b = (" ", " ")
 
     # KEYTHREAD THIS MUST BE HERE.....toi catch 1st letter
     #   only return         key, enter, abc = kthread.get_global_key()
     #                       key:mayreact on q;     enter==hit ; abc=>(a,b) for display.
     kthread = None
     if RUN_MMAP_INPUT:
+        # THis goes when mmap active
+        #print("i...   MMAP ACTIVE ...........................")
         kthread = key_enter.MmapSimulatedKeyboard(ending=".q")
     else:
+        #print("D...    MMAP NOT ACTIVE, using SSHKEYB.............")
         kthread = key_enter.KeyboardThreadSsh(ending=".q")
-    #
     # whatabout to have other terminal feeding mmapfile
     #
 
     df = create_dummy_df()
     terminal = Terminal()
     selection = None
     #terminal.clear()
-    os.system("reset")
     move_cursor(3, 1)
 #################################################################
     #          L O O P
     #################################################################
     while True:  # ================================= LOOP
 
         autoreset_terminal()
@@ -257,23 +287,27 @@
                     SHOW_LOGO_TABLE = not SHOW_LOGO_TABLE
                 elif cmd==".d":
                     SHOW_TIME = not SHOW_TIME
                 elif cmd==".r":
                     os.system("reset")
                     move_cursor(3,1)
                 else:
+                    print("...calling interpreter")
                     interpreter.main( cmd )
                 if RUN_SELECT_FROM_TABLE:
                     # list of row numbers from column 'n' :  assume whole word is list of rows:
                     if selection is not None and selection != "":
                         selection = ""
                     else:
                         selection = cmd
                 # ======================================================== INTERPRETER
             #print(f"----------- {cmd}; table_selection:{selection}--------------------- ***")
+            #print("...writeback try", key)
+            mmapwr.mmwrite( key , mmapwr.MMAPRESP)
+            #print("...writeback done",key)
         else:
             cmd = ""
 
         top.print_to(
             10,
             f" {fg.white}{fx.bold}{dt.datetime.now().strftime('%H:%M:%S')}\
 {fx.default}{fg.default}",
```

### Comparing `codeframe-0.5.3/codeframe/data/installation_files/distcheck.sh` & `codeframe-0.5.4/codeframe/data/installation_files/distcheck.sh`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe/data/installation_files/setup.py` & `codeframe-0.5.4/codeframe/data/installation_files/setup.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe/df_table.py` & `codeframe-0.5.4/codeframe/df_table.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe/installation.py` & `codeframe-0.5.4/codeframe/installation.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe/key_enter.py` & `codeframe-0.5.4/codeframe/key_enter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     global global_key
     a = global_key
     #global_key = ""
     return a
 
 # https://sshkeyboard.readthedocs.io/en/latest/reference.html#sshkeyboard.listen_keyboard_manual
 # https://github.com/ollipal/sshkeyboard
-
+#
+# MMAP VARIANT =============================================
+#
 class MmapSimulatedKeyboard(threading.Thread):
     def __init__(self,  name='mmap-input-thread', ending=None):
         '''
         Restart itself as thread
         '''
         self.block = False
         self.ending = ending
@@ -54,32 +56,38 @@
         '''
         global global_key
 
         self.t = threading.current_thread()
 
         while True:
             #print("!...  ........................keyboard listen START")
-            time.sleep(0.5)
+            time.sleep(.5)
             res = mmapwr.mmread_n_clear()
             #
+            # works here
+            #mmapwr.mmwrite(res, mmapwr.MMAPRESP)
+            #
             # earlier, tuple was sent.....
             #print("###", res, type(res) )
             if type(res)==tuple:
                 global_key=res[0]
             else:
                 global_key = res # maybe some operation is needed?
             #print("!...  ........................keyboard listen STOP")
             #print("D...",f"/{global_key}/")
             if global_key.strip() == self.ending:
                 #print("!...  ........................keyboard listen BREAK")
                 break
         #print("!...  ........................keyboard THREAD  ENDED")
 
 
-
+#
+#
+#   ======================= SSH KEYBOARD VARIANT ===============
+#
 class KeyboardThreadSsh(threading.Thread):
     def __init__(self,  name='keyboard-input-thread', ending=None):
         '''
         Restart itself as thread
         '''
         self.block = False
         self.ending = ending
@@ -273,15 +281,16 @@
                             delay_second_char=0.1,
                             delay_other_chars=0.1,
                             lower = False, # IT WAS DEFAULT
                             sequential=True) # syncio
             #print("!...  ........................keyboard listen STOP")
             #print("D...",f"/{global_key}/")
             if global_key.strip() == self.ending:
-                #print("!...  ........................keyboard listen BREAK")
+                print("D...  ........................keyboard listen got BREAK...")
+                time.sleep(0.7) # give time to main to exit
                 break
         #print("!...  ........................keyboard THREAD  ENDED")
 
 
 
 
 #--------https://stackoverflow.com/questions/2408560/python-nonblocking-console-input
```

### Comparing `codeframe-0.5.3/codeframe/mmapwr.py` & `codeframe-0.5.4/codeframe/mmapwr.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import mmap
 import time
 import sys
 
 
 MMAPFILE = os.path.expanduser("~/.config/codeframe/mmapfile")
+MMAPRESP = os.path.expanduser("~/.config/codeframe/mmapresponse")
 MMAPSIZE = 1000
 NULLCHAR = chr(127)
 # -------------------------------------------------------------------------
 
 def mmcreate(filename=MMAPFILE):
     # - to have different filenames on the same PC
     #PORT=config.CONFIG['netport']
@@ -63,27 +64,27 @@
     """
 TO DEBUG ONLY
     """
 
     #PORT=config.CONFIG['netport']
     #filename = f"{filename}{PORT}"
 
-    print(filename)
-    print(filename)
-    print(filename)
-    print(filename)
-    print(filename)
+    print("... MMREAD FROM",filename)
+    #print(filename)
+    #print(filename)
+    #print(filename)
+    #print(filename)
 #    with open(filename, mode="r", encoding="utf8") as file_obj:
 #        with mmap.mmap(file_obj.fileno(), length=0, access=mmap.ACCESS_READ) as mmap_obj:
 #            text = mmap_obj.read()
 #            print("READTEXT =",text)
 
     with open(filename, mode="r+", encoding="utf8") as file_obj:
         with mmap.mmap(file_obj.fileno(), length=0, access=mmap.ACCESS_WRITE, offset=0) as mmap_obj:
-            text = mmap_obj.read().decode("utf8").strip()
+            text = mmap_obj.read().decode("utf8").strip().strip(NULLCHAR)
             print(text)
             print(text)
             print(text)
             print(text)
             return text
 
 
@@ -103,31 +104,32 @@
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             print(f"! File Size == {file_size}, should be {MMAPSIZE}")
             os.remove( filename )
             #sys.exit(0)
-            mmcreate()
+            mmcreate( filename )
 
     if not os.path.exists(filename):
         print( f"xxxxxx ... {filename} not found... creating","1")
-        mmcreate()
+        mmcreate( filename)
         #return  "xxxxxx","1"
 
 
     with open(filename, mode="r+", encoding="utf8") as file_obj:
         with mmap.mmap(file_obj.fileno(), length=0, access=mmap.ACCESS_WRITE, offset=0) as mmap_obj:
             text = mmap_obj.read().decode("utf8").strip()
             # print("READTEXT: ",text)
 
 
             # execute(text.decode("utf8"))
             if text[0] == NULLCHAR:
                 response = ""#"xxxxxx","1"
+                #return response
             elif NULLCHAR in text:  # take everything before "*"
                 response = text.split(NULLCHAR)[0]
                 response = response+"\n" # BREAKING FLASHCAM SYSTEM
                 # if len(response.split())>1:
                 #     spl01 = response.split()[0].strip()
                 #     spl02 = " ".join(response.split()[1:])
                 #     spl02 = spl02.strip()
```

### Comparing `codeframe-0.5.3/codeframe/topbar.py` & `codeframe-0.5.4/codeframe/topbar.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.3/codeframe.egg-info/PKG-INFO` & `codeframe-0.5.4/codeframe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.5.3
+Version: 0.5.4
 Summary: Automatically created environment for python package
 Home-page: https://gitlab.com/jaromrax/codeframe
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `codeframe-0.5.3/codeframe.egg-info/SOURCES.txt` & `codeframe-0.5.4/codeframe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 README.md
 setup.py
 bin/codeframe
 codeframe/__init__.py
+codeframe/cmd_parser.py
 codeframe/config.py
 codeframe/df_table.py
+codeframe/fn_load.py
 codeframe/installation.py
 codeframe/interpreter.py
 codeframe/key_enter.py
 codeframe/mmapwr.py
 codeframe/topbar.py
 codeframe/version.py
 codeframe.egg-info/PKG-INFO
```

### Comparing `codeframe-0.5.3/setup.py` & `codeframe-0.5.4/setup.py`

 * *Files identical despite different names*

