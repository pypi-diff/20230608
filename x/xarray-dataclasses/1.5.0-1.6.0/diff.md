# Comparing `tmp/xarray_dataclasses-1.5.0.tar.gz` & `tmp/xarray_dataclasses-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_dataclasses-1.5.0.tar", max compression
+gzip compressed data, was "xarray_dataclasses-1.6.0.tar", max compression
```

## Comparing `xarray_dataclasses-1.5.0.tar` & `xarray_dataclasses-1.6.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-02-02 10:11:55.122267 xarray_dataclasses-1.5.0/LICENSE
--rw-r--r--   0        0        0     9502 2023-02-02 10:11:55.122267 xarray_dataclasses-1.5.0/README.md
--rw-r--r--   0        0        0     1315 2023-02-02 10:11:55.134267 xarray_dataclasses-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      558 2023-02-02 10:11:55.134267 xarray_dataclasses-1.5.0/xarray_dataclasses/__init__.py
--rw-r--r--   0        0        0     9557 2023-02-02 10:11:55.134267 xarray_dataclasses-1.5.0/xarray_dataclasses/dataarray.py
--rw-r--r--   0        0        0     7858 2023-02-02 10:11:55.134267 xarray_dataclasses-1.5.0/xarray_dataclasses/datamodel.py
--rw-r--r--   0        0        0      533 2023-02-02 10:11:55.134267 xarray_dataclasses-1.5.0/xarray_dataclasses/dataoptions.py
--rw-r--r--   0        0        0     9375 2023-02-02 10:11:55.142267 xarray_dataclasses-1.5.0/xarray_dataclasses/dataset.py
--rw-r--r--   0        0        0        0 2023-02-02 10:11:55.142267 xarray_dataclasses-1.5.0/xarray_dataclasses/py.typed
--rw-r--r--   0        0        0     8922 2023-02-02 10:11:55.142267 xarray_dataclasses-1.5.0/xarray_dataclasses/typing.py
--rw-r--r--   0        0        0    10967 1970-01-01 00:00:00.000000 xarray_dataclasses-1.5.0/setup.py
--rw-r--r--   0        0        0    10687 1970-01-01 00:00:00.000000 xarray_dataclasses-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-08 16:58:56.722813 xarray_dataclasses-1.6.0/LICENSE
+-rw-r--r--   0        0        0     9502 2023-06-08 16:58:56.722813 xarray_dataclasses-1.6.0/README.md
+-rw-r--r--   0        0        0     1092 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      558 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/xarray_dataclasses/__init__.py
+-rw-r--r--   0        0        0     9557 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/xarray_dataclasses/dataarray.py
+-rw-r--r--   0        0        0     7903 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/xarray_dataclasses/datamodel.py
+-rw-r--r--   0        0        0      533 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/xarray_dataclasses/dataoptions.py
+-rw-r--r--   0        0        0     9375 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/xarray_dataclasses/dataset.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/xarray_dataclasses/py.typed
+-rw-r--r--   0        0        0     8922 2023-06-08 16:58:56.738813 xarray_dataclasses-1.6.0/xarray_dataclasses/typing.py
+-rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 xarray_dataclasses-1.6.0/PKG-INFO
```

### Comparing `xarray_dataclasses-1.5.0/LICENSE` & `xarray_dataclasses-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_dataclasses-1.5.0/README.md` & `xarray_dataclasses-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `xarray_dataclasses-1.5.0/pyproject.toml` & `xarray_dataclasses-1.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 [tool.poetry]
 name = "xarray-dataclasses"
-version = "1.5.0"
+version = "1.6.0"
 description = "xarray data creation made easy by dataclass"
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 keywords = ["xarray", "dataclass", "dataarray", "dataset", "typing"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/astropenguin/xarray-dataclasses/"
 documentation = "https://astropenguin.github.io/xarray-dataclasses/"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1, <3.12"
-numpy = [
-    { version = ">=1.15, <1.22", python = ">=3.7.1, <3.8" },
-    { version = "^1.15", python = ">=3.8, <3.12" },
-]
-typing-extensions = ">=3.10, <5.0"
+python = ">=3.8, <3.12"
+numpy = "^1.22"
+typing-extensions = "^4.0"
 xarray = [
-    { version = ">=0.18, <0.21", python = ">=3.7.1, <3.8" },
-    { version = ">=0.18, <2023", python = ">=3.8, <3.12" },
+    { version = ">=2022.3, <2023.2", python = ">=3.8, <3.9" },
+    { version = "^2022.3", python = ">=3.9, <3.12" },
 ]
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.8"
-ipython = [
-    { version = "^7.32", python = ">=3.7.1, <3.8" },
-    { version = "^8.4", python = ">=3.8, <3.12" },
-]
-myst-parser = "^0.18"
-pydata-sphinx-theme = "^0.9"
+black = "^23.1"
+ipython = "^8.11"
+myst-parser = "^1.0"
+pydata-sphinx-theme = "^0.13"
 pyright = "^1.1"
-pytest = "^7.1"
-sphinx = "^5.1"
+pytest = "^7.2"
+sphinx = "^6.1"
 
 [tool.pyright]
 reportImportCycles = "warning"
 reportUnknownArgumentType = "warning"
 reportUnknownMemberType = "warning"
 reportUnknownVariableType = "warning"
 typeCheckingMode = "strict"
```

### Comparing `xarray_dataclasses-1.5.0/xarray_dataclasses/__init__.py` & `xarray_dataclasses-1.6.0/xarray_dataclasses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "asdataset",
     "dataarray",
     "dataset",
     "datamodel",
     "dataoptions",
     "typing",
 ]
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 
 # submodules
 from . import dataarray
 from . import dataset
 from . import datamodel
 from . import dataoptions
```

### Comparing `xarray_dataclasses-1.5.0/xarray_dataclasses/dataarray.py` & `xarray_dataclasses-1.6.0/xarray_dataclasses/dataarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 __all__ = ["AsDataArray", "asdataarray"]
 
 
 # standard library
 from functools import partial
 from inspect import signature
 from types import MethodType
-from typing import Any, Callable, Optional, Type, TypeVar, Union, overload
+from typing import Any, Callable, Optional, Protocol, Type, TypeVar, Union, overload
 
 
 # dependencies
 import numpy as np
 import xarray as xr
-from typing_extensions import ParamSpec, Protocol
+from typing_extensions import ParamSpec
 
 
 # submodules
 from .datamodel import DataModel
 from .dataoptions import DataOptions
 from .typing import AnyArray, AnyXarray, DataClass, Order, Shape, Sizes
```

### Comparing `xarray_dataclasses-1.5.0/xarray_dataclasses/datamodel.py` & `xarray_dataclasses-1.6.0/xarray_dataclasses/datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 """Submodule for data expression inside the package."""
 __all__ = ["DataModel"]
 
 
 # standard library
 from dataclasses import dataclass, field, is_dataclass
-from typing import Any, Dict, Hashable, List, Optional, Tuple, Type, Union, cast
+from typing import (
+    Any,
+    Dict,
+    Hashable,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 
 # dependencies
 import numpy as np
 import xarray as xr
-from typing_extensions import Literal, ParamSpec, get_type_hints
+from typing_extensions import ParamSpec, get_type_hints
 
 
 # submodules
 from .typing import (
     AnyDType,
     AnyField,
     AnyXarray,
```

### Comparing `xarray_dataclasses-1.5.0/xarray_dataclasses/dataoptions.py` & `xarray_dataclasses-1.6.0/xarray_dataclasses/dataoptions.py`

 * *Files identical despite different names*

### Comparing `xarray_dataclasses-1.5.0/xarray_dataclasses/dataset.py` & `xarray_dataclasses-1.6.0/xarray_dataclasses/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 __all__ = ["AsDataset", "asdataset"]
 
 
 # standard library
 from functools import partial
 from inspect import signature
 from types import MethodType
-from typing import Any, Callable, Dict, Optional, Type, TypeVar, overload
+from typing import Any, Callable, Dict, Optional, Protocol, Type, TypeVar, overload
 
 
 # dependencies
 import numpy as np
 import xarray as xr
-from typing_extensions import ParamSpec, Protocol
+from typing_extensions import ParamSpec
 
 
 # submodules
 from .datamodel import DataModel
 from .dataoptions import DataOptions
 from .typing import AnyArray, AnyXarray, DataClass, Order, Shape, Sizes
```

### Comparing `xarray_dataclasses-1.5.0/xarray_dataclasses/typing.py` & `xarray_dataclasses-1.6.0/xarray_dataclasses/typing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,31 +25,31 @@
     Any,
     ClassVar,
     Collection,
     Dict,
     Generic,
     Hashable,
     Iterable,
+    Literal,
     Optional,
+    Protocol,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 
 # dependencies
 import numpy as np
 import xarray as xr
 from typing_extensions import (
     Annotated,
-    Literal,
     ParamSpec,
-    Protocol,
     TypeAlias,
     get_args,
     get_origin,
     get_type_hints,
 )
```

### Comparing `xarray_dataclasses-1.5.0/setup.py` & `xarray_dataclasses-1.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,370 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: xarray-dataclasses
+Version: 1.6.0
+Summary: xarray data creation made easy by dataclass
+Home-page: https://github.com/astropenguin/xarray-dataclasses/
+License: MIT
+Keywords: xarray,dataclass,dataarray,dataset,typing
+Author: Akio Taniguchi
+Author-email: taniguchi@a.phys.nagoya-u.ac.jp
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: typing-extensions (>=4.0,<5.0)
+Requires-Dist: xarray (>=2022.3,<2023.0) ; python_version >= "3.9" and python_version < "3.12"
+Requires-Dist: xarray (>=2022.3,<2023.2) ; python_version >= "3.8" and python_version < "3.9"
+Project-URL: Documentation, https://astropenguin.github.io/xarray-dataclasses/
+Description-Content-Type: text/markdown
 
-packages = \
-['xarray_dataclasses']
+# xarray-dataclasses
 
-package_data = \
-{'': ['*']}
+[![Release](https://img.shields.io/pypi/v/xarray-dataclasses?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/xarray-dataclasses/)
+[![Python](https://img.shields.io/pypi/pyversions/xarray-dataclasses?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/xarray-dataclasses/)
+[![Downloads](https://img.shields.io/pypi/dm/xarray-dataclasses?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/xarray-dataclasses)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.4624819-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.4624819)
+[![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/xarray-dataclasses/tests.yml?label=Tests&style=flat-square)](https://github.com/astropenguin/xarray-dataclasses/actions)
 
-install_requires = \
-['typing-extensions>=3.10,<5.0']
-
-extras_require = \
-{':python_full_version >= "3.7.1" and python_version < "3.8"': ['numpy>=1.15,<1.22',
-                                                                'xarray>=0.18,<0.21'],
- ':python_version >= "3.8" and python_version < "3.12"': ['numpy>=1.15,<2.0',
-                                                          'xarray>=0.18,<2023']}
-
-setup_kwargs = {
-    'name': 'xarray-dataclasses',
-    'version': '1.5.0',
-    'description': 'xarray data creation made easy by dataclass',
-    'long_description': '# xarray-dataclasses\n\n[![Release](https://img.shields.io/pypi/v/xarray-dataclasses?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/xarray-dataclasses/)\n[![Python](https://img.shields.io/pypi/pyversions/xarray-dataclasses?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/xarray-dataclasses/)\n[![Downloads](https://img.shields.io/pypi/dm/xarray-dataclasses?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/xarray-dataclasses)\n[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.4624819-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.4624819)\n[![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/xarray-dataclasses/tests.yml?label=Tests&style=flat-square)](https://github.com/astropenguin/xarray-dataclasses/actions)\n\nxarray data creation made easy by dataclass\n\n## Overview\n\nxarray-dataclasses is a Python package that makes it easy to create [xarray]\'s DataArray and Dataset objects that are "typed" (i.e. fixed dimensions, data type, coordinates, attributes, and name) using [the Python\'s dataclass]:\n\n```python\nfrom dataclasses import dataclass\nfrom typing import Literal\nfrom xarray_dataclasses import AsDataArray, Coord, Data\n\n\nX = Literal["x"]\nY = Literal["y"]\n\n\n@dataclass\nclass Image(AsDataArray):\n    """2D image as DataArray."""\n\n    data: Data[tuple[X, Y], float]\n    x: Coord[X, int] = 0\n    y: Coord[Y, int] = 0\n```\n\n### Features\n\n- Typed DataArray or Dataset objects can easily be created:\n  ```python\n  image = Image.new([[0, 1], [2, 3]], [0, 1], [0, 1])\n  ```\n- NumPy-like filled-data creation is also available:\n  ```python\n  image = Image.zeros([2, 2], x=[0, 1], y=[0, 1])\n  ```\n- Support for features by [the Python\'s dataclass] (`field`, `__post_init__`, ...).\n- Support for static type check by [Pyright].\n\n### Installation\n\n```shell\npip install xarray-dataclasses\n```\n\n## Basic usage\n\nxarray-dataclasses uses [the Python\'s dataclass].\nData (or data variables), coordinates, attributes, and a name of DataArray or Dataset objects will be defined as dataclass fields by special type hints (`Data`, `Coord`, `Attr`, `Name`), respectively.\nNote that the following code is supposed in the examples below.\n\n```python\nfrom dataclasses import dataclass\nfrom typing import Literal\nfrom xarray_dataclasses import AsDataArray, AsDataset\nfrom xarray_dataclasses import Attr, Coord, Data, Name\n\n\nX = Literal["x"]\nY = Literal["y"]\n```\n\n### Data field\n\nData field is a field whose value will become the data of a DataArray object or a data variable of a Dataset object.\nThe type hint `Data[TDims, TDtype]` fixes the dimensions and the data type of the object.\nHere are some examples of how to specify them.\n\nType hint | Inferred dimensions\n--- | ---\n`Data[tuple[()], ...]` | `()`\n`Data[Literal["x"], ...]` | `("x",)`\n`Data[tuple[Literal["x"]], ...]` | `("x",)`\n`Data[tuple[Literal["x"], Literal["y"]], ...]` | `("x", "y")`\n\nType hint | Inferred data type\n--- | ---\n`Data[..., Any]` | `None`\n`Data[..., None]` | `None`\n`Data[..., float]` | `numpy.dtype("float64")`\n`Data[..., numpy.float128]` | `numpy.dtype("float128")`\n`Data[..., Literal["datetime64[ns]"]]` | `numpy.dtype("<M8[ns]")`\n\n### Coordinate field\n\nCoordinate field is a field whose value will become a coordinate of a DataArray or a Dataset object.\nThe type hint `Coord[TDims, TDtype]` fixes the dimensions and the data type of the object.\n\n### Attribute field\n\nAttribute field is a field whose value will become an attribute of a DataArray or a Dataset object.\nThe type hint `Attr[TAttr]` specifies the type of the value, which is used only for static type check.\n\n### Name field\n\nName field is a field whose value will become the name of a DataArray object.\nThe type hint `Name[TName]` specifies the type of the value, which is used only for static type check.\n\n### DataArray class\n\nDataArray class is a dataclass that defines typed DataArray specifications.\nExactly one data field is allowed in a DataArray class.\nThe second and subsequent data fields are just ignored in DataArray creation.\n\n```python\n@dataclass\nclass Image(AsDataArray):\n    """2D image as DataArray."""\n\n    data: Data[tuple[X, Y], float]\n    x: Coord[X, int] = 0\n    y: Coord[Y, int] = 0\n    units: Attr[str] = "cd / m^2"\n    name: Name[str] = "luminance"\n```\n\nA DataArray object will be created by a class method `new()`:\n\n```python\nImage.new([[0, 1], [2, 3]], x=[0, 1], y=[0, 1])\n\n<xarray.DataArray "luminance" (x: 2, y: 2)>\narray([[0., 1.],\n       [2., 3.]])\nCoordinates:\n  * x        (x) int64 0 1\n  * y        (y) int64 0 1\nAttributes:\n    units:    cd / m^2\n```\n\nNumPy-like class methods (`zeros()`, `ones()`, ...) are also available:\n\n```python\nImage.ones((3, 3))\n\n<xarray.DataArray "luminance" (x: 3, y: 3)>\narray([[1., 1., 1.],\n       [1., 1., 1.],\n       [1., 1., 1.]])\nCoordinates:\n  * x        (x) int64 0 0 0\n  * y        (y) int64 0 0 0\nAttributes:\n    units:    cd / m^2\n```\n\n### Dataset class\n\nDataset class is a dataclass that defines typed Dataset specifications.\nMultiple data fields are allowed to define the data variables of the object.\n\n```python\n@dataclass\nclass ColorImage(AsDataset):\n    """2D color image as Dataset."""\n\n    red: Data[tuple[X, Y], float]\n    green: Data[tuple[X, Y], float]\n    blue: Data[tuple[X, Y], float]\n    x: Coord[X, int] = 0\n    y: Coord[Y, int] = 0\n    units: Attr[str] = "cd / m^2"\n```\n\nA Dataset object will be created by a class method `new()`:\n\n```python\nColorImage.new(\n    [[0, 0], [0, 0]],  # red\n    [[1, 1], [1, 1]],  # green\n    [[2, 2], [2, 2]],  # blue\n)\n\n<xarray.Dataset>\nDimensions:  (x: 2, y: 2)\nCoordinates:\n  * x        (x) int64 0 0\n  * y        (y) int64 0 0\nData variables:\n    red      (x, y) float64 0.0 0.0 0.0 0.0\n    green    (x, y) float64 1.0 1.0 1.0 1.0\n    blue     (x, y) float64 2.0 2.0 2.0 2.0\nAttributes:\n    units:    cd / m^2\n```\n\n## Advanced usage\n\n### Coordof and Dataof type hints\n\nxarray-dataclasses provides advanced type hints, `Coordof` and `Dataof`.\nUnlike `Data` and `Coord`, they specify a dataclass that defines a DataArray class.\nThis is useful when users want to add metadata to dimensions for [plotting].\nFor example:\n\n```python\nfrom xarray_dataclasses import Coordof\n\n\n@dataclass\nclass XAxis:\n    data: Data[X, int]\n    long_name: Attr[str] = "x axis"\n    units: Attr[str] = "pixel"\n\n\n@dataclass\nclass YAxis:\n    data: Data[Y, int]\n    long_name: Attr[str] = "y axis"\n    units: Attr[str] = "pixel"\n\n\n@dataclass\nclass Image(AsDataArray):\n    """2D image as DataArray."""\n\n    data: Data[tuple[X, Y], float]\n    x: Coordof[XAxis] = 0\n    y: Coordof[YAxis] = 0\n```\n\n### General data variable names in Dataset creation\n\nDue to the limitation of Python\'s parameter names, it is not possible to define data variable names that contain white spaces, for example.\nIn such cases, please define DataArray classes of each data variable so that they have name fields and specify them by `Dataof` in a Dataset class.\nThen the values of the name fields will be used as data variable names.\nFor example:\n\n```python\n@dataclass\nclass Red:\n    data: Data[tuple[X, Y], float]\n    name: Name[str] = "Red image"\n\n\n@dataclass\nclass Green:\n    data: Data[tuple[X, Y], float]\n    name: Name[str] = "Green image"\n\n\n@dataclass\nclass Blue:\n    data: Data[tuple[X, Y], float]\n    name: Name[str] = "Blue image"\n\n\n@dataclass\nclass ColorImage(AsDataset):\n    """2D color image as Dataset."""\n\n    red: Dataof[Red]\n    green: Dataof[Green]\n    blue: Dataof[Blue]\n```\n\n```python\nColorImage.new(\n    [[0, 0], [0, 0]],\n    [[1, 1], [1, 1]],\n    [[2, 2], [2, 2]],\n)\n\n<xarray.Dataset>\nDimensions:      (x: 2, y: 2)\nDimensions without coordinates: x, y\nData variables:\n    Red image    (x, y) float64 0.0 0.0 0.0 0.0\n    Green image  (x, y) float64 1.0 1.0 1.0 1.0\n    Blue image   (x, y) float64 2.0 2.0 2.0 2.0\n```\n\n### Customization of DataArray or Dataset creation\n\nFor customization, users can add a special class attribute, `__dataoptions__`, to a DataArray or Dataset class.\nA custom factory for DataArray or Dataset creation is only supported in the current implementation.\n\n\n```python\nimport xarray as xr\nfrom xarray_dataclasses import DataOptions\n\n\nclass Custom(xr.DataArray):\n    """Custom DataArray."""\n\n    __slots__ = ()\n\n    def custom_method(self) -> bool:\n        """Custom method."""\n        return True\n\n\n@dataclass\nclass Image(AsDataArray):\n    """2D image as DataArray."""\n\n    data: Data[tuple[X, Y], float]\n    x: Coord[X, int] = 0\n    y: Coord[Y, int] = 0\n\n    __dataoptions__ = DataOptions(Custom)\n\n\nimage = Image.ones([3, 3])\nisinstance(image, Custom)  # True\nimage.custom_method()  # True\n```\n\n### DataArray and Dataset creation without shorthands\n\nxarray-dataclasses provides functions, `asdataarray` and `asdataset`.\nThis is useful when users do not want to inherit the mix-in class (`AsDataArray` or `AsDataset`) in a DataArray or Dataset dataclass.\nFor example:\n\n```python\nfrom xarray_dataclasses import asdataarray\n\n\n@dataclass\nclass Image:\n    """2D image as DataArray."""\n\n    data: Data[tuple[X, Y], float]\n    x: Coord[X, int] = 0\n    y: Coord[Y, int] = 0\n\n\nimage = asdataarray(Image([[0, 1], [2, 3]], [0, 1], [0, 1]))\n```\n\n\n<!-- References -->\n[Pyright]: https://github.com/microsoft/pyright\n[the Python\'s dataclass]: https://docs.python.org/3/library/dataclasses.html\n[xarray]: https://xarray.pydata.org/en/stable/index.html\n[plotting]: https://xarray.pydata.org/en/stable/user-guide/plotting.html#simple-example\n',
-    'author': 'Akio Taniguchi',
-    'author_email': 'taniguchi@a.phys.nagoya-u.ac.jp',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/astropenguin/xarray-dataclasses/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<3.12',
-}
+xarray data creation made easy by dataclass
 
+## Overview
+
+xarray-dataclasses is a Python package that makes it easy to create [xarray]'s DataArray and Dataset objects that are "typed" (i.e. fixed dimensions, data type, coordinates, attributes, and name) using [the Python's dataclass]:
+
+```python
+from dataclasses import dataclass
+from typing import Literal
+from xarray_dataclasses import AsDataArray, Coord, Data
+
+
+X = Literal["x"]
+Y = Literal["y"]
+
+
+@dataclass
+class Image(AsDataArray):
+    """2D image as DataArray."""
+
+    data: Data[tuple[X, Y], float]
+    x: Coord[X, int] = 0
+    y: Coord[Y, int] = 0
+```
+
+### Features
+
+- Typed DataArray or Dataset objects can easily be created:
+  ```python
+  image = Image.new([[0, 1], [2, 3]], [0, 1], [0, 1])
+  ```
+- NumPy-like filled-data creation is also available:
+  ```python
+  image = Image.zeros([2, 2], x=[0, 1], y=[0, 1])
+  ```
+- Support for features by [the Python's dataclass] (`field`, `__post_init__`, ...).
+- Support for static type check by [Pyright].
+
+### Installation
+
+```shell
+pip install xarray-dataclasses
+```
+
+## Basic usage
+
+xarray-dataclasses uses [the Python's dataclass].
+Data (or data variables), coordinates, attributes, and a name of DataArray or Dataset objects will be defined as dataclass fields by special type hints (`Data`, `Coord`, `Attr`, `Name`), respectively.
+Note that the following code is supposed in the examples below.
+
+```python
+from dataclasses import dataclass
+from typing import Literal
+from xarray_dataclasses import AsDataArray, AsDataset
+from xarray_dataclasses import Attr, Coord, Data, Name
+
+
+X = Literal["x"]
+Y = Literal["y"]
+```
+
+### Data field
+
+Data field is a field whose value will become the data of a DataArray object or a data variable of a Dataset object.
+The type hint `Data[TDims, TDtype]` fixes the dimensions and the data type of the object.
+Here are some examples of how to specify them.
+
+Type hint | Inferred dimensions
+--- | ---
+`Data[tuple[()], ...]` | `()`
+`Data[Literal["x"], ...]` | `("x",)`
+`Data[tuple[Literal["x"]], ...]` | `("x",)`
+`Data[tuple[Literal["x"], Literal["y"]], ...]` | `("x", "y")`
+
+Type hint | Inferred data type
+--- | ---
+`Data[..., Any]` | `None`
+`Data[..., None]` | `None`
+`Data[..., float]` | `numpy.dtype("float64")`
+`Data[..., numpy.float128]` | `numpy.dtype("float128")`
+`Data[..., Literal["datetime64[ns]"]]` | `numpy.dtype("<M8[ns]")`
+
+### Coordinate field
+
+Coordinate field is a field whose value will become a coordinate of a DataArray or a Dataset object.
+The type hint `Coord[TDims, TDtype]` fixes the dimensions and the data type of the object.
+
+### Attribute field
+
+Attribute field is a field whose value will become an attribute of a DataArray or a Dataset object.
+The type hint `Attr[TAttr]` specifies the type of the value, which is used only for static type check.
+
+### Name field
+
+Name field is a field whose value will become the name of a DataArray object.
+The type hint `Name[TName]` specifies the type of the value, which is used only for static type check.
+
+### DataArray class
+
+DataArray class is a dataclass that defines typed DataArray specifications.
+Exactly one data field is allowed in a DataArray class.
+The second and subsequent data fields are just ignored in DataArray creation.
+
+```python
+@dataclass
+class Image(AsDataArray):
+    """2D image as DataArray."""
+
+    data: Data[tuple[X, Y], float]
+    x: Coord[X, int] = 0
+    y: Coord[Y, int] = 0
+    units: Attr[str] = "cd / m^2"
+    name: Name[str] = "luminance"
+```
+
+A DataArray object will be created by a class method `new()`:
+
+```python
+Image.new([[0, 1], [2, 3]], x=[0, 1], y=[0, 1])
+
+<xarray.DataArray "luminance" (x: 2, y: 2)>
+array([[0., 1.],
+       [2., 3.]])
+Coordinates:
+  * x        (x) int64 0 1
+  * y        (y) int64 0 1
+Attributes:
+    units:    cd / m^2
+```
+
+NumPy-like class methods (`zeros()`, `ones()`, ...) are also available:
+
+```python
+Image.ones((3, 3))
+
+<xarray.DataArray "luminance" (x: 3, y: 3)>
+array([[1., 1., 1.],
+       [1., 1., 1.],
+       [1., 1., 1.]])
+Coordinates:
+  * x        (x) int64 0 0 0
+  * y        (y) int64 0 0 0
+Attributes:
+    units:    cd / m^2
+```
+
+### Dataset class
+
+Dataset class is a dataclass that defines typed Dataset specifications.
+Multiple data fields are allowed to define the data variables of the object.
+
+```python
+@dataclass
+class ColorImage(AsDataset):
+    """2D color image as Dataset."""
+
+    red: Data[tuple[X, Y], float]
+    green: Data[tuple[X, Y], float]
+    blue: Data[tuple[X, Y], float]
+    x: Coord[X, int] = 0
+    y: Coord[Y, int] = 0
+    units: Attr[str] = "cd / m^2"
+```
+
+A Dataset object will be created by a class method `new()`:
+
+```python
+ColorImage.new(
+    [[0, 0], [0, 0]],  # red
+    [[1, 1], [1, 1]],  # green
+    [[2, 2], [2, 2]],  # blue
+)
+
+<xarray.Dataset>
+Dimensions:  (x: 2, y: 2)
+Coordinates:
+  * x        (x) int64 0 0
+  * y        (y) int64 0 0
+Data variables:
+    red      (x, y) float64 0.0 0.0 0.0 0.0
+    green    (x, y) float64 1.0 1.0 1.0 1.0
+    blue     (x, y) float64 2.0 2.0 2.0 2.0
+Attributes:
+    units:    cd / m^2
+```
+
+## Advanced usage
+
+### Coordof and Dataof type hints
+
+xarray-dataclasses provides advanced type hints, `Coordof` and `Dataof`.
+Unlike `Data` and `Coord`, they specify a dataclass that defines a DataArray class.
+This is useful when users want to add metadata to dimensions for [plotting].
+For example:
+
+```python
+from xarray_dataclasses import Coordof
+
+
+@dataclass
+class XAxis:
+    data: Data[X, int]
+    long_name: Attr[str] = "x axis"
+    units: Attr[str] = "pixel"
+
+
+@dataclass
+class YAxis:
+    data: Data[Y, int]
+    long_name: Attr[str] = "y axis"
+    units: Attr[str] = "pixel"
+
+
+@dataclass
+class Image(AsDataArray):
+    """2D image as DataArray."""
+
+    data: Data[tuple[X, Y], float]
+    x: Coordof[XAxis] = 0
+    y: Coordof[YAxis] = 0
+```
+
+### General data variable names in Dataset creation
+
+Due to the limitation of Python's parameter names, it is not possible to define data variable names that contain white spaces, for example.
+In such cases, please define DataArray classes of each data variable so that they have name fields and specify them by `Dataof` in a Dataset class.
+Then the values of the name fields will be used as data variable names.
+For example:
+
+```python
+@dataclass
+class Red:
+    data: Data[tuple[X, Y], float]
+    name: Name[str] = "Red image"
+
+
+@dataclass
+class Green:
+    data: Data[tuple[X, Y], float]
+    name: Name[str] = "Green image"
+
+
+@dataclass
+class Blue:
+    data: Data[tuple[X, Y], float]
+    name: Name[str] = "Blue image"
+
+
+@dataclass
+class ColorImage(AsDataset):
+    """2D color image as Dataset."""
+
+    red: Dataof[Red]
+    green: Dataof[Green]
+    blue: Dataof[Blue]
+```
+
+```python
+ColorImage.new(
+    [[0, 0], [0, 0]],
+    [[1, 1], [1, 1]],
+    [[2, 2], [2, 2]],
+)
+
+<xarray.Dataset>
+Dimensions:      (x: 2, y: 2)
+Dimensions without coordinates: x, y
+Data variables:
+    Red image    (x, y) float64 0.0 0.0 0.0 0.0
+    Green image  (x, y) float64 1.0 1.0 1.0 1.0
+    Blue image   (x, y) float64 2.0 2.0 2.0 2.0
+```
+
+### Customization of DataArray or Dataset creation
+
+For customization, users can add a special class attribute, `__dataoptions__`, to a DataArray or Dataset class.
+A custom factory for DataArray or Dataset creation is only supported in the current implementation.
+
+
+```python
+import xarray as xr
+from xarray_dataclasses import DataOptions
+
+
+class Custom(xr.DataArray):
+    """Custom DataArray."""
+
+    __slots__ = ()
+
+    def custom_method(self) -> bool:
+        """Custom method."""
+        return True
+
+
+@dataclass
+class Image(AsDataArray):
+    """2D image as DataArray."""
+
+    data: Data[tuple[X, Y], float]
+    x: Coord[X, int] = 0
+    y: Coord[Y, int] = 0
+
+    __dataoptions__ = DataOptions(Custom)
+
+
+image = Image.ones([3, 3])
+isinstance(image, Custom)  # True
+image.custom_method()  # True
+```
+
+### DataArray and Dataset creation without shorthands
+
+xarray-dataclasses provides functions, `asdataarray` and `asdataset`.
+This is useful when users do not want to inherit the mix-in class (`AsDataArray` or `AsDataset`) in a DataArray or Dataset dataclass.
+For example:
+
+```python
+from xarray_dataclasses import asdataarray
+
+
+@dataclass
+class Image:
+    """2D image as DataArray."""
+
+    data: Data[tuple[X, Y], float]
+    x: Coord[X, int] = 0
+    y: Coord[Y, int] = 0
+
+
+image = asdataarray(Image([[0, 1], [2, 3]], [0, 1], [0, 1]))
+```
+
+
+<!-- References -->
+[Pyright]: https://github.com/microsoft/pyright
+[the Python's dataclass]: https://docs.python.org/3/library/dataclasses.html
+[xarray]: https://xarray.pydata.org/en/stable/index.html
+[plotting]: https://xarray.pydata.org/en/stable/user-guide/plotting.html#simple-example
 
-setup(**setup_kwargs)
```

