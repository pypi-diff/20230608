# Comparing `tmp/actymath-0.1.2.tar.gz` & `tmp/actymath-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actymath-0.1.2.tar", max compression
+gzip compressed data, was "actymath-0.1.3.tar", max compression
```

## Comparing `actymath-0.1.2.tar` & `actymath-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1062 2023-04-11 17:09:38.439250 actymath-0.1.2/LICENSE
--rw-r--r--   0        0        0     2155 2023-04-11 17:09:38.439385 actymath-0.1.2/README.md
--rw-r--r--   0        0        0       84 2023-04-11 17:09:38.439539 actymath-0.1.2/actymath/__init__.py
--rw-r--r--   0        0        0     3205 2023-04-11 17:09:38.439669 actymath-0.1.2/actymath/calc.py
--rw-r--r--   0        0        0      457 2023-04-11 17:09:38.439845 actymath-0.1.2/actymath/columns/__init__.py
--rw-r--r--   0        0        0     2832 2023-04-11 17:09:38.439973 actymath-0.1.2/actymath/columns/base.py
--rw-r--r--   0        0        0     2074 2023-04-11 17:09:38.440089 actymath-0.1.2/actymath/columns/commutation.py
--rw-r--r--   0        0        0      545 2023-04-11 17:09:38.440193 actymath-0.1.2/actymath/columns/interest_rates.py
--rw-r--r--   0        0        0     2746 2023-04-11 17:09:38.440314 actymath-0.1.2/actymath/columns/mortality.py
--rw-r--r--   0        0        0     7087 2023-04-11 17:09:38.440423 actymath-0.1.2/actymath/columns/term.py
--rw-r--r--   0        0        0      689 2023-04-11 17:09:38.440523 actymath-0.1.2/actymath/columns/timeline.py
--rw-r--r--   0        0        0     2689 2023-04-11 17:09:38.440663 actymath-0.1.2/actymath/columns/whole_of_life.py
--rw-r--r--   0        0        0       41 2023-04-11 17:09:38.440775 actymath-0.1.2/actymath/exceptions.py
--rw-r--r--   0        0        0     1399 2023-04-11 17:33:48.998331 actymath-0.1.2/actymath/indexers.py
--rw-r--r--   0        0        0     3625 2023-04-11 17:09:38.441087 actymath-0.1.2/actymath/table_data/a1967-70.csv
--rw-r--r--   0        0        0     3094 2023-04-11 17:09:38.441220 actymath-0.1.2/actymath/table_data/a1967-70_exam.csv
--rw-r--r--   0        0        0     2710 2023-04-11 17:09:38.441335 actymath-0.1.2/actymath/table_data/amc00.csv
--rw-r--r--   0        0        0     1279 2023-04-11 17:09:38.441452 actymath-0.1.2/actymath/table_data/test.csv
--rw-r--r--   0        0        0       88 2023-04-11 17:09:38.441551 actymath-0.1.2/actymath/table_data/test_lx.csv
--rw-r--r--   0        0        0     6687 2023-04-11 17:09:38.441763 actymath-0.1.2/actymath/tables.py
--rw-r--r--   0        0        0      751 2023-04-11 17:33:54.189540 actymath-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 actymath-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-11 17:09:38.439250 actymath-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2235 2023-06-08 08:15:21.728623 actymath-0.1.3/README.md
+-rw-r--r--   0        0        0       46 2023-06-08 08:46:56.458345 actymath-0.1.3/actymath/__init__.py
+-rw-r--r--   0        0        0     3236 2023-06-08 08:48:41.711133 actymath-0.1.3/actymath/calc.py
+-rw-r--r--   0        0        0      457 2023-04-11 17:09:38.439845 actymath-0.1.3/actymath/columns/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-08 08:49:47.202506 actymath-0.1.3/actymath/columns/base.py
+-rw-r--r--   0        0        0     2120 2023-06-08 08:49:53.822330 actymath-0.1.3/actymath/columns/commutation.py
+-rw-r--r--   0        0        0      556 2023-06-08 08:49:58.410615 actymath-0.1.3/actymath/columns/interest_rates.py
+-rw-r--r--   0        0        0     2757 2023-06-08 08:50:06.606044 actymath-0.1.3/actymath/columns/mortality.py
+-rw-r--r--   0        0        0     7098 2023-06-08 08:50:10.535538 actymath-0.1.3/actymath/columns/term.py
+-rw-r--r--   0        0        0      700 2023-06-08 08:50:14.520842 actymath-0.1.3/actymath/columns/timeline.py
+-rw-r--r--   0        0        0     2735 2023-06-08 08:50:17.267449 actymath-0.1.3/actymath/columns/whole_of_life.py
+-rw-r--r--   0        0        0       88 2023-06-08 08:48:58.964621 actymath-0.1.3/actymath/exceptions.py
+-rw-r--r--   0        0        0     1399 2023-04-11 17:33:48.998331 actymath-0.1.3/actymath/indexers.py
+-rw-r--r--   0        0        0     3625 2023-04-11 17:09:38.441087 actymath-0.1.3/actymath/table_data/a1967-70.csv
+-rw-r--r--   0        0        0     3094 2023-04-11 17:09:38.441220 actymath-0.1.3/actymath/table_data/a1967-70_exam.csv
+-rw-r--r--   0        0        0     2710 2023-04-11 17:09:38.441335 actymath-0.1.3/actymath/table_data/amc00.csv
+-rw-r--r--   0        0        0     1279 2023-04-11 17:09:38.441452 actymath-0.1.3/actymath/table_data/test.csv
+-rw-r--r--   0        0        0       88 2023-04-11 17:09:38.441551 actymath-0.1.3/actymath/table_data/test_lx.csv
+-rw-r--r--   0        0        0     8886 2023-06-08 08:49:05.770184 actymath-0.1.3/actymath/tables.py
+-rw-r--r--   0        0        0      768 2023-06-08 08:51:22.450057 actymath-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 actymath-0.1.3/PKG-INFO
```

### Comparing `actymath-0.1.2/LICENSE` & `actymath-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `actymath-0.1.2/README.md` & `actymath-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
 These formulae can be explored in the [actymath/columns directory](https://github.com/ttamg/actymath/tree/main/actymath/columns).
 
 ### Mortality tables
 
 Currently only a few old standard mortality tables are implemented, but there is support for 1D and 2D mortality tables [here](https://github.com/ttamg/actymath/blob/main/actymath/tables.py).
 
+New 1D and 2D mortality tables can be loaded in from CSV or pandas DataFrames.
+
 ## Contributing
 
 Feel free to contribute or suggest improvements.
 
 - Add suggested improvements as a GitHub issue on this project
 
 - Pull requests also welcomed, particularly for any fixes, new tables or useful actuarial formulae
```

### Comparing `actymath-0.1.2/actymath/calc.py` & `actymath-0.1.3/actymath/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 
 from .indexers import SliceNIndexer, SliceToEndIndexer
-from actymath import columns, ActyMathError
+from actymath import columns
+from actymath.exceptions import ActyMathError
 
 
 # A dictionary mapping all column names to Column classes - created on the fly at import time
 register = dict(
     [
         (cls.column_name, cls)
         for name, cls in columns.__dict__.items()
```

### Comparing `actymath-0.1.2/actymath/columns/base.py` & `actymath-0.1.3/actymath/columns/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractclassmethod
 
 import pandas as pd
 import parse
-from actymath import ActyMathError, columns
+from actymath.exceptions import ActyMathError
 
 
 class Column:
     """ An abstract class for columns to populate """
 
     default = None  # A default value to use if the value is missing
     parameters = {}  # Required kwargs parameters for populating this Column.
```

### Comparing `actymath-0.1.2/actymath/columns/commutation.py` & `actymath-0.1.3/actymath/columns/commutation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 
 from .base import Column
 from actymath.indexers import SliceToEndIndexer
+from actymath.exceptions import ActyMathError
 
 """ Commutation functions. """
 
 # Indexers to perform Pandas slice operations
 indexer_to_end = SliceToEndIndexer()
```

### Comparing `actymath-0.1.2/actymath/columns/interest_rates.py` & `actymath-0.1.3/actymath/columns/interest_rates.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .base import Column
-from actymath import ActyMathError
+from actymath.exceptions import ActyMathError
 
 
 class i(Column):
     """ Fixed interest rate """
 
     column_name = "i"
```

### Comparing `actymath-0.1.2/actymath/columns/mortality.py` & `actymath-0.1.3/actymath/columns/mortality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 
 from .base import Column
-from actymath import ActyMathError
+from actymath.exceptions import ActyMathError
 from actymath.indexers import SliceToEndIndexer
 
 
 """ Base mortality functions. """
 
 indexer_to_end = SliceToEndIndexer()
```

### Comparing `actymath-0.1.2/actymath/columns/term.py` & `actymath-0.1.3/actymath/columns/term.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import numpy as np
-from actymath import ActyMathError
+from actymath.exceptions import ActyMathError
 
 from .base import Column
 
 """ Actuarial formulae for term limited life insurance. """
 
 
 class a_due_x_n(Column):
```

### Comparing `actymath-0.1.2/actymath/columns/timeline.py` & `actymath-0.1.3/actymath/columns/timeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 from actymath.indexers import SliceNIndexer
 
 from .base import Column
-from actymath import ActyMathError
+from actymath.exceptions import ActyMathError
 
 """ Defining time periods. """
 
 
 class t(Column):
     """ Time period count starting at zero. """
```

### Comparing `actymath-0.1.2/actymath/columns/whole_of_life.py` & `actymath-0.1.3/actymath/columns/whole_of_life.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 
-from .base import Column
+from actymath.exceptions import ActyMathError
 
+from .base import Column
 
 """ Actuarial formulae for whole remainder of life. """
 
 
 class a_due_x(Column):
     """ PV of annuity due (paid in advance) for remainder of life. """
```

### Comparing `actymath-0.1.2/actymath/indexers.py` & `actymath-0.1.3/actymath/indexers.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.2/actymath/table_data/a1967-70.csv` & `actymath-0.1.3/actymath/table_data/a1967-70.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.2/actymath/table_data/a1967-70_exam.csv` & `actymath-0.1.3/actymath/table_data/a1967-70_exam.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.2/actymath/table_data/amc00.csv` & `actymath-0.1.3/actymath/table_data/amc00.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.2/actymath/table_data/test.csv` & `actymath-0.1.3/actymath/table_data/test.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.2/actymath/tables.py` & `actymath-0.1.3/actymath/tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import csv
 import os
 from abc import ABC, abstractmethod
 
+from actymath.exceptions import MortalityTableError
+
 DATA_PATH = os.path.dirname(__file__) + "/table_data"
 
 
 def convert_lx_to_qx(lx_list: list):
     """ Converts a list of lx values to a qx list. """
     q_values = []
     for i, l in enumerate(lx_list[:-1]):
         q_values.append(1 - lx_list[i + 1] / l)
     return q_values
 
 
-class MortalityTableError(Exception):
-    pass
+
 
 
 class MortalityTable(ABC):
     """ Abstract mortality table """
 
     def __init__(self):
         self.data = []
@@ -131,82 +132,141 @@
 
 class CSVMortalityTable(MortalityTable):
     """
     Loads a mortality table from CSV file
     Two dimensional tables are loaded into multiple columns.
     Specify table data type as 'qx' or 'lx'.
     Constructor will build lx, dx and qx data when it loads.
+
+    Set age_column to the name of the column where age sits.
+    Set value_columns to the name of the value columns in the order to be read.
     """
 
-    path = DATA_PATH
-    filename = None
+    path = None  # Path of the CSV file
+    filename = None  # Name of the CSV file
     age_column = ""  # The name of the column where age sits
-    table_type = "qx"  # data is either 'qx' or 'lx'
+    table_type = None  # data is either 'qx' or 'lx'
     value_columns = []  # The name of the value columns in the order to be read
 
     def __init__(self, filename=None, path=None):
         super().__init__()
         if path is not None:
             self.path = path
         if filename is not None:
             self.filename = filename
 
+        if self.path is None or self.filename is None:
+            raise MortalityTableError("Path and filename must be specified")
+        
+        if not self.age_column:
+            raise MortalityTableError("Age column name must be specified")
+
+        if not self.value_columns:
+            raise MortalityTableError("Value column names must be specified")
+        
+        if self.table_type not in ["qx", "lx"]:
+            raise MortalityTableError("Table type must be 'qx' or 'lx'")
+
         with open(f"{self.path}/{self.filename}") as f:
             reader = csv.DictReader(f)
             for i, row in enumerate(reader):
                 self.age_index[float(row[self.age_column])] = i
                 self.data.append(
                     [float(row[x]) if row[x] else None for x in self.value_columns]
                 )
 
         self.ultimate_col = len(self.value_columns) - 1  # Index for last column
 
+class PandasMortalityTable(MortalityTable):
+    """
+    Creates a mortality table from a pandas dataframe.
+    Two dimensional tables are to be across multiple columns.
+    Specify table data type as 'qx' or 'lx'.
+    Constructor will build lx, dx and qx data when it loads.
+
+    Set age_column to the name of the column where age sits.
+    Set value_columns to the name of the value columns in the order to be read.
+    """
+
+    df = None # The pandas dataframe containing mortality data
+    age_column = ""  # The name of the column where age sits
+    table_type = None  # data is either 'qx' or 'lx'
+    value_columns = []  # The name of the value columns in the order to be read
+
+
+    def __init__(self, df=None):
+        super().__init__()
+        if df is not None:
+            self.df = df
+        
+        if not self.age_column:
+            raise MortalityTableError("Age column name must be specified")
+
+        if not self.value_columns:
+            raise MortalityTableError("Value column names must be specified")
+        
+        if self.table_type not in ["qx", "lx"]:
+            raise MortalityTableError("Table type must be 'qx' or 'lx'")
+
+        self.data = df[self.value_columns].values.tolist()
+
+        self.age_index = {age: i for i, age in df[self.age_column].to_dict().items()}
+
+        self.ultimate_col = len(self.value_columns) - 1  # Index for last column
+
+
+"""Example tables"""
 
 class TestTable(OneDimensionTableMixIn, CSVMortalityTable):
     """ A test mortality table. """
 
+    path = DATA_PATH
     filename = "test.csv"
     age_column = "Age x"
     table_type = "qx"
     value_columns = ["q x"]
 
 
 class TestTable2(OneDimensionTableMixIn, CSVMortalityTable):
     """ A test mortality table using lx. """
 
+    path = DATA_PATH
     filename = "test_lx.csv"
     age_column = "Age x"
     table_type = "lx"
     value_columns = ["l x"]
 
 
 class AMC00(TwoDimensionDiagonalTableMixIn, CSVMortalityTable):
     """UK AMC00 mortality table.
     https://www.actuaries.org.uk/learn-and-develop/continuous-mortality-investigation/cmi-mortality-and-morbidity-tables/00-series-tables
     """
 
+    path = DATA_PATH
     filename = "amc00.csv"
     age_column = "Age x"
     table_type = "qx"
     value_columns = ["Duration 0", "Duration 1", "Durations 2+"]
 
 
 class A1967_70_Exams(TwoDimensionHorizontalTableMixIn, CSVMortalityTable):
     """UK A1967-70 mortality table used in actuarial examinations.
     https://www.actuaries.org.uk/learn-and-develop/continuous-mortality-investigation/cmi-mortality-and-morbidity-tables/mortality-rates-older-mortality-tables
     """
 
+    path = DATA_PATH
     filename = "a1967-70_exam.csv"
     age_column = "x"
     table_type = "lx"
     value_columns = ["l[x]", "l([x]+1)", "l(x+2)"]
 
 
 class A1967_70(TwoDimensionDiagonalTableMixIn, CSVMortalityTable):
     """UK A1967-70 mortality table provided by the CMI usese Qx in diagonal select pattern.
     https://www.actuaries.org.uk/learn-and-develop/continuous-mortality-investigation/cmi-mortality-and-morbidity-tables/mortality-rates-older-mortality-tables
     """
 
+    path = DATA_PATH
     filename = "a1967-70.csv"
     age_column = "Age x"
     table_type = "qx"
     value_columns = ["Duration 0", "Duration 1", "Durations 2+"]
```

### Comparing `actymath-0.1.2/pyproject.toml` & `actymath-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "actymath"
-version = "0.1.2"
+version = "0.1.3"
 description = "Actuarial Math and commutation functions for life insurance product - with a Pandas backend"
 authors = ["Matt Gosden <mdgosden@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 homepage = "https://github.com/ttamg/actymath"
 repository = "https://github.com/ttamg/actymath"
 exclude = ["notebooks"]
@@ -19,11 +19,12 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 pylint = "^2.17.2"
 black = "^23.3.0"
 pytest-randomly = "^3.12.0"
 jupyter = "^1.0.0"
 ipykernel = "^6.22.0"
+toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `actymath-0.1.2/PKG-INFO` & `actymath-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actymath
-Version: 0.1.2
+Version: 0.1.3
 Summary: Actuarial Math and commutation functions for life insurance product - with a Pandas backend
 Home-page: https://github.com/ttamg/actymath
 License: MIT
 Keywords: actuarial,pandas,insurance
 Author: Matt Gosden
 Author-email: mdgosden@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -53,14 +53,16 @@
 
 These formulae can be explored in the [actymath/columns directory](https://github.com/ttamg/actymath/tree/main/actymath/columns).
 
 ### Mortality tables
 
 Currently only a few old standard mortality tables are implemented, but there is support for 1D and 2D mortality tables [here](https://github.com/ttamg/actymath/blob/main/actymath/tables.py).
 
+New 1D and 2D mortality tables can be loaded in from CSV or pandas DataFrames.
+
 ## Contributing
 
 Feel free to contribute or suggest improvements.
 
 - Add suggested improvements as a GitHub issue on this project
 
 - Pull requests also welcomed, particularly for any fixes, new tables or useful actuarial formulae
```

