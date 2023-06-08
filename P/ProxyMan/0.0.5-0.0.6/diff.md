# Comparing `tmp/ProxyMan-0.0.5.tar.gz` & `tmp/ProxyMan-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProxyMan-0.0.5.tar", last modified: Thu Jun  8 15:37:52 2023, max compression
+gzip compressed data, was "ProxyMan-0.0.6.tar", last modified: Thu Jun  8 19:16:49 2023, max compression
```

## Comparing `ProxyMan-0.0.5.tar` & `ProxyMan-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:37:52.153687 ProxyMan-0.0.5/
--rw-r--r--   0 rawandahmad   (501) staff       (20)     3294 2023-06-08 15:37:52.153541 ProxyMan-0.0.5/PKG-INFO
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:37:52.152524 ProxyMan-0.0.5/ProxyMan/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      126 2023-06-08 15:37:51.000000 ProxyMan-0.0.5/ProxyMan/__init__.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)     6274 2023-06-08 15:19:36.000000 ProxyMan-0.0.5/ProxyMan/proxyman.py
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:37:52.153334 ProxyMan-0.0.5/ProxyMan.egg-info/
--rw-r--r--   0 rawandahmad   (501) staff       (20)     3294 2023-06-08 15:37:52.000000 ProxyMan-0.0.5/ProxyMan.egg-info/PKG-INFO
--rw-r--r--   0 rawandahmad   (501) staff       (20)      219 2023-06-08 15:37:52.000000 ProxyMan-0.0.5/ProxyMan.egg-info/SOURCES.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-08 15:37:52.000000 ProxyMan-0.0.5/ProxyMan.egg-info/dependency_links.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        8 2023-06-08 15:37:52.000000 ProxyMan-0.0.5/ProxyMan.egg-info/requires.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-08 15:37:52.000000 ProxyMan-0.0.5/ProxyMan.egg-info/top_level.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)     2083 2023-06-08 15:26:15.000000 ProxyMan-0.0.5/README.md
--rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-08 15:37:52.153735 ProxyMan-0.0.5/setup.cfg
--rw-r--r--   0 rawandahmad   (501) staff       (20)      831 2023-06-08 15:37:51.000000 ProxyMan-0.0.5/setup.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 19:16:49.917455 ProxyMan-0.0.6/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     3576 2023-06-08 19:16:49.917331 ProxyMan-0.0.6/PKG-INFO
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 19:16:49.916478 ProxyMan-0.0.6/ProxyMan/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      126 2023-06-08 19:16:34.000000 ProxyMan-0.0.6/ProxyMan/__init__.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     7465 2023-06-08 19:15:17.000000 ProxyMan-0.0.6/ProxyMan/proxyman.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 19:16:49.917139 ProxyMan-0.0.6/ProxyMan.egg-info/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     3576 2023-06-08 19:16:49.000000 ProxyMan-0.0.6/ProxyMan.egg-info/PKG-INFO
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      219 2023-06-08 19:16:49.000000 ProxyMan-0.0.6/ProxyMan.egg-info/SOURCES.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-08 19:16:49.000000 ProxyMan-0.0.6/ProxyMan.egg-info/dependency_links.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        8 2023-06-08 19:16:49.000000 ProxyMan-0.0.6/ProxyMan.egg-info/requires.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-08 19:16:49.000000 ProxyMan-0.0.6/ProxyMan.egg-info/top_level.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     2317 2023-06-08 19:04:11.000000 ProxyMan-0.0.6/README.md
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-08 19:16:49.917497 ProxyMan-0.0.6/setup.cfg
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      889 2023-06-08 19:16:20.000000 ProxyMan-0.0.6/setup.py
```

### Comparing `ProxyMan-0.0.5/PKG-INFO` & `ProxyMan-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ProxyMan
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple proxy manager for Python with WebShare API support
 Home-page: https://github.com/rawandahmad698/ProxyMan
 Author: Rawand Ahmed Shaswar
 Author-email: rawa@rawa.dev
 License: BSD 3-Clause License
 Description: # ProxyMan 🌐
         
         A simple Proxy manager for Python
         
+        Created with ❤️ by [**@MeshMonitors**](https://twitter.com/meshmonitors_)
+        
         ## Features
         
         ✨ Proxy Management:
         - Load proxies from a file
         - Support for IP-based and username-password authentication
         
         🔄 Proxy Refresh:
@@ -32,18 +34,22 @@
         ```
         
         ## Usage
         
         
         ### Loading proxies from a file
         ```python
-        from ProxyMan import ProxyMan
+        from ProxyMan import ProxyMan, AuthType
+        import os
         
         # Load proxies from a file
-        pm = ProxyMan(file_path="proxies.txt")
+        current_dir = os.path.dirname(os.path.realpath(__file__))
+        current_dir = os.path.dirname(current_dir)
+        
+        pm = ProxyMan(file_path=current_dir + "/proxies.txt", auth=AuthType.IP)
         ```
         
         ### Configuring ProxyMan
         ```python
         from ProxyMan import ProxyMan, Filter, AuthType
         
         # Create a ProxyMan instance
```

### Comparing `ProxyMan-0.0.5/ProxyMan/proxyman.py` & `ProxyMan-0.0.6/ProxyMan/proxyman.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 
 class AuthType(enum.Enum):
     IP = "ip"
     USERNAME_PASSWORD = "username:password"
 
 
 class ProxyMan:
-    def __init__(self, api_key: str = None, proxies_to_scrape: int = 3000, auth=AuthType.IP, file_path="../proxies.txt", fail_count=3, scrape_filter=Filter.ALL):
+    def __init__(self, api_key: str = None, proxies_to_scrape: int = 3000, auth=AuthType.IP, file_path="../proxies.txt", fail_count=3, scrape_filter=Filter.ALL, private_endpoint = None):
         self.api_key = api_key
         self.proxies_to_scrape = proxies_to_scrape
         self.parsed_proxies = []
         self.bad_proxies = []
         self.file_path = file_path
         self.proxies_to_ping = set()
         self.auth = auth
         self.fail_count = fail_count
         self.scrape_filter = scrape_filter
+        self.private_endpoint = private_endpoint
 
         self.__setup()
 
     def __setup(self):
         # Prepare proxies
         try:
             with open(self.file_path, "r") as proxy_file:
@@ -132,24 +133,55 @@
                             ports = result['ports']['http']
                             proxies.append(f"{proxy_ip}:{ports}")
                 else:
                     print(f"Error on page {page}: Response={resp.status}")
 
         return proxies
 
-    async def update_proxies(self):
+    async def _private_proxies(self):
+        """
+        Private, internal function
+        """
+        endpoint = self.private_endpoint
+        if self.scrape_filter == Filter.US:
+            endpoint += "?country=us"
+        elif self.scrape_filter == Filter.UK:
+            endpoint += "?country_code=uk"
+        elif self.scrape_filter == Filter.FR:
+            endpoint += "?country_code=fr"
+        all_proxies = []
+        async with aiohttp.ClientSession() as session:
+            async with session.get(endpoint) as resp:
+                if resp.status == 200 and 'json' in resp.headers['Content-Type']:
+                    data = await resp.json()
+                    if 'proxies' in data:
+                        results = data['proxies']
+                        all_proxies = results
+                else:
+                    print(f"Error on page {endpoint}: Response={resp.status}")
+
+        return all_proxies
+
+
+    async def update_proxies(self, private_proxies: bool = False):
         time_now = time.time()
-        request_count = math.ceil(self.proxies_to_scrape / 250) # 250 proxies per page
-        tasks = []
-        print(f">> [PROXYMAN] Refreshing proxies... (This may take a while)")
-        for i in range(1, int(request_count)):
-            tasks.append(asyncio.create_task(self._get_proxies(i)))
+        if not private_proxies:
+            request_count = math.ceil(self.proxies_to_scrape / 250) # 250 proxies per page
+            tasks = []
+            print(f">> [PROXYMAN] Refreshing proxies... (This may take a while)")
+            for i in range(1, int(request_count)):
+                tasks.append(asyncio.create_task(self._get_proxies(i)))
+
+            all_proxies = await asyncio.gather(*tasks)
+            proxies = [item for sublist in all_proxies for item in sublist]
+        else:
+            if self.private_endpoint is None:
+                raise Exception("Private endpoint is not set. Please set it before calling this method.")
 
-        all_proxies = await asyncio.gather(*tasks)
-        proxies = [item for sublist in all_proxies for item in sublist]
+            proxies = await self._private_proxies()
 
         proxies = list(set(proxies))
 
         if len(proxies) == 0:
             print(">> [PROXYMAN] No proxies found. Please try again later")
             return
 
@@ -178,14 +210,13 @@
             "http": rn,
             "https": rn
         }
         return proxy
 
 
 async def test_update():
-    pm = ProxyMan(auth=AuthType.IP, file_path="proxies.txt", fail_count=3, scrape_filter=Filter.US)
-    await pm.update_proxies()
+    pass
 
 
 if __name__ == "__main__":
     # Testing
     asyncio.run(test_update())
```

### Comparing `ProxyMan-0.0.5/ProxyMan.egg-info/PKG-INFO` & `ProxyMan-0.0.6/ProxyMan.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ProxyMan
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple proxy manager for Python with WebShare API support
 Home-page: https://github.com/rawandahmad698/ProxyMan
 Author: Rawand Ahmed Shaswar
 Author-email: rawa@rawa.dev
 License: BSD 3-Clause License
 Description: # ProxyMan 🌐
         
         A simple Proxy manager for Python
         
+        Created with ❤️ by [**@MeshMonitors**](https://twitter.com/meshmonitors_)
+        
         ## Features
         
         ✨ Proxy Management:
         - Load proxies from a file
         - Support for IP-based and username-password authentication
         
         🔄 Proxy Refresh:
@@ -32,18 +34,22 @@
         ```
         
         ## Usage
         
         
         ### Loading proxies from a file
         ```python
-        from ProxyMan import ProxyMan
+        from ProxyMan import ProxyMan, AuthType
+        import os
         
         # Load proxies from a file
-        pm = ProxyMan(file_path="proxies.txt")
+        current_dir = os.path.dirname(os.path.realpath(__file__))
+        current_dir = os.path.dirname(current_dir)
+        
+        pm = ProxyMan(file_path=current_dir + "/proxies.txt", auth=AuthType.IP)
         ```
         
         ### Configuring ProxyMan
         ```python
         from ProxyMan import ProxyMan, Filter, AuthType
         
         # Create a ProxyMan instance
```

### Comparing `ProxyMan-0.0.5/README.md` & `ProxyMan-0.0.6/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # ProxyMan 🌐
 
 A simple Proxy manager for Python
 
+Created with ❤️ by [**@MeshMonitors**](https://twitter.com/meshmonitors_)
+
 ## Features
 
 ✨ Proxy Management:
 - Load proxies from a file
 - Support for IP-based and username-password authentication
 
 🔄 Proxy Refresh:
@@ -24,18 +26,22 @@
 ```
 
 ## Usage
 
 
 ### Loading proxies from a file
 ```python
-from ProxyMan import ProxyMan
+from ProxyMan import ProxyMan, AuthType
+import os
 
 # Load proxies from a file
-pm = ProxyMan(file_path="proxies.txt")
+current_dir = os.path.dirname(os.path.realpath(__file__))
+current_dir = os.path.dirname(current_dir)
+
+pm = ProxyMan(file_path=current_dir + "/proxies.txt", auth=AuthType.IP)
 ```
 
 ### Configuring ProxyMan
 ```python
 from ProxyMan import ProxyMan, Filter, AuthType
 
 # Create a ProxyMan instance
```

### Comparing `ProxyMan-0.0.5/setup.py` & `ProxyMan-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 
 from setuptools import setup
 
+import ProxyMan
+
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
-
+# Get version from init file
 setup(
     name='ProxyMan',
-    version='0.0.5',
+    version=ProxyMan.__version__,
     description='A simple proxy manager for Python with WebShare API support',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/rawandahmad698/ProxyMan',
     author='Rawand Ahmed Shaswar',
     author_email='rawa@rawa.dev',
     license='BSD 3-Clause License',
```

