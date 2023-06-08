# Comparing `tmp/dataqualityx-0.1.0.tar.gz` & `tmp/dataqualityx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataqualityx-0.1.0.tar", last modified: Wed Jun  7 10:07:39 2023, max compression
+gzip compressed data, was "dataqualityx-0.1.1.tar", last modified: Thu Jun  8 05:42:04 2023, max compression
```

## Comparing `dataqualityx-0.1.0.tar` & `dataqualityx-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:39.201825 dataqualityx-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-06-05 03:43:08.000000 dataqualityx-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      390 2023-06-07 10:07:39.200821 dataqualityx-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-06-07 08:36:11.000000 dataqualityx-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:39.176232 dataqualityx-0.1.0/dataqualityx/
--rw-rw-rw-   0        0        0      749 2023-06-05 07:03:28.000000 dataqualityx-0.1.0/dataqualityx/AlterUtil.py
--rw-rw-rw-   0        0        0     1041 2023-06-01 09:53:40.000000 dataqualityx-0.1.0/dataqualityx/DateUtil.py
--rw-rw-rw-   0        0        0      628 2023-06-05 07:02:28.000000 dataqualityx-0.1.0/dataqualityx/DbUtil.py
--rw-rw-rw-   0        0        0       40 2023-06-07 09:31:10.000000 dataqualityx-0.1.0/dataqualityx/__init__.py
--rw-rw-rw-   0        0        0     4699 2023-06-06 01:46:25.000000 dataqualityx-0.1.0/dataqualityx/app.py
-drwxrwxrwx   0        0        0        0 2023-06-07 10:07:39.198822 dataqualityx-0.1.0/dataqualityx.egg-info/
--rw-rw-rw-   0        0        0      390 2023-06-07 10:07:39.000000 dataqualityx-0.1.0/dataqualityx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-07 10:07:39.000000 dataqualityx-0.1.0/dataqualityx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 10:07:39.000000 dataqualityx-0.1.0/dataqualityx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-07 10:07:39.000000 dataqualityx-0.1.0/dataqualityx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-07 10:07:39.000000 dataqualityx-0.1.0/dataqualityx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 10:07:39.201825 dataqualityx-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      688 2023-06-07 10:07:35.000000 dataqualityx-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:42:04.654614 dataqualityx-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 10:17:50.000000 dataqualityx-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1570 2023-06-08 05:42:04.653613 dataqualityx-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2023-06-08 05:38:16.000000 dataqualityx-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 05:42:04.640100 dataqualityx-0.1.1/dataqualityx/
+-rw-rw-rw-   0        0        0      749 2023-06-07 10:17:50.000000 dataqualityx-0.1.1/dataqualityx/AlterUtil.py
+-rw-rw-rw-   0        0        0     1041 2023-06-07 10:17:50.000000 dataqualityx-0.1.1/dataqualityx/DateUtil.py
+-rw-rw-rw-   0        0        0      628 2023-06-07 10:17:50.000000 dataqualityx-0.1.1/dataqualityx/DbUtil.py
+-rw-rw-rw-   0        0        0       40 2023-06-08 05:42:01.000000 dataqualityx-0.1.1/dataqualityx/__init__.py
+-rw-rw-rw-   0        0        0     5140 2023-06-08 03:47:09.000000 dataqualityx-0.1.1/dataqualityx/app.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:42:04.651611 dataqualityx-0.1.1/dataqualityx.egg-info/
+-rw-rw-rw-   0        0        0     1570 2023-06-08 05:42:04.000000 dataqualityx-0.1.1/dataqualityx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-08 05:42:04.000000 dataqualityx-0.1.1/dataqualityx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 05:42:04.000000 dataqualityx-0.1.1/dataqualityx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-08 05:42:04.000000 dataqualityx-0.1.1/dataqualityx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 05:42:04.000000 dataqualityx-0.1.1/dataqualityx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 05:42:04.654614 dataqualityx-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-06-08 05:41:44.000000 dataqualityx-0.1.1/setup.py
```

### Comparing `dataqualityx-0.1.0/LICENSE` & `dataqualityx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataqualityx-0.1.0/dataqualityx/AlterUtil.py` & `dataqualityx-0.1.1/dataqualityx/AlterUtil.py`

 * *Files identical despite different names*

### Comparing `dataqualityx-0.1.0/dataqualityx/DateUtil.py` & `dataqualityx-0.1.1/dataqualityx/DateUtil.py`

 * *Files identical despite different names*

### Comparing `dataqualityx-0.1.0/dataqualityx/DbUtil.py` & `dataqualityx-0.1.1/dataqualityx/DbUtil.py`

 * *Files identical despite different names*

### Comparing `dataqualityx-0.1.0/dataqualityx/app.py` & `dataqualityx-0.1.1/dataqualityx/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -71,32 +71,41 @@
     for x, y in zip(actual, exps):
         if len(x) > 1:
             raise Exception(f'目前只支持校验一个字段值，文件: {file_name}')
         calc_res = symbol_proc(x[0], y)
         if calc_res == False:
             err_info = f'错误xxx: 文件:{file_name} 中的 {sql} 计算出问题了, 实际结果是 {actual}, 但期望是 {task["expected"]}'
             print_color_text(err_info, 'red')
-            if 'none' in args.alerts: continue
+            if args.alerts is not None and 'none' in args.alerts: continue
             if task['alerts'] is not None:
                 for alert in task['alerts']:
                     alert = alert['alert']
                     AlterUtil.alter(alert['type'], err_info, alert['url'])
         else:
             print(f'文件:{file_name} 中的 {sql} 与期望值相同')
         print('--------------------------------------------')
 
 
 # 读取 yaml 中的数据
 def read_yaml(args):
-    current_path = os.path.abspath(".")
-    yaml_path = os.path.join(current_path, "../task")
+    if args.files is None:
+        raise Exception(f'请指定脚本路径, 例如 --files /home/user/xxx')
+    yaml_path = args.files
     infos = []
-    for filename in os.listdir(yaml_path):
-        # 支持命令行指定文件,如果不写就是全部
-        if args.files is None or filename in args.files:
+    # 检查指定路径是文件还是文件夹
+    if os.path.isfile(yaml_path):
+        # 如果是文件，则读取文件内容
+        with open(yaml_path, encoding='utf-8') as f:
+            yaml_data = yaml.safe_load(f)
+            yaml_data['file_name'] = os.path.basename(yaml_path)
+            infos.append(yaml_data)
+    else:
+        # 如果是文件夹，则列出文件夹中的所有文件/文件夹名称
+        for filename in os.listdir(yaml_path):
+            # 支持命令行指定文件,如果不写就是全部
             if filename.endswith('.yaml'):
                 with open(os.path.join(yaml_path, filename), encoding='utf-8') as f:
                     yaml_data = yaml.safe_load(f)
                     yaml_data['file_name'] = filename
                     infos.append(yaml_data)
     return infos
 
@@ -125,15 +134,15 @@
             sql = handle_sql(task['sql'], info['vars'])
             actualRes = DbUtil.query(cur, sql)
             compareResult(actualRes, info["file_name"], sql, task, args)
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('--files', dest='files', nargs='+', help='YAML files to process')
+    parser.add_argument('--files', dest='files', help='YAML files to process')
     parser.add_argument('--alerts', dest='alerts', nargs='+', help='YAML alerts to process')
     args = parser.parse_args()
     yaml_infos = read_yaml(args)
     process(yaml_infos, args)
 
 
 if __name__ == '__main__':
```

### Comparing `dataqualityx-0.1.0/setup.py` & `dataqualityx-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import shutil
 import subprocess
 
 from setuptools import find_packages, setup
 
 from dataqualityx import NAME, VERSION
 
-with open("README.md", "r") as f:
+
+shutil.rmtree('./dist')
+shutil.rmtree('./dataqualityx.egg-info')
+shutil.rmtree('./build')
+
+with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=NAME,
     version=VERSION,
     author="zzzzzzzs",
     author_email="1443539042@qq.com",
```

