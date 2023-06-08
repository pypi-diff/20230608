# Comparing `tmp/metal_sdk-1.0.7.tar.gz` & `tmp/metal_sdk-1.0.8.tar.gz`

## Comparing `metal_sdk-1.0.7.tar` & `metal_sdk-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/src/metal_sdk/motorhead.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/src/metal_sdk/motorhead_async.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/tests/test_metal.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/tests/test_metal_async.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/tests/test_motorhead.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/tests/test_motorhead_async.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/tests/fixtures/sample.csv
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_metal.py
+-rw-r--r--   0        0        0     9962 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_metal_async.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_motorhead.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 metal_sdk-1.0.8/PKG-INFO
```

### Comparing `metal_sdk-1.0.7/.github/workflows/publish.yml` & `metal_sdk-1.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.7/.github/workflows/test.yml` & `metal_sdk-1.0.8/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,12 +14,12 @@
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v1
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
-          pip install httpx
+          pip install httpx respx
           pip install typing_extensions
       - name: Test with unittest
         run: |
           python -m unittest discover -s ./tests  -p 'test_*.py'
```

### Comparing `metal_sdk-1.0.7/examples/example.py` & `metal_sdk-1.0.8/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.7/examples/example_async.py` & `metal_sdk-1.0.8/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.7/src/metal_sdk/metal.py` & `metal_sdk-1.0.8/src/metal_sdk/metal.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,29 +46,29 @@
         elif payload.get("text") is not None:
             data["text"] = payload["text"]
         elif payload.get("embedding") is not None:
             data["embedding"] = payload["embedding"]
 
         return data
 
-    def __validateIndexAndSearch(self, index=None, payload={}):
+    def __validateIndex(self, index=None, payload={}):
         if index is None:
             raise TypeError("index_id required")
 
         if (
             payload.get("imageBase64") is None
             and payload.get("imageUrl") is None
             and payload.get("text") is None
             and payload.get("embedding") is None
         ):
             raise TypeError("imageBase64, imageUrl, text, or embedding required")
 
     def index(self, payload: IndexPayload = {}, index_id=None):
         index = self.index_id or index_id
-        self.__validateIndexAndSearch(index, payload)
+        self.__validateIndex(index, payload)
         data = self.__getData(index, payload)
         url = "/v1/index"
 
         res = self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
@@ -80,15 +80,18 @@
         res.raise_for_status()
         return res.json()
 
     def search(
         self, payload: SearchPayload = {}, index_id=None, ids_only=False, limit=1
     ):
         index = index_id or self.index_id
-        self.__validateIndexAndSearch(index, payload)
+
+        if index is None:
+            raise TypeError("index_id required")
+
         data = self.__getData(index, payload)
 
         url = "/v1/search?limit=" + str(limit)
 
         if ids_only:
             url = url + "&idsOnly=true"
```

### Comparing `metal_sdk-1.0.7/src/metal_sdk/metal_async.py` & `metal_sdk-1.0.8/src/metal_sdk/metal_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,29 +46,29 @@
         elif payload.get("text") is not None:
             data["text"] = payload["text"]
         elif payload.get("embedding") is not None:
             data["embedding"] = payload["embedding"]
 
         return data
 
-    def __validateIndexAndSearch(self, index=None, payload={}):
+    def __validateIndex(self, index=None, payload={}):
         if index is None:
             raise TypeError("index_id required")
 
         if (
             payload.get("imageBase64") is None
             and payload.get("imageUrl") is None
             and payload.get("text") is None
             and payload.get("embedding") is None
         ):
             raise TypeError("imageBase64, imageUrl, text, or embedding required")
 
     async def index(self, payload: IndexPayload = {}, index_id=None):
         index = self.index_id or index_id
-        self.__validateIndexAndSearch(index, payload)
+        self.__validateIndex(index, payload)
         data = self.__getData(index, payload)
         url = "/v1/index"
 
         res = await self.request("post", url, json=data)
         res.raise_for_status()
         return res.json()
 
@@ -80,15 +80,18 @@
         res.raise_for_status()
         return res.json()
 
     async def search(
         self, payload: SearchPayload = {}, index_id=None, ids_only=False, limit=1
     ):
         index = index_id or self.index_id
-        self.__validateIndexAndSearch(index, payload)
+
+        if index is None:
+            raise TypeError("index_id required")
+
         data = self.__getData(index, payload)
 
         url = "/v1/search?limit=" + str(limit)
 
         if ids_only:
             url = url + "&idsOnly=true"
```

### Comparing `metal_sdk-1.0.7/src/metal_sdk/motorhead.py` & `metal_sdk-1.0.8/src/metal_sdk/motorhead.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 import httpx
 from .typings import MotorheadPayload
 
-API_URL = 'https://api.getmetal.io/v1/motorhead'
+API_URL = 'https://api.getmetal.io/v1/motorhead/'
 
 
-class Motorhead:
+class Motorhead(httpx.Client):
     def __init__(self, payload: MotorheadPayload = {}):
+        super().__init__()
         self.api_key = payload.get("api_key")
         self.client_id = payload.get("client_id")
         self.base_url = payload.get("base_url") or API_URL
 
-        if self.base_url == API_URL and not (self.api_key and self.client_id):
+        has_api_key = self.api_key is not None
+        has_client_id = self.client_id is not None
+        has_key_and_id = has_api_key and has_client_id
+
+        if self.base_url == API_URL and not has_key_and_id:
             raise ValueError('api_key and client_id required for managed motorhead')
 
-        self.client = httpx.Client(headers={
+        self.headers.update({
             'Content-Type': 'application/json',
             'x-metal-api-key': self.api_key,
             'x-metal-client-id': self.client_id,
         })
 
+    def request(self, method, url, *args, **kwargs):
+        return super().request(method, url, *args, **kwargs)
+
     def add_memory(self, sessionId, payload):
-        response = self.client.post(f'{self.base_url}/sessions/{sessionId}/memory', json=payload)
-        response.raise_for_status()
+        url = f'/sessions/{sessionId}/memory'
+        res = self.request("post", url, json=payload)
+        res.raise_for_status()
 
-        data = response.json()
+        data = res.json()
         memory = data.get('data', data)
         return memory
 
     def get_memory(self, sessionId):
-        response = self.client.get(f'{self.base_url}/sessions/{sessionId}/memory')
-        response.raise_for_status()
-
-        data = response.json()
+        url = f'/sessions/{sessionId}/memory'
+        res = self.request("get", url)
+        res.raise_for_status()
+        data = res.json()
         memory = data.get('data', data)
         return memory
 
     def delete_memory(self, sessionId):
-        response = self.client.delete(f'{self.base_url}/sessions/{sessionId}/memory')
-        response.raise_for_status()
+        url = f'/sessions/{sessionId}/memory'
+        res = self.request("delete", url)
+        res.raise_for_status()
 
-        data = response.json()
+        data = res.json()
         return data.get('data', data)
```

### Comparing `metal_sdk-1.0.7/src/metal_sdk/motorhead_async.py` & `metal_sdk-1.0.8/src/metal_sdk/motorhead_async.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 import httpx
+from .typings import MotorheadPayload
 
-API_URL = 'https://api.getmetal.io/v1/motorhead'
+API_URL = 'https://api.getmetal.io/v1/motorhead/'
 
 
 class Motorhead(httpx.AsyncClient):
-    def __init__(self, api_key=None, client_id=None, base_url=API_URL):
+    def __init__(self, payload: MotorheadPayload = {}):
         super().__init__()
-        self.api_key = api_key
-        self.client_id = client_id
-        self.base_url = base_url
+        self.api_key = payload.get("api_key")
+        self.client_id = payload.get("client_id")
+        self.base_url = payload.get("base_url") or API_URL
+
+        has_api_key = self.api_key is not None
+        has_client_id = self.client_id is not None
+        has_key_and_id = has_api_key and has_client_id
 
-        if base_url == API_URL and not (api_key and client_id):
+        if self.base_url == API_URL and not has_key_and_id:
             raise ValueError('api_key and client_id required for managed motorhead')
 
         self.headers.update({
             'Content-Type': 'application/json',
             'x-metal-api-key': self.api_key,
             'x-metal-client-id': self.client_id,
         })
 
+    async def request(self, method, url, *args, **kwargs):
+        return await super().request(method, url, *args, **kwargs)
+
     async def add_memory(self, sessionId, payload):
-        response = await self.post(f'{self.base_url}/sessions/{sessionId}/memory', json=payload)
-        response.raise_for_status()
+        url = f'/sessions/{sessionId}/memory'
+        res = await self.request("post", url, json=payload)
+        res.raise_for_status()
 
-        data = response.json()
+        data = res.json()
         memory = data.get('data', data)
         return memory
 
     async def get_memory(self, sessionId):
-        response = await self.get(f'{self.base_url}/sessions/{sessionId}/memory')
-        response.raise_for_status()
-
-        data = response.json()
+        url = f'/sessions/{sessionId}/memory'
+        res = await self.request("get", url)
+        res.raise_for_status()
+        data = res.json()
         memory = data.get('data', data)
         return memory
 
     async def delete_memory(self, sessionId):
-        response = await self.delete(f'{self.base_url}/sessions/{sessionId}/memory')
-        response.raise_for_status()
+        url = f'/sessions/{sessionId}/memory'
+        res = await self.request("delete", url)
+        res.raise_for_status()
 
-        data = response.json()
-        return data.get('data', data)
+        return
```

### Comparing `metal_sdk-1.0.7/src/metal_sdk/typings.py` & `metal_sdk-1.0.8/src/metal_sdk/typings.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.7/tests/test_metal.py` & `metal_sdk-1.0.8/tests/test_metal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import respx
+from httpx import Response
 from unittest import TestCase, mock
 from src.metal_sdk.metal import Metal
 
 
 API_KEY = "api-key"
 CLIENT_ID = "client-id"
 
@@ -11,14 +13,26 @@
     def test_metal_instantiate(self):
         index_id = "index-id"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         self.assertEqual(metal.api_key, API_KEY)
         self.assertEqual(metal.client_id, CLIENT_ID)
         self.assertEqual(metal.index_id, index_id)
 
+    @respx.mock
+    def test_request(self):
+        url = 'https://api.getmetal.io/foo/bar'
+        method = 'GET'
+        respx.get(url).mock(return_value=Response(200))
+
+        index_id = "index-id"
+        metal = Metal(API_KEY, CLIENT_ID, index_id)
+
+        response = metal.request(method, "/foo/bar")
+        assert response.status_code == 200
+
     def test_metal_index_without_index(self):
         metal = Metal(API_KEY, CLIENT_ID)
         with self.assertRaises(TypeError) as ctx:
             metal.index()
         self.assertEqual(str(ctx.exception), "index_id required")
 
     def test_metal_index_without_payload(self):
@@ -73,18 +87,30 @@
             metal.search()
         self.assertEqual(str(ctx.exception), "index_id required")
 
     def test_metal_search_without_payload(self):
         my_index = "my-index"
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
-        with self.assertRaises(TypeError) as ctx:
-            metal.search()
+        metal.request = mock.MagicMock(return_value=mock.Mock(status_code=200))
+        metal.search({"filters": [{"field": "foo", "value": "bar"}]}, limit=666)
+
+        self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(
-            str(ctx.exception), "imageBase64, imageUrl, text, or embedding required"
+            metal.request.call_args[0][0],
+            "post",
+        )
+        self.assertEqual(
+            metal.request.call_args[0][1],
+            "/v1/search?limit=666",
+        )
+        self.assertEqual(metal.request.call_args[1]["json"]["index"], my_index)
+        self.assertEqual(metal.request.call_args[1]["json"].get("text"), None)
+        self.assertEqual(
+            metal.request.call_args[1]["json"]["filters"], [{"field": "foo", "value": "bar"}]
         )
 
     def test_metal_search_with_text(self):
         my_index = "my-index"
         payload = {
             "text": "some text",
             "filters": [{"field": "number_of_the_beast", "value": 666}],
```

### Comparing `metal_sdk-1.0.7/tests/test_metal_async.py` & `metal_sdk-1.0.8/tests/test_metal_async.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 import os
-from unittest import TestCase, mock
+import respx
+from httpx import Response
+from unittest import IsolatedAsyncioTestCase, mock
 from src.metal_sdk.metal_async import Metal
 
 
 API_KEY = "api-key"
 CLIENT_ID = "client-id"
 
 
-class TestMetal(TestCase):
+class TestMetal(IsolatedAsyncioTestCase):
     def test_metal_instantiate(self):
         index_id = "index-id"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
         self.assertEqual(metal.api_key, API_KEY)
         self.assertEqual(metal.client_id, CLIENT_ID)
         self.assertEqual(metal.index_id, index_id)
 
+    @respx.mock
+    async def test_request(self):
+        url = 'https://api.getmetal.io/foo/bar'
+        method = 'GET'
+        respx.get(url).mock(return_value=Response(200))
+
+        index_id = "index-id"
+        metal = Metal(API_KEY, CLIENT_ID, index_id)
+
+        response = await metal.request(method, "/foo/bar")
+        assert response.status_code == 200
+
     async def test_metal_index_without_index(self):
         metal = Metal(API_KEY, CLIENT_ID)
         with self.assertRaises(TypeError) as ctx:
             await metal.index()
         self.assertEqual(str(ctx.exception), "index_id required")
 
     async def test_metal_index_without_payload(self):
@@ -36,15 +50,19 @@
         mock_text = "some text"
         mock_id = "some-id"
         mock_metadata = {"some": "metadata"}
 
         payload = {"id": mock_id, "text": mock_text, "metadata": mock_metadata}
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
-        metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
+
+        metal.request = mock.AsyncMock(return_value=mock_response)
         await metal.index(payload)
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(
             metal.request.call_args[0][0], "post"
         )
         self.assertEqual(
@@ -59,15 +77,19 @@
         mock_text = "some text"
         mock_id = "some-id"
         mock_metadata = {"some": "metadata"}
 
         payload = [{"id": mock_id, "text": mock_text, "metadata": mock_metadata, "index": my_index}]
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
-        metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
+
+        metal.request = mock.AsyncMock(return_value=mock_response)
         await metal.index_many(payload)
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(
             metal.request.call_args[0][0], "post"
         )
         self.assertEqual(
@@ -80,28 +102,45 @@
         with self.assertRaises(TypeError) as ctx:
             await metal.search()
         self.assertEqual(str(ctx.exception), "index_id required")
 
     async def test_metal_search_without_payload(self):
         my_index = "my-index"
         metal = Metal(API_KEY, CLIENT_ID, my_index)
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
 
-        with self.assertRaises(TypeError) as ctx:
-            await metal.search()
+        metal.request = mock.AsyncMock(return_value=mock_response)
+
+        await metal.search()
+
+        self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(
-            str(ctx.exception), "imageBase64, imageUrl, text, or embedding required"
+            metal.request.call_args[0][0],
+            "post",
         )
+        self.assertEqual(
+            metal.request.call_args[0][1],
+            "/v1/search?limit=1",
+        )
+        self.assertEqual(metal.request.call_args[1]["json"]["index"], my_index)
+        self.assertEqual(metal.request.call_args[1]["json"].get("text"), None)
 
     async def test_metal_search_with_text(self):
         my_index = "my-index"
         payload = {"text": "some text"}
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
-        metal.request = mock.MagicMock(return_value=mock.Mock(status_code=201))
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
+
+        metal.request = mock.AsyncMock(return_value=mock_response)
 
         await metal.search(payload, ids_only=True, limit=100)
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(
             metal.request.call_args[0][0],
             "post",
@@ -126,72 +165,85 @@
             await metal.tune()
         self.assertEqual(str(ctx.exception), "idA, idB, and label required")
 
     async def test_metal_tune_with_payload(self):
         index_id = "index-id"
         payload = {"idA": "id-a", "idB": "id-b", "label": -1}
         metal = Metal(API_KEY, CLIENT_ID, index_id)
-        return_value = mock.MagicMock(json=lambda: {"status": "success", "message": "ok"})
-        metal.request = mock.MagicMock(return_value=return_value)
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
+
+        metal.request = mock.AsyncMock(return_value=mock_response)
 
         await metal.tune(payload)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "post")
         self.assertEqual(metal.request.call_args[0][1], "/v1/tune")
         self.assertEqual(metal.request.call_args[1]["json"]["index"], index_id)
         self.assertEqual(metal.request.call_args[1]["json"]["idA"], payload["idA"])
         self.assertEqual(metal.request.call_args[1]["json"]["idB"], payload["idB"])
         self.assertEqual(metal.request.call_args[1]["json"]["label"], payload["label"])
 
     async def test_metal_get_one_with_payload(self):
         index_id = "index-id"
         id = "dave"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
-        return_value = mock.MagicMock(json=lambda: {"band": "Megadeth"})
-        metal.request = mock.MagicMock(return_value=return_value)
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
+
+        metal.request = mock.AsyncMock(return_value=mock_response)
 
         await metal.get_one(id)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "get")
         self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/dave")
 
     async def test_metal_delete_one_with_payload(self):
         index_id = "index-id"
         id = "dave"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
-        return_value = mock.MagicMock(json=lambda: {"band": "Megadeth"})
-        metal.request = mock.MagicMock(return_value=return_value)
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
+
+        metal.request = mock.AsyncMock(return_value=mock_response)
+
+        await metal.delete_one(id)
 
-        await metal.get_one(id)
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
         self.assertEqual(metal.request.call_args[0][1], "/v1/indexes/index-id/documents/dave")
 
     async def test_metal_delete_many_with_payload(self):
         index_id = "index-id"
         id = "ozzy"
         metal = Metal(API_KEY, CLIENT_ID, index_id)
-        return_value = mock.MagicMock(json=lambda: {"ozzy": "black sabbath"})
-        metal.request = mock.MagicMock(return_value=return_value)
+        mock_response = mock.Mock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {"data": "foo"}
+
+        metal.request = mock.AsyncMock(return_value=mock_response)
 
         await metal.delete_many([id])
 
         self.assertEqual(metal.request.call_count, 1)
         self.assertEqual(metal.request.call_args[0][0], "delete")
         self.assertEqual(metal.request.call_args[0][1], "/v1/documents/bulk")
         self.assertEqual(metal.request.call_args[1]["json"]["ids"], [id])
 
     async def test_upload_file(self):
         my_index = "my-index"
         mock_file_path = "/path/to/mockfile.csv"
 
         metal = Metal(API_KEY, CLIENT_ID, my_index)
 
-        metal._Metal__create_resource = mock.MagicMock(return_value={'data': {'url': 'https://mockuploadurl.com'}})
-        metal._Metal__upload_file_to_url = mock.MagicMock()
+        metal._Metal__create_resource = mock.AsyncMock(return_value={'data': {'url': 'https://mockuploadurl.com'}})
+        metal._Metal__upload_file_to_url = mock.AsyncMock()
         os.path.getsize = mock.MagicMock(return_value=1000)
         os.path.basename = mock.MagicMock(return_value="mockfile.csv")
 
         await metal.upload_file(my_index, mock_file_path)
 
         self.assertEqual(metal._Metal__create_resource.call_count, 1)
         self.assertEqual(metal._Metal__upload_file_to_url.call_count, 1)
```

### Comparing `metal_sdk-1.0.7/.gitignore` & `metal_sdk-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.7/LICENSE` & `metal_sdk-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.7/README.md` & `metal_sdk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-1.0.7/pyproject.toml` & `metal_sdk-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-1.0.7/PKG-INFO` & `metal_sdk-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

