# Comparing `tmp/ddreport-4.0.tar.gz` & `tmp/ddreport-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddreport-4.0.tar", last modified: Sat May  6 08:11:59 2023, max compression
+gzip compressed data, was "ddreport-4.1.tar", last modified: Thu Jun  8 08:38:22 2023, max compression
```

## Comparing `ddreport-4.0.tar` & `ddreport-4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.629799 ddreport-4.0/
--rw-rw-rw-   0        0        0       27 2022-11-03 01:34:06.000000 ddreport-4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      496 2023-05-06 08:11:59.629799 ddreport-4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.584015 ddreport-4.0/ddreport/
--rw-rw-rw-   0        0        0        0 2022-11-02 07:43:40.000000 ddreport-4.0/ddreport/__init__.py
--rw-rw-rw-   0        0        0     7107 2023-04-23 03:57:17.000000 ddreport-4.0/ddreport/api.py
--rw-rw-rw-   0        0        0     2554 2023-04-27 06:51:09.000000 ddreport-4.0/ddreport/db.py
--rw-rw-rw-   0        0        0      389 2023-04-22 12:51:35.000000 ddreport-4.0/ddreport/exceptd.py
--rw-rw-rw-   0        0        0     3756 2023-04-27 12:20:47.000000 ddreport-4.0/ddreport/func.py
--rw-rw-rw-   0        0        0     2016 2023-05-04 09:10:09.000000 ddreport-4.0/ddreport/handle.py
--rw-rw-rw-   0        0        0     1175 2023-03-08 10:44:46.000000 ddreport-4.0/ddreport/orm.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.629799 ddreport-4.0/ddreport/template/
--rw-rw-rw-   0        0        0    20482 2023-04-28 01:19:06.000000 ddreport-4.0/ddreport/template/index.html
--rw-rw-rw-   0        0        0    11205 2023-04-24 09:38:45.000000 ddreport-4.0/ddreport/testReport.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:11:59.617744 ddreport-4.0/ddreport.egg-info/
--rw-rw-rw-   0        0        0      496 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 08:11:59.000000 ddreport-4.0/ddreport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 08:11:59.629799 ddreport-4.0/setup.cfg
--rw-rw-rw-   0        0        0     1621 2023-04-26 03:12:31.000000 ddreport-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.878338 ddreport-4.1/
+-rw-rw-rw-   0        0        0       27 2022-11-03 01:34:06.000000 ddreport-4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      437 2023-06-08 08:38:22.878338 ddreport-4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.811053 ddreport-4.1/ddreport/
+-rw-rw-rw-   0        0        0        0 2022-11-02 07:43:40.000000 ddreport-4.1/ddreport/__init__.py
+-rw-rw-rw-   0        0        0     8128 2023-06-08 08:30:41.000000 ddreport-4.1/ddreport/api.py
+-rw-rw-rw-   0        0        0     2554 2023-04-27 06:51:09.000000 ddreport-4.1/ddreport/db.py
+-rw-rw-rw-   0        0        0      389 2023-04-22 12:51:35.000000 ddreport-4.1/ddreport/exceptd.py
+-rw-rw-rw-   0        0        0     4039 2023-06-08 08:05:35.000000 ddreport-4.1/ddreport/func.py
+-rw-rw-rw-   0        0        0     2016 2023-05-04 09:10:09.000000 ddreport-4.1/ddreport/handle.py
+-rw-rw-rw-   0        0        0     1175 2023-03-08 10:44:46.000000 ddreport-4.1/ddreport/orm.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.875345 ddreport-4.1/ddreport/template/
+-rw-rw-rw-   0        0        0    20482 2023-04-28 01:19:06.000000 ddreport-4.1/ddreport/template/index.html
+-rw-rw-rw-   0        0        0    11672 2023-06-08 08:03:55.000000 ddreport-4.1/ddreport/testReport.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:38:22.839039 ddreport-4.1/ddreport.egg-info/
+-rw-rw-rw-   0        0        0      437 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 08:38:22.000000 ddreport-4.1/ddreport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 08:38:22.878338 ddreport-4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1562 2023-06-08 08:37:51.000000 ddreport-4.1/setup.py
```

### Comparing `ddreport-4.0/ddreport/api.py` & `ddreport-4.1/ddreport/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         self.__typed = value
 
 
 class CustomQuery():
     def __init__(self, gg, host=''):
         self.__HOST = host
         self.__GG = gg
+        self.session = requests.session()
 
     def __assert(self, r, is_json, assert_list, E, Q):
         if not assert_list:
             if r.status_code != 200:
                 E.typed = 20                                                                           # 状态码错误
                 E.msg_dict = dict(status_code=r.status_code)
                 ExceptInfo(Q, E).raised()
@@ -150,24 +151,44 @@
             asserts = kwargs["asserts"]
             del kwargs['asserts']
         if "encode" in kwargs.keys():
             encode = kwargs["encode"]
             del kwargs['encode']
         if not kwargs['url'].startswith('http'):
             kwargs['url'] = self.__HOST + kwargs['url']
-        Q.query = kwargs
+
+        kwargs_copy = kwargs.copy()
+        if ("verify" not in kwargs_copy.keys()) and (self.__HOST.startswith("https")):
+            kwargs_copy['verify'] = self.session.verify
+        try:
+            if "headers" in kwargs_copy.keys() and kwargs_copy['headers']:
+                if self.session.headers:
+                    self.session.headers.update(kwargs_copy['headers'])
+            if self.session.headers:
+                kwargs_copy['headers'] = dict(self.session.headers)
+        except Exception:
+            kwargs_copy['headers'] = dict(self.session.headers)
         try:
-            r = requests.request(**kwargs)
+            if "cookies" in kwargs_copy.keys() and kwargs_copy['cookies']:
+                if self.session.cookies:
+                    self.session.cookies.update(kwargs_copy['cookies'])
+            if self.session.cookies:
+                kwargs_copy['cookies'] = self.session.cookies.get_dict()
+        except Exception:
+            kwargs_copy['cookies'] = self.session.cookies.get_dict()
+        Q.query = kwargs_copy
+        try:
+            r = self.session.request(**kwargs)
             r.encoding = encode
             status_code = r.status_code
             headers = dict(r.headers)
             cookies = r.cookies.get_dict()
-            if "application/json" in headers['Content-Type']:
+            try:
                 response, is_json = r.json(), True
-            else:
+            except Exception:
                 response, is_json = r.text, False
             Q.status_code, Q.resp_headers, Q.resp_cookies, Q.response = status_code, headers, cookies, response
             self.__GG.set("@@ddreportQuery", Q)
         except Exception:
             E.typed = 10
             E.msg_dict = traceback.format_exc()
             ExceptInfo(Q, E).raised()
```

### Comparing `ddreport-4.0/ddreport/db.py` & `ddreport-4.1/ddreport/db.py`

 * *Files identical despite different names*

### Comparing `ddreport-4.0/ddreport/func.py` & `ddreport-4.1/ddreport/func.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,8 +94,18 @@
         base64_img_str = f"data:image/{img_type};base64," + base64.b64encode(img_obj).decode(*agrs, **kwargs)
         return base64_img_str
 
     # 数据比对
     def dataDiff(self, data1, data2, **kwargs):
         diff = DeepDiff(data1, data2, **kwargs)
         if diff:
-            raise AssertionError(diff.pretty())
+            raise AssertionError(diff.pretty())
+
+    # url元组
+    def getUrl(self, url):
+        from urllib.parse import urlparse
+        return urlparse(url)
+
+    # 字典cookies转cookiejar格式
+    def toCookiejar(self, data: dict):
+        import requests
+        return requests.utils.cookiejar_from_dict(data)
```

### Comparing `ddreport-4.0/ddreport/handle.py` & `ddreport-4.1/ddreport/handle.py`

 * *Files identical despite different names*

### Comparing `ddreport-4.0/ddreport/orm.py` & `ddreport-4.1/ddreport/orm.py`

 * *Files identical despite different names*

### Comparing `ddreport-4.0/ddreport/template/index.html` & `ddreport-4.1/ddreport/template/index.html`

 * *Files identical despite different names*

### Comparing `ddreport-4.0/ddreport/testReport.py` & `ddreport-4.1/ddreport/testReport.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     def extend(self, key, value):
         self.__value.get(key).extend(value)
 
 GG = Gvalues()
 
 
-dd_paramet = {"ddreport": None}
+dd_paramet = dict()
 
 
 def getEnvData(env_path, env_name):
     try:
         with open(env_path, 'r', encoding='utf-8')as f:
             envs = json.loads(f.read())
         return jsonpath(envs, f'$..[?(@.env_name=="{env_name}")]')[0]
@@ -243,16 +243,26 @@
 
 @pytest.hookimpl(tryfirst=True, hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     outcome = yield
     report = outcome.get_result()
     call.duration = '%.2f' % call.duration          # 科学计数转普通格式
     if report.when == 'call':
-        if "ddreport" in item.funcargs.keys():
-            dd_paramet["ddreport"] = item.funcargs['ddreport']
+        # 过滤不需要的funcargs
+        dd_paramet.clear()
+        params_keys = [om.args[0] for om in item.own_markers]
+        for k in item.fixturenames:
+            if k in ["_session_faker", "request"]:
+                continue
+            elif k.startswith("dd__"):
+                continue
+            elif params_keys and k in params_keys:
+                continue
+            else:
+                dd_paramet[k] = item.funcargs[k]
         test_result[report.outcome] += 1
         info = node_handle(report, item, call)
         test_result["cases"].append(info)
         GG.set("@@ddreportQuery", None)
         GG.set("@ddimg", None)
     elif report.outcome == 'failed':
         report.outcome = 'error'
@@ -316,18 +326,21 @@
                 new_item.callspec.params[key] = paramet
                 new_item.callspec.indices[key] = n
                 new_item.callspec._idlist.append(f"{key}{n}")
                 del new_item.callspec._idlist[0]
                 new_item.name = new_item.originalname + f"[{key}{n}]"
                 new_nodeid = '::'.join(new_item.nodeid.split("::")[:-1] + [new_item.name])
                 new_item._nodeid = new_nodeid
-                new_item.funcargs["ddreport"] = dd_paramet["ddreport"]
-                new_item.ihook.pytest_runtest_logstart(nodeid=new_nodeid, location=item.location)
+                for k, v in dd_paramet.items():
+                    new_item.funcargs[k] = dd_paramet[k]
+                #new_item.ihook.pytest_runtest_logstart(nodeid=new_nodeid, location=item.location)
                 runtestprotocol(new_item, nextitem=None)
-                new_item.ihook.pytest_runtest_logfinish(nodeid=new_item.nodeid, location=item.location)
+                #new_item.ihook.pytest_runtest_logfinish(nodeid=new_item._nodeid, location=item.location)
             return True
-
+    else:
+        for k, v in dd_paramet.items():
+            item.funcargs[k] = dd_paramet[k]
 
 def pytest_report_teststatus(config, report):
     # 更新终端打印（.  s   F  E）
     if report.outcome == 'error':
         return report.outcome, 'E', None
```

### Comparing `ddreport-4.0/setup.py` & `ddreport-4.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 #### 每次更新需要修改 version 字段
 
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name = "ddreport",
-    version = "4.0",
+    version = "4.1",
     keywords = ("pip", "pytest", "testReport"),
     description = "pytest测试报告",
-    long_description = "1.增加正确的请求展示；2.增加用例运行时动态添加用例；3.添加测试报告中展示图片逻辑；4.api请求优化；5.异常信息优化；6.测试报告优化；7.数据对比采用deepdiff库",
+    long_description = "1.request使用session；2.解决动态化参数中调用其他fixture不生效问题；3.解决响应头获取content-type失败后，无法确定响应内容类型问题",
     license = "MIT Licence",
 
-    url = "https://gitee.com/duanliangcong/dlc_pytest-report.git",
+    url = "https://gitee.com/duanliangcong/ddreport",
     author = "duanliangcong",
     author_email = "137562703@qq.com",
     entry_points={"pytest11": ["test_report=ddreport.testReport"]},
 
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
```

