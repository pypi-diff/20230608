# Comparing `tmp/s3dlib-1.0.0.tar.gz` & `tmp/s3dlib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\s3dlib-1.0.0.tar", last modified: Thu Jul 30 19:52:46 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `s3dlib-1.0.0.tar` & `s3dlib-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,8 @@
-drwxrwxrwx   0        0        0        0 2020-07-30 19:52:46.000000 s3dlib-1.0.0/
--rw-rw-rw-   0        0        0     1952 2020-07-30 19:52:46.000000 s3dlib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      986 2020-07-30 19:28:21.000000 s3dlib-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2020-07-30 19:52:46.000000 s3dlib-1.0.0/s3dlib/
--rw-rw-rw-   0        0        0       21 2020-06-25 01:12:07.000000 s3dlib-1.0.0/s3dlib/__init__.py
--rw-rw-rw-   0        0        0    14197 2020-07-29 03:14:37.000000 s3dlib-1.0.0/s3dlib/cmap_utilities.py
--rw-rw-rw-   0        0        0   119873 2020-07-27 19:05:13.000000 s3dlib-1.0.0/s3dlib/surface.py
-drwxrwxrwx   0        0        0        0 2020-07-30 19:52:46.000000 s3dlib-1.0.0/s3dlib.egg-info/
--rw-rw-rw-   0        0        0     1952 2020-07-30 19:52:45.000000 s3dlib-1.0.0/s3dlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2020-07-30 19:52:46.000000 s3dlib-1.0.0/s3dlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-30 19:52:45.000000 s3dlib-1.0.0/s3dlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2020-07-30 19:52:45.000000 s3dlib-1.0.0/s3dlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-07-30 19:52:46.000000 s3dlib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      957 2020-07-30 19:43:43.000000 s3dlib-1.0.0/setup.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 s3dlib-1.1.0/src/s3dlib/__init__.py
+-rw-r--r--   0        0        0    29077 2020-02-02 00:00:00.000000 s3dlib-1.1.0/src/s3dlib/cmap_utilities.py
+-rw-r--r--   0        0        0    15498 2020-02-02 00:00:00.000000 s3dlib-1.1.0/src/s3dlib/cmap_xtra.py
+-rw-r--r--   0        0        0   331538 2020-02-02 00:00:00.000000 s3dlib-1.1.0/src/s3dlib/surface.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 s3dlib-1.1.0/LICENSE
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 s3dlib-1.1.0/README.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 s3dlib-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 s3dlib-1.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `s3dlib-1.0.0/README.md` & `s3dlib-1.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 
 # S3Dlib
 
-### Python classes to create 3D surface objects rendered in *Matplotlib*
+### Python classes to create 3D surface and line objects rendered in *Matplotlib*
 
 
 Detailed documentation and examples are provided at [s3dlib.org](https://s3dlib.org)
 
 ---
-
-A 3D surface object is a collection of faces with vertices ordered using
-the 'right hand rule' to designate the 'outer' surface normals.  All surface faces
-are joined with a minimum of one adjacent face. Adjacent faces share two
-common vertices.
-
-The surface object geomentry and color are controlled through various
-object methods in the 'Surface3DCollection' base class.
-Surface instantiation is performed using the four subclasses that
-have predefined surface topologies in native coordinates.
-Base class objects may be created by addition of subclass objects to
-form a single 'composite' surface.
-
-Objects are added to the mpl_toolkits.mplot3d.Art3d using
-the Axis3d.add_collection3d() method.
+S3Dlib simplifies the construction of 3D objects using predefined geometries in planar, polar, cylindrical, and spherical coordinates.
+Using these geometries remove the development effort of constructing a network of vertex coordinates.
+The object geometry and color are then controlled through various object methods. 
+Objects are finally added to the mpl_toolkits.mplot3d.axes3d.Axes3d using
+the Axes3d.add_collection3d() method.
 
 Included is a module containing functions to create custom Matplotlib color maps.
```

