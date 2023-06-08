# Comparing `tmp/consoleprint-1.2.5.tar.gz` & `tmp/consoleprint-1.2.7.tar.gz`

## Comparing `consoleprint-1.2.5.tar` & `consoleprint-1.2.7.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 consoleprint-1.2.5/him
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 consoleprint-1.2.5/qwe
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.5/src/ConsolePrint/__init__.py
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 consoleprint-1.2.5/src/ConsolePrint/animate.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.5/src/ConsolePrint/console2file.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.5/src/ConsolePrint/loading.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 consoleprint-1.2.5/tests/tests.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.5/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.5/LICENSE
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 consoleprint-1.2.5/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 consoleprint-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 consoleprint-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/__init__.py
+-rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/animate.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/console2file.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 consoleprint-1.2.7/src/ConsolePrint/loading.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 consoleprint-1.2.7/tests/tests.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 consoleprint-1.2.7/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 consoleprint-1.2.7/LICENSE
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 consoleprint-1.2.7/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 consoleprint-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 consoleprint-1.2.7/PKG-INFO
```

### Comparing `consoleprint-1.2.5/src/ConsolePrint/animate.py` & `consoleprint-1.2.7/src/ConsolePrint/animate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import os
 
-def ansify_color(color):  
+def ansify_color(color:str):  
     match color:
         #colours
         case 'default': color = '\033[0m'
         case 'grey': color = '\033[30m'
         case 'red': color = '\033[31m'
         case 'green': color = '\033[32m'
         case 'yellow': color = '\033[33m'
@@ -22,29 +22,27 @@
         case 'red_bg': color = '\033[41m'
         case 'green_bg': color = '\033[42m'
         case 'yellow_bg': color = '\033[43m'
         case 'blue_bg': color = '\033[44m'
         case 'magenta_bg': color = '\033[45m'
         case 'cyan_bg': color = '\033[46m'
         case 'white_bg': color = '\033[47m'
-    if '[' not in color or color[-1] != 'm' or not color[2:3].isdigit():
-        raise Exception("Invalid ANSI escape sequence for argument format")
+        case _:
+            if '[' not in color or color[-1] != 'm' or not color[2:3].isdigit():
+                raise Exception("Invalid ANSI escape sequence for argument format")
     return color
 
 
 if __name__ == "__main__":
     os.system('cls')
     print('\033[0m', end="\r")
-    print((terminal_size:=os.get_terminal_size()))
-    print(f'{terminal_size.columns = }, {terminal_size.lines = }')
-    print()
 
 terminal_width = os.get_terminal_size().columns
 
-def printing(text: str, delay=0.05, style='letter', stay=True, rev=False, format: str='default'):
+def printing(text:str, delay:float=0.05, style:str='letter', stay:bool=True, rev:bool=False, format:str='default'):
     """Prints text to console letter by letter or word by word"""
     format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     match rev:
         case False:
             if style.lower() == 'letter':
@@ -67,28 +65,28 @@
                     print(' '.join(text[-1 - _:]), end='\r')
                     time.sleep(delay)
     if stay:
         print()
     print('\033[0m', end='\r')
 
 
-def flashprint(text: str, blinks=5, delay=0.2, stay=True, format: str='default'):
+def flashprint(text:str, blinks:int=5, delay:float=0.2, stay:bool=True, format:str='default'):
     """Gets printed output to blink"""
     format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     for _ in range(blinks):
         print(text, end='\r'), time.sleep(delay)
         print(' ' * len(text), end='\r'), time.sleep(delay)
     if stay:
         print(text)
     print('\033[0m', end='\r')
 
 
-def flashtext(phrase: str, text: str, index='end', blinks=5, delay=0.2, format: str='default'):
+def flashtext(phrase:str, text:str, index='end', blinks:int=5, delay:float=0.2, format:str='default'):
     """Hilights key word by flashing it"""
     format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     phrase = phrase.strip()
     textb = ' ' * len(text)
     if index == 'end':
@@ -103,40 +101,46 @@
         time.sleep(delay)
         print(phrase1 + textb + phrase2, end='\r')
         time.sleep(delay)
     print(phrase1 + text + phrase2)
     print('\033[0m', end='\r')
 
 
-def animate1(text: str, symbol="#", format: str='default'):
+def animate1(text:str, symbol:str="#", format:str='default'):
     """Flashing masked text to transition to flasing text"""
+    if len(symbol) != 1:
+        raise Exception("Symbol input should be a single character")
     format = ansify_color(format)
-    print(format, end='\r')
     text = text.strip()
     symbol = len(text) * symbol
-    flashprint(symbol, blinks=3, stay=False)
-    flashprint(text, blinks=2, stay=True)
-    print('\033[0m', end='\r')
+    flashprint(symbol, blinks=3, stay=False, format=format)
+    flashprint(text, blinks=2, stay=True, format=format)
 
 
-def animate2(text: str, symbol="#", delay=0.05, format: str='default'):
+def animate2(text:str, symbol:str="#", delay:float=0.05, format:str='default'):
     """Reveals all characters text by text but first masked then flashes"""
+    if len(symbol) != 1:
+        raise Exception("Symbol input should be a single character")
     format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     symbol = len(text) * symbol
     for _ in symbol + "\r" + text + "\r":
         print(_, end="", flush=True)
         time.sleep(delay)
     flashprint(text, blinks=2, stay=True, format=format)
     print('\033[0m', end='\r')
 
-def text_box(text: str, symbol="#", padding: bool=False, wall: bool=True, align="center", format: str='default'):
+def text_box(text:str, symbol:str="#", spread:bool=False, padding:bool=False, wall:bool=True, align:str="center", format:str='default'):
     """Prints text in a box of symbols.
 If the align parameter is a number then the box is indented by the number count"""
+    if spread:
+        text = " ".join(list(text)).upper()
+    if len(symbol) != 1:
+        raise Exception("Symbol input should be a single character")
     format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     end = 5 if padding else 3
     text_row = 3 if padding else 2
     length = len(text) + 8
     left_border = text_row - 1  if padding else text_row
@@ -165,15 +169,17 @@
                     print("{:^{}}".format(text, length-2), end="")
             else:
                 print(" ", end="")  
             if col == length:
                 print('\033[0m')
                 
                 
-def star_square(num: int, symbol: str="#", align: str='center', flush: bool=True, format: str='default'):
+def star_square(num:int, symbol:str="#", align:str='center', flush:bool=True, format:str='default'):
+    if len(symbol) != 1:
+        raise Exception("Symbol input should be a single character")
     format = ansify_color(format)
     print(format, end='\r')
     if num < 5 or num > terminal_width or not isinstance(num, int):
         raise Exception(f"Invalid square size. Number must be an integer greater than 4 and less than the terminal width: {terminal_width}")
     elif align == 'center':
         indent = '\033[0m' + (' ' * (terminal_width//2 - num//2)) + format
     elif align == 'right':
@@ -182,15 +188,15 @@
         indent = ''  
     elif isinstance(align, int) and terminal_width - align > num:
         indent = '\033[0m' + (" " * align) + format
     else:
         raise Exception("Align parameter is invalid")    
           
     for row in range(1, num + 1):
-        # time.sleep(0.04)
+        time.sleep(0.04)
         print(indent, end="")
         for col in range(1, num + 1):
             if flush: time.sleep(0.04)                
             if row == 1 or col == 1 or row == num or col == num:
                 print(symbol, end="", flush=flush)
             elif row == col:
                 print(symbol, end="", flush=flush)
@@ -198,15 +204,15 @@
                 print(symbol, end="", flush=flush)  
             else:
                 print(" ", end="", flush=flush)              
             if col == num:
                 print('\033[0m')
     
 
-def asteriskify(text: str, align: str="left", underscore: bool=False, format: str='default'):
+def asteriskify(text:str, align:str="center", underscore:bool=True, format:str='default'):
     format = ansify_color(format)
     print(format, end='\r')
     text = text.strip()
     length = len(text)
     
     if align == 'center':
         indent = '\033[0m' + ' ' * (terminal_width//2 - length//2) + format
@@ -220,16 +226,16 @@
     if underscore:
         print(indent + '*' * length)
     print('\033[0m', end='\r')
     
 
 # Code test
 if __name__ == "__main__":
-    printing("hello this should print letter by letter      ", delay=0.05, style="letter", stay=True, rev=False, format='red_bg')
+    printing("hello this should print letter by letter ", delay=0.05, style="letter", stay=True, rev=False, format='red_bg')
     printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red')
     flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
     flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
-    animate1("This text is animated with #", symbol="#", format='white')
+    animate1("This text is animated with #", symbol="#", format='red')
     animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
-    text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
-    star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
+    text_box("boxed in", symbol="#", padding=False, wall=True, align='center', spread=True, format='\033[48;5;4m')
+    star_square(10, symbol="@", align=15, flush="True", format="strike")
     asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
```

### Comparing `consoleprint-1.2.5/src/ConsolePrint/console2file.py` & `consoleprint-1.2.7/src/ConsolePrint/console2file.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.5/src/ConsolePrint/loading.py` & `consoleprint-1.2.7/src/ConsolePrint/loading.py`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.5/tests/tests.py` & `consoleprint-1.2.7/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # animate.py
 import ConsolePrint.animate as prt
 
 prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
 prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
 prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
-prt.animate1("This text is animated with #", symbol="#", format='white')
+prt.animate1("This text is animated with #", symbol="#", format='strike')
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
 prt.star_square(10, symbol="@", align=15, flush="True", format="\033[104m")
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
 
 # console2file.pt
 import ConsolePrint.console2file as file
```

### Comparing `consoleprint-1.2.5/LICENSE` & `consoleprint-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleprint-1.2.5/README.md` & `consoleprint-1.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 # Installation
 You may install it form PyPI.org using the pip command.
 
 pip install ConsolePrint
 
 # Usage
 Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output on some terminals.
-
+```python
 import ConsolePrint.animate as prt    
 
 import ConsolePrint.console2file as file  
 
 import ConsolePrint.loading as load        
-
+```
 # Test Cases
 1.  Here uou may change the arguments as desired
-
+```python
 file.startConsoleSave()
 
 'Saves all output between the start and end functions to file.'
 
 from calendar import calendar
 
 print(calendar(2023))
 
 file.endConsoleSave()
-
+```
 2. Here you may use ANSI escape sequences for the format argument and change others as desired.
 Preset arguments for format:
 //colours
 'default':          '\033[0m'
 'grey':             '\033[30m'
 'red':              '\033[31m'
 'green':            '\033[32m'
@@ -53,14 +53,15 @@
 'green_bg':         '\033[42m'
 'yellow_bg':        '\033[43m'
 'blue_bg':          '\033[44m'
 'magenta_bg':       '\033[45m'
 'cyan_bg':          '\033[46m'
 'white_bg':         '\033[47m'
 
+```python
 prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
 
 prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
 
 prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
 
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
@@ -68,29 +69,30 @@
 prt.animate1("This text is animated with #", symbol="#", format='white')
 
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 
 prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
 
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
+```
 
 3.  Here, the load time is specified in seconds
-
+```python
 load.countdown(5)
 
 load.loading1(10)
 
 print()
 
 load.loading2(5)
 
 print()
 
 load.loading3(5)
-
+```
 # License
 This project is given free for use and download under the MIT license.
 
 # Project Status
 Still undergoing enhancements.
 
 # How to Contribute
```

### Comparing `consoleprint-1.2.5/pyproject.toml` & `consoleprint-1.2.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ConsolePrint"
-version = "1.2.5"
+version = "1.2.7"
 authors = [
   { name="Udemezue Iloabachie", email="udemezue@gmail.com" },
 ]
 description = "A package to animate and beautify print output to console"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `consoleprint-1.2.5/PKG-INFO` & `consoleprint-1.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ConsolePrint
-Version: 1.2.5
+Version: 1.2.7
 Summary: A package to animate and beautify print output to console
 Project-URL: Homepage, https://github.com/iloabachie/ConsolePrint
 Project-URL: Bug Tracker, https://github.com/iloabachie/ConsolePrint/issues
 Author-email: Udemezue Iloabachie <udemezue@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # ConsolePrint
 This module making printing to the terminal more exciting by animating the text output.
 It also makes output richer my modifying the color
 You can also save routine console output to a file using the console2file module.
 Created using python 3.11
@@ -21,34 +21,34 @@
 # Installation
 You may install it form PyPI.org using the pip command.
 
 pip install ConsolePrint
 
 # Usage
 Copy the code below and run it from your IDE, preferable Visual Studio Code.  May not produce the desired output on some terminals.
-
+```python
 import ConsolePrint.animate as prt    
 
 import ConsolePrint.console2file as file  
 
 import ConsolePrint.loading as load        
-
+```
 # Test Cases
 1.  Here uou may change the arguments as desired
-
+```python
 file.startConsoleSave()
 
 'Saves all output between the start and end functions to file.'
 
 from calendar import calendar
 
 print(calendar(2023))
 
 file.endConsoleSave()
-
+```
 2. Here you may use ANSI escape sequences for the format argument and change others as desired.
 Preset arguments for format:
 //colours
 'default':          '\033[0m'
 'grey':             '\033[30m'
 'red':              '\033[31m'
 'green':            '\033[32m'
@@ -67,14 +67,15 @@
 'green_bg':         '\033[42m'
 'yellow_bg':        '\033[43m'
 'blue_bg':          '\033[44m'
 'magenta_bg':       '\033[45m'
 'cyan_bg':          '\033[46m'
 'white_bg':         '\033[47m'
 
+```python
 prt.printing("hello this should print letter by letter", delay=0.05, style="letter", stay=True, rev=False, format='strike')
 
 prt.printing("hello this should print word by word but in reverse", delay=0.3, style="word", stay=True, rev=True, format='red_bg')
 
 prt.flashprint("The entire text should flash", blinks=5, delay=0.2, stay=True, format='green')
 
 prt.flashtext("The text in  will flash", "UPPER CASE", blinks=5, index=12, delay=0.2, format='yellow')
@@ -82,29 +83,30 @@
 prt.animate1("This text is animated with #", symbol="#", format='white')
 
 prt.animate2("Prints letter by letter but masked with # first  ", symbol="#", delay=0.05, format="\033[48;5;150m")
 
 prt.text_box("B O X E D  I N", symbol="#", padding=True, wall=True, align='center', format='\033[48;5;4m')
 
 prt.asteriskify('This has been asteriskified', align='center', underscore=True, format='cyan')
+```
 
 3.  Here, the load time is specified in seconds
-
+```python
 load.countdown(5)
 
 load.loading1(10)
 
 print()
 
 load.loading2(5)
 
 print()
 
 load.loading3(5)
-
+```
 # License
 This project is given free for use and download under the MIT license.
 
 # Project Status
 Still undergoing enhancements.
 
 # How to Contribute
```

