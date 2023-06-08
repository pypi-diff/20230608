# Comparing `tmp/vignette-5.0.0.tar.gz` & `tmp/vignette-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vignette-5.0.0.tar", last modified: Sat Sep 11 21:44:42 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `vignette-5.0.0.tar` & `vignette-5.1.0.tar`

### file list

```diff
@@ -1,20 +1,8 @@
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-09-11 21:44:42.193865 vignette-5.0.0/
--rw-r--r--   0 ntome     (1000) ntome     (1000)       53 2021-09-11 21:20:45.000000 vignette-5.0.0/MANIFEST.in
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2376 2021-09-11 21:44:42.193865 vignette-5.0.0/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)     4567 2021-09-11 21:20:45.000000 vignette-5.0.0/README.rst
--rw-r--r--   0 ntome     (1000) ntome     (1000)        6 2021-09-11 21:20:45.000000 vignette-5.0.0/VERSION.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1271 2021-09-11 21:44:42.193865 vignette-5.0.0/setup.cfg
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)      136 2021-09-11 21:20:45.000000 vignette-5.0.0/setup.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-09-11 21:44:42.193865 vignette-5.0.0/tools/
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)     1349 2021-09-11 21:20:45.000000 vignette-5.0.0/tools/thumbnails_lint.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-09-11 21:44:42.193865 vignette-5.0.0/vignette/
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)    32686 2021-09-11 21:20:45.000000 vignette-5.0.0/vignette/__init__.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)       27 2021-09-11 21:20:45.000000 vignette-5.0.0/vignette/__main__.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-09-11 21:44:42.193865 vignette-5.0.0/vignette.egg-info/
--rw-r--r--   0 ntome     (1000) ntome     (1000)     2376 2021-09-11 21:44:42.000000 vignette-5.0.0/vignette.egg-info/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      341 2021-09-11 21:44:42.000000 vignette-5.0.0/vignette.egg-info/SOURCES.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2021-09-11 21:44:42.000000 vignette-5.0.0/vignette.egg-info/dependency_links.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       44 2021-09-11 21:44:42.000000 vignette-5.0.0/vignette.egg-info/entry_points.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       59 2021-09-11 21:44:42.000000 vignette-5.0.0/vignette.egg-info/requires.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        9 2021-09-11 21:44:42.000000 vignette-5.0.0/vignette.egg-info/top_level.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2021-09-11 21:21:06.000000 vignette-5.0.0/vignette.egg-info/zip-safe
+-rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 vignette-5.1.0/README.rst
+-rwxr-xr-x   0        0        0    35291 2020-02-02 00:00:00.000000 vignette-5.1.0/vignette/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 vignette-5.1.0/vignette/__main__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 vignette-5.1.0/.gitignore
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 vignette-5.1.0/COPYING.WTFPL
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 vignette-5.1.0/description.txt
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 vignette-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 vignette-5.1.0/PKG-INFO
```

### Comparing `vignette-5.0.0/PKG-INFO` & `vignette-5.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 Metadata-Version: 2.1
 Name: vignette
-Version: 5.0.0
+Version: 5.1.0
 Summary: Library to create FreeDesktop-compatible thumbnails
-Home-page: https://github.com/hydrargyrum/vignette
-Author: Hg
-Author-email: dev@indigo.re
-License: WTFPLv2
-Description: Vignette is a library to create and manage thumbnails following the FreeDesktop standard.
-        
-        Thumbnails are stored in a shared directory so other apps following the standard can reuse
-        them without having to generate their own thumbnails.
-        
-        Vignette can typically be used in file managers, image browsers, etc.
-        
-        Thumbnails are not limited to image files on disk but can be generated for other file types,
-        for example videos or documents but also for any URL, for example a web browser could store
-        thumbnails for recently visited pages or bookmarks.
-        
-        Vignette by itself can only generate thumbnails for local files but can retrieve
-        thumbnail for any file or URL, if another app generated a thumbnail for it. An app can also
-        generate a thumbnail by its own means and use vignette to push that thumbnail to the store.
-        
-        Vignette has optional support for extra backends like ffmpegthumbnailer, poppler-utils,
-        ooo-thumbnailer, and more, if these tools are installed.
-        
-        The range of files for which vignette can generate thumbnails depends on plugins
-        as it supports third-party libraries and tools. For example, if the
-        evince-thumbnailer command is installed, it will be able to generate thumbnails
-        for PDF files.
-        
-Keywords: freedesktop,xdg,image,thumbnail,thumbnails,cache
-Platform: UNKNOWN
+Project-URL: Homepage, https://gitlab.com/hydrargyrum/vignette
+Project-URL: Documentation, https://vignette.readthedocs.io/
+Author-email: Hg <dev@indigo.re>
+License-Expression: WTFPL
+License-File: COPYING.WTFPL
+Keywords: cache,freedesktop,image,thumbnail,thumbnails,xdg
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
-Classifier: Topic :: Desktop Environment
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Desktop Environment
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6
+Requires-Dist: python-magic
 Provides-Extra: pillow
+Requires-Dist: pillow; extra == 'pillow'
+Provides-Extra: pyqt6
+Requires-Dist: pyqt6; extra == 'pyqt6'
 Provides-Extra: pythonmagick
+Requires-Dist: pythonmagick; extra == 'pythonmagick'
+Description-Content-Type: text/plain
+
+Vignette is a library to create and manage thumbnails following the FreeDesktop standard.
+
+Thumbnails are stored in a shared directory so other apps following the standard can reuse
+them without having to generate their own thumbnails.
+
+Vignette can typically be used in file managers, image browsers, etc.
+
+Thumbnails are not limited to image files on disk but can be generated for other file types,
+for example videos or documents but also for any URL, for example a web browser could store
+thumbnails for recently visited pages or bookmarks.
+
+Vignette by itself can only generate thumbnails for local files but can retrieve
+thumbnail for any file or URL, if another app generated a thumbnail for it. An app can also
+generate a thumbnail by its own means and use vignette to push that thumbnail to the store.
+
+Vignette has optional support for extra backends like ffmpegthumbnailer, poppler-utils,
+ooo-thumbnailer, and more, if these tools are installed.
+
+The range of files for which vignette can generate thumbnails depends on plugins
+as it supports third-party libraries and tools. For example, if the
+evince-thumbnailer command is installed, it will be able to generate thumbnails
+for PDF files.
```

### Comparing `vignette-5.0.0/README.rst` & `vignette-5.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
   local_app_display(thumb_image)
 
 
 Ask for a thumbnail or generate it manually, for example a web-browser generating pages previews, that this module can't do itself::
 
   import vignette
 
-  orig_url = 'http://example.com/file.pdf'
+  orig_url = 'https://example.com/file.pdf'
   thumb_image = vignette.try_get_thumbnail(orig_url, mtime=0) # mtime is not used in this example
 
   if not thumb_image:
     thumb_image = vignette.build_thumbnail_path(orig_url, 'large')
     try:
       local_app_make_preview(orig_url, thumb_image)
     except NetworkError:
@@ -125,8 +125,8 @@
 Vignette is licensed under the `WTFPLv2 <http://wtfpl.net>`_.
 
 Version
 =======
 
 .. $version
 
-Vignette is currently at version 5.0.0 and uses `Semantic Versioning <http://semver.org/>`_.
+Vignette is currently at version 5.1.0 and uses `Semantic Versioning <https://semver.org/>`_.
```

### Comparing `vignette-5.0.0/vignette/__init__.py` & `vignette-5.1.0/vignette/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,15 +129,15 @@
   local_app_display(thumb_image)
 
 Ask for a thumbnail or generate it manually, for example a web-browser generating pages previews,
 that this module can't do itself::
 
   import vignette
 
-  orig_url = 'http://example.com/file.pdf'
+  orig_url = 'https://example.com/file.pdf'
   thumb_image = vignette.try_get_thumbnail(orig_url, mtime=0) # mtime is not used in this example
 
   if not thumb_image:
     thumb_image = vignette.create_temp('large')
     try:
       local_app_make_preview(orig_url, thumb_image)
     except NetworkError:
@@ -157,14 +157,15 @@
 
 """
 
 from __future__ import unicode_literals
 
 from glob import glob
 import hashlib
+import logging
 import mimetypes
 import os
 import re
 import shlex
 import shutil
 import subprocess
 import sys
@@ -235,21 +236,24 @@
 """Optional thumbnail metadata key for software creating the thumbnail.
 
 If not set, appname for fail-files will be used.
 If this too is unset, "vignette-{version}" is used.
 """
 
 
-VERSION = '5.0.0'  # $version
+VERSION = '5.1.0'  # $version
 
 """Version of the vignette library."""
 
 __version__ = VERSION
 
 
+LOGGER = logging.getLogger("vignette")
+
+
 def _any2size(size):
 	if size in ('normal', 128, '128'):
 		return (128, 'normal')
 	elif size in ('large', 256, '256'):
 		return (256, 'large')
 	elif size in ('x-large', 512, '512'):
 		return (512, 'x-large')
@@ -438,14 +442,15 @@
 	else:
 		# thumb in any other dir
 		tmp = _mkstemp(dest)
 		shutil.move(thumb, tmp)
 
 	moreinfo = _info_dict(moreinfo, mtime=mtime, src=src)
 	if not get_metadata_backend().update_metadata(tmp, moreinfo):
+		LOGGER.error("backend could not update metadata for %s", tmp)
 		return
 
 	os.chmod(tmp, 0o600)
 	os.rename(tmp, dest)
 
 	return dest
 
@@ -564,25 +569,21 @@
 				outinfo.add_text(k, str(moreinfo[k]))
 
 		return outinfo
 
 	def create_thumbnail(self, src, dest, size):
 		import PIL.ImageOps
 
-		try:
-			img = self.mod.open(src)
-		except IOError:
-			return None
-
+		img = self.mod.open(src)
 		img = PIL.ImageOps.exif_transpose(img)
 
 		mtime = _any2mtime(src)
 
 		original_size = img.size
-		img.thumbnail((size, size), self.mod.ANTIALIAS)
+		img.thumbnail((size, size), self.mod.LANCZOS)
 
 		img.save(dest)
 		img.close()
 		return {
 			KEY_MTIME: mtime,
 			KEY_WIDTH: str(original_size[0]),
 			KEY_HEIGHT: str(original_size[1]),
@@ -677,18 +678,15 @@
 			return
 
 		img.rotate(cls.orientation_rotate.get(orientation, 0))
 		if orientation in cls.should_flop:
 			img.flop()
 
 	def create_thumbnail(self, src, dest, size):
-		try:
-			img = self.mod.Image(self.encode(src))
-		except RuntimeError:
-			return
+		img = self.mod.Image(self.encode(src))
 
 		original_geom = img.size()
 		mtime = _any2mtime(src)
 
 		self.reorient_image(img)
 		if original_geom.width() > size or original_geom.height() > size:
 			geom = self.mod.Geometry(size, size)
@@ -751,34 +749,28 @@
 	handled_types = frozenset([FILETYPE_DOCUMENT])
 	accepted_mimes = re.compile('^application/pdf$')
 	cmd = 'pdftocairo'
 
 	def create_thumbnail(self, src, dest, size):
 		prefix, _ = os.path.splitext(dest)
 		args = [self.cmd, '-png', '-singlefile', '-scale-to', str(size), src, prefix]
-		try:
-			subprocess.check_call(args)
-		except subprocess.CalledProcessError:
-			return
+		subprocess.check_call(args)
 		return {}
 
 
 class OooCliBackend(CliMixin, ThumbnailBackend):
 	handled_types = frozenset([FILETYPE_DOCUMENT])
 	accepted_mimes = re.compile('^application/vnd.oasis.opendocument.')
 	cmd = 'ooo-thumbnailer'
 
 	def create_thumbnail(self, src, dest, size):
 		args = [self.cmd, src, dest, str(size)]
-		try:
-			subprocess.check_call(args)
-		except subprocess.CalledProcessError:
-			return
+		subprocess.check_call(args)
 		if not (os.path.exists(dest) and os.path.getsize(dest)):
-			return
+			raise Exception("empty or non-existing output thumbnail")
 		return {}
 
 
 class EvinceCliBackend(CliMixin, ThumbnailBackend):
 	accepted_mimes = re.compile(
 		'^application/pdf|'
 		'image/vnd.djvu|'
@@ -786,68 +778,56 @@
 		'application/x-dvi$'
 	)
 	handled_types = frozenset([FILETYPE_DOCUMENT])
 	cmd = 'evince-thumbnailer'
 
 	def create_thumbnail(self, src, dest, size):
 		args = [self.cmd, '-s', str(size), src, dest]
-		try:
-			subprocess.check_call(args)
-		except subprocess.CalledProcessError:
-			return
+		subprocess.check_call(args)
 		if not (os.path.exists(dest) and os.path.getsize(dest)):
-			return
+			raise Exception("empty or non-existing output thumbnail")
 		return {}
 
 
 class AtrilCliBackend(EvinceCliBackend):
 	cmd = 'atril-thumbnailer'
 
 
 class ExeCliBackend(CliMixin, ThumbnailBackend):
 	handled_types = frozenset([FILETYPE_MISC])
 	accepted_mimes = re.compile('^application/x-dosexec|application/x-msi$')
 	cmd = 'exe-thumbnailer'
 
 	def create_thumbnail(self, src, dest, size):
 		args = [self.cmd, src, dest, 'this://is.invalid']
-		try:
-			subprocess.check_call(args)
-		except subprocess.CalledProcessError:
-			return
+		subprocess.check_call(args)
 		if not (os.path.exists(dest) and os.path.getsize(dest)):
-			return
+			raise Exception("empty or non-existing output thumbnail")
 		return {}
 
 
 class OggThumbCliBackend(CliMixin, ThumbnailBackend):
 	accepted_mimes = re.compile('^video/ogg$')
 	handled_types = frozenset([FILETYPE_VIDEO])
 	cmd = 'oggThumb'
 
 	def create_thumbnail(self, src, dest, size):
-		try:
-			len_ms = int(subprocess.check_output(['oggLength', src]).strip())
-		except subprocess.CalledProcessError:
-			return
+		len_ms = int(subprocess.check_output(['oggLength', src]).strip())
 
 		args = [
 			self.cmd,
 			'-o', 'png',
 			'-n', dest,
 			'-t', str(len_ms / 10000), # 10% of the file, in secs
 			'-s', '%{0}x%{0}'.format(size),
 			src,
 		]
-		try:
-			subprocess.check_call(args)
-		except subprocess.CalledProcessError:
-			return
+		subprocess.check_call(args)
 		if not (os.path.exists(dest) and os.path.getsize(dest)):
-			return
+			raise Exception("empty or non-existing output thumbnail")
 		return {
 			KEY_MOVIE_LENGTH: str(len_ms) / 1000,
 		}
 
 
 class QtBackend(MetadataBackend, ThumbnailBackend):
 	handled_types = frozenset([FILETYPE_IMAGE])
@@ -880,15 +860,15 @@
 		from PyQt5.QtCore import Qt
 		from PyQt5.QtGui import QImageReader
 
 		img_reader = QImageReader(str(src))
 		img_reader.setAutoTransform(True)
 		img = img_reader.read()
 		if img.isNull():
-			return
+			raise Exception("could not read image: %s" % img_reader.errorString())
 
 		res = {
 			KEY_MTIME: _any2mtime(src),
 			KEY_WIDTH: img.width(),
 			KEY_HEIGHT: img.height(),
 		}
 
@@ -935,14 +915,104 @@
 				'mtime': int(float(img.text(KEY_MTIME) or 0)),
 				'uri': img.text(KEY_URI),
 			}
 		except ValueError:
 			return
 
 
+class Qt6Backend(MetadataBackend, ThumbnailBackend):
+	handled_types = frozenset([FILETYPE_IMAGE])
+	_accepted_mimes = None
+
+	@classmethod
+	def is_available(cls):
+		try:
+			from PyQt6.QtGui import QImageReader
+		except (ImportError, RuntimeError):
+			return False
+		return True
+
+	@property
+	def accepted_mimes(self):
+		if self._accepted_mimes is None:
+			from PyQt6.QtGui import QImageReader
+
+			mimes = [bytes(ba).decode('ascii') for ba in QImageReader.supportedMimeTypes()]
+			self._accepted_mimes = re.compile('^(?:%s)$' % '|'.join(map(re.escape, mimes)))
+
+		return self._accepted_mimes
+
+	@staticmethod
+	def setattributes(img, moreinfo):
+		for k in moreinfo or {}:
+			img.setText(k, moreinfo[k])
+
+	def create_thumbnail(self, src, dest, size):
+		from PyQt6.QtCore import Qt
+		from PyQt6.QtGui import QImageReader
+
+		img_reader = QImageReader(str(src))
+		img_reader.setAutoTransform(True)
+		img = img_reader.read()
+		if img.isNull():
+			raise Exception("could not read image: %s" % img_reader.errorString())
+
+		res = {
+			KEY_MTIME: _any2mtime(src),
+			KEY_WIDTH: img.width(),
+			KEY_HEIGHT: img.height(),
+		}
+
+		if img.width() > size or img.height() > size:
+			img = img.scaled(size, size, Qt.AspectRatioMode.KeepAspectRatio, Qt.TransformationMode.SmoothTransformation)
+
+		img.save(dest)
+		return res
+
+	def update_metadata(self, dest, moreinfo=None):
+		from PyQt6.QtGui import QImage
+
+		img = QImage(dest)
+		if img.isNull():
+			return
+
+		self.setattributes(img, moreinfo)
+
+		tmp = _mkstemp(dest)
+		img.save(tmp)
+		os.rename(tmp, dest)
+		return dest
+
+	def create_fail(self, dest, moreinfo=None):
+		from PyQt6.QtGui import QImage
+
+		img = QImage(1, 1, QImage.Format.Format_RGB32)
+		self.setattributes(img, moreinfo)
+
+		tmp = _mkstemp(dest)
+		img.save(tmp)
+		os.rename(tmp, dest)
+		return dest
+
+	def get_info(self, path):
+		from PyQt6.QtGui import QImage
+
+		img = QImage(path)
+		if img.isNull():
+			return
+
+		try:
+			return {
+				'mtime': int(float(img.text(KEY_MTIME) or 0)),
+				'uri': img.text(KEY_URI),
+			}
+		except ValueError:
+			return
+
+
 class GnomeThumbnailer(CliMixin, ThumbnailBackend):
 	mime_to_handle = {
 		re.compile('^image/'): FILETYPE_IMAGE,
 		re.compile('^video/'): FILETYPE_VIDEO,
 		re.compile('^application/pdf'): FILETYPE_DOCUMENT,
 		re.compile('^application/vnd.oasis.opendocument.'): FILETYPE_DOCUMENT,
 		re.compile('^application/vnd.openxmlformats-officedocument.'): FILETYPE_DOCUMENT,
@@ -970,20 +1040,17 @@
 		vars = {
 			'i': src,
 			'o': dest,
 			'u': _any2uri(src),
 			's': str(size),
 		}
 		args = [arg % vars for arg in self.cmd_exec]
-		try:
-			subprocess.check_call(args)
-		except subprocess.CalledProcessError:
-			return
+		subprocess.check_call(args)
 		if not (os.path.exists(dest) and os.path.getsize(dest)):
-			return
+			raise Exception("empty or non-existing output thumbnail")
 		return {}
 
 
 GNOME_THUMBNAILERS_PATH = '/usr/share/thumbnailers/*.thumbnailer'
 
 
 def build_gnome_thumbnailers():
@@ -999,22 +1066,29 @@
 			cmd_test = None
 		cmd_exec = cfg.get(section, 'Exec')
 		mimes = [m for m in cfg.get(section, 'MimeType').split(';') if m]
 		backend = GnomeThumbnailer(cmd_test, cmd_exec, mimes)
 		yield backend
 
 
-METADATA_BACKENDS = [QtBackend(), PilBackend(), MagickBackend()]
+_QT_BACKENDS = {6: Qt6Backend(), 5: QtBackend()}
+_QT_PREFERRED = (
+	_QT_BACKENDS[6]
+	if (_QT_BACKENDS[6].is_available() or not _QT_BACKENDS[5].is_available())
+	else _QT_BACKENDS[5]
+)
+
+METADATA_BACKENDS = [_QT_PREFERRED, PilBackend(), MagickBackend()]
 
 ALL_THUMBNAILER_BACKENDS = [
 	OooCliBackend(),
 	PopplerCliBackend(),
 	EvinceCliBackend(),
 	AtrilCliBackend(),
-	QtBackend(),
+	_QT_PREFERRED,
 	PilBackend(),
 	MagickBackend()
 ]
 
 ALL_THUMBNAILER_BACKENDS.extend(build_gnome_thumbnailers())
 
 THUMBNAILER_BACKENDS = list(ALL_THUMBNAILER_BACKENDS)
@@ -1056,29 +1130,40 @@
 	"""
 
 	size = _any2size(size)[0]
 	tmp = create_temp(size)
 
 	for backend in iter_thumbnail_backends():
 		if FILTER_MIMETYPES and not backend.is_accepted(src):
+			LOGGER.debug("backend %r does not accept %r", backend, src)
 			continue
 
-		backend_moreinfo = backend.create_thumbnail(src, tmp, size)
-		if backend_moreinfo is not None:
+		try:
+			backend_moreinfo = backend.create_thumbnail(src, tmp, size)
+		except Exception:
+			LOGGER.warning(
+				"backend %r failed to create a thumbnail of %r", backend, src, exc_info=True,
+			)
+			continue
+
+		if backend_moreinfo is None:
+			LOGGER.warning("backend %r could not create a thumbnail of %r", backend, src)
+		else:
 			moreinfo = dict(moreinfo or (), **backend_moreinfo)
 
 			if use_fail_appname is not None:
 				moreinfo.setdefault(KEY_SOFTWARE, use_fail_appname)
 			moreinfo = _info_dict(moreinfo, src=src)
 			mtime = moreinfo[KEY_MTIME]
 
 			dest = put_thumbnail(src, size, tmp, mtime=mtime, moreinfo=moreinfo)
 			if dest:
 				return dest
 
+	LOGGER.warning("no backend could create a thumbnail of %r", src)
 	if use_fail_appname is not None:
 		put_fail(src, use_fail_appname)
 
 
 def build_thumbnail_path(src, size):
 	"""Get the path of the potential thumbnail.
 
@@ -1175,14 +1260,15 @@
 	if use_fail_appname is not None:
 		mtime = _any2mtime(src)
 		if is_thumbnail_failed(src, use_fail_appname, mtime):
 			return None
 
 	if size is None:
 		size = 'large'
+	LOGGER.debug("no existing thumbnail for %r, creating one", src)
 	return create_thumbnail(src, size, use_fail_appname=use_fail_appname)
 
 
 def thumbnail_info(thumbnail):
 	return get_metadata_backend().get_info(thumbnail)
```

