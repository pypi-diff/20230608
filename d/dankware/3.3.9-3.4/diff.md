# Comparing `tmp/dankware-3.3.9.tar.gz` & `tmp/dankware-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.3.9.tar", last modified: Fri May 26 12:37:54 2023, max compression
+gzip compressed data, was "dankware-3.4.tar", last modified: Thu Jun  8 11:39:02 2023, max compression
```

## Comparing `dankware-3.3.9.tar` & `dankware-3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:37:54.516018 dankware-3.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 12:37:43.000000 dankware-3.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-26 12:37:54.516018 dankware-3.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-26 12:37:43.000000 dankware-3.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:37:54.512018 dankware-3.3.9/dankware/
--rw-r--r--   0 runner    (1001) docker     (123)    46356 2023-05-26 12:37:43.000000 dankware-3.3.9/dankware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:37:54.516018 dankware-3.3.9/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 12:37:54.000000 dankware-3.3.9/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:37:54.516018 dankware-3.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-26 12:37:43.000000 dankware-3.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:39:02.130062 dankware-3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 11:38:49.000000 dankware-3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16297 2023-06-08 11:39:02.130062 dankware-3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-06-08 11:38:49.000000 dankware-3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:39:02.130062 dankware-3.4/dankware/
+-rw-r--r--   0 runner    (1001) docker     (123)    46643 2023-06-08 11:38:49.000000 dankware-3.4/dankware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:39:02.130062 dankware-3.4/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16297 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 11:39:02.000000 dankware-3.4/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:39:02.130062 dankware-3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-08 11:38:49.000000 dankware-3.4/setup.py
```

### Comparing `dankware-3.3.9/LICENSE` & `dankware-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.3.9/dankware/__init__.py` & `dankware-3.4/dankware/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,43 @@
 import sys
 import time
 import random
 from datetime import datetime
 from colorama import Fore, Style
 
 # colorama colours
+reset = Style.RESET_ALL
 
 black = Fore.BLACK + Style.BRIGHT
 blue = Fore.BLUE + Style.BRIGHT
 cyan = Fore.CYAN + Style.BRIGHT
 green = Fore.GREEN + Style.BRIGHT
 magenta = Fore.MAGENTA + Style.BRIGHT
 red = Fore.RED + Style.BRIGHT
-reset = Style.RESET_ALL
 white = Fore.WHITE + Style.BRIGHT
 yellow = Fore.YELLOW + Style.BRIGHT
 
+black_normal = Fore.BLACK + Style.NORMAL
+blue_normal = Fore.BLUE + Style.NORMAL
+cyan_normal = Fore.CYAN + Style.NORMAL
+green_normal = Fore.GREEN + Style.NORMAL
+magenta_normal = Fore.MAGENTA + Style.NORMAL
+red_normal = Fore.RED + Style.NORMAL
+white_normal = Fore.WHITE + Style.NORMAL
+yellow_normal = Fore.YELLOW + Style.NORMAL
+
+black_dim = Fore.BLACK + Style.DIM
+blue_dim = Fore.BLUE + Style.DIM
+cyan_dim = Fore.CYAN + Style.DIM
+green_dim = Fore.GREEN + Style.DIM
+magenta_dim = Fore.MAGENTA + Style.DIM
+red_dim = Fore.RED + Style.DIM
+white_dim = Fore.WHITE + Style.DIM
+yellow_dim = Fore.YELLOW + Style.DIM
+
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def multithread(function: callable, threads: int = 1, *args, progress_bar: bool = True) -> None:
     
     """
     Run the given function in multiple threads with the specified inputs.
     
@@ -44,22 +62,22 @@
     
     from rich.live import Live
     from rich.panel import Panel
     from rich.table import Table
     from shutil import get_terminal_size
     from concurrent.futures import ThreadPoolExecutor, as_completed
     from rich.progress import Progress, SpinnerColumn, BarColumn, TextColumn, TimeRemainingColumn, TimeElapsedColumn
+    
+    def submit_task(executor, *args):
+            return executor.submit(function, *args)
 
     try:
         
-        def submit_task(executor, *args):
-            return executor.submit(function, *args)
-        
         if threads < 1:
-            raise ValueError("The number of threads must be a positive integer.")
+            raise ValueError("The number of threads must be a positive integer!")
 
         futures = []
         executor = ThreadPoolExecutor(max_workers=threads)
 
         if not args:
             for _ in range(threads): futures.append(executor.submit(function))
         else:
@@ -71,18 +89,18 @@
                     input_lists.append([arg] * threads)
 
             for task_args in zip(*input_lists):
                 futures.append(submit_task(executor, *task_args))
 
         if progress_bar:
             width = get_terminal_size().columns
-            job_progress = Progress("{task.description}", SpinnerColumn(), BarColumn(bar_width=width), TextColumn("[deep_pink1][progress.percentage][bright_cyan]{task.percentage:>3.0f}%"), "[bright_cyan]ETA", TimeRemainingColumn(), TimeElapsedColumn())
+            job_progress = Progress("{task.description}", SpinnerColumn(), BarColumn(bar_width=width), TextColumn("[progress.percentage][bright_green]{task.percentage:>3.0f}%"), "[bright_cyan]ETA", TimeRemainingColumn(), TimeElapsedColumn())
             overall_task = job_progress.add_task("[bright_green]Progress", total=int(len(futures)))
             progress_table = Table.grid()
-            progress_table.add_row(Panel.fit(job_progress, title="[bright_red]Jobs", border_style="magenta1", padding=(1, 2)))
+            progress_table.add_row(Panel.fit(job_progress, title="[bright_white]Jobs", border_style="bright_red", padding=(1, 2)))
 
             with Live(progress_table, refresh_per_second=10):
                 while not job_progress.finished:
                     time.sleep(0.1)
                     for future in as_completed(futures):
                         if future.done():
                             try: future.result()
@@ -184,22 +202,29 @@
     ]
     
     - Note: Only urls with filenames not containing "EXAMPLE" were returned.
     
     """
 
     urls = []
+
     for file_url in github_downloads(user_repo):
-        if filter_mode == "add": valid = False
-        elif filter_mode == "remove": valid = True
+
+        if filter_mode == "add":
+            valid = False
+        elif filter_mode == "remove":
+            valid = True
         for name in name_list:
             if name in file_url.split('/')[-1]:
-                if filter_mode == "add": valid = True
-                elif filter_mode == "remove": valid = False
+                if filter_mode == "add":
+                    valid = True
+                elif filter_mode == "remove":
+                    valid = False
         if valid: urls.append(file_url)
+
     return urls
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def random_ip() -> str:
     
     """
@@ -235,20 +260,20 @@
         
     return f"{first_octet}.{second_octet}.{third_octet}.{fourth_octet}"
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def is_admin() -> bool:
     
-    import ctypes
-    
     """
     Checks if the current user has admin privileges and returns True if found else False
     """
     
+    import ctypes
+
     try: return ctypes.windll.shell32.IsUserAnAdmin()
     except: return False
     
 '''
 def run_as_admin() -> None:
     
     """
@@ -293,15 +318,15 @@
             'HKEY_USERS': winreg.HKEY_USERS,
             'HKEY_CURRENT_CONFIG': winreg.HKEY_CURRENT_CONFIG,
         }
         
         if not export_path.endswith('.reg'):
             raise ValueError("Invalid Export Path! export_path must end with '.reg'")
         if registry_root not in key_map.keys():
-            raise ValueError(f"Invalid Registry Root! Use one of the following: {', '.join(key_map.keys())}")
+            raise ValueError(f"Invalid Registry Root: {registry_root} | Valid Roots: {', '.join(key_map.keys())}")
         if not is_admin():
             raise RuntimeError("Current user is not an administrator! Exporting registry keys requires admin privileges!")
             # If the current user is not an admin, relaunch the script with admin privileges
             #run_as_admin()
             
         def exporter(key, registry_root, subkey_path, key_data, recursive) -> None:
 
@@ -328,136 +353,149 @@
         if verbose:
             print(clr(f"\n  > Successfully exported registry keys to \"{os.path.join(os.getcwd(), 'export.reg') if export_path == 'export.reg' else export_path}\""))
     
     except: sys.exit(clr(err(sys.exc_info()),2))
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def clr(text: str, mode: int = 1, colour_one: str = white, colour_two: str = magenta) -> str:
+def clr(text: str, preset: int = 1, colour_one: str = white, colour_two: str = red, colours: list = []) -> str:
     
     """
     
-    this function colours special characters inside the 'chars' list
+    this function colours special characters inside the 'symbols' list
     
     ___________________________________________
     
-    - mode: 1 | to display general text (default)
+    - preset: 1 | to display general text (default)
     - text = white (default) / specified colour
-    - spl = magenta (default) / specified colour
+    - spl = red (default) / specified colour
 
     ___________________________________________
 
-    - mode: 2 | to display error messages
+    - preset: 2 | to display error messages
     - text = red (fixed colour)
     - spl = white (fixed colour)
 
     ___________________________________________
 
-    - mode: 3
+    - preset: 3
     - text = random (fixed colour)
     - spl = white (fixed colour)
 
     ___________________________________________
 
-    - mode: 4 | to display banners
-    - text & spl = random (fixed colour)
+    - preset: 4 | to display banners
+    - text & spl = random (default) / colours inside input list
     
     """
     
-    chars = ['[',']','>','<','.',',','=','-','_','?','!','|','(',')','{','}','/','\\',':','"',"'","%"]
+    symbols = ['[', ']', '!', '@', '#', '$', '%', '^', '&', '*', '(', ')', '_', '+', '-', '=', '{', '}', '|', '\\', ';', ':', "'", '"', ',', '.', '<', '>', '/', '?', '`', '~']
     
     words_green = ['true', 'True', 'TRUE', 'online', 'Online', 'ONLINE', 'successfully', 'Successfully', 'SUCCESSFULLY', 'successful', 'Successful', 'SUCCESSFUL', 'success', 'Success', 'SUCCESS']
     words_red = ['falsely', 'Falsely', 'FALSELY', 'false', 'False', 'FALSE', 'offline', 'Offline', 'OFFLINE', 'failures', 'Failures', 'FAILURES', 'failure', 'Failure', 'FAILURE', 'failed', 'Failed', 'FAILED', 'fail', 'Fail', 'FAIL']
     
     colours_to_replace = [Fore.BLACK, Fore.BLUE, Fore.CYAN, Fore.GREEN, Fore.MAGENTA, Fore.RED, Fore.WHITE, Fore.YELLOW, Style.BRIGHT, Style.RESET_ALL]
     colours_alt = ["BBLACKK", "BBLUEE", "CCYANN", "GGREENN", "MMAGENTAA", "RREDD", "WWHITEE", "YYELLOWW", "BBRIGHTT", "RRESETT"]
     
     bad_colours = ['BLACK', 'WHITE', 'LIGHTBLACK_EX', 'LIGHTWHITE_EX', 'RESET']
-    codes = vars(Fore); colours = [codes[colour] for colour in codes if colour not in bad_colours]
     styles = [Style.BRIGHT, Style.DIM, Style.NORMAL]
     
+    if colours == []:
+        codes = vars(Fore)
+        colours = [codes[colour] for colour in codes if colour not in bad_colours]
+    
     try:
-        if mode not in [3, 4]:
+        if preset not in [3, 4]:
             for _ in range(len(colours_to_replace)):
                 text = text.replace(colours_to_replace[_], colours_alt[_])
         else:
             for _ in range(len(colours_to_replace)):
                 text = text.replace(colours_to_replace[_], '')
 
         # default
 
-        if mode == 1:
-            #text = text.replace("[",f"{colour_two}[{colour_one}").replace("]",f"{colour_two}]{colour_one}")
-            for char in chars: text = text.replace(char, f"{colour_two}{char}{colour_one}")
+        if preset == 1:
+            for symbol in symbols:
+                text = text.replace(symbol, f"{colour_two}{symbol}{colour_one}")
             for word in words_green:
                 replacement = green.join(list(word))
                 text = text.replace(word, f"{green}{replacement}{colour_one}")
             for word in words_red:
                 replacement = red.join(list(word))
                 text = text.replace(word, f"{red}{replacement}{colour_one}")
         
         # for error messages
         
-        elif mode == 2:
-            #text = text.replace("[",f"{white}[{red}").replace("]",f"{white}]{red}")
-            for char in chars: text = text.replace(char, f"{white}{char}{red}")
+        elif preset == 2:
+            for symbol in symbols:
+                text = text.replace(symbol, f"{white}{symbol}{red}")
             for word in words_green:
                 replacement = green.join(list(word))
                 text = text.replace(word, f"{green}{replacement}{red}")
         
         # random | TRUE, FALSE will not be coloured!
         
-        elif mode in [3, 4]:
+        elif preset in [3, 4]:
 
-            text = [char for char in text]
+            text = [_ for _ in text]
             
-            if mode == 3: colour_spl = True
-            else: colour_spl = False
+            if preset == 3: colour_spl = True
+            elif preset == 4: colour_spl = False
     
             for _ in range(len(text)):
                 char = text[_]
                 if char != ' ' and char != '\n':
                     if colour_spl:
-                        if char in chars:
+                        if char in symbols:
                             text[_] = white + char
                         else:
                             text[_] = random.choice(colours) + Style.BRIGHT + char
                     else:
                         text[_] = random.choice(colours) + Style.BRIGHT + char
 
             text = ''.join(text)
 
-        else: raise ValueError(f"\n  {white}> {red}Invalid Mode {white}[{red}{mode}{white}] | Valid Modes{white}: {red}1{white},{red}2{white},{red}3{white},{red}4" + reset)
+        else: raise ValueError(f"Invalid Preset: {preset} | Valid Presets: 1, 2, 3, 4")
 
-        if mode not in [3, 4]:
+        if preset not in [3, 4]:
             for _ in range(len(colours_to_replace)):
                 text = text.replace(colours_alt[_], colours_to_replace[_])
 
-        if mode == 1: return colour_one + text + reset
-        elif mode == 2: return red + text + reset
-        elif mode == 3 or mode == 4: return text + reset
+        if preset == 1: return colour_one + text + reset
+        elif preset == 2: return red + text + reset
+        elif preset == 3 or preset == 4: return text + reset
     
     except: sys.exit(clr(err(sys.exc_info()),2))
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def align(text: str) -> str: 
     
     """
     center align banner / line ( supports both coloured and non-coloured )
     - [NOTE] align supports: clr, does not support: fade
     """
     
     from shutil import get_terminal_size
 
-    width = get_terminal_size().columns; aligned = text
-    for colour in vars(Fore).values(): aligned = aligned.replace(colour,'')
-    for style in vars(Style).values(): aligned = aligned.replace(style,'')
-    text = text.split('\n'); aligned = aligned.split('\n')
-    for _ in range(len(aligned)): aligned[_] = aligned[_].center(width).replace(aligned[_],text[_])
+    width = get_terminal_size().columns
+    aligned = text
+    
+    for colour in vars(Fore).values():
+        aligned = aligned.replace(colour,'')
+    
+    for style in vars(Style).values():
+        aligned = aligned.replace(style,'')
+    
+    text = text.split('\n')
+    aligned = aligned.split('\n')
+    
+    for _ in range(len(aligned)):
+        aligned[_] = aligned[_].center(width).replace(aligned[_],text[_])
+
     return str('\n'.join(aligned) + reset)
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def fade(text: str, colour: str = "purple") -> str:
     
     """
@@ -465,15 +503,15 @@
     - available_colours = black, red, green, cyan, blue, purple, random, black-v, red-v, green-v, cyan-v, blue-v, purple-v, pink-v
     """
     
     available_colours = ['black','red','green','cyan','blue','purple','random','black-v','red-v','green-v','cyan-v','blue-v','purple-v','pink-v']
 
     try:
         colour = colour.lower()
-        if not colour in available_colours: raise ValueError(clr(f"\n  > Invalid Colour: {colour} | Available Colours: {', '.join(available_colours)}",2))
+        if not colour in available_colours: raise ValueError(f"Invalid Colour: {colour} | Available Colours: {', '.join(available_colours)}")
             
         faded = ""
         if len(text.splitlines()) > 1: multi_line = True
         else: multi_line = False
 
         if colour == "black":
             for line in text.splitlines():
@@ -592,15 +630,15 @@
         elif colour == "random":
             for line in text.splitlines():
                 for char in line:
                     R, G, B = random.randint(0,255), random.randint(0,255), random.randint(0,255)
                     faded += f"\033[38;2;{R};{G};{B}m{char}\033[0m"
                 if multi_line: faded += "\n"
         
-        else: raise ValueError(clr(f"\n  > FADE ERROR! - [{colour}] is not supported yet!",2))
+        else: raise ValueError(f"Invalid Colour: {colour} | Available Colours: {', '.join(available_colours)}")
         
         if multi_line: faded = faded[:-1]
         return faded
 
     except: sys.exit(clr(err(sys.exc_info()),2))
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
@@ -829,15 +867,15 @@
         time.sleep(duration)
         show_window()
     
     ThreadPoolExecutor(10).submit(tmp)
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def file_selector(title: str = "Open", icon_path: str = "") -> str:
+def file_selector(title: str = "Select File", icon_path: str = "") -> str:
     
     """
     Opens file selector and returns selected file path
     - Allows custom title and icon
     """
     
     from tkinter import Tk
@@ -845,38 +883,61 @@
 
     root = Tk()
     root.withdraw()
     if icon_path: root.iconbitmap(icon_path)
     file_path = askopenfilename(title=title)
     return file_path.replace("/", "\\")
 
+def folder_selector(title: str = "Select Folder", icon_path: str = "") -> str:
+
+    """
+    Opens folder selector and returns selected folder path
+    - Allows custom title and icon
+    """
+
+    from tkinter import Tk
+    from tkinter.filedialog import askdirectory
+
+    root = Tk()
+    root.withdraw()
+    if icon_path:
+        root.iconbitmap(icon_path)
+    folder_path = askdirectory(title=title)
+    return folder_path.replace("/", "\\")
+
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def get_path(name: str) -> str:
+def get_path(location: str) -> str:
     
     """
     Returns path from registry
     - Supports: Desktop / Documents / Favorites / Pictures / Videos / Music
     """
     
-    import os
-    import winreg
+    try:
     
-    if name in ["Desktop", "Documents", "Favorites", "Pictures", "My Pictures", "Videos", "My Video", "Music", "My Music"]:
+        import os
+        import winreg
         
-        if name == "Documents": name = "Personal"
-        elif name == "Pictures": name = "My Pictures"
-        elif name == "Videos": name = "My Video"
-        elif name == "Music": name = "My Music"
-
-        key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders", access=winreg.KEY_READ)
-        path = os.path.expandvars(winreg.QueryValueEx(key, name)[0])
-        return path
-    
-    else: raise ValueError("Invalid name")
+        valid_locations = ["AppData", "Desktop", "Documents", "Personal", "Favorites", "Local AppData", "Pictures", "My Pictures", "Videos", "My Video", "Music", "My Music"]
+        
+        if location in valid_locations:
+            
+            if location == "Documents": location = "Personal"
+            elif location == "Pictures": location = "My Pictures"
+            elif location == "Videos": location = "My Video"
+            elif location == "Music": location = "My Music"
+
+            key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders", access=winreg.KEY_READ)
+            path = os.path.expandvars(winreg.QueryValueEx(key, location)[0])
+            return path
+        
+        else: raise ValueError(f"Invalid location: {location} | Valid locations: {', '.join(valid_locations)}")
+
+    except: sys.exit(clr(err(sys.exc_info()),2))
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def cls() -> None: 
     
     """
     Clear screen for multi-os
@@ -906,30 +967,14 @@
     
     from shutil import get_terminal_size
 
     print("\033[A" + " " * (get_terminal_size().columns - 6) + "\033[A")
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
-def chdir(mode: str) -> str:
-    
-    """
-    - running "os.chdir(os.path.dirname(__file__))" inside example.py will change its directory to the example.py file's location
-    - running "os.chdir(os.path.dirname(sys.argv[0]))" inside example.exe will change its directory to the example.exe file's location (nuitka)
-    - for changing directory to exe's path as exe: exec(chdir("exe"))
-    - for changing directory to script's path as script: exec(chdir("script"))
-    - [NOTE] When I build executables, the [ exec_mode = "script" ] is automatically replaced with [ exec_mode = "exe" ] inside the script
-    - [NOTE] If you run "os.chdir(os.path.dirname(__file__))" as an executable, it will change its directory to its temp folder [ C:\\Users\\user\\AppData\\Local\\Temp\\dankware_PPID ]
-    """
-
-    if mode == "script": return "os.chdir(os.path.dirname(__file__))" # as .py
-    elif mode == "exe": return "os.chdir(os.path.dirname(sys.argv[0]))" # as .exe
-
-# --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
 def sys_open(item: str) -> None:
     
     """
     Can do the following:
     - Open the url on the default browser on windows / linux
     - Open directory
     - Start file
```

### Comparing `dankware-3.3.9/setup.py` & `dankware-3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.3.9",
+    version = "3.4",
     author = "SirDank",
     
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
```

