# Comparing `tmp/timona-0.0.4.tar.gz` & `tmp/timona-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timona-0.0.4.tar", max compression
+gzip compressed data, was "timona-0.0.5.tar", max compression
```

## Comparing `timona-0.0.4.tar` & `timona-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.4/LICENSE
--rw-r--r--   0        0        0      104 2023-05-30 12:02:34.562872 timona-0.0.4/README.md
--rw-r--r--   0        0        0      542 2023-05-31 06:58:01.033207 timona-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.4/timona/__init__.py
--rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.4/timona/__main__.py
--rw-r--r--   0        0        0       38 2023-05-31 06:58:01.033207 timona-0.0.4/timona/__version__.py
--rw-r--r--   0        0        0     1228 2023-05-30 14:40:01.114338 timona-0.0.4/timona/config.py
--rw-r--r--   0        0        0     2715 2023-05-30 12:27:04.454612 timona-0.0.4/timona/helm.py
--rw-r--r--   0        0        0     2771 2023-05-30 14:15:58.083494 timona-0.0.4/timona/main.py
--rw-r--r--   0        0        0     5236 2023-05-30 14:50:19.327125 timona-0.0.4/timona/releases.py
--rw-r--r--   0        0        0     2463 2023-05-30 14:56:57.258194 timona-0.0.4/timona/template/__init__.py
--rw-r--r--   0        0        0      201 2023-05-30 14:57:24.210402 timona-0.0.4/timona/template/module_jinja2.py
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 timona-0.0.4/setup.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 timona-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.5/LICENSE
+-rw-r--r--   0        0        0      104 2023-05-30 12:02:34.562872 timona-0.0.5/README.md
+-rw-r--r--   0        0        0      542 2023-06-08 07:15:04.719193 timona-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.5/timona/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.5/timona/__main__.py
+-rw-r--r--   0        0        0       38 2023-06-08 07:15:04.719193 timona-0.0.5/timona/__version__.py
+-rw-r--r--   0        0        0     1228 2023-05-30 14:40:01.114338 timona-0.0.5/timona/config.py
+-rw-r--r--   0        0        0     2715 2023-05-31 07:56:35.415665 timona-0.0.5/timona/helm.py
+-rw-r--r--   0        0        0     2730 2023-05-31 09:39:19.195374 timona-0.0.5/timona/main.py
+-rw-r--r--   0        0        0     5236 2023-05-30 14:50:19.327125 timona-0.0.5/timona/releases.py
+-rw-r--r--   0        0        0     2541 2023-06-08 07:06:35.419053 timona-0.0.5/timona/template/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-08 07:07:37.075544 timona-0.0.5/timona/template/module_jinja2.py
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 timona-0.0.5/setup.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 timona-0.0.5/PKG-INFO
```

### Comparing `timona-0.0.4/LICENSE` & `timona-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `timona-0.0.4/pyproject.toml` & `timona-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timona"
-version = "0.0.4"
+version = "0.0.5"
 description = "Tool to automate Helm deployments"
 authors = ["mihaiush <mihaiush@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mihaiush/timona"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `timona-0.0.4/timona/config.py` & `timona-0.0.5/timona/config.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.4/timona/helm.py` & `timona-0.0.5/timona/helm.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.4/timona/main.py` & `timona-0.0.5/timona/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,14 @@
         print('timona: {}'.format(version))
         print('template: {}'.format(T.version))
         print('helm: {}'.format(H.version))
         print('helm: diff: {}'.format(H.version_diff))
         sys.exit()
 
     RELEASES = get_releases(T, TMP, CONFIG)
-    if not RELEASES:
-        sys.exit(1)
 
     if R and R not in RELEASES:
         raise RuntimeError('Unknown release: {}'.format(R))
 
     def env():
         print()
         e = {R: {'values': CONFIG['values'], 'variables': RELEASES[R]}}
```

### Comparing `timona-0.0.4/timona/releases.py` & `timona-0.0.5/timona/releases.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.4/timona/template/__init__.py` & `timona-0.0.5/timona/template/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,27 @@
                 else:
                     with open(module) as f:
                         m = f.read()
                 with open('{}/module_template.py'.format(tmp), 'w') as f:
                     f.write(m)
                 self.module = importlib.import_module('module_template')
             v = 'module: {}'.format(self.module.version)
+            var_re = self.module.regex
         elif 'command' in config:
             self.cmd = config['command']['render']
             p = subprocess.run(
                 shlex.split(config['command']['version']),
                 capture_output=True, check=True, text=True
             )
             v = p.stdout.strip()
             v = 'command: {}'.format(v)
             self.stderr = config['command'].get('stderr')
+            var_re = config['command'].get('regex')
         self.version = v
-        self.var_re = config.get('regex')
+        self.var_re = var_re
         if self.var_re:
             self.var_re = re.compile(self.var_re)
 
     def render(self, tpl, env):
         if self.module:
             return self.module.render(tpl, env)
         elif self.cmd:
```

### Comparing `timona-0.0.4/setup.py` & `timona-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['deepmerge', 'jinja2', 'pyyaml', 'requests']
 
 entry_points = \
 {'console_scripts': ['timona = timona.main:main']}
 
 setup_kwargs = {
     'name': 'timona',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Tool to automate Helm deployments',
     'long_description': '# timona\n\nA tool to automate Helm deployments.\n\nFor usage see https://github.com/mihaiush/timona/wiki .\n',
     'author': 'mihaiush',
     'author_email': 'mihaiush@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mihaiush/timona',
```

### Comparing `timona-0.0.4/PKG-INFO` & `timona-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timona
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to automate Helm deployments
 Home-page: https://github.com/mihaiush/timona
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

