# Comparing `tmp/labonneboite_datamodel-1.0.8.tar.gz` & `tmp/labonneboite_datamodel-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labonneboite_datamodel-1.0.8.tar", max compression
+gzip compressed data, was "labonneboite_datamodel-1.0.9.tar", max compression
```

## Comparing `labonneboite_datamodel-1.0.8.tar` & `labonneboite_datamodel-1.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      240 2023-05-11 08:12:24.109377 labonneboite_datamodel-1.0.8/labonneboite_datamodel/__init__.py
--rw-r--r--   0        0        0      697 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.8/labonneboite_datamodel/crud.py
--rw-r--r--   0        0        0     2945 2023-05-11 08:12:24.109377 labonneboite_datamodel-1.0.8/labonneboite_datamodel/job.py
--rw-r--r--   0        0        0     7718 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.8/labonneboite_datamodel/office.py
--rw-r--r--   0        0        0        0 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.8/labonneboite_datamodel/tests/__init__.py
--rw-r--r--   0        0        0     3589 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.8/labonneboite_datamodel/tests/data/test.csv
--rw-r--r--   0        0        0     1530 2023-05-11 08:12:24.109377 labonneboite_datamodel-1.0.8/labonneboite_datamodel/tests/test_job.py
--rw-r--r--   0        0        0     5612 2023-05-10 08:44:21.026783 labonneboite_datamodel-1.0.8/labonneboite_datamodel/tests/test_office.py
--rw-r--r--   0        0        0     1205 2023-05-11 08:13:18.117050 labonneboite_datamodel-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/__init__.py
+-rw-r--r--   0        0        0      697 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/base.py
+-rw-r--r--   0        0        0     2945 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/job.py
+-rw-r--r--   0        0        0     7718 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/office.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/tests/__init__.py
+-rw-r--r--   0        0        0     3589 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/tests/data/test.csv
+-rw-r--r--   0        0        0     1530 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/tests/test_job.py
+-rw-r--r--   0        0        0     5612 2023-06-08 16:42:24.105781 labonneboite_datamodel-1.0.9/labonneboite_datamodel/tests/test_office.py
+-rw-r--r--   0        0        0     1205 2023-06-08 16:43:19.497465 labonneboite_datamodel-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.0.9/PKG-INFO
```

### Comparing `labonneboite_datamodel-1.0.8/labonneboite_datamodel/crud.py` & `labonneboite_datamodel-1.0.9/labonneboite_datamodel/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlmodel import Field, SQLModel, text
 
 from datetime import datetime
 
 
-class CRUDMixin(SQLModel):
+class BaseMixin(SQLModel):
     """This table provides the base elements for all tables in database
 
     Attributes:
         date_created:
         last_modified: This field should automatically update when the line is updated
     """
     date_created: datetime = Field(
```

### Comparing `labonneboite_datamodel-1.0.8/labonneboite_datamodel/job.py` & `labonneboite_datamodel-1.0.9/labonneboite_datamodel/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sqlmodel import Field
 from typing import Optional
-from .crud import CRUDMixin
+from .base import BaseMixin
 from pydantic import validator
 
 
-class Job(CRUDMixin, table=True):
+class Job(BaseMixin, table=True):
     """This table hosts the mapping between ROME and AF to be able to make a ROME search correspond to a SIRET
 
     Attributes:
         id:
         naf:
         rome:
         domain:
@@ -77,15 +77,15 @@
             raise ValueError(error)
 
         if v[0].isdigit():
             raise ValueError(error)
         return v
 
 
-class Naf(CRUDMixin, table=True):
+class Naf(BaseMixin, table=True):
     """This table hosts the Naf labels
 
     Attributes:
         id:
         naf:
         label:
     """
```

### Comparing `labonneboite_datamodel-1.0.8/labonneboite_datamodel/office.py` & `labonneboite_datamodel-1.0.9/labonneboite_datamodel/office.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from sqlmodel import Field
 from typing import Optional
-from .crud import CRUDMixin
+from .base import BaseMixin
 from pydantic import validator
 from sqlalchemy import UniqueConstraint
 
 
 # validators
-class OfficeCommon(CRUDMixin):
+class OfficeCommon(BaseMixin):
     """This is the base model applied to all Office tables
 
     Attributes:
         id: This is the primary key for the table
         siret: This is the company SIRET number
 
     """
```

### Comparing `labonneboite_datamodel-1.0.8/labonneboite_datamodel/tests/data/test.csv` & `labonneboite_datamodel-1.0.9/labonneboite_datamodel/tests/data/test.csv`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.8/labonneboite_datamodel/tests/test_job.py` & `labonneboite_datamodel-1.0.9/labonneboite_datamodel/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.8/labonneboite_datamodel/tests/test_office.py` & `labonneboite_datamodel-1.0.9/labonneboite_datamodel/tests/test_office.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.8/pyproject.toml` & `labonneboite_datamodel-1.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labonneboite-datamodel"
-version = "1.0.8"
+version = "1.0.9"
 description = "Datamodel for labonneboite"
 authors = ["Sylvain Touret"]
 license = "MIT"
 packages = [{include = "labonneboite_datamodel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

