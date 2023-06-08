# Comparing `tmp/numerous-solver-2.2.2.tar.gz` & `tmp/numerous-solver-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerous-solver-2.2.2.tar", last modified: Wed Feb  8 11:06:52 2023, max compression
+gzip compressed data, was "numerous-solver-2.2.3.tar", last modified: Thu Jun  8 13:28:03 2023, max compression
```

## Comparing `numerous-solver-2.2.2.tar` & `numerous-solver-2.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.778123 numerous-solver-2.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-01-30 13:12:22.000000 numerous-solver-2.2.2/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-10-25 15:22:05.000000 numerous-solver-2.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2177 2023-02-08 11:06:52.778123 numerous-solver-2.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1734 2022-10-27 09:14:20.000000 numerous-solver-2.2.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-08 11:06:52.778123 numerous-solver-2.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-02-06 09:03:37.000000 numerous-solver-2.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.750123 numerous-solver-2.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.746123 numerous-solver-2.2.2/src/numerous/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.766123 numerous-solver-2.2.2/src/numerous/solver/
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-01-23 16:08:47.000000 numerous-solver-2.2.2/src/numerous/solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9332 2023-01-27 11:41:15.000000 numerous-solver-2.2.2/src/numerous/solver/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2023-01-20 16:04:52.000000 numerous-solver-2.2.2/src/numerous/solver/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11447 2023-02-06 22:17:03.000000 numerous-solver-2.2.2/src/numerous/solver/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.766123 numerous-solver-2.2.2/src/numerous/solver/examples/
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-10-25 15:22:05.000000 numerous-solver-2.2.2/src/numerous/solver/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.770123 numerous-solver-2.2.2/src/numerous/solver/examples/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-08 11:06:21.000000 numerous-solver-2.2.2/src/numerous/solver/examples/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11635 2023-01-31 10:00:04.000000 numerous-solver-2.2.2/src/numerous/solver/examples/models/discrete_events.py
--rw-rw-rw-   0 root         (0) root         (0)     5931 2023-02-08 10:09:51.000000 numerous-solver-2.2.2/src/numerous/solver/examples/models/events_with_external_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     4760 2023-01-24 14:01:24.000000 numerous-solver-2.2.2/src/numerous/solver/examples/models/model_without_derivatives.py
--rw-rw-rw-   0 root         (0) root         (0)     4589 2023-01-23 16:08:47.000000 numerous-solver-2.2.2/src/numerous/solver/examples/models/simple_differential_equation.py
--rw-rw-rw-   0 root         (0) root         (0)     5138 2023-01-24 14:01:24.000000 numerous-solver-2.2.2/src/numerous/solver/examples/models/system_of_equations.py
--rw-rw-rw-   0 root         (0) root         (0)    18914 2023-01-31 10:00:04.000000 numerous-solver-2.2.2/src/numerous/solver/examples/models/time_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-01-24 14:01:24.000000 numerous-solver-2.2.2/src/numerous/solver/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)    10651 2023-02-06 23:51:56.000000 numerous-solver-2.2.2/src/numerous/solver/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.770123 numerous-solver-2.2.2/src/numerous/solver/linalg/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-08 11:06:21.000000 numerous-solver-2.2.2/src/numerous/solver/linalg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.774123 numerous-solver-2.2.2/src/numerous/solver/linalg/lapack/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-08 11:06:21.000000 numerous-solver-2.2.2/src/numerous/solver/linalg/lapack/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2022-10-25 15:22:05.000000 numerous-solver-2.2.2/src/numerous/solver/linalg/lapack/lapack_python.py
--rw-rw-rw-   0 root         (0) root         (0)     4902 2023-01-30 22:51:21.000000 numerous-solver-2.2.2/src/numerous/solver/models.py
--rw-rw-rw-   0 root         (0) root         (0)    24133 2023-02-06 15:06:35.000000 numerous-solver-2.2.2/src/numerous/solver/numerous_solver.py
--rw-rw-rw-   0 root         (0) root         (0)     2004 2023-01-20 13:59:47.000000 numerous-solver-2.2.2/src/numerous/solver/solve_states.py
--rw-rw-rw-   0 root         (0) root         (0)    19268 2023-01-26 20:11:45.000000 numerous-solver-2.2.2/src/numerous/solver/solver_methods.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 11:06:52.774123 numerous-solver-2.2.2/src/numerous_solver.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2177 2023-02-08 11:06:52.000000 numerous-solver-2.2.2/src/numerous_solver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1189 2023-02-08 11:06:52.000000 numerous-solver-2.2.2/src/numerous_solver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 11:06:52.000000 numerous-solver-2.2.2/src/numerous_solver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-08 11:06:52.000000 numerous-solver-2.2.2/src/numerous_solver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-08 11:06:52.000000 numerous-solver-2.2.2/src/numerous_solver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-02-08 11:06:24.000000 numerous-solver-2.2.2/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.039925 numerous-solver-2.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-06-08 13:28:03.039925 numerous-solver-2.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 13:28:03.039925 numerous-solver-2.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.031926 numerous-solver-2.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.031926 numerous-solver-2.2.3/src/numerous/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.035925 numerous-solver-2.2.3/src/numerous/solver/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9470 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11447 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.035925 numerous-solver-2.2.3/src/numerous/solver/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.039925 numerous-solver-2.2.3/src/numerous/solver/examples/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11635 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/models/discrete_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     5931 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/models/events_with_external_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4760 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/models/model_without_derivatives.py
+-rw-rw-rw-   0 root         (0) root         (0)     4589 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/models/simple_differential_equation.py
+-rw-rw-rw-   0 root         (0) root         (0)     5138 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/models/system_of_equations.py
+-rw-rw-rw-   0 root         (0) root         (0)    18914 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/examples/models/time_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10651 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.039925 numerous-solver-2.2.3/src/numerous/solver/linalg/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/linalg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.039925 numerous-solver-2.2.3/src/numerous/solver/linalg/lapack/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/linalg/lapack/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/linalg/lapack/lapack_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     4902 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    24133 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/numerous_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2004 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/solve_states.py
+-rw-rw-rw-   0 root         (0) root         (0)    19268 2023-05-17 13:10:25.000000 numerous-solver-2.2.3/src/numerous/solver/solver_methods.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:28:03.039925 numerous-solver-2.2.3/src/numerous_solver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-06-08 13:28:02.000000 numerous-solver-2.2.3/src/numerous_solver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-08 13:28:03.000000 numerous-solver-2.2.3/src/numerous_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:28:02.000000 numerous-solver-2.2.3/src/numerous_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-08 13:28:02.000000 numerous-solver-2.2.3/src/numerous_solver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-08 13:28:02.000000 numerous-solver-2.2.3/src/numerous_solver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-08 13:27:54.000000 numerous-solver-2.2.3/version.txt
```

### Comparing `numerous-solver-2.2.2/LICENSE.txt` & `numerous-solver-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/PKG-INFO` & `numerous-solver-2.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous-solver
-Version: 2.2.2
+Version: 2.2.3
 Summary: Numerous ODE solver
 Home-page: 
 Author: Tobias Dokkedal Elmoee, EnergyMachines ApS
 Author-email: tobias.dokkedal.elmoe@energymachines.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `numerous-solver-2.2.2/README.md` & `numerous-solver-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/setup.py` & `numerous-solver-2.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/base.py` & `numerous-solver-2.2.3/src/numerous/solver/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,51 +10,57 @@
 class _Jitter(object):
     """
     The base class used for jitting models
     """
     _reserved: None
     _assignments: None
     _compiled_model: None
+
     def _jit(self, jit=False):
 
         python_model = self
 
         if not jit:
             object.__setattr__(self, '_compiled_model', python_model)
             return python_model
 
-        if hasattr(self,'_compiled_model'):
+        if hasattr(self, '_compiled_model'):
             return self._compiled_model
 
         spec = []
 
         args = self._add_args(self._reserved['args'], jit=True)
         kwargs = self._add_kwargs(self._reserved["kwargs"], jit=True)
 
         spec_dict = {}
-        for k,v in python_model.__dict__.items():
+        for k, v in python_model.__dict__.items():
             if k in {'_reserved', '_interface_factory', '_time_events', '_assignments', '_initialized', '_interface'}:
                 continue
             spec_dict.update(self._add_kwargs({k: v}, jit=jit))
 
-        for k,v in spec_dict.items():
+        for k, v in spec_dict.items():
             nbtype = nb.typeof(v)
             if type(nbtype) == nb.types.Array:  # Array must be type 'A' -
                 # by default the nb.typeof evaluates them to type 'C'
                 spec.append((k, nb.types.Array(nbtype.dtype, nbtype.ndim, 'A')))
             else:
                 spec.append((k, nbtype))
 
+        class OuterWrapper(type(python_model)):
+            pass
+
+        OuterWrapper.__setattr__ = object.__setattr__
+
         @jitclass(spec=spec)
-        class Wrapper(type(self)):
+        class Wrapper(OuterWrapper):
             pass
 
         object.__setattr__(self, '_compiled_model', Wrapper(*args, **kwargs))
         if hasattr(self, '_assignments'):
-            for k,v in self._assignments.items():
+            for k, v in self._assignments.items():
                 setattr(self, k, v)
         return self._compiled_model
 
     def _add_args(self, args_: iter, jit=False):
         args__ = []
         for arg in args_:
             if not self._is_reserved_nested_type(arg):
@@ -75,15 +81,15 @@
                         args__.append(arg)
             else:
                 args__.append(arg)
         return tuple(args__)
 
     def _add_kwargs(self, kwargs_: dict, jit=False):
         kwargs__ = {}
-        for k,v in kwargs_.items():
+        for k, v in kwargs_.items():
             if not self._is_reserved_nested_type(v):
                 try:
                     _ = iter(v)
                     if isinstance(v, dict):
                         if jit:
                             raise TypeError(f"dicts are not allowed as arguments when jit=True {v}")
                         kwargs__.update({k: self._add_kwargs(v, jit)})
@@ -145,77 +151,87 @@
 
     def create_class(self, *args, **kwargs) -> object:
         raise NotImplementedError
 
     def post_create_class(self, new_class: object):
         object.__setattr__(new_class, '_initialized', True)
 
+
 class DefaultFactory(_Factory):
     def create_class(self, *args, **kwargs):
         new_class = self.class_type(*args, **kwargs)
         object.__setattr__(new_class, '_reserved', {'args': args, 'kwargs': kwargs})
         return new_class
 
+
 def model(model_class: type):
     """
     Decorator for model classes. Contains the ModelFactory, which creates the model object and its interface.
     Sets the interface_factory
     :param model_class: the :class:`~solver.model.Model` to decorate
     :return: returns the :class:`~solver.decorators.model.ModelFactory`
     """
+
     class ModelFactory(_Factory):
         interface_factory: type = None
         class_type = model_class
+
         def create_class(self, *args, **kwargs):
             new_class = self.class_type(*args, **kwargs)
             new_class._reserved = {'args': args, 'kwargs': kwargs}
             new_class._interface_factory = self.interface_factory
             return new_class
 
     return ModelFactory()
 
+
 def interface(interface_class: type):
     """
     Decorator of interfaces. Contains the InterfaceFactory which creates the interface. Sets the interface_factory
     property on the ModelFactory, using the annotation 'model' on the :class:`~solver.interface.Interface`.
     :param interface_class: the :class:`~solver.interface.Interface` to decorate
     :return: returns the :class:`~solver.decorators.interface.InterfaceFactory`
     """
     model_factory = interface_class.__annotations__.get('model')
     if not model_factory:
         raise AttributeError(f"No model property specified for interface {interface_class}")
     if not issubclass(type(interface_class.__annotations__['model']), _Factory):
         raise AttributeError(f"model {model_factory} must be a Factory type")
+
     class InterfaceFactory(DefaultFactory):
         class_type = interface_class
 
     model_factory.interface_factory = InterfaceFactory()
     return model_factory.interface_factory
 
+
 def event(event_class):
     """
     Decorator of events. Contains the EventFactory, which creates the events.
     :param event_class: the :class:`~solver.interface.Event` to decorate
     :return: returns the :class:`~solver.decorators.event.EventFactory`
     """
+
     class EventFactory(DefaultFactory):
         class_type = event_class
 
     return EventFactory()
 
 
 def component(component_class):
     class ComponentFactory(DefaultFactory):
         class_type = component_class
+
     return ComponentFactory()
 
 
 class Solution:
     """Default class which holds the solution in arrays.
     """
+
     def __init__(self):
         self.results = []
         self.state_event_results = []
         self.time_event_results = []
 
     def add_result(self, t, states):
         """
@@ -250,8 +266,7 @@
             decides by specifying in the :class:`~solver.interface.EventHandler`.
         :return:
         """
         self.time_event_results.append(np.append(t_event, states))
 
     def reset(self):
         self.__init__()
-
```

### Comparing `numerous-solver-2.2.2/src/numerous/solver/common.py` & `numerous-solver-2.2.3/src/numerous/solver/common.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/events.py` & `numerous-solver-2.2.3/src/numerous/solver/events.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/examples/models/discrete_events.py` & `numerous-solver-2.2.3/src/numerous/solver/examples/models/discrete_events.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/examples/models/events_with_external_functions.py` & `numerous-solver-2.2.3/src/numerous/solver/examples/models/events_with_external_functions.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/examples/models/model_without_derivatives.py` & `numerous-solver-2.2.3/src/numerous/solver/examples/models/model_without_derivatives.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/examples/models/simple_differential_equation.py` & `numerous-solver-2.2.3/src/numerous/solver/examples/models/simple_differential_equation.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/examples/models/system_of_equations.py` & `numerous-solver-2.2.3/src/numerous/solver/examples/models/system_of_equations.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/examples/models/time_events.py` & `numerous-solver-2.2.3/src/numerous/solver/examples/models/time_events.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/handlers.py` & `numerous-solver-2.2.3/src/numerous/solver/handlers.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/interface.py` & `numerous-solver-2.2.3/src/numerous/solver/interface.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/linalg/lapack/lapack_python.py` & `numerous-solver-2.2.3/src/numerous/solver/linalg/lapack/lapack_python.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/models.py` & `numerous-solver-2.2.3/src/numerous/solver/models.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/numerous_solver.py` & `numerous-solver-2.2.3/src/numerous/solver/numerous_solver.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/solve_states.py` & `numerous-solver-2.2.3/src/numerous/solver/solve_states.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous/solver/solver_methods.py` & `numerous-solver-2.2.3/src/numerous/solver/solver_methods.py`

 * *Files identical despite different names*

### Comparing `numerous-solver-2.2.2/src/numerous_solver.egg-info/PKG-INFO` & `numerous-solver-2.2.3/src/numerous_solver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerous-solver
-Version: 2.2.2
+Version: 2.2.3
 Summary: Numerous ODE solver
 Home-page: 
 Author: Tobias Dokkedal Elmoee, EnergyMachines ApS
 Author-email: tobias.dokkedal.elmoe@energymachines.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `numerous-solver-2.2.2/src/numerous_solver.egg-info/SOURCES.txt` & `numerous-solver-2.2.3/src/numerous_solver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

