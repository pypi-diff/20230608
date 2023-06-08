# Comparing `tmp/keypoint-moseq-0.1.4.tar.gz` & `tmp/keypoint-moseq-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.1.4.tar", last modified: Mon Jun  5 19:18:44 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.1.5.tar", last modified: Thu Jun  8 14:24:39 2023, max compression
```

## Comparing `keypoint-moseq-0.1.4.tar` & `keypoint-moseq-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-05 19:18:44.252938 keypoint-moseq-0.1.4/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.4/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.4/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-05 19:18:44.253141 keypoint-moseq-0.1.4/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.4/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-05 19:18:44.254788 keypoint-moseq-0.1.4/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-06-05 19:18:44.254916 keypoint-moseq-0.1.4/keypoint_moseq/_version.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17701 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17249 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    46339 2023-06-05 19:18:09.000000 keypoint-moseq-0.1.4/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    27260 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    68264 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-05 19:18:44.252365 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-06-05 19:18:44.000000 keypoint-moseq-0.1.4/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-06-05 19:18:44.254352 keypoint-moseq-0.1.4/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-06-05 18:56:39.000000 keypoint-moseq-0.1.4/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.4/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-08 14:24:39.510188 keypoint-moseq-0.1.5/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.5/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.5/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-08 14:24:39.510313 keypoint-moseq-0.1.5/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-16 23:54:35.000000 keypoint-moseq-0.1.5/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-08 14:24:39.511103 keypoint-moseq-0.1.5/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-06-08 14:24:39.511192 keypoint-moseq-0.1.5/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17701 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17249 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    46577 2023-06-08 14:18:49.000000 keypoint-moseq-0.1.5/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    27260 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    68266 2023-06-08 13:46:30.000000 keypoint-moseq-0.1.5/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-06-08 14:24:39.509860 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-06-08 14:24:39.000000 keypoint-moseq-0.1.5/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-06-08 14:24:39.510854 keypoint-moseq-0.1.5/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-06-06 15:33:16.000000 keypoint-moseq-0.1.5/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.5/versioneer.py
```

### Comparing `keypoint-moseq-0.1.4/LICENSE.md` & `keypoint-moseq-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/NOTICE.md` & `keypoint-moseq-0.1.5/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/README.md` & `keypoint-moseq-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/keypoint_moseq/__init__.py` & `keypoint-moseq-0.1.5/keypoint_moseq/__init__.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/keypoint_moseq/analysis.py` & `keypoint-moseq-0.1.5/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/keypoint_moseq/calibration.py` & `keypoint-moseq-0.1.5/keypoint_moseq/calibration.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/keypoint_moseq/fitting.py` & `keypoint-moseq-0.1.5/keypoint_moseq/fitting.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/keypoint_moseq/io.py` & `keypoint-moseq-0.1.5/keypoint_moseq/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -884,16 +884,16 @@
         'two_mice_track1'`.   
 
     - anipose
         .csv files generated by anipose. Each file should contain five columns
         per keypoint (x,y,z,error,score), plus a last column with the frame number.
         The `score` column is used as the keypoint confidence. 
 
-    - anipose-sleap
-        .h5/.hdf5 files generated by anipose-sleap. Each file should contain 
+    - sleap-anipose
+        .h5/.hdf5 files generated by sleap-anipose. Each file should contain 
         a dataset called `'tracks'` with shape (n_frames, 1, n_keypoints, 3).
         If there is also a `'point_scores'` dataset, it will be used as the
         keypoint confidence. Otherwise, the confidence will be set to 1.
 
     Parameters
     ----------
     filepath_pattern: str or list of str
@@ -903,15 +903,15 @@
         - single file (e.g. `/path/to/file.csv`) 
         - single directory (e.g. `/path/to/dir/`)
         - set of files (e.g. `/path/to/fileprefix*`)
         - set of directories (e.g. `/path/to/dirprefix*`)
 
     format: str
         Format of the files to load. Must be one of `'deeplabcut'`, 
-        `'sleap'`, `'anipose'`, or `'anipose-sleap'`.
+        `'sleap'`, `'anipose'`, or `'sleap-anipose'`.
 
     recursive: bool, default=True
         Whether to search recursively for deeplabcut csv or hdf5 files.
 
     path_in_name: bool, default=False
         Whether to name the tracking results from each file by the path
         to the file (True) or just the filename (False). If True, the
@@ -938,30 +938,30 @@
         Dictionary mapping filenames to `likelihood` scores as ndarrays
         of shape (n_frames, n_bodyparts)
 
     bodyparts: list of str
         List of bodypart names. The order of the names matches the order
         of the bodyparts in `coordinates` and `confidences`.
     """
-    formats = ['deeplabcut', 'sleap', 'anipose', 'anipose-sleap']
+    formats = ['deeplabcut', 'sleap', 'anipose', 'sleap-anipose']
     assert format in formats, fill(
         f'Unrecognized format {format}. Must be one of {formats}')
     
     extensions = {
         'deeplabcut': ['.csv','.h5','.hdf5'],
         'sleap': ['.h5','.hdf5'],
         'anipose': ['.csv'],
-        'anipose-sleap': ['.h5','.hdf5']
+        'sleap-anipose': ['.h5','.hdf5']
     }[format]
 
     loader = {
         'deeplabcut': _deeplabcut_loader,
         'sleap': _sleap_loader,
         'anipose': _anipose_loader,
-        'anipose-sleap': _anipose_sleap_loader
+        'sleap-anipose': _sleap_anipose_loader
     }[format]
 
     filepaths = list_files_with_exts(
         filepath_pattern, extensions, recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No files with extensions {extensions} found for {filepath_pattern}')
     
@@ -1023,25 +1023,29 @@
     bodyparts = [n.split('_x')[0] for n in df.columns[:-1][::5]] 
     arr = df.to_numpy()[:,:-1].reshape(len(df), len(bodyparts), 5)
     coordinates = {name: arr[:,:,:3]}
     confidences = {name: arr[:,:,4]}
     return coordinates,confidences,bodyparts
 
 
-def _anipose_sleap_loader(filepath, name):
-    """Load keypoints from anipose-sleap hdf5 files."""
+def _sleap_anipose_loader(filepath, name):
+    """Load keypoints from sleap-anipose hdf5 files."""
     with h5py.File(filepath, 'r') as f:
         coords = f['tracks'][()]
         if 'point_scores' in f.keys():
             confs = f['point_scores'][()]
         else:
             confs = np.ones_like(coords[...,0])
         bodyparts = ['bodypart{}'.format(i) for i in range(coords.shape[2])]
-        coordinates = {name: coords[0].T}
-        confidences = {name: confs[0].T}
+        if coords.shape[1] == 1:
+            coordinates = {name: coords[:,0]}
+            confidences = {name: confs[:,0]}
+        else:
+            coordinates = {f'{name}_track{i}': coords[:,i] for i in range(coords.shape[1])}
+            confidences = {f'{name}_track{i}': confs[:,i] for i in range(coords.shape[1])}
     return coordinates,confidences,bodyparts
 
 
 
 def load_deeplabcut_results(filepath_pattern, recursive=True, path_sep='-',
                             path_in_name=False, remove_extension=True):
     """
```

### Comparing `keypoint-moseq-0.1.4/keypoint_moseq/util.py` & `keypoint-moseq-0.1.5/keypoint_moseq/util.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/keypoint_moseq/viz.py` & `keypoint-moseq-0.1.5/keypoint_moseq/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1105,15 +1105,15 @@
 
 
 def generate_trajectory_plots(
     coordinates=None, results=None, output_dir=None, name=None, 
     project_dir=None, results_path=None, pre=5, post=15, 
     min_frequency=0.005, min_duration=3, use_reindexed=True, 
     use_estimated_coords=False, skeleton=[], bodyparts=None, 
-    use_bodyparts=None, num_samples=40, keypoint_colormap='autumn',
+    use_bodyparts=None, num_samples=50, keypoint_colormap='autumn',
     plot_options={}, sampling_options={'mode':'density'},
     padding={'left':0.1, 'right':0.1, 'top':0.2, 'bottom':0.2},
     save_individually=True, save_gifs=True, save_mp4s=False, fps=30, 
     projection_planes=['xy','xz'], **kwargs):
     """
     Generate trajectory plots for a modeled dataset.
 
@@ -1198,15 +1198,15 @@
         Ordered list of bodyparts to include in trajectory plot.
         If None, all bodyparts will be included.
 
     skeleton : list, default=[]
         List of edges that define the skeleton, where each edge is a
         pair of bodypart names or a pair of indexes.
 
-    num_samples: int, default=40
+    num_samples: int, default=50
         Number of samples to used to compute the average trajectory.
         Also used to set `n_neighbors` when sampling syllable instances
         in `density` mode. 
 
     keypoint_colormap : str
         Name of a matplotlib colormap to use for coloring the keypoints.
 
@@ -1293,15 +1293,15 @@
                 'If skeleton edges are specified using bodypart names, '
                 '`use_bodyparts` must be specified')
             edges = get_edges(use_bodyparts, skeleton)
         else: edges = skeleton
 
     syllables = sorted(trajectories.keys())
     titles = [f'Syllable {syllable}' for syllable in syllables]
-    Xs = np.nanmean(np.array([trajectories[syllable] for syllable in syllables]),axis=1)  
+    Xs = np.nanmedian(np.array([trajectories[syllable] for syllable in syllables]),axis=1)  
     
     if Xs.shape[-1]==3:
         projection_planes = [''.join(sorted(plane.lower())) for plane in projection_planes]
         assert set(projection_planes) <= set(['xy','yz','xz']), fill(
             "`projection_planes` must be a subset of `['xy','yz','xz']`")
         all_Xs = [Xs[...,np.array({'xy':[0,1], 'yz':[1,2], 'xz':[0,2]}[plane])] for plane in projection_planes]
         suffixes = ['.'+plane for plane in projection_planes]
```

### Comparing `keypoint-moseq-0.1.4/setup.cfg` & `keypoint-moseq-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.4/versioneer.py` & `keypoint-moseq-0.1.5/versioneer.py`

 * *Files identical despite different names*

