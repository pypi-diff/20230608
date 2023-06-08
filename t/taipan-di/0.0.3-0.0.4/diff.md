# Comparing `tmp/taipan_di-0.0.3.tar.gz` & `tmp/taipan_di-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipan_di-0.0.3.tar", max compression
+gzip compressed data, was "taipan_di-0.0.4.tar", max compression
```

## Comparing `taipan_di-0.0.3.tar` & `taipan_di-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,32 @@
--rw-r--r--   0        0        0     1063 2023-06-02 10:28:17.804484 taipan_di-0.0.3/LICENSE
--rw-r--r--   0        0        0     2894 2023-06-02 10:28:17.804484 taipan_di-0.0.3/README.md
--rw-r--r--   0        0        0     1004 2023-06-02 10:28:17.804484 taipan_di-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/__init__.py
--rw-r--r--   0        0        0       21 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/__version__.py
--rw-r--r--   0        0        0       55 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/__init__.py
--rw-r--r--   0        0        0     3181 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/dependency_collection.py
--rw-r--r--   0        0        0      676 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/dependency_container.py
--rw-r--r--   0        0        0      703 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/dependency_provider.py
--rw-r--r--   0        0        0     3677 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/instanciate_service.py
--rw-r--r--   0        0        0       83 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/scopes/__init__.py
--rw-r--r--   0        0        0      474 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/scopes/factory_scope.py
--rw-r--r--   0        0        0      594 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/classes/scopes/singleton_scope.py
--rw-r--r--   0        0        0      204 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/__init__.py
--rw-r--r--   0        0        0       38 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_error.py
--rw-r--r--   0        0        0      105 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_injection_error.py
--rw-r--r--   0        0        0      100 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_type_error.py
--rw-r--r--   0        0        0      108 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/errors/taipan_unregistered_error.py
--rw-r--r--   0        0        0      157 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/__init__.py
--rw-r--r--   0        0        0      938 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/base_dependency_container.py
--rw-r--r--   0        0        0     1029 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/base_dependency_provider.py
--rw-r--r--   0        0        0      519 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/interfaces/base_scope.py
--rw-r--r--   0        0        0        0 2023-06-02 10:28:17.804484 taipan_di-0.0.3/taipan_di/py.typed
--rw-r--r--   0        0        0     3816 1970-01-01 00:00:00.000000 taipan_di-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-08 10:19:39.479355 taipan_di-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2988 2023-06-08 10:19:39.479355 taipan_di-0.0.4/README.md
+-rw-r--r--   0        0        0     1004 2023-06-08 10:19:39.479355 taipan_di-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/__init__.py
+-rw-r--r--   0        0        0       21 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/__version__.py
+-rw-r--r--   0        0        0      115 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/__init__.py
+-rw-r--r--   0        0        0     4296 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/dependency_collection.py
+-rw-r--r--   0        0        0      676 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/dependency_container.py
+-rw-r--r--   0        0        0      702 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/dependency_provider.py
+-rw-r--r--   0        0        0     3696 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/instanciate_service.py
+-rw-r--r--   0        0        0       83 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/scopes/__init__.py
+-rw-r--r--   0        0        0      474 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/scopes/factory_scope.py
+-rw-r--r--   0        0        0      594 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/scopes/singleton_scope.py
+-rw-r--r--   0        0        0      364 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/__init__.py
+-rw-r--r--   0        0        0      872 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_factory.py
+-rw-r--r--   0        0        0      538 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_link.py
+-rw-r--r--   0        0        0     1902 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/chain_of_responsibility_registrator.py
+-rw-r--r--   0        0        0      780 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/pipeline_factory.py
+-rw-r--r--   0        0        0      652 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/pipeline_link.py
+-rw-r--r--   0        0        0     1740 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/classes/tools/pipeline_registrator.py
+-rw-r--r--   0        0        0      267 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_error.py
+-rw-r--r--   0        0        0      105 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_injection_error.py
+-rw-r--r--   0        0        0      108 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_registration_error.py
+-rw-r--r--   0        0        0      100 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_type_error.py
+-rw-r--r--   0        0        0      108 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/errors/taipan_unregistered_error.py
+-rw-r--r--   0        0        0      157 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/__init__.py
+-rw-r--r--   0        0        0      938 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/base_dependency_container.py
+-rw-r--r--   0        0        0     1029 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/base_dependency_provider.py
+-rw-r--r--   0        0        0      519 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/interfaces/base_scope.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:19:39.479355 taipan_di-0.0.4/taipan_di/py.typed
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 taipan_di-0.0.4/PKG-INFO
```

### Comparing `taipan_di-0.0.3/LICENSE` & `taipan_di-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.3/README.md` & `taipan_di-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 ## Features
 
  - Lightweight
  - No decorators
  - No hidden behaviour (what you write is what you get)
  - Automatic dependency injection on service resolving
- - Type-checking
+ - Type hinting
  - No global container by default
  - Singleton and factory scopes
+ - Register pipelines and chains of responsibility easily
 
 
 ## Constraints
 
  - Based purely on types (not on strings)
  - No automatic registration
  - It is necessary to write an `__init__` function or use `@dataclass`
@@ -49,32 +50,33 @@
 
 You can also provide a creator method or an instance (for singletons only) that will be used when resolving the services :
 
  - `services.register_factory_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_instance(Type, instance)`
 
+You can also register chains of responsibility and pipelines. Examples are given in the test files.
+
 Once your services are registered, you have to build a dependency provider which will be used to resolve services : 
 
 > `provider = services.build()`<br/>
 > `resolved = provider.resolve(InterfaceType)`
 
 If `ImplementationType` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `DependencyCollection`.
 
 
 ## Inspirations
 
-This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on a project previously but it didn't fit all my requirements.
+This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on another project previously but it didn't fit all my requirements.
 
 I also took inspiration from the [*injector*](https://pypi.org/project/injector/) library and .Net's dependency injection system.
 
 
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
- - Register singletons and factories without specifying the interface
  - Create configuration from environment or configuration files
```

### Comparing `taipan_di-0.0.3/pyproject.toml` & `taipan_di-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Taipan-DI"
-version = "0.0.3"
+version = "0.0.4"
 description = "Truly Amazing Inversion of control Python library Analogous to .Net's DI"
 authors = ["Billuc <billuc@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 keywords = ["taipan", "dependency injection", "dependency", "python"]
```

### Comparing `taipan_di-0.0.3/taipan_di/classes/dependency_container.py` & `taipan_di-0.0.4/taipan_di/classes/dependency_container.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.3/taipan_di/classes/instanciate_service.py` & `taipan_di-0.0.4/taipan_di/classes/instanciate_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         resolved_kwargs = _resolve_function_kwargs(parameters_name, parameters, provider)
 
         if len(resolved_kwargs) < len(parameters_name):
             missing_parameters = [
                 arg for arg in parameters_name if arg not in resolved_kwargs
             ]
             raise TaipanInjectionError(
-                "Cannot execute function without required parameters. "
+                f"Cannot instanciate service {str(service)} without required parameters. "
                 + f"Did you forget to bind the following parameters: `{'`, `'.join(missing_parameters)}`?"
             )
 
         return resolved_kwargs
 
     all_kwargs = _resolve_kwargs()
     instance = service(**all_kwargs)
```

### Comparing `taipan_di-0.0.3/taipan_di/classes/scopes/singleton_scope.py` & `taipan_di-0.0.4/taipan_di/classes/scopes/singleton_scope.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.3/taipan_di/interfaces/base_dependency_container.py` & `taipan_di-0.0.4/taipan_di/interfaces/base_dependency_container.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.3/taipan_di/interfaces/base_dependency_provider.py` & `taipan_di-0.0.4/taipan_di/interfaces/base_dependency_provider.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.3/taipan_di/interfaces/base_scope.py` & `taipan_di-0.0.4/taipan_di/interfaces/base_scope.py`

 * *Files identical despite different names*

### Comparing `taipan_di-0.0.3/PKG-INFO` & `taipan_di-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipan-di
-Version: 0.0.3
+Version: 0.0.4
 Summary: Truly Amazing Inversion of control Python library Analogous to .Net's DI
 Home-page: https://github.com/Billuc/Taipan-DI
 License: MIT
 Keywords: taipan,dependency injection,dependency,python
 Author: Billuc
 Author-email: billuc@hotmail.fr
 Requires-Python: >=3.9,<4.0
@@ -29,17 +29,18 @@
 
 ## Features
 
  - Lightweight
  - No decorators
  - No hidden behaviour (what you write is what you get)
  - Automatic dependency injection on service resolving
- - Type-checking
+ - Type hinting
  - No global container by default
  - Singleton and factory scopes
+ - Register pipelines and chains of responsibility easily
 
 
 ## Constraints
 
  - Based purely on types (not on strings)
  - No automatic registration
  - It is necessary to write an `__init__` function or use `@dataclass`
@@ -71,33 +72,34 @@
 
 You can also provide a creator method or an instance (for singletons only) that will be used when resolving the services :
 
  - `services.register_factory_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_creator(Type, lambda provider: create(provider))`
  - `services.register_singleton_instance(Type, instance)`
 
+You can also register chains of responsibility and pipelines. Examples are given in the test files.
+
 Once your services are registered, you have to build a dependency provider which will be used to resolve services : 
 
 > `provider = services.build()`<br/>
 > `resolved = provider.resolve(InterfaceType)`
 
 If `ImplementationType` has a constructor dependency, it will be automatically resolved, as long as the dependency has been registered in the `DependencyCollection`.
 
 
 ## Inspirations
 
-This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on a project previously but it didn't fit all my requirements.
+This library is partially based on the [*kink*](https://pypi.org/project/kink/) dependency injection library. I was using kink on another project previously but it didn't fit all my requirements.
 
 I also took inspiration from the [*injector*](https://pypi.org/project/injector/) library and .Net's dependency injection system.
 
 
 ## TODO
 
 This library isn't stable yet and a lot of things can still be improved.
 If there is something you want to see added or if something does not work as you want it to, feel free to open an issue.
 
 Here is a list of features I have in mind and will be working on :
 
- - Register singletons and factories without specifying the interface
  - Create configuration from environment or configuration files
```

