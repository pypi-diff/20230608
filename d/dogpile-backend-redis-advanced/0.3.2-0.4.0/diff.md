# Comparing `tmp/dogpile_backend_redis_advanced-0.3.2.tar.gz` & `tmp/dogpile_backend_redis_advanced-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dogpile_backend_redis_advanced-0.3.2.tar", last modified: Thu Mar 25 21:46:55 2021, max compression
+gzip compressed data, was "dogpile_backend_redis_advanced-0.4.0.tar", last modified: Wed Jun  7 22:11:34 2023, max compression
```

## Comparing `dogpile_backend_redis_advanced-0.3.2.tar` & `dogpile_backend_redis_advanced-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1191 2021-03-25 21:44:22.000000 dogpile_backend_redis_advanced-0.3.2/CHANGELOG.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1569 2016-08-11 23:29:06.000000 dogpile_backend_redis_advanced-0.3.2/LICENSE
--rw-r--r--   0 jvanasco   (501) admin       (80)      181 2021-03-25 21:43:09.000000 dogpile_backend_redis_advanced-0.3.2/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)    25382 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-14 23:11:00.000000 dogpile_backend_redis_advanced-0.3.2/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)    20595 2020-11-18 18:53:35.000000 dogpile_backend_redis_advanced-0.3.2/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)      271 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     2298 2021-03-25 21:44:51.000000 dogpile_backend_redis_advanced-0.3.2/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/
--rw-r--r--   0 jvanasco   (501) admin       (80)      423 2021-03-25 21:44:03.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/cache/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2016-08-11 16:25:37.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/cache/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/cache/backends/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2016-08-11 17:13:24.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/cache/backends/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    16152 2020-10-02 15:40:12.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/cache/backends/redis_advanced.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 21:46:54.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 21:45:05.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)    25382 2021-03-25 21:46:54.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2021-03-25 21:46:54.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      780 2021-03-25 21:46:54.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       31 2021-03-25 21:46:54.000000 dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2013-11-26 16:52:29.000000 dogpile_backend_redis_advanced-0.3.2/tests/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 21:46:55.000000 dogpile_backend_redis_advanced-0.3.2/tests/cache/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1195 2019-09-19 20:29:21.000000 dogpile_backend_redis_advanced-0.3.2/tests/cache/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    12235 2019-09-19 20:29:22.000000 dogpile_backend_redis_advanced-0.3.2/tests/cache/_fixtures.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    25319 2020-10-02 15:40:14.000000 dogpile_backend_redis_advanced-0.3.2/tests/cache/test_redis_backend.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1073 2020-10-02 19:43:34.000000 dogpile_backend_redis_advanced-0.3.2/tests/conftest.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      850 2020-10-14 23:25:10.000000 dogpile_backend_redis_advanced-0.3.2/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.188700 dogpile_backend_redis_advanced-0.4.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1317 2023-05-11 19:03:48.000000 dogpile_backend_redis_advanced-0.4.0/CHANGELOG.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1569 2016-08-11 23:29:06.000000 dogpile_backend_redis_advanced-0.4.0/LICENSE
+-rw-r--r--   0 jvanasco   (501) admin       (80)      181 2021-03-25 21:43:09.000000 dogpile_backend_redis_advanced-0.4.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)    21665 2023-06-07 22:11:34.189090 dogpile_backend_redis_advanced-0.4.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)    20737 2021-05-24 20:14:15.000000 dogpile_backend_redis_advanced-0.4.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-07 22:10:26.000000 dogpile_backend_redis_advanced-0.4.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      491 2023-06-07 22:11:34.190804 dogpile_backend_redis_advanced-0.4.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2594 2023-05-11 19:03:48.000000 dogpile_backend_redis_advanced-0.4.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.153245 dogpile_backend_redis_advanced-0.4.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.166311 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      447 2023-05-11 19:03:48.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.177647 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/cache/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2016-08-11 16:25:37.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/cache/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.179597 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/cache/backends/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2016-08-11 17:13:24.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/cache/backends/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    16806 2023-06-07 22:10:26.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/cache/backends/redis_advanced.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.176495 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    21665 2023-06-07 22:11:34.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      780 2023-06-07 22:11:34.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-07 22:11:34.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 21:45:05.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       52 2023-06-07 22:11:34.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       31 2023-06-07 22:11:34.000000 dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.181667 dogpile_backend_redis_advanced-0.4.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2013-11-26 16:52:29.000000 dogpile_backend_redis_advanced-0.4.0/tests/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-07 22:11:34.187041 dogpile_backend_redis_advanced-0.4.0/tests/cache/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1030 2023-05-11 19:03:48.000000 dogpile_backend_redis_advanced-0.4.0/tests/cache/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    12235 2019-09-19 20:29:22.000000 dogpile_backend_redis_advanced-0.4.0/tests/cache/_fixtures.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    25027 2023-05-11 19:03:48.000000 dogpile_backend_redis_advanced-0.4.0/tests/cache/test_redis_backend.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      954 2023-05-11 19:03:48.000000 dogpile_backend_redis_advanced-0.4.0/tests/conftest.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      906 2023-05-11 19:03:48.000000 dogpile_backend_redis_advanced-0.4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/CHANGELOG.txt` & `dogpile_backend_redis_advanced-0.4.0/CHANGELOG.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+v0.4.0
+    initial typing support
+    drop py2
+
+v0.3.3
+	improving py3 support
+	some prep for py2/py3 on "dogpile.cache>=1.0"
+
 v0.3.2
 	packaging fixes
 
 v0.3.1 
 	moving ancillary files into /experiments
 	committed some untracked experiments
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/LICENSE` & `dogpile_backend_redis_advanced-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dogpile_backend_redis_advanced-0.3.2/PKG-INFO` & `dogpile_backend_redis_advanced-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,532 +1,515 @@
-Metadata-Version: 2.1
-Name: dogpile_backend_redis_advanced
-Version: 0.3.2
-Summary: Advanced Redis plugins for `dogpile.cache`.
-Home-page: https://github.com/jvanasco/dogpile_backend_redis_advanced
-Author: Jonathan Vanasco
-Author-email: jonathan@findmeon.com
-License: BSD
-Description: ![Python package](https://github.com/jvanasco/dogpile_backend_redis_advanced/workflows/Python%20package/badge.svg)
-        
-        This package supports Python2 and Python3
-        
-        dogpile_backend_redis_advanced
-        ==============================
-        
-        This is a plugin for the **dogpile.cache** system that offers some alternatives
-        to the standard **Redis** datastore implementation.
-        
-        Two new backends are offered:
-        
-        | backend | description |
-        | --- | --- |
-        | `dogpile_backend_redis_advanced` | extends the `dogpile.cache.redis` backend and allows for custom pickling overrides |
-        | `dogpile_backend_redis_advanced_hstore` | extends `dogpile_backend_redis_advanced` and allows for some specific hstore operations |
-        
-        There is a negligible performance hit in `dogpile_backend_redis_advanced_hstore`,
-        as cache keys must be inspected to determine if they are an hstore or not -- and
-        there are some operations involved to coordinate values.
-        
-        Additionally, some behavior is changed:
-        
-        * The constructor now accepts a ``lock_class`` argument, which can be used to
-          wrap a mutex and alter how releases are handled.  This can be necessary if you
-          have a distributed lock and timeout or flush issues (via LRU or otherwise).
-          A lock disappearing in Redis will raise a fatal exception under the standard
-          Redis backend.
-        * The constructor now accepts a ``lock_prefix`` argument, which can be used to
-          alter the prefix used for locks.  The standard Redis backend uses `_lock` as
-          the prefix -- which can be hard to read or isolate for tests.  One might want
-          to use "\_" as the lock prefix (so that `keys "\_*"` will show all locks).
-        
-        Purpose:
-        --------
-        
-        Mike Bayer's **dogpile.cache** is an excellent package for general purpose
-        development.
-        
-        The system offers 3 key features:
-        
-        1. Elegant read-through caching functionality.
-        2. A locking mechanism that ensures only the first request of a cache-miss will
-           create the resource (turning the rest into consumers of the first-requestor's
-           creation).
-        3. Integrated cache expiry against time and library versions.
-        
-        
-        Unfortunately, the integrated cache expiry feature comes at a cost -- objects
-        are wrapped into a tuple with some metadata and pickled before hitting the
-        datastore.
-        
-        The additional metadata or pickle format may not be needed or wanted.  Look how
-        the size of "a" grows by the time it becomes something passed off to Redis:
-        
-        
-        | type  | example |
-        | ----- | ------- |
-        | string                        | a                                                                                                               |
-        | pickle(string)                | S'a'\np0\n.                                                                                                     |
-        | CachedValue(string)           | ('a', {'ct': 1471113698.76127, 'v': 1})                                                                         |
-        | pickle(CachedValue(string) )  | cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n. |
-        
-        By adding in hooks for custom serializers, this backend lets developers choose
-        better ways to cache data.  
-        
-        You may want a serializer that doesn't care about the expiry of cached data, so
-        just uses simpler strings.:
-        
-        | type  | example 1 | example 2 |
-        | ----- | --------- | --------- |
-        | string                                | a                         | mellifluous                         |
-        | json.dumps(string)                    | "a"                       | "mellifluous"                       |
-        | msgpack.packb(string)                 | \xa1a                     | \xabmellifluous                     |
-        
-        Or, you may want to fool **dogpile.cache** by manipulating what the cached is. 
-        Instead of using a Python dict, of time and API version, you might just track
-        the time but only to the second. 
-        
-        | type | example 1 | example 2 |
-        | ---- | --------- | --------- |
-        | AltCachedValue(string)                | ('a', 1471113698)         | ('mellifluous', 1471113698)         |
-        | json.dumps(AltCachedValue(string))    | '["a", 1471113698]'       | '["mellifluous", 1471113698]'       |
-        | msgpack.packb(AltCachedValue(string)) | '\x92\xa1a\xceW\xafi\xe2' | '\x92\xabmellifluous\xceW\xafi\xe2' |
-        
-        
-        This is how **dogpile.cache** stores "a":
-        
-        	cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n.
-        
-        This package lets us cache a raw string and trick **dogpile.cache** into
-        thinking our data parcel is "timely":
-        
-        	a
-        
-        Or, we include a simpler version of the time, along with a different serializer.
-        
-        This packet of data and time:
-        
-        	["a", 1471113698]
-        
-        Is then serialized to:
-        
-        	\x92\xa1a\xceW\xafi\xe2
-        	
-        If you cache lots of big objects, **dogpile.cache**'s overhead is minimal -- but
-        if you have a cache that works for mapping short bits of text, like ids to
-        usernames (and vice-versa) you will see considerable savings.
-        
-        Another way to make **Redis** more efficient is to use hash storage.
-        
-        Let's say you have a lot of keys that look like this:
-        
-        	region.set("user-15|posts", x)
-        	region.set("user-15|friends", y)
-        	region.set("user-15|profile", z)
-        	region.set("user-15|username", z1)
-        
-        You could make **Redis** a bit more efficient by using hash storage, in which
-        you have 1 key with multiple fields:
-        
-        	region.hset("user-15", {'posts': x,
-        							'friends', y,
-        							'profile', z,
-        							'username', z1,
-        							})
-        
-        Redis tends to operate much more efficiently in this situation (more below),
-        but you can also save some bytes by not repeating the key prefix. Instagram's
-        engineering team has a great article on this
-        [Instagram Engineering](http://instagram-engineering.tumblr.com/post/12202313862/storing-hundreds-of-millions-of-simple-key-value).
-        
-        90% of **dogpile.cache** users who choose **Redis** will never need this
-        package.  A decent number of other users with large datasets have been trying to
-        squeeze every last bit of memory and performance out of their machines -- and
-        this package is designed to facilitate that.
-        
-        
-        Usage:
-        ------
-        
-        myfile.py
-        
-            # importing will register the plugins
-            import dogpile_backend_redis_advanced
-        
-        then simply configure **dogpile.cache** with `dogpile_backend_redis_advanced` or 
-        `dogpile_backend_redis_advanced_hstore` as the backend.
-        
-        
-        RedisAdvancedBackend
-        --------------------
-        
-        Two new configuration options are offered to specify custom serializers via 
-        `loads` and `dumps`.  The default selection is to use **dogpile.cache**'s choice
-        of  `pickle`.
-        
-        This option was designed to support `msgpack` as the serializer:
-        
-            import msgpack
-            from dogpile.cache.api import CachedValue
-        
-            def msgpack_loads(value):
-                """pickle maintained the `CachedValue` wrapper of the tuple
-                   msgpack does not, so it must be added back in.
-                   """
-                value = msgpack.unpackb(value, use_list=False)
-                return CachedValue(*value)
-        
-            region = make_region().configure(
-                arguments= {'loads': msgpack_loads,
-                            'dumps': msgpack.packb,
-                            }
-                )
-        
-        
-        One can also abuse/misuse **dogpile.cache** and defer all cache expiry to
-        **Redis** using this serializer hook.
-        
-        **dogpile.cache** doesn't cache your value as-is, but wraps it in a CachedValue
-        object which contains an API version and a timestamp for the expiry.
-        
-        This format is necessary for most cache backends, but **Redis** offers the
-        ability to handle expiry in the cloud.  By using the slim msgpack format and
-        only storing the payload, you can drastically cut down the bytes needed to store
-        this information.
-        
-        This approach SHOULD NOT BE USED by 99% of users.  However, if you do aggressive
-        caching, this will allow you to leverage **dogpile.cache**'s excellent locking
-        mechanism for handling read-through caching while slimming down your cache size
-        and the traffic on-the-wire.  
-        
-            import time
-            from dogpile.cache.api import CachedValue
-            from dogpile.cache.region import value_version
-            import msgpack
-        
-            def raw_dumps(value):
-                ''''pull the payload out of the CachedValue and serialize that
-                '''
-                value = value.payload
-                value = msgpack.packb(value)
-                return value
-        
-            def raw_loads(value):
-                ''''unpack the value and return a CachedValue with the current time
-                '''
-                value = msgpack.unpackb(value, use_list=False)
-                return CachedValue(
-                    value,
-                    {
-                        "ct": time.time(),
-                        "v": value_version
-                    })
-        
-            region = make_region().configure(
-                arguments= {'loads': msgpack_loads,
-                            'dumps': msgpack.packb,
-                            'redis_expiration_time': 1,
-                            }
-                )
-        
-        
-        RedisAdvancedHstoreBackend
-        --------------------------
-        
-        This backend extends **RedisAdvancedBackend** with drop-in support for Hash
-        storage under Redis.
-        
-        * If key names are tuples, they will be treated as hash operations on Redis.
-        * By setting `redis_expiration_time_hash` to a boolean value, you can control
-          how expiry times work within Redis
-        
-        This backend has a slight, negligible, overhead:
-        
-        * All key operations (`get`/`get_multi`/`set`/`set_multi`/`delete`) require an
-          inspection of keys.
-        * `get_multi` requires the order of keys to be tracked, and results from
-          multiple `get`/`hget` operations are then correlated.
-        * `set_multi` requires the mapping to be analyzed and bucketed into different
-          hmsets
-        
-        `redis_expiration_time_hash` allows some extended management of expiry in Redis.
-        By default it is set to `None`.
-        
-        * `False` - ignore hash expiry. (never set a TTL in Redis)
-        * `None` - set `redis_expiration_time` on new hash creation only. This requires
-          a check to the **Redis** key before a set.
-        * `True` - unconditionally set `redis_expiration_time` on every hash key
-          set/update.
-        
-        Please note the following:
-        
-        * **Redis** manages the expiry of hashes on the key, making it global for all
-          fields in the hash.
-        * **Redis** does not support setting a TTL on hashes while doing another
-          operation.  TTL must be set via another request.
-        * If `redis_expiration_time_hash` is set to `True`, there will be 2 calls to
-          the **Redis** API for every key: `hset` or `hmset` then `expires`.
-        * If `redis_expiration_time_hash` is set to `None`, there will be 2-3 calls to
-          the **Redis** API for every key: `exists`, `hset` or `hmset`, and possibly
-          `expires`.
-        
-        
-        Memory Savings and Suggested Usage
-        --------------------------------------
-        
-        Redis is an in-memory datastore that offers persistence -- optimizing storage is
-        incredibly important because the entire set must be held in-memory.
-        
-        ### Example Demo
-        
-        The attached `demo.py` (results in `demo.txt`) shows some potential approaches
-        to caching and hashing by priming a **Redis** datastore with some possible
-        strategies of a single dataset.
-        
-        It's worth looking at `demo.txt` to see how the different serializesr encode the
-        data -- sample keys are pulled for each format.
-        
-        | test                     | memory bytes | memory human | relative | ttl on Redis? | ttl in dogpile? | backend                                 | encoder |
-        | ------------------------ | ------------ | ------------ | -------- | ------------- | --------------- | --------------------------------------- | ------- |
-        | region_redis             | 249399504    | 237.85M      | 0%       | Y             | Y               | `dogpile.cache.redis`                   | pickle  |
-        | region_json              | 222924496    | 212.60M      | 89.38%   | Y             | Y               | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack           | 188472048    | 179.74M      | 75.57%   | Y             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_redis_local       | 181501200    | 173.09M      | 72.78%   | -             | Y               | `dogpile.cache.redis`                   | pickle  |
-        | region_json_raw          | 171554880    | 163.61M      | 68.79%   | Y             | -               | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack_raw       | 170765872    | 162.86M      | 68.47%   | Y             | -               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_json_local        | 162612752    | 155.08M      | 65.20%   | -             | Y               | `dogpile_backend_redis_advanced`        | json    |
-        | region_json_local_int    | 128648576    | 122.69M      | 57.71%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack_local     | 128160048    | 122.22M      | 51.39%   | -             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_msgpack_local_int | 126938576    | 121.06M      | 50.89%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_json_raw_local    | 111241280    | 106.09M      | 44.60%   | -             | -               | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack_raw_local | 110455968    | 105.34M      | 44.29%   | -             | -               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_msgpack_raw_hash  | 28518864     | 27.20M       | 11.44%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | msgpack |
-        | region_json_raw_hash     | 24836160     | 23.69M       |  9.96%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | json    |
-        
-        Notes:
-        
-        * the `_local` variants do not set a TTL on Redis
-        * the `_raw` variants strip out the dogpile CachedValue wrapper and only store
-          the payload
-        * the `_msgpack` variants use msgpack instead of pickle 
-        * the `_json` variants use json instead of pickle 
-        * the `_int` variant applies int() to the dogpile timestamp, dropping a few
-          bytes per entry
-        
-        Wait WHAT? LOOK AT `region_msgpack_raw_hash` and `region_json_raw_hash` - that's
-        a HUGE savings!
-        
-        Yes.
-        
-        The HSTORE has considerable savings due to 2 reasons:
-        
-        * **Redis** internally manages a hash much more effectively than keys.
-        * **Redis** will only put an expiry on the keys (buckets), not the hash fields
-        
-        HSTORE ends up being a much tighter memory usage for this example set, as we're
-        setting 100 fields in each key.  The savings would not be so severe if you were
-        setting 5-10 fields per key
-        
-        Note that `region_msgpack_raw_local` and `region_json_raw_local` should not be
-        used unless you're running a LRU -- they have no expiry.
-        
-        ### Assumptions
-        
-        This demo is assuming a few things that are not tested here (but there are
-        plenty of benchmarks on the internet showing this):
-        
-        * msgpack is the fastest encoder for serializing and deserializing data.
-        * json outperforms cpickle on serializing; cpickle outperforms json on
-          deserializing data.
-        
-        Here are some benchmarks and links:
-        
-        * https://gist.github.com/justinfx/3174062
-        * https://gist.github.com/cactus/4073643
-        * http://www.benfrederickson.com/dont-pickle-your-data/
-        
-        #### Caveats
-        
-        In the examples above, we deal with (de)serializing simple, native, datatypes:
-        `string`, `int`, `bool`, `list`, `dict`, `tuple`.  For these datatypes, msgpack
-        is both the smallest datastore and the fastest performer.
-        
-        If you need to store more complex types, you will need to provide a custom
-        encoder/decoder and will likely suffer a performance hit on the speed of
-        (de)serialization.  Unfortunately, the more complex data types that require
-        custom encoding/decoding include standard `datetime` objects, which can be
-        annoying.
-        
-        The file `custom_serializer.py` shows an example class for handling
-        (de)serialization -- `MsgpackSerializer`.  Some common `datetime` formats are
-        supported; they are encoded as a specially formatted dict, and decoded
-        correspondingly.  A few tricks are used to shave off time and make it roughly
-        comparable to the speed of pickle.
-        
-        
-        ### Key Takeaways
-        
-        * this was surprising - while the differences are negligible on small datasets,
-          using **Redis** to track expiry on long data-sets is generally not a good
-          idea(!). **dogpile.cache** tracks this data much more efficiently.  you can
-          enable an LRU policy in **Redis** to aid in expiry.
-        * msgpack and json are usually fairly comparable in size [remember the
-          assumption that msgpack is better for speed].
-        * reformatting the **dogpile.cache** metadata (replacing a `dict` an `int()` of
-          the expiry) saves a lot of space under JSON when you have small payloads. the
-          strings are a fraction of the size.
-        * msgpack is really good with nested data structures 
-        
-        The following payloads for `1` are strings:
-        
-            region_json_local =        '[10, {"v": 1, "ct": 1471113698.76127}]'
-            region_json_local_int =    '[10, 1471113753]'
-            region_msgpack_local =     '\x92\n\x82\xa1v\x01\xa2ct\xcbA\xd5\xeb\x92\x83\xe9\x97\x9a'
-            region_msgpack_local_int = '\x92\n\xceW\xafct'
-        
-        
-        ### So what should you use?
-        
-        There are several tradeoffs and concepts to consider:
-        
-        1. Do you want to access information outside of **dogpile.cache** (in Python
-           scripts, or even in another language)
-        2. Are you worried about the time to serialize/deserialize?  are you write-heavy
-           or read-heavy?
-        3. Do you want the TTL to be handled by **Redis** or within Python?
-        4. What are your expiry needs?  what do your keys look like?  there may not be
-           any savings possible.  but if you have a lot of recycled prefixes, there
-           could be.
-        5. What do your values look like?  How many are there?
-        
-        This test uses a particular dataset, and differences are inherent to the types
-        of data and keys. Using the strategies from the `region_msgpack_raw_hash` on
-        our production data has consistently dropped a 300MB **Redis** imprint to the
-        60-80MB range.
-        
-        The **Redis** configuration file is also enclosed. The above tests are done with
-        **Redis** compression turned on (which is why memory size fluctuates in the full
-        demo reporting).   
-        
-        
-        Custom Lock Classes
-        -------------------
-        
-        If your Redis db gets flushed the lock will disappear. This will cause the Redis
-        backend to raise an exception EVEN THOUGH you have succeeded in generating your
-        data.
-        
-        By using a ``lock_class``, you can catch the exception and decide what to do --
-        log it?, continue on, raise an error?  It's up to you!
-        
-        	import redis.exceptions
-        
-        	class RedisDistributedLockProxy(object):
-        		"""example lock wrapper
-        		this will silently pass if a LockError is encountered
-        		"""
-        		mutex = None
-        
-        		def __init__(self, mutex):
-        			self.mutex = mutex
-        
-        		def acquire(self, *_args, **_kwargs):
-        			return self.mutex.acquire(*_args, **_kwargs)
-        
-        		def release(self):
-        			# defer imports until backend is used
-        			global redis
-        			import redis  # noqa
-        			try:
-        				self.mutex.release()
-        			except redis.exceptions.LockError, e:
-        				# log.debug("safe lock timeout")
-        				pass
-        			except Exception as e:
-        				raise
-        
-        
-        
-        To Do
-        --------------------------------------
-        
-        I've been experimenting with handling the TTL within a hash bucket (instead of
-        using the **Redis** or **dogpile.cache** methods). This looks promising.  The
-        rationale is that it is easier for **Redis** to get/set an extra field from the
-        same hash, than it is to do separate calls to TTL/EXPIRES.  
-        
-        in code:
-        
-        	- hset('example', 'foo', 'bar')
-        	- expires('example', 3600)
-        	+ hmset('example', {'foo': 'bar',
-        						'expires': time.time() + 3600,
-        						}
-        
-        I've also been experimenting with blessing the result into a subclass of `dict`
-        that would do the object pair decoding lazily as-needed.
-        That would speed up most use cases.
-        
-        
-        Maturity
-        --------------------------------------
-        
-        This package is pre-release.  I've been using these strategies in production
-        via a custom fork of **dogpile.cache** for several years, but am currently
-        migrating it to a plugin.
-        
-        
-        Maintenance and Upstream Compatibility
-        --------------------------------------
-        
-        Some files in /tests are entirely from **dogpile.cache** as-is:
-        
-        *   /tests/conftest.py
-        *   /tests/cache/\__init__.py
-        *   /tests/cache/\_fixtures.py
-                
-        They are versions from **dogpile.cache** 0.6.2
-        
-        The core file, `/cache/backends/redis_advanced.py` inherits from
-        **dogpile.cache**'s `/cache/backends/redis.py`
-        
-        
-        Testing
-        -------
-        
-        This ships with full tests.  
-        
-        Much of the core package and test fixtures are from **dogpile.cache** and
-        copyright from that project, which is available under the MIT license.
-        
-        Tests are handled through tox
-        
-        Examples:
-        
-        ```
-        tox
-        tox -e py27 -- tests/cache/test_redis_backend.py
-        tox -e py27 -- tests/cache/test_redis_backend.py::RedisAdvanced_SerializedRaw_Test
-        tox -e py27 -- tests/cache/test_redis_backend.py::HstoreTest
-        ``` 
-        
-        Tests pass on the enclosed `redis.conf` file:
-        
-        ```/usr/local/Cellar/redis/3.0.7/redis-server ./redis-server--6379.conf```
-        
-        
-        
-        License
-        -------
-        
-        This project is available under the same MIT license as **dogpile.cache**.
-        
-Keywords: caching dogpile
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: testing
+![Python package](https://github.com/jvanasco/dogpile_backend_redis_advanced/workflows/Python%20package/badge.svg)
+
+This package supports Python2 and Python3
+
+This package DOES NOT support `dogpile.cache>=1.0`. Support is planned, but there have been several major API changes that are incompatible.
+
+dogpile_backend_redis_advanced
+==============================
+
+This is a plugin for the **dogpile.cache** system that offers some alternatives
+to the standard **Redis** datastore implementation.
+
+Two new backends are offered:
+
+| backend | description |
+| --- | --- |
+| `dogpile_backend_redis_advanced` | extends the `dogpile.cache.redis` backend and allows for custom pickling overrides |
+| `dogpile_backend_redis_advanced_hstore` | extends `dogpile_backend_redis_advanced` and allows for some specific hstore operations |
+
+There is a negligible performance hit in `dogpile_backend_redis_advanced_hstore`,
+as cache keys must be inspected to determine if they are an hstore or not -- and
+there are some operations involved to coordinate values.
+
+Additionally, some behavior is changed:
+
+* The constructor now accepts a ``lock_class`` argument, which can be used to
+  wrap a mutex and alter how releases are handled.  This can be necessary if you
+  have a distributed lock and timeout or flush issues (via LRU or otherwise).
+  A lock disappearing in Redis will raise a fatal exception under the standard
+  Redis backend.
+* The constructor now accepts a ``lock_prefix`` argument, which can be used to
+  alter the prefix used for locks.  The standard Redis backend uses `_lock` as
+  the prefix -- which can be hard to read or isolate for tests.  One might want
+  to use "\_" as the lock prefix (so that `keys "\_*"` will show all locks).
+
+Purpose:
+--------
+
+Mike Bayer's **dogpile.cache** is an excellent package for general purpose
+development.
+
+The system offers 3 key features:
+
+1. Elegant read-through caching functionality.
+2. A locking mechanism that ensures only the first request of a cache-miss will
+   create the resource (turning the rest into consumers of the first-requestor's
+   creation).
+3. Integrated cache expiry against time and library versions.
+
+
+Unfortunately, the integrated cache expiry feature comes at a cost -- objects
+are wrapped into a tuple with some metadata and pickled before hitting the
+datastore.
+
+The additional metadata or pickle format may not be needed or wanted.  Look how
+the size of "a" grows by the time it becomes something passed off to Redis:
+
+
+| type  | example |
+| ----- | ------- |
+| string                        | a                                                                                                               |
+| pickle(string)                | S'a'\np0\n.                                                                                                     |
+| CachedValue(string)           | ('a', {'ct': 1471113698.76127, 'v': 1})                                                                         |
+| pickle(CachedValue(string) )  | cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n. |
+
+By adding in hooks for custom serializers, this backend lets developers choose
+better ways to cache data.  
+
+You may want a serializer that doesn't care about the expiry of cached data, so
+just uses simpler strings.:
+
+| type  | example 1 | example 2 |
+| ----- | --------- | --------- |
+| string                                | a                         | mellifluous                         |
+| json.dumps(string)                    | "a"                       | "mellifluous"                       |
+| msgpack.packb(string)                 | \xa1a                     | \xabmellifluous                     |
+
+Or, you may want to fool **dogpile.cache** by manipulating what the cached is. 
+Instead of using a Python dict, of time and API version, you might just track
+the time but only to the second. 
+
+| type | example 1 | example 2 |
+| ---- | --------- | --------- |
+| AltCachedValue(string)                | ('a', 1471113698)         | ('mellifluous', 1471113698)         |
+| json.dumps(AltCachedValue(string))    | '["a", 1471113698]'       | '["mellifluous", 1471113698]'       |
+| msgpack.packb(AltCachedValue(string)) | '\x92\xa1a\xceW\xafi\xe2' | '\x92\xabmellifluous\xceW\xafi\xe2' |
+
+
+This is how **dogpile.cache** stores "a":
+
+	cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n.
+
+This package lets us cache a raw string and trick **dogpile.cache** into
+thinking our data parcel is "timely":
+
+	a
+
+Or, we include a simpler version of the time, along with a different serializer.
+
+This packet of data and time:
+
+	["a", 1471113698]
+
+Is then serialized to:
+
+	\x92\xa1a\xceW\xafi\xe2
+	
+If you cache lots of big objects, **dogpile.cache**'s overhead is minimal -- but
+if you have a cache that works for mapping short bits of text, like ids to
+usernames (and vice-versa) you will see considerable savings.
+
+Another way to make **Redis** more efficient is to use hash storage.
+
+Let's say you have a lot of keys that look like this:
+
+	region.set("user-15|posts", x)
+	region.set("user-15|friends", y)
+	region.set("user-15|profile", z)
+	region.set("user-15|username", z1)
+
+You could make **Redis** a bit more efficient by using hash storage, in which
+you have 1 key with multiple fields:
+
+	region.hset("user-15", {'posts': x,
+							'friends', y,
+							'profile', z,
+							'username', z1,
+							})
+
+Redis tends to operate much more efficiently in this situation (more below),
+but you can also save some bytes by not repeating the key prefix. Instagram's
+engineering team has a great article on this
+[Instagram Engineering](http://instagram-engineering.tumblr.com/post/12202313862/storing-hundreds-of-millions-of-simple-key-value).
+
+90% of **dogpile.cache** users who choose **Redis** will never need this
+package.  A decent number of other users with large datasets have been trying to
+squeeze every last bit of memory and performance out of their machines -- and
+this package is designed to facilitate that.
+
+
+Usage:
+------
+
+myfile.py
+
+    # importing will register the plugins
+    import dogpile_backend_redis_advanced
+
+then simply configure **dogpile.cache** with `dogpile_backend_redis_advanced` or 
+`dogpile_backend_redis_advanced_hstore` as the backend.
+
+
+RedisAdvancedBackend
+--------------------
+
+Two new configuration options are offered to specify custom serializers via 
+`loads` and `dumps`.  The default selection is to use **dogpile.cache**'s choice
+of  `pickle`.
+
+This option was designed to support `msgpack` as the serializer:
+
+    import msgpack
+    from dogpile.cache.api import CachedValue
+
+    def msgpack_loads(value):
+        """pickle maintained the `CachedValue` wrapper of the tuple
+           msgpack does not, so it must be added back in.
+           """
+        value = msgpack.unpackb(value, use_list=False)
+        return CachedValue(*value)
+
+    region = make_region().configure(
+        arguments= {'loads': msgpack_loads,
+                    'dumps': msgpack.packb,
+                    }
+        )
+
+
+One can also abuse/misuse **dogpile.cache** and defer all cache expiry to
+**Redis** using this serializer hook.
+
+**dogpile.cache** doesn't cache your value as-is, but wraps it in a CachedValue
+object which contains an API version and a timestamp for the expiry.
+
+This format is necessary for most cache backends, but **Redis** offers the
+ability to handle expiry in the cloud.  By using the slim msgpack format and
+only storing the payload, you can drastically cut down the bytes needed to store
+this information.
+
+This approach SHOULD NOT BE USED by 99% of users.  However, if you do aggressive
+caching, this will allow you to leverage **dogpile.cache**'s excellent locking
+mechanism for handling read-through caching while slimming down your cache size
+and the traffic on-the-wire.  
+
+    import time
+    from dogpile.cache.api import CachedValue
+    from dogpile.cache.region import value_version
+    import msgpack
+
+    def raw_dumps(value):
+        ''''pull the payload out of the CachedValue and serialize that
+        '''
+        value = value.payload
+        value = msgpack.packb(value)
+        return value
+
+    def raw_loads(value):
+        ''''unpack the value and return a CachedValue with the current time
+        '''
+        value = msgpack.unpackb(value, use_list=False)
+        return CachedValue(
+            value,
+            {
+                "ct": time.time(),
+                "v": value_version
+            })
+
+    region = make_region().configure(
+        arguments= {'loads': msgpack_loads,
+                    'dumps': msgpack.packb,
+                    'redis_expiration_time': 1,
+                    }
+        )
+
+
+RedisAdvancedHstoreBackend
+--------------------------
+
+This backend extends **RedisAdvancedBackend** with drop-in support for Hash
+storage under Redis.
+
+* If key names are tuples, they will be treated as hash operations on Redis.
+* By setting `redis_expiration_time_hash` to a boolean value, you can control
+  how expiry times work within Redis
+
+This backend has a slight, negligible, overhead:
+
+* All key operations (`get`/`get_multi`/`set`/`set_multi`/`delete`) require an
+  inspection of keys.
+* `get_multi` requires the order of keys to be tracked, and results from
+  multiple `get`/`hget` operations are then correlated.
+* `set_multi` requires the mapping to be analyzed and bucketed into different
+  hmsets
+
+`redis_expiration_time_hash` allows some extended management of expiry in Redis.
+By default it is set to `None`.
+
+* `False` - ignore hash expiry. (never set a TTL in Redis)
+* `None` - set `redis_expiration_time` on new hash creation only. This requires
+  a check to the **Redis** key before a set.
+* `True` - unconditionally set `redis_expiration_time` on every hash key
+  set/update.
+
+Please note the following:
+
+* **Redis** manages the expiry of hashes on the key, making it global for all
+  fields in the hash.
+* **Redis** does not support setting a TTL on hashes while doing another
+  operation.  TTL must be set via another request.
+* If `redis_expiration_time_hash` is set to `True`, there will be 2 calls to
+  the **Redis** API for every key: `hset` or `hmset` then `expires`.
+* If `redis_expiration_time_hash` is set to `None`, there will be 2-3 calls to
+  the **Redis** API for every key: `exists`, `hset` or `hmset`, and possibly
+  `expires`.
+
+
+Memory Savings and Suggested Usage
+--------------------------------------
+
+Redis is an in-memory datastore that offers persistence -- optimizing storage is
+incredibly important because the entire set must be held in-memory.
+
+### Example Demo
+
+The attached `demo.py` (results in `demo.txt`) shows some potential approaches
+to caching and hashing by priming a **Redis** datastore with some possible
+strategies of a single dataset.
+
+It's worth looking at `demo.txt` to see how the different serializesr encode the
+data -- sample keys are pulled for each format.
+
+| test                     | memory bytes | memory human | relative | ttl on Redis? | ttl in dogpile? | backend                                 | encoder |
+| ------------------------ | ------------ | ------------ | -------- | ------------- | --------------- | --------------------------------------- | ------- |
+| region_redis             | 249399504    | 237.85M      | 0%       | Y             | Y               | `dogpile.cache.redis`                   | pickle  |
+| region_json              | 222924496    | 212.60M      | 89.38%   | Y             | Y               | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack           | 188472048    | 179.74M      | 75.57%   | Y             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_redis_local       | 181501200    | 173.09M      | 72.78%   | -             | Y               | `dogpile.cache.redis`                   | pickle  |
+| region_json_raw          | 171554880    | 163.61M      | 68.79%   | Y             | -               | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack_raw       | 170765872    | 162.86M      | 68.47%   | Y             | -               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_json_local        | 162612752    | 155.08M      | 65.20%   | -             | Y               | `dogpile_backend_redis_advanced`        | json    |
+| region_json_local_int    | 128648576    | 122.69M      | 57.71%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack_local     | 128160048    | 122.22M      | 51.39%   | -             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_msgpack_local_int | 126938576    | 121.06M      | 50.89%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | msgpack |
+| region_json_raw_local    | 111241280    | 106.09M      | 44.60%   | -             | -               | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack_raw_local | 110455968    | 105.34M      | 44.29%   | -             | -               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_msgpack_raw_hash  | 28518864     | 27.20M       | 11.44%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | msgpack |
+| region_json_raw_hash     | 24836160     | 23.69M       |  9.96%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | json    |
+
+Notes:
+
+* the `_local` variants do not set a TTL on Redis
+* the `_raw` variants strip out the dogpile CachedValue wrapper and only store
+  the payload
+* the `_msgpack` variants use msgpack instead of pickle 
+* the `_json` variants use json instead of pickle 
+* the `_int` variant applies int() to the dogpile timestamp, dropping a few
+  bytes per entry
+
+Wait WHAT? LOOK AT `region_msgpack_raw_hash` and `region_json_raw_hash` - that's
+a HUGE savings!
+
+Yes.
+
+The HSTORE has considerable savings due to 2 reasons:
+
+* **Redis** internally manages a hash much more effectively than keys.
+* **Redis** will only put an expiry on the keys (buckets), not the hash fields
+
+HSTORE ends up being a much tighter memory usage for this example set, as we're
+setting 100 fields in each key.  The savings would not be so severe if you were
+setting 5-10 fields per key
+
+Note that `region_msgpack_raw_local` and `region_json_raw_local` should not be
+used unless you're running a LRU -- they have no expiry.
+
+### Assumptions
+
+This demo is assuming a few things that are not tested here (but there are
+plenty of benchmarks on the internet showing this):
+
+* msgpack is the fastest encoder for serializing and deserializing data.
+* json outperforms cpickle on serializing; cpickle outperforms json on
+  deserializing data.
+
+Here are some benchmarks and links:
+
+* https://gist.github.com/justinfx/3174062
+* https://gist.github.com/cactus/4073643
+* http://www.benfrederickson.com/dont-pickle-your-data/
+
+#### Caveats
+
+In the examples above, we deal with (de)serializing simple, native, datatypes:
+`string`, `int`, `bool`, `list`, `dict`, `tuple`.  For these datatypes, msgpack
+is both the smallest datastore and the fastest performer.
+
+If you need to store more complex types, you will need to provide a custom
+encoder/decoder and will likely suffer a performance hit on the speed of
+(de)serialization.  Unfortunately, the more complex data types that require
+custom encoding/decoding include standard `datetime` objects, which can be
+annoying.
+
+The file `custom_serializer.py` shows an example class for handling
+(de)serialization -- `MsgpackSerializer`.  Some common `datetime` formats are
+supported; they are encoded as a specially formatted dict, and decoded
+correspondingly.  A few tricks are used to shave off time and make it roughly
+comparable to the speed of pickle.
+
+
+### Key Takeaways
+
+* this was surprising - while the differences are negligible on small datasets,
+  using **Redis** to track expiry on long data-sets is generally not a good
+  idea(!). **dogpile.cache** tracks this data much more efficiently.  you can
+  enable an LRU policy in **Redis** to aid in expiry.
+* msgpack and json are usually fairly comparable in size [remember the
+  assumption that msgpack is better for speed].
+* reformatting the **dogpile.cache** metadata (replacing a `dict` an `int()` of
+  the expiry) saves a lot of space under JSON when you have small payloads. the
+  strings are a fraction of the size.
+* msgpack is really good with nested data structures 
+
+The following payloads for `1` are strings:
+
+    region_json_local =        '[10, {"v": 1, "ct": 1471113698.76127}]'
+    region_json_local_int =    '[10, 1471113753]'
+    region_msgpack_local =     '\x92\n\x82\xa1v\x01\xa2ct\xcbA\xd5\xeb\x92\x83\xe9\x97\x9a'
+    region_msgpack_local_int = '\x92\n\xceW\xafct'
+
+
+### So what should you use?
+
+There are several tradeoffs and concepts to consider:
+
+1. Do you want to access information outside of **dogpile.cache** (in Python
+   scripts, or even in another language)
+2. Are you worried about the time to serialize/deserialize?  are you write-heavy
+   or read-heavy?
+3. Do you want the TTL to be handled by **Redis** or within Python?
+4. What are your expiry needs?  what do your keys look like?  there may not be
+   any savings possible.  but if you have a lot of recycled prefixes, there
+   could be.
+5. What do your values look like?  How many are there?
+
+This test uses a particular dataset, and differences are inherent to the types
+of data and keys. Using the strategies from the `region_msgpack_raw_hash` on
+our production data has consistently dropped a 300MB **Redis** imprint to the
+60-80MB range.
+
+The **Redis** configuration file is also enclosed. The above tests are done with
+**Redis** compression turned on (which is why memory size fluctuates in the full
+demo reporting).   
+
+
+Custom Lock Classes
+-------------------
+
+If your Redis db gets flushed the lock will disappear. This will cause the Redis
+backend to raise an exception EVEN THOUGH you have succeeded in generating your
+data.
+
+By using a ``lock_class``, you can catch the exception and decide what to do --
+log it?, continue on, raise an error?  It's up to you!
+
+	import redis.exceptions
+
+	class RedisDistributedLockProxy(object):
+		"""example lock wrapper
+		this will silently pass if a LockError is encountered
+		"""
+		mutex = None
+
+		def __init__(self, mutex):
+			self.mutex = mutex
+
+		def acquire(self, *_args, **_kwargs):
+			return self.mutex.acquire(*_args, **_kwargs)
+
+		def release(self):
+			# defer imports until backend is used
+			global redis
+			import redis  # noqa
+			try:
+				self.mutex.release()
+			except redis.exceptions.LockError, e:
+				# log.debug("safe lock timeout")
+				pass
+			except Exception as e:
+				raise
+
+
+
+To Do
+--------------------------------------
+
+I've been experimenting with handling the TTL within a hash bucket (instead of
+using the **Redis** or **dogpile.cache** methods). This looks promising.  The
+rationale is that it is easier for **Redis** to get/set an extra field from the
+same hash, than it is to do separate calls to TTL/EXPIRES.  
+
+in code:
+
+	- hset('example', 'foo', 'bar')
+	- expires('example', 3600)
+	+ hmset('example', {'foo': 'bar',
+						'expires': time.time() + 3600,
+						}
+
+I've also been experimenting with blessing the result into a subclass of `dict`
+that would do the object pair decoding lazily as-needed.
+That would speed up most use cases.
+
+
+Maturity
+--------------------------------------
+
+This package is pre-release.  I've been using these strategies in production
+via a custom fork of **dogpile.cache** for several years, but am currently
+migrating it to a plugin.
+
+
+Maintenance and Upstream Compatibility
+--------------------------------------
+
+Some files in /tests are entirely from **dogpile.cache** as-is:
+
+*   /tests/conftest.py
+*   /tests/cache/\__init__.py
+*   /tests/cache/\_fixtures.py
+        
+They are versions from **dogpile.cache** 0.6.2
+
+The core file, `/cache/backends/redis_advanced.py` inherits from
+**dogpile.cache**'s `/cache/backends/redis.py`
+
+
+Testing
+-------
+
+This ships with full tests.  
+
+Much of the core package and test fixtures are from **dogpile.cache** and
+copyright from that project, which is available under the MIT license.
+
+Tests are handled through tox
+
+Examples:
+
+```
+tox
+tox -e py27 -- tests/cache/test_redis_backend.py
+tox -e py27 -- tests/cache/test_redis_backend.py::RedisAdvanced_SerializedRaw_Test
+tox -e py27 -- tests/cache/test_redis_backend.py::HstoreTest
+``` 
+
+Tests pass on the enclosed `redis.conf` file:
+
+```/usr/local/Cellar/redis/3.0.7/redis-server ./redis-server--6379.conf```
+
+
+
+License
+-------
+
+This project is available under the same MIT license as **dogpile.cache**.
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/README.md` & `dogpile_backend_redis_advanced-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,37 @@
+Metadata-Version: 2.1
+Name: dogpile_backend_redis_advanced
+Version: 0.4.0
+Summary: Advanced Redis plugins for `dogpile.cache`.
+Home-page: https://github.com/jvanasco/dogpile_backend_redis_advanced
+Author: Jonathan Vanasco
+Author-email: jonathan@findmeon.com
+License: BSD
+Keywords: caching dogpile
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 ![Python package](https://github.com/jvanasco/dogpile_backend_redis_advanced/workflows/Python%20package/badge.svg)
 
 This package supports Python2 and Python3
 
+This package DOES NOT support `dogpile.cache>=1.0`. Support is planned, but there have been several major API changes that are incompatible.
+
 dogpile_backend_redis_advanced
 ==============================
 
 This is a plugin for the **dogpile.cache** system that offers some alternatives
 to the standard **Redis** datastore implementation.
 
 Two new backends are offered:
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/setup.py` & `dogpile_backend_redis_advanced-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,28 +34,27 @@
 
 long_description = description = "Advanced Redis plugins for `dogpile.cache`."
 with open(os.path.join(HERE, "README.md")) as fp:
     long_description = fp.read()
 
 
 install_requires = [
+    "dogpile.cache>=1.0",
     "redis",
-    "dogpile.cache<1.0.0",
 ]
-tests_require = [
+
+tests_require = install_requires + [
     "pytest",
     "pytest-cov",
     "mock",
     "msgpack-python",
-    "dogpile.cache<1.0.0",
-    "redis",
-    "six",
 ]
 testing_extras = [
     "flake8",
+    "mypy",
     "tox",
 ]
 
 
 setup(
     name="dogpile_backend_redis_advanced",
     version=VERSION,
@@ -63,26 +62,32 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="caching dogpile",
     author="Jonathan Vanasco",
     author_email="jonathan@findmeon.com",
     url="https://github.com/jvanasco/dogpile_backend_redis_advanced",
     license="BSD",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"dogpile_backend_redis_advanced": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
     },
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced/cache/backends/redis_advanced.py` & `dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced/cache/backends/redis_advanced.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,46 @@
 Redis Backends
 ------------------
 
 Provides backends for talking to `Redis <http://redis.io>`_.
 
 """
 from __future__ import absolute_import
-from dogpile.cache.api import NO_VALUE
-from dogpile.cache.backends.redis import RedisBackend
-from dogpile.util.compat import pickle, u
 
+# stdlib
 from collections import defaultdict
+import pickle
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Tuple
+
+# pypi
+from dogpile.cache.api import NO_VALUE  # type: ignore[import]
+from dogpile.cache.backends.redis import RedisBackend  # type: ignore[import]
+
+# only needed for testing
+# import redis
+
+
+# - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
-import redis
 
 __all__ = ("RedisAdvancedBackend", "RedisAdvancedHstoreBackend")
 
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
-default_loads = pickle.loads
+default_loads: Callable = pickle.loads
 
 
-def default_dumps_factory():
+def default_dumps_factory() -> Callable:
     """
     optimized for the cpython compiler. shaves a tiny bit off.
     this turns 'pickle_dumps' into a local variable to the dump function.
     original:
               0 LOAD_GLOBAL              0 (pickle)
               3 LOAD_ATTR                1 (dumps)
               6 LOAD_GLOBAL              2 (v)
@@ -147,52 +161,52 @@
 
     :param lock_prefix: string, prefix used for generating locks. By default
      the backend uses `_lock`.
      .. versionadded:: 0.1.0
 
     """
 
-    def __init__(self, arguments):
+    def __init__(self, arguments: Dict):
         arguments = arguments.copy()
         super(RedisAdvancedBackend, self).__init__(arguments)
         self.loads = arguments.pop("loads", default_loads)
         self.dumps = arguments.pop("dumps", default_dumps)
         self.lock_class = arguments.pop("lock_class", None)
         self.lock_prefix = "%s{0}" % arguments.pop("lock_prefix", "_lock")
 
-    def get_mutex(self, key):
+    def get_mutex(self, key: str) -> Optional[Any]:
         if self.distributed_lock:
-            _key = u(self.lock_prefix).format(key)
+            _key = self.lock_prefix.format(key)
             _mutex = self.client.lock(_key, self.lock_timeout, self.lock_sleep)
             if self.lock_class:
                 return self.lock_class(_mutex)
             return _mutex
         else:
             return None
 
-    def get(self, key):
+    def get(self, key: str) -> Any:
         value = self.client.get(key)
         if value is None:
             return NO_VALUE
         return self.loads(value)
 
-    def get_multi(self, keys):
+    def get_multi(self, keys: Tuple[str]) -> List[Any]:
         if not keys:
             return []
         values = self.client.mget(keys)
         loads = self.loads  # potentially faster on large lists
         return [loads(v) if v is not None else NO_VALUE for v in values]
 
-    def set(self, key, value):
+    def set(self, key: str, value: Any) -> None:
         if self.redis_expiration_time:
             self.client.setex(key, self.redis_expiration_time, self.dumps(value))
         else:
             self.client.set(key, self.dumps(value))
 
-    def set_multi(self, mapping):
+    def set_multi(self, mapping: Dict) -> None:
         dumps = self.dumps  # potentially faster on large lists
         mapping = dict((k, dumps(v)) for k, v in mapping.items())
         if not self.redis_expiration_time:
             self.client.mset(mapping)
         else:
             pipe = self.client.pipeline()
             for key, value in mapping.items():
@@ -241,103 +255,103 @@
     if `redis_expiration_time_hash` is set to `True`.
 
     if `redis_expiration_time_hash` is set to `False`, then dogpile will not set
     expiry times on hashes.
 
     """
 
-    def __init__(self, arguments):
+    def __init__(self, arguments: Dict):
         arguments = arguments.copy()
         super(RedisAdvancedHstoreBackend, self).__init__(arguments)
         self.redis_expiration_time_hash = arguments.pop(
             "redis_expiration_time_hash", None
         )  # noqa
 
-    def get_mutex(self, key):
+    def get_mutex(self, key: str) -> Optional[Any]:
         if isinstance(key, tuple):
             # key can be a tuple
             key = ",".join(key)
         if self.distributed_lock:
             # redis.py command: `lock(name, timeout=None, sleep=0.1)`
-            _key = u(self.lock_prefix).format(key)
+            _key = self.lock_prefix.format(key)
             _mutex = self.client.lock(_key, self.lock_timeout, self.lock_sleep)
             if self.lock_class:
                 return self.lock_class(_mutex)
             return _mutex
         else:
             return None
 
-    def get(self, key):
+    def get(self, key: str) -> Any:
         if isinstance(key, tuple):
             # redis.py command: `hget(hashname, key)`
             value = self.client.hget(key[0], key[1])
         else:
             # redis.py command: `get(name)`
             value = self.client.get(key)
         if value is None:
             return NO_VALUE
         return self.loads(value)
 
-    def get_multi(self, keys):
+    def get_multi(self, keys: Tuple[str]) -> List[Any]:
         """
         * figure out which are string keys vs hashes, process 2 queues
         * for hashes, bucket into multiple requests
         * reintegrate the values in the right order
         this is sadly complex as we may have duplicate keys - so can't stash
         position in a dict.
         """
         # scoping
-        _keys_str = []
-        _keys_str_idx = []
-        _keys_hash = []
-        _keys_hash_idx = []
+        _keys_str: List[str] = []
+        _keys_str_idx: List[int] = []
+        _keys_hash: List[str] = []
+        _keys_hash_idx: List[int] = []
 
         # initialize this list
         values = [None] * len(keys)
 
-        for (_idx, _k) in enumerate(keys):
+        for _idx, _k in enumerate(keys):
             if isinstance(_k, tuple):
                 _keys_hash.append(_k)
                 _keys_hash_idx.append(_idx)
             else:
                 _keys_str.append(_k)
                 _keys_str_idx.append(_idx)
 
         # batch the keys at once
         if _keys_str:
             # redis.py command: `mget(keys, *args)`
             _values = self.client.mget(_keys_str)
             # build this back into the results in the right order
             _values = zip(_keys_str_idx, _values)
-            for (_idx, _v) in _values:
+            for _idx, _v in _values:
                 values[_idx] = _v
 
         # group and batch the hashed as needed
         if _keys_hash:
-            _hashed = {}
+            _hashed: Dict[str, Dict[str, List]] = {}
             for k in _keys_hash:
                 # k[0] is our bucket
                 if k[0] not in _hashed:
                     _hashed[k[0]] = {"keys": [], "idx": []}
             for idx, k in enumerate(_keys_hash):
                 # note that we're using the _keys_hash_idx here
                 _hashed[k[0]]["keys"].append(k[1])
                 _hashed[k[0]]["idx"].append(_keys_hash_idx[idx])
             for name in _hashed:
                 # redis.py command: `hmget(name, keys, *args)`
                 _values = self.client.hmget(name, _hashed[name]["keys"])
                 # build this back into the results in the right order
                 _values = zip(_hashed[name]["idx"], _values)
-                for (_idx, _v) in _values:
+                for _idx, _v in _values:
                     values[_idx] = _v
 
         loads = self.loads  # potentially faster on large lists
         return [loads(v) if v is not None else NO_VALUE for v in values]
 
-    def set(self, key, value):
+    def set(self, key: str, value: Any) -> None:
         if isinstance(key, tuple):
             _set_expiry = None
             if self.redis_expiration_time_hash is True:
                 # unconditionally set
                 _set_expiry = True
             elif self.redis_expiration_time_hash is None:
                 # conditionally set
@@ -355,26 +369,26 @@
             if self.redis_expiration_time:
                 # redis.py command: `setex(name, time, value)`
                 self.client.setex(key, self.redis_expiration_time, self.dumps(value))
             else:
                 # redis.py command: `set(name, value)`
                 self.client.set(key, self.dumps(value))
 
-    def set_multi(self, mapping):
+    def set_multi(self, mapping: Dict) -> None:
         """
         we'll always use a pipeline for this class
         """
         # encode
         dumps = self.dumps  # potentially faster on large lists
         mapping = dict((k, dumps(v)) for k, v in mapping.items())
 
         # derive key types
         _keys_str = []
         _keys_hash = []
-        _hash_bucketed = None
+        _hash_bucketed: Optional[Dict] = None
         for _k in mapping.keys():
             if isinstance(_k, tuple):
                 _keys_hash.append(_k)
             else:
                 _keys_str.append(_k)
 
         # redis.py command: `pipeline(transaction=True, shard_hint=None)`
@@ -417,37 +431,37 @@
                     # redis.py command: `setex(name, time, value)`
                     pipe.setex(key, self.redis_expiration_time, mapping[key])
             # bucketed hash was set above
 
         # run the pipeline
         pipe.execute()
 
-    def delete(self, key):
+    def delete(self, key: str) -> None:
         if isinstance(key, tuple):
             # redis.py command: hdel(`name, *keys)`
             self.client.hdel(key[0], key[1])
         else:
             # redis.py command: delete(*names)`
             self.client.delete(key)
 
-    def delete_multi(self, keys):
+    def delete_multi(self, keys: Tuple[str]) -> None:
         """
         In order to handle multiple deletes, we need to inspect the keys and
         batch them into the appropriate method.  This has a negligible cost.
         """
-        _keys = []
-        _keys_hash = []
+        _keys: List = []
+        _keys_hash: List = []
         for k in keys:
             if isinstance(k, tuple):
                 _keys_hash.append(k)
             else:
                 _keys.append(k)
         if _keys:
             # redis.py command: delete(*names)`
             self.client.delete(*_keys)
         if _keys_hash:
-            _hashed = {k[0]: [] for k in _keys_hash}
+            _hashed: Dict[str, List] = {k[0]: [] for k in _keys_hash}
             for k in _keys_hash:
                 _hashed[k[0]].append(k[1])
             for name in _hashed:
                 # redis.py command: `hdel(name, *keys)`
                 self.client.hdel(name, *_hashed[name])
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/PKG-INFO` & `dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,532 +1,539 @@
 Metadata-Version: 2.1
 Name: dogpile-backend-redis-advanced
-Version: 0.3.2
+Version: 0.4.0
 Summary: Advanced Redis plugins for `dogpile.cache`.
 Home-page: https://github.com/jvanasco/dogpile_backend_redis_advanced
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: BSD
-Description: ![Python package](https://github.com/jvanasco/dogpile_backend_redis_advanced/workflows/Python%20package/badge.svg)
-        
-        This package supports Python2 and Python3
-        
-        dogpile_backend_redis_advanced
-        ==============================
-        
-        This is a plugin for the **dogpile.cache** system that offers some alternatives
-        to the standard **Redis** datastore implementation.
-        
-        Two new backends are offered:
-        
-        | backend | description |
-        | --- | --- |
-        | `dogpile_backend_redis_advanced` | extends the `dogpile.cache.redis` backend and allows for custom pickling overrides |
-        | `dogpile_backend_redis_advanced_hstore` | extends `dogpile_backend_redis_advanced` and allows for some specific hstore operations |
-        
-        There is a negligible performance hit in `dogpile_backend_redis_advanced_hstore`,
-        as cache keys must be inspected to determine if they are an hstore or not -- and
-        there are some operations involved to coordinate values.
-        
-        Additionally, some behavior is changed:
-        
-        * The constructor now accepts a ``lock_class`` argument, which can be used to
-          wrap a mutex and alter how releases are handled.  This can be necessary if you
-          have a distributed lock and timeout or flush issues (via LRU or otherwise).
-          A lock disappearing in Redis will raise a fatal exception under the standard
-          Redis backend.
-        * The constructor now accepts a ``lock_prefix`` argument, which can be used to
-          alter the prefix used for locks.  The standard Redis backend uses `_lock` as
-          the prefix -- which can be hard to read or isolate for tests.  One might want
-          to use "\_" as the lock prefix (so that `keys "\_*"` will show all locks).
-        
-        Purpose:
-        --------
-        
-        Mike Bayer's **dogpile.cache** is an excellent package for general purpose
-        development.
-        
-        The system offers 3 key features:
-        
-        1. Elegant read-through caching functionality.
-        2. A locking mechanism that ensures only the first request of a cache-miss will
-           create the resource (turning the rest into consumers of the first-requestor's
-           creation).
-        3. Integrated cache expiry against time and library versions.
-        
-        
-        Unfortunately, the integrated cache expiry feature comes at a cost -- objects
-        are wrapped into a tuple with some metadata and pickled before hitting the
-        datastore.
-        
-        The additional metadata or pickle format may not be needed or wanted.  Look how
-        the size of "a" grows by the time it becomes something passed off to Redis:
-        
-        
-        | type  | example |
-        | ----- | ------- |
-        | string                        | a                                                                                                               |
-        | pickle(string)                | S'a'\np0\n.                                                                                                     |
-        | CachedValue(string)           | ('a', {'ct': 1471113698.76127, 'v': 1})                                                                         |
-        | pickle(CachedValue(string) )  | cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n. |
-        
-        By adding in hooks for custom serializers, this backend lets developers choose
-        better ways to cache data.  
-        
-        You may want a serializer that doesn't care about the expiry of cached data, so
-        just uses simpler strings.:
-        
-        | type  | example 1 | example 2 |
-        | ----- | --------- | --------- |
-        | string                                | a                         | mellifluous                         |
-        | json.dumps(string)                    | "a"                       | "mellifluous"                       |
-        | msgpack.packb(string)                 | \xa1a                     | \xabmellifluous                     |
-        
-        Or, you may want to fool **dogpile.cache** by manipulating what the cached is. 
-        Instead of using a Python dict, of time and API version, you might just track
-        the time but only to the second. 
-        
-        | type | example 1 | example 2 |
-        | ---- | --------- | --------- |
-        | AltCachedValue(string)                | ('a', 1471113698)         | ('mellifluous', 1471113698)         |
-        | json.dumps(AltCachedValue(string))    | '["a", 1471113698]'       | '["mellifluous", 1471113698]'       |
-        | msgpack.packb(AltCachedValue(string)) | '\x92\xa1a\xceW\xafi\xe2' | '\x92\xabmellifluous\xceW\xafi\xe2' |
-        
-        
-        This is how **dogpile.cache** stores "a":
-        
-        	cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n.
-        
-        This package lets us cache a raw string and trick **dogpile.cache** into
-        thinking our data parcel is "timely":
-        
-        	a
-        
-        Or, we include a simpler version of the time, along with a different serializer.
-        
-        This packet of data and time:
-        
-        	["a", 1471113698]
-        
-        Is then serialized to:
-        
-        	\x92\xa1a\xceW\xafi\xe2
-        	
-        If you cache lots of big objects, **dogpile.cache**'s overhead is minimal -- but
-        if you have a cache that works for mapping short bits of text, like ids to
-        usernames (and vice-versa) you will see considerable savings.
-        
-        Another way to make **Redis** more efficient is to use hash storage.
-        
-        Let's say you have a lot of keys that look like this:
-        
-        	region.set("user-15|posts", x)
-        	region.set("user-15|friends", y)
-        	region.set("user-15|profile", z)
-        	region.set("user-15|username", z1)
-        
-        You could make **Redis** a bit more efficient by using hash storage, in which
-        you have 1 key with multiple fields:
-        
-        	region.hset("user-15", {'posts': x,
-        							'friends', y,
-        							'profile', z,
-        							'username', z1,
-        							})
-        
-        Redis tends to operate much more efficiently in this situation (more below),
-        but you can also save some bytes by not repeating the key prefix. Instagram's
-        engineering team has a great article on this
-        [Instagram Engineering](http://instagram-engineering.tumblr.com/post/12202313862/storing-hundreds-of-millions-of-simple-key-value).
-        
-        90% of **dogpile.cache** users who choose **Redis** will never need this
-        package.  A decent number of other users with large datasets have been trying to
-        squeeze every last bit of memory and performance out of their machines -- and
-        this package is designed to facilitate that.
-        
-        
-        Usage:
-        ------
-        
-        myfile.py
-        
-            # importing will register the plugins
-            import dogpile_backend_redis_advanced
-        
-        then simply configure **dogpile.cache** with `dogpile_backend_redis_advanced` or 
-        `dogpile_backend_redis_advanced_hstore` as the backend.
-        
-        
-        RedisAdvancedBackend
-        --------------------
-        
-        Two new configuration options are offered to specify custom serializers via 
-        `loads` and `dumps`.  The default selection is to use **dogpile.cache**'s choice
-        of  `pickle`.
-        
-        This option was designed to support `msgpack` as the serializer:
-        
-            import msgpack
-            from dogpile.cache.api import CachedValue
-        
-            def msgpack_loads(value):
-                """pickle maintained the `CachedValue` wrapper of the tuple
-                   msgpack does not, so it must be added back in.
-                   """
-                value = msgpack.unpackb(value, use_list=False)
-                return CachedValue(*value)
-        
-            region = make_region().configure(
-                arguments= {'loads': msgpack_loads,
-                            'dumps': msgpack.packb,
-                            }
-                )
-        
-        
-        One can also abuse/misuse **dogpile.cache** and defer all cache expiry to
-        **Redis** using this serializer hook.
-        
-        **dogpile.cache** doesn't cache your value as-is, but wraps it in a CachedValue
-        object which contains an API version and a timestamp for the expiry.
-        
-        This format is necessary for most cache backends, but **Redis** offers the
-        ability to handle expiry in the cloud.  By using the slim msgpack format and
-        only storing the payload, you can drastically cut down the bytes needed to store
-        this information.
-        
-        This approach SHOULD NOT BE USED by 99% of users.  However, if you do aggressive
-        caching, this will allow you to leverage **dogpile.cache**'s excellent locking
-        mechanism for handling read-through caching while slimming down your cache size
-        and the traffic on-the-wire.  
-        
-            import time
-            from dogpile.cache.api import CachedValue
-            from dogpile.cache.region import value_version
-            import msgpack
-        
-            def raw_dumps(value):
-                ''''pull the payload out of the CachedValue and serialize that
-                '''
-                value = value.payload
-                value = msgpack.packb(value)
-                return value
-        
-            def raw_loads(value):
-                ''''unpack the value and return a CachedValue with the current time
-                '''
-                value = msgpack.unpackb(value, use_list=False)
-                return CachedValue(
-                    value,
-                    {
-                        "ct": time.time(),
-                        "v": value_version
-                    })
-        
-            region = make_region().configure(
-                arguments= {'loads': msgpack_loads,
-                            'dumps': msgpack.packb,
-                            'redis_expiration_time': 1,
-                            }
-                )
-        
-        
-        RedisAdvancedHstoreBackend
-        --------------------------
-        
-        This backend extends **RedisAdvancedBackend** with drop-in support for Hash
-        storage under Redis.
-        
-        * If key names are tuples, they will be treated as hash operations on Redis.
-        * By setting `redis_expiration_time_hash` to a boolean value, you can control
-          how expiry times work within Redis
-        
-        This backend has a slight, negligible, overhead:
-        
-        * All key operations (`get`/`get_multi`/`set`/`set_multi`/`delete`) require an
-          inspection of keys.
-        * `get_multi` requires the order of keys to be tracked, and results from
-          multiple `get`/`hget` operations are then correlated.
-        * `set_multi` requires the mapping to be analyzed and bucketed into different
-          hmsets
-        
-        `redis_expiration_time_hash` allows some extended management of expiry in Redis.
-        By default it is set to `None`.
-        
-        * `False` - ignore hash expiry. (never set a TTL in Redis)
-        * `None` - set `redis_expiration_time` on new hash creation only. This requires
-          a check to the **Redis** key before a set.
-        * `True` - unconditionally set `redis_expiration_time` on every hash key
-          set/update.
-        
-        Please note the following:
-        
-        * **Redis** manages the expiry of hashes on the key, making it global for all
-          fields in the hash.
-        * **Redis** does not support setting a TTL on hashes while doing another
-          operation.  TTL must be set via another request.
-        * If `redis_expiration_time_hash` is set to `True`, there will be 2 calls to
-          the **Redis** API for every key: `hset` or `hmset` then `expires`.
-        * If `redis_expiration_time_hash` is set to `None`, there will be 2-3 calls to
-          the **Redis** API for every key: `exists`, `hset` or `hmset`, and possibly
-          `expires`.
-        
-        
-        Memory Savings and Suggested Usage
-        --------------------------------------
-        
-        Redis is an in-memory datastore that offers persistence -- optimizing storage is
-        incredibly important because the entire set must be held in-memory.
-        
-        ### Example Demo
-        
-        The attached `demo.py` (results in `demo.txt`) shows some potential approaches
-        to caching and hashing by priming a **Redis** datastore with some possible
-        strategies of a single dataset.
-        
-        It's worth looking at `demo.txt` to see how the different serializesr encode the
-        data -- sample keys are pulled for each format.
-        
-        | test                     | memory bytes | memory human | relative | ttl on Redis? | ttl in dogpile? | backend                                 | encoder |
-        | ------------------------ | ------------ | ------------ | -------- | ------------- | --------------- | --------------------------------------- | ------- |
-        | region_redis             | 249399504    | 237.85M      | 0%       | Y             | Y               | `dogpile.cache.redis`                   | pickle  |
-        | region_json              | 222924496    | 212.60M      | 89.38%   | Y             | Y               | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack           | 188472048    | 179.74M      | 75.57%   | Y             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_redis_local       | 181501200    | 173.09M      | 72.78%   | -             | Y               | `dogpile.cache.redis`                   | pickle  |
-        | region_json_raw          | 171554880    | 163.61M      | 68.79%   | Y             | -               | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack_raw       | 170765872    | 162.86M      | 68.47%   | Y             | -               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_json_local        | 162612752    | 155.08M      | 65.20%   | -             | Y               | `dogpile_backend_redis_advanced`        | json    |
-        | region_json_local_int    | 128648576    | 122.69M      | 57.71%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack_local     | 128160048    | 122.22M      | 51.39%   | -             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_msgpack_local_int | 126938576    | 121.06M      | 50.89%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_json_raw_local    | 111241280    | 106.09M      | 44.60%   | -             | -               | `dogpile_backend_redis_advanced`        | json    |
-        | region_msgpack_raw_local | 110455968    | 105.34M      | 44.29%   | -             | -               | `dogpile_backend_redis_advanced`        | msgpack |
-        | region_msgpack_raw_hash  | 28518864     | 27.20M       | 11.44%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | msgpack |
-        | region_json_raw_hash     | 24836160     | 23.69M       |  9.96%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | json    |
-        
-        Notes:
-        
-        * the `_local` variants do not set a TTL on Redis
-        * the `_raw` variants strip out the dogpile CachedValue wrapper and only store
-          the payload
-        * the `_msgpack` variants use msgpack instead of pickle 
-        * the `_json` variants use json instead of pickle 
-        * the `_int` variant applies int() to the dogpile timestamp, dropping a few
-          bytes per entry
-        
-        Wait WHAT? LOOK AT `region_msgpack_raw_hash` and `region_json_raw_hash` - that's
-        a HUGE savings!
-        
-        Yes.
-        
-        The HSTORE has considerable savings due to 2 reasons:
-        
-        * **Redis** internally manages a hash much more effectively than keys.
-        * **Redis** will only put an expiry on the keys (buckets), not the hash fields
-        
-        HSTORE ends up being a much tighter memory usage for this example set, as we're
-        setting 100 fields in each key.  The savings would not be so severe if you were
-        setting 5-10 fields per key
-        
-        Note that `region_msgpack_raw_local` and `region_json_raw_local` should not be
-        used unless you're running a LRU -- they have no expiry.
-        
-        ### Assumptions
-        
-        This demo is assuming a few things that are not tested here (but there are
-        plenty of benchmarks on the internet showing this):
-        
-        * msgpack is the fastest encoder for serializing and deserializing data.
-        * json outperforms cpickle on serializing; cpickle outperforms json on
-          deserializing data.
-        
-        Here are some benchmarks and links:
-        
-        * https://gist.github.com/justinfx/3174062
-        * https://gist.github.com/cactus/4073643
-        * http://www.benfrederickson.com/dont-pickle-your-data/
-        
-        #### Caveats
-        
-        In the examples above, we deal with (de)serializing simple, native, datatypes:
-        `string`, `int`, `bool`, `list`, `dict`, `tuple`.  For these datatypes, msgpack
-        is both the smallest datastore and the fastest performer.
-        
-        If you need to store more complex types, you will need to provide a custom
-        encoder/decoder and will likely suffer a performance hit on the speed of
-        (de)serialization.  Unfortunately, the more complex data types that require
-        custom encoding/decoding include standard `datetime` objects, which can be
-        annoying.
-        
-        The file `custom_serializer.py` shows an example class for handling
-        (de)serialization -- `MsgpackSerializer`.  Some common `datetime` formats are
-        supported; they are encoded as a specially formatted dict, and decoded
-        correspondingly.  A few tricks are used to shave off time and make it roughly
-        comparable to the speed of pickle.
-        
-        
-        ### Key Takeaways
-        
-        * this was surprising - while the differences are negligible on small datasets,
-          using **Redis** to track expiry on long data-sets is generally not a good
-          idea(!). **dogpile.cache** tracks this data much more efficiently.  you can
-          enable an LRU policy in **Redis** to aid in expiry.
-        * msgpack and json are usually fairly comparable in size [remember the
-          assumption that msgpack is better for speed].
-        * reformatting the **dogpile.cache** metadata (replacing a `dict` an `int()` of
-          the expiry) saves a lot of space under JSON when you have small payloads. the
-          strings are a fraction of the size.
-        * msgpack is really good with nested data structures 
-        
-        The following payloads for `1` are strings:
-        
-            region_json_local =        '[10, {"v": 1, "ct": 1471113698.76127}]'
-            region_json_local_int =    '[10, 1471113753]'
-            region_msgpack_local =     '\x92\n\x82\xa1v\x01\xa2ct\xcbA\xd5\xeb\x92\x83\xe9\x97\x9a'
-            region_msgpack_local_int = '\x92\n\xceW\xafct'
-        
-        
-        ### So what should you use?
-        
-        There are several tradeoffs and concepts to consider:
-        
-        1. Do you want to access information outside of **dogpile.cache** (in Python
-           scripts, or even in another language)
-        2. Are you worried about the time to serialize/deserialize?  are you write-heavy
-           or read-heavy?
-        3. Do you want the TTL to be handled by **Redis** or within Python?
-        4. What are your expiry needs?  what do your keys look like?  there may not be
-           any savings possible.  but if you have a lot of recycled prefixes, there
-           could be.
-        5. What do your values look like?  How many are there?
-        
-        This test uses a particular dataset, and differences are inherent to the types
-        of data and keys. Using the strategies from the `region_msgpack_raw_hash` on
-        our production data has consistently dropped a 300MB **Redis** imprint to the
-        60-80MB range.
-        
-        The **Redis** configuration file is also enclosed. The above tests are done with
-        **Redis** compression turned on (which is why memory size fluctuates in the full
-        demo reporting).   
-        
-        
-        Custom Lock Classes
-        -------------------
-        
-        If your Redis db gets flushed the lock will disappear. This will cause the Redis
-        backend to raise an exception EVEN THOUGH you have succeeded in generating your
-        data.
-        
-        By using a ``lock_class``, you can catch the exception and decide what to do --
-        log it?, continue on, raise an error?  It's up to you!
-        
-        	import redis.exceptions
-        
-        	class RedisDistributedLockProxy(object):
-        		"""example lock wrapper
-        		this will silently pass if a LockError is encountered
-        		"""
-        		mutex = None
-        
-        		def __init__(self, mutex):
-        			self.mutex = mutex
-        
-        		def acquire(self, *_args, **_kwargs):
-        			return self.mutex.acquire(*_args, **_kwargs)
-        
-        		def release(self):
-        			# defer imports until backend is used
-        			global redis
-        			import redis  # noqa
-        			try:
-        				self.mutex.release()
-        			except redis.exceptions.LockError, e:
-        				# log.debug("safe lock timeout")
-        				pass
-        			except Exception as e:
-        				raise
-        
-        
-        
-        To Do
-        --------------------------------------
-        
-        I've been experimenting with handling the TTL within a hash bucket (instead of
-        using the **Redis** or **dogpile.cache** methods). This looks promising.  The
-        rationale is that it is easier for **Redis** to get/set an extra field from the
-        same hash, than it is to do separate calls to TTL/EXPIRES.  
-        
-        in code:
-        
-        	- hset('example', 'foo', 'bar')
-        	- expires('example', 3600)
-        	+ hmset('example', {'foo': 'bar',
-        						'expires': time.time() + 3600,
-        						}
-        
-        I've also been experimenting with blessing the result into a subclass of `dict`
-        that would do the object pair decoding lazily as-needed.
-        That would speed up most use cases.
-        
-        
-        Maturity
-        --------------------------------------
-        
-        This package is pre-release.  I've been using these strategies in production
-        via a custom fork of **dogpile.cache** for several years, but am currently
-        migrating it to a plugin.
-        
-        
-        Maintenance and Upstream Compatibility
-        --------------------------------------
-        
-        Some files in /tests are entirely from **dogpile.cache** as-is:
-        
-        *   /tests/conftest.py
-        *   /tests/cache/\__init__.py
-        *   /tests/cache/\_fixtures.py
-                
-        They are versions from **dogpile.cache** 0.6.2
-        
-        The core file, `/cache/backends/redis_advanced.py` inherits from
-        **dogpile.cache**'s `/cache/backends/redis.py`
-        
-        
-        Testing
-        -------
-        
-        This ships with full tests.  
-        
-        Much of the core package and test fixtures are from **dogpile.cache** and
-        copyright from that project, which is available under the MIT license.
-        
-        Tests are handled through tox
-        
-        Examples:
-        
-        ```
-        tox
-        tox -e py27 -- tests/cache/test_redis_backend.py
-        tox -e py27 -- tests/cache/test_redis_backend.py::RedisAdvanced_SerializedRaw_Test
-        tox -e py27 -- tests/cache/test_redis_backend.py::HstoreTest
-        ``` 
-        
-        Tests pass on the enclosed `redis.conf` file:
-        
-        ```/usr/local/Cellar/redis/3.0.7/redis-server ./redis-server--6379.conf```
-        
-        
-        
-        License
-        -------
-        
-        This project is available under the same MIT license as **dogpile.cache**.
-        
 Keywords: caching dogpile
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+![Python package](https://github.com/jvanasco/dogpile_backend_redis_advanced/workflows/Python%20package/badge.svg)
+
+This package supports Python2 and Python3
+
+This package DOES NOT support `dogpile.cache>=1.0`. Support is planned, but there have been several major API changes that are incompatible.
+
+dogpile_backend_redis_advanced
+==============================
+
+This is a plugin for the **dogpile.cache** system that offers some alternatives
+to the standard **Redis** datastore implementation.
+
+Two new backends are offered:
+
+| backend | description |
+| --- | --- |
+| `dogpile_backend_redis_advanced` | extends the `dogpile.cache.redis` backend and allows for custom pickling overrides |
+| `dogpile_backend_redis_advanced_hstore` | extends `dogpile_backend_redis_advanced` and allows for some specific hstore operations |
+
+There is a negligible performance hit in `dogpile_backend_redis_advanced_hstore`,
+as cache keys must be inspected to determine if they are an hstore or not -- and
+there are some operations involved to coordinate values.
+
+Additionally, some behavior is changed:
+
+* The constructor now accepts a ``lock_class`` argument, which can be used to
+  wrap a mutex and alter how releases are handled.  This can be necessary if you
+  have a distributed lock and timeout or flush issues (via LRU or otherwise).
+  A lock disappearing in Redis will raise a fatal exception under the standard
+  Redis backend.
+* The constructor now accepts a ``lock_prefix`` argument, which can be used to
+  alter the prefix used for locks.  The standard Redis backend uses `_lock` as
+  the prefix -- which can be hard to read or isolate for tests.  One might want
+  to use "\_" as the lock prefix (so that `keys "\_*"` will show all locks).
+
+Purpose:
+--------
+
+Mike Bayer's **dogpile.cache** is an excellent package for general purpose
+development.
+
+The system offers 3 key features:
+
+1. Elegant read-through caching functionality.
+2. A locking mechanism that ensures only the first request of a cache-miss will
+   create the resource (turning the rest into consumers of the first-requestor's
+   creation).
+3. Integrated cache expiry against time and library versions.
+
+
+Unfortunately, the integrated cache expiry feature comes at a cost -- objects
+are wrapped into a tuple with some metadata and pickled before hitting the
+datastore.
+
+The additional metadata or pickle format may not be needed or wanted.  Look how
+the size of "a" grows by the time it becomes something passed off to Redis:
+
+
+| type  | example |
+| ----- | ------- |
+| string                        | a                                                                                                               |
+| pickle(string)                | S'a'\np0\n.                                                                                                     |
+| CachedValue(string)           | ('a', {'ct': 1471113698.76127, 'v': 1})                                                                         |
+| pickle(CachedValue(string) )  | cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n. |
+
+By adding in hooks for custom serializers, this backend lets developers choose
+better ways to cache data.  
+
+You may want a serializer that doesn't care about the expiry of cached data, so
+just uses simpler strings.:
+
+| type  | example 1 | example 2 |
+| ----- | --------- | --------- |
+| string                                | a                         | mellifluous                         |
+| json.dumps(string)                    | "a"                       | "mellifluous"                       |
+| msgpack.packb(string)                 | \xa1a                     | \xabmellifluous                     |
+
+Or, you may want to fool **dogpile.cache** by manipulating what the cached is. 
+Instead of using a Python dict, of time and API version, you might just track
+the time but only to the second. 
+
+| type | example 1 | example 2 |
+| ---- | --------- | --------- |
+| AltCachedValue(string)                | ('a', 1471113698)         | ('mellifluous', 1471113698)         |
+| json.dumps(AltCachedValue(string))    | '["a", 1471113698]'       | '["mellifluous", 1471113698]'       |
+| msgpack.packb(AltCachedValue(string)) | '\x92\xa1a\xceW\xafi\xe2' | '\x92\xabmellifluous\xceW\xafi\xe2' |
+
+
+This is how **dogpile.cache** stores "a":
+
+	cdogpile.cache.api\nCachedValue\np0\n(S'a'\np1\n(dp2\nS'ct'\np3\nF1471113698.76127\nsS'v'\np4\nI1\nstp5\nRp6\n.
+
+This package lets us cache a raw string and trick **dogpile.cache** into
+thinking our data parcel is "timely":
+
+	a
+
+Or, we include a simpler version of the time, along with a different serializer.
+
+This packet of data and time:
+
+	["a", 1471113698]
+
+Is then serialized to:
+
+	\x92\xa1a\xceW\xafi\xe2
+	
+If you cache lots of big objects, **dogpile.cache**'s overhead is minimal -- but
+if you have a cache that works for mapping short bits of text, like ids to
+usernames (and vice-versa) you will see considerable savings.
+
+Another way to make **Redis** more efficient is to use hash storage.
+
+Let's say you have a lot of keys that look like this:
+
+	region.set("user-15|posts", x)
+	region.set("user-15|friends", y)
+	region.set("user-15|profile", z)
+	region.set("user-15|username", z1)
+
+You could make **Redis** a bit more efficient by using hash storage, in which
+you have 1 key with multiple fields:
+
+	region.hset("user-15", {'posts': x,
+							'friends', y,
+							'profile', z,
+							'username', z1,
+							})
+
+Redis tends to operate much more efficiently in this situation (more below),
+but you can also save some bytes by not repeating the key prefix. Instagram's
+engineering team has a great article on this
+[Instagram Engineering](http://instagram-engineering.tumblr.com/post/12202313862/storing-hundreds-of-millions-of-simple-key-value).
+
+90% of **dogpile.cache** users who choose **Redis** will never need this
+package.  A decent number of other users with large datasets have been trying to
+squeeze every last bit of memory and performance out of their machines -- and
+this package is designed to facilitate that.
+
+
+Usage:
+------
+
+myfile.py
+
+    # importing will register the plugins
+    import dogpile_backend_redis_advanced
+
+then simply configure **dogpile.cache** with `dogpile_backend_redis_advanced` or 
+`dogpile_backend_redis_advanced_hstore` as the backend.
+
+
+RedisAdvancedBackend
+--------------------
+
+Two new configuration options are offered to specify custom serializers via 
+`loads` and `dumps`.  The default selection is to use **dogpile.cache**'s choice
+of  `pickle`.
+
+This option was designed to support `msgpack` as the serializer:
+
+    import msgpack
+    from dogpile.cache.api import CachedValue
+
+    def msgpack_loads(value):
+        """pickle maintained the `CachedValue` wrapper of the tuple
+           msgpack does not, so it must be added back in.
+           """
+        value = msgpack.unpackb(value, use_list=False)
+        return CachedValue(*value)
+
+    region = make_region().configure(
+        arguments= {'loads': msgpack_loads,
+                    'dumps': msgpack.packb,
+                    }
+        )
+
+
+One can also abuse/misuse **dogpile.cache** and defer all cache expiry to
+**Redis** using this serializer hook.
+
+**dogpile.cache** doesn't cache your value as-is, but wraps it in a CachedValue
+object which contains an API version and a timestamp for the expiry.
+
+This format is necessary for most cache backends, but **Redis** offers the
+ability to handle expiry in the cloud.  By using the slim msgpack format and
+only storing the payload, you can drastically cut down the bytes needed to store
+this information.
+
+This approach SHOULD NOT BE USED by 99% of users.  However, if you do aggressive
+caching, this will allow you to leverage **dogpile.cache**'s excellent locking
+mechanism for handling read-through caching while slimming down your cache size
+and the traffic on-the-wire.  
+
+    import time
+    from dogpile.cache.api import CachedValue
+    from dogpile.cache.region import value_version
+    import msgpack
+
+    def raw_dumps(value):
+        ''''pull the payload out of the CachedValue and serialize that
+        '''
+        value = value.payload
+        value = msgpack.packb(value)
+        return value
+
+    def raw_loads(value):
+        ''''unpack the value and return a CachedValue with the current time
+        '''
+        value = msgpack.unpackb(value, use_list=False)
+        return CachedValue(
+            value,
+            {
+                "ct": time.time(),
+                "v": value_version
+            })
+
+    region = make_region().configure(
+        arguments= {'loads': msgpack_loads,
+                    'dumps': msgpack.packb,
+                    'redis_expiration_time': 1,
+                    }
+        )
+
+
+RedisAdvancedHstoreBackend
+--------------------------
+
+This backend extends **RedisAdvancedBackend** with drop-in support for Hash
+storage under Redis.
+
+* If key names are tuples, they will be treated as hash operations on Redis.
+* By setting `redis_expiration_time_hash` to a boolean value, you can control
+  how expiry times work within Redis
+
+This backend has a slight, negligible, overhead:
+
+* All key operations (`get`/`get_multi`/`set`/`set_multi`/`delete`) require an
+  inspection of keys.
+* `get_multi` requires the order of keys to be tracked, and results from
+  multiple `get`/`hget` operations are then correlated.
+* `set_multi` requires the mapping to be analyzed and bucketed into different
+  hmsets
+
+`redis_expiration_time_hash` allows some extended management of expiry in Redis.
+By default it is set to `None`.
+
+* `False` - ignore hash expiry. (never set a TTL in Redis)
+* `None` - set `redis_expiration_time` on new hash creation only. This requires
+  a check to the **Redis** key before a set.
+* `True` - unconditionally set `redis_expiration_time` on every hash key
+  set/update.
+
+Please note the following:
+
+* **Redis** manages the expiry of hashes on the key, making it global for all
+  fields in the hash.
+* **Redis** does not support setting a TTL on hashes while doing another
+  operation.  TTL must be set via another request.
+* If `redis_expiration_time_hash` is set to `True`, there will be 2 calls to
+  the **Redis** API for every key: `hset` or `hmset` then `expires`.
+* If `redis_expiration_time_hash` is set to `None`, there will be 2-3 calls to
+  the **Redis** API for every key: `exists`, `hset` or `hmset`, and possibly
+  `expires`.
+
+
+Memory Savings and Suggested Usage
+--------------------------------------
+
+Redis is an in-memory datastore that offers persistence -- optimizing storage is
+incredibly important because the entire set must be held in-memory.
+
+### Example Demo
+
+The attached `demo.py` (results in `demo.txt`) shows some potential approaches
+to caching and hashing by priming a **Redis** datastore with some possible
+strategies of a single dataset.
+
+It's worth looking at `demo.txt` to see how the different serializesr encode the
+data -- sample keys are pulled for each format.
+
+| test                     | memory bytes | memory human | relative | ttl on Redis? | ttl in dogpile? | backend                                 | encoder |
+| ------------------------ | ------------ | ------------ | -------- | ------------- | --------------- | --------------------------------------- | ------- |
+| region_redis             | 249399504    | 237.85M      | 0%       | Y             | Y               | `dogpile.cache.redis`                   | pickle  |
+| region_json              | 222924496    | 212.60M      | 89.38%   | Y             | Y               | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack           | 188472048    | 179.74M      | 75.57%   | Y             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_redis_local       | 181501200    | 173.09M      | 72.78%   | -             | Y               | `dogpile.cache.redis`                   | pickle  |
+| region_json_raw          | 171554880    | 163.61M      | 68.79%   | Y             | -               | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack_raw       | 170765872    | 162.86M      | 68.47%   | Y             | -               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_json_local        | 162612752    | 155.08M      | 65.20%   | -             | Y               | `dogpile_backend_redis_advanced`        | json    |
+| region_json_local_int    | 128648576    | 122.69M      | 57.71%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack_local     | 128160048    | 122.22M      | 51.39%   | -             | Y               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_msgpack_local_int | 126938576    | 121.06M      | 50.89%   | -             | Y, `int(time)`  | `dogpile_backend_redis_advanced`        | msgpack |
+| region_json_raw_local    | 111241280    | 106.09M      | 44.60%   | -             | -               | `dogpile_backend_redis_advanced`        | json    |
+| region_msgpack_raw_local | 110455968    | 105.34M      | 44.29%   | -             | -               | `dogpile_backend_redis_advanced`        | msgpack |
+| region_msgpack_raw_hash  | 28518864     | 27.20M       | 11.44%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | msgpack |
+| region_json_raw_hash     | 24836160     | 23.69M       |  9.96%   | Y, only keys  | -               | `dogpile_backend_redis_advanced_hstore` | json    |
+
+Notes:
+
+* the `_local` variants do not set a TTL on Redis
+* the `_raw` variants strip out the dogpile CachedValue wrapper and only store
+  the payload
+* the `_msgpack` variants use msgpack instead of pickle 
+* the `_json` variants use json instead of pickle 
+* the `_int` variant applies int() to the dogpile timestamp, dropping a few
+  bytes per entry
+
+Wait WHAT? LOOK AT `region_msgpack_raw_hash` and `region_json_raw_hash` - that's
+a HUGE savings!
+
+Yes.
+
+The HSTORE has considerable savings due to 2 reasons:
+
+* **Redis** internally manages a hash much more effectively than keys.
+* **Redis** will only put an expiry on the keys (buckets), not the hash fields
+
+HSTORE ends up being a much tighter memory usage for this example set, as we're
+setting 100 fields in each key.  The savings would not be so severe if you were
+setting 5-10 fields per key
+
+Note that `region_msgpack_raw_local` and `region_json_raw_local` should not be
+used unless you're running a LRU -- they have no expiry.
+
+### Assumptions
+
+This demo is assuming a few things that are not tested here (but there are
+plenty of benchmarks on the internet showing this):
+
+* msgpack is the fastest encoder for serializing and deserializing data.
+* json outperforms cpickle on serializing; cpickle outperforms json on
+  deserializing data.
+
+Here are some benchmarks and links:
+
+* https://gist.github.com/justinfx/3174062
+* https://gist.github.com/cactus/4073643
+* http://www.benfrederickson.com/dont-pickle-your-data/
+
+#### Caveats
+
+In the examples above, we deal with (de)serializing simple, native, datatypes:
+`string`, `int`, `bool`, `list`, `dict`, `tuple`.  For these datatypes, msgpack
+is both the smallest datastore and the fastest performer.
+
+If you need to store more complex types, you will need to provide a custom
+encoder/decoder and will likely suffer a performance hit on the speed of
+(de)serialization.  Unfortunately, the more complex data types that require
+custom encoding/decoding include standard `datetime` objects, which can be
+annoying.
+
+The file `custom_serializer.py` shows an example class for handling
+(de)serialization -- `MsgpackSerializer`.  Some common `datetime` formats are
+supported; they are encoded as a specially formatted dict, and decoded
+correspondingly.  A few tricks are used to shave off time and make it roughly
+comparable to the speed of pickle.
+
+
+### Key Takeaways
+
+* this was surprising - while the differences are negligible on small datasets,
+  using **Redis** to track expiry on long data-sets is generally not a good
+  idea(!). **dogpile.cache** tracks this data much more efficiently.  you can
+  enable an LRU policy in **Redis** to aid in expiry.
+* msgpack and json are usually fairly comparable in size [remember the
+  assumption that msgpack is better for speed].
+* reformatting the **dogpile.cache** metadata (replacing a `dict` an `int()` of
+  the expiry) saves a lot of space under JSON when you have small payloads. the
+  strings are a fraction of the size.
+* msgpack is really good with nested data structures 
+
+The following payloads for `1` are strings:
+
+    region_json_local =        '[10, {"v": 1, "ct": 1471113698.76127}]'
+    region_json_local_int =    '[10, 1471113753]'
+    region_msgpack_local =     '\x92\n\x82\xa1v\x01\xa2ct\xcbA\xd5\xeb\x92\x83\xe9\x97\x9a'
+    region_msgpack_local_int = '\x92\n\xceW\xafct'
+
+
+### So what should you use?
+
+There are several tradeoffs and concepts to consider:
+
+1. Do you want to access information outside of **dogpile.cache** (in Python
+   scripts, or even in another language)
+2. Are you worried about the time to serialize/deserialize?  are you write-heavy
+   or read-heavy?
+3. Do you want the TTL to be handled by **Redis** or within Python?
+4. What are your expiry needs?  what do your keys look like?  there may not be
+   any savings possible.  but if you have a lot of recycled prefixes, there
+   could be.
+5. What do your values look like?  How many are there?
+
+This test uses a particular dataset, and differences are inherent to the types
+of data and keys. Using the strategies from the `region_msgpack_raw_hash` on
+our production data has consistently dropped a 300MB **Redis** imprint to the
+60-80MB range.
+
+The **Redis** configuration file is also enclosed. The above tests are done with
+**Redis** compression turned on (which is why memory size fluctuates in the full
+demo reporting).   
+
+
+Custom Lock Classes
+-------------------
+
+If your Redis db gets flushed the lock will disappear. This will cause the Redis
+backend to raise an exception EVEN THOUGH you have succeeded in generating your
+data.
+
+By using a ``lock_class``, you can catch the exception and decide what to do --
+log it?, continue on, raise an error?  It's up to you!
+
+	import redis.exceptions
+
+	class RedisDistributedLockProxy(object):
+		"""example lock wrapper
+		this will silently pass if a LockError is encountered
+		"""
+		mutex = None
+
+		def __init__(self, mutex):
+			self.mutex = mutex
+
+		def acquire(self, *_args, **_kwargs):
+			return self.mutex.acquire(*_args, **_kwargs)
+
+		def release(self):
+			# defer imports until backend is used
+			global redis
+			import redis  # noqa
+			try:
+				self.mutex.release()
+			except redis.exceptions.LockError, e:
+				# log.debug("safe lock timeout")
+				pass
+			except Exception as e:
+				raise
+
+
+
+To Do
+--------------------------------------
+
+I've been experimenting with handling the TTL within a hash bucket (instead of
+using the **Redis** or **dogpile.cache** methods). This looks promising.  The
+rationale is that it is easier for **Redis** to get/set an extra field from the
+same hash, than it is to do separate calls to TTL/EXPIRES.  
+
+in code:
+
+	- hset('example', 'foo', 'bar')
+	- expires('example', 3600)
+	+ hmset('example', {'foo': 'bar',
+						'expires': time.time() + 3600,
+						}
+
+I've also been experimenting with blessing the result into a subclass of `dict`
+that would do the object pair decoding lazily as-needed.
+That would speed up most use cases.
+
+
+Maturity
+--------------------------------------
+
+This package is pre-release.  I've been using these strategies in production
+via a custom fork of **dogpile.cache** for several years, but am currently
+migrating it to a plugin.
+
+
+Maintenance and Upstream Compatibility
+--------------------------------------
+
+Some files in /tests are entirely from **dogpile.cache** as-is:
+
+*   /tests/conftest.py
+*   /tests/cache/\__init__.py
+*   /tests/cache/\_fixtures.py
+        
+They are versions from **dogpile.cache** 0.6.2
+
+The core file, `/cache/backends/redis_advanced.py` inherits from
+**dogpile.cache**'s `/cache/backends/redis.py`
+
+
+Testing
+-------
+
+This ships with full tests.  
+
+Much of the core package and test fixtures are from **dogpile.cache** and
+copyright from that project, which is available under the MIT license.
+
+Tests are handled through tox
+
+Examples:
+
+```
+tox
+tox -e py27 -- tests/cache/test_redis_backend.py
+tox -e py27 -- tests/cache/test_redis_backend.py::RedisAdvanced_SerializedRaw_Test
+tox -e py27 -- tests/cache/test_redis_backend.py::HstoreTest
+``` 
+
+Tests pass on the enclosed `redis.conf` file:
+
+```/usr/local/Cellar/redis/3.0.7/redis-server ./redis-server--6379.conf```
+
+
+
+License
+-------
+
+This project is available under the same MIT license as **dogpile.cache**.
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/src/dogpile_backend_redis_advanced.egg-info/SOURCES.txt` & `dogpile_backend_redis_advanced-0.4.0/src/dogpile_backend_redis_advanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dogpile_backend_redis_advanced-0.3.2/tests/cache/_fixtures.py` & `dogpile_backend_redis_advanced-0.4.0/tests/cache/_fixtures.py`

 * *Files identical despite different names*

### Comparing `dogpile_backend_redis_advanced-0.3.2/tests/cache/test_redis_backend.py` & `dogpile_backend_redis_advanced-0.4.0/tests/cache/test_redis_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 from mock import patch, Mock
 import msgpack
 import pytest
 
 REDIS_HOST = "127.0.0.1"
 REDIS_PORT = int(os.getenv("DOGPILE_REDIS_PORT", "6379"))
 
-COMPAT_PY3 = True if (sys.version_info > (3, 0)) else False
-
-
 # import to register the plugin
 import dogpile_backend_redis_advanced
 
 """
 ABOUT THESE TESTS
 
 Compatibility Tests
@@ -191,19 +188,16 @@
 def my_loads(value):
     """'
     we need to unpack the value and stash it into a CachedValue
     we support strings in this version, because it's used in unit tests
     that require the ability to set/read raw data.
     we could disable that test, but this workaround supports it.
     """
-    if COMPAT_PY3:
-        # this is True for backward compatibility
-        value = msgpack.unpackb(value, use_list=False, raw=False)
-    else:
-        value = msgpack.unpackb(value, use_list=False)
+    # this is True for backward compatibility
+    value = msgpack.unpackb(value, use_list=False, raw=False)
     if isinstance(value, tuple):
         return CachedValue(*value)
     return value
 
 
 class _SerializedAlternate_Test(_TestRedisConn, _GenericBackendTest):
     config_args = {
@@ -229,19 +223,15 @@
 # ==============================================================================
 
 
 def raw_loads(value):
     """'
     we need to unpack the value and stash it into a CachedValue
     """
-    if COMPAT_PY3:
-        # this is True for backward compatibility
-        value = msgpack.unpackb(value, use_list=False, raw=False)
-    else:
-        value = msgpack.unpackb(value, use_list=False)
+    value = msgpack.unpackb(value, use_list=False, raw=False)
     return CachedValue(value, {"ct": time.time(), "v": value_version})
 
 
 def raw_dumps(value):
     if isinstance(value, CachedValue):
         value = value.payload
     value = msgpack.packb(value)
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/tests/conftest.py` & `dogpile_backend_redis_advanced-0.4.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 import logging
 
 import logging.config
 
 logging.config.fileConfig("log_tests.ini")
 
 
-import six
-
-
 def is_unittest(obj):
     """Is obj a subclass of unittest.TestCase?
 
     Lifted from older versions of py.test, as this seems to be removed.
 
     """
     unittest = sys.modules.get("unittest")
@@ -25,16 +22,13 @@
         raise
     except:
         return False
 
 
 def pytest_pycollect_makeitem(collector, name, obj):
     if is_unittest(obj) and not obj.__name__.startswith("_"):
-        if six.PY3:
-            # pytest changed in 5.4.0; things behave differently on py2 & py3
-            return UnitTestCase.from_parent(collector, name=name)
-        else:
-            # pytest 4.6 is the last to support py2.7
-            # https://docs.pytest.org/en/stable/py27-py34-deprecation.html
-            return UnitTestCase(name, parent=collector)
+        # pytest changed in 5.4.0; things behave differently on py2 & py3
+        return UnitTestCase.from_parent(collector, name=name)
+        # pytest 4.6 is the last to support py2.7
+        # https://docs.pytest.org/en/stable/py27-py34-deprecation.html
     else:
         return []
```

### Comparing `dogpile_backend_redis_advanced-0.3.2/tox.ini` & `dogpile_backend_redis_advanced-0.4.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 [tox]
 minversion=1.8.dev1
-envlist = py{27,36}
+envlist =
+	lint,
+	mypy,
+	py36,py37,py38,py39,py310,py311
 
 [testenv]
-cov_args=--cov=dogpile --cov-append --cov-report term --cov-report xml
+extras =
+    testing
 
+cov_args=--cov=dogpile --cov-append --cov-report term --cov-report xml
 
 setenv=
 	BASECOMMAND=python -m pytest
 
 	{generic}: 	RUNTESTS=-k 'not test_redis_backend not _fixtures'
 
 	{redis}: PIFPAF=pifpaf --env-prefix DOGPILE run redis --port {env:TOX_DOGPILE_PORT:6379} --
 	{redis}: RUNTESTS=tests/cache/test_redis_backend.py
 
     {cov}: COVERAGE={[testenv]cov_args}
 
 
 deps=
-	dogpile.cache<1.0.0
+	dogpile.cache<1.0
 	pytest
 	mock
 	msgpack-python
 	redis
 
 	{redis}: redis
 	{redis}: pifpaf
```

