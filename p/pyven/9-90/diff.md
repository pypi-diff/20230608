# Comparing `tmp/pyven-9.tar.gz` & `tmp/pyven-90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyven-9.tar", last modified: Sun Jan 12 18:18:15 2020, max compression
+gzip compressed data, was "dist/pyven-90.tar", last modified: Thu Jun  8 19:46:51 2023, max compression
```

## Comparing `pyven-9.tar` & `pyven-90.tar`

### file list

```diff
@@ -1,32 +1,53 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-01-12 18:18:15.000000 pyven-9/
--rwxrwxr-x   0 arc       (1000) arc       (1000)     3613 2019-11-03 21:14:06.000000 pyven-9/pyven.py
--rwxrwxr-x   0 arc       (1000) arc       (1000)     3519 2019-11-03 21:14:06.000000 pyven-9/gclean.py
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-01-12 18:18:15.000000 pyven-9/pyven.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-01-12 18:18:15.000000 pyven-9/pyven.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)        8 2020-01-12 18:18:15.000000 pyven-9/pyven.egg-info/requires.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      475 2020-01-12 18:18:15.000000 pyven-9/pyven.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       71 2020-01-12 18:18:15.000000 pyven-9/pyven.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      425 2020-01-12 18:18:15.000000 pyven-9/pyven.egg-info/PKG-INFO
--rw-rw-r--   0 arc       (1000) arc       (1000)      880 2020-01-12 18:18:14.000000 pyven-9/setup.py
--rwxrwxr-x   0 arc       (1000) arc       (1000)     1499 2019-11-03 21:14:06.000000 pyven-9/tasks.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-01-12 18:18:15.000000 pyven-9/setup.cfg
--rwxrwxr-x   0 arc       (1000) arc       (1000)      124 2019-11-03 21:14:06.000000 pyven-9/foreignsyms
--rwxrwxr-x   0 arc       (1000) arc       (1000)     2623 2019-11-03 21:14:06.000000 pyven-9/travis_ci.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      126 2019-11-03 21:14:06.000000 pyven-9/README.md
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-01-12 18:18:15.000000 pyven-9/pyvenimpl/
--rw-rw-r--   0 arc       (1000) arc       (1000)      802 2019-11-03 21:14:06.000000 pyven-9/pyvenimpl/util.py
--rwxrwxr-x   0 arc       (1000) arc       (1000)      980 2019-11-03 21:14:06.000000 pyven-9/pyvenimpl/inpkg.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2580 2019-11-03 21:14:06.000000 pyven-9/pyvenimpl/licheck.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2276 2020-01-12 15:50:53.000000 pyven-9/pyvenimpl/miniconda.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3784 2019-11-03 21:14:06.000000 pyven-9/pyvenimpl/projectinfo.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1284 2019-11-03 21:14:06.000000 pyven-9/pyvenimpl/divcheck.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1056 2019-11-03 21:14:06.000000 pyven-9/pyvenimpl/nlcheck.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     2359 2019-11-03 21:14:06.000000 pyven-9/pyvenimpl/execcheck.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      705 2019-11-25 22:16:59.000000 pyven-9/pyvenimpl/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     4895 2020-01-12 15:50:53.000000 pyven-9/tests.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      425 2020-01-12 18:18:15.000000 pyven-9/PKG-INFO
--rwxrwxr-x   0 arc       (1000) arc       (1000)     1291 2019-11-10 11:04:53.000000 pyven-9/tests
--rwxrwxr-x   0 arc       (1000) arc       (1000)     2718 2019-11-03 21:14:06.000000 pyven-9/release.py
--rwxrwxr-x   0 arc       (1000) arc       (1000)     3613 2019-11-03 21:14:06.000000 pyven-9/pyven
--rwxrwxr-x   0 arc       (1000) arc       (1000)     1291 2019-11-10 11:04:53.000000 pyven-9/runtests.py
--rwxrwxr-x   0 arc       (1000) arc       (1000)      824 2019-11-03 21:14:06.000000 pyven-9/toplevel.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-08 19:46:51.000000 pyven-90/
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-08 19:46:51.000000 pyven-90/pyven.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2023-06-08 19:46:51.000000 pyven-90/pyven.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       80 2023-06-08 19:46:51.000000 pyven-90/pyven.egg-info/requires.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      279 2023-06-08 19:46:51.000000 pyven-90/pyven.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      950 2023-06-08 19:46:51.000000 pyven-90/pyven.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)        6 2023-06-08 19:46:51.000000 pyven-90/pyven.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1794 2023-06-08 19:46:51.000000 pyven-90/pyven.egg-info/PKG-INFO
+-rw-rw-r--   0 arc       (1000) arc       (1000)     6315 2023-06-08 19:46:50.000000 pyven-90/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2023-06-08 19:46:51.000000 pyven-90/setup.cfg
+-rw-rw-r--   0 arc       (1000) arc       (1000)    35147 2019-11-03 21:14:06.000000 pyven-90/COPYING
+-rwxrwxr-x   0 arc       (1000) arc       (1000)      124 2019-11-03 21:14:06.000000 pyven-90/foreignsyms
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1519 2023-03-18 20:46:42.000000 pyven-90/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1794 2023-06-08 19:46:51.000000 pyven-90/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-08 19:46:51.000000 pyven-90/pyven/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1817 2022-10-30 15:25:10.000000 pyven-90/pyven/launch.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3564 2022-10-30 15:25:10.000000 pyven-90/pyven/gclean.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1411 2023-03-19 16:37:34.000000 pyven-90/pyven/projectinfo.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2857 2022-10-30 15:25:10.000000 pyven-90/pyven/util.py
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-08 19:46:51.000000 pyven-90/pyven/setuproot/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1962 2022-10-30 15:25:10.000000 pyven-90/pyven/setuproot/fakesetup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      757 2022-06-13 21:12:55.000000 pyven-90/pyven/setuproot/setuptools.arid
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-08 19:46:51.000000 pyven-90/pyven/setuproot/Cython/
+-rw-rw-r--   0 arc       (1000) arc       (1000)      772 2022-10-30 15:25:10.000000 pyven-90/pyven/setuproot/Cython/Build.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      717 2022-10-30 15:25:10.000000 pyven-90/pyven/setuproot/Cython/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      777 2022-10-30 15:25:10.000000 pyven-90/pyven/setuproot/ez_setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2026 2022-10-30 15:25:10.000000 pyven-90/pyven/setuproot/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       37 2020-05-04 18:35:22.000000 pyven-90/pyven/setup.cfg.aridt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     7010 2023-06-07 21:36:59.000000 pyven-90/pyven/pipify.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2427 2023-03-18 20:46:42.000000 pyven-90/pyven/mainmodules.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2101 2022-12-15 22:15:11.000000 pyven-90/pyven/bdist.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3448 2022-10-30 15:25:10.000000 pyven-90/pyven/licheck.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2531 2022-10-30 15:25:10.000000 pyven-90/pyven/sourceinfo.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     8183 2023-06-07 21:51:20.000000 pyven-90/pyven/projectinfo.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1675 2022-09-27 20:02:12.000000 pyven-90/pyven/setup.py.aridt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       77 2020-05-09 17:11:23.000000 pyven-90/pyven/pyproject.toml.aridt
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1630 2022-10-30 15:25:10.000000 pyven-90/pyven/tasks.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1791 2022-10-30 15:25:10.000000 pyven-90/pyven/cythonize.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1215 2022-10-30 15:25:10.000000 pyven-90/pyven/divcheck.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     9275 2023-03-29 19:49:33.000000 pyven-90/pyven/checks.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1029 2022-10-30 15:25:10.000000 pyven-90/pyven/nlcheck.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1006 2022-10-30 15:25:10.000000 pyven-90/pyven/drmake.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      858 2022-06-13 21:12:55.000000 pyven-90/pyven/release.arid
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1043 2022-10-30 15:25:10.000000 pyven-90/pyven/minreqs.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4120 2022-10-30 15:25:10.000000 pyven-90/pyven/files.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1499 2022-10-30 15:25:10.000000 pyven-90/pyven/execcheck.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     2411 2022-10-30 15:25:10.000000 pyven-90/pyven/tryinstall.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1021 2022-06-13 21:06:55.000000 pyven-90/pyven/README.md.aridt
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2023-06-08 19:46:51.000000 pyven-90/pyven/tests/
+-rw-rw-r--   0 arc       (1000) arc       (1000)      839 2022-10-30 15:25:10.000000 pyven-90/pyven/tests/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     8692 2023-03-29 19:50:09.000000 pyven-90/pyven/release.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      741 2022-10-30 15:25:10.000000 pyven-90/pyven/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1245 2022-10-30 15:25:10.000000 pyven-90/pyven/patchpolicy.py
```

### Comparing `pyven-9/gclean.py` & `pyven-90/pyven/gclean.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python3
-
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,16 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
+'Remove files matching patterns below #glean in .gitignore file.'
+from .util import stderr
 import re, os, sys, shutil
-from pyvenimpl.util import stderr
 
 def removedir(path):
     if os.path.islink(path):
         os.remove(path)
     else:
         shutil.rmtree(path)
```

### Comparing `pyven-9/tasks.py` & `pyven-90/pyven/execcheck.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python3
-
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,28 +11,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-from tests import Files
-import os, subprocess
-
-def isproject():
-    for name in '.hg', '.svn', '.git':
-        if os.path.exists(name):
-            return True
+import os
 
-def main():
-    while not isproject():
-        os.chdir('..')
-    agcommand = ['ag', '--noheading', '--nobreak']
-    paths = list(Files.findfiles('.py', '.pyx', '.h', '.cpp', '.ui', '.java', '.kt', '.c', '.s', '.sh'))
-    ignored = set(subprocess.Popen(['git', 'check-ignore'] + paths, stdout = subprocess.PIPE).communicate()[0].decode().splitlines())
-    paths = [p for p in paths if p not in ignored]
-    for tag in 'XXX', 'TODO', 'FIXME':
-        subprocess.call(agcommand + [tag + ' LATER'] + paths)
-        subprocess.call(agcommand + [tag + '(?! LATER)'] + paths)
+execmask = 0x49
+magic = '#!'
 
-if '__main__' == __name__:
-    main()
+def execcheck(paths):
+    for path in paths:
+        basename = os.path.basename(path)
+        executable = bool(os.stat(path).st_mode & execmask)
+        with open(path) as f:
+            hasmagic = f.readline().startswith(magic)
+        if basename.lower().startswith('test'):
+            if not basename.startswith('test_'):
+                raise Exception("Inconsistent name: %s" % path) # Note pyflakes already checks for duplicate method names.
+            if executable:
+                raise Exception("Should not be executable: %s" % path)
+            if hasmagic:
+                raise Exception("Using %s is obsolete: %s" % (magic, path))
+        else:
+            if executable != hasmagic:
+                raise Exception(path)
```

### Comparing `pyven-9/pyvenimpl/util.py` & `pyven-90/pyven/setuproot/Cython/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,12 +11,7 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-import sys, os
-
-def stderr(obj):
-    sys.stderr.write(str(obj))
-    sys.stderr.write(os.linesep)
```

### Comparing `pyven-9/pyvenimpl/inpkg.py` & `pyven-90/pyven/tests/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env pyven
-
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,19 +11,12 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-import sys
-if '__main__' == __name__:
-    from util import stderr
-else:
-    from .util import stderr
-
-def main():
-    for name in 'path', 'executable', 'argv':
-        stderr("%s: %s" % (name, getattr(sys, name)))
+'Run project unit tests and more, also suitable for CI.'
+from ..checks import main
 
 if '__main__' == __name__:
     main()
```

### Comparing `pyven-9/pyvenimpl/licheck.py` & `pyven-90/pyven/licheck.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,18 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-from __future__ import with_statement
-import re, os, hashlib
+import hashlib, os, re, shlex, sys
 
-template="""# Copyright %(years)s %(author)s
+gpltemplate = """# Copyright %(years)s %(author)s
 
 # This file is part of %(name)s.
 #
 # %(name)s is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -30,37 +29,57 @@
 # %(name)s is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with %(name)s.  If not, see <http://www.gnu.org/licenses/>.
-
-""" # Check it ends with 2 newlines.
-
-def mainimpl(info, paths):
-    master = template % {
-        'years': ', '.join(str(y) for y in info['years']),
-        'author': info['author'],
-        'name': info['name'],
-    }
-    for path in paths:
+"""
+intersection = '''# This file incorporates work covered by the following copyright and
+# permission notice:
+'''
+
+def _hassuffix(name, *suffixes):
+    return name.endswith(suffixes) or name.endswith(tuple("%s.aridt" % s for s in suffixes))
+
+def licheck(info, paths):
+    if not info.config.licheck.enabled:
+        sys.stderr.write('SKIP ')
+        return
+    sections = []
+    for name in info.config.licenses:
+        if sections:
+            sections.append(intersection)
+        if 'GPL' == name:
+            sections.append(gpltemplate % {
+                'years': ', '.join(str(y) for y in info.config.years),
+                'author': info.config.author,
+                'name': info.config.name,
+            })
+        elif 'MIT' == name:
+            with open(info.mitpath()) as f:
+                sections.append(''.join(('# ' if l.rstrip() else '#') + l for l in f))
+        else:
+            raise Exception(name)
+    master = ''.join(s + '\n' for s in sections) # Check each section ends with 2 newlines.
+    def checkone(path):
         with open(path) as f:
             text = f.read()
         if text.startswith('#!'):
             for _ in range(2):
                 text = text[text.index('\n') + 1:]
-        if path.endswith('.s'):
+        if _hassuffix(path, '.s'):
             text = re.sub('^;', '#', text, flags = re.MULTILINE)
-        elif path.endswith('.h') or path.endswith('.cpp') or path.endswith('.cxx'):
+        elif _hassuffix(path, '.h', '.cpp', '.cxx', '.gradle', '.java'):
             text = re.sub('^//', '#', text, flags = re.MULTILINE)
-        elif path.endswith('.arid'):
+        elif _hassuffix(path, '.arid'):
             text = re.sub('^:', '#', text, flags = re.MULTILINE)
-        text = text[:len(master)]
-        if master != text:
-            raise Exception(path)
+        return master == text[:len(master)]
+    badpaths = [p for p in paths if not checkone(p)]
+    if badpaths:
+        raise Exception(' '.join(map(shlex.quote, badpaths)))
     gplpath = os.path.join(info.projectdir, 'COPYING')
     md5 = hashlib.md5()
     with open(gplpath) as f:
         md5.update(f.read().encode('utf_8'))
     if 'd32239bcb673463ab874e80d47fae504' != md5.hexdigest():
         raise Exception(gplpath)
```

### Comparing `pyven-9/pyvenimpl/divcheck.py` & `pyven-90/pyven/divcheck.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,25 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-from __future__ import with_statement
-import re, ast, sys
+import ast, re, sys
 
-def mainimpl(paths):
-    if sys.version_info[0] >= 3:
-        sys.stderr.write('SKIP ')
-        return
-    for path in paths:
+def main():
+    for path in sys.argv[1:]:
         with open(path) as f:
             text = f.read()
         for node in ast.walk(ast.parse(text)):
             if 'Div' == type(node).__name__:
                 hasdiv = True
                 break
         else:
             hasdiv = False
         if hasdiv == (re.search('^from __future__ import division(?: # .+)?$', text, flags = re.MULTILINE) is None):
             raise Exception(path)
+
+if ('__main__' == __name__):
+    main()
```

### Comparing `pyven-9/pyvenimpl/nlcheck.py` & `pyven-90/pyven/nlcheck.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,19 +11,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-from __future__ import with_statement
 import re
 
 class MoreThanOneEolStyleException(Exception): pass
 
-def mainimpl(paths):
+def nlcheck(paths):
     for path in paths:
         with open(path, 'rb') as f:
             text = f.read().decode()
         eols = set(re.findall(r'\r\n|[\r\n]', text))
         if len(eols) > 1:
             raise MoreThanOneEolStyleException(path)
```

### Comparing `pyven-9/pyvenimpl/__init__.py` & `pyven-90/pyven/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,7 +11,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
+targetremote = 'origin'
```

### Comparing `pyven-9/tests.py` & `pyven-90/pyven/files.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,116 +11,76 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-from __future__ import with_statement
-from pyvenimpl import licheck as licheckimpl, nlcheck as nlcheckimpl, divcheck as divcheckimpl, execcheck as execcheckimpl, projectinfo
-from pyvenimpl.util import stderr
-import subprocess, sys, os, re, xml.dom.minidom as dom, collections
-
-def stripeol(line):
-    line, = line.splitlines()
-    return line
+from .util import stripeol
+from collections import defaultdict
+import os, subprocess, xml.dom.minidom as dom
 
 class Files:
 
-    reportpath = 'nosetests.xml'
-
     @staticmethod
-    def findfiles(*suffixes):
-        walkpath = '.'
+    def _findfiles(walkpath, suffixes, prefixes):
+        def acceptname():
+            for suffix in suffixes:
+                if name.endswith(suffix):
+                    return True
+            for prefix in prefixes:
+                if name.startswith(prefix):
+                    return True
         prefixlen = len(walkpath + os.sep)
         for dirpath, dirnames, filenames in os.walk(walkpath):
             for name in sorted(filenames):
-                for suffix in suffixes:
-                    if name.endswith(suffix):
-                        yield os.path.join(dirpath, name)[prefixlen:]
-                        break # Next name.
+                if acceptname():
+                    yield os.path.join(dirpath, name)[prefixlen:]
             dirnames.sort()
 
     @classmethod
-    def filterfiles(cls, *suffixes):
-        paths = list(cls.findfiles(*suffixes))
-        if os.path.exists('.hg'):
-            badstatuses = set('IR ')
-            for line in subprocess.Popen(['hg', 'st', '-A'] + paths, stdout = subprocess.PIPE).stdout:
-                line = stripeol(line).decode()
-                if line[0] not in badstatuses:
-                    yield line[2:]
-        else:
-            ignored = set(subprocess.Popen(['git', 'check-ignore'] + paths, stdout = subprocess.PIPE).communicate()[0].decode().splitlines())
-            for path in paths:
-                if path not in ignored:
-                    yield path
-
-    def __init__(self):
-        self.allsrcpaths = list(p for p in self.filterfiles('.py', '.py3', '.pyx', '.s', '.sh', '.h', '.cpp', '.cxx', '.arid'))
+    def relpaths(cls, root, suffixes, prefixes):
+        paths = list(cls._findfiles(root, suffixes, prefixes))
+        with open(os.devnull) as devnull:
+            if not subprocess.call(['hg', 'root'], stdout = devnull, stderr = devnull, cwd = root):
+                badstatuses = set('IR ')
+                for line in subprocess.Popen(['hg', 'st', '-A'] + paths, stdout = subprocess.PIPE, cwd = root).stdout:
+                    line = stripeol(line).decode()
+                    if line[0] not in badstatuses:
+                        yield line[2:]
+            else:
+                if os.path.exists(os.path.join(root, '.gitmodules')):
+                    for submoduleslash in (l.split(' ', 1)[1] + os.sep for l in subprocess.check_output(['git', 'config', '--file', '.gitmodules', '--get-regexp', '^submodule[.].+[.]path$'], cwd = root).decode().splitlines()):
+                        paths = [p for p in paths if not p.startswith(submoduleslash)]
+                if paths:
+                    p = subprocess.Popen(['git', 'check-ignore'] + paths, stdout = subprocess.PIPE, cwd = root)
+                    ignored = set(p.communicate()[0].decode().splitlines())
+                    assert p.wait() in [0, 1]
+                    for path in paths:
+                        if path not in ignored:
+                            yield path
+
+    def __init__(self, root):
+        srcsuffixes = sum(([s, "%s.aridt" % s] for s in ['.py', '.py3', '.pyx', '.s', '.sh', '.h', '.cpp', '.cxx', '.arid', '.gradle', '.java', '.mk']), [])
+        self.allsrcpaths = [os.path.join(root, p) for p in self.relpaths(root, srcsuffixes, ['Dockerfile', 'Makefile'])]
         self.pypaths = [p for p in self.allsrcpaths if p.endswith('.py')]
+        self.root = root
 
-    def testpaths(self):
+    def testpaths(self, reportpath):
         paths = [p for p in self.pypaths if os.path.basename(p).startswith('test_')]
-        if os.path.exists(self.reportpath):
-            with open(self.reportpath) as f:
+        if os.path.exists(reportpath):
+            with open(reportpath) as f:
                 doc = dom.parse(f)
-            nametopath = dict([p[:-len('.py')].replace(os.sep, '.'), p] for p in paths)
-            pathtotime = collections.defaultdict(lambda: 0)
+            nametopath = dict([p[len(self.root + os.sep):-len('.py')].replace(os.sep, '.'), p] for p in paths)
+            pathtotime = defaultdict(int)
             for e in doc.getElementsByTagName('testcase'):
                 name = e.getAttribute('classname')
                 while True:
                     i = name.rfind('.')
                     if -1 == i:
                         break
                     name = name[:i]
                     if name in nametopath:
                         pathtotime[nametopath[name]] += float(e.getAttribute('time'))
                         break
             paths.sort(key = lambda p: pathtotime.get(p, float('inf')))
         return paths
-
-def licheck(info, files):
-    def g():
-        for path in files.allsrcpaths:
-            parentname = os.path.basename(os.path.dirname(path))
-            if parentname != 'contrib' and not parentname.endswith('_turbo'):
-                yield path
-    licheckimpl.mainimpl(info, list(g()))
-
-def nlcheck(info, files):
-    nlcheckimpl.mainimpl(files.allsrcpaths)
-
-def divcheck(info, files):
-    divcheckimpl.mainimpl(files.pypaths)
-
-def execcheck(info, files):
-    execcheckimpl.mainimpl(files.pypaths)
-
-def pyflakes(info, files):
-    with open('.flakesignore') as f:
-        ignores = [re.compile(stripeol(l)) for l in f]
-    def accept(path):
-        for pattern in ignores:
-            if pattern.search(path) is not None:
-                return False
-        return True
-    paths = [p for p in files.pypaths if accept(p)]
-    if paths:
-        subprocess.check_call([pathto('pyflakes')] + paths)
-
-def pathto(executable):
-    return os.path.join(os.path.dirname(sys.executable), executable)
-
-def main():
-    while not (os.path.exists('.hg') or os.path.exists('.svn') or os.path.exists('.git')):
-        os.chdir('..')
-    info = projectinfo.ProjectInfo(os.getcwd())
-    files = Files()
-    for check in (() if info['proprietary'] else (licheck,)) + (nlcheck, divcheck, execcheck, pyflakes):
-        sys.stderr.write("%s: " % check.__name__)
-        check(info, files)
-        stderr('OK')
-    sys.exit(subprocess.call([pathto('nosetests'), '--exe', '-v', '--with-xunit'] + files.testpaths() + sys.argv[1:]))
-
-if '__main__' == __name__:
-    main()
```

### Comparing `pyven-9/tests` & `pyven-90/pyven/minreqs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python3
-
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,22 +11,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-from pyvenimpl import projectinfo, miniconda as mc
-import os, pyven, tests, sys
+'Print project.arid snippet pinning requires to their minimum allowed versions.'
+from .projectinfo import ProjectInfo
+from venvpool import initlogging
 
 def main():
-    info = projectinfo.ProjectInfo(os.getcwd())
-    minicondas = [mc.pyversiontominiconda[v] for v in info['pyversions']]
-    testspath = tests.__file__
-    if testspath.endswith('.pyc'):
-        testspath = testspath[:-1]
-    for miniconda in minicondas:
-        # Equivalent to running tests.py directly but with one fewer process launch:
-        pyven.Launcher(info, miniconda.pyversion).check_call([testspath] + sys.argv[1:])
+    initlogging()
+    print("requires = $list(%s)" % ' '.join(r.minstr() for r in ProjectInfo.seek('.').parsedrequires()))
 
 if '__main__' == __name__:
     main()
```

### Comparing `pyven-9/runtests.py` & `pyven-90/pyven/drmake.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python3
-
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+# Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
 # This file is part of pyven.
 #
 # pyven is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,22 +11,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-from pyvenimpl import projectinfo, miniconda as mc
-import os, pyven, tests, sys
+'Build a Docker image with automatic tag.'
+from .projectinfo import ProjectInfo
+import os
 
 def main():
-    info = projectinfo.ProjectInfo(os.getcwd())
-    minicondas = [mc.pyversiontominiconda[v] for v in info['pyversions']]
-    testspath = tests.__file__
-    if testspath.endswith('.pyc'):
-        testspath = testspath[:-1]
-    for miniconda in minicondas:
-        # Equivalent to running tests.py directly but with one fewer process launch:
-        pyven.Launcher(info, miniconda.pyversion).check_call([testspath] + sys.argv[1:])
+    info = ProjectInfo.seek('.')
+    command = 'docker', 'build', '-t', info.config.docker.tag, info.projectdir
+    os.execvp(command[0], command)
 
 if '__main__' == __name__:
     main()
```

### Comparing `pyven-9/toplevel.py` & `pyven-90/pyven/setuproot/setuptools.arid`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-#!/usr/bin/env pyven
+: Copyright 2013, 2014, 2015, 2016, 2017, 2020, 2022 Andrzej Cichocki
 
-# Copyright 2013, 2014, 2015, 2016, 2017 Andrzej Cichocki
+: This file is part of pyven.
+:
+: pyven is free software: you can redistribute it and/or modify
+: it under the terms of the GNU General Public License as published by
+: the Free Software Foundation, either version 3 of the License, or
+: (at your option) any later version.
+:
+: pyven is distributed in the hope that it will be useful,
+: but WITHOUT ANY WARRANTY; without even the implied warranty of
+: MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+: GNU General Public License for more details.
+:
+: You should have received a copy of the GNU General Public License
+: along with pyven.  If not, see <http://www.gnu.org/licenses/>.
 
-# This file is part of pyven.
-#
-# pyven is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# pyven is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with pyven.  If not, see <http://www.gnu.org/licenses/>.
-
-from pyvenimpl import inpkg
-
-def main():
-    inpkg.main()
-
-if '__main__' == __name__:
-    main()
+licheck enabled = false
+pyversions += 3
```

