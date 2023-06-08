# Comparing `tmp/bigboat-0.2.9.tar.gz` & `tmp/bigboat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bigboat-0.2.9.tar", last modified: Fri Oct 27 09:09:26 2017, max compression
+gzip compressed data, was "bigboat-0.3.0.tar", last modified: Thu Jun  8 11:21:33 2023, max compression
```

## Comparing `bigboat-0.2.9.tar` & `bigboat-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 leonhelwerda   (501) staff       (20)        0 2017-10-27 09:09:26.000000 bigboat-0.2.9/
-drwxr-xr-x   0 leonhelwerda   (501) staff       (20)        0 2017-10-27 09:09:26.000000 bigboat-0.2.9/bigboat/
--rw-r--r--   0 leonhelwerda   (501) staff       (20)      655 2017-10-27 09:05:51.000000 bigboat-0.2.9/bigboat/__init__.py
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     2116 2017-06-02 20:29:32.000000 bigboat-0.2.9/bigboat/application.py
--rw-r--r--   0 leonhelwerda   (501) staff       (20)    13349 2017-10-27 09:03:03.000000 bigboat-0.2.9/bigboat/client.py
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     1605 2017-06-06 11:38:32.000000 bigboat-0.2.9/bigboat/entity.py
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     2473 2017-07-22 12:45:02.000000 bigboat-0.2.9/bigboat/instance.py
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     5169 2017-07-22 14:46:17.000000 bigboat-0.2.9/bigboat/utils.py
-drwxr-xr-x   0 leonhelwerda   (501) staff       (20)        0 2017-10-27 09:09:26.000000 bigboat-0.2.9/bigboat.egg-info/
--rw-r--r--   0 leonhelwerda   (501) staff       (20)        1 2017-10-27 09:09:25.000000 bigboat-0.2.9/bigboat.egg-info/dependency_links.txt
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     1137 2017-10-27 09:09:25.000000 bigboat-0.2.9/bigboat.egg-info/PKG-INFO
--rw-r--r--   0 leonhelwerda   (501) staff       (20)       45 2017-10-27 09:09:25.000000 bigboat-0.2.9/bigboat.egg-info/requires.txt
--rw-r--r--   0 leonhelwerda   (501) staff       (20)      288 2017-10-27 09:09:25.000000 bigboat-0.2.9/bigboat.egg-info/SOURCES.txt
--rw-r--r--   0 leonhelwerda   (501) staff       (20)        8 2017-10-27 09:09:25.000000 bigboat-0.2.9/bigboat.egg-info/top_level.txt
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     1137 2017-10-27 09:09:26.000000 bigboat-0.2.9/PKG-INFO
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     3124 2017-07-22 15:56:00.000000 bigboat-0.2.9/README.md
--rw-r--r--   0 leonhelwerda   (501) staff       (20)       38 2017-10-27 09:09:26.000000 bigboat-0.2.9/setup.cfg
--rw-r--r--   0 leonhelwerda   (501) staff       (20)     2272 2017-07-22 14:55:34.000000 bigboat-0.2.9/setup.py
+drwxr-xr-x   0 leonhelwerda   (501) staff       (20)        0 2023-06-08 11:21:33.180923 bigboat-0.3.0/
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)    11357 2023-06-08 11:08:33.000000 bigboat-0.3.0/LICENSE
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)       25 2022-12-06 13:57:08.000000 bigboat-0.3.0/MANIFEST.in
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     1124 2023-06-08 11:21:33.181199 bigboat-0.3.0/PKG-INFO
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     3941 2023-06-08 11:00:20.000000 bigboat-0.3.0/README.md
+drwxr-xr-x   0 leonhelwerda   (501) staff       (20)        0 2023-06-08 11:21:33.166482 bigboat-0.3.0/bigboat/
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)      732 2023-06-08 11:08:33.000000 bigboat-0.3.0/bigboat/__init__.py
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     2524 2023-06-08 11:08:33.000000 bigboat-0.3.0/bigboat/application.py
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)    14615 2023-06-08 11:08:33.000000 bigboat-0.3.0/bigboat/client.py
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     1947 2023-06-08 11:08:33.000000 bigboat-0.3.0/bigboat/entity.py
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     3013 2023-06-08 11:08:33.000000 bigboat-0.3.0/bigboat/instance.py
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)        0 2022-12-06 13:57:08.000000 bigboat-0.3.0/bigboat/py.typed
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     2414 2023-06-08 11:08:33.000000 bigboat-0.3.0/bigboat/utils.py
+drwxr-xr-x   0 leonhelwerda   (501) staff       (20)        0 2023-06-08 11:21:33.180324 bigboat-0.3.0/bigboat.egg-info/
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     1124 2023-06-08 11:21:33.000000 bigboat-0.3.0/bigboat.egg-info/PKG-INFO
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)      352 2023-06-08 11:21:33.000000 bigboat-0.3.0/bigboat.egg-info/SOURCES.txt
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)        1 2023-06-08 11:21:33.000000 bigboat-0.3.0/bigboat.egg-info/dependency_links.txt
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)       30 2023-06-08 11:21:33.000000 bigboat-0.3.0/bigboat.egg-info/requires.txt
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)        8 2023-06-08 11:21:33.000000 bigboat-0.3.0/bigboat.egg-info/top_level.txt
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)       30 2022-12-06 13:57:08.000000 bigboat-0.3.0/requirements.txt
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)       67 2023-06-08 11:21:33.183084 bigboat-0.3.0/setup.cfg
+-rw-r--r--   0 leonhelwerda   (501) staff       (20)     2418 2023-06-08 11:15:27.000000 bigboat-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bigboat-0.2.9/bigboat/application.py` & `bigboat-0.3.0/bigboat/instance.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,84 @@
 """
-Application entity from the API.
+Instance entity from the API.
 
-Copyright 2017 ICTU
+Copyright 2017-2020 ICTU
+Copyright 2017-2022 Leiden University
+Copyright 2017-2023 Leon Helwerda
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from typing import Any, Dict, List, Optional, Tuple, Union, TYPE_CHECKING
 from .entity import Entity
 from .utils import readonly
-
-@readonly("name", "version")
-class Application(Entity):
+if TYPE_CHECKING: # pragma: no cover
+    # pylint: disable=cyclic-import
+    from .application import Application
+    from .client import Client
+else:
+    Application = object
+    Client = object
+
+@readonly("name", "current_state", "desired_state", "application", "services",
+          "parameters", "options")
+class Instance(Entity):
     """
-    An application definition entity.
+    A deployed (parameterized) application instance entity.
     """
 
-    def __init__(self, client, name, version):
-        super(Application, self).__init__(client)
-
+    def __init__(self, client: Client, name: str,
+                 current_state: Optional[str] = None,
+                 **kwargs: Optional[Union[str, Application, Dict[str, Any]]]):
+        super().__init__(client)
         self._name = name
-        self._version = version
+        self._current_state = current_state
+        self._desired_state = kwargs.get('desired_state')
+        self._application = kwargs.get('application')
+        self._services = kwargs.get('services')
 
-    def update(self):
-        """
-        Register the application definition in the BigBoat API.
-        """
+        self._parameters = kwargs.get('parameters')
+        self._options = kwargs.get('options')
 
-        return self.client.update_app(self.name, self.version)
-
-    def delete(self):
+    def update(self) -> Optional['Instance']:
         """
-        Delete the application definition in the BigBoat API.
+        Request the instance to be created with a desired state of 'running'.
         """
 
-        return self.client.delete_app(self.name, self.version)
+        if self.application is None:
+            raise ValueError('Application information required to start instance')
 
-    def start(self, name=None, **kwargs):
-        """
-        Request an instance to be created with a desired state of 'running'
-        for this application.
+        return self.client.update_instance(self.name, self.application.name,
+                                           self.application.version,
+                                           parameters=self.parameters,
+                                           options=self.options)
 
-        Args:
-            name (:obj:`str` or `None`): The name of the instance to be
-                started, or `None` to use the application name.
-            **kwargs: Additional properties to use when starting the instance.
-
-        Returns:
-            :obj:`bigboat.instance.Instance` or `None`: The instance
-            if it was started or `None` if the instance failed to start.
+    def delete(self) -> bool:
+        """
+        Request the instance to be stopped.
         """
 
-        if name is None:
-            name = self.name
+        return self.client.delete_instance(self.name) is not None
 
-        return self.client.update_instance(name, self.name, self.version,
-                                           **kwargs)
+    def __repr__(self) -> str:
+        parts: List[Tuple[str, Union[str, Application, Dict[str, Any]]]] = [
+            ('name', self.name),
+            ('current_state', self.current_state),
+            ('desired_state', self.desired_state),
+            ('application', self.application),
+            ('services', self.services),
+            ('parameters', self.parameters),
+            ('options', self.options)
+        ]
+        properties = [f'{key}={value!r}' for (key, value) in parts]
 
-    def __repr__(self):
-        return 'Application(name={!r}, version={!r})'.format(self.name, self.version)
+        return f'Instance({", ".join(properties)})'
```

### Comparing `bigboat-0.2.9/bigboat/client.py` & `bigboat-0.3.0/bigboat/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 """
 Clients that connect to the BigBoat API.
 
-Copyright 2017 ICTU
+Copyright 2017-2020 ICTU
+Copyright 2017-2022 Leiden University
+Copyright 2017-2023 Leon Helwerda
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from builtins import str
-from builtins import object
+from typing import Any, Dict, List, Optional, Union
 import requests
+from requests.models import Response
 import yaml
 from .application import Application
 from .instance import Instance
-from .utils import Inherited as inherit
 
-class Client(object):
+class Client:
     """
     Generic client base class, enforcing minimum required interface.
     """
 
-    def __init__(self, base_url, **kwargs):
+    def __init__(self, base_url: str):
         self._base_url = base_url.rstrip('/')
-        self._options = kwargs
 
     @property
-    def base_url(self):
+    def base_url(self) -> str:
         """
         The base URL of the BigBoat instance.
         """
 
         return self._base_url
 
-    def apps(self):
+    def apps(self) -> List[Application]:
         """
         Retrieve all application definitions from the API.
 
         Returns:
             :obj:`list` of :obj:`application.Application`
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def get_app(self, name, version):
+    def get_app(self, name: str, version: str) -> Optional[Application]:
         """
         Retrieve a specific application definition from the API.
 
         Args:
             name (str): The name of the application
             version (str): The version of the application
 
@@ -63,68 +63,69 @@
             :obj:`bigboat.application.Application` or `None`: The application
             definition if it was found or `None` if the definition does not
             exist.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def update_app(self, name, version):
+    def update_app(self, name: str, version: str) -> Optional[Application]:
         """
         Register an application definition in the API.
 
         Args:
             name (str): The name of the application
             version (str): The version of the application
 
         Returns:
             :obj:`bigboat.application.Application` or `None`: The application
             definition if it was successfully created.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def delete_app(self, name, version):
+    def delete_app(self, name: str, version: str) -> bool:
         """
         Delete an application definition in the API.
 
         Args:
             name (str): The name of the application
             version (str): The version of the application
 
         Returns:
             bool: Whether the application was successfully deleted.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def instances(self):
+    def instances(self) -> List[Instance]:
         """
         Retrieve all live instances from the API.
 
         Returns:
             :obj:`list` of :obj:`bigboat.instance.Instance`
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def get_instance(self, name):
+    def get_instance(self, name: str) -> Optional[Instance]:
         """
         Retrieve a specific live instance from the API.
 
         Args:
             name (str): The name of the instance.
 
         Returns:
             :obj:`bigboat.instance.Instance` or `None`: The instance
             if it was found or `None` if the instance does not exist.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def update_instance(self, name, app_name, version, **kwargs):
+    def update_instance(self, name: str, app_name: str, version: str,
+                        **kwargs: Dict[str, str]) -> Optional[Instance]:
         """
         Request the instance to be created with a desired state of 'running'.
 
         Args:
             name (str): The name of the instance to be started.
             app_name (str): The name of the application to be started.
             version (str): The version of the application to be started.
@@ -133,305 +134,306 @@
         Returns:
             :obj:`bigboat.instance.Instance` or `None`: The instance
             if it was started or `None` if the instance failed to start.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def delete_instance(self, name):
+    def delete_instance(self, name: str) -> Optional[Instance]:
         """
-        Retrieve a specific live instance from the API.
+        Delete a specific live instance from the API.
 
         Args:
             name (str): The name of the instance.
 
         Returns:
             :obj:`bigboat.instance.Instance` or `None`: The instance
-            if it was found or `None` if the instance does not exist.
+            if it was found or `None` if the instance did not exist.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
 class Client_v1(Client):
     """
     Client for the deprecated BigBoat v1 API.
     """
 
-    def _format_url(self, path):
-        return '{}/api/v1/{}'.format(self._base_url, path)
+    TIMEOUT = 60
+
+    def _format_url(self, path: str) -> str:
+        return f'{self._base_url}/api/v1/{path}'
 
-    def _get(self, path):
-        return requests.get(self._format_url(path))
+    def _get(self, path: str) -> Response:
+        return requests.get(self._format_url(path), timeout=self.TIMEOUT)
 
-    def _delete(self, path):
-        return requests.delete(self._format_url(path))
+    def _delete(self, path: str) -> Response:
+        return requests.delete(self._format_url(path), timeout=self.TIMEOUT)
 
-    @inherit
-    def apps(self):
+    def apps(self) -> List[Application]:
         return []
 
-    @inherit
-    def get_app(self, name, version):
+    def get_app(self, name: str, version: str) -> Optional[Application]:
         try:
-            request = self._get('appdef/{}/{}'.format(name, version))
+            request = self._get(f'appdef/{name}/{version}')
         except requests.exceptions.ConnectionError:
             return None
 
-        document = yaml.load(request.text)
+        document = yaml.safe_load(request.text)
 
         return Application(self, document['name'], str(document['version']))
 
-    @inherit
-    def update_app(self, name, version):
+    def update_app(self, name: str, version: str) -> Optional[Application]:
         # Cannot create new apps through v1 API
         return None
 
-    @inherit
-    def delete_app(self, name, version):
-        request = self._delete('appdef/{}/{}'.format(name, version))
+    def delete_app(self, name: str, version: str) -> bool:
+        request = self._delete(f'appdef/{name}/{version}')
 
         if request.status_code == 404:
             return False
 
         return request.status_code == 200
 
-    @inherit
-    def instances(self):
+    def instances(self) -> List[Instance]:
         request = self._get('instances')
 
         if request.status_code == 404:
             return []
 
         data = request.json()
         return [Instance(self, name) for name in data['instances']]
 
-    @inherit
-    def get_instance(self, name):
-        request = self._get('state/{}'.format(name))
+    def get_instance(self, name: str) -> Optional[Instance]:
+        request = self._get(f'state/{name}')
 
         if request.status_code == 404:
             return None
 
         state = 'running' if request.text == 'active' else request.text
 
         return Instance(self, name, state)
 
-    @inherit
-    def update_instance(self, name, app_name, version, **kwargs):
-        request = self._get('start-app/{}/{}/{}'.format(app_name, version, name))
+    def update_instance(self, name: str, app_name: str, version: str,
+                        **kwargs: Dict[str, str]) -> Optional[Instance]:
+        request = self._get(f'start-app/{app_name}/{version}/{name}')
 
         if request.status_code == 404:
             return None
 
         return Instance(self, name, current_state='running',
                         application=Application(self, app_name, version))
 
-    @inherit
-    def delete_instance(self, name):
-        request = self._get('stop-app/{}'.format(name))
+    def delete_instance(self, name: str) -> Optional[Instance]:
+        request = self._get(f'stop-app/{name}')
 
         if request.status_code == 404:
             return None
 
         return Instance(self, name, 'created')
 
 class Client_v2(Client):
     """
     Client for the BigBoat v2 API.
     """
 
-    def __init__(self, base_url, api_key):
-        super(Client_v2, self).__init__(base_url)
+    TIMEOUT = 60
+
+    def __init__(self, base_url: str, api_key: str):
+        super().__init__(base_url)
         self._api_key = api_key
         self._session = requests.Session()
         self._session.headers.update({'api-key': self._api_key})
 
-    def _format_url(self, path):
-        return '{}/api/v2/{}'.format(self._base_url, path)
+    def _format_url(self, path: str) -> str:
+        return f'{self._base_url}/api/v2/{path}'
 
-    def _get(self, path):
-        return self._session.get(self._format_url(path))
+    def _get(self, path: str) -> Response:
+        return self._session.get(self._format_url(path), timeout=self.TIMEOUT)
 
-    def _put(self, path, content_type=None, data=None, json=None):
-        headers = {}
+    def _put(self, path: str, content_type: Optional[str] = None,
+             data: Optional[Union[str, bytes]] = None,
+             json: Optional[Any] = None) -> Response:
+        headers: Dict[str, str] = {}
         if content_type is not None:
             headers['Content-Type'] = content_type
         elif json is not None:
             headers['Content-Type'] = 'application/json'
 
         return self._session.put(self._format_url(path), headers=headers,
-                                 data=data, json=json)
+                                 data=data, json=json, timeout=self.TIMEOUT)
 
-    def _delete(self, path):
-        return self._session.delete(self._format_url(path))
+    def _delete(self, path: str) -> Response:
+        return self._session.delete(self._format_url(path),
+                                    timeout=self.TIMEOUT)
 
     @staticmethod
-    def _check_bad_request(request):
+    def _check_bad_request(request: Response) -> None:
         # Bad Request should raise an exception
         if request.status_code == 400:
             if request.headers['Content-Type'] == 'application/json':
                 response = request.json()
                 raise ValueError(response['message'])
-            else:
-                raise ValueError(request.text)
+
+            raise ValueError(request.text)
 
         # Unauthorized should raise an exception
         if request.status_code == 401:
             response = request.json()
             raise ValueError(response['message'])
 
-    def _format_app(self, app):
+    def _format_app(self, app: Dict[str, str]) -> Application:
         return Application(self, app['name'], app['version'])
 
-    @inherit
-    def apps(self):
+    def apps(self) -> List[Application]:
         request = self._get('apps')
         self._check_bad_request(request)
         return [self._format_app(app) for app in request.json()]
 
-    @inherit
-    def get_app(self, name, version):
-        request = self._get('apps/{}/{}'.format(name, version))
+    def get_app(self, name: str, version: str) -> Optional[Application]:
+        request = self._get(f'apps/{name}/{version}')
         self._check_bad_request(request)
         if request.status_code == 404:
             return None
 
         return self._format_app(request.json())
 
-    @inherit
-    def update_app(self, name, version):
+    def update_app(self, name: str, version: str) -> Optional[Application]:
         try:
-            request = self._put('apps/{}/{}'.format(name, version))
+            request = self._put(f'apps/{name}/{version}')
         except requests.exceptions.ConnectionError:
             return None
 
         self._check_bad_request(request)
         return self._format_app(request.json())
 
-    @inherit
-    def delete_app(self, name, version):
-        request = self._delete('apps/{}/{}'.format(name, version))
+    def delete_app(self, name: str, version: str) -> bool:
+        request = self._delete(f'apps/{name}/{version}')
         self._check_bad_request(request)
         if request.status_code == 404:
             return False
 
         return True
 
-    def get_compose(self, name, version, file_name):
+    def get_compose(self, name: str, version: str, file_name: str) -> \
+            Optional[str]:
         """
         Retrieve a docker compose or bigboat compose file for the application.
 
         Args:
             name (str): The name of the application
             version (str): The version of the application
             file_name (str): 'dockerCompose' or 'bigboatCompose'
 
         Returns:
             :obj:`str` or `None`: The application definition's docker compose
             file contents if the application was found, or `None` if the
             definition does not exist.
         """
 
-        path = 'apps/{}/{}/files/{}'.format(name, version, file_name)
+        path = f'apps/{name}/{version}/files/{file_name}'
         request = self._get(path)
         self._check_bad_request(request)
         if request.status_code == 404:
             return None
 
         content_type = request.headers.get('content-type')
         if content_type not in ('text/plain', 'text/yaml'):
             return None
 
         return request.text
 
-    def update_compose(self, name, version, file_name, content):
+    def update_compose(self, name: str, version: str, file_name: str,
+                       content: Union[str, bytes]) -> bool:
         """
         Update a docker compose or bigboat compose file for the application.
 
         Args:
             name (str): The name of the application
             version (str): The version of the application
             file_name (str): 'dockerCompose' or 'bigboatCompose'
-            content (str): The file contents
+            content (str or bytes): The file contents
 
         Returns:
             bool: Whether the compose file was successfully updated.
 
         Raises:
             ValueError: When the compose file could not be parsed as a valid
             YAML file.
             ValueError: When the bigboatCompose file contains name or version
             properties that do not match the provided application name/verison.
         """
 
-        path = 'apps/{}/{}/files/{}'.format(name, version, file_name)
+        path = f'apps/{name}/{version}/files/{file_name}'
         request = self._put(path, content_type='text/plain', data=content)
         self._check_bad_request(request)
         if request.status_code == 404:
             return False
 
         if request.status_code != 201:
             return False
 
         return True
 
-    def _format_instance(self, instance):
-        if 'app' in instance and instance['app']:
+    def _format_instance(self,
+                         instance: Dict[str, Union[str, Dict[str, Any]]]) -> \
+            Instance:
+        if 'app' in instance and isinstance(instance['app'], dict):
             application = self._format_app(instance['app'])
         else:
             application = None
 
         services = instance.get('services')
+        if not isinstance(services, dict):
+            services = None
 
-        state = instance.get('state', {})
+        state = instance.get('state')
+        if not isinstance(state, dict):
+            state = {}
 
-        return Instance(self, instance.get('name'),
+        return Instance(self, str(instance.get('name')),
                         current_state=state.get('current', 'running'),
                         desired_state=state.get('desired'),
                         application=application, services=services)
 
-    @inherit
-    def instances(self):
+    def instances(self) -> List[Instance]:
         request = self._get('instances')
         self._check_bad_request(request)
         return [self._format_instance(instance) for instance in request.json()]
 
-    @inherit
-    def get_instance(self, name):
-        request = self._get('instances/{}'.format(name))
+    def get_instance(self, name: str) -> Optional[Instance]:
+        request = self._get(f'instances/{name}')
         self._check_bad_request(request)
 
         if request.status_code == 404:
             return None
 
         return self._format_instance(request.json())
 
-    @inherit
-    def update_instance(self, name, app_name, version, **kwargs):
+    def update_instance(self, name: str, app_name: str, version: str,
+                        **kwargs: Dict[str, str]) -> Optional[Instance]:
         data = {
             'app': app_name,
             'version': version,
             'parameters': kwargs.get('parameters') or {},
             'options': kwargs.get('options') or {}
         }
-        request = self._put('instances/{}'.format(name), json=data)
+        request = self._put(f'instances/{name}', json=data)
 
         self._check_bad_request(request)
 
         return self._format_instance(request.json())
 
-    @inherit
-    def delete_instance(self, name):
-        request = self._delete('instances/{}'.format(name))
+    def delete_instance(self, name: str) -> Optional[Instance]:
+        request = self._delete(f'instances/{name}')
 
         self._check_bad_request(request)
 
         return self._format_instance(request.json())
 
-    def statuses(self):
+    def statuses(self) -> List[Dict[str, Any]]:
         """
         Retrieve all status items reported by BigBoat.
 
         Returns:
             :obj:`list` of :obj:`dict`: The status items
         """
```

### Comparing `bigboat-0.2.9/bigboat/entity.py` & `bigboat-0.3.0/bigboat/entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 """
 Generic base enntity.
 
-Copyright 2017 ICTU
+Copyright 2017-2020 ICTU
+Copyright 2017-2022 Leiden University
+Copyright 2017-2023 Leon Helwerda
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from builtins import object
+from typing import Any, Generic, Optional, TypeVar, TYPE_CHECKING
 from .utils import readonly
+if TYPE_CHECKING: # pragma: no cover
+    from .client import Client
+else:
+    Client = object
+
+EntityT_co = TypeVar('EntityT_co', bound='Entity', covariant=True)
 
 @readonly("client")
-class Entity(object):
+class Entity(Generic[EntityT_co]):
     """
     An entity from the BigBoat API.
     """
 
-    def __init__(self, client):
+    def __init__(self, client: Client):
         self._client = client
 
-    def update(self):
+    def update(self) -> Optional[EntityT_co]:
         """
         Send the data of the entity as an update for its properties to the
         BigBoat API. The entity calls the relevant update method of the client.
 
         Returns:
             :obj:`bigboat.entity.Entity` or `None`: The updated entity object
             from the API response if it was successfully updated.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def delete(self):
+    def delete(self) -> bool:
         """
         Delete the entity from the BigBoat API. The entity calls the relevant
         update method of the client.
 
         Returns:
             bool: Whether the entity was successfully deleted.
         """
 
         raise NotImplementedError('Must be implemented by subclasses')
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         raise AttributeError
```

### Comparing `bigboat-0.2.9/bigboat.egg-info/PKG-INFO` & `bigboat-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bigboat
-Version: 0.2.9
+Version: 0.3.0
 Summary: BigBoat docker dashboard API
-Home-page: https://github.com/ICTU/bigboat-python-api
-Author: ICTU
-Author-email: leon.helwerda@ictu.nl
+Home-page: https://github.com/grip-on-software/bigboat-python-api
+Author: Leon Helwerda
+Author-email: l.s.helwerda@liacs.leidenuniv.nl
 License: Apache License, Version 2.0
-Description-Content-Type: UNKNOWN
-Description: Python wrapper library for the BigBoat API.
-        Support for v2 and the deprecated v1 is included.
-        This API can create, retrieve, update and delete application definitions,
-        do similar operations for instances and poll for status
-Keywords: docker,dashboard,bigboat,api
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Keywords: docker dashboard bigboat api
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3
+License-File: LICENSE
+
+Python wrapper library for the BigBoat API.
+Support for v2 and the deprecated v1 is included.
+This API can create, retrieve, update and delete application definitions,
+do similar operations for instances and poll for status
```

### Comparing `bigboat-0.2.9/PKG-INFO` & `bigboat-0.3.0/bigboat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bigboat
-Version: 0.2.9
+Version: 0.3.0
 Summary: BigBoat docker dashboard API
-Home-page: https://github.com/ICTU/bigboat-python-api
-Author: ICTU
-Author-email: leon.helwerda@ictu.nl
+Home-page: https://github.com/grip-on-software/bigboat-python-api
+Author: Leon Helwerda
+Author-email: l.s.helwerda@liacs.leidenuniv.nl
 License: Apache License, Version 2.0
-Description-Content-Type: UNKNOWN
-Description: Python wrapper library for the BigBoat API.
-        Support for v2 and the deprecated v1 is included.
-        This API can create, retrieve, update and delete application definitions,
-        do similar operations for instances and poll for status
-Keywords: docker,dashboard,bigboat,api
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Keywords: docker dashboard bigboat api
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3
+License-File: LICENSE
+
+Python wrapper library for the BigBoat API.
+Support for v2 and the deprecated v1 is included.
+This API can create, retrieve, update and delete application definitions,
+do similar operations for instances and poll for status
```

### Comparing `bigboat-0.2.9/README.md` & `bigboat-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # BigBoat docker dashboard Python API
 
 [![PyPI](https://img.shields.io/pypi/v/bigboat.svg)](https://pypi.python.org/pypi/bigboat)
 [![Build 
-Status](https://travis-ci.org/ICTU/bigboat-python-api.svg?branch=master)](https://travis-ci.org/ICTU/bigboat-python-api)
+status](https://github.com/grip-on-software/bigboat-python-api/actions/workflows/bigboat-python-api.yml/badge.svg)](https://github.com/grip-on-software/bigboat-python-api/actions/workflows/bigboat-python-api.yml)
 [![Coverage 
-Status](https://coveralls.io/repos/github/ICTU/bigboat-python-api/badge.svg?branch=master)](https://coveralls.io/github/ICTU/bigboat-python-api?branch=master)
+Status](https://coveralls.io/repos/github/grip-on-software/bigboat-python-api/badge.svg?branch=master)](https://coveralls.io/github/grip-on-software/bigboat-python-api?branch=master)
+[![Quality Gate 
+Status](https://sonarcloud.io/api/project_badges/measure?project=grip-on-software_bigboat-python-api&metric=alert_status)](https://sonarcloud.io/project/overview?id=grip-on-software_bigboat-python-api)
 
 Python wrapper library for the BigBoat API. This API can create, retrieve, 
 update and delete application definitions, do similar operations for instances 
 and poll for status.
 
 Support for v2 and the deprecated v1 APIs (limited to certain operations) is 
-included.
+included. Note that BigBoat development itself has halted.
 
 ## Requirements
 
-The BigBoat Python API has been tested to work on Python 2.7 and 3.6. The API 
-has few dependencies; see `requirements.txt` for the list of installation 
-requirements. The short list is also repeated here:
+The BigBoat Python API has been tested to work on Python 3.8+. The API has few 
+dependencies; see `requirements.txt` for the list of installation requirements. 
+The short list is also repeated here:
 
-- [Future](http://python-future.org/overview.html)
 - [Requests](http://docs.python-requests.org/en/master/user/install/)
 - [PyYAML](http://pyyaml.org/wiki/PyYAMLDocumentation)
 
 ## Installation
 
 Install the latest version from PyPI using:
 
@@ -48,37 +49,44 @@
 api = bigboat.Client_v2('http://BIG_BOAT', 'MY_API_KEY')
 ```
 
 You can then use various methods on the client API, namely:
 - `api.apps()`: List of Applications
 - `api.get_app(name, version)`: Retrieve a specific Application
 - `api.update_app(name, version)`: Register an Application
-- `api.delete_app(name, version`: Delete an Application
+- `api.delete_app(name, version)`: Delete an Application
 - `api.instances()`: List of Instances
 - `api.get_instance()`: Retrieve a specific Instance
 - `api.update_instance(name, app_name, version, ...)`: Start an Instance
 - `api.delete_instance(name)`: Stop an Instance
 
 In addition to the common methods, v2 has the following API methods:
 - `api.get_compose(name, version, file_name)`: Retrieve a docker compose or 
   bigboat compose file for an Application
 - `api.update_compose(name, version, file_name, content)`: Update a docker 
   compose or bigboat compose file for an Application
-- `api.statuses()`: Retrieve a list of satus dictionaries
+- `api.statuses()`: Retrieve a list of status dictionaries
 
 ## Development
 
-- [Travis](https://travis-ci.org/ICTU/bigboat-python-api) is used to run unit 
-  tests and report on coverage.
-- [Coveralls](https://coveralls.io/github/ICTU/bigboat-python-api) receives 
-  coverage reports and tracks them.
-- You can perform local lint checks, tests and coverage during development 
-  using `make pylint`, `make test` and `make coverage`, respectively.
+- [GitHub 
+  Actions](https://github.com/grip-on-software/bigboat-python-api/actions) is 
+  used to run unit tests and report on coverage for commits and pull requests.
+- [SonarCloud](https://sonarcloud.io/project/overview?id=grip-on-software_bigboat-python-api) 
+  performs quality gate scans and tracks them.
+- [Coveralls](https://coveralls.io/github/grip-on-software/bigboat-python-api) 
+  receives coverage reports and tracks them.
+- You can perform local lint checks, typing checks, tests and coverage during 
+  development with `make pylint`, `make mypy`, `make test` and `make coverage`, 
+  respectively, after installing dependencies from `analysis-requirements.txt` 
+  (for the `pylint` and `mypy` recipes) and `test-requirements.txt` (necessary 
+  to let all recipes for checks function correctly).
 - We publish releases to [PyPI](https://pypi.python.org/pypi/bigboat) using 
-  `make release` which performs lint and unit test checks.
+  `make release` which performs multiple checks: version number consistency, 
+  lint, typing and unit tests.
 
 ## License
 
 The API wrapper library is licensed under the Apache 2.0 License.
 
 ## References
```

### Comparing `bigboat-0.2.9/setup.py` & `bigboat-0.3.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 #!/usr/bin/env python
 
 """
 Package setup script.
 
-Copyright 2017 ICTU
+Copyright 2017-2020 ICTU
+Copyright 2017-2022 Leiden University
+Copyright 2017-2023 Leon Helwerda
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from builtins import str
-from pip.download import PipSession
-from pip.req import parse_requirements
 from setuptools import setup, find_packages
-from bigboat import __version__
 
-setup(name='bigboat',
-      version=__version__,
-      description='BigBoat docker dashboard API',
-      long_description='''Python wrapper library for the BigBoat API.
+def main() -> None:
+    """
+    Setup the package.
+    """
+
+    setup(name='bigboat',
+          version='0.3.0',
+          description='BigBoat docker dashboard API',
+          long_description='''Python wrapper library for the BigBoat API.
 Support for v2 and the deprecated v1 is included.
 This API can create, retrieve, update and delete application definitions,
 do similar operations for instances and poll for status''',
-      author='ICTU',
-      author_email='leon.helwerda@ictu.nl',
-      url='https://github.com/ICTU/bigboat-python-api',
-      license='Apache License, Version 2.0',
-      packages=find_packages(exclude=['tests*']),
-      scripts=[],
-      include_package_data=True,
-      install_requires=[
-          str(requirement.req)
-          for requirement in parse_requirements('requirements.txt',
-                                                session=PipSession())
-      ],
-      test_suite='tests',
-      classifiers=[
-          'Development Status :: 3 - Alpha',
-          'Environment :: Web Environment',
-          'Intended Audience :: Developers',
-          'License :: OSI Approved :: Apache Software License',
-          'Operating System :: OS Independent',
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 2.7',
-          'Programming Language :: Python :: 3.6',
-          'Topic :: Internet :: WWW/HTTP',
-          'Topic :: Software Development :: Libraries :: Python Modules',
-          'Topic :: Software Development :: Build Tools'],
-      keywords=['docker', 'dashboard', 'bigboat', 'api'])
+          author='Leon Helwerda',
+          author_email='l.s.helwerda@liacs.leidenuniv.nl',
+          url='https://github.com/grip-on-software/bigboat-python-api',
+          license='Apache License, Version 2.0',
+          packages=find_packages(exclude=['tests*']),
+          package_data={'bigboat': ['py.typed']},
+          scripts=[],
+          include_package_data=True,
+          install_requires=[
+              'requests>=2.17.3',
+              'pyyaml>=3.12'
+          ],
+          python_requires='>=3',
+          test_suite='tests',
+          classifiers=[
+              'Development Status :: 4 - Beta',
+              'Environment :: Web Environment',
+              'Intended Audience :: Developers',
+              'License :: OSI Approved :: Apache Software License',
+              'Operating System :: OS Independent',
+              'Programming Language :: Python',
+              'Programming Language :: Python :: 3.8',
+              'Programming Language :: Python :: 3.11',
+              'Topic :: Internet :: WWW/HTTP',
+              'Topic :: Software Development :: Libraries :: Python Modules',
+              'Topic :: Software Development :: Build Tools'],
+          keywords='docker dashboard bigboat api')
+
+if __name__ == "__main__":
+    main()
```

