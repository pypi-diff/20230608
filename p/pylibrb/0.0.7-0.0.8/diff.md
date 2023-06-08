# Comparing `tmp/pylibrb-0.0.7.tar.gz` & `tmp/pylibrb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibrb-0.0.7.tar", last modified: Tue May 30 10:56:07 2023, max compression
+gzip compressed data, was "pylibrb-0.0.8.tar", last modified: Thu Jun  8 13:44:25 2023, max compression
```

## Comparing `pylibrb-0.0.7.tar` & `pylibrb-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-30 10:55:55.000000 pylibrb-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 10:55:55.000000 pylibrb-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-30 10:56:07.871985 pylibrb-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-30 10:55:55.000000 pylibrb-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 10:55:55.000000 pylibrb-0.0.7/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-30 10:55:55.000000 pylibrb-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 10:56:07.871985 pylibrb-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-30 10:55:55.000000 pylibrb-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.867985 pylibrb-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/src/pylibrb/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-30 10:55:55.000000 pylibrb-0.0.7/src/pylibrb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:55.000000 pylibrb-0.0.7/src/pylibrb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36591 2023-05-30 10:55:55.000000 pylibrb-0.0.7/src/pylibrb/pylibrb_ext.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/src/pylibrb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-30 10:55:55.000000 pylibrb-0.0.7/tests/test_stretcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-30 10:55:55.000000 pylibrb-0.0.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:25.812331 pylibrb-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-06-08 13:44:13.000000 pylibrb-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 13:44:13.000000 pylibrb-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-08 13:44:25.812331 pylibrb-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-08 13:44:13.000000 pylibrb-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 13:44:13.000000 pylibrb-0.0.8/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 13:44:13.000000 pylibrb-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 13:44:25.816331 pylibrb-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 13:44:13.000000 pylibrb-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:25.812331 pylibrb-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:25.812331 pylibrb-0.0.8/src/pylibrb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-08 13:44:13.000000 pylibrb-0.0.8/src/pylibrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:13.000000 pylibrb-0.0.8/src/pylibrb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-06-08 13:44:13.000000 pylibrb-0.0.8/src/pylibrb/pylibrb_ext.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:25.812331 pylibrb-0.0.8/src/pylibrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-08 13:44:25.000000 pylibrb-0.0.8/src/pylibrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 13:44:25.000000 pylibrb-0.0.8/src/pylibrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:44:25.000000 pylibrb-0.0.8/src/pylibrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 13:44:25.000000 pylibrb-0.0.8/src/pylibrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 13:44:25.000000 pylibrb-0.0.8/src/pylibrb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:25.812331 pylibrb-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-08 13:44:13.000000 pylibrb-0.0.8/tests/test_stretcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-08 13:44:13.000000 pylibrb-0.0.8/tests/test_utils.py
```

### Comparing `pylibrb-0.0.7/LICENSE` & `pylibrb-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.7/PKG-INFO` & `pylibrb-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pylibrb
 [![tests](https://github.com/pawel-glomski/pylibrb/actions/workflows/test.yml/badge.svg)](https://github.com/pawel-glomski/pylibrb/actions/workflows/test.yml)
+[![PyPI version](https://img.shields.io/pypi/v/pylibrb)](https://pypi.org/project/pylibrb/)
 
 pylibrb (py-lib-rubberband) is a simple Python extension exposing [Rubber Band Library](https://breakfastquay.com/rubberband/) using [nanobind](https://github.com/wjakob/nanobind) bindings.
 
-Since this is not a wrapper around a command-line app (like [pyrubberband](https://github.com/bmcfee/pyrubberband)), both offline and real-time modes are available.
+Since this is not a wrapper around a command-line tool (like [pyrubberband](https://github.com/bmcfee/pyrubberband)), both offline and real-time modes are available.
 
 Currently this extenstion exposes only a single class: `RubberBandStretcher`, which implements all the functionalities of the underlying C++ class. The interface is nearly identical to the original library, with a few changes to make it a bit more Pythonic by:
 - using `snake_case` for functions, variables and properties, and `SNAKE_CASE` for constants
 - not using (magic) numbers to represent the state
   - use `is_done()` to see if all the data has been processed and returned from the stretcher, instead of `available() == -1`
   - use `stretcher.formant_scale = pylibrb.AUTO_FORMANT_SCALE` instead of `stretcher.formant_scale = 0`
-- not using `final` argument in `process()`
-  - use `flush()` to finish processing and get the remaining samples
 
 Throughout the library, audio is accepted and returned in the form of [NumPy](https://github.com/numpy/numpy) ndarrays.
 
 ## Example
 
 ```python
 from pylibrb import RubberBandStretcher, Option, create_audio_array
```

### Comparing `pylibrb-0.0.7/README.md` & `pylibrb-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # pylibrb
 [![tests](https://github.com/pawel-glomski/pylibrb/actions/workflows/test.yml/badge.svg)](https://github.com/pawel-glomski/pylibrb/actions/workflows/test.yml)
+[![PyPI version](https://img.shields.io/pypi/v/pylibrb)](https://pypi.org/project/pylibrb/)
 
 pylibrb (py-lib-rubberband) is a simple Python extension exposing [Rubber Band Library](https://breakfastquay.com/rubberband/) using [nanobind](https://github.com/wjakob/nanobind) bindings.
 
-Since this is not a wrapper around a command-line app (like [pyrubberband](https://github.com/bmcfee/pyrubberband)), both offline and real-time modes are available.
+Since this is not a wrapper around a command-line tool (like [pyrubberband](https://github.com/bmcfee/pyrubberband)), both offline and real-time modes are available.
 
 Currently this extenstion exposes only a single class: `RubberBandStretcher`, which implements all the functionalities of the underlying C++ class. The interface is nearly identical to the original library, with a few changes to make it a bit more Pythonic by:
 - using `snake_case` for functions, variables and properties, and `SNAKE_CASE` for constants
 - not using (magic) numbers to represent the state
   - use `is_done()` to see if all the data has been processed and returned from the stretcher, instead of `available() == -1`
   - use `stretcher.formant_scale = pylibrb.AUTO_FORMANT_SCALE` instead of `stretcher.formant_scale = 0`
-- not using `final` argument in `process()`
-  - use `flush()` to finish processing and get the remaining samples
 
 Throughout the library, audio is accepted and returned in the form of [NumPy](https://github.com/numpy/numpy) ndarrays.
 
 ## Example
 
 ```python
 from pylibrb import RubberBandStretcher, Option, create_audio_array
@@ -34,8 +33,8 @@
   stretcher.process(audio_in)
 
 # retrieve the available samples
 audio_out = stretcher.retrieve(stretcher.available())
 
 ```
 
-For more instructions, read the docstings of the `RubberBandStretcher` class and the `Option` enum, or see the [documentation of Rubber Band Library](https://breakfastquay.com/rubberband/documentation.html).
+For more instructions, read the docstings of the `RubberBandStretcher` class and the `Option` enum, or see the [documentation of Rubber Band Library](https://breakfastquay.com/rubberband/documentation.html).
```

### Comparing `pylibrb-0.0.7/setup.cfg` & `pylibrb-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.7/setup.py` & `pylibrb-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.7/src/pylibrb/pylibrb_ext.pyi` & `pylibrb-0.0.8/src/pylibrb/pylibrb_ext.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
   Offline mode:
     In offline mode, you must provide the audio block-by-block in two passes. In the first pass,
     call `study()` on each block; in the second pass, call `process()` on each block and
     receive the output via `retrieve()`.
 
     In offline mode, the time and pitch ratios are fixed as soon as the study pass has begun and
     cannot be changed afterwards. (But see `set_keyframe_map()` for a way to do pre-planned
-    variable time stretching in offline mode.) Offline mode also performs padding and delay
+    variable time stretching in offline mode). Offline mode also performs padding and delay
     compensation so that the stretched result has an exact start and duration.
   
   Real-time mode:
     In real-time mode, there is no study pass, just a single streaming pass in which the audio is
     passed to `process()` and output received via `retrieve()`.
   
     In real-time mode you can change the time and pitch ratios at any time. You may need to perform
@@ -268,15 +268,15 @@
   error states and extremely rapid changes between extreme ratios, as well as the case in which more
   frames are passed to `process()` than the values returned by `get_samples_required()` or set using
   `set_max_process_size()`, when buffer reallocation may occur. Note that offline mode is never
   RT-safe.
   
   Thread safety:
     Multiple instances of `RubberBandStretcher` may be created and used in separate threads
-    concurrently However, for any single instance of `RubberBandStretcher`, you may not call
+    concurrently. However, for any single instance of `RubberBandStretcher`, you may not call
     `process()` more than once concurrently, and you may not change the time or pitch ratio while a
     `process()` call is being executed (if the stretcher was created in real-time mode; in offline
     mode you can't change the ratios during use anyway). So you can run `process()` in its own
     thread if you like, but if you want to change ratios dynamically from a different thread, you
     will need some form of mutex in your code. Changing the time or pitch ratio is real-time safe
     except in extreme circumstances, so for most applications that may change these dynamically it
     probably makes most sense to do so from the same thread as calls `process()`, even if that is a
@@ -403,28 +403,28 @@
     '''
 
   @time_ratio.setter
   def time_ratio(self, ratio: float) -> float:
     ...
 
   def calculate_stretch(self) -> None:
-    '''Force the stretcher to calculate a stretch profile Normally this happens automatically for
+    '''Force the stretcher to calculate a stretch profile. Normally this happens automatically for
     the first `process()` call in offline mode.
 
     This function is provided for diagnostic purposes only and is supported only with the R2 engine.
     '''
 
   def available(self) -> int:
     '''Ask the stretcher how many audio samples of output data are available for reading via
     `retrieve()`.
 
     Returns:
       The number of available samples or 0 if no samples are available - this usually means more
       input data needs to be provided, but if the stretcher is running in threaded mode it may just
-      mean that not enough data has yet been processed Call `get_samples_required()` to discover
+      mean that not enough data has yet been processed. Call `get_samples_required()` to discover
       whether more input is needed.
     '''
 
   def get_exact_time_points(self) -> list[float]:
     '''This function is provided for diagnostic purposes only and is supported only with the R2
     engine.
 
@@ -544,23 +544,25 @@
     '''Checks whether the stretcher has already processed all the provided data and the resulting
     audio has been retrieved.
     
     Returns:
       `True` if the "final" block has been processed and already retrieved, `False` otherwise.
     '''
 
-  def process(self, audio: np.ndarray) -> None:
+  def process(self, audio: np.ndarray, final: bool = False) -> None:
     '''Provide a block of samples for processing.
     
     See also `get_samples_required()` and `set_max_process_size()`.
     
     Args:
       audio:
         De-interleaved audio data with one float array per channel. Sample values are conventionally
         expected to be in the range -1.0f to +1.0f
+      final:
+        Is this the last audio block to process.
     '''
 
   def reset(self) -> None:
     '''Reset the stretcher's internal buffers.
 
     The stretcher should subsequently behave as if it had just been constructed (although retaining
     the current time and pitch ratio).
@@ -585,22 +587,14 @@
   def retrieve_available(self) -> np.ndarray:
     '''Obtains the currently available output from the stretcher.
     
     Returns:
       An array the currently available samples (returns an empty array when nothing is available).
     '''
 
-  def flush(self) -> np.ndarray:
-    '''Flushes the stretcher and returns the remaining samples. Stretcher resets on this operation
-    (as if `reset()` was called).
-
-    Returns:
-      An array with the remaining samples. Returns an empty array when nothing is available.
-    '''
-
   def set_detector_options(self, options: int) -> None:
     '''Change an `Option.DETECTOR` configuration setting.
     
     This may be called at any time in RealTime mode.
     
     It may not be called in Offline mode (for which the detector option is fixed on construction).
     
@@ -705,28 +699,28 @@
 
     If you don't call this, the stretcher will assume that you are calling `get_samples_required()`
     at each cycle and are never passing more samples than are suggested by that function.
 
     If your application has some external constraint that means you prefer a fixed block size, then
     your normal mode of operation would be to provide that block size to this function; to loop
     calling `process()` with that size of block; after each call to `process()`, test whether output
-    has been generated by calling `available()`; and, if so, call `retrieve()` to obtain it See
+    has been generated by calling `available()`; and, if so, call `retrieve()` to obtain it. See
     `get_samples_required()` for a more suitable operating mode for applications without such
     external constraints.
 
     This function may not be called after the first call to `study()` or `process()`.
 
     Note that this value is only relevant to `process()`, not to `study()`.
 
     Args:
       samples: The maximum number of samples that will be ever passed in a single `process()` call.
     '''
 
   def set_phase_options(self, options: int) -> None:
-    '''Change an `Option.PHASE` configuration setting This may be called at any time in any mode.
+    '''Change an `Option.PHASE` configuration setting. This may be called at any time in any mode.
     
     This has no effect when using the R3 engine.
 
     Note that if running multi-threaded in Offline mode, the change may not take effect immediately
     if processing is already under way when this function is called.
 
     Args:
```

### Comparing `pylibrb-0.0.7/src/pylibrb.egg-info/PKG-INFO` & `pylibrb-0.0.8/src/pylibrb.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pylibrb
 [![tests](https://github.com/pawel-glomski/pylibrb/actions/workflows/test.yml/badge.svg)](https://github.com/pawel-glomski/pylibrb/actions/workflows/test.yml)
+[![PyPI version](https://img.shields.io/pypi/v/pylibrb)](https://pypi.org/project/pylibrb/)
 
 pylibrb (py-lib-rubberband) is a simple Python extension exposing [Rubber Band Library](https://breakfastquay.com/rubberband/) using [nanobind](https://github.com/wjakob/nanobind) bindings.
 
-Since this is not a wrapper around a command-line app (like [pyrubberband](https://github.com/bmcfee/pyrubberband)), both offline and real-time modes are available.
+Since this is not a wrapper around a command-line tool (like [pyrubberband](https://github.com/bmcfee/pyrubberband)), both offline and real-time modes are available.
 
 Currently this extenstion exposes only a single class: `RubberBandStretcher`, which implements all the functionalities of the underlying C++ class. The interface is nearly identical to the original library, with a few changes to make it a bit more Pythonic by:
 - using `snake_case` for functions, variables and properties, and `SNAKE_CASE` for constants
 - not using (magic) numbers to represent the state
   - use `is_done()` to see if all the data has been processed and returned from the stretcher, instead of `available() == -1`
   - use `stretcher.formant_scale = pylibrb.AUTO_FORMANT_SCALE` instead of `stretcher.formant_scale = 0`
-- not using `final` argument in `process()`
-  - use `flush()` to finish processing and get the remaining samples
 
 Throughout the library, audio is accepted and returned in the form of [NumPy](https://github.com/numpy/numpy) ndarrays.
 
 ## Example
 
 ```python
 from pylibrb import RubberBandStretcher, Option, create_audio_array
```

### Comparing `pylibrb-0.0.7/tests/test_stretcher.py` & `pylibrb-0.0.8/tests/test_stretcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                                     initial_pitch_scale=0.5)
 
     assert stretcher.channels == pylibrb.MAX_CHANNELS_NUM
     assert stretcher.engine_version == 3
     assert stretcher.time_ratio == 0.5
     assert stretcher.pitch_scale == 0.5
     assert stretcher.available() == 0
-    assert stretcher.is_done() == False
+    assert stretcher.is_done() is False
 
 
 class TestRealtimeStretcher:
 
   def test_process_should_raise_value_error_when_incorrect_audio_layout(
       self, realtime_stretcher: RubberBandStretcher):
     stretcher = realtime_stretcher
@@ -161,22 +161,21 @@
     stretcher.time_ratio = 1.0
     for _ in range(iters):
       stretcher.process(audio_data)
       expected_samples += audio_samples * stretcher.time_ratio
       observed_samples += stretcher.retrieve(stretcher.available()).shape[pylibrb.SAMPLES_AXIS]
 
     stretcher.time_ratio = time_ratio
-    for _ in range(iters):
-      stretcher.process(audio_data)
+    for i in range(iters):
+      stretcher.process(audio_data, final=(i + 1) == iters)
       expected_samples += audio_samples * stretcher.time_ratio
       observed_samples += stretcher.retrieve(stretcher.available()).shape[pylibrb.SAMPLES_AXIS]
 
-    observed_samples += stretcher.flush().shape[pylibrb.SAMPLES_AXIS]
-
     relative_error = abs(expected_samples - observed_samples) / expected_samples
+    assert stretcher.is_done()
     assert relative_error <= 0.05
 
   def test_retrieve_available_should_return_available_samples(
       self, realtime_stretcher: RubberBandStretcher):
     stretcher = realtime_stretcher
     audio_data = pylibrb.create_audio_array(stretcher.channels, stretcher.get_samples_required())
 
@@ -187,49 +186,7 @@
     result = stretcher.retrieve_available()
 
     assert result.shape[pylibrb.SAMPLES_AXIS] == available_samples
     assert result.shape[pylibrb.CHANNELS_AXIS] == stretcher.channels
 
     # since we just took all the available audio, there shouldn't be any left
     assert stretcher.retrieve_available().size == 0
-
-  def test_flush_should_return_empty_array_when_stretcher_is_empty(
-      self, realtime_stretcher: RubberBandStretcher):
-    stretcher = realtime_stretcher
-
-    flushed_audio = stretcher.flush()
-
-    assert flushed_audio.size == 0
-
-  def test_flush_should_return_empty_array_when_stretcher_is_already_flushed(
-      self, realtime_stretcher: RubberBandStretcher):
-    stretcher = realtime_stretcher
-    audio_data = pylibrb.create_audio_array(stretcher.channels, stretcher.get_samples_required())
-    stretcher.process(audio_data)
-
-    stretcher.flush()
-    flushed_audio = stretcher.flush()
-
-    assert flushed_audio.size == 0
-
-  def test_flush_should_return_something_when_stretcher_is_not_empty(
-      self, realtime_stretcher: RubberBandStretcher):
-    stretcher = realtime_stretcher
-    audio_data = pylibrb.create_audio_array(stretcher.channels,
-                                            int(1.5 * stretcher.get_samples_required()))
-    stretcher.process(audio_data)
-
-    flushed_audio = stretcher.flush()
-
-    assert flushed_audio.size > 0
-
-  def test_flush_should_return_something_when_stretcher_is_not_empty_and_retrieve_was_called_before(
-      self, realtime_stretcher: RubberBandStretcher):
-    stretcher = realtime_stretcher
-    audio_data = pylibrb.create_audio_array(stretcher.channels,
-                                            int(1.5 * stretcher.get_samples_required()))
-    stretcher.process(audio_data)
-    stretcher.retrieve_available()
-
-    flushed_audio = stretcher.flush()
-
-    assert flushed_audio.size > 0
```

### Comparing `pylibrb-0.0.7/tests/test_utils.py` & `pylibrb-0.0.8/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 import numpy as np
 
 import pylibrb
 from pylibrb import create_audio_array, reorder_to_rb, reorder_from_rb
 
 
 def test_create_audio_array_should_create_array_with_correct_shape():
@@ -13,39 +15,80 @@
 
 def test_create_audio_array_should_create_array_with_correct_value():
   audio = create_audio_array(2, 128, 321)
 
   assert np.all(audio == 321)
 
 
+def test_reorder_to_rb_should_raise_index_error_when_bad_samples_axis():
+  audio = create_audio_array(2, 128)
+
+  with pytest.raises(IndexError):
+    reorder_to_rb(audio, samples_axis=2)
+
+
 def test_reorder_to_rb_should_do_nothing_when_audio_with_correct_layout():
   audio = create_audio_array(2, 128)
 
-  audio_reordered = reorder_to_rb(audio, channels_axis=pylibrb.CHANNELS_AXIS)
+  audio_reordered = reorder_to_rb(audio, samples_axis=pylibrb.SAMPLES_AXIS)
 
   assert audio_reordered.shape == audio.shape
 
 
 def test_reorder_to_rb_should_reorder_audio_array_when_audio_with_wrong_layout():
   audio = create_audio_array(2, 128)
 
-  # pass transposed audio array and thus also transposed channels axis (i.e. samples axis)
-  audio_reordered = reorder_to_rb(audio.T, channels_axis=pylibrb.SAMPLES_AXIS)
+  # pass transposed audio array and thus also transposed samples axis (i.e. channels axis)
+  audio_reordered = reorder_to_rb(audio.T, samples_axis=pylibrb.CHANNELS_AXIS)
 
   assert audio_reordered.shape == audio.shape
 
 
+def test_reorder_to_rb_should_reorder_audio_array_when_audio_with_wrong_complex_layout():
+  audio = create_audio_array(1, 2 * 4 * 8 * 4).reshape(2, 4, 8, 4)
+
+  audio_reordered = reorder_to_rb(audio, samples_axis=2)  # select 3rd axis of shape 8
+
+  expected_shape = [8, 8]
+  expected_shape[pylibrb.CHANNELS_AXIS] = 2 * 4 * 1 * 4
+  assert audio_reordered.shape == tuple(expected_shape)
+
+
+def test_reorder_from_rb_should_raise_value_error_when_missing_None_in_wanted_shape():
+  audio = create_audio_array(2, 128)
+
+  with pytest.raises(ValueError):
+    reorder_from_rb(audio, wanted_shape=(2, 128))
+
+
 def test_reorder_from_rb_should_do_nothing_when_audio_with_correct_layout():
   rb_audio = create_audio_array(2, 128)
 
-  audio_reordered = reorder_from_rb(rb_audio, wanted_channels_axis=pylibrb.CHANNELS_AXIS)
+  wanted_shape = [-1, -1]
+  wanted_shape[pylibrb.SAMPLES_AXIS] = None
+  audio_reordered = reorder_from_rb(rb_audio, wanted_shape=wanted_shape)
 
   assert audio_reordered.shape == rb_audio.shape
 
 
 def test_reorder_from_rb_should_reorder_audio_array_when_audio_with_wrong_layout():
   rb_audio = create_audio_array(2, 128)
 
   # pass samples axis as channels axis
-  audio_reordered = reorder_from_rb(rb_audio, wanted_channels_axis=pylibrb.SAMPLES_AXIS)
+  wanted_shape = [2, 2]
+  wanted_shape[pylibrb.CHANNELS_AXIS] = None
+  audio_reordered = reorder_from_rb(rb_audio, wanted_shape=wanted_shape)
 
   assert audio_reordered.shape == rb_audio.T.shape
+
+
+def test_reorder_from_rb_should_reorder_audio_array_when_audio_with_wrong_complex_layout():
+  audio = create_audio_array(24, 128).reshape(1, 2, 128, 3, 4)
+  audio[0, 0, :, 0, 0] = np.arange(128)
+  audio[-1, -1, :, -1, -1] = np.arange(128, 2 * 128)
+
+  rb_audio = reorder_to_rb(audio, samples_axis=2)
+  audio_reordered = reorder_from_rb(rb_audio, wanted_shape=[1, 2, None, 3, 4])
+
+  assert audio_reordered.shape == audio.shape
+  assert np.array_equal(audio[0, 0, :, 0, 0], np.arange(128))
+  assert np.array_equal(audio[-1, -1, :, -1, -1], np.arange(128, 2 * 128))
```

