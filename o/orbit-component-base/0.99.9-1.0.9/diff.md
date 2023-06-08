# Comparing `tmp/orbit_component_base-0.99.9.tar.gz` & `tmp/orbit_component_base-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-0.99.9.tar", max compression
+gzip compressed data, was "orbit_component_base-1.0.9.tar", max compression
```

## Comparing `orbit_component_base-0.99.9.tar` & `orbit_component_base-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/LICENSE.md
--rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/README.md
--rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      698 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1020 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/schema/OrbitUsers.py
--rwxr-xr-x   0        0        0     3506 2023-05-30 20:47:27.827498 orbit_component_base-0.99.9/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     6315 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     6281 2023-05-30 16:47:54.685910 orbit_component_base-0.99.9/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-0.99.9/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     8612 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6409 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     2293 2023-05-30 15:19:20.188832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     1243 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     2329 2023-05-30 21:39:29.016203 orbit_component_base-0.99.9/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/src/orbit_version.py
--rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-0.99.9/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0       23 2023-05-31 19:03:52.281919 orbit_component_base-0.99.9/orbit_component_base/version.py
--rw-r--r--   0        0        0     1395 2023-05-31 19:03:52.281919 orbit_component_base-0.99.9/pyproject.toml
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 orbit_component_base-0.99.9/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/README.md
+-rw-r--r--   0        0        0      248 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-07 22:18:42.405891 orbit_component_base-1.0.9/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1290 2023-06-08 11:30:57.895776 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitUsers.py
+-rw-r--r--   0        0        0     1787 2023-06-08 11:31:11.007490 orbit_component_base-1.0.9/orbit_component_base/schema/OrbitVersions.py
+-rwxr-xr-x   0        0        0     3603 2023-06-08 10:02:49.715966 orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6551 2023-06-08 12:34:02.238300 orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6878 2023-06-05 13:02:31.115557 orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-30 16:30:11.592032 orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-06-07 11:18:34.376181 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-30 15:19:20.188832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6554 2023-06-07 23:22:03.266791 orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2983 2023-06-08 12:54:23.664990 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     2148 2023-06-02 16:17:04.740333 orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2323 2023-06-05 13:10:08.334760 orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-30 15:19:20.192832 orbit_component_base-1.0.9/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0       22 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/orbit_component_base/version.py
+-rw-r--r--   0        0        0     1394 2023-06-08 17:25:09.459041 orbit_component_base-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 orbit_component_base-1.0.9/PKG-INFO
```

### Comparing `orbit_component_base-0.99.9/LICENSE.md` & `orbit_component_base-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_app.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,53 +38,55 @@
         'engineio_logger': False,
         'cors_allowed_origins': '*'
     }
 
     def __init__ (self, app=None):
         if app:
             self.APPLICATION = app
-        self._modules = []
+        self._router = None
 
     async def startup (self, app=None):
-        for module in self._modules:
-            module.open()
+        if world.conf.sio_debug:
+            self.SERVER_PARAMS['logger'] = self.LOGGER()
+        sio = world.sio = AsyncServer(**self.SERVER_PARAMS)
+        odb = self.MAINDB().open()
+        
+        for plugin in Plugins('Plugin'):
+            plugin = plugin.Plugin(odb=odb).open().register(sio)
+            sio.attach(app, socketio_path=plugin.ns)
+            self._router.add_namespace(plugin.NAMESPACE)
 
     async def shutdown(self, app=None):
         await sleep(1)
         raise GracefulExit()
 
     def run (self):
         set_start_method('spawn')
         freeze_support()
+       
+        world.conf = self.CONFIG(self.APPLICATION).open()       
+
         parser = ArgumentParser()
-        plugins = [plugin.Args(parser=parser).setup() for plugin in Plugins('Args')]
-        world.conf = self.CONFIG(self.APPLICATION).open()
-        world.args = parser.parse_args()
-        odb = self.MAINDB().open()
-        for plugin in plugins:
-            plugin.open(odb=odb, args=world.args).process()
-        if not 'run' in world.args:
+        for plugin in Plugins('Args'):
+            plugin.Args(parser=parser).setup()
+        world.args = parser.parse_args()        
+
+        if not world.args.run:
+            odb = self.MAINDB().open()
+            for plugin in Plugins('Plugin'):
+                plugin = plugin.Plugin(odb=odb).open(nql=False)
+            for plugin in Plugins('Args'):
+                plugin.Args(parser=parser).open(odb, world.args).process()
             print('Please add "run" if you wish to launch the application')
             exit()
-    
-        if world.conf.sio_debug:
-            self.SERVER_PARAMS['logger'] = self.LOGGER()
-        sio = world.sio = AsyncServer(**self.SERVER_PARAMS)
-
-        router = self.ROUTER()
+  
+        self._router = router = self.ROUTER()
         app = router.application()
         app.on_startup.append(self.startup)
         app.on_shutdown.append(self.shutdown)
-
-        for plugin in Plugins('Plugin'):
-            plugin = plugin.Plugin(odb=odb)
-            sio.attach(app, socketio_path=plugin.ns)
-            sio.register_namespace(plugin)
-            self._modules.append(plugin)
-            router.add_namespace(plugin.NAMESPACE)
         try:
             if world.conf.secure:
                 ssl = self.MAKSSL().open()        
                 ssl_context = create_default_context(Purpose.CLIENT_AUTH)
                 ssl_context.load_cert_chain(ssl.crt, ssl.key)
                 web.run_app(
                     app,
```

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,21 @@
             user_id = cipher.decrypt(b64decode(secret)).decode()
             user = UsersTable().from_key(host_id)
             if user.isValid:
                 if user._user_id == user_id:
                     if user._active or world.conf.authentication == 'autoenroll':
                         session['activated'] = True
                         session['perm'] = user._perm
-                        await save_session(self._sid, session)
-                        self.activate_session(user._user_id, auth, session)
+                        log.debug(f'Save: {self._sid} / {self._ns} => {session}')
+                        try:
+                            await save_session(self._sid, session)
+                            self.activate_session(user._user_id, auth, session)
+                        except Exception as e:
+                            log.error(e)
+                            
                         return {'ok': True, 'validate': False}
                     return {'ok': True, 'validate': True}
                 else:
                     log.warning(f'login failure, wanted: {user._user_id}, found: {user_id}')
                     return {'ok': False, 'error': 'Lgin failed'}
             else:
                 activate = (UsersCollection().records() == 0 and
```

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_config.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 from configparser import ConfigParser
 from pathlib import Path
 from datetime import datetime
 from loguru import logger as log
-from warnings import filterwarnings
 from orbit_component_base.src.orbit_shared import world
 from platform import system
 
 
 class OrbitConfig:
 
     BASE_authentication = 'autoenroll'
@@ -34,17 +33,14 @@
     @property
     def host (self):            return self._conf.get('NETWORK', 'host')
 
     @property
     def port (self):            return self._conf.getint('NETWORK', 'port')
 
     @property
-    def local_port (self):      return self._conf.getint('NETWORK', 'local_port')
-
-    @property
     def sio_debug (self):       return self._conf.getboolean('NETWORK', 'sio_debug')
 
     @property
     def engineio_debug (self):  return self._conf.getboolean('NETWORK', 'engineio_debug')
 
     @property
     def vite_port (self):       return self._conf.getint('DEV', 'vite_port')
@@ -86,16 +82,17 @@
             log.remove()
             Path(self.logs).mkdir(exist_ok=True)
             log.add((self.logs / 'orbit_access.log').as_posix(), level='RPC', colorize=True, rotation="10 MB", retention="3 days",
                 filter=lambda record: record['name'] == 'src.orbit_decorators', enqueue=True)
             log.add((self.logs / 'orbit_system.log').as_posix(), colorize=True, rotation="10 MB", retention="3 days",
                 filter=lambda record: record['name'] != 'src.orbit_decorators', enqueue=True)
 
-    def _option (self, section, name, value):
+    def _option (self, section, name, value, comment):
         if not self._conf.has_option(section, name):
+            self._conf.set(section, f'# {name}', comment)
             self._conf.set(section, name, value)
             self._changed = True
 
     def mkpath (self, section, option):
         return self.mk(section, option, self.path)
     
     def mkcode (self, section, option):
@@ -120,33 +117,32 @@
         self._conf = ConfigParser()
         self._conf.read(self._file.as_posix())
         for section in ['BASE', 'NETWORK', 'TOOLS', 'DATA', 'SSL', 'DEV']:
             if section not in self._conf.sections():
                 self._conf.add_section(section)
                 self._changed = True
         code_path = f'/Applications/{self._appl}.app/Contents/Resources/' if system() == 'Darwin' else f'/opt/{self._appl}'
-        self._option('BASE', 'path', f'~/.local/{self._appl}')
-        self._option('BASE', 'code', code_path)
-        self._option('BASE', 'authentication', self.BASE_authentication)
-        self._option('SSL', 'name', 'localhost')
-        self._option('SSL', 'ssl', 'ssl')
-        self._option('SSL', 'secure', 'true')
-        self._option('NETWORK', 'host', '127.0.0.1')
-        self._option('NETWORK', 'port', '8445')
-        self._option('NETWORK', 'local_port', '8445')
-        self._option('DEV', 'vite_port', '5173')
-        self._option('NETWORK', 'sio_debug', 'false')
-        self._option('NETWORK', 'engineio_debug', 'false')
-        self._option('DATA', 'database', 'orbit_database')
-        self._option('DATA', 'tmp', 'tmp')
-        self._option('DATA', 'templates', 'templates')
-        self._option('DATA', 'web', 'web')
-        self._option('DATA', 'logs', 'logs')
-        self._option('DATA', 'writemap', 'true')        
-        self._option('TOOLS', 'make_keys', 'scripts/make_keys.sh')
+        self._option('BASE', 'path', f'~/.local/{self._appl}', 'base location for this application')
+        self._option('BASE', 'code', code_path, "where the application's code is located")
+        self._option('BASE', 'authentication', self.BASE_authentication, 'the default type of authentication (autoenroll/secure)')
+        self._option('SSL', 'name', 'localhost', 'the host name (CN) for our SSL certificate')
+        self._option('SSL', 'ssl', 'ssl', 'the folder to store SSL files in')
+        self._option('SSL', 'secure', 'true', 'whether to use SSL or not')
+        self._option('NETWORK', 'host', '127.0.0.1', 'the host to expose the server on, use "0.0.0.0" for a local network')
+        self._option('NETWORK', 'port', '8445', "the port to expose the server on")
+        self._option('DEV', 'vite_port', '5173', 'the port to run "vite" on')
+        self._option('NETWORK', 'sio_debug', 'false', 'SIO debugging')
+        self._option('NETWORK', 'engineio_debug', 'false', 'AIO debugging')
+        self._option('DATA', 'database', 'orbit_database', 'the path name of the folder to store data in')
+        self._option('DATA', 'tmp', 'tmp', 'the path name of a temporary folder')
+        self._option('DATA', 'templates', 'templates', 'the path name of the folder to store templates in')
+        self._option('DATA', 'web', 'web', 'the path name of the folder to store web assets for in production mode')
+        self._option('DATA', 'logs', 'logs', 'the path name of the folder to store logs in')
+        self._option('DATA', 'writemap', 'true', 'whether to use WRITEMAP on the database')
+        self._option('TOOLS', 'make_keys', 'scripts/make_keys.sh', 'the folder we store our make_keys script in')
         if self._changed:
             with open(self._file.as_posix(), 'w') as configfile:
                 self._conf.set('DEFAULT', 'updated', datetime.now().isoformat())
                 self._conf.write(configfile)
         self.setup_logging()                
         return self
 
@@ -155,14 +151,13 @@
     conf = OrbitConfig('Demo').open()
     print("Path           =", conf.path)
     print("Code           =", conf.code)
     print("Name           =", conf.name)
     print("SSL            =", conf.ssl)
     print("Host           =", conf.host)
     print("Port           =", conf.port)
-    print("Local Port     =", conf.local_port)
     print("sio_debug      =", conf.sio_debug)
     print("engineio_debug =", conf.engineio_debug)
     print("make_keys      =", conf.make_keys)
     print("database       =", conf.database)
     print("templates      =", conf.templates)
     print("web            =", conf.web)
```

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_database.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_database.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_decorators.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_nql_session.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,18 @@
     _nql = None
     _api = {}
 
     table_class = None
     table_strip = None
     table_methods = []
 
-    def __init__ (self, sid=None, session=None):
+    def __init__ (self, sid=None, session=None, ns=None):
         self._sid = sid
         self._session = session
+        self._ns = ns
 
     def __iter__ (self, param=None):
         return self.table_class().norm_tb.filter()
 
     @property
     def write_transaction (self):
         return WriteTransaction(self._dbh._database)
@@ -145,19 +146,22 @@
     async def callback(self, docs):
         try:
             await self._nql.update(self.table_class.norm_table_name, docs)
         except Exception as e:
             log.exception(e)
        
     def filter(self, *args, **kwargs):
-        if self.table_class.norm_tb:
-            return self.table_class.norm_tb.filter(*args, **kwargs)
-        else:
-            log.error(f'table not initialised: {self.table_class}')
-            return []
+        try:
+            if self.table_class.norm_tb:
+                return self.table_class.norm_tb.filter(*args, **kwargs)
+            else:
+                log.error(f'table not initialised: {self.table_name} // {self.table_class}')
+                return []
+        except Exception as e:
+            log.exception(e)
 
     def records(self, transaction=None):
         return self.table_class.norm_tb.records()
 
     def empty(self, transaction=None):
         if self.table_class.norm_tb is not None:
             return self.table_class.norm_tb.empty(txn=transaction)
```

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugin.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 from socketio import AsyncNamespace
 from orbit_component_base.src.orbit_nql import NQL
 from orbit_component_base.src.orbit_auth import OrbitAuth
 from orbit_component_base.src.orbit_decorators import navGuard
 from orbit_component_base.schema.OrbitSessions import SessionsCollection
+from orbit_component_base.schema.OrbitSessions import SessionsTable
+from orbit_component_base.schema.OrbitVersions import VersionsCollection
 from loguru import logger as log
 
 
 class PluginBase (AsyncNamespace):
 
     NAMESPACE = ''
     COLLECTIONS = []
 
     @property
     def ns (self):
         return f'/{self.NAMESPACE}'
 
     def __init__(self, *args, **kwargs):
-        log.success(f'Initialise namespace: {self.ns}')
+        log.debug(f'Initialise namespace: {self.ns}')
         kwargs['namespace'] = self.ns
         self._odb = kwargs.pop('odb')
-        self._nql = NQL(self.emit, self.ns)
+        self._nql = None
         self._collections = []
         super().__init__(*args, **kwargs)
 
-    def open (self):
-        self._nql.open()
+    def open (self, nql=True):
+        if nql:
+            self._nql = NQL(self.emit, self.ns).open()
         for cls in self.COLLECTIONS:
             cls().open(self._odb, self._nql)
-        SessionsCollection().flush(self.ns)
+        if nql:
+            SessionsCollection().flush(self.ns)
+        return self
+    
+    def register (self, sio):
+        sio.register_namespace(self)
         return self
     
     async def on_connect(self, sid, environ):
         await self.save_session(sid, {
             'sid': sid,
             'address': environ['aiohttp.request'].transport.get_extra_info('peername')[0]
         })
         self._nql.connect(sid)
 
     async def on_disconnect(self, sid):
+        log.error(f"DISCONNECT={sid}")
         self._nql.disconnect(sid)
+        SessionsTable().from_sid(sid).delete()
+
+    async def on_get_version (self, sid, product, version):
+        log.debug(f"NS={self.ns} product={product} version={version}")
+        return await VersionsCollection(sid=sid, session=await self.get_session(sid), ns=self.ns).get_version(product, version)
 
     async def on_auth_hello(self, sid, auth):
         return await OrbitAuth(sid, self.ns).hello(auth, self.get_session, self.save_session)
 
     async def on_auth_validate(self, sid, auth):
+        log.info(f'Validate: {sid} / {self.NAMESPACE}')
         return await OrbitAuth(sid, self.ns).validate(auth, self.get_session, self.save_session)
 
     async def on_auth_confirm(self, sid, auth):
         return await OrbitAuth(sid, self.ns).confirm(auth, self.get_session, self.save_session)
 
     @navGuard
     async def on_call_nql(self, sid, params):
```

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_plugins.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_plugins.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,46 @@
 
     PLUGIN_FOLDER = 'orbit_plugins'
 
     def __init__ (self, cls):
         self._cls = cls
 
     def __iter__ (self):
-        for importer, package_name, _ in iter_modules([self.PLUGIN_FOLDER]):
+        tracker = set()
+        for importer, package_name, _ in iter_modules():
+            if package_name != 'orbit_component_base':
+                continue
             full_package_name = f'{self.PLUGIN_FOLDER}.{package_name}'
             if full_package_name not in modules:
                 plugin= importer.find_module(package_name).load_module(package_name)
                 globals()[package_name] = plugin
             else:
                 plugin = modules[full_package_name]
             if hasattr(plugin, self._cls):
-                yield plugin
+                if full_package_name not in tracker:
+                    tracker.add(full_package_name)
+                    yield plugin
 
+        for importer, package_name, _ in iter_modules([self.PLUGIN_FOLDER]):
+            full_package_name = f'{self.PLUGIN_FOLDER}.{package_name}'
+            if full_package_name not in modules:
+                plugin= importer.find_module(package_name).load_module(package_name)
+                globals()[package_name] = plugin
+            else:
+                plugin = modules[full_package_name]
+            if hasattr(plugin, self._cls):
+               if full_package_name not in tracker:
+                    tracker.add(full_package_name)
+                    yield plugin
+                
         for importer, package_name, _ in iter_modules():
             if package_name.startswith('orbit_component'):
                 full_package_name = f'{self.PLUGIN_FOLDER}.{package_name}'
                 if full_package_name not in modules:
                     plugin= importer.find_module(package_name).load_module(package_name)
                     globals()[package_name] = plugin
                 else:
                     plugin = modules[full_package_name]
                 if hasattr(plugin, self._cls):
-                    yield plugin
+                    if full_package_name not in tracker:
+                        tracker.add(full_package_name)
+                        yield plugin
```

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_router.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_router.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,24 @@
         self._context = context
         self._args = args
         self._namespaces = set([])
 
     async def redirect(self, request):
         try:
             if not world.conf.web or world.args.dev:
-                # log.debug(f'[Access via dev passthru: {request.rel_url}]')
-                async with ClientSession(connector=TCPConnector(), skip_auto_headers=['accept-encoding']) as session:
-                    origin = f"http://localhost:{world.conf.vite_port}"
+                async with ClientSession(connector=TCPConnector(verify_ssl=False), skip_auto_headers=['accept-encoding']) as session:
+                    origin = f"https://{world.conf.name}:{world.conf.vite_port}"
                     try:
                         async with session.get(f'{origin}{request.rel_url}') as resp:
                             headers = dict(resp.headers)
                             headers['Origin'] = origin
                             headers['Cache-Control'] = 'max-age=0, s-maxage=0'
                             return web.Response(body=await resp.content.read(), status=resp.status, headers=headers)
-                    except client_exceptions.ClientConnectorError:
+                    except client_exceptions.ClientConnectorError as e:
+                        log.exception(e)
                         log.error(f'VITE server is down on: {origin}')
                         return ''
             else:
                 path = (request.path if request.path != '/' else 'index.html').strip('/')
                 headers = {'Cache-Control': 'max-age=0, s-maxage=0'}
                 fullpath = world.conf.web / path
                 log.debug(f'Delivering from filesystem: {fullpath.as_posix()}')
```

### Comparing `orbit_component_base-0.99.9/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-1.0.9/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.9/pyproject.toml` & `orbit_component_base-1.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-base"
-version = "0.99.9"
+version = "1.0.9"
 description = "Orbit Framework - base component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "orbit_component_base"}]
 include = ['README.md', 'LICENSE.md']
 keywords = ['orbit-framework', 'orbit-component', 'orbit-database']
```

### Comparing `orbit_component_base-0.99.9/PKG-INFO` & `orbit_component_base-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-base
-Version: 0.99.9
+Version: 1.0.9
 Summary: Orbit Framework - base component
 Home-page: https://gitlab.com/madpenguin/orbit-component-base
 License: MIT
 Keywords: orbit-framework,orbit-component,orbit-database
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4.0
```

