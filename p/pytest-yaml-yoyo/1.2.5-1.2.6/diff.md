# Comparing `tmp/pytest-yaml-yoyo-1.2.5.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.5.tar", last modified: Wed Jun  7 14:33:02 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.6.tar", last modified: Thu Jun  8 15:20:09 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.2.5.tar` & `pytest-yaml-yoyo-1.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.808215 pytest-yaml-yoyo-1.2.5/
--rw-rw-rw-   0        0        0    24946 2023-06-07 14:33:02.808215 pytest-yaml-yoyo-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    24447 2023-06-07 14:32:57.000000 pytest-yaml-yoyo-1.2.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-07 14:33:02.809212 pytest-yaml-yoyo-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-06-07 14:31:06.000000 pytest-yaml-yoyo-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.756354 pytest-yaml-yoyo-1.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.796248 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0       20 2023-06-07 14:28:14.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     4113 2023-05-30 00:16:10.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0     3063 2023-06-07 14:30:58.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     9783 2023-06-07 14:28:48.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/request_session.py
--rw-rw-rw-   0        0        0    28695 2023-05-30 00:24:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:33:02.806220 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    24946 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-07 14:33:02.000000 pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.360916 pytest-yaml-yoyo-1.2.6/
+-rw-rw-rw-   0        0        0    25252 2023-06-08 15:20:09.359919 pytest-yaml-yoyo-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    24753 2023-06-08 15:19:36.000000 pytest-yaml-yoyo-1.2.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-08 15:20:09.360916 pytest-yaml-yoyo-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-06-08 15:20:07.000000 pytest-yaml-yoyo-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.326009 pytest-yaml-yoyo-1.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.349944 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0       20 2023-06-07 14:28:14.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     4113 2023-05-30 00:16:10.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0     3063 2023-06-07 14:30:58.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0     9783 2023-06-08 07:14:20.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4690 2023-06-08 15:17:14.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    28695 2023-05-30 00:24:02.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3803 2023-06-08 08:28:11.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:20:09.358924 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    25252 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-08 15:20:09.000000 pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.2.5/PKG-INFO` & `pytest-yaml-yoyo-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.5
+Version: 1.2.6
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -212,14 +212,24 @@
 
 v1.2.5 发布 2023-06-07
 
 优化以下问题
 
 - 1.优化参数化路径读取，以项目根路径拼接路径
 
+v1.2.6 发布 2023-06-08
+
+优化以下问题
+
+- 1.优化断言方式 len_eq
+- 2.模板过滤器 filter 支持
+- 3.变量取值优化, 所有的取值，数字类型默认int
+- 4.取值结果数字转字符串，可以用`${str(取值表达式)} 或者过滤器方式 `${取值表达式 | str}`
+
+
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.5/README.rst` & `pytest-yaml-yoyo-1.2.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,24 @@
 
 v1.2.5 发布 2023-06-07
 
 优化以下问题
 
 - 1.优化参数化路径读取，以项目根路径拼接路径
 
+v1.2.6 发布 2023-06-08
+
+优化以下问题
+
+- 1.优化断言方式 len_eq
+- 2.模板过滤器 filter 支持
+- 3.变量取值优化, 所有的取值，数字类型默认int
+- 4.取值结果数字转字符串，可以用`${str(取值表达式)} 或者过滤器方式 `${取值表达式 | str}`
+
+
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.5/setup.py` & `pytest-yaml-yoyo-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.2.5',
+    version='v1.2.6',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
```

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/create_funtion.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/extract.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/my_builtins.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/my_builtins.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/render_template_obj.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/render_template_obj.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,74 @@
-from jinja2 import Template
 import re
 from .log import log
+import jinja2
+import yaml
 
 
-class NewDict(dict):
-    """dict按点方式取值
-        a = {
-                "x": 123,
-                "y": "hello"
-            }
-        print(a.x)
-    """
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+# 解决 yaml 文件中日期被转成 datetime 类型
+yaml.SafeLoader.yaml_implicit_resolvers = {
+    k: [r for r in v if r[0] != 'tag:yaml.org,2002:timestamp'] for
+    k, v in yaml.SafeLoader.yaml_implicit_resolvers.items()
+}
+
+
+def add(value, num=0):
+    """jinja2 过滤器 add函数"""
+    return int(value)+num
+
 
-    def __getattr__(self, name):
-        value = self[name]
-        if isinstance(value, dict):
-            value = NewDict(value)
-        return value
+def to_str(value):
+    return f'"{value}"'
+
+
+env_filter = jinja2.Environment(
+    variable_start_string='${', variable_end_string='}'
+)
+env_filter.filters["add"] = add
+env_filter.filters["str"] = to_str
 
 
 def rend_template_str(template_str, *args, **kwargs):
     """
        渲染模板字符串, 改写了默认的引用变量语法{{var}}, 换成${var}
             模板中引用变量语法 ${var},
             调用函数 ${fun()}
         :return: 渲染之后的值
     """
     # -------------解决函数内部参数引用变量-------
     def re_replace_template_str(match) -> str:
-        """匹配的值--渲染模板加载内部引用变量"""
+        """
+        匹配的值--渲染模板加载内部引用变量
+        """
         res_result = match.group()
         res_result_ = str(res_result).lstrip('${').rstrip('}')
         if '${' in res_result_ and '}' in res_result_ and res_result_.find('${') < res_result_.find('}'):
-            # 渲染结果
-            instance_temp = Template(res_result_, variable_start_string='${', variable_end_string='}')
+            instance_temp = env_filter.from_string(res_result_)
             temp_render_res = instance_temp.render(*args, **kwargs)
             return '${' + temp_render_res + '}'
         else:
             return res_result
-
-    template_str = re.sub('\$\{(.+)\}', re_replace_template_str, template_str)  # noqa
-    # ----------------end----------
-
-    instance_template = Template(template_str, variable_start_string='${', variable_end_string='}')
+    # 正则替换
+    template_str = re.sub('\$\{(.+)\}', re_replace_template_str, template_str) # noqa
+    instance_template = env_filter.from_string(template_str)
     template_render_res = instance_template.render(*args, **kwargs)
     if template_str.startswith("${") and template_str.endswith("}") and template_str.count('${') == 1:
+        template_raw_str = template_str.rstrip('}').lstrip('${')
+        if kwargs.get(template_raw_str):
+            log.info(f"取值表达式: {template_raw_str}, 取值结果：{kwargs.get(template_raw_str)} {type(kwargs.get(template_raw_str))}")
+            return kwargs.get(template_raw_str)
+        if template_raw_str.startswith("str(") and template_raw_str.endswith(")"):
+            log.info(f"取值表达式: {template_raw_str}, 取值结果：{template_render_res} {type(template_render_res)}")
+            return str(template_render_res)
         try:
-            template_raw_str = template_str.rstrip('}').lstrip('${')
-            # 先判断有没有list 取值如： user.0 换成[0]
-            template_find_res = re.findall('\.[0-9]+', template_raw_str)
-            if template_find_res:
-                for template_i in template_find_res:
-                    template_raw_str = template_raw_str.replace(template_i, f"[{str(template_i).lstrip('.')}]")
-            # 根据表达式取值
-            log.info(f"取值表达式 {template_raw_str}")
-            locals().update(**NewDict(kwargs))  # 更新成本地变量
-            for kwargs_locals_key, kwargs_locals_value in kwargs.items():
-                if isinstance(kwargs_locals_value, dict):
-                    locals()[kwargs_locals_key] = NewDict(kwargs_locals_value)
-                else:
-                    locals()[kwargs_locals_key] = kwargs_locals_value
-            template_render_result = eval(template_raw_str)
-            log.info(f"取值结果：{template_render_result}, {type(template_render_result)}")
-            return template_render_result
-        except Exception:      # noqa
-            log.info(f"取值异常：{template_str}, 返回模板渲染结果: {template_render_res}")
+            result_value = yaml.safe_load(template_render_res)
+            log.info(f"取值表达式: {template_raw_str}, 取值结果：{result_value} {type(result_value)}")
+            return result_value
+        except Exception as msg:   # noqa
+            log.info(f"取值表达式: {template_raw_str}, 取值结果：{template_render_res}  {type(template_render_res)}")
             return template_render_res
     else:
         return template_render_res
 
 
 def rend_template_obj(t_obj: dict, *args, **kwargs):
     """
```

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/request_session.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/request_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/runner.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,18 @@
     assert str(check_value) == str(expect_value), f'{check_value} == {expect_value}'
 
 
 def length_equals(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
     if isinstance(check_value, list):
         assert len(check_value) == expect_len, f'{len(check_value)} == {expect_value}'
-    else:
+    elif isinstance(check_value, (int, float)):
         assert len(str(check_value)) == expect_len, f'{len(str(check_value))} == {expect_value}'
+    else:
+        assert len(check_value) == expect_len, f'{len(check_value)} == {expect_value}'
 
 
 def length_greater_than(check_value, expect_value):
     expect_len = _cast_to_int(expect_value)
     assert len(check_value) > expect_len, f'{len(check_value)} > {expect_value}'
```

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.5
+Version: 1.2.6
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -212,14 +212,24 @@
 
 v1.2.5 发布 2023-06-07
 
 优化以下问题
 
 - 1.优化参数化路径读取，以项目根路径拼接路径
 
+v1.2.6 发布 2023-06-08
+
+优化以下问题
+
+- 1.优化断言方式 len_eq
+- 2.模板过滤器 filter 支持
+- 3.变量取值优化, 所有的取值，数字类型默认int
+- 4.取值结果数字转字符串，可以用`${str(取值表达式)} 或者过滤器方式 `${取值表达式 | str}`
+
+
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.5/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.6/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

