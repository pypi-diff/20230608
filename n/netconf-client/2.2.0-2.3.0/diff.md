# Comparing `tmp/netconf_client-2.2.0.tar.gz` & `tmp/netconf_client-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netconf_client-2.2.0.tar", max compression
+gzip compressed data, was "netconf_client-2.3.0.tar", max compression
```

## Comparing `netconf_client-2.2.0.tar` & `netconf_client-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1528 2023-03-02 14:42:21.746430 netconf_client-2.2.0/README.md
--rw-r--r--   0        0        0        0 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/__init__.py
--rw-r--r--   0        0        0     6598 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/connect.py
--rw-r--r--   0        0        0      511 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/constants.py
--rw-r--r--   0        0        0     1911 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/error.py
--rw-r--r--   0        0        0       61 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/log.py
--rw-r--r--   0        0        0    18737 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/ncclient.py
--rw-r--r--   0        0        0     4401 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/parser.py
--rw-r--r--   0        0        0     5621 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/rpc.py
--rw-r--r--   0        0        0     4795 2023-03-02 14:42:21.746430 netconf_client-2.2.0/netconf_client/session.py
--rw-r--r--   0        0        0      961 2023-03-02 14:42:21.746430 netconf_client-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 netconf_client-2.2.0/setup.py
--rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 netconf_client-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1528 2023-06-08 18:09:51.081109 netconf_client-2.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/__init__.py
+-rw-r--r--   0        0        0     7190 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/connect.py
+-rw-r--r--   0        0        0      511 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/constants.py
+-rw-r--r--   0        0        0     1911 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/error.py
+-rw-r--r--   0        0        0       61 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/log.py
+-rw-r--r--   0        0        0    18737 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/ncclient.py
+-rw-r--r--   0        0        0     4401 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/parser.py
+-rw-r--r--   0        0        0     5621 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/rpc.py
+-rw-r--r--   0        0        0     4795 2023-06-08 18:09:51.081109 netconf_client-2.3.0/netconf_client/session.py
+-rw-r--r--   0        0        0      961 2023-06-08 18:09:51.085109 netconf_client-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 netconf_client-2.3.0/setup.py
+-rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 netconf_client-2.3.0/PKG-INFO
```

### Comparing `netconf_client-2.2.0/README.md` & `netconf_client-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `netconf_client-2.2.0/netconf_client/connect.py` & `netconf_client-2.3.0/netconf_client/connect.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     port=830,
     username="netconf",
     password=None,
     key_filename=None,
     sock=None,
     timeout=120,
     hostkey_b64=None,
+    initial_timeout=None,
+    general_timeout=None,
 ):
     """Connect to a NETCONF server over SSH.
 
     :param str host: Hostname or IP address; unused if an already-open
                      socket is provided
 
     :param int port: TCP port to initiate the connection; unused if an
@@ -34,26 +36,36 @@
 
     :param str key_filename: Path to an SSH private key; not required
                              if a password is provided instead
 
     :param sock: An already-open TCP socket; SSH will be setup on top
                  of it
 
-    :param int timeout: Seconds to wait when connecting the socket
+    :param int initial_timeout: Seconds to wait when first connecting the socket.
+
+    :param int general_timeout: Seconds to wait for a response from the server after connecting.
+
+    :param int timeout: (Deprecated) Seconds to wait when connecting the socket if initial_timeout is None.  This will
+                        be ignored if initial_timeout is not None, and will be removed in the next major release.
+
+    :param str hostkey_b64: (Deprecated) Base64-encoded SSH host key.  This will
+    be ignored if hostkey_b64 is not None.
+
+    :return: :class:`Session` object
 
     :param str hostkey_b64: base64 encoded hostkey.
 
     :rtype: :class:`netconf_client.session.Session`
 
     """
     if not sock:
         sock = socket.socket()
-        sock.settimeout(timeout)
+        sock.settimeout(initial_timeout or timeout)
         sock.connect((host, port))
-        sock.settimeout(None)
+        sock.settimeout(general_timeout)
     transport = paramiko.transport.Transport(sock)
     pkey = _try_load_pkey(key_filename) if key_filename else None
     hostkey = _try_load_hostkey_b64(hostkey_b64) if hostkey_b64 else None
     transport.connect(hostkey=hostkey, username=username, password=password, pkey=pkey)
     channel = transport.open_session()
     channel.invoke_subsystem("netconf")
     bundle = SshSessionSock(sock, transport, channel)
```

### Comparing `netconf_client-2.2.0/netconf_client/error.py` & `netconf_client-2.3.0/netconf_client/error.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.2.0/netconf_client/ncclient.py` & `netconf_client-2.3.0/netconf_client/ncclient.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.2.0/netconf_client/parser.py` & `netconf_client-2.3.0/netconf_client/parser.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.2.0/netconf_client/rpc.py` & `netconf_client-2.3.0/netconf_client/rpc.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.2.0/netconf_client/session.py` & `netconf_client-2.3.0/netconf_client/session.py`

 * *Files identical despite different names*

### Comparing `netconf_client-2.2.0/pyproject.toml` & `netconf_client-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netconf_client"
-version = "2.2.0"
+version = "2.3.0"
 description = "A Python NETCONF client"
 authors = ["ADTRAN, Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ADTRAN/netconf_client"
 repository = "https://github.com/ADTRAN/netconf_client"
 documentation = "https://netconf-client.readthedocs.io"
```

### Comparing `netconf_client-2.2.0/setup.py` & `netconf_client-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['lxml>=4.6.3,<5.0.0', 'paramiko>=2.7.2,<4']
 
 setup_kwargs = {
     'name': 'netconf-client',
-    'version': '2.2.0',
+    'version': '2.3.0',
     'description': 'A Python NETCONF client',
     'long_description': '![Build Status](https://github.com/ADTRAN/netconf_client/workflows/CI%20Checks/badge.svg)\n[![PyPI version](https://badge.fury.io/py/netconf-client.svg)](https://badge.fury.io/py/netconf-client)\n[![Documentation Status](https://readthedocs.org/projects/netconf-client/badge/?version=latest)](https://netconf-client.readthedocs.io/en/latest/?badge=latest)\n\n# netconf_client\n\nA NETCONF client for Python 3.6+.\n\n## Basic Usage\n\n```python\nfrom netconf_client.connect import connect_ssh\nfrom netconf_client.ncclient import Manager\n\nsession = connect_ssh(host="localhost", port=830, username="admin", password="password")\nmgr = Manager(session, timeout=120)\n\nmgr.edit_config(config="""<config> ... </config>""")\nprint(mgr.get(filter="""<filter> ... </filter>""").data_xml)\n```\n\nMore complete documentation can be found in the [User Guide]\n\n## Comparison with `ncclient`\n\nCompared to [ncclient](https://github.com/ncclient/ncclient),\n`netconf_client` has several advantages:\n\n - It\'s simpler (at the time of writing: 789 LoC vs 2889 LoC)\n - lxml can be bypassed, which can work around issues where lxml\n   breaks namespaces of e.g. identityrefs\n - Support for TLS sessions\n\nAnd a few disadvantages:\n\n - Support for non-RFC-compliant devices isn\'t really included in\n   `netconf_client`\n - `netconf_client` does a lot less error checking and assumes you\'re\n   sending valid messages to the server (however this can be useful\n   for testing edge-case behavior of a server)\n\n\n[User Guide]: https://netconf-client.readthedocs.io/en/latest/\n',
     'author': 'ADTRAN, Inc.',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ADTRAN/netconf_client',
```

### Comparing `netconf_client-2.2.0/PKG-INFO` & `netconf_client-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netconf-client
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Python NETCONF client
 Home-page: https://github.com/ADTRAN/netconf_client
 License: Apache-2.0
 Keywords: netconf
 Author: ADTRAN, Inc.
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

