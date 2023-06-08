# Comparing `tmp/hexbytes-0.3.0.tar.gz` & `tmp/hexbytes-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexbytes-0.3.0.tar", last modified: Wed Aug 17 16:24:52 2022, max compression
+gzip compressed data, was "hexbytes-0.3.1.tar", last modified: Thu Jun  8 20:36:12 2023, max compression
```

## Comparing `hexbytes-0.3.0.tar` & `hexbytes-0.3.1.tar`

### file list

```diff
@@ -1,2057 +1,20 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.288259 hexbytes-0.3.0/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003345 hexbytes-0.3.0/.tox/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.997746 hexbytes-0.3.0/.tox/docs/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.997789 hexbytes-0.3.0/.tox/docs/lib/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.997835 hexbytes-0.3.0/.tox/docs/lib/python3.10/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.998140 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.010823 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/
--rw-r--r--   0 eve        (501) staff       (20)    15137 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      357 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/_cmp.pyi
--rw-r--r--   0 eve        (501) staff       (20)      209 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/_version_info.pyi
--rw-r--r--   0 eve        (501) staff       (20)      416 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/converters.pyi
--rw-r--r--   0 eve        (501) staff       (20)      539 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/exceptions.pyi
--rw-r--r--   0 eve        (501) staff       (20)      215 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/filters.pyi
--rw-r--r--   0 eve        (501) staff       (20)      573 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/setters.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2355 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attr/validators.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.011052 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attrs/
--rw-r--r--   0 eve        (501) staff       (20)     2100 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/attrs/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.011189 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/iniconfig/
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-11 20:34:21.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/iniconfig/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.011405 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/markupsafe/
--rw-r--r--   0 eve        (501) staff       (20)      229 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/markupsafe/_speedups.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.012545 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/
--rw-r--r--   0 eve        (501) staff       (20)      341 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.998240 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.012674 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/_vendored_packages/iniconfig/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3409 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/error.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/iniconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5277 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/io.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7168 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/path.pyi
--rw-r--r--   0 eve        (501) staff       (20)      787 2022-08-11 20:34:22.000000 hexbytes-0.3.0/.tox/docs/lib/python3.10/site-packages/py/xml.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.998338 hexbytes-0.3.0/.tox/lint/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.998375 hexbytes-0.3.0/.tox/lint/lib/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.998413 hexbytes-0.3.0/.tox/lint/lib/python3.9/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003187 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.014541 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/
--rw-r--r--   0 eve        (501) staff       (20)    15137 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      357 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/_cmp.pyi
--rw-r--r--   0 eve        (501) staff       (20)      209 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/_version_info.pyi
--rw-r--r--   0 eve        (501) staff       (20)      416 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/converters.pyi
--rw-r--r--   0 eve        (501) staff       (20)      539 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/exceptions.pyi
--rw-r--r--   0 eve        (501) staff       (20)      215 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/filters.pyi
--rw-r--r--   0 eve        (501) staff       (20)      573 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/setters.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2355 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attr/validators.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.014709 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attrs/
--rw-r--r--   0 eve        (501) staff       (20)     2100 2022-08-10 21:21:57.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/attrs/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.014888 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/iniconfig/
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/iniconfig/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:51.998688 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.002960 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.053880 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.094661 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/
--rw-r--r--   0 eve        (501) staff       (20)     1702 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/BaseHTTPServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)      163 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/CGIHTTPServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3752 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ConfigParser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1302 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Cookie.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1051 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/HTMLParser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      872 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Queue.pyi
--rw-r--r--   0 eve        (501) staff       (20)      613 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SimpleHTTPServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4487 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SocketServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1127 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/StringIO.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1551 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserDict.pyi
--rw-r--r--   0 eve        (501) staff       (20)      623 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserList.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3760 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserString.pyi
--rw-r--r--   0 eve        (501) staff       (20)    48328 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__builtin__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      512 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__future__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       63 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__main__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5288 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)      449 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4542 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1406 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_collections.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1256 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_csv.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13695 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_curses.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3918 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_dummy_threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)      554 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_functools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      543 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)      607 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_hotshot.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6831 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_io.pyi
--rw-r--r--   0 eve        (501) staff       (20)      198 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_json.pyi
--rw-r--r--   0 eve        (501) staff       (20)      230 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_markupbase.pyi
--rw-r--r--   0 eve        (501) staff       (20)      300 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_md5.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2205 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1807 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_osx_support.pyi
--rw-r--r--   0 eve        (501) staff       (20)      405 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_random.pyi
--rw-r--r--   0 eve        (501) staff       (20)      348 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha.pyi
--rw-r--r--   0 eve        (501) staff       (20)      597 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha256.pyi
--rw-r--r--   0 eve        (501) staff       (20)      597 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha512.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6253 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1874 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sre.pyi
--rw-r--r--   0 eve        (501) staff       (20)      760 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_struct.pyi
--rw-r--r--   0 eve        (501) staff       (20)      646 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_symtable.pyi
--rw-r--r--   0 eve        (501) staff       (20)      795 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)      319 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_threading_local.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2709 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_tkinter.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.095300 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/
--rw-r--r--   0 eve        (501) staff       (20)     4464 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1261 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/wsgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)      483 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/xml.pyi
--rw-r--r--   0 eve        (501) staff       (20)      876 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)      926 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2181 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_weakrefset.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4022 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_winreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1155 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2738 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/aifc.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/antigravity.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13985 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/argparse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3023 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/array.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1155 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1434 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/asynchat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5277 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/asyncore.pyi
--rw-r--r--   0 eve        (501) staff       (20)      117 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/atexit.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2074 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/audioop.pyi
--rw-r--r--   0 eve        (501) staff       (20)      903 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/base64.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4500 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/bdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      967 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/binascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1127 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/binhex.pyi
--rw-r--r--   0 eve        (501) staff       (20)       67 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)    48328 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/builtins.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1344 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/bz2.pyi
--rw-r--r--   0 eve        (501) staff       (20)      789 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cPickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1288 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cProfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1797 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cStringIO.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4934 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/calendar.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3957 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1307 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgitb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      613 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/chunk.pyi
--rw-r--r--   0 eve        (501) staff       (20)      875 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cmath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1596 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cmd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1060 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/code.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11793 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)      455 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/codeop.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4759 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/collections.pyi
--rw-r--r--   0 eve        (501) staff       (20)      552 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/colorsys.pyi
--rw-r--r--   0 eve        (501) staff       (20)      322 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/commands.pyi
--rw-r--r--   0 eve        (501) staff       (20)      549 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/compileall.pyi
--rw-r--r--   0 eve        (501) staff       (20)      906 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/contextlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4664 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cookielib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      309 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      794 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy_reg.pyi
--rw-r--r--   0 eve        (501) staff       (20)      794 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copyreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)       88 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/crypt.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2510 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/csv.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.095828 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/
--rw-r--r--   0 eve        (501) staff       (20)    11288 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      129 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4642 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/wintypes.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.096382 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/
--rw-r--r--   0 eve        (501) staff       (20)      356 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1127 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/ascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)      801 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/panel.pyi
--rw-r--r--   0 eve        (501) staff       (20)      431 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/textpad.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7839 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/datetime.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.097168 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/
--rw-r--r--   0 eve        (501) staff       (20)      974 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      994 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1348 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/gnu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1222 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/ndbm.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13228 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/decimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3521 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/difflib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      249 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dircache.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1044 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dis.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.101036 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      388 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/archive_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/bcppcompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6237 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/ccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2745 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cmd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.103359 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      242 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_packager.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_rpm.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_wininst.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_clib.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_ext.pyi
--rw-r--r--   0 eve        (501) staff       (20)      181 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_py.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/check.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/clean.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2882 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)      316 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_data.pyi
--rw-r--r--   0 eve        (501) staff       (20)      354 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_egg_info.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_lib.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/register.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/sdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      273 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/upload.pyi
--rw-r--r--   0 eve        (501) staff       (20)      497 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1637 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/core.pyi
--rw-r--r--   0 eve        (501) staff       (20)      138 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cygwinccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)       12 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/debug.pyi
--rw-r--r--   0 eve        (501) staff       (20)      220 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dep_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      530 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dir_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      470 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dist.pyi
--rw-r--r--   0 eve        (501) staff       (20)       90 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/emxccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      852 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      658 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/extension.pyi
--rw-r--r--   0 eve        (501) staff       (20)      805 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/fancy_getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      419 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/file_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)       20 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/filelist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      863 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/log.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/msvccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      186 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/spawn.pyi
--rw-r--r--   0 eve        (501) staff       (20)      586 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)      672 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/text_file.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/unixccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      841 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1132 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/version.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6694 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/doctest.pyi
--rw-r--r--   0 eve        (501) staff       (20)      762 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_threading.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.105256 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/
--rw-r--r--   0 eve        (501) staff       (20)      159 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/MIMEText.pyi
--rw-r--r--   0 eve        (501) staff       (20)      265 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1059 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/_parseaddr.pyi
--rw-r--r--   0 eve        (501) staff       (20)      303 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/base64mime.pyi
--rw-r--r--   0 eve        (501) staff       (20)      902 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/charset.pyi
--rw-r--r--   0 eve        (501) staff       (20)      143 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/encoders.pyi
--rw-r--r--   0 eve        (501) staff       (20)      536 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/feedparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      377 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/generator.pyi
--rw-r--r--   0 eve        (501) staff       (20)      457 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/header.pyi
--rw-r--r--   0 eve        (501) staff       (20)      256 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/iterators.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1950 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/message.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.106433 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      351 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/application.pyi
--rw-r--r--   0 eve        (501) staff       (20)      176 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/audio.pyi
--rw-r--r--   0 eve        (501) staff       (20)      128 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/base.pyi
--rw-r--r--   0 eve        (501) staff       (20)      176 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/image.pyi
--rw-r--r--   0 eve        (501) staff       (20)      147 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/message.pyi
--rw-r--r--   0 eve        (501) staff       (20)      159 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/multipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      107 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/nonmultipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      159 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)      415 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      490 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/quoprimime.pyi
--rw-r--r--   0 eve        (501) staff       (20)      738 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/utils.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.106664 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/
--rw-r--r--   0 eve        (501) staff       (20)      184 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      566 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/utf_8.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.106788 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ensurepip/
--rw-r--r--   0 eve        (501) staff       (20)      214 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ensurepip/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2011 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/errno.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1756 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/exceptions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1903 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fcntl.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1415 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/filecmp.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1479 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fileinput.pyi
--rw-r--r--   0 eve        (501) staff       (20)      329 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fnmatch.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4565 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/formatter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5216 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fractions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4847 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ftplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1112 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/functools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      194 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/future_builtins.pyi
--rw-r--r--   0 eve        (501) staff       (20)      739 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1082 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/genericpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      382 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      160 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getpass.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2190 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gettext.pyi
--rw-r--r--   0 eve        (501) staff       (20)      344 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/glob.pyi
--rw-r--r--   0 eve        (501) staff       (20)      345 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/grp.pyi
--rw-r--r--   0 eve        (501) staff       (20)      997 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gzip.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1059 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hashlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      719 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)      787 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hmac.pyi
--rw-r--r--   0 eve        (501) staff       (20)       89 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/htmlentitydefs.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5818 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/httplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6213 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imaplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      441 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imghdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1264 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imp.pyi
--rw-r--r--   0 eve        (501) staff       (20)      121 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/importlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4588 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/inspect.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1124 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/io.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5957 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/itertools.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3041 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/json.pyi
--rw-r--r--   0 eve        (501) staff       (20)       94 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/keyword.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.107219 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.108199 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      931 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/driver.pyi
--rw-r--r--   0 eve        (501) staff       (20)      683 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/grammar.pyi
--rw-r--r--   0 eve        (501) staff       (20)      166 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/literals.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1055 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2130 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/pgen.pyi
--rw-r--r--   0 eve        (501) staff       (20)      913 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)      870 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2208 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pygram.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3147 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pytree.pyi
--rw-r--r--   0 eve        (501) staff       (20)      435 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/linecache.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2183 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/locale.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.108615 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/
--rw-r--r--   0 eve        (501) staff       (20)     9521 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      359 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4137 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1633 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/macpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      140 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/macurl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7507 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mailbox.pyi
--rw-r--r--   0 eve        (501) staff       (20)      282 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mailcap.pyi
--rw-r--r--   0 eve        (501) staff       (20)      238 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/markupbase.pyi
--rw-r--r--   0 eve        (501) staff       (20)      253 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/marshal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1979 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/math.pyi
--rw-r--r--   0 eve        (501) staff       (20)       74 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/md5.pyi
--rw-r--r--   0 eve        (501) staff       (20)      703 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetools.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1390 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetypes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1797 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mmap.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3072 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/modulefinder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.109097 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/
--rw-r--r--   0 eve        (501) staff       (20)     5847 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2141 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/schema.pyi
--rw-r--r--   0 eve        (501) staff       (20)      312 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/sequence.pyi
--rw-r--r--   0 eve        (501) staff       (20)      155 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)      795 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msvcrt.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.109559 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/
--rw-r--r--   0 eve        (501) staff       (20)     1890 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.109792 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/
--rw-r--r--   0 eve        (501) staff       (20)     1167 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      641 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/connection.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1957 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/pool.pyi
--rw-r--r--   0 eve        (501) staff       (20)      870 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/process.pyi
--rw-r--r--   0 eve        (501) staff       (20)      736 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      362 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mutex.pyi
--rw-r--r--   0 eve        (501) staff       (20)      515 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/netrc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      293 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nis.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4227 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nntplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2784 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ntpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      115 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nturl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3654 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/numbers.pyi
--rw-r--r--   0 eve        (501) staff       (20)      267 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/opcode.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7382 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/operator.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9977 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/optparse.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.110192 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/
--rw-r--r--   0 eve        (501) staff       (20)    11473 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2779 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2784 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os2emxpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3618 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ossaudiodev.pyi
--rw-r--r--   0 eve        (501) staff       (20)      927 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6493 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2093 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2941 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pickletools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      467 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pipes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1193 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pkgutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1786 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/platform.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1002 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/plistlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      960 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/popen2.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1410 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/poplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6345 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posix.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2784 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posixpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      878 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pprint.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1304 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/profile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1908 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pstats.pyi
--rw-r--r--   0 eve        (501) staff       (20)      482 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pty.pyi
--rw-r--r--   0 eve        (501) staff       (20)      405 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pwd.pyi
--rw-r--r--   0 eve        (501) staff       (20)      465 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/py_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)      645 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyclbr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10143 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.110395 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc_data/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc_data/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       23 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc_data/topics.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.110759 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/
--rw-r--r--   0 eve        (501) staff       (20)     3184 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1152 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      205 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/model.pyi
--rw-r--r--   0 eve        (501) staff       (20)      343 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/quopri.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3130 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/random.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3381 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/re.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1573 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/readline.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1089 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/repr.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1056 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/resource.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2147 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rfc822.pyi
--rw-r--r--   0 eve        (501) staff       (20)      325 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rlcompleter.pyi
--rw-r--r--   0 eve        (501) staff       (20)      230 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/robotparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      519 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/runpy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      725 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sched.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3551 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/select.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2813 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sets.pyi
--rw-r--r--   0 eve        (501) staff       (20)      236 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sha.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1603 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shelve.pyi
--rw-r--r--   0 eve        (501) staff       (20)      965 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shlex.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1791 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1271 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/signal.pyi
--rw-r--r--   0 eve        (501) staff       (20)      375 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/site.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1639 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtpd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2542 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      184 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sndhdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12509 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)      388 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/spwd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.110992 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sqlite3/
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sqlite3/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9542 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sqlite3/dbapi2.pyi
--rw-r--r--   0 eve        (501) staff       (20)      765 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1732 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2216 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9476 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ssl.pyi
--rw-r--r--   0 eve        (501) staff       (20)      992 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3501 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/string.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1985 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringold.pyi
--rw-r--r--   0 eve        (501) staff       (20)      817 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringprep.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1151 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/strop.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1021 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/struct.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3169 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2352 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sunau.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1316 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symbol.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1683 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symtable.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3524 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sys.pyi
--rw-r--r--   0 eve        (501) staff       (20)      820 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1019 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/syslog.pyi
--rw-r--r--   0 eve        (501) staff       (20)      413 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tabnanny.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9244 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tarfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2512 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/telnetlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3578 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tempfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4499 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/termios.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1842 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/textwrap.pyi
--rw-r--r--   0 eve        (501) staff       (20)       25 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/this.pyi
--rw-r--r--   0 eve        (501) staff       (20)      963 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3927 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1337 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/time.pyi
--rw-r--r--   0 eve        (501) staff       (20)      855 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/timeit.pyi
--rw-r--r--   0 eve        (501) staff       (20)      213 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/toaiff.pyi
--rw-r--r--   0 eve        (501) staff       (20)      874 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2660 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2424 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/trace.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1448 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/traceback.pyi
--rw-r--r--   0 eve        (501) staff       (20)      340 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tty.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17275 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/turtle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5356 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)    18009 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2910 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing_extensions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1620 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unicodedata.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12541 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unittest.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4714 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8224 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib2.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1890 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urlparse.pyi
--rw-r--r--   0 eve        (501) staff       (20)       83 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/user.pyi
--rw-r--r--   0 eve        (501) staff       (20)      306 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/uu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2373 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/uuid.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2017 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2081 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wave.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2842 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2997 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/webbrowser.pyi
--rw-r--r--   0 eve        (501) staff       (20)       72 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/whichdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      782 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/winsound.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.111803 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2996 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)      964 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1385 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/simple_server.pyi
--rw-r--r--   0 eve        (501) staff       (20)       71 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)      782 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1591 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/validate.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2309 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xdrlib.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.111924 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/
--rw-r--r--   0 eve        (501) staff       (20)       30 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.112886 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/
--rw-r--r--   0 eve        (501) staff       (20)      457 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/NodeFilter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1844 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      409 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/domreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)       77 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/expatbuilder.pyi
--rw-r--r--   0 eve        (501) staff       (20)      508 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/minicompat.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10318 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/minidom.pyi
--rw-r--r--   0 eve        (501) staff       (20)       77 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/pulldom.pyi
--rw-r--r--   0 eve        (501) staff       (20)      141 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/xmlbuilder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.113526 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/
--rw-r--r--   0 eve        (501) staff       (20)      574 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/ElementInclude.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1516 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/ElementPath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8739 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/ElementTree.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       36 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/cElementTree.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.113684 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/
--rw-r--r--   0 eve        (501) staff       (20)       34 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.114169 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/
--rw-r--r--   0 eve        (501) staff       (20)       22 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)       28 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/model.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.114865 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/
--rw-r--r--   0 eve        (501) staff       (20)     1213 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1391 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/handler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2464 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/saxutils.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2424 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/xmlreader.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9512 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xmlrpclib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3410 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/zipfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)      618 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/zipimport.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1214 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/zlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      914 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/__future__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       63 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/__main__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14688 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2510 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)       63 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bootlocale.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6813 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2123 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      356 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compat_pickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)      954 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compression.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2355 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_csv.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17284 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_curses.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13492 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_decimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1177 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5425 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)      324 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1149 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_imp.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1481 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_json.pyi
--rw-r--r--   0 eve        (501) staff       (20)      762 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_markupbase.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2217 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5907 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_operator.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1993 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_osx_support.pyi
--rw-r--r--   0 eve        (501) staff       (20)      647 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_posixsubprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)      378 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_py_abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      951 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_pydecimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)      404 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_random.pyi
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_sitebuiltins.pyi
--rw-r--r--   0 eve        (501) staff       (20)    16847 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2944 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_stat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1660 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)      552 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_threading_local.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3942 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tkinter.pyi
--rw-r--r--   0 eve        (501) staff       (20)      552 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tracemalloc.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.115669 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/
--rw-r--r--   0 eve        (501) staff       (20)     8558 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1638 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/dbapi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1623 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/wsgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)      490 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/xml.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1026 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1263 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2490 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7621 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_winapi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1451 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3385 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/aifc.pyi
--rw-r--r--   0 eve        (501) staff       (20)       76 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/antigravity.pyi
--rw-r--r--   0 eve        (501) staff       (20)    19820 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/argparse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3685 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/array.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10501 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1099 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asynchat.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.120916 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/
--rw-r--r--   0 eve        (501) staff       (20)      722 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    21068 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1014 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_futures.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3270 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)      404 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_tasks.pyi
--rw-r--r--   0 eve        (501) staff       (20)       99 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/compat.pyi
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)      857 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/coroutines.pyi
--rw-r--r--   0 eve        (501) staff       (20)    27578 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1001 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/exceptions.pyi
--rw-r--r--   0 eve        (501) staff       (20)      886 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/format_helpers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3382 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/futures.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4380 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/locks.pyi
--rw-r--r--   0 eve        (501) staff       (20)       39 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/log.pyi
--rw-r--r--   0 eve        (501) staff       (20)      210 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/mixins.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3681 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/proactor_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1815 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/protocols.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1395 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/queues.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1006 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/runners.pyi
--rw-r--r--   0 eve        (501) staff       (20)      314 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/selector_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7275 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/sslproto.pyi
--rw-r--r--   0 eve        (501) staff       (20)      340 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/staggered.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7066 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/streams.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6097 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)      691 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/taskgroups.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13461 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/tasks.pyi
--rw-r--r--   0 eve        (501) staff       (20)      265 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/threads.pyi
--rw-r--r--   0 eve        (501) staff       (20)      662 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/timeouts.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2361 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/transports.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4575 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/trsock.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6543 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/unix_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4077 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2476 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_utils.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3718 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncore.pyi
--rw-r--r--   0 eve        (501) staff       (20)      394 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/atexit.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2145 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/audioop.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2117 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/base64.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4670 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/bdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1825 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/binascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1269 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/binhex.pyi
--rw-r--r--   0 eve        (501) staff       (20)       67 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)    77449 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/builtins.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4849 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/bz2.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1549 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cProfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6037 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/calendar.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4168 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1381 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgitb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      613 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/chunk.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1324 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1750 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1443 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/code.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11547 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)      516 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/codeop.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.121204 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/
--rw-r--r--   0 eve        (501) staff       (20)    20922 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      648 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/colorsys.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3340 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/compileall.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.121323 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.122053 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/
--rw-r--r--   0 eve        (501) staff       (20)      977 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5254 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/_base.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7135 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/process.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2285 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10691 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/configparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8440 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1914 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextvars.pyi
--rw-r--r--   0 eve        (501) staff       (20)      350 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/copy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      995 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/copyreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)      532 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/crypt.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4661 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/csv.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.122536 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/
--rw-r--r--   0 eve        (501) staff       (20)    11583 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      129 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5232 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.122986 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/
--rw-r--r--   0 eve        (501) staff       (20)      622 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1393 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/ascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)      931 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/panel.pyi
--rw-r--r--   0 eve        (501) staff       (20)      511 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/textpad.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7916 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dataclasses.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11113 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/datetime.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.123571 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/
--rw-r--r--   0 eve        (501) staff       (20)     1775 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1092 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1643 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/gnu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1429 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/ndbm.pyi
--rw-r--r--   0 eve        (501) staff       (20)      117 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/decimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4525 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/difflib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4573 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dis.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.126660 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/archive_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/bcppcompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6315 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/ccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2758 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cmd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.130003 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      540 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      450 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1489 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_packager.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1104 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi
--rw-r--r--   0 eve        (501) staff       (20)      638 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi
--rw-r--r--   0 eve        (501) staff       (20)      711 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build.pyi
--rw-r--r--   0 eve        (501) staff       (20)      668 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_clib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1257 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_ext.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1444 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_py.pyi
--rw-r--r--   0 eve        (501) staff       (20)      574 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)      961 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/check.pyi
--rw-r--r--   0 eve        (501) staff       (20)      377 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/clean.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2644 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1689 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install.pyi
--rw-r--r--   0 eve        (501) staff       (20)      436 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_data.pyi
--rw-r--r--   0 eve        (501) staff       (20)      490 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_egg_info.pyi
--rw-r--r--   0 eve        (501) staff       (20)      387 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)      598 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_lib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      426 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)      569 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/register.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1118 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/sdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      462 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/upload.pyi
--rw-r--r--   0 eve        (501) staff       (20)      497 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1664 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/core.pyi
--rw-r--r--   0 eve        (501) staff       (20)      138 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)       19 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/debug.pyi
--rw-r--r--   0 eve        (501) staff       (20)      220 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dep_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      530 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dir_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2451 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      852 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1222 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/extension.pyi
--rw-r--r--   0 eve        (501) staff       (20)      966 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      428 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/file_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2224 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/filelist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      845 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/log.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/msvccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      186 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/spawn.pyi
--rw-r--r--   0 eve        (501) staff       (20)      559 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)      679 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/text_file.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/unixccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1549 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1361 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/version.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7634 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/doctest.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dummy_threading.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.132182 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/
--rw-r--r--   0 eve        (501) staff       (20)     1032 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11761 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/_header_value_parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      400 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/base64mime.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1067 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/charset.pyi
--rw-r--r--   0 eve        (501) staff       (20)      516 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi
--rw-r--r--   0 eve        (501) staff       (20)      293 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/encoders.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1532 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      951 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/feedparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1329 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/generator.pyi
--rw-r--r--   0 eve        (501) staff       (20)      952 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/header.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5903 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/headerregistry.pyi
--rw-r--r--   0 eve        (501) staff       (20)      641 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/iterators.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5065 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/message.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.133155 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      472 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/application.pyi
--rw-r--r--   0 eve        (501) staff       (20)      466 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/audio.pyi
--rw-r--r--   0 eve        (501) staff       (20)      270 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/base.pyi
--rw-r--r--   0 eve        (501) staff       (20)      466 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/image.pyi
--rw-r--r--   0 eve        (501) staff       (20)      288 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/message.pyi
--rw-r--r--   0 eve        (501) staff       (20)      478 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/multipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      108 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/nonmultipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      273 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1449 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3055 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/policy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      735 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/quoprimime.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2107 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/utils.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.133488 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/
--rw-r--r--   0 eve        (501) staff       (20)      306 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      825 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1232 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8_sig.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.133600 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/
--rw-r--r--   0 eve        (501) staff       (20)      257 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9490 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/enum.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2661 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/errno.pyi
--rw-r--r--   0 eve        (501) staff       (20)      644 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/faulthandler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3358 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fcntl.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1961 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/filecmp.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11065 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fileinput.pyi
--rw-r--r--   0 eve        (501) staff       (20)      339 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fnmatch.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4654 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/formatter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5365 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fractions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6067 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ftplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6363 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/functools.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1326 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/gc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1750 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/genericpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      442 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      217 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/getpass.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6147 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/gettext.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1397 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/glob.pyi
--rw-r--r--   0 eve        (501) staff       (20)      913 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/graphlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      730 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/grp.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4956 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/gzip.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5546 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/hashlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      712 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1506 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/hmac.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.134201 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/
--rw-r--r--   0 eve        (501) staff       (20)      156 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      182 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/entities.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1846 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/parser.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.135099 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/
--rw-r--r--   0 eve        (501) staff       (20)     2407 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7659 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/client.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7478 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookiejar.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2414 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookies.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3895 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/server.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7693 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/imaplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      500 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/imghdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2376 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/imp.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.135681 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/
--rw-r--r--   0 eve        (501) staff       (20)      800 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7512 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5770 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.135907 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata/
--rw-r--r--   0 eve        (501) staff       (20)     6609 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      752 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1497 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/resources.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1872 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17776 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/inspect.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8007 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/io.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7131 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ipaddress.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10786 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/itertools.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.136353 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/
--rw-r--r--   0 eve        (501) staff       (20)     1981 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1113 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/decoder.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1035 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/encoder.pyi
--rw-r--r--   0 eve        (501) staff       (20)       24 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/tool.pyi
--rw-r--r--   0 eve        (501) staff       (20)      357 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/keyword.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.136759 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.137626 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      984 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi
--rw-r--r--   0 eve        (501) staff       (20)      724 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi
--rw-r--r--   0 eve        (501) staff       (20)      155 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/literals.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1119 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2135 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1005 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2073 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2208 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pygram.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3206 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pytree.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3278 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/refactor.pyi
--rw-r--r--   0 eve        (501) staff       (20)      941 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/linecache.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3784 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/locale.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.138014 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/
--rw-r--r--   0 eve        (501) staff       (20)    26790 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2360 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9838 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5435 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lzma.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2405 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/macpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      184 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/macurl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10420 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailbox.pyi
--rw-r--r--   0 eve        (501) staff       (20)      378 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailcap.pyi
--rw-r--r--   0 eve        (501) staff       (20)      253 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/marshal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4584 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/math.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1985 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mimetypes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3766 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mmap.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3606 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/modulefinder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.138469 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/
--rw-r--r--   0 eve        (501) staff       (20)     6071 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2141 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/schema.pyi
--rw-r--r--   0 eve        (501) staff       (20)      363 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/sequence.pyi
--rw-r--r--   0 eve        (501) staff       (20)      155 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)      840 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msvcrt.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.139869 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/
--rw-r--r--   0 eve        (501) staff       (20)     5177 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2467 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/connection.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7459 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/context.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.140097 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/
--rw-r--r--   0 eve        (501) staff       (20)     1958 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1335 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8556 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/managers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4755 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/pool.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1371 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/process.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1398 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/queues.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2619 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/reduction.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1348 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4000 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi
--rw-r--r--   0 eve        (501) staff       (20)      859 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/spawn.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2278 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi
--rw-r--r--   0 eve        (501) staff       (20)      639 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/netrc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      293 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/nis.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4457 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/nntplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2815 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ntpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)       76 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/nturl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3912 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/numbers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1228 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/opcode.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1645 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/operator.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10273 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/optparse.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.140396 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/
--rw-r--r--   0 eve        (501) staff       (20)    36999 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      186 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3618 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ossaudiodev.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1046 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7828 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pathlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7494 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6773 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3777 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickletools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      538 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pipes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1610 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pkgutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2327 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/platform.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3976 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/plistlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2149 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/poplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10709 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/posix.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4241 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/posixpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3835 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pprint.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1413 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/profile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2994 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pstats.pyi
--rw-r--r--   0 eve        (501) staff       (20)      679 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pty.pyi
--rw-r--r--   0 eve        (501) staff       (20)      931 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pwd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1574 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/py_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2198 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyclbr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10457 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.140585 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       23 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/topics.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.140938 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/
--rw-r--r--   0 eve        (501) staff       (20)     3374 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1477 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      205 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/model.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2219 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/queue.pyi
--rw-r--r--   0 eve        (501) staff       (20)      407 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/quopri.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4767 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/random.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5091 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/re.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1854 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/readline.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1340 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/reprlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2763 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/resource.pyi
--rw-r--r--   0 eve        (501) staff       (20)      321 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/rlcompleter.pyi
--rw-r--r--   0 eve        (501) staff       (20)      774 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/runpy.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1339 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sched.pyi
--rw-r--r--   0 eve        (501) staff       (20)      621 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/secrets.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4559 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/select.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3714 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/selectors.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1724 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/shelve.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1545 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/shlex.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6435 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/shutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5287 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/signal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1355 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/site.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2978 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtpd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6168 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      353 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sndhdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    23499 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6364 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/socketserver.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1180 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/spwd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.141163 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    16847 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi
--rw-r--r--   0 eve        (501) staff       (20)      320 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3982 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4130 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)    18944 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ssl.pyi
--rw-r--r--   0 eve        (501) staff       (20)       20 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/stat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4922 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/statistics.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2011 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/string.pyi
--rw-r--r--   0 eve        (501) staff       (20)      910 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/stringprep.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1287 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/struct.pyi
--rw-r--r--   0 eve        (501) staff       (20)    58351 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2870 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sunau.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1566 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/symbol.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2391 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/symtable.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11053 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sys.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1085 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1357 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/syslog.pyi
--rw-r--r--   0 eve        (501) staff       (20)      514 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tabnanny.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12696 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tarfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2809 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/telnetlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14679 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tempfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4753 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/termios.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3190 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/textwrap.pyi
--rw-r--r--   0 eve        (501) staff       (20)       25 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/this.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6178 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3789 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/time.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1197 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/timeit.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.143364 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/
--rw-r--r--   0 eve        (501) staff       (20)   135621 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      335 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/colorchooser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      355 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/commondialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1886 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)      361 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)      724 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dnd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5130 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/filedialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4039 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/font.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1350 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/messagebox.pyi
--rw-r--r--   0 eve        (501) staff       (20)      329 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/scrolledtext.pyi
--rw-r--r--   0 eve        (501) staff       (20)      970 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/simpledialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14753 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/tix.pyi
--rw-r--r--   0 eve        (501) staff       (20)    44937 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/ttk.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2625 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4546 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)      374 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tomllib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2759 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/trace.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8798 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/traceback.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4488 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tracemalloc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      434 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tty.pyi
--rw-r--r--   0 eve        (501) staff       (20)    21951 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/turtle.pyi
--rw-r--r--   0 eve        (501) staff       (20)    21717 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)    34098 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7844 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1864 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unicodedata.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.144770 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/
--rw-r--r--   0 eve        (501) staff       (20)     1840 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      892 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/_log.pyi
--rw-r--r--   0 eve        (501) staff       (20)      663 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/async_case.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14516 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/case.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2161 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/loader.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1669 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/main.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14446 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1718 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1384 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi
--rw-r--r--   0 eve        (501) staff       (20)      487 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi
--rw-r--r--   0 eve        (501) staff       (20)      982 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi
--rw-r--r--   0 eve        (501) staff       (20)      976 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/util.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.145475 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      768 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/error.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5682 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17137 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/request.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2250 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/response.pyi
--rw-r--r--   0 eve        (501) staff       (20)      734 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/robotparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      593 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/uu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2645 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/uuid.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.145591 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/
--rw-r--r--   0 eve        (501) staff       (20)     2579 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3654 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2723 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wave.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5833 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2567 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/webbrowser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4368 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/winreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)      898 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/winsound.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.146360 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3064 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1020 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1465 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/simple_server.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1248 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)      993 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1658 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/validate.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2398 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xdrlib.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.146481 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/
--rw-r--r--   0 eve        (501) staff       (20)       30 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.147410 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/
--rw-r--r--   0 eve        (501) staff       (20)      457 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/NodeFilter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1889 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      418 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/domreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4570 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi
--rw-r--r--   0 eve        (501) staff       (20)      606 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minicompat.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11646 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minidom.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3407 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/pulldom.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4237 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.147965 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/
--rw-r--r--   0 eve        (501) staff       (20)      935 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1616 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14083 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       36 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/cElementTree.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.148077 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/
--rw-r--r--   0 eve        (501) staff       (20)       34 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.148426 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/
--rw-r--r--   0 eve        (501) staff       (20)       22 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)       28 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/model.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.148880 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/
--rw-r--r--   0 eve        (501) staff       (20)     1553 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1730 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/handler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2496 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/saxutils.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2433 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.149186 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12334 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/client.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6813 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/server.pyi
--rw-r--r--   0 eve        (501) staff       (20)      338 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xxlimited.pyi
--rw-r--r--   0 eve        (501) staff       (20)      777 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipapp.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10985 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1321 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipimport.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1743 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zlib.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.149297 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/
--rw-r--r--   0 eve        (501) staff       (20)     1241 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.002998 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stubs/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.149420 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/
--rw-r--r--   0 eve        (501) staff       (20)     2262 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003094 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypyc/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003129 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypyc/test-data/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.149539 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypyc/test-data/fixtures/
--rw-r--r--   0 eve        (501) staff       (20)     4902 2022-08-10 21:21:49.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/mypyc/test-data/fixtures/typing-full.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.150575 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/
--rw-r--r--   0 eve        (501) staff       (20)      341 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003279 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.150695 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3409 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/error.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/iniconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5277 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/io.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7168 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/path.pyi
--rw-r--r--   0 eve        (501) staff       (20)      787 2022-08-10 21:21:56.000000 hexbytes-0.3.0/.tox/lint/lib/python3.9/site-packages/py/xml.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003381 hexbytes-0.3.0/.tox/py39-lint/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003419 hexbytes-0.3.0/.tox/py39-lint/lib/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003455 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.007874 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.152103 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/
--rw-r--r--   0 eve        (501) staff       (20)    15137 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      357 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/_cmp.pyi
--rw-r--r--   0 eve        (501) staff       (20)      209 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/_version_info.pyi
--rw-r--r--   0 eve        (501) staff       (20)      416 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/converters.pyi
--rw-r--r--   0 eve        (501) staff       (20)      539 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/exceptions.pyi
--rw-r--r--   0 eve        (501) staff       (20)      215 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/filters.pyi
--rw-r--r--   0 eve        (501) staff       (20)      573 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/setters.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2355 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attr/validators.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.152294 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attrs/
--rw-r--r--   0 eve        (501) staff       (20)     2100 2022-08-10 21:22:27.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/attrs/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.152493 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/iniconfig/
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/iniconfig/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.003686 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.007654 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.192633 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.233247 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/
--rw-r--r--   0 eve        (501) staff       (20)     1702 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/BaseHTTPServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)      163 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/CGIHTTPServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3752 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ConfigParser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1302 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Cookie.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1051 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/HTMLParser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      872 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Queue.pyi
--rw-r--r--   0 eve        (501) staff       (20)      613 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SimpleHTTPServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4487 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SocketServer.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1127 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/StringIO.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1551 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserDict.pyi
--rw-r--r--   0 eve        (501) staff       (20)      623 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserList.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3760 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserString.pyi
--rw-r--r--   0 eve        (501) staff       (20)    48328 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__builtin__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      512 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__future__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       63 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__main__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5288 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)      449 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4542 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1406 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_collections.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1256 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_csv.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13695 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_curses.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3918 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_dummy_threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)      554 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_functools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      543 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)      607 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_hotshot.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6831 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_io.pyi
--rw-r--r--   0 eve        (501) staff       (20)      198 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_json.pyi
--rw-r--r--   0 eve        (501) staff       (20)      230 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_markupbase.pyi
--rw-r--r--   0 eve        (501) staff       (20)      300 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_md5.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2205 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1807 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_osx_support.pyi
--rw-r--r--   0 eve        (501) staff       (20)      405 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_random.pyi
--rw-r--r--   0 eve        (501) staff       (20)      348 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha.pyi
--rw-r--r--   0 eve        (501) staff       (20)      597 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha256.pyi
--rw-r--r--   0 eve        (501) staff       (20)      597 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha512.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6253 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1874 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sre.pyi
--rw-r--r--   0 eve        (501) staff       (20)      760 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_struct.pyi
--rw-r--r--   0 eve        (501) staff       (20)      646 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_symtable.pyi
--rw-r--r--   0 eve        (501) staff       (20)      795 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)      319 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_threading_local.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2709 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_tkinter.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.233797 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/
--rw-r--r--   0 eve        (501) staff       (20)     4464 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1261 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/wsgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)      483 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_typeshed/xml.pyi
--rw-r--r--   0 eve        (501) staff       (20)      876 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)      926 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2181 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_weakrefset.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4022 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_winreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1155 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2738 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/aifc.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/antigravity.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13985 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/argparse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3023 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/array.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1155 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1434 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/asynchat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5277 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/asyncore.pyi
--rw-r--r--   0 eve        (501) staff       (20)      117 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/atexit.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2074 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/audioop.pyi
--rw-r--r--   0 eve        (501) staff       (20)      903 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/base64.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4500 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/bdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      967 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/binascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1127 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/binhex.pyi
--rw-r--r--   0 eve        (501) staff       (20)       67 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)    48328 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/builtins.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1344 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/bz2.pyi
--rw-r--r--   0 eve        (501) staff       (20)      789 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cPickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1288 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cProfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1797 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cStringIO.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4934 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/calendar.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3957 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1307 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgitb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      613 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/chunk.pyi
--rw-r--r--   0 eve        (501) staff       (20)      875 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cmath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1596 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cmd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1060 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/code.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11793 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)      455 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/codeop.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4759 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/collections.pyi
--rw-r--r--   0 eve        (501) staff       (20)      552 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/colorsys.pyi
--rw-r--r--   0 eve        (501) staff       (20)      322 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/commands.pyi
--rw-r--r--   0 eve        (501) staff       (20)      549 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/compileall.pyi
--rw-r--r--   0 eve        (501) staff       (20)      906 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/contextlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4664 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cookielib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      309 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      794 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy_reg.pyi
--rw-r--r--   0 eve        (501) staff       (20)      794 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copyreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)       88 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/crypt.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2510 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/csv.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.234354 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/
--rw-r--r--   0 eve        (501) staff       (20)    11288 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      129 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4642 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ctypes/wintypes.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.234845 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/
--rw-r--r--   0 eve        (501) staff       (20)      356 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1127 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/ascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)      801 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/panel.pyi
--rw-r--r--   0 eve        (501) staff       (20)      431 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/curses/textpad.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7839 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/datetime.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.235555 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/
--rw-r--r--   0 eve        (501) staff       (20)      974 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      994 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1348 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/gnu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1222 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dbm/ndbm.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13228 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/decimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3521 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/difflib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      249 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dircache.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1044 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dis.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.239090 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      388 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/archive_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/bcppcompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6237 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/ccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2745 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cmd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.241514 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      242 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_packager.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_rpm.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_wininst.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_clib.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_ext.pyi
--rw-r--r--   0 eve        (501) staff       (20)      181 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_py.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/check.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/clean.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2882 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)      316 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_data.pyi
--rw-r--r--   0 eve        (501) staff       (20)      354 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_egg_info.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_lib.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/register.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/sdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      273 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/upload.pyi
--rw-r--r--   0 eve        (501) staff       (20)      497 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1637 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/core.pyi
--rw-r--r--   0 eve        (501) staff       (20)      138 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cygwinccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)       12 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/debug.pyi
--rw-r--r--   0 eve        (501) staff       (20)      220 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dep_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      530 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dir_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      470 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dist.pyi
--rw-r--r--   0 eve        (501) staff       (20)       90 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/emxccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      852 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      658 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/extension.pyi
--rw-r--r--   0 eve        (501) staff       (20)      805 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/fancy_getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      419 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/file_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)       20 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/filelist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      863 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/log.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/msvccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      186 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/spawn.pyi
--rw-r--r--   0 eve        (501) staff       (20)      586 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)      672 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/text_file.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/unixccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      841 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1132 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/version.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6694 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/doctest.pyi
--rw-r--r--   0 eve        (501) staff       (20)      762 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_threading.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.243311 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/
--rw-r--r--   0 eve        (501) staff       (20)      159 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/MIMEText.pyi
--rw-r--r--   0 eve        (501) staff       (20)      265 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1059 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/_parseaddr.pyi
--rw-r--r--   0 eve        (501) staff       (20)      303 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/base64mime.pyi
--rw-r--r--   0 eve        (501) staff       (20)      902 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/charset.pyi
--rw-r--r--   0 eve        (501) staff       (20)      143 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/encoders.pyi
--rw-r--r--   0 eve        (501) staff       (20)      536 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/feedparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      377 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/generator.pyi
--rw-r--r--   0 eve        (501) staff       (20)      457 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/header.pyi
--rw-r--r--   0 eve        (501) staff       (20)      256 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/iterators.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1950 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/message.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.244295 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      351 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/application.pyi
--rw-r--r--   0 eve        (501) staff       (20)      176 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/audio.pyi
--rw-r--r--   0 eve        (501) staff       (20)      128 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/base.pyi
--rw-r--r--   0 eve        (501) staff       (20)      176 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/image.pyi
--rw-r--r--   0 eve        (501) staff       (20)      147 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/message.pyi
--rw-r--r--   0 eve        (501) staff       (20)      159 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/multipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      107 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/nonmultipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      159 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)      415 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      490 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/quoprimime.pyi
--rw-r--r--   0 eve        (501) staff       (20)      738 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/utils.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.244519 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/
--rw-r--r--   0 eve        (501) staff       (20)      184 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      566 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/utf_8.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.244647 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ensurepip/
--rw-r--r--   0 eve        (501) staff       (20)      214 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ensurepip/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2011 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/errno.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1756 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/exceptions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1903 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fcntl.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1415 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/filecmp.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1479 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fileinput.pyi
--rw-r--r--   0 eve        (501) staff       (20)      329 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fnmatch.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4565 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/formatter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5216 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fractions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4847 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ftplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1112 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/functools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      194 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/future_builtins.pyi
--rw-r--r--   0 eve        (501) staff       (20)      739 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1082 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/genericpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      382 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      160 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getpass.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2190 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gettext.pyi
--rw-r--r--   0 eve        (501) staff       (20)      344 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/glob.pyi
--rw-r--r--   0 eve        (501) staff       (20)      345 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/grp.pyi
--rw-r--r--   0 eve        (501) staff       (20)      997 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gzip.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1059 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hashlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      719 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)      787 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hmac.pyi
--rw-r--r--   0 eve        (501) staff       (20)       89 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/htmlentitydefs.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5818 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/httplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6213 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imaplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      441 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imghdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1264 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imp.pyi
--rw-r--r--   0 eve        (501) staff       (20)      121 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/importlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4588 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/inspect.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1124 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/io.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5957 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/itertools.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3041 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/json.pyi
--rw-r--r--   0 eve        (501) staff       (20)       94 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/keyword.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.244955 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.245860 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      931 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/driver.pyi
--rw-r--r--   0 eve        (501) staff       (20)      683 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/grammar.pyi
--rw-r--r--   0 eve        (501) staff       (20)      166 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/literals.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1055 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2130 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/pgen.pyi
--rw-r--r--   0 eve        (501) staff       (20)      913 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)      870 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pgen2/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2208 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pygram.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3147 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/lib2to3/pytree.pyi
--rw-r--r--   0 eve        (501) staff       (20)      435 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/linecache.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2183 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/locale.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.246204 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/
--rw-r--r--   0 eve        (501) staff       (20)     9521 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      359 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4137 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1633 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/macpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      140 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/macurl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7507 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mailbox.pyi
--rw-r--r--   0 eve        (501) staff       (20)      282 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mailcap.pyi
--rw-r--r--   0 eve        (501) staff       (20)      238 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/markupbase.pyi
--rw-r--r--   0 eve        (501) staff       (20)      253 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/marshal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1979 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/math.pyi
--rw-r--r--   0 eve        (501) staff       (20)       74 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/md5.pyi
--rw-r--r--   0 eve        (501) staff       (20)      703 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetools.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1390 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetypes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1797 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mmap.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3072 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/modulefinder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.246653 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/
--rw-r--r--   0 eve        (501) staff       (20)     5847 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2141 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/schema.pyi
--rw-r--r--   0 eve        (501) staff       (20)      312 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/sequence.pyi
--rw-r--r--   0 eve        (501) staff       (20)      155 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msilib/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)      795 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/msvcrt.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.247118 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/
--rw-r--r--   0 eve        (501) staff       (20)     1890 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.247342 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/
--rw-r--r--   0 eve        (501) staff       (20)     1167 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      641 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/connection.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1957 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/pool.pyi
--rw-r--r--   0 eve        (501) staff       (20)      870 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/process.pyi
--rw-r--r--   0 eve        (501) staff       (20)      736 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      362 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mutex.pyi
--rw-r--r--   0 eve        (501) staff       (20)      515 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/netrc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      293 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nis.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4227 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nntplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2784 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ntpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      115 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nturl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3654 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/numbers.pyi
--rw-r--r--   0 eve        (501) staff       (20)      267 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/opcode.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7382 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/operator.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9977 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/optparse.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.247568 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/
--rw-r--r--   0 eve        (501) staff       (20)    11473 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2779 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2784 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os2emxpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3618 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ossaudiodev.pyi
--rw-r--r--   0 eve        (501) staff       (20)      927 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6493 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2093 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2941 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pickletools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      467 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pipes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1193 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pkgutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1786 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/platform.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1002 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/plistlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      960 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/popen2.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1410 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/poplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6345 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posix.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2784 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posixpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      878 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pprint.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1304 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/profile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1908 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pstats.pyi
--rw-r--r--   0 eve        (501) staff       (20)      482 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pty.pyi
--rw-r--r--   0 eve        (501) staff       (20)      405 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pwd.pyi
--rw-r--r--   0 eve        (501) staff       (20)      465 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/py_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)      645 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyclbr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10143 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.247753 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc_data/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc_data/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       23 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pydoc_data/topics.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.248256 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/
--rw-r--r--   0 eve        (501) staff       (20)     3184 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1152 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      205 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pyexpat/model.pyi
--rw-r--r--   0 eve        (501) staff       (20)      343 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/quopri.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3130 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/random.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3381 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/re.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1573 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/readline.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1089 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/repr.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1056 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/resource.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2147 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rfc822.pyi
--rw-r--r--   0 eve        (501) staff       (20)      325 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rlcompleter.pyi
--rw-r--r--   0 eve        (501) staff       (20)      230 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/robotparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      519 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/runpy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      725 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sched.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3551 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/select.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2813 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sets.pyi
--rw-r--r--   0 eve        (501) staff       (20)      236 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sha.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1603 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shelve.pyi
--rw-r--r--   0 eve        (501) staff       (20)      965 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shlex.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1791 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1271 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/signal.pyi
--rw-r--r--   0 eve        (501) staff       (20)      375 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/site.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1639 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtpd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2542 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      184 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sndhdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12509 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)      388 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/spwd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.248497 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sqlite3/
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sqlite3/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9542 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sqlite3/dbapi2.pyi
--rw-r--r--   0 eve        (501) staff       (20)      765 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1732 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2216 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9476 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ssl.pyi
--rw-r--r--   0 eve        (501) staff       (20)      992 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3501 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/string.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1985 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringold.pyi
--rw-r--r--   0 eve        (501) staff       (20)      817 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringprep.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1151 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/strop.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1021 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/struct.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3169 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2352 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sunau.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1316 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symbol.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1683 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symtable.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3524 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sys.pyi
--rw-r--r--   0 eve        (501) staff       (20)      820 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1019 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/syslog.pyi
--rw-r--r--   0 eve        (501) staff       (20)      413 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tabnanny.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9244 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tarfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2512 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/telnetlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3578 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tempfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4499 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/termios.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1842 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/textwrap.pyi
--rw-r--r--   0 eve        (501) staff       (20)       25 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/this.pyi
--rw-r--r--   0 eve        (501) staff       (20)      963 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3927 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1337 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/time.pyi
--rw-r--r--   0 eve        (501) staff       (20)      855 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/timeit.pyi
--rw-r--r--   0 eve        (501) staff       (20)      213 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/toaiff.pyi
--rw-r--r--   0 eve        (501) staff       (20)      874 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2660 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2424 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/trace.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1448 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/traceback.pyi
--rw-r--r--   0 eve        (501) staff       (20)      340 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tty.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17275 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/turtle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5356 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)    18009 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2910 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing_extensions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1620 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unicodedata.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12541 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unittest.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4714 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8224 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib2.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1890 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urlparse.pyi
--rw-r--r--   0 eve        (501) staff       (20)       83 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/user.pyi
--rw-r--r--   0 eve        (501) staff       (20)      306 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/uu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2373 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/uuid.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2017 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2081 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wave.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2842 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2997 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/webbrowser.pyi
--rw-r--r--   0 eve        (501) staff       (20)       72 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/whichdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      782 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/winsound.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.249253 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2996 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)      964 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1385 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/simple_server.pyi
--rw-r--r--   0 eve        (501) staff       (20)       71 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)      782 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1591 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/wsgiref/validate.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2309 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xdrlib.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.249364 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/
--rw-r--r--   0 eve        (501) staff       (20)       30 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.250272 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/
--rw-r--r--   0 eve        (501) staff       (20)      457 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/NodeFilter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1844 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      409 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/domreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)       77 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/expatbuilder.pyi
--rw-r--r--   0 eve        (501) staff       (20)      508 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/minicompat.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10318 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/minidom.pyi
--rw-r--r--   0 eve        (501) staff       (20)       77 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/pulldom.pyi
--rw-r--r--   0 eve        (501) staff       (20)      141 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/dom/xmlbuilder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.250824 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/
--rw-r--r--   0 eve        (501) staff       (20)      574 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/ElementInclude.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1516 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/ElementPath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8739 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/ElementTree.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       36 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/etree/cElementTree.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.250938 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/
--rw-r--r--   0 eve        (501) staff       (20)       34 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.251280 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/
--rw-r--r--   0 eve        (501) staff       (20)       22 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)       28 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/parsers/expat/model.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.251737 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/
--rw-r--r--   0 eve        (501) staff       (20)     1213 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1391 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/handler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2464 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/saxutils.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2424 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xml/sax/xmlreader.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9512 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xmlrpclib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3410 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/zipfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)      618 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/zipimport.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1214 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/zlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      914 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/__future__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       63 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/__main__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14688 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2510 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)       63 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bootlocale.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6813 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2123 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      356 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compat_pickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)      954 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compression.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2355 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_csv.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17284 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_curses.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13492 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_decimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1177 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5425 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)      324 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1149 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_imp.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1481 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_json.pyi
--rw-r--r--   0 eve        (501) staff       (20)      762 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_markupbase.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2217 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5907 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_operator.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1993 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_osx_support.pyi
--rw-r--r--   0 eve        (501) staff       (20)      647 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_posixsubprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)      378 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_py_abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      951 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_pydecimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)      404 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_random.pyi
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_sitebuiltins.pyi
--rw-r--r--   0 eve        (501) staff       (20)    16847 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2944 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_stat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1660 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)      552 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_threading_local.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3942 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tkinter.pyi
--rw-r--r--   0 eve        (501) staff       (20)      552 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tracemalloc.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.252430 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/
--rw-r--r--   0 eve        (501) staff       (20)     8558 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1638 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/dbapi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1623 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/wsgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)      490 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/xml.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1026 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1263 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2490 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7621 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/_winapi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1451 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3385 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/aifc.pyi
--rw-r--r--   0 eve        (501) staff       (20)       76 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/antigravity.pyi
--rw-r--r--   0 eve        (501) staff       (20)    19820 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/argparse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3685 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/array.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10501 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ast.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1099 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asynchat.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.257294 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/
--rw-r--r--   0 eve        (501) staff       (20)      722 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    21068 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1014 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_futures.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3270 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)      404 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_tasks.pyi
--rw-r--r--   0 eve        (501) staff       (20)       99 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/compat.pyi
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)      857 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/coroutines.pyi
--rw-r--r--   0 eve        (501) staff       (20)    27578 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1001 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/exceptions.pyi
--rw-r--r--   0 eve        (501) staff       (20)      886 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/format_helpers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3382 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/futures.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4380 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/locks.pyi
--rw-r--r--   0 eve        (501) staff       (20)       39 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/log.pyi
--rw-r--r--   0 eve        (501) staff       (20)      210 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/mixins.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3681 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/proactor_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1815 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/protocols.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1395 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/queues.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1006 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/runners.pyi
--rw-r--r--   0 eve        (501) staff       (20)      314 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/selector_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7275 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/sslproto.pyi
--rw-r--r--   0 eve        (501) staff       (20)      340 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/staggered.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7066 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/streams.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6097 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)      691 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/taskgroups.pyi
--rw-r--r--   0 eve        (501) staff       (20)    13461 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/tasks.pyi
--rw-r--r--   0 eve        (501) staff       (20)      265 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/threads.pyi
--rw-r--r--   0 eve        (501) staff       (20)      662 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/timeouts.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2361 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/transports.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4575 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/trsock.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6543 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/unix_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4077 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_events.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2476 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_utils.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3718 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncore.pyi
--rw-r--r--   0 eve        (501) staff       (20)      394 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/atexit.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2145 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/audioop.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2117 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/base64.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4670 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/bdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1825 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/binascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1269 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/binhex.pyi
--rw-r--r--   0 eve        (501) staff       (20)       67 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/bisect.pyi
--rw-r--r--   0 eve        (501) staff       (20)    77449 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/builtins.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4849 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/bz2.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1549 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cProfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6037 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/calendar.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4168 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgi.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1381 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgitb.pyi
--rw-r--r--   0 eve        (501) staff       (20)      613 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/chunk.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1324 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1750 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1443 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/code.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11547 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/codecs.pyi
--rw-r--r--   0 eve        (501) staff       (20)      516 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/codeop.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.257587 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/
--rw-r--r--   0 eve        (501) staff       (20)    20922 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      648 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/colorsys.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3340 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/compileall.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.257702 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.258342 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/
--rw-r--r--   0 eve        (501) staff       (20)      977 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5254 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/_base.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7135 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/process.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2285 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/thread.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10691 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/configparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8440 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1914 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextvars.pyi
--rw-r--r--   0 eve        (501) staff       (20)      350 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/copy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      995 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/copyreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)      532 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/crypt.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4661 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/csv.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.258918 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/
--rw-r--r--   0 eve        (501) staff       (20)    11583 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      129 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5232 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.259390 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/
--rw-r--r--   0 eve        (501) staff       (20)      622 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1393 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/ascii.pyi
--rw-r--r--   0 eve        (501) staff       (20)      931 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/panel.pyi
--rw-r--r--   0 eve        (501) staff       (20)      511 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/textpad.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7916 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dataclasses.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11113 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/datetime.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.260049 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/
--rw-r--r--   0 eve        (501) staff       (20)     1775 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1092 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1643 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/gnu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1429 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/ndbm.pyi
--rw-r--r--   0 eve        (501) staff       (20)      117 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/decimal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4525 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/difflib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4573 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dis.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.262935 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      548 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/archive_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/bcppcompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6315 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/ccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2758 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cmd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.265654 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      540 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      450 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_dumb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1489 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_packager.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1104 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi
--rw-r--r--   0 eve        (501) staff       (20)      638 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi
--rw-r--r--   0 eve        (501) staff       (20)      711 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build.pyi
--rw-r--r--   0 eve        (501) staff       (20)      668 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_clib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1257 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_ext.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1444 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_py.pyi
--rw-r--r--   0 eve        (501) staff       (20)      574 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)      961 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/check.pyi
--rw-r--r--   0 eve        (501) staff       (20)      377 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/clean.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2644 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1689 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install.pyi
--rw-r--r--   0 eve        (501) staff       (20)      436 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_data.pyi
--rw-r--r--   0 eve        (501) staff       (20)      490 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_egg_info.pyi
--rw-r--r--   0 eve        (501) staff       (20)      387 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)      598 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_lib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      426 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_scripts.pyi
--rw-r--r--   0 eve        (501) staff       (20)      569 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/register.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1118 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/sdist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      462 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/upload.pyi
--rw-r--r--   0 eve        (501) staff       (20)      497 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1664 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/core.pyi
--rw-r--r--   0 eve        (501) staff       (20)      138 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)       19 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/debug.pyi
--rw-r--r--   0 eve        (501) staff       (20)      220 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dep_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)      530 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dir_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2451 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      852 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1222 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/extension.pyi
--rw-r--r--   0 eve        (501) staff       (20)      966 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      428 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/file_util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2224 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/filelist.pyi
--rw-r--r--   0 eve        (501) staff       (20)      845 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/log.pyi
--rw-r--r--   0 eve        (501) staff       (20)       78 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/msvccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)      186 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/spawn.pyi
--rw-r--r--   0 eve        (501) staff       (20)      559 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)      679 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/text_file.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/unixccompiler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1549 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1361 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/version.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7634 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/doctest.pyi
--rw-r--r--   0 eve        (501) staff       (20)       79 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/dummy_threading.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.268076 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/
--rw-r--r--   0 eve        (501) staff       (20)     1032 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11761 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/_header_value_parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      400 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/base64mime.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1067 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/charset.pyi
--rw-r--r--   0 eve        (501) staff       (20)      516 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi
--rw-r--r--   0 eve        (501) staff       (20)      293 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/encoders.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1532 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      951 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/feedparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1329 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/generator.pyi
--rw-r--r--   0 eve        (501) staff       (20)      952 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/header.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5903 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/headerregistry.pyi
--rw-r--r--   0 eve        (501) staff       (20)      641 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/iterators.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5065 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/message.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.269307 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      472 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/application.pyi
--rw-r--r--   0 eve        (501) staff       (20)      466 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/audio.pyi
--rw-r--r--   0 eve        (501) staff       (20)      270 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/base.pyi
--rw-r--r--   0 eve        (501) staff       (20)      466 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/image.pyi
--rw-r--r--   0 eve        (501) staff       (20)      288 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/message.pyi
--rw-r--r--   0 eve        (501) staff       (20)      478 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/multipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      108 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/nonmultipart.pyi
--rw-r--r--   0 eve        (501) staff       (20)      273 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1449 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3055 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/policy.pyi
--rw-r--r--   0 eve        (501) staff       (20)      735 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/quoprimime.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2107 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/utils.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.269649 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/
--rw-r--r--   0 eve        (501) staff       (20)      306 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      825 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1232 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8_sig.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.269773 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/
--rw-r--r--   0 eve        (501) staff       (20)      257 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9490 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/enum.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2661 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/errno.pyi
--rw-r--r--   0 eve        (501) staff       (20)      644 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/faulthandler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3358 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fcntl.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1961 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/filecmp.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11065 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fileinput.pyi
--rw-r--r--   0 eve        (501) staff       (20)      339 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fnmatch.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4654 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/formatter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5365 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/fractions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6067 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ftplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6363 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/functools.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1326 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/gc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1750 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/genericpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      442 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/getopt.pyi
--rw-r--r--   0 eve        (501) staff       (20)      217 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/getpass.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6147 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/gettext.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1397 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/glob.pyi
--rw-r--r--   0 eve        (501) staff       (20)      913 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/graphlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      730 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/grp.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4956 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/gzip.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5546 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/hashlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      712 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/heapq.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1506 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/hmac.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.270306 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/
--rw-r--r--   0 eve        (501) staff       (20)      156 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      182 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/entities.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1846 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/parser.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.270884 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/
--rw-r--r--   0 eve        (501) staff       (20)     2407 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7659 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/client.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7478 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookiejar.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2414 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookies.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3895 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/server.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7693 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/imaplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      500 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/imghdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2376 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/imp.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.271430 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/
--rw-r--r--   0 eve        (501) staff       (20)      800 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7512 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5770 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.271655 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata/
--rw-r--r--   0 eve        (501) staff       (20)     6609 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      752 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1497 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/resources.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1872 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17776 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/inspect.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8007 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/io.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7131 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ipaddress.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10786 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/itertools.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.272086 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/
--rw-r--r--   0 eve        (501) staff       (20)     1981 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1113 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/decoder.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1035 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/encoder.pyi
--rw-r--r--   0 eve        (501) staff       (20)       24 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/tool.pyi
--rw-r--r--   0 eve        (501) staff       (20)      357 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/keyword.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.272500 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.273388 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      984 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi
--rw-r--r--   0 eve        (501) staff       (20)      724 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi
--rw-r--r--   0 eve        (501) staff       (20)      155 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/literals.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1119 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2135 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1005 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2073 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2208 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pygram.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3206 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pytree.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3278 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/refactor.pyi
--rw-r--r--   0 eve        (501) staff       (20)      941 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/linecache.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3784 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/locale.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.273770 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/
--rw-r--r--   0 eve        (501) staff       (20)    26790 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2360 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/config.pyi
--rw-r--r--   0 eve        (501) staff       (20)     9838 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5435 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/lzma.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2405 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/macpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)      184 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/macurl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10420 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailbox.pyi
--rw-r--r--   0 eve        (501) staff       (20)      378 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailcap.pyi
--rw-r--r--   0 eve        (501) staff       (20)      253 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/marshal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4584 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/math.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1985 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mimetypes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3766 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/mmap.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3606 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/modulefinder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.274220 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/
--rw-r--r--   0 eve        (501) staff       (20)     6071 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2141 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/schema.pyi
--rw-r--r--   0 eve        (501) staff       (20)      363 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/sequence.pyi
--rw-r--r--   0 eve        (501) staff       (20)      155 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/text.pyi
--rw-r--r--   0 eve        (501) staff       (20)      840 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/msvcrt.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.275584 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/
--rw-r--r--   0 eve        (501) staff       (20)     5177 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2467 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/connection.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7459 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/context.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.275810 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/
--rw-r--r--   0 eve        (501) staff       (20)     1958 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1335 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8556 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/managers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4755 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/pool.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1371 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/process.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1398 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/queues.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2619 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/reduction.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1348 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4000 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi
--rw-r--r--   0 eve        (501) staff       (20)      859 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/spawn.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2278 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi
--rw-r--r--   0 eve        (501) staff       (20)      639 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/netrc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      293 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/nis.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4457 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/nntplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2815 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ntpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)       76 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/nturl2path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3912 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/numbers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1228 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/opcode.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1645 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/operator.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10273 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/optparse.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.276095 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/
--rw-r--r--   0 eve        (501) staff       (20)    36999 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      186 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/path.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3618 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ossaudiodev.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1046 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/parser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7828 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pathlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7494 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pdb.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6773 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickle.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3777 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickletools.pyi
--rw-r--r--   0 eve        (501) staff       (20)      538 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pipes.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1610 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pkgutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2327 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/platform.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3976 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/plistlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2149 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/poplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10709 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/posix.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4241 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/posixpath.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3835 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pprint.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1413 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/profile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2994 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pstats.pyi
--rw-r--r--   0 eve        (501) staff       (20)      679 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pty.pyi
--rw-r--r--   0 eve        (501) staff       (20)      931 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pwd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1574 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/py_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2198 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyclbr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10457 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.276283 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       23 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/topics.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.276613 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/
--rw-r--r--   0 eve        (501) staff       (20)     3374 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1477 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)      205 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/model.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2219 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/queue.pyi
--rw-r--r--   0 eve        (501) staff       (20)      407 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/quopri.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4767 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/random.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5091 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/re.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1854 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/readline.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1340 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/reprlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2763 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/resource.pyi
--rw-r--r--   0 eve        (501) staff       (20)      321 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/rlcompleter.pyi
--rw-r--r--   0 eve        (501) staff       (20)      774 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/runpy.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1339 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sched.pyi
--rw-r--r--   0 eve        (501) staff       (20)      621 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/secrets.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4559 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/select.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3714 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/selectors.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1724 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/shelve.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1545 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/shlex.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6435 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/shutil.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5287 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/signal.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1355 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/site.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2978 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtpd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6168 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtplib.pyi
--rw-r--r--   0 eve        (501) staff       (20)      353 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sndhdr.pyi
--rw-r--r--   0 eve        (501) staff       (20)    23499 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/socket.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6364 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/socketserver.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1180 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/spwd.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.276828 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    16847 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi
--rw-r--r--   0 eve        (501) staff       (20)      320 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_compile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3982 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4130 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)    18944 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/ssl.pyi
--rw-r--r--   0 eve        (501) staff       (20)       20 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/stat.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4922 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/statistics.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2011 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/string.pyi
--rw-r--r--   0 eve        (501) staff       (20)      910 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/stringprep.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1287 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/struct.pyi
--rw-r--r--   0 eve        (501) staff       (20)    58351 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/subprocess.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2870 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sunau.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1566 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/symbol.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2391 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/symtable.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11053 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sys.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1085 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/sysconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1357 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/syslog.pyi
--rw-r--r--   0 eve        (501) staff       (20)      514 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tabnanny.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12696 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tarfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2809 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/telnetlib.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14679 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tempfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4753 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/termios.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3190 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/textwrap.pyi
--rw-r--r--   0 eve        (501) staff       (20)       25 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/this.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6178 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/threading.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3789 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/time.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1197 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/timeit.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.279094 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/
--rw-r--r--   0 eve        (501) staff       (20)   135621 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      335 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/colorchooser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      355 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/commondialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1886 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/constants.pyi
--rw-r--r--   0 eve        (501) staff       (20)      361 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)      724 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dnd.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5130 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/filedialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4039 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/font.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1350 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/messagebox.pyi
--rw-r--r--   0 eve        (501) staff       (20)      329 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/scrolledtext.pyi
--rw-r--r--   0 eve        (501) staff       (20)      970 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/simpledialog.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14753 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/tix.pyi
--rw-r--r--   0 eve        (501) staff       (20)    44937 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/ttk.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2625 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/token.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4546 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tokenize.pyi
--rw-r--r--   0 eve        (501) staff       (20)      374 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tomllib.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2759 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/trace.pyi
--rw-r--r--   0 eve        (501) staff       (20)     8798 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/traceback.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4488 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tracemalloc.pyi
--rw-r--r--   0 eve        (501) staff       (20)      434 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/tty.pyi
--rw-r--r--   0 eve        (501) staff       (20)    21951 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/turtle.pyi
--rw-r--r--   0 eve        (501) staff       (20)    21717 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)    34098 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7844 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1864 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unicodedata.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.280527 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/
--rw-r--r--   0 eve        (501) staff       (20)     1840 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      892 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/_log.pyi
--rw-r--r--   0 eve        (501) staff       (20)      663 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/async_case.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14516 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/case.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2161 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/loader.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1669 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/main.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14446 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1718 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1384 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi
--rw-r--r--   0 eve        (501) staff       (20)      487 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi
--rw-r--r--   0 eve        (501) staff       (20)      982 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi
--rw-r--r--   0 eve        (501) staff       (20)      976 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/util.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.281236 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      768 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/error.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5682 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi
--rw-r--r--   0 eve        (501) staff       (20)    17137 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/request.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2250 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/response.pyi
--rw-r--r--   0 eve        (501) staff       (20)      734 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/robotparser.pyi
--rw-r--r--   0 eve        (501) staff       (20)      593 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/uu.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2645 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/uuid.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.281353 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/
--rw-r--r--   0 eve        (501) staff       (20)     2579 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3654 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/warnings.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2723 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wave.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5833 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/weakref.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2567 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/webbrowser.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4368 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/winreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)      898 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/winsound.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.282229 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3064 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/handlers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1020 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/headers.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1465 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/simple_server.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1248 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/types.pyi
--rw-r--r--   0 eve        (501) staff       (20)      993 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/util.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1658 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/validate.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2398 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xdrlib.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.282339 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/
--rw-r--r--   0 eve        (501) staff       (20)       30 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.283288 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/
--rw-r--r--   0 eve        (501) staff       (20)      457 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/NodeFilter.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1889 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)      418 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/domreg.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4570 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi
--rw-r--r--   0 eve        (501) staff       (20)      606 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minicompat.pyi
--rw-r--r--   0 eve        (501) staff       (20)    11646 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minidom.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3407 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/pulldom.pyi
--rw-r--r--   0 eve        (501) staff       (20)     4237 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.283841 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/
--rw-r--r--   0 eve        (501) staff       (20)      935 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1616 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi
--rw-r--r--   0 eve        (501) staff       (20)    14083 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       36 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/cElementTree.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.283960 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/
--rw-r--r--   0 eve        (501) staff       (20)       34 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.284326 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/
--rw-r--r--   0 eve        (501) staff       (20)       22 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)       29 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/errors.pyi
--rw-r--r--   0 eve        (501) staff       (20)       28 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/model.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.284803 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/
--rw-r--r--   0 eve        (501) staff       (20)     1553 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1730 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/handler.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2496 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/saxutils.pyi
--rw-r--r--   0 eve        (501) staff       (20)     2433 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.285118 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)    12334 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/client.pyi
--rw-r--r--   0 eve        (501) staff       (20)     6813 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/server.pyi
--rw-r--r--   0 eve        (501) staff       (20)      338 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/xxlimited.pyi
--rw-r--r--   0 eve        (501) staff       (20)      777 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipapp.pyi
--rw-r--r--   0 eve        (501) staff       (20)    10985 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipfile.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1321 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipimport.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1743 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zlib.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.285235 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/
--rw-r--r--   0 eve        (501) staff       (20)     1241 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.007690 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stubs/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.285348 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/
--rw-r--r--   0 eve        (501) staff       (20)     2262 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.007784 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypyc/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.007820 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypyc/test-data/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.285563 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypyc/test-data/fixtures/
--rw-r--r--   0 eve        (501) staff       (20)     4902 2022-08-10 21:22:18.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/mypyc/test-data/fixtures/typing-full.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.286637 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/
--rw-r--r--   0 eve        (501) staff       (20)      341 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/__init__.pyi
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.007968 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/_vendored_packages/
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.286751 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/__init__.pyi
--rw-r--r--   0 eve        (501) staff       (20)     3409 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/error.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1205 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/iniconfig.pyi
--rw-r--r--   0 eve        (501) staff       (20)     5277 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/io.pyi
--rw-r--r--   0 eve        (501) staff       (20)     7168 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/path.pyi
--rw-r--r--   0 eve        (501) staff       (20)      787 2022-08-10 21:22:25.000000 hexbytes-0.3.0/.tox/py39-lint/lib/python3.9/site-packages/py/xml.pyi
--rw-r--r--   0 eve        (501) staff       (20)     1090 2022-08-08 16:52:51.000000 hexbytes-0.3.0/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      160 2022-08-08 16:52:51.000000 hexbytes-0.3.0/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     4801 2022-08-17 16:24:52.288131 hexbytes-0.3.0/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     3796 2022-08-08 16:52:51.000000 hexbytes-0.3.0/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.287365 hexbytes-0.3.0/hexbytes/
--rw-r--r--   0 eve        (501) staff       (20)       60 2022-08-08 20:46:53.000000 hexbytes-0.3.0/hexbytes/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1687 2022-08-11 19:47:41.000000 hexbytes-0.3.0/hexbytes/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1954 2022-08-11 19:47:41.000000 hexbytes-0.3.0/hexbytes/main.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-08 16:52:51.000000 hexbytes-0.3.0/hexbytes/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-08-17 16:24:52.287962 hexbytes-0.3.0/hexbytes.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     4801 2022-08-17 16:24:50.000000 hexbytes-0.3.0/hexbytes.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)   152023 2022-08-17 16:24:51.000000 hexbytes-0.3.0/hexbytes.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2022-08-17 16:24:50.000000 hexbytes-0.3.0/hexbytes.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2022-08-17 16:24:50.000000 hexbytes-0.3.0/hexbytes.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)      555 2022-08-17 16:24:50.000000 hexbytes-0.3.0/hexbytes.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)        9 2022-08-17 16:24:50.000000 hexbytes-0.3.0/hexbytes.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1129 2022-08-08 16:52:51.000000 hexbytes-0.3.0/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       14 2022-08-08 16:52:51.000000 hexbytes-0.3.0/requirements-docs.txt
--rw-r--r--   0 eve        (501) staff       (20)       38 2022-08-17 16:24:52.288292 hexbytes-0.3.0/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     2247 2022-08-17 16:24:08.000000 hexbytes-0.3.0/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:36:12.615462 hexbytes-0.3.1/
+-rw-r--r--   0 eve        (501) staff       (20)     1090 2022-08-08 16:52:51.000000 hexbytes-0.3.1/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      141 2023-06-08 20:29:36.000000 hexbytes-0.3.1/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     3897 2023-06-08 20:36:12.615338 hexbytes-0.3.1/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     2861 2023-06-08 20:29:36.000000 hexbytes-0.3.1/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:36:12.614634 hexbytes-0.3.1/hexbytes/
+-rw-r--r--   0 eve        (501) staff       (20)       60 2022-08-08 20:46:53.000000 hexbytes-0.3.1/hexbytes/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1687 2022-08-11 19:47:41.000000 hexbytes-0.3.1/hexbytes/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     2004 2023-06-08 20:29:36.000000 hexbytes-0.3.1/hexbytes/main.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-08-08 16:52:51.000000 hexbytes-0.3.1/hexbytes/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-08 20:36:12.615194 hexbytes-0.3.1/hexbytes.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     3897 2023-06-08 20:36:11.000000 hexbytes-0.3.1/hexbytes.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)      318 2023-06-08 20:36:12.000000 hexbytes-0.3.1/hexbytes.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 20:36:11.000000 hexbytes-0.3.1/hexbytes.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-08 20:36:09.000000 hexbytes-0.3.1/hexbytes.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)      562 2023-06-08 20:36:11.000000 hexbytes-0.3.1/hexbytes.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)        9 2023-06-08 20:36:11.000000 hexbytes-0.3.1/hexbytes.egg-info/top_level.txt
+-rw-r--r--   0 eve        (501) staff       (20)     1129 2022-08-08 16:52:51.000000 hexbytes-0.3.1/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-06-08 20:36:12.615498 hexbytes-0.3.1/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     2314 2023-06-08 20:35:36.000000 hexbytes-0.3.1/setup.py
```

### Comparing `hexbytes-0.3.0/LICENSE` & `hexbytes-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexbytes-0.3.0/PKG-INFO` & `hexbytes-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: hexbytes
-Version: 0.3.0
+Version: 0.3.1
 Summary: hexbytes: Python `bytes` subclass that decodes hex, with a readable console output
 Home-page: https://github.com/ethereum/hexbytes
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # HexBytes
 
-[![Join the chat at https://gitter.im/ethereum/web3.py](https://badges.gitter.im/ethereum/web3.py.svg)](https://gitter.im/ethereum/web3.py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![Build Status](https://circleci.com/gh/ethereum/hexbytes.svg?style=shield)](https://circleci.com/gh/ethereum/hexbytes)
 [![PyPI version](https://badge.fury.io/py/hexbytes.svg)](https://badge.fury.io/py/hexbytes)
 [![Python versions](https://img.shields.io/pypi/pyversions/hexbytes.svg)](https://pypi.python.org/pypi/hexbytes)
 [![Docs build](https://readthedocs.org/projects/hexbytes/badge/?version=latest)](http://hexbytes.readthedocs.io/en/latest/?badge=latest)
    
 
 Python `bytes` subclass that decodes hex, with a readable console output
@@ -84,51 +83,19 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:carver/hexbytes.git
 cd hexbytes
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 hexbytes/ tests/ -c "clear; flake8 hexbytes tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on hexbytes failed'" ../tests ../hexbytes
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
@@ -141,9 +108,7 @@
 master branch, except when releasing a beta (in which case the beta is released from master,
 and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hexbytes-0.3.0/README.md` & `hexbytes-0.3.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # HexBytes
 
-[![Join the chat at https://gitter.im/ethereum/web3.py](https://badges.gitter.im/ethereum/web3.py.svg)](https://gitter.im/ethereum/web3.py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![Build Status](https://circleci.com/gh/ethereum/hexbytes.svg?style=shield)](https://circleci.com/gh/ethereum/hexbytes)
 [![PyPI version](https://badge.fury.io/py/hexbytes.svg)](https://badge.fury.io/py/hexbytes)
 [![Python versions](https://img.shields.io/pypi/pyversions/hexbytes.svg)](https://pypi.python.org/pypi/hexbytes)
 [![Docs build](https://readthedocs.org/projects/hexbytes/badge/?version=latest)](http://hexbytes.readthedocs.io/en/latest/?badge=latest)
    
 
 Python `bytes` subclass that decodes hex, with a readable console output
@@ -55,51 +54,19 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:carver/hexbytes.git
 cd hexbytes
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 hexbytes/ tests/ -c "clear; flake8 hexbytes tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on hexbytes failed'" ../tests ../hexbytes
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hexbytes-0.3.0/hexbytes/_utils.py` & `hexbytes-0.3.1/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `hexbytes-0.3.0/hexbytes/main.py` & `hexbytes-0.3.1/hexbytes/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,21 @@
     to_bytes,
 )
 
 if TYPE_CHECKING:
     # remove once hexbytes supports python>=3.8
     # Types was added to typing in 3.8
     if sys.version_info >= (3, 8):
-        from typing import SupportsIndex
+        from typing import (
+            SupportsIndex,
+        )
     else:
-        from typing_extensions import SupportsIndex  # noqa: F401
+        from typing_extensions import (  # noqa: F401
+            SupportsIndex,
+        )
 
 
 BytesLike = Union[bool, bytearray, bytes, int, str, memoryview]
 
 
 class HexBytes(bytes):
     """
```

### Comparing `hexbytes-0.3.0/hexbytes.egg-info/PKG-INFO` & `hexbytes-0.3.1/hexbytes.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: hexbytes
-Version: 0.3.0
+Version: 0.3.1
 Summary: hexbytes: Python `bytes` subclass that decodes hex, with a readable console output
 Home-page: https://github.com/ethereum/hexbytes
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # HexBytes
 
-[![Join the chat at https://gitter.im/ethereum/web3.py](https://badges.gitter.im/ethereum/web3.py.svg)](https://gitter.im/ethereum/web3.py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![Build Status](https://circleci.com/gh/ethereum/hexbytes.svg?style=shield)](https://circleci.com/gh/ethereum/hexbytes)
 [![PyPI version](https://badge.fury.io/py/hexbytes.svg)](https://badge.fury.io/py/hexbytes)
 [![Python versions](https://img.shields.io/pypi/pyversions/hexbytes.svg)](https://pypi.python.org/pypi/hexbytes)
 [![Docs build](https://readthedocs.org/projects/hexbytes/badge/?version=latest)](http://hexbytes.readthedocs.io/en/latest/?badge=latest)
    
 
 Python `bytes` subclass that decodes hex, with a readable console output
@@ -84,51 +83,19 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:carver/hexbytes.git
 cd hexbytes
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 hexbytes/ tests/ -c "clear; flake8 hexbytes tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on hexbytes failed'" ../tests ../hexbytes
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
@@ -141,9 +108,7 @@
 master branch, except when releasing a beta (in which case the beta is released from master,
 and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hexbytes-0.3.0/pyproject.toml` & `hexbytes-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexbytes-0.3.0/setup.py` & `hexbytes-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 from setuptools import (
     setup,
     find_packages,
 )
 
 extras_require = {
     "test": [
-        "pytest>=7,<8",
-        "pytest-xdist",
-        "tox>=3.25.1,<4",
+        "pytest>=7.0.0",
+        "pytest-xdist>=2.4.0",
         "hypothesis>=3.44.24,<=6.31.6",
         "eth-utils>=1.0.1,<3",
     ],
     "lint": [
-        "flake8==3.7.9",
-        "isort>=4.2.15,<5",
+        "flake8==6.0.0",
+        "flake8-bugbear==23.3.23",
+        "isort>=5.10.1",
         "mypy==0.971",
-        "pydocstyle>=5.0.0,<6",
-        "black>=22,<23",
+        "pydocstyle>=5.0.0",
+        "black>=22",
     ],
     "doc": [
-        "Sphinx>=4.0.0,<5",
-        "sphinx_rtd_theme>=0.1.9,<1",
+        "sphinx>=5.0.0",
+        "sphinx_rtd_theme>=1.0.0",
         "towncrier>=21,<22",
     ],
     "dev": [
-        "bumpversion>=0.5.3,<1",
-        "pytest-watch>=4.1.0,<5",
+        "bumpversion>=0.5.3",
+        "pytest-watch>=4.1.0",
+        "tox>=4.0.0",
         "wheel",
         "twine",
         "ipython",
     ],
 }
 
 extras_require["dev"] = (
@@ -45,15 +46,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="hexbytes",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="0.3.0",
+    version="0.3.1",
     description="""hexbytes: Python `bytes` subclass that decodes hex, with a readable console output""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/hexbytes",
     include_package_data=True,
@@ -74,9 +75,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

