# Comparing `tmp/FiniteDiffX-0.0.4.tar.gz` & `tmp/FiniteDiffX-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiniteDiffX-0.0.4.tar", last modified: Wed Jun  7 05:10:59 2023, max compression
+gzip compressed data, was "FiniteDiffX-0.0.5.tar", last modified: Thu Jun  8 12:45:48 2023, max compression
```

## Comparing `FiniteDiffX-0.0.4.tar` & `FiniteDiffX-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 05:10:59.000000 FiniteDiffX-0.0.4/FiniteDiffX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/finitediffx/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/finitediffx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/finitediffx/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:59.460806 FiniteDiffX-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/tests/test_fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-06-07 05:10:43.000000 FiniteDiffX-0.0.4/tests/test_finite_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 12:45:48.000000 FiniteDiffX-0.0.5/FiniteDiffX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9581 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/finitediffx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/finitediffx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/finitediffx/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:48.216653 FiniteDiffX-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/tests/test_fgrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-06-08 12:45:38.000000 FiniteDiffX-0.0.5/tests/test_finite_diff.py
```

### Comparing `FiniteDiffX-0.0.4/FiniteDiffX.egg-info/PKG-INFO` & `FiniteDiffX-0.0.5/FiniteDiffX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FiniteDiffX
-Version: 0.0.4
+Version: 0.0.5
 Summary: Finite difference tools in JAX.
 Home-page: https://github.com/ASEM000/FiniteDiffX
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: MIT
 Keywords: python jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FiniteDiffX-0.0.4/LICENSE` & `FiniteDiffX-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.4/PKG-INFO` & `FiniteDiffX-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FiniteDiffX
-Version: 0.0.4
+Version: 0.0.5
 Summary: Finite difference tools in JAX.
 Home-page: https://github.com/ASEM000/FiniteDiffX
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: MIT
 Keywords: python jax
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FiniteDiffX-0.0.4/README.md` & `FiniteDiffX-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.4/finitediffx/__init__.py` & `FiniteDiffX-0.0.5/finitediffx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     "value_and_fgrad",
     "Offset",
     "define_fdjvp",
     "generate_finitediff_coeffs",
 )
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

### Comparing `FiniteDiffX-0.0.4/finitediffx/_src/__init__.py` & `FiniteDiffX-0.0.5/finitediffx/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.4/finitediffx/_src/fgrad.py` & `FiniteDiffX-0.0.5/finitediffx/_src/fgrad.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,39 +10,51 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import dataclasses as dc
 import functools as ft
-from typing import Callable, NamedTuple, TypeVar, Union
+from typing import Any, Callable, Sequence, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from typing_extensions import ParamSpec
 
 from finitediffx._src.utils import _generate_central_offsets, generate_finitediff_coeffs
 
+__all__ = ("fgrad", "Offset", "define_fdjvp", "value_and_fgrad")
+
 P = ParamSpec("P")
 T = TypeVar("T")
+constant_treedef = jtu.tree_structure(0)
+PyTree = Any
 
 
-__all__ = ("fgrad", "Offset", "define_fdjvp", "value_and_fgrad")
+@dc.dataclass(frozen=True)
+class Offset:
+    """Convinience class for finite difference offsets used inside `fgrad`
 
+    Args:
+        accuracy: The accuracy of the finite difference scheme. Must be >=2.
 
-class Offset(NamedTuple):
-    """Convinience class for finite difference offsets used inside `fgrad`"""
+    Example:
+        >>> import finitediffx as fdx
+        >>> fdx.fgrad(lambda x: x**2, offsets=fdx.Offset(accuracy=2))(1.0)
+        Array(2., dtype=float32)
+    """
 
     accuracy: int
 
 
-OffsetType = Union[jax.Array, Offset]
-StepsizeType = Union[jax.Array, float]
+OffsetType = Union[jax.Array, Offset, PyTree]
+StepsizeType = Union[jax.Array, float, PyTree]
 
 
 def _evaluate_func_at_shifted_steps_along_argnum(
     func: Callable[P, T],
     *,
     coeffs: jax.Array,
     offsets: jax.Array,
@@ -50,91 +62,116 @@
     step_size: StepsizeType,
     derivative: int,
 ):
     if not isinstance(argnum, int) or argnum < 0:
         raise ValueError(f"argnum must be a non-negative integer, got {argnum}")
 
     dxs = offsets * step_size
+    den = step_size**derivative
 
     def wrapper(*args, **kwargs):
-        # yield function output at shifted points
-        result = []
-        for coeff, dx in zip(coeffs, dxs):
-            args_ = list(args)
-            args_[argnum] += dx
-            result += [coeff * func(*args_, **kwargs) / (step_size**derivative)]
-        return sum(result)
+        if not hasattr(args[argnum], "shape"):
+            # scalar perturbation
+            def perturb(h):
+                args_ = list(args)
+                args_[argnum] += h
+                return func(*args_, **kwargs)
+
+            return sum([coeff * perturb(dx) / den for coeff, dx in zip(coeffs, dxs)])
+
+        # elementwise perturbation
+        # should be much slower than jax.grad for large arrays
+        # but can be used for non-tracable code where jax.grad fails
+        def perturb(h):
+            xflat = jnp.array(args[argnum].flatten())
+            arange = jnp.arange(len(xflat))
+            shape = args[argnum].shape
+
+            def perturb_element(i):
+                xflat_ = xflat.at[i].add(h)
+                args_ = list(args)
+                args_[argnum] = xflat_.reshape(shape)
+                return func(*args_, **kwargs)
+
+            # `jax.vmap` can be used here and perform better
+            # but it would fail in case of non-tracable code
+            # may have try/excpet wiht `jax.errors.TracerArrayConversionError``
+            result = jnp.array([perturb_element(i) for i in arange])
+
+            # the function might return non-scalars
+            try:
+                return result.reshape(shape)
+            except Exception:
+                raise TypeError("Non scalar-output.")
+
+        return sum([coeff * perturb(dx) / den for coeff, dx in zip(coeffs, dxs)])
 
     return wrapper
 
 
 def resolve_step_size(
-    step_size: StepsizeType | tuple[StepsizeType, ...] | None,
-    length: int | None,
+    step_size: StepsizeType | Sequence[StepsizeType] | None,
+    treedef: jtu.PyTreeDef,
     derivative: int,
-) -> tuple[StepsizeType, ...] | StepsizeType:
+) -> Sequence[StepsizeType] | StepsizeType:
     # return non-tuple values if length is None
+    length = treedef.num_leaves
+
     if isinstance(step_size, (jax.Array, float)):
-        return ((step_size,) * length) if length else step_size
+        return (step_size,) * length
+
     if step_size is None:
         default = (2) ** (-23 / (2 * derivative))
-        return ((default,) * length) if length else default
+        return (default,) * length
+
+    step_size_leaves, step_size_treedef = jtu.tree_flatten(step_size)
 
-    if isinstance(step_size, tuple) and length:
-        assert len(step_size) == length, f"step_size must be a tuple of length {length}"
-        step_size = list(step_size)
-        for i, s in enumerate(step_size):
-            if s is None:
-                step_size[i] = (2) ** (-23 / (2 * derivative))
-            elif not isinstance(s, (jax.Array, float)):
-                raise TypeError(f"{type(s)} not in {(jax.Array, float)}")
-        return tuple(step_size)
+    if step_size_treedef == treedef:
+        # step_size is a pytree with the same structure as the input
+        return step_size_leaves
 
     raise TypeError(
         f"`step_size` must be of type:\n"
         f"- `jax.Array`\n"
         f"- `float`\n"
         f"- tuple of `jax.Array` or `float` for tuple argnums.\n"
+        f"- pytree with the same structure as the desired arg.\n"
         f"but got {type(step_size)=}"
     )
 
 
 def resolve_offsets(
-    offsets: tuple[OffsetType | None, ...] | OffsetType | None,
-    length: int,
+    offsets: Sequence[OffsetType | None] | OffsetType | None,
+    treedef: jax.tree_util.PyTreeDef,
     derivative: int,
 ) -> tuple[OffsetType, ...] | OffsetType:
     # single value
+    length = treedef.num_leaves
+
     if isinstance(offsets, Offset):
         if offsets.accuracy < 2:
             raise ValueError(f"offset accuracy must be >=2, got {offsets.accuracy}")
         offsets = jnp.array(_generate_central_offsets(derivative, offsets.accuracy))
-        return ((offsets,) * length) if length else offsets
+        return (offsets,) * length
+
     if isinstance(offsets, jax.Array):
-        return ((offsets,) * length) if length else offsets
+        return (offsets,) * length
 
-    if isinstance(offsets, tuple) and length:
-        assert len(offsets) == length, f"`offsets` must be a tuple of length {length}"
-        offsets = list(offsets)
-        for i, o in enumerate(offsets):
-            if isinstance(o, Offset):
-                if o.accuracy < 2:
-                    raise ValueError(f"offset accuracy must be >=2, got {o.accuracy}")
-                o = jnp.array(_generate_central_offsets(derivative, o.accuracy))
-                offsets[i] = o
-            elif not isinstance(o, (Offset, jax.Array)):
-                raise TypeError(f"{type(o)} not an Offset")
+    offsets_leaves, offsets_treedef = jtu.tree_flatten(offsets)
 
-        return tuple(offsets)
+    if offsets_treedef == treedef:
+        # offsets is a pytree with the same structure as the input
+        return offsets_leaves
 
     raise TypeError(
         f"`offsets` must be of type:\n"
         f"- `Offset`\n"
         f"- `jax.Array`\n"
         f"- tuple of `Offset` or `jax.Array` for tuple argnums.\n"
+        f"- pytree with the same structure as the desired arg.\n"
         f"but got {type(offsets)=}"
     )
 
 
 def _fgrad_along_argnum(
     func: Callable,
     *,
@@ -142,47 +179,39 @@
     step_size: StepsizeType | None = None,
     offsets: OffsetType = Offset(accuracy=3),
     derivative: int = 1,
 ):
     if not isinstance(argnum, int):
         raise TypeError(f"argnum must be an integer, got {type(argnum)}")
 
-    def _leaves_fgrad(func: Callable, *, length: int):
-        kwargs = dict(length=length, derivative=derivative)
-        resolved_step_size = resolve_step_size(step_size, **kwargs)
-        resolved_offsets = resolve_offsets(offsets, **kwargs)
+    def wrapper(*args, **kwargs):
+        flat_args, arg_treedef = jtu.tree_flatten(args[argnum])
+        args_ = list(args)
 
-        dfuncs = [
+        def func_wrapper(*leaves):
+            args_[argnum] = jtu.tree_unflatten(arg_treedef, leaves)
+            return func(*args_, **kwargs)
+
+        spec = dict(treedef=arg_treedef, derivative=derivative)
+        step_size_ = resolve_step_size(step_size, **spec)
+        offsets_ = resolve_offsets(offsets, **spec)
+
+        flat_result = [
             _evaluate_func_at_shifted_steps_along_argnum(
-                func=func,
+                func=func_wrapper,
                 coeffs=generate_finitediff_coeffs(oi, derivative),
                 offsets=oi,
                 step_size=si,
                 derivative=derivative,
                 argnum=i,
-            )
-            for i, (oi, si) in enumerate(zip(resolved_offsets, resolved_step_size))
+            )(*flat_args)
+            for i, (oi, si) in enumerate(zip(offsets_, step_size_))
         ]
 
-        def wrapper(*a, **k):
-            return [df(*a, **k) for df in dfuncs]
-
-        return wrapper
-
-    def wrapper(*args, **kwargs):
-        arg_leaves, arg_treedef = jtu.tree_flatten(args[argnum])
-        args_ = list(args)
-
-        def func_wrapper(*leaves):
-            args_[argnum] = jtu.tree_unflatten(arg_treedef, leaves)
-            return func(*args_, **kwargs)
-
-        dfunc = _leaves_fgrad(func=func_wrapper, length=len(arg_leaves))
-
-        return jtu.tree_unflatten(arg_treedef, dfunc(*arg_leaves))
+        return jtu.tree_unflatten(arg_treedef, flat_result)
 
     return wrapper
 
 
 def value_and_fgrad(
     func: Callable,
     *,
@@ -201,14 +230,16 @@
             If a tuple is passed, the function is differentiated with respect to
             all the arguments in the tuple.
         step_size: step size for the finite difference stencil. If `None`, the step size
             is set to `(2) ** (-23 / (2 * derivative))`
         offsets: offsets for the finite difference stencil. Accepted types are:
             - `jax.Array` defining location of function evaluation points.
             - `Offset` with accuracy field to automatically generate offsets.
+            - pytree of `jax.Array`/`Offset` to define offsets for each argument
+                of the same pytree structure as argument defined by `argnums`.
         derivative: derivative order. Defaults to 1.
         has_aux: whether the function returns an auxiliary output. Defaults to False.
             If True, the derivative function will return a tuple of the form:
             ((value,aux), derivative) otherwise (value, derivative)
 
     Returns:
         Value and derivative of the function if `has_aux` is False.
@@ -237,21 +268,19 @@
     if not isinstance(has_aux, bool):
         raise TypeError(f"{type(has_aux)} not a bool")
 
     func_ = (lambda *a, **k: func(*a, **k)[0]) if has_aux else func
 
     if isinstance(argnums, int):
         # fgrad(func, argnums=0)
-        kwargs = dict(length=None, derivative=derivative)
-
         dfunc = _fgrad_along_argnum(
             func=func_,
             argnum=argnums,
-            step_size=resolve_step_size(step_size, **kwargs),
-            offsets=resolve_offsets(offsets, **kwargs),
+            step_size=step_size,
+            offsets=offsets,
             derivative=derivative,
         )
 
         if has_aux is True:
 
             @ft.wraps(func)
             def wrapper(*a, **k):
@@ -266,29 +295,38 @@
 
         return wrapper
 
     if isinstance(argnums, tuple):
         # fgrad(func, argnums=(0,1))
         # return a tuple of derivatives evaluated at each argnum
         # this behavior is similar to jax.grad(func, argnums=(...))
-        kwargs = dict(length=len(argnums), derivative=derivative)
+        if isinstance(offsets, tuple):
+            if len(offsets) != len(argnums):
+                raise AssertionError("offsets must have the same length as argnums")
+            offsets_ = offsets
+        else:
+            offsets_ = (offsets,) * len(argnums)
+
+        if isinstance(step_size, tuple):
+            if len(step_size) != len(argnums):
+                raise AssertionError("step_size must have the same length as argnums")
+            step_size_ = step_size
+
+        else:
+            step_size_ = (step_size,) * len(argnums)
 
         dfuncs = [
             _fgrad_along_argnum(
                 func=func_,
-                argnum=argnum_i,
-                step_size=step_size_i,
-                offsets=offsets_i,
+                argnum=ai,
+                step_size=si,
+                offsets=oi,
                 derivative=derivative,
             )
-            for offsets_i, step_size_i, argnum_i in zip(
-                resolve_offsets(offsets, **kwargs),
-                resolve_step_size(step_size, **kwargs),
-                argnums,
-            )
+            for oi, si, ai in zip(offsets_, step_size_, argnums)
         ]
 
         if has_aux:
 
             @ft.wraps(func)
             def wrapper(*a, **k):
                 # destructuring the tuple to ensure
@@ -325,14 +363,16 @@
             If a tuple is passed, the function is differentiated with respect to
             all the arguments in the tuple.
         step_size: step size for the finite difference stencil. If `None`, the step size
             is set to `(2) ** (-23 / (2 * derivative))`
         offsets: offsets for the finite difference stencil. Accepted types are:
             - `jax.Array` defining location of function evaluation points.
             - `Offset` with accuracy field to automatically generate offsets.
+            - pytree of `jax.Array`/`Offset` to define offsets for each argument
+                of the same pytree structure as argument defined by `argnums`.
         derivative: derivative order. Defaults to 1.
         has_aux: whether the function returns an auxiliary output. Defaults to False.
             If True, the derivative function will return a tuple of the form:
             (derivative, aux) otherwise it will return only the derivative.
 
     Returns:
         Derivative of the function if `has_aux` is False, otherwise a tuple of
@@ -364,26 +404,26 @@
         derivative=derivative,
         has_aux=has_aux,
     )
 
     if has_aux:
 
         @ft.wraps(func)
-        def aux_wrapper(*a, **k):
+        def wrapper(*a, **k):
             (_, aux), g = value_and_fgrad_func(*a, **k)
             return g, aux
 
-    else:
+        return wrapper
 
-        @ft.wraps(func)
-        def wrapper(*a, **k):
-            _, g = value_and_fgrad_func(*a, **k)
-            return g
+    @ft.wraps(func)
+    def wrapper(*a, **k):
+        _, g = value_and_fgrad_func(*a, **k)
+        return g
 
-    return aux_wrapper if has_aux else wrapper
+    return wrapper
 
 
 def define_fdjvp(
     func: Callable[P, T],
     offsets: tuple[OffsetType, ...] | OffsetType = Offset(accuracy=2),
     step_size: tuple[float, ...] | float | None = None,
 ) -> Callable[P, T]:
@@ -435,15 +475,15 @@
             >>> print(numpy_func(1., 2.))
             0.5402466
     """
     func = jax.custom_jvp(func)
 
     @func.defjvp
     def _(primals, tangents):
-        kwargs = dict(length=len(primals), derivative=1)
+        kwargs = dict(treedef=jtu.tree_structure(primals), derivative=1)
         step_size_ = resolve_step_size(step_size, **kwargs)
         offsets_ = resolve_offsets(offsets, **kwargs)
         primal_out = func(*primals)
         tangent_out = sum(
             fgrad(func, argnums=i, step_size=si, offsets=oi)(*primals) * ti
             for i, (si, oi, ti) in enumerate(zip(step_size_, offsets_, tangents))
         )
```

### Comparing `FiniteDiffX-0.0.4/finitediffx/_src/finite_diff.py` & `FiniteDiffX-0.0.5/finitediffx/_src/finite_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
 @ft.partial(jax.jit, static_argnames=("accuracy", "axis", "derivative", "method"))
 def difference(
     array: jax.Array,
     *,
     axis: int = 0,
     accuracy: int = 1,
-    step_size: float | jax.Array = 1,
+    step_size: float | jax.Array = 1.0,
     derivative: int = 1,
     method: MethodKind = "central",
 ) -> jax.Array:
     """Compute the finite difference derivative along a given axis with a given accuracy
     using central difference for interior points and forward/backward difference for boundary points
     Similar to np.gradient, but with the option to specify accuracy, derivative and step size
     See: https://github.com/google/jax/blob/main/jax/_src/numpy/lax_numpy.py
```

### Comparing `FiniteDiffX-0.0.4/finitediffx/_src/utils.py` & `FiniteDiffX-0.0.5/finitediffx/_src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,10 +134,12 @@
 
     See:
         https://en.wikipedia.org/wiki/Finite_difference_coefficient
         https://web.media.mit.edu/~crtaylor/calculator.html
     """
 
     if derivative >= len(offsets):
-        raise ValueError(f"{len(offsets)=} must be larger than {derivative=}.")
+        raise ValueError(
+            f"{offsets=} of {len(offsets)=} must be larger than {derivative=}."
+        )
 
     return _generate_finitediff_coeffs(offsets, derivative)
```

### Comparing `FiniteDiffX-0.0.4/setup.py` & `FiniteDiffX-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `FiniteDiffX-0.0.4/tests/test_fgrad.py` & `FiniteDiffX-0.0.5/tests/test_fgrad.py`

 * *Files 19% similar despite different names*

```diff
@@ -144,14 +144,16 @@
 
     with pytest.raises(TypeError):
         dfunc = fgrad(
             func,
             step_size=(None, 1e-3),
             offsets=(jnp.array([-1, 1.0]), jnp.array([-2, 2.0])),
             argnums=0,
+        )(
+            1.0, 2.0
         )  # non-tuple argnums with tuple step_size
 
     with pytest.raises(AssertionError):
         # mismatched argnums length and step_size length
         dfunc = fgrad(func, step_size=(None,), argnums=(0, 1))
 
     with pytest.raises(AssertionError):
@@ -160,19 +162,22 @@
 
     with pytest.raises(ValueError):
         # wrong accuracy
         dfunc = fgrad(
             func,
             offsets=(Offset(accuracy=0), Offset(accuracy=1)),
             argnums=(0, 1),
-        )
+        )(1.0, 1.0)
 
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         # wrong accuracy
-        dfunc = fgrad(func, offsets=(Offset(accuracy=2), ""), argnums=(0, 1))
+        dfunc = fgrad(
+            func, offsets=(Offset(accuracy=2), Offset(accuracy=1)), argnums=(0, 1)
+        )
+        dfunc(1.0, 1.0)
 
 
 def test_fgrad_argnum():
     with enable_x64():
         all_correct = lambda lhs, rhs: np.testing.assert_allclose(lhs, rhs, atol=0.05)
 
         # test argnums
@@ -207,18 +212,18 @@
 
 
 def test_fgrad_error():
     with pytest.raises(TypeError):
         fgrad(lambda x: x, argnums=1.0)
 
     with pytest.raises(ValueError):
-        fgrad(lambda x: x, offsets=Offset(accuracy=1))
+        fgrad(lambda x: x, offsets=Offset(accuracy=1))(1.0)
 
     with pytest.raises(TypeError):
-        fgrad(lambda x: x, argnums=[1, 2])
+        fgrad(lambda x: x, argnums=[1, 2])(1.0)
 
 
 def test_fdjvp():
     def wrap_pure_callback(func):
         @ft.wraps(func)
         def wrapper(*args, **kwargs):
             args = [jnp.asarray(arg) for arg in args]
@@ -255,22 +260,74 @@
         return x**2, "value"
 
     assert value_and_fgrad(func, has_aux=True)(1.0) == ((1.0, "value"), 2.0)
 
     with pytest.raises(TypeError):
         value_and_fgrad(func, has_aux="")(1.0)
 
+    v, g = value_and_fgrad(func, has_aux=True, argnums=(0,))(1.0)
+
+    assert v == (1.0, "value")
+    assert g[0] == jnp.array(2.0)
+
 
 def test_fgrad_pytree():
     params = {"a": 1.0, "b": 2.0, "c": 3.0}
 
     def f(params):
         return params["a"] ** 2 + params["b"]
 
-    jax.grad(f)(params), fgrad(f)(params)
-
     dparams_fdx = fgrad(f)(params)
     dparams_jax = jax.grad(f)(params)
 
     npt.assert_allclose(dparams_fdx["a"], dparams_jax["a"], atol=1e-3)
     npt.assert_allclose(dparams_fdx["b"], dparams_jax["b"], atol=1e-3)
     npt.assert_allclose(dparams_fdx["c"], dparams_jax["c"], atol=1e-3)
+
+    step_size = {"a": 1, "b": 1, "c": 1}
+    offsets = {
+        "a": jnp.array([-1, 1]),
+        "b": jnp.array([-1, 1]),
+        "c": jnp.array([-1, 1]),
+    }
+
+    dparams_fdx = fgrad(f, step_size=step_size, offsets=offsets)(params)
+    dparams_jax = jax.grad(f)(params)
+
+    npt.assert_allclose(dparams_fdx["a"], dparams_jax["a"], atol=1e-3)
+    npt.assert_allclose(dparams_fdx["b"], dparams_jax["b"], atol=1e-3)
+    npt.assert_allclose(dparams_fdx["c"], dparams_jax["c"], atol=1e-3)
+
+    step_size = {"a": 1, "b": 1, "c": 0}
+    dparams_fdx = fgrad(f, step_size=step_size)(params)
+
+    # divide by zero
+    assert jnp.isnan(dparams_fdx["c"])
+
+    offsets = {"a": jnp.array([0, 0]), "b": jnp.array([-1, 1]), "c": jnp.array([-1, 1])}
+    dparams_fdx = fgrad(f, offsets=offsets)(params)
+
+    # generating coefficients for a will fail
+    assert jnp.isnan(dparams_fdx["a"])
+
+    (dparams_fdx,) = fgrad(f, argnums=(0,))(params)
+    (dparams_jax,) = jax.grad(f, argnums=(0,))(params)
+
+    npt.assert_allclose(dparams_fdx["a"], dparams_jax["a"], atol=1e-3)
+    npt.assert_allclose(dparams_fdx["b"], dparams_jax["b"], atol=1e-3)
+    npt.assert_allclose(dparams_fdx["c"], dparams_jax["c"], atol=1e-3)
+
+    step_size = {"a": 1, "b": 1, "c": 1}
+    offsets = {
+        "a": jnp.array([-1, 1]),
+        "b": jnp.array([-1, 1]),
+        "c": jnp.array([-1, 1]),
+    }
+
+    (dparams_fdx,) = fgrad(f, step_size=(step_size,), offsets=(offsets,), argnums=(0,))(
+        params
+    )
+    dparams_jax = jax.grad(f)(params)
+
+    npt.assert_allclose(dparams_fdx["a"], dparams_jax["a"], atol=1e-3)
+    npt.assert_allclose(dparams_fdx["b"], dparams_jax["b"], atol=1e-3)
+    npt.assert_allclose(dparams_fdx["c"], dparams_jax["c"], atol=1e-3)
```

### Comparing `FiniteDiffX-0.0.4/tests/test_finite_diff.py` & `FiniteDiffX-0.0.5/tests/test_finite_diff.py`

 * *Files identical despite different names*

