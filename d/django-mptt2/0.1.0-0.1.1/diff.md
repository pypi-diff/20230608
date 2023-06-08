# Comparing `tmp/django-mptt2-0.1.0.tar.gz` & `tmp/django-mptt2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mptt2-0.1.0.tar", last modified: Sat Apr 29 17:59:36 2023, max compression
+gzip compressed data, was "django-mptt2-0.1.1.tar", last modified: Thu Jun  8 07:09:44 2023, max compression
```

## Comparing `django-mptt2-0.1.0.tar` & `django-mptt2-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:59:36.697808 django-mptt2-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-29 17:59:36.697808 django-mptt2-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:59:36.697808 django-mptt2-0.1.0/django_mptt2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/django_mptt2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/django_mptt2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/django_mptt2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/django_mptt2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/django_mptt2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:59:36.697808 django-mptt2-0.1.0/mptt2/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:59:36.697808 django-mptt2-0.1.0/mptt2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/mptt2/query.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 17:59:36.697808 django-mptt2-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-29 17:59:36.000000 django-mptt2-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/django_mptt2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/django_mptt2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/mptt2/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/mptt2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/mptt2/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:09:44.446549 django-mptt2-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-08 07:09:44.000000 django-mptt2-0.1.1/setup.py
```

### Comparing `django-mptt2-0.1.0/LICENSE` & `django-mptt2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mptt2-0.1.0/PKG-INFO` & `django-mptt2-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mptt2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utilities for implementing a modified pre-order traversal tree (nested sets) in django.
 Home-page: https://github.com/jokiefer/django-mptt2
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,17 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/django-mptt2/badge/?version=latest
     :target: https://django-mptt2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+.. image:: https://badge.fury.io/py/django-mptt2.svg
+    :target: https://pypi.org/project/django-mptt2/
+    :alt: PyPi version
 
 django-mptt2
 ============
 Based on the idea of the unmaintained `django-mptt <https://github.com/django-mptt/django-mptt>`_ package i implemented this new code base to replace it.
 
 Cause no other package fits all of my use cases, which are primary in fast reading tree's from the database, i started working on this project.
```

### Comparing `django-mptt2-0.1.0/README.rst` & `django-mptt2-0.1.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 .. image:: https://readthedocs.org/projects/django-mptt2/badge/?version=latest
     :target: https://django-mptt2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+.. image:: https://badge.fury.io/py/django-mptt2.svg
+    :target: https://pypi.org/project/django-mptt2/
+    :alt: PyPi version
 
 django-mptt2
 ============
 Based on the idea of the unmaintained `django-mptt <https://github.com/django-mptt/django-mptt>`_ package i implemented this new code base to replace it.
 
 Cause no other package fits all of my use cases, which are primary in fast reading tree's from the database, i started working on this project.
```

### Comparing `django-mptt2-0.1.0/django_mptt2.egg-info/PKG-INFO` & `django-mptt2-0.1.1/django_mptt2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mptt2
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utilities for implementing a modified pre-order traversal tree (nested sets) in django.
 Home-page: https://github.com/jokiefer/django-mptt2
 Author: Jonas Kiefer
 Author-email: jonas.kiefer@live.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,17 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/django-mptt2/badge/?version=latest
     :target: https://django-mptt2.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
+.. image:: https://badge.fury.io/py/django-mptt2.svg
+    :target: https://pypi.org/project/django-mptt2/
+    :alt: PyPi version
 
 django-mptt2
 ============
 Based on the idea of the unmaintained `django-mptt <https://github.com/django-mptt/django-mptt>`_ package i implemented this new code base to replace it.
 
 Cause no other package fits all of my use cases, which are primary in fast reading tree's from the database, i started working on this project.
```

### Comparing `django-mptt2-0.1.0/mptt2/expressions.py` & `django-mptt2-0.1.1/mptt2/expressions.py`

 * *Files identical despite different names*

### Comparing `django-mptt2-0.1.0/mptt2/managers.py` & `django-mptt2-0.1.1/mptt2/managers.py`

 * *Files identical despite different names*

### Comparing `django-mptt2-0.1.0/mptt2/models.py` & `django-mptt2-0.1.1/mptt2/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,91 +116,91 @@
     def get_children(self, asc=False) -> QuerySet:
         """returns a queryset representing the children of the current node
 
         :param asc: switch to sort the queryset ascending
         :type asc: bool
 
         """
-        children = self.objects.filter(ChildrenQuery(of=self))
+        children = self.__class__.objects.filter(ChildrenQuery(of=self))
         return children.order_by("-mptt_lft") if asc else children
 
     def get_descendants(self, include_self=False, asc=False) -> QuerySet:
         """returns a queryset representing the descendants of the current node
 
         :param asc: switch to include the current node with the queryset
         :type asc: bool
 
         :param asc: switch to sort the queryset ascending
         :type asc: bool
 
         """
-        descendants = self.objects.filter(
+        descendants = self.__class__.objects.filter(
             DescendantsQuery(of=self, include_self=include_self))
         return descendants.order_by("-mptt_lft") if asc else descendants
 
     def get_ancestors(self, include_self=False, asc=False) -> QuerySet:
         """returns a queryset representing the ancestors of the current node
 
         :param asc: switch to include the current node with the queryset
         :type asc: bool
 
         :param asc: switch to sort the queryset ascending
         :type asc: bool
 
         """
-        ancestors = self.objects.filter(
+        ancestors = self.__class__.objects.filter(
             AncestorsQuery(of=self, include_self=include_self))
         return ancestors.order_by("-mptt_lft") if asc else ancestors
 
     def get_family(self, include_self=False, asc=False) -> QuerySet:
         """returns a queryset representing the family of the current node (descendants and ancestors)
 
         :param asc: switch to include the current node with the queryset
         :type asc: bool
 
         :param asc: switch to sort the queryset ascending
         :type asc: bool
 
         """
-        family = self.objects.filter(FamilyQuery(
+        family = self.__class__.objects.filter(FamilyQuery(
             of=self, include_self=include_self))
         return family.order_by("-mptt_lft") if asc else family
 
     def get_siblings(self, include_self=False, asc=False) -> QuerySet:
         """returns a queryset representing siblings of the current node
 
         :param asc: switch to include the current node with the queryset
         :type asc: bool
 
         :param asc: switch to sort the queryset ascending
         :type asc: bool
 
         """
-        siblings = self.objects.filter(
+        siblings = self.__class__.objects.filter(
             SiblingsQuery(of=self, include_self=include_self))
         return siblings.order_by("-mptt_lft") if asc else siblings
 
     def get_root(self):
         """returns the root node of the tree where this node is part of"""
-        return self.objects.get(RootQuery(of=self))
+        return self.__class__.objects.get(RootQuery(of=self))
 
     def move_to(self, target, position: Position = Position.LAST_CHILD):
         """Tree function to move a node relative to a given target by the given position
 
         :param target: The target node where the given node shall be inserted relative to.
         :type target: :class:`mptt2.models.Node`
 
         :param position: The relative position to the target
                          (Default: ``Position.LAST_CHILD``)
         :type position: :class:`mptt2.enums.Position`, optional
 
         :returns: the inserted node it self
         :rtype: :class:`mptt2.models.Node`
         """
-        return self.objects.move_node(
+        return self.__class__.objects.move_node(
             node=self,
             target=target,
             position=position
         )
 
     def insert_at(self, target, position: Position = Position.LAST_CHILD):
         """Tree function to insert this node to a given target relative by the given position
@@ -211,15 +211,15 @@
         :param position: The relative position to the target
                          (Default: ``Position.LAST_CHILD``)
         :type target: :class:`mptt2.enums.Position`, optional
 
         :returns: the inserted node it self
         :rtype: :class:`mptt2.models.Node`
         """
-        return self.objects.insert_node(
+        return self.__class__.objects.insert_node(
             node=self,
             target=target,
             position=position
         )
 
     @ property
     def is_root_node(self) -> bool:
```

### Comparing `django-mptt2-0.1.0/mptt2/query.py` & `django-mptt2-0.1.1/mptt2/query.py`

 * *Files identical despite different names*

### Comparing `django-mptt2-0.1.0/setup.py` & `django-mptt2-0.1.1/setup.py`

 * *Files identical despite different names*

