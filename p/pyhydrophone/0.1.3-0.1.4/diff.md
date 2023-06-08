# Comparing `tmp/pyhydrophone-0.1.3.tar.gz` & `tmp/pyhydrophone-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhydrophone-0.1.3.tar", last modified: Tue Jan 31 08:11:46 2023, max compression
+gzip compressed data, was "dist\pyhydrophone-0.1.4.tar", last modified: Thu Jun  8 09:33:19 2023, max compression
```

## Comparing `pyhydrophone-0.1.3.tar` & `pyhydrophone-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/
--rw-rw-rw-   0        0        0    35823 2022-01-11 08:38:32.000000 pyhydrophone-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6163 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4753 2022-02-01 08:48:19.000000 pyhydrophone-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/pyhydrophone/
--rw-rw-rw-   0        0        0      345 2022-11-23 08:43:01.000000 pyhydrophone-0.1.3/pyhydrophone/__init__.py
--rw-rw-rw-   0        0        0     2979 2022-02-01 08:48:19.000000 pyhydrophone-0.1.3/pyhydrophone/amar.py
--rw-rw-rw-   0        0        0     6112 2022-01-11 08:38:32.000000 pyhydrophone-0.1.3/pyhydrophone/bruelkjaer.py
--rw-rw-rw-   0        0        0     2091 2022-02-01 08:48:19.000000 pyhydrophone-0.1.3/pyhydrophone/ears.py
--rw-rw-rw-   0        0        0     4377 2022-02-04 13:20:07.000000 pyhydrophone-0.1.3/pyhydrophone/hydrophone.py
--rw-rw-rw-   0        0        0     2132 2022-11-23 08:32:21.000000 pyhydrophone-0.1.3/pyhydrophone/icListen.py
--rw-rw-rw-   0        0        0     1999 2022-02-01 08:48:19.000000 pyhydrophone-0.1.3/pyhydrophone/mte.py
--rw-rw-rw-   0        0        0     9465 2022-10-20 13:36:40.000000 pyhydrophone-0.1.3/pyhydrophone/rtsys.py
--rw-rw-rw-   0        0        0    12907 2022-11-08 13:21:18.000000 pyhydrophone-0.1.3/pyhydrophone/soundtrap.py
--rw-rw-rw-   0        0        0     2028 2022-02-01 08:48:19.000000 pyhydrophone-0.1.3/pyhydrophone/upam.py
-drwxrwxrwx   0        0        0        0 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/pyhydrophone.egg-info/
--rw-rw-rw-   0        0        0     6163 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/pyhydrophone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/pyhydrophone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/pyhydrophone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-02-03 15:24:29.000000 pyhydrophone-0.1.3/pyhydrophone.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/pyhydrophone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      585 2023-01-31 08:11:46.000000 pyhydrophone-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      434 2023-01-31 08:11:05.000000 pyhydrophone-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/
+-rw-rw-rw-   0        0        0    35823 2022-01-11 08:38:32.000000 pyhydrophone-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6522 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5016 2023-06-08 09:09:29.000000 pyhydrophone-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone/
+-rw-rw-rw-   0        0        0      345 2022-11-23 08:43:01.000000 pyhydrophone-0.1.4/pyhydrophone/__init__.py
+-rw-rw-rw-   0        0        0     2979 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/amar.py
+-rw-rw-rw-   0        0        0     6112 2022-01-11 08:38:32.000000 pyhydrophone-0.1.4/pyhydrophone/bruelkjaer.py
+-rw-rw-rw-   0        0        0     2091 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/ears.py
+-rw-rw-rw-   0        0        0     4377 2022-02-04 13:20:07.000000 pyhydrophone-0.1.4/pyhydrophone/hydrophone.py
+-rw-rw-rw-   0        0        0     2132 2022-11-23 08:32:21.000000 pyhydrophone-0.1.4/pyhydrophone/icListen.py
+-rw-rw-rw-   0        0        0     1999 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/mte.py
+-rw-rw-rw-   0        0        0    11405 2023-06-08 09:32:37.000000 pyhydrophone-0.1.4/pyhydrophone/rtsys.py
+-rw-rw-rw-   0        0        0    13860 2023-06-02 14:38:03.000000 pyhydrophone-0.1.4/pyhydrophone/soundtrap.py
+-rw-rw-rw-   0        0        0     2028 2022-02-01 08:48:19.000000 pyhydrophone-0.1.4/pyhydrophone/upam.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/
+-rw-rw-rw-   0        0        0     6522 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-02-03 15:24:29.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/pyhydrophone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      585 2023-06-08 09:33:19.000000 pyhydrophone-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      363 2023-06-08 09:25:01.000000 pyhydrophone-0.1.4/setup.py
```

### Comparing `pyhydrophone-0.1.3/LICENSE` & `pyhydrophone-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/PKG-INFO` & `pyhydrophone-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhydrophone
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python scripts to read hydrophones files
 Home-page: https://github.com/lifewatch/pyhydrophone.git
 Author: Clea Parcerisas
 Author-email: clea.parcerisas@vliz.be
 License: UNKNOWN
 Description: # pyhydrophone
         
@@ -18,15 +18,16 @@
         - AMAR (JASCO)
         - B&K Nexus (Bruel & Kjaer)
         - RTSys (RESEA)
         - EARS
         - MTE AURAL (Seiche)
         
         They all inherit from the main class Hydrophone. 
-        If a hydrophone provides an output different than a regular wav file, functions to read and understand the output are provided. 
+        If a hydrophone provides an output different from a regular wav file, functions to read and understand the 
+        output are provided. 
         Functions to read the metadata are also provided (which is often encoded in the file name).
         
         
         ## How to install
         # Using pip
         ```bash
         pip install pyhydrophone
@@ -37,19 +38,22 @@
         pip install setup.py
         ```
         ```bash
         pip install -r requirements.txt
         ```
         
         ## How to use
-        pyhydrophone allows to create an object which represents the hydrophone so you can just pass the hydrophone object from one function to another of your analysis without repeating all the parameters. 
+        pyhydrophone allows to create an object which represents the hydrophone so you can just pass the hydrophone object from 
+        one function to another of your analysis without repeating all the parameters. 
         
-        The object has some extra functions as reading the datetime when it was recorded (usually it is stored in the file name, but some times there is an extra metadata file). 
+        The object has some extra functions as reading the datetime when it was recorded (usually it is stored in the file name, 
+        but sometimes there is an extra metadata file). 
         
-        The normal use would be to create the hydrophone object and then start reading your files. Every time you want to know the datetime of your file you would do:
+        The normal use would be to create the hydrophone object and then start reading your files. Every time you want to know 
+        the datetime of your file you would do:
         ```
         hydrophone.get_name_date(path_to_your_file) 
         ```
         and you would not have to worry about which format the file name has or where the information of the datetime is stored.
         
         
         
@@ -68,22 +72,26 @@
         It is the base class, which can be used in case the user is only interested in keeping the parameters together. 
         
         ### SoundTrap 
         Provides two classes, SoundTrap and SoundTrapHF. 
         
         The date format of the file is assumed to be: *model_name.yymmddHHMMSS.ext*
         
-        To create a SoundTrap object, sensitiviy and preamp_gain are read from the configuration file. They do not have to be specified by the user.
+        To create a SoundTrap object, sensitiviy and preamp_gain are read from the configuration file. 
+        They do not have to be specified by the user.
         (Gain type "High" or "Low" has to be specified).
         A routine for reading the xml file is provided (still some parameters missing).
         
-        In a future it will be implemented to read the calibration from oceaninstruments but now the calibration file has to be saved inside the folder "calibration/" under the name of the serial number with THE SAME structure than the one exemplified. 
-        (information can be obtained from http://oceaninstruments.azurewebsites.net/App/#/%23)
+        If the serial number is passed, the calibration information will automatically be obtained
+        from http://oceaninstruments.azurewebsites.net/App/#/%23). 
+        If when searching for your serial number there are multiple options, it is important that you specify the model of the 
+        hydrophone correctly (as listed in the calibration sheed in oceaninstruments) so the right calibration is selected.
         
-        SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the high frequency clicks as a pandas df to be able to work with them. 
+        SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the 
+        high frequency clicks as a pandas df to be able to work with them. 
         
         A folder with several (xml, bcl, dwv) files can be specified and passed to the function.
         
         ### uPam
         For now only provides a method to read the date from the filename as it comes out from the device.
         
         The date format of the file is assumed to be: *project_name_yymmdd_HHMMSS_NUM.ext*
@@ -107,23 +115,27 @@
         signal is created at the beggining of the file. It has to be specified if it is a "test" signal or a "reference" signal
         to be used for calibration.
         
         https://www.bksv.com/en/products/transducers/conditioning/microphone/2690-A-0F2
         
         
         ### RTSys
-        Provides a method to read the date from the file name. It also adds a method to compute the power consumtion and plot it
-        over time.
+        Provides a method to read the date from the file name. 
+        It has a method to read the header from a wav file recorded using a RESEA recorder.
+        It also adds a method to compute the power consumption and plot it over time.
         https://rtsys.eu/acoustic-recorders
         
         ### EARS
         Just provides a method to read the date time from the name.
         
         ### MTE AURAL
         Just provides a method to read the date time from the name.
         http://www.multi-electronique.com/files/AURAL/user/AURAL-M2_USER_GUIDE.pdf
+        
+        ### icListen 
+        In development. Just provides a method to read the date time from the name for the moment.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyhydrophone-0.1.3/README.md` & `pyhydrophone-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 - AMAR (JASCO)
 - B&K Nexus (Bruel & Kjaer)
 - RTSys (RESEA)
 - EARS
 - MTE AURAL (Seiche)
 
 They all inherit from the main class Hydrophone. 
-If a hydrophone provides an output different than a regular wav file, functions to read and understand the output are provided. 
+If a hydrophone provides an output different from a regular wav file, functions to read and understand the 
+output are provided. 
 Functions to read the metadata are also provided (which is often encoded in the file name).
 
 
 ## How to install
 # Using pip
 ```bash
 pip install pyhydrophone
@@ -29,19 +30,22 @@
 pip install setup.py
 ```
 ```bash
 pip install -r requirements.txt
 ```
 
 ## How to use
-pyhydrophone allows to create an object which represents the hydrophone so you can just pass the hydrophone object from one function to another of your analysis without repeating all the parameters. 
+pyhydrophone allows to create an object which represents the hydrophone so you can just pass the hydrophone object from 
+one function to another of your analysis without repeating all the parameters. 
 
-The object has some extra functions as reading the datetime when it was recorded (usually it is stored in the file name, but some times there is an extra metadata file). 
+The object has some extra functions as reading the datetime when it was recorded (usually it is stored in the file name, 
+but sometimes there is an extra metadata file). 
 
-The normal use would be to create the hydrophone object and then start reading your files. Every time you want to know the datetime of your file you would do:
+The normal use would be to create the hydrophone object and then start reading your files. Every time you want to know 
+the datetime of your file you would do:
 ```
 hydrophone.get_name_date(path_to_your_file) 
 ```
 and you would not have to worry about which format the file name has or where the information of the datetime is stored.
 
 
 
@@ -60,22 +64,26 @@
 It is the base class, which can be used in case the user is only interested in keeping the parameters together. 
 
 ### SoundTrap 
 Provides two classes, SoundTrap and SoundTrapHF. 
 
 The date format of the file is assumed to be: *model_name.yymmddHHMMSS.ext*
 
-To create a SoundTrap object, sensitiviy and preamp_gain are read from the configuration file. They do not have to be specified by the user.
+To create a SoundTrap object, sensitiviy and preamp_gain are read from the configuration file. 
+They do not have to be specified by the user.
 (Gain type "High" or "Low" has to be specified).
 A routine for reading the xml file is provided (still some parameters missing).
 
-In a future it will be implemented to read the calibration from oceaninstruments but now the calibration file has to be saved inside the folder "calibration/" under the name of the serial number with THE SAME structure than the one exemplified. 
-(information can be obtained from http://oceaninstruments.azurewebsites.net/App/#/%23)
+If the serial number is passed, the calibration information will automatically be obtained
+from http://oceaninstruments.azurewebsites.net/App/#/%23). 
+If when searching for your serial number there are multiple options, it is important that you specify the model of the 
+hydrophone correctly (as listed in the calibration sheed in oceaninstruments) so the right calibration is selected.
 
-SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the high frequency clicks as a pandas df to be able to work with them. 
+SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the 
+high frequency clicks as a pandas df to be able to work with them. 
 
 A folder with several (xml, bcl, dwv) files can be specified and passed to the function.
 
 ### uPam
 For now only provides a method to read the date from the filename as it comes out from the device.
 
 The date format of the file is assumed to be: *project_name_yymmdd_HHMMSS_NUM.ext*
@@ -99,17 +107,21 @@
 signal is created at the beggining of the file. It has to be specified if it is a "test" signal or a "reference" signal
 to be used for calibration.
 
 https://www.bksv.com/en/products/transducers/conditioning/microphone/2690-A-0F2
 
 
 ### RTSys
-Provides a method to read the date from the file name. It also adds a method to compute the power consumtion and plot it
-over time.
+Provides a method to read the date from the file name. 
+It has a method to read the header from a wav file recorded using a RESEA recorder.
+It also adds a method to compute the power consumption and plot it over time.
 https://rtsys.eu/acoustic-recorders
 
 ### EARS
 Just provides a method to read the date time from the name.
 
 ### MTE AURAL
 Just provides a method to read the date time from the name.
-http://www.multi-electronique.com/files/AURAL/user/AURAL-M2_USER_GUIDE.pdf
+http://www.multi-electronique.com/files/AURAL/user/AURAL-M2_USER_GUIDE.pdf
+
+### icListen 
+In development. Just provides a method to read the date time from the name for the moment.
```

### Comparing `pyhydrophone-0.1.3/pyhydrophone/amar.py` & `pyhydrophone-0.1.4/pyhydrophone/amar.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/pyhydrophone/bruelkjaer.py` & `pyhydrophone-0.1.4/pyhydrophone/bruelkjaer.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/pyhydrophone/ears.py` & `pyhydrophone-0.1.4/pyhydrophone/ears.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/pyhydrophone/hydrophone.py` & `pyhydrophone-0.1.4/pyhydrophone/hydrophone.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/pyhydrophone/icListen.py` & `pyhydrophone-0.1.4/pyhydrophone/icListen.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/pyhydrophone/mte.py` & `pyhydrophone-0.1.4/pyhydrophone/mte.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/pyhydrophone/rtsys.py` & `pyhydrophone-0.1.4/pyhydrophone/rtsys.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,21 +28,28 @@
         Serial number of the acoustic recorder
     sensitivity : float
         Sensitivity of the acoustic recorder in db
     preamp_gain : float
         Gain of the preamplifier in dB
     Vpp : float
         Voltage peak to peak in volts
+    mode: string
+        Can be 'lowpower' or 'broadband'
+    channel: string
+        Channel to process, 'A', 'B', 'C' or 'D'
     string_format : string
         Format of the datetime string present in the filename
     """
-    def __init__(self, name, model, serial_number, sensitivity, preamp_gain, Vpp, string_format="%Y-%m-%d_%H-%M-%S"):
+    def __init__(self, name, model, serial_number, sensitivity, preamp_gain, Vpp, mode, channel='A',
+                 string_format="%Y-%m-%d_%H-%M-%S"):
         super().__init__(name, model, serial_number, sensitivity, preamp_gain, Vpp, string_format)
         self.cal_freq = 250
         self.cal_value = 114
+        self.mode = mode
+        self.channel = channel
 
     def get_name_datetime(self, file_name):
         """
         Get the data and time of recording from the name of the file
         Parameters
         ----------
         file_name : string
@@ -71,18 +78,26 @@
 
         return new_filename
 
     @staticmethod
     def _parse_board_file(board_file_path):
         board_info = pd.read_csv(board_file_path, delimiter=';', names=['id', 'T', 'V', 'I', 'P'],
                                  usecols=[0, 1, 2, 3, 4])
-        board_info['T'] = board_info['T'].str.replace('T:', '').astype(float)
-        board_info['V'] = board_info['V'].str.replace('V:', '').astype(float)
-        board_info['I'] = board_info['I'].str.replace('I:', '').astype(float)
-        board_info['P'] = board_info['P'].str.replace('P:', '').astype(float)
+        board_info['T'] = board_info['T'].str.replace('T:', '')
+        board_info.loc[board_info['T'] == ''] = np.nan
+        board_info['T'] = board_info['T'].astype(float)
+        board_info['V'] = board_info['V'].str.replace('V:', '')
+        board_info.loc[board_info['V'] == ''] = np.nan
+        board_info['V'] = board_info['V'].astype(float)
+        board_info['I'] = board_info['I'].str.replace('I:', '')
+        board_info.loc[board_info['I'] == ''] = np.nan
+        board_info['I'] = board_info['I'].astype(float)
+        board_info['P'] = board_info['P'].str.replace('P:', '')
+        board_info.loc[board_info['P'] == ''] = np.nan
+        board_info['P'] = board_info['P'].astype(float)
         board_info['timestamp'] = pd.to_datetime(board_info['id'].str.replace('@:', '').astype(float), unit='s')
         board_info['dP'] = board_info['timestamp'].diff().dt.total_seconds() * board_info['P']
 
         return board_info
 
     def plot_consumption(self, board_file_path):
         """
@@ -91,26 +106,29 @@
         ----------
         board_file_path : str or Path
         """
         board_info = self._parse_board_file(board_file_path)
         board_info.plot(y=['V', 'P'])
         plt.show()
 
-    def plot_consumption_total_mission(self, mission_folder_path):
+    def plot_consumption_total_mission(self, mission_folder_path, ax=None, show=True):
         if not isinstance(mission_folder_path, pathlib.Path):
             mission_folder_path = pathlib.Path(mission_folder_path)
 
         total_board = pd.DataFrame()
         for board_file_i in mission_folder_path.glob('**/*.txt'):
             if 'board' in board_file_i.name:
                 board_i = self._parse_board_file(board_file_i)
                 total_board = pd.concat([total_board, board_i])
 
-        total_board.plot(x='timestamp', y=['V', 'P'], secondary_y='P')
-        plt.show()
+        if ax is None:
+            fig, ax = plt.subplots()
+        total_board.plot(x='timestamp', y=['V', 'P'], secondary_y='P', ax=ax)
+        if show:
+            plt.show()
 
     def compute_consumption(self, board_file_path):
         """
         Calculate the total energy consumption of the file
         Parameters
         ----------
         board_file_path : str or Path
@@ -198,35 +216,61 @@
                 extra_header[chunk_name] = struct.unpack(chunk_format['format'],
                                                          header_buffer[chunk_format['start']:chunk_format['end']])[0]
             else:
                 extra_header[chunk_name] = bytes.decode(header_buffer[chunk_format['start']:chunk_format['end']])
 
         return extra_header
 
-    @staticmethod
-    def from_header(file_path, mode='broadband', zip_mode=False):
-        extra_header = RTSys.read_header(file_path, zip_mode)
+    def update_metadata(self, file_path, zip_mode=False):
+        """
+        Creates a new RTSys object from an already existing one but updating the metadata from the file header.
+        The "mode" parameter stays the same.
+
+        Parameters
+        ----------
+        file_path: str or Path
+            path to the wav file recorded with RTSys with a correc header
+        zip_mode: bool
+            True if file is zipped, otherwise false
+        """
+        header = self.read_header(file_path, zip_mode)
+        name, model, serial_number, sens, ampl = self.meta_from_header(header)
+        return RTSys(name=name, model=model, serial_number=serial_number, sensitivity=sens, preamp_gain=ampl, Vpp=5.0,
+                     mode=self.mode)
+
+    def meta_from_header(self, header):
+        sens = header['hydrophone_sensitivity_%s' % self.channel]
+        name = 'RTSys'
+        model = None
+        serial_number = header['serial_number']
+
+        if self.mode == 'lowpower':
+            ampl = 20 * np.log10(5 / np.sqrt(2))
+        else:
+            ampl = 20 * np.log10((1 / (header['hydrophone_amplification_%s' % self.channel] *
+                                       header['correction_factor_%s' % self.channel])))
+        return name, model, serial_number, sens, ampl
+
+    def one_rtsys_per_channel_from_header(self, file_path, zip_mode=False):
+        extra_header = self.read_header(file_path, zip_mode)
         active_channels = []
         for channel_i in np.arange(4):
             if extra_header['active_channels'][channel_i] != '\x00':
                 active_channels.append(extra_header['active_channels'][channel_i])
 
         rtsys_list = []
         for channel in active_channels:
-            sens = extra_header['hydrophone_sensitivity_%s' % channel]
-            name = 'RTSys'
-            model = None
-            serial_number = extra_header['serial_number']
-
-            if mode == 'lowpower':
-                ampl = 20 * np.log10(5/np.sqrt(2))
-            else:
-                ampl = 20 * np.log10((1 / (extra_header['hydrophone_amplification_%s' % channel] *
-                                      extra_header['correction_factor_%s' % channel])))
-
+            name, model, serial_number, sens, ampl = self.meta_from_header(extra_header)
             rtsys_list.append(RTSys(name=name, model=model, serial_number=serial_number, sensitivity=sens,
-                                    preamp_gain=ampl, Vpp=5.0))
+                                    preamp_gain=ampl, Vpp=5.0, channel=channel))
 
         if len(rtsys_list) == 1:
             return rtsys_list[0]
         else:
             return rtsys_list
+
+    def calibrate(self, file_path, zip_mode=False):
+        header = self.read_header(file_path, zip_mode)
+        name, model, serial_number, sens, ampl = self.meta_from_header(header)
+        self.sensitivity = sens
+        self.preamp_gain = ampl
+        self.Vpp = 5.0
```

### Comparing `pyhydrophone-0.1.3/pyhydrophone/soundtrap.py` & `pyhydrophone-0.1.4/pyhydrophone/soundtrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,31 @@
     string_format : string
         Format of the datetime string present in the filename
     """
     def __init__(self, name, model, serial_number, sensitivity=None, gain_type='High', string_format="%y%m%d%H%M%S"):
         if sensitivity is None:
             try:
                 query = 'http://oceaninstruments.azurewebsites.net/api/Devices/Search/%s' % serial_number
-                response = requests.get(query).json()[0]
-                device_id = response['deviceId']
+                response = requests.get(query).json()
+                if len(response) > 1:
+                    models_available = {}
+                    for device in response:
+                        if device['serialNo'] == str(serial_number):
+                            models_available[device['modelName']] = device['deviceId']
+
+                    if model not in models_available.keys():
+                        raise AttributeError('There are multiple instruments with serial number %s. Set the model '
+                                             'parameter to match the model specified in the SoundTrap calibration '
+                                             'webpage to chose the correct one: %s' %
+                                             (serial_number, models_available.keys()))
+                    else:
+                        device_id = models_available[model]
+                else:
+                    # Ignore the model name if there is only one serial number
+                    device_id = response[0]['deviceId']
                 query = 'http://oceaninstruments.azurewebsites.net/api/Calibrations/Device/%s' % device_id
                 response = requests.get(query).json()[0]
                 if gain_type == 'High':
                     sensitivity = -response['highFreq']
                 elif gain_type == 'Low':
                     sensitivity = -response['lowFreq']
                 else:
```

### Comparing `pyhydrophone-0.1.3/pyhydrophone/upam.py` & `pyhydrophone-0.1.4/pyhydrophone/upam.py`

 * *Files identical despite different names*

### Comparing `pyhydrophone-0.1.3/pyhydrophone.egg-info/PKG-INFO` & `pyhydrophone-0.1.4/pyhydrophone.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhydrophone
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python scripts to read hydrophones files
 Home-page: https://github.com/lifewatch/pyhydrophone.git
 Author: Clea Parcerisas
 Author-email: clea.parcerisas@vliz.be
 License: UNKNOWN
 Description: # pyhydrophone
         
@@ -18,15 +18,16 @@
         - AMAR (JASCO)
         - B&K Nexus (Bruel & Kjaer)
         - RTSys (RESEA)
         - EARS
         - MTE AURAL (Seiche)
         
         They all inherit from the main class Hydrophone. 
-        If a hydrophone provides an output different than a regular wav file, functions to read and understand the output are provided. 
+        If a hydrophone provides an output different from a regular wav file, functions to read and understand the 
+        output are provided. 
         Functions to read the metadata are also provided (which is often encoded in the file name).
         
         
         ## How to install
         # Using pip
         ```bash
         pip install pyhydrophone
@@ -37,19 +38,22 @@
         pip install setup.py
         ```
         ```bash
         pip install -r requirements.txt
         ```
         
         ## How to use
-        pyhydrophone allows to create an object which represents the hydrophone so you can just pass the hydrophone object from one function to another of your analysis without repeating all the parameters. 
+        pyhydrophone allows to create an object which represents the hydrophone so you can just pass the hydrophone object from 
+        one function to another of your analysis without repeating all the parameters. 
         
-        The object has some extra functions as reading the datetime when it was recorded (usually it is stored in the file name, but some times there is an extra metadata file). 
+        The object has some extra functions as reading the datetime when it was recorded (usually it is stored in the file name, 
+        but sometimes there is an extra metadata file). 
         
-        The normal use would be to create the hydrophone object and then start reading your files. Every time you want to know the datetime of your file you would do:
+        The normal use would be to create the hydrophone object and then start reading your files. Every time you want to know 
+        the datetime of your file you would do:
         ```
         hydrophone.get_name_date(path_to_your_file) 
         ```
         and you would not have to worry about which format the file name has or where the information of the datetime is stored.
         
         
         
@@ -68,22 +72,26 @@
         It is the base class, which can be used in case the user is only interested in keeping the parameters together. 
         
         ### SoundTrap 
         Provides two classes, SoundTrap and SoundTrapHF. 
         
         The date format of the file is assumed to be: *model_name.yymmddHHMMSS.ext*
         
-        To create a SoundTrap object, sensitiviy and preamp_gain are read from the configuration file. They do not have to be specified by the user.
+        To create a SoundTrap object, sensitiviy and preamp_gain are read from the configuration file. 
+        They do not have to be specified by the user.
         (Gain type "High" or "Low" has to be specified).
         A routine for reading the xml file is provided (still some parameters missing).
         
-        In a future it will be implemented to read the calibration from oceaninstruments but now the calibration file has to be saved inside the folder "calibration/" under the name of the serial number with THE SAME structure than the one exemplified. 
-        (information can be obtained from http://oceaninstruments.azurewebsites.net/App/#/%23)
+        If the serial number is passed, the calibration information will automatically be obtained
+        from http://oceaninstruments.azurewebsites.net/App/#/%23). 
+        If when searching for your serial number there are multiple options, it is important that you specify the model of the 
+        hydrophone correctly (as listed in the calibration sheed in oceaninstruments) so the right calibration is selected.
         
-        SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the high frequency clicks as a pandas df to be able to work with them. 
+        SoundTrapHF (inherited from SoundTrap) comes with a routine to read the *.dwv files from SoundTrap and store all the 
+        high frequency clicks as a pandas df to be able to work with them. 
         
         A folder with several (xml, bcl, dwv) files can be specified and passed to the function.
         
         ### uPam
         For now only provides a method to read the date from the filename as it comes out from the device.
         
         The date format of the file is assumed to be: *project_name_yymmdd_HHMMSS_NUM.ext*
@@ -107,23 +115,27 @@
         signal is created at the beggining of the file. It has to be specified if it is a "test" signal or a "reference" signal
         to be used for calibration.
         
         https://www.bksv.com/en/products/transducers/conditioning/microphone/2690-A-0F2
         
         
         ### RTSys
-        Provides a method to read the date from the file name. It also adds a method to compute the power consumtion and plot it
-        over time.
+        Provides a method to read the date from the file name. 
+        It has a method to read the header from a wav file recorded using a RESEA recorder.
+        It also adds a method to compute the power consumption and plot it over time.
         https://rtsys.eu/acoustic-recorders
         
         ### EARS
         Just provides a method to read the date time from the name.
         
         ### MTE AURAL
         Just provides a method to read the date time from the name.
         http://www.multi-electronique.com/files/AURAL/user/AURAL-M2_USER_GUIDE.pdf
+        
+        ### icListen 
+        In development. Just provides a method to read the date time from the name for the moment.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyhydrophone-0.1.3/setup.cfg` & `pyhydrophone-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7968 7964 726f 7068 6f6e 650d   = pyhydrophone.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e33  .version = 0.1.3
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e34  .version = 0.1.4
 00000030: 0d0a 6175 7468 6f72 203d 2043 6c65 6120  ..author = Clea 
 00000040: 5061 7263 6572 6973 6173 0d0a 6175 7468  Parcerisas..auth
 00000050: 6f72 5f65 6d61 696c 203d 2063 6c65 612e  or_email = clea.
 00000060: 7061 7263 6572 6973 6173 4076 6c69 7a2e  parcerisas@vliz.
 00000070: 6265 0d0a 6465 7363 7269 7074 696f 6e20  be..description 
 00000080: 3d20 5079 7468 6f6e 2073 6372 6970 7473  = Python scripts
 00000090: 2074 6f20 7265 6164 2068 7964 726f 7068   to read hydroph
```

