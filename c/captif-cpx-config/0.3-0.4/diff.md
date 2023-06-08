# Comparing `tmp/captif_cpx_config-0.3.tar.gz` & `tmp/captif_cpx_config-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.3.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.4.tar", max compression
```

## Comparing `captif_cpx_config-0.3.tar` & `captif_cpx_config-0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/LICENSE
--rw-r--r--   0        0        0       19 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/README.md
--rw-r--r--   0        0        0       44 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     3959 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      498 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/LICENSE
+-rw-r--r--   0        0        0       19 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/README.md
+-rw-r--r--   0        0        0       44 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     4168 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      521 2023-06-08 04:28:05.170526 captif_cpx_config-0.4/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.4/PKG-INFO
```

### Comparing `captif_cpx_config-0.3/LICENSE` & `captif_cpx_config-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.3/captif_cpx_config/metadata.py` & `captif_cpx_config-0.4/captif_cpx_config/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,58 @@
 from datetime import date as date_
 import json
 from typing import Literal, Optional
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, condecimal
 
 
 class MicrophoneDetails(BaseModel):
     microphone_position: int = Field(
         description="microphone position (1-6) as per ISO 11819-2:2017",
     )
     microphone_serial_number: str = Field(
         description="microphone serial number",
     )
-    microphone_sensitivity_mv_pa: float = Field(
+    microphone_sensitivity_mv_pa: condecimal(decimal_places=2) = Field(
         description="microphone sensitivity in mV/Pa",
     )
     microphone_calibration_date: date_ = Field(
         description="microphone calibration date",
     )
     wav_file_channel_number: int = Field(
         description=(
-            "channel number in the wav file corresponding to the microphone " "position"
+            "channel number in the wav file corresponding to the microphone "
+            "position. The channels number uses zero-based indexing."
         ),
     )
 
 
 class AccelerometerDetails(BaseModel):
     accelerometer_position: Literal["chassis", "axle"] = Field(
         description="accelerometer position ('chassis' or 'axle')",
     )
     accelerometer_serial_number: str = Field(
         description="accelerometer serial number",
     ),
-    accelerometer_sensitivity_mv_g: float = Field(
+    accelerometer_sensitivity_mv_g: condecimal(decimal_places=2) = Field(
         description="accelerometer sensitivity in mV/g",
     )
     wav_file_channel_number: int = Field(
         description=(
-            "channel number in the wav file corresponding to the accelerometer"
+            "channel number in the wav file corresponding to the "
+            "accelerometer. The channels number uses zero-based indexing."
         ),
     )
 
 
-class TyreDetails(BaseModel):
-    tyre: str = Field(
-        description="tyre name/type (e.g. 'P1', 'H1', etc.)",
-    )
-    tyre_purchase_date: date_ = Field(
-        description="tyre purchase date",
-    )
-    hardness: float = Field(
-        description="tyre hardness in Shore A",
-    )
-    hardness_date: date_ = Field(
-        description="tyre hardness measurement date",
-    )
-
 
 class DeviceCorrections(BaseModel):
-    frequency_hz: list[float] = Field(
+    frequency_hz: list[condecimal(decimal_places=1)] = Field(
         description="list third-octave band centre frequencies in Hz",
     )
-    correction_db: list[float] = Field(
+    correction_db: list[condecimal(decimal_places=2)] = Field(
         description="list of device corrections in dB",
     )
 
 
 class MeasurementDetails(BaseModel):
     date: date_ = Field(
         description="date of measurement",
@@ -86,15 +74,15 @@
     )
     wheel_track: Literal["left", "right", "both"] = Field(
         description="wheel track being measured (left, right, or both)",
     )
     hours_since_last_rain: int = Field(
         description="hours since last rain",
     )
-    wav_scale: float = Field(
+    wav_scale: condecimal(decimal_places=1) = Field(
         description=(
             "scale factor to apply to the raw wav file data (-1 to + 1 range) "
             "to convert the data back into volts."
         ),
     )
     notes: str = Field(
         description="any additional notes",
@@ -107,17 +95,29 @@
     )
     wheel_bay_configuration_details: str = Field(
         description="description of the wheel bay configuration",
     )
     wheel_bay_calibration_date: date_ = Field(
         description="wheel bay / device correction calibration date"
     )
+    tyre: str = Field(
+        description="tyre name/type (e.g. 'P1', 'H1', etc.)",
+    )
+    tyre_purchase_date: date_ = Field(
+        description="tyre purchase date",
+    )
+    hardness: condecimal(decimal_places=1) = Field(
+        description="tyre hardness in Shore A",
+    )
+    hardness_date: date_ = Field(
+        description="tyre hardness measurement date",
+    )
+
     microphone_details: list["MicrophoneDetails"]
     accelerometer_details: list["AccelerometerDetails"] = []
-    tyre_details: "TyreDetails"
     device_corrections: "DeviceCorrections"
 
 
 class Metadata(BaseModel):
     measurement_details: "MeasurementDetails"
     wheel_bay_details: list["WheelBayDetails"]
```

### Comparing `captif_cpx_config-0.3/PKG-INFO` & `captif_cpx_config-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.3
+Version: 0.4
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

