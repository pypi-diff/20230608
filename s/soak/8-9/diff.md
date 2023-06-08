# Comparing `tmp/soak-8.tar.gz` & `tmp/soak-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soak-8.tar", last modified: Sun May 10 13:54:11 2020, max compression
+gzip compressed data, was "dist/soak-9.tar", last modified: Fri Jul 31 19:03:05 2020, max compression
```

## Comparing `soak-8.tar` & `soak-9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-10 13:54:11.000000 soak-8/
--rw-rw-r--   0 arc       (1000) arc       (1000)     3241 2020-05-10 13:54:10.000000 soak-8/setup.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-05-10 13:54:11.000000 soak-8/setup.cfg
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-10 13:54:11.000000 soak-8/soak/
--rw-rw-r--   0 arc       (1000) arc       (1000)     1880 2020-05-09 09:37:33.000000 soak-8/soak/util.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3901 2020-05-09 10:38:28.000000 soak-8/soak/context.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     1637 2020-05-10 13:47:34.000000 soak-8/soak/terminal.py
--rw-rw-r--   0 arc       (1000) arc       (1000)     3514 2020-05-09 08:36:12.000000 soak-8/soak/soak.py
--rw-rw-r--   0 arc       (1000) arc       (1000)      815 2020-03-21 13:40:40.000000 soak-8/soak/__init__.py
--rw-rw-r--   0 arc       (1000) arc       (1000)       50 2020-05-10 13:54:10.000000 soak-8/pyproject.toml
--rw-rw-r--   0 arc       (1000) arc       (1000)      123 2020-03-08 14:57:32.000000 soak-8/README.md
--rw-rw-r--   0 arc       (1000) arc       (1000)      413 2020-05-10 13:54:11.000000 soak-8/PKG-INFO
-drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-05-10 13:54:11.000000 soak-8/soak.egg-info/
--rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-05-10 13:54:11.000000 soak-8/soak.egg-info/dependency_links.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       35 2020-05-10 13:54:11.000000 soak-8/soak.egg-info/requires.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)       46 2020-05-10 13:54:11.000000 soak-8/soak.egg-info/entry_points.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      289 2020-05-10 13:54:11.000000 soak-8/soak.egg-info/SOURCES.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)        5 2020-05-10 13:54:11.000000 soak-8/soak.egg-info/top_level.txt
--rw-rw-r--   0 arc       (1000) arc       (1000)      413 2020-05-10 13:54:11.000000 soak-8/soak.egg-info/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-07-31 19:03:05.000000 soak-9/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     4720 2020-07-31 19:03:04.000000 soak-9/setup.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)       67 2020-07-31 19:03:05.000000 soak-9/setup.cfg
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-07-31 19:03:05.000000 soak-9/soak/
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1880 2020-05-09 09:37:33.000000 soak-9/soak/util.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3725 2020-07-03 16:57:24.000000 soak-9/soak/context.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     1637 2020-05-10 13:47:34.000000 soak-9/soak/terminal.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)     3514 2020-05-09 08:36:12.000000 soak-9/soak/soak.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      815 2020-03-21 13:40:40.000000 soak-9/soak/__init__.py
+-rw-rw-r--   0 arc       (1000) arc       (1000)      123 2020-03-08 14:57:32.000000 soak-9/README.md
+-rw-rw-r--   0 arc       (1000) arc       (1000)      417 2020-07-31 19:03:05.000000 soak-9/PKG-INFO
+drwxrwxr-x   0 arc       (1000) arc       (1000)        0 2020-07-31 19:03:05.000000 soak-9/soak.egg-info/
+-rw-rw-r--   0 arc       (1000) arc       (1000)        1 2020-07-31 19:03:05.000000 soak-9/soak.egg-info/dependency_links.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       35 2020-07-31 19:03:05.000000 soak-9/soak.egg-info/requires.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)       46 2020-07-31 19:03:05.000000 soak-9/soak.egg-info/entry_points.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      274 2020-07-31 19:03:05.000000 soak-9/soak.egg-info/SOURCES.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)        5 2020-07-31 19:03:05.000000 soak-9/soak.egg-info/top_level.txt
+-rw-rw-r--   0 arc       (1000) arc       (1000)      417 2020-07-31 19:03:05.000000 soak-9/soak.egg-info/PKG-INFO
```

### Comparing `soak-8/soak/util.py` & `soak-9/soak/util.py`

 * *Files identical despite different names*

### Comparing `soak-8/soak/context.py` & `soak-9/soak/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,18 +45,14 @@
     else:
         modulepath = Path(toplevelres.resolve(context).cat(), relpath)
     g = {} if modulename is None else dict(__name__ = modulename)
     with modulepath.open() as f:
         exec(f.read(), g)
     g[globalname](context)
 
-def xmlquote(context, resolvable):
-    from xml.sax.saxutils import escape
-    return Text(escape(resolvable.resolve(context).cat()))
-
 def blockliteral(context, textresolvable):
     text = yaml.dump(textresolvable.resolve(context).cat(), default_style = '|')
     header, *lines = text.splitlines() # For template interpolation convenience we discard the (insignificant) trailing newline.
     if not lines:
         return Text(header)
     if '...' == lines[-1]:
         lines.pop() # XXX: Could this result in no remaining lines?
@@ -79,15 +75,14 @@
         return Text(toplevel)
     except subprocess.CalledProcessError:
         raise NoSuchPathException('Git property: toplevel')
 
 def createparent(soakroot):
     parent = Context()
     parent['plugin',] = Directive(plugin)
-    parent['xml"',] = Function(xmlquote)
     parent['|',] = Function(blockliteral)
     parent['//',] = Function(rootpath)
     parent['toplevel',] = Snapshot(lambda: _toplevel(soakroot))
     with Repl(parent) as repl:
         repl('data = $processtemplate$(from)') # XXX: Too easy to accidentally override?
         repl.printf("indentunit = %s", 4 * ' ')
     return parent
```

### Comparing `soak-8/soak/terminal.py` & `soak-9/soak/terminal.py`

 * *Files identical despite different names*

### Comparing `soak-8/soak/soak.py` & `soak-9/soak/soak.py`

 * *Files identical despite different names*

### Comparing `soak-8/soak/__init__.py` & `soak-9/soak/__init__.py`

 * *Files identical despite different names*

