# Comparing `tmp/streamlitopencvplayer-1.2.2.tar.gz` & `tmp/streamlitopencvplayer-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.2.tar", last modified: Thu Jun  8 10:41:18 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.3.tar", last modified: Thu Jun  8 10:44:22 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.2.tar` & `streamlitopencvplayer-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:18.031095 streamlitopencvplayer-1.2.2/
--rw-rw-rw-   0        0        0      419 2023-06-08 10:41:18.029090 streamlitopencvplayer-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 10:41:18.032093 streamlitopencvplayer-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-06-08 10:40:38.000000 streamlitopencvplayer-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:17.974718 streamlitopencvplayer-1.2.2/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.2/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     7441 2023-06-08 10:37:25.000000 streamlitopencvplayer-1.2.2/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:18.007094 streamlitopencvplayer-1.2.2/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-08 10:41:17.000000 streamlitopencvplayer-1.2.2/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-08 10:41:17.000000 streamlitopencvplayer-1.2.2/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 10:41:17.000000 streamlitopencvplayer-1.2.2/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-08 10:41:17.000000 streamlitopencvplayer-1.2.2/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:18.021091 streamlitopencvplayer-1.2.2/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.2/test/__init__.py
--rw-rw-rw-   0        0        0      820 2023-05-30 21:53:29.000000 streamlitopencvplayer-1.2.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:44:22.599085 streamlitopencvplayer-1.2.3/
+-rw-rw-rw-   0        0        0      419 2023-06-08 10:44:22.596053 streamlitopencvplayer-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:44:22.600292 streamlitopencvplayer-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-06-08 10:43:55.000000 streamlitopencvplayer-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:44:22.561033 streamlitopencvplayer-1.2.3/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.3/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     7356 2023-06-08 10:44:16.000000 streamlitopencvplayer-1.2.3/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:44:22.582032 streamlitopencvplayer-1.2.3/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-08 10:44:22.000000 streamlitopencvplayer-1.2.3/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-06-08 10:44:22.000000 streamlitopencvplayer-1.2.3/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:44:22.000000 streamlitopencvplayer-1.2.3/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-08 10:44:22.000000 streamlitopencvplayer-1.2.3/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 10:44:22.591031 streamlitopencvplayer-1.2.3/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.3/test/__init__.py
+-rw-rw-rw-   0        0        0      820 2023-05-30 21:53:29.000000 streamlitopencvplayer-1.2.3/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.2/README.md` & `streamlitopencvplayer-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.2/setup.py` & `streamlitopencvplayer-1.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.2' 
+VERSION = '1.2.3' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.2/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.2.3/streamlitopencvplayer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
                 st.session_state['frames'].append(frames)
             else:
                 break
         cap.release()
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
-        if 'myslider' in st.session_state:
-            del st.session_state.myslider
+        #if 'myslider' in st.session_state:
+            
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
 
     while st.session_state['counter'] < len(st.session_state['frames']):
         if not resume:
             if i < len(data):
                 if st.session_state['counter'] == int(alerts[i]*fps):
@@ -133,15 +133,15 @@
             st.session_state['counter'] += 1
             # update slider value
 
             frame_num = widget.slider("", min_value=0, max_value=int(
                 cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
             if 'myslider' in st.session_state:
                 if st.session_state.myslider > frame_num:
-                    del st.session_state.myslider
+                    
                     #st.session_state.clear()
                     st.session_state['counter'] = frame_num
                     #st.session_state['counter'] = 0
                     resume = True
                     #st.experimental_rerun() #remove cache
                 
 
@@ -157,16 +157,16 @@
                 break
             if replay:
                 st.session_state['counter'] = 0
                 st.session_state['frames'] = []
                 # back to the first frame if the video is finished
             if st.session_state['counter'] == len(st.session_state['frames']):
                 st.session_state['counter'] = 0
-                if 'myslider'  in st.session_state:
-                    del st.session_state.myslider
+                #if 'myslider'  in st.session_state:
+                    
             st.session_state['counter'] = frame_num
 
     if resume:
         container_2.empty()
         pause = container_2.button('▶')
         resume = False
```

### Comparing `streamlitopencvplayer-1.2.2/test/test.py` & `streamlitopencvplayer-1.2.3/test/test.py`

 * *Files identical despite different names*

