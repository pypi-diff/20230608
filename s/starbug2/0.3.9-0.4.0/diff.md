# Comparing `tmp/starbug2-0.3.9.tar.gz` & `tmp/starbug2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.3.9.tar", last modified: Wed Apr 26 09:25:29 2023, max compression
+gzip compressed data, was "starbug2-0.4.0.tar", last modified: Thu Jun  8 13:00:33 2023, max compression
```

## Comparing `starbug2-0.3.9.tar` & `starbug2-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 09:25:08.000000 starbug2-0.3.9/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 09:25:08.000000 starbug2-0.3.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 09:25:08.000000 starbug2-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 09:25:29.438328 starbug2-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-26 09:25:08.000000 starbug2-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.434328 starbug2-0.3.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10896 2023-04-26 09:25:08.000000 starbug2-0.3.9/bin/starbug2
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-26 09:25:08.000000 starbug2-0.3.9/bin/starbug2-match
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.434328 starbug2-0.3.9/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-26 09:25:08.000000 starbug2-0.3.9/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 09:25:08.000000 starbug2-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 09:25:29.438328 starbug2-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-26 09:25:08.000000 starbug2-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.434328 starbug2-0.3.9/starbug2/
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/starbug2/param/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/param/default.param
--rw-r--r--   0 runner    (1001) docker     (123)    28226 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28295 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-26 09:25:08.000000 starbug2-0.3.9/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 09:25:29.000000 starbug2-0.3.9/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:25:29.438328 starbug2-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-26 09:25:08.000000 starbug2-0.3.9/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-26 09:25:08.000000 starbug2-0.3.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-08 13:00:18.000000 starbug2-0.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 13:00:18.000000 starbug2-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 13:00:18.000000 starbug2-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-08 13:00:33.490545 starbug2-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-08 13:00:18.000000 starbug2-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.486544 starbug2-0.4.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-08 13:00:18.000000 starbug2-0.4.0/bin/starbug2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4292 2023-06-08 13:00:18.000000 starbug2-0.4.0/bin/starbug2-match
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.486544 starbug2-0.4.0/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-08 13:00:18.000000 starbug2-0.4.0/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 13:00:18.000000 starbug2-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 13:00:33.490545 starbug2-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-08 13:00:18.000000 starbug2-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.486544 starbug2-0.4.0/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/starbug2/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/param/default.param
+-rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-06-08 13:00:18.000000 starbug2-0.4.0/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 13:00:33.000000 starbug2-0.4.0/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:00:33.490545 starbug2-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-08 13:00:18.000000 starbug2-0.4.0/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-08 13:00:18.000000 starbug2-0.4.0/tests/test_utils.py
```

### Comparing `starbug2-0.3.9/LICENSE.txt` & `starbug2-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.9/PKG-INFO` & `starbug2-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.3.9
+Version: 0.4.0
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
@@ -44,54 +44,52 @@
 ```
 
 Finally verify the installation by running `starbug2 --version`
 
 ## Usage
 
 ```bash
-
 Starbug II - JWST PSF photometry
-usage: starbug2 [-ABCDfhMPv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
+usage: starbug2 [-ABDfGhMPSv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
    -A  --apphot          : run aperture photometry on a source list
    -B  --background      : run background estimation
    -b  --bgdfile         : load background (-bgd.fits) file
-   -C  --clean           : run source cleaning before photometry 
    -d  --apfile  ap.fits : load a source detection (-ap.fits) file to skip the source detection step
    -D  --detect          : run source detection
    -f  --find            : attempt to find associated -ap -bgd files
    -G  --geom            : calculate geometric stats on source list
    -h  --help            : display uasage information
    -M  --match           : match outputs from all input image files
    -n  --ncores      num : number of CPU cores to split process between
    -o  --output      dir : output directory
    -p  --param   a.param : load parameter file
-   -P  --photom          : run psf photometry
+   -P  --psf             : run psf photometry
    -s  --set      option : set value in parameter file at runtime (-s SIGSKY=3)
    -S  --subbgd          : subtract background from image
    -v  --verbose         : display verbose outputs
 
    --> Single run commands
        --init                     : Initialise Starbug (post install)
        --local-param              : Make a local copy of the default parameter file
        --update-param             : Update an out-of-date local parameter file
        --generate-psf             : Generate ALL the PSF files to "STARBUG_DATDIR"
        --generate-region   a.fits : Make a ds9 region file with a detection file
        --generate-run      *.fits : Generate a simple run script
        --clean-table       a.fits : Clean up an individual table
        --version                  : Print starbug2 version
 
+       --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
+       --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
+
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
-
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
 * MIRI Background masking
-* findpeaks on convl method
-* rickerwavelet radius
 * psf dither match dropping apMag
```

### Comparing `starbug2-0.3.9/README.md` & `starbug2-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,54 +35,52 @@
 ```
 
 Finally verify the installation by running `starbug2 --version`
 
 ## Usage
 
 ```bash
-
 Starbug II - JWST PSF photometry
-usage: starbug2 [-ABCDfhMPv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
+usage: starbug2 [-ABDfGhMPSv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
    -A  --apphot          : run aperture photometry on a source list
    -B  --background      : run background estimation
    -b  --bgdfile         : load background (-bgd.fits) file
-   -C  --clean           : run source cleaning before photometry 
    -d  --apfile  ap.fits : load a source detection (-ap.fits) file to skip the source detection step
    -D  --detect          : run source detection
    -f  --find            : attempt to find associated -ap -bgd files
    -G  --geom            : calculate geometric stats on source list
    -h  --help            : display uasage information
    -M  --match           : match outputs from all input image files
    -n  --ncores      num : number of CPU cores to split process between
    -o  --output      dir : output directory
    -p  --param   a.param : load parameter file
-   -P  --photom          : run psf photometry
+   -P  --psf             : run psf photometry
    -s  --set      option : set value in parameter file at runtime (-s SIGSKY=3)
    -S  --subbgd          : subtract background from image
    -v  --verbose         : display verbose outputs
 
    --> Single run commands
        --init                     : Initialise Starbug (post install)
        --local-param              : Make a local copy of the default parameter file
        --update-param             : Update an out-of-date local parameter file
        --generate-psf             : Generate ALL the PSF files to "STARBUG_DATDIR"
        --generate-region   a.fits : Make a ds9 region file with a detection file
        --generate-run      *.fits : Generate a simple run script
        --clean-table       a.fits : Clean up an individual table
        --version                  : Print starbug2 version
 
+       --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
+       --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
+
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
-
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
 * MIRI Background masking
-* findpeaks on convl method
-* rickerwavelet radius
 * psf dither match dropping apMag
```

### Comparing `starbug2-0.3.9/bin/starbug2` & `starbug2-0.4.0/bin/starbug2`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 #!/usr/bin/python3 -Wignore
 """Starbug II - JWST PSF photometry
-usage: starbug2 [-ABCDfhMPv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
+usage: starbug2 [-ABDfGhMPSv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
    -A  --apphot          : run aperture photometry on a source list
    -B  --background      : run background estimation
    -b  --bgdfile         : load background (-bgd.fits) file
-   -C  --clean           : run source cleaning before photometry 
    -d  --apfile  ap.fits : load a source detection (-ap.fits) file to skip the source detection step
    -D  --detect          : run source detection
    -f  --find            : attempt to find associated -ap -bgd files
    -G  --geom            : calculate geometric stats on source list
    -h  --help            : display uasage information
    -M  --match           : match outputs from all input image files
    -n  --ncores      num : number of CPU cores to split process between
    -o  --output      dir : output directory
    -p  --param   a.param : load parameter file
-   -P  --photom          : run psf photometry
+   -P  --psf             : run psf photometry
    -s  --set      option : set value in parameter file at runtime (-s SIGSKY=3)
    -S  --subbgd          : subtract background from image
    -v  --verbose         : display verbose outputs
 
    --> Single run commands
        --init                     : Initialise Starbug (post install)
        --local-param              : Make a local copy of the default parameter file
        --update-param             : Update an out-of-date local parameter file
        --generate-psf             : Generate ALL the PSF files to "STARBUG_DATDIR"
        --generate-region   a.fits : Make a ds9 region file with a detection file
        --generate-run      *.fits : Generate a simple run script
        --clean-table       a.fits : Clean up an individual table
        --version                  : Print starbug2 version
 
+       --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
+       --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
+
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
 
 """
 import os,sys,getopt
-sys.stdout.write("loading..\r")
+#sys.stdout.write("loading..\r")
+sys.stdout.write("\x1b[1mlaunching \x1b[36mstarbug\x1b[0m\n")
 import pkg_resources
 from starbug2.utils import *
 from starbug2.misc import *
 
 VERBOSE= 0x01
 KILLPROC=0x02
 STOPPROC=0x04
@@ -57,112 +60,132 @@
 DOGEOM  =0x10000
 
 GENRATPSF =0x100000
 GENRATRUN =0x200000
 GENRATREG =0x400000
 INITSB    =0x800000
 UPDATEPRM =0x1000000
+DODEBUG   =0x2000000
+CALCINSTZP=0x4000000
+APPLYZP   =0x8000000
+
 
 options=0
 
 pfile=None
-setdict={}
+setopt={}
 output='.'
 ncores=1
-misc={}
 
 def usage():
-    if not (options&VERBOSE): quit(__doc__.split('\n')[1])
-    else: quit(__doc__)
+    if not (options&VERBOSE): perror(__doc__.split('\n')[1])
+    else: perror(__doc__)
+    quit(0)
 
-opts,args=getopt.getopt(sys.argv[1:],"ABCDfGhMPSvb:d:n:o:p:s:", ("apphot","background", "clean", "detect", "find", "geom", "help", "match", "photom", "subbgd", "verbose", "xtest",
+opts,args=getopt.getopt(sys.argv[1:],"ABDfGhMPSvb:d:n:o:p:s:", ("apphot","background", "detect", "find", "geom", "help", "match", "psf", "subbgd", "verbose", "xtest",
                                                       "bgdfile=", "apfile=", "ncores=", "output=", "param=", "set=",
-                                                      "init", "generate-psf", "local-param", "generate-region=", "clean-table", "version", "generate-run", "update-param"))
+                                                      "init", "generate-psf", "local-param", "generate-region=", "clean-table", "version", "generate-run", "update-param",
+                                                      "calc-instr-zp=", "apply-zeropoint=",
+                                                      "debug"))
 
 for opt,optarg in opts:
     if opt in ("-h","--help"):    usage()
     if opt in ("-p","--param"):   pfile= optarg
     if opt in ("-v","--verbose"):
         options|=VERBOSE
 
     if opt in ("-A","--apphot"): options |= DOAPPHOT
     if opt in ("-B","--background"): options|=DOBGDEST
-    if opt in ("-C","--clean"):  options |=DOCLEAN
+    #if opt in ("-C","--clean"):  options |=DOCLEAN
     if opt in ("-D","--detect"): options |= DODETECT
     if opt in ("-G","--geom"): options |= DOGEOM
     if opt in ("-M","--match"):  options |= DOMATCH
-    if opt in ("-P","--photom"): options |= DOPHOTOM
+    if opt in ("-P","--psf"): options |= DOPHOTOM
     if opt in ("-S","--subbgd"): options |= DOBGDSUB
 
     if opt in ("-d","--apfile"):
-        if os.path.exists(optarg): setdict["AP_FILE"]=optarg
-        else: perror("AP_FILE does not exist\n")
+        if os.path.exists(optarg): setopt["AP_FILE"]=optarg
+        else: perror("AP_FILE \"%s\" does not exist\n"%optarg)
 
     if opt in ("-b","--bgdfile"):
-        if os.path.exists(optarg): setdict["BGD_FILE"]=optarg
-        else: perror("BGD_FILE does not exist\n")
+        if os.path.exists(optarg): setopt["BGD_FILE"]=optarg
+        else: perror("BGD_FILE \"%s\" does not exist\n"%optarg)
 
     if opt in ("-f","--find"): options|=FINDFILE
     if opt in ("-n","--ncores"): ncores=int(optarg)
 
     if opt in ("-o","--output"):
-        if os.path.exists(optarg): 
-            output=optarg
-            setdict["OUTDIR"]=optarg
-        else:
-            perror("output directory '%s' does not exist\n"%optarg)
-            options|=KILLPROC
+        output=optarg
+        setopt["OUTPUT"]=optarg
 
     if opt in ("-s","--set"): 
         if '=' in optarg:
             key,val=optarg.split('=')
             try: val=float(val)
             except: pass
-            setdict[key]=val
+            setopt[key]=val
         else:
             perror("unable to set parameter, use syntax -s KEY=VALUE\n")
             options|=KILLPROC
 
     if opt=="--init": options|=(INITSB|STOPPROC)
     if opt=="--generate-psf": options|=(GENRATPSF|STOPPROC)
     if opt=="--update-param": options|=(UPDATEPRM|STOPPROC)
     if opt=="--generate-run": options|=(GENRATRUN|STOPPROC)
+    if opt=="--debug":
+        os.environ["SBIIDEBUG"]="/tmp/starbug.log"
+        #open("/tmp/starbug.log","w").close()
 
     if opt=="--local-param":
         os.system("cp %s/default.param starbug.param"%pkg_resources.resource_filename("starbug2","param/"))
         printf("--> generating starbug.param\n")
         options|=STOPPROC
 
     if opt=="--generate-region":
-        misc["REGION_TAB"]=optarg
+        setopt["REGION_TAB"]=optarg
         options|=(GENRATREG|STOPPROC)
 
     if opt=="--clean-table":
         printf("cleaning table <-- %s\n"%optarg)
         table=Table.read(optarg,format="fits")#load_table(optarg)
         options|=STOPPROC
 
-    if opt=="--version": quit(starbug2.logo%("starbug2-v%s"%pkg_resources.get_distribution("starbug2").version))
+    if opt=="--version": 
+        printf(starbug2.logo%("starbug2-v%s"%pkg_resources.get_distribution("starbug2").version))
+        options|=STOPPROC
+
+    if opt=="--calc-instr-zp":
+        setopt["ZP_PSF_CAT"]=optarg
+        options|=(CALCINSTZP|APPLYZP|STOPPROC)
+    if opt=="--apply-zeropoint":
+        setopt["ZP_PSF_CAT"]=optarg
+        options|=(APPLYZP|STOPPROC)
+
 
 
 ##############################################
 # Options set, verify/run one time functions #
 ##############################################
 
-if ncores>1: options&= ~VERBOSE
-
 ## Load parameter files
 if pfile==None:
     if os.path.exists("./starbug.param"):pfile="starbug.param"
     else:
-        perror("no local parameter file found, using default.param\n")
+        #perror("no local parameter file found, using default.param\n")
         pfile="%s/default.param"%pkg_resources.resource_filename("starbug2","param/")
 
 init_parameters=load_params(pfile)
-init_parameters.update(setdict)
+#for key in set(setopt.keys() & init_parameters.keys()):
+init_parameters.update(setopt)
+
+
+
+#########################
+# One time run commands #
+#########################
 
 if options&INITSB:
     init_starbug()
 
 if options&GENRATPSF:
     generate_psfs()
 
@@ -170,23 +193,59 @@
     cmd="starbug2 "#"+ " ".join( ["-vf"])
     generate_runscript(args, cmd)
 
 if options&UPDATEPRM:
     update_paramfile(pfile)
 
 if options&GENRATREG:
-    fname=misc.get("REGION_TAB")
+    fname=setopt.get("REGION_TAB")
     if fname and os.path.exists(fname):
         table=Table.read(fname,format="fits")
         _,name,_=split_fname(fname)
         export_region(table, colour=init_parameters["REGION_COL"], scale_radius=init_parameters["REGION_SCAL"],
                              region_radius=init_parameters["REGION_RAD"], xcol=init_parameters["REGION_XCOL"],
                              ycol=init_parameters["REGION_YCOL"], wcs=init_parameters["REGION_WCS"], fname="%s/%s.reg"%(output,name))
         printf("generating region --> %s/%s.reg\n"%(output,name))
 
+###########################
+# instrumental zero point #
+###########################
+if options&APPLYZP:
+    _fname=setopt.get("ZP_PSF_CAT")
+    _zp=setopt.get("ZEROPOINT")
+    _std=0
+    if _fname and os.path.exists(_fname):
+        psftable=Table.read(_fname, format="fits")
+        with fits.open(_fname) as fp: _header=fp[1].header ##thats a bit rubbish
+
+        if (fltr:=_header.get("FILTER")) is None:
+            if (fltr:=setopt.get("FILTER")) is None:
+                perror("Unable to determine table FILTER: set manually with `-s FILTER=F000W`\n")
+                quit(1) ## thats a bit hardcore
+
+        if options&CALCINSTZP:
+            _aptable=None
+            _apfname=setopt.get("AP_FILE")
+            if _apfname and os.path.exists(_apfname):
+                _aptable=Table.read(_apfname, format="fits")
+
+                if (res:=calc_instrumental_zeropint(psftable, _aptable, fltr=fltr)) is not None:
+                    _zp,_std=res
+
+        if _zp is not None:
+            psftable.meta["%s ZEROPOINT"%fltr]=_zp
+            psftable.meta["%s eZEROPOINT"%fltr]=_std
+            psftable[fltr]=psftable[fltr]+_zp
+
+            dname,fname,_=split_fname(_fname)
+            printf("--> %s/%s-zp.fits\n"%(dname,fname))
+            export_table( psftable, fname="%s/%s-zp.fits"%(dname,fname), header=_header)
+        else: perror("Unable to set ZEROPOINT, set it with -sZEROPOINT=000\n")
+    else: perror("Unable to locate table \"%s\".\n"%_fname)
+
 if options&STOPPROC: quit(0) ## quiet ending the process if required
 
 if len(args)==0: 
     perror("must include fits image file\n")
     options|=KILLPROC
 
 if options&KILLPROC:
@@ -202,86 +261,109 @@
 from starbug2.matching import dither_match
 from multiprocessing import Pool
 
 def fn(fname):
     sb=None
     if os.path.exists(fname):
         dname,bname,ext=split_fname(fname)
-        if ncores>1: puts(fname)
 
         if options&FINDFILE:
             ap="%s/%s-ap.fits"%(dname,bname)
             bgd="%s/%s-bgd.fits"%(dname,bname)
-            if os.path.exists(ap)  and not setdict.get("AP_FILE"):  setdict["AP_FILE"]=ap
-            if os.path.exists(bgd) and not setdict.get("BGD_FILE"): setdict["BGD_FILE"]=bgd
+            if os.path.exists(ap)  and not setopt.get("AP_FILE"):  setopt["AP_FILE"]=ap
+            if os.path.exists(bgd) and not setopt.get("BGD_FILE"): setopt["BGD_FILE"]=bgd
+
+        ## Sorting out the stdout
+        if options&VERBOSE:
+            setopt["VERBOSE"]=1
+            if ncores>1:
+                if fname==args[0]:
+                    printf("showing starbug stdout for \"%s\"\n"%fname)
+                else:
+                    setopt["VERBOSE"]=0
+                    puts("-> hiding \"%s\""%fname)
+        else:
+            puts(fname)
 
         if ext==".fits":
-            if options&VERBOSE: setdict["VERBOSE"]=1
-            sb=StarbugBase(fname, pfile=pfile, options=setdict)
-            
+            sb=StarbugBase(fname, pfile=pfile, options=setopt)
             if sb.verify(): return#quit("..quitting :(")
-            
+
             if options & DODETECT: sb.detect()
-            if options & DOCLEAN: sb.cleanup()
+            #if options & DOCLEAN: sb.cleanup()
             if options & DOBGDEST: sb.bgd_estimate()
             if options & DOBGDSUB: sb.bgd_subtraction()
             if options & DOGEOM: sb.source_geometry()
 
             if options & DOAPPHOT: sb.aperture_photometry()
-            if options & DOPHOTOM:
-                sb.photometry()
-                if options & DOCLEAN: sb.cleanup()
+            if options & DOPHOTOM: sb.photometry()
+            #if options & DOCLEAN: sb.cleanup()
+
             if options & DOARTIFL: sb.artificial_stars()
-            sb.export(outdir=output)
+            #sb.export(outdir=output)
 
         else: perror("file must be type '.fits' not %s\n"%ext)
     else: perror("can't access %s\n"%fname)
     return sb
 
 if __name__=="__main__":
-    printf("\x1b[1mlaunching \x1b[36mstarbug\x1b[0m\n")
+    puts(starbug2.logo%starbug2.motd)
 
     if ncores==1: starbugs=[ fn(fname) for fname in args ]
     else:
         pool=Pool(processes=ncores)
-        starbugs=pool.map(fn,args)
+        starbugs=pool.map(fn,args) ##
+        pool.close()
 
     for n,sb in enumerate(starbugs): 
         if not sb: perror("FAILED: %s\n"%args[n])
 
     ###########################
     # Match Output Catalogues #
     ###########################
 
     if options&DOMATCH and len(starbugs)>1:
+        if options&VERBOSE: printf("Matching outputs\n")
+
         if (fname:=combine_fnames( [sb.fname for sb in starbugs] )):
-            dname,name,ext=split_fname(fname)
-            dname=output if dname=="." else dname
-            fname="%s/%s"%(dname, name)
+            _,name,_=split_fname(os.path.basename(fname))
+            fname="%s/%s"%(starbugs[0].outdir, name)
         else: fname="out"
 
-        param=load_params(pfile)
         header=starbugs[0].header
         colnames=starbug2.match_cols
-        colnames+=[ name for name in param["MATCH_COLS"].split() if name not in colnames]
+        colnames+=[ name for name in init_parameters["MATCH_COLS"].split() if name not in colnames]
+        dthreshold=init_parameters["MATCH_THRESH"]
+        nthreshold=init_parameters["NEXP_THRESH"]
+        rmmatch=init_parameters["RM_MATCH"]
+        if rmmatch!=-1: 
+            warn()
+            perror("RM_MATCH is about to be depricated\n")
 
-        if options&VERBOSE: printf("Matching outputs\n")
 
         if options&(DODETECT|DOAPPHOT):
-            av,full=dither_match( [sb.detections for sb in starbugs] , threshold=param["MATCH_THRESH"], colnames=colnames)
+            av,full=dither_match([sb.detections for sb in starbugs], threshold=dthreshold, colnames=colnames)
 
-            N=len(starbugs)-param["RM_MATCH"]
-            mask=( (av["NUM"]>N) if param["RM_MATCH"]>=0 else (av["NUM"]>0))
+            if nthreshold>0:
+                mask=av["NUM"] >= nthreshold
+            else:
+                N=len(starbugs)-init_parameters["RM_MATCH"]
+                mask=( (av["NUM"]>N) if init_parameters["RM_MATCH"]>=0 else (av["NUM"]>0))
 
-            printf("-> %s-ap*...\n"%(fname))
             av.meta.update(header)
-            #export_table(hstack((av,full)), fname="%s-apfull.fits"%(fname), header=header)
+            printf("-> %s-ap*...\n"%(fname))
             export_table(full, fname="%s-apfull.fits"%(fname), header=header)
             export_table(av[mask], fname="%s-apmatch.fits"%(fname), header=header)
 
         if options&DOPHOTOM:
-            av,full=dither_match( [sb.psfcatalogue for sb in starbugs], threshold=param["MATCH_THRESH"], colnames=colnames)
-            printf("-> %s-psf*...\n"%(fname))
+            av,full=dither_match([sb.psfcatalogue for sb in starbugs], threshold=dthreshold, colnames=colnames)
+            if nthreshold>0:
+                mask=av["NUM"] >= nthreshold
+            else:
+                N=len(starbugs)-init_parameters["RM_MATCH"]
+                mask=( (av["NUM"]>N) if init_parameters["RM_MATCH"]>=0 else (av["NUM"]>0))
+
             av.meta.update(header)
-            export_table(hstack((av,full)), fname="%s-psffull.fits"%(fname), header=header)
-            export_table(av, fname="%s-psfmatch.fits"%(fname), header=header)
+            printf("-> %s-psf*...\n"%(fname))
+            export_table(full, fname="%s-psffull.fits"%(fname), header=header)
+            export_table(av[mask], fname="%s-psfmatch.fits"%(fname), header=header)
```

### Comparing `starbug2-0.3.9/bin/starbug2-match` & `starbug2-0.4.0/bin/starbug2-match`

 * *Files 18% similar despite different names*

```diff
@@ -76,31 +76,49 @@
     utils.perror("failed to load parameter file\n")
     quit("..quitting :(")
 
 tables=[Table.read(fname,format="fits") for fname in args]
 
 colnames=starbug2.match_cols
 colnames+=[ name for name in parameters["MATCH_COLS"].split() if name not in colnames]
+dthreshold=parameters["MATCH_THRESH"]
+nthreshold=parameters["NEXP_THRESH"]
+rmmatch=parameters["RM_MATCH"]
 
 if options & BANDMATCH:
-    matched=matching.band_match(tables,parameters["MATCH_THRESH"],colnames)
-    utils.export_table(matched,fname="out.fits")
+    filters= [ tab.meta.get("FILTER") for tab in tables ]
+    efilters=["e%s"%f for f in filters]
+    matched=matching.band_match(tables,dthreshold,["RA","DEC",*filters,*efilters])
+    fname=output if output else "out.fits"
+    utils.export_table(matched,fname=fname)
 
 else:
-    if options & DITHERMATCH: av,full=matching.dither_match(tables, parameters["MATCH_THRESH"], colnames)
+    if options & DITHERMATCH: av,full=matching.dither_match(tables, threshold=dthreshold, colnames=colnames)
     if options & GENERICMATCH: 
-        full=matching.generic_match(tables,threshold=parameters["MATCH_THRESH"], add_src=True)
+        options|=EXPFULL
+        full=matching.generic_match(tables,threshold=dthreshold, add_src=True)
         av=None#_=matching.finish_matching(full, colnames=tables[0].colnames)
     else:
-        av,full=matching.cascade_match(tables, parameters["MATCH_THRESH"], colnames)
+        av,full=matching.cascade_match(tables, threshold=dthreshold, colnames=colnames)
 
-
-    full=Table(full,dtype=[float]*len(full.colnames)).filled(np.nan) ## fill empty values with null
-
-    if av: av.meta.update(tables[0].meta)
+    dtypes=[]
+    for name in full.colnames:
+        if name=="Catalogue_Number": dtypes.append(str)
+        elif name=="flag": dtypes.append(np.uint16)
+        else: dtypes.append(float)
+    full=Table(full,dtype=dtypes).filled(np.nan) ## fill empty values with null
+
+    if av: 
+        av.meta.update(tables[0].meta)
+        if nthreshold!=-1:
+            mask=av["NUM"]>=nthreshold
+            av=av[mask]
+        if rmmatch!=-1:
+            warn()
+            perror("RM_MATCH has been removed, use NEXP_THRESH instead\n")
 
     if output is None:
         output=utils.combine_fnames( [ name for name in args] , ntrys=100)
     dname,fname,ext=utils.split_fname(output)
 
     utils.printf("-> %s/%s*\n"%(dname,fname))
     if options&EXPFULL: utils.export_table(full,fname="%s/%sfull.fits"%(dname,fname))
```

### Comparing `starbug2-0.3.9/extras/starbug2.completion` & `starbug2-0.4.0/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.9/starbug2/matching.py` & `starbug2-0.4.0/starbug2/matching.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,38 +89,46 @@
     _dec_cols= list( name for name in cat2.colnames if "DEC" in name)
     _ra= np.nanmean( tab2array( cat2, colnames=_ra_cols), axis=1)
     _dec=np.nanmean( tab2array( cat2, colnames=_dec_cols), axis=1)
     skycoord2=SkyCoord( ra=_ra*u.deg, dec=_dec*u.deg)
 
     return skycoord2.match_to_catalog_3d(skycoord1)
 
-def generic_match(catalogues, threshold=0.25, add_src=True):
+def generic_match(catalogues, threshold=0.25, add_src=True, load=None):
     """
     """
     threshold=threshold*u.arcsec
     base=Table(None)
 
     for n,cat in enumerate(catalogues,1):
         if "Catalogue_Number" in cat.colnames: cat.remove_column("Catalogue_Number")
         if not len(base):
             tmp=cat.copy()
         else:
-            tmp=Table(tmp,dtype=[float]*len(tmp.colnames)).filled(np.nan) ## fill empty values with null
+            #tmp=Table(tmp,dtype=[float]*len(tmp.colnames)).filled(np.nan) ## fill empty values with null
             idx,d2d,_=_match(base,cat)
             tmp=Table(np.full( (len(base),len(cat.colnames)), np.nan), names=cat.colnames)
 
             for src,IDX,sep in zip(cat,idx,d2d):
+                if load:
+                    load()
+                    load.show()
                 if (sep<=threshold) and (sep==min(d2d[idx==IDX])): ## GOOD MATCH
                     tmp[IDX]=src
                 elif add_src:   ##BAD MATCH / NEW SOURCE
                     tmp.add_row( src )
         tmp.rename_columns( tmp.colnames, ["%s_%d"%(name,n) for name in tmp.colnames] )
         base=hstack((base,tmp))
         #base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan) ## fill empty values with null
-    return base
+
+    for colname in base.colnames:
+        basename=colname[:colname.rfind("_")]
+        all_cols=find_colnames(base,basename)
+        if len(all_cols)==1: base.rename_column(colname,basename)
+    return reindex(base)
 
 
 
 def dither_match(catalogues, threshold, colnames):
     """
     This is the match for when you simultaneously detect sources over
     a series of pipeline stage2 dithers and wich to combine it into a single catalogue
@@ -200,16 +208,15 @@
     """
     Given a list of catalogues (with filter names in the meta data), match them
     in order of decreasing astrometric accuracy. 
     If F115W, F444W, F770W are input, the F115W centroid positions will be 
     taken as "correct". If a source is not resolved in this band, the next most 
     astrometrically accurate position is taken, i.e. F444W
     """
-    threshold=threshold*u.arcsec
-    colnames= list( name for name in catalogues[0].colnames if name in colnames)
+    #threshold=threshold*u.arcsec
     ### ORDER the tables into the correct order (increasing wavelength)
     tables=np.full( len(starbug2.filters), None)
     mask=np.full(len(starbug2.filters), False)
     for tab in catalogues:
         if "FILTER" in tab.meta.keys():
             if tab.meta["FILTER"] in starbug2.filters: 
                 ii=list(starbug2.filters.keys()).index(tab.meta["FILTER"])
@@ -221,46 +228,60 @@
     for fltr,tab in zip(starbug2.filters.keys(),tables):
         if tab: s+="%5s "%fltr
         #else: s+=". "
     puts(s)
 
     ### Match in increasing wavelength order
     base=Table(None)
-    load=loading(sum( [len(t) for t in tables[mask][1:]]),"matching", res=10)
+    load=loading(sum( [len(t) for t in tables[mask][1:]]),"matching", res=100)
     for fltr,tab in zip(starbug2.filters.keys(),tables):
         if not tab: continue
         load.msg="matching:%s"%fltr
-        if not len(base): tmp=tab[colnames].copy()
+        _colnames= list( name for name in tab.colnames if name in colnames)
+        if not len(base): 
+            tmp=tab[_colnames].copy()
         else:
             idx,d2d,_=_match(base,tab)
-            tmp=Table(np.full( (len(base),len(colnames)), np.nan), names=colnames)
+            tmp=Table(np.full( (len(base),len(_colnames)), np.nan), names=_colnames)
+            
+            ###################################
+            # Hard coding separations for now #
+            separation=0.06
+            f_id=list(starbug2.filters.keys()).index(fltr)
+            if f_id >= list(starbug2.filters.keys()).index("F277W"): separation=0.10
+            if f_id >= list(starbug2.filters.keys()).index("F560W"): separation=0.15
+            if f_id >= list(starbug2.filters.keys()).index("F1000W"): separation=0.20
+            if f_id >= list(starbug2.filters.keys()).index("F1500W"): separation=0.25
+
 
             for ii,(src,IDX,sep) in enumerate(zip(tab,idx,d2d)):
+                load.msg="matching:%s(%.2g)"%(fltr,separation)
                 load();load.show()
-                if (sep<=threshold) and (sep==min(d2d[idx==IDX])):
-                    for name in colnames: tmp[IDX][name]=src[name]
+                if (sep<=separation*u.arcsec) and (sep==min(d2d[idx==IDX])):
+                    for name in _colnames: tmp[IDX][name]=src[name]
                 else:
-                    tmp.add_row(src[colnames])
-
-        base=hstack(( base,tmp[["flux","eflux"]] ))
-        mag,magerr=flux2ABmag(tmp["flux"], tmp["eflux"],fltr)
-        base.add_column(mag,name=fltr)
-        base.add_column(magerr,name="e%s"%fltr)
+                    tmp.add_row(src[_colnames])
+            #tmp=generic_match((base,tab), threshold=threshold, add_src=True, load=load)
 
-        base.rename_column("flux","%s_flux"%fltr)
-        base.rename_column("eflux","%s_eflux"%fltr)
+        #base=hstack(( base,tmp[["flux","eflux"]] ))
+        #mag,magerr=flux2ABmag(tmp["flux"], tmp["eflux"],fltr)
+        #base.add_column(mag,name=fltr)
+        #base.add_column(magerr,name="e%s"%fltr)
+
+        #base.rename_column("flux","%s_flux"%fltr)
+        #base.rename_column("eflux","%s_eflux"%fltr)
+        base=hstack(( base,tmp[[fltr,"e%s"%fltr]] ))
         base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan)
 
         ### Only keep the most astromectrically correct position
         if "RA" not in base.colnames: base=hstack(( tmp[["RA","DEC"]], base))
         else:
             _mask=np.logical_and( np.isnan(base["RA"]), tmp["RA"]!=np.nan)
             base["RA"][_mask]=tmp["RA"][_mask]
             base["DEC"][_mask]=tmp["DEC"][_mask]
-    export_table(base,"/tmp/tab.fits")
     return base
 
 def stage_match(stage2, stage3, threshold):
     """
     Match together a stage 2 and stage 3 catalogue
     if the star is resolved in just the stage 3, it takes on that value
     if the star is resolved in both, the stage3 is ignored
@@ -309,22 +330,25 @@
         elif name== "eflux":
             col=Column(np.sqrt(np.nansum(ar*ar, axis=1)), name=name)
         elif name=="stdflux": 
             col=Column(np.nanmax(ar,axis=1),name=name)
         elif name=="flag":
             col=Column(flags, name=name)
             for fcol in ar.T: col|=fcol.astype(np.uint16)
+        elif name=="NUM":
+            col=Column(np.nansum(ar, axis=1), name=name)
         else: col=Column(np.nanmedian(ar, axis=1),name=name)
         
         av[name]=col
     mag,magerr=flux2ABmag(av["flux"],av["eflux"], tab.meta["FILTER"])
     av.add_column(mag,name=tab.meta["FILTER"])
     av.add_column(magerr,name="e%s"%tab.meta["FILTER"])
-    narr= np.nansum( np.invert( np.isnan(tab2array(tab,find_colnames(tab,colnames[0])))),axis=1)
-    av.add_column(Column(narr, name="NUM"))
+    if "NUM" not in av.colnames:
+        narr= np.nansum( np.invert( np.isnan(tab2array(tab,find_colnames(tab,colnames[0])))),axis=1)
+        av.add_column(Column(narr, name="NUM"))
     return (av,tab)
 
 
 def remove_NUM(tab, N):
     """
     Remove sources from the list of tab if they have >N non matches
     """
```

### Comparing `starbug2-0.3.9/starbug2/misc.py` & `starbug2-0.4.0/starbug2/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Miscillaneous functions...
 """
 import os,stat,sys,numpy as np
 import pkg_resources
 import starbug2
 from starbug2.utils import *
-from starbug2.matching import sort_exposures
+from starbug2.matching import sort_exposures, generic_match
 from astropy.io import fits
 
 
 
 ##########################
 # One time run functions #
 ##########################
@@ -159,8 +159,32 @@
             fpo.write(outline)
         fpi.close()
         fpo.close()
         fpd.close()
         os.system("mv /tmp/starbug.param %s"%fname)
     else: perror("local parameter file '%s' does not exist\n"%fname)
 
+def calc_instrumental_zeropint(psftable, aptable, fltr=None ):
+    """
 
+    """
+    printf("Calculating instrumental zeropoint.\n")
+    if fltr is None and not (fltr:=psftable.meta.get("FILTER")):
+        perror("Unable to determine filter, set with '--set FILTER=F000W'.\n")
+        return None
+    
+
+    matched=generic_match((psftable, aptable), threshold=0.1, add_src=False)
+    dist=np.array((matched["%s_2"%fltr]-matched["%s_1"%fltr]).value)
+    zp=np.nanmedian(dist)
+    std=np.nanstd(dist)
+    printf("-> zp=%.3f +/- %.2g\n"%(zp,std))
+    return (zp,std)
+#def tmpfn(psftable, aptable):
+#    if "flux" in psftable.colnames and "flux" in aptable.colnames:
+#        matched=generic_match((psftable, aptable), threshold=0.1, add_src=False)
+#        dist=np.array((matched["flux_1"]-matched["flux_2"]).value)
+#        zp=np.nanmedian(dist)
+#        std=np.nanstd(dist)
+#        printf("-> zp=%.3f +/- %.2g\n"%(zp,std))
+#        return (zp,std)
+#    else: return None
```

### Comparing `starbug2-0.3.9/starbug2/param/default.param` & `starbug2-0.4.0/starbug2/param/default.param`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,71 @@
 ## STARBUG CONFIG FILE
-PARAM = STARBUGII PARAMETERS    //COMMENT
-TEST = 0    //.
+PARAM       =  STARBUGII PARAMETERS     //COMMENT
+TEST        = 0          //.
 
 ## GENERIC
-VERBOSE =0       // (0:false 1:true)
-OUTDIR	=. //.
-HDUNAME =  //If using a non standard HDU name, name it here (str or int)
+VERBOSE     = 0          // (0:false 1:true)
+OUTPUT      = .          //Directory or filename to output to 
+HDUNAME     =            //If using a non standard HDU name, name it here (str or int)
 
 ## DETECTETION 
-SIGSKY		=2.0  // (float>0) 
-SIGSRC		=5.0  // (float>0) Source value mininmum N sigma above background
-BOX_SIZE	=2    // (int>0) Background estimation kernal size (pix)
-DOBGD2D     =1    // Run background2D estimation (usually finds more sources but takes time)
-CLEANSRC    =1    // Run source cleaning after detection (removes likely contaminants)
-SHARP_LO    = 0.4 // cutoff in detection
-SHARP_HI    = 0.9 // cutoff in detection
-ROUND_LO    =-1.0 // cutoff in detection
-ROUND_HI    = 1.0 // cutoff in detection
-RICKER_R    = 1.0 // Radius (pix) of ricker wavelet 
+SIGSKY      = 2.0        // (float>0) 
+SIGSRC      = 5.0        // (float>0) Source value mininmum N sigma above background
+DOBGD2D     = 1          // Run background2D estimation (usually finds more sources but takes time)
+CLEANSRC    = 1          // Run source cleaning after detection (removes likely contaminants)
+SHARP_LO    = 0.4        // cutoff in detection
+SHARP_HI    = 0.9        // cutoff in detection
+ROUND_LO    = -1.0       // cutoff in detection
+ROUND_HI    = 1.0        // cutoff in detection
+RICKER_R    = 1.0        // Radius (pix) of ricker wavelet 
 
 ## APERTURE PHOTOMOETRY
-APPHOT_R    =1.5   //Radius in number of pixels
-ENCENERGY	=0.5   //Fraction encircled energy (mutually exclusive with APPHOT_R)
-FIT_APP_R	=1	   //Fit APPHOT_R to the aperture correction CRDS (if =0, use ENCENRGY instead)
-SKY_RIN     =3     //Sky annulus inner radius
-SKY_ROUT    =4.5   //Sky annulus outer radius
+APPHOT_R    = 1.5        //Radius in number of pixels
+ENCENERGY   = 0.5        //Fraction encircled energy (mutually exclusive with APPHOT_R)
+FIT_APP_R   = 1          //Fit APPHOT_R to the aperture correction CRDS (if =0, use ENCENRGY instead)
+SKY_RIN     = 3          //Sky annulus inner radius
+SKY_ROUT    = 4.5        //Sky annulus outer radius
 
 ## CLEANUP
-ERROR_CUT       =1  // cut sources with errors larger than value
-SHARP_HI_SIG    =2  // after detection, number of sigma above gaussian mean to cut off sources
-SHARP_LO_SIG    =2  // after detection, number of sigma above gaussian mean to cut off sources
-ROUND_HI_SIG    =2  // after detection, number of sigma above gaussian mean to cut off sources
-ROUND_LO_SIG    =2  // after detection, number of sigma above gaussian mean to cut off sources
+ERROR_CUT   = 1          // cut sources with errors larger than value
+SHARP_HI_SIG= 2          // after detection, number of sigma above gaussian mean to cut off sources
+SHARP_LO_SIG= 2          // after detection, number of sigma above gaussian mean to cut off sources
+ROUND_HI_SIG= 2          // after detection, number of sigma above gaussian mean to cut off sources
+ROUND_LO_SIG= 2          // after detection, number of sigma above gaussian mean to cut off sources
 
 ## BACKGROUNDESTIMATION
-BGD_R	=	0//.
+BGD_R       = 0          //.
+BOX_SIZE    = 2          // (int>0) Background estimation kernal size (pix)
 
 ## PHOTOMETRY
-AP_FILE     =      //Detection file to use instead of detecting
-BGD_FILE    =      //Background estimation file
-PSF_FILE    =      //Non default PSF file
-CRIT_SEP    =8     //minimum distance for grouping (pixels) between two sources
-FORCE_POS   =0     //Force centroid position (1) or allow psf fitting to fit position too (0)
-DPOS_THRESH =0.1   //If allowed to fit position, max separation (arcsec) from source list centroid
-PSF_SIZE    =-1    //Set fit size of psf (>0) or -1 to take PSF file dimensions
-GEN_RESIDUAL=0     //generate a residual image
+AP_FILE     =            //Detection file to use instead of detecting
+BGD_FILE    =            //Background estimation file
+PSF_FILE    =            //Non default PSF file
+CRIT_SEP    = 8          //minimum distance for grouping (pixels) between two sources
+FORCE_POS   = 0          //Force centroid position (1) or allow psf fitting to fit position too (0)
+DPOS_THRESH = 0.1        //If allowed to fit position, max separation (arcsec) from source list centroid
+PSF_SIZE    = -1         //Set fit size of psf (>0) or -1 to take PSF file dimensions
+GEN_RESIDUAL= 0          //generate a residual image
 
 ## SOURCE STATS
-CALC_CROWD  =1     //Run crowding metric calculation (execution time scales N^2)
+CALC_CROWD  = 1          //Run crowding metric calculation (execution time scales N^2)
 
 ## CATALOGUE MATCHING
-MATCH_THRESH =0.1  					//when combining background subtraction catalogue, minimum separation (arcsec) of centroids to be considered separate sources
-MATCH_COLS =                        // EXTRA columns to include in output matched table i.e sharpness
-RM_MATCH =-1                        // Remove any sources with less matches than N-RM_MATCH. (if -1, keep everything)
+MATCH_THRESH= 0.1        //when combining background subtraction catalogue, minimum separation (arcsec) of centroids to be considered separate sources
+MATCH_COLS  =            // EXTRA columns to include in output matched table i.e sharpness
+RM_MATCH    = -1         // [REMOVING THIS SOON] Remove any sources with less matches than N-RM_MATCH. (if -1, keep everything) 
+NEXP_THRESH = -1         // Keep sources that appear in NUM >= NEXP_THRESH (if -1 keep everything)
 
 ## ARTIFICAL STARS
-NUMBER_ARTIFICIAL_STARS =500   //number of individual stars to test
-SUBIMAGE_SIZE =500             //number of pixels ? to crop around artificial star
-MIN_FLUX    =10                //minimun flux for artificial star
-MAX_FLUX    =10000             //maximum flux for artificial star
-SEPARATION_THRESH =2           //number pixels above which the separation is too high and the artifical star failed to be detected
+NUMBER_ARTIFICIAL_STARS= 500 //number of individual stars to test
+SUBIMAGE_SIZE= 500       //number of pixels ? to crop around artificial star
+MIN_FLUX    = 10         //minimun flux for artificial star
+MAX_FLUX    = 10000      //maximum flux for artificial star
+SEPARATION_THRESH= 2     //number pixels above which the separation is too high and the artifical star failed to be detected
 
 ## MISC EXTRAS
-REGION_COL  = green     //DS9 region colour
-REGION_SCAL = 1         //Scale region to flux if possible
-REGION_RAD  = 3         //Region radius default
-REGION_XCOL = RA        //X column name to use for region
-REGION_YCOL = DEC       //Y column name to use for region
-REGION_WCS  = 1         //If X/Y column names correspind to WCS values
+REGION_COL  = green      //DS9 region colour
+REGION_SCAL = 1          //Scale region to flux if possible
+REGION_RAD  = 3          //Region radius default
+REGION_XCOL = RA         //X column name to use for region
+REGION_YCOL = DEC        //Y column name to use for region
+REGION_WCS  = 1          //If X/Y column names correspind to WCS values
```

### Comparing `starbug2-0.3.9/starbug2/routines.py` & `starbug2-0.4.0/starbug2/routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Routines for Starbug
 """
+import os
 import sys
 import time
 import numpy as np
 import pkg_resources
 from scipy.stats import norm#, mode
 from scipy.optimize import curve_fit
 from scipy.ndimage import convolve
@@ -126,18 +127,19 @@
         if self.verbose: printf("-> [BGD2D] pass: %d sources\n"%len(self.catalogue))
 
         ## 2nd order differential detection
         kernel=RickerWavelet2DKernel(self.ricker_r)
         conv=convolve(data, kernel)
         corr=match_template(conv/np.amax(conv), kernel.array)
         _detections=self.detect(corr, method="findpeaks")
-        _detections["x_peak"]+=kernel.shape[0]//2
-        _detections["y_peak"]+=kernel.shape[0]//2
-        _detections.rename_columns( ("x_peak","y_peak"),("xcentroid","ycentroid"))
-        self.catalogue=self.match(self.catalogue, _detections)
+        if _detections:
+            _detections["x_peak"]+=kernel.shape[0]//2
+            _detections["y_peak"]+=kernel.shape[0]//2
+            _detections.rename_columns( ("x_peak","y_peak"),("xcentroid","ycentroid"))
+            self.catalogue=self.match(self.catalogue, _detections)
         if self.verbose: printf("-> [CONVL] pass: %d sources\n"%len(self.catalogue))
 
         ## Now with xycoords DAOStarfinder will refit the sharp and round values at the detected locations
         #self.catalogue=self.detect(data, xycoords=np.array([self.catalogue["xcentroid"],self.catalogue["ycentroid"]]).T)#, clean=0)
         tmp=SourceProperties(data,self.catalogue, verbose=self.verbose).calculate_geometry(self.fwhm)
         if tmp: self.catalogue=tmp
 
@@ -350,33 +352,42 @@
     Issue:6 recursion during fitting.
         >>> the fitting seems to include this recursive step within a given source of sources
             if the group contains more members than the system recursion limit then it will
             unceremonially crash on a recursion error.
         >>> for now at least, I will give a warning that this would have occurred, but then 
             ill override the recursion limit and avoid the crash. Hopefully
     """
+    logfile=None
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.ngroups=0
+        if os.getenv("SBIIDEBUG"):
+            self.logfile=open(os.getenv("SBIIDEBUG"),'a')
+            self.logfile.write("# PSF Source Grouping\n")
+
     def __call__(self, *args):
         res=super().__call__(*args)
         self.ngroups=max(res["group_id"])
 
         #### hacking recursion error
         for gid in set(res["group_id"]):
             n_members=sum(res["group_id"]==gid)
+            if self.logfile:
+                self.logfile.write("GID:%d (%d)\n"%(gid,n_members))
+
             ## It seems to not quite hit the recursion limit
             ## Crashed on 980 with a limit of 1000, so im going to try 90%
             if n_members > (0.9*sys.getrecursionlimit()):
                 warn()
                 perror("This run will exceed the recursion depth of the system. "
                        "Starbug will intervene and override the recursion limit but "
                        "the parameter \"CRIT_SEP\" should be reduced to avoid this.\n"
-                       "Setting recursion limit %d -> %d\n"%(sys.getrecursionlimit(), n_members))
+                       "Setting recursion limit %d -> %d\n"%(sys.getrecursionlimit(), int(1.1*n_members)))
                 sys.setrecursionlimit(int(1.1*n_members))
+        if self.logfile: self.logfile.close()
         return res
 
 class _fitmodel(LevMarLSQFitter):
     load=None
     def __init__(self, grouper=None, verbose=1):
         super().__init__()
         self.grouper=grouper
```

### Comparing `starbug2-0.3.9/starbug2/starbug.py` & `starbug2-0.4.0/starbug2/starbug.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     StarbugBase is the overall container for the photometry package. It holds the active image,
     the parameter file and the output images/tables.
     It is self contained enough to simply run "photometry" and everything should just take care
     of itself from there on.
     """
     filter=None
     stage=0
+    outdir=""
     fname=None
+    bname=""
+
     detections=None
     psfcatalogue=None
     residuals=None
     background=None
     source_stats=None
     psf=None
 
@@ -33,17 +36,18 @@
         """
         fname : FITS image file name
         pfile : parameter file name
         options : extra options to load into starbug
         """
         if not pfile: pfile="%s/default.param"%pkg_resources.resource_filename("starbug2","param/")
         self.options=load_params(pfile)
-        self.options.update(options)
-
+        self.options.update(dict((key,options[key]) for key in options.keys() if key in self.options))
         self.load_image(fname)   ## Load the fits image
+
+
         if self.options["AP_FILE"]: self.load_apfile() ## Load the source list if given
         if self.options["BGD_FILE"]: self.load_bgdfile()
 
         #_=self.image ## Force self._nHDU
 
     @property
     def header(self):
@@ -123,15 +127,24 @@
     def load_image(self, fname):
         """
         Given fname, load the image into starbug to be worked on.
         Will return None if file isnt readable
         """
         self.fname=fname
         if fname:
-            dname,bname,extension=split_fname(fname)
+            #########################################
+            # Sorting out the file names and what not
+            #########################################
+            self.outdir,self.bname,extension=split_fname(fname)
+            if (tmp_outname:=self.options.get("OUTPUT")) and tmp_outname !='.':
+                outdir,bname,_=split_fname(tmp_outname)
+                if os.path.exists(outdir) and os.path.isdir(outdir): self.outdir=outdir
+                else: perror("unable to locate output directory \"%s\"\n"%outdir)
+                if bname: self.bname=bname
+
             if extension==".fits":
                 if os.path.exists(fname):
                     self.log("loaded: \"%s\"\n"%fname)
                     self._image=fits.open(fname)
                     _=self.image ## Force assigning _nHDU
                     self.log("-> using image HDU: %d (%s)\n"%(self._nHDU,self.image.name))
 
@@ -179,15 +192,21 @@
             if "flag" in cn:
                 self.detections["flag"]=Column(self.detections["flag"], dtype=np.uint16)
 
             self.log("loaded AP_FILE='%s'\n"%fname)
 
             if not any( _ in cn for _ in ("xcentroid","ycentroid","x_0","y_0")):
                 if all( _ in cn for _ in ("RA","DEC")):
-                    xy=self.wcs.all_world2pix(self.detections["RA"], self.detections["DEC"],0)
+                    try:
+                        xy=self.wcs.all_world2pix(self.detections["RA"], self.detections["DEC"],0)
+                    except:
+                        warn()
+                        perror("Something went wrong converting WCS to pixels, trying wcs_world2pix next.\n")
+                        xy=self.wcs.wcs_world2pix(self.detections["RA"], self.detections["DEC"],0)
+
                     self.detections.add_columns(xy,names=("xcentroid","ycentroid"),indexes=[0,0])
                     self.log("-> using RADEC coordinates\n")
                 else: perror("WARNING, unable to determine physical coordinates from detections table\n")
             if len( set(("x_0","y_0"))&set(self.detections.colnames))==2: self.detections.rename_columns(("x_0","y_0"),("xcentroid","ycentroid"))
         else: perror("AP_FILE='%s' does not exists\n"%fname)
 
     def load_bgdfile(self,fname=None):
@@ -250,20 +269,20 @@
                                         boxsize=int(self.options["BOX_SIZE"]),
                                         cleansrc=self.options["CLEANSRC"],
                                         verbose=self.options["VERBOSE"])
 
             self.detections=detector(self.image.data.copy())["xcentroid","ycentroid","sharpness","roundness1","roundness2"]
 
             ra,dec=self.wcs.all_pix2world(self.detections["xcentroid"], self.detections["ycentroid"],0)
-            self.detections.add_column( Column(ra, name="RA"), index=1)
-            self.detections.add_column( Column(dec, name="DEC"), index=2)
-            self.aperture_photometry()
-
+            self.detections.add_column( Column(ra, name="RA"), index=2)
+            self.detections.add_column( Column(dec, name="DEC"), index=3)
             self.detections.meta=dict(self.header.items())
             self.detections.meta.update({"ROUNTINE":"DETECT"})
+            self.aperture_photometry()
+
 
 
     def aperture_photometry(self):
 
         if self.detections is None:
             perror("No detection source file loaded (-d file-ap.fits)\n")
             return
@@ -327,14 +346,23 @@
         else: ##stage 3 version
             ap_cat=apphot(self.detections, image, error=error, apcorr=apcorr, sig_sky=self.options["SIGSKY"])
 
         mag,magerr=flux2ABmag( ap_cat["flux"], ap_cat["eflux"], filter=self.filter)
         ap_cat.add_column(Column(mag,self.filter))
         ap_cat.add_column(Column(magerr,"e%s"%self.filter))
         self.detections=hstack((self.detections,ap_cat))
+        #self.detections.meta=dict(self.header.items())
+        #self.detections.meta.update({"ROUNTINE":"DETECT"})
+
+        reindex(self.detections)
+        self.detections.meta["FILTER"]=self.filter
+        _fname="%s/%s-ap.fits"%(self.outdir, self.bname)
+        self.log("--> %s\n"%_fname)
+        fits.BinTableHDU( data=self.detections, header=self.header ).writeto(_fname, overwrite=True)
+
 
     def bgd_estimate(self):
         """
         Estimate the background of the active image
         Saves the result as an ImageHDU self.background
         """
         self.log("Estimating Background\n")
@@ -347,30 +375,37 @@
             sources=sources[ sources[yname]>=0 ]
             sources=sources[ sources[xname]<self.image.header["NAXIS1"]]
             sources=sources[ sources[yname]<self.image.header["NAXIS2"]]
             bgd=BackGround_Estimate_Routine(sources,
                                             boxsize=int(self.options["BOX_SIZE"]),
                                             fwhm=starbug2.filters[self.filter].pFWHM,
                                             verbose=self.options["VERBOSE"])
-            self.background=fits.ImageHDU(data=bgd(self.image.data.copy()), header=self.wcs.to_header())
+            header=fits.Header({**self.header,**self.wcs.to_header()})
+            self.background=fits.ImageHDU(data=bgd(self.image.data.copy()), header=header)
+            _fname="%s/%s-bgd.fits"%(self.outdir, self.bname)
+            self.log("--> %s\n"%_fname)
+            self.background.writeto(_fname,overwrite=True)
         else:
             perror("unable to estimate background, no source list loaded\n")
 
+
+
     def bgd_subtraction(self):
         """
         Internally subtract a background array from an image array
         """
         self.log("Subtracting Background\n")
 
         if self.background is None:
             perror("No background array loaded (-b file-bgd.fits)\n")
             return
         array= self.image.data - self.background.data
         self.residuals = array
         self._image[self._nHDU].data=array
+        fits.ImageHDU(data=self.residuals, name="RES", header=fits.Header({**self.header,**self.wcs.to_header()})).writeto("%s/%s-res.fits"%(self.outdir,self.bname), overwrite=True)
 
     def photometry(self):
         """
         Full photometry routine
         Saves the result as a table self.psfcatalogue
         // Additionally it appends a residual Image onto the self.residuals HDUList
         """
@@ -392,18 +427,20 @@
             ###################################
             # Collect relevent files and data #
             ###################################
 
             image=self.image.data.copy()
             bgd = self.background.data.copy()
 
-            _bunit=self.image.header.get("BUNIT")
-            _scalefactor=self.image.header.get("PHOTMJSR")
-            if _scalefactor:#https://spacetelescope.github.io/jdat_notebooks/notebooks/psf_photometry/NIRCam_PSF_Photometry_Example.html
-                self.log("-> PHOTMJSR: %f\n"%_scalefactor)
+            #_scalefactor=self.image.header.get("PHOTMJSR")#https://spacetelescope.github.io/jdat_notebooks/notebooks/psf_photometry/NIRCam_PSF_Photometry_Example.html
+            #_bunit=self.image.header.get("BUNIT")
+                #self.log("-> PHOTMJSR: %f\n"%_scalefactor)
+            _scalefactor=get_MJysr2Jy_scalefactor(self.image)
+            if _scalefactor:
+                self.log("-> converting unit from MJy/sr to Jr with factor: %e\n"%_scalefactor)
                 image/=_scalefactor
                 bgd/=_scalefactor
 
             psf_model=FittableImageModel(self.psf)
             #psf_model=EPSFModel(fp[1].data)
             if self.options["PSF_SIZE"]>0: size=int(self.options["PSF_SIZE"])
             else: size=psf_model.shape[0]
@@ -418,18 +455,27 @@
             if "xcentroid" in init_guesses.colnames: init_guesses.rename_column("xcentroid", "x_0")
             if "ycentroid" in init_guesses.colnames: init_guesses.rename_column("ycentroid", "y_0")
 
             init_guesses=init_guesses[ init_guesses["x_0"]>=0 ]
             init_guesses=init_guesses[ init_guesses["y_0"]>=0 ]
             init_guesses=init_guesses[ init_guesses["x_0"]<self.image.header["NAXIS1"]]
             init_guesses=init_guesses[ init_guesses["y_0"]<self.image.header["NAXIS2"]]
-            init_guesses=init_guesses[["x_0","y_0","flux",self.filter, "flag"]]
+
+            ######
+            # Allow tables that dont have the correct columns through
+            ######
+            required=["x_0","y_0","flux",self.filter, "flag"]
+            for notfound in  set(required)-set(init_guesses.colnames):
+                dtype=np.uint16 if notfound=="flag" else float
+                init_guesses.add_column( Column( np.zeros(len(init_guesses)), name=notfound, dtype=dtype) )
+
+            init_guesses=init_guesses[required]
             init_guesses.remove_column("flux")
-            #init_guesses.rename_column("flux","flux_0")
             init_guesses.rename_column(self.filter,"ap_%s"%self.filter)
+            #init_guesses.rename_column("flux","flux_0")
             #init_guesses=init_guesses[init_guesses["flux_0"]>0]
             #init_guesses.remove_column("flux_0")
 
             ###########
             # Run Fit #
             ###########
 
@@ -454,25 +500,26 @@
                 _fixpsf_cat["flag"] |= starbug2.SRC_FIX
 
             if _psf_cat is not None and _fixpsf_cat is not None: psf_cat=vstack((_psf_cat,_fixpsf_cat))
             elif _psf_cat is None: psf_cat=_fixpsf_cat
             else: psf_cat=_psf_cat
 
             ra,dec=self.wcs.all_pix2world(psf_cat["x_fit"], psf_cat["y_fit"],0)
-            psf_cat.add_column( Column(ra, name="RA"), index=1)
-            psf_cat.add_column( Column(dec, name="DEC"), index=2)
+            psf_cat.add_column( Column(ra, name="RA"), index=2)
+            psf_cat.add_column( Column(dec, name="DEC"), index=3)
 
             ##################
             # Residual Image #
             ##################
 
             if self.options["GEN_RESIDUAL"]:
                 self.log("-> generating residual\n")
                 residual = subtract_psf(image-bgd, psf_model, psf_cat[["x_fit","y_fit","flux_fit"]], subshape=(size,size))
                 self.residuals=residual
+                fits.ImageHDU(data=self.residuals, name="RES", header=fits.Header({**self.header,**self.wcs.to_header()})).writeto("%s/%s-res.fits"%(self.outdir,self.bname), overwrite=True)
 
             ######################
             # Photometric offset # takes the top 50% least crowded sources
             ######################
 
             #crowd=SourceProperties(self._image["SCI"].data, psf_cat[["RA","DEC"]]).calculate_crowding()
             #ii=np.argsort(crowd)[len(crowd)//2:]
@@ -485,15 +532,20 @@
 
             psf_cat.add_column(mag,name=self.filter)
             psf_cat.add_column(magerr,name="e%s"%self.filter)
             self.psfcatalogue=tabppend(self.psfcatalogue, psf_cat)
             self.psfcatalogue.meta=dict(self.header.items())
             self.psfcatalogue.meta["AP_FILE"]=self.options["AP_FILE"]
             self.psfcatalogue.meta["BGD_FILE"]=self.options["BGD_FILE"]
-            #self.background=fits.ImageHDU(data=phot.bkg_estimator.bgd, name="BACKGROUND", header=self.wcs.to_header()) ##So is it supposed to be a fits image or a numpy array?!
+
+            reindex(self.psfcatalogue)
+            _fname="%s/%s-psf.fits"%(self.outdir, self.bname)
+            self.log("--> %s\n"%_fname)
+            fits.BinTableHDU(data=self.psfcatalogue, header=self.header).writeto(_fname,overwrite=True)
+
 
     def cleanup(self):
         """
         """
         self.log("Cleaning up..\n")
 
         if self.detections:
@@ -547,46 +599,47 @@
 
         art=ArtificialStar_Routine(detector, phot, psf_model)
         self.log("Artificial Star Testing (n=%d)\n"%(self.options["NUMBER_ARTIFICIAL_STARS"]))
         result=art.run(self.image.data, ntests=self.options["NUMBER_ARTIFICIAL_STARS"], flux_range=(self.options["MIN_FLUX"], self.options["MAX_FLUX"]),
                 subimage_size=self.options["SUBIMAGE_SIZE"], separation_thresh=self.options["SEPARATION_THRESH"], fwhm=starbug2.filters[self.filter].pFWHM)
         export_table(result, "/tmp/artificialstars.fits")
 
-    def export(self, outdir=None):
-        """
-        Export all the current catalogues
-        """
-        if not outdir: outdir=self.options["OUTDIR"]
-        if not os.path.exists("%s/"%outdir):
-            perror("output directory '%s' does not exist, using /tmp instead\n"%outdir)
-            outdir="/tmp"
-
-        dname,fname,ext=split_fname(self.fname)
-        if self.detections:
-            self.detections.meta["FILTER"]=self.filter
-            reindex(self.detections)
-            hdulist=[fits.PrimaryHDU(header=self.header),fits.BinTableHDU(data=self.detections)]
-            fits.HDUList(hdulist).writeto("%s/%s-ap.fits"%(outdir,fname), overwrite=True)
-            #export_table(self.detections, fname="%s/%s-ap.fits"%(outdir,fname))
-        if self.psfcatalogue:
-            reindex(self.psfcatalogue)
-            hdulist=[fits.PrimaryHDU(header=self.header),fits.BinTableHDU(data=self.psfcatalogue)]
-            fits.HDUList(hdulist).writeto("%s/%s-psf.fits"%(outdir,fname), overwrite=True)
-            #export_table(self.psfcatalogue, fname="%s/%s-psf.fits"%(outdir,fname))
-        if self.background: 
-            #self.background.header.update(header)
-            self.background.writeto("%s/%s-bgd.fits"%(outdir,fname), overwrite=True)
-        if self.residuals is not None:
-            im=fits.ImageHDU(data=self.residuals, name="RES", header=self.header)
-            im.header.update(self.wcs.to_header())
-            im.writeto("%s/%s-res.fits"%(outdir,fname), overwrite=True)
-        if self.source_stats is not None:
-            reindex(self.source_stats)
-            hdulist=[fits.PrimaryHDU(header=self.header),fits.BinTableHDU(data=self.source_stats)]
-            fits.HDUList(hdulist).writeto("%s/%s-stat.fits"%(outdir,fname), overwrite=True)
+    #def export_residuals(self):
+    #def export(self, outdir=None):
+    #    """
+    #    Export all the current catalogues
+    #    """
+    #    if not outdir: outdir=self.options["OUTPUT"]
+    #    if not os.path.exists("%s/"%outdir):
+    #        perror("output directory '%s' does not exist, using /tmp instead\n"%outdir)
+    #        outdir="/tmp"
+
+    #    dname,fname,ext=split_fname(self.fname)
+    #    if self.detections:
+    #        self.detections.meta["FILTER"]=self.filter
+    #        reindex(self.detections)
+    #        hdulist=[fits.PrimaryHDU(header=self.header),fits.BinTableHDU(data=self.detections)]
+    #        fits.HDUList(hdulist).writeto("%s/%s-ap.fits"%(outdir,fname), overwrite=True)
+    #        #export_table(self.detections, fname="%s/%s-ap.fits"%(outdir,fname))
+    #    if self.psfcatalogue:
+    #        reindex(self.psfcatalogue)
+    #        hdulist=[fits.PrimaryHDU(header=self.header),fits.BinTableHDU(data=self.psfcatalogue)]
+    #        fits.HDUList(hdulist).writeto("%s/%s-psf.fits"%(outdir,fname), overwrite=True)
+    #        #export_table(self.psfcatalogue, fname="%s/%s-psf.fits"%(outdir,fname))
+    #    if self.background: 
+    #        #self.background.header.update(header)
+    #        self.background.writeto("%s/%s-bgd.fits"%(outdir,fname), overwrite=True)
+    #    if self.residuals is not None:
+    #        im=fits.ImageHDU(data=self.residuals, name="RES", header=self.header)
+    #        im.header.update(self.wcs.to_header())
+    #        im.writeto("%s/%s-res.fits"%(outdir,fname), overwrite=True)
+    #    if self.source_stats is not None:
+    #        reindex(self.source_stats)
+    #        hdulist=[fits.PrimaryHDU(header=self.header),fits.BinTableHDU(data=self.source_stats)]
+    #        fits.HDUList(hdulist).writeto("%s/%s-stat.fits"%(outdir,fname), overwrite=True)
 
     def source_geometry(self):
         """
         Calculate source geometry stats for a given image and source list
         """
         if self.detections is None: perror("No source file loaded\n")
         else:
@@ -598,14 +651,18 @@
             slist=slist[ slist["ycentroid"]<self.image.header["NAXIS2"]]
 
             sp=SourceProperties(self.image.data, slist, verbose=self.options["VERBOSE"])
             stat=sp(fwhm=starbug2.filters[self.filter].pFWHM, do_crowd=self.options["CALC_CROWD"])
             #geom=sp.calculate_geometry(fwhm=starbug2.filters[self.filter].pFWHM)
             
             self.source_stats=hstack((slist,stat))
+            _fname="%s/%s-stat.fits"%(self.outdir, self.bname)
+            self.log("--> %s\n"%_fname)
+            reindex(self.source_stats)
+            fits.BinTableHDU(data=self.source_stats,header=self.header).writeto(_fname, overwrite=True)
 
 
 
     def verify(self):
         """
         This simple function verifies that everything necessary has been loaded properly
         RETURN: 
@@ -629,31 +686,47 @@
         else:
             pass
             #if not os.path.exists("%s/%s%s.fits"%(dname, self.filter, self.info["DETECTOR"])):
             #        warn()
             #        perror("Unable to locate filter PSF for '%s'\n"%self.filter)
             #        status=1
         
-        if not os.path.exists((dname:=os.path.expandvars(self.options["OUTDIR"]))):
+        if not os.path.exists(self.outdir):
             warn()
-            perror("Unable to locate OUTDIR='%s'\n"%dname)
+            perror("Unable to locate OUTPUT='%s'\n"%self.outdir)
             status=1
 
         tmp=load_params("%sdefault.param"%pkg_resources.resource_filename("starbug2","param/"))
         if set(tmp.keys()) - set(self.options.keys()):
             warn()
             perror("parameter file version mismatch. Run starbug --update-param to update\n")
             status=1
 
+        if self.options["AP_FILE"] and self.detections is not None:
+            test=self.detections[["xcentroid","ycentroid"]]
+            test=test[ test["xcentroid"]>=0 ]
+            test=test[ test["ycentroid"]>=0 ]
+            test=test[ test["xcentroid"]<self.image.header["NAXIS1"]]
+            test=test[ test["ycentroid"]<self.image.header["NAXIS2"]]
+            if not len(test):
+                warn()
+                perror("Detection file empty or no sources overlap the image.\n")
+                status=1
+
         return status
 
     def __getstate__(self):
+        self._image.close()
+        #if self.background: self.background.close()
         state=self.__dict__.copy()
         if "_image" in state:
             del state["_image"] ##Sorry but we cant have that
+        if "background" in state: ## This currently doesnt get reloaded
+            del state["background"]
+            
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         v=self.options["VERBOSE"]
         self.options["VERBOSE"]=0
         self.load_image(self.fname)
```

### Comparing `starbug2-0.3.9/starbug2/utils.py` & `starbug2-0.4.0/starbug2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                 try:
                     if '.' in value: value=float(value)
                     else: value=int(value)
                 except:
                     pass
 
                 ## Special case values
-                if key in ("AP_FILE","BGD_FILE","PSF_FILE"): value=os.path.expandvars(value)
+                if key in ("OUTPUT", "AP_FILE","BGD_FILE","PSF_FILE"): value=os.path.expandvars(value)
                 config[key]=value
     else:
         perror("config file \"%s\" does not exist\n"%fname)
         config=None
     return config
 
 def tab2array(tab,colnames=None):
```

### Comparing `starbug2-0.3.9/starbug2.egg-info/PKG-INFO` & `starbug2-0.4.0/starbug2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.3.9
+Version: 0.4.0
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
@@ -44,54 +44,52 @@
 ```
 
 Finally verify the installation by running `starbug2 --version`
 
 ## Usage
 
 ```bash
-
 Starbug II - JWST PSF photometry
-usage: starbug2 [-ABCDfhMPv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
+usage: starbug2 [-ABDfGhMPSv] [-b bgdfile] [-d apfile] [-n ncores] [-o directory] [-p file.param] [-s opt=val] image.fits ...
    -A  --apphot          : run aperture photometry on a source list
    -B  --background      : run background estimation
    -b  --bgdfile         : load background (-bgd.fits) file
-   -C  --clean           : run source cleaning before photometry 
    -d  --apfile  ap.fits : load a source detection (-ap.fits) file to skip the source detection step
    -D  --detect          : run source detection
    -f  --find            : attempt to find associated -ap -bgd files
    -G  --geom            : calculate geometric stats on source list
    -h  --help            : display uasage information
    -M  --match           : match outputs from all input image files
    -n  --ncores      num : number of CPU cores to split process between
    -o  --output      dir : output directory
    -p  --param   a.param : load parameter file
-   -P  --photom          : run psf photometry
+   -P  --psf             : run psf photometry
    -s  --set      option : set value in parameter file at runtime (-s SIGSKY=3)
    -S  --subbgd          : subtract background from image
    -v  --verbose         : display verbose outputs
 
    --> Single run commands
        --init                     : Initialise Starbug (post install)
        --local-param              : Make a local copy of the default parameter file
        --update-param             : Update an out-of-date local parameter file
        --generate-psf             : Generate ALL the PSF files to "STARBUG_DATDIR"
        --generate-region   a.fits : Make a ds9 region file with a detection file
        --generate-run      *.fits : Generate a simple run script
        --clean-table       a.fits : Clean up an individual table
        --version                  : Print starbug2 version
 
+       --apply-zeropint    a.fits : Apply a zeropoint (-s ZEROPOINT=1.0) to a.fits
+       --calc-instr-zp     a.fits : Calculate and apply an instrumental zero point onto a.fits
+
    --> typical runs
       $~ starbug2 -vD -p file.param image.fits      //Source detect on image with a parameter file
       $~ starbug2 -vDM -n4 images*.fits             //Source detect and match outputs of a list of images
       $~ starbug2 -vd image-ap.fits -BP image.fits  //PSF photometry on an image with a source file (image-ap.fits)
-
 ```
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
 * MIRI Background masking
-* findpeaks on convl method
-* rickerwavelet radius
 * psf dither match dropping apMag
```

### Comparing `starbug2-0.3.9/tests/test_routines.py` & `starbug2-0.4.0/tests/test_routines.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from starbug2 import routines
 from astropy.table import Table, hstack
 from astropy.io import fits
 from astropy.wcs import WCS
 
-#image=fits.open("tests/dat/image.fits")
+import os
+go=os.path.exists("tests/dat/image.fits")
+if go: image=fits.open("tests/dat/image.fits")
+else: image=None
+
+def test_Detection_Routine_none():
+    dt=routines.Detection_Routine()
+    assert dt.find_stars(None) is None
+
+def test_Detection_Routine_crashes():
+    dt=routines.Detection_Routine()
+    if image:
+        out=dt.find_stars(image["SCI"].data)
+        assert out is not None
+
+def test_BackGround_Estimate_Routine_none():
+    bg=routines.BackGround_Estimate_Routine(None)
+    assert bg(None) is None
 
-#def test_Detection_Routine_none():
-#    dt=routines.Detection_Routine()
-#    assert dt.find_stars(None) is None
-#
-#def test_Detection_Routine_crashes():
-#    dt=routines.Detection_Routine()
-#    out=dt.find_stars(image["SCI"].data)
-#    assert out is not None
-#
-#def test_BackGround_Estimate_Routine_none():
-#    bg=routines.BackGround_Estimate_Routine(None)
-#    assert bg(None) is None
-#
 #def test_BackGround_Estimate_Routine_crashes():
 #    pass
 #
 #
 #
 #
-#def test_SourceProperties_none():
-#    sp=routines.SourceProperties(None,None)
-#    assert sp.calculate_crowding() is None
-#    assert sp.calculate_geometry(1)==None
-#
+def test_SourceProperties_none():
+    sp=routines.SourceProperties(None,None)
+    assert sp.calculate_crowding() is None
+    assert sp.calculate_geometry(1)==None
+
 #def test_SourceProperties_crashes():
 #    ## yeh i know this isnt how youre supposed to test
 #    ## im just verifying it doesnt crash
 #    print("testing crashes")
 #    slist=Table.read("tests/dat/image-ap.fits", format="fits")
 #    sp=routines.SourceProperties(image["SCI"].data, slist[["xcentroid","ycentroid"]])
 #    a=sp(fwhm=2.3)
```

### Comparing `starbug2-0.3.9/tests/test_utils.py` & `starbug2-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

