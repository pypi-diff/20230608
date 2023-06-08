# Comparing `tmp/pywellcad-0.2.0.tar.gz` & `tmp/pywellcad-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Projects\pywellcad\dist\.tmp-bs586v8y\pywellcad-0.2.0.tar", last modified: Wed May  3 13:47:18 2023, max compression
+gzip compressed data, was "pywellcad-0.2.1.tar", last modified: Thu Jun  8 12:31:41 2023, max compression
```

## Comparing `pywellcad-0.2.0.tar` & `pywellcad-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.916174 pywellcad-0.2.0/
--rw-rw-rw-   0        0        0      217 2023-05-03 13:38:48.000000 pywellcad-0.2.0/.gitignore
--rw-rw-rw-   0        0        0     1565 2021-11-24 11:08:07.000000 pywellcad-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       49 2022-01-17 15:04:12.000000 pywellcad-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2751 2023-05-03 13:47:18.918174 pywellcad-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2313 2023-04-18 06:11:17.000000 pywellcad-0.2.0/README.md
--rw-rw-rw-   0        0        0      149 2021-11-24 11:08:07.000000 pywellcad-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.648294 pywellcad-0.2.0/pywellcad.egg-info/
--rw-rw-rw-   0        0        0     2751 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-05-03 13:47:18.000000 pywellcad-0.2.0/pywellcad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-10-01 07:44:06.000000 pywellcad-0.2.0/pywellcad.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 13:47:15.000000 pywellcad-0.2.0/pywellcad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      579 2023-05-03 13:47:18.929174 pywellcad-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       37 2021-11-24 11:08:07.000000 pywellcad-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.654069 pywellcad-0.2.0/wellcad/
--rw-rw-rw-   0        0        0       17 2023-03-20 09:55:35.000000 pywellcad-0.2.0/wellcad/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:47:18.910194 pywellcad-0.2.0/wellcad/com/
--rw-rw-rw-   0        0        0      816 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/__init__.py
--rw-rw-rw-   0        0        0     8895 2023-05-03 12:03:11.000000 pywellcad-0.2.0/wellcad/com/_application.py
--rw-rw-rw-   0        0        0   170263 2023-05-03 13:38:49.000000 pywellcad-0.2.0/wellcad/com/_borehole.py
--rw-rw-rw-   0        0        0      622 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_comment_box.py
--rw-rw-rw-   0        0        0      870 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_cross_section_box.py
--rw-rw-rw-   0        0        0     4388 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_depth.py
--rw-rw-rw-   0        0        0     2445 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_dispatch_wrapper.py
--rw-rw-rw-   0        0        0     1689 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_drill_item.py
--rw-rw-rw-   0        0        0     5092 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_equipment_item.py
--rw-rw-rw-   0        0        0     2825 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_font.py
--rw-rw-rw-   0        0        0     1695 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_fossil_item.py
--rw-rw-rw-   0        0        0     3678 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_header.py
--rw-rw-rw-   0        0        0     1056 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_interval_item.py
--rw-rw-rw-   0        0        0     1903 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_litho_bed.py
--rw-rw-rw-   0        0        0     1605 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_litho_dictionary.py
--rw-rw-rw-   0        0        0     1298 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_litho_pattern.py
--rw-rw-rw-   0        0        0    77009 2023-05-03 12:03:11.000000 pywellcad-0.2.0/wellcad/com/_log.py
--rw-rw-rw-   0        0        0     1233 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_marker_item.py
--rw-rw-rw-   0        0        0      891 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_odbc.py
--rw-rw-rw-   0        0        0     5280 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_page.py
--rw-rw-rw-   0        0        0     1229 2022-01-19 13:44:07.000000 pywellcad-0.2.0/wellcad/com/_polar_and_rose_box.py
--rw-rw-rw-   0        0        0     1618 2022-02-10 08:01:00.000000 pywellcad-0.2.0/wellcad/com/_stacking_pattern_item.py
--rw-rw-rw-   0        0        0    11640 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_structure.py
--rw-rw-rw-   0        0        0    13377 2022-02-11 10:29:24.000000 pywellcad-0.2.0/wellcad/com/_title.py
--rw-rw-rw-   0        0        0    12431 2023-05-03 13:38:49.000000 pywellcad-0.2.0/wellcad/com/_workspace.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:31:41.009512 pywellcad-0.2.1/
+-rw-rw-rw-   0        0        0      229 2023-06-07 06:40:01.000000 pywellcad-0.2.1/.gitignore
+-rw-rw-rw-   0        0        0     1565 2022-10-11 07:39:08.000000 pywellcad-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       49 2022-10-11 07:39:08.000000 pywellcad-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2751 2023-06-08 12:31:41.010492 pywellcad-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2313 2023-04-28 08:03:58.000000 pywellcad-0.2.1/README.md
+-rw-rw-rw-   0        0        0      149 2022-10-11 07:39:08.000000 pywellcad-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-08 12:31:40.809337 pywellcad-0.2.1/pywellcad.egg-info/
+-rw-rw-rw-   0        0        0     2751 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-06-08 12:31:40.000000 pywellcad-0.2.1/pywellcad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-11 07:43:31.000000 pywellcad-0.2.1/pywellcad.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      579 2023-06-08 12:31:41.016348 pywellcad-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-10-11 07:39:08.000000 pywellcad-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:31:40.815196 pywellcad-0.2.1/wellcad/
+-rw-rw-rw-   0        0        0       17 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:31:41.005605 pywellcad-0.2.1/wellcad/com/
+-rw-rw-rw-   0        0        0      839 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_application.py
+-rw-rw-rw-   0        0        0   174458 2023-06-07 06:40:01.000000 pywellcad-0.2.1/wellcad/com/_borehole.py
+-rw-rw-rw-   0        0        0      647 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_comment_box.py
+-rw-rw-rw-   0        0        0      902 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_cross_section_box.py
+-rw-rw-rw-   0        0        0     4534 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_depth.py
+-rw-rw-rw-   0        0        0     3086 2023-06-07 09:03:05.000000 pywellcad-0.2.1/wellcad/com/_dispatch_wrapper.py
+-rw-rw-rw-   0        0        0     1740 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_drill_item.py
+-rw-rw-rw-   0        0        0     5267 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_equipment_item.py
+-rw-rw-rw-   0        0        0     2935 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_font.py
+-rw-rw-rw-   0        0        0     1765 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_fossil_item.py
+-rw-rw-rw-   0        0        0     3799 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_header.py
+-rw-rw-rw-   0        0        0     1097 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_interval_item.py
+-rw-rw-rw-   0        0        0     1972 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_litho_bed.py
+-rw-rw-rw-   0        0        0     1672 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_litho_dictionary.py
+-rw-rw-rw-   0        0        0     1344 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_litho_pattern.py
+-rw-rw-rw-   0        0        0    79368 2023-04-25 10:02:45.000000 pywellcad-0.2.1/wellcad/com/_log.py
+-rw-rw-rw-   0        0        0     1282 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_marker_item.py
+-rw-rw-rw-   0        0        0      920 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_odbc.py
+-rw-rw-rw-   0        0        0     5459 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_page.py
+-rw-rw-rw-   0        0        0     1273 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_polar_and_rose_box.py
+-rw-rw-rw-   0        0        0     1675 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_stacking_pattern_item.py
+-rw-rw-rw-   0        0        0    11879 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_structure.py
+-rw-rw-rw-   0        0        0    13812 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_title.py
+-rw-rw-rw-   0        0        0    12737 2023-06-07 06:40:01.000000 pywellcad-0.2.1/wellcad/com/_workspace.py
```

### Comparing `pywellcad-0.2.0/LICENSE.txt` & `pywellcad-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.0/PKG-INFO` & `pywellcad-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywellcad
-Version: 0.2.0
+Version: 0.2.1
 Summary: a Python client for the WellCAD Automation API
 Home-page: https://www.alt.lu/
 Author: Advanced Logic Technology
 Author-email: support@alt.lu
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pywellcad-0.2.0/README.md` & `pywellcad-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.0/pywellcad.egg-info/PKG-INFO` & `pywellcad-0.2.1/pywellcad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywellcad
-Version: 0.2.0
+Version: 0.2.1
 Summary: a Python client for the WellCAD Automation API
 Home-page: https://www.alt.lu/
 Author: Advanced Logic Technology
 Author-email: support@alt.lu
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pywellcad-0.2.0/pywellcad.egg-info/SOURCES.txt` & `pywellcad-0.2.1/pywellcad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.0/setup.cfg` & `pywellcad-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.0/wellcad/com/_application.py` & `pywellcad-0.2.1/wellcad/com/_application.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-from win32com.client import Dispatch
-from ._dispatch_wrapper import DispatchWrapper
-from ._borehole import Borehole
-
-class Application(DispatchWrapper):
-    """The core class used to interact with WellCAD via its COM API.
-
-    In general, it is the only class you should instantiate directly. All
-    interaction with borehole documents, logs, etc, should be done through
-    this initial ``Application`` instance.
-
-    Instantiating an ``Application`` will automatically open a WellCAD instance
-    if there is not one already open, or connect to an existing WellCAD
-    instance if there is one open.
-
-    Before using the COM API, ensure WellCAD has been started at least once by
-    an administrator in order to register it in the computer registry.
-
-    Example
-    -------
-    >>> import wellcad.com
-    >>> app = wellcad.com.Application()
-    >>> app.show_window()
-    True
-    >>> app.new_borehole()
-    <wellcad.com._borehole.Borehole object at 0x000001D6973FBD30>
-    """
-
-    _DISPATCH_METHODS = ("ShowWindow", "NewBorehole", "OpenBorehole",
-        "GetBorehole", "GetActiveBorehole", "FileImport", "MultiFileImport")
-    
-    def __new__(cls):
-        return object.__new__(cls)
-    
-    def __init__(self):
-        super().__init__(Dispatch("WellCAD.Application"))
-        
-    def show_window(self):
-        """Attempts to display the WellCAD workspace on screen.
-        
-        Returns
-        -------
-        bool
-            Whether the window was successfully shown.
-        """
-        return self._dispatch.ShowWindow()
-        
-    def minimize_window(self):
-        """Collapses the application window to an icon."""
-        self._dispatch.MinimizeWindow()
-    
-    def maximize_window(self):
-        """Extends the application window to full screen."""
-        self._dispatch.MaximizeWindow()
-    
-    def cascade(self):
-        """Cascades all borehole document windows (unless tabbed)."""
-        self._dispatch.Cascade()
-    
-    def tile_horizontally(self):
-        """Arranges document windows horizontally (unless tabbed)."""
-        self._dispatch.TileHorizontally()
-    
-    def tile_vertically(self):
-        """Arranges document windows vertically (unless tabbed)."""
-        self._dispatch.TileVertically()
-    
-    def new_borehole(self, template=None):
-        """Creates a new borehole document object.
-
-        The new borehole object is blank unless a template file is provided.
-        
-        Parameters
-        ----------
-        template : str, optional
-            An optional path to a borehole document template (.wdt).
-            If provided, the new borehole will be created using the
-            template.
-        
-        Returns
-        -------
-        Borehole
-            The new borehole document.
-        """
-        return Borehole(self._dispatch.NewBorehole(template))
-
-        
-    def open_borehole(self, path=None):
-        """Opens a WellCAD borehole document file (.wcl file).
-        
-        Parameters
-        ----------
-        path : str, optional
-            The file path to the WellCAD borehole document file to open. If no
-            file path is provided, the user will be prompted to select a file
-            using a standard File Open dialog box.
-        
-        Returns
-        -------
-        Borehole or None
-            The opened borehole document, or ``None`` if opening the file
-            failed.
-        """
-        return Borehole(self._dispatch.OpenBorehole(path))
-        
-
-    def get_borehole(self, index=None):
-        """Gets an existing borehole document by index.
-        
-        Gets a borehole document object according to the zero-based index of
-        the document open in WellCAD.
-        
-        Parameters
-        ----------
-        index : int, optional
-            A zero based index of the borehole document. If no index is
-            provided, the index of the most recently used document is used.
-        
-        Returns
-        -------
-        Borehole or None
-            The borehole document object with the specified index, or ``None``
-            if the index is out of bounds.
-        """
-        return Borehole(self._dispatch.GetBorehole(index))
-        
-        
-    def get_active_borehole(self):
-        """Gets the active borehole document (i.e. the one that currently has focus).
-                   
-        Returns
-        -------
-        Borehole or None
-            The current active borehole document object, or ``None`` if no
-            document has focus.
-        """
-        return Borehole(self._dispatch.GetActiveBorehole())
-        
-        
-    def close_borehole(self, prompt_for_saving=None, index=None):
-        """Closes a specific borehole document.
-        
-        The borehole document that is closed can be specified by an index,
-        or, if none is provided, the most recently opened borehole document
-        will be closed.
-        
-        Parameters
-        ----------
-        prompt_for_saving : bool, optional
-            Whether or not to prompt the user to save the borehole document.
-        index : int or str, optional
-            The (zero-based) index of the document to close, or the document
-            name. If not provided, the most recently opened document will be
-            closed.
-        """
-        self._dispatch.CloseBorehole(prompt_for_saving, index)
-    
-    @property
-    def nb_of_documents(self):
-        """int: The number of borehole documents open in WellCAD."""
-        return self._dispatch.NbOfDocuments
-    
-    def file_import(self,
-                    file_name=None,
-                    prompt_user=None,
-                    config_file=None,
-                    log_file=None):
-        """Imports the specified file into a new borehole document.
-        
-        Allows import of TFD, LAS, DLIS, TXT, CSV and other file
-        formats into WellCAD. Please refer to the WellCAD help
-        file for a description of all import parameters to be used
-        in the configuration file / parameter string. If filename
-        is left blank the File Open dialog will be displayed. 
-
-        Parameters
-        ----------
-        file_name : str, optional
-            The path of the file to import.
-        prompt_user : bool, optional
-            Whether to display an import dialog box to allow the user
-            to specify import settings.
-        config_file : str, optional
-            Path and filename of the configuration file or parameter string.
-        log_file : str, optional
-            Path and name of the file to log error messages.
-        
-        Returns
-        -------
-        Borehole
-            A new borehole document containing the imported data.
-        """
-        return Borehole(self._dispatch.FileImport(file_name,
-                                                  prompt_user,
-                                                  config_file,
-                                                  log_file))
-        
-    def multi_file_import(self,
-                          file_name=None,
-                          prompt_user=None,
-                          config_file=None,
-                          log_file=None):
-        """Creates a single borehole document from all specified files.
-
-        Allows import of multiple TFD, LAS, DLIS, TXT, CSV and other
-        file formats into WellCAD. Imported data will be merged into
-        the same document. Please refer to the WellCAD help file for
-        a description of all import parameters to be used in the
-        configuration file / parameter string. If filename is left
-        blank the File Open dialog will be displayed.
-
-        Parameters
-        ----------
-        file_name : str, optional
-            A comma separated list of input files (path and file name). 
-        prompt_user : bool, optional
-            Boolean to display the import dialog boxes.
-        config_file : str, optional
-            Path and filename of the configuration file or parameter string.
-        log_file : str, optional
-            Path and name of the file to log error messages.
-        
-        Returns
-        -------
-        Borehole
-            A newly created borehole document containing the data from the
-            imported files.
-        """
-        return Borehole(self._dispatch.MultiFileImport(file_name,
-                                                       prompt_user,
-                                                       config_file,
-                                                       log_file))       
-    
-    def quit(self, prompt_for_saving=None):
-        """Closes all borehole documents and exits WellCAD.
-        
-        Parameters
-        ----------
-        prompt_for_saving : bool, optional
-            Whether to display the Save As dialog box for unsaved documents.
-            Default behaviour is to prompt the user.
-        """
+from win32com.client import Dispatch
+from ._dispatch_wrapper import DispatchWrapper
+from ._borehole import Borehole
+
+class Application(DispatchWrapper):
+    """The core class used to interact with WellCAD via its COM API.
+
+    In general, it is the only class you should instantiate directly. All
+    interaction with borehole documents, logs, etc, should be done through
+    this initial ``Application`` instance.
+
+    Instantiating an ``Application`` will automatically open a WellCAD instance
+    if there is not one already open, or connect to an existing WellCAD
+    instance if there is one open.
+
+    Before using the COM API, ensure WellCAD has been started at least once by
+    an administrator in order to register it in the computer registry.
+
+    Example
+    -------
+    >>> import wellcad.com
+    >>> app = wellcad.com.Application()
+    >>> app.show_window()
+    True
+    >>> app.new_borehole()
+    <wellcad.com._borehole.Borehole object at 0x000001D6973FBD30>
+    """
+
+    _DISPATCH_METHODS = ("ShowWindow", "NewBorehole", "OpenBorehole",
+        "GetBorehole", "GetActiveBorehole", "FileImport", "MultiFileImport")
+    
+    def __new__(cls):
+        return object.__new__(cls)
+    
+    def __init__(self):
+        super().__init__(Dispatch("WellCAD.Application"))
+        
+    def show_window(self):
+        """Attempts to display the WellCAD workspace on screen.
+        
+        Returns
+        -------
+        bool
+            Whether the window was successfully shown.
+        """
+        return self._dispatch.ShowWindow()
+        
+    def minimize_window(self):
+        """Collapses the application window to an icon."""
+        self._dispatch.MinimizeWindow()
+    
+    def maximize_window(self):
+        """Extends the application window to full screen."""
+        self._dispatch.MaximizeWindow()
+    
+    def cascade(self):
+        """Cascades all borehole document windows (unless tabbed)."""
+        self._dispatch.Cascade()
+    
+    def tile_horizontally(self):
+        """Arranges document windows horizontally (unless tabbed)."""
+        self._dispatch.TileHorizontally()
+    
+    def tile_vertically(self):
+        """Arranges document windows vertically (unless tabbed)."""
+        self._dispatch.TileVertically()
+    
+    def new_borehole(self, template=None):
+        """Creates a new borehole document object.
+
+        The new borehole object is blank unless a template file is provided.
+        
+        Parameters
+        ----------
+        template : str, optional
+            An optional path to a borehole document template (.wdt).
+            If provided, the new borehole will be created using the
+            template.
+        
+        Returns
+        -------
+        Borehole
+            The new borehole document.
+        """
+        return Borehole(self._dispatch.NewBorehole(template))
+
+        
+    def open_borehole(self, path=None):
+        """Opens a WellCAD borehole document file (.wcl file).
+        
+        Parameters
+        ----------
+        path : str, optional
+            The file path to the WellCAD borehole document file to open. If no
+            file path is provided, the user will be prompted to select a file
+            using a standard File Open dialog box.
+        
+        Returns
+        -------
+        Borehole or None
+            The opened borehole document, or ``None`` if opening the file
+            failed.
+        """
+        return Borehole(self._dispatch.OpenBorehole(path))
+        
+
+    def get_borehole(self, index=None):
+        """Gets an existing borehole document by index.
+        
+        Gets a borehole document object according to the zero-based index of
+        the document open in WellCAD.
+        
+        Parameters
+        ----------
+        index : int, optional
+            A zero based index of the borehole document. If no index is
+            provided, the index of the most recently used document is used.
+        
+        Returns
+        -------
+        Borehole or None
+            The borehole document object with the specified index, or ``None``
+            if the index is out of bounds.
+        """
+        return Borehole(self._dispatch.GetBorehole(index))
+        
+        
+    def get_active_borehole(self):
+        """Gets the active borehole document (i.e. the one that currently has focus).
+                   
+        Returns
+        -------
+        Borehole or None
+            The current active borehole document object, or ``None`` if no
+            document has focus.
+        """
+        return Borehole(self._dispatch.GetActiveBorehole())
+        
+        
+    def close_borehole(self, prompt_for_saving=None, index=None):
+        """Closes a specific borehole document.
+        
+        The borehole document that is closed can be specified by an index,
+        or, if none is provided, the most recently opened borehole document
+        will be closed.
+        
+        Parameters
+        ----------
+        prompt_for_saving : bool, optional
+            Whether or not to prompt the user to save the borehole document.
+        index : int or str, optional
+            The (zero-based) index of the document to close, or the document
+            name. If not provided, the most recently opened document will be
+            closed.
+        """
+        self._dispatch.CloseBorehole(prompt_for_saving, index)
+    
+    @property
+    def nb_of_documents(self):
+        """int: The number of borehole documents open in WellCAD."""
+        return self._dispatch.NbOfDocuments
+    
+    def file_import(self,
+                    file_name=None,
+                    prompt_user=None,
+                    config_file=None,
+                    log_file=None):
+        """Imports the specified file into a new borehole document.
+        
+        Allows import of TFD, LAS, DLIS, TXT, CSV and other file
+        formats into WellCAD. Please refer to the WellCAD help
+        file for a description of all import parameters to be used
+        in the configuration file / parameter string. If filename
+        is left blank the File Open dialog will be displayed. 
+
+        Parameters
+        ----------
+        file_name : str, optional
+            The path of the file to import.
+        prompt_user : bool, optional
+            Whether to display an import dialog box to allow the user
+            to specify import settings.
+        config_file : str, optional
+            Path and filename of the configuration file or parameter string.
+        log_file : str, optional
+            Path and name of the file to log error messages.
+        
+        Returns
+        -------
+        Borehole
+            A new borehole document containing the imported data.
+        """
+        return Borehole(self._dispatch.FileImport(file_name,
+                                                  prompt_user,
+                                                  config_file,
+                                                  log_file))
+        
+    def multi_file_import(self,
+                          file_name=None,
+                          prompt_user=None,
+                          config_file=None,
+                          log_file=None):
+        """Creates a single borehole document from all specified files.
+
+        Allows import of multiple TFD, LAS, DLIS, TXT, CSV and other
+        file formats into WellCAD. Imported data will be merged into
+        the same document. Please refer to the WellCAD help file for
+        a description of all import parameters to be used in the
+        configuration file / parameter string. If filename is left
+        blank the File Open dialog will be displayed.
+
+        Parameters
+        ----------
+        file_name : str, optional
+            A comma separated list of input files (path and file name). 
+        prompt_user : bool, optional
+            Boolean to display the import dialog boxes.
+        config_file : str, optional
+            Path and filename of the configuration file or parameter string.
+        log_file : str, optional
+            Path and name of the file to log error messages.
+        
+        Returns
+        -------
+        Borehole
+            A newly created borehole document containing the data from the
+            imported files.
+        """
+        return Borehole(self._dispatch.MultiFileImport(file_name,
+                                                       prompt_user,
+                                                       config_file,
+                                                       log_file))       
+    
+    def quit(self, prompt_for_saving=None):
+        """Closes all borehole documents and exits WellCAD.
+        
+        Parameters
+        ----------
+        prompt_for_saving : bool, optional
+            Whether to display the Save As dialog box for unsaved documents.
+            Default behaviour is to prompt the user.
+        """
         self._dispatch.Quit(prompt_for_saving)
```

### Comparing `pywellcad-0.2.0/wellcad/com/_borehole.py` & `pywellcad-0.2.1/wellcad/com/_borehole.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,4195 +1,4195 @@
-from ._dispatch_wrapper import DispatchWrapper
-from ._log import Log
-from ._depth import Depth
-from ._header import Header
-from ._title import Title
-from ._page import Page
-from ._workspace import Workspace
-from ._odbc import Odbc
-
-
-class Borehole(DispatchWrapper):
-    _DISPATCH_METHODS = ("Log", "ApplyStructureTrueToApparentCorrection", "ApplyStructureApparentToTrueCorrection",
-                         "RemoveStructuralDip", "ExtractStructureIntervalStatistic", "ColorClassification",
-                         "RepresentativePicks", "ImageComplexityMap", "NormalizeImage", "OrientImageToNorth",
-                         "FilterImageLog", "ApplyConditionalTesting", "RQD", "GrainSizeSorting", "StackTraces",
-                         "AverageFilterFWSLog", "FreqFilterFwsLog", "ApplyStandOffCorrection",
-                         "CompensatedVelocity", "ApplySemblanceProcessing", "ProcessReflectedTubeWave",
-                         "PickFirstArrival", "PickE1Arrival", "ExtractE1Amplitude", "AdjustPickToExtremum",
-                         "ExtractWindowPeakAmplitude", "ApplyNaturalGammaBoreholeCorrection",
-                         "ApplyTotalGammaCalibration", "CorrectDeadSensor", "CalculateFluidVelocity",
-                         "CalculateApparentMetalLoss", "GetLog", "CreateNewWorkspace",  "Workspace", "FileExport",
-                         "ConvertLogTo", "FilterLog", "ResampleLog", "InterpolateLog", "ElogCorrection",
-                         "NMRFluidVolumes", "ROPAverage", "SharpenRGBLog", "RetinexFilterRGBLog", )
-
-    @property
-    def name(self):
-        """str: The title of a borehole document."""
-        return self._dispatch.Name
-
-    @name.setter
-    def name(self, name):
-        self._dispatch.Name = name
-
-    @property
-    def version_major(self):
-        """int: The major version number of WellCAD."""
-        return self._dispatch.VersionMajor
-
-    @property
-    def version_minor(self):
-        """int: The minor version number of WellCAD."""
-        return self._dispatch.VersionMinor
-
-    @property
-    def version_build(self):
-        """int: The build number of WellCAD."""
-        return self._dispatch.VersionBuild
-
-    @property
-    def top_depth(self):
-        """float: The top depth of a borehole in units of the master depth axis."""
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of a borehole in units of the master depth axis."""
-        return self._dispatch.BottomDepth
-
-    @property
-    def nb_of_logs(self):
-        """int: The number of logs in a borehole."""
-        return self._dispatch.NbOfLogs
-
-    @property
-    def auto_update(self):
-        """bool: The auto update status of the borehole."""
-        return self._dispatch.AutoUpdate
-
-    @auto_update.setter
-    def auto_update(self, flag):
-        self._dispatch.AutoUpdate = flag
-
-    def refresh_window(self):
-        """Performs a one time refresh of the borehole view"""
-        self._dispatch.RefreshWindow()
-
-    def show_window(self):
-        """Puts the borhole into focus."""
-        self._dispatch.ShowWindow()
-
-    def set_draft_mode(self, display_mode=None):
-        """Toggles the view of the borehole document.
-
-        Parameters
-        ----------
-        display_mode : int, optional
-            The document viewing mode.  A borehole document can be displayed in the following modes:
-
-                * 0 = Page Layout
-                * 1 = Draft and fit
-                * 2 = Draft
-        """
-        self._dispatch.SetDraftMode(display_mode)
-
-    def minimize_window(self):
-        """Shrinks the document window to an icon.
-
-        Works only if document windows are not tabbed.
-        """
-        self._dispatch.MinimizeWindow()
-
-    def maximize_window(self):
-        """Enlarges the document window to fit the WellCAD frame.
-
-        Works only if document windows are not tabbed.
-        """
-        self._dispatch.MaximizeWindow()
-
-    def set_visible_depth_range(self, top_depth=None, bottom_depth=None):
-        """Adjusts the depth range displayed in a borehole view.
-
-        Parameters
-        ----------
-        top_depth : float
-            The top depth of the visible depth range.
-            If not provided, the current top depth of the document will be used
-        bottom_depth : float
-            The bottom depth of the visible depth range.
-            If not provided, the current bottom depth of the document will be used
-        """
-        self._dispatch.SetVisibleDepthRange(top_depth, bottom_depth)
-
-    @property
-    def depth(self):
-        """Depth: The reference/master vertical axis. Can be in depth or time."""
-        return Depth(self._dispatch.Depth)
-
-    @property
-    def header(self):
-        """Header: The document header for this borehole document."""
-        return Header(self._dispatch.Header)
-
-    @property
-    def page(self):
-        """Page: A page object for the borehole document."""
-        return Page(self._dispatch.Page)
-
-    def create_new_workspace(self, workspace_type, config):
-        """Creates a new workspace object.
-
-        Parameters
-        ----------
-        workspace_type : int
-            * 1 = ISI workspace
-            * 2 = Casing integrity
-            * 3 = NMR
-        config : str
-            Path to a configuration file containing the workspace initialization parameters. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ISIWorkspace]
-                Name= workspace name
-                Log= log name
-                Caliper=100
-                DepthOfImage=0
-                CaliperUnit=mm / inch
-                ApertureUnit=mm / inch/10
-                LengthUnit=m / mm / cm / ft / inch / inch/10
-                RunApparentToTrue=yes
-                Azimuth= log name
-                Tilt= log name
-                ImageOrientation=North / High Side
-                RunRecalculateAzimuth=yes
-                RotationAngle=-12
-                NavigationLog=ICM (log name or nothing)
-                ' RGB OTV image
-                ImageType= 0,
-                'Greyscale OTV image.
-                ImageType=1
-                ' Diamond-drilled hole, ATV image
-                ImageType=2
-                'RC-drilled hole, ATV image
-                ImageType=3
-                'FMI image
-                ImageType=4
-                ICMPalette=0,0,0,255,56,255,0,0,12,64,224,208,21,50,205,50,31,255,255,0,39,255,215,0,47,255,104,32
-                [CasingIntegrityWorkspace]
-                Name= workspace name
-                Log= log name
-                LogUnit=mm / inch
-                DataType=radius / diameter
-                DrillerCasingTable=C:/Temp/Table.txt
-                DrillerCasingTableDepthUnit=meters / feet
-                DrillerCasingTableWeightUnit=lbs/ft / kg/m
-                DrillerCasingTableODUnit=inch / mm
-                [NMRWorkspace]
-                Name= workspace name
-                T2Distribution= log name
-                TraceUnitOfT2Distribution=milliseconds / seconds
-                DefaultLithoDatabase=C:/Program Files/Advanced Logic Technology/WellCAD/Dictionaries/NMR Volumes.lth
-                FluidVolumeComponents=Bound Water, Moveable Water
-                FluidVolumeLithoUseAssociatedColor=no
-                DefaultCutoffValues=33
-                LastDefaultCutoffValueMax=yes
-                DisplayPermeabilityTIMModel=yes
-                PermeabilityTIMModelVariableC=1 (i.e. premultiplier)
-                PermeabilityTIMModelExponentM=4
-                PermeabilityTIMModelExponentN=2
-                PermeabilityTIMModelBFVandFFVLimit= Bound Water
-                DisplayPermeabilitySDRModel=yes
-                PermeabilitySDRModelVariableC=1 (i.e. premultiplier)
-                PermeabilitySDRModelExponentM=4
-                PermeabilitySDRModelExponentN=2
-                DisplayDryMatrixDensity=no
-                BulkDensity=Bulk_Density
-
-        Returns
-        -------
-        Workspace
-            The new workspace object.
-        """
-        return Workspace(self._dispatch.CreateNewWorkspace(workspace_type, config))
-
-    def workspace(self, workspace_id):
-        """Gets an existing workspace object in the document.
-
-        Parameters
-        ----------
-        workspace_id : int or str
-            The zero based index or the name of the workspace
-        Returns
-        -------
-        Workspace or None
-            The workspace object with the specified index or name, or ``None``
-            if the index is out of bounds or if name does not match any of the workspace name.
-        """
-        return Workspace(self._dispatch.Workspace(workspace_id))
-
-    def check_formula(self, formula):
-        """Verifies the syntax of a formula used in a Formula Log.
-
-        Parameters
-        ----------
-        formula : str
-            The formula that needs to be checked.
-            Example: "({GR}-min({GR}))/(max({GR})- min({GR}))"
-
-        Returns
-        -------
-        bool
-            Whether the formula is correct or not.
-        """
-        return self._dispatch.CheckFormula(formula)
-
-    @property
-    def odbc(self):
-        """Odbc: An ODBC object that allows interaction with a database."""
-        return Odbc(self._dispatch.ODBC)
-
-    def connect_to(self, server_name, server_address, port_number):
-        """Connects the current borehole document to an external data source provider.
-
-        Parameters
-        ----------
-        server_name : str
-            The name of the server (TFD is currently the only one supported)
-        server_address : str
-            The IP address of the computer to connect to.
-        port_number : int
-            The part number to connect to.
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
-        """
-
-        self._dispatch.ConnectTo(server_name, server_address, port_number)
-
-    def disconnect_from(self, server_name, server_address):
-        """Cuts the connection between the borehole document and the external data source provider.
-
-        Parameters
-        ----------
-        server_name : str
-            The name of the server (TFD is currently the only one supported)
-        server_address : str
-            The IP address of the computer connected to.
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
-        """
-        self._dispatch.DisconnectFrom(server_name, server_address)
-
-    def save_as(self, path):
-        """Saves the borehole document as WCL file.
-
-        Parameters
-        ----------
-        path : str, optional
-            The file path to the WellCAD borehole document file to save. If no
-            file path is provided, the user will be prompted to select a file
-            using a standard File Save As dialog box.
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
-        """
-        return self._dispatch.SaveAs(path)
-
-    def file_export(self, file_name=None, prompt_user=None, config=None, log_file=None):
-        """Exports the document to the specified file.
-
-        Supported file formats are LAS, DLIS, EMF, CGM, JPG, PNG, TIF,
-        BMP, WCL and PDF. Please refer to the WellCAD help file for a
-        description of the export parameters to be used in the
-        configuration file and parameter string.
-
-        Parameters
-        ----------
-        file_name : str, optional
-            The path and name of the file to export.
-            If not provided, the dialog will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [LASExport]
-                ; LAS files
-                ; For compatibility with older versions of WellCAD:
-                NbEndDepthDigits = 4
-                NbSmpRateDigits = 4
-                LASVersion = 2 / 3
-                Log1 = Depth,Auto,Auto (Log name, Precision, Column width)
-                Log2 = GR, 0, 10
-                'Log3 = … (if no Log is specified all logs will be exported)
-                MaxDepthRange = yes / no
-                TopDepth = 0.0
-                BottomDepth = 150.0
-                SamplingRate = 0.1
-                EnableHeader = yes / no
-                EnableWrap = yes / no
-                NullValue = -999.25
-                Delimiter = 0 (Comma) /1 (Tab) / 2 (Space)
-                CheckConstSmpRate = yes (optional)
-                LimitLineLength = no (optional)
-                ShortMnemonics = no (optional)
-                AlignColumns = yes (optional)
-                ForceDecimalPoint = yes (optional)
-                SignificantDigits = 7 (optional)
-                [DLISExport]
-                ; DLIS files
-                ; If no Log is specified all logs will be exported
-                Log1 = GR
-                Log2 = RHO
-                [ImageExport]
-                ; JPG, PNG, BMP, GIF, TIF files
-                MaxDepthRange = yes / no
-                TopDepth= 0.0
-                BottomDepth= 10.0
-                Resolution=300
-                [EMFExport]
-                ; EMF files
-                MaxDepthRange = yes / no
-                TopDepth= 0.0
-                BottomDepth= 10.0
-                [CGMExport]
-                ; CGM files
-                MaxDepthRange = yes / no
-                TopDepth= 0.0
-                BottomDepth= 10.0
-                [PDFExport]
-                ; PDF files
-                MaxDepthRange = yes / no
-                TopDepth= 0.0
-                BottomDepth= 10.0
-                ; Single page
-                PageStyle=Single
-                ShowProgress=TRUE
-                OpenPDFFile=TRUE
-                ; Standard page
-                PageStyle=Standard
-                Orientation=Portrait / Landscape
-                PaperSize=A4
-                ShowProgress=TRUE
-                OpenPDFFile=TRUE
-                ; Custom page
-                PageStyle=Custom
-                Orientation=Portrait
-                'Orientation=Landscape
-                PaperWidth=2100
-                PaperLength=2970
-                ShowProgress=TRUE
-                OpenPDFFile=TRUE
-                [WCLExport]
-                ; WCL files
-                Format = 5.0
-        log_file : str, optional
-            Path and name of the file to log error messages.
-
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
-        """
-        return self._dispatch.FileExport(file_name, prompt_user, config, log_file)
-
-    def do_print(self, enable_dialog=None, top_depth=None, bottom_depth=None, nb_of_copies=None):
-        """Sends the current document to the printer.
-        If the print dialog box is displayed the user can select the
-        printer otherwise the printer installed as default is used.
-
-        Parameters
-        ----------
-        enable_dialog : bool, optional
-            Whether to display the print dialog box or not.
-        top_depth : float, optional
-            The start depth of the interval to print
-            If not provided, the current top depth of the document will be used.
-        bottom_depth : float, optional
-            The bottom depth of the printed depth interval.
-            If not provided, the current bottom depth of the document will be used.
-        nb_of_copies : int, optional
-            The number of copies to be printed.
-        """
-        self._dispatch.DoPrint(enable_dialog, top_depth, bottom_depth, nb_of_copies)
-
-    def read_database(self, script_path):
-        """Opens and interprets an SQL script to download data from a database.
-
-        Parameters
-        ----------
-        script_path : str
-            The path to the SQL script to be called
-
-        Returns
-        -------
-        bool
-            Whether the operation was successful or not.
-        """
-        return self._dispatch.ReadDatabase(script_path)
-
-    def write_database(self, script_path):
-        """Opens and interprets an SQL script to upload data to a database.
-
-        Parameters
-        ----------
-        script_path : str
-            The path to the SQL script to be called
-
-        Returns
-        -------
-        bool
-            Whether the operation was successful or not.
-        """
-        return self._dispatch.WriteDatabase(script_path)
-
-    def get_log(self, index_or_name):
-        """Gets an existing log object in the document.
-
-        Parameters
-        ----------
-        index_or_name :  int or str
-            The zero based index or the name of the log.
-        Returns
-        -------
-        Log
-            The log object with the specified index or name, or ``None``
-            if the index is out of bounds or if name does not match any of the log name.
-        """
-        return Log(self._dispatch.GetLog(index_or_name))
-
-    def title(self, name):
-        """Gets the title object for the specified name.
-
-        Parameters
-        ----------
-        name : str, optional
-            The name of the log or the name of a title box.
-        Returns
-        -------
-        Title
-            The Title object if found, otherwise "None"
-        """
-        return Title(self._dispatch.Title(name))
-
-    def insert_new_log(self, log_type):
-        """Creates a new log and log object.
-
-        Parameters
-        ----------
-            log_type : int, optional
-                The type of log.  Allowed values are :
-
-                    * 1 = Well Log
-                    * 2 = Formula Log
-                    * 3 = Mud Log
-                    * 4 = FWS Log
-                    * 5 = Image Log
-                    * 6 = Structure Log
-                    * 7 = Litho Log
-                    * 8 = Comment Log
-                    * 9 = Engineering Log
-                    * 10 = RGB Log
-                    * 13 = Interval Log
-                    * 14 = Analysis Log
-                    * 15 = Percent Log
-                    * 16 = CoreDesc Log
-                    * 17 = Depth Log
-                    * 18 = Strata Log
-                    * 19 = Stacking Pattern Log
-                    * 20 = Polar and Rose Log
-                    * 21 = Cross Section Log
-                    * 22 = OLE Log
-                    * 23 = Shading Log
-                    * 24 = Marker Log
-                    * 25 = Breakout Log
-                    * 26 = Bio Log
-                    * 27 = Lineation Log
-        Returns
-        -------
-        Log
-            A log object.
-        """
-        return Log(self._dispatch.InsertNewLog(log_type))
-
-    def convert_log_to(self, log, log_type, prompt_user=None, config=None):
-        """New log object by converting one log type into another.
-
-        Please refer to the WellCAD documentation about which log type
-        conversions are possible.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log to convert.
-        log_type : int
-            The type of log to be created.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ConvertLog]
-                ; Analysis, Percentage Log to Litho log
-                ; ComponentNames : list of component names to convert, if not specified all components are taken
-                ComponentNames=A,B
-                ; Bio Log to Bio Log
-                ; TaxonNames : list of taxon names to convert, if not specified all taxons are taken
-                TaxonNames=A,B
-                ; Image, RGB Log to WellLog
-                StartIndex=0
-                Increment=1
-                ; Breakout Log to Breakout, Mud Log
-                FilterOnAttributes= yes / no
-                AttributeName1=Type
-                AttributeList1=RF,MB,…
-                AttributeName2=Condition
-                AttributeList2=Open,Loose,…
-                FilterOnAzimuth= yes / no
-                AzimuthLow=0
-                AzimuthHigh=360
-                FilterOnTilt= yes / no
-                TiltLow=30
-                TiltHigh=90
-                FilterOnLength= yes / no
-                LengthLow=0
-                LengthHigh=100
-                FilterOnOpening= yes / no
-                OpeningLow=0
-                OpeningHigh=45
-                ; Comment Log to Litho Log
-                LithoDatabase=C:/Default.lth
-                ; CoreDesc Log to Interval Log
-                ; CoreDescItemNames : list of symbol codes to convert
-                CoreDescItemNames=AX3, AX5, BZ5
-                ; Structure Log to Structure, Mud Log
-                FilterOnAttributes=TRUE
-                AttributeName1=Type
-                AttributeList1=RF,MB
-                AttributeName2=Condition
-                AttributeList2=Open,Loose
-                FilterOnAzimuth= yes / no
-                AzimuthLow=0
-                AzimuthHigh=360
-                FilterOnTilt= yes / no
-                DipLow=30
-                DipHigh=90
-                FilterOnOpening= yes / no
-                ApertureLow=0
-                ApertureHigh=100
-                ; Structure, Breakout Log to Marker Log
-                DisplayIndex= yes / no
-                DisplayAzimuth= yes / no
-                DisplayTilt= yes / no
-                DisplayAttributes= yes / no
-                ; Interval Log to Mud Log
-                ; ConvertValue : 0=Min, 1=Max, 2=Ave
-                ; AttachDepthTo : 1=attach to top, 2=middle, 3=bottom
-                ConvertValue=0
-                AttachDepthTo=2
-                ; Mud Log to Well Log
-                ; Interpolation : 0 = No Interpolation, 1 = Prev. Data, 2 = Interpol.
-                CreateNewLog= yes / no
-                SamplingRate=0.1
-                MaximumGap=10.0
-                Interpolation=0
-                Tolerance=0.1
-                CircularData = yes / no
-                DataUnit = degrees / radians
-                ; Mud Log to Depth Log
-                ; ConversionType : 1=from m, 2=from ft, 3=from sec; 4=msec, 5=usec
-                ConversionType=1
-                ; Mud Log to Litho Log
-                ; <ClassifierName>=<LithoName> (classification name and corresponding litho code)
-                LithoDatabase=C:/Default.lth
-                className1 = Coal
-                className2 = Limestone
-                ; Percent Log to Analysis Log
-                SamplingRate=0.1
-                ; RGB Log to Image Log (int, float 2 and float 4)
-                ; Color : 0=all, 1=red, 2=green, 3=blue
-                Color=0
-                ; Stack Log to Well Log
-                SamplingRate=0.1
-                ; Strata Log to Comment, Litho Log
-                ; ColumnNames : list of column titles
-                ColumnNames=columnname1, columname4
-                ; VSP Log to Well Log
-                ; TraceNames : list of trace titles
-                TraceNames=
-                ; Well Log to Depth Log
-                ; ConversionType : 1=from m, 2=from ft, 3=from sec; 4=msec, 5=usec
-                ConversionType=1
-                ; Well Log to Litho Log
-                ; <ClassifierName>=<LithoName> (classification name and corresponding litho code)
-                ; SplitLithoLog : creates one litho column per litho type
-                LithoDatabase=C:/Default.lth
-                className1 = Coal
-                className2 = Limestone
-                SplitLithoLog= yes / no
-                ; Litho Log to Strata Log
-                ; SplitColumns : creates one column per litho type
-                SplitColumns= yes / no (creates one column per litho type)
-                ; Litho Log to Litho Log
-                ; LithoBedNames : list of litho codes to convert, if not specified all components are taken
-                LithoBedNames=sst,lst,dst
-
-        Returns
-        -------
-        Log
-            The object of the new log.
-        """
-        return Log(self._dispatch.ConvertLogTo(log, log_type, prompt_user, config))
-
-    def add_log(self, log):
-        """Adds the log object passed as argument of the function into the calling borehole document.
-
-        Parameters
-        ----------
-        log : Log
-            An object of the log to copy.
-        Returns
-        -------
-        Log
-            A copy of the log.
-        """
-        return Log(self._dispatch.AddLog(log._dispatch))
-
-    def remove_log(self, log):
-        """Deletes the specified log from the borehole document.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log to remove.
-        """
-        self._dispatch.RemoveLog(log)
-
-    def clear_log_contents(self, log):
-        """Removes the data from a log and leaves the log empty.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log to remove.
-        """
-        self._dispatch.ClearLogContents(log)
-
-    def apply_template(self, path, prompt_if_not_found=None, create_new_logs=None, create_new_layers=None,
-                       apply_annotation_settings=None, replace_header=None, keep_charts=None, new_charts=None,
-                       overwrite_workspaces=None, new_workspaces=None, delete_non_associated_logs=None, config=None):
-        """Loads and applies a document layout template (.WDT)
-
-        Parameters
-        ----------
-        path : str
-            The path and name of the template WDT file.
-        prompt_if_not_found : bool, optional
-            If True, a dialog box will be displayed for each log not found. Default : True.
-        create_new_logs : bool, optional
-            If True, new logs will be loaded from the template. Default : False.
-        create_new_layers : bool, optional
-            If True, new annotation layers will be loaded from the template. Default : False.
-        apply_annotation_settings : bool, optional
-            If True, settings  will be applied to annotations. Default : False.
-        replace_header : bool, optional
-            If True, the current document header will be replaced. Default : True.
-        keep_charts : bool, optional
-            If True, cross-plot charts will be kept in the document. Default : True.
-        new_charts : bool, optional
-            If True, cross-plot charts will be loaded from the template. Default : False.
-        overwrite_workspaces : bool
-            If True, work spaces in the document will be overwritten. Default : False.
-        new_workspaces : bool, optional
-            If True, work spaces will be loaded from the template. Default : False.
-        delete_non_associated_logs : bool, optional
-            If True, only logs from the template will be kept in the document. Default : True.
-        config : str, optional
-            Path and filename of the configuration file or parameter string.
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
-        """
-        return self._dispatch.ApplyTemplate(path, prompt_if_not_found, create_new_logs, create_new_layers,
-                                            apply_annotation_settings, replace_header, keep_charts, new_charts,
-                                            overwrite_workspaces, new_workspaces, delete_non_associated_logs, config)
-
-    def slice_log(self, log, slice_depth, create_top=None, create_bottom=None, keep_original=None):
-        """Allows the separation of the log data into a top and bottom section. New logs can be created \
-        holding the data of the top and bottom parts of the data set.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log to slice.
-        slice_depth : float
-            The depth at which the slice will be made.
-        create_top : bool, optional
-            If set to TRUE (default) a new log will be created holding the data from the current
-            top of the data set down to the slice depth..
-        create_bottom : bool, optional
-            If set to TRUE (default) a new log will be created holding the data from the slice depth
-            down to the bottom of the data set.
-        keep_original : bool, optional
-            If set to TRUE (default) the original log will be kept in the document.
-        """
-        self._dispatch.SliceLog(log, slice_depth, create_top, create_bottom, keep_original)
-
-    def merge_logs(self, log_a, log_b, ave_overlap=None, create_new=None):
-        """Merges the data of the two specified logs.
-
-        Parameters
-        ----------
-        log_a : str or int
-            The title or the zero based index of the log. If no new log is created this log
-            will receive the data from log_b.
-        log_b : str or int
-            The title or the zero based index of the log.
-        ave_overlap : bool, optional
-            If set to False log_a will overwrite log_b, if set to True, data from the two logs will be averaged
-            over the depth overlap.
-        create_new : bool
-            If set to False log_b will be pushed into log_a and the log_b will be removed
-        """
-        self._dispatch.MergeLogs(log_a, log_b, ave_overlap, create_new)
-
-    def merge_same_log_items(self, log):
-        """Merges consecutive data intervals of same litho codes, text or data within the specified log.
-        This function applies to Litho, Comment, Engineering, CoreDesc, Interval, Stack and Bio logs.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            The title or the zero based index of the log.
-        """
-        self._dispatch.MergeSameLogItems(log)
-
-    def extend_log(self, log, top_depth, bottom_depth):
-        """Extends the allocated depth range of Well, Formula and Analysis Logs.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the Well log.
-        top_depth : float
-            The new top depth of the log in units of the current depth axis.
-        bottom_depth : float
-            The new bottom depth of the log in units of the current depth axis.
-        """
-        self._dispatch.ExtendLog(log, top_depth, bottom_depth)
-
-    def depth_shift_log(self, log, shift, top_depth=None, bottom_depth=None):
-        """Allows the depth shifting of the log's data by the specified amount.
-        By default, the entire data column will be shifted (i.e. block shift). If a Top and Bottom depth
-        has been specified only the data within the specified interval will be shifted.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log.
-        shift : float
-            The amount of depth shift to be applied. A negative value will shift the data up and
-            a positive value applies a downward shift.
-        top_depth : float, optional
-            The upper depth limit of the shifted interval.
-            If not provided, this is the current top depth of the log
-        bottom_depth : float, optional
-            The lower depth limit of the shifted interval.
-            If not provided, this is the current bottom depth of the log
-        """
-        self._dispatch.DepthShiftLog(log, shift, top_depth, bottom_depth)
-
-    def depth_match_log(self, log=None, depth_log=None):
-        """Depth matches the specified log using the links created from the specified depth_log (i.e. a shift table).
-
-        Parameters
-        ----------
-        log : str or int, optional
-            The title or the zero based index of the log.
-            If not provided, the Depth Matcher dialog box will be displayed.
-        depth_log : str or int, optional
-            The title or the zero based index of the Depth log containing the shift table.
-            If not provided, the Depth Matcher dialog box will be displayed.
-        """
-        self._dispatch.DepthMatchLog(log, depth_log)
-
-    def fill_log(self, log, top_depth, bottom_depth, step, thickness, user_defined_intervals=None, interval_log=None):
-        """Fill a Cross-section Log or a Polar & Rose Log with intervals automatically.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log.
-        top_depth : float
-            The top depth of the first interval in units of the current depth axis.
-        bottom_depth : float
-            The last depth at which an interval could start in units of the current depth axis.
-        step : float
-            The frequency of the intervals in units of the current depth axis (every 2 m).
-        thickness : float
-            The interval thickness in units of the current depth axis.
-        user_defined_intervals : bool, optional
-            If set to False the intervals will be loaded from a reference log.
-        interval_log : str or int, optional
-            The title or the zero based index of the log containing the reference intervals.
-        """
-        self._dispatch.FillLog(log, top_depth, bottom_depth, step, thickness, user_defined_intervals, interval_log)
-
-    def filter_log(self, log, prompt_user=None, config=None):
-        """Calculates a new filtered data set of a Well Log.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [FilterLog]
-                ; FilterType : Median, MovingAverage, WeightedAverage
-                ; DataUnit : degrees, radians
-                FilterType =
-                FilterWidth = 5
-                MaxDepthRange = yes
-                TopDepth = 5.0
-                BottomDepth = 10.0
-                CircularData = yes
-                DataUnit = degrees
-
-        Returns
-        -------
-        Log
-            An object of the filtered log.
-        """
-        return Log(self._dispatch.FilterLog(log, prompt_user, config))
-
-    def block_log(self, log=None, prompt_user=None, config=None):
-        """Calculates statistical values for each depth interval determined from a
-        reference log or specified by the user.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            The title or the zero based index of the log.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [BlockLog]
-                CircularData = yes / no
-                DataUnit = degrees / radians
-                ReferenceInterval = Lithology / 10.0
-                Cumulate = yes / no
-                OutputLogAsText = yes / no
-                OutputLogAsGraphic = yes / no
-                Minimum = yes / no
-                Maximum = yes / no
-                Mode = yes / no
-                Average = yes / no
-                Median = yes / no
-                StdDev = yes / no
-                Percentage = yes / no
-                Sum = yes / no
-                SumNorm= yes / no
-                Area = yes / no
-                MeanAbsoluteDeviation = yes / no
-                GeometricMean = yes / no
-                GeometricStdDev = yes / no
-                Skewness = yes / no
-                Kurtosis = yes / no
-                Quartiles = yes / no
-                AveragePlusStdDev = yes / no
-                AverageMinusStdDev = yes / no
-                RMS = Yes / No
-                Value1 = 50 / NULL
-                Value2 = 100
-                Resolution = 0.1
-                EmptyIntervalMode = Interpolate / Maximum / Minimum / Null
-        """
-        self._dispatch.BlockLog(log, prompt_user, config)
-
-    def extract_well_log_statistics(self, logs=None, prompt_user=None, config=None):
-        """Extracts minimum, maximum, average, median and other statistical values fulfilling
-        an optional condition from each Well log
-
-        Parameters
-        ----------
-        logs : list, optional
-            The list of the titles or the zero base indexes of the logs to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ExtractWellLogStatistics]
-                ; Condition : 0=None, 1=lower than Value 1, 2=larger than Value1, 3=lower and equal,
-                ; 4=larger and equal,5=equal, 6=not equal, 7=between Value1 and Value2,
-                ; 8=between and equal to Value1 and Value2
-                Minimum = yes / no
-                Maximum = yes / no
-                Mode = yes / no
-                Average = yes / no
-                Median = yes / no
-                StandardDeviation = yes / no
-                Percentage = yes / no
-                MeanAbsoluteDeviation = yes / no
-                GeometricMean = yes / no
-                GeometricStandardDeviation = yes / no
-                Skewness = yes / no
-                Kurtosis = yes / no
-                Quartiles = yes / no
-                RMS = yes / no
-                RMSD = yes / no
-                Condition = 0
-                Value1 = 50
-                Value2 = 100
-                OneOutputlogPerImageLog = yes / no
-        """
-        self._dispatch.ExtractWellLogStatistics(logs, prompt_user, config)
-
-    def normalize(self, log=None, prompt_user=None, config=None):
-        """Normalizes the data in a Percentage or Analysis Log.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            The title or the zero based index of the log.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [AnalysisLogNormalize]
-                ComponentsToDelete= 20, 05#1, Artifacts (Codes of the patterns to be
-                removed separated by commas)
-                CreateNewLog=yes
-                At100=yes
-        """
-        self._dispatch.Normalize(log, prompt_user, config)
-
-    def tvd(self, log=None, prompt_user=None, config=None):
-        """Calculates a TVD either from another TVD log (Depth Log) or from a tilt log (Well Log).
-
-        Parameters
-        ----------
-        log : str or int, optional
-            The title or the zero based index of the log.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [TVD]
-                Output=TVD /Elevation
-                ExtrapolateBack=yes /no
-                TVDAtZero=0.0
-
-        Returns
-        -------
-        Log
-            The newly created Log containing the TVD data.
-        """
-        return Log(self._dispatch.TVD(log, prompt_user, config))
-
-    def rop_average(self, log=None, prompt_user=None, config=None):
-        """Computes the average rate of penetration over specified depth intervals
-        for a Mud Log or a Well Log.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            The title or the zero based index of the log.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ROPAverage]
-                ReferenceInterval=Litho ; log title or constant value indicating the interval height
-                OutputLogAsGraphic=no
-                OutputLogAsText=yes
-                DepthRange=Maximum ;Maximum, UserDefined, Zones, LogZones
-                TopDepth=105
-                BottomDepth=120
-                ;LogZones : top1, bot1, top2, bot2, ... topN, botN
-                LogZones=
-                ; LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
-                LogZonesDepthRange=Litho,06,05#1
-
-        Returns
-        -------
-        Log
-            The newly created Log.
-        """
-        return Log(self._dispatch.ROPAverage(log, prompt_user, config))
-
-    def unit_conversion(self, log=None, prompt_user=None, config=None):
-        """Converts the units used in a log.
-
-        Units are organized in categories (e.g. Length, Weight or Temperature).
-
-        Parameters
-        ----------
-        log : str or int, optional
-            The title or the zero based index of the log.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [UnitConversion]
-                Category=Length / Weight / Temperature
-                FromUnit=mm
-                ToUnit=in
-                CreateNewLogs=yes/no
-        """
-        self._dispatch.UnitConversion(log, prompt_user, config)
-
-    def zonation(self, logs=None, prompt_user=None, config=None):
-        """Splits log data into zones.
-
-        This is an automated version of the Zonation process in WellCAD.
-
-        Parameters
-        ----------
-        logs : list, optional
-            The list of the titles or the zero base indexes of the logs to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [Zonation]
-                UseIntervalThickness = yes/no (set to "no" to neglect theNbOuptutIntervals parameter)
-                NbOutputIntervals = 2
-                IntervalMinThickness = 0.5
-                UseLithoLogAsOutput = yes/no
-        """
-        self._dispatch.Zonation(logs, prompt_user, config)
-
-    def resample_log(self, log, prompt_user=None, config=None):
-        """Resamples a data set according to a new constant sampling rate or sample point
-        determined from a reference log.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ResampleLog]
-                ; For mud / well logs
-                ; ReferenceLog : log title of a Mud or Percentage Log
-                SamplingRate = 0.1
-                ReferenceLog = Plugs
-                UseReferenceLog = yes / no
-                UseNearestPoint = yes / no
-                CircularData = yes / no
-                DataUnit = degrees / radians
-                ; For image logs
-                VerticalSamplingFactor = 1
-                RadialSamplingFactor = 1
-                RadialDownSampling = yes / no
-        """
-        return Log(self._dispatch.ResampleLog(log, prompt_user, config))
-
-    def interpolate_log(self, log, prompt_user=None, config=None):
-        """Allows the interpolation of Mud and Well Log data to close no data gaps in a data set.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [InterpolateLog]
-                MaximumGap = 0.25
-                CircularData = yes / no
-                DataUnit = degrees / radians
-        Returns
-        -------
-        Log
-            An object of the interpolated log.
-        """
-        return Log(self._dispatch.InterpolateLog(log, prompt_user, config))
-
-    def auto_joint_detection(self, log, prompt_user=None, config=None):
-        """Detects the joints from the main log (data source) used
-        in the workspace.
-
-        Note: only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        log : str or int
-            The title or the zero based index of the log.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [AutoJointDetection]
-                Sensitivity = 5
-                TopAndBottom = yes
-        """
-        self._dispatch.AutoJointDetection(log, prompt_user, config)
-
-    def calculate_borehole_deviation(self, prompt_user=None, config=None):
-        """Calculates borehole Azimuth, RBR and Tilt from magnetometer and inclinometer / accelerometer data.
-
-        Parameters
-        ----------
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CalculateBoreholeDeviation]
-                ; MagX, MagY, MagZ : the title of the corresponding log
-                ; InclX, InclY, InclZ : the title of the corresponding log
-                MagX = Mag X
-                MagY = Mag Y
-                MagZ = Mag Z
-                InclX = Acc X
-                InclY = Acc Y
-                InclZ =
-                MagXPositive = yes / no
-                MagYPositive = yes / no
-                MagZPositive = yes / no
-                InclXPositive = yes / no
-                InclYPositive = yes / no
-                InclZPositive = yes / no
-                IsAccelerometer = yes / no
-                MarkerPosition = 182.5
-        """
-        self._dispatch.CalculateBoreholeDeviation(prompt_user, config)
-
-    def calculate_borehole_volume(self, prompt_user=None, config=None):
-        """Calculates the volume of an entire hole or annulus (e.g. between casing and borehole wall)
-        from an Image logs containing radius values or a Well logs providing caliper values.
-
-        Parameters
-        ----------
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            Note: This configuration is for WellCAD version 5.7 and onwards. For prior version, see the next section.
-
-            .. code-block:: ini
-
-                [VolumeProcess]
-                ; OuterDiam, InnerDiam : name of a well log, img log or a constant value
-                ; OuterDiamUnit, InnerDiamUnit : inch or mm, default to mm
-                ; OuterDiam1, InnerDiam1 : name of a well log, img log or a constant value.
-                ; Use either OuterDiam, InnerDiam or OuterDiam1, InnerDiam1 but not both !
-                ; OuterDiamUnit1, InnerDiamUnit1 : inch or mm, default to mm.
-                ; Use either OuterDiamUnit, InnerDiamUnit or OuterDiamUnit1, InnerDiamUnit1 but not both !
-                ; OuterDiam2, InnerDiam2 : name of a well log
-                ; OuterDiamUnit2, InnerDiamUnit2 : inch or mm, default to mm
-                ; IntervalRef : name of a well log or value (if value, in depth units of the borehole doc)
-                ; DepthRange : Maximum, UserDefined, Zones, LogZones
-                ; LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
-                OuterDiam=
-                OuterDiamUnit=mm
-                InnerDiam=
-                InnerDiamUnit=mm
-                OuterDiam1=w_diam_ext
-                OuterDiamUnit1=mm
-                OuterDiam2=
-                OuterDiamUnit2=mm
-                OuterDiam3=
-                OuterDiamUnit3=mm
-                OuterDiam4=
-                OuterDiamUni4t=mm
-                InnerDiamUnit=mm
-                InnerDiam1=
-                InnerDiamUnit1=mm
-                OuterDiamAsDiameter=yes
-                InnerDiamAsDiameter=yes
-                AnnularVolume=no
-                BottomToTop=yes
-                VolumeUnit=litre
-                DisplayTick=no
-                SmallTickFreq=1
-                MediumTickFreq=10
-                LargeTickFreq=100
-                DisplayNumerical=no
-                NumericalFreq=10
-                DisplayInterval=no
-                IntervalRef=10
-                DisplayCurve=yes
-                DepthRange=Maximum
-                TopDepth=10
-                BottomDepth=19
-                ZonesDepthRange=
-                LogZonesDepthRange=Litho,06,05#1
-
-
-            For WellCAD version 5.5 and 5.6, use this configuration instead:
-
-            .. code-block:: ini
-
-                [VolumeProcess]
-                InnerDiam = 100 / log name
-                InnerDiamUnit = mm/in/cm/ft/yd
-                OuterDiam = 110 / log name
-                OuterDiamUnit = mm/in/cm/ft/yd
-                AnnularVolume = yes/no
-                BottomToTop = yes/no
-                VolumeUnit = litre/cu.yd/cu.ft/cu.in/cu.cm/cu.m
-                DisplayTick = yes/no
-                SmallTickFreq = 1
-                MediumTickFreq = 10
-                LargeTickFreq = 100
-                DisplayNumerical = yes/no
-                NumericalFreq = 10
-                DisplayCurve = yes/no
-                DisplayInterval = yes/no
-                IntervalRef = 10
-                MaxDepthRange = yes/no
-                TopDepth = 0.0
-                BottomDepth = 123.5
-        """
-        self._dispatch.CalculateBoreholeVolume(prompt_user, config)
-
-    def calculate_borehole_coordinates(self, prompt_user=None, config=None):
-        """Calculates the deviation path coordinates Northing, Easting and TVD.
-
-        Parameters
-        ----------
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CalculateBoreholeCoordinates]
-                ; Method : Classic Tangential, Balanced Tangential, Radius Of Curvature, MinimumCurvature
-                ; AzimuthLog : the title of the log corresponding to the azimuth.
-                ; TiltLog : the title of the log corresponding to the tilt.
-                Method = Classic Tangential
-                Unit = m / ft
-                AzimuthLog = AZI
-                TiltLog = TILT
-                NewDepthLog = yes / no
-                CountTVDFromLogTop = yes / no
-                TVDStartDepth = 0.0
-                MagDeclination = 11.5
-                EstimateErrors = yes / no
-                AziError = 0.1
-                TiltError = 0.1
-        """
-        self._dispatch.CalculateBoreholeCoordinates(prompt_user, config)
-
-    def calculate_borehole_closure(self, prompt_user=None, config=None):
-        """Calculates the deviation path closure distance, closure angle and DLS.
-
-        Parameters
-        ----------
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CalculateBoreholeClosure]
-                ; AzimuthLog : the title of the log corresponding to the azimuth.
-                ; TiltLog : the title of the log corresponding to the tilt.
-                ; NorthingLog : the title of the log corresponding to the deviation along the north axis.
-                ; EastingLog : the title of the log corresponding to the deviation along the east axis.
-                AzimuthLog = AZI
-                TiltLog = TILT
-                NorthingLog = NORTH
-                EastingLog = EAST
-        """
-        self._dispatch.CalculateBoreholeClosure(prompt_user, config)
-
-    def elog_correction(self, prompt_user=None, config=None):
-        """Applies the environmental corrections for normal resisitivity data.
-
-        Parameters
-        ----------
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ElogCorrection]
-                ; Method : QL40-Elog (Bridle), QL40-Elog (Surface fish), Schlumberger
-                ; LogN8 : the title of the log corresponding to the electrode N8.
-                ; LogN16 : the title of the log corresponding to the electrode N16.
-                ; LogN32 : the title of the log corresponding to the electrode N32.
-                ; LogN64 : the title of the log corresponding to the electrode N64.
-                ; LogNx : the title of the log corresponding to the electrode Nx.
-                Method=QL40-Elog (Bridle)
-                LogN8=N8
-                LogN16=N16
-                LogN32=
-                LogN64=
-                LogNx=
-                ElectrodeSpacingNx=8
-                ElectrodeSpacingNxUnit=inch (in inch, in, inches or mm)
-                ElectrodeDiameter=1.57
-                ElectrodeDiameterUnit=inch (in inch, in, inches or mm)
-                BoreholeDiameter=2.20
-                BoreholeDiameterUnit=inch (in inch, in, inches or mm)
-                FluidResistivity=25 (log name or value in ohm.m)
-        Returns
-        -------
-        Log
-            An object of the last corrected log.
-        """
-        return Log(self._dispatch.ElogCorrection(prompt_user, config))
-
-    def correct_bad_traces(self, log=None):
-        """Replaces NULL data traces in Image, RGB and FWS logs.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        """
-        self._dispatch.CorrectBadTraces(log)
-
-    def stack_traces(self, is_spectrum=None, log=None, prompt_user=None, config=None):
-        """Stacks multiple FWS traces to create and average trace.
-
-        Parameters
-        ----------
-        is_spectrum : bool, optional
-            Whether the log is a spectrum or not.
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [StackTraces]
-                NumberOfStacks = 5
-        Returns
-        -------
-        Log
-            The resulting log.
-        """
-
-        return Log(self._dispatch.StackTraces(is_spectrum, log, prompt_user, config))
-
-    def slice_traces(self, log=None, prompt_user=None, config=None):
-        """Allows the user to keep only a portion of a FWS log's traces. Updates the log in place.
-        
-        Note: only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [SliceTraces]
-                start = 0  ; in log units
-                end = 0  ; in log units
-        """
-
-        self._dispatch.SliceTraces(log, prompt_user, config)
-
-    def apply_conditional_testing(self, log_if=None, log_then=None, prompt_user=None, config=None):
-        """Applies conditional testing (If-Then-Else) to image log
-        values.
-
-        Parameters
-        ----------
-        log_if : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log used for the 'If' clause.
-        log_then : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log used for the 'Then' clause.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ApplyConditionalTesting]
-                Condition = != / <= / >= / > / < / ==
-                ConditionValue = 100.0
-                IsSecondCondition = yes / no
-                SecondLogTest = <title of second log to test>
-                OperatorSecondCondition = AND / OR
-                SecondCondition = != / <= / >= / > / < / ==
-                SecondConditionValue = 120.0
-                ThenValue = NULL
-                ElseValue = Amplitude
-
-        Returns
-        -------
-        Log
-            A newly created log.
-        """
-        return Log(self._dispatch.ApplyConditionalTesting(log_if, log_then, prompt_user, config))
-
-    def filter_image_log(self, log=None, prompt_user=None, config=None):
-        """Average, median and clipping filter for image logs.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [FilterImageLog]
-                FilterType = Average / Median / Despiking
-                FilterWidth = 3
-                FilterHeight = 3
-                HighCutLimit = 75
-                LowCutLimit = 15
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-        return Log(self._dispatch.FilterImageLog(log, prompt_user, config))
-
-    def mirror_image(self, log=None):
-        """Rearranges the data within an image log so that the data
-        appears mirrored when compared to the original image.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        """
-        self._dispatch.MirrorImage(log)
-
-    def rotate_image(self, log=None, prompt_user=None, config=None):
-        """Rotate the image data by adding an angle (clockwise
-        rotation) or subtracting it (counterclockwise rotation).
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RotateImage]
-                RotateBy= 1.2 / Log
-                RotateClockwise = yes / no
-        """
-        self._dispatch.RotateImage(log, prompt_user, config)
-
-    def orient_image_to_highside(self, log=None, prompt_user=None, config=None):
-        """Rotates an image log to high side according to the
-        deviation channels provided.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [OrientImageToHighside]
-                InclX = Acc X
-                InclY = Acc Y
-                InclZ =
-                InclXPositive = yes / no
-                InclYPositive = yes / no
-                InclZPositive = yes / no
-                IsAccelerometer = yes / no
-                MarkerPosition = 180.2
-        """
-        self._dispatch.OrientImageToHighside(log, prompt_user, config)
-
-    def orient_image_to_north(self, log=None, prompt_user=None, config=None):
-        """Rotates an image log to magnetic north according to the
-        deviation channels provided.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-                        Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [OrientImageToNorth]
-                MagX = Mag X
-                MagY = Mag Y
-                MagZ = Mag Z
-                InclX = Acc X
-                InclY = Acc Y
-                InclZ =
-                MagXPositive = yes / no
-                MagYPositive = yes / no
-                MagZPositive = yes / no
-                InclXPositive = yes / no
-                InclYPositive = yes / no
-                InclZPositive = yes / no
-                IsAccelerometer = yes / no
-                MarkerPosition = 180.2
-        """
-        self._dispatch.OrientImageToNorth(log, prompt_user, config)
-
-    def extract_image_log_statistics(self, log=None, prompt_user=None, config=None):
-        """Extracts minimum, maximum, average, median and other
-        statistical values fulfilling an optional condition from each
-        image log trace.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ExtractImageLogStatistics]
-                Minimum = yes / no
-                Maximum = yes / no
-                Mode = yes / no
-                Average = yes / no
-                Median = yes / no
-                StandardDeviation = yes / no
-                Percentage = yes / no
-                MeanAbsoluteDeviation = yes / no
-                GeometricMean = yes / no
-                GeometricStandardDeviation = yes / no
-                Skewness = yes / no
-                Kurtosis = yes / no
-                Quartiles = yes / no
-                RMS = yes / no
-                RMSD = yes / no
-                Condition = 0 (None) / 1 (lower than Value 1) / 2 (larger than Value1) / 3 (lower and equal)
-                / 4 (larger and equal) / 5 (equal) / 6 (not equal) / 7 (between Value1 and Value2)
-                / 8 (between and equal to Value1 and Value2)
-                Value1 = 50
-                Value2 = 100
-                OneOutputlogPerImageLog = yes / no
-                DepthRange = Maximum / UserDefined / Zones / LogZones
-                TopDepth = 1.0
-                BottomDepth = 200.0
-                ZonesDepthRange = 10.0, 20.0, 50.0, 80.0 (top1, bottom1,...,topN, bottomN)
-                LogZonesDepthRange=Litho,06,05 (log name, interval code 1, interval code 2,...)
-        """
-        self._dispatch.ExtractImageLogStatistics(log, prompt_user, config)
-
-    def normalize_image(self, log=None, prompt_user=None, config=None):
-        """Applies Static or Dynamic normalization to image logs
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [NormalizeImage]
-                Mode = Static /Dynamic_1D / Dynamic_2D / HighPass
-                WindowHeight = 0.3
-                WindowWidth = 5
-
-
-        Returns
-        -------
-        Log
-            The normalized log.
-        """
-        return Log(self._dispatch.NormalizeImage(log, prompt_user, config))
-
-    def image_complexity_map(self, log=None, prompt_user=None, config=None):
-        """Computes the complexity map from an RGB or image log.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ImageComplexityMap]
-                LogType=1
-                ;RGB OTV image: 0,
-                ;Greyscale OTV image: 1,
-                ;Diamond-drilled hole, ATV image: 2,
-                ;RC-drilled hole, ATV image: 3,
-                ;FMI image: 4,
-                Palette=0,0,0,255,56,255,0,0,12,64,224,208,21,50,205,50,31,255,255,0,39,255,215,0,47,255,104,32
-
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-        return Log(self._dispatch.ImageComplexityMap(log, prompt_user, config))
-
-    def apply_structure_apparent_to_true_correction(self, log=None, prompt_user=None, config=None):
-        """Corrects the apparent azimuth and dip angles in a
-        Structure log
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-            [ApplyStructureApparentToTrueCorrection]
-            AzimuthLog = azimuth log name
-            TiltLog = tilt log name
-            ReferenceIsNorth = yes / no
-
-        Returns
-        -------
-        Log
-            The corrected log.
-        """
-        return Log(self._dispatch.ApplyStructureApparentToTrueCorrection(log, prompt_user, config))
-
-    def apply_structure_true_to_apparent_correction(self, log=None, prompt_user=None, config=None):
-        """Recalculates the apparent azimuth and dip angles in a
-        Structure log from the true structure angles.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ApplyStructureApparentToTrueCorrection]
-                AzimuthLog = azimuth log name
-                TiltLog = tilt log name
-                ReferenceIsNorth = yes / no
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-        return Log(self._dispatch.ApplyStructureTrueToApparentCorrection(log, prompt_user, config))
-
-    def recalculate_structure_azimuth(self, log=None, prompt_user=None, config=None):
-        """Adds or subtracts a value from all Azimuth data within a
-        structure log.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RecalculateStructureAzimuth]
-                Angle = 45 / Log
-                RotateClockwise = yes / no
-                MaxDepthRange = yes / no
-                TopDepth = 0.0
-                BottomDepth = 1.0
-
-        """
-        self._dispatch.RecalculateStructureAzimuth(log, prompt_user, config)
-
-    def recalculate_structure_dip(self, log=None, prompt_user=None, config=None):
-        """Correct the dip angle data within a structure log for new
-        caliper settings.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RecalculateStructureDip]
-                Caliper = Log / 200.0
-                CaliperUnit = mm / in
-                MaxDepthRange = yes / no
-                TopDepth = 0
-                BottomDepth = 1
-
-        """
-        self._dispatch.RecalculateStructureDip(log, prompt_user, config)
-
-    def remove_structural_dip(self, log=None, prompt_user=None, config=None):
-        """Removes a given regional dip and azimuth from the data in
-        a structure log and recalculates new Dip and Azimuth angles.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RemoveStructuralDip]
-                Azimuth = Log /45
-                Dip = Log /10
-                MaxDepthRange = yes / no
-                TopDepth = 0.0
-                BottomDepth = 1.0
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-        return Log(self._dispatch.RemoveStructuralDip(log, prompt_user, config))
-
-    def extract_color_components(self, log=None, method=None, color_model=None, prompt_user=None):
-        """Allows the extraction of color data from an RGB Log.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        method : int, optional
-            The methode used.
-            Available models are:
-
-            * 0 = Average
-            * 1 = Mode
-            * 2 = Image Log
-        color_model : int, optional
-            The color model used.
-            Available models are:
-
-            * 0 = RGB
-            * 1 = HSV
-            * 2 = YUV
-            * 3 = CIELAB
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        """
-        self._dispatch.ExtractColorComponents(log, method, color_model, prompt_user)
-
-    def color_classification(self, log=None, prompt_user=None, config=None):
-        """Builds color classes from an RGB Log based on user
-        specified reference colors.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the RGB log to process.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ColorClassification]
-                OutputImage = yes
-                OutputAnalysis = yes
-                NoiseReduction = 10
-                Class1="Class 1";"0,255,0";58;50;"166,143,81"
-                Class2="Class 2";"255,0,255";37;50;"44,42,34"
-                Class3="Class 3";"255,255,0";34;50;"251,165,75"
-
-        Returns
-        -------
-        Log
-            Returns an RGB Log or an Analysis Log depending on the configuration file.
-            Returns the RGB Log if both options are selected.
-        """
-        return Log(self._dispatch.ColorClassification(log, prompt_user, config))
-
-    def adjust_image_brightness_and_contrast(self, log=None, prompt_user=None):
-        """Adjusts the brightness and contrast in RGB logs
-
-        Parameters
-        ----------
-        log : str or int, optional
-            A string specifying the log name or an integer
-            representing the index of the log to be processed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to False, the new brightness and
-            contrast values will be determined automatically.
-        """
-        self._dispatch.AdjustImageBrightnessAndContrast(log, prompt_user)
-
-    def retinex_filter_rgb_log(self, log=None, prompt_user=None, config=None):
-        """Applies a retinex filter to the RGB log.
-
-        Note: only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Not Used for this function.
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-
-        return Log(self._dispatch.RetinexFilterRGBLog(log, prompt_user, config))
-
-    def sharpen_rgb_log(self, log=None, prompt_user=None, config=None):
-        """Sharpens the RGB log.
-
-        Note: only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Not Used for this function.
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-
-        return Log(self._dispatch.SharpenRGBLog(log, prompt_user, config))
-
-    def extract_structure_interval_statistic(self, log=None, prompt_user=None, config=None):
-        """Allows determination of statistical values (e.g. frequency
-        of dips) per interval from a structure log.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ExtractStructureIntervalStatistic]
-                Reference = 5.0 / Log
-                OutputMinAzimuth = yes / no
-                OutputMaxAzimuth = yes / no
-                OutputAverageAzimuth = yes / no
-                OutputMinDip = yes / no
-                OutputMaxDip = yes / no
-                OutputAverageDip = yes / no
-                OutputMinTilt = yes / no
-                OutputMaxTilt = yes / no
-                OutputAverageTilt = yes / no
-                OutputMinAperture = yes / no
-                OutputMaxAperture = yes / no
-                OutputAverageAperture = yes / no
-                OutputMinLength = yes / no
-                OutputMaxLength = yes / no
-                OutputAverageLength = yes / no
-                OutputMinOpening = yes / no
-                OutputMaxOpening = yes / no
-
-        Returns
-        -------
-        Log
-            One of the computed log.
-        """
-        return Log(self._dispatch.ExtractStructureIntervalStatistic(log, prompt_user, config))
-
-    def rqd(self, log=None, prompt_user=None, config=None):
-        """Computes the Rock Quality Designation from the structure
-        picks in a Structure Log.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RQD]
-                CorePieceLength = 0.1
-                CoreLength = 1
-                AttributeName1 = Defect Type
-                AttributeValues1 = JT-MAJ, JT-MED, JT-MIN,
-                AttributeName2 = Defect Condition
-                AttributeValues2 = cont, part
-                DepthRange = Maximum / UserDefined / Zones
-                'UserDefined
-                TopDepth=25
-                BottomDepth=30
-                'Zones
-                ZonesDepthRange = 20,26, 24,30
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-        return Log(self._dispatch.RQD(log, prompt_user, config))
-
-    def representative_picks(self, log=None, prompt_user=None, config=None):
-        """Used to derive the most representative picks from a
-        Structure log given user defined classification limits.
-
-        Parameters
-        ----------
-        log : str or int, optional
-            Zero based index (integer) or title (string) of
-            the log to process. If not provided, a dialog box
-            displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with
-            the user. If set to  ``False`` the processing parameters
-            will be retrieved from the specified configuration
-            file. If no configuration file has been specified,
-            default values will be used.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RepresentativePicks]
-                TopDepth=0.0
-                BottomDepth=10.0
-                TiltWindow=5.0 (structural dip angle interval, here +/- 5 degrees)
-                AzimuthWindow=15.0 (structural azimuth angle interval, here +/- 15 degrees)
-                DepthWindow=0.5
-                KeepFeaturesUngrouped=TRUE / FALSE
-
-        Returns
-        -------
-        Log
-            The computed log.
-        """
-        return Log(self._dispatch.RepresentativePicks(log, prompt_user, config))
-
-    def correct_dead_sensor(self, log=None, prompt_user=None, config=None):
-        """Corrects the Null and invalid data columns in Image logs.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [DeadSensor]
-                ; Method : Automatic, Range, Columns
-                ; ReplaceBy : Null, Average, Median, Interpolate, LogName or a numerical value
-                Method = Automatic
-                ReplaceBy = Average
-                ; If Method = Automatic
-                WindowHeight = 0
-                Discrimination = 0.125
-                MinDataHeight = 0
-                ; If Method = Range
-                WindowHeight = 0
-                Low = 0
-                High = 0
-                ; If Method = Columns
-                ; Columns : single index value or range like 15-20
-                Columns = 1
-        Returns
-        -------
-        Log
-            A log with the corrected data.
-        """
-        return Log(self._dispatch.CorrectDeadSensor(log, prompt_user, config))
-
-    def shift_correction(self, log=None, prompt_user=None, config=None):
-        """Corrects the drift of data (e.g. MFC) in Image logs.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ShiftCorrection]
-                ; Zone1 : name, top, bottom, value
-                OutputCorrections = yes / no
-                ExtendTrends = yes / no
-                Zone1=ref1, 25.0, 26.0, 101.2
-                Zone2=ref2, 45.0, 47.0, 125.3
-
-        Returns
-        -------
-        Log
-            A log that has been corrected.
-        """
-        return Log(self._dispatch.ShiftCorrection(log, prompt_user, config))
-
-    def calculate_fluid_velocity(self, log=None, prompt_user=None, config=None):
-        """Estimates the fluid velocity from travel time measurements and given calibration points.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CalculateFluidVelocity]
-                ; If the AutoFill option is used the CalibrationPoints are not used.
-                ; ToolRadius : in mmm
-                ; TimeWindow : log name or value
-                ; CalibrationPoint1 : depth, diameter in mm
-                ; AutoFillFrom : depth value or 'Top'
-                 ; AutoFillTo : depth value or 'Bottom'
-                TravelTimeUnit = 0.1
-                ToolRadius = 19
-                TimeWindow = TimeWndLog / 74
-                CalibrationPoint1 = 20.44, 96
-                CalibrationPoint2 = 36.85, 96
-                CalibrationPoint3 = ...
-                ExtendTrends = yes / no
-                AutoFillFrom = 0 / Top
-                AutoFillTo = 0 / Bottom
-                AutoFillCaliper = 0 / Log Name
-                AutoFillStepSize = 1.0
-
-        Returns
-        -------
-        Log
-            A log giving the fluid velocity.
-        """
-        return Log(self._dispatch.CalculateFluidVelocity(log, prompt_user, config))
-
-    def centralize(self, log=None, prompt_user=None, config=None):
-        """Corrects travel time or multi-finger-caliper data for de-centralization effects
-        and outputs a new image log.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [Centralize]
-                ; UseRange : use clipping range
-                UseRange = yes / no
-                CaliperLow = 0
-                CaliperHigh = 0
-                OutputEccentricity = yes / no
-                OutputEccentricityDir = yes / no
-
-        Returns
-        -------
-        Log
-            A log with the data corrected for decentralization.
-        """
-        return Log(self._dispatch.Centralize(log, prompt_user, config))
-
-    def calculate_acoustic_caliper(self, log=None, prompt_user=None, config=None):
-        """Calculates borehole radius and caliper values from acoustic travel time measurements.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CalculateAcousticCaliper]
-                ; CaliperUnit : mm, cm, in
-                ; FluidVelocityUnit : m/s, km/s, m/ms, m/us, ft/s, ft/ms, ft/us, s/km, s/m, us/m, s/ft, us/ft
-                ; ToolRadius : in mm
-                TravelTimeUnit = 0.1
-                CaliperUnit = mm
-                ToolRadius = 19
-                TimeWindow = TimeWndLog / 74
-                FluidVelocity = VelocityLog / 1440
-                FluidVelocityUnit= m/s
-                CurveOutput = yes / no
-                ImageOutput  = yes / no
-        """
-        self._dispatch.CalculateAcousticCaliper(log, prompt_user, config)
-
-    def calculate_casing_thickness(self, log=None, prompt_user=None, config=None):
-        """Calculates thickness values for a casing pipe from acoustic thickness travel time measurements.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CalculateCasingThickness]
-                ; ThicknessUnit : mm, cm, in
-                ; SteelVelocityUnit : m/s, km/s, m/ms, m/us, ft/s, ft/ms, ft/us, s/km, s/m, us/m, s/ft, us/ft
-                ; CurveOutput : output min, max, average thickness
-                ; ImageOutput  : output the thickness as an image log
-                TravelTimeUnit = 0.01
-                SteelVelocity = VelocityLog / 5200
-                SteelVelocityUnit= m/s
-                CurveOutput = yes / no
-                ImageOutput = yes / no
-        """
-        self._dispatch.CalculateCasingThickness(log, prompt_user, config)
-
-    def cased_hole_ultrasonics(self, wavelet_log=None, zone_log=None, prompt_user=None, config=None):
-        """Processes ultrasonic waveforms from a wavelet log using the processing parameters from a zone log.
-
-        Parameters
-        ----------
-        wavelet_log : int or str, optional
-            Zero based index or title of the wavelet log to process.
-            If not provided, the process dialog box will be displayed.
-        zone_log : int or str, optional
-            Zero based index or title of the zone log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CasedHoleUltrasonics]
-                ; Thickness : output the thickness as an image log
-                ; Cadi  : output the cadi as an image log
-                ; Score  : output the score as an image log
-                Thickness = yes / no
-                Cadi = yes / no
-                Score = yes / no
-        """
-        self._dispatch.CasedHoleUltrasonics(wavelet_log, zone_log, prompt_user, config)
-
-    def calculate_apparent_metal_loss(self, log=None, prompt_user=None, config=None):
-        """Calculates an apparent metal loss value for each trace of radius values stored in an image log.
-
-        Note: This function is deprecated in WellCAD 5.7 and onwards. Please use calculate_apparent_metal_loss_ex instead.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CalculateApparentMetalLoss]
-                ; The units of the internal / external pipe radius values must be the same as the unit
-                ; of the radius values in the image log.
-                InternalPipeRadius = 1.9
-                ExternalPipeRadius = 2.2
-        Returns
-        -------
-        Log
-            A log giving the metal loss.
-        """
-        return Log(self._dispatch.CalculateApparentMetalLoss(log, prompt_user, config))
-
-    def calculate_apparent_metal_loss_ex(self, log=None, prompt_user=None, config=None):
-        """Calculates an apparent metal loss value for each trace of radius/thickness values stored in an
-        image log or well log.
-
-        Note: only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, either here or in the config, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [MetalLoss]
-                ; ID : name of a well log or img log
-                ; Thickness : name of a well log or img log
-                ; NomOD : name of a well log or value
-                ; NomThickness : name of a well log or value
-                ; NomODUnit, NomThicknessUnit : inch or mm, default to mm
-                ; DepthRange : Maximum, UserDefined, Zones, LogZones
-                ; ZonesDepthRange : top1, bot1, top2, bot2, ... topN, botN
-                ; LogZonesDepthRange = logname, depthsectionName1, depthsectionName2, ....depthsectionname3
-                ID=
-                Thickness=
-                NomOD=50
-                NomODUnit=mm
-                NomThickness=10
-                NomThicknessUnit=mm
-                DepthRange=Maximum
-                TopDepth = 10
-                BottomDepth = 19
-                ZonesDepthRange=
-                LogZonesDepthRange = Litho,06,05#1
-        """
-        self._dispatch.CalculateApparentMetalLossEx(log, prompt_user, config)
-
-    def radius_to_from_diameter(self, log=None, prompt_user=None, config=None):
-        """Converts values data in an Image log from radius to diameter values or vice versa.
-
-        Parameters
-        ----------
-        log : int or str
-            Zero based index or title of the log to process.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RadiusToFromDiameter]
-                ;  Method : TwoTimesRadius, OppositeValues, HalfDiameter
-                Method = TwoTimesRadius
-        Returns
-        -------
-        Log
-            A log giving diameter/radius.
-        """
-        return Log(self._dispatch.RadiusToFromDiameter(log, prompt_user, config))
-
-    def outer_inner_radius_diameter(self, log=None, prompt_user=None, config=None):
-        """The process takes an Image, Well or Mud log as input and computes from radius/diameter
-        and thickness values an outer radius/diameter value.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [OuterInnerRadiusDiameter]
-                ; InputType : InnerRadius, OuterRadius, InnerDiameter, OuterDiameter
-                ; OutputType : InnerRadius, OuterRadius, InnerDiameter, OuterDiameter
-                ; Thickness = log name or value
-                Thickness = THK
-                InputType = InnerRadius
-                OutputType = OuterDiameter
-        Returns
-        -------
-        Log
-            A log giving the outer radius/diameter.
-        """
-        return Log(self._dispatch.OuterInnerRadiusDiameter(log, prompt_user, config))
-
-    def cased_hole_normalization(self, log=None, prompt_user=None, config=None):
-        """Subtracts the trace average, median, min, max or a custom value from all data points
-        of the same trace.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns ''None''.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CasedHoleNormalization]
-                ; Method : Mean, Median, Min, Max, Other
-                ; The Value parameter is used when the Method has been set to Other
-                ; Value : log name or constant numerical value
-                Method = Mean
-                Value = 10.5
-
-        Returns
-        -------
-        Log
-            The resulting log.
-        """
-        return Log(self._dispatch.CasedHoleNormalization(log, prompt_user, config))
-
-    def reverse_amplitude(self, log=None):
-        """Inverts the amplitudes in a FWS log.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, a dialog box displaying a list of available logs will be displayed.
-        """
-
-        self._dispatch.ReverseAmplitude(log)
-
-    def average_filter_fws_log(self, log=None, filter_width=None, filter_type=None):
-        """Applies a moving average filter to the traces of an FWS log.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.  If not provided, the process returns None.
-        filter_width : float, optional
-            Length of the filter window in us.  If not provided, default value will be used.
-        filter_type : int, optional
-            If not provided, default value will be used.
-            Type of the filter :
-
-                * 0 = moving average
-                * 1 = weighted average
-
-        Returns
-        -------
-        Log
-            The resulting log.
-        """
-
-        return Log(self._dispatch.AverageFilterFWSLog(log, filter_width, filter_type))
-
-    def freq_filter_fws_log(self, log, low_cut, low_pass, high_pass, high_cut):
-        """Applies a frequency filter to the traces of an FWS log.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.  If not provided, the process returns None.
-        low_cut : float
-            The low cut-off frequency of filter in kHz. If not provided, default value will be used.
-        low_pass : float
-            The low pass frequency of filter in kHz. If not provided, default value will be used.
-        high_pass : float
-            The high pass frequency of filter in kHz. If not provided, default value will be used.
-        high_cut : float
-            The high cut-off frequency of filter in kHz. If not provided, default value will be used.
-
-        Returns
-        -------
-        Log
-            Object of the filtered FWS log.
-        """
-
-        return Log(self._dispatch.FreqFilterFwsLog(log, low_cut, low_pass, high_pass, high_cut))
-
-    def apply_stand_off_correction(self, log=None, prompt_user=None, config=None):
-        """Corrects intercept times for the stand-off of tool and formation.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog settings will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ApplyStandOffCorrection]
-                ; LogUnit : s, ms, msec, us, usec, sec
-                ; ToolSpacingUnit, ToolDiameterUnit, HoleDiameterUnit : m, mm, inch, cm, ft
-                ; FluidVelocityUnit : us/ft, us/m, ft/us, m/s
-                ; VelocityUnit : us/ft, us/m, ft/us, m/s
-                ; HoleDiameter, FluidVelocity : log name or constant
-                LogUnit=us
-                ToolSpacing=0.6
-                ToolSpacingUnit=m ; m, mm, inch, cm, ft
-                ToolDiameter=50
-                ToolDiameterUnit=mm
-                HoleDiameter=100
-                HoleDiameterUnit=mm
-                FluidVelocity=1500
-                FluidVelocityUnit=m/s
-                VelocityUnit=m/s
-
-        Returns
-        -------
-        Log
-            The resulting log.
-        """
-
-        return Log(self._dispatch.ApplyStandOffCorrection(log, prompt_user, config))
-
-    def compensated_velocity(self, log=None, prompt_user=None, config=None):
-        """Slowness or velocity computed from two receiver arrival times.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log containing the travel times to the first receiver.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [FwsCompensatedVelocity]
-                ; RX1Log, RX2Log : log name
-                ; RX1LogUnit, RX2LogUnit : s, ms, msec, us, usec, sec
-                ; SpacingUnit : m, mm, inch, ft, cm
-                ; VelocityUnit : us/ft, us/m, ft/us, m/s
-                RX1Log =RX1 - dt
-                RX2Log = RX2 - dt
-                RX1LogUnit = us
-                RX2LogUnit = us
-                Spacing = 0.2
-                SpacingUnit = m
-                VelocityUnit =us/m
-
-        Returns
-        -------
-        Log
-            The resulting log.
-        """
-
-        return Log(self._dispatch.CompensatedVelocity(log, prompt_user, config))
-
-    def apply_semblance_processing(self, prompt_user=None, config=None):
-        """Performs a velocity analysis for the multiple receivers.
-
-        Parameters
-        ----------
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file.
-            The configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ApplySemblanceProcessing]
-                Rx1_Log = RX1
-                Rx1_Offset = 0.0
-                Rx1_TxDistance = 0.6
-                Rx1_Unit = m
-                Rx2_Log = RX2
-                Rx2_Offset = 0.0
-                Rx2_TxDistance = 0.8
-                Rx2_Unit = m
-                Rx3_Log= ...
-
-                [FwsVelocityAnalysis]
-                EnableFilter=false
-                FreqFilterLowPass=2.5 ; in kHz
-                FreqFilterLowPass=5.0
-                FreqFilterHighPass=30.0
-                FreqFilterHighCut=35.0
-                ToolDiameter=50.0
-                ToolDiameterUnit=mm ;mm, cm, inch
-                BoreholeDiameter=100.0
-                BoreholeDiameterUnit=mm ;mm, cm, inch
-                FluidSlowness=666.67
-                FluidSlownessUnit=us/m ; us/ft, us/m, ft/us, m/s, us/m
-
-        Returns
-        -------
-        Log
-            The log containing the semblance results.
-        """
-
-        return Log(self._dispatch.ApplySemblanceProcessing(prompt_user, config))
-
-    def process_reflected_tube_wave(self, log=None, prompt_user=None, config=None):
-        """Extracts the cumulative energy from reflected tube wave arrivals.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog settings will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ProcessReflectedTubeWave]
-                ; Side : both,  upper, lower
-                Side = both
-                Offset = 25.0 'measured in us
-                Blanking = 50.0 'measured in us
-                FluidSlowness = 696.0 'measured in us/m
-                TxFrequency = 15000.0 'measured in Hz
-
-        Returns
-        -------
-        Log
-            The resulting log containing the cumulative energy.
-        """
-
-        return Log(self._dispatch.ProcessReflectedTubeWave(log, prompt_user, config))
-
-    def pick_first_arrival(self, log=None, prompt_user=None, config=None):
-        """Picks the first arrival time using the standard threshold or advanced method.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.  If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file.
-            The configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [FwsFirstArrival]
-                ;Method=Standard Threshold Pickup Algorithm
-                Method=Advanced Threshold Pickup Algorithm
-
-                [Standard Threshold Pickup Algorithm]
-                Blanking=100.0
-                Threshold=15.0
-                BackInterpolation=yes
-                LockToSampling=yes
-                ; the next two are advanced settings
-                BaseLine=0.0
-                AutoAdjustThreshold=no
-
-                [Advanced Threshold Pickup Algorithm]
-                Blanking=0.0
-                Threshold=3.0
-                LargeWidth=120.0
-                SmallWidth=40.0
-
-        Returns
-        -------
-        Log
-            The resulting log containing the first arrival times.
-        """
-
-        return Log(self._dispatch.PickFirstArrival(log, prompt_user, config))
-
-    def cement_bond(self, log=None, prompt_user=None, config=None):
-        """Determines the cement bond based on the Standard Gate Method.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [CementBondProcess]
-                ; Logs : comma-separated FWS log names of the receivers to be processed
-                Logs=WVFS1,WVFS2,WVFS3
-                AreRadiiSectors=no
-                EnableT0Gate=yes
-                EnableTXGate=no
-                T0GateStart=237.4
-                T0GateLength=40
-                TXGateBlanking=0
-                TXGateThreshold=15
-                EnableCalibration=no
-                BLGateStart=50
-                BLGateLength=25
-                FreePipeTargetAmplitude=100
-                FreePipeTargetAmplitudeUnits=mV
-                FreePipeTopDepth=0
-                FreePipeBotDepth=0
-        """
-
-        self._dispatch.CementBond(log, prompt_user, config)
-
-    def pick_e1_arrival(self, fws_log=None, dt_log=None, prompt_user=None, config=None):
-        """Determines the arrival time of the E1 amplitude.
-
-        Parameters
-        ----------
-        fws_log : int or str, optional
-            Zero based index or title of the FWS log to process.
-            If not provided, the process dialog box will be displayed.
-        dt_log : int or str, optional
-            Zero based index or title of the arrival time log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [PickE1Arrival]
-                PickPositivPolarity = yes
-                FilterWidth = 5
-
-        Returns
-        -------
-        Log
-            The resulting log containing the E1 arrival times.
-        """
-
-        return Log(self._dispatch.PickE1Arrival(fws_log, dt_log, prompt_user, config))
-
-    def extract_e1_amplitude(self, fws_log=None, arrival_log=None, prompt_user=None):
-        """Uses the E1 arrival time to extract the E1 amplitude.
-
-        Parameters
-        ----------
-        fws_log : int or str, optional
-            Zero based index or title of the log to process.
-        arrival_log : int, str or float, optional
-            int, str : Zero based index or title of the log containing the first E1 arrival times.
-            float : constant E1 arrival time
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-
-        Returns
-        -------
-        Log
-            The resulting log containing the E1 amplitude.
-        """
-
-        return Log(self._dispatch.ExtractE1Amplitude(fws_log, arrival_log, prompt_user))
-
-    def adjust_pick_to_extremum(self, fws_log=None, arrival_log=None, prompt_user=None, config=None):
-        """Adjusts the pick given in arrival_log to the next maximum or minimum amplitude in fws_log.
-
-        Parameters
-        ----------
-        fws_log : int or str, optional
-            Zero based index or title of the fws log.
-            If not provided, the process dialog box will be displayed.
-        arrival_log : int or str, optional
-            Zero based index or title of the arrival time log.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [AdjustPickToExtremum]
-                PickPositivPolarity = yes
-                FilterWidth = 5
-
-        Returns
-        -------
-        Log
-            Object of the log containing the pick times shifted to the nearest amplitude extremum.
-        """
-
-        return Log(self._dispatch.AdjustPickToExtremum(fws_log, arrival_log, prompt_user, config))
-
-    def extract_window_peak_amplitude(self, log=None, prompt_user=None, config=None):
-        """Extracts the maximum amplitude found in a time window of a FWS log trace.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [ExtractWindowPeakAmplitude]
-                ; WindowStart : value or log name, units : us
-                ; WindowLength : value, units : us
-                ; PickType : 0 = peak, 1 = max, 2 = average
-                WindowStart=0
-                WindowLength=15
-                PickMax=yes
-                PickPos=yes
-                PickType=1
-                EnableResampling=yes
-
-        Returns
-        -------
-        Log
-            The resulting log containing the amplitude.
-        """
-
-        return Log(self._dispatch.ExtractWindowPeakAmplitude(log, prompt_user, config))
-
-    def calculate_mechanical_properties(self, p_slowness=None, s_slowness=None, density=None):
-        """Computes a set of rock mechanical parameters from the input data.
-
-        Parameters
-        ----------
-        p_slowness : int or str, optional
-            Zero based index or title of the log containing the p-slowness data.
-            If not provided, the process dialog box will be displayed.
-        s_slowness : int or str, optional
-            Zero based index or title of the log containing the s-slowness data.
-            If not provided, the process dialog box will be displayed.
-        density :int or str, optional
-            Zero based index or title of the log containing the density data.
-        """
-
-        self._dispatch.CalculateMechanicalProperties(p_slowness, s_slowness, density)
-
-    def integrated_travel_time(self, log=None, prompt_user=None, config=None):
-        """Computes the integrated travel time from slowness or velocity data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [IntegratedTravelTime]
-                TimeOffset = 0 'in us
-                TWT = Yes/No
-
-        Returns
-        -------
-        Log
-            The resulting log containing the integrated times.
-        """
-
-        return Log(self._dispatch.IntegratedTravelTime(log, prompt_user, config))
-
-    def bond_index(self, log=None, prompt_user=None, config=None):
-        """Computes the bond index of the cement behind the casing.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [FwsBondIndex]
-                CementAmplitude = 2 'in mV
-                FreePipeAmplitude = 62.2 'in mV
-
-        Returns
-        -------
-        Log
-            The resulting log containing the bond index.
-        """
-
-        return Log(self._dispatch.BondIndex(log, prompt_user, config))
-
-    def compressive_strength(self, log=None, prompt_user=None, config=None):
-        """Computes the compressive strength of the cement behind a casing.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.  A cement bond amplitude log (Well or Mud log type)
-            or amplitude map (Image log) can be used.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [FwsCompressiveStrength]
-                CasingOD = 7 ' in inch
-                CasingWeight = 23 ' in lbs/ft
-
-        Returns
-        -------
-        Log
-            The resulting log containing the compressive strength.
-        """
-
-        return Log(self._dispatch.CompressiveStrength(log, prompt_user, config))
-
-    def apply_natural_gamma_borehole_correction(self, log=None, prompt_user=None, config=None):
-        """Applies borehole corrections to FWS and Well logs
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [BoreholeConditionCorrections]
-                DeadTime = 7.2 ' in us
-                EnableDeadTime = yes
-                EnableFactors = yes
-                FactorName1 = Water Factor
-                FactorName2 = Pipe Factor
-                Top1 = 0.0
-                Bot1 = 2.85
-                Factor1-1 = 1
-                Factor1-2 = 1.49
-                Top2 = 2.85
-                Bot2 = bot
-                Factor2-1 = 1.12
-                Factor2-2 = 1
-
-        Returns
-        -------
-        Log
-            A log containing the corrected count rates.
-        """
-
-        return Log(self._dispatch.ApplyNaturalGammaBoreholeCorrection(log, prompt_user, config))
-
-    def apply_total_gamma_calibration(self, log=None, prompt_user=None, config=None):
-        """Applies a calibration factor or equation to the values in the specified Well Log.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [BoreholeConditionCorrections]
-                K-Factor=2*0.00001028
-
-        Returns
-        -------
-        Log
-            A log containing the modified gamma values.
-        """
-
-        return Log(self._dispatch.ApplyTotalGammaCalibration(log, prompt_user, config))
-
-    def calculate_spectrum_total_count(self, log=None, prompt_user=None, config=None):
-        """Extracts the total count, min, max, average or median from each spectrum trace of the specified log
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [SpectralGamma_Statistic]
-                ; WinLow, WinHigh expressed in channel number or keV according to Channel
-                Total = yes
-                Min = yes
-                Max = yes
-                Ave = yes
-                Median = yes
-                UseWindow = yes
-                Channel = yes
-                WinLow = 410
-                WinHigh = 2850
-        """
-
-        self._dispatch.CalculateSpectrumTotalCount(log, prompt_user, config)
-
-    def spectrometric_ratios(self, log_a=None, log_b=None, log_c=None, prompt_user=None, config=None):
-        """Computes spectrometric ratios like U/Th or U/k
-
-        By default, the ratios log_b/log_a, log_b/log_c and log_c/log_a
-        will be computed.
-
-        Parameters
-        ----------
-        log_a : int or str, optional
-            Zero based index or title of the log to process.
-        log_b : int or str, optional
-            Zero based index or title of the log to process.
-        log_c : int or str, optional
-            Zero based index or title of the log to process.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [SpectrometricRatios]
-                ; ratio : A / B
-                A=K
-                B=U
-        """
-
-        self._dispatch.SpectrometricRatios(log_a, log_b, log_c, prompt_user, config)
-
-    def process_medusa_spectrum_data(self, log_spectrum=None, log_time=None, prompt_user=None, config=None):
-        """Performs a full spectrum analysis using a calibration after Medusa
-
-        Parameters
-        ----------
-        log_spectrum : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        log_time : int or str, optional
-            Zero based index or title of the log with the live time data.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [SpectralGammaMedusaProcess]
-                CalibrationFilePath = C:\\Temp\\NSG1234.mcf
-                EnableFittedSpectrum = yes
-                EnableConcentrationErrors = yes
-                EnableStabilizationFactor = yes
-                DeadTime = 5 (in us/pulse)
-                HoleDiameter = 96 / Caliper (fixed value or data from log in mm)
-                CasingThickness = 8 / Thickness (fixed value or data from log mm)
-                CasingType = 0 (Steel) / 1 (PVC)
-                FluidDensity = 1.1 / RHOFL (fixed value or data from log in g/ccm)
-                FluidK = 0.0 / K (Potassium concentration in the fluid; fixed value or data from log in Bq/kg)
-                FluidU = 0.0 / U (eq Uranium concentration in the fluid; fixed value or data from log in Bq/kg)
-                FluidTh = 0.0 / Th (Thorium concentration in the fluid; fixed value or data from log in Bq/kg)
-                ToolPosition = 0 (Alongside) / 1 (Centered)
-                """
-        self._dispatch.ProcessMedusaSpectrumData(log_spectrum, log_time, prompt_user, config)
-
-    def process_spectrum_data(self, log=None, prompt_user=None, config=None):
-        """Performs a windows stripping based on a calibration model
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [SpectralGamma]
-                OutputWindowCounts = yes / no
-                ProcessModel = "C:\Temp\Test.sgm"
-        """
-
-        self._dispatch.ProcessSpectrumData(log, prompt_user, config)
-
-    def compute_gr(self, log_k=None, log_u=None, log_th=None, prompt_user=None, config=None):
-        """Computes total gamma ray from K, U and Th isotope concentrations using the MEDUSA
-        calibration file.
-
-        Parameters
-        ----------
-        log_k : int or str, optional
-            Zero based index or title of the log containing the concentrations of K.
-        log_u : int or str, optional
-            Zero based index or title of the log containing the concentrations of U.
-        log_th : int or str, optional
-            Zero based index or title of the log containing the concentrations of Th.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [SpectralGammaMedusaCGR]
-                CalibrationFilePath=C:\Tools\Calibrations\QL40-SGR-154904.mcf
-
-        Returns
-        -------
-        Log
-            A log containing the gamma ray values.
-        """
-
-        return Log(self._dispatch.ComputeGR(log_k, log_u, log_th, prompt_user, config))
-
-    def process_nmrsa_data(self, log=None, prompt_user=None, config=None):
-        """Performs a post-processing of NMRSA's BMR tool raw data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path and name of the configuration file or a parameter string.  The configuration file or
-            string can contain the following options:
-
-            .. code-block:: ini
-
-                [NMRSA]
-                UseDefaultOutputs = yes / no
-                MasterCalibrationFile=
-                ProcessingConfigurationFile=
-                DepthRange=Maximum / UserDefined / Zones /LogZones
-                TopDepth=20
-                BottomDepth=22
-                LogZones : top1, bot1, top2, bot2, ... topN, botN
-                LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
-        """
-
-        self._dispatch.ProcessNMRSAData(log, prompt_user, config)
-
-    def nmr_total_porosity(self, log=None, prompt_user=None, config=None):
-        """Computes the total porosity from a T2 distribution.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path and name of the configuration file or a parameter string.  The configuration file
-            or string can contain the following options:
-
-            .. code-block:: ini
-
-                [NMRTotalPorosity]
-                MaxCutoffValue=-1
-                UseTimeMaxCutoff= yes / no
-
-                DepthRange=Maximum / UserDefined / Zones /LogZones
-                TopDepth=20
-                BottomDepth=22
-                LogZones : top1, bot1, top2, bot2, ... topN, botN
-                LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
-
-        Returns
-        -------
-        Log
-            The resulting log object
-        """
-
-        return Log(self._dispatch.NMRTotalPorosity(log, prompt_user, config))
-
-    def nmr_permeability(self, log=None, prompt_user=None, config=None):
-        """Computes the permeability from a T2 distribution.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path and name of the configuration file or a parameter string.  The configuration file
-            or string can contain the following options:
-
-            .. code-block:: ini
-
-            [NMRPermeability]
-            T2DistributionTraceUnit= seconds / milliseconds
-            UseTimeMaxCutoff= yes / no
-            MaxCutoffValue=-1
-            DisplayTIMModel= yes / no
-            VariableCforTIMModel=1
-            ExponentMforTIMModel=4
-            BFVCutoffForTIMModel=2
-            BFVCutoffForTIMModel=0.3
-            UseTimeMaxForFFVCutoff= yes / no
-            FFVCutoffForTIMModel=0
-            DisplaySDRModel= yes / no
-            VariableCforSDRModel=4
-            ExponentMforSDRModel=4
-            ExponentNforSDRModel=2
-            DisplayT2LogMean= yes / no
-            DepthRange=Maximum / UserDefined / Zones /LogZones
-            TopDepth=20
-            BottomDepth=22
-            LogZones : top1, bot1, top2, bot2, ... topN, botN
-            LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
-        """
-
-        self._dispatch.NMRPermeability(log, prompt_user, config)
-
-    def nmr_fluid_volumes(self, log=None, prompt_user=None, config=None):
-        """Computes the fluid volumes from a T2 distribution.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log to process.
-            If not provided, the process dialog box will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path and name of the configuration file or a parameter string.  The configuration file
-            or string can contain the following options:
-
-            .. code-block:: ini
-
-            [NMRFluidVolumes]
-            LithoDatabase=
-            UseLithoDatabaseAssociatedColor= yes/no
-            Components=
-            Cutoff=
-            DepthRange=Maximum / UserDefined / Zones /LogZones
-            TopDepth=20
-            BottomDepth=22
-            LogZones : top1, bot1, top2, bot2, ... topN, botN
-            LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
-
-        Returns
-        -------
-        Log
-            The resulting log object
-        """
-
-        return Log(self._dispatch.NMRFluidVolumes(log, prompt_user, config))
-
-    def water_salinity(self, log=None, prompt_user=None, config=None):
-        """Salinity estimation from fluid conductivity.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the fluid conductivity log to process.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [WaterSalinity]
-                Temperature = log name or constant value
-                TemperatureUnit = degC / degF / degK
-
-        Returns
-        -------
-        Log
-            A log of the resulting salinity.
-        """
-
-        return Log(self._dispatch.WaterSalinity(log, prompt_user, config))
-
-    def water_resistivity(self, log=None, prompt_user=None, config=None):
-        """Temperature correction for fluid conductivity or resistivity.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log containing the conductivity or resistivity values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-             .. code-block:: ini
-
-                [WaterResistivity]
-                Temperature = log name or constant value
-                TemperatureUnit = degC / degF / degK
-                RefTemperature = log name or constant value
-                RefTemperatureUnit = degC / degF / degK
-                Method = 0 (Arp) / 1 (Hilchie)
-
-        Returns
-        -------
-        Log
-            A log of the corrected conductivity or resistivity.
-        """
-
-        return Log(self._dispatch.WaterResistivity(log, prompt_user, config))
-
-    def shale_volume(self, log=None, prompt_user=None, config=None):
-        """Estimates the shale volume from Gamma Ray or SP data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the well or mud log containing the Gamma Ray or SP values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-             .. code-block:: ini
-
-                [ShaleVolume]
-                Equation = 0
-                ; 0 = Linear (default), 1 = Larionov (Tertiary), 2 = Steiber,
-                ; 3 = Clavier, 4 = Larionov (older rocks)
-                Shale=150
-                ShaleValueType=1
-                ; ...Type: 0 = value, 1 = minmax, 2 = avginterval
-                ShaleTopDepth=0
-                ShaleBotDepth=0
-                Sandstone=75
-                SandstoneValueType=1
-                ; ...Type: 0 = value, 1 = minmax, 2 = avginterval
-                SandstoneTopDepth=0
-                SandstoneBotDepth=0
-
-        Returns
-        -------
-        Log
-            A log of the resulting shale volume.
-        """
-
-        return Log(self._dispatch.ShaleVolume(log, prompt_user, config))
-
-    def porosity_sonic(self, log=None, prompt_user=None, config=None):
-        """Computes porosity from transit time data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the well or mud log containing the formation resistivity (Rt) values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [PorositySonic]
-                ; Method : 0 = Wylie, 1 = WylieCompaction, 2 = AbbreviatedRaymerHunt, 3 = RaymerHunt
-                ; Slowness units: us/ft, us/m, ft/us, m/s
-                Method = 1
-                MatrixSlowness = log name or constant value
-                MatrixSlownessUnit = us/ft
-                FluidSlowness= = log name or constant value
-                FluidSlownessUnit = us/ft
-                Compaction= = log name or constant value
-                C = 0.67
-
-        Returns
-        -------
-        Log
-            A log of the resulting porosity.
-        """
-
-        return Log(self._dispatch.PorositySonic(log, prompt_user, config))
-
-    def porosity_archie(self, log=None, prompt_user=None, config=None):
-        """Computes porosity from formation resistivity data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the well or mud log containing the formation resistivity (Rt) values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [PorosityArchie]
-                ; Method : 0 = Standard, 1 = FreshWater, 2 = shale, 3= shaleAndFreshWater
-                ; Rw and Rsh units: ohm.m, ohm.ft
-                Method = 1
-                Vsh = log name or constant value
-                Rw = log name or constant value
-                RwUnit=ohm.m
-                Rsh = 30.0
-                RshUnit=ohm.m
-                CementationFactor = 1.0
-                CementationExponent = 2.0
-                Cs = 1.0
-
-        Returns
-        -------
-        Log
-            A log of the resulting porosity.
-        """
-
-        return Log(self._dispatch.PorosityArchie(log, prompt_user, config))
-
-    def porosity_density(self, log=None, prompt_user=None, config=None):
-        """Computes porosity from density data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the well or mud log containing the  density values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [PorosityDensity]
-                ; Method : 0 = Standard, 1 = Shale
-                ; MatrixDensity, FluidDensity, ShaleVolume : value or log
-                ; Density units: g/cc or kg/m3
-                MatrixDensity=2.7
-                MatrixDensityUnit=g/cc
-                FluidDensity=1.0
-                FluidDensityUnit=g/cc
-                ShaleVolume=0
-                ShaleDensity=1.5
-                ShaleDensityUnit=g/cc
-
-        Returns
-        -------
-        Log
-            A log of the resulting porosity.
-        """
-
-        return Log(self._dispatch.PorosityDensity(log, prompt_user, config))
-
-    def porosity_neutron(self, log=None, prompt_user=None, config=None):
-        """Applies a shale correction to neutron porosity data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the well or mud log containing the neutron porosity values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [PorosityNeutron]
-                ; Vsh : log name
-                ; ShaleNPhi = value
-                Vsh=VSh
-                ShaleNPhi=50
-
-        Returns
-        -------
-        Log
-            A log of the resulting corrected porosity.
-        """
-
-        return Log(self._dispatch.PorosityNeutron(log, prompt_user, config))
-
-    def permeability(self, log=None, prompt_user=None, config=None):
-        """Estimates permeability from porosity data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the well or mud log containing the neutron porosity values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [Permeability]
-                CementationFactor=1.0
-
-        Returns
-        -------
-        Log
-            A log of the resulting permeability.
-        """
-
-        return Log(self._dispatch.Permeability(log, prompt_user, config))
-
-    def hydraulic_conductivity(self, log=None, prompt_user=None, config=None):
-        """Computes the hydraulic conductivity from permeability data.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the well or mud log containing the permeability values.
-            If not provided, the process returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [HydraulicConductivity]
-                ; Density, Viscosity, DensityTemperature, ViscosityTemperature : log name or value
-                ; Temperature units : degC, degF, degK
-                ; Permeability units : m2, Darcy, mD, sq.ft
-                ; Density units : kg/m3, g/m3, g/cc, lb/in3, lb/ft3
-                ; Viscosity units : Pa.s, cP, p, dyn.s/cm2
-                Density=1000
-                DensityUnit= kg/m3
-                Viscosity=0.000890439
-                ViscosityUnit=Pa.s
-                DensityTemperature=25
-                DensityTemperatureUnit=degC
-                ViscosityTemperature=25
-                ViscosityTemperatureUnit=degC
-
-        Returns
-        -------
-        Log
-            A Log object of the resulting hydraulic conductivity.
-        """
-
-        return Log(self._dispatch.HydraulicConductivity(log, prompt_user, config))
-
-    def extract_grain_size_statistics(self, log=None, prompt_user=None, config=None):
-        """Computes statistics from a grain size distribution curve.
-
-        Parameters
-        ----------
-        log : int or str, optional
-            Zero based index or title of the log containing the grain size values.
-            If not provided, a dialog box displaying a list of available logs will be displayed.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-             .. code-block:: ini
-
-                [GrainSizeStatistics]
-                ; Method : 0 = Logarithmic (original Folk and Ward; default),
-                ; 1 = Geometric (modified Folk and Ward),
-                ; 2 = Logarithmic method of moments,
-                ; 3= Geometric method of moments
-                Mean = yes
-                Median = yes
-                Sorting = yes
-                Skewness = yes
-                Kurtosis = yes
-                Histo = yes
-        """
-
-        self._dispatch.ExtractGrainSizeStatistics(log, prompt_user, config)
-
-    def grain_size_sorting(self, log_min, log_max, prompt_user=None, config=None):
-        """Classifies grain size values based on min and max logs.
-
-        Parameters
-        ----------
-        log_min : int or str, optional
-            Zero based index or title of the log containing logged minimum grain size value.
-            If not provided, the method returns None.
-        log_max : int or str, optional
-            Zero based index or title of the log containing logged maximum grain size value.
-            If not provided, the method returns None.
-        prompt_user : bool, optional
-            Whether dialog boxes are displayed to interact with the user.
-            If set to ``False`` the processing parameters will be retrieved from the specified
-            configuration.  If no configuration has been specified, default values will be used.
-            Default is True.
-        config : bool, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-             .. code-block:: ini
-
-                [GrainSizeSorting]
-                ; Method : 0 = Logarithmic (original Folk and Ward; default),
-                ; 1 = Geometric (modified Folk and Ward),
-                ; 2 = Logarithmic method of moments,
-                ; 3= Geometric method of moments
-                BlockedAverage = yes
-
-        Returns
-        -------
-        Log
-            A log containing the sorted values
-        """
-
-        return Log(self._dispatch.GrainSizeSorting(log_min, log_max, prompt_user, config))
-
-    def enable_protection(self, enable, password):
-        """Changes the protection status of a document using a password
-
-        Parameters
-        ----------
-        enable : bool
-            Set to True to protect the borehole document.
-        password : str
-            The password used to allow this option.
-        """
-
-        self._dispatch.EnableProtection(enable, password)
-
-    def allow_insert_log(self, enable, password):
-        """Changes the protection status for inserting new logs.
-
-        Parameters
-        ----------
-        enable : bool
-            Set to True to allow adding new logs to the borehole document.
-        password : str
-            The password used to allow this option.
-        """
-
-        self._dispatch.AllowInsertLog(enable, password)
-
-    def allow_save_template(self, enable, password):
-        """Changes the protection status for saving layout templates.
-
-        Parameters
-        ----------
-        enable : bool
-            Set to True to allow saving layout templates of the borehole document.
-        password : str
-            The password used to allow this option.
-        """
-
-        self._dispatch.AllowSaveTemplate(enable, password)
-
-    def allow_export_file(self, enable, password):
-        """Changes the protection status for exporting data.
-
-        Parameters
-        ----------
-        enable : bool
-            Set to True to allow the export of data from the borehole document.
-        password : str
-            The password used to allow this option.
-        """
-
-        self._dispatch.AllowExportFile(enable, password)
-
-    def allow_modify_annotation(self, enable, password):
-        """Changes the protection status to modify annotations.
-
-        Parameters
-        ----------
-        enable : bool
-            Set to True to allow editing existing annotations in the borehole document.
-        password : str
-            The password used to allow this option.
-        """
-
-        self._dispatch.AllowModifyAnnotation(enable, password)
-
-    def allow_insert_annotation(self, enable, password):
-        """Changes the protection status for inserting annotations.
-
-        Parameters
-        ----------
-        enable : bool
-            Set to True to allow adding new annotations in the borehole document.
-        password : str
-            The password used to allow this option.
-        """
-
-        self._dispatch.AllowInsertAnnotation(enable, password)
-
-    def allow_modify_headers_content(self, enable, password):
-        """Changes the protection status of the header content.
-
-        Parameters
-        ----------
-        enable : bool
-            Set to True to allow edition of the document header data.
-        password : str
-            The password used to allow this option.
-        """
-
-        self._dispatch.AllowModifyHeadersContent(enable, password)
-
-    def set_metadata(self, id, value):
-        """Sets a metadata value. If the id doesn't exist, this will create it and set the value.
-        Only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        id : str
-            The metadata id.
-        value : str
-            The value to set the metadata to.
-        """
-
-        self._dispatch.SetMetadata(id, value)
-
-    def get_metadata(self, id):
-        """Gets the value metadata value.
-        Only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        id : str
-            The metadata id.
-
-        Returns
-        -------
-        str
-            The value associated with the metadata.
-        """
-
-        return self._dispatch.GetMetadata(id)
-
-    def delete_metadata(self, id):
-        """Removes a metadata id and value pair.
-        Warning: if this metadata is used within a header, the metadata id will remain valid and it's value will be set to null.
-        Only compatible with WellCAD version 5.7 and onwards.
-
-        Parameters
-        ----------
-        id : str
-            The metadata id.
-        """
-
-        self._dispatch.DeleteMetadata(id)
+from ._dispatch_wrapper import DispatchWrapper
+from ._log import Log
+from ._depth import Depth
+from ._header import Header
+from ._title import Title
+from ._page import Page
+from ._workspace import Workspace
+from ._odbc import Odbc
+
+
+class Borehole(DispatchWrapper):
+    _DISPATCH_METHODS = ("Log", "ApplyStructureTrueToApparentCorrection", "ApplyStructureApparentToTrueCorrection",
+                         "RemoveStructuralDip", "ExtractStructureIntervalStatistic", "ColorClassification",
+                         "RepresentativePicks", "ImageComplexityMap", "NormalizeImage", "OrientImageToNorth",
+                         "FilterImageLog", "ApplyConditionalTesting", "RQD", "GrainSizeSorting", "StackTraces",
+                         "AverageFilterFWSLog", "FreqFilterFwsLog", "ApplyStandOffCorrection",
+                         "CompensatedVelocity", "ApplySemblanceProcessing", "ProcessReflectedTubeWave",
+                         "PickFirstArrival", "PickE1Arrival", "ExtractE1Amplitude", "AdjustPickToExtremum",
+                         "ExtractWindowPeakAmplitude", "ApplyNaturalGammaBoreholeCorrection",
+                         "ApplyTotalGammaCalibration", "CorrectDeadSensor", "CalculateFluidVelocity",
+                         "CalculateApparentMetalLoss", "GetLog", "CreateNewWorkspace",  "Workspace", "FileExport",
+                         "ConvertLogTo", "FilterLog", "ResampleLog", "InterpolateLog", "ElogCorrection",
+                         "NMRFluidVolumes", "ROPAverage", "SharpenRGBLog", "RetinexFilterRGBLog", )
+
+    @property
+    def name(self):
+        """str: The title of a borehole document."""
+        return self._dispatch.Name
+
+    @name.setter
+    def name(self, name):
+        self._dispatch.Name = name
+
+    @property
+    def version_major(self):
+        """int: The major version number of WellCAD."""
+        return self._dispatch.VersionMajor
+
+    @property
+    def version_minor(self):
+        """int: The minor version number of WellCAD."""
+        return self._dispatch.VersionMinor
+
+    @property
+    def version_build(self):
+        """int: The build number of WellCAD."""
+        return self._dispatch.VersionBuild
+
+    @property
+    def top_depth(self):
+        """float: The top depth of a borehole in units of the master depth axis."""
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of a borehole in units of the master depth axis."""
+        return self._dispatch.BottomDepth
+
+    @property
+    def nb_of_logs(self):
+        """int: The number of logs in a borehole."""
+        return self._dispatch.NbOfLogs
+
+    @property
+    def auto_update(self):
+        """bool: The auto update status of the borehole."""
+        return self._dispatch.AutoUpdate
+
+    @auto_update.setter
+    def auto_update(self, flag):
+        self._dispatch.AutoUpdate = flag
+
+    def refresh_window(self):
+        """Performs a one time refresh of the borehole view"""
+        self._dispatch.RefreshWindow()
+
+    def show_window(self):
+        """Puts the borhole into focus."""
+        self._dispatch.ShowWindow()
+
+    def set_draft_mode(self, display_mode=None):
+        """Toggles the view of the borehole document.
+
+        Parameters
+        ----------
+        display_mode : int, optional
+            The document viewing mode.  A borehole document can be displayed in the following modes:
+
+                * 0 = Page Layout
+                * 1 = Draft and fit
+                * 2 = Draft
+        """
+        self._dispatch.SetDraftMode(display_mode)
+
+    def minimize_window(self):
+        """Shrinks the document window to an icon.
+
+        Works only if document windows are not tabbed.
+        """
+        self._dispatch.MinimizeWindow()
+
+    def maximize_window(self):
+        """Enlarges the document window to fit the WellCAD frame.
+
+        Works only if document windows are not tabbed.
+        """
+        self._dispatch.MaximizeWindow()
+
+    def set_visible_depth_range(self, top_depth=None, bottom_depth=None):
+        """Adjusts the depth range displayed in a borehole view.
+
+        Parameters
+        ----------
+        top_depth : float
+            The top depth of the visible depth range.
+            If not provided, the current top depth of the document will be used
+        bottom_depth : float
+            The bottom depth of the visible depth range.
+            If not provided, the current bottom depth of the document will be used
+        """
+        self._dispatch.SetVisibleDepthRange(top_depth, bottom_depth)
+
+    @property
+    def depth(self):
+        """Depth: The reference/master vertical axis. Can be in depth or time."""
+        return Depth(self._dispatch.Depth)
+
+    @property
+    def header(self):
+        """Header: The document header for this borehole document."""
+        return Header(self._dispatch.Header)
+
+    @property
+    def page(self):
+        """Page: A page object for the borehole document."""
+        return Page(self._dispatch.Page)
+
+    def create_new_workspace(self, workspace_type, config):
+        """Creates a new workspace object.
+
+        Parameters
+        ----------
+        workspace_type : int
+            * 1 = ISI workspace
+            * 2 = Casing integrity
+            * 3 = NMR
+        config : str
+            Path to a configuration file containing the workspace initialization parameters. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ISIWorkspace]
+                Name= workspace name
+                Log= log name
+                Caliper=100
+                DepthOfImage=0
+                CaliperUnit=mm / inch
+                ApertureUnit=mm / inch/10
+                LengthUnit=m / mm / cm / ft / inch / inch/10
+                RunApparentToTrue=yes
+                Azimuth= log name
+                Tilt= log name
+                ImageOrientation=North / High Side
+                RunRecalculateAzimuth=yes
+                RotationAngle=-12
+                NavigationLog=ICM (log name or nothing)
+                ' RGB OTV image
+                ImageType= 0,
+                'Greyscale OTV image.
+                ImageType=1
+                ' Diamond-drilled hole, ATV image
+                ImageType=2
+                'RC-drilled hole, ATV image
+                ImageType=3
+                'FMI image
+                ImageType=4
+                ICMPalette=0,0,0,255,56,255,0,0,12,64,224,208,21,50,205,50,31,255,255,0,39,255,215,0,47,255,104,32
+                [CasingIntegrityWorkspace]
+                Name= workspace name
+                Log= log name
+                LogUnit=mm / inch
+                DataType=radius / diameter
+                DrillerCasingTable=C:/Temp/Table.txt
+                DrillerCasingTableDepthUnit=meters / feet
+                DrillerCasingTableWeightUnit=lbs/ft / kg/m
+                DrillerCasingTableODUnit=inch / mm
+                [NMRWorkspace]
+                Name= workspace name
+                T2Distribution= log name
+                TraceUnitOfT2Distribution=milliseconds / seconds
+                DefaultLithoDatabase=C:/Program Files/Advanced Logic Technology/WellCAD/Dictionaries/NMR Volumes.lth
+                FluidVolumeComponents=Bound Water, Moveable Water
+                FluidVolumeLithoUseAssociatedColor=no
+                DefaultCutoffValues=33
+                LastDefaultCutoffValueMax=yes
+                DisplayPermeabilityTIMModel=yes
+                PermeabilityTIMModelVariableC=1 (i.e. premultiplier)
+                PermeabilityTIMModelExponentM=4
+                PermeabilityTIMModelExponentN=2
+                PermeabilityTIMModelBFVandFFVLimit= Bound Water
+                DisplayPermeabilitySDRModel=yes
+                PermeabilitySDRModelVariableC=1 (i.e. premultiplier)
+                PermeabilitySDRModelExponentM=4
+                PermeabilitySDRModelExponentN=2
+                DisplayDryMatrixDensity=no
+                BulkDensity=Bulk_Density
+
+        Returns
+        -------
+        Workspace
+            The new workspace object.
+        """
+        return Workspace(self._dispatch.CreateNewWorkspace(workspace_type, config))
+
+    def workspace(self, workspace_id):
+        """Gets an existing workspace object in the document.
+
+        Parameters
+        ----------
+        workspace_id : int or str
+            The zero based index or the name of the workspace
+        Returns
+        -------
+        Workspace or None
+            The workspace object with the specified index or name, or ``None``
+            if the index is out of bounds or if name does not match any of the workspace name.
+        """
+        return Workspace(self._dispatch.Workspace(workspace_id))
+
+    def check_formula(self, formula):
+        """Verifies the syntax of a formula used in a Formula Log.
+
+        Parameters
+        ----------
+        formula : str
+            The formula that needs to be checked.
+            Example: "({GR}-min({GR}))/(max({GR})- min({GR}))"
+
+        Returns
+        -------
+        bool
+            Whether the formula is correct or not.
+        """
+        return self._dispatch.CheckFormula(formula)
+
+    @property
+    def odbc(self):
+        """Odbc: An ODBC object that allows interaction with a database."""
+        return Odbc(self._dispatch.ODBC)
+
+    def connect_to(self, server_name, server_address, port_number):
+        """Connects the current borehole document to an external data source provider.
+
+        Parameters
+        ----------
+        server_name : str
+            The name of the server (TFD is currently the only one supported)
+        server_address : str
+            The IP address of the computer to connect to.
+        port_number : int
+            The part number to connect to.
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+        """
+
+        self._dispatch.ConnectTo(server_name, server_address, port_number)
+
+    def disconnect_from(self, server_name, server_address):
+        """Cuts the connection between the borehole document and the external data source provider.
+
+        Parameters
+        ----------
+        server_name : str
+            The name of the server (TFD is currently the only one supported)
+        server_address : str
+            The IP address of the computer connected to.
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+        """
+        self._dispatch.DisconnectFrom(server_name, server_address)
+
+    def save_as(self, path):
+        """Saves the borehole document as WCL file.
+
+        Parameters
+        ----------
+        path : str, optional
+            The file path to the WellCAD borehole document file to save. If no
+            file path is provided, the user will be prompted to select a file
+            using a standard File Save As dialog box.
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+        """
+        return self._dispatch.SaveAs(path)
+
+    def file_export(self, file_name=None, prompt_user=None, config=None, log_file=None):
+        """Exports the document to the specified file.
+
+        Supported file formats are LAS, DLIS, EMF, CGM, JPG, PNG, TIF,
+        BMP, WCL and PDF. Please refer to the WellCAD help file for a
+        description of the export parameters to be used in the
+        configuration file and parameter string.
+
+        Parameters
+        ----------
+        file_name : str, optional
+            The path and name of the file to export.
+            If not provided, the dialog will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [LASExport]
+                ; LAS files
+                ; For compatibility with older versions of WellCAD:
+                NbEndDepthDigits = 4
+                NbSmpRateDigits = 4
+                LASVersion = 2 / 3
+                Log1 = Depth,Auto,Auto (Log name, Precision, Column width)
+                Log2 = GR, 0, 10
+                'Log3 = … (if no Log is specified all logs will be exported)
+                MaxDepthRange = yes / no
+                TopDepth = 0.0
+                BottomDepth = 150.0
+                SamplingRate = 0.1
+                EnableHeader = yes / no
+                EnableWrap = yes / no
+                NullValue = -999.25
+                Delimiter = 0 (Comma) /1 (Tab) / 2 (Space)
+                CheckConstSmpRate = yes (optional)
+                LimitLineLength = no (optional)
+                ShortMnemonics = no (optional)
+                AlignColumns = yes (optional)
+                ForceDecimalPoint = yes (optional)
+                SignificantDigits = 7 (optional)
+                [DLISExport]
+                ; DLIS files
+                ; If no Log is specified all logs will be exported
+                Log1 = GR
+                Log2 = RHO
+                [ImageExport]
+                ; JPG, PNG, BMP, GIF, TIF files
+                MaxDepthRange = yes / no
+                TopDepth= 0.0
+                BottomDepth= 10.0
+                Resolution=300
+                [EMFExport]
+                ; EMF files
+                MaxDepthRange = yes / no
+                TopDepth= 0.0
+                BottomDepth= 10.0
+                [CGMExport]
+                ; CGM files
+                MaxDepthRange = yes / no
+                TopDepth= 0.0
+                BottomDepth= 10.0
+                [PDFExport]
+                ; PDF files
+                MaxDepthRange = yes / no
+                TopDepth= 0.0
+                BottomDepth= 10.0
+                ; Single page
+                PageStyle=Single
+                ShowProgress=TRUE
+                OpenPDFFile=TRUE
+                ; Standard page
+                PageStyle=Standard
+                Orientation=Portrait / Landscape
+                PaperSize=A4
+                ShowProgress=TRUE
+                OpenPDFFile=TRUE
+                ; Custom page
+                PageStyle=Custom
+                Orientation=Portrait
+                'Orientation=Landscape
+                PaperWidth=2100
+                PaperLength=2970
+                ShowProgress=TRUE
+                OpenPDFFile=TRUE
+                [WCLExport]
+                ; WCL files
+                Format = 5.0
+        log_file : str, optional
+            Path and name of the file to log error messages.
+
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+        """
+        return self._dispatch.FileExport(file_name, prompt_user, config, log_file)
+
+    def do_print(self, enable_dialog=None, top_depth=None, bottom_depth=None, nb_of_copies=None):
+        """Sends the current document to the printer.
+        If the print dialog box is displayed the user can select the
+        printer otherwise the printer installed as default is used.
+
+        Parameters
+        ----------
+        enable_dialog : bool, optional
+            Whether to display the print dialog box or not.
+        top_depth : float, optional
+            The start depth of the interval to print
+            If not provided, the current top depth of the document will be used.
+        bottom_depth : float, optional
+            The bottom depth of the printed depth interval.
+            If not provided, the current bottom depth of the document will be used.
+        nb_of_copies : int, optional
+            The number of copies to be printed.
+        """
+        self._dispatch.DoPrint(enable_dialog, top_depth, bottom_depth, nb_of_copies)
+
+    def read_database(self, script_path):
+        """Opens and interprets an SQL script to download data from a database.
+
+        Parameters
+        ----------
+        script_path : str
+            The path to the SQL script to be called
+
+        Returns
+        -------
+        bool
+            Whether the operation was successful or not.
+        """
+        return self._dispatch.ReadDatabase(script_path)
+
+    def write_database(self, script_path):
+        """Opens and interprets an SQL script to upload data to a database.
+
+        Parameters
+        ----------
+        script_path : str
+            The path to the SQL script to be called
+
+        Returns
+        -------
+        bool
+            Whether the operation was successful or not.
+        """
+        return self._dispatch.WriteDatabase(script_path)
+
+    def get_log(self, index_or_name):
+        """Gets an existing log object in the document.
+
+        Parameters
+        ----------
+        index_or_name :  int or str
+            The zero based index or the name of the log.
+        Returns
+        -------
+        Log
+            The log object with the specified index or name, or ``None``
+            if the index is out of bounds or if name does not match any of the log name.
+        """
+        return Log(self._dispatch.GetLog(index_or_name))
+
+    def title(self, name):
+        """Gets the title object for the specified name.
+
+        Parameters
+        ----------
+        name : str, optional
+            The name of the log or the name of a title box.
+        Returns
+        -------
+        Title
+            The Title object if found, otherwise "None"
+        """
+        return Title(self._dispatch.Title(name))
+
+    def insert_new_log(self, log_type):
+        """Creates a new log and log object.
+
+        Parameters
+        ----------
+            log_type : int, optional
+                The type of log.  Allowed values are :
+
+                    * 1 = Well Log
+                    * 2 = Formula Log
+                    * 3 = Mud Log
+                    * 4 = FWS Log
+                    * 5 = Image Log
+                    * 6 = Structure Log
+                    * 7 = Litho Log
+                    * 8 = Comment Log
+                    * 9 = Engineering Log
+                    * 10 = RGB Log
+                    * 13 = Interval Log
+                    * 14 = Analysis Log
+                    * 15 = Percent Log
+                    * 16 = CoreDesc Log
+                    * 17 = Depth Log
+                    * 18 = Strata Log
+                    * 19 = Stacking Pattern Log
+                    * 20 = Polar and Rose Log
+                    * 21 = Cross Section Log
+                    * 22 = OLE Log
+                    * 23 = Shading Log
+                    * 24 = Marker Log
+                    * 25 = Breakout Log
+                    * 26 = Bio Log
+                    * 27 = Lineation Log
+        Returns
+        -------
+        Log
+            A log object.
+        """
+        return Log(self._dispatch.InsertNewLog(log_type))
+
+    def convert_log_to(self, log, log_type, prompt_user=None, config=None):
+        """New log object by converting one log type into another.
+
+        Please refer to the WellCAD documentation about which log type
+        conversions are possible.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log to convert.
+        log_type : int
+            The type of log to be created.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ConvertLog]
+                ; Analysis, Percentage Log to Litho log
+                ; ComponentNames : list of component names to convert, if not specified all components are taken
+                ComponentNames=A,B
+                ; Bio Log to Bio Log
+                ; TaxonNames : list of taxon names to convert, if not specified all taxons are taken
+                TaxonNames=A,B
+                ; Image, RGB Log to WellLog
+                StartIndex=0
+                Increment=1
+                ; Breakout Log to Breakout, Mud Log
+                FilterOnAttributes= yes / no
+                AttributeName1=Type
+                AttributeList1=RF,MB,…
+                AttributeName2=Condition
+                AttributeList2=Open,Loose,…
+                FilterOnAzimuth= yes / no
+                AzimuthLow=0
+                AzimuthHigh=360
+                FilterOnTilt= yes / no
+                TiltLow=30
+                TiltHigh=90
+                FilterOnLength= yes / no
+                LengthLow=0
+                LengthHigh=100
+                FilterOnOpening= yes / no
+                OpeningLow=0
+                OpeningHigh=45
+                ; Comment Log to Litho Log
+                LithoDatabase=C:/Default.lth
+                ; CoreDesc Log to Interval Log
+                ; CoreDescItemNames : list of symbol codes to convert
+                CoreDescItemNames=AX3, AX5, BZ5
+                ; Structure Log to Structure, Mud Log
+                FilterOnAttributes=TRUE
+                AttributeName1=Type
+                AttributeList1=RF,MB
+                AttributeName2=Condition
+                AttributeList2=Open,Loose
+                FilterOnAzimuth= yes / no
+                AzimuthLow=0
+                AzimuthHigh=360
+                FilterOnTilt= yes / no
+                DipLow=30
+                DipHigh=90
+                FilterOnOpening= yes / no
+                ApertureLow=0
+                ApertureHigh=100
+                ; Structure, Breakout Log to Marker Log
+                DisplayIndex= yes / no
+                DisplayAzimuth= yes / no
+                DisplayTilt= yes / no
+                DisplayAttributes= yes / no
+                ; Interval Log to Mud Log
+                ; ConvertValue : 0=Min, 1=Max, 2=Ave
+                ; AttachDepthTo : 1=attach to top, 2=middle, 3=bottom
+                ConvertValue=0
+                AttachDepthTo=2
+                ; Mud Log to Well Log
+                ; Interpolation : 0 = No Interpolation, 1 = Prev. Data, 2 = Interpol.
+                CreateNewLog= yes / no
+                SamplingRate=0.1
+                MaximumGap=10.0
+                Interpolation=0
+                Tolerance=0.1
+                CircularData = yes / no
+                DataUnit = degrees / radians
+                ; Mud Log to Depth Log
+                ; ConversionType : 1=from m, 2=from ft, 3=from sec; 4=msec, 5=usec
+                ConversionType=1
+                ; Mud Log to Litho Log
+                ; <ClassifierName>=<LithoName> (classification name and corresponding litho code)
+                LithoDatabase=C:/Default.lth
+                className1 = Coal
+                className2 = Limestone
+                ; Percent Log to Analysis Log
+                SamplingRate=0.1
+                ; RGB Log to Image Log (int, float 2 and float 4)
+                ; Color : 0=all, 1=red, 2=green, 3=blue
+                Color=0
+                ; Stack Log to Well Log
+                SamplingRate=0.1
+                ; Strata Log to Comment, Litho Log
+                ; ColumnNames : list of column titles
+                ColumnNames=columnname1, columname4
+                ; VSP Log to Well Log
+                ; TraceNames : list of trace titles
+                TraceNames=
+                ; Well Log to Depth Log
+                ; ConversionType : 1=from m, 2=from ft, 3=from sec; 4=msec, 5=usec
+                ConversionType=1
+                ; Well Log to Litho Log
+                ; <ClassifierName>=<LithoName> (classification name and corresponding litho code)
+                ; SplitLithoLog : creates one litho column per litho type
+                LithoDatabase=C:/Default.lth
+                className1 = Coal
+                className2 = Limestone
+                SplitLithoLog= yes / no
+                ; Litho Log to Strata Log
+                ; SplitColumns : creates one column per litho type
+                SplitColumns= yes / no (creates one column per litho type)
+                ; Litho Log to Litho Log
+                ; LithoBedNames : list of litho codes to convert, if not specified all components are taken
+                LithoBedNames=sst,lst,dst
+
+        Returns
+        -------
+        Log
+            The object of the new log.
+        """
+        return Log(self._dispatch.ConvertLogTo(log, log_type, prompt_user, config))
+
+    def add_log(self, log):
+        """Adds the log object passed as argument of the function into the calling borehole document.
+
+        Parameters
+        ----------
+        log : Log
+            An object of the log to copy.
+        Returns
+        -------
+        Log
+            A copy of the log.
+        """
+        return Log(self._dispatch.AddLog(log._dispatch))
+
+    def remove_log(self, log):
+        """Deletes the specified log from the borehole document.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log to remove.
+        """
+        self._dispatch.RemoveLog(log)
+
+    def clear_log_contents(self, log):
+        """Removes the data from a log and leaves the log empty.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log to remove.
+        """
+        self._dispatch.ClearLogContents(log)
+
+    def apply_template(self, path, prompt_if_not_found=None, create_new_logs=None, create_new_layers=None,
+                       apply_annotation_settings=None, replace_header=None, keep_charts=None, new_charts=None,
+                       overwrite_workspaces=None, new_workspaces=None, delete_non_associated_logs=None, config=None):
+        """Loads and applies a document layout template (.WDT)
+
+        Parameters
+        ----------
+        path : str
+            The path and name of the template WDT file.
+        prompt_if_not_found : bool, optional
+            If True, a dialog box will be displayed for each log not found. Default : True.
+        create_new_logs : bool, optional
+            If True, new logs will be loaded from the template. Default : False.
+        create_new_layers : bool, optional
+            If True, new annotation layers will be loaded from the template. Default : False.
+        apply_annotation_settings : bool, optional
+            If True, settings  will be applied to annotations. Default : False.
+        replace_header : bool, optional
+            If True, the current document header will be replaced. Default : True.
+        keep_charts : bool, optional
+            If True, cross-plot charts will be kept in the document. Default : True.
+        new_charts : bool, optional
+            If True, cross-plot charts will be loaded from the template. Default : False.
+        overwrite_workspaces : bool
+            If True, work spaces in the document will be overwritten. Default : False.
+        new_workspaces : bool, optional
+            If True, work spaces will be loaded from the template. Default : False.
+        delete_non_associated_logs : bool, optional
+            If True, only logs from the template will be kept in the document. Default : True.
+        config : str, optional
+            Path and filename of the configuration file or parameter string.
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+        """
+        return self._dispatch.ApplyTemplate(path, prompt_if_not_found, create_new_logs, create_new_layers,
+                                            apply_annotation_settings, replace_header, keep_charts, new_charts,
+                                            overwrite_workspaces, new_workspaces, delete_non_associated_logs, config)
+
+    def slice_log(self, log, slice_depth, create_top=None, create_bottom=None, keep_original=None):
+        """Allows the separation of the log data into a top and bottom section. New logs can be created \
+        holding the data of the top and bottom parts of the data set.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log to slice.
+        slice_depth : float
+            The depth at which the slice will be made.
+        create_top : bool, optional
+            If set to TRUE (default) a new log will be created holding the data from the current
+            top of the data set down to the slice depth..
+        create_bottom : bool, optional
+            If set to TRUE (default) a new log will be created holding the data from the slice depth
+            down to the bottom of the data set.
+        keep_original : bool, optional
+            If set to TRUE (default) the original log will be kept in the document.
+        """
+        self._dispatch.SliceLog(log, slice_depth, create_top, create_bottom, keep_original)
+
+    def merge_logs(self, log_a, log_b, ave_overlap=None, create_new=None):
+        """Merges the data of the two specified logs.
+
+        Parameters
+        ----------
+        log_a : str or int
+            The title or the zero based index of the log. If no new log is created this log
+            will receive the data from log_b.
+        log_b : str or int
+            The title or the zero based index of the log.
+        ave_overlap : bool, optional
+            If set to False log_a will overwrite log_b, if set to True, data from the two logs will be averaged
+            over the depth overlap.
+        create_new : bool
+            If set to False log_b will be pushed into log_a and the log_b will be removed
+        """
+        self._dispatch.MergeLogs(log_a, log_b, ave_overlap, create_new)
+
+    def merge_same_log_items(self, log):
+        """Merges consecutive data intervals of same litho codes, text or data within the specified log.
+        This function applies to Litho, Comment, Engineering, CoreDesc, Interval, Stack and Bio logs.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        """
+        self._dispatch.MergeSameLogItems(log)
+
+    def extend_log(self, log, top_depth, bottom_depth):
+        """Extends the allocated depth range of Well, Formula and Analysis Logs.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the Well log.
+        top_depth : float
+            The new top depth of the log in units of the current depth axis.
+        bottom_depth : float
+            The new bottom depth of the log in units of the current depth axis.
+        """
+        self._dispatch.ExtendLog(log, top_depth, bottom_depth)
+
+    def depth_shift_log(self, log, shift, top_depth=None, bottom_depth=None):
+        """Allows the depth shifting of the log's data by the specified amount.
+        By default, the entire data column will be shifted (i.e. block shift). If a Top and Bottom depth
+        has been specified only the data within the specified interval will be shifted.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log.
+        shift : float
+            The amount of depth shift to be applied. A negative value will shift the data up and
+            a positive value applies a downward shift.
+        top_depth : float, optional
+            The upper depth limit of the shifted interval.
+            If not provided, this is the current top depth of the log
+        bottom_depth : float, optional
+            The lower depth limit of the shifted interval.
+            If not provided, this is the current bottom depth of the log
+        """
+        self._dispatch.DepthShiftLog(log, shift, top_depth, bottom_depth)
+
+    def depth_match_log(self, log=None, depth_log=None):
+        """Depth matches the specified log using the links created from the specified depth_log (i.e. a shift table).
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+            If not provided, the Depth Matcher dialog box will be displayed.
+        depth_log : str or int, optional
+            The title or the zero based index of the Depth log containing the shift table.
+            If not provided, the Depth Matcher dialog box will be displayed.
+        """
+        self._dispatch.DepthMatchLog(log, depth_log)
+
+    def fill_log(self, log, top_depth, bottom_depth, step, thickness, user_defined_intervals=None, interval_log=None):
+        """Fill a Cross-section Log or a Polar & Rose Log with intervals automatically.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log.
+        top_depth : float
+            The top depth of the first interval in units of the current depth axis.
+        bottom_depth : float
+            The last depth at which an interval could start in units of the current depth axis.
+        step : float
+            The frequency of the intervals in units of the current depth axis (every 2 m).
+        thickness : float
+            The interval thickness in units of the current depth axis.
+        user_defined_intervals : bool, optional
+            If set to False the intervals will be loaded from a reference log.
+        interval_log : str or int, optional
+            The title or the zero based index of the log containing the reference intervals.
+        """
+        self._dispatch.FillLog(log, top_depth, bottom_depth, step, thickness, user_defined_intervals, interval_log)
+
+    def filter_log(self, log, prompt_user=None, config=None):
+        """Calculates a new filtered data set of a Well Log.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [FilterLog]
+                ; FilterType : Median, MovingAverage, WeightedAverage
+                ; DataUnit : degrees, radians
+                FilterType =
+                FilterWidth = 5
+                MaxDepthRange = yes
+                TopDepth = 5.0
+                BottomDepth = 10.0
+                CircularData = yes
+                DataUnit = degrees
+
+        Returns
+        -------
+        Log
+            An object of the filtered log.
+        """
+        return Log(self._dispatch.FilterLog(log, prompt_user, config))
+
+    def block_log(self, log=None, prompt_user=None, config=None):
+        """Calculates statistical values for each depth interval determined from a
+        reference log or specified by the user.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [BlockLog]
+                CircularData = yes / no
+                DataUnit = degrees / radians
+                ReferenceInterval = Lithology / 10.0
+                Cumulate = yes / no
+                OutputLogAsText = yes / no
+                OutputLogAsGraphic = yes / no
+                Minimum = yes / no
+                Maximum = yes / no
+                Mode = yes / no
+                Average = yes / no
+                Median = yes / no
+                StdDev = yes / no
+                Percentage = yes / no
+                Sum = yes / no
+                SumNorm= yes / no
+                Area = yes / no
+                MeanAbsoluteDeviation = yes / no
+                GeometricMean = yes / no
+                GeometricStdDev = yes / no
+                Skewness = yes / no
+                Kurtosis = yes / no
+                Quartiles = yes / no
+                AveragePlusStdDev = yes / no
+                AverageMinusStdDev = yes / no
+                RMS = Yes / No
+                Value1 = 50 / NULL
+                Value2 = 100
+                Resolution = 0.1
+                EmptyIntervalMode = Interpolate / Maximum / Minimum / Null
+        """
+        self._dispatch.BlockLog(log, prompt_user, config)
+
+    def extract_well_log_statistics(self, logs=None, prompt_user=None, config=None):
+        """Extracts minimum, maximum, average, median and other statistical values fulfilling
+        an optional condition from each Well log
+
+        Parameters
+        ----------
+        logs : list, optional
+            The list of the titles or the zero base indexes of the logs to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ExtractWellLogStatistics]
+                ; Condition : 0=None, 1=lower than Value 1, 2=larger than Value1, 3=lower and equal,
+                ; 4=larger and equal,5=equal, 6=not equal, 7=between Value1 and Value2,
+                ; 8=between and equal to Value1 and Value2
+                Minimum = yes / no
+                Maximum = yes / no
+                Mode = yes / no
+                Average = yes / no
+                Median = yes / no
+                StandardDeviation = yes / no
+                Percentage = yes / no
+                MeanAbsoluteDeviation = yes / no
+                GeometricMean = yes / no
+                GeometricStandardDeviation = yes / no
+                Skewness = yes / no
+                Kurtosis = yes / no
+                Quartiles = yes / no
+                RMS = yes / no
+                RMSD = yes / no
+                Condition = 0
+                Value1 = 50
+                Value2 = 100
+                OneOutputlogPerImageLog = yes / no
+        """
+        self._dispatch.ExtractWellLogStatistics(logs, prompt_user, config)
+
+    def normalize(self, log=None, prompt_user=None, config=None):
+        """Normalizes the data in a Percentage or Analysis Log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [AnalysisLogNormalize]
+                ComponentsToDelete= 20, 05#1, Artifacts (Codes of the patterns to be
+                removed separated by commas)
+                CreateNewLog=yes
+                At100=yes
+        """
+        self._dispatch.Normalize(log, prompt_user, config)
+
+    def tvd(self, log=None, prompt_user=None, config=None):
+        """Calculates a TVD either from another TVD log (Depth Log) or from a tilt log (Well Log).
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [TVD]
+                Output=TVD /Elevation
+                ExtrapolateBack=yes /no
+                TVDAtZero=0.0
+
+        Returns
+        -------
+        Log
+            The newly created Log containing the TVD data.
+        """
+        return Log(self._dispatch.TVD(log, prompt_user, config))
+
+    def rop_average(self, log=None, prompt_user=None, config=None):
+        """Computes the average rate of penetration over specified depth intervals
+        for a Mud Log or a Well Log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ROPAverage]
+                ReferenceInterval=Litho ; log title or constant value indicating the interval height
+                OutputLogAsGraphic=no
+                OutputLogAsText=yes
+                DepthRange=Maximum ;Maximum, UserDefined, Zones, LogZones
+                TopDepth=105
+                BottomDepth=120
+                ;LogZones : top1, bot1, top2, bot2, ... topN, botN
+                LogZones=
+                ; LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+                LogZonesDepthRange=Litho,06,05#1
+
+        Returns
+        -------
+        Log
+            The newly created Log.
+        """
+        return Log(self._dispatch.ROPAverage(log, prompt_user, config))
+
+    def unit_conversion(self, log=None, prompt_user=None, config=None):
+        """Converts the units used in a log.
+
+        Units are organized in categories (e.g. Length, Weight or Temperature).
+
+        Parameters
+        ----------
+        log : str or int, optional
+            The title or the zero based index of the log.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [UnitConversion]
+                Category=Length / Weight / Temperature
+                FromUnit=mm
+                ToUnit=in
+                CreateNewLogs=yes/no
+        """
+        self._dispatch.UnitConversion(log, prompt_user, config)
+
+    def zonation(self, logs=None, prompt_user=None, config=None):
+        """Splits log data into zones.
+
+        This is an automated version of the Zonation process in WellCAD.
+
+        Parameters
+        ----------
+        logs : list, optional
+            The list of the titles or the zero base indexes of the logs to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [Zonation]
+                UseIntervalThickness = yes/no (set to "no" to neglect theNbOuptutIntervals parameter)
+                NbOutputIntervals = 2
+                IntervalMinThickness = 0.5
+                UseLithoLogAsOutput = yes/no
+        """
+        self._dispatch.Zonation(logs, prompt_user, config)
+
+    def resample_log(self, log, prompt_user=None, config=None):
+        """Resamples a data set according to a new constant sampling rate or sample point
+        determined from a reference log.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ResampleLog]
+                ; For mud / well logs
+                ; ReferenceLog : log title of a Mud or Percentage Log
+                SamplingRate = 0.1
+                ReferenceLog = Plugs
+                UseReferenceLog = yes / no
+                UseNearestPoint = yes / no
+                CircularData = yes / no
+                DataUnit = degrees / radians
+                ; For image logs
+                VerticalSamplingFactor = 1
+                RadialSamplingFactor = 1
+                RadialDownSampling = yes / no
+        """
+        return Log(self._dispatch.ResampleLog(log, prompt_user, config))
+
+    def interpolate_log(self, log, prompt_user=None, config=None):
+        """Allows the interpolation of Mud and Well Log data to close no data gaps in a data set.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [InterpolateLog]
+                MaximumGap = 0.25
+                CircularData = yes / no
+                DataUnit = degrees / radians
+        Returns
+        -------
+        Log
+            An object of the interpolated log.
+        """
+        return Log(self._dispatch.InterpolateLog(log, prompt_user, config))
+
+    def auto_joint_detection(self, log, prompt_user=None, config=None):
+        """Detects the joints from the main log (data source) used
+        in the workspace.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : str or int
+            The title or the zero based index of the log.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [AutoJointDetection]
+                Sensitivity = 5
+                TopAndBottom = yes
+        """
+        self._dispatch.AutoJointDetection(log, prompt_user, config)
+
+    def calculate_borehole_deviation(self, prompt_user=None, config=None):
+        """Calculates borehole Azimuth, RBR and Tilt from magnetometer and inclinometer / accelerometer data.
+
+        Parameters
+        ----------
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CalculateBoreholeDeviation]
+                ; MagX, MagY, MagZ : the title of the corresponding log
+                ; InclX, InclY, InclZ : the title of the corresponding log
+                MagX = Mag X
+                MagY = Mag Y
+                MagZ = Mag Z
+                InclX = Acc X
+                InclY = Acc Y
+                InclZ =
+                MagXPositive = yes / no
+                MagYPositive = yes / no
+                MagZPositive = yes / no
+                InclXPositive = yes / no
+                InclYPositive = yes / no
+                InclZPositive = yes / no
+                IsAccelerometer = yes / no
+                MarkerPosition = 182.5
+        """
+        self._dispatch.CalculateBoreholeDeviation(prompt_user, config)
+
+    def calculate_borehole_volume(self, prompt_user=None, config=None):
+        """Calculates the volume of an entire hole or annulus (e.g. between casing and borehole wall)
+        from an Image logs containing radius values or a Well logs providing caliper values.
+
+        Parameters
+        ----------
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            Note: This configuration is for WellCAD version 5.7 and onwards. For prior version, see the next section.
+
+            .. code-block:: ini
+
+                [VolumeProcess]
+                ; OuterDiam, InnerDiam : name of a well log, img log or a constant value
+                ; OuterDiamUnit, InnerDiamUnit : inch or mm, default to mm
+                ; OuterDiam1, InnerDiam1 : name of a well log, img log or a constant value.
+                ; Use either OuterDiam, InnerDiam or OuterDiam1, InnerDiam1 but not both !
+                ; OuterDiamUnit1, InnerDiamUnit1 : inch or mm, default to mm.
+                ; Use either OuterDiamUnit, InnerDiamUnit or OuterDiamUnit1, InnerDiamUnit1 but not both !
+                ; OuterDiam2, InnerDiam2 : name of a well log
+                ; OuterDiamUnit2, InnerDiamUnit2 : inch or mm, default to mm
+                ; IntervalRef : name of a well log or value (if value, in depth units of the borehole doc)
+                ; DepthRange : Maximum, UserDefined, Zones, LogZones
+                ; LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+                OuterDiam=
+                OuterDiamUnit=mm
+                InnerDiam=
+                InnerDiamUnit=mm
+                OuterDiam1=w_diam_ext
+                OuterDiamUnit1=mm
+                OuterDiam2=
+                OuterDiamUnit2=mm
+                OuterDiam3=
+                OuterDiamUnit3=mm
+                OuterDiam4=
+                OuterDiamUni4t=mm
+                InnerDiamUnit=mm
+                InnerDiam1=
+                InnerDiamUnit1=mm
+                OuterDiamAsDiameter=yes
+                InnerDiamAsDiameter=yes
+                AnnularVolume=no
+                BottomToTop=yes
+                VolumeUnit=litre
+                DisplayTick=no
+                SmallTickFreq=1
+                MediumTickFreq=10
+                LargeTickFreq=100
+                DisplayNumerical=no
+                NumericalFreq=10
+                DisplayInterval=no
+                IntervalRef=10
+                DisplayCurve=yes
+                DepthRange=Maximum
+                TopDepth=10
+                BottomDepth=19
+                ZonesDepthRange=
+                LogZonesDepthRange=Litho,06,05#1
+
+
+            For WellCAD version 5.5 and 5.6, use this configuration instead:
+
+            .. code-block:: ini
+
+                [VolumeProcess]
+                InnerDiam = 100 / log name
+                InnerDiamUnit = mm/in/cm/ft/yd
+                OuterDiam = 110 / log name
+                OuterDiamUnit = mm/in/cm/ft/yd
+                AnnularVolume = yes/no
+                BottomToTop = yes/no
+                VolumeUnit = litre/cu.yd/cu.ft/cu.in/cu.cm/cu.m
+                DisplayTick = yes/no
+                SmallTickFreq = 1
+                MediumTickFreq = 10
+                LargeTickFreq = 100
+                DisplayNumerical = yes/no
+                NumericalFreq = 10
+                DisplayCurve = yes/no
+                DisplayInterval = yes/no
+                IntervalRef = 10
+                MaxDepthRange = yes/no
+                TopDepth = 0.0
+                BottomDepth = 123.5
+        """
+        self._dispatch.CalculateBoreholeVolume(prompt_user, config)
+
+    def calculate_borehole_coordinates(self, prompt_user=None, config=None):
+        """Calculates the deviation path coordinates Northing, Easting and TVD.
+
+        Parameters
+        ----------
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CalculateBoreholeCoordinates]
+                ; Method : Classic Tangential, Balanced Tangential, Radius Of Curvature, MinimumCurvature
+                ; AzimuthLog : the title of the log corresponding to the azimuth.
+                ; TiltLog : the title of the log corresponding to the tilt.
+                Method = Classic Tangential
+                Unit = m / ft
+                AzimuthLog = AZI
+                TiltLog = TILT
+                NewDepthLog = yes / no
+                CountTVDFromLogTop = yes / no
+                TVDStartDepth = 0.0
+                MagDeclination = 11.5
+                EstimateErrors = yes / no
+                AziError = 0.1
+                TiltError = 0.1
+        """
+        self._dispatch.CalculateBoreholeCoordinates(prompt_user, config)
+
+    def calculate_borehole_closure(self, prompt_user=None, config=None):
+        """Calculates the deviation path closure distance, closure angle and DLS.
+
+        Parameters
+        ----------
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CalculateBoreholeClosure]
+                ; AzimuthLog : the title of the log corresponding to the azimuth.
+                ; TiltLog : the title of the log corresponding to the tilt.
+                ; NorthingLog : the title of the log corresponding to the deviation along the north axis.
+                ; EastingLog : the title of the log corresponding to the deviation along the east axis.
+                AzimuthLog = AZI
+                TiltLog = TILT
+                NorthingLog = NORTH
+                EastingLog = EAST
+        """
+        self._dispatch.CalculateBoreholeClosure(prompt_user, config)
+
+    def elog_correction(self, prompt_user=None, config=None):
+        """Applies the environmental corrections for normal resisitivity data.
+
+        Parameters
+        ----------
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ElogCorrection]
+                ; Method : QL40-Elog (Bridle), QL40-Elog (Surface fish), Schlumberger
+                ; LogN8 : the title of the log corresponding to the electrode N8.
+                ; LogN16 : the title of the log corresponding to the electrode N16.
+                ; LogN32 : the title of the log corresponding to the electrode N32.
+                ; LogN64 : the title of the log corresponding to the electrode N64.
+                ; LogNx : the title of the log corresponding to the electrode Nx.
+                Method=QL40-Elog (Bridle)
+                LogN8=N8
+                LogN16=N16
+                LogN32=
+                LogN64=
+                LogNx=
+                ElectrodeSpacingNx=8
+                ElectrodeSpacingNxUnit=inch (in inch, in, inches or mm)
+                ElectrodeDiameter=1.57
+                ElectrodeDiameterUnit=inch (in inch, in, inches or mm)
+                BoreholeDiameter=2.20
+                BoreholeDiameterUnit=inch (in inch, in, inches or mm)
+                FluidResistivity=25 (log name or value in ohm.m)
+        Returns
+        -------
+        Log
+            An object of the last corrected log.
+        """
+        return Log(self._dispatch.ElogCorrection(prompt_user, config))
+
+    def correct_bad_traces(self, log=None):
+        """Replaces NULL data traces in Image, RGB and FWS logs.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        """
+        self._dispatch.CorrectBadTraces(log)
+
+    def stack_traces(self, is_spectrum=None, log=None, prompt_user=None, config=None):
+        """Stacks multiple FWS traces to create and average trace.
+
+        Parameters
+        ----------
+        is_spectrum : bool, optional
+            Whether the log is a spectrum or not.
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [StackTraces]
+                NumberOfStacks = 5
+        Returns
+        -------
+        Log
+            The resulting log.
+        """
+
+        return Log(self._dispatch.StackTraces(is_spectrum, log, prompt_user, config))
+
+    def slice_traces(self, log=None, prompt_user=None, config=None):
+        """Allows the user to keep only a portion of a FWS log's traces. Updates the log in place.
+        
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [SliceTraces]
+                start = 0  ; in log units
+                end = 0  ; in log units
+        """
+
+        self._dispatch.SliceTraces(log, prompt_user, config)
+
+    def apply_conditional_testing(self, log_if=None, log_then=None, prompt_user=None, config=None):
+        """Applies conditional testing (If-Then-Else) to image log
+        values.
+
+        Parameters
+        ----------
+        log_if : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log used for the 'If' clause.
+        log_then : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log used for the 'Then' clause.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ApplyConditionalTesting]
+                Condition = != / <= / >= / > / < / ==
+                ConditionValue = 100.0
+                IsSecondCondition = yes / no
+                SecondLogTest = <title of second log to test>
+                OperatorSecondCondition = AND / OR
+                SecondCondition = != / <= / >= / > / < / ==
+                SecondConditionValue = 120.0
+                ThenValue = NULL
+                ElseValue = Amplitude
+
+        Returns
+        -------
+        Log
+            A newly created log.
+        """
+        return Log(self._dispatch.ApplyConditionalTesting(log_if, log_then, prompt_user, config))
+
+    def filter_image_log(self, log=None, prompt_user=None, config=None):
+        """Average, median and clipping filter for image logs.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [FilterImageLog]
+                FilterType = Average / Median / Despiking
+                FilterWidth = 3
+                FilterHeight = 3
+                HighCutLimit = 75
+                LowCutLimit = 15
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+        return Log(self._dispatch.FilterImageLog(log, prompt_user, config))
+
+    def mirror_image(self, log=None):
+        """Rearranges the data within an image log so that the data
+        appears mirrored when compared to the original image.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        """
+        self._dispatch.MirrorImage(log)
+
+    def rotate_image(self, log=None, prompt_user=None, config=None):
+        """Rotate the image data by adding an angle (clockwise
+        rotation) or subtracting it (counterclockwise rotation).
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RotateImage]
+                RotateBy= 1.2 / Log
+                RotateClockwise = yes / no
+        """
+        self._dispatch.RotateImage(log, prompt_user, config)
+
+    def orient_image_to_highside(self, log=None, prompt_user=None, config=None):
+        """Rotates an image log to high side according to the
+        deviation channels provided.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [OrientImageToHighside]
+                InclX = Acc X
+                InclY = Acc Y
+                InclZ =
+                InclXPositive = yes / no
+                InclYPositive = yes / no
+                InclZPositive = yes / no
+                IsAccelerometer = yes / no
+                MarkerPosition = 180.2
+        """
+        self._dispatch.OrientImageToHighside(log, prompt_user, config)
+
+    def orient_image_to_north(self, log=None, prompt_user=None, config=None):
+        """Rotates an image log to magnetic north according to the
+        deviation channels provided.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+                        Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [OrientImageToNorth]
+                MagX = Mag X
+                MagY = Mag Y
+                MagZ = Mag Z
+                InclX = Acc X
+                InclY = Acc Y
+                InclZ =
+                MagXPositive = yes / no
+                MagYPositive = yes / no
+                MagZPositive = yes / no
+                InclXPositive = yes / no
+                InclYPositive = yes / no
+                InclZPositive = yes / no
+                IsAccelerometer = yes / no
+                MarkerPosition = 180.2
+        """
+        self._dispatch.OrientImageToNorth(log, prompt_user, config)
+
+    def extract_image_log_statistics(self, log=None, prompt_user=None, config=None):
+        """Extracts minimum, maximum, average, median and other
+        statistical values fulfilling an optional condition from each
+        image log trace.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ExtractImageLogStatistics]
+                Minimum = yes / no
+                Maximum = yes / no
+                Mode = yes / no
+                Average = yes / no
+                Median = yes / no
+                StandardDeviation = yes / no
+                Percentage = yes / no
+                MeanAbsoluteDeviation = yes / no
+                GeometricMean = yes / no
+                GeometricStandardDeviation = yes / no
+                Skewness = yes / no
+                Kurtosis = yes / no
+                Quartiles = yes / no
+                RMS = yes / no
+                RMSD = yes / no
+                Condition = 0 (None) / 1 (lower than Value 1) / 2 (larger than Value1) / 3 (lower and equal)
+                / 4 (larger and equal) / 5 (equal) / 6 (not equal) / 7 (between Value1 and Value2)
+                / 8 (between and equal to Value1 and Value2)
+                Value1 = 50
+                Value2 = 100
+                OneOutputlogPerImageLog = yes / no
+                DepthRange = Maximum / UserDefined / Zones / LogZones
+                TopDepth = 1.0
+                BottomDepth = 200.0
+                ZonesDepthRange = 10.0, 20.0, 50.0, 80.0 (top1, bottom1,...,topN, bottomN)
+                LogZonesDepthRange=Litho,06,05 (log name, interval code 1, interval code 2,...)
+        """
+        self._dispatch.ExtractImageLogStatistics(log, prompt_user, config)
+
+    def normalize_image(self, log=None, prompt_user=None, config=None):
+        """Applies Static or Dynamic normalization to image logs
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [NormalizeImage]
+                Mode = Static /Dynamic_1D / Dynamic_2D / HighPass
+                WindowHeight = 0.3
+                WindowWidth = 5
+
+
+        Returns
+        -------
+        Log
+            The normalized log.
+        """
+        return Log(self._dispatch.NormalizeImage(log, prompt_user, config))
+
+    def image_complexity_map(self, log=None, prompt_user=None, config=None):
+        """Computes the complexity map from an RGB or image log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ImageComplexityMap]
+                LogType=1
+                ;RGB OTV image: 0,
+                ;Greyscale OTV image: 1,
+                ;Diamond-drilled hole, ATV image: 2,
+                ;RC-drilled hole, ATV image: 3,
+                ;FMI image: 4,
+                Palette=0,0,0,255,56,255,0,0,12,64,224,208,21,50,205,50,31,255,255,0,39,255,215,0,47,255,104,32
+
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+        return Log(self._dispatch.ImageComplexityMap(log, prompt_user, config))
+
+    def apply_structure_apparent_to_true_correction(self, log=None, prompt_user=None, config=None):
+        """Corrects the apparent azimuth and dip angles in a
+        Structure log
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+            [ApplyStructureApparentToTrueCorrection]
+            AzimuthLog = azimuth log name
+            TiltLog = tilt log name
+            ReferenceIsNorth = yes / no
+
+        Returns
+        -------
+        Log
+            The corrected log.
+        """
+        return Log(self._dispatch.ApplyStructureApparentToTrueCorrection(log, prompt_user, config))
+
+    def apply_structure_true_to_apparent_correction(self, log=None, prompt_user=None, config=None):
+        """Recalculates the apparent azimuth and dip angles in a
+        Structure log from the true structure angles.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ApplyStructureApparentToTrueCorrection]
+                AzimuthLog = azimuth log name
+                TiltLog = tilt log name
+                ReferenceIsNorth = yes / no
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+        return Log(self._dispatch.ApplyStructureTrueToApparentCorrection(log, prompt_user, config))
+
+    def recalculate_structure_azimuth(self, log=None, prompt_user=None, config=None):
+        """Adds or subtracts a value from all Azimuth data within a
+        structure log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RecalculateStructureAzimuth]
+                Angle = 45 / Log
+                RotateClockwise = yes / no
+                MaxDepthRange = yes / no
+                TopDepth = 0.0
+                BottomDepth = 1.0
+
+        """
+        self._dispatch.RecalculateStructureAzimuth(log, prompt_user, config)
+
+    def recalculate_structure_dip(self, log=None, prompt_user=None, config=None):
+        """Correct the dip angle data within a structure log for new
+        caliper settings.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RecalculateStructureDip]
+                Caliper = Log / 200.0
+                CaliperUnit = mm / in
+                MaxDepthRange = yes / no
+                TopDepth = 0
+                BottomDepth = 1
+
+        """
+        self._dispatch.RecalculateStructureDip(log, prompt_user, config)
+
+    def remove_structural_dip(self, log=None, prompt_user=None, config=None):
+        """Removes a given regional dip and azimuth from the data in
+        a structure log and recalculates new Dip and Azimuth angles.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RemoveStructuralDip]
+                Azimuth = Log /45
+                Dip = Log /10
+                MaxDepthRange = yes / no
+                TopDepth = 0.0
+                BottomDepth = 1.0
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+        return Log(self._dispatch.RemoveStructuralDip(log, prompt_user, config))
+
+    def extract_color_components(self, log=None, method=None, color_model=None, prompt_user=None):
+        """Allows the extraction of color data from an RGB Log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        method : int, optional
+            The methode used.
+            Available models are:
+
+            * 0 = Average
+            * 1 = Mode
+            * 2 = Image Log
+        color_model : int, optional
+            The color model used.
+            Available models are:
+
+            * 0 = RGB
+            * 1 = HSV
+            * 2 = YUV
+            * 3 = CIELAB
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        """
+        self._dispatch.ExtractColorComponents(log, method, color_model, prompt_user)
+
+    def color_classification(self, log=None, prompt_user=None, config=None):
+        """Builds color classes from an RGB Log based on user
+        specified reference colors.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the RGB log to process.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ColorClassification]
+                OutputImage = yes
+                OutputAnalysis = yes
+                NoiseReduction = 10
+                Class1="Class 1";"0,255,0";58;50;"166,143,81"
+                Class2="Class 2";"255,0,255";37;50;"44,42,34"
+                Class3="Class 3";"255,255,0";34;50;"251,165,75"
+
+        Returns
+        -------
+        Log
+            Returns an RGB Log or an Analysis Log depending on the configuration file.
+            Returns the RGB Log if both options are selected.
+        """
+        return Log(self._dispatch.ColorClassification(log, prompt_user, config))
+
+    def adjust_image_brightness_and_contrast(self, log=None, prompt_user=None):
+        """Adjusts the brightness and contrast in RGB logs
+
+        Parameters
+        ----------
+        log : str or int, optional
+            A string specifying the log name or an integer
+            representing the index of the log to be processed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to False, the new brightness and
+            contrast values will be determined automatically.
+        """
+        self._dispatch.AdjustImageBrightnessAndContrast(log, prompt_user)
+
+    def retinex_filter_rgb_log(self, log=None, prompt_user=None, config=None):
+        """Applies a retinex filter to the RGB log.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Not Used for this function.
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+
+        return Log(self._dispatch.RetinexFilterRGBLog(log, prompt_user, config))
+
+    def sharpen_rgb_log(self, log=None, prompt_user=None, config=None):
+        """Sharpens the RGB log.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Not Used for this function.
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+
+        return Log(self._dispatch.SharpenRGBLog(log, prompt_user, config))
+
+    def extract_structure_interval_statistic(self, log=None, prompt_user=None, config=None):
+        """Allows determination of statistical values (e.g. frequency
+        of dips) per interval from a structure log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ExtractStructureIntervalStatistic]
+                Reference = 5.0 / Log
+                OutputMinAzimuth = yes / no
+                OutputMaxAzimuth = yes / no
+                OutputAverageAzimuth = yes / no
+                OutputMinDip = yes / no
+                OutputMaxDip = yes / no
+                OutputAverageDip = yes / no
+                OutputMinTilt = yes / no
+                OutputMaxTilt = yes / no
+                OutputAverageTilt = yes / no
+                OutputMinAperture = yes / no
+                OutputMaxAperture = yes / no
+                OutputAverageAperture = yes / no
+                OutputMinLength = yes / no
+                OutputMaxLength = yes / no
+                OutputAverageLength = yes / no
+                OutputMinOpening = yes / no
+                OutputMaxOpening = yes / no
+
+        Returns
+        -------
+        Log
+            One of the computed log.
+        """
+        return Log(self._dispatch.ExtractStructureIntervalStatistic(log, prompt_user, config))
+
+    def rqd(self, log=None, prompt_user=None, config=None):
+        """Computes the Rock Quality Designation from the structure
+        picks in a Structure Log.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RQD]
+                CorePieceLength = 0.1
+                CoreLength = 1
+                AttributeName1 = Defect Type
+                AttributeValues1 = JT-MAJ, JT-MED, JT-MIN,
+                AttributeName2 = Defect Condition
+                AttributeValues2 = cont, part
+                DepthRange = Maximum / UserDefined / Zones
+                'UserDefined
+                TopDepth=25
+                BottomDepth=30
+                'Zones
+                ZonesDepthRange = 20,26, 24,30
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+        return Log(self._dispatch.RQD(log, prompt_user, config))
+
+    def representative_picks(self, log=None, prompt_user=None, config=None):
+        """Used to derive the most representative picks from a
+        Structure log given user defined classification limits.
+
+        Parameters
+        ----------
+        log : str or int, optional
+            Zero based index (integer) or title (string) of
+            the log to process. If not provided, a dialog box
+            displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with
+            the user. If set to  ``False`` the processing parameters
+            will be retrieved from the specified configuration
+            file. If no configuration file has been specified,
+            default values will be used.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RepresentativePicks]
+                TopDepth=0.0
+                BottomDepth=10.0
+                TiltWindow=5.0 (structural dip angle interval, here +/- 5 degrees)
+                AzimuthWindow=15.0 (structural azimuth angle interval, here +/- 15 degrees)
+                DepthWindow=0.5
+                KeepFeaturesUngrouped=TRUE / FALSE
+
+        Returns
+        -------
+        Log
+            The computed log.
+        """
+        return Log(self._dispatch.RepresentativePicks(log, prompt_user, config))
+
+    def correct_dead_sensor(self, log=None, prompt_user=None, config=None):
+        """Corrects the Null and invalid data columns in Image logs.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [DeadSensor]
+                ; Method : Automatic, Range, Columns
+                ; ReplaceBy : Null, Average, Median, Interpolate, LogName or a numerical value
+                Method = Automatic
+                ReplaceBy = Average
+                ; If Method = Automatic
+                WindowHeight = 0
+                Discrimination = 0.125
+                MinDataHeight = 0
+                ; If Method = Range
+                WindowHeight = 0
+                Low = 0
+                High = 0
+                ; If Method = Columns
+                ; Columns : single index value or range like 15-20
+                Columns = 1
+        Returns
+        -------
+        Log
+            A log with the corrected data.
+        """
+        return Log(self._dispatch.CorrectDeadSensor(log, prompt_user, config))
+
+    def shift_correction(self, log=None, prompt_user=None, config=None):
+        """Corrects the drift of data (e.g. MFC) in Image logs.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ShiftCorrection]
+                ; Zone1 : name, top, bottom, value
+                OutputCorrections = yes / no
+                ExtendTrends = yes / no
+                Zone1=ref1, 25.0, 26.0, 101.2
+                Zone2=ref2, 45.0, 47.0, 125.3
+
+        Returns
+        -------
+        Log
+            A log that has been corrected.
+        """
+        return Log(self._dispatch.ShiftCorrection(log, prompt_user, config))
+
+    def calculate_fluid_velocity(self, log=None, prompt_user=None, config=None):
+        """Estimates the fluid velocity from travel time measurements and given calibration points.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CalculateFluidVelocity]
+                ; If the AutoFill option is used the CalibrationPoints are not used.
+                ; ToolRadius : in mmm
+                ; TimeWindow : log name or value
+                ; CalibrationPoint1 : depth, diameter in mm
+                ; AutoFillFrom : depth value or 'Top'
+                 ; AutoFillTo : depth value or 'Bottom'
+                TravelTimeUnit = 0.1
+                ToolRadius = 19
+                TimeWindow = TimeWndLog / 74
+                CalibrationPoint1 = 20.44, 96
+                CalibrationPoint2 = 36.85, 96
+                CalibrationPoint3 = ...
+                ExtendTrends = yes / no
+                AutoFillFrom = 0 / Top
+                AutoFillTo = 0 / Bottom
+                AutoFillCaliper = 0 / Log Name
+                AutoFillStepSize = 1.0
+
+        Returns
+        -------
+        Log
+            A log giving the fluid velocity.
+        """
+        return Log(self._dispatch.CalculateFluidVelocity(log, prompt_user, config))
+
+    def centralize(self, log=None, prompt_user=None, config=None):
+        """Corrects travel time or multi-finger-caliper data for de-centralization effects
+        and outputs a new image log.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [Centralize]
+                ; UseRange : use clipping range
+                UseRange = yes / no
+                CaliperLow = 0
+                CaliperHigh = 0
+                OutputEccentricity = yes / no
+                OutputEccentricityDir = yes / no
+
+        Returns
+        -------
+        Log
+            A log with the data corrected for decentralization.
+        """
+        return Log(self._dispatch.Centralize(log, prompt_user, config))
+
+    def calculate_acoustic_caliper(self, log=None, prompt_user=None, config=None):
+        """Calculates borehole radius and caliper values from acoustic travel time measurements.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CalculateAcousticCaliper]
+                ; CaliperUnit : mm, cm, in
+                ; FluidVelocityUnit : m/s, km/s, m/ms, m/us, ft/s, ft/ms, ft/us, s/km, s/m, us/m, s/ft, us/ft
+                ; ToolRadius : in mm
+                TravelTimeUnit = 0.1
+                CaliperUnit = mm
+                ToolRadius = 19
+                TimeWindow = TimeWndLog / 74
+                FluidVelocity = VelocityLog / 1440
+                FluidVelocityUnit= m/s
+                CurveOutput = yes / no
+                ImageOutput  = yes / no
+        """
+        self._dispatch.CalculateAcousticCaliper(log, prompt_user, config)
+
+    def calculate_casing_thickness(self, log=None, prompt_user=None, config=None):
+        """Calculates thickness values for a casing pipe from acoustic thickness travel time measurements.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CalculateCasingThickness]
+                ; ThicknessUnit : mm, cm, in
+                ; SteelVelocityUnit : m/s, km/s, m/ms, m/us, ft/s, ft/ms, ft/us, s/km, s/m, us/m, s/ft, us/ft
+                ; CurveOutput : output min, max, average thickness
+                ; ImageOutput  : output the thickness as an image log
+                TravelTimeUnit = 0.01
+                SteelVelocity = VelocityLog / 5200
+                SteelVelocityUnit= m/s
+                CurveOutput = yes / no
+                ImageOutput = yes / no
+        """
+        self._dispatch.CalculateCasingThickness(log, prompt_user, config)
+
+    def cased_hole_ultrasonics(self, wavelet_log=None, zone_log=None, prompt_user=None, config=None):
+        """Processes ultrasonic waveforms from a wavelet log using the processing parameters from a zone log.
+
+        Parameters
+        ----------
+        wavelet_log : int or str, optional
+            Zero based index or title of the wavelet log to process.
+            If not provided, the process dialog box will be displayed.
+        zone_log : int or str, optional
+            Zero based index or title of the zone log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CasedHoleUltrasonics]
+                ; Thickness : output the thickness as an image log
+                ; Cadi  : output the cadi as an image log
+                ; Score  : output the score as an image log
+                Thickness = yes / no
+                Cadi = yes / no
+                Score = yes / no
+        """
+        self._dispatch.CasedHoleUltrasonics(wavelet_log, zone_log, prompt_user, config)
+
+    def calculate_apparent_metal_loss(self, log=None, prompt_user=None, config=None):
+        """Calculates an apparent metal loss value for each trace of radius values stored in an image log.
+
+        Note: This function is deprecated in WellCAD 5.7 and onwards. Please use calculate_apparent_metal_loss_ex instead.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CalculateApparentMetalLoss]
+                ; The units of the internal / external pipe radius values must be the same as the unit
+                ; of the radius values in the image log.
+                InternalPipeRadius = 1.9
+                ExternalPipeRadius = 2.2
+        Returns
+        -------
+        Log
+            A log giving the metal loss.
+        """
+        return Log(self._dispatch.CalculateApparentMetalLoss(log, prompt_user, config))
+
+    def calculate_apparent_metal_loss_ex(self, log=None, prompt_user=None, config=None):
+        """Calculates an apparent metal loss value for each trace of radius/thickness values stored in an
+        image log or well log.
+
+        Note: only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, either here or in the config, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [MetalLoss]
+                ; ID : name of a well log or img log
+                ; Thickness : name of a well log or img log
+                ; NomOD : name of a well log or value
+                ; NomThickness : name of a well log or value
+                ; NomODUnit, NomThicknessUnit : inch or mm, default to mm
+                ; DepthRange : Maximum, UserDefined, Zones, LogZones
+                ; ZonesDepthRange : top1, bot1, top2, bot2, ... topN, botN
+                ; LogZonesDepthRange = logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+                ID=
+                Thickness=
+                NomOD=50
+                NomODUnit=mm
+                NomThickness=10
+                NomThicknessUnit=mm
+                DepthRange=Maximum
+                TopDepth = 10
+                BottomDepth = 19
+                ZonesDepthRange=
+                LogZonesDepthRange = Litho,06,05#1
+        """
+        self._dispatch.CalculateApparentMetalLossEx(log, prompt_user, config)
+
+    def radius_to_from_diameter(self, log=None, prompt_user=None, config=None):
+        """Converts values data in an Image log from radius to diameter values or vice versa.
+
+        Parameters
+        ----------
+        log : int or str
+            Zero based index or title of the log to process.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RadiusToFromDiameter]
+                ;  Method : TwoTimesRadius, OppositeValues, HalfDiameter
+                Method = TwoTimesRadius
+        Returns
+        -------
+        Log
+            A log giving diameter/radius.
+        """
+        return Log(self._dispatch.RadiusToFromDiameter(log, prompt_user, config))
+
+    def outer_inner_radius_diameter(self, log=None, prompt_user=None, config=None):
+        """The process takes an Image, Well or Mud log as input and computes from radius/diameter
+        and thickness values an outer radius/diameter value.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [OuterInnerRadiusDiameter]
+                ; InputType : InnerRadius, OuterRadius, InnerDiameter, OuterDiameter
+                ; OutputType : InnerRadius, OuterRadius, InnerDiameter, OuterDiameter
+                ; Thickness = log name or value
+                Thickness = THK
+                InputType = InnerRadius
+                OutputType = OuterDiameter
+        Returns
+        -------
+        Log
+            A log giving the outer radius/diameter.
+        """
+        return Log(self._dispatch.OuterInnerRadiusDiameter(log, prompt_user, config))
+
+    def cased_hole_normalization(self, log=None, prompt_user=None, config=None):
+        """Subtracts the trace average, median, min, max or a custom value from all data points
+        of the same trace.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns ''None''.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CasedHoleNormalization]
+                ; Method : Mean, Median, Min, Max, Other
+                ; The Value parameter is used when the Method has been set to Other
+                ; Value : log name or constant numerical value
+                Method = Mean
+                Value = 10.5
+
+        Returns
+        -------
+        Log
+            The resulting log.
+        """
+        return Log(self._dispatch.CasedHoleNormalization(log, prompt_user, config))
+
+    def reverse_amplitude(self, log=None):
+        """Inverts the amplitudes in a FWS log.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, a dialog box displaying a list of available logs will be displayed.
+        """
+
+        self._dispatch.ReverseAmplitude(log)
+
+    def average_filter_fws_log(self, log=None, filter_width=None, filter_type=None):
+        """Applies a moving average filter to the traces of an FWS log.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.  If not provided, the process returns None.
+        filter_width : float, optional
+            Length of the filter window in us.  If not provided, default value will be used.
+        filter_type : int, optional
+            If not provided, default value will be used.
+            Type of the filter :
+
+                * 0 = moving average
+                * 1 = weighted average
+
+        Returns
+        -------
+        Log
+            The resulting log.
+        """
+
+        return Log(self._dispatch.AverageFilterFWSLog(log, filter_width, filter_type))
+
+    def freq_filter_fws_log(self, log, low_cut, low_pass, high_pass, high_cut):
+        """Applies a frequency filter to the traces of an FWS log.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.  If not provided, the process returns None.
+        low_cut : float
+            The low cut-off frequency of filter in kHz. If not provided, default value will be used.
+        low_pass : float
+            The low pass frequency of filter in kHz. If not provided, default value will be used.
+        high_pass : float
+            The high pass frequency of filter in kHz. If not provided, default value will be used.
+        high_cut : float
+            The high cut-off frequency of filter in kHz. If not provided, default value will be used.
+
+        Returns
+        -------
+        Log
+            Object of the filtered FWS log.
+        """
+
+        return Log(self._dispatch.FreqFilterFwsLog(log, low_cut, low_pass, high_pass, high_cut))
+
+    def apply_stand_off_correction(self, log=None, prompt_user=None, config=None):
+        """Corrects intercept times for the stand-off of tool and formation.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog settings will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ApplyStandOffCorrection]
+                ; LogUnit : s, ms, msec, us, usec, sec
+                ; ToolSpacingUnit, ToolDiameterUnit, HoleDiameterUnit : m, mm, inch, cm, ft
+                ; FluidVelocityUnit : us/ft, us/m, ft/us, m/s
+                ; VelocityUnit : us/ft, us/m, ft/us, m/s
+                ; HoleDiameter, FluidVelocity : log name or constant
+                LogUnit=us
+                ToolSpacing=0.6
+                ToolSpacingUnit=m ; m, mm, inch, cm, ft
+                ToolDiameter=50
+                ToolDiameterUnit=mm
+                HoleDiameter=100
+                HoleDiameterUnit=mm
+                FluidVelocity=1500
+                FluidVelocityUnit=m/s
+                VelocityUnit=m/s
+
+        Returns
+        -------
+        Log
+            The resulting log.
+        """
+
+        return Log(self._dispatch.ApplyStandOffCorrection(log, prompt_user, config))
+
+    def compensated_velocity(self, log=None, prompt_user=None, config=None):
+        """Slowness or velocity computed from two receiver arrival times.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log containing the travel times to the first receiver.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [FwsCompensatedVelocity]
+                ; RX1Log, RX2Log : log name
+                ; RX1LogUnit, RX2LogUnit : s, ms, msec, us, usec, sec
+                ; SpacingUnit : m, mm, inch, ft, cm
+                ; VelocityUnit : us/ft, us/m, ft/us, m/s
+                RX1Log =RX1 - dt
+                RX2Log = RX2 - dt
+                RX1LogUnit = us
+                RX2LogUnit = us
+                Spacing = 0.2
+                SpacingUnit = m
+                VelocityUnit =us/m
+
+        Returns
+        -------
+        Log
+            The resulting log.
+        """
+
+        return Log(self._dispatch.CompensatedVelocity(log, prompt_user, config))
+
+    def apply_semblance_processing(self, prompt_user=None, config=None):
+        """Performs a velocity analysis for the multiple receivers.
+
+        Parameters
+        ----------
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file.
+            The configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ApplySemblanceProcessing]
+                Rx1_Log = RX1
+                Rx1_Offset = 0.0
+                Rx1_TxDistance = 0.6
+                Rx1_Unit = m
+                Rx2_Log = RX2
+                Rx2_Offset = 0.0
+                Rx2_TxDistance = 0.8
+                Rx2_Unit = m
+                Rx3_Log= ...
+
+                [FwsVelocityAnalysis]
+                EnableFilter=false
+                FreqFilterLowPass=2.5 ; in kHz
+                FreqFilterLowPass=5.0
+                FreqFilterHighPass=30.0
+                FreqFilterHighCut=35.0
+                ToolDiameter=50.0
+                ToolDiameterUnit=mm ;mm, cm, inch
+                BoreholeDiameter=100.0
+                BoreholeDiameterUnit=mm ;mm, cm, inch
+                FluidSlowness=666.67
+                FluidSlownessUnit=us/m ; us/ft, us/m, ft/us, m/s, us/m
+
+        Returns
+        -------
+        Log
+            The log containing the semblance results.
+        """
+
+        return Log(self._dispatch.ApplySemblanceProcessing(prompt_user, config))
+
+    def process_reflected_tube_wave(self, log=None, prompt_user=None, config=None):
+        """Extracts the cumulative energy from reflected tube wave arrivals.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog settings will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ProcessReflectedTubeWave]
+                ; Side : both,  upper, lower
+                Side = both
+                Offset = 25.0 'measured in us
+                Blanking = 50.0 'measured in us
+                FluidSlowness = 696.0 'measured in us/m
+                TxFrequency = 15000.0 'measured in Hz
+
+        Returns
+        -------
+        Log
+            The resulting log containing the cumulative energy.
+        """
+
+        return Log(self._dispatch.ProcessReflectedTubeWave(log, prompt_user, config))
+
+    def pick_first_arrival(self, log=None, prompt_user=None, config=None):
+        """Picks the first arrival time using the standard threshold or advanced method.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.  If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file.
+            The configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [FwsFirstArrival]
+                ;Method=Standard Threshold Pickup Algorithm
+                Method=Advanced Threshold Pickup Algorithm
+
+                [Standard Threshold Pickup Algorithm]
+                Blanking=100.0
+                Threshold=15.0
+                BackInterpolation=yes
+                LockToSampling=yes
+                ; the next two are advanced settings
+                BaseLine=0.0
+                AutoAdjustThreshold=no
+
+                [Advanced Threshold Pickup Algorithm]
+                Blanking=0.0
+                Threshold=3.0
+                LargeWidth=120.0
+                SmallWidth=40.0
+
+        Returns
+        -------
+        Log
+            The resulting log containing the first arrival times.
+        """
+
+        return Log(self._dispatch.PickFirstArrival(log, prompt_user, config))
+
+    def cement_bond(self, log=None, prompt_user=None, config=None):
+        """Determines the cement bond based on the Standard Gate Method.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [CementBondProcess]
+                ; Logs : comma-separated FWS log names of the receivers to be processed
+                Logs=WVFS1,WVFS2,WVFS3
+                AreRadiiSectors=no
+                EnableT0Gate=yes
+                EnableTXGate=no
+                T0GateStart=237.4
+                T0GateLength=40
+                TXGateBlanking=0
+                TXGateThreshold=15
+                EnableCalibration=no
+                BLGateStart=50
+                BLGateLength=25
+                FreePipeTargetAmplitude=100
+                FreePipeTargetAmplitudeUnits=mV
+                FreePipeTopDepth=0
+                FreePipeBotDepth=0
+        """
+
+        self._dispatch.CementBond(log, prompt_user, config)
+
+    def pick_e1_arrival(self, fws_log=None, dt_log=None, prompt_user=None, config=None):
+        """Determines the arrival time of the E1 amplitude.
+
+        Parameters
+        ----------
+        fws_log : int or str, optional
+            Zero based index or title of the FWS log to process.
+            If not provided, the process dialog box will be displayed.
+        dt_log : int or str, optional
+            Zero based index or title of the arrival time log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [PickE1Arrival]
+                PickPositivPolarity = yes
+                FilterWidth = 5
+
+        Returns
+        -------
+        Log
+            The resulting log containing the E1 arrival times.
+        """
+
+        return Log(self._dispatch.PickE1Arrival(fws_log, dt_log, prompt_user, config))
+
+    def extract_e1_amplitude(self, fws_log=None, arrival_log=None, prompt_user=None):
+        """Uses the E1 arrival time to extract the E1 amplitude.
+
+        Parameters
+        ----------
+        fws_log : int or str, optional
+            Zero based index or title of the log to process.
+        arrival_log : int, str or float, optional
+            int, str : Zero based index or title of the log containing the first E1 arrival times.
+            float : constant E1 arrival time
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+
+        Returns
+        -------
+        Log
+            The resulting log containing the E1 amplitude.
+        """
+
+        return Log(self._dispatch.ExtractE1Amplitude(fws_log, arrival_log, prompt_user))
+
+    def adjust_pick_to_extremum(self, fws_log=None, arrival_log=None, prompt_user=None, config=None):
+        """Adjusts the pick given in arrival_log to the next maximum or minimum amplitude in fws_log.
+
+        Parameters
+        ----------
+        fws_log : int or str, optional
+            Zero based index or title of the fws log.
+            If not provided, the process dialog box will be displayed.
+        arrival_log : int or str, optional
+            Zero based index or title of the arrival time log.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [AdjustPickToExtremum]
+                PickPositivPolarity = yes
+                FilterWidth = 5
+
+        Returns
+        -------
+        Log
+            Object of the log containing the pick times shifted to the nearest amplitude extremum.
+        """
+
+        return Log(self._dispatch.AdjustPickToExtremum(fws_log, arrival_log, prompt_user, config))
+
+    def extract_window_peak_amplitude(self, log=None, prompt_user=None, config=None):
+        """Extracts the maximum amplitude found in a time window of a FWS log trace.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [ExtractWindowPeakAmplitude]
+                ; WindowStart : value or log name, units : us
+                ; WindowLength : value, units : us
+                ; PickType : 0 = peak, 1 = max, 2 = average
+                WindowStart=0
+                WindowLength=15
+                PickMax=yes
+                PickPos=yes
+                PickType=1
+                EnableResampling=yes
+
+        Returns
+        -------
+        Log
+            The resulting log containing the amplitude.
+        """
+
+        return Log(self._dispatch.ExtractWindowPeakAmplitude(log, prompt_user, config))
+
+    def calculate_mechanical_properties(self, p_slowness=None, s_slowness=None, density=None):
+        """Computes a set of rock mechanical parameters from the input data.
+
+        Parameters
+        ----------
+        p_slowness : int or str, optional
+            Zero based index or title of the log containing the p-slowness data.
+            If not provided, the process dialog box will be displayed.
+        s_slowness : int or str, optional
+            Zero based index or title of the log containing the s-slowness data.
+            If not provided, the process dialog box will be displayed.
+        density :int or str, optional
+            Zero based index or title of the log containing the density data.
+        """
+
+        self._dispatch.CalculateMechanicalProperties(p_slowness, s_slowness, density)
+
+    def integrated_travel_time(self, log=None, prompt_user=None, config=None):
+        """Computes the integrated travel time from slowness or velocity data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [IntegratedTravelTime]
+                TimeOffset = 0 'in us
+                TWT = Yes/No
+
+        Returns
+        -------
+        Log
+            The resulting log containing the integrated times.
+        """
+
+        return Log(self._dispatch.IntegratedTravelTime(log, prompt_user, config))
+
+    def bond_index(self, log=None, prompt_user=None, config=None):
+        """Computes the bond index of the cement behind the casing.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [FwsBondIndex]
+                CementAmplitude = 2 'in mV
+                FreePipeAmplitude = 62.2 'in mV
+
+        Returns
+        -------
+        Log
+            The resulting log containing the bond index.
+        """
+
+        return Log(self._dispatch.BondIndex(log, prompt_user, config))
+
+    def compressive_strength(self, log=None, prompt_user=None, config=None):
+        """Computes the compressive strength of the cement behind a casing.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.  A cement bond amplitude log (Well or Mud log type)
+            or amplitude map (Image log) can be used.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [FwsCompressiveStrength]
+                CasingOD = 7 ' in inch
+                CasingWeight = 23 ' in lbs/ft
+
+        Returns
+        -------
+        Log
+            The resulting log containing the compressive strength.
+        """
+
+        return Log(self._dispatch.CompressiveStrength(log, prompt_user, config))
+
+    def apply_natural_gamma_borehole_correction(self, log=None, prompt_user=None, config=None):
+        """Applies borehole corrections to FWS and Well logs
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [BoreholeConditionCorrections]
+                DeadTime = 7.2 ' in us
+                EnableDeadTime = yes
+                EnableFactors = yes
+                FactorName1 = Water Factor
+                FactorName2 = Pipe Factor
+                Top1 = 0.0
+                Bot1 = 2.85
+                Factor1-1 = 1
+                Factor1-2 = 1.49
+                Top2 = 2.85
+                Bot2 = bot
+                Factor2-1 = 1.12
+                Factor2-2 = 1
+
+        Returns
+        -------
+        Log
+            A log containing the corrected count rates.
+        """
+
+        return Log(self._dispatch.ApplyNaturalGammaBoreholeCorrection(log, prompt_user, config))
+
+    def apply_total_gamma_calibration(self, log=None, prompt_user=None, config=None):
+        """Applies a calibration factor or equation to the values in the specified Well Log.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [BoreholeConditionCorrections]
+                K-Factor=2*0.00001028
+
+        Returns
+        -------
+        Log
+            A log containing the modified gamma values.
+        """
+
+        return Log(self._dispatch.ApplyTotalGammaCalibration(log, prompt_user, config))
+
+    def calculate_spectrum_total_count(self, log=None, prompt_user=None, config=None):
+        """Extracts the total count, min, max, average or median from each spectrum trace of the specified log
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [SpectralGamma_Statistic]
+                ; WinLow, WinHigh expressed in channel number or keV according to Channel
+                Total = yes
+                Min = yes
+                Max = yes
+                Ave = yes
+                Median = yes
+                UseWindow = yes
+                Channel = yes
+                WinLow = 410
+                WinHigh = 2850
+        """
+
+        self._dispatch.CalculateSpectrumTotalCount(log, prompt_user, config)
+
+    def spectrometric_ratios(self, log_a=None, log_b=None, log_c=None, prompt_user=None, config=None):
+        """Computes spectrometric ratios like U/Th or U/k
+
+        By default, the ratios log_b/log_a, log_b/log_c and log_c/log_a
+        will be computed.
+
+        Parameters
+        ----------
+        log_a : int or str, optional
+            Zero based index or title of the log to process.
+        log_b : int or str, optional
+            Zero based index or title of the log to process.
+        log_c : int or str, optional
+            Zero based index or title of the log to process.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [SpectrometricRatios]
+                ; ratio : A / B
+                A=K
+                B=U
+        """
+
+        self._dispatch.SpectrometricRatios(log_a, log_b, log_c, prompt_user, config)
+
+    def process_medusa_spectrum_data(self, log_spectrum=None, log_time=None, prompt_user=None, config=None):
+        """Performs a full spectrum analysis using a calibration after Medusa
+
+        Parameters
+        ----------
+        log_spectrum : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        log_time : int or str, optional
+            Zero based index or title of the log with the live time data.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [SpectralGammaMedusaProcess]
+                CalibrationFilePath = C:\\Temp\\NSG1234.mcf
+                EnableFittedSpectrum = yes
+                EnableConcentrationErrors = yes
+                EnableStabilizationFactor = yes
+                DeadTime = 5 (in us/pulse)
+                HoleDiameter = 96 / Caliper (fixed value or data from log in mm)
+                CasingThickness = 8 / Thickness (fixed value or data from log mm)
+                CasingType = 0 (Steel) / 1 (PVC)
+                FluidDensity = 1.1 / RHOFL (fixed value or data from log in g/ccm)
+                FluidK = 0.0 / K (Potassium concentration in the fluid; fixed value or data from log in Bq/kg)
+                FluidU = 0.0 / U (eq Uranium concentration in the fluid; fixed value or data from log in Bq/kg)
+                FluidTh = 0.0 / Th (Thorium concentration in the fluid; fixed value or data from log in Bq/kg)
+                ToolPosition = 0 (Alongside) / 1 (Centered)
+                """
+        self._dispatch.ProcessMedusaSpectrumData(log_spectrum, log_time, prompt_user, config)
+
+    def process_spectrum_data(self, log=None, prompt_user=None, config=None):
+        """Performs a windows stripping based on a calibration model
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [SpectralGamma]
+                OutputWindowCounts = yes / no
+                ProcessModel = "C:\Temp\Test.sgm"
+        """
+
+        self._dispatch.ProcessSpectrumData(log, prompt_user, config)
+
+    def compute_gr(self, log_k=None, log_u=None, log_th=None, prompt_user=None, config=None):
+        """Computes total gamma ray from K, U and Th isotope concentrations using the MEDUSA
+        calibration file.
+
+        Parameters
+        ----------
+        log_k : int or str, optional
+            Zero based index or title of the log containing the concentrations of K.
+        log_u : int or str, optional
+            Zero based index or title of the log containing the concentrations of U.
+        log_th : int or str, optional
+            Zero based index or title of the log containing the concentrations of Th.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [SpectralGammaMedusaCGR]
+                CalibrationFilePath=C:\Tools\Calibrations\QL40-SGR-154904.mcf
+
+        Returns
+        -------
+        Log
+            A log containing the gamma ray values.
+        """
+
+        return Log(self._dispatch.ComputeGR(log_k, log_u, log_th, prompt_user, config))
+
+    def process_nmrsa_data(self, log=None, prompt_user=None, config=None):
+        """Performs a post-processing of NMRSA's BMR tool raw data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path and name of the configuration file or a parameter string.  The configuration file or
+            string can contain the following options:
+
+            .. code-block:: ini
+
+                [NMRSA]
+                UseDefaultOutputs = yes / no
+                MasterCalibrationFile=
+                ProcessingConfigurationFile=
+                DepthRange=Maximum / UserDefined / Zones /LogZones
+                TopDepth=20
+                BottomDepth=22
+                LogZones : top1, bot1, top2, bot2, ... topN, botN
+                LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+        """
+
+        self._dispatch.ProcessNMRSAData(log, prompt_user, config)
+
+    def nmr_total_porosity(self, log=None, prompt_user=None, config=None):
+        """Computes the total porosity from a T2 distribution.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path and name of the configuration file or a parameter string.  The configuration file
+            or string can contain the following options:
+
+            .. code-block:: ini
+
+                [NMRTotalPorosity]
+                MaxCutoffValue=-1
+                UseTimeMaxCutoff= yes / no
+
+                DepthRange=Maximum / UserDefined / Zones /LogZones
+                TopDepth=20
+                BottomDepth=22
+                LogZones : top1, bot1, top2, bot2, ... topN, botN
+                LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+
+        Returns
+        -------
+        Log
+            The resulting log object
+        """
+
+        return Log(self._dispatch.NMRTotalPorosity(log, prompt_user, config))
+
+    def nmr_permeability(self, log=None, prompt_user=None, config=None):
+        """Computes the permeability from a T2 distribution.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path and name of the configuration file or a parameter string.  The configuration file
+            or string can contain the following options:
+
+            .. code-block:: ini
+
+            [NMRPermeability]
+            T2DistributionTraceUnit= seconds / milliseconds
+            UseTimeMaxCutoff= yes / no
+            MaxCutoffValue=-1
+            DisplayTIMModel= yes / no
+            VariableCforTIMModel=1
+            ExponentMforTIMModel=4
+            BFVCutoffForTIMModel=2
+            BFVCutoffForTIMModel=0.3
+            UseTimeMaxForFFVCutoff= yes / no
+            FFVCutoffForTIMModel=0
+            DisplaySDRModel= yes / no
+            VariableCforSDRModel=4
+            ExponentMforSDRModel=4
+            ExponentNforSDRModel=2
+            DisplayT2LogMean= yes / no
+            DepthRange=Maximum / UserDefined / Zones /LogZones
+            TopDepth=20
+            BottomDepth=22
+            LogZones : top1, bot1, top2, bot2, ... topN, botN
+            LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+        """
+
+        self._dispatch.NMRPermeability(log, prompt_user, config)
+
+    def nmr_fluid_volumes(self, log=None, prompt_user=None, config=None):
+        """Computes the fluid volumes from a T2 distribution.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log to process.
+            If not provided, the process dialog box will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path and name of the configuration file or a parameter string.  The configuration file
+            or string can contain the following options:
+
+            .. code-block:: ini
+
+            [NMRFluidVolumes]
+            LithoDatabase=
+            UseLithoDatabaseAssociatedColor= yes/no
+            Components=
+            Cutoff=
+            DepthRange=Maximum / UserDefined / Zones /LogZones
+            TopDepth=20
+            BottomDepth=22
+            LogZones : top1, bot1, top2, bot2, ... topN, botN
+            LogZonesDepthRange=logname, depthsectionName1, depthsectionName2, ....depthsectionname3
+
+        Returns
+        -------
+        Log
+            The resulting log object
+        """
+
+        return Log(self._dispatch.NMRFluidVolumes(log, prompt_user, config))
+
+    def water_salinity(self, log=None, prompt_user=None, config=None):
+        """Salinity estimation from fluid conductivity.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the fluid conductivity log to process.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [WaterSalinity]
+                Temperature = log name or constant value
+                TemperatureUnit = degC / degF / degK
+
+        Returns
+        -------
+        Log
+            A log of the resulting salinity.
+        """
+
+        return Log(self._dispatch.WaterSalinity(log, prompt_user, config))
+
+    def water_resistivity(self, log=None, prompt_user=None, config=None):
+        """Temperature correction for fluid conductivity or resistivity.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log containing the conductivity or resistivity values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+             .. code-block:: ini
+
+                [WaterResistivity]
+                Temperature = log name or constant value
+                TemperatureUnit = degC / degF / degK
+                RefTemperature = log name or constant value
+                RefTemperatureUnit = degC / degF / degK
+                Method = 0 (Arp) / 1 (Hilchie)
+
+        Returns
+        -------
+        Log
+            A log of the corrected conductivity or resistivity.
+        """
+
+        return Log(self._dispatch.WaterResistivity(log, prompt_user, config))
+
+    def shale_volume(self, log=None, prompt_user=None, config=None):
+        """Estimates the shale volume from Gamma Ray or SP data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the well or mud log containing the Gamma Ray or SP values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+             .. code-block:: ini
+
+                [ShaleVolume]
+                Equation = 0
+                ; 0 = Linear (default), 1 = Larionov (Tertiary), 2 = Steiber,
+                ; 3 = Clavier, 4 = Larionov (older rocks)
+                Shale=150
+                ShaleValueType=1
+                ; ...Type: 0 = value, 1 = minmax, 2 = avginterval
+                ShaleTopDepth=0
+                ShaleBotDepth=0
+                Sandstone=75
+                SandstoneValueType=1
+                ; ...Type: 0 = value, 1 = minmax, 2 = avginterval
+                SandstoneTopDepth=0
+                SandstoneBotDepth=0
+
+        Returns
+        -------
+        Log
+            A log of the resulting shale volume.
+        """
+
+        return Log(self._dispatch.ShaleVolume(log, prompt_user, config))
+
+    def porosity_sonic(self, log=None, prompt_user=None, config=None):
+        """Computes porosity from transit time data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the well or mud log containing the formation resistivity (Rt) values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [PorositySonic]
+                ; Method : 0 = Wylie, 1 = WylieCompaction, 2 = AbbreviatedRaymerHunt, 3 = RaymerHunt
+                ; Slowness units: us/ft, us/m, ft/us, m/s
+                Method = 1
+                MatrixSlowness = log name or constant value
+                MatrixSlownessUnit = us/ft
+                FluidSlowness= = log name or constant value
+                FluidSlownessUnit = us/ft
+                Compaction= = log name or constant value
+                C = 0.67
+
+        Returns
+        -------
+        Log
+            A log of the resulting porosity.
+        """
+
+        return Log(self._dispatch.PorositySonic(log, prompt_user, config))
+
+    def porosity_archie(self, log=None, prompt_user=None, config=None):
+        """Computes porosity from formation resistivity data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the well or mud log containing the formation resistivity (Rt) values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [PorosityArchie]
+                ; Method : 0 = Standard, 1 = FreshWater, 2 = shale, 3= shaleAndFreshWater
+                ; Rw and Rsh units: ohm.m, ohm.ft
+                Method = 1
+                Vsh = log name or constant value
+                Rw = log name or constant value
+                RwUnit=ohm.m
+                Rsh = 30.0
+                RshUnit=ohm.m
+                CementationFactor = 1.0
+                CementationExponent = 2.0
+                Cs = 1.0
+
+        Returns
+        -------
+        Log
+            A log of the resulting porosity.
+        """
+
+        return Log(self._dispatch.PorosityArchie(log, prompt_user, config))
+
+    def porosity_density(self, log=None, prompt_user=None, config=None):
+        """Computes porosity from density data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the well or mud log containing the  density values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [PorosityDensity]
+                ; Method : 0 = Standard, 1 = Shale
+                ; MatrixDensity, FluidDensity, ShaleVolume : value or log
+                ; Density units: g/cc or kg/m3
+                MatrixDensity=2.7
+                MatrixDensityUnit=g/cc
+                FluidDensity=1.0
+                FluidDensityUnit=g/cc
+                ShaleVolume=0
+                ShaleDensity=1.5
+                ShaleDensityUnit=g/cc
+
+        Returns
+        -------
+        Log
+            A log of the resulting porosity.
+        """
+
+        return Log(self._dispatch.PorosityDensity(log, prompt_user, config))
+
+    def porosity_neutron(self, log=None, prompt_user=None, config=None):
+        """Applies a shale correction to neutron porosity data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the well or mud log containing the neutron porosity values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [PorosityNeutron]
+                ; Vsh : log name
+                ; ShaleNPhi = value
+                Vsh=VSh
+                ShaleNPhi=50
+
+        Returns
+        -------
+        Log
+            A log of the resulting corrected porosity.
+        """
+
+        return Log(self._dispatch.PorosityNeutron(log, prompt_user, config))
+
+    def permeability(self, log=None, prompt_user=None, config=None):
+        """Estimates permeability from porosity data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the well or mud log containing the neutron porosity values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [Permeability]
+                CementationFactor=1.0
+
+        Returns
+        -------
+        Log
+            A log of the resulting permeability.
+        """
+
+        return Log(self._dispatch.Permeability(log, prompt_user, config))
+
+    def hydraulic_conductivity(self, log=None, prompt_user=None, config=None):
+        """Computes the hydraulic conductivity from permeability data.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the well or mud log containing the permeability values.
+            If not provided, the process returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [HydraulicConductivity]
+                ; Density, Viscosity, DensityTemperature, ViscosityTemperature : log name or value
+                ; Temperature units : degC, degF, degK
+                ; Permeability units : m2, Darcy, mD, sq.ft
+                ; Density units : kg/m3, g/m3, g/cc, lb/in3, lb/ft3
+                ; Viscosity units : Pa.s, cP, p, dyn.s/cm2
+                Density=1000
+                DensityUnit= kg/m3
+                Viscosity=0.000890439
+                ViscosityUnit=Pa.s
+                DensityTemperature=25
+                DensityTemperatureUnit=degC
+                ViscosityTemperature=25
+                ViscosityTemperatureUnit=degC
+
+        Returns
+        -------
+        Log
+            A Log object of the resulting hydraulic conductivity.
+        """
+
+        return Log(self._dispatch.HydraulicConductivity(log, prompt_user, config))
+
+    def extract_grain_size_statistics(self, log=None, prompt_user=None, config=None):
+        """Computes statistics from a grain size distribution curve.
+
+        Parameters
+        ----------
+        log : int or str, optional
+            Zero based index or title of the log containing the grain size values.
+            If not provided, a dialog box displaying a list of available logs will be displayed.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+             .. code-block:: ini
+
+                [GrainSizeStatistics]
+                ; Method : 0 = Logarithmic (original Folk and Ward; default),
+                ; 1 = Geometric (modified Folk and Ward),
+                ; 2 = Logarithmic method of moments,
+                ; 3= Geometric method of moments
+                Mean = yes
+                Median = yes
+                Sorting = yes
+                Skewness = yes
+                Kurtosis = yes
+                Histo = yes
+        """
+
+        self._dispatch.ExtractGrainSizeStatistics(log, prompt_user, config)
+
+    def grain_size_sorting(self, log_min, log_max, prompt_user=None, config=None):
+        """Classifies grain size values based on min and max logs.
+
+        Parameters
+        ----------
+        log_min : int or str, optional
+            Zero based index or title of the log containing logged minimum grain size value.
+            If not provided, the method returns None.
+        log_max : int or str, optional
+            Zero based index or title of the log containing logged maximum grain size value.
+            If not provided, the method returns None.
+        prompt_user : bool, optional
+            Whether dialog boxes are displayed to interact with the user.
+            If set to ``False`` the processing parameters will be retrieved from the specified
+            configuration.  If no configuration has been specified, default values will be used.
+            Default is True.
+        config : bool, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+             .. code-block:: ini
+
+                [GrainSizeSorting]
+                ; Method : 0 = Logarithmic (original Folk and Ward; default),
+                ; 1 = Geometric (modified Folk and Ward),
+                ; 2 = Logarithmic method of moments,
+                ; 3= Geometric method of moments
+                BlockedAverage = yes
+
+        Returns
+        -------
+        Log
+            A log containing the sorted values
+        """
+
+        return Log(self._dispatch.GrainSizeSorting(log_min, log_max, prompt_user, config))
+
+    def enable_protection(self, enable, password):
+        """Changes the protection status of a document using a password
+
+        Parameters
+        ----------
+        enable : bool
+            Set to True to protect the borehole document.
+        password : str
+            The password used to allow this option.
+        """
+
+        self._dispatch.EnableProtection(enable, password)
+
+    def allow_insert_log(self, enable, password):
+        """Changes the protection status for inserting new logs.
+
+        Parameters
+        ----------
+        enable : bool
+            Set to True to allow adding new logs to the borehole document.
+        password : str
+            The password used to allow this option.
+        """
+
+        self._dispatch.AllowInsertLog(enable, password)
+
+    def allow_save_template(self, enable, password):
+        """Changes the protection status for saving layout templates.
+
+        Parameters
+        ----------
+        enable : bool
+            Set to True to allow saving layout templates of the borehole document.
+        password : str
+            The password used to allow this option.
+        """
+
+        self._dispatch.AllowSaveTemplate(enable, password)
+
+    def allow_export_file(self, enable, password):
+        """Changes the protection status for exporting data.
+
+        Parameters
+        ----------
+        enable : bool
+            Set to True to allow the export of data from the borehole document.
+        password : str
+            The password used to allow this option.
+        """
+
+        self._dispatch.AllowExportFile(enable, password)
+
+    def allow_modify_annotation(self, enable, password):
+        """Changes the protection status to modify annotations.
+
+        Parameters
+        ----------
+        enable : bool
+            Set to True to allow editing existing annotations in the borehole document.
+        password : str
+            The password used to allow this option.
+        """
+
+        self._dispatch.AllowModifyAnnotation(enable, password)
+
+    def allow_insert_annotation(self, enable, password):
+        """Changes the protection status for inserting annotations.
+
+        Parameters
+        ----------
+        enable : bool
+            Set to True to allow adding new annotations in the borehole document.
+        password : str
+            The password used to allow this option.
+        """
+
+        self._dispatch.AllowInsertAnnotation(enable, password)
+
+    def allow_modify_headers_content(self, enable, password):
+        """Changes the protection status of the header content.
+
+        Parameters
+        ----------
+        enable : bool
+            Set to True to allow edition of the document header data.
+        password : str
+            The password used to allow this option.
+        """
+
+        self._dispatch.AllowModifyHeadersContent(enable, password)
+
+    def set_metadata(self, id, value):
+        """Sets a metadata value. If the id doesn't exist, this will create it and set the value.
+        Only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        id : str
+            The metadata id.
+        value : str
+            The value to set the metadata to.
+        """
+
+        self._dispatch.SetMetadata(id, value)
+
+    def get_metadata(self, id):
+        """Gets the value metadata value.
+        Only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        id : str
+            The metadata id.
+
+        Returns
+        -------
+        str
+            The value associated with the metadata.
+        """
+
+        return self._dispatch.GetMetadata(id)
+
+    def delete_metadata(self, id):
+        """Removes a metadata id and value pair.
+        Warning: if this metadata is used within a header, the metadata id will remain valid and it's value will be set to null.
+        Only compatible with WellCAD version 5.7 and onwards.
+
+        Parameters
+        ----------
+        id : str
+            The metadata id.
+        """
+
+        self._dispatch.DeleteMetadata(id)
```

### Comparing `pywellcad-0.2.0/wellcad/com/_comment_box.py` & `pywellcad-0.2.1/wellcad/com/_comment_box.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class CommentBox(DispatchWrapper):
-    @property
-    def top_depth(self):
-        """float: The top depth of the comment box in current depth
-        units."""
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of the comment box in current depth
-        units."""
-        return self._dispatch.BottomDepth
-
-    @property
-    def text(self):
-        """str: The text of the comment box."""
-        return self._dispatch.Text
-
-    @text.setter
-    def text(self, value):
-        self._dispatch.Text = value
-
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class CommentBox(DispatchWrapper):
+    @property
+    def top_depth(self):
+        """float: The top depth of the comment box in current depth
+        units."""
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of the comment box in current depth
+        units."""
+        return self._dispatch.BottomDepth
+
+    @property
+    def text(self):
+        """str: The text of the comment box."""
+        return self._dispatch.Text
+
+    @text.setter
+    def text(self, value):
+        self._dispatch.Text = value
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_cross_section_box.py` & `pywellcad-0.2.1/wellcad/com/_cross_section_box.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class CrossSectionBox(DispatchWrapper):
-    """ Stores a depth interval over which a cross section from an image log is created.
-
-    CrossSection boxes are part of a CrossSection Log and stores a depth interval.
-    Top and bottom depths of the intervals can be the same.
-
-    Example
-    -------
-    >>> cross_log = borehole.log("Test")
-    >>> cross_box = cross_log.insert_new_cross_box(10.5, 12.5)
-    >>> data.top_depth
-    10.5
-    >>> data.top_depth
-    12.5
-    """
-
-    @property
-    def top_depth(self):
-        """float : The top depth of the box in current
-        depth reference units."""
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float : The bottom depth of the box in current
-        depth reference units."""
-        return self._dispatch.BottomDepth
-
-
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class CrossSectionBox(DispatchWrapper):
+    """ Stores a depth interval over which a cross section from an image log is created.
+
+    CrossSection boxes are part of a CrossSection Log and stores a depth interval.
+    Top and bottom depths of the intervals can be the same.
+
+    Example
+    -------
+    >>> cross_log = borehole.log("Test")
+    >>> cross_box = cross_log.insert_new_cross_box(10.5, 12.5)
+    >>> data.top_depth
+    10.5
+    >>> data.top_depth
+    12.5
+    """
+
+    @property
+    def top_depth(self):
+        """float : The top depth of the box in current
+        depth reference units."""
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float : The bottom depth of the box in current
+        depth reference units."""
+        return self._dispatch.BottomDepth
+
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_depth.py` & `pywellcad-0.2.1/wellcad/com/_depth.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class Depth(DispatchWrapper):
-    """ The reference/master vertical axis. Can be in depth or time.
-
-    Depth objects allow setting properties for the master depth axis
-    such as scale, unit, decimals, ….
-
-    Example
-    -------
-    >>> import wellcad.com
-    >>> app = wellcad.com.Application()
-    >>> app.new_borehole()
-    <wellcad.com._borehole.Borehole object at 0x0000018B3DAF9D30>
-    >>> borehole = app.get_active_borehole()
-    >>> depth = borehole.depth
-    """
-
-    @property
-    def decimals(self):
-        """int: the number of decimals displayed in the depth string of the master depth axis."""
-        return self._dispatch.Decimals
-
-    @decimals.setter
-    def decimals(self, decimals):
-        self._dispatch.Decimals = decimals
-
-    @property
-    def horizontal_grid_spacing(self):
-        """float: The depth grid spacing for the master depth axis"""
-        return self._dispatch.HorizontalGridSpacing
-
-    @horizontal_grid_spacing.setter
-    def horizontal_grid_spacing(self, grid_spacing):
-        self._dispatch.HorizontalGridSpacing = grid_spacing
-
-    @property
-    def scale(self):
-        """float: The depth scale used for the master depth axis.
-        
-        The resulting scale is 1:``scale``.
-        
-        Example
-        -------
-        >>> depth.scale = 100 # Scale is 1:100
-        """
-        return self._dispatch.Scale
-
-    @scale.setter
-    def scale(self, scale):
-        self._dispatch.Scale = scale
-
-    @property
-    def used_as_depth_scale(self):
-        """bool: Whether this depth scale is used as the current reference axis.
-
-        Setting this property to True on another depth log changes
-        the property to False on this object. If no other depth log
-        is used as the depth scale, the main depth log will
-        automatically be used as the depth scale."""
-        return self._dispatch.UsedAsDepthScale
-
-    @used_as_depth_scale.setter
-    def used_as_depth_scale(self, enable):
-        self._dispatch.UsedAsDepthScale = enable
-
-    @property
-    def horizontal_grid(self):
-        """int: The depth grid type.
-
-        The available types are the following:
-
-        * 0 = none
-        * 1 = major grid lines only
-        * 2 = major & minor grid lines
-        """
-        return self._dispatch.HorizontalGrid
-
-    @horizontal_grid.setter
-    def horizontal_grid(self, grid_type):
-        self._dispatch.HorizontalGrid = grid_type
-
-    @property
-    def left_position(self):
-        """float: The position of the left side of the master depth column as a
-        fraction of the document width.
-        
-        In the case that this is set to be a value higher than
-        ``right_position``, the two attributes will swap. Values will be
-        clamped in the range [0.0, 1.0].
-        """
-        return self._dispatch.LeftPosition
-
-    @left_position.setter
-    def left_position(self, left_pos):
-        self._dispatch.LeftPosition = left_pos
-
-    @property
-    def right_position(self):
-        """float: The position of the right side of the master depth column as
-        a fraction of the document width.
-        
-        In the case that this is set to be a value lower than
-        ``left_position``, the two attributes will swap. Values will be
-        clamped in the range [0.0, 1.0].
-        """
-        return self._dispatch.RightPosition
-
-    @right_position.setter
-    def right_position(self, right_pos):
-        self._dispatch.RightPosition = right_pos
-
-    @property
-    def unit(self):
-        """int: The depth unit
-
-        The available units are the following:
-
-        * 0 = meter
-        * 1 = feet
-        """
-        return self._dispatch.Unit
-
-    @unit.setter
-    def unit(self, unit):
-        self._dispatch.Unit = unit
-
-    def set_position(self, left, right):
-        """Sets the position and width of the master depth column.
-
-        Values given outside the range of [0.0, 1.0] will be clamped. If
-        ``left`` > ``right``, the arguments are swapped.
-
-        Parameters
-        ----------
-        left : float
-            The position of the left side of the depth column as a fraction of
-            the document width.
-
-        right : float
-            The position of the right side of the depth column as a fraction of
-            the document width.
-        """
-        self._dispatch.SetPosition(left, right)
-
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class Depth(DispatchWrapper):
+    """ The reference/master vertical axis. Can be in depth or time.
+
+    Depth objects allow setting properties for the master depth axis
+    such as scale, unit, decimals, ….
+
+    Example
+    -------
+    >>> import wellcad.com
+    >>> app = wellcad.com.Application()
+    >>> app.new_borehole()
+    <wellcad.com._borehole.Borehole object at 0x0000018B3DAF9D30>
+    >>> borehole = app.get_active_borehole()
+    >>> depth = borehole.depth
+    """
+
+    @property
+    def decimals(self):
+        """int: the number of decimals displayed in the depth string of the master depth axis."""
+        return self._dispatch.Decimals
+
+    @decimals.setter
+    def decimals(self, decimals):
+        self._dispatch.Decimals = decimals
+
+    @property
+    def horizontal_grid_spacing(self):
+        """float: The depth grid spacing for the master depth axis"""
+        return self._dispatch.HorizontalGridSpacing
+
+    @horizontal_grid_spacing.setter
+    def horizontal_grid_spacing(self, grid_spacing):
+        self._dispatch.HorizontalGridSpacing = grid_spacing
+
+    @property
+    def scale(self):
+        """float: The depth scale used for the master depth axis.
+        
+        The resulting scale is 1:``scale``.
+        
+        Example
+        -------
+        >>> depth.scale = 100 # Scale is 1:100
+        """
+        return self._dispatch.Scale
+
+    @scale.setter
+    def scale(self, scale):
+        self._dispatch.Scale = scale
+
+    @property
+    def used_as_depth_scale(self):
+        """bool: Whether this depth scale is used as the current reference axis.
+
+        Setting this property to True on another depth log changes
+        the property to False on this object. If no other depth log
+        is used as the depth scale, the main depth log will
+        automatically be used as the depth scale."""
+        return self._dispatch.UsedAsDepthScale
+
+    @used_as_depth_scale.setter
+    def used_as_depth_scale(self, enable):
+        self._dispatch.UsedAsDepthScale = enable
+
+    @property
+    def horizontal_grid(self):
+        """int: The depth grid type.
+
+        The available types are the following:
+
+        * 0 = none
+        * 1 = major grid lines only
+        * 2 = major & minor grid lines
+        """
+        return self._dispatch.HorizontalGrid
+
+    @horizontal_grid.setter
+    def horizontal_grid(self, grid_type):
+        self._dispatch.HorizontalGrid = grid_type
+
+    @property
+    def left_position(self):
+        """float: The position of the left side of the master depth column as a
+        fraction of the document width.
+        
+        In the case that this is set to be a value higher than
+        ``right_position``, the two attributes will swap. Values will be
+        clamped in the range [0.0, 1.0].
+        """
+        return self._dispatch.LeftPosition
+
+    @left_position.setter
+    def left_position(self, left_pos):
+        self._dispatch.LeftPosition = left_pos
+
+    @property
+    def right_position(self):
+        """float: The position of the right side of the master depth column as
+        a fraction of the document width.
+        
+        In the case that this is set to be a value lower than
+        ``left_position``, the two attributes will swap. Values will be
+        clamped in the range [0.0, 1.0].
+        """
+        return self._dispatch.RightPosition
+
+    @right_position.setter
+    def right_position(self, right_pos):
+        self._dispatch.RightPosition = right_pos
+
+    @property
+    def unit(self):
+        """int: The depth unit
+
+        The available units are the following:
+
+        * 0 = meter
+        * 1 = feet
+        """
+        return self._dispatch.Unit
+
+    @unit.setter
+    def unit(self, unit):
+        self._dispatch.Unit = unit
+
+    def set_position(self, left, right):
+        """Sets the position and width of the master depth column.
+
+        Values given outside the range of [0.0, 1.0] will be clamped. If
+        ``left`` > ``right``, the arguments are swapped.
+
+        Parameters
+        ----------
+        left : float
+            The position of the left side of the depth column as a fraction of
+            the document width.
+
+        right : float
+            The position of the right side of the depth column as a fraction of
+            the document width.
+        """
+        self._dispatch.SetPosition(left, right)
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_drill_item.py` & `pywellcad-0.2.1/wellcad/com/_drill_item.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class DrillItem(DispatchWrapper):
-    """ A Drill Item found in an engineering log gives information about the dimensions of the drilled borehole.
-
-    The drill item gives information about the diameter and length of the borehole. You can have multiple drill items
-    in a borehole if the diameter varies at certain depths. Only a bottom depth is specified: it will range from the
-    top of the borehole (at depth 0) to the specified bottom_depth OR if another drill item is present above,
-    it will range from the bottom of the other drill to the bottom_depth of the current drill.
-
-    Example
-    -------
-    >>> log = borehole.log("Well Sketch")
-    >>> drill_item = log.drill_item(0)
-    >>> drill_item.diameter
-    300
-    >>> drill_item.comment
-    'Drill
-    0.00-15.00
-    diameter:300'
-    """
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of the drill in current depth units."""
-        return self._dispatch.BottomDepth
-
-    @bottom_depth.setter
-    def bottom_depth(self, value):
-        self._dispatch.BottomDepth = value
-
-    @property
-    def diameter(self):
-        """float: The diameter of the drill in arbitrary units.
-
-        Note that some other dimensions in an engineering log are
-        relative to this measure."""
-        return self._dispatch.Diameter
-
-    @diameter.setter
-    def diameter(self, value):
-        self._dispatch.Diameter = value
-
-    @property
-    def comment(self):
-        """str: The comment associated with the drill item."""
-        return self._dispatch.Comment
-
-    @comment.setter
-    def comment(self, value):
-        self._dispatch.Comment = value
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class DrillItem(DispatchWrapper):
+    """ A Drill Item found in an engineering log gives information about the dimensions of the drilled borehole.
+
+    The drill item gives information about the diameter and length of the borehole. You can have multiple drill items
+    in a borehole if the diameter varies at certain depths. Only a bottom depth is specified: it will range from the
+    top of the borehole (at depth 0) to the specified bottom_depth OR if another drill item is present above,
+    it will range from the bottom of the other drill to the bottom_depth of the current drill.
+
+    Example
+    -------
+    >>> log = borehole.log("Well Sketch")
+    >>> drill_item = log.drill_item(0)
+    >>> drill_item.diameter
+    300
+    >>> drill_item.comment
+    'Drill
+    0.00-15.00
+    diameter:300'
+    """
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of the drill in current depth units."""
+        return self._dispatch.BottomDepth
+
+    @bottom_depth.setter
+    def bottom_depth(self, value):
+        self._dispatch.BottomDepth = value
+
+    @property
+    def diameter(self):
+        """float: The diameter of the drill in arbitrary units.
+
+        Note that some other dimensions in an engineering log are
+        relative to this measure."""
+        return self._dispatch.Diameter
+
+    @diameter.setter
+    def diameter(self, value):
+        self._dispatch.Diameter = value
+
+    @property
+    def comment(self):
+        """str: The comment associated with the drill item."""
+        return self._dispatch.Comment
+
+    @comment.setter
+    def comment(self, value):
+        self._dispatch.Comment = value
```

### Comparing `pywellcad-0.2.0/wellcad/com/_equipment_item.py` & `pywellcad-0.2.1/wellcad/com/_equipment_item.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class EquipmentItem(DispatchWrapper):
-    """A Equipment Item found in an engineering log gives information about the elements present in a borehole.
-
-    Base available equipments are listed below, but you can modify or add your own in the Equipment dictionary.
-    
-        * plain casing
-        * wire wound casing
-        * slotted casing
-        * perforated casing
-        * centralizer
-        * shoe
-        * packer
-        * water
-        * wedge
-        * headWorks
-        * transducer
-        * gauge
-        * cement
-        * gravel
-        * normal thread
-        * reverse thread
-        * plug
-
-    Example
-    -------
-    >>> log = borehole.log("Well Sketch")
-    >>> equipment_item = log.eqp_item(5)
-    >>> equipment_item.name
-    "Plain casing"
-    >>> equipment_item.type
-    2  # Hollow item
-    """
-    @property
-    def top_depth(self):
-        """float: The top depth of the equipment item in current
-        depth units."""
-        return self._dispatch.TopDepth
-
-    @top_depth.setter
-    def top_depth(self, value):
-        """Value must be smaller than bottom_depth."""
-        self._dispatch.TopDepth = value
-
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of the equipment item in current
-        depth units."""
-        return self._dispatch.BottomDepth
-
-    @bottom_depth.setter
-    def bottom_depth(self, value):
-        """Value must be greater than top_depth."""
-        self._dispatch.BottomDepth = value
-
-    @property
-    def axis_position(self):
-        """float: The axis position for a solid item in an
-        Engineering Log in same units as the drill diameter."""
-        return self._dispatch.AxisPosition
-
-    @axis_position.setter
-    def axis_position(self, value):
-        self._dispatch.AxisPosition = value
-
-    @property
-    def external_diameter(self):
-        """float: The external diameter for a hollow or solid item in
-        an Engineering Log in the same units as the drill diameter."""
-        return self._dispatch.ExternalDiameter
-
-    @external_diameter.setter
-    def external_diameter(self, value):
-        """Value must be greater than internal_diameter."""
-        self._dispatch.ExternalDiameter = value
-
-    @property
-    def internal_diameter(self):
-        """float: The internal diameter for a hollow item in an
-        Engineering Log in the same units as the drill diameter."""
-        return self._dispatch.InternalDiameter
-
-    @internal_diameter.setter
-    def internal_diameter(self, value):
-        """Value must be smaller than external_diameter."""
-        self._dispatch.InternalDiameter = value
-
-    @property
-    def injection_position(self):
-        """float: The injection position for a liquid item in an
-        Engineering Log in same units as the drill diameter."""
-        return self._dispatch.InjectionPosition
-
-    @injection_position.setter
-    def injection_position(self, value):
-        self._dispatch.InjectionPosition = value
-
-    @property
-    def injection_depth(self):
-        """float: The injection depth for a liquid item in an
-        Engineering Log in current depth reference units."""
-        return self._dispatch.InjectionDepth
-
-    @injection_depth.setter
-    def injection_depth(self, value):
-        """The depth must be between top_depth and bottom_depth"""
-        self._dispatch.InjectionDepth = value
-
-    @property
-    def type(self):
-        """int: The type of the equipment item.
-
-        Possible types are:
-
-        * 0 = Undefined
-        * 1 = Solid Item
-        * 2 = Hollow Item
-        * 3 = Liquid Item
-        """
-        return self._dispatch.Type
-
-    @property
-    def name(self):
-        """str: The name of the equipment item.
-
-        It is the same name as shown in the first column of the
-        tabular editor."""
-        return self._dispatch.Name
-
-    @property
-    def description(self):
-        """str: A more descriptive name for an equiment item."""
-        return self._dispatch.Description
-
-    @property
-    def comment(self):
-        """str: The comment associated with the equipment item."""
-        return self._dispatch.Comment
-
-    @comment.setter
-    def comment(self, value):
-        self._dispatch.Comment = value
-
-    @property
-    def weight(self):
-        """float: The weight of a hollow item in lbs/ft"""
-        return self._dispatch.Weight
-
-    @weight.setter
-    def weight(self, value):
-        self._dispatch.Weight = value
-        
-    @property
-    def thickness(self):
-        """float: The thickness of a hollow item in the same units as
-        the drill diameter."""
-        return self._dispatch.Thickness
-
-    @thickness.setter
-    def thickness(self, value):
-        """When modifying the thickness, the inner diameter of the
-        equipment item is changed"""
-        self._dispatch.Thickness = value
-
-    @property
-    def grade(self):
-        """str: The grade (e.g. type of casing) of a hollow item."""
-        return self._dispatch.Grade
-
-    @grade.setter
-    def grade(self, value):
-        self._dispatch.Grade = value
-
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class EquipmentItem(DispatchWrapper):
+    """A Equipment Item found in an engineering log gives information about the elements present in a borehole.
+
+    Base available equipments are listed below, but you can modify or add your own in the Equipment dictionary.
+    
+        * plain casing
+        * wire wound casing
+        * slotted casing
+        * perforated casing
+        * centralizer
+        * shoe
+        * packer
+        * water
+        * wedge
+        * headWorks
+        * transducer
+        * gauge
+        * cement
+        * gravel
+        * normal thread
+        * reverse thread
+        * plug
+
+    Example
+    -------
+    >>> log = borehole.log("Well Sketch")
+    >>> equipment_item = log.eqp_item(5)
+    >>> equipment_item.name
+    "Plain casing"
+    >>> equipment_item.type
+    2  # Hollow item
+    """
+    @property
+    def top_depth(self):
+        """float: The top depth of the equipment item in current
+        depth units."""
+        return self._dispatch.TopDepth
+
+    @top_depth.setter
+    def top_depth(self, value):
+        """Value must be smaller than bottom_depth."""
+        self._dispatch.TopDepth = value
+
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of the equipment item in current
+        depth units."""
+        return self._dispatch.BottomDepth
+
+    @bottom_depth.setter
+    def bottom_depth(self, value):
+        """Value must be greater than top_depth."""
+        self._dispatch.BottomDepth = value
+
+    @property
+    def axis_position(self):
+        """float: The axis position for a solid item in an
+        Engineering Log in same units as the drill diameter."""
+        return self._dispatch.AxisPosition
+
+    @axis_position.setter
+    def axis_position(self, value):
+        self._dispatch.AxisPosition = value
+
+    @property
+    def external_diameter(self):
+        """float: The external diameter for a hollow or solid item in
+        an Engineering Log in the same units as the drill diameter."""
+        return self._dispatch.ExternalDiameter
+
+    @external_diameter.setter
+    def external_diameter(self, value):
+        """Value must be greater than internal_diameter."""
+        self._dispatch.ExternalDiameter = value
+
+    @property
+    def internal_diameter(self):
+        """float: The internal diameter for a hollow item in an
+        Engineering Log in the same units as the drill diameter."""
+        return self._dispatch.InternalDiameter
+
+    @internal_diameter.setter
+    def internal_diameter(self, value):
+        """Value must be smaller than external_diameter."""
+        self._dispatch.InternalDiameter = value
+
+    @property
+    def injection_position(self):
+        """float: The injection position for a liquid item in an
+        Engineering Log in same units as the drill diameter."""
+        return self._dispatch.InjectionPosition
+
+    @injection_position.setter
+    def injection_position(self, value):
+        self._dispatch.InjectionPosition = value
+
+    @property
+    def injection_depth(self):
+        """float: The injection depth for a liquid item in an
+        Engineering Log in current depth reference units."""
+        return self._dispatch.InjectionDepth
+
+    @injection_depth.setter
+    def injection_depth(self, value):
+        """The depth must be between top_depth and bottom_depth"""
+        self._dispatch.InjectionDepth = value
+
+    @property
+    def type(self):
+        """int: The type of the equipment item.
+
+        Possible types are:
+
+        * 0 = Undefined
+        * 1 = Solid Item
+        * 2 = Hollow Item
+        * 3 = Liquid Item
+        """
+        return self._dispatch.Type
+
+    @property
+    def name(self):
+        """str: The name of the equipment item.
+
+        It is the same name as shown in the first column of the
+        tabular editor."""
+        return self._dispatch.Name
+
+    @property
+    def description(self):
+        """str: A more descriptive name for an equiment item."""
+        return self._dispatch.Description
+
+    @property
+    def comment(self):
+        """str: The comment associated with the equipment item."""
+        return self._dispatch.Comment
+
+    @comment.setter
+    def comment(self, value):
+        self._dispatch.Comment = value
+
+    @property
+    def weight(self):
+        """float: The weight of a hollow item in lbs/ft"""
+        return self._dispatch.Weight
+
+    @weight.setter
+    def weight(self, value):
+        self._dispatch.Weight = value
+        
+    @property
+    def thickness(self):
+        """float: The thickness of a hollow item in the same units as
+        the drill diameter."""
+        return self._dispatch.Thickness
+
+    @thickness.setter
+    def thickness(self, value):
+        """When modifying the thickness, the inner diameter of the
+        equipment item is changed"""
+        self._dispatch.Thickness = value
+
+    @property
+    def grade(self):
+        """str: The grade (e.g. type of casing) of a hollow item."""
+        return self._dispatch.Grade
+
+    @grade.setter
+    def grade(self, value):
+        self._dispatch.Grade = value
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_font.py` & `pywellcad-0.2.1/wellcad/com/_font.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class Font(DispatchWrapper):
-    """ This class encapsulates the properties of fonts used throughout WellCAD
-
-    For example, fonts can be specified in the following places:
-
-    * Comment log
-    * Comment partition
-    * Property partition
-    * Log title
-
-    In general, attributes of this class reflect those of the ``LOGFONT``
-    structure in the Win32 API. Documentation for this structure can be found
-    `here <https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-logfonta>`_.
-
-    Example
-    -------
-    >>> log = borehole.log("Comments")
-    >>> font = log.font
-    >>> font.name
-    'Arial Narrow'
-    >>> font.italic
-    False
-    """
-
-    @property
-    def name(self):
-        """str: The name of the font type used."""
-        return self._dispatch.Name
-
-    @name.setter
-    def name(self, new_name):
-        self._dispatch.Name = new_name
-
-    @property
-    def weight(self):
-        """int: The weight (boldness) of the font used.
-
-        Values typically range from 100 to 900 where
-        400 is regular weight and 700 is bold.
-        """
-        return self._dispatch.Weight
-
-    @weight.setter
-    def weight(self, new_weight):
-        self._dispatch.Weight = new_weight
-
-    @property
-    def italic(self):
-        """bool: Whether the font is italicized."""
-        return self._dispatch.Italic
-
-    @italic.setter
-    def italic(self, flag):
-        self._dispatch.Italic = flag
-
-    @property
-    def underline(self):
-        """bool: Whether the font is underlined."""
-        return self._dispatch.Underline
-
-    @underline.setter
-    def underline(self, flag):
-        self._dispatch.Underline = flag
-
-    @property
-    def bold(self):
-        """bool: Whether the font is bold."""
-        return self._dispatch.Bold
-
-    @bold.setter
-    def bold(self, flag):
-        self._dispatch.Bold = flag
-
-    @property
-    def strikethrough (self):
-        """bool: Whether the font is struck through."""
-        return self._dispatch.Strikethrough
-
-    @strikethrough.setter
-    def strikethrough(self, flag):
-        self._dispatch.Strikethrough = flag
-
-    @property
-    def size(self):
-        """int: The size of the font.
-
-        See the Win32 ``LOGFONT`` documentation for more of an
-        explanation.
-        """
-        return self._dispatch.Size
-
-    @size.setter
-    def size(self, new_size):
-        self._dispatch.Size = new_size
-
-    @property
-    def charset(self):
-        """int: The index of the character set used.
-        
-        The character set can be selected from a list of available values
-        documented in the Win32 ``LOGFONT`` documentation).
-        """
-        return self._dispatch.Charset
-
-    @charset.setter
-    def charset(self, new_charset):
-        self._dispatch.Charset = new_charset
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class Font(DispatchWrapper):
+    """ This class encapsulates the properties of fonts used throughout WellCAD
+
+    For example, fonts can be specified in the following places:
+
+    * Comment log
+    * Comment partition
+    * Property partition
+    * Log title
+
+    In general, attributes of this class reflect those of the ``LOGFONT``
+    structure in the Win32 API. Documentation for this structure can be found
+    `here <https://docs.microsoft.com/en-us/windows/win32/api/wingdi/ns-wingdi-logfonta>`_.
+
+    Example
+    -------
+    >>> log = borehole.log("Comments")
+    >>> font = log.font
+    >>> font.name
+    'Arial Narrow'
+    >>> font.italic
+    False
+    """
+
+    @property
+    def name(self):
+        """str: The name of the font type used."""
+        return self._dispatch.Name
+
+    @name.setter
+    def name(self, new_name):
+        self._dispatch.Name = new_name
+
+    @property
+    def weight(self):
+        """int: The weight (boldness) of the font used.
+
+        Values typically range from 100 to 900 where
+        400 is regular weight and 700 is bold.
+        """
+        return self._dispatch.Weight
+
+    @weight.setter
+    def weight(self, new_weight):
+        self._dispatch.Weight = new_weight
+
+    @property
+    def italic(self):
+        """bool: Whether the font is italicized."""
+        return self._dispatch.Italic
+
+    @italic.setter
+    def italic(self, flag):
+        self._dispatch.Italic = flag
+
+    @property
+    def underline(self):
+        """bool: Whether the font is underlined."""
+        return self._dispatch.Underline
+
+    @underline.setter
+    def underline(self, flag):
+        self._dispatch.Underline = flag
+
+    @property
+    def bold(self):
+        """bool: Whether the font is bold."""
+        return self._dispatch.Bold
+
+    @bold.setter
+    def bold(self, flag):
+        self._dispatch.Bold = flag
+
+    @property
+    def strikethrough (self):
+        """bool: Whether the font is struck through."""
+        return self._dispatch.Strikethrough
+
+    @strikethrough.setter
+    def strikethrough(self, flag):
+        self._dispatch.Strikethrough = flag
+
+    @property
+    def size(self):
+        """int: The size of the font.
+
+        See the Win32 ``LOGFONT`` documentation for more of an
+        explanation.
+        """
+        return self._dispatch.Size
+
+    @size.setter
+    def size(self, new_size):
+        self._dispatch.Size = new_size
+
+    @property
+    def charset(self):
+        """int: The index of the character set used.
+        
+        The character set can be selected from a list of available values
+        documented in the Win32 ``LOGFONT`` documentation).
+        """
+        return self._dispatch.Charset
+
+    @charset.setter
+    def charset(self, new_charset):
+        self._dispatch.Charset = new_charset
```

### Comparing `pywellcad-0.2.0/wellcad/com/_header.py` & `pywellcad-0.2.1/wellcad/com/_header.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class Header(DispatchWrapper):
-    """The class that manages the headers fields.
-
-    Example
-    -------
-    >>> header = borehole.header
-    >>> for i in range(header.nb_of_items):
-    >>>     print(header.item_name(i))
-    COMPANY
-    Title
-    STATE
-    FIELD
-    Features
-    email
-    Complementary1
-    Complementary2
-    Tools
-    """
-
-    @property
-    def nb_of_items(self):
-        """int: Number of dynamic text fields in the entire header."""
-        return self._dispatch.NbOfItems
-
-    def get_item_text(self, name):
-        """Contents of a dynamic text field in the header.
-
-        Parameters
-        ----------
-        name : str
-            ID of the text field as entered in HeadCAD.
-
-        Returns
-        -------
-        str
-            The text contained in the dynamic text field.
-        """
-
-        return self._dispatch.GetItemText(name)
-
-    def set_item_text(self, name, text):
-        """Adds the content of a dynamic text field in the header.
-
-        Parameters
-        ----------
-        name : str
-            ID of the text field as entered in HeadCAD.
-        text : str
-            Text to add into the dynamic text field.
-        """
-
-        self._dispatch.SetItemText(name, text)
-
-    def item_name(self, index):
-        """Returns the ID of a dynamic text field.
-
-        Returns the ID of a dynamic text field in the header based on
-        the zero based index. Use GetNbOfItems to retrieve the total
-        number of text fields in the header.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the dynamic text field.
-
-        Returns
-        -------
-        str
-            The ID of the dynamic text field.
-        """
-
-        return self._dispatch.ItemName(index)
-
-    def allow_export_header(self, index, enable, password):
-        """Changes the protection status to export the header design
-
-        When dealing with a protected document you can use this method to
-        enable / disable the protection to export the header attached to a
-        borehole document as a WCH file. This assumes you are in possession
-        of the password. You still have to export the header manually,
-        this method only toggles the protection.
-
-        Parameters
-        ----------
-        index : int
-            index of the sub-header
-        enable : bool
-            Set this boolean to True to allow the export of the header.
-            Set it to False to protect the header again.
-        password : str
-            String of the password needed to make changes to the
-            protection level of a header.
-        """
-
-        self._dispatch.AllowExportHeader(index, enable, password)
-
-    def allow_export_trailer(self, index, enable, password):
-        """Changes the protection status to export the trailer design
-
-        When dealing with a protected document you can use this method to
-        enable / disable the protection to export the trailer attached to a
-        borehole document as a WCH file. This assumes you are in possession
-        of the password. You still have to export the trailer manually,
-        this method only toggles the protection.
-
-        Parameters
-        ----------
-        index : int
-            index of the sub-trailer
-        enable : bool
-            Set this boolean to True to allow the export of the trailer.
-            Set it to False to protect the trailer again.
-        password : str
-            String of the password needed to make changes to the
-            protection level of a trailer.
-        """
-
-        self._dispatch.AllowExportTrailer(index, enable, password)
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class Header(DispatchWrapper):
+    """The class that manages the headers fields.
+
+    Example
+    -------
+    >>> header = borehole.header
+    >>> for i in range(header.nb_of_items):
+    >>>     print(header.item_name(i))
+    COMPANY
+    Title
+    STATE
+    FIELD
+    Features
+    email
+    Complementary1
+    Complementary2
+    Tools
+    """
+
+    @property
+    def nb_of_items(self):
+        """int: Number of dynamic text fields in the entire header."""
+        return self._dispatch.NbOfItems
+
+    def get_item_text(self, name):
+        """Contents of a dynamic text field in the header.
+
+        Parameters
+        ----------
+        name : str
+            ID of the text field as entered in HeadCAD.
+
+        Returns
+        -------
+        str
+            The text contained in the dynamic text field.
+        """
+
+        return self._dispatch.GetItemText(name)
+
+    def set_item_text(self, name, text):
+        """Adds the content of a dynamic text field in the header.
+
+        Parameters
+        ----------
+        name : str
+            ID of the text field as entered in HeadCAD.
+        text : str
+            Text to add into the dynamic text field.
+        """
+
+        self._dispatch.SetItemText(name, text)
+
+    def item_name(self, index):
+        """Returns the ID of a dynamic text field.
+
+        Returns the ID of a dynamic text field in the header based on
+        the zero based index. Use GetNbOfItems to retrieve the total
+        number of text fields in the header.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the dynamic text field.
+
+        Returns
+        -------
+        str
+            The ID of the dynamic text field.
+        """
+
+        return self._dispatch.ItemName(index)
+
+    def allow_export_header(self, index, enable, password):
+        """Changes the protection status to export the header design
+
+        When dealing with a protected document you can use this method to
+        enable / disable the protection to export the header attached to a
+        borehole document as a WCH file. This assumes you are in possession
+        of the password. You still have to export the header manually,
+        this method only toggles the protection.
+
+        Parameters
+        ----------
+        index : int
+            index of the sub-header
+        enable : bool
+            Set this boolean to True to allow the export of the header.
+            Set it to False to protect the header again.
+        password : str
+            String of the password needed to make changes to the
+            protection level of a header.
+        """
+
+        self._dispatch.AllowExportHeader(index, enable, password)
+
+    def allow_export_trailer(self, index, enable, password):
+        """Changes the protection status to export the trailer design
+
+        When dealing with a protected document you can use this method to
+        enable / disable the protection to export the trailer attached to a
+        borehole document as a WCH file. This assumes you are in possession
+        of the password. You still have to export the trailer manually,
+        this method only toggles the protection.
+
+        Parameters
+        ----------
+        index : int
+            index of the sub-trailer
+        enable : bool
+            Set this boolean to True to allow the export of the trailer.
+            Set it to False to protect the trailer again.
+        password : str
+            String of the password needed to make changes to the
+            protection level of a trailer.
+        """
+
+        self._dispatch.AllowExportTrailer(index, enable, password)
```

### Comparing `pywellcad-0.2.0/wellcad/com/_interval_item.py` & `pywellcad-0.2.1/wellcad/com/_interval_item.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class IntervalItem(DispatchWrapper):
-    """ Stores a value that spans a depth interval.
-
-    Interval items are part of an Interval Log and store a single data value.
-    Only numerical values are supported and depth intervals may overlap.
-
-    Example
-    -------
-    >>> interval_log = borehole.log("Test")
-    >>> data = interval_log.interval_item_at_depth(10.5)
-    >>> data.value
-    23.45
-    >>> data.top_depth
-    9.0
-    """
-
-    @property
-    def top_depth(self):
-        """float: The top depth of the interval item in current
-        depth reference units"""
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of the interval item in current
-        depth reference units"""
-        return self._dispatch.BottomDepth
-
-    @property
-    def value(self):
-        """float: The value of the interval item."""
-        return self._dispatch.Value
-
-    @value.setter
-    def value(self, value):
-        self._dispatch.Value = value
-
-
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class IntervalItem(DispatchWrapper):
+    """ Stores a value that spans a depth interval.
+
+    Interval items are part of an Interval Log and store a single data value.
+    Only numerical values are supported and depth intervals may overlap.
+
+    Example
+    -------
+    >>> interval_log = borehole.log("Test")
+    >>> data = interval_log.interval_item_at_depth(10.5)
+    >>> data.value
+    23.45
+    >>> data.top_depth
+    9.0
+    """
+
+    @property
+    def top_depth(self):
+        """float: The top depth of the interval item in current
+        depth reference units"""
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of the interval item in current
+        depth reference units"""
+        return self._dispatch.BottomDepth
+
+    @property
+    def value(self):
+        """float: The value of the interval item."""
+        return self._dispatch.Value
+
+    @value.setter
+    def value(self, value):
+        self._dispatch.Value = value
+
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_litho_bed.py` & `pywellcad-0.2.1/wellcad/com/_litho_bed.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class LithoBed(DispatchWrapper):
-    """ This class represents a lithological bed. These are sections within a lithology log (Litho Log)
-
-        You can find more information on your defined lithologies in your LithCAD library.
-
-        Example
-        -------
-        >>> log = borehole.log("Lithology")
-        >>> bed = log.litho_bed_at_depth(10.5)
-        >>> bed.top_contact
-        'undulating'
-        >>> bed.top_contact = 'sharp'
-        """
-
-    @property
-    def top_depth(self):
-        """float: The top depth of a lithology bed in current depth
-        units."""
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of a lithology bed in current depth
-        units."""
-        return self._dispatch.BottomDepth
-
-    @property
-    def value(self):
-        """float: The hardness of the bed (between 0 and 1)"""
-        return self._dispatch.Value
-
-    @value.setter
-    def value(self, hardness):
-        self._dispatch.Value = hardness
-
-    @property
-    def litho_code(self):
-        """str: The lithological code of the bed.
-
-        You can use the LithCAD tool to see your lithological
-        symbols and associated codes"""
-        return self._dispatch.LithoCode
-
-    @litho_code.setter
-    def litho_code(self, value):
-        self._dispatch.LithoCode = value
-
-    @property
-    def top_contact(self):
-        """str: The contact code of the top of the bed."""
-        return self._dispatch.TopContact
-
-    @top_contact.setter
-    def top_contact(self, value):
-        self._dispatch.TopContact = value
-
-    @property
-    def bottom_contact(self):
-        """str: The contact code of the bottom of the bed."""
-        return self._dispatch.BottomContact
-
-    @bottom_contact.setter
-    def bottom_contact(self, value):
-        self._dispatch.BottomContact = value
-
-
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class LithoBed(DispatchWrapper):
+    """ This class represents a lithological bed. These are sections within a lithology log (Litho Log)
+
+        You can find more information on your defined lithologies in your LithCAD library.
+
+        Example
+        -------
+        >>> log = borehole.log("Lithology")
+        >>> bed = log.litho_bed_at_depth(10.5)
+        >>> bed.top_contact
+        'undulating'
+        >>> bed.top_contact = 'sharp'
+        """
+
+    @property
+    def top_depth(self):
+        """float: The top depth of a lithology bed in current depth
+        units."""
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of a lithology bed in current depth
+        units."""
+        return self._dispatch.BottomDepth
+
+    @property
+    def value(self):
+        """float: The hardness of the bed (between 0 and 1)"""
+        return self._dispatch.Value
+
+    @value.setter
+    def value(self, hardness):
+        self._dispatch.Value = hardness
+
+    @property
+    def litho_code(self):
+        """str: The lithological code of the bed.
+
+        You can use the LithCAD tool to see your lithological
+        symbols and associated codes"""
+        return self._dispatch.LithoCode
+
+    @litho_code.setter
+    def litho_code(self, value):
+        self._dispatch.LithoCode = value
+
+    @property
+    def top_contact(self):
+        """str: The contact code of the top of the bed."""
+        return self._dispatch.TopContact
+
+    @top_contact.setter
+    def top_contact(self, value):
+        self._dispatch.TopContact = value
+
+    @property
+    def bottom_contact(self):
+        """str: The contact code of the bottom of the bed."""
+        return self._dispatch.BottomContact
+
+    @bottom_contact.setter
+    def bottom_contact(self, value):
+        self._dispatch.BottomContact = value
+
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_litho_dictionary.py` & `pywellcad-0.2.1/wellcad/com/_litho_dictionary.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from ._dispatch_wrapper import DispatchWrapper
-from ._litho_pattern import LithoPattern
-
-
-class LithoDictionary(DispatchWrapper):
-    """A dictionary containing patterns used to represent lithologies.
-
-    You can find more information on your defined lithologies in your LithCAD library.
-
-    Example
-    -------
-    >>> log = borehole.log("Lithology")
-    >>> dict = log.litho_dictionary
-    >>> dict.name
-    'Sst'
-    >>> dict.nb_of_patterns
-    12
-    """
-
-    _DISPATCH_METHODS = ("LithoPattern",)
-
-    @property
-    def name(self):
-        """str: The name of the dictionary."""
-        return self._dispatch.Name
-
-    @name.setter
-    def name(self, value):
-        self._dispatch.Name = value
-
-    @property
-    def nb_of_patterns(self):
-        """int: The number of patterns in the dictionary."""
-        return self._dispatch.NbOfPatterns
-
-    def is_pattern(self, code):
-        """Checks if the dictionary contains a pattern with the specified code.
-
-        Parameters
-        ----------
-        code : str
-            The code of the pattern.
-
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
-        """
-        return self._dispatch.IsPattern(code)
-
-    def litho_pattern(self, index_or_code):
-        """Gets a pattern by index or by code.
-
-        Parameters
-        ----------
-        index_or_code : int or str
-            The index or the code of the pattern
-
-        Returns
-        -------
-        LithoPattern
-            The LithoPattern object.
-        """
-        return LithoPattern(self._dispatch.LithoPattern(index_or_code))
-
-
-
+from ._dispatch_wrapper import DispatchWrapper
+from ._litho_pattern import LithoPattern
+
+
+class LithoDictionary(DispatchWrapper):
+    """A dictionary containing patterns used to represent lithologies.
+
+    You can find more information on your defined lithologies in your LithCAD library.
+
+    Example
+    -------
+    >>> log = borehole.log("Lithology")
+    >>> dict = log.litho_dictionary
+    >>> dict.name
+    'Sst'
+    >>> dict.nb_of_patterns
+    12
+    """
+
+    _DISPATCH_METHODS = ("LithoPattern",)
+
+    @property
+    def name(self):
+        """str: The name of the dictionary."""
+        return self._dispatch.Name
+
+    @name.setter
+    def name(self, value):
+        self._dispatch.Name = value
+
+    @property
+    def nb_of_patterns(self):
+        """int: The number of patterns in the dictionary."""
+        return self._dispatch.NbOfPatterns
+
+    def is_pattern(self, code):
+        """Checks if the dictionary contains a pattern with the specified code.
+
+        Parameters
+        ----------
+        code : str
+            The code of the pattern.
+
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+        """
+        return self._dispatch.IsPattern(code)
+
+    def litho_pattern(self, index_or_code):
+        """Gets a pattern by index or by code.
+
+        Parameters
+        ----------
+        index_or_code : int or str
+            The index or the code of the pattern
+
+        Returns
+        -------
+        LithoPattern
+            The LithoPattern object.
+        """
+        return LithoPattern(self._dispatch.LithoPattern(index_or_code))
+
+
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_litho_pattern.py` & `pywellcad-0.2.1/wellcad/com/_litho_pattern.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class LithoPattern(DispatchWrapper):
-    """Represents a lithological pattern. These are patterns within a litho dictionary (LithoDictionary).
-
-    You can find more information on your defined lithologies in your LithCAD library.
-
-    Example
-    -------
-    >>> log = borehole.log("Lithology")
-    >>> dictionary = log.litho_dictionary
-    >>> pattern = dictionary.litho_pattern(0)
-    >>> pattern.code
-    'Sst'
-    """
-
-    @property
-    def code(self):
-        """str: The lithological code of the pattern.
-
-        You can use the LithCAD tool to see your lithological
-        symbols and associated codes."""
-        return self._dispatch.Code
-
-    @property
-    def description(self):
-        """str: The description ot the pattern."""
-        return self._dispatch.Description
-
-    @property
-    def width(self):
-        """int: The width of the pattern (in 1/10 mm)."""
-        return self._dispatch.Width
-
-    @property
-    def height(self):
-        """int: The height of the pattern (in 1/10 mm)."""
-        return self._dispatch.Height
-
-    @property
-    def repeatable(self):
-        """bool: The option of the symbol to be repeated
-        to fill an entire depth interval or not.
-        """
-        return self._dispatch.Repeatable
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class LithoPattern(DispatchWrapper):
+    """Represents a lithological pattern. These are patterns within a litho dictionary (LithoDictionary).
+
+    You can find more information on your defined lithologies in your LithCAD library.
+
+    Example
+    -------
+    >>> log = borehole.log("Lithology")
+    >>> dictionary = log.litho_dictionary
+    >>> pattern = dictionary.litho_pattern(0)
+    >>> pattern.code
+    'Sst'
+    """
+
+    @property
+    def code(self):
+        """str: The lithological code of the pattern.
+
+        You can use the LithCAD tool to see your lithological
+        symbols and associated codes."""
+        return self._dispatch.Code
+
+    @property
+    def description(self):
+        """str: The description ot the pattern."""
+        return self._dispatch.Description
+
+    @property
+    def width(self):
+        """int: The width of the pattern (in 1/10 mm)."""
+        return self._dispatch.Width
+
+    @property
+    def height(self):
+        """int: The height of the pattern (in 1/10 mm)."""
+        return self._dispatch.Height
+
+    @property
+    def repeatable(self):
+        """bool: The option of the symbol to be repeated
+        to fill an entire depth interval or not.
+        """
+        return self._dispatch.Repeatable
```

### Comparing `pywellcad-0.2.0/wellcad/com/_log.py` & `pywellcad-0.2.1/wellcad/com/_log.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,2359 +1,2359 @@
-from ._dispatch_wrapper import DispatchWrapper
-from ._font import Font
-from ._drill_item import DrillItem
-from ._structure import Structure
-from ._litho_bed import LithoBed
-from ._polar_and_rose_box import PolarAndRoseBox
-from ._interval_item import IntervalItem
-from ._fossil_item import FossilItem
-from ._equipment_item import EquipmentItem
-from ._comment_box import CommentBox
-from ._marker_item import MarkerItem
-from ._stacking_pattern_item import StackingPatternItem
-from ._cross_section_box import CrossSectionBox
-from ._litho_dictionary import LithoDictionary
-
-
-class Log(DispatchWrapper):
-    """The Log class represents a depth or time referenced set of data displayed as a column in a borehole document.
-    Logs can be added/removed/manipulated from the borehole document itself.
-
-    >>> import wellcad.com
-    >>> app = wellcad.com.Application()
-    >>> borehole = app.new_borehole()
-    >>> log = borehole.insert_new_log(1) # Create a new well log
-    """
-    
-    _DISPATCH_METHODS = ("Structure",)
-    _DISPATCH_ATTRIBUTES = ("Style",)
-
-    def file_export(self, directory, file_title=None, extension=None, prompt_user=None, config_filename=None):
-        """Exports the data of the log in the specified format (TXT, CSV, ASC,
-        WA* for all log types, BMP, TIF, GIF, JPG, PNG in addition for RGB and
-        Image Logs).
-
-        Parameters
-        ----------
-        directory : str
-            Path to the location where the file should be stored.
-        file_title : str, optional
-            Name of the file that will be created. By default the log title
-            will be taken.
-        extension : str, optional
-            The file extension to be used.
-        prompt_user: bool, optional
-            If set to ``True`` any warning messages during the graphic file
-            export will be shown.
-        config_filename : str, optional
-            Configuration file used for ASCII (TXT, CSV, ASC, WA*) export only.
-        
-        Returns
-        -------
-        bool
-            Whether the log was successfully exported.
-        """
-        return self._dispatch.FileExport(directory, file_title, extension, prompt_user, config_filename)
-
-    @property
-    def nb_of_data(self):
-        """int: The number of data points in a log."""
-        return self._dispatch.NbOfData
-
-    @property
-    def name(self):
-        """str: The title of the log."""
-        return self._dispatch.Name
-
-    @name.setter
-    def name(self, value):
-        self._dispatch.Name = value
-
-    @property
-    def title_comment(self):
-        """str: The title comment for this log."""
-        return self._dispatch.TitleComment
-
-    @title_comment.setter
-    def title_comment(self, comment):
-        self._dispatch.TitleComment = comment
-
-    @property
-    def top_depth(self):
-        """float: The depth of the first top-most (shallowest) data point in
-        the log using the current depth reference units."""
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float: The depth of the of the bottom-most (deepest) data point in
-        the log using the current depth reference units."""
-        return self._dispatch.BottomDepth
-
-
-    @property
-    def data_table(self):
-        """tuple of tuples: The data table for a log. The first row in the data
-        table is reserved for the log titles (e.g. for a Well Log the fist row
-        in the data table contains the column titles "Depth" and the actual log
-        title). The data format for each log equals the data displayed in the
-        Tabular Editor."""
-        return self._dispatch.DataTable
-
-    @data_table.setter
-    def data_table(self, data):
-        self._dispatch.DataTable = data
-
-    @property
-    def data_min(self):
-        """float: The minimum data value of the Well, Mud or Interval Log."""
-        return self._dispatch.DataMin
-
-    @property
-    def data_max(self):
-        """float: The maximum data value of the Well, Mud or Interval Log."""
-        return self._dispatch.DataMax
-
-    @property
-    def log_unit(self):
-        """str: The unit of a log. Restricted to log types having a unit in the log title."""
-        return self._dispatch.LogUnit
-
-    @log_unit.setter
-    def log_unit(self, unit):
-        self._dispatch.LogUnit = unit
-
-    @property
-    def left_position(self):
-        """float: The position of the left side of the log column as a fraction
-        of the document width.
-        
-        In the case that this is set to be a value higher than
-        ``right_position``, the two attributes will swap. Values will be
-        clamped in the range [0.0, 1.0].
-        """
-        return self._dispatch.LeftPosition
-
-    @left_position.setter
-    def left_position(self, position):
-        self._dispatch.LeftPosition = position
-
-    @property
-    def right_position(self):
-        """float: The position of the right side of the log column as a
-        fraction of the document width.
-        
-        In the case that this is set to be a value lower than
-        ``left_position``, the two attributes will swap. Values will be
-        clamped in the range [0.0, 1.0].
-        """
-        return self._dispatch.RightPosition
-
-    @right_position.setter
-    def right_position(self, position):
-        self._dispatch.RightPosition = position
-
-    def set_position(self, left, right):
-        """Sets the position and width of the log.
-
-        Values given outside the range of [0.0, 1.0] will be clamped. If
-        ``left`` > ``right``, the arguments are swapped.
-
-        Parameters
-        ----------
-        left : float
-            The position of the left side of the log column as a fraction of
-            the document width.
-
-        right : float
-            The position of the right side of the log column as a fraction of
-            the document width.
-        """
-        self._dispatch.SetPosition(left, right)
-
-    @property
-    def type(self):
-        """int: The log type index.
-
-        Log types are one of the below:
-
-        * Undefined = 0
-        * Well log = 1
-        * Formula log = 2
-        * Mud log = 3
-        * FWS log = 4
-        * Image log = 5
-        * Structure log = 6
-        * Litho log = 7
-        * Comment log = 8
-        * Engineering log = 9
-        * RGB log = 10
-        * Image Float 2 log = 11
-        * Image float 4 log = 12
-        * Interval log = 13
-        * Analysis log = 14
-        * Percentage log = 15
-        * Coredesc log = 16
-        * Depth log = 17
-        * Strata log = 18
-        * Stack log = 19
-        * Polar & Rose log = 20
-        * Cross log = 21
-        * OLE log = 22
-        * Shading log = 23
-        * Marker log = 24
-        * Breakout log = 25
-        * Bio log = 26
-        * Lineation log = 27
-        """
-        return self._dispatch.Type
-
-    @property
-    def hide_log_title(self):
-        """bool: Whether the log title is hidden."""
-        return self._dispatch.HideLogTitle
-
-    @hide_log_title.setter
-    def hide_log_title(self, value):
-        self._dispatch.HideLogTitle = value
-
-    @property
-    def hide_log_data(self):
-        """bool: Whether the log data is hidden."""
-        return self._dispatch.HideLogData
-
-    @hide_log_data.setter
-    def hide_log_data(self, value):
-        self._dispatch.HideLogData = value
-
-    @property
-    def log_background_color(self):
-        """int: The background color of the log column.
-        
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values. Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
-        """
-        return self._dispatch.LogBackgroundColor
-
-    @log_background_color.setter
-    def log_background_color(self, value):
-        self._dispatch.LogBackgroundColor = value
-
-    @property
-    def border_style(self):
-        """int: The border line style of the log column.
-        
-        Styles are specified as an integer:
-
-        * Solid = 0
-        * Dashed = 1
-        * Dotted = 2
-        * Dash-Dot = 3
-        * Dash-dot-dot = 4
-        """
-        return self._dispatch.BorderStyle
-
-    @border_style.setter
-    def border_style(self, style):
-        self._dispatch.BorderStyle = style
-
-    @property
-    def border_width(self):
-        """float: The width for the log column border in 1/10 mm."""
-        return self._dispatch.BorderWidth
-
-    @border_width.setter
-    def border_width(self, width):
-        self._dispatch.BorderWidth = width
-
-    @property
-    def border_color(self):
-        """int: The border color of the log column.
-        
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values. Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
-        """
-        return self._dispatch.BorderColor
-
-    @border_color.setter
-    def border_color(self, value):
-        self._dispatch.BorderColor = value
-
-    @property
-    def display_border(self):
-        """bool: Whether the log column border is displayed."""
-        return self._dispatch.DisplayBorder
-
-    @display_border.setter
-    def display_border(self, value):
-        self._dispatch.DisplayBorder = value
-
-    def clear_history(self):
-        """Removes all entries from the log history."""
-        self._dispatch.ClearHistory()
-
-    @property
-    def nb_of_history_item(self):
-        """int: The number of entries in the history (audit trail) of a log."""
-        return self._dispatch.NbOfHistoryItem
-
-    def history_item_date(self, index):
-        """Gets the date of the history item at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the history entry.
-        
-        Returns
-        -------
-        pywintypes.datetime
-            The timezone-aware datetime of the history item.
-        """
-        return self._dispatch.HistoryItemDate(index).replace(tzinfo=None).astimezone()
-
-    def history_item_description(self, index):
-        """Gets the description of the history item at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the history entry.
-        
-        Returns
-        -------
-        str
-            The description of the specified history entry.
-        """
-        return self._dispatch.HistoryItemDescription(index)
-
-    @property
-    def null_value(self):
-        """float: The value that is treated as ``Null`` (not displayed) in a log."""
-        return self._dispatch.NullValue
-
-    @null_value.setter
-    def null_value(self, value):
-        self._dispatch.NullValue = value
-
-    @property
-    def mask_contacts(self):
-        """bool: Whether contact lines within the log column are masked or not."""
-        return self._dispatch.MaskContacts
-
-    @mask_contacts.setter
-    def mask_contacts(self, value):
-        self._dispatch.MaskContacts = value
-
-    @property
-    def mask_horizontal_grid(self):
-        """bool: Whether the horizontal (depth) gridlines of a log are masked or not."""
-        return self._dispatch.MaskHorizontalGrid
-
-    @mask_horizontal_grid.setter
-    def mask_horizontal_grid(self, value):
-        self._dispatch.MaskHorizontalGrid = value
-
-    @property
-    def sample_rate(self):
-        """float: The sample interval of a log in current master depth units."""
-        return self._dispatch.SampleRate
-
-    @sample_rate.setter
-    def sample_rate(self, rate):
-        self._dispatch.SampleRate = rate
-
-    @property
-    def scale_low(self):
-        """float: The low value of the log scale."""
-        return self._dispatch.ScaleLow
-
-    @scale_low.setter
-    def scale_low(self, scale):
-        self._dispatch.ScaleLow = scale
-
-    @property
-    def scale_high(self):
-        """float: The high value of the log scale."""
-        return self._dispatch.ScaleHigh
-
-    @scale_high.setter
-    def scale_high(self, scale):
-        self._dispatch.ScaleHigh = scale
-
-    @property
-    def scale_mode(self):
-        """int: The horizontal scale mode (linear or logarithmic) of a log.
-
-        This property is only available for Well or Mud logs, and can have the
-        following values:
-
-        * Linear = 0
-        * Logarithmic = 1
-        """
-        return self._dispatch.ScaleMode
-
-    @scale_mode.setter
-    def scale_mode(self, mode):
-        self._dispatch.ScaleMode = mode
-
-    @property
-    def scale_reversed(self):
-        """bool: Whether the data display scale is reversed."""
-        return self._dispatch.ScaleReversed
-
-    @scale_reversed.setter
-    def scale_reversed(self, value):
-        self._dispatch.ScaleReversed = value
-
-    @property
-    def use_log_colored_background(self):
-        """bool: Whether the background color of a log is displayed."""
-        return self._dispatch.UseLogColoredBackground
-
-    @use_log_colored_background.setter
-    def use_log_colored_background(self, value):
-        self._dispatch.UseLogColoredBackground = value
-
-    @property
-    def maj_grid_enable(self):
-        """bool: Whether to display major vertical gridlines."""
-        return self._dispatch.MajGridEnable
-
-    @maj_grid_enable.setter
-    def maj_grid_enable(self, value):
-        self._dispatch.MajGridEnable = value
-
-    @property
-    def min_grid_enable(self):
-        """bool: Whether to display minor vertical gridlines."""
-        return self._dispatch.MinGridEnable
-
-    @min_grid_enable.setter
-    def min_grid_enable(self, value):
-        self._dispatch.MinGridEnable = value
-
-    @property
-    def maj_grid_spacing(self):
-        """float: The spacing between major vertical gridlines."""
-        return self._dispatch.MajGridSpacing
-
-    @maj_grid_spacing.setter
-    def maj_grid_spacing(self, spacing):
-        self._dispatch.MajGridSpacing = spacing
-
-    @property
-    def min_grid_spacing(self):
-        """float: The spacing between minor vertical gridlines."""
-        return self._dispatch.MinGridSpacing
-
-    @min_grid_spacing.setter
-    def min_grid_spacing(self, spacing):
-        self._dispatch.MinGridSpacing = spacing
-
-    @property
-    def lock_log_data(self):
-        """bool: Whether the log data is protected from editing."""
-        return self._dispatch.LockLogData
-
-    @lock_log_data.setter
-    def lock_log_data(self, value):
-        self._dispatch.LockLogData = value
-
-    def get_data(self, index):
-        """Gets the data value for the specified index.
-
-        This method is only applicable for a Well, Mud, Interval or Depth Log.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the data to be retrieved.
-        
-        Returns
-        -------
-        float
-            The value of the log data at the specified index.
-        """
-        return self._dispatch.GetData(index)
-
-    def set_data(self, index, value):
-        """Sets the data value for the specified index.
-
-        This method is only applicable for a Well, Mud, Interval or Depth Log.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the data to be retrieved.
-        value : float
-            The value you want to set the data to.
-        """
-        self._dispatch.SetData(index, value)
-
-    def get_data_at_depth(self, depth):
-        """Gets the log data value at the specified depth.
-        
-        This method is only applicable for a Well, Mud, Interval or Depth Log.
-
-        Parameters
-        ----------
-        depth : float
-            Depth value in current master depth units.
-        
-        Returns
-        -------
-        float
-            The value of the log data at the specified depth.
-        """
-        return self._dispatch.GetDataAtDepth(depth)
-
-    def set_data_at_depth(self, depth, value):
-        """Sets the log data value at the specified depth.
-
-        This method is only applicable for a Well, Mud, Interval or Depth Log.
-
-        Parameters
-        ----------
-        depth : float
-            Depth value in current master depth units.
-        value : float
-            The value you want to set the data to.
-        """
-        self._dispatch.SetDataAtDepth(depth, value)
-
-    def data_depth(self, index):
-        """Gets the log data depth for the specified index.
-        
-        This method can be called for Mud, Well, Depth, Percent, Analysis, FWS,
-        Image and RGB Logs. For logs with a constant sample step (Well, Image,
-        RGB, Analysis Logs), the index 0 corresponds to the Bottom Depth.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the data to be retrieved.
-        
-        Returns
-        -------
-        float
-            The depth of the log data at the specified index. If the index is
-            out of bounds, this will be 0.0 for a Mud Log, and an extrapolated
-            value for a Well Log.
-        """
-        return self._dispatch.DataDepth(index)
-
-    def insert_data(self, index, value):
-        """Inserts a new data value at the specified index.
-
-        If necessary existing data points will be shifted.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the new data point will be inserted. The
-            index must be lower or equal to the number of data points in the
-            log.
-        value : float
-            The new data value.
-        
-        Raises
-        ------
-        pywintypes.com_error
-            If the data couldn't be inserted (out-of-bounds index or other)
-        """
-        self._dispatch.InsertData(index, value)
-
-    def insert_data_at_depth(self, depth, value):
-        """Inserts a new data value at the specified depth.
-
-        Data points above (shallower depth) will be shifted upward to
-        accomodate the newly inserted point in a Well Log.
-
-        Parameters
-        ----------
-        depth : float
-            Depth in current master units at which the new data point should be
-            inserted. Depth is rounded to the nearest sample for Well Logs.
-        value : float
-            The new data value
-        """
-        self._dispatch.InsertDataAtDepth(depth, value)
-
-    @property
-    def formula(self):
-        """str: The mathematical formula used for a Formula log.
-        
-        Raises
-        ------
-        pywintypes.com_error
-            If, during setting, the supplied formula is invalid.
-        """
-        return self._dispatch.Formula
-
-    @formula.setter
-    def formula(self, value):
-        self._dispatch.Formula = value
-
-    @property
-    def filter(self):
-        """int: The width (in samples) of the display filter used for Well Logs."""
-        return self._dispatch.Filter
-
-    @filter.setter
-    def filter(self, value):
-        self._dispatch.Filter = value
-
-    @property
-    def fixed_bar_width(self):
-        """int: The fixed bar width, in units of 1/10 mm, for Mud Logs."""
-        return self._dispatch.FixedBarWidth
-
-    @fixed_bar_width.setter
-    def fixed_bar_width(self, width):
-        self._dispatch.FixedBarWidth = width
-
-    def insert_new_interval_item(self, top_depth, bottom_depth, value):
-        """Inserts a new interval in an Interval log.
-
-        Parameters
-        ----------
-        top_depth : float
-            The top depth of the new interval in current depth units.
-        bottom_depth : float
-            The bottom depth of the new interval in current depth units.
-        value : float
-            The value of the new interval item.
-        
-        Returns
-        -------
-        IntervalItem
-            The newly inserted interval item.
-        """
-        return IntervalItem(self._dispatch.InsertNewIntervalItem(top_depth, bottom_depth, value))
-
-    def interval_item(self, index):
-        """Gets an interval item object from an Interval Log.
-
-        Items are ordered by ascending top depth.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the interval item.
-        
-        Returns
-        -------
-        IntervalItem or None
-            The interval item at the specified index, or None if the index
-            is out of range.
-        """
-        return IntervalItem(self._dispatch.IntervalItem(index))
-
-    def interval_item_at_depth(self, depth):
-        """Gets an interval item object from an Interval Log at the specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            Depth value of the interval item, in current master depth units.
-        
-        Returns
-        -------
-        IntervalItem or None
-            The interval item at the specified depth, or None if no interval
-            item exists at the specified depth.
-        """
-        return IntervalItem(self._dispatch.IntervalItemAtDepth(depth))
-
-    @property
-    def pen_color(self):
-        """int: The pen color for a Well or Mud log.
-        
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.  Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
-        """
-        return self._dispatch.PenColor
-
-    @pen_color.setter
-    def pen_color(self, color):
-        self._dispatch.PenColor = color
-
-    @property
-    def pen_style(self):
-        """int: The pen style for the Well or Mud log.
-        
-        Styles are specified as an integer:
-
-        * Solid = 0
-        * Dashed = 1
-        * Dotted = 2
-        * Dash-Dot = 3
-        * Dash-dot-dot = 4
-        """
-        return self._dispatch.PenStyle
-
-    @pen_style.setter
-    def pen_style(self, style):
-        self._dispatch.PenStyle = style
-
-    @property
-    def pen_width(self):
-        """int: The pen width used in a Well or Mud Log in units of 1/10 mm."""
-        return self._dispatch.PenWidth
-
-    @pen_width.setter
-    def pen_width(self, width):
-        self._dispatch.PenWidth = width
-
-    def remove_data(self, index):
-        """Removes a data point from a Mud or Well Log.
-        
-        For Well Logs the data value will be set to ``Null``.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index for the data point to be removed
-        """
-        self._dispatch.RemoveData(index)
-
-    def remove_data_at_depth(self, depth):
-        """Removes a data point from a Mud or Well Log.
-        
-        All data points above (shallower depth) the removed point will be
-        shifted downward (deeper) when data is removed from a Well Log.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value (in current master units) at which the data point.
-            will be removed.
-        """
-        self._dispatch.RemoveDataAtDepth(depth)
-
-    def remove_interval_item(self, index):
-        """Removes a data interval from an Interval log.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index to specify which data interval will be removed.
-        """
-        self._dispatch.RemoveIntervalItem(index)
-
-    def remove_interval_item_at_depth(self, depth):
-        """Removes a data interval from an Interval log.
-
-        Parameters
-        ----------
-        depth : float
-            Depth value in current master units to specify which interval item
-            will be removed.
-        """
-        self._dispatch.RemoveIntervalItemAtDepth(depth)
-
-    @property
-    def shading(self):
-        """int: The shading position used in a Well or Mud Log.
-        
-        * None = 0
-        * Left = 1
-        * Right = 2
-        * Full = 3
-        """
-        return self._dispatch.Shading
-
-    @shading.setter
-    def shading(self, position):
-        self._dispatch.Shading = position
-
-    @property
-    def style(self):
-        """int: The data display style for a log.
-        
-        For Mud logs:
-
-        * Fixed Bar = 1
-        * Dynamic Bar = 2
-        * Line = 3
-        
-        For Engineering logs:
-
-        * Full = 0
-        * Left = 1
-        * Right = 2
-        """
-        return self._dispatch.Style
-
-    @style.setter
-    def style(self, style):
-        self._dispatch.Style = style
-
-    def attach_litho_dictionary(self, dictionary):
-        """Attaches a new symbol or pattern library (\*.LTH file) to Litho, CoreDesc,
-        Strata, Analysis or Percentage Log.
-
-        Parameters
-        ----------
-        dictionary : str
-            path and name of the LTH file to attach
-
-        Returns
-        -------
-            LithoDictionary
-                The LithoDictionary object
-        """
-        return LithoDictionary(self._dispatch.AttachLithoDictionary(dictionary))
-
-    def get_component_name(self, column):
-        """Gets the name (i.e. litho code) for the component used in
-        the specified data column of a Percentage or Analysis Log.
-
-        Parameters
-        ----------
-        column : int
-            Zero based index of the data column in the tabular editor for
-            which the component name should be set or retrieved.
-
-        Returns
-        -------
-        str
-            The code of the component used in the specified data
-            column of a Percentage or Analysis Log.
-        """
-        return self._dispatch.GetComponentName(column)
-
-    def set_component_name(self, column, code):
-        """Sets the name (i.e. litho code) for the component used in
-        the specified data column of a Percentage or Analysis Log.
-
-        Parameters
-        ----------
-        column : int
-            Zero based index of the data column in the tabular editor for
-            which the component name should be set or retrieved.
-        code : str
-            Code of the component to be used in the specified data
-            column of a Percentage or Analysis Log.
-        """
-        self._dispatch.SetComponentName(column, code)
-
-    def fossil_item(self, index):
-        """Gets a Fossil Item object from the CoreDesc Log at the specified index.
-
-        Items are ordered by ascending top depth.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the item to be retrieved.
-
-        Returns
-        -------
-        FossilItem or None
-            The FossilItem at the desired index or none if index is out of range.
-        """
-        return FossilItem(self._dispatch.FossilItem(index))
-
-    def fossil_item_at_depth(self, depth):
-        """Gets a fossil item object from the CoreDesc Log at the specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            depth value in current depth units at which the item will be retrieved
-
-        Returns
-        -------
-        FossilItem or None
-            The FossilItem at the desired depth or None if depth is out of range.
-        """
-        return FossilItem(self._dispatch.FossilItemAtDepth(depth))
-
-    def insert_new_fossil_item(self, top_depth, bottom_depth, litho_code, abundance, dominance, position):
-        """Inserts a new data point or interval into a Core Description Log.
-
-        Parameters
-        ----------
-        top_depth : float
-            Top depth of the new data interval in current depth units.
-        bottom_depth : float
-            Bottom depth of the new data interval in current depth units.
-        litho_code : str
-            Code of the symbol representing the feature as defined in the symbol library of the log.
-        abundance : int
-            The abundance value associated with the symbol (e.g. between 0 and 9).
-        dominance : int
-            The dominance value associated with the symbol
-            undiff = 0
-            minor = 1
-            major = 2
-        position : float
-            A value between 0 and 1 determining the horizontal position of the symbol within the log column.
-
-        Returns
-        -------
-        FossilItem
-            The newly created FossilItem.
-        """
-        return FossilItem(self._dispatch.InsertNewFossilItem(top_depth, bottom_depth, litho_code, abundance, dominance, position))
-
-    def insert_new_litho_bed(self, top_depth, bottom_depth, litho_code, value, position):
-        """Inserts a new lithology bed into a Litho Log.
-
-        Parameters
-        ----------
-        top_depth : float
-            Top depth of the new data interval in current depth units.
-        bottom_depth : float
-            Bottom depth of the new data interval in current depth units.
-        litho_code : str
-            Code of the symbol representing the feature as defined in the symbol library of the log.
-        value : float
-            Hardness value between 0 and 1.
-        position : float
-            A value between 0 and 1 determining the horizontal position of a non repeated symbol
-            in percent of the track width.
-
-        Returns
-        -------
-        LithoBed
-            The newly created LithoBed.
-        """
-        return LithoBed(self._dispatch.InsertNewLithoBed(top_depth, bottom_depth, litho_code, value, position))
-
-    def get_litho_bed(self, index):
-        """Gets a LithoBed object at the specified index from a Lithology Log.
-
-        Items are ordered by ascending top depth.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the LithoBed to retrieve.
-
-        Returns
-        -------
-        LithoBed
-            The LithoBed at the desired index.
-        """
-        return LithoBed(self._dispatch.GetLithoBed(index))
-
-    def set_litho_bed(self, index, litho_bed):
-        """Sets a LithoBed object at the specified index from another
-        LithoBed object.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the LithoBed to retrieve.
-        litho_bed : LithoBed
-            The LithoBed object to copy.
-        """
-        self._dispatch.SetLithoBed(index, litho_bed._dispatch)
-
-    def get_litho_bed_at_depth(self, depth):
-        """Gets a LithoBed object at the specified depth from a Lithology Log.
-
-        Parameters
-        ----------
-        depth : float
-            Depth value in current depth units at which the item will be retrieved.
-
-        Returns
-        -------
-        LithoBed
-            The LithoBed at the desired depth.
-        """
-        return LithoBed(self._dispatch.GetLithoBedAtDepth(depth))
-
-    def set_litho_bed_at_depth(self, depth, litho_bed):
-        """Sets a LithoBed object at the specified depth from another
-        LithoBed object.
-
-        Parameters
-        ----------
-        depth : float
-            Depth value in current depth units at which the item will be retrieved.
-        litho_bed : LithoBed
-            The LithoBed object to copy.
-        """
-        self._dispatch.SetLithoBedAtDepth(depth, litho_bed._dispatch)
-
-    @property
-    def litho_dictionary(self):
-        """LithoDictionary: The symbol library used by the log as LithoDictionary object."""
-        return LithoDictionary(self._dispatch.LithoDictionary)
-
-    @litho_dictionary.setter
-    def litho_dictionary(self, dictionary):
-        self._dispatch.LithoDictionary = dictionary._dispatch
-
-    def remove_fossil_item(self, index):
-        """Removes an item at the specified index from a CoreDesc Log.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the fossil item to be removed.
-        """
-        self._dispatch.RemoveFossilItem(index)
-
-    def remove_fossil_item_at_depth(self, depth):
-        """Removes an item at the specified index from a CoreDesc Log.
-
-        Parameters
-        ----------
-        depth : float
-            the depth value of the symbol in current depth units at which it will be removed.
-        """
-        self._dispatch.RemoveFossilItemAtDepth(depth)
-
-    def remove_litho_bed(self, index):
-        """Removes a lithology bed from the Lithology log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the lithology bed item to be removed.
-        """
-        self._dispatch.RemoveLithoBed(index)
-
-    def remove_litho_bed_at_depth(self, depth):
-        """Removes a lithology bed from the Lithology log at the specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            the depth value in current depth units at which the lithological bed will be removed.
-        """
-        self._dispatch.RemoveLithoBedAtDepth(depth)
-
-    def insert_trace(self, index):
-        """Inserts a new data trace into an Image, FWS or Analysis Log at the specified index.
-
-        Columns for the newly inserted trace are filled with No-Data
-        value. Edit them with set_trace_data or set_trace_data_at_depth.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the trace should be added.
-            Index zero represents the deepest trace.
-            The maximum allowed index is (number of traces + 1).
-            For Image and Analysis logs, existing traces will be shifted upwards depth wise.
-        """
-        self._dispatch.InsertTrace(index)
-
-    def insert_trace_at_depth(self, depth):
-        """Inserts a new data trace into an Image, FWS or Analysis or Percent Log at the specified depth.
-
-        Columns for the newly inserted trace are filled with No-Data
-        value. Edit them with set_trace_data or set_trace_data_at_depth.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the new
-            data trace will be inserted.
-            For Image and Analysis logs:
-            Insertion depth is rounded to the nearest sample.
-            Value must be within the depth range of the existing
-            traces or contiguous to that range (± 1.5 * sampling rate).
-            If necessary existing traces will be shifted upwards.
-            For Percent and FWS logs, if there is already data at that
-            depth, it is replaced with No-Data value, otherwise a trace
-            is inserted at the desired depth without shifting other
-            traces depth wise.
-
-        """
-        self._dispatch.InsertTraceAtDepth(depth)
-
-    def remove_trace(self, index):
-        """Remove an entire data trace from an Image, FWS, Analysis
-        or Percentage Log.
-
-        For Image logs, if the trace is the first or
-        the last, it is removed. Otherwise, it sets all values of that
-        trace to No-Data value.
-        For Analysis, it is the same as for Image logs, but the
-        replacement value is 0.
-        For FWS logs, it removes the trace and shifts down all above
-        traces.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the trace (0 = bottom depth).
-        """
-        self._dispatch.RemoveTrace(index)
-
-    def remove_trace_at_depth(self, depth):
-        """Remove an entire data trace from an Image, FWS, Analysis or
-        Percentage Log.
-
-        For Image logs, if the trace is the first or
-        the last, it is removed. Otherwise, it sets all values of that
-        trace to No-Data value.
-        For Analysis, it is the same as for Image logs, but the
-        replacement value is 0.
-        For FWS logs and Percent, it removes the trace and shifts down
-        all above traces.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the trace
-            will be removed or set to No-Data value.
-        """
-        self._dispatch.RemoveTraceAtDepth(depth)
-
-    def get_trace_data(self, depth_index, trace_index):
-        """Gets the data value at the specified row index and position within the trace
-        (column index) of an Analysis, Percentage, FWS, Image or RGB Log.
-
-        Parameters
-        ----------
-        depth_index : int
-            zero based index of the depth (0 = bottom depth for FWS,
-            Image, RGB and Analysis logs, top depth for Percent logs).
-        trace_index : int
-            zero based index of the column.
-
-        Returns
-        -------
-        float
-            The data value at the specified index and column.
-            The current No-Data value (e.g. -999) will be returned if
-            the depth or trace index refers to a non-existent (out of
-            index range) data point.
-        """
-        return self._dispatch.GetTraceData(depth_index, trace_index)
-
-    def set_trace_data(self, depth_index, trace_index, value):
-        """Sets the data value at the specified row index and position within the trace
-        (column index) of an Analysis, Percentage, FWS, Image or RGB Log.
-
-        Parameters
-        ----------
-        depth_index : int
-            zero based index of the depth (0 = bottom depth).
-        trace_index : int
-            zero based index of the column.
-        value : float
-            The value you want to set the data to.
-        """
-        self._dispatch.SetTraceData(depth_index, trace_index, value)
-
-    def get_trace_data_at_depth(self, depth, trace_position):
-        """Gets the data value at the specified depth and position within the trace of an Analysis,
-        Percentage, FWS, Image or RGB Log.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value at which you would like to retrieve the
-            data value in the current depth units.
-        trace_position : float
-            The position within the trace (time or angle as shown in
-            the column header of the tabular editor, not the index)
-            at which you would like to retrieve the data value.
-
-        Returns
-        -------
-        float
-            The data value at the specified depth and column.
-            The current No-Data value (e.g. -999) will be returned if
-            the depth or trace index refers to a non-existent (out of
-            index range) data point.
-        """
-        return self._dispatch.GetTraceDataAtDepth(depth, trace_position)
-
-    def set_trace_data_at_depth(self, depth, trace_position, value):
-        """set the data value at the specified depth and position within
-        the trace of an Analysis, Percentage, FWS, Image or RGB Log
-
-        Parameters
-        ----------
-        depth : float
-            The depth value at which you would like to retrieve the data value in the current depth units.
-        trace_position : float
-            The position within the trace (time or angle as shown in the column header of the tabular editor,
-            not the index) at which you would like to retrieve the data value.
-        value : float
-            The value you want to set the data to.
-        """
-        self._dispatch.SetTraceDataAtDepth(depth, trace_position, value)
-
-    @property
-    def trace_length(self):
-        """int: The length of a data trace in Image, RGB and FWS Logs.
-
-        For FWS, Analysis and Percent logs:
-        If trace_length is set to a lower value than the current one,
-        all the trace columns past the desired length are discared.
-        If trace_length is set to a higher value than the current one,
-        additional columns are filled with No-data values.
-        For Image and RGB logs:
-        If trace_length is set to a lower value than the current one,
-        trace value are resampled and averaged.
-        If trace_length is set to a higher value than the current one,
-        TODO determine behaviour here.
-        """
-        return self._dispatch.TraceLength
-
-    @trace_length.setter
-    def trace_length(self, length):
-        self._dispatch.TraceLength = length
-
-    @property
-    def trace_offset(self):
-        """float: The offset of a data trace in the FWS Log."""
-        return self._dispatch.TraceOffset
-
-    @trace_offset.setter
-    def trace_offset(self, offset):
-        self._dispatch.TraceOffset = offset
-
-    @property
-    def trace_sample_rate(self):
-        """float: The trace sample interval for a FWS Logs."""
-        return self._dispatch.TraceSampleRate
-
-    @trace_sample_rate.setter
-    def trace_sample_rate(self, rate):
-        self._dispatch.TraceSampleRate = rate
-
-    def get_column_name(self, column):
-        """Gets set the name of a Strata Log column.
-
-        Parameters
-        ----------
-        column : int
-            Zero based index of the column to be retrieved
-
-        Returns
-        -------
-        str
-            The name of the column.
-        """
-        return self._dispatch.GetColumnName(column)
-
-    def set_column_name(self, column, name):
-        """Sets set the name of a Strata Log column.
-
-        Parameters
-        ----------
-        column : int
-            Zero based index of the column to be retrieved
-        name : str
-            New name of the column.
-        """
-        self._dispatch.SetColumnName(column, name)
-
-    def comment_box(self, index):
-        """Gets the Comment Box object from the Comment Log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the box will be retrieved.
-
-        Returns
-        -------
-        CommentBox or None
-            The CommentBox at the desired index or None if index is out of range.
-        """
-        return CommentBox(self._dispatch.CommentBox(index))
-
-    def comment_box_at_depth(self, depth):
-        """Gets the Comment Box object from the Comment Log at the specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the comment box will be retrieved.
-
-        Returns
-        -------
-        CommentBox or None
-            The CommentBox at the desired depth or None if depth is out of range.
-        """
-        return CommentBox(self._dispatch.CommentBoxAtDepth(depth))
-
-    def insert_new_comment_box(self, top_depth, bottom_depth, text):
-        """Sets a new box with the specified text into a Comment Log.
-
-        Parameters
-        ----------
-        top_depth : float
-            The top of the box in current depth units.
-        bottom_depth : float
-            The bottom of the box in current depth units.
-        text : str
-            The text to be displayed in the new box.
-
-        Returns
-        -------
-        CommentBox
-            The newly created CommentBox.
-        """
-        return CommentBox(self._dispatch.InsertNewCommentBox(top_depth, bottom_depth, text))
-
-    def marker(self, index):
-        """Gets the marker with the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the marker.
-
-        Returns
-        -------
-        MarkerItem
-            The marker with the specified index.
-        """
-        return MarkerItem(self._dispatch.Marker(index))
-
-    def marker_by_name(self, name):
-        """Gets the marker with the specified name.
-
-        Parameters
-        ----------
-        name : str
-            Name of the marker to be retrieved.
-
-        Returns
-        -------
-        MarkerItem
-            The marker with the specified name.
-        """
-        return MarkerItem(self._dispatch.MarkerByName(name))
-
-    def insert_new_marker(self, depth, name, comment, contact):
-        """Inserts a new marker at the specified depth into a Marker Log
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the marker will be added.
-        name : str
-            The name (or identifier) of the marker.
-        comment : str
-            The optional comment for the marker.
-        contact : str
-            Name of a contact style to be used and available in the contact dictionary of the Marker Log.
-
-        Returns
-        -------
-        MarkerItem
-            The Marker object at the desired depth with the specified attributes.
-        """
-        return MarkerItem(self._dispatch.InsertNewMarker(depth, name, comment, contact))
-
-    def remove_comment_box(self, index):
-        """Removes a comment box from the Comment log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the comment box will be removed.
-        """
-        self._dispatch.RemoveCommentBox(index)
-
-    def remove_comment_box_at_depth(self, depth):
-        """Removes a comment box from the Comment log at the specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the comment box will be removed.
-        """
-        self._dispatch.RemoveCommentBoxAtDepth(depth)
-
-    def remove_marker(self, index):
-        """Removes the marker from a Marker Log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the marker box will be removed.
-        """
-        self._dispatch.RemoveMarker(index)
-
-    def strata_column(self, index):
-        """Gets a column from a Strata Log as Comment Log object.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index  of the column to be returned.
-
-        Returns
-        -------
-        Log
-            A comment log object.
-        """
-        return Log(self._dispatch.StrataColumn(index))
-
-    def remove_strata_column(self, index):
-        """Removes the the specified column from a Strata Log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the column to be removed.
-        """
-        self._dispatch.RemoveStrataColumn(index)
-
-    @property
-    def font(self):
-        """Gets the font used in a Comment Log as Font Object."""
-        return Font(self._dispatch.Font)
-
-    @font.setter
-    def font(self, font):
-        self._dispatch.Font = font._dispatch
-
-    def attach_attribute_dictionary(self, attribute, file):
-        """Attaches a new attribute library (\*.TAD file) to a
-        Breakout, Lineation or Structure Log.
-
-        Parameters
-        ----------
-        attribute : str
-            Name of the classification column.
-        file : str
-            Path to the TAD file to attach.
-
-        Raises
-        ------
-        pywintypes.com_error
-            If the classification column doesn't exist, an exception is raised.
-        """
-        self._dispatch.AttachAttributeDictionary(attribute, file)
-
-    def insert_new_attribute(self, attribute_name):
-        """Inserts a new blank classification column to a Breakout,
-        Lineation or Structure Log.
-
-        Parameters
-        ----------
-        attribute_name : str
-            Name of the new class.
-        """
-        self._dispatch.InsertNewAttribute(attribute_name)
-
-    def get_attribute_name(self, index):
-        """Gets the name of the attribute class (i.e. classification
-        column) in a Breakout, Lineation or Structure Log.
-
-        Parameters
-        ----------
-        index : str
-            Zero based index of the column.
-
-        Returns
-        -------
-        str
-            The name of the attribute class (classification column)
-
-        Raises
-        ------
-        pywintypes.com_error
-            If the column index points to a non existent column (out
-            of index range) an exception will be raised.
-        """
-        return self._dispatch.GetAttributeName(index)
-
-    def set_attribute_name(self, index, name):
-        """Sets the name of the attribute class (i.e. classification
-        column) in a Breakout, Lineation or Structure Log.
-
-        Parameters
-        ----------
-        index : str
-            Zero based index of the column.
-        name : str
-            New name of the classification column.
-
-        Raises
-        ------
-        pywintypes.com_error
-            If the column index points to a non existent column (out
-            of index range) an exception will be raised.
-        """
-        self._dispatch.SetAttributeName(index, name)
-
-    def structure(self, index):
-        """Gets a Structure object from the Structure Log at the
-        specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the structure object to be retrieved.
-
-        Returns
-        -------
-        Structure or None
-            The structure at the specified index. If the index is outside the valid range no exception
-            will be raised and ``None`` will be returned.
-        """
-        return Structure(self._dispatch.Structure(index))
-
-    def structure_at_depth(self, depth):
-        """Gets the closest Structure object from the Structure Log
-        to the specified depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the
-            structure object will be retrieved.
-
-        Returns
-        -------
-        Structure or None
-            The feature closest to the specified depth will be returned.
-            If the depth is outside the valid range no exception
-            will be raised and ``None`` will be returned.
-        """
-        return Structure(self._dispatch.StructureAtDepth(depth))
-
-    def insert_new_structure_ex(self, depth, azimuth, dip, aperture):
-        """Sets a new structure in a Structure Log.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in the current units of the breakout structure to
-            be inserted.
-        azimuth : float
-            The azimuth angle of the structure measured in degrees.
-        dip : float
-            The tilt angle of the structure measured in degrees.
-        aperture : float
-            The aperture of the structure in meters.
-
-        Returns
-        -------
-        Structure
-            The newly created structure object.
-        """
-        return Structure(self._dispatch.InsertNewStructureEx(depth, azimuth, dip, aperture))
-
-    def remove_structure(self, index):
-        """Removes a structure from the Structure Log at the
-        specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the structure to be removed.
-        """
-        self._dispatch.RemoveStructure(index)
-
-    def remove_structure_at_depth(self, depth):
-        """Removes a structure from the Structure Log at the
-        specified depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the
-            structure will be removed.
-        """
-        self._dispatch.RemoveStructureAtDepth(depth)
-
-    def breakout(self, index):
-        """Gets a breakout structure from the Breakout Log at the specified
-        index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the breakout to be retrieved.
-
-        Returns
-        -------
-        Structure or None
-            The breakout at the specified index. If the index is
-            outside the valid range no exception will be raised and
-            ``None`` will be returned.
-
-        """
-        return Structure(self._dispatch.Breakout(index))
-
-    def breakout_at_depth(self, depth):
-        """Gets a breakout structure from the Breakout Log at the specified
-        depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the
-            breakout will be retrieved.
-
-        Returns
-        -------
-        Structure or None
-            The feature closest to the specified depth will be returned.
-            If the depth is outside the valid range no exception
-            will be raised and ``None`` will be returned.
-        """
-        return Structure(self._dispatch.BreakoutAtDepth(depth))
-
-    def insert_new_breakout_ex(self, depth, azimuth, tilt, length, opening):
-        """Sets a new breakout structure in a Breakout Log.
-
-        If the mirror option is active, a second breakout structure object is
-        added 180° degrees apart.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value of the breakout structure in current depth units.
-        azimuth : float
-            The azimuth angle of the breakout structure measured in degrees.
-        tilt : float
-            The tilt angle of the breakout structure measured in degrees.
-        length : float
-            The length of the breakout structure in meters.
-        opening : float
-            The opening (or aperture) angle of the breakout structure in degrees.
-
-        Returns
-        -------
-        Structure
-            The newly created breakout structure.
-        """
-        return Structure(self._dispatch.InsertNewBreakoutEx(depth, azimuth, tilt, length, opening))
-
-    def remove_breakout(self, index):
-        """Removes a breakout structure from the Breakout Log at the specified
-        index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the breakout structure to be removed.
-        """
-        self._dispatch.RemoveBreakout(index)
-
-    def remove_breakout_at_depth(self, depth):
-        """Removes a breakout structure from the Breakout Log at the specified
-        depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the
-            breakout structure will be removed.
-        """
-        self._dispatch.RemoveBreakoutAtDepth(depth)
-    
-    def lineation(self, index):
-        """Gets a lineation pick from the Lineation Log at the specified
-        index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the lineation to be retrieved.
-
-        Returns
-        -------
-        Structure or None
-            The lineation at the specified index. If the index is
-            outside the valid range no exception will be raised and
-            ``None`` will be returned.
-        """
-        return Structure(self._dispatch.Lineation(index))
-
-    def lineation_at_depth(self, depth):
-        """Gets a lineation structure from the Lineation Log at the specified
-        depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the
-            lineation will be retrieved.
-
-        Returns
-        -------
-        Structure or None
-            The feature closest to the specified depth will be returned.
-            If the depth is outside the valid range no exception
-            will be raised and ``None`` will be returned.
-        """
-        return Structure(self._dispatch.LineationAtDepth(depth))
-
-    def insert_new_lineation_ex(self, depth, trend, plunge, eccentricity):
-        """Sets a new linear structure in a Lineation Log.
-
-        Parameters
-        ----------
-        depth : float
-            Depth of the mid-point of the fitted line in current depth units.
-        trend : float
-            Trend direction of the vector in degrees.
-        plunge : float
-            "Dip" angle of the vector in degrees.
-        eccentricity : float
-            Offset of the lineation from the center of the borehole.
-            A value between -1 and 1 can be set. An eccentricity of 0
-            corresponds to a line going straight through the center
-            of the borehole.
-
-        Returns
-        -------
-        Structure
-            The newly created lineation structure.
-        """
-        return Structure(self._dispatch.InsertNewLineationEx(depth, trend, plunge, eccentricity))
-
-    def remove_lineation(self, index):
-        """Removes a lineation from the Lineation Log at the
-        specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the lineation to be removed.
-        """
-        self._dispatch.RemoveLineation(index)
-
-    def remove_lineation_at_depth(self, depth):
-        """Removes a lineation from the Lineation Log at the
-        specified depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth value in current depth units at which the
-            lineation will be removed.
-        """
-        self._dispatch.RemoveLineationAtDepth(depth)
-
-    @property
-    def length_unit(self):
-        """float: The conversion factor (from meters) for the
-        breakout structure length measured in the breakout log
-
-        Set it to 0.001 when measured in mm and to 0.0254 when
-        measured in inches."""
-        return self._dispatch.LengthUnit
-
-    @length_unit.setter
-    def length_unit(self, factor):
-        self._dispatch.LengthUnit = factor
-
-    @property
-    def caliper_unit(self):
-        """float: The conversion factor (from meters) for the caliper
-        value in a structure log.
-
-        Set it to 0.001 when measured in mm and to 0.0254 when
-        measured in inches."""
-        return self._dispatch.CaliperUnit
-
-    @caliper_unit.setter
-    def caliper_unit(self, factor):
-        self._dispatch.CaliperUnit = factor
-
-    @property
-    def aperture_unit(self):
-        """float: The conversion factor (from meters) for the 
-        aperture value in a structure log.  
-
-        Set it to 0.001 when measured in mm and to 0.00254 when
-        measured in 1/10th inches."""
-        return self._dispatch.ApertureUnit
-
-    @aperture_unit.setter
-    def aperture_unit(self, factor):
-        self._dispatch.ApertureUnit = factor
-
-    def insert_new_schmit_box(self, top_depth, bottom_depth, text):
-        """Inserts a new box into a Polar & Rose Log.
-
-        Parameters
-        ----------
-        top_depth : float
-            The top depth value of the interval in the current depth units.
-        bottom_depth : float
-            The bottom depth value of the interval in the current depth units.
-        text : string
-            A text description which is only shown in the tabular editor display.
-
-        Returns
-        -------
-        PolarAndRoseBox
-            The newly created Polar & Rose box.
-        """
-        return PolarAndRoseBox(self._dispatch.InsertNewSchmitBox(top_depth, bottom_depth, text))
-
-    def schmit_box(self, index):
-        """Gets a box object from the Polar & Rose Log at the
-        specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the box to be returned.
-
-        Returns
-        -------
-        PolarAndRoseBox
-            The Polar & Rose box at the desired index.
-        """
-        return PolarAndRoseBox(self._dispatch.SchmitBox(index))
-
-    def schmit_box_at_depth(self, depth):
-        """Gets a box object from the Polar & Rose Log
-        at the specified depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth of the box to be returned in current depth units.
-
-        Returns
-        -------
-        PolarAndRoseBox
-            The Polar & Rose box at the desired depth.
-        """
-        return PolarAndRoseBox(self._dispatch.SchmitBoxAtDepth(depth))
-
-    def remove_schmit_box(self, index):
-        """Removes a box from the Polar & Rose Log at the
-        specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the Polar & Rose box to be removed.
-        """
-        self._dispatch.RemoveSchmitBox(index)
-
-    def remove_schmit_box_at_depth(self, depth):
-        """Removes a box from the Polar & Rose log at the specified
-        depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth of the Polar & Rose box to be removed in
-            current depth units.
-        """
-        self._dispatch.RemoveSchmitBoxAtDepth(depth)
-
-    def cross_box(self, index):
-        """Gets a Cross Box object from the Cross Section Log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the box to be retrieved.
-
-        Returns
-        -------
-        CrossSectionBox or None
-            The CrossSectionBox at the desired index or None if index is out of range.
-        """
-        return CrossSectionBox(self._dispatch.CrossBox(index))
-
-    def cross_box_at_depth(self, depth):
-        """Gets a Cross Box object from the Cross Section Log at the specified depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth of the box to be retrieved in current depth units.
-
-        Returns
-        -------
-        CrossSectionBox or None
-            The CrossSectionBox at the desired index or None if the index is out of range.
-        """
-        return CrossSectionBox(self._dispatch.CrossBoxAtDepth(depth))
-
-    def insert_new_cross_box(self, top_depth, bottom_depth):
-        """Inserts a new box into the Cross Section Log.
-
-        Parameters
-        ----------
-        top_depth : float
-            The top depth value of the cross section box in current depth units.
-        bottom_depth : float
-            The bottom depth value of the cross section box in current depth units.
-
-        Returns
-        -------
-        CrossSectionBox
-            The newly created CrossSectionBox.
-        """
-        return CrossSectionBox(self._dispatch.InsertNewCrossBox(top_depth, bottom_depth))
-
-    def remove_cross_box(self, index):
-        """Removes a box from the Cross Section Log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the box to be removed.
-        """
-        self._dispatch.RemoveCrossBox(index)
-
-    def remove_cross_box_at_depth(self, depth):
-        """Removes a box from the Cross Section Log at the specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            The depth in current units at which the box will be removed.
-        """
-        self._dispatch.RemoveCrossBoxAtDepth(depth)
-
-    def insert_new_stack_item(self, top_depth, bottom_depth, top_width, bottom_width):
-        """Inserts a new data interval into a Stacking Pattern Log.
-
-        Parameters
-        ----------
-        top_depth : float
-            The top depth value of the interval in the current depth units.
-        bottom_depth : float
-            The bottom depth value of the interval in the current depth units.
-        top_width : float
-           Width value at the top of the new interval.
-        bottom_width : float
-            Width value at the bottom of the new interval.
-
-        Returns
-        -------
-        StackingPatternItem
-            The newly created StackingPatternItem.
-        """
-        return StackingPatternItem(self._dispatch.InsertNewStackItem(top_depth, bottom_depth, top_width, bottom_width))
-
-    def stack_item(self, index):
-        """Gets a Stack Item object from the Stacking Pattern Log at the specified depth index.
-
-        Items are ordered by ascending top depth.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the item to be retrieved.
-
-        Returns
-        -------
-        StackingPatternItem or None
-            The StackingPatternItem at the desired index or None if the index is out of range.
-        """
-        return StackingPatternItem(self._dispatch.StackItem(index))
-
-    def stack_item_at_depth(self, depth):
-        """Gets a Stack Item object from the Stacking Pattern Log at the specified depth in current depth units.
-
-        Parameters
-        ----------
-        depth : float
-            The depth of the item to be retrieved in current depth units.
-
-        Returns
-        -------
-        StackingPatternItem or None
-            The StackingPatternItem at the desired depth or None if depth is out of range.
-        """
-        return StackingPatternItem(self._dispatch.StackItemAtDepth(depth))
-
-    def remove_stack_item(self, index):
-        """Removes an item from the Stacking Pattern Log at the specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index  of the stacking pattern box to be removed.
-        """
-        self._dispatch.RemoveStackItem(index)
-
-    def remove_stack_item_at_depth(self, depth):
-        """Removes an item from the Stacking Pattern Log at the specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            The depth of the stack item to be removed in current depth units.
-        """
-        self._dispatch.RemoveStackItemAtDepth(depth)
-
-    @property
-    def used_as_depth_scale(self):
-        """bool: Whether the Depth Log is used as the current depth
-        reference axis."""
-        return self._dispatch.UsedAsDepthScale
-
-    @used_as_depth_scale.setter
-    def used_as_depth_scale(self, mode):
-        self._dispatch.UsedAsDepthScale = mode
-
-    def insert_new_ole_box_from_file(self, file_name, allow_picture, top_depth, bottom_depth):
-        """Inserts a new OLE object between the specified interval
-        into an OLE Log.
-
-        OLE objects can be files such as images, Excel charts,
-        Word documents or pdfs.
-
-        Parameters
-        ----------
-        file_name : str
-            Path and name of the file to be loaded.
-        allow_picture : bool
-            Set to True to allow graphic files to be displayed using
-            an internal viewer.
-        top_depth : float
-            Top depth of the OLE object in current depth units.
-        bottom_depth : float
-            Bottom depth of the OLE object in current depth units.
-        """
-        self._dispatch.InsertNewOleBoxFromFile(file_name, allow_picture, top_depth, bottom_depth)
-
-    def drill_item(self, index):
-        """Gets a Drill Item object from the Engineering Log at the
-        specified index.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the drill item will be retrieved.
-
-        Returns
-        -------
-        DrillItem
-            The drill item at the specified index.
-        """
-        return DrillItem(self._dispatch.DrillItem(index))
-
-    def drill_item_at_depth(self, depth):
-        """Gets a Drill Item object from the Engineering Log at the
-        specified depth.
-
-        Parameters
-        ----------
-        depth : float
-            The depth of the item to be retrieved in current depth
-            units.
-
-        Returns
-        -------
-        DrillItem
-            The drill item at the specified depth.
-        """
-        return DrillItem(self._dispatch.DrillItemAtDepth(depth))
-
-    def eqp_item(self, index):
-        """Gets an Equipment Item object at the specified index from
-        the Engineering Log.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the item will be retrieved.
-
-        Returns
-        -------
-        EquipmentItem
-            The equipment item at the specified index.
-        """
-        return EquipmentItem(self._dispatch.EqpItem(index))
-
-    @property
-    def comment_style(self):
-        """int: The position of the comment associated with an engineering log.
-
-        The following styles are available:
-
-            * 0 = None, comment is not displayed
-            * 1 = Left, comment displayed on the left of the engineering log
-            * 2 = Right, comment displayed on the right of the engineering log
-        """
-        return self._dispatch.CommentStyle
-
-    @comment_style.setter
-    def comment_style(self, style):
-        self._dispatch.CommentStyle = style
-
-    @property
-    def ground_depth(self):
-        """float: The starting point (reference datum) of the
-        borehole."""
-        return self._dispatch.GroundDepth
-
-    @ground_depth.setter
-    def ground_depth(self, starting_point):
-        self._dispatch.GroundDepth = starting_point
-
-    @property
-    def diameter_high(self):
-        """float: The maximum diameter scaling value
-        (width of the log column) for an Engineering Log."""
-        return self._dispatch.DiameterHigh
-
-    @diameter_high.setter
-    def diameter_high(self, diameter):
-        self._dispatch.DiameterHigh = diameter
-
-    def insert_new_drill_item(self, bottom_depth, diameter):
-        """Inserts a new drill item into the Engineering Log.
-
-        Item index are ordered by depth value in the stack of drill
-        items.
-
-        Parameters
-        ----------
-        bottom_depth : float
-            The bottom depth of the borehole in current depth units.
-            (The top depth is either the ground_depth or the former
-            bottom depth).
-        diameter : float
-            The diameter of the borehole.
-
-        Returns
-        -------
-        DrillItem
-            The inserted DrillItem
-        """
-        return DrillItem(self._dispatch.InsertNewDrillItem(bottom_depth, diameter))
-
-    def insert_new_eqp_item(self, top_depth, bottom_depth, name):
-        """Inserts a new equipment item of the specified name and
-        depth interval into the Engineering Log.
-
-        The new item is given the last index in the list of equipment
-        items.
-
-        Parameters
-        ----------
-        top_depth : float
-            The top depth of the equipment item interval
-            in current units.
-        bottom_depth : float
-            The bottom depth of the equipment item interval
-            in current units.
-        name : str
-            The name (code) of the equipment item to be inserted.
-            Base available equipments names are listed below, but you
-            can modify or add your own in the Equipment dictionary.
-
-                * PlainCasing
-                * WireWoundCasing
-                * SlottedCasing
-                * PerforatedCasing
-                * Centralizer
-                * Shoe
-                * Packer
-                * Water
-                * Wedge
-                * HeadWorks
-                * Transducer
-                * Gauge
-                * Cement
-                * Gravel
-                * NormalThread
-                * ReverseThread
-                * Plug
-
-            If an invalid name is provided, no item will be inserted.
-
-        Returns
-        -------
-        EqpItem
-            The inserted EqpItem
-        """
-        return EquipmentItem(self._dispatch.InsertNewEqpItem(top_depth, bottom_depth, name))
-
-    @property
-    def nb_of_drill_item(self):
-        """int: The number of drill items in an Engineering Log."""
-        return self._dispatch.NbOfDrillItem
-
-    @property
-    def nb_of_eqp_item(self):
-        """int: The number of equipment items in an Engineering Log."""
-        return self._dispatch.NbOfEqpItem
-
-    def remove_drill_item(self, index):
-        """Removes the drill item at the specified index from an
-        Engineering Log.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the item will be removed.
-        """
-        self._dispatch.RemoveDrillItem(index)
-
-    def remove_eqp_item(self, index):
-        """Removes an equipment item at the specified depth index
-        from an Engineering Log.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index at which the item will be removed.
-        """
-        self._dispatch.RemoveEqpItem(index)
-
-    @property
-    def background_color(self):
-        """int: The background color of the engineering log.
-
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
-        """
-        return self._dispatch.BackgroundColor
-
-    @background_color.setter
-    def background_color(self, value):
-        self._dispatch.BackgroundColor = value
-
-
-    @property
-    def background_hatch_style(self):
-        """int: The background hatch style for the Engineering Log.
-
-        Available styles are:
-
-        * 0: horizontal
-        * 1: vertical
-        * 2: forward diagonal
-        * 3: backward diagonal
-        * 4: cross
-        * 5: diagonal cross
-
-        If an invalid style is set, nothing will happen.
-        """
-        return self._dispatch.BackgroundHatchStyle
-
-    @background_hatch_style.setter
-    def background_hatch_style(self, code):
-        self._dispatch.BackgroundHatchStyle = code
-
-    @property
-    def background_style(self):
-        """int: The background style for the Engineering Log.
-
-        Available styles are:
-
-        * 0: none
-        * 1: solid
-        * 2: hatch
-
-        If an invalid style is set, nothing will happen.
-        """
-        return self._dispatch.BackgroundStyle
-
-    @background_style.setter
-    def background_style(self, code):
-        self._dispatch.BackgroundStyle = code
-
-    def allow_export_attribute_dictionary(self, index, export, password):
-        """When dealing with a protected document you can use this method to enable/disable the option
-        to export the tadpole dictionary (\*.TAD) from a specific classification column of a Structure or
-        Breakout Log. This assumes you are in possession of the password.
-
-        Parameters
-        ----------
-        index : int
-            Zero based index of the classification column for which the protection level should eb changed.
-        export : bool
-            Set this boolean to True to allow an export as \*.tad file. Set it to False to protect the dictionary.
-        password : str
-            the password needed to make changes to the protection level.
-        """
-        self._dispatch.AllowExportAttributeDictionary(index, export, password)
-
-    def allow_export_litho_dictionary(self, export, password):
-        """When dealing with a protected document you can use this method to enable / disable the option
-        to export the symbol dictionary (\*.LTH) of a log. This assumes you are in possession of the password.
-
-        Parameters
-        ----------
-        export : bool
-            Set this boolean to True to allow the dictionary export. Set it to False to protect the dictionary.
-        password : str
-            the password needed to make changes to the protection level.
-        """
-        self._dispatch.AllowExportLithoDictionary(export, password)
-
-    def allow_modify_log_data(self, export, password):
-        """When dealing with a protected document you can use this method to enable / disable the option
-        to edit the data of a log. This assumes you are in possession of the password.
-
-        Parameters
-        ----------
-        export : bool
-            Set this boolean to True to allow the modification of log data. Set it to False to protect the data.
-        password : str
-            the password needed to make changes to the protection level.
-        """
-        self._dispatch.AllowModifyLogData(export, password)
-
-    def allow_modify_log_settings(self, export, password):
-        """When dealing with a protected document you can use this method to enable / disable the option
-        to change the settings of a log. This assumes you are in possession of the password.
-
-        Parameters
-        ----------
-        export : bool
-            Set this boolean to True to allow access to the log settings. Set it to False to protect the log settings.
-        password : str
-            the password needed to make changes to the protection level.
-        """
-        self._dispatch.AllowModifyLogSettings(export, password)
-
-    def allow_use_formula(self, export, password):
-        """When dealing with a protected document you can use this method to enable / disable the option
-        to access and use the formula in a Formula Log. This assumes you are in possession of the password.
-
-        Parameters
-        ----------
-        export : bool
-            Set this boolean to True to allow access the formula. Set it to False to protect the formula.
-        password : str
-            the password needed to make changes to the protection level.
-        """
-        self._dispatch.AllowUseFormula(export, password)
-
-    def allow_view_formula(self, export, password):
-        """When dealing with a protected document you can use this method to enable / disable the option
-        to see the formula used in a Formula Log. This assumes you are in possession of the password.
-
-        Parameters
-        ----------
-        export : bool
-            Set this boolean to True to see the formula. Set it to False to protect the formula.
-        password : str
-            the password needed to make changes to the protection level.
-        """
-        self._dispatch.AllowViewFormula(export, password)
-
-    def allow_view_log_history(self, export, password):
-        """When dealing with a protected document you can use this method to enable / disable the option
-        to view the log history. This assumes you are in possession of the password.
-
-        Parameters
-        ----------
-        export : bool
-            Set this boolean to True to access the log history. Set it to False to protect the log history.
-        password : str
-            the password needed to make changes to the protection level.
-        """
-        self._dispatch.AllowViewLogHistory(export, password)
+from ._dispatch_wrapper import DispatchWrapper
+from ._font import Font
+from ._drill_item import DrillItem
+from ._structure import Structure
+from ._litho_bed import LithoBed
+from ._polar_and_rose_box import PolarAndRoseBox
+from ._interval_item import IntervalItem
+from ._fossil_item import FossilItem
+from ._equipment_item import EquipmentItem
+from ._comment_box import CommentBox
+from ._marker_item import MarkerItem
+from ._stacking_pattern_item import StackingPatternItem
+from ._cross_section_box import CrossSectionBox
+from ._litho_dictionary import LithoDictionary
+
+
+class Log(DispatchWrapper):
+    """The Log class represents a depth or time referenced set of data displayed as a column in a borehole document.
+    Logs can be added/removed/manipulated from the borehole document itself.
+
+    >>> import wellcad.com
+    >>> app = wellcad.com.Application()
+    >>> borehole = app.new_borehole()
+    >>> log = borehole.insert_new_log(1) # Create a new well log
+    """
+    
+    _DISPATCH_METHODS = ("Structure",)
+    _DISPATCH_ATTRIBUTES = ("Style",)
+
+    def file_export(self, directory, file_title=None, extension=None, prompt_user=None, config_filename=None):
+        """Exports the data of the log in the specified format (TXT, CSV, ASC,
+        WA* for all log types, BMP, TIF, GIF, JPG, PNG in addition for RGB and
+        Image Logs).
+
+        Parameters
+        ----------
+        directory : str
+            Path to the location where the file should be stored.
+        file_title : str, optional
+            Name of the file that will be created. By default the log title
+            will be taken.
+        extension : str, optional
+            The file extension to be used.
+        prompt_user: bool, optional
+            If set to ``True`` any warning messages during the graphic file
+            export will be shown.
+        config_filename : str, optional
+            Configuration file used for ASCII (TXT, CSV, ASC, WA*) export only.
+        
+        Returns
+        -------
+        bool
+            Whether the log was successfully exported.
+        """
+        return self._dispatch.FileExport(directory, file_title, extension, prompt_user, config_filename)
+
+    @property
+    def nb_of_data(self):
+        """int: The number of data points in a log."""
+        return self._dispatch.NbOfData
+
+    @property
+    def name(self):
+        """str: The title of the log."""
+        return self._dispatch.Name
+
+    @name.setter
+    def name(self, value):
+        self._dispatch.Name = value
+
+    @property
+    def title_comment(self):
+        """str: The title comment for this log."""
+        return self._dispatch.TitleComment
+
+    @title_comment.setter
+    def title_comment(self, comment):
+        self._dispatch.TitleComment = comment
+
+    @property
+    def top_depth(self):
+        """float: The depth of the first top-most (shallowest) data point in
+        the log using the current depth reference units."""
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float: The depth of the of the bottom-most (deepest) data point in
+        the log using the current depth reference units."""
+        return self._dispatch.BottomDepth
+
+
+    @property
+    def data_table(self):
+        """tuple of tuples: The data table for a log. The first row in the data
+        table is reserved for the log titles (e.g. for a Well Log the fist row
+        in the data table contains the column titles "Depth" and the actual log
+        title). The data format for each log equals the data displayed in the
+        Tabular Editor."""
+        return self._dispatch.DataTable
+
+    @data_table.setter
+    def data_table(self, data):
+        self._dispatch.DataTable = data
+
+    @property
+    def data_min(self):
+        """float: The minimum data value of the Well, Mud or Interval Log."""
+        return self._dispatch.DataMin
+
+    @property
+    def data_max(self):
+        """float: The maximum data value of the Well, Mud or Interval Log."""
+        return self._dispatch.DataMax
+
+    @property
+    def log_unit(self):
+        """str: The unit of a log. Restricted to log types having a unit in the log title."""
+        return self._dispatch.LogUnit
+
+    @log_unit.setter
+    def log_unit(self, unit):
+        self._dispatch.LogUnit = unit
+
+    @property
+    def left_position(self):
+        """float: The position of the left side of the log column as a fraction
+        of the document width.
+        
+        In the case that this is set to be a value higher than
+        ``right_position``, the two attributes will swap. Values will be
+        clamped in the range [0.0, 1.0].
+        """
+        return self._dispatch.LeftPosition
+
+    @left_position.setter
+    def left_position(self, position):
+        self._dispatch.LeftPosition = position
+
+    @property
+    def right_position(self):
+        """float: The position of the right side of the log column as a
+        fraction of the document width.
+        
+        In the case that this is set to be a value lower than
+        ``left_position``, the two attributes will swap. Values will be
+        clamped in the range [0.0, 1.0].
+        """
+        return self._dispatch.RightPosition
+
+    @right_position.setter
+    def right_position(self, position):
+        self._dispatch.RightPosition = position
+
+    def set_position(self, left, right):
+        """Sets the position and width of the log.
+
+        Values given outside the range of [0.0, 1.0] will be clamped. If
+        ``left`` > ``right``, the arguments are swapped.
+
+        Parameters
+        ----------
+        left : float
+            The position of the left side of the log column as a fraction of
+            the document width.
+
+        right : float
+            The position of the right side of the log column as a fraction of
+            the document width.
+        """
+        self._dispatch.SetPosition(left, right)
+
+    @property
+    def type(self):
+        """int: The log type index.
+
+        Log types are one of the below:
+
+        * Undefined = 0
+        * Well log = 1
+        * Formula log = 2
+        * Mud log = 3
+        * FWS log = 4
+        * Image log = 5
+        * Structure log = 6
+        * Litho log = 7
+        * Comment log = 8
+        * Engineering log = 9
+        * RGB log = 10
+        * Image Float 2 log = 11
+        * Image float 4 log = 12
+        * Interval log = 13
+        * Analysis log = 14
+        * Percentage log = 15
+        * Coredesc log = 16
+        * Depth log = 17
+        * Strata log = 18
+        * Stack log = 19
+        * Polar & Rose log = 20
+        * Cross log = 21
+        * OLE log = 22
+        * Shading log = 23
+        * Marker log = 24
+        * Breakout log = 25
+        * Bio log = 26
+        * Lineation log = 27
+        """
+        return self._dispatch.Type
+
+    @property
+    def hide_log_title(self):
+        """bool: Whether the log title is hidden."""
+        return self._dispatch.HideLogTitle
+
+    @hide_log_title.setter
+    def hide_log_title(self, value):
+        self._dispatch.HideLogTitle = value
+
+    @property
+    def hide_log_data(self):
+        """bool: Whether the log data is hidden."""
+        return self._dispatch.HideLogData
+
+    @hide_log_data.setter
+    def hide_log_data(self, value):
+        self._dispatch.HideLogData = value
+
+    @property
+    def log_background_color(self):
+        """int: The background color of the log column.
+        
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values. Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
+        """
+        return self._dispatch.LogBackgroundColor
+
+    @log_background_color.setter
+    def log_background_color(self, value):
+        self._dispatch.LogBackgroundColor = value
+
+    @property
+    def border_style(self):
+        """int: The border line style of the log column.
+        
+        Styles are specified as an integer:
+
+        * Solid = 0
+        * Dashed = 1
+        * Dotted = 2
+        * Dash-Dot = 3
+        * Dash-dot-dot = 4
+        """
+        return self._dispatch.BorderStyle
+
+    @border_style.setter
+    def border_style(self, style):
+        self._dispatch.BorderStyle = style
+
+    @property
+    def border_width(self):
+        """float: The width for the log column border in 1/10 mm."""
+        return self._dispatch.BorderWidth
+
+    @border_width.setter
+    def border_width(self, width):
+        self._dispatch.BorderWidth = width
+
+    @property
+    def border_color(self):
+        """int: The border color of the log column.
+        
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values. Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
+        """
+        return self._dispatch.BorderColor
+
+    @border_color.setter
+    def border_color(self, value):
+        self._dispatch.BorderColor = value
+
+    @property
+    def display_border(self):
+        """bool: Whether the log column border is displayed."""
+        return self._dispatch.DisplayBorder
+
+    @display_border.setter
+    def display_border(self, value):
+        self._dispatch.DisplayBorder = value
+
+    def clear_history(self):
+        """Removes all entries from the log history."""
+        self._dispatch.ClearHistory()
+
+    @property
+    def nb_of_history_item(self):
+        """int: The number of entries in the history (audit trail) of a log."""
+        return self._dispatch.NbOfHistoryItem
+
+    def history_item_date(self, index):
+        """Gets the date of the history item at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the history entry.
+        
+        Returns
+        -------
+        pywintypes.datetime
+            The timezone-aware datetime of the history item.
+        """
+        return self._dispatch.HistoryItemDate(index).replace(tzinfo=None).astimezone()
+
+    def history_item_description(self, index):
+        """Gets the description of the history item at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the history entry.
+        
+        Returns
+        -------
+        str
+            The description of the specified history entry.
+        """
+        return self._dispatch.HistoryItemDescription(index)
+
+    @property
+    def null_value(self):
+        """float: The value that is treated as ``Null`` (not displayed) in a log."""
+        return self._dispatch.NullValue
+
+    @null_value.setter
+    def null_value(self, value):
+        self._dispatch.NullValue = value
+
+    @property
+    def mask_contacts(self):
+        """bool: Whether contact lines within the log column are masked or not."""
+        return self._dispatch.MaskContacts
+
+    @mask_contacts.setter
+    def mask_contacts(self, value):
+        self._dispatch.MaskContacts = value
+
+    @property
+    def mask_horizontal_grid(self):
+        """bool: Whether the horizontal (depth) gridlines of a log are masked or not."""
+        return self._dispatch.MaskHorizontalGrid
+
+    @mask_horizontal_grid.setter
+    def mask_horizontal_grid(self, value):
+        self._dispatch.MaskHorizontalGrid = value
+
+    @property
+    def sample_rate(self):
+        """float: The sample interval of a log in current master depth units."""
+        return self._dispatch.SampleRate
+
+    @sample_rate.setter
+    def sample_rate(self, rate):
+        self._dispatch.SampleRate = rate
+
+    @property
+    def scale_low(self):
+        """float: The low value of the log scale."""
+        return self._dispatch.ScaleLow
+
+    @scale_low.setter
+    def scale_low(self, scale):
+        self._dispatch.ScaleLow = scale
+
+    @property
+    def scale_high(self):
+        """float: The high value of the log scale."""
+        return self._dispatch.ScaleHigh
+
+    @scale_high.setter
+    def scale_high(self, scale):
+        self._dispatch.ScaleHigh = scale
+
+    @property
+    def scale_mode(self):
+        """int: The horizontal scale mode (linear or logarithmic) of a log.
+
+        This property is only available for Well or Mud logs, and can have the
+        following values:
+
+        * Linear = 0
+        * Logarithmic = 1
+        """
+        return self._dispatch.ScaleMode
+
+    @scale_mode.setter
+    def scale_mode(self, mode):
+        self._dispatch.ScaleMode = mode
+
+    @property
+    def scale_reversed(self):
+        """bool: Whether the data display scale is reversed."""
+        return self._dispatch.ScaleReversed
+
+    @scale_reversed.setter
+    def scale_reversed(self, value):
+        self._dispatch.ScaleReversed = value
+
+    @property
+    def use_log_colored_background(self):
+        """bool: Whether the background color of a log is displayed."""
+        return self._dispatch.UseLogColoredBackground
+
+    @use_log_colored_background.setter
+    def use_log_colored_background(self, value):
+        self._dispatch.UseLogColoredBackground = value
+
+    @property
+    def maj_grid_enable(self):
+        """bool: Whether to display major vertical gridlines."""
+        return self._dispatch.MajGridEnable
+
+    @maj_grid_enable.setter
+    def maj_grid_enable(self, value):
+        self._dispatch.MajGridEnable = value
+
+    @property
+    def min_grid_enable(self):
+        """bool: Whether to display minor vertical gridlines."""
+        return self._dispatch.MinGridEnable
+
+    @min_grid_enable.setter
+    def min_grid_enable(self, value):
+        self._dispatch.MinGridEnable = value
+
+    @property
+    def maj_grid_spacing(self):
+        """float: The spacing between major vertical gridlines."""
+        return self._dispatch.MajGridSpacing
+
+    @maj_grid_spacing.setter
+    def maj_grid_spacing(self, spacing):
+        self._dispatch.MajGridSpacing = spacing
+
+    @property
+    def min_grid_spacing(self):
+        """float: The spacing between minor vertical gridlines."""
+        return self._dispatch.MinGridSpacing
+
+    @min_grid_spacing.setter
+    def min_grid_spacing(self, spacing):
+        self._dispatch.MinGridSpacing = spacing
+
+    @property
+    def lock_log_data(self):
+        """bool: Whether the log data is protected from editing."""
+        return self._dispatch.LockLogData
+
+    @lock_log_data.setter
+    def lock_log_data(self, value):
+        self._dispatch.LockLogData = value
+
+    def get_data(self, index):
+        """Gets the data value for the specified index.
+
+        This method is only applicable for a Well, Mud, Interval or Depth Log.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the data to be retrieved.
+        
+        Returns
+        -------
+        float
+            The value of the log data at the specified index.
+        """
+        return self._dispatch.GetData(index)
+
+    def set_data(self, index, value):
+        """Sets the data value for the specified index.
+
+        This method is only applicable for a Well, Mud, Interval or Depth Log.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the data to be retrieved.
+        value : float
+            The value you want to set the data to.
+        """
+        self._dispatch.SetData(index, value)
+
+    def get_data_at_depth(self, depth):
+        """Gets the log data value at the specified depth.
+        
+        This method is only applicable for a Well, Mud, Interval or Depth Log.
+
+        Parameters
+        ----------
+        depth : float
+            Depth value in current master depth units.
+        
+        Returns
+        -------
+        float
+            The value of the log data at the specified depth.
+        """
+        return self._dispatch.GetDataAtDepth(depth)
+
+    def set_data_at_depth(self, depth, value):
+        """Sets the log data value at the specified depth.
+
+        This method is only applicable for a Well, Mud, Interval or Depth Log.
+
+        Parameters
+        ----------
+        depth : float
+            Depth value in current master depth units.
+        value : float
+            The value you want to set the data to.
+        """
+        self._dispatch.SetDataAtDepth(depth, value)
+
+    def data_depth(self, index):
+        """Gets the log data depth for the specified index.
+        
+        This method can be called for Mud, Well, Depth, Percent, Analysis, FWS,
+        Image and RGB Logs. For logs with a constant sample step (Well, Image,
+        RGB, Analysis Logs), the index 0 corresponds to the Bottom Depth.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the data to be retrieved.
+        
+        Returns
+        -------
+        float
+            The depth of the log data at the specified index. If the index is
+            out of bounds, this will be 0.0 for a Mud Log, and an extrapolated
+            value for a Well Log.
+        """
+        return self._dispatch.DataDepth(index)
+
+    def insert_data(self, index, value):
+        """Inserts a new data value at the specified index.
+
+        If necessary existing data points will be shifted.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the new data point will be inserted. The
+            index must be lower or equal to the number of data points in the
+            log.
+        value : float
+            The new data value.
+        
+        Raises
+        ------
+        pywintypes.com_error
+            If the data couldn't be inserted (out-of-bounds index or other)
+        """
+        self._dispatch.InsertData(index, value)
+
+    def insert_data_at_depth(self, depth, value):
+        """Inserts a new data value at the specified depth.
+
+        Data points above (shallower depth) will be shifted upward to
+        accomodate the newly inserted point in a Well Log.
+
+        Parameters
+        ----------
+        depth : float
+            Depth in current master units at which the new data point should be
+            inserted. Depth is rounded to the nearest sample for Well Logs.
+        value : float
+            The new data value
+        """
+        self._dispatch.InsertDataAtDepth(depth, value)
+
+    @property
+    def formula(self):
+        """str: The mathematical formula used for a Formula log.
+        
+        Raises
+        ------
+        pywintypes.com_error
+            If, during setting, the supplied formula is invalid.
+        """
+        return self._dispatch.Formula
+
+    @formula.setter
+    def formula(self, value):
+        self._dispatch.Formula = value
+
+    @property
+    def filter(self):
+        """int: The width (in samples) of the display filter used for Well Logs."""
+        return self._dispatch.Filter
+
+    @filter.setter
+    def filter(self, value):
+        self._dispatch.Filter = value
+
+    @property
+    def fixed_bar_width(self):
+        """int: The fixed bar width, in units of 1/10 mm, for Mud Logs."""
+        return self._dispatch.FixedBarWidth
+
+    @fixed_bar_width.setter
+    def fixed_bar_width(self, width):
+        self._dispatch.FixedBarWidth = width
+
+    def insert_new_interval_item(self, top_depth, bottom_depth, value):
+        """Inserts a new interval in an Interval log.
+
+        Parameters
+        ----------
+        top_depth : float
+            The top depth of the new interval in current depth units.
+        bottom_depth : float
+            The bottom depth of the new interval in current depth units.
+        value : float
+            The value of the new interval item.
+        
+        Returns
+        -------
+        IntervalItem
+            The newly inserted interval item.
+        """
+        return IntervalItem(self._dispatch.InsertNewIntervalItem(top_depth, bottom_depth, value))
+
+    def interval_item(self, index):
+        """Gets an interval item object from an Interval Log.
+
+        Items are ordered by ascending top depth.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the interval item.
+        
+        Returns
+        -------
+        IntervalItem or None
+            The interval item at the specified index, or None if the index
+            is out of range.
+        """
+        return IntervalItem(self._dispatch.IntervalItem(index))
+
+    def interval_item_at_depth(self, depth):
+        """Gets an interval item object from an Interval Log at the specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            Depth value of the interval item, in current master depth units.
+        
+        Returns
+        -------
+        IntervalItem or None
+            The interval item at the specified depth, or None if no interval
+            item exists at the specified depth.
+        """
+        return IntervalItem(self._dispatch.IntervalItemAtDepth(depth))
+
+    @property
+    def pen_color(self):
+        """int: The pen color for a Well or Mud log.
+        
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values.  Other allowed values are : 0xFFFFFFFF (None) and 0xFF000000 (automatic color).
+        """
+        return self._dispatch.PenColor
+
+    @pen_color.setter
+    def pen_color(self, color):
+        self._dispatch.PenColor = color
+
+    @property
+    def pen_style(self):
+        """int: The pen style for the Well or Mud log.
+        
+        Styles are specified as an integer:
+
+        * Solid = 0
+        * Dashed = 1
+        * Dotted = 2
+        * Dash-Dot = 3
+        * Dash-dot-dot = 4
+        """
+        return self._dispatch.PenStyle
+
+    @pen_style.setter
+    def pen_style(self, style):
+        self._dispatch.PenStyle = style
+
+    @property
+    def pen_width(self):
+        """int: The pen width used in a Well or Mud Log in units of 1/10 mm."""
+        return self._dispatch.PenWidth
+
+    @pen_width.setter
+    def pen_width(self, width):
+        self._dispatch.PenWidth = width
+
+    def remove_data(self, index):
+        """Removes a data point from a Mud or Well Log.
+        
+        For Well Logs the data value will be set to ``Null``.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index for the data point to be removed
+        """
+        self._dispatch.RemoveData(index)
+
+    def remove_data_at_depth(self, depth):
+        """Removes a data point from a Mud or Well Log.
+        
+        All data points above (shallower depth) the removed point will be
+        shifted downward (deeper) when data is removed from a Well Log.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value (in current master units) at which the data point.
+            will be removed.
+        """
+        self._dispatch.RemoveDataAtDepth(depth)
+
+    def remove_interval_item(self, index):
+        """Removes a data interval from an Interval log.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index to specify which data interval will be removed.
+        """
+        self._dispatch.RemoveIntervalItem(index)
+
+    def remove_interval_item_at_depth(self, depth):
+        """Removes a data interval from an Interval log.
+
+        Parameters
+        ----------
+        depth : float
+            Depth value in current master units to specify which interval item
+            will be removed.
+        """
+        self._dispatch.RemoveIntervalItemAtDepth(depth)
+
+    @property
+    def shading(self):
+        """int: The shading position used in a Well or Mud Log.
+        
+        * None = 0
+        * Left = 1
+        * Right = 2
+        * Full = 3
+        """
+        return self._dispatch.Shading
+
+    @shading.setter
+    def shading(self, position):
+        self._dispatch.Shading = position
+
+    @property
+    def style(self):
+        """int: The data display style for a log.
+        
+        For Mud logs:
+
+        * Fixed Bar = 1
+        * Dynamic Bar = 2
+        * Line = 3
+        
+        For Engineering logs:
+
+        * Full = 0
+        * Left = 1
+        * Right = 2
+        """
+        return self._dispatch.Style
+
+    @style.setter
+    def style(self, style):
+        self._dispatch.Style = style
+
+    def attach_litho_dictionary(self, dictionary):
+        """Attaches a new symbol or pattern library (\*.LTH file) to Litho, CoreDesc,
+        Strata, Analysis or Percentage Log.
+
+        Parameters
+        ----------
+        dictionary : str
+            path and name of the LTH file to attach
+
+        Returns
+        -------
+            LithoDictionary
+                The LithoDictionary object
+        """
+        return LithoDictionary(self._dispatch.AttachLithoDictionary(dictionary))
+
+    def get_component_name(self, column):
+        """Gets the name (i.e. litho code) for the component used in
+        the specified data column of a Percentage or Analysis Log.
+
+        Parameters
+        ----------
+        column : int
+            Zero based index of the data column in the tabular editor for
+            which the component name should be set or retrieved.
+
+        Returns
+        -------
+        str
+            The code of the component used in the specified data
+            column of a Percentage or Analysis Log.
+        """
+        return self._dispatch.GetComponentName(column)
+
+    def set_component_name(self, column, code):
+        """Sets the name (i.e. litho code) for the component used in
+        the specified data column of a Percentage or Analysis Log.
+
+        Parameters
+        ----------
+        column : int
+            Zero based index of the data column in the tabular editor for
+            which the component name should be set or retrieved.
+        code : str
+            Code of the component to be used in the specified data
+            column of a Percentage or Analysis Log.
+        """
+        self._dispatch.SetComponentName(column, code)
+
+    def fossil_item(self, index):
+        """Gets a Fossil Item object from the CoreDesc Log at the specified index.
+
+        Items are ordered by ascending top depth.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the item to be retrieved.
+
+        Returns
+        -------
+        FossilItem or None
+            The FossilItem at the desired index or none if index is out of range.
+        """
+        return FossilItem(self._dispatch.FossilItem(index))
+
+    def fossil_item_at_depth(self, depth):
+        """Gets a fossil item object from the CoreDesc Log at the specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            depth value in current depth units at which the item will be retrieved
+
+        Returns
+        -------
+        FossilItem or None
+            The FossilItem at the desired depth or None if depth is out of range.
+        """
+        return FossilItem(self._dispatch.FossilItemAtDepth(depth))
+
+    def insert_new_fossil_item(self, top_depth, bottom_depth, litho_code, abundance, dominance, position):
+        """Inserts a new data point or interval into a Core Description Log.
+
+        Parameters
+        ----------
+        top_depth : float
+            Top depth of the new data interval in current depth units.
+        bottom_depth : float
+            Bottom depth of the new data interval in current depth units.
+        litho_code : str
+            Code of the symbol representing the feature as defined in the symbol library of the log.
+        abundance : int
+            The abundance value associated with the symbol (e.g. between 0 and 9).
+        dominance : int
+            The dominance value associated with the symbol
+            undiff = 0
+            minor = 1
+            major = 2
+        position : float
+            A value between 0 and 1 determining the horizontal position of the symbol within the log column.
+
+        Returns
+        -------
+        FossilItem
+            The newly created FossilItem.
+        """
+        return FossilItem(self._dispatch.InsertNewFossilItem(top_depth, bottom_depth, litho_code, abundance, dominance, position))
+
+    def insert_new_litho_bed(self, top_depth, bottom_depth, litho_code, value, position):
+        """Inserts a new lithology bed into a Litho Log.
+
+        Parameters
+        ----------
+        top_depth : float
+            Top depth of the new data interval in current depth units.
+        bottom_depth : float
+            Bottom depth of the new data interval in current depth units.
+        litho_code : str
+            Code of the symbol representing the feature as defined in the symbol library of the log.
+        value : float
+            Hardness value between 0 and 1.
+        position : float
+            A value between 0 and 1 determining the horizontal position of a non repeated symbol
+            in percent of the track width.
+
+        Returns
+        -------
+        LithoBed
+            The newly created LithoBed.
+        """
+        return LithoBed(self._dispatch.InsertNewLithoBed(top_depth, bottom_depth, litho_code, value, position))
+
+    def get_litho_bed(self, index):
+        """Gets a LithoBed object at the specified index from a Lithology Log.
+
+        Items are ordered by ascending top depth.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the LithoBed to retrieve.
+
+        Returns
+        -------
+        LithoBed
+            The LithoBed at the desired index.
+        """
+        return LithoBed(self._dispatch.GetLithoBed(index))
+
+    def set_litho_bed(self, index, litho_bed):
+        """Sets a LithoBed object at the specified index from another
+        LithoBed object.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the LithoBed to retrieve.
+        litho_bed : LithoBed
+            The LithoBed object to copy.
+        """
+        self._dispatch.SetLithoBed(index, litho_bed._dispatch)
+
+    def get_litho_bed_at_depth(self, depth):
+        """Gets a LithoBed object at the specified depth from a Lithology Log.
+
+        Parameters
+        ----------
+        depth : float
+            Depth value in current depth units at which the item will be retrieved.
+
+        Returns
+        -------
+        LithoBed
+            The LithoBed at the desired depth.
+        """
+        return LithoBed(self._dispatch.GetLithoBedAtDepth(depth))
+
+    def set_litho_bed_at_depth(self, depth, litho_bed):
+        """Sets a LithoBed object at the specified depth from another
+        LithoBed object.
+
+        Parameters
+        ----------
+        depth : float
+            Depth value in current depth units at which the item will be retrieved.
+        litho_bed : LithoBed
+            The LithoBed object to copy.
+        """
+        self._dispatch.SetLithoBedAtDepth(depth, litho_bed._dispatch)
+
+    @property
+    def litho_dictionary(self):
+        """LithoDictionary: The symbol library used by the log as LithoDictionary object."""
+        return LithoDictionary(self._dispatch.LithoDictionary)
+
+    @litho_dictionary.setter
+    def litho_dictionary(self, dictionary):
+        self._dispatch.LithoDictionary = dictionary._dispatch
+
+    def remove_fossil_item(self, index):
+        """Removes an item at the specified index from a CoreDesc Log.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the fossil item to be removed.
+        """
+        self._dispatch.RemoveFossilItem(index)
+
+    def remove_fossil_item_at_depth(self, depth):
+        """Removes an item at the specified index from a CoreDesc Log.
+
+        Parameters
+        ----------
+        depth : float
+            the depth value of the symbol in current depth units at which it will be removed.
+        """
+        self._dispatch.RemoveFossilItemAtDepth(depth)
+
+    def remove_litho_bed(self, index):
+        """Removes a lithology bed from the Lithology log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the lithology bed item to be removed.
+        """
+        self._dispatch.RemoveLithoBed(index)
+
+    def remove_litho_bed_at_depth(self, depth):
+        """Removes a lithology bed from the Lithology log at the specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            the depth value in current depth units at which the lithological bed will be removed.
+        """
+        self._dispatch.RemoveLithoBedAtDepth(depth)
+
+    def insert_trace(self, index):
+        """Inserts a new data trace into an Image, FWS or Analysis Log at the specified index.
+
+        Columns for the newly inserted trace are filled with No-Data
+        value. Edit them with set_trace_data or set_trace_data_at_depth.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the trace should be added.
+            Index zero represents the deepest trace.
+            The maximum allowed index is (number of traces + 1).
+            For Image and Analysis logs, existing traces will be shifted upwards depth wise.
+        """
+        self._dispatch.InsertTrace(index)
+
+    def insert_trace_at_depth(self, depth):
+        """Inserts a new data trace into an Image, FWS or Analysis or Percent Log at the specified depth.
+
+        Columns for the newly inserted trace are filled with No-Data
+        value. Edit them with set_trace_data or set_trace_data_at_depth.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the new
+            data trace will be inserted.
+            For Image and Analysis logs:
+            Insertion depth is rounded to the nearest sample.
+            Value must be within the depth range of the existing
+            traces or contiguous to that range (± 1.5 * sampling rate).
+            If necessary existing traces will be shifted upwards.
+            For Percent and FWS logs, if there is already data at that
+            depth, it is replaced with No-Data value, otherwise a trace
+            is inserted at the desired depth without shifting other
+            traces depth wise.
+
+        """
+        self._dispatch.InsertTraceAtDepth(depth)
+
+    def remove_trace(self, index):
+        """Remove an entire data trace from an Image, FWS, Analysis
+        or Percentage Log.
+
+        For Image logs, if the trace is the first or
+        the last, it is removed. Otherwise, it sets all values of that
+        trace to No-Data value.
+        For Analysis, it is the same as for Image logs, but the
+        replacement value is 0.
+        For FWS logs, it removes the trace and shifts down all above
+        traces.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the trace (0 = bottom depth).
+        """
+        self._dispatch.RemoveTrace(index)
+
+    def remove_trace_at_depth(self, depth):
+        """Remove an entire data trace from an Image, FWS, Analysis or
+        Percentage Log.
+
+        For Image logs, if the trace is the first or
+        the last, it is removed. Otherwise, it sets all values of that
+        trace to No-Data value.
+        For Analysis, it is the same as for Image logs, but the
+        replacement value is 0.
+        For FWS logs and Percent, it removes the trace and shifts down
+        all above traces.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the trace
+            will be removed or set to No-Data value.
+        """
+        self._dispatch.RemoveTraceAtDepth(depth)
+
+    def get_trace_data(self, depth_index, trace_index):
+        """Gets the data value at the specified row index and position within the trace
+        (column index) of an Analysis, Percentage, FWS, Image or RGB Log.
+
+        Parameters
+        ----------
+        depth_index : int
+            zero based index of the depth (0 = bottom depth for FWS,
+            Image, RGB and Analysis logs, top depth for Percent logs).
+        trace_index : int
+            zero based index of the column.
+
+        Returns
+        -------
+        float
+            The data value at the specified index and column.
+            The current No-Data value (e.g. -999) will be returned if
+            the depth or trace index refers to a non-existent (out of
+            index range) data point.
+        """
+        return self._dispatch.GetTraceData(depth_index, trace_index)
+
+    def set_trace_data(self, depth_index, trace_index, value):
+        """Sets the data value at the specified row index and position within the trace
+        (column index) of an Analysis, Percentage, FWS, Image or RGB Log.
+
+        Parameters
+        ----------
+        depth_index : int
+            zero based index of the depth (0 = bottom depth).
+        trace_index : int
+            zero based index of the column.
+        value : float
+            The value you want to set the data to.
+        """
+        self._dispatch.SetTraceData(depth_index, trace_index, value)
+
+    def get_trace_data_at_depth(self, depth, trace_position):
+        """Gets the data value at the specified depth and position within the trace of an Analysis,
+        Percentage, FWS, Image or RGB Log.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value at which you would like to retrieve the
+            data value in the current depth units.
+        trace_position : float
+            The position within the trace (time or angle as shown in
+            the column header of the tabular editor, not the index)
+            at which you would like to retrieve the data value.
+
+        Returns
+        -------
+        float
+            The data value at the specified depth and column.
+            The current No-Data value (e.g. -999) will be returned if
+            the depth or trace index refers to a non-existent (out of
+            index range) data point.
+        """
+        return self._dispatch.GetTraceDataAtDepth(depth, trace_position)
+
+    def set_trace_data_at_depth(self, depth, trace_position, value):
+        """set the data value at the specified depth and position within
+        the trace of an Analysis, Percentage, FWS, Image or RGB Log
+
+        Parameters
+        ----------
+        depth : float
+            The depth value at which you would like to retrieve the data value in the current depth units.
+        trace_position : float
+            The position within the trace (time or angle as shown in the column header of the tabular editor,
+            not the index) at which you would like to retrieve the data value.
+        value : float
+            The value you want to set the data to.
+        """
+        self._dispatch.SetTraceDataAtDepth(depth, trace_position, value)
+
+    @property
+    def trace_length(self):
+        """int: The length of a data trace in Image, RGB and FWS Logs.
+
+        For FWS, Analysis and Percent logs:
+        If trace_length is set to a lower value than the current one,
+        all the trace columns past the desired length are discared.
+        If trace_length is set to a higher value than the current one,
+        additional columns are filled with No-data values.
+        For Image and RGB logs:
+        If trace_length is set to a lower value than the current one,
+        trace value are resampled and averaged.
+        If trace_length is set to a higher value than the current one,
+        TODO determine behaviour here.
+        """
+        return self._dispatch.TraceLength
+
+    @trace_length.setter
+    def trace_length(self, length):
+        self._dispatch.TraceLength = length
+
+    @property
+    def trace_offset(self):
+        """float: The offset of a data trace in the FWS Log."""
+        return self._dispatch.TraceOffset
+
+    @trace_offset.setter
+    def trace_offset(self, offset):
+        self._dispatch.TraceOffset = offset
+
+    @property
+    def trace_sample_rate(self):
+        """float: The trace sample interval for a FWS Logs."""
+        return self._dispatch.TraceSampleRate
+
+    @trace_sample_rate.setter
+    def trace_sample_rate(self, rate):
+        self._dispatch.TraceSampleRate = rate
+
+    def get_column_name(self, column):
+        """Gets set the name of a Strata Log column.
+
+        Parameters
+        ----------
+        column : int
+            Zero based index of the column to be retrieved
+
+        Returns
+        -------
+        str
+            The name of the column.
+        """
+        return self._dispatch.GetColumnName(column)
+
+    def set_column_name(self, column, name):
+        """Sets set the name of a Strata Log column.
+
+        Parameters
+        ----------
+        column : int
+            Zero based index of the column to be retrieved
+        name : str
+            New name of the column.
+        """
+        self._dispatch.SetColumnName(column, name)
+
+    def comment_box(self, index):
+        """Gets the Comment Box object from the Comment Log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the box will be retrieved.
+
+        Returns
+        -------
+        CommentBox or None
+            The CommentBox at the desired index or None if index is out of range.
+        """
+        return CommentBox(self._dispatch.CommentBox(index))
+
+    def comment_box_at_depth(self, depth):
+        """Gets the Comment Box object from the Comment Log at the specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the comment box will be retrieved.
+
+        Returns
+        -------
+        CommentBox or None
+            The CommentBox at the desired depth or None if depth is out of range.
+        """
+        return CommentBox(self._dispatch.CommentBoxAtDepth(depth))
+
+    def insert_new_comment_box(self, top_depth, bottom_depth, text):
+        """Sets a new box with the specified text into a Comment Log.
+
+        Parameters
+        ----------
+        top_depth : float
+            The top of the box in current depth units.
+        bottom_depth : float
+            The bottom of the box in current depth units.
+        text : str
+            The text to be displayed in the new box.
+
+        Returns
+        -------
+        CommentBox
+            The newly created CommentBox.
+        """
+        return CommentBox(self._dispatch.InsertNewCommentBox(top_depth, bottom_depth, text))
+
+    def marker(self, index):
+        """Gets the marker with the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the marker.
+
+        Returns
+        -------
+        MarkerItem
+            The marker with the specified index.
+        """
+        return MarkerItem(self._dispatch.Marker(index))
+
+    def marker_by_name(self, name):
+        """Gets the marker with the specified name.
+
+        Parameters
+        ----------
+        name : str
+            Name of the marker to be retrieved.
+
+        Returns
+        -------
+        MarkerItem
+            The marker with the specified name.
+        """
+        return MarkerItem(self._dispatch.MarkerByName(name))
+
+    def insert_new_marker(self, depth, name, comment, contact):
+        """Inserts a new marker at the specified depth into a Marker Log
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the marker will be added.
+        name : str
+            The name (or identifier) of the marker.
+        comment : str
+            The optional comment for the marker.
+        contact : str
+            Name of a contact style to be used and available in the contact dictionary of the Marker Log.
+
+        Returns
+        -------
+        MarkerItem
+            The Marker object at the desired depth with the specified attributes.
+        """
+        return MarkerItem(self._dispatch.InsertNewMarker(depth, name, comment, contact))
+
+    def remove_comment_box(self, index):
+        """Removes a comment box from the Comment log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the comment box will be removed.
+        """
+        self._dispatch.RemoveCommentBox(index)
+
+    def remove_comment_box_at_depth(self, depth):
+        """Removes a comment box from the Comment log at the specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the comment box will be removed.
+        """
+        self._dispatch.RemoveCommentBoxAtDepth(depth)
+
+    def remove_marker(self, index):
+        """Removes the marker from a Marker Log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the marker box will be removed.
+        """
+        self._dispatch.RemoveMarker(index)
+
+    def strata_column(self, index):
+        """Gets a column from a Strata Log as Comment Log object.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index  of the column to be returned.
+
+        Returns
+        -------
+        Log
+            A comment log object.
+        """
+        return Log(self._dispatch.StrataColumn(index))
+
+    def remove_strata_column(self, index):
+        """Removes the the specified column from a Strata Log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the column to be removed.
+        """
+        self._dispatch.RemoveStrataColumn(index)
+
+    @property
+    def font(self):
+        """Gets the font used in a Comment Log as Font Object."""
+        return Font(self._dispatch.Font)
+
+    @font.setter
+    def font(self, font):
+        self._dispatch.Font = font._dispatch
+
+    def attach_attribute_dictionary(self, attribute, file):
+        """Attaches a new attribute library (\*.TAD file) to a
+        Breakout, Lineation or Structure Log.
+
+        Parameters
+        ----------
+        attribute : str
+            Name of the classification column.
+        file : str
+            Path to the TAD file to attach.
+
+        Raises
+        ------
+        pywintypes.com_error
+            If the classification column doesn't exist, an exception is raised.
+        """
+        self._dispatch.AttachAttributeDictionary(attribute, file)
+
+    def insert_new_attribute(self, attribute_name):
+        """Inserts a new blank classification column to a Breakout,
+        Lineation or Structure Log.
+
+        Parameters
+        ----------
+        attribute_name : str
+            Name of the new class.
+        """
+        self._dispatch.InsertNewAttribute(attribute_name)
+
+    def get_attribute_name(self, index):
+        """Gets the name of the attribute class (i.e. classification
+        column) in a Breakout, Lineation or Structure Log.
+
+        Parameters
+        ----------
+        index : str
+            Zero based index of the column.
+
+        Returns
+        -------
+        str
+            The name of the attribute class (classification column)
+
+        Raises
+        ------
+        pywintypes.com_error
+            If the column index points to a non existent column (out
+            of index range) an exception will be raised.
+        """
+        return self._dispatch.GetAttributeName(index)
+
+    def set_attribute_name(self, index, name):
+        """Sets the name of the attribute class (i.e. classification
+        column) in a Breakout, Lineation or Structure Log.
+
+        Parameters
+        ----------
+        index : str
+            Zero based index of the column.
+        name : str
+            New name of the classification column.
+
+        Raises
+        ------
+        pywintypes.com_error
+            If the column index points to a non existent column (out
+            of index range) an exception will be raised.
+        """
+        self._dispatch.SetAttributeName(index, name)
+
+    def structure(self, index):
+        """Gets a Structure object from the Structure Log at the
+        specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the structure object to be retrieved.
+
+        Returns
+        -------
+        Structure or None
+            The structure at the specified index. If the index is outside the valid range no exception
+            will be raised and ``None`` will be returned.
+        """
+        return Structure(self._dispatch.Structure(index))
+
+    def structure_at_depth(self, depth):
+        """Gets the closest Structure object from the Structure Log
+        to the specified depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the
+            structure object will be retrieved.
+
+        Returns
+        -------
+        Structure or None
+            The feature closest to the specified depth will be returned.
+            If the depth is outside the valid range no exception
+            will be raised and ``None`` will be returned.
+        """
+        return Structure(self._dispatch.StructureAtDepth(depth))
+
+    def insert_new_structure_ex(self, depth, azimuth, dip, aperture):
+        """Sets a new structure in a Structure Log.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in the current units of the breakout structure to
+            be inserted.
+        azimuth : float
+            The azimuth angle of the structure measured in degrees.
+        dip : float
+            The tilt angle of the structure measured in degrees.
+        aperture : float
+            The aperture of the structure in meters.
+
+        Returns
+        -------
+        Structure
+            The newly created structure object.
+        """
+        return Structure(self._dispatch.InsertNewStructureEx(depth, azimuth, dip, aperture))
+
+    def remove_structure(self, index):
+        """Removes a structure from the Structure Log at the
+        specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the structure to be removed.
+        """
+        self._dispatch.RemoveStructure(index)
+
+    def remove_structure_at_depth(self, depth):
+        """Removes a structure from the Structure Log at the
+        specified depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the
+            structure will be removed.
+        """
+        self._dispatch.RemoveStructureAtDepth(depth)
+
+    def breakout(self, index):
+        """Gets a breakout structure from the Breakout Log at the specified
+        index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the breakout to be retrieved.
+
+        Returns
+        -------
+        Structure or None
+            The breakout at the specified index. If the index is
+            outside the valid range no exception will be raised and
+            ``None`` will be returned.
+
+        """
+        return Structure(self._dispatch.Breakout(index))
+
+    def breakout_at_depth(self, depth):
+        """Gets a breakout structure from the Breakout Log at the specified
+        depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the
+            breakout will be retrieved.
+
+        Returns
+        -------
+        Structure or None
+            The feature closest to the specified depth will be returned.
+            If the depth is outside the valid range no exception
+            will be raised and ``None`` will be returned.
+        """
+        return Structure(self._dispatch.BreakoutAtDepth(depth))
+
+    def insert_new_breakout_ex(self, depth, azimuth, tilt, length, opening):
+        """Sets a new breakout structure in a Breakout Log.
+
+        If the mirror option is active, a second breakout structure object is
+        added 180° degrees apart.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value of the breakout structure in current depth units.
+        azimuth : float
+            The azimuth angle of the breakout structure measured in degrees.
+        tilt : float
+            The tilt angle of the breakout structure measured in degrees.
+        length : float
+            The length of the breakout structure in meters.
+        opening : float
+            The opening (or aperture) angle of the breakout structure in degrees.
+
+        Returns
+        -------
+        Structure
+            The newly created breakout structure.
+        """
+        return Structure(self._dispatch.InsertNewBreakoutEx(depth, azimuth, tilt, length, opening))
+
+    def remove_breakout(self, index):
+        """Removes a breakout structure from the Breakout Log at the specified
+        index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the breakout structure to be removed.
+        """
+        self._dispatch.RemoveBreakout(index)
+
+    def remove_breakout_at_depth(self, depth):
+        """Removes a breakout structure from the Breakout Log at the specified
+        depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the
+            breakout structure will be removed.
+        """
+        self._dispatch.RemoveBreakoutAtDepth(depth)
+    
+    def lineation(self, index):
+        """Gets a lineation pick from the Lineation Log at the specified
+        index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the lineation to be retrieved.
+
+        Returns
+        -------
+        Structure or None
+            The lineation at the specified index. If the index is
+            outside the valid range no exception will be raised and
+            ``None`` will be returned.
+        """
+        return Structure(self._dispatch.Lineation(index))
+
+    def lineation_at_depth(self, depth):
+        """Gets a lineation structure from the Lineation Log at the specified
+        depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the
+            lineation will be retrieved.
+
+        Returns
+        -------
+        Structure or None
+            The feature closest to the specified depth will be returned.
+            If the depth is outside the valid range no exception
+            will be raised and ``None`` will be returned.
+        """
+        return Structure(self._dispatch.LineationAtDepth(depth))
+
+    def insert_new_lineation_ex(self, depth, trend, plunge, eccentricity):
+        """Sets a new linear structure in a Lineation Log.
+
+        Parameters
+        ----------
+        depth : float
+            Depth of the mid-point of the fitted line in current depth units.
+        trend : float
+            Trend direction of the vector in degrees.
+        plunge : float
+            "Dip" angle of the vector in degrees.
+        eccentricity : float
+            Offset of the lineation from the center of the borehole.
+            A value between -1 and 1 can be set. An eccentricity of 0
+            corresponds to a line going straight through the center
+            of the borehole.
+
+        Returns
+        -------
+        Structure
+            The newly created lineation structure.
+        """
+        return Structure(self._dispatch.InsertNewLineationEx(depth, trend, plunge, eccentricity))
+
+    def remove_lineation(self, index):
+        """Removes a lineation from the Lineation Log at the
+        specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the lineation to be removed.
+        """
+        self._dispatch.RemoveLineation(index)
+
+    def remove_lineation_at_depth(self, depth):
+        """Removes a lineation from the Lineation Log at the
+        specified depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth value in current depth units at which the
+            lineation will be removed.
+        """
+        self._dispatch.RemoveLineationAtDepth(depth)
+
+    @property
+    def length_unit(self):
+        """float: The conversion factor (from meters) for the
+        breakout structure length measured in the breakout log
+
+        Set it to 0.001 when measured in mm and to 0.0254 when
+        measured in inches."""
+        return self._dispatch.LengthUnit
+
+    @length_unit.setter
+    def length_unit(self, factor):
+        self._dispatch.LengthUnit = factor
+
+    @property
+    def caliper_unit(self):
+        """float: The conversion factor (from meters) for the caliper
+        value in a structure log.
+
+        Set it to 0.001 when measured in mm and to 0.0254 when
+        measured in inches."""
+        return self._dispatch.CaliperUnit
+
+    @caliper_unit.setter
+    def caliper_unit(self, factor):
+        self._dispatch.CaliperUnit = factor
+
+    @property
+    def aperture_unit(self):
+        """float: The conversion factor (from meters) for the 
+        aperture value in a structure log.  
+
+        Set it to 0.001 when measured in mm and to 0.00254 when
+        measured in 1/10th inches."""
+        return self._dispatch.ApertureUnit
+
+    @aperture_unit.setter
+    def aperture_unit(self, factor):
+        self._dispatch.ApertureUnit = factor
+
+    def insert_new_schmit_box(self, top_depth, bottom_depth, text):
+        """Inserts a new box into a Polar & Rose Log.
+
+        Parameters
+        ----------
+        top_depth : float
+            The top depth value of the interval in the current depth units.
+        bottom_depth : float
+            The bottom depth value of the interval in the current depth units.
+        text : string
+            A text description which is only shown in the tabular editor display.
+
+        Returns
+        -------
+        PolarAndRoseBox
+            The newly created Polar & Rose box.
+        """
+        return PolarAndRoseBox(self._dispatch.InsertNewSchmitBox(top_depth, bottom_depth, text))
+
+    def schmit_box(self, index):
+        """Gets a box object from the Polar & Rose Log at the
+        specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the box to be returned.
+
+        Returns
+        -------
+        PolarAndRoseBox
+            The Polar & Rose box at the desired index.
+        """
+        return PolarAndRoseBox(self._dispatch.SchmitBox(index))
+
+    def schmit_box_at_depth(self, depth):
+        """Gets a box object from the Polar & Rose Log
+        at the specified depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth of the box to be returned in current depth units.
+
+        Returns
+        -------
+        PolarAndRoseBox
+            The Polar & Rose box at the desired depth.
+        """
+        return PolarAndRoseBox(self._dispatch.SchmitBoxAtDepth(depth))
+
+    def remove_schmit_box(self, index):
+        """Removes a box from the Polar & Rose Log at the
+        specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the Polar & Rose box to be removed.
+        """
+        self._dispatch.RemoveSchmitBox(index)
+
+    def remove_schmit_box_at_depth(self, depth):
+        """Removes a box from the Polar & Rose log at the specified
+        depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth of the Polar & Rose box to be removed in
+            current depth units.
+        """
+        self._dispatch.RemoveSchmitBoxAtDepth(depth)
+
+    def cross_box(self, index):
+        """Gets a Cross Box object from the Cross Section Log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the box to be retrieved.
+
+        Returns
+        -------
+        CrossSectionBox or None
+            The CrossSectionBox at the desired index or None if index is out of range.
+        """
+        return CrossSectionBox(self._dispatch.CrossBox(index))
+
+    def cross_box_at_depth(self, depth):
+        """Gets a Cross Box object from the Cross Section Log at the specified depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth of the box to be retrieved in current depth units.
+
+        Returns
+        -------
+        CrossSectionBox or None
+            The CrossSectionBox at the desired index or None if the index is out of range.
+        """
+        return CrossSectionBox(self._dispatch.CrossBoxAtDepth(depth))
+
+    def insert_new_cross_box(self, top_depth, bottom_depth):
+        """Inserts a new box into the Cross Section Log.
+
+        Parameters
+        ----------
+        top_depth : float
+            The top depth value of the cross section box in current depth units.
+        bottom_depth : float
+            The bottom depth value of the cross section box in current depth units.
+
+        Returns
+        -------
+        CrossSectionBox
+            The newly created CrossSectionBox.
+        """
+        return CrossSectionBox(self._dispatch.InsertNewCrossBox(top_depth, bottom_depth))
+
+    def remove_cross_box(self, index):
+        """Removes a box from the Cross Section Log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the box to be removed.
+        """
+        self._dispatch.RemoveCrossBox(index)
+
+    def remove_cross_box_at_depth(self, depth):
+        """Removes a box from the Cross Section Log at the specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            The depth in current units at which the box will be removed.
+        """
+        self._dispatch.RemoveCrossBoxAtDepth(depth)
+
+    def insert_new_stack_item(self, top_depth, bottom_depth, top_width, bottom_width):
+        """Inserts a new data interval into a Stacking Pattern Log.
+
+        Parameters
+        ----------
+        top_depth : float
+            The top depth value of the interval in the current depth units.
+        bottom_depth : float
+            The bottom depth value of the interval in the current depth units.
+        top_width : float
+           Width value at the top of the new interval.
+        bottom_width : float
+            Width value at the bottom of the new interval.
+
+        Returns
+        -------
+        StackingPatternItem
+            The newly created StackingPatternItem.
+        """
+        return StackingPatternItem(self._dispatch.InsertNewStackItem(top_depth, bottom_depth, top_width, bottom_width))
+
+    def stack_item(self, index):
+        """Gets a Stack Item object from the Stacking Pattern Log at the specified depth index.
+
+        Items are ordered by ascending top depth.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the item to be retrieved.
+
+        Returns
+        -------
+        StackingPatternItem or None
+            The StackingPatternItem at the desired index or None if the index is out of range.
+        """
+        return StackingPatternItem(self._dispatch.StackItem(index))
+
+    def stack_item_at_depth(self, depth):
+        """Gets a Stack Item object from the Stacking Pattern Log at the specified depth in current depth units.
+
+        Parameters
+        ----------
+        depth : float
+            The depth of the item to be retrieved in current depth units.
+
+        Returns
+        -------
+        StackingPatternItem or None
+            The StackingPatternItem at the desired depth or None if depth is out of range.
+        """
+        return StackingPatternItem(self._dispatch.StackItemAtDepth(depth))
+
+    def remove_stack_item(self, index):
+        """Removes an item from the Stacking Pattern Log at the specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index  of the stacking pattern box to be removed.
+        """
+        self._dispatch.RemoveStackItem(index)
+
+    def remove_stack_item_at_depth(self, depth):
+        """Removes an item from the Stacking Pattern Log at the specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            The depth of the stack item to be removed in current depth units.
+        """
+        self._dispatch.RemoveStackItemAtDepth(depth)
+
+    @property
+    def used_as_depth_scale(self):
+        """bool: Whether the Depth Log is used as the current depth
+        reference axis."""
+        return self._dispatch.UsedAsDepthScale
+
+    @used_as_depth_scale.setter
+    def used_as_depth_scale(self, mode):
+        self._dispatch.UsedAsDepthScale = mode
+
+    def insert_new_ole_box_from_file(self, file_name, allow_picture, top_depth, bottom_depth):
+        """Inserts a new OLE object between the specified interval
+        into an OLE Log.
+
+        OLE objects can be files such as images, Excel charts,
+        Word documents or pdfs.
+
+        Parameters
+        ----------
+        file_name : str
+            Path and name of the file to be loaded.
+        allow_picture : bool
+            Set to True to allow graphic files to be displayed using
+            an internal viewer.
+        top_depth : float
+            Top depth of the OLE object in current depth units.
+        bottom_depth : float
+            Bottom depth of the OLE object in current depth units.
+        """
+        self._dispatch.InsertNewOleBoxFromFile(file_name, allow_picture, top_depth, bottom_depth)
+
+    def drill_item(self, index):
+        """Gets a Drill Item object from the Engineering Log at the
+        specified index.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the drill item will be retrieved.
+
+        Returns
+        -------
+        DrillItem
+            The drill item at the specified index.
+        """
+        return DrillItem(self._dispatch.DrillItem(index))
+
+    def drill_item_at_depth(self, depth):
+        """Gets a Drill Item object from the Engineering Log at the
+        specified depth.
+
+        Parameters
+        ----------
+        depth : float
+            The depth of the item to be retrieved in current depth
+            units.
+
+        Returns
+        -------
+        DrillItem
+            The drill item at the specified depth.
+        """
+        return DrillItem(self._dispatch.DrillItemAtDepth(depth))
+
+    def eqp_item(self, index):
+        """Gets an Equipment Item object at the specified index from
+        the Engineering Log.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the item will be retrieved.
+
+        Returns
+        -------
+        EquipmentItem
+            The equipment item at the specified index.
+        """
+        return EquipmentItem(self._dispatch.EqpItem(index))
+
+    @property
+    def comment_style(self):
+        """int: The position of the comment associated with an engineering log.
+
+        The following styles are available:
+
+            * 0 = None, comment is not displayed
+            * 1 = Left, comment displayed on the left of the engineering log
+            * 2 = Right, comment displayed on the right of the engineering log
+        """
+        return self._dispatch.CommentStyle
+
+    @comment_style.setter
+    def comment_style(self, style):
+        self._dispatch.CommentStyle = style
+
+    @property
+    def ground_depth(self):
+        """float: The starting point (reference datum) of the
+        borehole."""
+        return self._dispatch.GroundDepth
+
+    @ground_depth.setter
+    def ground_depth(self, starting_point):
+        self._dispatch.GroundDepth = starting_point
+
+    @property
+    def diameter_high(self):
+        """float: The maximum diameter scaling value
+        (width of the log column) for an Engineering Log."""
+        return self._dispatch.DiameterHigh
+
+    @diameter_high.setter
+    def diameter_high(self, diameter):
+        self._dispatch.DiameterHigh = diameter
+
+    def insert_new_drill_item(self, bottom_depth, diameter):
+        """Inserts a new drill item into the Engineering Log.
+
+        Item index are ordered by depth value in the stack of drill
+        items.
+
+        Parameters
+        ----------
+        bottom_depth : float
+            The bottom depth of the borehole in current depth units.
+            (The top depth is either the ground_depth or the former
+            bottom depth).
+        diameter : float
+            The diameter of the borehole.
+
+        Returns
+        -------
+        DrillItem
+            The inserted DrillItem
+        """
+        return DrillItem(self._dispatch.InsertNewDrillItem(bottom_depth, diameter))
+
+    def insert_new_eqp_item(self, top_depth, bottom_depth, name):
+        """Inserts a new equipment item of the specified name and
+        depth interval into the Engineering Log.
+
+        The new item is given the last index in the list of equipment
+        items.
+
+        Parameters
+        ----------
+        top_depth : float
+            The top depth of the equipment item interval
+            in current units.
+        bottom_depth : float
+            The bottom depth of the equipment item interval
+            in current units.
+        name : str
+            The name (code) of the equipment item to be inserted.
+            Base available equipments names are listed below, but you
+            can modify or add your own in the Equipment dictionary.
+
+                * PlainCasing
+                * WireWoundCasing
+                * SlottedCasing
+                * PerforatedCasing
+                * Centralizer
+                * Shoe
+                * Packer
+                * Water
+                * Wedge
+                * HeadWorks
+                * Transducer
+                * Gauge
+                * Cement
+                * Gravel
+                * NormalThread
+                * ReverseThread
+                * Plug
+
+            If an invalid name is provided, no item will be inserted.
+
+        Returns
+        -------
+        EqpItem
+            The inserted EqpItem
+        """
+        return EquipmentItem(self._dispatch.InsertNewEqpItem(top_depth, bottom_depth, name))
+
+    @property
+    def nb_of_drill_item(self):
+        """int: The number of drill items in an Engineering Log."""
+        return self._dispatch.NbOfDrillItem
+
+    @property
+    def nb_of_eqp_item(self):
+        """int: The number of equipment items in an Engineering Log."""
+        return self._dispatch.NbOfEqpItem
+
+    def remove_drill_item(self, index):
+        """Removes the drill item at the specified index from an
+        Engineering Log.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the item will be removed.
+        """
+        self._dispatch.RemoveDrillItem(index)
+
+    def remove_eqp_item(self, index):
+        """Removes an equipment item at the specified depth index
+        from an Engineering Log.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index at which the item will be removed.
+        """
+        self._dispatch.RemoveEqpItem(index)
+
+    @property
+    def background_color(self):
+        """int: The background color of the engineering log.
+
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values.
+        """
+        return self._dispatch.BackgroundColor
+
+    @background_color.setter
+    def background_color(self, value):
+        self._dispatch.BackgroundColor = value
+
+
+    @property
+    def background_hatch_style(self):
+        """int: The background hatch style for the Engineering Log.
+
+        Available styles are:
+
+        * 0: horizontal
+        * 1: vertical
+        * 2: forward diagonal
+        * 3: backward diagonal
+        * 4: cross
+        * 5: diagonal cross
+
+        If an invalid style is set, nothing will happen.
+        """
+        return self._dispatch.BackgroundHatchStyle
+
+    @background_hatch_style.setter
+    def background_hatch_style(self, code):
+        self._dispatch.BackgroundHatchStyle = code
+
+    @property
+    def background_style(self):
+        """int: The background style for the Engineering Log.
+
+        Available styles are:
+
+        * 0: none
+        * 1: solid
+        * 2: hatch
+
+        If an invalid style is set, nothing will happen.
+        """
+        return self._dispatch.BackgroundStyle
+
+    @background_style.setter
+    def background_style(self, code):
+        self._dispatch.BackgroundStyle = code
+
+    def allow_export_attribute_dictionary(self, index, export, password):
+        """When dealing with a protected document you can use this method to enable/disable the option
+        to export the tadpole dictionary (\*.TAD) from a specific classification column of a Structure or
+        Breakout Log. This assumes you are in possession of the password.
+
+        Parameters
+        ----------
+        index : int
+            Zero based index of the classification column for which the protection level should eb changed.
+        export : bool
+            Set this boolean to True to allow an export as \*.tad file. Set it to False to protect the dictionary.
+        password : str
+            the password needed to make changes to the protection level.
+        """
+        self._dispatch.AllowExportAttributeDictionary(index, export, password)
+
+    def allow_export_litho_dictionary(self, export, password):
+        """When dealing with a protected document you can use this method to enable / disable the option
+        to export the symbol dictionary (\*.LTH) of a log. This assumes you are in possession of the password.
+
+        Parameters
+        ----------
+        export : bool
+            Set this boolean to True to allow the dictionary export. Set it to False to protect the dictionary.
+        password : str
+            the password needed to make changes to the protection level.
+        """
+        self._dispatch.AllowExportLithoDictionary(export, password)
+
+    def allow_modify_log_data(self, export, password):
+        """When dealing with a protected document you can use this method to enable / disable the option
+        to edit the data of a log. This assumes you are in possession of the password.
+
+        Parameters
+        ----------
+        export : bool
+            Set this boolean to True to allow the modification of log data. Set it to False to protect the data.
+        password : str
+            the password needed to make changes to the protection level.
+        """
+        self._dispatch.AllowModifyLogData(export, password)
+
+    def allow_modify_log_settings(self, export, password):
+        """When dealing with a protected document you can use this method to enable / disable the option
+        to change the settings of a log. This assumes you are in possession of the password.
+
+        Parameters
+        ----------
+        export : bool
+            Set this boolean to True to allow access to the log settings. Set it to False to protect the log settings.
+        password : str
+            the password needed to make changes to the protection level.
+        """
+        self._dispatch.AllowModifyLogSettings(export, password)
+
+    def allow_use_formula(self, export, password):
+        """When dealing with a protected document you can use this method to enable / disable the option
+        to access and use the formula in a Formula Log. This assumes you are in possession of the password.
+
+        Parameters
+        ----------
+        export : bool
+            Set this boolean to True to allow access the formula. Set it to False to protect the formula.
+        password : str
+            the password needed to make changes to the protection level.
+        """
+        self._dispatch.AllowUseFormula(export, password)
+
+    def allow_view_formula(self, export, password):
+        """When dealing with a protected document you can use this method to enable / disable the option
+        to see the formula used in a Formula Log. This assumes you are in possession of the password.
+
+        Parameters
+        ----------
+        export : bool
+            Set this boolean to True to see the formula. Set it to False to protect the formula.
+        password : str
+            the password needed to make changes to the protection level.
+        """
+        self._dispatch.AllowViewFormula(export, password)
+
+    def allow_view_log_history(self, export, password):
+        """When dealing with a protected document you can use this method to enable / disable the option
+        to view the log history. This assumes you are in possession of the password.
+
+        Parameters
+        ----------
+        export : bool
+            Set this boolean to True to access the log history. Set it to False to protect the log history.
+        password : str
+            the password needed to make changes to the protection level.
+        """
+        self._dispatch.AllowViewLogHistory(export, password)
```

### Comparing `pywellcad-0.2.0/wellcad/com/_odbc.py` & `pywellcad-0.2.1/wellcad/com/_odbc.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-class Odbc(DispatchWrapper):
-    """ An ODBC object allows interaction with databases from within WellCAD.
-
-    Example
-    -------
-    >>> odbc = borehole.odbc
-    >>> odbc.interpret_sql_statement('$dsn = OpenDatabase(Test, Admin)')
-    >>> odbc.interpret_sql_statement('$log = SELECT Depth, Value FROM tblGamma')
-    """
-
-    def interpret_sql_statement(self, statement):
-        """Executes the SQL statement provided
-
-        A user manual documenting the syntax of the SQL statements that can be
-        used can be obtained by contacting support@alt.lu.
-
-        Parameters
-        ----------
-        statement : str
-            The SQL statement to execute.
-
-        Returns
-        -------
-        bool
-            Whether the statement executed successfully.
-        """
-        return self._dispatch.InterpretSQLStatement(statement)
+from ._dispatch_wrapper import DispatchWrapper
+
+class Odbc(DispatchWrapper):
+    """ An ODBC object allows interaction with databases from within WellCAD.
+
+    Example
+    -------
+    >>> odbc = borehole.odbc
+    >>> odbc.interpret_sql_statement('$dsn = OpenDatabase(Test, Admin)')
+    >>> odbc.interpret_sql_statement('$log = SELECT Depth, Value FROM tblGamma')
+    """
+
+    def interpret_sql_statement(self, statement):
+        """Executes the SQL statement provided
+
+        A user manual documenting the syntax of the SQL statements that can be
+        used can be obtained by contacting support@alt.lu.
+
+        Parameters
+        ----------
+        statement : str
+            The SQL statement to execute.
+
+        Returns
+        -------
+        bool
+            Whether the statement executed successfully.
+        """
+        return self._dispatch.InterpretSQLStatement(statement)
```

### Comparing `pywellcad-0.2.0/wellcad/com/_page.py` & `pywellcad-0.2.1/wellcad/com/_page.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class Page(DispatchWrapper):
-    """ The Page class manages properties for the document print out.
-
-    Example
-    -------
-    >>> import wellcad.com
-    >>> app = wellcad.com.Application()
-    >>> app.new_borehole()
-    <wellcad.com._borehole.Borehole object at 0x0000018B3DAF9D30>
-    >>> borehole = app.get_active_borehole()
-    >>> page = borehole.page
-    """
-
-    @property
-    def depth_range(self):
-        """int : Identify the depth range mode
-
-        The available modes are the following:
-
-        * 0 = depth range not defined (maximum depth range to be printed)
-        * 1 = depth range defined by the user
-        """
-        return self._dispatch.DepthRange
-
-    @depth_range.setter
-    def depth_range(self, mode):
-        self._dispatch.DepthRange = mode
-
-    @property
-    def document_height(self):
-        """float: The document height in mm."""
-        return self._dispatch.DocumentHeight
-
-    @property
-    def document_width(self):
-        """float: The document width in mm."""
-        return self._dispatch.DocumentWidth
-
-    @document_width.setter
-    def document_width(self, value):
-        self._dispatch.DocumentWidth = value
-
-    @property
-    def nb_of_depth_range(self):
-        """double: The number of defined depth ranges."""
-        return self._dispatch.NbOfDepthRange
-
-    @property
-    def paper_mode(self):
-        """int: 0 for page-by-page and 1 for fanfold."""
-        return self._dispatch.PaperMode
-
-    @paper_mode.setter
-    def paper_mode(self, mode):
-        self._dispatch.PaperMode = mode
-
-    @property
-    def print_titles_on_top(self):
-        """bool: Show the log titles at the top of the printout."""
-        return self._dispatch.PrintTitlesOnTop
-
-    @print_titles_on_top.setter
-    def print_titles_on_top(self, show):
-        self._dispatch.PrintTitlesOnTop = show
-
-    @property
-    def print_titles_on_bottom(self):
-        """bool: Show the log titles at the bottom of the printout."""
-        return self._dispatch.PrintTitlesOnBottom
-
-    @print_titles_on_bottom.setter
-    def print_titles_on_bottom(self, show):
-        self._dispatch.PrintTitlesOnBottom = show
-
-    @property
-    def print_titles_on_bottom_on_each_page(self):
-        """bool: Repeat the log titles at the bottom of each printed page."""
-        return self._dispatch.PrintTitlesOnBottomOnEachPage
-
-    @print_titles_on_bottom_on_each_page.setter
-    def print_titles_on_bottom_on_each_page(self, show):
-        self._dispatch.PrintTitlesOnBottomOnEachPage = show
-
-    @property
-    def print_titles_on_top_on_each_page(self):
-        """bool: Repeat the log titles at the top of each printed page."""
-        return self._dispatch.PrintTitlesOnTopOnEachPage
-
-    @print_titles_on_top_on_each_page.setter
-    def print_titles_on_top_on_each_page(self, flag):
-        self._dispatch.PrintTitlesOnTopOnEachPage = flag
-
-    @property
-    def top_margin(self):
-        """int: The top margin of the page to print in mm."""
-        return self._dispatch.TopMargin
-
-    @top_margin.setter
-    def top_margin(self, value):
-        self._dispatch.TopMargin = value
-
-    @property
-    def bottom_margin(self):
-        """int: The bottom margin of the page to print in mm."""
-        return self._dispatch.BottomMargin
-
-    @bottom_margin.setter
-    def bottom_margin(self, value):
-        self._dispatch.BottomMargin = value
-
-    @property
-    def left_margin(self):
-        """int: The left margin of the page to print in mm."""
-        return self._dispatch.LeftMargin
-
-    @left_margin.setter
-    def left_margin(self, value):
-        self._dispatch.LeftMargin = value
-
-    @property
-    def right_margin(self):
-        """int: The right margin of the page to print in mm."""
-        return self._dispatch.RightMargin
-
-    @right_margin.setter
-    def right_margin(self, value):
-        self._dispatch.RightMargin = value
-
-    @property
-    def numbering(self):
-        """int: The page numbering mode
-
-        The available modes are the following:
-
-        * 0 = none
-        * 1 = left
-        * 2 = right
-        * 3 = center
-        * 4 = alternating
-        """
-        return self._dispatch.Numbering
-
-    @numbering.setter
-    def numbering(self, mode):
-        self._dispatch.Numbering = mode
-
-    @property
-    def print_header(self):
-        """bool: Option to print the document header or not."""
-        return self._dispatch.PrintHeader
-
-    @print_header.setter
-    def print_header(self, flag):
-        self._dispatch.PrintHeader = flag
-
-    def add_depth_range(self, top, bottom):
-        """Adds a new depth range to be printed in current master depth units.
-        
-        Parameters
-        ----------
-        top : float
-            Top depth of the interval that will be added to the print list.
-        bottom : float
-            Bottom depth of the interval that will be added to the print list.
-        """
-        return self._dispatch.AddDepthRange(top, bottom)
-
-    def remove_depth_range(self, index):
-        """Remove an entry from the list of depth ranges.
-        
-        Parameters
-        ----------
-        index : int
-            Zero based index of the entry to be removed from the list.
-        """
-        return self._dispatch.RemoveDepthRange(index)
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class Page(DispatchWrapper):
+    """ The Page class manages properties for the document print out.
+
+    Example
+    -------
+    >>> import wellcad.com
+    >>> app = wellcad.com.Application()
+    >>> app.new_borehole()
+    <wellcad.com._borehole.Borehole object at 0x0000018B3DAF9D30>
+    >>> borehole = app.get_active_borehole()
+    >>> page = borehole.page
+    """
+
+    @property
+    def depth_range(self):
+        """int : Identify the depth range mode
+
+        The available modes are the following:
+
+        * 0 = depth range not defined (maximum depth range to be printed)
+        * 1 = depth range defined by the user
+        """
+        return self._dispatch.DepthRange
+
+    @depth_range.setter
+    def depth_range(self, mode):
+        self._dispatch.DepthRange = mode
+
+    @property
+    def document_height(self):
+        """float: The document height in mm."""
+        return self._dispatch.DocumentHeight
+
+    @property
+    def document_width(self):
+        """float: The document width in mm."""
+        return self._dispatch.DocumentWidth
+
+    @document_width.setter
+    def document_width(self, value):
+        self._dispatch.DocumentWidth = value
+
+    @property
+    def nb_of_depth_range(self):
+        """double: The number of defined depth ranges."""
+        return self._dispatch.NbOfDepthRange
+
+    @property
+    def paper_mode(self):
+        """int: 0 for page-by-page and 1 for fanfold."""
+        return self._dispatch.PaperMode
+
+    @paper_mode.setter
+    def paper_mode(self, mode):
+        self._dispatch.PaperMode = mode
+
+    @property
+    def print_titles_on_top(self):
+        """bool: Show the log titles at the top of the printout."""
+        return self._dispatch.PrintTitlesOnTop
+
+    @print_titles_on_top.setter
+    def print_titles_on_top(self, show):
+        self._dispatch.PrintTitlesOnTop = show
+
+    @property
+    def print_titles_on_bottom(self):
+        """bool: Show the log titles at the bottom of the printout."""
+        return self._dispatch.PrintTitlesOnBottom
+
+    @print_titles_on_bottom.setter
+    def print_titles_on_bottom(self, show):
+        self._dispatch.PrintTitlesOnBottom = show
+
+    @property
+    def print_titles_on_bottom_on_each_page(self):
+        """bool: Repeat the log titles at the bottom of each printed page."""
+        return self._dispatch.PrintTitlesOnBottomOnEachPage
+
+    @print_titles_on_bottom_on_each_page.setter
+    def print_titles_on_bottom_on_each_page(self, show):
+        self._dispatch.PrintTitlesOnBottomOnEachPage = show
+
+    @property
+    def print_titles_on_top_on_each_page(self):
+        """bool: Repeat the log titles at the top of each printed page."""
+        return self._dispatch.PrintTitlesOnTopOnEachPage
+
+    @print_titles_on_top_on_each_page.setter
+    def print_titles_on_top_on_each_page(self, flag):
+        self._dispatch.PrintTitlesOnTopOnEachPage = flag
+
+    @property
+    def top_margin(self):
+        """int: The top margin of the page to print in mm."""
+        return self._dispatch.TopMargin
+
+    @top_margin.setter
+    def top_margin(self, value):
+        self._dispatch.TopMargin = value
+
+    @property
+    def bottom_margin(self):
+        """int: The bottom margin of the page to print in mm."""
+        return self._dispatch.BottomMargin
+
+    @bottom_margin.setter
+    def bottom_margin(self, value):
+        self._dispatch.BottomMargin = value
+
+    @property
+    def left_margin(self):
+        """int: The left margin of the page to print in mm."""
+        return self._dispatch.LeftMargin
+
+    @left_margin.setter
+    def left_margin(self, value):
+        self._dispatch.LeftMargin = value
+
+    @property
+    def right_margin(self):
+        """int: The right margin of the page to print in mm."""
+        return self._dispatch.RightMargin
+
+    @right_margin.setter
+    def right_margin(self, value):
+        self._dispatch.RightMargin = value
+
+    @property
+    def numbering(self):
+        """int: The page numbering mode
+
+        The available modes are the following:
+
+        * 0 = none
+        * 1 = left
+        * 2 = right
+        * 3 = center
+        * 4 = alternating
+        """
+        return self._dispatch.Numbering
+
+    @numbering.setter
+    def numbering(self, mode):
+        self._dispatch.Numbering = mode
+
+    @property
+    def print_header(self):
+        """bool: Option to print the document header or not."""
+        return self._dispatch.PrintHeader
+
+    @print_header.setter
+    def print_header(self, flag):
+        self._dispatch.PrintHeader = flag
+
+    def add_depth_range(self, top, bottom):
+        """Adds a new depth range to be printed in current master depth units.
+        
+        Parameters
+        ----------
+        top : float
+            Top depth of the interval that will be added to the print list.
+        bottom : float
+            Bottom depth of the interval that will be added to the print list.
+        """
+        return self._dispatch.AddDepthRange(top, bottom)
+
+    def remove_depth_range(self, index):
+        """Remove an entry from the list of depth ranges.
+        
+        Parameters
+        ----------
+        index : int
+            Zero based index of the entry to be removed from the list.
+        """
+        return self._dispatch.RemoveDepthRange(index)
```

### Comparing `pywellcad-0.2.0/wellcad/com/_polar_and_rose_box.py` & `pywellcad-0.2.1/wellcad/com/_polar_and_rose_box.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class PolarAndRoseBox(DispatchWrapper):
-    """A polar or rose diagram with annotations. These diagrams or "boxes" are stored in a Polar & Rose Log.
-
-    Polar & Rose boxes are sometimes refered to as Schmit boxes (see example below)
-
-    Example
-    -------
-    >>> log = borehole.log("Rose Diagram")
-    >>> box = log.schmit_box_at_depth(10.5)  # Polar & Rose box called schmit box
-    >>> box.text
-    "Intervals Automatically Determined"
-    """
-
-    @property
-    def top_depth(self):
-        """float: The top depth of the Polar & Rose box in current
-        depth reference units.
-        """
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of the Polar & Rose box in current
-        depth reference units.
-        """
-        return self._dispatch.BottomDepth
-
-    @property
-    def text(self):
-        """str: The text for a Polar & Rose Log box.
-
-        The text is not displayed in the plot and is only visible in
-        the tabular editor or when exporting the data.
-        """
-        return self._dispatch.Text
-
-    @text.setter
-    def text(self, value):
-        self._dispatch.Text = value
-
-
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class PolarAndRoseBox(DispatchWrapper):
+    """A polar or rose diagram with annotations. These diagrams or "boxes" are stored in a Polar & Rose Log.
+
+    Polar & Rose boxes are sometimes refered to as Schmit boxes (see example below)
+
+    Example
+    -------
+    >>> log = borehole.log("Rose Diagram")
+    >>> box = log.schmit_box_at_depth(10.5)  # Polar & Rose box called schmit box
+    >>> box.text
+    "Intervals Automatically Determined"
+    """
+
+    @property
+    def top_depth(self):
+        """float: The top depth of the Polar & Rose box in current
+        depth reference units.
+        """
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of the Polar & Rose box in current
+        depth reference units.
+        """
+        return self._dispatch.BottomDepth
+
+    @property
+    def text(self):
+        """str: The text for a Polar & Rose Log box.
+
+        The text is not displayed in the plot and is only visible in
+        the tabular editor or when exporting the data.
+        """
+        return self._dispatch.Text
+
+    @text.setter
+    def text(self, value):
+        self._dispatch.Text = value
+
+
```

### Comparing `pywellcad-0.2.0/wellcad/com/_stacking_pattern_item.py` & `pywellcad-0.2.1/wellcad/com/_stacking_pattern_item.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class StackingPatternItem(DispatchWrapper):
-    """Stores a stacking pattern over an interval.
-
-    StackingPattern items are part of a StackingPattern Log and stores the top and bottom widths
-    over a depth interval.
-    Width values are between 0.0 and 1.0 and depth intervals can not overlap.
-
-    Example
-    -------
-    >>> stack_log = borehole.log("Test")
-    >>> stack_box = stack_box.insert_new_stack_item(10.5, 12.5, 0.5, 0.8)
-    >>> stack_box.top_depth
-    10.5
-    >>> stack_box.top_depth
-    12.5
-    """
-
-    @property
-    def top_depth(self):
-        """float: The top depth of the item in current depth
-        units."""
-        return self._dispatch.TopDepth
-
-    @property
-    def bottom_depth(self):
-        """float: The bottom depth of the item in current depth
-        units."""
-        return self._dispatch.BottomDepth
-
-    @property
-    def top_width(self):
-        """float: The top width of the item.
-        
-        This should be a value between 0.0 and 1.0. Setting it out of these
-        bounds will clamp the value.
-        """
-        return self._dispatch.TopWidth
-
-    @top_width.setter
-    def top_width(self, value):
-        self._dispatch.TopWidth = value
-
-    @property
-    def bottom_width(self):
-        """float: The bottom width of the item.
-        
-        This should be a value between 0.0 and 1.0. Setting it out of these
-        bounds will clamp the value.
-        """
-        return self._dispatch.BottomWidth
-
-    @bottom_width.setter
-    def bottom_width(self, value):
-        self._dispatch.BottomWidth = value
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class StackingPatternItem(DispatchWrapper):
+    """Stores a stacking pattern over an interval.
+
+    StackingPattern items are part of a StackingPattern Log and stores the top and bottom widths
+    over a depth interval.
+    Width values are between 0.0 and 1.0 and depth intervals can not overlap.
+
+    Example
+    -------
+    >>> stack_log = borehole.log("Test")
+    >>> stack_box = stack_box.insert_new_stack_item(10.5, 12.5, 0.5, 0.8)
+    >>> stack_box.top_depth
+    10.5
+    >>> stack_box.top_depth
+    12.5
+    """
+
+    @property
+    def top_depth(self):
+        """float: The top depth of the item in current depth
+        units."""
+        return self._dispatch.TopDepth
+
+    @property
+    def bottom_depth(self):
+        """float: The bottom depth of the item in current depth
+        units."""
+        return self._dispatch.BottomDepth
+
+    @property
+    def top_width(self):
+        """float: The top width of the item.
+        
+        This should be a value between 0.0 and 1.0. Setting it out of these
+        bounds will clamp the value.
+        """
+        return self._dispatch.TopWidth
+
+    @top_width.setter
+    def top_width(self, value):
+        self._dispatch.TopWidth = value
+
+    @property
+    def bottom_width(self):
+        """float: The bottom width of the item.
+        
+        This should be a value between 0.0 and 1.0. Setting it out of these
+        bounds will clamp the value.
+        """
+        return self._dispatch.BottomWidth
+
+    @bottom_width.setter
+    def bottom_width(self, value):
+        self._dispatch.BottomWidth = value
```

### Comparing `pywellcad-0.2.0/wellcad/com/_title.py` & `pywellcad-0.2.1/wellcad/com/_title.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,435 +1,435 @@
-from ._dispatch_wrapper import DispatchWrapper
-from ._font import Font
-
-
-class Title(DispatchWrapper):
-    """Represents the title of a log.
-
-    A title object is represented by a box at the top of a log. Inside the title box are three sections: the title, the comments and the properties.
-    For each of these sections, you can specify properties such as text, font, color, alignment etc. The title box frame and background can also be customized.
-
-    ::
-
-        |-------------------|-----------------------------|-------------------|
-        |                   |                             |                   |
-        |     Title         |           Title             |                   |
-        |                   |                             |                   |
-        |                   |          comment            |      Title        |
-        |                   |                             |                   |
-        |    properties     |         properties          |                   |
-        |-------------------|-----------------------------|-------------------|
-        |                   |                             |                   |
-        |                   |                             |                   |
-        |    log data       |         log data            |     log data      |
-        |                   |                             |                   |
-
-    Example
-    -------
-    >>> borehole = app.get_active_borehole()
-    >>> title = borehole.title("GR")
-    >>> title.left_position
-    0.2
-    >>> title.box_height = 200
-    """
-
-    @property
-    def left_position(self):
-        """float: The position of the left side of a title for a log or group,
-        as a fraction of the document width.
-
-        If set for a group title, the logs that are a part of the group will
-        be moved/scaled accordingly. In the case that this is set to be a value
-        higher than ``right_position``, the two attributes will swap. Values
-        will be clamped in the range [0.0, 1.0].
-        """
-        return self._dispatch.LeftPosition
-
-    @left_position.setter
-    def left_position(self, value):
-        self._dispatch.LeftPosition = value
-
-    @property
-    def right_position(self):
-        """float: The position of the right side of a title for a log or group,
-        as a fraction of the document width.
-
-        If set for a group title, the logs that are a part of the group will
-        be moved/scaled accordingly. In the case that this is set to be a value
-        lower than ``left_position``, the two attributes will swap. Values
-        will be clamped in the range [0.0, 1.0].
-        """
-        return self._dispatch.RightPosition
-
-    @right_position.setter
-    def right_position(self, value):
-        self._dispatch.RightPosition = value
-
-    @property
-    def box_height(self):
-        """float: The title box height in mm."""
-        return self._dispatch.BoxHeight
-
-    @box_height.setter
-    def box_height(self, value):
-        self._dispatch.BoxHeight = value
-
-    @property
-    def display_frame(self):
-        """bool: Whether the title box frame is displayed."""
-        return self._dispatch.DisplayFrame
-
-    @display_frame.setter
-    def display_frame(self, flag):
-        """Set to True to display the title box frame."""
-        self._dispatch.DisplayFrame = flag
-
-    @property
-    def frame_color(self):
-        """int: The color of the frame.
-
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
-        """
-        return self._dispatch.FrameColor
-
-    @frame_color.setter
-    def frame_color(self, value):
-        self._dispatch.FrameColor = value
-
-    @property
-    def frame_style(self):
-        """int: The frame's display style.
-
-        Available styles are:
-
-        * 0 = solid
-        * 1 = dashed
-        * 2 = dotted
-        * 3 = dash-dot
-        * 4 =  dash-dot-dot
-        """
-        return self._dispatch.FrameStyle
-
-    @frame_style.setter
-    def frame_style(self, style):
-        self._dispatch.FrameStyle = style
-
-    @property
-    def frame_width(self):
-        """int: The line width of the frame in 1/10 mm."""
-        return self._dispatch.FrameWidth
-
-    @frame_width.setter
-    def frame_width(self, value):
-        self._dispatch.FrameWidth = value
-
-    @property
-    def background_color(self):
-        """int: The background color of a group or log title.
-
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
-        """
-        return self._dispatch.BackgroundColor
-
-    @background_color.setter
-    def background_color(self, value):
-        self._dispatch.BackgroundColor = value
-
-    @property
-    def use_colored_background(self):
-        """bool: Whether the colored background is used."""
-        return self._dispatch.UseColoredBackground
-
-    @use_colored_background.setter
-    def use_colored_background(self, flag):
-        self._dispatch.UseColoredBackground = flag
-
-    @property
-    def display_title(self):
-        """bool: Whether the title partition is displayed."""
-        return self._dispatch.DisplayTitle
-
-    @display_title.setter
-    def display_title(self, flag):
-        self._dispatch.DisplayTitle = flag
-
-    @property
-    def display_comment(self):
-        """bool: Whether the comment partition is displayed."""
-        return self._dispatch.DisplayComment
-
-    @display_comment.setter
-    def display_comment(self, flag):
-        self._dispatch.DisplayComment = flag
-
-    @property
-    def display_properties(self):
-        """bool: Whether the property partition is displayed."""
-        return self._dispatch.DisplayProperties
-
-    @display_properties.setter
-    def display_properties(self, flag):
-        self._dispatch.DisplayProperties = flag
-
-    @property
-    def title_text(self):
-        """str: The text for the title partition."""
-        return self._dispatch.TitleText
-
-    @title_text.setter
-    def title_text(self, text):
-        self._dispatch.TitleText = text
-
-    @property
-    def comment_text(self):
-        """str: The text for the comment partition."""
-        return self._dispatch.CommentText
-
-    @comment_text.setter
-    def comment_text(self, text):
-        self._dispatch.CommentText = text
-
-    @property
-    def title_top(self):
-        """float: The top of the title partition of a group or log
-        title box as a fraction of the box height (value between 0 and 1)."""
-        return self._dispatch.TitleTop
-
-    @title_top.setter
-    def title_top(self, value):
-        self._dispatch.TitleTop = value
-
-    @property
-    def title_bottom(self):
-        """float: The bottom of the title partition of a group or log
-        title box as a fraction of the box height (value between 0 and 1)."""
-        return self._dispatch.TitleBottom
-
-    @title_bottom.setter
-    def title_bottom(self, value):
-        self._dispatch.TitleBottom = value
-
-    @property
-    def title_color(self):
-        """int: The font color of the title part of a group or log
-        title.
-
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
-        """
-        return self._dispatch.TitleColor
-
-    @title_color.setter
-    def title_color(self, value):
-        self._dispatch.TitleColor = value
-
-    @property
-    def comment_top(self):
-        """float: The top of the comment partition of a group or log
-        title box as a fraction of the box height (value between 0
-        and 1)."""
-        return self._dispatch.CommentTop
-
-    @comment_top.setter
-    def comment_top(self, value):
-        self._dispatch.CommentTop = value
-
-    @property
-    def comment_bottom(self):
-        """float: The bottom of the comment partition of a group or
-        log title box as a fraction of the box height (value between 0
-        and 1)."""
-        return self._dispatch.CommentBottom
-
-    @comment_bottom.setter
-    def comment_bottom(self, value):
-        self._dispatch.CommentBottom = value
-
-    @property
-    def comment_color(self):
-        """int: The coment color of the title part of a group or log
-        title.
-
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
-        """
-        return self._dispatch.CommentColor
-
-    @comment_color.setter
-    def comment_color(self, value):
-        self._dispatch.CommentColor = value
-
-    @property
-    def properties_top(self):
-        """float: The top of the properties partition of a log title
-        box as a fraction of the box height (value between 0 and 1).
-        """
-        return self._dispatch.PropertiesTop
-
-    @properties_top.setter
-    def properties_top(self, value):
-        self._dispatch.PropertiesTop = value
-
-    @property
-    def properties_bottom(self):
-        """float: The bottom of the properties partition of a log title
-        box as a fraction of the box height (value between 0 and 1).
-        """
-        return self._dispatch.PropertiesBottom
-
-    @properties_bottom.setter
-    def properties_bottom(self, value):
-        self._dispatch.PropertiesBottom = value
-
-    @property
-    def properties_color(self):
-        """int: The font color of the property part of a group or log
-        title.
-
-        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
-        Each of the blue (B), green (G) and red (R) components are 8 bit
-        values.
-        """
-        return self._dispatch.PropertiesColor
-
-    @properties_color.setter
-    def properties_color(self, value):
-        self._dispatch.PropertiesColor = value
-
-    @property
-    def title_horizontal_position(self):
-        """int: Index specifying the horizontal alignment of the title.
-
-        Available options are:
-
-        * 0 = left
-        * 1 = center
-        * 2 = right
-        """
-        return self._dispatch.TitleHorizontalPosition
-
-    @title_horizontal_position.setter
-    def title_horizontal_position(self, index):
-        self._dispatch.TitleHorizontalPosition = index
-
-    @property
-    def title_vertical_position(self):
-        """int: Index specifying the vertical alignment of the title.
-
-        Available options are:
-
-        * 0 = left
-        * 1 = center
-        * 2 = right
-        """
-        return self._dispatch.TitleVerticalPosition
-
-    @title_vertical_position.setter
-    def title_vertical_position(self, index):
-        self._dispatch.TitleVerticalPosition = index
-
-    @property
-    def title_orientation(self):
-        """int: Index specifying the title orientation.
-
-        Available options are:
-
-        * 0 = horizontal
-        * 1 = rotated left
-        * 2 = reversed
-        * 3 = rotated right
-        """
-        return self._dispatch.TitleOrientation
-
-    @title_orientation.setter
-    def title_orientation(self, index):
-        self._dispatch.TitleOrientation = index
-
-    @property
-    def comment_horizontal_position(self):
-        """int: Index specifying the horizontal alignment of the comment.
-
-        Available options are:
-
-        * 0 = left
-        * 1 = center
-        * 2 = right
-        """
-        return self._dispatch.CommentHorizontalPosition
-
-    @comment_horizontal_position.setter
-    def comment_horizontal_position(self, index):
-        self._dispatch.CommentHorizontalPosition = index
-
-    @property
-    def comment_vertical_position(self):
-        """int: Index specifying the vertical alignment of the comment.
-
-        Available options are:
-
-        * 0 = left
-        * 1 = center
-        * 2 = right
-        """
-        return self._dispatch.CommentVerticalPosition
-
-    @comment_vertical_position.setter
-    def comment_vertical_position(self, index):
-        self._dispatch.CommentVerticalPosition = index
-
-    @property
-    def comment_alignment(self):
-        """int: Index specifying the comment alignment within the
-        partition.
-
-        Available options are:
-
-        * 0 = left
-        * 1 = center
-        * 2 = right
-        """
-        return self._dispatch.CommentAlignment
-
-    @comment_alignment.setter
-    def comment_alignment(self, index):
-        self._dispatch.CommentAlignment = index
-
-    @property
-    def comment_orientation(self):
-        """int: Index specifying the comment orientation.
-
-        Available options are:
-
-        * 0 = horizontal
-        * 1 = rotated left
-        * 2 = reversed
-        * 3 = rotated right
-        """
-        return self._dispatch.CommentOrientation
-
-    @comment_orientation.setter
-    def comment_orientation(self, index):
-        self._dispatch.CommentOrientation = index
-
-    @property
-    def title_font(self):
-        """Font: The font of the title partition of a group or log
-        title."""
-        return Font(self._dispatch.TitleFont)
-
-    @property
-    def comment_font(self):
-        """Font: The font of the comment partition of a group or log
-        title."""
-        return Font(self._dispatch.CommentFont)
-
-    @property
-    def properties_font(self):
-        """Font: The font of the properties  partition of a group or log
-        title."""
-        return Font(self._dispatch.PropertiesFont)
+from ._dispatch_wrapper import DispatchWrapper
+from ._font import Font
+
+
+class Title(DispatchWrapper):
+    """Represents the title of a log.
+
+    A title object is represented by a box at the top of a log. Inside the title box are three sections: the title, the comments and the properties.
+    For each of these sections, you can specify properties such as text, font, color, alignment etc. The title box frame and background can also be customized.
+
+    ::
+
+        |-------------------|-----------------------------|-------------------|
+        |                   |                             |                   |
+        |     Title         |           Title             |                   |
+        |                   |                             |                   |
+        |                   |          comment            |      Title        |
+        |                   |                             |                   |
+        |    properties     |         properties          |                   |
+        |-------------------|-----------------------------|-------------------|
+        |                   |                             |                   |
+        |                   |                             |                   |
+        |    log data       |         log data            |     log data      |
+        |                   |                             |                   |
+
+    Example
+    -------
+    >>> borehole = app.get_active_borehole()
+    >>> title = borehole.title("GR")
+    >>> title.left_position
+    0.2
+    >>> title.box_height = 200
+    """
+
+    @property
+    def left_position(self):
+        """float: The position of the left side of a title for a log or group,
+        as a fraction of the document width.
+
+        If set for a group title, the logs that are a part of the group will
+        be moved/scaled accordingly. In the case that this is set to be a value
+        higher than ``right_position``, the two attributes will swap. Values
+        will be clamped in the range [0.0, 1.0].
+        """
+        return self._dispatch.LeftPosition
+
+    @left_position.setter
+    def left_position(self, value):
+        self._dispatch.LeftPosition = value
+
+    @property
+    def right_position(self):
+        """float: The position of the right side of a title for a log or group,
+        as a fraction of the document width.
+
+        If set for a group title, the logs that are a part of the group will
+        be moved/scaled accordingly. In the case that this is set to be a value
+        lower than ``left_position``, the two attributes will swap. Values
+        will be clamped in the range [0.0, 1.0].
+        """
+        return self._dispatch.RightPosition
+
+    @right_position.setter
+    def right_position(self, value):
+        self._dispatch.RightPosition = value
+
+    @property
+    def box_height(self):
+        """float: The title box height in mm."""
+        return self._dispatch.BoxHeight
+
+    @box_height.setter
+    def box_height(self, value):
+        self._dispatch.BoxHeight = value
+
+    @property
+    def display_frame(self):
+        """bool: Whether the title box frame is displayed."""
+        return self._dispatch.DisplayFrame
+
+    @display_frame.setter
+    def display_frame(self, flag):
+        """Set to True to display the title box frame."""
+        self._dispatch.DisplayFrame = flag
+
+    @property
+    def frame_color(self):
+        """int: The color of the frame.
+
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values.
+        """
+        return self._dispatch.FrameColor
+
+    @frame_color.setter
+    def frame_color(self, value):
+        self._dispatch.FrameColor = value
+
+    @property
+    def frame_style(self):
+        """int: The frame's display style.
+
+        Available styles are:
+
+        * 0 = solid
+        * 1 = dashed
+        * 2 = dotted
+        * 3 = dash-dot
+        * 4 =  dash-dot-dot
+        """
+        return self._dispatch.FrameStyle
+
+    @frame_style.setter
+    def frame_style(self, style):
+        self._dispatch.FrameStyle = style
+
+    @property
+    def frame_width(self):
+        """int: The line width of the frame in 1/10 mm."""
+        return self._dispatch.FrameWidth
+
+    @frame_width.setter
+    def frame_width(self, value):
+        self._dispatch.FrameWidth = value
+
+    @property
+    def background_color(self):
+        """int: The background color of a group or log title.
+
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values.
+        """
+        return self._dispatch.BackgroundColor
+
+    @background_color.setter
+    def background_color(self, value):
+        self._dispatch.BackgroundColor = value
+
+    @property
+    def use_colored_background(self):
+        """bool: Whether the colored background is used."""
+        return self._dispatch.UseColoredBackground
+
+    @use_colored_background.setter
+    def use_colored_background(self, flag):
+        self._dispatch.UseColoredBackground = flag
+
+    @property
+    def display_title(self):
+        """bool: Whether the title partition is displayed."""
+        return self._dispatch.DisplayTitle
+
+    @display_title.setter
+    def display_title(self, flag):
+        self._dispatch.DisplayTitle = flag
+
+    @property
+    def display_comment(self):
+        """bool: Whether the comment partition is displayed."""
+        return self._dispatch.DisplayComment
+
+    @display_comment.setter
+    def display_comment(self, flag):
+        self._dispatch.DisplayComment = flag
+
+    @property
+    def display_properties(self):
+        """bool: Whether the property partition is displayed."""
+        return self._dispatch.DisplayProperties
+
+    @display_properties.setter
+    def display_properties(self, flag):
+        self._dispatch.DisplayProperties = flag
+
+    @property
+    def title_text(self):
+        """str: The text for the title partition."""
+        return self._dispatch.TitleText
+
+    @title_text.setter
+    def title_text(self, text):
+        self._dispatch.TitleText = text
+
+    @property
+    def comment_text(self):
+        """str: The text for the comment partition."""
+        return self._dispatch.CommentText
+
+    @comment_text.setter
+    def comment_text(self, text):
+        self._dispatch.CommentText = text
+
+    @property
+    def title_top(self):
+        """float: The top of the title partition of a group or log
+        title box as a fraction of the box height (value between 0 and 1)."""
+        return self._dispatch.TitleTop
+
+    @title_top.setter
+    def title_top(self, value):
+        self._dispatch.TitleTop = value
+
+    @property
+    def title_bottom(self):
+        """float: The bottom of the title partition of a group or log
+        title box as a fraction of the box height (value between 0 and 1)."""
+        return self._dispatch.TitleBottom
+
+    @title_bottom.setter
+    def title_bottom(self, value):
+        self._dispatch.TitleBottom = value
+
+    @property
+    def title_color(self):
+        """int: The font color of the title part of a group or log
+        title.
+
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values.
+        """
+        return self._dispatch.TitleColor
+
+    @title_color.setter
+    def title_color(self, value):
+        self._dispatch.TitleColor = value
+
+    @property
+    def comment_top(self):
+        """float: The top of the comment partition of a group or log
+        title box as a fraction of the box height (value between 0
+        and 1)."""
+        return self._dispatch.CommentTop
+
+    @comment_top.setter
+    def comment_top(self, value):
+        self._dispatch.CommentTop = value
+
+    @property
+    def comment_bottom(self):
+        """float: The bottom of the comment partition of a group or
+        log title box as a fraction of the box height (value between 0
+        and 1)."""
+        return self._dispatch.CommentBottom
+
+    @comment_bottom.setter
+    def comment_bottom(self, value):
+        self._dispatch.CommentBottom = value
+
+    @property
+    def comment_color(self):
+        """int: The coment color of the title part of a group or log
+        title.
+
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values.
+        """
+        return self._dispatch.CommentColor
+
+    @comment_color.setter
+    def comment_color(self, value):
+        self._dispatch.CommentColor = value
+
+    @property
+    def properties_top(self):
+        """float: The top of the properties partition of a log title
+        box as a fraction of the box height (value between 0 and 1).
+        """
+        return self._dispatch.PropertiesTop
+
+    @properties_top.setter
+    def properties_top(self, value):
+        self._dispatch.PropertiesTop = value
+
+    @property
+    def properties_bottom(self):
+        """float: The bottom of the properties partition of a log title
+        box as a fraction of the box height (value between 0 and 1).
+        """
+        return self._dispatch.PropertiesBottom
+
+    @properties_bottom.setter
+    def properties_bottom(self, value):
+        self._dispatch.PropertiesBottom = value
+
+    @property
+    def properties_color(self):
+        """int: The font color of the property part of a group or log
+        title.
+
+        Colours are specified as a 32 bit integer with an ``xBGR`` structure.
+        Each of the blue (B), green (G) and red (R) components are 8 bit
+        values.
+        """
+        return self._dispatch.PropertiesColor
+
+    @properties_color.setter
+    def properties_color(self, value):
+        self._dispatch.PropertiesColor = value
+
+    @property
+    def title_horizontal_position(self):
+        """int: Index specifying the horizontal alignment of the title.
+
+        Available options are:
+
+        * 0 = left
+        * 1 = center
+        * 2 = right
+        """
+        return self._dispatch.TitleHorizontalPosition
+
+    @title_horizontal_position.setter
+    def title_horizontal_position(self, index):
+        self._dispatch.TitleHorizontalPosition = index
+
+    @property
+    def title_vertical_position(self):
+        """int: Index specifying the vertical alignment of the title.
+
+        Available options are:
+
+        * 0 = left
+        * 1 = center
+        * 2 = right
+        """
+        return self._dispatch.TitleVerticalPosition
+
+    @title_vertical_position.setter
+    def title_vertical_position(self, index):
+        self._dispatch.TitleVerticalPosition = index
+
+    @property
+    def title_orientation(self):
+        """int: Index specifying the title orientation.
+
+        Available options are:
+
+        * 0 = horizontal
+        * 1 = rotated left
+        * 2 = reversed
+        * 3 = rotated right
+        """
+        return self._dispatch.TitleOrientation
+
+    @title_orientation.setter
+    def title_orientation(self, index):
+        self._dispatch.TitleOrientation = index
+
+    @property
+    def comment_horizontal_position(self):
+        """int: Index specifying the horizontal alignment of the comment.
+
+        Available options are:
+
+        * 0 = left
+        * 1 = center
+        * 2 = right
+        """
+        return self._dispatch.CommentHorizontalPosition
+
+    @comment_horizontal_position.setter
+    def comment_horizontal_position(self, index):
+        self._dispatch.CommentHorizontalPosition = index
+
+    @property
+    def comment_vertical_position(self):
+        """int: Index specifying the vertical alignment of the comment.
+
+        Available options are:
+
+        * 0 = left
+        * 1 = center
+        * 2 = right
+        """
+        return self._dispatch.CommentVerticalPosition
+
+    @comment_vertical_position.setter
+    def comment_vertical_position(self, index):
+        self._dispatch.CommentVerticalPosition = index
+
+    @property
+    def comment_alignment(self):
+        """int: Index specifying the comment alignment within the
+        partition.
+
+        Available options are:
+
+        * 0 = left
+        * 1 = center
+        * 2 = right
+        """
+        return self._dispatch.CommentAlignment
+
+    @comment_alignment.setter
+    def comment_alignment(self, index):
+        self._dispatch.CommentAlignment = index
+
+    @property
+    def comment_orientation(self):
+        """int: Index specifying the comment orientation.
+
+        Available options are:
+
+        * 0 = horizontal
+        * 1 = rotated left
+        * 2 = reversed
+        * 3 = rotated right
+        """
+        return self._dispatch.CommentOrientation
+
+    @comment_orientation.setter
+    def comment_orientation(self, index):
+        self._dispatch.CommentOrientation = index
+
+    @property
+    def title_font(self):
+        """Font: The font of the title partition of a group or log
+        title."""
+        return Font(self._dispatch.TitleFont)
+
+    @property
+    def comment_font(self):
+        """Font: The font of the comment partition of a group or log
+        title."""
+        return Font(self._dispatch.CommentFont)
+
+    @property
+    def properties_font(self):
+        """Font: The font of the properties  partition of a group or log
+        title."""
+        return Font(self._dispatch.PropertiesFont)
```

### Comparing `pywellcad-0.2.0/wellcad/com/_workspace.py` & `pywellcad-0.2.1/wellcad/com/_workspace.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,306 +1,306 @@
-from ._dispatch_wrapper import DispatchWrapper
-
-
-class Workspace(DispatchWrapper):
-    """Use functionalities from the Image & Structure Interpretation Workspace (ISI Workspace)
-    and the Casing Integrity Workspace.
-
-    Example
-    -------
-    >>> borehole = app.get_active_borehole()
-    >>> workspace = borehole.workspace("ISI workspace")
-    >>> workspace.representative_picks(config_file_name=config_file)
-    """
-    _DISPATCH_METHODS = ("PickSimilarFeatures", "RepresentativePicks", )
-
-    def auto_detect_zones(self):
-        """Automaticaly detects zones in the image log of a workspace."""
-        self._dispatch.AutoDetectZones()
-
-    def pick_similar_features(self, config_file_name):
-        """Runs an automated similar structure picking in ISI workspace.
-
-        The Pick Similar Features process takes one or more manual
-        picks as input, runs the automated picking and keeps only
-        picks which do not deviate from the reference(s) by a defined
-        tolerance value in Dip Azimuth and Dip angle. Picks detected
-        as similar are then added to the pick repository.
-        You need to have **manually** selected the input picks first
-        in the WellCAD window.
-
-        Parameters
-        ----------
-        config_file_name : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [PickSimilarFeatures]
-                InputLog = (title of the log to process)
-                TopDepth = 0 '(top of the interval to process)
-                BottomDepth = 10 '(top of the interval to process)
-                ImageType = 3 '(0 = RGB OTV, 1 = Greyscale OTV, 2 = Diamond Drilled ATV, 3 = RC Drilled ATV, 4 = FMI)
-                DarkFeatures = yes /no
-                BrightFeatures = yes / no
-                Aperture = yes / no
-                PartialPicks = yes / no
-                AzimuthTolerance = 5.0
-                TiltTolerance = 5.0 '(i.e. dip angle tolerance)
-                UseDefaultSettings = yes / no
-
-                ' Processing Paraemters
-                ImageWidth = 144
-                ImageSmoothingIterations = 2
-                MinimumFeatureSize = 5
-                DesiredFeatureStrength = 0.5
-                MinimumFeatureStrength = 0.2
-                MinimumStructureAperture = 0.008
-                MaximumStructureAperture = 0.032
-                SinusoidalDeviationTolerance = 30
-                MaximumSinusoidAmplitude = 0.6
-                MinimumSinusoidAmplitude = 0
-
-                ' Advanced Processing Parameters
-                FeatureDistanceDeviation = 2
-                FeatureOrientationDeviation = 20
-                HandleOverlappingSinusoids = 1 '(1 = yes, 0 = no)
-                FeatureMergingConstraint = 0.6
-                SinusoidCompleteness = 1 '(1 = yes, 0 = no)
-                ClusterDipTolerance = 15
-                ClusterAzimuthTolerance = 15
-                DepthOffsetTolerance = 30
-                PixelBrightnessTolerance = 1
-                ImageSmoothingStrength = 20
-                ImageSmoothingSpeed = 0.25
-                ImageContrastSensitivity = 0.05
-
-        """
-        self._dispatch.PickSimilarFeatures(config_file_name)
-
-    def representative_picks(self, config_file_name):
-        """Runs the representative picks process in ISI
-
-        The representative Picks process uses an adapted Ward
-        algorithm to cluster picks which have the least dissimilarity
-        in azimuth, dip, depth distance from each other and pick type
-        (i.e. classification). As a result it determines the most
-        representative pick of each cluster - i.e. the (real) pick
-        with the highest confidence and closest to the center of each
-        cluster.
-
-        Parameters
-        ----------
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [RepresentativePicks]
-                InputLog = '(title of the log to process)
-                TopDepth = 0 '(top of the interval to process)
-                BottomDepth = 10 '(top of the interval to process)
-                AzimuthWindow = 5.0
-                TiltWindow = 5.0'(i.e. dip angle window)
-                DepthWindow = 0.5
-                KeepFeaturesUngrouped = yes / no
-        """
-        self._dispatch.RepresentativePicks(config_file_name)
-
-    def automatic_picking(self, config_file_name):
-        """Runs an automated structure picking in the ISI workspace
-
-        The Auto Picker allows the detection of planar structures in
-        televiewer (ATV, OTV) and electrical imager (e.g. FMI) images.
-        3D core scans are similar to OTV images and can be processed
-        as well.
-
-        Parameters
-        ----------
-        config : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [AutomaticPicking]
-                InputLog = Amplitude '(title of the log to process)
-                TopDepth = 0 '(top of the interval to process)
-                BottomDepth = 10 '(top of the interval to process)
-                ImageType = 3 '(0 = RGB OTV, 1 = Greyscale OTV, 2 = Diamond Drilled ATV, 3 = RC Drilled ATV, 4 = FMI)
-                DarkFeatures = yes /no
-                BrightFeatures = yes / no
-                Aperture = yes / no
-                PartialPicks = yes / no
-                UseDefaultSettings = yes / no
-
-                ' Processing Parameters
-                ImageWidth = 144
-                ImageSmoothingIterations = 2
-                MinimumFeatureSize = 5
-                DesiredFeatureStrength = 0.5
-                MinimumFeatureStrength = 0.2
-                MinimumStructureAperture = 0.008
-                MaximumStructureAperture = 0.032
-                SinusoidalDeviationTolerance = 30
-                MaximumSinusoidAmplitude = 0.6
-                MinimumSinusoidAmplitude = 0
-
-                ' Advanced Processing Parameters
-                FeatureDistanceDeviation = 2
-                FeatureOrientationDeviation = 20
-                HandleOverlappingSinusoids = 1 '(1 = yes, 0 = no)
-                FeatureMergingConstraint = 0.6
-                SinusoidCompleteness = 1 '(1 = yes, 0 = no)
-                ClusterDipTolerance = 15
-                ClusterAzimuthTolerance = 15
-                DepthOffsetTolerance = 30
-                PixelBrightnessTolerance = 1
-                ImageSmoothingStrength = 20
-                ImageSmoothingSpeed = 0.25
-                ImageContrastSensitivity = 0.05
-        """
-        self._dispatch.AutomaticPicking(config_file_name)
-
-    def quick_pick(self, config_file_name):
-        """Runs a quick pick in ISI
-
-        The Quick Pick Process analyzes the image for features with
-        the highest confidence within given Azimuth, Dip and Depth
-        tolerances. E.g. if you would like to pick just the main event
-        every 1m interval and leave all other features unaccounted you
-        can use this process.
-
-        Parameters
-        ----------
-        config_file_name : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            .. code-block:: ini
-
-                [QuickPick]
-                InputLog = Amplitude '(title of the log to process)
-                TopDepth = 0 '(top of the interval to process)
-                BottomDepth = 10 '(top of the interval to process)
-                ImageType = 3 '(0 = RGB OTV, 1 = Greyscale OTV, 2 = Diamond Drilled ATV, 3 = RC Drilled ATV, 4 = FMI)
-                DarkFeatures = yes /no
-                BrightFeatures = yes / no
-                Aperture = yes / no
-                PartialPicks = yes / no
-                AzimuthWindow = 5.0
-                TiltWindow = 5.0'(i.e. dip angle window)
-                DepthWindow = 0.5
-                UseDefaultSettings = yes / no
-
-                ' Processing Parameters
-                ImageWidth = 144
-                ImageSmoothingIterations = 2
-                MinimumFeatureSize = 5
-                DesiredFeatureStrength = 0.5
-                MinimumFeatureStrength = 0.2
-                MinimumStructureAperture = 0.008
-                MaximumStructureAperture = 0.032
-                SinusoidalDeviationTolerance = 30
-                MaximumSinusoidAmplitude = 0.6
-                MinimumSinusoidAmplitude = 0
-
-                ' Advanced Processing Parameters
-                FeatureDistanceDeviation = 2
-                FeatureOrientationDeviation = 20
-                HandleOverlappingSinusoids = 1 '(1 = yes, 0 = no)
-                FeatureMergingConstraint = 0.6
-                SinusoidCompleteness = 1 '(1 = yes, 0 = no)
-                ClusterDipTolerance = 15
-                ClusterAzimuthTolerance = 15
-                DepthOffsetTolerance = 30
-                PixelBrightnessTolerance = 1
-                ImageSmoothingStrength = 20
-                ImageSmoothingSpeed = 0.25
-                ImageContrastSensitivity = 0.05
-        """
-
-        self._dispatch.QuickPick(config_file_name)
-
-    def apply_template(self, path, prompt_if_not_found=None, config_file_name=None):
-        """Applies a workspace template
-        
-        Allows the application of an ISI Workspace,
-        Casing Integrity Workspace or NMR Workspace template.
-
-        Parameters
-        ----------
-        path: str
-            String specifying the name and path of the
-            workspace template to be applied (\*.ist). Please note
-            that the file extension is different for the
-            ISI, Casing Integrity and NMR Workspaces.
-        prompt_if_not_found: bool, optional
-            Boolean indicating whether the dialog box to
-            prompt the user for logs not found in the
-            template is displayed or not. The default is
-            set to True.
-        config_file_name : str, optional
-            The configuration file. Read the WellCAD Help for
-            information on the syntax of the file.
-
-        Returns
-        -------
-        bool
-            Always returns True except for the WellCAD Reader and
-            Demo version for which the function returns False.
-        """
-        return self._dispatch.ApplyTemplate(path, prompt_if_not_found, config_file_name)
-
-    def auto_joint_detection(self, config_file_name):
-        """Detects the joints from the main log (data source) used
-        in the workspace.
-
-        Parameters
-        ----------
-        config_file_name : str, optional
-            Path to a configuration file or a parameter string. The
-            configuration file can contain the following options:
-
-            Note: This configuration is for WellCAD version 5.7 and onwards. For prior version, see the next section.
-
-            .. code-block:: ini
-
-                [AutoJointDetection]
-                Sensitivity = 5
-                TopAndBottom = yes
-
-            For WellCAD version 5.5 and 5.6, use this configuration instead:
-
-            .. code-block:: ini
-
-                [AutoJointDetection]
-                JointHeight=0.5
-                Sensitivity=100
-        """
-        self._dispatch.AutoJointDetection(config_file_name)
-
-    def add_joint_log_to_b_hole(self):
-        """Adds the Marker Log from the Casing Integrity
-        Workspace displaying the casing joints back to the
-        borehole document.
-        """
-        self._dispatch.AddJointLogToBHole()
-
-    def add_engin_log_from_driller_casing_table_to_b_hole(self):
-        """Adds the Engineering Log from the Navigation Bar
-        of the Casing Integrity Workspace displaying the
-        drillers casing info back to the borehole document.
-
-        Note: this function is deprecated in WellCAD 5.7 and onwards
-        """
-        self._dispatch.AddEnginLogFromDrillerCasingTableToBHole()
-
-    def add_engin_log_from_logger_casing_table_to_b_hole(self):
-        """Adds the Engineering Log from the Navigation Bar
-        of the Casing Integrity Workspace displaying the
-        casing info derived from the logged data back to the
-        borehole document.
-        """
-        self._dispatch.AddEnginLogFromLoggerCasingTableToBHole()
+from ._dispatch_wrapper import DispatchWrapper
+
+
+class Workspace(DispatchWrapper):
+    """Use functionalities from the Image & Structure Interpretation Workspace (ISI Workspace)
+    and the Casing Integrity Workspace.
+
+    Example
+    -------
+    >>> borehole = app.get_active_borehole()
+    >>> workspace = borehole.workspace("ISI workspace")
+    >>> workspace.representative_picks(config_file_name=config_file)
+    """
+    _DISPATCH_METHODS = ("PickSimilarFeatures", "RepresentativePicks", )
+
+    def auto_detect_zones(self):
+        """Automaticaly detects zones in the image log of a workspace."""
+        self._dispatch.AutoDetectZones()
+
+    def pick_similar_features(self, config_file_name):
+        """Runs an automated similar structure picking in ISI workspace.
+
+        The Pick Similar Features process takes one or more manual
+        picks as input, runs the automated picking and keeps only
+        picks which do not deviate from the reference(s) by a defined
+        tolerance value in Dip Azimuth and Dip angle. Picks detected
+        as similar are then added to the pick repository.
+        You need to have **manually** selected the input picks first
+        in the WellCAD window.
+
+        Parameters
+        ----------
+        config_file_name : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [PickSimilarFeatures]
+                InputLog = (title of the log to process)
+                TopDepth = 0 '(top of the interval to process)
+                BottomDepth = 10 '(top of the interval to process)
+                ImageType = 3 '(0 = RGB OTV, 1 = Greyscale OTV, 2 = Diamond Drilled ATV, 3 = RC Drilled ATV, 4 = FMI)
+                DarkFeatures = yes /no
+                BrightFeatures = yes / no
+                Aperture = yes / no
+                PartialPicks = yes / no
+                AzimuthTolerance = 5.0
+                TiltTolerance = 5.0 '(i.e. dip angle tolerance)
+                UseDefaultSettings = yes / no
+
+                ' Processing Paraemters
+                ImageWidth = 144
+                ImageSmoothingIterations = 2
+                MinimumFeatureSize = 5
+                DesiredFeatureStrength = 0.5
+                MinimumFeatureStrength = 0.2
+                MinimumStructureAperture = 0.008
+                MaximumStructureAperture = 0.032
+                SinusoidalDeviationTolerance = 30
+                MaximumSinusoidAmplitude = 0.6
+                MinimumSinusoidAmplitude = 0
+
+                ' Advanced Processing Parameters
+                FeatureDistanceDeviation = 2
+                FeatureOrientationDeviation = 20
+                HandleOverlappingSinusoids = 1 '(1 = yes, 0 = no)
+                FeatureMergingConstraint = 0.6
+                SinusoidCompleteness = 1 '(1 = yes, 0 = no)
+                ClusterDipTolerance = 15
+                ClusterAzimuthTolerance = 15
+                DepthOffsetTolerance = 30
+                PixelBrightnessTolerance = 1
+                ImageSmoothingStrength = 20
+                ImageSmoothingSpeed = 0.25
+                ImageContrastSensitivity = 0.05
+
+        """
+        self._dispatch.PickSimilarFeatures(config_file_name)
+
+    def representative_picks(self, config_file_name):
+        """Runs the representative picks process in ISI
+
+        The representative Picks process uses an adapted Ward
+        algorithm to cluster picks which have the least dissimilarity
+        in azimuth, dip, depth distance from each other and pick type
+        (i.e. classification). As a result it determines the most
+        representative pick of each cluster - i.e. the (real) pick
+        with the highest confidence and closest to the center of each
+        cluster.
+
+        Parameters
+        ----------
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [RepresentativePicks]
+                InputLog = '(title of the log to process)
+                TopDepth = 0 '(top of the interval to process)
+                BottomDepth = 10 '(top of the interval to process)
+                AzimuthWindow = 5.0
+                TiltWindow = 5.0'(i.e. dip angle window)
+                DepthWindow = 0.5
+                KeepFeaturesUngrouped = yes / no
+        """
+        self._dispatch.RepresentativePicks(config_file_name)
+
+    def automatic_picking(self, config_file_name):
+        """Runs an automated structure picking in the ISI workspace
+
+        The Auto Picker allows the detection of planar structures in
+        televiewer (ATV, OTV) and electrical imager (e.g. FMI) images.
+        3D core scans are similar to OTV images and can be processed
+        as well.
+
+        Parameters
+        ----------
+        config : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [AutomaticPicking]
+                InputLog = Amplitude '(title of the log to process)
+                TopDepth = 0 '(top of the interval to process)
+                BottomDepth = 10 '(top of the interval to process)
+                ImageType = 3 '(0 = RGB OTV, 1 = Greyscale OTV, 2 = Diamond Drilled ATV, 3 = RC Drilled ATV, 4 = FMI)
+                DarkFeatures = yes /no
+                BrightFeatures = yes / no
+                Aperture = yes / no
+                PartialPicks = yes / no
+                UseDefaultSettings = yes / no
+
+                ' Processing Parameters
+                ImageWidth = 144
+                ImageSmoothingIterations = 2
+                MinimumFeatureSize = 5
+                DesiredFeatureStrength = 0.5
+                MinimumFeatureStrength = 0.2
+                MinimumStructureAperture = 0.008
+                MaximumStructureAperture = 0.032
+                SinusoidalDeviationTolerance = 30
+                MaximumSinusoidAmplitude = 0.6
+                MinimumSinusoidAmplitude = 0
+
+                ' Advanced Processing Parameters
+                FeatureDistanceDeviation = 2
+                FeatureOrientationDeviation = 20
+                HandleOverlappingSinusoids = 1 '(1 = yes, 0 = no)
+                FeatureMergingConstraint = 0.6
+                SinusoidCompleteness = 1 '(1 = yes, 0 = no)
+                ClusterDipTolerance = 15
+                ClusterAzimuthTolerance = 15
+                DepthOffsetTolerance = 30
+                PixelBrightnessTolerance = 1
+                ImageSmoothingStrength = 20
+                ImageSmoothingSpeed = 0.25
+                ImageContrastSensitivity = 0.05
+        """
+        self._dispatch.AutomaticPicking(config_file_name)
+
+    def quick_pick(self, config_file_name):
+        """Runs a quick pick in ISI
+
+        The Quick Pick Process analyzes the image for features with
+        the highest confidence within given Azimuth, Dip and Depth
+        tolerances. E.g. if you would like to pick just the main event
+        every 1m interval and leave all other features unaccounted you
+        can use this process.
+
+        Parameters
+        ----------
+        config_file_name : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            .. code-block:: ini
+
+                [QuickPick]
+                InputLog = Amplitude '(title of the log to process)
+                TopDepth = 0 '(top of the interval to process)
+                BottomDepth = 10 '(top of the interval to process)
+                ImageType = 3 '(0 = RGB OTV, 1 = Greyscale OTV, 2 = Diamond Drilled ATV, 3 = RC Drilled ATV, 4 = FMI)
+                DarkFeatures = yes /no
+                BrightFeatures = yes / no
+                Aperture = yes / no
+                PartialPicks = yes / no
+                AzimuthWindow = 5.0
+                TiltWindow = 5.0'(i.e. dip angle window)
+                DepthWindow = 0.5
+                UseDefaultSettings = yes / no
+
+                ' Processing Parameters
+                ImageWidth = 144
+                ImageSmoothingIterations = 2
+                MinimumFeatureSize = 5
+                DesiredFeatureStrength = 0.5
+                MinimumFeatureStrength = 0.2
+                MinimumStructureAperture = 0.008
+                MaximumStructureAperture = 0.032
+                SinusoidalDeviationTolerance = 30
+                MaximumSinusoidAmplitude = 0.6
+                MinimumSinusoidAmplitude = 0
+
+                ' Advanced Processing Parameters
+                FeatureDistanceDeviation = 2
+                FeatureOrientationDeviation = 20
+                HandleOverlappingSinusoids = 1 '(1 = yes, 0 = no)
+                FeatureMergingConstraint = 0.6
+                SinusoidCompleteness = 1 '(1 = yes, 0 = no)
+                ClusterDipTolerance = 15
+                ClusterAzimuthTolerance = 15
+                DepthOffsetTolerance = 30
+                PixelBrightnessTolerance = 1
+                ImageSmoothingStrength = 20
+                ImageSmoothingSpeed = 0.25
+                ImageContrastSensitivity = 0.05
+        """
+
+        self._dispatch.QuickPick(config_file_name)
+
+    def apply_template(self, path, prompt_if_not_found=None, config_file_name=None):
+        """Applies a workspace template
+        
+        Allows the application of an ISI Workspace,
+        Casing Integrity Workspace or NMR Workspace template.
+
+        Parameters
+        ----------
+        path: str
+            String specifying the name and path of the
+            workspace template to be applied (\*.ist). Please note
+            that the file extension is different for the
+            ISI, Casing Integrity and NMR Workspaces.
+        prompt_if_not_found: bool, optional
+            Boolean indicating whether the dialog box to
+            prompt the user for logs not found in the
+            template is displayed or not. The default is
+            set to True.
+        config_file_name : str, optional
+            The configuration file. Read the WellCAD Help for
+            information on the syntax of the file.
+
+        Returns
+        -------
+        bool
+            Always returns True except for the WellCAD Reader and
+            Demo version for which the function returns False.
+        """
+        return self._dispatch.ApplyTemplate(path, prompt_if_not_found, config_file_name)
+
+    def auto_joint_detection(self, config_file_name):
+        """Detects the joints from the main log (data source) used
+        in the workspace.
+
+        Parameters
+        ----------
+        config_file_name : str, optional
+            Path to a configuration file or a parameter string. The
+            configuration file can contain the following options:
+
+            Note: This configuration is for WellCAD version 5.7 and onwards. For prior version, see the next section.
+
+            .. code-block:: ini
+
+                [AutoJointDetection]
+                Sensitivity = 5
+                TopAndBottom = yes
+
+            For WellCAD version 5.5 and 5.6, use this configuration instead:
+
+            .. code-block:: ini
+
+                [AutoJointDetection]
+                JointHeight=0.5
+                Sensitivity=100
+        """
+        self._dispatch.AutoJointDetection(config_file_name)
+
+    def add_joint_log_to_b_hole(self):
+        """Adds the Marker Log from the Casing Integrity
+        Workspace displaying the casing joints back to the
+        borehole document.
+        """
+        self._dispatch.AddJointLogToBHole()
+
+    def add_engin_log_from_driller_casing_table_to_b_hole(self):
+        """Adds the Engineering Log from the Navigation Bar
+        of the Casing Integrity Workspace displaying the
+        drillers casing info back to the borehole document.
+
+        Note: this function is deprecated in WellCAD 5.7 and onwards
+        """
+        self._dispatch.AddEnginLogFromDrillerCasingTableToBHole()
+
+    def add_engin_log_from_logger_casing_table_to_b_hole(self):
+        """Adds the Engineering Log from the Navigation Bar
+        of the Casing Integrity Workspace displaying the
+        casing info derived from the logged data back to the
+        borehole document.
+        """
+        self._dispatch.AddEnginLogFromLoggerCasingTableToBHole()
```

