# Comparing `tmp/spectrum_card-1.0.1.tar.gz` & `tmp/spectrum_card-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_card-1.0.1.tar", max compression
+gzip compressed data, was "spectrum_card-1.1.0.tar", max compression
```

## Comparing `spectrum_card-1.0.1.tar` & `spectrum_card-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1537 2023-04-06 02:01:50.678562 spectrum_card-1.0.1/LICENSE
--rw-r--r--   0        0        0      389 2023-05-12 07:08:28.077948 spectrum_card-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      104 2023-04-06 02:01:50.678562 spectrum_card-1.0.1/README.md
--rw-r--r--   0        0        0   155889 2023-05-12 07:08:54.332975 spectrum_card-1.0.1/spectrum_card/__init__.py
--rw-r--r--   0        0        0    83349 2022-11-08 15:04:34.000000 spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/regs.py
--rw-r--r--   0        0        0     2124 2022-11-08 15:04:34.000000 spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/spcerr.py
--rw-r--r--   0        0        0     8681 2023-05-12 07:04:19.611035 spectrum_card-1.0.1/spectrum_card/spectrum_header/pyspcm.py
--rw-r--r--   0        0        0     2025 2023-04-06 01:54:09.473754 spectrum_card-1.0.1/spectrum_card/spectrum_header/spcm_tools.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 spectrum_card-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1537 2023-04-06 02:01:50.678562 spectrum_card-1.1.0/LICENSE
+-rw-r--r--   0        0        0      389 2023-06-08 04:26:08.218740 spectrum_card-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-04-06 02:01:50.678562 spectrum_card-1.1.0/README.md
+-rw-r--r--   0        0        0   156105 2023-06-08 04:21:52.529944 spectrum_card-1.1.0/spectrum_card/__init__.py
+-rw-r--r--   0        0        0    83349 2022-11-08 15:04:34.000000 spectrum_card-1.1.0/spectrum_card/spectrum_header/py_header/regs.py
+-rw-r--r--   0        0        0     2124 2022-11-08 15:04:34.000000 spectrum_card-1.1.0/spectrum_card/spectrum_header/py_header/spcerr.py
+-rw-r--r--   0        0        0     8681 2023-05-12 07:04:19.611035 spectrum_card-1.1.0/spectrum_card/spectrum_header/pyspcm.py
+-rw-r--r--   0        0        0     2025 2023-04-06 01:54:09.473754 spectrum_card-1.1.0/spectrum_card/spectrum_header/spcm_tools.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 spectrum_card-1.1.0/PKG-INFO
```

### Comparing `spectrum_card-1.0.1/LICENSE` & `spectrum_card-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.1/spectrum_card/__init__.py` & `spectrum_card-1.1.0/spectrum_card/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3966,14 +3966,16 @@
       self.set_current_segment(segment)
 
     # Initialise buffer
     stride = self.get_sample_resolution()
     channels = self.get_number_of_active_channels()
     data_buffer = spcm_tools.pvAllocMemPageAligned(channels*stride*data[0].size)
     data_pointer = spcm_tools.cast(data_buffer, spcm.ptr16)
+    if aux_data is None:
+      data_np = np.frombuffer(data_buffer, dtype = np.int16)
 
     digital_output_used = [False, False, False]
     for channel in range(channels):
       # Find out if there are digital outs and, if so, set the discretisation rate
       max_bits = self.get_sample_resolution_bits()
       aux_data_reverse_lookup = []
       if aux_data is not None:
@@ -3984,20 +3986,23 @@
             aux_data_reverse_lookup.append([aux_data_channel_index, bit])
             self.use_io_mode_digital_out(aux_data_channel["Port"], aux_data_channel["Channel"], aux_data_channel["Bit"])
             digital_output_used[aux_data_channel["Port"]] = True
       limit = int(2**(max_bits - 1) - 1)
 
       # Add waveform and digital outs to buffer
       channel_data = data[channel]
-      for sample_index, sample in enumerate(channel_data):
-        # Discretise waveform, and blank out bits meant for aux digital out
-        data_pointer[channel + channels*sample_index] = int(limit*np.clip(sample, -1, 1)) & (~(0x7 << max_bits))
-        # Append aux digital outs
-        for reverse_lookup in aux_data_reverse_lookup:
-          data_pointer[channel + channels*sample_index] |= (int(aux_data[reverse_lookup[0]][sample_index]) & 1) << reverse_lookup[1]
+      if aux_data is None:
+        data_np[channel::channels] = limit*np.clip(channel_data, -1, 1)
+      else:
+        for sample_index, sample in enumerate(channel_data):
+          # Discretise waveform, and blank out bits meant for aux digital out
+          data_pointer[channel + channels*sample_index] = int(limit*np.clip(sample, -1, 1)) & (~(0x7 << max_bits))
+          # Append aux digital outs
+          for reverse_lookup in aux_data_reverse_lookup:
+            data_pointer[channel + channels*sample_index] |= (int(aux_data[reverse_lookup[0]][sample_index]) & 1) << reverse_lookup[1]
     
     # Disable ports if digital io are not in use
     for port in range(3):
       if not digital_output_used[port]:
         io_mode = self.get_io_mode_information(port)
         if "Digital out" in io_mode:
           self.io_port_disable(port)
@@ -4769,8 +4774,8 @@
     
     Returns
     -------
     value : :obj:`bool`
       Port value.
     """
     bit_code = self.get_io_asynchronous_register()
-    return (bit_code & (1 << port)) != 0
+    return (bit_code & (1 << port)) != 0
```

### Comparing `spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/regs.py` & `spectrum_card-1.1.0/spectrum_card/spectrum_header/py_header/regs.py`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.1/spectrum_card/spectrum_header/py_header/spcerr.py` & `spectrum_card-1.1.0/spectrum_card/spectrum_header/py_header/spcerr.py`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.1/spectrum_card/spectrum_header/pyspcm.py` & `spectrum_card-1.1.0/spectrum_card/spectrum_header/pyspcm.py`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.1/spectrum_card/spectrum_header/spcm_tools.py` & `spectrum_card-1.1.0/spectrum_card/spectrum_header/spcm_tools.py`

 * *Files identical despite different names*

### Comparing `spectrum_card-1.0.1/PKG-INFO` & `spectrum_card-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum-card
-Version: 1.0.1
+Version: 1.1.0
 Summary: Wrapper to be used with AWG cards from Spectrum Instruments.
 License: BSD 3 Clause
 Author: Alexander Tritt Monash
 Author-email: alexander.tritt@monash.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

