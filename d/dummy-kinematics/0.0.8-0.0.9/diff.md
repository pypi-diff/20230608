# Comparing `tmp/dummy_kinematics-0.0.8.tar.gz` & `tmp/dummy_kinematics-0.0.9.tar.gz`

## Comparing `dummy_kinematics-0.0.8.tar` & `dummy_kinematics-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/PKG-INFO
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/test2.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/__about__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/__init__.py
--rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/chart_element.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/config.py
--rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/data_converter.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/descriptors.py
--rw-r--r--   0        0        0    54622 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/dummy_iso_config.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/json_file_helper.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/logger_helper.py
--rw-r--r--   0        0        0    20807 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/ppt_factory.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/ppt_insert_helper.py
--rw-r--r--   0        0        0    15270 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/unitils.py
--rw-r--r--   0        0        0   252577 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/dummy_kinematics/default/default_template.pptx
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/README.md
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/test2.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/__about__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/__init__.py
+-rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/chart_element.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/config.py
+-rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/data_converter.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/descriptors.py
+-rw-r--r--   0        0        0    54622 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/dummy_iso_config.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/json_file_helper.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/logger_helper.py
+-rw-r--r--   0        0        0    20807 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/ppt_factory.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/ppt_insert_helper.py
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/unitils.py
+-rw-r--r--   0        0        0   252577 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/dummy_kinematics/default/default_template.pptx
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/README.md
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 dummy_kinematics-0.0.9/PKG-INFO
```

### Comparing `dummy_kinematics-0.0.8/PKG-INFO` & `dummy_kinematics-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dummy-kinematics
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/unknown/dummy-kinematics#readme
 Project-URL: Issues, https://github.com/unknown/dummy-kinematics/issues
 Project-URL: Source, https://github.com/unknown/dummy-kinematics
 Author-email: xiaochai <1219295581@qq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dummy_kinematics-0.0.8/test2.py` & `dummy_kinematics-0.0.9/test2.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/chart_element.py` & `dummy_kinematics-0.0.9/dummy_kinematics/chart_element.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/data_converter.py` & `dummy_kinematics-0.0.9/dummy_kinematics/data_converter.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/descriptors.py` & `dummy_kinematics-0.0.9/dummy_kinematics/descriptors.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/dummy_iso_config.py` & `dummy_kinematics-0.0.9/dummy_kinematics/dummy_iso_config.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/logger_helper.py` & `dummy_kinematics-0.0.9/dummy_kinematics/logger_helper.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/ppt_factory.py` & `dummy_kinematics-0.0.9/dummy_kinematics/ppt_factory.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/ppt_insert_helper.py` & `dummy_kinematics-0.0.9/dummy_kinematics/ppt_insert_helper.py`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/unitils.py` & `dummy_kinematics-0.0.9/dummy_kinematics/unitils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from decimal import Decimal
 from pptx import Presentation
 from colorama import Fore, Style, init
-from numpy.typing import NDArray
 import pandas as pd
 import numpy as np
 import copy
 from scipy import signal
 from typing import NoReturn, Tuple
 from pptx.presentation import Presentation as _PresentationObj
 from collections.abc import Iterable
 from collections import Counter
 from scipy.integrate import cumulative_trapezoid
+from typing import Sequence
+from numpy.typing import NDArray
 
 init(autoreset=True)  # 彩打完成后默认重置恢复默认样式
 
 
 def pptx_identify(prs_path: str, output_file: bool = True) -> NoReturn:
     """识别pptx模板占位符,打印输出占位符情况，默认输出确认文件。
     prs_path: 字符串输入需要确认的模板文件，如"template.pptx"
@@ -462,7 +463,116 @@
     index, number = index_number(df['sd_relative'], inch3)
     rttf_min = timeseries[index] - 30
     rttf_min = round(rttf_min, 2)
     index, number = index_number(df['sd_relative'], inch5)
     rttf_max = timeseries[index] - 30
     rttf_max = round(rttf_max, 2)
     return rttf_min, rttf_max
+
+
+
+
+def increase_index_number(li: Sequence, target: float):
+    res = (0, li[0])
+    gap = abs(res[1] - target)
+    for idx, value in enumerate(li):
+        if idx == 0:
+            continue
+        elif (abs(value - target) < gap) and ((value - li[idx - 1]) > 0):
+            gap = abs(value - target)
+            res = (idx, value)
+    return res
+
+
+def _init_seg_points(x: NDArray, *segs) -> list[tuple[int, float]]:
+    """
+    :param x:
+    :param segs: 分割点
+    :return: 返回[(index, number)...]
+    """
+
+    x_min = min(x)
+    x_max = max(x)
+    inputs = [x_min, *segs, x_max]
+    inputs.sort()
+    res = [increase_index_number(x, target) for target in inputs]
+    return res
+
+
+def get_seg_mean(seg_to_last_intg: list[float], seg_points_values: list[float]) -> list[float]:
+    assert len(seg_to_last_intg) == len(seg_points_values), "inputs list should be ths same len"
+    li_len = len(seg_points_values)
+    res = []
+    for i in range(li_len):
+        try:
+            res.append(seg_to_last_intg[i] / (seg_points_values[i] - seg_points_values[i - 1]))
+        except IndexError:
+            res.append(0)
+    return res
+
+
+def make_output_xy(x: NDArray, index_series: list[int], seg_to_last_mean: list[float]) -> tuple:
+    """
+
+    :param x:
+    :param index_series:
+    :param seg_to_last_mean:
+    :return: 返回处理后的x,y , 均为 NDArray
+    """
+    assert len(index_series) == len(seg_to_last_mean), "input list should be the same length"
+    out_x = x[:max(index_series) + 1]
+    out_y = np.empty(max(index_series) + 1)
+    index_mean = list(zip(index_series, seg_to_last_mean))
+
+    def match_y(index: int):
+        for idx1, mean in index_mean:
+            if index <= idx1:
+                return mean
+
+    for idx, value in enumerate(out_y):
+        out_y[idx] = match_y(idx)
+
+    return out_x, out_y
+
+
+def _get_seg_intg(x: NDArray, y: NDArray, start_index: int, end_index: int) -> float:
+    from scipy.integrate import trapezoid
+    filtered_y = y[start_index:end_index + 1]
+    filtered_x = x[start_index:end_index + 1]
+    return trapezoid(y=filtered_y, x=filtered_x)
+
+
+def get_seg_to_last_intg(x: NDArray, y: NDArray, index_series: list[int]) -> list[float]:
+    seg_to_last_intg = []
+    for i in range(len(index_series)):
+        if i == 0:
+            seg_to_last_intg.append(0)
+
+        else:
+            seg_to_last_intg.append(_get_seg_intg(x, y, start_index=index_series[i - 1], end_index=index_series[i]))
+
+    return seg_to_last_intg
+
+
+def make_seg_mean(x: NDArray, y: NDArray, *segs) -> dict:
+    """
+
+    :param x:
+    :param y:
+    :param segs:
+    :return: out_x=out_x, out_y=out_y, result_dict=result_dict
+    """
+    result_dict = {}
+    segs_tuples = _init_seg_points(x, *segs)
+    result_dict["seg_pt_values"] = [tup[1] for tup in segs_tuples]
+    result_dict["index"] = [tup[0] for tup in segs_tuples]
+    result_dict["seg_to_last_intg"] = get_seg_to_last_intg(x, y, result_dict["index"])
+    result_dict["seg_to_last_mean"] = get_seg_mean(result_dict["seg_to_last_intg"], result_dict["seg_pt_values"])
+
+    out_x, out_y = make_output_xy(x, result_dict["index"], result_dict["seg_to_last_mean"])
+    return dict(out_x=out_x, out_y=out_y, result_dict=result_dict)
+
+
+
+
+
+
```

### Comparing `dummy_kinematics-0.0.8/dummy_kinematics/default/default_template.pptx` & `dummy_kinematics-0.0.9/dummy_kinematics/default/default_template.pptx`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/README.md` & `dummy_kinematics-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dummy_kinematics-0.0.8/pyproject.toml` & `dummy_kinematics-0.0.9/pyproject.toml`

 * *Files identical despite different names*

