# Comparing `tmp/pyhatching-0.0.1.tar.gz` & `tmp/pyhatching-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhatching-0.0.1.tar", last modified: Mon Jun  5 03:54:26 2023, max compression
+gzip compressed data, was "pyhatching-0.0.2.tar", last modified: Thu Jun  8 01:57:26 2023, max compression
```

## Comparing `pyhatching-0.0.1.tar` & `pyhatching-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 03:54:26.045759 pyhatching-0.0.1/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 03:15:48.000000 pyhatching-0.0.1/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-05 03:54:26.045610 pyhatching-0.0.1/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      248 2023-05-21 14:55:53.000000 pyhatching-0.0.1/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      576 2023-06-05 03:54:21.000000 pyhatching-0.0.1/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-05 03:54:26.045801 pyhatching-0.0.1/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 03:54:26.043506 pyhatching-0.0.1/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 03:54:26.044627 pyhatching-0.0.1/src/pyhatching/
--rw-r--r--   0 gormo      (501) staff       (20)      429 2023-06-05 03:54:21.000000 pyhatching-0.0.1/src/pyhatching/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)    10033 2023-06-05 03:35:35.000000 pyhatching-0.0.1/src/pyhatching/base.py
--rw-r--r--   0 gormo      (501) staff       (20)    13488 2023-06-05 03:40:30.000000 pyhatching-0.0.1/src/pyhatching/client.py
--rw-r--r--   0 gormo      (501) staff       (20)     6452 2023-05-21 19:16:04.000000 pyhatching-0.0.1/src/pyhatching/enums.py
--rw-r--r--   0 gormo      (501) staff       (20)      290 2023-05-21 19:23:55.000000 pyhatching-0.0.1/src/pyhatching/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)     1325 2023-05-21 19:44:15.000000 pyhatching-0.0.1/src/pyhatching/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-05 03:54:26.045288 pyhatching-0.0.1/src/pyhatching.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-05 03:54:26.000000 pyhatching-0.0.1/src/pyhatching.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      369 2023-06-05 03:54:26.000000 pyhatching-0.0.1/src/pyhatching.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-05 03:54:26.000000 pyhatching-0.0.1/src/pyhatching.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       32 2023-06-05 03:54:26.000000 pyhatching-0.0.1/src/pyhatching.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-05 03:54:26.000000 pyhatching-0.0.1/src/pyhatching.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.648196 pyhatching-0.0.2/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-05 03:15:48.000000 pyhatching-0.0.2/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-08 01:57:26.648060 pyhatching-0.0.2/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      248 2023-05-21 14:55:53.000000 pyhatching-0.0.2/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      576 2023-06-08 01:57:22.000000 pyhatching-0.0.2/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-08 01:57:26.648235 pyhatching-0.0.2/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.646129 pyhatching-0.0.2/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.647271 pyhatching-0.0.2/src/pyhatching/
+-rw-r--r--   0 gormo      (501) staff       (20)      429 2023-06-08 01:57:22.000000 pyhatching-0.0.2/src/pyhatching/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)    10033 2023-06-05 03:35:35.000000 pyhatching-0.0.2/src/pyhatching/base.py
+-rw-r--r--   0 gormo      (501) staff       (20)    16259 2023-06-08 01:55:08.000000 pyhatching-0.0.2/src/pyhatching/client.py
+-rw-r--r--   0 gormo      (501) staff       (20)     6452 2023-05-21 19:16:04.000000 pyhatching-0.0.2/src/pyhatching/enums.py
+-rw-r--r--   0 gormo      (501) staff       (20)      393 2023-06-08 01:29:54.000000 pyhatching-0.0.2/src/pyhatching/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1325 2023-05-21 19:44:15.000000 pyhatching-0.0.2/src/pyhatching/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-08 01:57:26.647877 pyhatching-0.0.2/src/pyhatching.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1831 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      369 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       32 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-08 01:57:26.000000 pyhatching-0.0.2/src/pyhatching.egg-info/top_level.txt
```

### Comparing `pyhatching-0.0.1/LICENSE` & `pyhatching-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhatching-0.0.1/PKG-INFO` & `pyhatching-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhatching
-Version: 0.0.1
+Version: 0.0.2
 Summary: An async Python client for the Hatching Triage Sandbox.
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyhatching-0.0.1/pyproject.toml` & `pyhatching-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyhatching"
-version = "0.0.1"
+version = "0.0.2"
 description = "An async Python client for the Hatching Triage Sandbox."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
     "aiohttp==3.8.4",
     "pydantic==1.10.7",
 ]
```

### Comparing `pyhatching-0.0.1/src/pyhatching/base.py` & `pyhatching-0.0.2/src/pyhatching/base.py`

 * *Files identical despite different names*

### Comparing `pyhatching-0.0.1/src/pyhatching/client.py` & `pyhatching-0.0.2/src/pyhatching/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,160 @@
 """The pyhatching HTTP client implementation."""
 
 # import asyncio
+import functools
 from json import JSONDecodeError
 import pathlib
 
 import aiohttp
 from pydantic.error_wrappers import ValidationError  # pylint: disable=E0611
 
 from . import base
 from . import enums
 from . import errors
 from . import utils
 from . import BASE_URL, __version__
 
 
+def convert_to_model(
+    model: base.HatchingResponse,
+    resp: aiohttp.ClientResponse,
+    obj: dict,
+    raise_on_api_err: bool = False,
+) -> base.HatchingResponse | list[base.HatchingResponse]:
+    """Convert an API response to the given model.
+
+    Parameters
+    ----------
+    model : base.HatchingResponse
+        The model to convert the response to.
+    resp : aiohttp.ClientResponse
+        The HTTP response object so it can be added to the model.
+    obj : dict
+        The already deserialized JSON data from the given response.
+    raise_on_api_err : bool, optional
+        Whether to raise if ``obj`` is actually an API error (``base.ErrorResponse``).
+        By default False.
+
+    Returns
+    -------
+    base.HatchingResponse | list[base.HatchingResponse]
+        The API can return either a list or a single item depending on the endpoint
+        so can this method. The objects returned are of the same type as ``model``.
+
+    Raises
+    ------
+    errors.PyHatchingParseError
+        If ``obj`` could not be validated when passed to ``model``. Or when
+        ``obj`` is not a dict.
+    errors.PyHatchingResponseError
+        If ``raise_on_api_err`` is ``True`` and ``obj`` represents an error
+        returned by the Hatching Triage API and not a successful response.
+    """
+
+    ret = []
+    url = resp.request_info.url
+    try:
+        if "data" in obj:
+            for item in obj["data"]:
+                ret.append(model(resp_obj=obj, **item))
+        elif "error" in obj:
+            ret = base.ErrorResponse(resp_obj=resp, **obj)
+        elif isinstance(obj, dict):
+            ret = model(resp_obj=resp, **obj)
+        else:
+            raise errors.PyHatchingParseError(
+                f"Unexpected response from the {url} endpoint: {obj}"
+            )
+    except ValidationError as err:
+        raise errors.PyHatchingParseError(
+            f"Unable to validate {url} response: {err}"
+        ) from err
+
+    if raise_on_api_err and isinstance(ret, base.ErrorResponse):
+        raise errors.PyHatchingResponseError(
+            f"Hatching Triage API Error - {ret.error} - {ret.message}"
+        )
+
+    return ret
+
+
 class PyHatchingClient:
     """An async HTTP client that interfaces with the Hatching Triage Sandbox.
 
     Any method that makes HTTP requests (calls ``_request``) may raise either
-    a ``PyHatchingRequestError`` or ``PyHatchingParseError``. If the specific method
-    also explicitly raises exceptions, it will be documented.
+    a ``PyHatchingRequestError`` or ``PyHatchingParseError``.
+
+    Additionally, any method that returns a Pydantic model (``base.HatchingResponse``)
+    may raise a ``PyHatchingParseError``. If ``raise_on_api_err`` is ``True``, these
+    methods may raise a ``PyHatchingResponseError`` as well.
+    
+    If a specific method also explicitly raises exceptions, it will be documented.
+
     Catch all handled errors with ``PyHatchingError``.
 
     Parameters
     ----------
     api_key : str
         The Hatching Triage Sandbox API key to use for requests.
     url : str, optional
         The URL to use as a base in all requests, by default BASE_URL.
     timeout : int, optional
         The total timeout for all requests, by default 60.
+    raise_on_api_err : bool, optional
+        Whether to raise when the Hatching Triage API returns an API error response
+        (an HTTP 200 response that describes a handled error with the request).
+        See the `docs`_ for further information.
 
     Attributes
     ----------
     api_key : str
         The Hatching Triage Sandbox API key to use for requests.
     headers : dict
         The headers used with every request, has API key and custom User Agent.
     session : aiohttp.ClientSession
         The underlying ClientSession used to make requests.
     timeout : aiohttp.ClientTimeout
         The timeout object used by ``session``.
+    convert_resp : typing.Callable
+        A ``functools.partial`` for ``convert_to_model`` with ```raise_on_api_err``
+        saved so that it doesn't have to be passed to each method call.
 
+    .. _docs: https://tria.ge/docs/cloud-api/conventions/
     """
 
-    def __init__(self, api_key: str, url: str = BASE_URL, timeout: int = 60) -> None:
+    def __init__(
+        self,
+        api_key: str,
+        url: str = BASE_URL,
+        timeout: int = 60,
+        raise_on_api_err: bool = False,
+    ) -> None:
         self.api_key = api_key
         self.headers = {
             "Authorization": f"Bearer {self.api_key}",
-            "User-Agent": f"pyhatching v{__version__}",
+            "User-Agent": f"{aiohttp.http.SERVER_SOFTWARE} pyhatching/{__version__}",
         }
         self.timeout = aiohttp.ClientTimeout(total=timeout)
         self.session = aiohttp.ClientSession(
             base_url=url, headers=self.headers, timeout=self.timeout
         )
 
+        self.convert_resp = functools.partial(
+            convert_to_model, raise_on_api_err=raise_on_api_err
+        )
+
     async def _request(
         self,
         method: str,
         uri: str,
         data: dict | None = None,
         json: dict | None = None,
         params: dict | None = None,
-        raw: bool = False
+        raw: bool = False,
     ) -> tuple[aiohttp.ClientResponse, dict]:
         """Make an HTTP request to the Hatching Triage Sandbox API.
 
         Returns both the response and the deserialized JSON response.
 
         The response and deserialized JSON are returned regardless of the HTTP
         status code. This way, endpoint specific methods can handle errors. We
@@ -148,15 +236,17 @@
 
         if utils.is_hash(sample):
             sample_id = await self.sample_id(sample)
         else:
             sample_id = sample
 
         if sample_id is None:
-            raise errors.PyHatchingParseError(f"Unable to determine sample_id from: {sample}")
+            raise errors.PyHatchingParseError(
+                f"Unable to determine sample_id from: {sample}"
+            )
 
         resp, _ = await self._request("get", f"/samples/{sample_id}/sample", raw=True)
 
         if resp.status == 200:
             sample_bytes = await resp.read()
             return sample_bytes
 
@@ -176,14 +266,18 @@
         -------
         base.HatchingProfileResponse
             If successful, the requested sandbox profile.
         base.ErrorResponse
             If there was an error.
         """
 
+        resp, resp_dict = await self._request("get", f"/profiles/{profile_id}")
+
+        return self.convert_resp(base.HatchingProfileResponse, resp, resp_dict)
+
     async def get_profiles(
         self,
     ) -> list[base.HatchingProfileResponse] | base.ErrorResponse:
         """Get all sandbox analysis profiles for your account.
 
         Returns
         -------
@@ -220,15 +314,15 @@
         """Return a sample's Overview Report.
 
         Parameters
         ----------
         sample : str
             The sample to download, this can be any of the following
             as the value is passed to ``sample_id`` if needed to find the ID::
-    
+
                 sample_id, md5, sha1, sha2, ssdeep
 
         Returns
         -------
         base.OverviewReport
             If successful, the return Overview Report.
         """
@@ -263,15 +357,17 @@
 
         if len(samples) > 1:
             # TODO There should only be one sample per hash right?
             return samples[0].id
 
         return None
 
-    async def search(self, query: str) -> list[base.SamplesResponse] | base.ErrorResponse:
+    async def search(
+        self, query: str
+    ) -> list[base.SamplesResponse] | base.ErrorResponse:
         """Search the Hatching Triage Sandbox for samples matching ``query``.
 
         See the Hatching Triage `docs`_ for how to search.
 
         Does not handle pagination yet, returns only the first 20 hits!
 
         Parameters
@@ -289,31 +385,15 @@
         """
 
         # TODO Handle pagination
         params = {"query": query}
 
         resp, resp_dict = await self._request("get", "/search", params=params)
 
-        try:
-            if "data" in resp_dict:
-                ret = []
-                for item in resp_dict["data"]:
-                    ret.append(base.SamplesResponse(resp_obj=resp, **item))
-            elif "error" in resp_dict:
-                ret = base.ErrorResponse(resp_obj=resp, **resp_dict)
-            else:
-                raise errors.PyHatchingParseError(
-                    f"Unexpected response from the /search endpoint: {resp_dict}"
-                )
-        except ValidationError as err:
-            raise errors.PyHatchingParseError(
-                f"Unable to validate /search response: {err}"
-            ) from err
-
-        return ret
+        return self.convert_resp(base.SamplesResponse, resp, resp_dict)
 
     async def submit_profile(
         self,
         name: str,
         tags: list[str],
         timeout: int,
         network: enums.ProfileNetworkOptions,
@@ -321,15 +401,16 @@
         """Add a new sandbox analysis profile to your account.
 
         Parameters
         ----------
         name : str
             The name of the new profile, must not exist already.
         tags : list[str]
-            The tags that match this profile to samples (TODO find the documented options).
+            The tags that match this profile to samples.
+            TODO find the documented options
         timeout : int
             The profiles timeout length in seconds.
         network : enums.ProfileNetworkOptions
             The network option for this analysis profile.
 
         Returns
         -------
@@ -403,15 +484,16 @@
         -------
         None | base.ErrorResponse
             None if successful, otherwise a ``base.ErrorResponse``.
 
         Raises
         ------
         ValueError
-            If both ``name`` and ``profile_id`` are not set. Or if both parameters are set.
+            If both ``name`` and ``profile_id`` are not set.
+            Or if both parameters are set.
         """
 
     async def update_rule(self, name: str, contents: str) -> base.ErrorResponse | None:
         """Update an existing Yara rule.
 
         Parameters
         ----------
```

### Comparing `pyhatching-0.0.1/src/pyhatching/enums.py` & `pyhatching-0.0.2/src/pyhatching/enums.py`

 * *Files identical despite different names*

### Comparing `pyhatching-0.0.1/src/pyhatching/utils.py` & `pyhatching-0.0.2/src/pyhatching/utils.py`

 * *Files identical despite different names*

### Comparing `pyhatching-0.0.1/src/pyhatching.egg-info/PKG-INFO` & `pyhatching-0.0.2/src/pyhatching.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhatching
-Version: 0.0.1
+Version: 0.0.2
 Summary: An async Python client for the Hatching Triage Sandbox.
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

