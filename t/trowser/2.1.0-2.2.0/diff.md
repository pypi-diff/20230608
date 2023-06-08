# Comparing `tmp/trowser-2.1.0.tar.gz` & `tmp/trowser-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trowser-2.1.0.tar", last modified: Sun Apr 23 10:13:49 2023, max compression
+gzip compressed data, was "trowser-2.2.0.tar", last modified: Thu Jun  8 19:05:11 2023, max compression
```

## Comparing `trowser-2.1.0.tar` & `trowser-2.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-23 10:13:49.486427 trowser-2.1.0/
--rw-r--r--   0 tom      (31978) tom       (2000)    35149 2019-10-03 08:02:54.000000 trowser-2.1.0/LICENSE
--rw-r--r--   0 tom      (31978) tom       (2000)       98 2023-04-23 09:49:26.000000 trowser-2.1.0/MANIFEST.in
--rw-r--r--   0 tom      (31978) tom       (2000)    25740 2023-04-23 10:13:49.486427 trowser-2.1.0/PKG-INFO
--rw-r--r--   0 tom      (31978) tom       (2000)    10444 2023-04-23 09:49:26.000000 trowser-2.1.0/README.md
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-23 10:13:49.486427 trowser-2.1.0/bin/
--rwxr-xr-x   0 tom      (31978) tom       (2000)   345741 2023-04-23 10:13:49.000000 trowser-2.1.0/bin/trowser.py
--rw-r--r--   0 tom      (31978) tom       (2000)       38 2023-04-23 10:13:49.486427 trowser-2.1.0/setup.cfg
--rwxr-xr-x   0 tom      (31978) tom       (2000)     1967 2023-04-23 10:13:12.000000 trowser-2.1.0/setup.py
-drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-04-23 10:13:49.486427 trowser-2.1.0/trowser.egg-info/
--rw-r--r--   0 tom      (31978) tom       (2000)    25740 2023-04-23 10:13:49.000000 trowser-2.1.0/trowser.egg-info/PKG-INFO
--rw-r--r--   0 tom      (31978) tom       (2000)      177 2023-04-23 10:13:49.000000 trowser-2.1.0/trowser.egg-info/SOURCES.txt
--rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-04-23 10:13:49.000000 trowser-2.1.0/trowser.egg-info/dependency_links.txt
--rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-04-23 10:13:49.000000 trowser-2.1.0/trowser.egg-info/top_level.txt
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-06-08 19:05:11.089450 trowser-2.2.0/
+-rw-r--r--   0 tom      (31978) tom       (2000)    35149 2019-10-03 08:02:54.000000 trowser-2.2.0/LICENSE
+-rw-r--r--   0 tom      (31978) tom       (2000)       74 2023-06-08 18:59:54.000000 trowser-2.2.0/MANIFEST.in
+-rw-r--r--   0 tom      (31978) tom       (2000)    26263 2023-06-08 19:05:11.089450 trowser-2.2.0/PKG-INFO
+-rw-r--r--   0 tom      (31978) tom       (2000)    10385 2023-06-08 18:57:20.000000 trowser-2.2.0/README.md
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-06-08 19:05:11.089450 trowser-2.2.0/bin/
+-rwxr-xr-x   0 tom      (31978) tom       (2000)   340253 2023-06-08 19:05:11.000000 trowser-2.2.0/bin/trowser.py
+-rw-r--r--   0 tom      (31978) tom       (2000)       38 2023-06-08 19:05:11.089450 trowser-2.2.0/setup.cfg
+-rwxr-xr-x   0 tom      (31978) tom       (2000)     2031 2023-06-08 18:57:20.000000 trowser-2.2.0/setup.py
+drwxr-xr-x   0 tom      (31978) tom       (2000)        0 2023-06-08 19:05:11.089450 trowser-2.2.0/trowser.egg-info/
+-rw-r--r--   0 tom      (31978) tom       (2000)    26263 2023-06-08 19:05:11.000000 trowser-2.2.0/trowser.egg-info/PKG-INFO
+-rw-r--r--   0 tom      (31978) tom       (2000)      207 2023-06-08 19:05:11.000000 trowser-2.2.0/trowser.egg-info/SOURCES.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-06-08 19:05:11.000000 trowser-2.2.0/trowser.egg-info/dependency_links.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)       41 2023-06-08 19:05:11.000000 trowser-2.2.0/trowser.egg-info/requires.txt
+-rw-r--r--   0 tom      (31978) tom       (2000)        1 2023-06-08 19:05:11.000000 trowser-2.2.0/trowser.egg-info/top_level.txt
```

### Comparing `trowser-2.1.0/LICENSE` & `trowser-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trowser-2.1.0/PKG-INFO` & `trowser-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trowser
-Version: 2.1.0
+Version: 2.2.0
 Summary: Trowser is a graphical browser for large line-oriented text files with sytax highlighting and search facilities tailored for analysis of debug log files.
 Home-page: https://github.com/tomzox/trowser
 Author: T. Zoerner
 Author-email: tomzox@gmail.com
 License: UNKNOWN
 Keywords: color-highlighter,text-search,text-browser,tkinter-gui,GUI
 Platform: posix
@@ -23,17 +23,17 @@
 
 trowser := Trace Browser
 ========================
 
 Description
 -----------
 
-*Trowser* is a graphical browser for large line-oriented text files with color highlighting and a highly flexible search and cherry-picking window. Trowser was developed as an alternative to UNIX-tool "less" when analyzing debug log files (aka traces - hence the name).
+*Trowser* is a graphical browser for large line-oriented text files with color highlighting and a highly flexible search and cherry-picking window. Trowser was developed as an alternative to tools such as "less" (UNIX) or "Notepad++" (Windows) when analyzing debug log files (or "trace files", as they are often called in embedded software world - hence the name).
 
-Trowser has a graphical interface, but is designed to allow browsing via the keyboard at least to the same extent as less. Key bindings and the cursor positioning concept are derived from vim.
+Trowser has a graphical interface, but is designed to allow browsing via the keyboard at least to the same extent as less. Additional key bindings and the cursor positioning concept are derived from the Vim text editor.
 
 Note in this context "line-oriented" denotes that each line of text is considered a data unit.  Color highlighting (including search matches) will always apply the highlight to a complete line of text.
 
 When you start trowser for the first time, you'll have to create highlight patterns for your type of file.  To do this, first enter a search pattern and verify that it matches the intended lines. Then open the *Edit highlight patterns* dialog in the *Search* menu, press the right mouse button to open the context menu and select *Add current search*. You can change the highlight color or select a different kind of mark-up by double-clicking on the new entry in the dialog, or by selecting *Edit markup* in the context menu.  To define new colors, click on *Edit color palette* at the bottom of the markup editor dialog.
 
 There are several ways to quickly navigate in the file to lines matching search patterns: Firstly, you can search forwards or backwards to any sub-string or pattern you enter in the *Find:* field. Secondly, you can repeat previous searches by opening the search history dialog and double-clicking on an entry, or by clicking *Next* or *Previous*. Third, you can assign bookmarks to selected text lines and jump in-between those lines by clicking on them in the bookmark list dialog or via ``'+`` and ``'-`` key bindings (not in vim.) Fourth, you can search for patterns defined in the color highlight list by selecting a pattern in the list and then clicking on *Next* or *Previous* in the pattern list dialog. Fifth, you can open the *Search result list* (via the *Search* menu or by clicking on *List all* in any dialog or by entering ``ALT-a``) to display all text lines which match a set of patterns and click on an entry in this list to jump to the respective line in the main window. Sixth, you can manually copy arbitrary lines from the main text window into the search result window via the ``'i'`` key (not in vim.)
 
@@ -283,38 +283,42 @@
 
 Options
 -------
 
 The following command line options are available:
 
 **-h** *limit*, **--head=limit**
-  This option specifies the maximum number of bytes read from the start of the input file or stream, i.e. any following text is silently ignored.
+  This option specifies the maximum number of bytes to load from input file or stream for display. When loading from a stream via STDIN, it's possible to continue reading more data later via command *Continue loading STDIN*.
 
-  The limit value is remembered in the configuration file and used in the next invocation unless overridden.  When neither **-h** or **-t** are specified and data is loaded from a stream via STDIN, a small dialog window pops up when the buffer limit is exceeded. This allows the user to select between head and tail modes manually.
+  The limit value is remembered in the configuration file and used as default the next time data is loaded from STDIN. When loading from a file, default is to load the complete file.
+
+  When neither option **-h** or **-t** are specified and data is loaded from a stream via STDIN, a small dialog window pops up when the buffer limit is exceeded. This allows the user to select between head and tail modes manually.
 
 **-t** *limit*, **--tail=limit**
-  This option specifies the maximum number of bytes to be read into the display buffer.  If the input is a file which is larger then the given buffer limit, text at the beginning of the file is skipped. If the input is a stream, all data is read into a temporary queue until the end-of-stream is reached; then the last *limit* number of bytes which were read from the stream are loaded into the display buffer.
+  This option specifies to load only the given maximum number of bytes into the display from the end of the file or input stream. This means when reading from a file, data from the beginning is skipped if the file is larger than the limit.  If the input is a STDIN stream, data is read into a ring buffer of the given size. Once the end-of-stream is reached, the last content of the ring buffer is loaded into the display.
 
-  The limit value is remembered in the configuration file and used in the next invocation unless overridden.
+  The limit value is remembered in the configuration file equivalently as described for the "head" option.
 
 **-r** *path*, **--rcfile=path**
-  This option can be used to specify an alternate configuration file. When this option is not present, the configuration file is stored in the home directory, see section FILES.
+  This option can be used to specify an alternate configuration file. When this option is not present, the configuration file is stored in system directories, see `Files`_.
 
 Environment
 -----------
 
 **trowser** only evaluates the standard variables **DISPLAY** (X11 display address) and **HOME** (home directory, for storing the configuration file.)
 
 Files
 -----
 
 **$HOME/.config/trowser/trowser.py.rc**
-  *UNIX*: Configuration file where all personal settings and the search history are stored. Per default this file is created in your home directory, but a different path and file name can be specified with the **--rcfile** option (see `Options`_).
+  *UNIX*: Configuration file where all personal settings and the search history are stored. The path may be overriden via environment variable ``XDG_CONFIG_HOME``. A different file name can be specified with the **--rcfile** option (see `Options`_).
+
+  During updates to this file, trowser temporarily creates a new file the same directory, where "XXXXX" is a random number. The old file is then replaced with this new file. This procedure will obviously fail if the target directory (not the file itself!) is not writable.
 
-  During updates to this file, trowser temporarily creates a file called ``.trowserc.XXXXX.tmp`` in the home directory, where "XXXXX" is a random number. The old file is then replaced with this new file. This procedure will obviously fail if your home directory is not writable.
+  *MS Windows*: On the MS Windows platform, the configuration file is created in the hidden application data directory in your user home. The specific path depends on your operating system version. (The path is qeried via a system API.)
 
 Caveats
 -------
 
 Currently only one pattern list for color highlighting is supported. Hence different highlighting for different file types can only be done by choosing different configuration files when starting trowser (see the *--rcfile* option.)
 
 Vim compatibility: Not all vim navigation commands are implemented; Command repetition is supported only for a small sub-set of commands; Some commands behave slightly differently from vim (most notably the bookmark related commands.) vim's range and selection commands are not supported at all.
```

### Comparing `trowser-2.1.0/README.md` & `trowser-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Trowser
 
 Trowser is a browser for large line-oriented text files with color highlighting
 and a highly flexible search and cherry-picking window.  Trowser was developed
-as an alternative to UNIX-tool "less" when analyzing debug log/trace files
+as an alternative to tools such as "less" (UNIX) or "Notepad++" (Windows)
+when analyzing debug log/trace files
 created by other applications. Trowser integrates well with
-[GtestGui](http://github.com/tomzox/gtest_gui) as viewer for text output of test
-applications using GoogleTest framework.
+[GtestGui test-runner](http://github.com/tomzox/gtest_gui) as viewer for
+text output of test applications using GoogleTest (GTest) framework.
 
 Compared to plain text viewers, trowser adds color highlighting, a persistent
 search history, graphical bookmarking and a separate search result window. The
 search window is especially designed to be main facility for performing trace
 analysis: Using multiple consecutive searches, manual additions or removals,
 undo/redo and subtractive searches, it can be filled with a condensed view of
 the trace file, holding only the lines relevant to the issue under analysis.
@@ -129,63 +130,59 @@
 appropriate font and configuring expressions for syntax highlighting under menu
 "Search / Edit highlight patterns". Then adjust the window and dialog sizes and
 locations. trowser will remember these settings in its configuration file
 stored in `$HOME/.config/trowser/`.
 
 ## Installing Tcl/Tk & Python versions
 
+The Python variant is available as a package on
+[PyPi](https://pypi.org/project/trowser/)
+
 Software Requirements: trowser can be used on all platforms which are supported
 by either the Tcl/Tk or Python interpreters. This means all UNIX variants,
 Linux, Mac, and even MS Windows. On the other hand, this means a prerequisite
 is installing either [Tcl/Tk](http://tcl.tk/) (version 8.5 or later) or
 [Python](https://www.python.org/). The latter can be done semi-automatically
 when creating packages using the scripts described below.
 
-Hardware requirements: trowser loads the complete text into memory (i.e. in
-a Tk text widget) and also applies highlighting to the complete text to
-allow fast navigation.  Hence when browsing large files, trowser benefits
-from using a fast machine and at least 5 times your text size in RAM.
-
 trowser can be used without installation, if you copy the script simply in
 the same directory as the files you want to open with it. Note trowser
 expects to be given the name of the file you want to open on the command line.
 
-Otherwise, manual installation on UNIX-like systems is also simple:
-Just copy the script into /usr/bin (optionally you can remove the ".tcl"
-appendix) and the manual page to /usr/share/man/man1.
-However it's recommended to properly install the files using a package,
-as this will also take care of dependencies and allow easy removal.
-
-If you're using a Debian, Ubuntu or a compatible Linux distribution, you
-can create a package for the Tcl/Tk version using script `create_deb.sh`,
-or for the Python version using `create_deb_py.sh` respectively.
-The scripts will copy the required files into a local sub-directory `deb`
-and then create a package (e.g. `deb/trowser_1.3-3.deb`) which can be installed.
-In summary:
+The Python version is best installed using `pip3 install trowser`. This will
+automatically download the latest release of the package from pypi.org (plus
+dependency "appdirs" on the Win32 platform) and install them.
+
+Alternatively, or if you want to install the latest code found here on GitHub,
+Python and Tcl/Tk versions can be installed as a system package if you're using
+a Debian, Ubuntu or a compatible Linux distribution: You can create a Debian
+package for using script `create_deb.sh` for Tcl/Tk, or using script
+`create_deb_py.sh` for Python respectively. The scripts will copy the required
+files into a local sub-directory `deb` and then create a package which can be
+installed using the generated package file. Example:
 
 ```console
     bash create_deb.sh
     dpkg -i deb/trowser_1.3-3_all.deb
 ```
 
 The software is released under the
 [GNU General Public License, version 3](http://www.fsf.org/copyleft/gpl.html)
 
-Originally the project homepage was <http://www.nefkom.net/tomzo/prj/trowser/>,
-but this page is now defunct.
-
 ## Troubleshooting (Tcl/Tk version)
 
 If trowser fails to start or aborts with an interpreter error, you should
 check if Tcl/Tk is installed and has the required version by entering the
 following command line in a terminal window (i.e. in a shell):
 
 ```console
     echo 'puts $tcl_patchLevel;exit' | wish
 ```
 In some Tcl/Tk installations "wish" as such may not exist, but instead the
 major and minor version are appended to the executable name (e.g."wish8.5".)
 In this case, change the third line in the trowser.tcl script file accordingly.
 
-As of writing this (2009), trowser is tested against Tcl/Tk version 8.5.6. If the
-above command returns a version older than 8.4.0, you'd have to upgrade
-your Tcl/Tk library.
+Current version of trowser is tested against Tcl/Tk version 8.6, but it should
+also still work with predecessor Tcl/Tk versions 8.5 and 8.4. If the above
+command returns an even older version, you'll have to upgrade your Tcl/Tk
+library for using trowser. In Python, you can determine the version of
+underlying Tcl/Tk simply by running `python -m tkinter`.
```

### Comparing `trowser-2.1.0/bin/trowser.py` & `trowser-2.2.0/bin/trowser.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,27 @@
 from datetime import datetime
 from datetime import timedelta
 import time
 import tempfile
 import json
 import re
 import traceback
-import tkinter
 import tkinter.font as tkf
 from tkinter import *
 from tkinter import messagebox
 from tkinter import filedialog
 from tkinter import colorchooser
 
+# Module "appdirs" is required on Windows to learn the directory where to store
+# application configuration files. Install the module via "pip3 install appdirs"
+# if the import fails. (Alternatively, you could replace the one function call
+# into the module with a hard-coded path.)
+if sys.platform == "win32":
+    import appdirs
+
 #
 # This function is used during start-up to define fonts, colors and
 # global event binding tags.
 #
 def InitResources():
   global font_normal, font_bold, font_hlink, img_marker
 
@@ -102,59 +108,56 @@
 
 #
 # This function creates the main window of the trace browser, including the
 # menu at the top, the text area and a vertical scrollbar in the middle, and
 # the search control dialog at the bottom.
 #
 def CreateMainWindow():
-  global font_content, col_bg_content, col_fg_content, fmt_selection
-  global win_geom, fmt_find, fmt_findinc
-  global tlb_find, tlb_hall, tlb_case, tlb_regexp
-
   # menubar at the top of the main window
   wt.menubar = Menu(tk)
 
-  wt.menubar_ctrl = Menu(wt.menubar, tearoff=0, postcommand=lambda:MenuPosted())
-  wt.menubar_ctrl.add_command(label="Open file...", command=lambda:MenuCmd_OpenFile())
-  wt.menubar_ctrl.add_command(label="Reload current file", state=DISABLED, command=lambda:MenuCmd_Reload())
+  wt.menubar_ctrl = Menu(wt.menubar, tearoff=0, postcommand=MenuPosted)
+  wt.menubar_ctrl.add_command(label="Open file...", command=MenuCmd_OpenFile)
+  wt.menubar_ctrl.add_command(label="Reload current file", state=DISABLED, command=MenuCmd_Reload)
   wt.menubar_ctrl.add_separator()
   wt.menubar_ctrl.add_command(label="Discard above cursor...", command=lambda:MenuCmd_Discard(False))
   wt.menubar_ctrl.add_command(label="Discard below cursor...", command=lambda:MenuCmd_Discard(True))
   wt.menubar_ctrl.add_separator()
-  wt.menubar_ctrl.add_command(label="Font selection...", command=lambda:FontList_OpenDialog())
+  wt.menubar_ctrl.add_command(label="Font selection...", command=FontList_OpenDialog)
+  wt.menubar_ctrl.add_command(label="Toggle line-wrap", command=ToggleLineWrap, accelerator="ALT-w")
   wt.menubar_ctrl.add_separator()
-  wt.menubar_ctrl.add_command(label="Quit", command=lambda:UserQuit())
+  wt.menubar_ctrl.add_command(label="Quit", command=UserQuit)
 
-  wt.menubar_search = Menu(wt.menubar, tearoff=0, postcommand=lambda:MenuPosted())
-  wt.menubar_search.add_command(label="Search history...", command=lambda:SearchHistory_Open())
-  wt.menubar_search.add_command(label="Edit highlight patterns...", command=lambda:TagList_OpenDialog())
+  wt.menubar_search = Menu(wt.menubar, tearoff=0, postcommand=MenuPosted)
+  wt.menubar_search.add_command(label="Search history...", command=SearchHistory_Open)
+  wt.menubar_search.add_command(label="Edit highlight patterns...", command=TagList_OpenDialog)
   wt.menubar_search.add_separator()
   wt.menubar_search.add_command(label="List all search matches...", command=lambda:SearchAll(True, 0), accelerator="ALT-a")
   wt.menubar_search.add_command(label="List all matches above...", command=lambda:SearchAll(True, 1), accelerator="ALT-P")
   wt.menubar_search.add_command(label="List all matches below...", command=lambda:SearchAll(True, 1), accelerator="ALT-N")
   wt.menubar_search.add_separator()
-  wt.menubar_search.add_command(label="Clear search highlight", command=lambda:SearchHighlightClear(), accelerator="&")
+  wt.menubar_search.add_command(label="Clear search highlight", command=SearchHighlightClear, accelerator="&")
   wt.menubar_search.add_separator()
   wt.menubar_search.add_command(label="Goto line number...", command=lambda:KeyCmd_OpenDialog("goto"))
 
-  wt.menubar_mark = Menu(wt.menubar, tearoff=0, postcommand=lambda:MenuPosted())
+  wt.menubar_mark = Menu(wt.menubar, tearoff=0, postcommand=MenuPosted)
   wt.menubar_mark.add_command(label="Toggle bookmark", accelerator="m", command=Mark_ToggleAtInsert)
-  wt.menubar_mark.add_command(label="List bookmarks", command=lambda:MarkList_OpenDialog())
-  wt.menubar_mark.add_command(label="Delete all bookmarks", command=lambda:Mark_DeleteAll())
+  wt.menubar_mark.add_command(label="List bookmarks", command=MarkList_OpenDialog)
+  wt.menubar_mark.add_command(label="Delete all bookmarks", command=Mark_DeleteAll)
   wt.menubar_mark.add_separator()
   wt.menubar_mark.add_command(label="Jump to prev. bookmark", command=lambda:Mark_JumpNext(False), accelerator="'-")
   wt.menubar_mark.add_command(label="Jump to next bookmark", command=lambda:Mark_JumpNext(True), accelerator="'+")
   wt.menubar_mark.add_separator()
-  wt.menubar_mark.add_command(label="Read bookmarks from file...", command=lambda:Mark_ReadFileFrom())
-  wt.menubar_mark.add_command(label="Save bookmarks to file...", command=lambda:Mark_SaveFileAs())
+  wt.menubar_mark.add_command(label="Read bookmarks from file...", command=Mark_ReadFileFrom)
+  wt.menubar_mark.add_command(label="Save bookmarks to file...", command=Mark_SaveFileAs)
 
-  wt.menubar_help = Menu(wt.menubar, name="help", tearoff=0, postcommand=lambda:MenuPosted())
+  wt.menubar_help = Menu(wt.menubar, name="help", tearoff=0, postcommand=MenuPosted)
   dlg_help_add_menu_commands(wt.menubar_help)
   wt.menubar_help.add_separator()
-  wt.menubar_help.add_command(label="About", command=lambda:OpenAboutDialog())
+  wt.menubar_help.add_command(label="About", command=OpenAboutDialog)
 
   wt.menubar.add_cascade(label="Control", menu=wt.menubar_ctrl, underline=0)
   wt.menubar.add_cascade(label="Search", menu=wt.menubar_search, underline=0)
   wt.menubar.add_cascade(label="Bookmarks", menu=wt.menubar_mark, underline=0)
   wt.menubar.add_cascade(label="Help", menu=wt.menubar_help)
   tk.config(menu=wt.menubar)
 
@@ -345,16 +348,14 @@
 
 # ----------------------------------------------------------------------------
 #
 # This function is called during start-up to create tags for all color
 # highlights.
 #
 def HighlightCreateTags():
-  global patlist
-
   for w in patlist:
     tagnam = w[4]
 
     HighlightConfigure(wt.f1_t, tagnam, w)
     wt.f1_t.tag_lower(tagnam, "find")
 
 
@@ -362,15 +363,15 @@
 # This function is called after loading a new text to apply the color
 # highlighting to the complete text. This means all matches on all
 # highlight patterns has to be searched for. Since this can take some
 # time, the operation done in the background to avoid blocking the user.
 # The CPU is given up voluntarily after each pattern and after max. 100ms
 #
 def HighlightInit():
-  global patlist, tid_high_init
+  global tid_high_init
 
   if wt_exists(wt.hipro):
     wt.hipro.destroy()
     wt.hipro = None
 
   if len(patlist) > 0:
     # create a progress bar as overlay to the main window
@@ -395,16 +396,15 @@
 #
 # This function is a slave-function of HighlightInit. The function
 # loops across all members in the global pattern list to apply color
 # the respective highlighting. The loop is broken up by installing each
 # new iteration as an idle event (and limiting each step to 100ms)
 #
 def HighlightInitBg(pat_idx, cid, line, loop_cnt):
-  global block_bg_tasks, tid_search_inc, tid_search_hall, tid_search_list
-  global patlist, tid_high_init
+  global tid_high_init
 
   if block_bg_tasks or (tid_search_inc is not None) or (tid_search_hall is not None) or (tid_search_list is not None):
     # background tasks are suspended - re-schedule with timer
     tid_high_init = tk.after(100, lambda:HighlightInitBg(pat_idx, cid, line, 0))
   elif loop_cnt > 10:
     # insert a small timer delay to allow for idle-driven interactive tasks (e.g. selections)
     tid_high_init = tk.after(10, lambda:HighlightInitBg(pat_idx, cid, line, 0))
@@ -442,25 +442,25 @@
 # This function searches for all lines in the main text widget which match the
 # given pattern and adds the given tag to them.  If the loop doesn't complete
 # within 100ms, the search is paused and the function returns the number of the
 # last searched line.  In this case the caller must invoke the funtion again
 # (as an idle event, to allow user-interaction in-between.)
 #
 def HighlightLines(pat, tagnam, opt, line):
-  max_line = int(wt.f1_t.index("end").split(".")[0])
+  max_line = int(wt.f1_t.index("end").split(".", maxsplit=1)[0])
   start_t = datetime.now()
   max_delta = timedelta(microseconds=100000)
 
   while line < max_line:
     pos = wt.f1_t.search(pat, "%d.0" % line, "end", **opt)
     if pos == "":
       break
 
     # match found, highlight this line
-    line = int(pos.split(".")[0])
+    line = int(pos.split(".", maxsplit=1)[0])
     wt.f1_t.tag_add(tagnam, "%d.0" % line, "%d.0" % (line + 1))
     # trigger the search result list dialog in case the line is included there too
     SearchList_HighlightLine(tagnam, line)
     line += 1
 
     # limit the runtime of the loop - return start line number for the next invocation
     if (datetime.now() - start_t > max_delta) and (line < max_line):
@@ -473,15 +473,15 @@
 #
 # This helper function schedules the line highlight function until highlighting
 # is complete for the given pattern.  This function is used to add highlighting
 # for single tags (e.g. modified highlight patterns or colors; currently not used
 # for search highlighting because a separate "cancel ID" is required.)
 #
 def HighlightAll(pat, tagnam, opt, line=1, loop_cnt=0):
-  global tid_high_init, block_bg_tasks
+  global tid_high_init
 
   if block_bg_tasks:
     # background tasks are suspended - re-schedule with timer
     tid_high_init = tk.after(100, lambda: HighlightAll(pat, tagnam, opt, line, 0))
   elif loop_cnt > 10:
     # insert a small timer delay to allow for idle-driven interactive tasks (e.g. selections)
     tid_high_init = tk.after(10, lambda: HighlightAll(pat, tagnam, opt, line, 0))
@@ -498,43 +498,39 @@
 #
 # This function searches the currently visible text content for all lines
 # which contain the given sub-string and marks these lines with the given tag.
 #
 def HighlightVisible(pat, tagnam, opt):
   start_pos = wt.f1_t.index("@1,1")
   end_pos = wt.f1_t.index("@%d,%d" % (wt.f1_t.winfo_width() - 1, wt.f1_t.winfo_height() - 1))
-  line = int(start_pos.split(".")[0])
-  max_line = int(end_pos.split(".")[0])
+  line = int(start_pos.split(".", maxsplit=1)[0])
+  max_line = int(end_pos.split(".", maxsplit=1)[0])
   #puts "visible $start_pos...$end_pos: $pat $opt"
 
   while line < max_line:
     pos = wt.f1_t.search(pat, "%d.0" % line, "end", **opt)
     if pos == "":
       break
-    line = int(pos.split(".")[0])
+    line = int(pos.split(".", maxsplit=1)[0])
     wt.f1_t.tag_add(tagnam, "%d.0" % line, "%d.0" % (line + 1))
     line += 1
 
 
 #
 # This callback is installed to the main text widget's yview. It is used
 # to detect changes in the view to update highlighting if the highlighting
 # task is not complete yet. The event is forwarded to the vertical scrollbar.
 #
 def Highlight_YviewCallback(frac1, frac2):
-  global tid_high_init, tid_search_hall
-
   if tid_high_init is not None:
-    global patlist
     for w in patlist:
       opt = Search_GetOptions(w[0], w[1], w[2])
       HighlightVisible(w[0], w[4], opt)
 
   if tid_search_hall is not None:
-    global tlb_cur_hall_opt
     HighlightVisible(tlb_cur_hall_opt[0], "find", tlb_cur_hall_opt[1])
 
   # automatically remove the redirect if no longer needed
   if (tid_high_init is None) and (tid_search_hall is None):
     wt.f1_t.configure(yscrollcommand=wt.f1_sb.set)
 
   wt.f1_sb.set(frac1, frac2)
@@ -552,16 +548,14 @@
 #
 # This function creates or updates a text widget tag with the options of
 # a color highlight entry.  The function is called during start-up for all
 # highlight patterns, and by the highlight edit dialog (also used for the
 # sample text widget.)
 #
 def HighlightConfigure(wid, tagname, w):
-  global font_content
-
   cfg = {}
   if w[8]:
     cfg["font"] = DeriveFont(font_content, 0, "bold")
   else:
     cfg["font"] = ""
 
   if w[9]:
@@ -619,15 +613,15 @@
 #
 # This function triggers color highlighting of all lines of text which match
 # the current search string.  The function is called when global highlighting
 # is en-/disabled, when the search string is modified or when search options
 # are changed.
 #
 def SearchHighlightUpdate(pat, opt):
-  global tlb_hall, tlb_cur_hall_opt, tid_search_hall
+  global tlb_cur_hall_opt, tid_search_hall
 
   if pat != "":
     if tlb_hall.get():
       if opt.get("forwards"): del opt["forwards"]
       if opt.get("backwards"): del opt["backwards"]
 
       if tk.focus_get() != wt.f2_e:
@@ -657,30 +651,28 @@
 
 
 #
 # This is a wrapper for the above function which works on the current
 # pattern in the search entry field.
 #
 def SearchHighlightUpdateCurrent():
-  global tlb_hall, tlb_find, tlb_regexp, tlb_case
-
   if tlb_hall.get():
     pat = tlb_find.get()
     if pat != "":
       if SearchExprCheck(pat, tlb_regexp.get(), True):
         opt = Search_GetOptions(pat, tlb_regexp.get(), tlb_case.get())
         SearchHighlightUpdate(pat, opt)
 
 
 #
 # This helper function calls the global search highlight function until
 # highlighting is complete.
 #
 def SearchHighlightAll(pat, tagnam, opt, line=1, loop_cnt=0):
-  global tid_search_hall, block_bg_tasks
+  global tid_search_hall
 
   if block_bg_tasks:
     # background tasks are suspended - re-schedule with timer
     tid_search_hall = tk.after(100, lambda: SearchHighlightAll(pat, tagnam, opt, line, 0))
   elif loop_cnt > 10:
     # insert a small timer delay to allow for idle-driven interactive tasks (e.g. selections)
     tid_search_hall = tk.after(10, lambda: SearchHighlightAll(pat, tagnam, opt, line, 0))
@@ -695,31 +687,27 @@
 
 
 #
 # This function is bound to the "Highlight all" checkbutton to en- or disable
 # global highlighting.
 #
 def SearchHighlightOnOff():
-  global tlb_hall
-
   tlb_hall.set(not tlb_hall.get())
   UpdateRcAfterIdle()
 
   SearchHighlightUpdateCurrent()
 
 
 #
 # This function is invoked after a change in search settings (i.e. case
 # match, reg.exp. or global highlighting.)  The changed settings are
 # stored in the RC file and a possible search highlighting is removed
 # or updated (the latter only if global highlighting is enabled)
 #
 def SearchHighlightSettingChange():
-  global tlb_hall
-
   UpdateRcAfterIdle()
 
   SearchHighlightClear()
   if tlb_hall.get():
     SearchHighlightUpdateCurrent()
 
 
@@ -730,39 +718,38 @@
 #
 # This function is invoked when the user enters text in the "find" entry field.
 # In contrary to the "atomic" search, this function only searches a small chunk
 # of text, then re-schedules itself as an "idle" task.  The search can be aborted
 # at any time by canceling the task.
 #
 def Search_Background(pat, is_fwd, opt, start, is_changed, callback):
-  global block_bg_tasks, tid_search_inc, tid_search_list
   global tid_search_inc
 
   if block_bg_tasks:
     # background tasks are suspended - re-schedule with timer
     tid_search_inc = tk.after(100, lambda: Search_Background(pat, is_fwd, opt, start, is_changed, callback))
     return
 
   if is_fwd:
     end = wt.f1_t.index("end")
   else:
     end = "1.0"
 
   if start != end:
     if is_fwd:
-      next = wt.f1_t.index(start + " + 5000 lines lineend")
+      next_line = wt.f1_t.index(start + " + 5000 lines lineend")
     else:
-      next = wt.f1_t.index(start + " - 5000 lines linestart")
+      next_line = wt.f1_t.index(start + " - 5000 lines linestart")
 
     # invoke the actual search in the text widget content
     match_len = IntVar(tk, 0)
-    pos = wt.f1_t.search(pat, start, next, count=match_len, **opt)
+    pos = wt.f1_t.search(pat, start, next_line, count=match_len, **opt)
 
     if pos == "":
-      tid_search_inc = tk.after_idle(lambda: Search_Background(pat, is_fwd, opt, next, is_changed, callback))
+      tid_search_inc = tk.after_idle(lambda: Search_Background(pat, is_fwd, opt, next_line, is_changed, callback))
     else:
       tid_search_inc = None
       Search_HandleMatch(pos, match_len.get(), pat, opt, is_changed)
       callback(pos, pat, is_fwd, is_changed)
 
   else:
     tid_search_inc = None
@@ -772,15 +759,15 @@
 
 #
 # This function searches the main text content for the expression in the
 # search entry field, starting at the current cursor position. When a match
 # is found, the cursor is moved there and the line is highlighed.
 #
 def Search_Atomic(pat, is_re, use_case, is_fwd, is_changed):
-  global tlb_hall, tlb_last_dir
+  global tlb_last_dir
 
   pos = ""
   if (pat != "") and SearchExprCheck(pat, is_re, True):
 
     tlb_last_dir = is_fwd
     search_opt = Search_GetOptions(pat, is_re, use_case, tlb_last_dir)
     start_pos = Search_GetBase(is_fwd, False)
@@ -850,15 +837,15 @@
 # This function handles the result of a text search in the main window. If
 # a match was found, the cursor is moved to the start of the match and the
 # matching section and complete line are highlighted. Optionally, a background
 # process to highlight all matches is started. If no match is found, any
 # previously applied search highlighting is removed.
 #
 def Search_HandleMatch(pos, match_len, pat, opt, is_changed):
-  global tlb_find_line, tlb_hall, tlb_cur_hall_opt
+  global tlb_find_line
 
   if (pos != "") or is_changed:
     if not tlb_hall.get() or (tlb_cur_hall_opt[0] != pat):
       SearchHighlightClear()
     else:
       wt.f1_t.tag_remove("findinc", "1.0", "end")
 
@@ -894,28 +881,28 @@
 
 #
 # This function is bound to all changes of the search text in the
 # "find" entry field. It's called when the user enters new text and
 # triggers an incremental search.
 #
 def SearchVarTrace(name1, name2, op):
+  # pylint: disable=unused-argument  # signature cannot be changed
   global tid_search_inc
-  global tlb_last_dir
 
   if tid_search_inc is not None: tk.after_cancel(tid_search_inc)
   tid_search_inc = tk.after(50, lambda: SearchIncrement(tlb_last_dir, True))
 
 
 #
 # This function performs a so-called "incremental" search after the user
 # has modified the search text. This means searches are started already
 # while the user is typing.
 #
 def SearchIncrement(is_fwd, is_changed):
-  global tlb_find, tlb_regexp, tlb_case, tlb_last_dir, tlb_inc_base, tlb_inc_view
+  global tlb_inc_base, tlb_inc_view
   global tid_search_inc
 
   tid_search_inc = None
 
   if tk.focus_get() == wt.f2_e:
     pat = tlb_find.get()
     if (pat != "") and SearchExprCheck(pat, tlb_regexp.get(), False):
@@ -950,15 +937,15 @@
 
 #
 # This function is invoked as callback after a background search for the
 # incremental search in the entry field is completed.  (Before this call,
 # cursor position and search highlights are already updated.)
 #
 def Search_IncMatch(pos, pat, is_fwd, is_changed):
-  global tlb_inc_base, tlb_inc_view, tlb_history, tlb_hist_pos, tlb_hist_prefix
+  global tlb_hist_pos, tlb_hist_prefix
 
   if (pos == "") and (tlb_inc_base is not None):
     if is_changed:
       wt.f1_t.xview_moveto(tlb_inc_view[0])
       wt.f1_t.yview_moveto(tlb_inc_view[1])
       wt.f1_t.mark_set("insert", tlb_inc_base)
       wt.f1_t.see("insert")
@@ -981,21 +968,21 @@
 # This function checks if the search pattern syntax is valid
 #
 def SearchExprCheck(pat, is_re, display):
   if is_re:
     try:
       # Text widget uses Tcl "re_syntax" which slightly differs from Python "re"
       #re.compile(pat)
-      foo = Text(tk)
-      foo.search(pat, 1.0, regexp=True)
+      dummy_wid = Text(tk)
+      dummy_wid.search(pat, 1.0, regexp=True)
       return True
     #except re.error as e:
     except Exception as e:
       if display:
-        DisplayStatusLine("search", "error", "Syntax error in search expression: " + e.msg)
+        DisplayStatusLine("search", "error", "Syntax error in search expression: " + str(e))
       return False
   else:
     return True
 
 
 #
 # This function returns the start position for a search.  The first search
@@ -1066,16 +1053,14 @@
 
 
 #
 # This function is used by the various key bindings which repeat a
 # previous search.
 #
 def SearchNext(is_fwd):
-  global tlb_find, tlb_regexp, tlb_case, tlb_history
-
   ClearStatusLine("search")
 
   pat = tlb_find.get()
   if pat != "":
     found = Search_Atomic(pat, tlb_regexp.get(), tlb_case.get(), is_fwd, False)
     if found == "":
       Search_HandleNoMatch(pat, is_fwd)
@@ -1096,16 +1081,14 @@
 
 #
 # This function is used by the "All" or "List all" buttons and assorted
 # keyboard shortcuts to list all text lines matching the current search
 # expression in a separate dialog window.
 #
 def SearchAll(raise_win, direction):
-  global tlb_find, tlb_regexp, tlb_case, tlb_last_wid, tlb_find_focus
-
   pat = tlb_find.get()
   if pat:
     if SearchExprCheck(pat, tlb_regexp.get(), True):
       is_re = tlb_regexp.get()
       use_case = tlb_case.get()
 
       Search_AddHistory(pat, is_re, use_case)
@@ -1171,15 +1154,15 @@
 #
 # This function is called to move keyboard focus into the search entry field.
 # The focus change will trigger the "init" function.  The caller can pass a
 # widget to which focus is passed when leaving the search via the Return or
 # Escape keys.
 #
 def SearchEnter(is_fwd, wid=None):
-  global tlb_find, tlb_last_dir, tlb_last_wid
+  global tlb_last_dir, tlb_last_wid
 
   tlb_last_dir = is_fwd
   tlb_find.set("")
   wt.f2_e.focus_set()
 
   # clear "highlight all" since search pattern is reset above
   SearchHighlightClear()
@@ -1192,15 +1175,14 @@
 
 
 #
 # This function is bound to the FocusOut event in the search entry field.
 # It resets the incremental search state.
 #
 def SearchLeave():
-  global tlb_find, tlb_regexp, tlb_case, tlb_hall
   global tlb_inc_base, tlb_inc_view, tlb_find_focus, tlb_last_wid
   global tlb_hist_pos, tlb_hist_prefix
   global tid_search_inc
 
   if tid_search_inc is not None:
     tk.after_cancel(tid_search_inc)
     tid_search_inc = None
@@ -1222,48 +1204,45 @@
 
     tlb_inc_base = None
     tlb_inc_view = None
     tlb_hist_pos = None
     tlb_hist_prefix = None
 
     tlb_last_wid = None
-    tlb_find_focus = 0
+    tlb_find_focus = False
 
 
 #
 # This function is called when the search window is left via "Escape" key.
 # The search highlighting is removed and the search text is deleted.
 #
 def SearchAbort():
-  global tlb_find, tlb_regexp, tlb_case, tlb_last_wid
-
   pat = tlb_find.get()
   if SearchExprCheck(pat, tlb_regexp.get(), False):
     Search_AddHistory(pat, tlb_regexp.get(), tlb_case.get())
 
   tlb_find.set("")
   SearchReset()
   # note more clean-up is triggered via the focus-out event
   wt.f1_t.focus_set()
 
   if tlb_last_wid is not None:
-    tk.focus_set(tlb_last_wid)
+    tlb_last_wid.focus_set()
 
     top_wid = tlb_last_wid.winfo_toplevel()
     top_wid.lift()
 
 
 #
 # This function is bound to the Return key in the search entry field.
 # If the search pattern is invalid (reg.exp. syntax) an error message is
 # displayed and the focus stays in the entry field. Else, the keyboard
 # focus is switched to the main window.
 #
 def SearchReturn():
-  global tlb_find, tlb_regexp, tlb_history, tlb_last_dir, tlb_last_wid
   global tid_search_inc
 
   if tid_search_inc is not None:
     tk.after_cancel(tid_search_inc)
     tid_search_inc = None
     restart = True
   else:
@@ -1278,15 +1257,14 @@
     else:
       DisplayStatusLine("search", "error", "No pattern defined for search repetition")
 
   if SearchExprCheck(tlb_find.get(), tlb_regexp.get(), True):
     if restart:
       # incremental search not completed -> start regular search
       if SearchNext(tlb_last_dir) == "":
-        global tlb_inc_view, tlb_inc_base
         if tlb_inc_base is not None:
           wt.f1_t.xview_moveto(tlb_inc_view[0])
           wt.f1_t.yview_moveto(tlb_inc_view[1])
           wt.f1_t.mark_set("insert", tlb_inc_base)
           wt.f1_t.see("insert")
 
     # note this implicitly triggers the leave event
@@ -1300,15 +1278,15 @@
 
 #
 # This function add the given search string to the search history stack.
 # If the string is already on the stack, it's moved to the top. Note: top
 # of the stack is the front of the list.
 #
 def Search_AddHistory(txt, is_re, use_case):
-  global tlb_history, tlb_hist_maxlen
+  global tlb_history
 
   if txt != "":
     old_sel = SearchHistory_StoreSel()
 
     # search for the expression in the history (options not compared)
     idx = 0
     for hl in tlb_history:
@@ -1337,15 +1315,15 @@
 # This function is bound to the up/down cursor keys in the search entry
 # field. The function is used to iterate through the search history stack.
 # The "up" key starts with the most recently used pattern, the "down" key
 # with the oldest. When the end of the history is reached, the original
 # search string is displayed again.
 #
 def Search_BrowseHistory(is_up):
-  global tlb_find, tlb_history, tlb_hist_pos, tlb_hist_prefix
+  global tlb_hist_pos, tlb_hist_prefix
 
   if len(tlb_history) > 0:
     if tlb_hist_pos is None:
       tlb_hist_prefix = tlb_find.get()
       if is_up:
         tlb_hist_pos = 0
       else:
@@ -1375,16 +1353,14 @@
 
 
 #
 # This helper function searches the search history stack for a search
 # string with a given prefix.
 #
 def Search_HistoryComplete(step):
-  global tlb_find, tlb_hist_prefix, tlb_history, tlb_hist_pos, tlb_hist_prefix
-
   pat = tlb_find.get()
   pf_len = len(tlb_hist_prefix)
   idx = tlb_hist_pos
 
   while (idx >= 0) and (idx < len(tlb_history)):
     hl = tlb_history[idx]
     if hl[0][0:pf_len] == pat[0:pf_len]:
@@ -1396,16 +1372,14 @@
 
 #
 # This function is bound to "CTRL-d" in the "Find" entry field and
 # performs auto-completion of a search text by adding any following
 # characters in the word matched by the current expression.
 #
 def Search_Complete():
-  global tlb_find, tlb_regexp, tlb_case
-
   pos = wt.f1_t.index("insert")
   if pos != "":
     dump = ExtractText(pos, pos + " lineend")
     off = 0
 
     if tlb_regexp.get():
       if tlb_case.get():
@@ -1434,16 +1408,14 @@
 
 #
 # This function is bound to "CTRL-SHIFT-D" in the "Find" entry field and
 # performs auto-completion to the left by adding any preceding characters
 # before the current cursor position.
 #
 def Search_CompleteLeft():
-  global tlb_find, tlb_regexp
-
   pos = wt.f1_t.index("insert")
   if pos != "":
     dump = ExtractText(pos + " linestart", pos)
 
     match = re.search(r"(?:\W+|\w+)$", dump)
     if match:
       word = Search_EscapeSpecialChars(match.group(0), tlb_regexp.get())
@@ -1456,16 +1428,14 @@
 
 #
 # This function if bound to "*" and "#" in the main text window (as in VIM)
 # These keys allow to search for the word under the cursor in forward and
 # backwards direction respectively.
 #
 def SearchWord(is_fwd):
-  global tlb_find, tlb_regexp, tlb_case
-
   pos = wt.f1_t.index("insert")
   if pos != "":
     # extract word to the right starting at the cursor position
     dump = ExtractText(pos, pos + " lineend")
     match = re.match(r"^[\w\-]+", dump)
     if match:
       word = match.group(0)
@@ -1491,32 +1461,32 @@
         Search_HandleNoMatch(tlb_find.get(), is_fwd)
 
 
 #
 # This function moves the cursor onto the next occurence of the given
 # character in the current line.
 #
-def SearchCharInLine(char, dir):
+def SearchCharInLine(char, direction):
   global last_inline_char, last_inline_dir
 
   ClearStatusLine("search_inline")
   if char != "":
     last_inline_char = char
-    last_inline_dir = dir
+    last_inline_dir = direction
   else:
     if last_inline_char is not None:
       char = last_inline_char
-      dir = dir * last_inline_dir
+      direction = direction * last_inline_dir
     else:
       DisplayStatusLine("search_inline", "error", "No previous in-line character search")
       return
 
   pos = wt.f1_t.index("insert")
   if pos != "":
-    if dir > 0:
+    if direction > 0:
       dump = ExtractText(pos, pos + " lineend")
       idx = dump.find(char)
       if idx != -1:
         wt.f1_t.mark_set("insert", "insert + %s chars" % idx)
         wt.f1_t.see("insert")
       else:
         DisplayStatusLine("search_inline", "warn", "Character \"%s\" not found until line end" % char)
@@ -1545,15 +1515,15 @@
 
 
 #
 # This function is bound to "CTRL-x" in the "Find" entry field and
 # removes the current entry from the search history.
 #
 def Search_RemoveFromHistory():
-  global tlb_history, tlb_hist_pos, tlb_hist_prefix
+  global tlb_hist_pos, tlb_hist_prefix
 
   if (tlb_hist_pos is not None) and (tlb_hist_pos < len(tlb_history)):
     old_sel = SearchHistory_StoreSel()
 
     del tlb_history[tlb_hist_pos]
     UpdateRcAfterIdle()
 
@@ -1569,30 +1539,30 @@
 
 
 # ----------------------------------------------------------------------------
 #
 # This function creates a small overlay which displays a temporary status
 # message.
 #
-def DisplayStatusLine(topic, type, msg):
-  global col_bg_content, tid_status_line, status_line_topic
+def DisplayStatusLine(topic, msg_type, msg):
+  global tid_status_line, status_line_topic
 
   focus_nam = tk.focus_get()
   focus_wid = tk._nametowidget(focus_nam) if focus_nam is not None else None
   top_wid = focus_wid.winfo_toplevel() if focus_wid is not None else None
 
   if (top_wid is None):          wid = wt.f1_t
   elif (top_wid == wt.dlg_srch): wid = wt.dlg_srch_f1_l
   elif (top_wid == wt.dlg_hist): wid = wt.dlg_hist_f1_l
   elif (top_wid == wt.dlg_tags): wid = wt.dlg_tags_f1_l
   else:                          wid = wt.f1_t
 
-  if   type == "error": col = "#ff6b6b"
-  elif type == "warn":  col = "#ffcc5d"
-  else:                 col = col_bg_content
+  if   msg_type == "error": col = "#ff6b6b"
+  elif msg_type == "warn":  col = "#ffcc5d"
+  else:                     col = col_bg_content
 
   if not wt_exists(wt.stline):
     wt.stline = Frame(wid, background=col_bg_content, relief=RIDGE, borderwidth=2, takefocus=0)
 
     wt.stline_l = Label(wt.stline, text=msg, background=col, anchor=W)
     wt.stline_l.pack(side=LEFT, fill=BOTH, expand=1)
 
@@ -1625,16 +1595,14 @@
 
 #
 # This function is bound to CTRL-G in the main window. It displays the
 # current line number and fraction of lines above the cursor in percent
 # (i.e. same as VIM)
 #
 def DisplayLineNumber():
-  global cur_filename
-
   if wt.f1_t.bbox("insert") is not None:
     pos = wt.f1_t.index("insert").split(".")
     if len(pos) == 2:
       (line, char) = map(int, pos)
       (end_line, char) = map(int, wt.f1_t.index("end").split("."))
       # if the last line is properly terminated with a newline char,
       # Tk inserts an empty line below - this should not be counted
@@ -1661,16 +1629,14 @@
 # window is closed and re-opened.
 #
 # Note: this event is installed on the toplevel window, but also called for
 # all its childs when they are resized (due to the bindtag mechanism.) This
 # is the reason for passing widget and compare parameters.
 #
 def ToplevelResized(wid, top, cmp, var_id):
-  global win_geom
-
   if wid == cmp:
     new_size = top.wm_geometry()
 
     if new_size != win_geom.get(var_id):
       win_geom[var_id] = new_size
       UpdateRcAfterIdle()
 
@@ -1694,16 +1660,14 @@
 
 
 #
 # This function is bound to the Control +/- keys as a way to quickly
 # adjust the content font size (as in web browsers)
 #
 def ChangeFontSize(delta):
-  global font_content
-
   font_content.configure(size=font_content.cget("size") + delta)
 
   cerr = ApplyFont()
   if cerr is not None:
     DisplayStatusLine("font", "error", "Failed to apply the new font: " + cerr)
   else:
     ClearStatusLine("font")
@@ -1711,16 +1675,14 @@
 
 #
 # This function is called after a new fonct has been configured to apply
 # the new font in the main window, text highlight tags and dialog texts.
 # The function returns 1 on success and saves the font setting in the RC.
 #
 def ApplyFont():
-  global font_content
-
   cerr = None
   try:
     wt.f1_t.configure(font=font_content)
 
     # save to rc
     UpdateRcAfterIdle()
 
@@ -1757,16 +1719,14 @@
 
 
 #
 # This function adjusts the view so that the line holding the cursor is
 # placed at the top, center or bottom of the viewable area, if possible.
 #
 def YviewSet(wid, where, col):
-  global font_content
-
   wid.see("insert")
   pos = wid.bbox("insert")
   if pos is not None:
     fh = font_content.metrics("linespace")
     wh = wid.winfo_height()
     bbox_y = pos[1]
     bbox_h = pos[3]
@@ -1792,26 +1752,24 @@
       wid.xview_moveto(0)
       wid.mark_set("insert", "insert linestart")
       CursorMoveLine(wid, 0)
     else:
       wid.see("insert")
 
   # synchronize the search result list (if open) with the main text
-  (idx_l, idx_c) = map(int, wt.f1_t.index("insert").split("."))
+  idx_l = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
   SearchList_MatchView(idx_l)
 
 
 #
 # This function scrolls the view vertically by the given number of lines.
 # When the line holding the cursor is scrolled out of the window, the cursor
 # is placed in the last visible line in scrolling direction.
 #
 def YviewScroll(wid, delta):
-  global font_content
-
   wid.yview_scroll(delta, "units")
 
   fh = font_content.metrics("linespace")
   pos = wid.bbox("insert")
 
   # check if cursor is fully visible
   if (pos is None) or (pos[3] < fh):
@@ -1821,34 +1779,33 @@
       wid.mark_set("insert", "@1,1")
 
 
 #
 # This function scrolls the view vertically by half the screen height
 # in the given direction.
 #
-def YviewScrollHalf(wid, dir):
-  global font_content
-
+def YviewScrollHalf(wid, direction):
   wh = wid.winfo_height()
   fh = font_content.metrics("linespace")
   if fh > 0:
     wh = int((wh + fh/2) / fh)
-    YviewScroll(wid, int(wh/2 * dir))
+    YviewScroll(wid, int(wh/2 * direction))
 
 #
 # This function moves the cursor into a given line in the current view.
 #
 def CursorSetLine(wid, where, off):
   CursorJumpPushPos(wid)
 
   if where == "top":
     index = wid.index("@1,1 + %d lines" % off)
     if (off > 0) and not IsRowFullyVisible(wid, index):
       # offset out of range - set to bottom instead
-      return CursorSetLine(wid, "bottom", 0)
+      CursorSetLine(wid, "bottom", 0)
+      return
     else:
       wid.mark_set("insert", index)
 
   elif where == "center":
     # note the offset parameter is not applicable in this case
     wid.mark_set("insert", "@1,%d" % (wid.winfo_height() // 2))
 
@@ -1856,15 +1813,16 @@
     index = wid.index("@1,%d linestart - %d lines" % (wid.winfo_height(), off))
     if not IsRowFullyVisible(wid, index):
       if off == 0:
         # move cursor to the last fully visible line to avoid scrolling
         index = wid.index(index + " - 1 lines")
       else:
         # offset out of range - set to top instead
-        return CursorSetLine(wid, "top", 0)
+        CursorSetLine(wid, "top", 0)
+        return
 
     wid.mark_set("insert", index)
   else:
     wid.mark_set("insert", "insert linestart")
 
   # place cursor on first non-blank character in the selected row
   CursorMoveLine(wid, 0)
@@ -1935,47 +1893,47 @@
 
 
 #
 # This function scrolls the view horizontally by the given number of characters.
 # When the cursor is scrolled out of the window, it's placed in the last visible
 # column in scrolling direction.
 #
-def XviewScroll(wid, how, delta, dir):
+def XviewScroll(wid, how, delta, direction):
   pos_old = wid.bbox("insert")
 
   if how == "scroll":
-    wid.xview_scroll(dir * delta, "units")
+    wid.xview_scroll(direction * delta, "units")
   else:
     wid.xview_moveto(delta)
 
   if pos_old is not None:
     # check if cursor is fully visible
     pos_new = wid.bbox("insert")
     if (pos_new is None) or (pos_new[2] == 0):
       ycoo = pos_old[1] + pos_old[3] // 2
-      if dir < 0:
+      if direction < 0:
         wid.mark_set("insert", "@%d,%d" % (wid.winfo_width(), ycoo))
       else:
         wid.mark_set("insert", "@1,%d + 1 chars" % ycoo)
 
 
 #
 # This function scrolls the view horizontally by half the screen width
 # in the given direction.
 #
-def XviewScrollHalf(wid, dir):
+def XviewScrollHalf(wid, direction):
   xpos = wid.xview()
   w = wid.winfo_width()
   if w != 0:
     fract_visible = xpos[1] - xpos[0]
-    off = xpos[0] + dir * (0.5 * fract_visible)
+    off = xpos[0] + direction * (0.5 * fract_visible)
     if off > 1:  off = 1
     if off < 0:  off = 0
 
-  XviewScroll(wid, "moveto", off, dir)
+  XviewScroll(wid, "moveto", off, direction)
 
 
 #
 # This function adjusts the view so that the column holding the cursor is
 # placed at the left or right of the viewable area, if possible.
 #
 def XviewSet(wid, where):
@@ -1983,19 +1941,17 @@
   coo = wid.bbox("insert")
   w = wid.winfo_width()
   if (coo is not None) and (w != 0):
     fract_visible = xpos[1] - xpos[0]
     fract_insert = (2 + coo[0] + coo[2]) / w
 
     if where == "left":
-      off = xpos[0] + (fract_insert * fract_visible)
-      if off > 1.0: off = 1.0
+      off = min(xpos[0] + (fract_insert * fract_visible), 1.0)
     else:
-      off = xpos[0] - ((1 - fract_insert) * fract_visible)
-      if off < 0.0: off = 0.0
+      off = max(xpos[0] - ((1 - fract_insert) * fract_visible), 0.0)
 
     wid.xview_moveto(off)
     wid.see("insert")
 
 
 #
 # This function moves the cursor into a given column in the current view.
@@ -2021,89 +1977,84 @@
 def CursorMoveWord(is_fwd, spc_only, to_end):
   pos = wt.f1_t.index("insert")
   if pos != "":
     if is_fwd:
       dump = ExtractText(pos, pos + " lineend")
       if spc_only:
         if to_end:
-          match = re.match("^\s*\S*", dump)
+          match = re.match(r"^\s*\S*", dump)
         else:
-          match = re.match("^\S*\s*", dump)
+          match = re.match(r"^\S*\s*", dump)
       else:
         if to_end:
-          match = re.match("^\W*\w*", dump)
+          match = re.match(r"^\W*\w*", dump)
         else:
-          match = re.match("^\w*\W*", dump)
+          match = re.match(r"^\w*\W*", dump)
 
       if match and ((len(match.group(0)) < len(dump)) or to_end):
         wt.f1_t.mark_set("insert", "insert + %d chars" % len(match.group(0)))
       else:
         wt.f1_t.mark_set("insert", "insert linestart + 1 lines")
 
     else:
       dump = ExtractText(pos + " linestart", pos)
       if spc_only:
         if to_end:
-          match = re.search("\s(\s+)$", dump)
+          match = re.search(r"\s(\s+)$", dump)
         else:
-          match = re.search("(\S+\s*)$", dump)
+          match = re.search(r"(\S+\s*)$", dump)
       else:
         if to_end:
-          match = re.search("\w(\W+\w*)$", dump)
+          match = re.search(r"\w(\W+\w*)$", dump)
         else:
-          match = re.search("(\w+|\w+\W+)$", dump)
+          match = re.search(r"(\w+|\w+\W+)$", dump)
 
       if match:
         wt.f1_t.mark_set("insert", "insert - %d chars" % len(match.group(1)))
       else:
         wt.f1_t.mark_set("insert", "insert - 1 lines lineend")
 
     wt.f1_t.see("insert")
 
 
 #
 # Helper function which determines if the text at the given index in
 # the given window is fully visible.
 #
 def IsRowFullyVisible(wid, index):
-  global font_content
-
   fh = font_content.metrics("linespace")
-  bbox = wid.bbox("insert")
+  bbox = wid.bbox(index)
 
-  if (bbox is None) or (bbox[3] < fh):
-    return 0
-  else:
-    return 1
+  return bbox and (bbox[3] >= fh)
 
 
 #
 # Helper function to extrace a range of characters from the content.
 #
 def ExtractText(pos1, pos2):
   dump = []
-  for (key, val, idx) in wt.f1_t.dump(pos1, pos2, text=1):
+  for (key, val, _) in wt.f1_t.dump(pos1, pos2, text=1):
     if key == "text":
       dump.append(val)
 
   return ''.join(dump)
 
 
 #
 # This function is called by all key bindings which make a large jump to
 # push the current cusor position onto the jump stack. Both row and column
 # are stored.  If the position is already on the stack, this entry is
 # deleted (note for this comparison only the line number is considered.)
 #
 def CursorJumpPushPos(wid):
-  global cur_jump_stack, cur_jump_idx
+  global cur_jump_idx
 
   if wid == wt.f1_t:
     cur_pos = wt.f1_t.index("insert")
-    line = int(cur_pos.split(".")[0])
+    line = int(cur_pos.split(".", maxsplit=1)[0])
     # remove the line if already on the stack
     idx = 0
     for pos in cur_jump_stack:
       prev_line = int(pos.split(".")[0])
       if prev_line == line:
         del cur_jump_stack[idx]
         break
@@ -2121,15 +2072,15 @@
 #
 # This function is bound to command "''" (i.e. two apostrophes) in the main
 # window. The command makes the cursor jump back to the origin of the last
 # jump (NOT to the target of the last jump, which may be confusing.) The
 # current position is pushed to the jump stack, if not already on the stack.
 #
 def CursorJumpToggle(wid):
-  global cur_jump_stack, cur_jump_idx
+  global cur_jump_idx
 
   if len(cur_jump_stack) > 0:
     ClearStatusLine("keycmd")
 
     # push current position to the stack
     CursorJumpPushPos(wid)
 
@@ -2154,15 +2105,15 @@
 #
 # This function is bound to the CTRL-O and CTRL-I commands in the main
 # window. The function traverses backwards or forwards respectively
 # through the jump stack. During the first call the current cursor
 # position is pushed to the stack.
 #
 def CursorJumpHistory(wid, rel):
-  global cur_jump_stack, cur_jump_idx
+  global cur_jump_idx
 
   ClearStatusLine("keycmd")
   if len(cur_jump_stack) > 0:
     if cur_jump_idx < 0:
       # push current position to the stack
       CursorJumpPushPos(wid)
       if (rel < 0) and (len(cur_jump_stack) >= 2):
@@ -2212,17 +2163,18 @@
 # complex key sequences, but also has to handle single key bindings for
 # keys which can be part of sequences (e.g. "b" due to "zb")
 #
 def KeyCmd(wid, char):
   global last_key_char
 
   reg = key_cmd_reg.get(wid)
-  if reg is None: return
+  if reg is None:
+      return False
 
-  result = 0
+  result = False
   if char != "":
     if last_key_char == "'":
       # single quote char: jump to marker or bookmark
       ClearStatusLine("keycmd")
       if char == "'":
         CursorJumpToggle(wid)
       elif char == "^":
@@ -2234,68 +2186,68 @@
         Mark_JumpNext(True)
       elif char == "-":
         Mark_JumpNext(False)
       else:
         DisplayStatusLine("keycmd", "error", "Undefined key sequence \"'%s\"" % char)
 
       last_key_char = ""
-      result = 1
+      result = True
 
     elif (last_key_char == "z") or (last_key_char == "g"):
       ClearStatusLine("keycmd")
       char = last_key_char + char
       cb = reg.get(char)
       if cb is not None:
         cb()
       else:
         DisplayStatusLine("keycmd", "error", "Undefined key sequence \"%s\"" % char)
 
       last_key_char = ""
-      result = 1
+      result = True
 
     elif last_key_char == "f":
       SearchCharInLine(char, 1)
       last_key_char = ""
-      result = 1
+      result = True
 
     elif last_key_char == "F":
       SearchCharInLine(char, -1)
       last_key_char = ""
-      result = 1
+      result = True
 
     else:
       last_key_char = ""
 
       cb = reg.get(char)
       if cb is not None:
         cb()
 
       elif "1" <= char <= "9":
         KeyCmd_OpenDialog("any", char)
         last_key_char = ""
-        result = 1
+        result = True
 
       elif char in "z'fFg":
         last_key_char = char
-        result = 1
+        result = True
 
-  # return 1 if the key was consumed, else 0
+  # return True if the key was consumed, else False
   return result
 
 
 #
 # This function is called for all explicit key bindings to forget about
 # any previously buffered partial multi-keypress commands.
 #
 def KeyClr():
   global last_key_char
   last_key_char = ""
 
-def KeyHomeEnd(wid, dir):
-  CursorSetColumn(wid, dir)
+def KeyHomeEnd(wid, direction):
+  CursorSetColumn(wid, direction)
   KeyClr()
 
 #
 # This function adds key bindings for scrolling vertically
 # to the given text widget.
 #
 def KeyBinding_UpDown(wid):
@@ -2349,46 +2301,46 @@
 
 # ----------------------------------------------------------------------------
 #
 # This function opens a tiny "overlay" dialog which allows to enter a line
 # number.  The dialog is placed into the upper left corner of the text
 # widget in the main window.
 #
-def KeyCmd_OpenDialog(type, txt=""):
+def KeyCmd_OpenDialog(dlg_type, txt=""):
   global keycmd_ent
 
   PreemptBgTasks()
   if not wt_exists(wt.dlg_key_e):
     wt.dlg_key = Frame(wt.f1_t, borderwidth=2, relief=RAISED)
 
-    if type == "goto":
+    if dlg_type == "goto":
       cmd_text = "Goto line:"
     else:
       cmd_text = "Command:"
 
     keycmd_ent = StringVar(tk, txt)
 
     wt.dlg_key_l = Label(wt.dlg_key, text=cmd_text)
     wt.dlg_key_l.pack(side=LEFT, padx=5)
     wt.dlg_key_e = Entry(wt.dlg_key, width=12, textvariable=keycmd_ent, exportselection=0)
     wt.dlg_key_e.pack(side=LEFT, padx=5)
 
-    if type == "goto":
+    if dlg_type == "goto":
       wt.dlg_key_e.bind("<Return>", lambda e: BindCallAndBreak(KeyCmd_ExecGoto))
     else:
       # line goto key binding
       wt.dlg_key_e.bind("<Key-g>", lambda e: BindCallAndBreak(KeyCmd_ExecGoto))
       wt.dlg_key_e.bind("<Shift-Key-G>", lambda e: BindCallAndBreak(KeyCmd_ExecGoto))
       # vertical cursor movement binding
-      wt.dlg_key_e.bind("<Key-minus>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(0)))
-      wt.dlg_key_e.bind("<Key-plus>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(1)))
-      wt.dlg_key_e.bind("<Return>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(1)))
-      wt.dlg_key_e.bind("<Key-bar>", lambda e: KeyCmd_ExecAbsColumn)
-      wt.dlg_key_e.bind("<Key-k>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(0)))
-      wt.dlg_key_e.bind("<Key-j>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(1)))
+      wt.dlg_key_e.bind("<Key-minus>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(False)))
+      wt.dlg_key_e.bind("<Key-plus>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(True)))
+      wt.dlg_key_e.bind("<Return>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(True)))
+      wt.dlg_key_e.bind("<Key-bar>", lambda e: KeyCmd_ExecAbsColumn()) # pipe character
+      wt.dlg_key_e.bind("<Key-k>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(False)))
+      wt.dlg_key_e.bind("<Key-j>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorUpDown(True)))
       wt.dlg_key_e.bind("<Key-H>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorVertSet("top")))
       wt.dlg_key_e.bind("<Key-M>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorVertSet("center")))
       wt.dlg_key_e.bind("<Key-L>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorVertSet("bottom")))
       # horizontal/in-line cursor movement binding
       wt.dlg_key_e.bind("<Key-w>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-w>")))
       wt.dlg_key_e.bind("<Key-e>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-e>")))
       wt.dlg_key_e.bind("<Key-b>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-b>")))
@@ -2398,63 +2350,70 @@
       wt.dlg_key_e.bind("<Key-colon>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-colon>")))
       wt.dlg_key_e.bind("<Key-semicolon>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-semicolon>")))
       wt.dlg_key_e.bind("<Key-space>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-space>")))
       wt.dlg_key_e.bind("<Key-BackSpace>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-BackSpace>")))
       wt.dlg_key_e.bind("<Key-h>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-h>")))
       wt.dlg_key_e.bind("<Key-l>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecCursorMove("<Key-l>")))
       # search key binding
-      wt.dlg_key_e.bind("<Key-n>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecSearch(1)))
-      wt.dlg_key_e.bind("<Key-p>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecSearch(0)))
-      wt.dlg_key_e.bind("<Shift-Key-N>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecSearch(0)))
+      wt.dlg_key_e.bind("<Key-n>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecSearch(True)))
+      wt.dlg_key_e.bind("<Key-p>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecSearch(False)))
+      wt.dlg_key_e.bind("<Shift-Key-N>", lambda e: BindCallAndBreak(lambda:KeyCmd_ExecSearch(False)))
       # catch-all
-      wt.dlg_key_e.bind("<KeyPress>", lambda e: KeyCmd_KeyPress(e))
+      wt.dlg_key_e.bind("<KeyPress>", KeyCmd_KeyPress)
 
     wt.dlg_key_e.bind("<Escape>", lambda e: BindCallAndBreak(KeyCmd_Leave))
     wt.dlg_key_e.bind("<Leave>", lambda e: BindCallAndBreak(KeyCmd_Leave))
     wt.dlg_key_e.bind("<FocusOut>", lambda e: BindCallAndBreak(KeyCmd_Leave))
     wt.dlg_key.bind("<Leave>", lambda e: wt.dlg_key.destroy())
     wt.dlg_key_e.icursor("end")
 
     wt.dlg_key.place(anchor=NW, x=0, y=0) #in=wt.f1_t
     wt.dlg_key_e.focus_set()
 
   ResumeBgTasks()
 
+
+#
+# This handler is bound to any key press in the "Key" dialog overlay window.
+# The handler is invoked only, if no more specific handler did match previously
+# (or the handler did not invoked "break"). The handler serves as a catch-all
+# to block unwanted characters to be entered.
+#
 def KeyCmd_KeyPress(ev):
   if ev.char == "|":
     # work-around: keysym <Key-bar> doesn't work on German keyboard
     KeyCmd_ExecAbsColumn()
     return "break"
-  elif not ev.char.isdigit() and re.match(r'[\x21-\x7e]\s', ev.char): # [[:graph:]][[:space:]]
+  elif not ev.char.isdigit() and re.match(r'[\x21-\x7e\s\n]', ev.char): # [[:graph:][:space:]]
+    print("XXX break")
     return "break"
   else:
     return None
 
 
 #
 # This function is bound to all events which signal an exit of the goto
 # dialog window. The window is destroyed.
 #
 def KeyCmd_Leave():
+  # pylint: disable=W0602  # false positive: "del" requires "global"
   global keycmd_ent
 
   wt.f1_t.focus_set()
   wt.dlg_key.destroy()
   del keycmd_ent
 
 
 #
 # This function scrolls the text in the main window to the line number
 # entered in the "goto line" dialog window and closes the dialog. Line
 # numbers start with 1. If the line numbers is negative, -1 refers to
 # the last line.
 #
 def KeyCmd_ExecGoto():
-  global keycmd_ent
-
   # check if the content is a valid line number
   val = 0
   try:
     val = int(keycmd_ent.get())
   except:
     DisplayStatusLine("keycmd", "error", "Input is not a valid line number: \"%s\"" % keycmd_ent.get())
     return
@@ -2465,16 +2424,14 @@
   KeyCmd_Leave()
 
 
 #
 # This function moves the cursor up or down by a given number of lines.
 #
 def KeyCmd_ExecCursorUpDown(is_fwd):
-  global keycmd_ent
-
   # check if the content is a valid line number
   val = 0
   try:
     val = int(keycmd_ent.get())
   except:
     DisplayStatusLine("keycmd", "error", "Cursor movement commands require numeric input.")
     return
@@ -2491,16 +2448,14 @@
 
 
 #
 # This function sets the cursor into a given row, relative to top, or bottom.
 # Placement into the middle is also supported, but without offset.
 #
 def KeyCmd_ExecCursorVertSet(where):
-  global keycmd_ent
-
   # check if the content is a valid line number
   val = 0
   try:
     val = int(keycmd_ent.get())
   except:
     DisplayStatusLine("keycmd", "error", "Cursor movement commands require numeric input.")
     return
@@ -2510,43 +2465,38 @@
   KeyCmd_Leave()
 
 
 #
 # This function sets the cursor into a given column
 #
 def KeyCmd_ExecAbsColumn():
-  global keycmd_ent
-
   # check if the content is a valid line number
   val = 0
   try:
     val = int(keycmd_ent.get())
   except:
     DisplayStatusLine("keycmd", "error", "Cursor column placement requires numeric input.")
     return
 
   ClearStatusLine("keycmd")
   # prevent running beyond the end of the line
-  (max_line, max_col) = map(int, wt.f1_t.index("insert lineend").split("."))
+  max_col = int(wt.f1_t.index("insert lineend").split(".")[1])
   if val < max_col:
     wt.f1_t.mark_set("insert", "insert linestart + %d chars" % val)
   else:
     wt.f1_t.mark_set("insert", "insert lineend")
 
   wt.f1_t.see("insert")
   KeyCmd_Leave()
 
 
 #
 # This function starts a search from within the command popup window.
 #
 def KeyCmd_ExecSearch(is_fwd):
-  global tlb_history, tlb_find, tlb_regexp, tlb_case
-  global keycmd_ent
-
   # check if the content is a repeat count
   val = 0
   try:
     val = int(keycmd_ent.get())
   except:
     DisplayStatusLine("keycmd", "error", "Search repetition requires a numeric value as input.")
     return
@@ -2559,70 +2509,66 @@
     # empty expression: repeat last search
     if len(tlb_history) > 0:
       hl = tlb_history[0]
       tlb_find.set(hl[0])
 
   if tlb_find.get() != "":
     count = 0
-    for idx in range(val):
+    for _ in range(val):
       found = Search_Atomic(tlb_find.get(), tlb_regexp.get(), tlb_case.get(), is_fwd, False)
       if found == "":
         limit = "end" if is_fwd else "start"
         if count == 0:
-          DisplayStatusLine("search", "warn", "No match until %d of file: %s" % (limit, tlb_find.get()))
+          DisplayStatusLine("search", "warn", "No match until %s of file: %s" % (limit, tlb_find.get()))
         else:
           DisplayStatusLine("search", "warn",
-                            "Only %d of %d matches until %d of file" % (count, val, limit))
+                            "Only %d of %d matches until %s of file" % (count, val, limit))
       count += 1
   else:
     DisplayStatusLine("search", "error", "No pattern defined for search repetition")
 
 
 #
 # This function moves the cursor as if the given key had been pressed
 # the number of times specified in the number entry field.
 #
 def KeyCmd_ExecCursorMove(key):
-  global keycmd_ent
-
   # check if the content is a repeat count
   val = 0
   try:
     val = int(keycmd_ent.get())
   except:
     DisplayStatusLine("keycmd", "error", "Cursor movement commands require numeric input.")
     return
 
   if val < 10000:
     ClearStatusLine("keycmd")
     KeyCmd_Leave()
-    for idx in range(val):
+    for _ in range(val):
       wt.f1_t.event_generate(key)
   else:
     DisplayStatusLine("keycmd", "error", "Repetition value too large: %d" % val)
 
 
 
 # ----------------------------------------------------------------------------
 #
 # This function retrieves the "frame number" (timestamp) to which a given line
 # of text belongs via pattern matching. Two methods for retrieving the number
 # can be used, depending on which patterns are defined.
 #
 def ParseFrameTickNo(pos, fn_cache=None):
-  global tick_pat_sep, tick_pat_num, tick_str_prefix
-
   # query the cache before parsing for the frame number
   if fn_cache is not None:
     if fn_cache.get(pos) is not None:
       # FN of this line is already known
       return fn_cache[pos]
     elif fn_cache.get(-1):
       prev_rslt = fn_cache[-1]
-      line = int(wt.f1_t.index(pos).split(".")[0])
+      line = int(wt.f1_t.index(pos).split(".", maxsplit=1)[0])
       if (line >= prev_rslt[0]) and (line < prev_rslt[1]):
         # line is within the range of the most recently parsed frame
         fn_cache[pos] = prev_rslt[2:4]
         return fn_cache[pos]
 
   # catch Reg-Exp exceptions because patterns are supplied by user
   try:
@@ -2656,16 +2602,16 @@
 
       prefix = [fn, tick_no]
 
       if fn_cache is not None:
         # add result to the cache
         fn_cache[pos] = prefix
         # add a special entry to the cache remembering the extent of the current frame
-        line1 = int(wt.f1_t.index(pos1).split(".")[0])
-        line2 = int(wt.f1_t.index(pos2).split(".")[0])
+        line1 = int(wt.f1_t.index(pos1).split(".", maxsplit=1)[0])
+        line2 = int(wt.f1_t.index(pos2).split(".", maxsplit=1)[0])
         fn_cache[-1] = [line1, line2, fn, tick_no]
 
     elif tick_pat_num != "":
       # determine frame number by searching backwards for the line holding the FN
       match_len = IntVar(tk, 0)
       prefix = []
       pos3 = wt.f1_t.search(tick_pat_num, pos + " lineend", "1.0", regexp=1, backwards=1, count=match_len)
@@ -2680,28 +2626,27 @@
 
     else:
       # FN parsing is disabled: omit the prefix
       prefix = []
 
   except re.error as e:
     print("Warning: tick pattern match error: " + e.msg, file=sys.stderr)
-  except IndexError as e:
+  except IndexError:
     print("Warning: tick pattern contains no capture", file=sys.stderr)
 
   return prefix
 
 
 #
 # This function adds or removes a bookmark at the given text line.
 # The line is marked by inserting an image in the text and the bookmark
 # is added to the bookmark list dialog, if it's currently open.
 #
 def Mark_Toggle(line, txt=""):
-  global img_marker, mark_list, mark_list_modified
-  global tick_str_prefix
+  global mark_list_modified
 
   if mark_list.get(line) is None:
     if txt == "":
       fn_prefix = ParseFrameTickNo("insert")
       txt = ExtractText("%d.0" % line, "%d.0 lineend" % line).strip()
       mark_list[line] = tick_str_prefix + " ".join(str(x) for x in fn_prefix) + " " + txt
     else:
@@ -2729,15 +2674,15 @@
 #
 # This function adds or removes a bookmark at the current cursor position.
 # The function is used to set bookmarks via key bindings.
 #
 def Mark_ToggleAtInsert():
   pos = wt.f1_t.index("insert")
   if pos != "":
-    line = int(pos.split(".")[0])
+    line = int(pos.split(".", maxsplit=1)[0])
     Mark_Toggle(line)
 
 
 #
 # This function moves the cursor into the given line and highlights the entire
 # line. The "line" parameter is a text widget line number, starting at 1.
 #
@@ -2756,20 +2701,18 @@
 
 
 #
 # This function moves the cursor onto the next bookmark in the given
 # direction.
 #
 def Mark_JumpNext(is_fwd):
-  global mark_list
-
   pos = wt.f1_t.index("insert")
   if pos != "":
     goto = None
-    line = int(pos.split(".")[0])
+    line = int(pos.split(".", maxsplit=1)[0])
     if is_fwd:
       for mark_line in sorted(mark_list.keys()):
         if mark_line > line:
           goto = mark_line
           break
 
     else:
@@ -2795,15 +2738,15 @@
 
 #
 # This function deletes all bookmarks. It's called via the main menu.
 # The function is intended esp. if a large number of bookmarks was imported
 # previously from a file.
 #
 def Mark_DeleteAll():
-  global mark_list, mark_list_modified
+  global mark_list_modified
 
   count = len(mark_list)
   if count > 0:
     pls = "" if (count == 1) else "s"
     msg = "Really delete %d bookmark%s?" % (count, pls)
     answer = messagebox.askokcancel(parent=tk, message=msg)
     if answer:
@@ -2817,15 +2760,15 @@
 
 #
 # This function reads a list of line numbers and tags from a file and
 # adds them to the bookmark list. (Note already existing bookmarks are
 # not discarded, hence there's no warning when bookmarks already exist.)
 #
 def Mark_ReadFile(filename):
-  global mark_list, mark_list_modified
+  global mark_list_modified
 
   bol = []
   line_num = 0
   try:
     with open(filename, "r") as f:
       for line in f.readlines():
         line_num += 1
@@ -2848,16 +2791,15 @@
 
   except OSError as e:
     messagebox.showerror(parent=tk, message="Failed to read bookmarks file %s: %s" % (filename, e.strerror))
 
   if line_num >= 0:
     modif = mark_list_modified or (len(mark_list) != 0)
 
-    pos = wt.f1_t.index("end")
-    max_line = int(wt.f1_t.index("end").split(".")[0])
+    max_line = int(wt.f1_t.index("end").split(".", maxsplit=1)[0])
     warned = False
 
     for (line, txt) in bol:
       if (line < 0) or (line > max_line):
         if not warned:
           warned = True
           msg = "Invalid line number %d in bookmarks file \"%s\" (should be in range 0...%d)" % (line, filename, max_line)
@@ -2874,15 +2816,15 @@
     MarkList_Fill()
 
 
 #
 # This function stores the bookmark list in a file.
 #
 def Mark_SaveFile(filename):
-  global mark_list, mark_list_modified
+  global mark_list_modified
 
   try:
     with open(filename, "w") as f:
       try:
         for line in sorted(mark_list.keys()):
           print("%d %s" % (line, mark_list[line]), file=f)
 
@@ -2895,16 +2837,14 @@
 
 
 #
 # This function is called by menu entry "Read bookmarks from file"
 # The user is asked to select a file; if he does so it's content is read.
 #
 def Mark_ReadFileFrom():
-  global cur_filename
-
   def_name = Mark_DefaultFile(cur_filename)
   if not os.path.isfile(def_name):
     def_name = ""
 
   filename = filedialog.askopenfilename(parent=tk, filetypes=(("Bookmarks", "*.bok"), ("all", "*")),
                                         title="Select bookmark file",
                                         initialfile=os.path.basename(def_name),
@@ -2915,16 +2855,14 @@
 
 #
 # This function automatically reads a previously stored bookmark list
 # for a newly loaded file, if the bookmark file is named by the default
 # naming convention, i.e. with ".bok" extension.
 #
 def Mark_ReadFileAuto():
-  global cur_filename
-
   bok_name = Mark_DefaultFile(cur_filename)
   if bok_name != "":
     Mark_ReadFile(bok_name)
 
 
 #
 # This helper function determines the default filename for reading bookmarks.
@@ -2963,16 +2901,14 @@
 
 
 #
 # This function is called by menu entry "Save bookmarks to file".
 # The user is asked to select a file; if he does so the bookmarks are written to it.
 #
 def Mark_SaveFileAs():
-  global mark_list, cur_filename
-
   if len(mark_list) > 0:
     if cur_filename != "":
       def_name = cur_filename + ".bok"
     else:
       def_name = ""
 
     filename = filedialog.asksaveasfilename(parent=tk, filetypes=(("Bookmarks", "*.bok"), ("all", "*")),
@@ -2988,34 +2924,33 @@
 
 #
 # This function offers to store the bookmark list into a file if the list was
 # modified.  The function is called when the application is closed or a new file
 # is loaded.
 #
 def Mark_OfferSave():
-  global mark_list, mark_list_modified
-
   if mark_list_modified and (len(mark_list) > 0):
-    answer = messagebox.askyesno(parent=tk, default="yes", title="Trace browser",
-                                 message="Store changes in the bookmark list before quitting?")
+    answer = messagebox.askyesnocancel(parent=tk, default="yes", title="Trace browser",
+                                       message="Store changes in the bookmark list before quitting?")
+    if answer is None:
+        return False
     if answer:
       Mark_SaveFileAs()
       if mark_list_modified == 0:
         DisplayStatusLine("bookmark", "info", "Bookmarks have been saved")
+  return True
 
 
 # ----------------------------------------------------------------------------
 #
 # This function inserts a bookmark text into the listbox and copies
 # color highlight tags from the main window so that the text displays
 # in the same way.
 #
 def MarkList_Insert(idx, line):
-  global patlist, mark_list
-
   tag_list = []
   for tag in wt.f1_t.tag_names("%d.1" % line):
     if re.match(r"^tag\d+$", tag):
       tag_list.append(tag)
 
   txt = mark_list[line] + "\n"
 
@@ -3023,15 +2958,15 @@
   wt.dlg_mark_l.insert("%d.0" % (idx + 1), "  ", "margin", txt, tag_list)
 
 
 #
 # This function fills the bookmark list dialog window with all bookmarks.
 #
 def MarkList_Fill():
-  global dlg_mark_shown, dlg_mark_list, mark_list
+  global dlg_mark_list
 
   if dlg_mark_shown:
     wt.dlg_mark_l.delete("1.0", "end")
     dlg_mark_list = []
 
     idx = 0
     for line in sorted(mark_list.keys()):
@@ -3041,16 +2976,14 @@
 
 
 #
 # This function is called after a bookmark was added to insert the text
 # into the bookmark list dialog window.
 #
 def MarkList_Add(line):
-  global dlg_mark_shown, mark_list, dlg_mark_list, dlg_mark_sel
-
   if dlg_mark_shown:
     idx = 0
     for l in dlg_mark_list:
       if l > line:
         break
       idx += 1
 
@@ -3061,16 +2994,14 @@
 
 
 #
 # This function is called after a bookmark was deleted to remove the text
 # from the bookmark list dialog window.
 #
 def MarkList_Delete(line):
-  global dlg_mark_shown, mark_list, dlg_mark_list, dlg_mark_sel
-
   if dlg_mark_shown:
     try:
       idx = dlg_mark_list.index(line)
       del dlg_mark_list[idx]
       wt.dlg_mark_l.delete("%d.0" % (idx + 1), "%d.0" % (idx + 2))
       dlg_mark_sel.TextSel_SetSelection([])
     except:
@@ -3078,16 +3009,14 @@
 
 
 #
 # This function is bound to the "delete" key and context menu entry to
 # allow the user to remove a bookmark via the bookmark list dialog.
 #
 def MarkList_RemoveSelected():
-  global dlg_mark_list, dlg_mark_sel
-
   sel = dlg_mark_sel.TextSel_GetSelection()
 
   # translate list indices to text lines, because indices change during removal
   line_list = [dlg_mark_list[idx] for idx in sel]
 
   # remove bookmarks on all selected lines
   for line in line_list:
@@ -3096,30 +3025,26 @@
 
 #
 # This function is bound to the "insert" key and "rename" context menu
 # entry to allow the user to edit the tag assigned to the selected bookmark.
 # The function opens an "overlay" window with an entry field.
 #
 def MarkList_RenameSelected():
-  global dlg_mark_sel
-
   sel = dlg_mark_sel.TextSel_GetSelection()
   if len(sel) == 1:
     MarkList_OpenRename(sel[0])
 
 
 #
 # This function is bound to changes of the selection in the bookmark list,
 # i.e. it's called when the user uses the cursor keys or mouse button to
 # select an entry.  The view in the main window is set to display the line
 # which contains the bookmark. If more than one bookmark nothing is done.
 #
 def MarkList_SelectionChange(sel):
-  global dlg_mark_list
-
   if len(sel) >= 1:
     line = dlg_mark_list[sel[0]]
     Mark_Line(line)
     SearchList_MatchView(line)
 
   if len(sel) > 1:
     for idx in sel[1:]:
@@ -3128,15 +3053,14 @@
 
 
 #
 # This callback is used by the selection "library" to query the number of
 # elements in the list to determine the possible selection range.
 #
 def MarkList_GetLen():
-  global dlg_mark_list
   return len(dlg_mark_list)
 
 
 #
 # This function must be called when portions of the text in the main window
 # have been deleted to update references to text lines. Parameter meaning:
 # + top_l: this is the first line which is not deleted, or 1 if none
@@ -3156,15 +3080,15 @@
 
 #
 # This function assigns the given text to a bookmark with the given index
 # in the bookmark list dialog.  The function is called when the user has
 # closed the bookmark text entry dialog with "Return"
 #
 def MarkList_Rename(idx, txt):
-  global dlg_mark_shown, dlg_mark_list, dlg_mark_sel, mark_list, mark_list_modified
+  global mark_list_modified
 
   if dlg_mark_shown and (idx < len(dlg_mark_list)):
     line = dlg_mark_list[idx]
     if txt != "":
       mark_list[line] = txt
       mark_list_modified = True
 
@@ -3174,16 +3098,14 @@
       dlg_mark_sel.TextSel_SetSelection([idx])
 
 
 #
 # This function pops up a context menu for the bookmark list dialog.
 #
 def MarkList_ContextMenu(xcoo, ycoo):
-  global dlg_mark_list, dlg_mark_sel
-
   dlg_mark_sel.TextSel_ContextSelection(xcoo, ycoo)
 
   sel = dlg_mark_sel.TextSel_GetSelection()
   if len(sel) > 0:
     wt.dlg_mark_ctxmen.delete(0, "end")
     if len(sel) == 1:
       wt.dlg_mark_ctxmen.add_command(label="Rename marker", command=lambda sel=sel:MarkList_OpenRename(sel[0]))
@@ -3196,16 +3118,15 @@
 
 
 #
 # This function creates or raises the bookmark list dialog. This dialog shows
 # all currently defined bookmarks.
 #
 def MarkList_OpenDialog():
-  global font_content, col_bg_content, col_fg_content
-  global cur_filename, dlg_mark_shown, dlg_mark_sel, dlg_mark_geom
+  global dlg_mark_shown, dlg_mark_sel
 
   PreemptBgTasks()
   if not dlg_mark_shown:
     wt.dlg_mark = Toplevel(tk)
     if cur_filename != "":
       wt.dlg_mark.wm_title("Bookmark list - " + cur_filename)
     else:
@@ -3230,17 +3151,17 @@
     wt.dlg_mark_l.bind("<Insert>", lambda e:BindCallAndBreak(MarkList_RenameSelected))
     wt.dlg_mark_l.bind("<Delete>", lambda e:BindCallAndBreak(MarkList_RemoveSelected))
     wt.dlg_mark_l.bind("<Escape>", lambda e:BindCallAndBreak(wt.dlg_mark.destroy))
     wt.dlg_mark_l.bind("<ButtonRelease-3>", lambda e: MarkList_ContextMenu(e.x, e.y))
     wt.dlg_mark_l.focus_set()
 
     dlg_mark_shown = True
-    wt.dlg_mark_l.bind("<Destroy>", lambda e:MarkList_Quit(1), add="+")
+    wt.dlg_mark_l.bind("<Destroy>", lambda e:MarkList_Quit(True), add="+")
     wt.dlg_mark.bind("<Configure>", lambda e:ToplevelResized(e.widget, wt.dlg_mark, wt.dlg_mark, "dlg_mark"))
-    wt.dlg_mark.wm_protocol("WM_DELETE_WINDOW", lambda: MarkList_Quit(0))
+    wt.dlg_mark.wm_protocol("WM_DELETE_WINDOW", lambda: MarkList_Quit(False))
     wt.dlg_mark.wm_geometry(win_geom["dlg_mark"])
     wt.dlg_mark.wm_positionfrom("user")
 
     MarkList_CreateHighlightTags()
     MarkList_Fill()
 
   else:
@@ -3252,16 +3173,14 @@
 
 
 #
 # This function creates the tags for selection and color highlighting.
 # This is used for initialisation and after editing highlight tags.
 #
 def MarkList_CreateHighlightTags():
-  global dlg_mark_shown, patlist, fmt_selection
-
   if dlg_mark_shown:
     for w in patlist:
       tagnam = w[4]
       HighlightConfigure(wt.dlg_mark_l, tagnam, w)
 
     HighlightConfigure(wt.dlg_mark_l, "sel", fmt_selection)
 
@@ -3269,16 +3188,14 @@
     wt.dlg_mark_l.tag_lower("sel")
 
 
 #
 # This function is called after removal of tags in the Tag list dialog.
 #
 def MarkList_DeleteTag(tag):
-  global dlg_mark_shown
-
   if dlg_mark_shown:
     wt.dlg_mark_l.tag_delete(tag)
 
 
 #
 # This function is bound to destroy
 #
@@ -3297,17 +3214,15 @@
 #
 # This function opens a tiny dialog window which allows to enter a new text
 # tag for a selected bookmark. The dialog window is sized and placed so that
 # it exactly covers the respective entry in the bookmark list dialog to make
 # it appear as if the listbox entry could be edited directly.
 #
 def MarkList_OpenRename(idx):
-  global dlg_mark_shown, dlg_mark_list, mark_list
   global mark_rename, mark_rename_idx
-  global font_normal, font_bold, tick_str_prefix, tick_pat_num
 
   if dlg_mark_shown and (idx < len(dlg_mark_list)):
     wt.dlg_mark_l.see("%d.0" % (idx + 1))
     coo = wt.dlg_mark_l.dlineinfo("%d.0" % (idx + 1))
     if len(coo) == 5:
       SafeDestroy(wt.dlg_mark_mren)
       wt.dlg_mark_mren = Frame(wt.dlg_mark_l, takefocus=0, borderwidth=2, relief=RAISED)
@@ -3338,39 +3253,36 @@
 
       wt.dlg_mark_mren_e.selection_from(off)
       wt.dlg_mark_mren_e.selection_to("end")
       wt.dlg_mark_mren_e.icursor(off)
 
       xcoo = coo[0] - 3
       ycoo = coo[1] - 3
-      w = wt.dlg_mark_l.winfo_width()
-      h = coo[3] + 6
       wt.dlg_mark_mren.place(anchor=NW, x=xcoo, y=ycoo, relwidth=1.0) # -in .dlg_mark.l
 
       wt.dlg_mark_mren_e.focus_set()
       wt.dlg_mark_mren.grab_set()
 
 
 #
 # This function is bound to the enter key-press in the renaming popup window.
 # The function assigned the entered text to the bookmark and closes the popup.
 #
 def MarkList_Assign():
-  global mark_rename, mark_rename_idx
-
   MarkList_Rename(mark_rename_idx, mark_rename.get())
   MarkList_LeaveRename()
 
 
 #
 # This function is bound to all events which signal an exit of the rename
 # dialog window. The window is destroyed.
 #
 def MarkList_LeaveRename():
   global mark_rename, mark_rename_idx
+
   mark_rename = None
   mark_rename_idx = None
   SafeDestroy(wt.dlg_mark_mren)
   try:
     wt.dlg_mark_l.focus_set()
   except:
     pass
@@ -3378,16 +3290,15 @@
 
 # ----------------------------------------------------------------------------
 #
 # This function creates or raises a dialog window which contains the
 # search history, i.e. a list of previously used search expressions.
 #
 def SearchHistory_Open():
-  global font_content, col_bg_content, col_fg_content, cur_filename
-  global dlg_hist_shown, dlg_hist_sel, dlg_hist_geom
+  global dlg_hist_shown, dlg_hist_sel
 
   PreemptBgTasks()
   if not dlg_hist_shown:
     wt.dlg_hist = Toplevel(tk)
     if cur_filename != "":
       wt.dlg_hist.wm_title("Search history - " + cur_filename)
     else:
@@ -3461,24 +3372,23 @@
 
 #
 # This function is bound to destruction events on the search history dialog.
 # The function releases all dialog resources.
 #
 def SearchHistory_Close():
   global dlg_hist_sel, dlg_hist_shown
+
   dlg_hist_sel = None
   dlg_hist_shown = False
 
 
 #
 # This function pops up a context menu for the search history dialog.
 #
 def SearchHistory_ContextMenu(xcoo, ycoo):
-  global dlg_hist_sel
-
   dlg_hist_sel.TextSel_ContextSelection(xcoo, ycoo)
   sel = dlg_hist_sel.TextSel_GetSelection()
 
   wt.dlg_hist_ctxmen.delete(0, "end")
 
   c = 0
   if len(sel) > 0:
@@ -3497,25 +3407,22 @@
 
 
 #
 # This function is bound to double-click on a history entry. The function
 # starts a search with the selected expression.
 #
 def SearchHistory_Trigger():
-  global tlb_last_dir
   SearchHistory_CopyToSearch()
   SearchHistory_SearchNext(tlb_last_dir)
 
 #
 # This function returns all currently selected patterns. This is used only
 # to save the selection across history modifications.
 #
 def SearchHistory_StoreSel():
-  global dlg_hist_shown, dlg_hist_sel, tlb_history
-
   copy = []
   if dlg_hist_shown:
     sel = dlg_hist_sel.TextSel_GetSelection()
     for idx in sel:
       copy.append(tlb_history[idx])
 
   return copy
@@ -3524,16 +3431,14 @@
 
 #
 # This function selects all patterns in the given list. This is used only
 # to restore a previous selection after history modifications (e.g. sort
 # order change due to use of a pattern for a search)
 #
 def SearchHistory_RestoreSel(copy):
-  global dlg_hist_shown, dlg_hist_sel, tlb_history
-
   if dlg_hist_shown:
     sel = []
     for cphl in copy:
       idx = 0
       for hl in tlb_history:
         if ((hl[0] == cphl[0]) and
             (hl[1] == cphl[1]) and
@@ -3547,16 +3452,14 @@
 
 
 #
 # This function fills the search history dialog with all search expressions
 # in the search history stack.  The last used expression is placed on top.
 #
 def SearchHistory_Fill():
-  global dlg_hist_shown, tlb_history
-
   if dlg_hist_shown:
     wt.dlg_hist_f1_l.delete("1.0", "end")
 
     for hl in tlb_history:
       wt.dlg_hist_f1_l.insert("end", "\t", [],
                                      ("reg.exp." if hl[1] else "-"), ["small"], "\t", [],
                                      ("ign.case" if hl[2] else "-"), ["small"], "\t", [],
@@ -3567,16 +3470,14 @@
 
 #
 # This function is bound to the "Remove selected lines" command in the
 # search history list dialog's context menu.  All currently selected text
 # lines are removed from the search list.
 #
 def SearchHistory_Remove():
-  global dlg_hist_sel, tlb_history
-
   sel = dlg_hist_sel.TextSel_GetSelection()
   sel.sort(reverse=True)
   for idx in sel:
     line = "%d.0" % (idx + 1)
     del tlb_history[idx]
     wt.dlg_hist_f1_l.delete(line, line + " + 1 lines")
 
@@ -3586,22 +3487,21 @@
 
 #
 # This function is invoked by the "Copy to search field" command in the
 # search history list's context menu. (Note an almost identical menu entry
 # exists in the tag list dialog.)
 #
 def SearchHistory_CopyToSearch():
-  global tlb_history, tlb_find, tlb_regexp, tlb_case, tlb_find_focus
-  global dlg_hist_sel
+  global tlb_find_focus
 
   sel = dlg_hist_sel.TextSel_GetSelection()
   if len(sel) == 1:
     # force focus into find entry field & suppress "Enter" event
     SearchInit()
-    tlb_find_focus = 1
+    tlb_find_focus = True
     wt.f2_e.focus_set()
 
     hl = tlb_history[sel[0]]
 
     SearchHighlightClear()
     tlb_find.set(hl[0])
     tlb_regexp.set(hl[1])
@@ -3611,16 +3511,14 @@
 
 #
 # This function starts a search in the main text content for the selected
 # expression, i.e. as if the word had been entered to the search text
 # entry field. TODO: currently only one expression at a time can be searched
 #
 def SearchHistory_SearchNext(is_fwd):
-  global dlg_hist_sel, tlb_history, tlb_find
-
   ClearStatusLine("search")
 
   sel = dlg_hist_sel.TextSel_GetSelection()
   if len(sel) == 1:
     hl = tlb_history[sel[0]]
 
     pat = hl[0]
@@ -3646,17 +3544,14 @@
 #
 # This function is bound to the "list all" button in the search history
 # dialog. The function opens the search result list window and starts a
 # search for all expressions which are currently selected in the history
 # list (serializing multiple searches is handled by the search list dialog)
 #
 def SearchHistory_SearchAll(direction):
-  global tlb_history
-  global dlg_hist_sel
-
   ClearStatusLine("search")
 
   sel = dlg_hist_sel.TextSel_GetSelection()
   if len(sel) > 0:
     pat_list = []
     for idx in sel:
       hl = tlb_history[idx]
@@ -3695,31 +3590,27 @@
 
 
 #
 # This callback is used by the selection "library" to query the number of
 # elements in the list to determine the possible selection range.
 #
 def SearchHistory_GetLen():
-  global tlb_history
   return len(tlb_history)
 
 
 
 # ----------------------------------------------------------------------------
 #
 # This function creates or raises a dialog window which collects text lines
 # matching one or more search expressions.  The user can also freely add or
 # remove lines from the list.
 #
 def SearchList_Open(raise_win):
-  global font_content, col_bg_content, col_fg_content, cur_filename
-  global dlg_srch_shown, dlg_srch_geom, dlg_srch_sel, dlg_srch_lines, dlg_srch_fn_cache
-  global dlg_srch_show_fn, dlg_srch_show_tick, dlg_srch_tick_delta, dlg_srch_tick_root
-  global dlg_srch_highlight, dlg_srch_undo, dlg_srch_redo
-  global tick_pat_sep, tick_pat_num
+  global dlg_srch_shown, dlg_srch_sel
+  global dlg_srch_show_fn, dlg_srch_show_tick, dlg_srch_tick_delta, dlg_srch_highlight
 
   PreemptBgTasks()
   if not dlg_srch_shown:
     # create/teser variables to default values
     dlg_srch_shown = True
     SearchList_Init()
     dlg_srch_show_fn = BooleanVar(tk, False)
@@ -3744,33 +3635,33 @@
       with_fn = NORMAL
 
     wt.dlg_srch.wm_group(tk)
 
     wt.dlg_srch_menubar = Menu(wt.dlg_srch)
     wt.dlg_srch_menubar_ctrl = Menu(wt.dlg_srch_menubar, tearoff=0, postcommand=MenuPosted)
     wt.dlg_srch_menubar_ctrl.add_command(label="Load line numbers...", command=SearchList_LoadFrom)
-    wt.dlg_srch_menubar_ctrl.add_command(label="Save text as...", command=lambda:SearchList_SaveFileAs(0))
-    wt.dlg_srch_menubar_ctrl.add_command(label="Save line numbers...", command=lambda:SearchList_SaveFileAs(1))
+    wt.dlg_srch_menubar_ctrl.add_command(label="Save text as...", command=lambda:SearchList_SaveFileAs(False))
+    wt.dlg_srch_menubar_ctrl.add_command(label="Save line numbers...", command=lambda:SearchList_SaveFileAs(True))
     wt.dlg_srch_menubar_ctrl.add_separator()
     wt.dlg_srch_menubar_ctrl.add_command(label="Clear all", command=SearchList_Clear)
     wt.dlg_srch_menubar_ctrl.add_command(label="Close", command=wt.dlg_srch.destroy)
     wt.dlg_srch_menubar_edit = Menu(wt.dlg_srch_menubar, tearoff=0, postcommand=SearchList_MenuPosted)
     wt.dlg_srch_menubar_edit.add_command(label="Undo", command=SearchList_Undo, accelerator="u")
     wt.dlg_srch_menubar_edit.add_command(label="Redo", command=SearchList_Redo, accelerator="^r")
     wt.dlg_srch_menubar_edit.add_separator()
     wt.dlg_srch_menubar_edit.add_command(label="Import selected lines from main window", command=SearchList_CopyCurrentLine)
     wt.dlg_srch_menubar_edit.add_separator()
     wt.dlg_srch_menubar_edit.add_command(label="Remove selected lines", accelerator="Del", command=SearchList_RemoveSelection)
     wt.dlg_srch_menubar_search = Menu(wt.dlg_srch_menubar, tearoff=0, postcommand=MenuPosted)
     wt.dlg_srch_menubar_search.add_command(label="Search history...", command=SearchHistory_Open)
     wt.dlg_srch_menubar_search.add_command(label="Edit highlight patterns...", command=TagList_OpenDialog)
     wt.dlg_srch_menubar_search.add_separator()
-    wt.dlg_srch_menubar_search.add_command(label="Insert all search matches...", command=lambda:SearchAll(1, 0), accelerator="ALT-a")
-    wt.dlg_srch_menubar_search.add_command(label="Insert all matches above...", command=lambda:SearchAll(1 -1), accelerator="ALT-P")
-    wt.dlg_srch_menubar_search.add_command(label="Insert all matches below...", command=lambda:SearchAll(1, 1), accelerator="ALT-N")
+    wt.dlg_srch_menubar_search.add_command(label="Insert all search matches...", command=lambda:SearchAll(True, 0), accelerator="ALT-a")
+    wt.dlg_srch_menubar_search.add_command(label="Insert all matches above...", command=lambda:SearchAll(True, -1), accelerator="ALT-P")
+    wt.dlg_srch_menubar_search.add_command(label="Insert all matches below...", command=lambda:SearchAll(True, 1), accelerator="ALT-N")
     wt.dlg_srch_menubar_edit.add_separator()
     wt.dlg_srch_menubar_edit.add_command(label="Add main window search matches", command=lambda:SearchList_AddMatches(0))
     wt.dlg_srch_menubar_edit.add_command(label="Remove main window search matches", command=lambda:SearchList_RemoveMatches(0))
     wt.dlg_srch_menubar_search.add_separator()
     wt.dlg_srch_menubar_search.add_command(label="Clear search highlight", command=SearchHighlightClear, accelerator="&")
     wt.dlg_srch_menubar_options = Menu(wt.dlg_srch_menubar, tearoff=0, postcommand=MenuPosted)
     wt.dlg_srch_menubar_options.add_checkbutton(label="Show frame number", command=SearchList_ToggleFrameNo, state=with_fn, variable=dlg_srch_show_fn, accelerator="ALT-f")
@@ -3819,17 +3710,17 @@
     wt.dlg_srch_f1_l.bind("<Alt-Key-h>", lambda e:BindCallAndBreak(lambda:SearchList_ToggleOpt("highlight")))
     wt.dlg_srch_f1_l.bind("<Alt-Key-f>", lambda e:BindCallAndBreak(lambda:SearchList_ToggleOpt("show_fn")))
     wt.dlg_srch_f1_l.bind("<Alt-Key-t>", lambda e:BindCallAndBreak(lambda:SearchList_ToggleOpt("show_tick")))
     wt.dlg_srch_f1_l.bind("<Alt-Key-d>", lambda e:BindCallAndBreak(lambda:SearchList_ToggleOpt("tick_delta")))
     wt.dlg_srch_f1_l.bind("<Alt-Key-0>", lambda e:BindCallAndBreak(SearchList_SetFnRoot))
     wt.dlg_srch_f1_l.bind("<Alt-Key-n>", lambda e:BindCallAndBreak(lambda:SearchNext(1)))
     wt.dlg_srch_f1_l.bind("<Alt-Key-p>", lambda e:BindCallAndBreak(lambda:SearchNext(0)))
-    wt.dlg_srch_f1_l.bind("<Alt-Key-a>", lambda e:BindCallAndBreak(lambda:SearchAll(0, 0)))
-    wt.dlg_srch_f1_l.bind("<Alt-Key-N>", lambda e:BindCallAndBreak(lambda:SearchAll(0, 1)))
-    wt.dlg_srch_f1_l.bind("<Alt-Key-P>", lambda e:BindCallAndBreak(lambda:SearchAll(0, -1)))
+    wt.dlg_srch_f1_l.bind("<Alt-Key-a>", lambda e:BindCallAndBreak(lambda:SearchAll(False, 0)))
+    wt.dlg_srch_f1_l.bind("<Alt-Key-N>", lambda e:BindCallAndBreak(lambda:SearchAll(False, 1)))
+    wt.dlg_srch_f1_l.bind("<Alt-Key-P>", lambda e:BindCallAndBreak(lambda:SearchAll(False, -1)))
     wt.dlg_srch_f1_l.focus_set()
 
     wt.dlg_srch_ctxmen = Menu(wt.dlg_srch, tearoff=0)
 
     dlg_srch_shown = True
     wt.dlg_srch_f1_l.bind("<Destroy>", lambda e:SearchList_Close(), add="+")
     wt.dlg_srch.bind("<Configure>", lambda e:ToplevelResized(e.widget, wt.dlg_srch, wt.dlg_srch, "dlg_srch"))
@@ -3847,14 +3738,15 @@
 
 #
 # This function is bound to destruction events on the search list dialog window.
 # The function stops background processes and releases all dialog resources.
 #
 def SearchList_Close():
   global dlg_srch_sel, dlg_srch_lines, dlg_srch_fn_cache, dlg_srch_shown
+  global dlg_srch_undo, dlg_srch_redo
 
   SearchList_SearchAbort(False)
 
   dlg_srch_sel = None
   dlg_srch_lines = []
   dlg_srch_shown = False
   dlg_srch_undo = []
@@ -3862,16 +3754,15 @@
   dlg_srch_fn_cache = {}
 
 
 #
 # This function removes all content in the search list.
 #
 def SearchList_Clear():
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel
-  global dlg_srch_undo, dlg_srch_redo
+  global dlg_srch_lines, dlg_srch_redo
 
   if dlg_srch_shown:
     SearchList_SearchAbort(False)
 
     if len(dlg_srch_lines) > 0:
       dlg_srch_undo.append([-1, [dlg_srch_lines[-1]]])
       dlg_srch_redo = []
@@ -3883,15 +3774,15 @@
 
 
 #
 # This function clears the content and resets the dialog state variables.
 # The function is used when the window is newly opened or a new file is loaded.
 #
 def SearchList_Init():
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_fn_cache, dlg_srch_tick_root
+  global dlg_srch_lines, dlg_srch_fn_cache, dlg_srch_tick_root
   global dlg_srch_undo, dlg_srch_redo
 
   if dlg_srch_shown:
     dlg_srch_lines = []
     dlg_srch_undo = []
     dlg_srch_redo = []
     dlg_srch_tick_root = -1
@@ -3899,16 +3790,14 @@
 
 
 #
 # This function is bound to several ALT key combinations in the search list to
 # allow quick toggling of menu options.
 #
 def SearchList_ToggleOpt(opt):
-  global dlg_srch_show_fn, dlg_srch_show_tick, dlg_srch_tick_delta, dlg_srch_highlight
-
   if opt == "highlight":
     dlg_srch_highlight.set(not dlg_srch_highlight.get())
     SearchList_ToggleHighlight()
   elif opt == "show_fn":
     dlg_srch_show_fn.set(not dlg_srch_show_fn.get())
     SearchList_ToggleFrameNo()
   elif opt == "show_tick":
@@ -3919,16 +3808,14 @@
     SearchList_ToggleFrameNo()
 
 
 #
 # This function is called when the "edit" menu in the search list dialog is opened.
 #
 def SearchList_MenuPosted():
-  global dlg_srch_undo, dlg_srch_redo
-
   if len(dlg_srch_undo) > 0:
     cmd = dlg_srch_undo[-1]
     op = "addition" if cmd[0] > 0 else "removal"
     wt.dlg_srch_menubar_edit.entryconfigure("Undo*", state=NORMAL,
                                             label="Undo (%s of %d lines)" % (op, len(cmd[1])))
   else:
     wt.dlg_srch_menubar_edit.entryconfigure("Undo*", state=DISABLED, label="Undo")
@@ -3944,18 +3831,14 @@
   MenuPosted()
 
 
 #
 # This function pops up a context menu for the search list dialog.
 #
 def SearchList_ContextMenu(xcoo, ycoo):
-  global tlb_find
-  global dlg_srch_sel, dlg_srch_lines
-  global tick_pat_sep, tick_pat_num, tick_str_prefix, dlg_srch_fn_cache
-
   dlg_srch_sel.TextSel_ContextSelection(xcoo, ycoo)
   sel = dlg_srch_sel.TextSel_GetSelection()
 
   wt.dlg_srch_ctxmen.delete(0, "end")
 
   c = 0
   if tlb_find.get() != "":
@@ -3987,16 +3870,16 @@
 
 #
 # This function is bound to the "Remove selected lines" command in the
 # search list dialog's context menu.  All currently selected text lines
 # are removed from the search list.
 #
 def SearchList_RemoveSelection():
-  global dlg_srch_sel, dlg_srch_lines
-  global dlg_srch_undo, dlg_srch_redo
+  global dlg_srch_lines
+  global dlg_srch_redo
 
   if SearchList_SearchAbort():
     sel = dlg_srch_sel.TextSel_GetSelection()
     sel = sorted(sel, reverse=True)
     if len(sel) > 0:
       new_lines = dlg_srch_lines
       line_list = []
@@ -4016,16 +3899,14 @@
 
 
 # This function is bound to "n", "N" in the search filter dialog. The function
 # starts a regular search in the main window, but repeats until a matching
 # line is found which is also listed in the filter dialog.
 #
 def SearchList_SearchNext(is_fwd):
-  global dlg_srch_sel, dlg_srch_lines
-
   old_yview = wt.f1_t.yview()
   old_cpos = wt.f1_t.index("insert")
 
   if is_fwd:
     wt.f1_t.mark_set("insert", "insert lineend")
   else:
     wt.f1_t.mark_set("insert", "insert linestart")
@@ -4056,17 +3937,14 @@
 
 
 #
 # This function is bound to the "Show frame number" checkbutton which toggles
 # the display of frame numbers in front of each line on/off.
 #
 def SearchList_ToggleFrameNo():
-  global dlg_srch_sel, dlg_srch_lines, dlg_srch_fn_cache, tick_pat_sep, tick_pat_num
-  global dlg_srch_show_fn, dlg_srch_show_tick, dlg_srch_tick_delta, dlg_srch_tick_root
-
   if tick_pat_num == "":
     DisplayStatusLine("search", "error", "No patterns defined in the RC file for parsing frame numbers")
     dlg_srch_tick_delta.set(False)
     dlg_srch_show_tick.set(False)
     dlg_srch_show_fn.set(False)
 
   elif (tick_pat_sep == "") and (dlg_srch_show_tick.get() or dlg_srch_tick_delta.get()):
@@ -4085,16 +3963,15 @@
 #
 # This function is bound to ALT-0 in the search result list and to the
 # "Select root FN" context menu command. The function sets the currently
 # selected line as origin for frame number delta calculations and enables
 # frame number delta display, which requires a complete refresh of the list.
 #
 def SearchList_SetFnRoot():
-  global dlg_srch_sel, dlg_srch_lines, dlg_srch_fn_cache, tick_pat_sep, tick_pat_num
-  global dlg_srch_show_fn, dlg_srch_show_tick, dlg_srch_tick_delta, dlg_srch_tick_root
+  global dlg_srch_tick_root
 
   if tick_pat_sep != "":
     if SearchList_SearchAbort():
       sel = dlg_srch_sel.TextSel_GetSelection()
       if len(sel) > 0:
         line = dlg_srch_lines[sel[0]]
         # extract the frame number from the text in the main window around the referenced line
@@ -4116,15 +3993,15 @@
 
 
 #
 # This function is bound to the "Highlight search" checkbutton which toggles
 # highlighting of lines matching searches in the main window on/off.
 #
 def SearchList_ToggleHighlight():
-  global dlg_srch_highlight, tlb_cur_hall_opt
+  global tlb_cur_hall_opt
 
   if dlg_srch_highlight.get():
     # search highlighting was enabled:
     # force update of global highlighting (in main and search result windows)
     tlb_cur_hall_opt = ["", []]
     SearchHighlightUpdateCurrent()
   else:
@@ -4134,15 +4011,14 @@
 
 #
 # This function is bound to the "Undo" menu command any keyboard shortcut.
 # This reverts the last modification of the line list (i.e. last removal or
 # addition, either via search or manually.)
 #
 def SearchList_Undo():
-  global dlg_srch_shown, dlg_srch_undo, dlg_srch_redo
   global tid_search_list
 
   ClearStatusLine("search")
   if dlg_srch_shown:
     if len(dlg_srch_undo) > 0:
       if SearchList_SearchAbort():
         cmd = dlg_srch_undo[-1]
@@ -4154,15 +4030,14 @@
 
 
 #
 # This function is bound to the "Redo" menu command any keyboard shortcut.
 # This reverts the last "undo", if any.
 #
 def SearchList_Redo():
-  global dlg_srch_shown, dlg_srch_undo, dlg_srch_redo
   global tid_search_list
 
   ClearStatusLine("search")
   if dlg_srch_shown:
     if len(dlg_srch_redo) > 0:
       if SearchList_SearchAbort():
         cmd = dlg_srch_redo[-1]
@@ -4174,17 +4049,15 @@
 
 
 #
 # This function acts as background process for undo and redo operations.
 # Each iteration of this task works on at most 250-500 lines.
 #
 def SearchList_BgUndoRedoLoop(op, line_list, mode, off):
-  global block_bg_tasks, tid_search_inc, tid_search_hall, tid_search_list
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel
-  global dlg_srch_undo, dlg_srch_redo
+  global tid_search_list
 
   if block_bg_tasks or (tid_search_inc is not None) or (tid_search_hall is not None):
     # background tasks are suspended - re-schedule with timer
     tid_search_list = tk.after(100, lambda: SearchList_BgUndoRedoLoop(op, line_list, mode, off))
 
   elif dlg_srch_shown:
     anchor = SearchList_GetViewAnchor()
@@ -4260,47 +4133,42 @@
     dlg_srch_lines.sort()
 
 
 #
 # Wrapper functions to simplify external interfaces
 #
 def SearchList_AddMatches(direction):
-  global tlb_find, tlb_regexp, tlb_case
   SearchList_SearchMatches(1, tlb_find.get(), tlb_regexp.get(), tlb_case.get(), direction)
 
 
 def SearchList_RemoveMatches(direction):
-  global tlb_find, tlb_regexp, tlb_case
   SearchList_SearchMatches(0, tlb_find.get(), tlb_regexp.get(), tlb_case.get(), direction)
 
 
 #
 # This function is the external interface to the search list for adding
 # or removing lines matching the given search pattern.  The search is
 # performed in a background task, i.e. it's not completed when this
 # function returns.
 #
 def SearchList_SearchMatches(do_add, pat, is_re, use_case, direction):
-  global dlg_srch_sel
-
   if pat != "":
     if SearchExprCheck(pat, is_re, True):
       hl = [pat, is_re, use_case]
       pat_list = [hl]
       SearchList_StartSearchAll(pat_list, do_add, direction)
 
 
 #
 # Helper function which performs a binary search in the sorted line index
 # list for the first value which is larger or equal to the given value.
 # Returns the index of the element, or the length of the list if all
 # values in the list are smaller.
 #
 def SearchList_GetLineIdx(ins_line):
-  global dlg_srch_lines
   return bisect.bisect_left(dlg_srch_lines, ins_line)
 #  end = len(dlg_srch_lines)
 #  min = -1
 #  max = end
 #  if end > 0:
 #    idx = end >> 1
 #    end -= 1
@@ -4334,40 +4202,39 @@
 def SearchList_StartSearchAll(pat_list, do_add, direction):
   global dlg_srch_redo, tid_search_list
 
   if SearchList_SearchAbort():
     if direction == 0:
       line = 1
     else:
-      line = int(wt.f1_t.index("insert").split(".")[0])
+      line = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
 
     # reset redo list
     dlg_srch_redo = []
 
     tid_search_list = tk.after(10, lambda: SearchList_BgSearchLoop(pat_list, do_add, direction, line, 0, 0))
 
 
 #
 # This function acts as background process to fill the search list window.
 # The search loop continues for at most 100ms, then the function re-schedules
 # itself as idle task.
 #
 def SearchList_BgSearchLoop(pat_list, do_add, direction, line, pat_idx, loop_cnt):
-  global block_bg_tasks, tid_search_inc, tid_search_hall, tid_search_list
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel, dlg_srch_undo
+  global tid_search_list
 
   if block_bg_tasks or (tid_search_inc is not None) or (tid_search_hall is not None):
     # background tasks are suspended - re-schedule with timer
     tid_search_list = tk.after(100, lambda line=line: SearchList_BgSearchLoop(pat_list, do_add, direction, line, pat_idx, 0))
 
   elif loop_cnt > 10:
     tid_search_list = tk.after(10, lambda line=line: SearchList_BgSearchLoop(pat_list, do_add, direction, line, pat_idx, 0))
 
   elif dlg_srch_shown:
-    max_line = int(wt.f1_t.index("end").split(".")[0])
+    max_line = int(wt.f1_t.index("end").split(".", maxsplit=1)[0])
     anchor = SearchList_GetViewAnchor()
     stop_t = datetime.now() + timedelta(microseconds=100000)
     hl = pat_list[pat_idx]
     pat = hl[0]
     opt = Search_GetOptions(pat, hl[1], hl[2], (0 if direction < 0 else 1))
     line_list = []
     off = 0
@@ -4377,15 +4244,15 @@
       last_line = "1.0"
 
     while line < max_line:
       pos = wt.f1_t.search(pat, ("%d.0" % line), last_line, **opt)
       if pos == "":
         break
 
-      line = int(pos.split(".")[0])
+      line = int(pos.split(".", maxsplit=1)[0])
       idx = SearchList_GetLineIdx(line)
       if do_add:
         if (idx >= len(dlg_srch_lines)) or (dlg_srch_lines[idx] != line):
           SearchList_InsertLine(line, "%d.0" % (idx + off + 1))
           line_list.append(line)
           if direction >= 0:
             off += 1
@@ -4414,18 +4281,18 @@
       SearchList_SeeViewAnchor(anchor)
 
     if (line < max_line) and (pos != ""):
       # create or update the progress bar
       if direction == 0:
         ratio = line / max_line
       elif direction < 0:
-        thresh = int(wt.f1_t.index("insert").split(".")[0])
+        thresh = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
         ratio = 1 - (line / thresh)
       else:
-        thresh = int(wt.f1_t.index("insert").split(".")[0])
+        thresh = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
         ratio = line / (max_line - thresh)
 
       ratio = int(100.0*(ratio + pat_idx)/len(pat_list))
       SearchList_SearchProgress(ratio)
 
       loop_cnt += 1
       tid_search_list = tk.after_idle(lambda line=line, loop_cnt=loop_cnt:
@@ -4435,15 +4302,15 @@
       SearchList_BgSearch_FinalizeUndoList(dlg_srch_undo)
       pat_idx += 1
       if pat_idx < len(pat_list):
         loop_cnt += 1
         if direction == 0:
           line = 1
         else:
-          line = int(wt.f1_t.index("insert").split(".")[0])
+          line = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
 
         tid_search_list = tk.after_idle(lambda line=line, loop_cnt=loop_cnt:
                                           SearchList_BgSearchLoop(pat_list, do_add, direction, line, pat_idx, loop_cnt))
       else:
         tid_search_list = None
         SafeDestroy(wt.dlg_srch_slpro)
         SafeDestroy(wt.srch_abrt)
@@ -4454,35 +4321,34 @@
 
 
 #
 # This function inserts all lines of text tagged with one of the given
 # tags in the main window content into the search list.
 #
 def SearchList_StartSearchTags(tag_list, direction):
-  global tid_search_list
+  global tid_search_list, dlg_srch_redo
 
   if SearchList_SearchAbort():
     if direction == 1:
-      line = int(wt.f1_t.index("insert").split(".")[0])
+      line = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
     else:
       line = 1
 
     # reset redo list
     dlg_srch_redo = []
 
     tid_search_list = tk.after(10, lambda: SearchList_BgSearchTagsLoop(tag_list, 0, direction, line, 0))
 
 
 #
 # This function acts as background process to fill the search list window with
 # matches on highlight tags.
 #
 def SearchList_BgSearchTagsLoop(tag_list, tag_idx, direction, line, loop_cnt):
-  global block_bg_tasks, tid_search_inc, tid_search_hall, tid_search_list
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel, dlg_srch_undo
+  global tid_search_list
 
   if block_bg_tasks or (tid_search_inc is not None) or (tid_search_hall is not None):
     # background tasks are suspended - re-schedule with timer
     tid_search_list = tk.after(100, lambda: SearchList_BgSearchTagsLoop(tag_list, tag_idx, direction, line, 0))
 
   elif loop_cnt > 10:
     tid_search_list = tk.after(10, lambda: SearchList_BgSearchTagsLoop(tag_list, tag_idx, direction, line, 0))
@@ -4523,16 +4389,16 @@
       dlg_srch_lines.sort()
 
       # select previously selected line again
       SearchList_SeeViewAnchor(anchor)
 
     if len(pos12) == 2:
       # create or update the progress bar
-      max_line = int(last_line.split(".")[0])
-      thresh = int(wt.f1_t.index("insert").split(".")[0])
+      max_line = int(last_line.split(".", maxsplit=1)[0])
+      thresh = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
       if direction == 0:
         ratio = line / max_line
       elif direction < 0:
         ratio = line / thresh
       else:
         ratio = line / (max_line - thresh)
 
@@ -4544,19 +4410,19 @@
 
     else:
       SearchList_BgSearch_FinalizeUndoList(dlg_srch_undo)
       tag_idx += 1
       if tag_idx < len(tag_list):
         loop_cnt += 1
         if direction == 1:
-          line = int(wt.f1_t.index("insert").split(".")[0])
+          line = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
         else:
           line = 1
 
-        tid_search_list = tk.after_idle(lambda: SearchList_BgSearchTagsLoop(tag_list, tag_idx, line, direction, loop_cnt))
+        tid_search_list = tk.after_idle(lambda: SearchList_BgSearchTagsLoop(tag_list, tag_idx, direction, line, loop_cnt))
       else:
         tid_search_list = None
         SafeDestroy(wt.dlg_srch_slpro)
         SafeDestroy(wt.srch_abrt)
         wt.dlg_srch_f1_l.configure(cursor="top_left_arrow")
 
   else:
@@ -4586,15 +4452,15 @@
 # This function stops a possibly ongoing background search in the search
 # list dialog. Optionally the user is asked it he really wants to abort.
 # The function returns 0 and does not abort the background action if the
 # user selects "Cancel", else it returns 1.  The caller MUST check the
 # return value if parameter "do_warn" is TRUE.
 #
 def SearchList_SearchAbort(do_warn=True):
-  global tid_search_list, dlg_srch_undo, dlg_srch_redo
+  global tid_search_list
   global vwait_search_complete
 
   cancel_new = False
 
   if tid_search_list is not None:
     if do_warn:
       vwait_search_complete = StringVar(tk, "wait")
@@ -4671,50 +4537,46 @@
 def SearchList_DestroyCb():
   if vwait_search_complete.get() == "wait":
     if tid_search_list is not None:
       vwait_search_complete.set("cancel_new")
     else:
       vwait_search_complete.set("obsolete")
 
+
 def SearchList_AbortVwaitSet(val):
-  global vwait_search_complete
   vwait_search_complete.set(val)
 
 #
 # This helper function is called before modifications of the search result
 # list by the various background tasks to determine a line which can serve
 # as "anchor" for the view, i.e. which will be made visible again after the
 # insertions or removals (which may lead to scrolling.)
 #
 def SearchList_GetViewAnchor():
-  global dlg_srch_sel, dlg_srch_lines
-
   sel = dlg_srch_sel.TextSel_GetSelection()
   if len(sel) > 0:
     # keep selection visible
     return [1, dlg_srch_lines[sel[0]]]
   else:
     # no selection - check if line near cursor in main win is visible
-    line = int(wt.f1_t.index("insert").split(".")[0])
+    line = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
     idx = SearchList_GetLineIdx(line)
     if ((idx < len(dlg_srch_lines)) and
         (wt.dlg_srch_f1_l.bbox("%d.0" % idx) is not None)):
       return [0, dlg_srch_lines[idx]]
 
   return [0, -1]
 
 
 #
 # This helper function is called after modifications of the search result
 # list by the various background tasks to make the previously determined
 # "anchor" line visible and to adjust the selection.
 #
 def SearchList_SeeViewAnchor(info):
-  global dlg_srch_sel, dlg_srch_lines
-
   anchor = info[1]
   if anchor >= 0:
     #set idx [lsearch -exact -integer -sorted -increasing $dlg_srch_lines $anchor]
     idx = SearchList_GetLineIdx(anchor)
     if (idx < len(dlg_srch_lines)) and (dlg_srch_lines[idx] == anchor):
       wt.dlg_srch_f1_l.see("%d.0" % (idx + 1))
       if info[0]:
@@ -4755,16 +4617,15 @@
       undo_list[-1][0] = prev_op
 
 
 #
 # This function inserts all selected lines in the main window into the list.
 #
 def SearchList_AddMainSelection():
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel
-  global dlg_srch_undo, dlg_srch_redo
+  global dlg_srch_redo
 
   if dlg_srch_shown and SearchList_SearchAbort():
     pos12 = wt.f1_t.tag_nextrange("sel", "1.0")
     if len(pos12) == 2:
       line = int(pos12[0].split(".")[0])
       (line_2, char) = map(int, pos12[1].split("."))
       if char == 0: line_2 -= 1
@@ -4792,30 +4653,29 @@
 
 #
 # This function inserts either the line in the main window holding the cursor
 # or all selected lines into the search result list.  It's bound to the "i" key
 # press event in the main window.
 #
 def SearchList_CopyCurrentLine():
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel
-  global dlg_srch_undo, dlg_srch_redo
+  global dlg_srch_redo
 
   if not dlg_srch_shown:
     SearchList_Open(False)
 
   if dlg_srch_shown and SearchList_SearchAbort():
     pos12 = wt.f1_t.tag_nextrange("sel", "1.0")
     # ignore selection if not visible (because it can be irritating when "i"
     # inserts some random line instead of the one holding the cursor)
     if (len(pos12) == 2) and (wt.f1_t.bbox(pos12[0]) is not None):
       # selection exists: add all selected lines
       SearchList_AddMainSelection()
     else:
       # get line number of the cursor position
-      line = int(wt.f1_t.index("insert").split(".")[0])
+      line = int(wt.f1_t.index("insert").split(".", maxsplit=1)[0])
       idx = SearchList_GetLineIdx(line)
       if (idx >= len(dlg_srch_lines)) or (dlg_srch_lines[idx] != line):
         dlg_srch_lines.insert(idx, line)
         pos = "%d.0" % (idx + 1)
         SearchList_InsertLine(line, pos)
         wt.dlg_srch_f1_l.see(pos)
         dlg_srch_sel.TextSel_SetSelection([idx], False)
@@ -4829,17 +4689,14 @@
 
 
 #
 # This function creates the tags for selection and color highlighting.
 # This is used for initialisation and after editing highlight tags.
 #
 def SearchList_CreateHighlightTags():
-  global patlist, fmt_find, fmt_selection
-  global dlg_srch_sel, dlg_srch_shown
-
   if dlg_srch_shown:
     # create highlight tags
     for w in patlist:
       HighlightConfigure(wt.dlg_srch_f1_l, w[4], w)
 
     # create text tag for search highlights
     HighlightConfigure(wt.dlg_srch_f1_l, "find", fmt_find)
@@ -4856,28 +4713,23 @@
     wt.dlg_srch_f1_l.tag_configure("bookmark", lmargin1=0)
 
 
 #
 # This function is called after removal of tags in the Tag list dialog.
 #
 def SearchList_DeleteTag(tag):
-  global dlg_srch_shown
-
   if dlg_srch_shown:
     wt.dlg_srch_f1_l.tag_delete(tag)
 
 
 #
 # This function is called out of the main window's highlight loop for every line
 # to which a highlight is applied.
 #
 def SearchList_HighlightLine(tag, line):
-  global dlg_srch_shown, dlg_srch_highlight, dlg_srch_lines
-  global tid_high_init
-
   if dlg_srch_shown:
     if dlg_srch_highlight.get() or (tid_high_init is not None):
       idx = SearchList_GetLineIdx(line)
       if (idx < len(dlg_srch_lines)) and (dlg_srch_lines[idx] == line):
         try:
           wt.dlg_srch_f1_l.tag_add(tag, "%d.0" % (idx + 1), "%d.0" % (idx + 2))
         except:
@@ -4885,27 +4737,23 @@
 
 
 #
 # This function is bound to the "Toggle highlight" checkbutton in the
 # search list dialog's menu.  The function enables or disables search highlight.
 #
 def SearchList_HighlightClear():
-  global dlg_srch_shown
-
   if dlg_srch_shown:
     wt.dlg_srch_f1_l.tag_remove("find", "1.0", "end")
 
 
 #
 # This function adjusts the view in the search result list so that the given
 # main window's text line becomes visible.
 #
 def SearchList_MatchView(line):
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel
-
   if dlg_srch_shown:
     idx = SearchList_GetLineIdx(line)
     if idx < len(dlg_srch_lines):
       wt.dlg_srch_f1_l.see("%d.0" % idx)
       wt.dlg_srch_f1_l.see("%d.0" % (idx + 1))
       wt.dlg_srch_f1_l.mark_set("insert", "%d.0" % (idx + 1))
 
@@ -4924,17 +4772,14 @@
 # This function is called when a bookmark is added or removed in the main
 # window.  The function displays the bookmark in the respective line in
 # the search filter dialog, if the line is currently visible.  (Note this
 # function is not used to mark lines which are newly inserted into the
 # dialog and which already have a bookmark; see the insert function below)
 #
 def SearchList_MarkLine(line):
-  global dlg_srch_shown, dlg_srch_lines
-  global img_marker, mark_list
-
   if dlg_srch_shown:
     idx = SearchList_GetLineIdx(line)
     if (idx < len(dlg_srch_lines)) and (dlg_srch_lines[idx] == line):
       pos = "%d.0" % (idx + 1)
       if mark_list.get(line):
         wt.dlg_srch_f1_l.image_create(pos, image=img_marker, padx=2)
         wt.dlg_srch_f1_l.tag_add("bookmark", pos)
@@ -4950,31 +4795,25 @@
 
 #
 # This function is bound to the "m" key in the search filter dialog.
 # The function adds or removes a bookmark on the currently selected
 # line (but only if exactly one line is selected.)
 #
 def SearchList_ToggleMark():
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_sel
-
   sel = dlg_srch_sel.TextSel_GetSelection()
   if len(sel) == 1:
     line = dlg_srch_lines[sel[0]]
     Mark_Toggle(line)
 
 
 #
 # This function copies a line of text (including highlighting tags and
 # bookmark marker) from the main window into the the search filter dialog.
 #
 def SearchList_InsertLine(line_idx, ins_pos):
-  global dlg_srch_show_fn, dlg_srch_show_tick, dlg_srch_tick_delta, dlg_srch_tick_root
-  global dlg_srch_fn_cache
-  global tick_pat_sep, tick_str_prefix, img_marker, mark_list
-
   # copy text content and tags out of the main window
   pos = "%d.0" % line_idx
   dump = ExtractText(pos + " linestart", pos + " lineend")
   tag_list = [x for x in wt.f1_t.tag_names(pos) if x.startswith("tag")]
 
   if dlg_srch_tick_delta.get() or dlg_srch_show_fn.get() or dlg_srch_show_tick.get():
     fn = ParseFrameTickNo(pos, dlg_srch_fn_cache)
@@ -5016,25 +4855,25 @@
 
 
 #
 # This function fills the search list dialog with all text lines indicated in
 # the dialog's line number list (note the first line has number 1)
 #
 def SearchList_Refill():
+  global tid_search_list
   # WARNING: caller must invoke SearchList_SearchAbort
   tid_search_list = tk.after(10, lambda: SearchList_BgRefillLoop(0))
 
 
 #
 # This function acts as background process to refill the search list window
 # with previous content, but in a different format (e.g. with added frame nums)
 #
 def SearchList_BgRefillLoop(off):
-  global block_bg_tasks, tid_search_inc, tid_search_hall, tid_search_list
-  global dlg_srch_shown, dlg_srch_lines
+  global tid_search_list
 
   if block_bg_tasks or (tid_search_inc is not None) or (tid_search_hall is not None):
     # background tasks are suspended - re-schedule with timer
     tid_search_list = tk.after(100, lambda: SearchList_BgRefillLoop(off))
 
   elif dlg_srch_shown:
     end_off = off + 400               # end_off is actually last+1
@@ -5072,39 +4911,36 @@
 
 #
 # This function is a callback for selection changes in the search list dialog.
 # If a single line is selected, the view in the main window is changed to
 # display the respective line.
 #
 def SearchList_SelectionChange(sel):
-  global dlg_srch_sel, dlg_srch_lines
-
   if len(sel) == 1:
     idx = sel[0]
     if idx < len(dlg_srch_lines):
       Mark_Line(dlg_srch_lines[idx])
 
 
 #
 # This callback is used by the selection "library" to query the number of
 # elements in the list to determine the possible selection range.
 #
 def SearchList_GetLen():
-  global dlg_srch_sel, dlg_srch_lines
   return len(dlg_srch_lines)
 
 
 #
 # This function must be called when portions of the text in the main window
 # have been deleted to update references to text lines. Parameter meaning:
 # - top_l: this is the first line which is not deleted, or 1 if none
 # - bottom_l: this line and all below have been removed, or 0 if none
 #
 def SearchList_AdjustLineNums(top_l, bottom_l):
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_undo, dlg_srch_redo, dlg_srch_fn_cache
+  global dlg_srch_lines, dlg_srch_undo, dlg_srch_redo, dlg_srch_fn_cache
 
   if dlg_srch_shown:
     if bottom_l == 0:
       # delete from 1 ... topl
       idx = SearchList_GetLineIdx(top_l)
       if idx > 0:
         wt.dlg_srch_f1_l.delete("1.0", "%d.0" % (idx + 1))
@@ -5133,16 +4969,14 @@
     dlg_srch_fn_cache = {}
 
 
 #
 # This function stores all text lines in the search result window into a file.
 #
 def SearchList_SaveFile(filename, lnum_only):
-  global dlg_srch_lines
-
   try:
     with open(filename, "w") as f:
       if lnum_only:
         # save line numbers only (i.e. line numbers in main window)
         for line in dlg_srch_lines:
           print(line, file=f)
       else:
@@ -5155,16 +4989,14 @@
 
 #
 # This function is called by menu entry "Save as..." in the search dialog.
 # The user is asked to select an output file; if he does so the list
 # content is written into it, in the format selected by the user.
 #
 def SearchList_SaveFileAs(lnum_only):
-  global dlg_srch_lines
-
   PreemptBgTasks()
   if len(dlg_srch_lines) > 0:
     def_name = ""
     filename = filedialog.asksaveasfilename(parent=wt.dlg_srch, filetypes=(("all", "*"), ("Text", "*.txt")),
                                             title="Select output file",
                                             initialfile=os.path.basename(def_name),
                                             initialdir=os.path.dirname(def_name))
@@ -5179,27 +5011,29 @@
 #
 # This function is called by menu entry "Load line numbers..." in the search
 # result dialog. The user is asked to select an input file; if he does so a
 # list of line numbers is extracted from it and lines with these numbers is
 # copied from the main window.
 #
 def SearchList_LoadFrom():
+  global tid_search_list
+
   if dlg_srch_shown and SearchList_SearchAbort():
     PreemptBgTasks()
     def_name = ""
     filename = filedialog.askopenfilename(parent=wt.dlg_srch, filetypes=(("all", "*"), ("Text", "*.txt")),
                                           title="Select file for reading",
                                           initialfile=os.path.basename(def_name),
                                           initialdir=os.path.dirname(def_name))
     ResumeBgTasks()
 
     if len(filename) != 0:
       try:
         with open(filename, "r") as f:
-          max_line = int(wt.f1_t.index("end").split(".")[0])
+          max_line = int(wt.f1_t.index("end").split(".", maxsplit=1)[0])
           answer = ""
           skipped = 0
           synerr = 0
           line_list = []
 
           for line_str in f.readlines():
             match = re.match(r"^(\d+)", line_str)
@@ -5235,16 +5069,16 @@
 
 
 #
 # This function acts as background process to fill the search list window
 # with a given list of line indices.
 #
 def SearchList_BgLoadLoop(line_list, off):
-  global block_bg_tasks, tid_search_inc, tid_search_hall, tid_search_list
-  global dlg_srch_shown, dlg_srch_lines, dlg_srch_undo, dlg_srch_redo
+  global tid_search_list
+  global dlg_srch_redo
 
   if block_bg_tasks or (tid_search_inc is not None) or (tid_search_hall is not None):
     # background tasks are suspended - re-schedule with timer
     tid_search_list = tk.after(100, lambda: SearchList_BgLoadLoop(line_list, off))
 
   elif dlg_srch_shown:
     anchor = SearchList_GetViewAnchor()
@@ -5289,16 +5123,14 @@
 
 
 #
 # This function is bound to CTRL-g in the search list and displays stats
 # about the content of the search result list.
 #
 def SearchList_DisplayStats():
-  global dlg_srch_sel, dlg_srch_lines
-
   sel = dlg_srch_sel.TextSel_GetSelection()
   if len(sel) == 1:
     line_idx = sel[0] + 1
     msg = "line %d of %d in the search list" % (line_idx, len(dlg_srch_lines))
   else:
     msg = "%d lines in the search list" % len(dlg_srch_lines)
 
@@ -5307,16 +5139,15 @@
 
 # ----------------------------------------------------------------------------
 #
 # This function creates or raises the color highlighting tags list dialog.
 # This dialog shows all currently defined tag assignments.
 #
 def TagList_OpenDialog():
-  global font_content, col_bg_content, col_fg_content
-  global dlg_tags_shown, dlg_tags_geom, dlg_tags_sel
+  global dlg_tags_shown, dlg_tags_sel
 
   PreemptBgTasks()
   if not dlg_tags_shown:
     wt.dlg_tags = Toplevel(tk)
     wt.dlg_tags.wm_title("Color highlights list")
     wt.dlg_tags.wm_group(tk)
 
@@ -5357,15 +5188,15 @@
     wt.dlg_tags_f2_but_blw.grid(sticky="we", column=4, row=0)
     wt.dlg_tags_f2_but_abve = Button(wt.dlg_tags_f2, text="All above", command=lambda: TagList_SearchList(-1), state=DISABLED)
     wt.dlg_tags_f2_but_abve.grid(sticky="we", column=5, row=0)
     wt.dlg_tags_f2.pack(side=TOP, anchor=W, pady=2)
 
     wt.dlg_tags_ctxmen = Menu(wt.dlg_tags, tearoff=0)
 
-    wt.dlg_tags_f1_l.bind("<Double-Button-1>", lambda e:BindCallAndBreak(lambda: TagList_DoubleClick(e.x, e.y)))
+    wt.dlg_tags_f1_l.bind("<Double-Button-1>", lambda e:BindCallAndBreak(lambda: TagList_DoubleClick()))
     wt.dlg_tags_f1_l.bind("<ButtonRelease-3>", lambda e:BindCallAndBreak(lambda: TagList_ContextMenu(e.x, e.y)))
     wt.dlg_tags_f1_l.bind("<Delete>", lambda e:BindCallAndBreak(TagList_RemoveSelection))
     wt.dlg_tags_f1_l.bind("<Key-slash>", lambda e:BindCallAndBreak(lambda: SearchEnter(1, wt.dlg_tags_f1_l)))
     wt.dlg_tags_f1_l.bind("<Key-question>", lambda e:BindCallAndBreak(lambda: SearchEnter(0, wt.dlg_tags_f1_l)))
     wt.dlg_tags_f1_l.bind("<Key-ampersand>", lambda e:BindCallAndBreak(SearchHighlightClear))
     wt.dlg_tags_f1_l.bind("<Key-n>", lambda e:BindCallAndBreak(lambda: TagList_Search(1)))
     wt.dlg_tags_f1_l.bind("<Key-N>", lambda e:BindCallAndBreak(lambda: TagList_Search(0)))
@@ -5403,32 +5234,28 @@
 #
 # This function is bound to right mouse clicks in the highlight tag list and pops
 # up a context menu. If the mouse click occurred outside of the current selection
 # the selection is updated. Then the menu is populated and shown at the mouse
 # coordinates.
 #
 def TagList_ContextMenu(xcoo, ycoo):
-  global dlg_tags_sel
-
   dlg_tags_sel.TextSel_ContextSelection(xcoo, ycoo)
 
   TagList_ContextPopulate(wt.dlg_tags_ctxmen, 0)
 
   rootx = wt.dlg_tags.winfo_rootx() + xcoo
   rooty = wt.dlg_tags.winfo_rooty() + ycoo
   tk.call("tk_popup", wt.dlg_tags_ctxmen, rootx, rooty, 0)
 
 
 #
 # This function is used both to populate the "Edit" menu and the context menu.
 # The contents depend on the number of selected items.
 #
 def TagList_ContextPopulate(wid, show_all):
-  global tlb_find, dlg_tags_sel
-
   sel = dlg_tags_sel.TextSel_GetSelection()
   sel_cnt = len(sel)
   sel_el = sel[0] if (sel_cnt > 0) else None
 
   state_find = DISABLED if (tlb_find.get() == "") else NORMAL
   state_find_sel_1 = DISABLED if ((tlb_find.get() == "") or (sel_cnt != 1)) else NORMAL
   state_sel_1 = DISABLED if (sel_cnt != 1) else NORMAL
@@ -5448,29 +5275,25 @@
     wid.add_command(label="Remove selected entries", command=lambda:TagList_Remove(sel), state=state_sel_n0)
 
 
 #
 # This function is bound to double mouse button clicks onto an entry in
 # the highlight list. The function opens the markup editor dialog.
 #
-def TagList_DoubleClick(xcoo, ycoo):
-  global patlist, dlg_tags_sel
-
+def TagList_DoubleClick():
   sel = dlg_tags_sel.TextSel_GetSelection()
   if len(sel) == 1:
     Markup_OpenDialog(sel[0])
 
 
 #
 # This function is bound to the "up" button next to the color highlight list.
 # Each selected item (selection may be non-consecutive) is shifted up by one line.
 #
 def TagList_ShiftUp():
-  global patlist, dlg_tags_sel
-
   sel = dlg_tags_sel.TextSel_GetSelection()
   sel = sorted(sel) # must not sort inline
   if (len(sel) > 0) and (sel[0] > 0):
     new_sel = []
     for idx in sel:
       # remove the item in the listbox widget above the shifted one
       TagList_DisplayDelete(idx - 1)
@@ -5487,16 +5310,14 @@
 
 
 #
 # This function is bound to the "down" button next to the color highlight
 # list.  Each selected item is shifted down by one line.
 #
 def TagList_ShiftDown():
-  global patlist, dlg_tags_sel
-
   sel = dlg_tags_sel.TextSel_GetSelection()
   sel = sorted(sel, reverse=True) # must not sort inline
   if (len(sel) > 0) and (sel[0] < len(patlist) - 1):
     new_sel = []
     for idx in sel:
       TagList_DisplayDelete(idx + 1)
       TagList_DisplayInsert(idx, idx + 1)
@@ -5512,16 +5333,14 @@
 #
 # This function is bound to the next/prev buttons below the highlight tags
 # list. The function searches for the next line which is tagged with one of
 # the selected highlighting tags (i.e. no text search is performed!) When
 # multiple tags are searched for, the closest match is used.
 #
 def TagList_Search(is_fwd):
-  global patlist, dlg_tags_sel
-
   min_line = -1
   sel = dlg_tags_sel.TextSel_GetSelection()
 
   for pat_idx in sel:
     w = patlist[pat_idx]
 
     Search_AddHistory(w[0], w[1], w[2])
@@ -5554,17 +5373,14 @@
 
 #
 # This function is bound to the "List all" button in the color tags dialog.
 # The function opens the search result window and adds all lines matching
 # the pattern for the currently selected color tags.
 #
 def TagList_SearchList(direction):
-  global patlist, dlg_tags_sel
-
-  min_line = -1
   sel = dlg_tags_sel.TextSel_GetSelection()
   if len(sel) > 0:
     tag_list = []
     for pat_idx in sel:
       w = patlist[pat_idx]
       tag_list.append(w[4])
 
@@ -5576,16 +5392,14 @@
     DisplayStatusLine("search", "error", "No pattern is selected in the list")
 
 
 #
 # This function is bound to changes of the selection in the color tags list.
 #
 def TagList_SelectionChange(sel):
-  global dlg_tags_sel
-
   state = DISABLED if (len(sel) == 0) else NORMAL
 
   wt.dlg_tags_f2_but_next.configure(state=state)
   wt.dlg_tags_f2_but_prev.configure(state=state)
   wt.dlg_tags_f2_but_all.configure(state=state)
   wt.dlg_tags_f2_but_blw.configure(state=state)
   wt.dlg_tags_f2_but_abve.configure(state=state)
@@ -5595,28 +5409,23 @@
 
 
 #
 # This callback is used by the selection "library" to query the number of
 # elements in the list to determine the possible selection range.
 #
 def TagList_GetLen():
-  global patlist
   return len(patlist)
 
 
 #
 # This function updates a color tag text in the listbox.
 #
 def TagList_Update(pat_idx):
-  global dlg_tags_shown, patlist
-
   if dlg_tags_shown:
     if pat_idx < len(patlist):
-      w = patlist[pat_idx]
-
       TagList_Fill()
       dlg_tags_sel.TextSel_SetSelection([])
 
       wt.dlg_tags_f1_l.see("%d.0" % (pat_idx + 1))
 
 
 #
@@ -5627,30 +5436,26 @@
 
 
 #
 # This function inserts a color tag text into the listbox and applies its
 # highlight format options.
 #
 def TagList_DisplayInsert(pos, pat_idx):
-  global patlist
-
   w = patlist[pat_idx]
   txt = w[0] + "\n"
 
   # insert text (prepend space to improve visibility of selection)
   wt.dlg_tags_f1_l.insert("%d.0" % (pos + 1), "  ", "margin", txt, w[4])
 
 
 #
 # This function fills the highlight pattern list dialog window with all
 # list entries.
 #
 def TagList_Fill():
-  global dlg_tags_shown, patlist, fmt_selection
-
   if dlg_tags_shown:
     wt.dlg_tags_f1_l.delete("1.0", "end")
 
     idx = 0
     for w in patlist:
       HighlightConfigure(wt.dlg_tags_f1_l, w[4], w)
 
@@ -5663,41 +5468,36 @@
     wt.dlg_tags_f1_l.tag_lower("sel")
 
 
 #
 # This function allows to edit a color assigned to a tags entry.
 #
 def TagList_PopupColorPalette(pat_idx, is_fg):
-  global patlist
-
   if pat_idx < len(patlist):
     wt.dlg_tags_f1_l.see("%d.0" % (pat_idx + 1))
 
     cool = wt.dlg_tags_f1_l.dlineinfo("%d.0" % (pat_idx + 1))
     rootx = wt.dlg_tags.winfo_rootx() + cool[0]
     rooty = wt.dlg_tags.winfo_rooty() + cool[1]
 
     w = patlist[pat_idx]
     col_idx = 7 if is_fg else 6
-    def_col = w[col_idx]
 
     PaletteMenu_Popup(wt.dlg_tags, rootx, rooty,
                       lambda col:TagList_UpdateColor(col, pat_idx, is_fg),
                       w[col_idx])
 
 
 #
 # This function is invoked after a direct color change via the popup color palette.
 # The new color is saved in the highlight list and applied to the main window
 # and the highlight dialog's list. NOTE: the color value my be an empty string
 # (color "none" refers to the default fore- and background colors)
 #
 def TagList_UpdateColor(col, pat_idx, is_fg):
-  global patlist, dlg_tags_sel
-
   if pat_idx < len(patlist):
     w = patlist[pat_idx]
     col_idx = 7 if is_fg else 6
 
     w[col_idx] = col
     try:
       wt.dlg_tags_f1_l.tag_configure(w[4], background=w[6], foreground=w[7])
@@ -5707,26 +5507,23 @@
       patlist[pat_idx] = w
       UpdateRcAfterIdle()
 
       wt.f1_t.tag_configure(w[4], background=w[6], foreground=w[7])
 
       SearchList_CreateHighlightTags()
       MarkList_CreateHighlightTags()
-    except Exception as e:
+    except Exception:
       messagebox.showerror(parent=wt.dlg_srch, message="Failed to update color")
 
 
 #
 # This function is invoked by the "Add current search" entry in the highlight
 # list's context menu.
 #
 def TagList_AddSearch(parent):
-  global tlb_find, tlb_regexp, tlb_case
-  global dlg_tags_shown, dlg_tags_sel, patlist, fmt_find
-
   if tlb_find.get() != "":
     # search a free tag index
     dup_idx = -1
     nam_idx = 0
     idx = 0
     for w in patlist:
       tag_idx = int(w[4][3:]) # parse tag name: "tag%d"
@@ -5783,39 +5580,35 @@
 
 
 #
 # This function is invoked by the "Copy to search field" command in the
 # highlight list's context menu.
 #
 def TagList_CopyToSearch(pat_idx):
-  global patlist
-  global tlb_find_focus, tlb_find, tlb_regexp, tlb_case
+  global tlb_find_focus
 
   if pat_idx < len(patlist):
     w = patlist[pat_idx]
 
     # force focus into find entry field & suppress "Enter" event
     SearchInit()
-    tlb_find_focus = 1
+    tlb_find_focus = True
     wt.f2_e.focus_set()
 
     SearchHighlightClear()
     tlb_find.set(w[0])
     tlb_regexp.set(w[1])
     tlb_case.set(w[2])
 
 
 #
 # This function is invoked by the "Update from search field" command in the
 # highlight list's context menu.
 #
 def TagList_CopyFromSearch(pat_idx):
-  global tlb_find_focus, tlb_find, tlb_regexp, tlb_case
-  global patlist
-
   if pat_idx < len(patlist):
     answer = messagebox.askokcancel(parent=wt.dlg_tags, message="Please confirm overwriting the search pattern for this entry? This cannot be undone")
     if answer:
       w = patlist[pat_idx]
       w[0] = tlb_find.get()
       w[1] = int(tlb_regexp.get())
       w[2] = int(tlb_case.get())
@@ -5833,16 +5626,14 @@
 
 
 #
 # This function is invoked by the "Remove entry" command in the highlight
 # list's context menu.
 #
 def TagList_Remove(pat_sel):
-  global patlist
-
   cnt = len(pat_sel)
   if cnt > 0:
     if cnt == 1:
       msg = "Really remove this entry? This cannot be undone"
     else:
       msg = "Really remove all %d selected entries? This cannot be undone" % cnt
 
@@ -5867,28 +5658,26 @@
       dlg_tags_sel.TextSel_SetSelection([])
 
 
 #
 # This function is bound to the "Delete" key in the highlight list.
 #
 def TagList_RemoveSelection():
-  global dlg_tags_sel
-
   sel = dlg_tags_sel.TextSel_GetSelection()
   if len(sel) > 0:
     TagList_Remove(sel)
 
 
 # ----------------------------------------------------------------------------
 #
 # This function creates or raises the font selection dialog.
 #
 def FontList_OpenDialog():
-  global font_normal, font_content, dlg_font_shown
-  global dlg_font_fams, dlg_font_size, dlg_font_bold
+  global dlg_font_shown
+  global dlg_font_bold, dlg_font_size
 
   PreemptBgTasks()
   if not dlg_font_shown:
     wt.dlg_font = Toplevel(tk)
     wt.dlg_font.wm_title("Font selection")
     wt.dlg_font.wm_group(tk)
 
@@ -5973,31 +5762,29 @@
 
 
 #
 # This function fills the font selection listbox with  list of all
 # font families which are available on the system.
 #
 def FontList_Fill():
-  global dlg_font_fams, dlg_font_size, dlg_font_bold
+  global dlg_font_fams
 
   # remove duplicates, then sort alphabetically
   dlg_font_fams = sorted(set(tkf.families(displayof=tk)))
 
   for f in dlg_font_fams:
     wt.dlg_font_f1_fams.insert("end", f)
 
 
 #
 # This function is bound to changes of the selection in the font list
 # or changes in the size and weight controls.  The function applies
 # the selection to the demo text.
 #
 def FontList_Selection():
-  global dlg_font_fams, dlg_font_size, dlg_font_bold
-
   sel = wt.dlg_font_f1_fams.curselection()
   if (len(sel) == 1) and (sel[0] < len(dlg_font_fams)):
     name = "{%s} %d" % (dlg_font_fams[sel[0]], dlg_font_size.get())
     if dlg_font_bold.get():
       name = name + " bold"
 
     # note this succeeds even for unknown fonts, so no try/except needed
@@ -6007,15 +5794,14 @@
 #
 # This function is bound to the "Ok" and "Abort" command buttons.
 # In case of OK the function checks and stores the selection.
 # In case of abort, the function just closes the dialog.
 #
 def FontList_Quit(do_store):
   global dlg_font_fams, dlg_font_size, dlg_font_bold
-  global font_content
 
   if do_store:
     sel = wt.dlg_font_f1_fams.curselection()
     if (len(sel) == 1) and (sel[0] < len(dlg_font_fams)):
       font_content.configure(family=dlg_font_fams[sel[0]],
                              size=dlg_font_size.get(),
                              weight=(tkf.BOLD if dlg_font_bold.get() else tkf.NORMAL))
@@ -6036,18 +5822,15 @@
 
 
 # ----------------------------------------------------------------------------
 #
 # This function creates or raises the color highlight edit dialog.
 #
 def Markup_OpenDialog(pat_idx):
-  global font_normal, font_bold, font_content, font_hlink
-  global col_bg_content, col_fg_content
-  global fmt_selection, dlg_fmt_shown, dlg_fmt
-  global patlist, col_palette
+  global dlg_fmt_shown
 
   # fail-safety
   if pat_idx >= len(patlist): return
   Markup_InitConfig(pat_idx)
 
   if not dlg_fmt_shown:
     wt.dlg_fmt = Toplevel(tk)
@@ -6202,15 +5985,15 @@
   dlg_fmt_shown = False
 
 #
 # This function is called when the mark-up dialog is opened to copy the
 # format parameters from the global patlist into the dialog's hash array.
 #
 def Markup_InitConfig(pat_idx):
-  global patlist, dlg_fmt
+  global dlg_fmt
 
   dlg_fmt = {}
 
   w = patlist[pat_idx]
   dlg_fmt["pat"] = StringVar(tk, w[0])
   dlg_fmt["regexp"] = BooleanVar(tk, w[1])
   dlg_fmt["mcase"] = BooleanVar(tk, w[2])
@@ -6228,16 +6011,14 @@
 
 
 #
 # This function is called when the mark-up dialog is closed to build a
 # parameter list from the dialog's temporary hash array.
 #
 def Markup_GetConfig(pat_idx):
-  global dlg_fmt, patlist
-
   if pat_idx >= 0:
     w = patlist[pat_idx]
   else:
     w = [""] * 16
 
   bgpat = dlg_fmt["bgpat"].get()
   fgpat = dlg_fmt["fgpat"].get()
@@ -6268,15 +6049,15 @@
   return w
 
 
 #
 # This function is bound to the "Ok" and "Abort" buttons in the mark-up dialog.
 #
 def Markup_Save(do_save, do_quit):
-  global dlg_fmt, patlist
+  global dlg_fmt
 
   if do_save:
     # determine the edited pattern's index in the list (use the unique tag
     # which doesn't change even if the list is reordered)
     pat_idx = -1
     tagnam = dlg_fmt["tagnam"]
     idx = 0
@@ -6323,27 +6104,24 @@
 
 
 #
 # This function is called whenever a format parameter is changed to update
 # the sample text and the control widgets.
 #
 def Markup_UpdateFormat():
-  global dlg_fmt, font_content, col_bg_content, col_fg_content
-
   HighlightConfigure(wt.dlg_fmt_sample, "sample", Markup_GetConfig(-1))
 
   if dlg_fmt["relief"].get() != "none":
     wt.dlg_fmt_mb_bdw_sb.configure(state=NORMAL)
   else:
     wt.dlg_fmt_mb_bdw_sb.configure(state=DISABLED)
 
   # adjust spacing above first line to center the content vertically
   lh = font_content.metrics("linespace")
-  spc = lh - dlg_fmt["spacing"].get()
-  if spc < 0: spc = 0
+  spc = max(lh - dlg_fmt["spacing"].get(), 0)
   wt.dlg_fmt_sample.tag_configure("spacing", spacing1=spc)
 
   # update the entry widgets
   if dlg_fmt["bgcol"].get() != "":
     wt.dlg_fmt_mb_bgcol_mb.wid_c.configure(background=dlg_fmt["bgcol"].get())
   else:
     wt.dlg_fmt_mb_bgcol_mb.wid_c.configure(background=col_bg_content)
@@ -6368,82 +6146,77 @@
 
 #
 # This function is used during creation of the markup editor dialog to
 # create the widgets for color, pattern and relief selection. The widget
 # consists of a rectangle which displays the current choice and a button
 # which triggers a popup menu when pressed.
 #
-class Markup_ImageButton(object):
-  def __init__(self, parent, type):
-    global dlg_fmt
-
+class Markup_ImageButton:
+  def __init__(self, parent, wid_type):
     CreateButtonBitmap("img_dropdown")
     self.wid = Frame(parent, relief=SUNKEN, borderwidth=1)
     iw = tk.call("image", "width", "img_dropdown") + 4
     ih = tk.call("image", "height", "img_dropdown")
     self.wid_c = Canvas(self.wid, width=iw, height=ih, highlightthickness=0, takefocus=0, borderwidth=0)
     self.wid_c.pack(fill=BOTH, expand=1, side=LEFT)
     self.wid_b = Button(self.wid, image="img_dropdown", highlightthickness=1, borderwidth=1, relief=RAISED)
     self.wid_b.pack(side=LEFT)
     self.wid_men = Menu(self.wid, tearoff=0)
 
-    if type.endswith("col"):
-      self.wid_b.configure(command=lambda:Markup_PopupColorPalette(self.wid, type))
-    elif type.endswith("pat"):
+    if wid_type.endswith("col"):
+      self.wid_b.configure(command=lambda:Markup_PopupColorPalette(self.wid, wid_type))
+    elif wid_type.endswith("pat"):
       self.wid_c.create_bitmap(2, 2, anchor="nw")
       self.wid_b.configure(command=lambda:Markup_PopupPatternMenu(self.wid, self.wid_men))
-    elif type == "relief":
+    elif wid_type == "relief":
       self.wid_c_w = Frame(self.wid_c, width=10, height=10, borderwidth=2, relief=FLAT)
       self.wid_c.create_window(3, 3, anchor="nw", window=self.wid_c_w, width=12, height=12)
       self.wid_b.configure(command=lambda:Markup_PopupPatternMenu(self.wid, self.wid_men))
 
 
 #
 # This helper function is invoked when the "drop down" button is pressed
-# on a color selction widget: it opens the color palette menu directly
+# on a color selection widget: it opens the color palette menu directly
 # below the widget.
 #
-def Markup_PopupColorPalette(wid, type):
-  global dlg_fmt
-
+def Markup_PopupColorPalette(wid, wid_type):
   rootx = wid.winfo_rootx()
   rooty = wid.winfo_rooty() + wid.winfo_height()
   PaletteMenu_Popup(wt.dlg_fmt, rootx, rooty,
-                    lambda col:Markup_UpdateColor(col, type, 0),
-                    dlg_fmt[type].get())
+                    lambda col:Markup_UpdateColor(wid_type, col),
+                    dlg_fmt[wid_type].get())
 
 
 #
 # This helper function is invoked when the "drop down" button is pressed
-# on a pattern selction widget: it opens the associated menu directly
+# on a pattern selection widget: it opens the associated menu directly
 # below the widget.
 #
 def Markup_PopupPatternMenu(wid, wid_men):
   rootx = wid.winfo_rootx()
   rooty = wid.winfo_rooty() + wid.winfo_height()
   tk.call("tk_popup", wid_men, rootx, rooty, 0)
 
 
 #
 # This helper function is invoked as callback after a color was selected
 # in the palette popup menu.
 #
-def Markup_UpdateColor(col, type, is_fg):
-  dlg_fmt[type].set(col)
+def Markup_UpdateColor(wid_type, col):
+  dlg_fmt[wid_type].set(col)
   Markup_UpdateFormat()
 
 
 # ----------------------------------------------------------------------------
 #
 # This function creates or raises the color palette dialog which allows to
 # add, delete, modify or reorder colors used for highlighting.
 #
 def Palette_OpenDialog():
-  global font_normal, dlg_cols_shown, dlg_cols_palette, dlg_cols_cid
-  global col_palette
+  global dlg_cols_shown, dlg_cols_palette, dlg_cols_cid
 
   if not dlg_cols_shown:
     wt.dlg_cols = Toplevel(tk)
     wt.dlg_cols.wm_title("Color palette")
     wt.dlg_cols.wm_group(tk)
 
     msg = "Pre-define a color palette for quick selection\n" \
@@ -6456,24 +6229,26 @@
     wt.dlg_cols_c.pack(side=TOP, padx=10, pady=10, anchor=W)
 
     wt.dlg_cols_c.bind("<ButtonRelease-3>", lambda e: Palette_ContextMenu(e.x, e.y))
     wt.dlg_cols_c.bind("<Destroy>", lambda e: Palette_ClosedDialog(), add="+")
     dlg_cols_shown = True
 
     wt.dlg_cols_f2 = Frame(wt.dlg_cols)
-    wt.dlg_cols_f2_abort = Button(wt.dlg_cols_f2, text="Abort", command=lambda:Palette_Save(0))
-    wt.dlg_cols_f2_ok = Button(wt.dlg_cols_f2, text="Ok", default="active", command=lambda:Palette_Save(1))
+    wt.dlg_cols_f2_abort = Button(wt.dlg_cols_f2, text="Abort", command=lambda:Palette_Save(False))
+    wt.dlg_cols_f2_ok = Button(wt.dlg_cols_f2, text="Ok", default="active", command=lambda:Palette_Save(True))
     wt.dlg_cols_f2_abort.pack(side=LEFT, padx=10, pady=5)
     wt.dlg_cols_f2_ok.pack(side=LEFT, padx=10, pady=5)
     wt.dlg_cols_f2.pack(side=TOP)
 
     wt.dlg_cols_ctxmen = Menu(wt.dlg_cols, tearoff=0)
 
-    dlg_cols_palette = col_palette
-    Palette_Fill(wt.dlg_cols_c, dlg_cols_palette)
+    dlg_cols_palette = col_palette.copy()
+    dlg_cols_cid = []
+
+    Palette_Fill(wt.dlg_cols_c, dlg_cols_palette, dlg_cols_cid)
 
   else:
     wt.dlg_cols.wm_deiconify()
     wt.dlg_cols.lift()
 
 
 #
@@ -6485,162 +6260,148 @@
   dlg_cols_shown = False
 
 #
 # This function fills the color palette canvas with rectangles which
 # each display one of the currently defined colors. Each rectangle gets
 # mouse bindings for a context menu and changing the order of colors.
 #
-def Palette_Fill(wid, pal, sz=20, sel_cmd=None):
-  global dlg_cols_cid
-
+def Palette_Fill(wid, palette, cids, sz=20, sel_cmd=None):
   wid.delete("all")
-  dlg_cols_cid = []
+  del cids[0:]
 
   x = 2
   y = 2
   col_idx = 0
   idx = 0
-  for col in pal:
+  for col in palette:
     cid = wid.create_rectangle(x, y, x + sz, y + sz,
                                outline="black", fill=col,
                                activeoutline="black", activewidth=2)
-    dlg_cols_cid.append(cid)
+    cids.append(cid)
 
     if sel_cmd is None:
       wid.tag_bind(cid, "<Double-Button-1>", lambda e, idx=idx, cid=cid: Palette_EditColor(idx, cid))
-      wid.tag_bind(cid, "<B1-Motion>", lambda e, idx=idx, cid=cid: Palette_MoveColor(idx, cid, e.x, e.y))
-      wid.tag_bind(cid, "<ButtonRelease-1>", lambda e, idx=idx, cid=cid: Palette_MoveColorEnd(idx, cid, e.x, e.y))
+      wid.tag_bind(cid, "<B1-Motion>", lambda e, idx=idx, cid=cid: Palette_MoveColor(cid, e.x, e.y))
+      wid.tag_bind(cid, "<ButtonRelease-1>", lambda e, idx=idx, cid=cid: Palette_MoveColorEnd(idx, e.x, e.y))
     else:
       wid.tag_bind(cid, "<Button-1>", lambda e, col=col: sel_cmd(col))
 
     x += sz
     col_idx += 1
     if col_idx >= 10:
       y += sz
       x = 2
       col_idx = 0
 
     idx += 1
 
   wid.configure(width=(10 * sz + 3+3),
-                height=(int((len(pal) + 10-1) / 10) * sz + 2+2))
+                height=(int((len(palette) + 10-1) / 10) * sz + 2+2))
 
 
 #
 # This function is bound to right mouse clicks on color items.
 #
 def Palette_ContextMenu(xcoo, ycoo):
-  global dlg_cols_palette, dlg_cols_cid
-
   cid = wt.dlg_cols_c.find("closest", xcoo, ycoo)
   if len(cid) == 1:
     cid = cid[0]
     for idx in range(len(dlg_cols_cid)):
       if dlg_cols_cid[idx] == cid:
         break
     else:
       return
 
     wt.dlg_cols_ctxmen.delete(0, "end")
     wt.dlg_cols_ctxmen.add_command(label="", background=dlg_cols_palette[idx], state=DISABLED)
     wt.dlg_cols_ctxmen.add_separator()
     wt.dlg_cols_ctxmen.add_command(label="Change this color...", command=lambda:Palette_EditColor(idx, cid))
-    wt.dlg_cols_ctxmen.add_command(label="Duplicate this color", command=lambda:Palette_DuplicateColor(idx, cid))
-    wt.dlg_cols_ctxmen.add_command(label="Insert new color (white)", command=lambda:Palette_InsertColor(idx, cid))
+    wt.dlg_cols_ctxmen.add_command(label="Duplicate this color", command=lambda:Palette_DuplicateColor(idx))
+    wt.dlg_cols_ctxmen.add_command(label="Insert new color (white)", command=lambda:Palette_InsertColor(idx))
     wt.dlg_cols_ctxmen.add_separator()
     wt.dlg_cols_ctxmen.add_command(label="Remove this color", command=lambda: Palette_RemoveColor(idx))
 
     rootx = wt.dlg_cols.winfo_rootx() + xcoo
     rooty = wt.dlg_cols.winfo_rooty() + ycoo
     tk.call("tk_popup", wt.dlg_cols_ctxmen, rootx, rooty, 0)
 
 
 #
 # This function is bound to the "remove this color" menu item in the
 # color palette context menu.
 #
 def Palette_RemoveColor(idx):
-  global dlg_cols_palette
-
   if idx < len(dlg_cols_palette):
     del dlg_cols_palette[idx]
-    Palette_Fill(wt.dlg_cols_c, dlg_cols_palette)
+    Palette_Fill(wt.dlg_cols_c, dlg_cols_palette, dlg_cols_cid)
 
 
 #
 # This function is bound to the "insert new color" menu item in the
 # color palette entries. It inserts an white color entry at the mouse
 # pointer position.
 #
-def Palette_InsertColor(idx, cid):
-  global dlg_cols_palette
-
+def Palette_InsertColor(idx):
   dlg_cols_palette.insert(idx, "#ffffff")
-  Palette_Fill(wt.dlg_cols_c, dlg_cols_palette)
+  Palette_Fill(wt.dlg_cols_c, dlg_cols_palette, dlg_cols_cid)
 
 
-def Palette_DuplicateColor(idx, cid):
-  global dlg_cols_palette
-
+def Palette_DuplicateColor(idx):
   if idx < len(dlg_cols_palette):
     col = dlg_cols_palette[idx]
     dlg_cols_palette.insert(idx, col)
-    Palette_Fill(wt.dlg_cols_c, dlg_cols_palette)
+    Palette_Fill(wt.dlg_cols_c, dlg_cols_palette, dlg_cols_cid)
 
 
 #
 # This function is bound to the "edit this color" menu item in the
 # color palette context menu.
 #
 def Palette_EditColor(idx, cid):
-  global dlg_cols_palette
-
   col = dlg_cols_palette[idx]
   col = colorchooser.askcolor(initialcolor=col, parent=wt.dlg_cols, title="Select color")
   if col is not None:
     col = col[1]
     dlg_cols_palette[idx] = col
     wt.dlg_cols_c.itemconfigure(cid, fill=col)
 
 
 #
 # This function is bound to motion events on color palette entries while
 # the left mouse button is helt down.
 #
-def Palette_MoveColor(idx, cid, xcoo, ycoo):
+def Palette_MoveColor(cid, xcoo, ycoo):
   sz = 20
   sz_2 = 0 - (sz /2)
   xcoo += sz_2
   ycoo += sz_2
   wt.dlg_cols_c.tag_raise(cid)
   wt.dlg_cols_c.coords(xcoo + sz, ycoo + sz)
 
 
 #
 # This function is bound to the mouse button release event on color palette
 # entries. It's used to change the order of colors by drag-and-drop.
 #
-def Palette_MoveColorEnd(idx, cid, xcoo, ycoo):
-  global dlg_cols_palette
-
+def Palette_MoveColorEnd(idx, xcoo, ycoo):
   sz = 20
   xcoo -= 2
   ycoo -= 2
   col_idx = 0 if xcoo < 0 else xcoo // sz
   row_idx = 0 if ycoo < 0 else ycoo // sz
 
   new_idx = (row_idx * 10) + col_idx
   col = dlg_cols_palette[idx]
   del dlg_cols_palette[idx]
   if new_idx < len(dlg_cols_palette):
     dlg_cols_palette.insert(new_idx, col)
   else:
     dlg_cols_palette.append(col)
 
-  Palette_Fill(wt.dlg_cols_c, dlg_cols_palette)
+  Palette_Fill(wt.dlg_cols_c, dlg_cols_palette, dlg_cols_cid)
 
 
 #
 # This function is bound to the "ok" and "abort" buttons. Ths function
 # closes the color palette dialog. In case of "ok" the edited palette
 # is stored.
 #
@@ -6657,16 +6418,14 @@
 
 
 #
 # This function creates a menu with all the colors. It's usually used as
 # sub-menu (i.e. cascade) in other menus.
 #
 def PaletteMenu_Popup(parent, rootx, rooty, cmd, col_def):
-  global col_palette, font_hlink
-
   wt.colsel = Toplevel(tk, highlightthickness=0)
   wt.colsel.wm_title("Color selection menu")
   wt.colsel.wm_transient(parent)
   wt.colsel.wm_geometry("+%d+%d" % (rootx, rooty))
   wt.colsel.wm_resizable(0, 0)
 
   wt.colsel_c = Canvas(wt.colsel, background=wt.colsel.cget("background"),
@@ -6681,15 +6440,16 @@
   wt.colsel_f1_b_other.pack(side=LEFT, expand=1, anchor=W)
   wt.colsel_f1_b_none = Button(wt.colsel_f1, text="None", command=lambda:cmd(""),
                                borderwidth=0, relief=FLAT, font=font_hlink,
                                foreground="#0000ff", activeforeground="#0000ff", padx=0, pady=0)
   wt.colsel_f1_b_none.pack(side=LEFT, expand=1, anchor=E)
   wt.colsel_f1.pack(side=TOP, fill=X, expand=1)
 
-  Palette_Fill(wt.colsel_c, col_palette, 15, cmd)
+  cids = []
+  Palette_Fill(wt.colsel_c, col_palette, cids, 15, cmd)
 
   wt.colsel.bind("<ButtonRelease-1>", lambda e: wt.colsel.destroy())
   wt.colsel_c.focus_set()
   wt.colsel.grab_set()
 
 
 #
@@ -6709,28 +6469,26 @@
 
 
 # ----------------------------------------------------------------------------
 #
 # This function creates the "About" dialog with copyleft info
 #
 def OpenAboutDialog():
-  global font_normal, font_bold
-
   PreemptBgTasks()
   if not wt_exists(wt.about):
     wt.about = Toplevel(tk)
     wt.about.wm_title("About")
     wt.about.wm_group(tk)
     wt.about.wm_transient(tk)
     wt.about.wm_resizable(1, 1)
 
     wt.about_name = Label(wt.about, text="Trace Browser", font=font_bold)
     wt.about_name.pack(side=TOP, padx=5, pady=5)
 
-    wt.about_copyr1 = Label(wt.about, text="Version 2.1\n"
+    wt.about_copyr1 = Label(wt.about, text="Version 2.2\n"
                                            "Copyright (C) 2007-2010,2019-2020,2023 T. Zoerner")
     wt.about_copyr1.pack(side=TOP, padx=5)
 
     url = "https://github.com/tomzox/trowser"
     wt.about_url = Label(wt.about, text=url, fg="blue", cursor="top_left_arrow")
     wt.about_url.pack(side=TOP, padx=5, pady=5)
 
@@ -6772,15 +6530,15 @@
 # - callback to invoke after selection changes
 # - callback which provides the content list length
 # - ID of "after" event handler while scrolling via mouse, or None
 # - scrolling speed
 # - anchor element index OR last selection cursor pos
 # - list of indices of selected lines (starting at zero)
 #
-class TextSel(object):
+class TextSel:
   #
   # This constructor is called after a text widget is created for initializing
   # all member variables and for adding key and mouse event bindings for
   # handling the selection.
   #
   def __init__(self, wid, cb_proc, len_proc, mode):
     self.wid = wid
@@ -7155,14 +6913,15 @@
       self.cb_proc(self.sel)
 
 
   #
   # This helper function is used to build a list of all indices between
   # (and including) two given values in increasing order.
   #
+  @staticmethod
   def IdxRange(start, end):
     if start > end:
       return list(range(end, start + 1))
     else:
       return list(range(start, end + 1))
 
 
@@ -7236,46 +6995,48 @@
 # This helper function is installed as "selection handler" on a dummy widget in
 # the main window. The function simply returns a text that was previously
 # stored for export via the selection. After storing a new text the selection
 # must be set to be "owned" by the dummy widget, so that it gets querues by the
 # X window system.
 #
 def TextSel_XselectionHandler(off, xlen):
-  global main_selection_txt
   try:
       off = int(off)
       xlen = int(xlen)
       return main_selection_txt[off : (off + xlen)]
   except:
       return ""
 
 
 #
 # This function can be called to copy the given text to the clipboard (from
 # where it can by retrieved by other applications, usually upon "paste"
 # commands by the user) and X selection mechanism (from where the user can
 # paste it via click with the middle mouse button).
 #
-def TextSel_XselectionExport(to_clipboard, str):
+def TextSel_XselectionExport(to_clipboard, txt):
   global main_selection_txt
 
   # update X selection
-  main_selection_txt = str
+  main_selection_txt = txt
   wt.xselection.selection_own()
 
   if to_clipboard:
     tk.clipboard_clear()
-    tk.clipboard_append(str)
+    tk.clipboard_append(txt)
 
 
 # ----------------------------------------------------------------------------
 
-class LoadPipe(object):
+class LoadPipe:
   def __init__(self):
-    global load_file_mode
+    global load_buf_size
+
+    if not load_buf_size:
+      load_buf_size = load_buf_size_default
 
     self._opt_file_close = IntVar(tk, 0)             # option configurable via dlg.
     self._opt_file_mode = IntVar(tk, load_file_mode) # copy of cfg. opt. for display
     self._dlg_read_total = IntVar(tk, 0)     # copy of _read_total for display
     self._dlg_read_buffered = IntVar(tk, 0)  # copy of _read_buffered for display
     self._dlg_file_limit = IntVar(tk, (load_buf_size + (1024*1024-1)) // (1024*1024))
 
@@ -7296,15 +7057,15 @@
     self._ctrl_upd_cnf = 0
 
 
   #
   # This function opens the "Loading from STDIN" status dialog.
   #
   def LoadPipe_OpenDialog(self):
-    global font_normal, dlg_load_shown
+    global dlg_load_shown
 
     if not dlg_load_shown:
       wt.dlg_load = Toplevel(tk)
       wt.dlg_load.wm_title("Loading from STDIN...")
       wt.dlg_load.wm_group(tk)
       wt.dlg_load.wm_transient(tk)
       xcoo = wt.f1_t.winfo_rootx() + 50
@@ -7410,26 +7171,28 @@
       self._thr_cv.notify()
 
 
   #
   # This function is bound to the "Ok" button in the "Load from pipe"
   #
   def LoadPipe_CmdContinue(self):
-    global load_buf_size, load_file_mode
+    global load_buf_size, load_buf_size_default, load_file_mode
 
     # apply possible change of buffer mode and limit by the user
     load_file_mode = self._opt_file_mode.get()
     try:
       val = 1024*1024 * int(self._dlg_file_limit.get())
     except:
       tk.after_idle(lambda:messagebox.showerror(parent=tk, message="Buffer size is not a number: " + self._dlg_file_limit.get()))
       return
 
     if abs(val - load_buf_size) >= 1024*1024:
       load_buf_size = val
+
+      load_buf_size_default = val
       UpdateRcAfterIdle()
 
     if (self._opt_file_mode.get() == 0) and (self._read_buffered >= load_buf_size):
       # "head" mode confirmed by user and buffer is full -> close the dialog
       self.LoadPipe_Insert(False)
     else:
       self.LoadPipe_DialogConfigure(False)
@@ -7444,16 +7207,14 @@
   # This function discards data in the load buffer queue if the length
   # limit is exceeded.  The buffer queue is an array of character strings
   # (each string the result of a "read" command.)  The function is called
   # after each read in tail mode, so it must be efficient (i.e. esp. avoid
   # copying large buffers.)
   #
   def LoadPipe_LimitData(self, exact):
-    global load_buf_size
-
     # tail mode: delete oldest data / head mode: delete newest data
     if load_file_mode == 0:
       lidx = -1
     else:
       lidx = 0
 
     # calculate how much data must be discarded
@@ -7483,24 +7244,22 @@
 
 
   #
   # This function is installed as handler for asynchronous read events
   # when reading text data from STDIN, i.e. via a pipe.
   #
   def LoadPipe_BgLoop(self):
-    global load_buf_size
-
     try:
       while True:
         # limit read length to buffer size ("head" mode only)
         with self._thr_lock:
           while self._thr_ctrl == 1:
             self._thr_cv.wait()
           if self._thr_ctrl == 2:
-            break;
+            break
 
           size = 64000
           if (load_file_mode == 0) and (self._read_buffered + size > load_buf_size):
             size = load_buf_size - self._read_buffered
 
         if size > 0:
           data = sys.stdin.read(size)
@@ -7656,35 +7415,37 @@
 
 
 # ----------------------------------------------------------------------------
 #
 # This function loads a text file (or parts of it) into the text widget.
 #
 def LoadFile(filename):
-  global cur_filename, load_pipe, load_buf_size, load_file_mode
+  global cur_filename, load_pipe
 
   cur_filename = filename
   load_pipe = None
 
   try:
-    file = open(filename, "rb")
+    with open(filename, "rb") as infile:
+      if load_buf_size:
+        # apply head/tail mode and length limit
+        stat = os.fstat(infile.fileno())
+        if load_file_mode and (stat.st_size > load_buf_size):
+          # FIXME this won't work well on a file containing UTF
+          infile.seek(0 - load_buf_size, 2)
 
-    # apply file length limit
-    stat = os.fstat(file.fileno())
-    if load_file_mode and (stat.st_size > load_buf_size):
-      file.seek(0 - load_buf_size, 2)
-
-    # insert the data into the text widget
-    data = file.read(load_buf_size)
-    file.close()
+        data = infile.read(load_buf_size)
+      else:
+        data = infile.read()
 
   except OSError as e:
     messagebox.showerror(message="Failed to load file %s: %s" % (filename, e.strerror))
     data = b""
 
+  # insert the data into the text widget
   wt.f1_t.insert("end", data)
 
   # add missing newline at end of file
   if data and (data[-1] != b"\n"[0]):
     wt.f1_t.insert("end", "\n")
 
   InitContent()
@@ -7692,15 +7453,14 @@
 
 #
 # This function initializes the text widget and control state for a
 # newly loaded text.
 #
 def InitContent():
   global tid_search_inc, tid_search_hall, tid_high_init
-  global cur_filename, load_pipe, dlg_mark_shown
 
   if tid_high_init is not None: tk.after_cancel(tid_high_init)
   if tid_search_inc is not None: tk.after_cancel(tid_search_inc)
   if tid_search_hall is not None: tk.after_cancel(tid_search_hall)
   tid_high_init = None
   tid_search_inc = None
   tid_search_hall = None
@@ -7723,30 +7483,30 @@
 
   # switch from "watch" to default cursor
   wt.f1_t.configure(cursor="top_left_arrow")
   # set cursor to the end of file
   wt.f1_t.mark_set("insert", "end")
   CursorMoveLine(wt.f1_t, 0)
 
-  global cur_jump_stack
+  global cur_jump_stack, cur_jump_idx
   cur_jump_stack = []
   cur_jump_idx = -1
   # read bookmarks from the default file
   Mark_ReadFileAuto()
   # start color highlighting in the background
   HighlightInit()
 
 
 #
 # This procedure discards all text content and aborts all ongoing
 # activity and timers. The function is called before new data is
 # loaded.
 #
 def DiscardContent():
-  global patlist, mark_list, mark_list_modified
+  global mark_list, mark_list_modified
 
   # the following is a work-around for a performance issue in the text widget:
   # deleting text with large numbers of tags is extremely slow, so we clear
   # the tags first (needed for Tcl/Tk 8.4.7)
   for w in patlist:
     wt.f1_t.tag_remove(w[4], "1.0", "end")
 
@@ -7764,16 +7524,14 @@
 
 
 #
 # This function is bound to the "Discard content" menu commands.
 # The parameter specifies if content above or below the cursor is discarded.
 #
 def MenuCmd_Discard(is_fwd):
-  global cur_filename
-
   PreemptBgTasks()
   if is_fwd:
     # delete everything below the line holding the cursor
     (first_l, first_c) = map(int, wt.f1_t.index("insert +1 lines linestart").split("."))
     (last_l, last_c) = map(int, wt.f1_t.index("end").split("."))
     count = last_l - first_l
     if (last_c == 0) and (count > 0):
@@ -7813,15 +7571,14 @@
     if answer:
       if SearchList_SearchAbort():
         SearchHighlightClear()
 
         # the following is a work-around for a performance issue in the text widget:
         # deleting text with large numbers of tags is extremely slow, so we clear
         # the tags first (needed as of Tcl/Tk 8.4.7 to .13)
-        global patlist
         for w in patlist:
           wt.f1_t.tag_remove(w[4], "%d.%d" % (first_l, first_c), "%d.%d" % (last_l, last_c))
 
         # perform the removal
         wt.f1_t.delete("%d.%d" % (first_l, first_c), "%d.%d" % (last_l, last_c))
 
         # re-start initial highlighting, if not complete yet
@@ -7840,15 +7597,17 @@
         SearchList_AdjustLineNums(1 if is_fwd else last_l, first_l if is_fwd else 0)
 
 
 #
 # This function is bound to the "Reload current file" menu command.
 #
 def MenuCmd_Reload():
-  global load_pipe, cur_filename
+  # offer to save old bookmarks before discarding them below
+  if not Mark_OfferSave():
+    return
 
   if load_pipe is not None:
     if not load_pipe.is_eof:
       DiscardContent()
       tk.after_idle(lambda: load_pipe.LoadPipe_Start())
   else:
     DiscardContent()
@@ -7858,41 +7617,45 @@
 #
 # This function is bound to the "Load file" menu command.  The function
 # allows to specify a file from which a new trace is read. The current browser
 # contents are discarded and all bookmarks are cleared.
 #
 def MenuCmd_OpenFile():
   # offer to save old bookmarks before discarding them below
-  Mark_OfferSave()
+  if not Mark_OfferSave():
+    return
 
-  filename = filedialog.askopenfilename(parent=tk, filetypes=(("trace", "out.*"), ("all", "*")))
+  filename = filedialog.askopenfilename(parent=tk, filetypes=(("all", "*"),
+                                                              ("log", "*.log"),
+                                                              ("trace", "trace.*")))
   if filename:
     DiscardContent()
     tk.after_idle(lambda: LoadFile(filename))
 
 
 #
 # This function is installed as callback for destroy requests on the
 # main window to store the search history and bookmarks.
 #
 def UserQuit():
   UpdateRcFile()
-  Mark_OfferSave()
+  if not Mark_OfferSave():
+    return
   tk.destroy()
   sys.exit(0)
 
 
 #
 # This function sets a global flag which makes background tasks sleep
 # for a short time so that an interactive task can be completed. It's
 # essential that ResumeBgTasks is called afterwards and that the caller
 # doesn't block.
 #
 def PreemptBgTasks():
-  global block_bg_tasks, block_bg_caller, tid_resume_bg
+  global block_bg_tasks, tid_resume_bg
 
   block_bg_caller.append(["LOCK", traceback.format_tb(sys.exc_info()[2], limit=-2)])
   if tid_resume_bg is not None:
     # no incr in this case b/c resume was called, but decr delayed
     block_bg_tasks = 1
     tk.after_cancel(tid_resume_bg)
     tid_resume_bg = None
@@ -7903,45 +7666,45 @@
 #
 # This function allows background tasks to resume after all pending events
 # have been processed.  Note the extra delay via idle and additional timer
 # is required to make sure all X events (e.g. from opening a new dialog
 # window) have been processed.
 #
 def ResumeBgTasks():
-  global block_bg_tasks, block_bg_caller, tid_resume_bg
+  global block_bg_tasks, tid_resume_bg
 
   if block_bg_tasks > 1:
     block_bg_caller.append(["DEC #"+str(block_bg_tasks), traceback.format_tb(sys.exc_info()[2], limit=-2)])
     block_bg_tasks -= 1
   else:
     block_bg_caller.append(["UNLOCK", traceback.format_tb(sys.exc_info()[2], limit=-2)])
     if tid_resume_bg is not None: tk.after_cancel(tid_resume_bg)
-    tid_resume_bg = tk.after_idle(lambda: ClearBgTasks(1))
+    tid_resume_bg = tk.after_idle(lambda: ClearBgTasks(True))
 
 
 #
 # This function is installed as idle and timer event to finally allow
 # background tasks to resume.  The handler once re-installs itself via
 # a timer to make extra-sure all pending activity is done.  Note the
 # whole procedure is similar to calling "update" (which is avoided
 # though because it inflicts race conditions.)
 #
 def ClearBgTasks(flag):
-  global block_bg_tasks, tid_resume_bg
+  global block_bg_tasks, block_bg_caller, tid_resume_bg
 
   if flag:
     if block_bg_tasks == 0:
       print("Warning: nested call of ResumeBgTasks(?) - internal error", file=sys.stderr)
     else:
       block_bg_tasks -= 1
       block_bg_caller = []
 
     tid_resume_bg = None
   else:
-    tid_resume_bg = tk.after(250, lambda: ClearBgTasks(0))
+    tid_resume_bg = tk.after(250, lambda: ClearBgTasks(False))
 
 
 #
 # This helper function is installed as post command for all menu popups
 # so that idle-event driven background tasks are shortly suspended while
 # a menu popup is displayed. Without this the GUI may freeze until the
 # background task has finished.
@@ -7967,17 +7730,17 @@
 def DebugDumpAllState():
   print("#--- debug dump of scalars and lists ---#", file=sys.stderr)
   for (var,val) in globals().items():
     if not var.startswith("__"):
       print(var, "=", val, file=sys.stderr)
 
   print("#--- debug dump of tasks ---#", file=sys.stderr)
-  for id in tk.call("after", "info"):
+  for tid in tk.call("after", "info"):
     try:
-      print(id, "=", tk.call("after", "info", id))
+      print(tid, "=", tk.call("after", "info", tid))
     except:
       pass
 
 
 # ----------------------------------------------------------------------------
 # The following data is automatically generated - do not edit
 # Generated by ./tools/pod2help.py from doc/trowser.pod
@@ -7994,19 +7757,19 @@
 helpSections[(1,1)] = '''Key Bindings in the Main Window'''
 helpSections[(1,2)] = '''Key Bindings in the Search Entry Field'''
 helpSections[(1,3)] = '''Key Bindings in the Search Result Window'''
 helpSections[(1,4)] = '''Key Bindings in Dialogs'''
 
 helpTexts = {}
 helpTexts[0] = (('''Description''', 'title1'), ('''
-''', ''), ('''Trowser''', 'underlined'), (''' is a graphical browser for large line-oriented text files with color highlighting and a highly flexible search and cherry-picking window. Trowser was developed as an alternative to UNIX-tool "less" when analyzing debug log files (aka traces - hence the name).
-''', ''), ('''Trowser has a graphical interface, but is designed to allow browsing via the keyboard at least to the same extent as less. Key bindings and the cursor positioning concept are derived from vim.
+''', ''), ('''Trowser''', 'underlined'), (''' is a graphical browser for large line-oriented text files with color highlighting and a highly flexible search and cherry-picking window. Trowser was developed as an alternative to tools such as "less" (UNIX) or "Notepad++" (Windows) when analyzing debug log files (or "trace files", as they are often called in embedded software world - hence the name).
+''', ''), ('''Trowser has a graphical interface, but is designed to allow browsing via the keyboard at least to the same extent as less. Additional key bindings and the cursor positioning concept are derived from the Vim text editor.
 ''', ''), ('''Note in this context "line-oriented" denotes that each line of text is considered a data unit.  Color highlighting (including search matches) will always apply the highlight to a complete line of text.
 ''', ''), ('''When you start trowser for the first time, you'll have to create highlight patterns for your type of file.  To do this, first enter a search pattern and verify that it matches the intended lines. Then open the ''', ''), ('''Edit highlight patterns''', 'underlined'), (''' dialog in the ''', ''), ('''Search''', 'underlined'), (''' menu, press the right mouse button to open the context menu and select ''', ''), ('''Add current search''', 'underlined'), ('''. You can change the highlight color or select a different kind of mark-up by double-clicking on the new entry in the dialog, or by selecting ''', ''), ('''Edit markup''', 'underlined'), (''' in the context menu.  To define new colors, click on ''', ''), ('''Edit color palette''', 'underlined'), (''' at the bottom of the markup editor dialog.
-''', ''), ('''There are several ways to quickly navigate in the file to lines matching search patterns: Firstly, you can search forwards or backwards to any sub-string or pattern you enter in the ''', ''), ('''Find:''', 'underlined'), (''' field. Secondly, you can repeat previous searches by opening the search history dialog and double-clicking on an entry, or by clicking ''', ''), ('''Next''', 'underlined'), (''' or ''', ''), ('''Previous''', 'underlined'), ('''. Third, you can assign bookmarks to selected text lines and jump in-between those lines by clicking on them in the bookmark list dialog or via ''', ''), (''''+''', 'fixed'), (''' and ''', ''), (''''-''', 'fixed'), (''' key bindings (not in vim.) Fourth, you can search for patterns defined in the color highlight list by selecting a pattern in the list and then clicking on ''', ''), ('''Next''', 'underlined'), (''' or ''', ''), ('''Previous''', 'underlined'), (''' in the pattern list dialog. Fifth, you can open the ''', ''), ('''Search result list''', 'underlined'), (''' (via the ''', ''), ('''Search''', 'underlined'), (''' menu or by clicking on ''', ''), ('''List all''', 'underlined'), (''' in any dialog or by entering ''', ''), ('''ALT-a''', 'fixed'), (''') to display all text lines which match a set of patterns and click on an entry in this list to jump to the respective line in the main window. Sixth, you can manually copy arbitrary lines from the main text window into the search result window via the ''', ''), ('''\ 'i'\ ''', 'fixed'), (''' key (not in vim.)
+''', ''), ('''There are several ways to quickly navigate in the file to lines matching search patterns: Firstly, you can search forwards or backwards to any sub-string or pattern you enter in the ''', ''), ('''Find:''', 'underlined'), (''' field. Secondly, you can repeat previous searches by opening the search history dialog and double-clicking on an entry, or by clicking ''', ''), ('''Next''', 'underlined'), (''' or ''', ''), ('''Previous''', 'underlined'), ('''. Third, you can assign bookmarks to selected text lines and jump in-between those lines by clicking on them in the bookmark list dialog or via ''', ''), (''''+''', 'fixed'), (''' and ''', ''), (''''-''', 'fixed'), (''' key bindings (not in vim.) Fourth, you can search for patterns defined in the color highlight list by selecting a pattern in the list and then clicking on ''', ''), ('''Next''', 'underlined'), (''' or ''', ''), ('''Previous''', 'underlined'), (''' in the pattern list dialog. Fifth, you can open the ''', ''), ('''Search result list''', 'underlined'), (''' (via the ''', ''), ('''Search''', 'underlined'), (''' menu or by clicking on ''', ''), ('''List all''', 'underlined'), (''' in any dialog or by entering ''', ''), ('''ALT-a''', 'fixed'), (''') to display all text lines which match a set of patterns and click on an entry in this list to jump to the respective line in the main window. Sixth, you can manually copy arbitrary lines from the main text window into the search result window via the ''', ''), (''''i\'''', 'fixed'), (''' key (not in vim.)
 ''', ''), ('''The search filter list is one of the main features of the trace browser, as it allows to consecutively build an arbitrary sub-set of text lines in the main window. You can not only use one or more search patterns to add text, but also add selected text lines from the main text window via the ''', ''), ('''i''', 'fixed'), (''' key binding and remove individual lines again, either manually or by use of a search pattern.  Additionally you can use bookmarks in the search result window. When searching in the main window, the search result list will scroll to show the same region of text. Thus you effectively can navigate the text on three levels: Bookmarks > Search list > Main text.
 ''', ''), ('''Both the bookmark and search result lists support prefixing all entries with a "frame number". This is useful when your input file does not have time-stamp prefixes on each line. In this case trowser can search for a preceding time-stamp and automatically prefix bookmarked lines with this number.  Additionally trowser allows to fetch a "frame number" which is not printed in the same line as the frame interval start line. In this case trowser searches the next frame start lines in forward and backward direction and then inside of that range for a line containing the frame number value.  Note for the search result list this feature is disabled by default for performance reasons. It must be enabled in the dialog's ''', ''), ('''Options''', 'underlined'), (''' menu. The search patterns used to locate time-stamps currently have to be inserted into the RC file manually.
 ''', ''), ('''For performance reasons most search-related commands are executed as background processes, so that the GUI remains responsive during search. For example, this applies to the initial color highlighting, global search highlighting, incremental search while editing search patterns and filling the search result list.  Such background activity is indicated by display of a progress bar and switching the mouse cursor to a watch or hourglass image.  You still can use trowser as usual during this time though.  The background activity is automatically aborted or restarted when a conflicting command is entered (e.g. when the search pattern is modified during global search highlighting.)
 ''', ''), )
 
 helpTexts[1] = (('''Key bindings''', 'title1'), ('''
 ''', ''), ('''Generally, keyboard focus can be moved between control elements (e.g. buttons, check-boxes and text containers) using the ''', ''), ('''TAB''', 'underlined'), (''' or ''', ''), ('''Shift-TAB''', 'underlined'), ('''.  The widget with the keyboard focus is marked by a black border.  After start-up, keyboard focus is in the main text window.  Functions which are bound to mouse clicks on buttons etc. can be activated via the keyboard using the ''', ''), ('''Space''', 'underlined'), (''' bar. Many functions can also be activated via shortcuts: Press the ''', ''), ('''ALT''', 'underlined'), (''' key plus the character which is underlines in the button description (e.g. Press ''', ''), ('''ALT-c''', 'fixed'), (''' to open the ''', ''), ('''Control''', 'underlined'), (''' menu, or ''', ''), ('''ALT-a''', 'fixed'), (''' to simulate a mouse-click on the ''', ''), ('''All''', 'underlined'), (''' button at the bottom of the main window.)
@@ -8042,29 +7805,29 @@
 ''', ''), ('''Move the view horizontally to the left or right (same as in vim)
 ''', 'indent'), ('''zs''', 'fixed'), (''', ''', ''), ('''ze''', 'fixed'), ('''
 ''', ''), ('''Scroll the view horizontally so that the current cursor column is placed at the left or the right side of the screen (as far as possible); in any case the cursor position remains unchanged (same as in vim)
 ''', 'indent'), ('''f''', 'fixed'), (''', ''', ''), ('''F''', 'fixed'), ('''
 ''', ''), ('''Search for the following character in the same line to the right or left respectively (same as in vim)
 ''', 'indent'), (''';''', 'fixed'), (''', ''', ''), (''',''', 'fixed'), (''' (semicolon, comma)
 ''', ''), ('''Repeat a previous in-line search (''', 'indent'), ('''f''', ('fixed', 'indent')), (''' or ''', 'indent'), ('''F''', ('fixed', 'indent')), (''') in the same or opposite direction respectively (same as in vim)
-''', 'indent'), ('''''''', 'fixed'), (''' (two apostrophes)
-''', ''), ('''Moves the cursor to the position before the latest jump (same as in vim and less.)  A "jump" is one of the following commands: ''', 'indent'), ('''\ '\ ''', ('fixed', 'indent')), (''', ''', 'indent'), ('''G''', ('fixed', 'indent')), (''', ''', 'indent'), ('''/''', ('fixed', 'indent')), (''', ''', 'indent'), ('''?''', ('fixed', 'indent')), (''', ''', 'indent'), ('''n''', ('fixed', 'indent')), (''', ''', 'indent'), ('''N''', ('fixed', 'indent')), (''', ''', 'indent'), ('''L''', ('fixed', 'indent')), (''', ''', 'indent'), ('''M''', ('fixed', 'indent')), (''' and ''', 'indent'), ('''H''', ('fixed', 'indent')), (''' (same as in vim.)  Note movements controlled via the GUI, such as the bookmark list or search result list, do not modify the jump list.
+''', 'indent'), (''''\'''', 'fixed'), (''' (two apostrophes)
+''', ''), ('''Moves the cursor to the position before the latest jump (same as in vim and less.)  A "jump" is one of the following commands: ''', 'indent'), ('''\'''', ('fixed', 'indent')), (''', ''', 'indent'), ('''G''', ('fixed', 'indent')), (''', ''', 'indent'), ('''/''', ('fixed', 'indent')), (''', ''', 'indent'), ('''?''', ('fixed', 'indent')), (''', ''', 'indent'), ('''n''', ('fixed', 'indent')), (''', ''', 'indent'), ('''N''', ('fixed', 'indent')), (''', ''', 'indent'), ('''L''', ('fixed', 'indent')), (''', ''', 'indent'), ('''M''', ('fixed', 'indent')), (''' and ''', 'indent'), ('''H''', ('fixed', 'indent')), (''' (same as in vim.)  Note movements controlled via the GUI, such as the bookmark list or search result list, do not modify the jump list.
 ''', 'indent'), (''''+''', 'fixed'), (''', ''', ''), (''''-''', 'fixed'), ('''
 ''', ''), ('''Moves the cursor to the next or previous bookmark (not in vim)
 ''', 'indent'), (''''^''', 'fixed'), (''', ''', ''), (''''$''', 'fixed'), ('''
 ''', ''), ('''Moves the cursor to the start or end of file (same as in less; not in vim)
 ''', 'indent'), ('''^o''', 'fixed'), (''', ''', ''), ('''^i''', 'fixed'), ('''
-''', ''), ('''Moves the cursor to the next older (or newer respectively) position in the jump list (same as in vim; note ''', 'indent'), ('''TAB''', ('fixed', 'indent')), (''' which is identical to ''', 'indent'), ('''^i''', ('fixed', 'indent')), (''' in vim has a different meaning here.) See ''', 'indent'), ('''''''', ('fixed', 'indent')), (''' for a list of commands which are considered jumps and add pre-jump cursor positions to the list.
+''', ''), ('''Moves the cursor to the next older (or newer respectively) position in the jump list (same as in vim; note ''', 'indent'), ('''TAB''', ('fixed', 'indent')), (''' which is identical to ''', 'indent'), ('''^i''', ('fixed', 'indent')), (''' in vim has a different meaning here.) See ''', 'indent'), (''''\'''', ('fixed', 'indent')), (''' for a list of commands which are considered jumps and add pre-jump cursor positions to the list.
 ''', 'indent'), ('''1''', 'fixed'), (''', ''', ''), ('''2''', 'fixed'), (''', ... ''', ''), ('''9''', 'fixed'), ('''
 ''', ''), ('''A number without leading zeroes can be used to repeat the subsequent key command or place the cursor on a given line or column (same as in vim)
 ''', 'indent'), ('''For example: ''', 'indent'), ('''1G''', ('fixed', 'indent')), (''' places the cursor in the first line of the file; ''', 'indent'), ('''10|''', ('fixed', 'indent')), (''' places the cursor in the tenth column of the current line (line and column numbering starts at 1.)  Note the number cannot start with zero, as ''', 'indent'), ('''0''', ('fixed', 'indent')), (''' is treated specially (immediately moves the cursor into the first column, same as in vim.)
 ''', 'indent'), ('''Searching and repeating:
 ''', ''), ('''/''', 'fixed'), (''', ''', ''), ('''?''', 'fixed'), ('''
 ''', ''), ('''Search for the following pattern (same as in vim.) Similar to vim, the keyboard focus is moved from the main text into a small text entry field (command line in vim) Note the previous search pattern is always cleared when re-entering the entry field, but all previously used patterns are still available in the history which can be accessed with the cursor up/down keys like in vim. Note in addition, you can use ''', 'indent'), ('''^d''', ('fixed', 'indent')), (''' in the search field to copy the text under the cursor in the main window into the search field, word by word.
-''', 'indent'), ('''As soon as a search expression is typed into the field, an incremental search is started and matching lines are highlighted. The cursor in the main text isn't actually moved there until the search is completed by pressing ''', 'indent'), ('''Return''', ('fixed', 'indent')), ('''.  The search can be aborted by ''', 'indent'), ('''^C''', ('fixed', 'indent')), (''' or ''', 'indent'), ('''Escape''', ('fixed', 'indent')), ('''. For more details see ''', 'indent'), ('''Key bindings: Key Bindings in the Search Entry Field''', ('href', 'indent')), ('''.
+''', 'indent'), ('''As soon as a search expression is typed into the field, an incremental search is started and matching lines are highlighted. The cursor in the main text isn't actually moved there until the search is completed by pressing ''', 'indent'), ('''Return''', ('fixed', 'indent')), ('''.  The search can be aborted by ''', 'indent'), ('''^C''', ('fixed', 'indent')), (''' or ''', 'indent'), ('''Escape''', ('fixed', 'indent')), ('''. For more details see ''', 'indent'), ('''Key bindings: Key bindings in the search entry field''', ('href', 'indent')), ('''.
 ''', 'indent'), ('''n''', 'fixed'), (''', ''', ''), ('''N''', 'fixed'), ('''
 ''', ''), ('''Repeats the previous search in forward or backwards direction respectively (similar to vim - however in contrary to vim ''', 'indent'), ('''n''', ('fixed', 'indent')), (''' always searches forward and ''', 'indent'), ('''N''', ('fixed', 'indent')), (''' always backwards because the standard vim behavior of remembering and reversing the search direction with ''', 'indent'), ('''N''', ('fixed', 'indent')), (''' is very confusing.)
 ''', 'indent'), ('''*''', 'fixed'), (''', ''', ''), ('''#''', 'fixed'), ('''
 ''', ''), ('''Searches for the word under the cursor in forward or backwards direction respectively (same as in vim)  Note when regular expression search mode is not enabled, this command performs a plain sub-string text search. Else, word boundary matches are placed around the search text, as done by vim.
 ''', 'indent'), ('''&''', 'fixed'), ('''
 ''', ''), ('''Remove the highlighting of previous search matches (not in vim as such, but can be added via ''', 'indent'), ('''map & :nohlsearch^M''', ('fixed', 'indent')), (''' in ''', 'indent'), ('''.vimrc''', ('underlined', 'indent')), (''')  Note this does not disable highlighting in subsequent searches.
 ''', 'indent'), ('''ALT-''', 'underlined'), (''' ''', ''), ('''f''', 'fixed'), ('''
@@ -8119,15 +7882,15 @@
 ''', 'indent'), ('''ALT-''', 'underlined'), (''' ''', ''), ('''a''', 'fixed'), ('''
 ''', ''), ('''Open the search result window and fill it with all text lines which match the current search pattern (not in vim)  Additionally, keyboard focus is moved back into the main window.
 ''', 'indent'), ('''ALT-''', 'underlined'), (''' ''', ''), ('''N''', 'fixed'), (''', ''', ''), ('''ALT-''', 'underlined'), (''' ''', ''), ('''P''', 'fixed'), ('''
 ''', ''), ('''Open the search result window and fill it with all text lines below or above the current cursor position respectively which match the current search pattern (not in vim)  Additionally, the keyboard focus is moved back into the main window.
 ''', 'indent'), ('''ALT-''', 'underlined'), (''' ''', ''), ('''c''', 'fixed'), ('''
 ''', ''), ('''Toggle the "match case" option, i.e. equivalent to clicking on ''', 'indent'), ('''Match case''', ('underlined', 'indent')), (''' (not in vim)
 ''', 'indent'), ('''ALT-''', 'underlined'), (''' ''', ''), ('''e''', 'fixed'), ('''
-''', ''), ('''Toggle the regular expression search option, i.e. equivalent to clicking on button ''', 'indent'), ('''Reg.Exp.''', ('underlined', 'indent')), (''' (not in vim.)  When this option is enabled, special characters are parsed according to ''', 'indent'), ('''re_syntax''', ('underlined', 'indent')), (''' Tcl manual page; the syntax is almost identical to Perl with few exceptions (notably ''', 'indent'), ('''\m''', ('fixed', 'indent')), (''' and ''', 'indent'), ('''\M''', ('fixed', 'indent')), (''' to match beginning and end of words)  When the option is not enabled, no characters have a special meaning (i.e. even "''', 'indent'), ('''*''', ('fixed', 'indent')), ('''") and a simple sub-string search is started.
+''', ''), ('''Toggle the regular expression search option, i.e. equivalent to clicking on button ''', 'indent'), ('''Reg.Exp.''', ('underlined', 'indent')), (''' (not in vim.)  When this option is enabled, special characters are parsed according to ''', 'indent'), ('''re_syntax''', ('underlined', 'indent')), (''' Tcl manual page; the syntax is almost identical to Perl with few exceptions (notably ''', 'indent'), ('''\\m''', ('fixed', 'indent')), (''' and ''', 'indent'), ('''\\M''', ('fixed', 'indent')), (''' to match beginning and end of words)  When the option is not enabled, no characters have a special meaning (i.e. even "''', 'indent'), ('''*''', ('fixed', 'indent')), ('''") and a simple sub-string search is started.
 ''', 'indent'), ('''Note: for performance reasons it's recommended to use case-sensitive sub-string searches for color highlighting, especially if you have many patterns. This is usually faster than combining multiple patterns with ''', 'indent'), ('''|''', ('fixed', 'indent')), (''' in a regular expression.
 ''', 'indent'), ('''Key Bindings in the Search Result Window''', 'title2'), ('''
 ''', ''), ('''The following commands can be used in the search result window (i.e. the list filled by "Search All" and lines copied from the main window via the ''', ''), ('''i''', 'fixed'), (''' key binding.)
 ''', ''), ('''For users who prefer controls via the mouse it should be noted that there's a context menu which opens via a click with the right mouse button into a line, which has equivalent commands to the ones listed below.
 ''', ''), ('''m''', 'fixed'), ('''
 ''', ''), ('''Bookmark the currently selected line.  The line will be marked both in the search result window and the main window.
 ''', 'indent'), ('''Delete''', 'underlined'), ('''
@@ -8157,31 +7920,33 @@
 ''', 'indent'), ('''Page-Up''', 'underlined'), (''', ''', ''), ('''Page-Down''', 'underlined'), ('''
 ''', ''), ('''Scroll the view up or down by a page. These commands remove the selection cursor.
 ''', 'indent'), )
 
 helpTexts[2] = (('''Options''', 'title1'), ('''
 ''', ''), ('''The following command line options are available:
 ''', ''), ('''-h''', 'bold'), (''' ''', ''), ('''limit''', 'underlined'), (''', ''', ''), ('''--head=limit''', 'bold'), ('''
-''', ''), ('''This option specifies the maximum number of bytes read from the start of the input file or stream, i.e. any following text is silently ignored.
-''', 'indent'), ('''The limit value is remembered in the configuration file and used in the next invocation unless overridden.  When neither ''', 'indent'), ('''-h''', ('bold', 'indent')), (''' or ''', 'indent'), ('''-t''', ('bold', 'indent')), (''' are specified and data is loaded from a stream via STDIN, a small dialog window pops up when the buffer limit is exceeded. This allows the user to select between head and tail modes manually.
+''', ''), ('''This option specifies the maximum number of bytes to load from input file or stream for display. When loading from a stream via STDIN, it's possible to continue reading more data later via command ''', 'indent'), ('''Continue loading STDIN''', ('underlined', 'indent')), ('''.
+''', 'indent'), ('''The limit value is remembered in the configuration file and used as default the next time data is loaded from STDIN. When loading from a file, default is to load the complete file.
+''', 'indent'), ('''When neither option ''', 'indent'), ('''-h''', ('bold', 'indent')), (''' or ''', 'indent'), ('''-t''', ('bold', 'indent')), (''' are specified and data is loaded from a stream via STDIN, a small dialog window pops up when the buffer limit is exceeded. This allows the user to select between head and tail modes manually.
 ''', 'indent'), ('''-t''', 'bold'), (''' ''', ''), ('''limit''', 'underlined'), (''', ''', ''), ('''--tail=limit''', 'bold'), ('''
-''', ''), ('''This option specifies the maximum number of bytes to be read into the display buffer.  If the input is a file which is larger then the given buffer limit, text at the beginning of the file is skipped. If the input is a stream, all data is read into a temporary queue until the end-of-stream is reached; then the last ''', 'indent'), ('''limit''', ('underlined', 'indent')), (''' number of bytes which were read from the stream are loaded into the display buffer.
-''', 'indent'), ('''The limit value is remembered in the configuration file and used in the next invocation unless overridden.
+''', ''), ('''This option specifies to load only the given maximum number of bytes into the display from the end of the file or input stream. This means when reading from a file, data from the beginning is skipped if the file is larger than the limit.  If the input is a STDIN stream, data is read into a ring buffer of the given size. Once the end-of-stream is reached, the last content of the ring buffer is loaded into the display.
+''', 'indent'), ('''The limit value is remembered in the configuration file equivalently as described for the "head" option.
 ''', 'indent'), ('''-r''', 'bold'), (''' ''', ''), ('''path''', 'underlined'), (''', ''', ''), ('''--rcfile=path''', 'bold'), ('''
-''', ''), ('''This option can be used to specify an alternate configuration file. When this option is not present, the configuration file is stored in the home directory, see section FILES.
+''', ''), ('''This option can be used to specify an alternate configuration file. When this option is not present, the configuration file is stored in system directories, see ''', 'indent'), ('''Files''', ('href', 'indent')), ('''.
 ''', 'indent'), )
 
 helpTexts[3] = (('''Environment''', 'title1'), ('''
 ''', ''), ('''trowser''', 'bold'), (''' only evaluates the standard variables ''', ''), ('''DISPLAY''', 'bold'), (''' (X11 display address) and ''', ''), ('''HOME''', 'bold'), (''' (home directory, for storing the configuration file.)
 ''', ''), )
 
 helpTexts[4] = (('''Files''', 'title1'), ('''
 ''', ''), ('''$HOME/.config/trowser/trowser.py.rc''', 'bold'), ('''
-''', ''), ('''UNIX''', ('underlined', 'indent')), (''': Configuration file where all personal settings and the search history are stored. Per default this file is created in your home directory, but a different path and file name can be specified with the ''', 'indent'), ('''--rcfile''', ('bold', 'indent')), (''' option (see ''', 'indent'), ('''Options''', ('href', 'indent')), (''').
-''', 'indent'), ('''During updates to this file, trowser temporarily creates a file called ''', 'indent'), ('''.trowserc.XXXXX.tmp''', ('fixed', 'indent')), (''' in the home directory, where "XXXXX" is a random number. The old file is then replaced with this new file. This procedure will obviously fail if your home directory is not writable.
+''', ''), ('''UNIX''', ('underlined', 'indent')), (''': Configuration file where all personal settings and the search history are stored. The path may be overriden via environment variable ''', 'indent'), ('''XDG_CONFIG_HOME''', ('fixed', 'indent')), ('''. A different file name can be specified with the ''', 'indent'), ('''--rcfile''', ('bold', 'indent')), (''' option (see ''', 'indent'), ('''Options''', ('href', 'indent')), (''').
+''', 'indent'), ('''During updates to this file, trowser temporarily creates a new file the same directory, where "XXXXX" is a random number. The old file is then replaced with this new file. This procedure will obviously fail if the target directory (not the file itself!) is not writable.
+''', 'indent'), ('''MS Windows''', ('underlined', 'indent')), (''': On the MS Windows platform, the configuration file is created in the hidden application data directory in your user home. The specific path depends on your operating system version. (The path is qeried via a system API.)
 ''', 'indent'), )
 
 helpTexts[5] = (('''Caveats''', 'title1'), ('''
 ''', ''), ('''Currently only one pattern list for color highlighting is supported. Hence different highlighting for different file types can only be done by choosing different configuration files when starting trowser (see the ''', ''), ('''--rcfile''', 'underlined'), (''' option.)
 ''', ''), ('''Vim compatibility: Not all vim navigation commands are implemented; Command repetition is supported only for a small sub-set of commands; Some commands behave slightly differently from vim (most notably the bookmark related commands.) vim's range and selection commands are not supported at all.
 ''', ''), ('''Search repetition by pressing "Next" or "Previous" or the search history dialog is currently not interruptable and may take quite a while if the next match is several MB away. (This can be avoided by repeating the search via the entry field's internal search history, i.e. ''', ''), ('''/''', 'fixed'), (''' and ''', ''), ('''Up''', 'underlined'), (''')
 ''', ''), ('''Searching with regular expressions is very slow in large files. This is unfortunately a property of the "text" Tk widget. Thus use of regular expressions for highlighting is not recommended. (As a work-around, trowser automatically falls back to plain string search if there are no control characters in the search expression.)
@@ -8232,25 +7997,22 @@
     opt["size"] += 2
     help_font_title2 = tkf.Font(**opt)
     opt["size"] += 2
     help_font_title1 = tkf.Font(**opt)
 
 
 def dlg_help_add_menu_commands(wid_men):
-    global help_titles
-
-    for title, idx in helpIndex.items():
+    for title in helpIndex:
         help_titles.append(title)
 
     Help_dialog.fill_menu(wid_men)
 
 
-class Help_dialog(object):
+class Help_dialog:
     def __init__(self, index, subheading, subrange):
-        global win_geom
         self.chapter_idx = -1
         self.help_stack = []
 
         self.wid_top = Toplevel(tk)
         self.wid_top.wm_title("GtestGui: Manual")
         self.wid_top.wm_group(tk)
 
@@ -8290,15 +8052,15 @@
         self.but_cmd_next = but_cmd_next
 
     @staticmethod
     def fill_menu(wid_men):
         for idx in range(len(help_titles)):
             wid_men.add_command(label=help_titles[idx],
                                 command=lambda idx=idx: dlg_help_create_dialog(idx))
-            for foo, sub in sorted([x for x in helpSections.keys() if x[0] == idx]):
+            for _, sub in sorted([x for x in helpSections if x[0] == idx]):
                 title = helpSections[(idx, sub)]
                 wid_men.add_command(label="- " + title,
                             command=lambda idx=idx, title=title: dlg_help_create_dialog(idx, title))
 
 
     def __create_text_widget(self):
         wid_frm = Frame(self.wid_top)
@@ -8398,24 +8160,22 @@
     def __destroy_window(self):
         global dlg_help
         SafeDestroy(self.wid_top)
         dlg_help = None
 
 
     def __follow_help_hyperlink(self):
-        global helpIndex
-
         # the text under the mouse carries the mark 'current'
         curidx = self.wid_txt.index("current + 1 char")
 
         # determine the range of the 'href' tag under the mouse
-        range = self.wid_txt.tag_prevrange("href", curidx)
+        href_range = self.wid_txt.tag_prevrange("href", curidx)
 
         # cut out the text in that range
-        hlink = self.wid_txt.get(*range)
+        hlink = self.wid_txt.get(*href_range)
 
         # check if the text contains a sub-section specification
         match = re.match(r"(.*): *(.*)", hlink)
         if match:
             hlink = match.group(1)
             subsect = match.group(2)
         else:
@@ -8427,20 +8187,20 @@
 
 # ----------------------------------------------------------------------------
 #
 # This function reads configuration variables from the rc file.
 # The function is called once during start-up.
 #
 def LoadRcFile():
-  global tlb_history, tlb_hist_maxlen, tlb_case, tlb_regexp, tlb_hall
+  global tlb_history, tlb_hist_maxlen
   global patlist, col_palette, tick_pat_sep, tick_pat_num, tick_str_prefix
   global font_content, col_bg_content, col_fg_content, fmt_find, fmt_findinc
-  global win_geom, fmt_selection
-  global load_buf_size
+  global fmt_selection, load_buf_size_default
   global rcfile_version, myrcfile
+  #global tlb_case, tlb_regexp, tlb_hall, win_geom  # modified, but not assigned
 
   error = False
   ver_check = False
   rc_compat_version = None
   line_no = 0
   font_content_opt = ""
 
@@ -8471,15 +8231,15 @@
             elif (var == "tick_str_prefix"):   tick_str_prefix = val
             elif (var == "font_content"):      font_content_opt = val
             elif (var == "fmt_selection"):     fmt_selection = val
             elif (var == "col_bg_content"):    col_bg_content = val
             elif (var == "col_fg_content"):    col_fg_content = val
             elif (var == "fmt_find"):          fmt_find = val
             elif (var == "fmt_findinc"):       fmt_findinc = val
-            elif (var == "load_buf_size"):     load_buf_size = val
+            elif (var == "load_buf_size"):     load_buf_size_default = val
             elif (var == "rcfile_version"):    rcfile_version = val
             elif (var == "rc_compat_version"): rc_compat_version = val
             elif (var == "rc_timestamp"):      pass
             elif (var.startswith("win_geom:")): win_geom[var[9:]] = val
             else:
               print("Warning: ignoring unknown keyword in rcfile line %d:" % line_no, var, file=sys.stderr)
 
@@ -8508,38 +8268,24 @@
 
     try:
       if font_content_opt:
         font_content = tkf.Font(**font_content_opt)
     except Exception as e:
       print("Error configuring content font:", str(e), file=sys.stderr)
 
-    # override config var with command line options
-    try:
-      global load_buf_size_opt
-      if load_buf_size_opt != 0:
-        load_buf_size = load_buf_size_opt
-    except:
-      pass
-
   except OSError as e:
     if e.errno != errno.ENOENT:
       print("Failed to load config file:", str(e), file=sys.stderr)
 
 
 #
 # This function writes persistent configuration variables into the RC file
 #
 def UpdateRcFile():
-  global myrcfile, rcfile_compat, rcfile_version
-  global tid_update_rc_sec, tid_update_rc_min, rc_file_error
-  global tlb_history, tlb_hist_maxlen, tlb_case, tlb_regexp, tlb_hall
-  global dlg_mark_geom, dlg_hist_geom, dlg_srch_geom, dlg_tags_geom, main_win_geom
-  global patlist, col_palette, tick_pat_sep, tick_pat_num, tick_str_prefix
-  global font_content, col_bg_content, col_fg_content, fmt_find, fmt_findinc
-  global fmt_selection, load_buf_size
+  global tid_update_rc_min, rc_file_error
 
   if tid_update_rc_sec: tk.after_cancel(tid_update_rc_sec)
   if tid_update_rc_min: tk.after_cancel(tid_update_rc_min)
   tid_update_rc_min = None
 
   try:
     with tempfile.NamedTemporaryFile(mode="w", delete=False, dir=os.path.dirname(myrcfile),
@@ -8590,27 +8336,27 @@
       print("font_content=", json.dumps(font_content.configure()), file=rcfile)
       print("col_bg_content=", json.dumps(col_bg_content), file=rcfile)
       print("col_fg_content=", json.dumps(col_fg_content), file=rcfile)
       print("fmt_find=", json.dumps(fmt_find), file=rcfile)
       print("fmt_findinc=", json.dumps(fmt_findinc), file=rcfile)
       print("fmt_selection=", json.dumps(fmt_selection), file=rcfile)
 
-      # misc (note the head/tail mode is omitted intentionally)
-      print("load_buf_size=", json.dumps(load_buf_size), file=rcfile)
+      # file/stream load parameters
+      print("load_buf_size=", json.dumps(load_buf_size_default), file=rcfile)
 
     # copy attributes on the new file
     try:
       st = os.stat(myrcfile)
       try:
         os.chmod(rcfile.name, st.st_mode & 0o777)
         if (os.name == "posix"):
           os.chown(rcfile.name, st.st_uid, st.st_gid)
       except OSError as e:
         print("Warning: Failed to update mode/permissions on %s: %s" % (myrcfile, e.strerror), file=sys.stderr)
-    except OSError as e:
+    except OSError:
       pass
 
     # move the new file over the old one
     try:
       # MS-Windows does not allow renaming when the target file already exists,
       # so we need to remove the target first. DISADVANTAGE: operation is not atomic
       if (os.name != "posix"):
@@ -8646,14 +8392,18 @@
   if tid_update_rc_sec: tk.after_cancel(tid_update_rc_sec)
   tid_update_rc_sec = tk.after(3000, UpdateRcFile)
 
   if not tid_update_rc_min:
     tid_update_rc_min = tk.after(60000, UpdateRcFile)
 
 
+#
+# This function determines the default path for the configuration file, if none
+# is specified on the command line.
+#
 def GetRcFilePath():
     if (os.name == "posix"):
         xdg_config_home = os.environ.get("XDG_CONFIG_HOME")
         home = os.path.expanduser("~")
 
         if xdg_config_home is not None and os.path.exists(xdg_config_home):
             rc_file = os.path.join(xdg_config_home, "trowser", "trowser.py.rc")
@@ -8666,16 +8416,21 @@
                 rc_file = os.path.join(home, ".trowser.py.rc")
 
         else:
             rc_file = ".trowser.py.rc"
 
         os.makedirs(os.path.dirname(rc_file), exist_ok=True)
 
-    else: # TODO win32
-        rc_file = "trowser.ini"
+    else:
+        # Query system library for the common path for application configuration.
+        # e.g. on Win10: C:\Users\USERNAME\AppData\Local\Trowser (hidden directory)
+        config_dir = appdirs.user_config_dir(appname="Trowser", appauthor=False)
+        os.makedirs(config_dir, exist_ok=True)
+
+        rc_file = os.path.join(config_dir, "trowser.rc")
 
     return rc_file
 
 
 # ----------------------------------------------------------------------------
 #
 # This function is called when the program is started with -help to list all
@@ -8711,66 +8466,67 @@
 # This helper function reads an integer value from a command line parameter
 #
 def ParseArgInt(opt, val):
   try:
     return int(val)
   except:
     PrintUsage(opt, "\"%s\" is not a numerical value" % val)
+    return 0 # never reached - dummy for pylint
 
 #
 # This function parses and evaluates the command line arguments.
 #
 def ParseArgv():
-  global load_file_mode, load_buf_size_opt
+  global load_file_mode, load_buf_size, myrcfile
 
   file_seen = False
   arg_idx = 1
   while arg_idx < len(sys.argv):
     arg = sys.argv[arg_idx]
 
     if arg.startswith("-") and (arg != "-"):
       if arg == "-t":
         ParseArgvLenCheck(arg_idx)
         arg_idx += 1
-        load_buf_size_opt = ParseArgInt(arg, sys.argv[arg_idx])
+        load_buf_size = ParseArgInt(arg, sys.argv[arg_idx])
         load_file_mode = 1
 
       elif arg.startswith("--tail"):
         match = re.match("^--tail=(.+)$", arg)
         if match:
-          load_buf_size_opt = ParseArgInt(arg, match.group(1))
+          load_buf_size = ParseArgInt(arg, match.group(1))
           load_file_mode = 1
         else:
           PrintUsage(arg, "requires a numerical argument (e.g. --tail=10000000)")
 
       elif arg == "-h":
         ParseArgvLenCheck(arg_idx)
         arg_idx += 1
-        load_buf_size_opt = ParseArgInt(arg, sys.argv[arg_idx])
+        load_buf_size = ParseArgInt(arg, sys.argv[arg_idx])
         load_file_mode = 0
 
       elif arg.startswith("--head"):
         match = re.match("^--head=(.+)$", arg)
         if match:
-          load_buf_size_opt = ParseArgInt(arg, match.group(1))
+          load_buf_size = ParseArgInt(arg, match.group(1))
           load_file_mode = 0
         else:
           PrintUsage(arg, "requires a numerical argument (e.g. --head=10000000)")
 
       elif arg == "-r":
         if arg_idx + 1 < len(sys.argv):
           arg_idx += 1
           myrcfile = sys.argv[arg_idx]
         else:
           PrintUsage(arg, "this option requires an argument")
 
       elif arg.startswith("--rcfile"):
         match = re.match("^--rcfile=(.+)$", arg)
         if match:
-          myrcfile = match.group(0)
+          myrcfile = match.group(1)
         else:
           PrintUsage(arg, "requires a path argument (e.g. --rcfile=foo/bar)")
 
       elif arg == "-?" or arg == "--help":
         PrintUsage()
 
       else:
@@ -8781,17 +8537,15 @@
         file_seen = True
       else:
         arg_idx += 1
         PrintUsage(sys.argv[arg_idx], "only one file name expected")
 
     arg_idx += 1
 
-  if not file_seen:
-    print("File name missing (use \"-\" for stdin)", file=sys.stderr)
-    PrintUsage()
+  return file_seen
 
 
 # ----------------------------------------------------------------------------
 # This section defines a "dummy" class which is used to emulate a global
 # namespace for widgets equivalently to Tcl/Tk. Every created widget is
 # assigned to a variable within this static namespace (i.e. the class is
 # never instantiated), so that all other functions have access. Note this
@@ -8819,17 +8573,17 @@
 # currently open.
 #
 def wt_exists(obj):
   if obj is not None:
     try:
       obj.configure()
       return True
-    except Exception as e:
-      return False
-    return False
+    except Exception:
+      pass
+  return False
 
 # ----------------------------------------------------------------------------
 #
 # Global variables
 #
 # IMPORTANT NOTE: A lot of the variables definitions below are copied into
 # the personal configuration files. Hence the assignments below are only
@@ -8865,15 +8619,15 @@
 tlb_regexp = False
 tlb_hall = False
 
 # This variable stores the search direction: 0:=backwards, 1:=forwards
 tlb_last_dir = 1
 
 # This variable indicates if the search entry field has keyboard focus.
-tlb_find_focus = 0
+tlb_find_focus = False
 
 # This variable contains the name of the widget which had input focus before
 # the focus was moved into the search entry field. Focus will return there
 # after Return or Escape
 tlb_last_wid = None
 
 # These variables hold the cursor position and Y-view from before the start of an
@@ -9042,19 +8796,19 @@
 # 14: relief borderwidth: 1,2,...,9
 # 15: spacing: 0,1,2,...
 patlist = [
   [": Failure", False, True, "default", "tag0", "", "#e73c39", "", True, False, False, "", "", "", 1, 0],
   ["^\\[ ", True, True, "default", "tag1", "", "#b4e79c", "", False, False, False, "", "", "", 1, 0]
 ]
 
-# This variable contains the mode and limit for file load. The mode can be
-# 0 for "head" or 1 for "tail" (i.e. load data from end of the file). The
-# values can be changed by the "head" and "tail" command line options.
+# This variable contains the limit in Bytes to read from input file or stream,
+# set via "head" and "tail" command line options. Default is no limit.
 load_file_mode = 0
-load_buf_size = 0x100000
+load_buf_size = 0
+load_buf_size_default = 0x100000
 
 # define RC file version limit for forwards compatibility
 rcfile_compat = 0x02000001
 rcfile_version = 0x02010000
 rc_file_error = 0
 
 #
@@ -9070,32 +8824,33 @@
   sys.exit(1)
 
 # convert into Tk variables (i.e. variables accessed by widgets or vwait)
 tlb_case = BooleanVar(tk, tlb_case)
 tlb_regexp = BooleanVar(tk, tlb_regexp)
 tlb_hall = BooleanVar(tk, tlb_hall)
 tlb_find = StringVar(tk, tlb_find)
-font_content = tkf.nametofont(font_content_default)
+font_content = tkf.Font(font=tkf.nametofont(font_content_default))
 
 # Parse command line parameters & load configuration options
 myrcfile = GetRcFilePath()
-ParseArgv()
+load_initial_file = ParseArgv()
 LoadRcFile()
 
 InitResources()
 CreateMainWindow()
 HighlightCreateTags()
 tk.wm_deiconify()
 
-if sys.argv[-1] == "-":
-  cur_filename = ""
-  load_pipe = LoadPipe()
-  load_pipe.LoadPipe_Start()
-else:
-  LoadFile(sys.argv[-1])
+if load_initial_file:
+  if sys.argv[-1] == "-":
+    cur_filename = ""
+    load_pipe = LoadPipe()
+    load_pipe.LoadPipe_Start()
+  else:
+    LoadFile(sys.argv[-1])
 
 # done - all following actions are event-driven
 # the application exits when the main window is closed
 try:
   tk.mainloop()
 except KeyboardInterrupt:
   pass
```

### Comparing `trowser-2.1.0/setup.py` & `trowser-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,20 @@
             print("#!pythonw", file=fout)
             for line in fin:
                 print(line, file=fout, end="")
     os.chmod("bin/trowser.py", 0o755)
 
 setup(
     name='trowser',
-    version='2.1.0',
+    version='2.2.0',
     scripts=['bin/trowser.py'],
     packages=[],
 
+    install_requires=['appdirs ; platform_system=="Windows"'],
+
     author='T. Zoerner',
     author_email='tomzox@gmail.com',
 
     url='https://github.com/tomzox/trowser',
 
     description='Trowser is a graphical browser for large line-oriented text files ' \
                 'with sytax highlighting and search facilities tailored for analysis ' \
```

### Comparing `trowser-2.1.0/trowser.egg-info/PKG-INFO` & `trowser-2.2.0/trowser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trowser
-Version: 2.1.0
+Version: 2.2.0
 Summary: Trowser is a graphical browser for large line-oriented text files with sytax highlighting and search facilities tailored for analysis of debug log files.
 Home-page: https://github.com/tomzox/trowser
 Author: T. Zoerner
 Author-email: tomzox@gmail.com
 License: UNKNOWN
 Keywords: color-highlighter,text-search,text-browser,tkinter-gui,GUI
 Platform: posix
@@ -23,17 +23,17 @@
 
 trowser := Trace Browser
 ========================
 
 Description
 -----------
 
-*Trowser* is a graphical browser for large line-oriented text files with color highlighting and a highly flexible search and cherry-picking window. Trowser was developed as an alternative to UNIX-tool "less" when analyzing debug log files (aka traces - hence the name).
+*Trowser* is a graphical browser for large line-oriented text files with color highlighting and a highly flexible search and cherry-picking window. Trowser was developed as an alternative to tools such as "less" (UNIX) or "Notepad++" (Windows) when analyzing debug log files (or "trace files", as they are often called in embedded software world - hence the name).
 
-Trowser has a graphical interface, but is designed to allow browsing via the keyboard at least to the same extent as less. Key bindings and the cursor positioning concept are derived from vim.
+Trowser has a graphical interface, but is designed to allow browsing via the keyboard at least to the same extent as less. Additional key bindings and the cursor positioning concept are derived from the Vim text editor.
 
 Note in this context "line-oriented" denotes that each line of text is considered a data unit.  Color highlighting (including search matches) will always apply the highlight to a complete line of text.
 
 When you start trowser for the first time, you'll have to create highlight patterns for your type of file.  To do this, first enter a search pattern and verify that it matches the intended lines. Then open the *Edit highlight patterns* dialog in the *Search* menu, press the right mouse button to open the context menu and select *Add current search*. You can change the highlight color or select a different kind of mark-up by double-clicking on the new entry in the dialog, or by selecting *Edit markup* in the context menu.  To define new colors, click on *Edit color palette* at the bottom of the markup editor dialog.
 
 There are several ways to quickly navigate in the file to lines matching search patterns: Firstly, you can search forwards or backwards to any sub-string or pattern you enter in the *Find:* field. Secondly, you can repeat previous searches by opening the search history dialog and double-clicking on an entry, or by clicking *Next* or *Previous*. Third, you can assign bookmarks to selected text lines and jump in-between those lines by clicking on them in the bookmark list dialog or via ``'+`` and ``'-`` key bindings (not in vim.) Fourth, you can search for patterns defined in the color highlight list by selecting a pattern in the list and then clicking on *Next* or *Previous* in the pattern list dialog. Fifth, you can open the *Search result list* (via the *Search* menu or by clicking on *List all* in any dialog or by entering ``ALT-a``) to display all text lines which match a set of patterns and click on an entry in this list to jump to the respective line in the main window. Sixth, you can manually copy arbitrary lines from the main text window into the search result window via the ``'i'`` key (not in vim.)
 
@@ -283,38 +283,42 @@
 
 Options
 -------
 
 The following command line options are available:
 
 **-h** *limit*, **--head=limit**
-  This option specifies the maximum number of bytes read from the start of the input file or stream, i.e. any following text is silently ignored.
+  This option specifies the maximum number of bytes to load from input file or stream for display. When loading from a stream via STDIN, it's possible to continue reading more data later via command *Continue loading STDIN*.
 
-  The limit value is remembered in the configuration file and used in the next invocation unless overridden.  When neither **-h** or **-t** are specified and data is loaded from a stream via STDIN, a small dialog window pops up when the buffer limit is exceeded. This allows the user to select between head and tail modes manually.
+  The limit value is remembered in the configuration file and used as default the next time data is loaded from STDIN. When loading from a file, default is to load the complete file.
+
+  When neither option **-h** or **-t** are specified and data is loaded from a stream via STDIN, a small dialog window pops up when the buffer limit is exceeded. This allows the user to select between head and tail modes manually.
 
 **-t** *limit*, **--tail=limit**
-  This option specifies the maximum number of bytes to be read into the display buffer.  If the input is a file which is larger then the given buffer limit, text at the beginning of the file is skipped. If the input is a stream, all data is read into a temporary queue until the end-of-stream is reached; then the last *limit* number of bytes which were read from the stream are loaded into the display buffer.
+  This option specifies to load only the given maximum number of bytes into the display from the end of the file or input stream. This means when reading from a file, data from the beginning is skipped if the file is larger than the limit.  If the input is a STDIN stream, data is read into a ring buffer of the given size. Once the end-of-stream is reached, the last content of the ring buffer is loaded into the display.
 
-  The limit value is remembered in the configuration file and used in the next invocation unless overridden.
+  The limit value is remembered in the configuration file equivalently as described for the "head" option.
 
 **-r** *path*, **--rcfile=path**
-  This option can be used to specify an alternate configuration file. When this option is not present, the configuration file is stored in the home directory, see section FILES.
+  This option can be used to specify an alternate configuration file. When this option is not present, the configuration file is stored in system directories, see `Files`_.
 
 Environment
 -----------
 
 **trowser** only evaluates the standard variables **DISPLAY** (X11 display address) and **HOME** (home directory, for storing the configuration file.)
 
 Files
 -----
 
 **$HOME/.config/trowser/trowser.py.rc**
-  *UNIX*: Configuration file where all personal settings and the search history are stored. Per default this file is created in your home directory, but a different path and file name can be specified with the **--rcfile** option (see `Options`_).
+  *UNIX*: Configuration file where all personal settings and the search history are stored. The path may be overriden via environment variable ``XDG_CONFIG_HOME``. A different file name can be specified with the **--rcfile** option (see `Options`_).
+
+  During updates to this file, trowser temporarily creates a new file the same directory, where "XXXXX" is a random number. The old file is then replaced with this new file. This procedure will obviously fail if the target directory (not the file itself!) is not writable.
 
-  During updates to this file, trowser temporarily creates a file called ``.trowserc.XXXXX.tmp`` in the home directory, where "XXXXX" is a random number. The old file is then replaced with this new file. This procedure will obviously fail if your home directory is not writable.
+  *MS Windows*: On the MS Windows platform, the configuration file is created in the hidden application data directory in your user home. The specific path depends on your operating system version. (The path is qeried via a system API.)
 
 Caveats
 -------
 
 Currently only one pattern list for color highlighting is supported. Hence different highlighting for different file types can only be done by choosing different configuration files when starting trowser (see the *--rcfile* option.)
 
 Vim compatibility: Not all vim navigation commands are implemented; Command repetition is supported only for a small sub-set of commands; Some commands behave slightly differently from vim (most notably the bookmark related commands.) vim's range and selection commands are not supported at all.
```

