# Comparing `tmp/charset_mnbvc-0.0.6.tar.gz` & `tmp/charset_mnbvc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charset_mnbvc-0.0.6.tar", last modified: Fri May 26 06:35:44 2023, max compression
+gzip compressed data, was "charset_mnbvc-0.0.7.tar", last modified: Thu Jun  8 01:59:34 2023, max compression
```

## Comparing `charset_mnbvc-0.0.6.tar` & `charset_mnbvc-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-26 06:35:44.724753 charset_mnbvc-0.0.6/
--rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.6/LICENSE
--rw-r--r--   0 alan       (501) staff       (20)     9748 2023-05-26 06:35:44.724596 charset_mnbvc-0.0.6/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)     9108 2023-03-27 15:02:20.000000 charset_mnbvc-0.0.6/README.md
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-26 06:35:44.724008 charset_mnbvc-0.0.6/charset_mnbvc/
--rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.6/charset_mnbvc/__init__.py
--rw-r--r--   0 alan       (501) staff       (20)     3109 2023-04-06 08:14:07.000000 charset_mnbvc-0.0.6/charset_mnbvc/api.py
--rw-r--r--   0 alan       (501) staff       (20)      453 2023-05-26 03:45:39.000000 charset_mnbvc-0.0.6/charset_mnbvc/common_utils.py
--rw-r--r--   0 alan       (501) staff       (20)     2902 2023-03-27 14:46:45.000000 charset_mnbvc-0.0.6/charset_mnbvc/constant.py
--rw-r--r--   0 alan       (501) staff       (20)     1144 2023-05-26 06:34:46.000000 charset_mnbvc-0.0.6/charset_mnbvc/verify.py
--rw-r--r--   0 alan       (501) staff       (20)       70 2023-05-26 03:30:47.000000 charset_mnbvc-0.0.6/charset_mnbvc/version.py
-drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-05-26 06:35:44.724430 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/
--rw-r--r--   0 alan       (501) staff       (20)     9748 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/PKG-INFO
--rw-r--r--   0 alan       (501) staff       (20)      326 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (501) staff       (20)        1 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (501) staff       (20)       14 2023-05-26 06:35:44.000000 charset_mnbvc-0.0.6/charset_mnbvc.egg-info/top_level.txt
--rw-r--r--   0 alan       (501) staff       (20)       38 2023-05-26 06:35:44.724795 charset_mnbvc-0.0.6/setup.cfg
--rw-r--r--   0 alan       (501) staff       (20)      962 2023-05-26 03:31:25.000000 charset_mnbvc-0.0.6/setup.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-06-08 01:59:34.334869 charset_mnbvc-0.0.7/
+-rw-r--r--   0 alan       (501) staff       (20)     1064 2023-02-09 08:52:50.000000 charset_mnbvc-0.0.7/LICENSE
+-rw-r--r--   0 alan       (501) staff       (20)    12261 2023-06-08 01:59:34.334678 charset_mnbvc-0.0.7/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)    11621 2023-06-08 01:44:43.000000 charset_mnbvc-0.0.7/README.md
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-06-08 01:59:34.333996 charset_mnbvc-0.0.7/charset_mnbvc/
+-rw-r--r--   0 alan       (501) staff       (20)        0 2023-02-09 02:34:27.000000 charset_mnbvc-0.0.7/charset_mnbvc/__init__.py
+-rw-r--r--   0 alan       (501) staff       (20)     4674 2023-06-05 07:27:58.000000 charset_mnbvc-0.0.7/charset_mnbvc/api.py
+-rw-r--r--   0 alan       (501) staff       (20)      453 2023-05-26 03:45:39.000000 charset_mnbvc-0.0.7/charset_mnbvc/common_utils.py
+-rw-r--r--   0 alan       (501) staff       (20)     2902 2023-03-27 14:46:45.000000 charset_mnbvc-0.0.7/charset_mnbvc/constant.py
+-rw-r--r--   0 alan       (501) staff       (20)     1144 2023-05-26 06:34:46.000000 charset_mnbvc-0.0.7/charset_mnbvc/verify.py
+-rw-r--r--   0 alan       (501) staff       (20)       70 2023-06-08 01:59:32.000000 charset_mnbvc-0.0.7/charset_mnbvc/version.py
+drwxr-xr-x   0 alan       (501) staff       (20)        0 2023-06-08 01:59:34.334493 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/
+-rw-r--r--   0 alan       (501) staff       (20)    12261 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (501) staff       (20)      326 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (501) staff       (20)        1 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (501) staff       (20)       14 2023-06-08 01:59:34.000000 charset_mnbvc-0.0.7/charset_mnbvc.egg-info/top_level.txt
+-rw-r--r--   0 alan       (501) staff       (20)       38 2023-06-08 01:59:34.334986 charset_mnbvc-0.0.7/setup.cfg
+-rw-r--r--   0 alan       (501) staff       (20)      962 2023-05-26 03:31:25.000000 charset_mnbvc-0.0.7/setup.py
```

### Comparing `charset_mnbvc-0.0.6/LICENSE` & `charset_mnbvc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.6/PKG-INFO` & `charset_mnbvc-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,10 @@
-Metadata-Version: 2.1
-Name: charset_mnbvc
-Version: 0.0.6
-Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
-Home-page: https://github.com/alanshi/charset_mnbvc
-Author: Alan Shi
-Author-email: alan.shi86@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
-Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ### 项目描述
 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 
-#### 实现机制
-1. 读取每个文件的前500个字符(长度可定义)
-2. 尝试使用4种编码对字符进行decode ```utf_8```,```utf_16```,```gb18030```,```big5```
-3. 将每一组decode的结果对中文字符串和常用中文字进行正则匹配,有匹配结果的表明符合编码要求
-4. 当charset-mnbvc无法检测编码或检测到多个编码结果时,会自动调用cchardect进行备用检测机制
 
 #### 模块安装
 ```
 pip install charset-mnbvc
 ```
 
 #### charset-mnbvc pypi url:
@@ -51,14 +29,39 @@
 
 file_path = "test.txt"
 coding_name = get_cn_charset(file_path)
 print(f"文件名: {file_path}, 编码: {coding_name}")
 
 ```
 
+##### 获取二进制数据编码
+```
+from charset_mnbvc import api
+
+with open("tests/fixtures/10.txt", "rb") as f:
+    data = f.read()
+    coding_name = api.from_data(data=data, mode=2)
+    print(f"数据编码: {coding_name}")
+```
+
+###### 转换二进制数据编码
+```
+from charset_mnbvc import api
+
+source_data = b'\xb5\xda\xcb\xc4\xd5\xc2' #gbk 编码
+
+ret = api.convert_encoding(
+    source_data=source_data,
+    source_encoding="gbk",
+    target_encoding="utf-8",
+)
+print(ret)
+```
+
+
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
 2: 将文本使用utf-8格式覆盖到test.txt
 
@@ -74,31 +77,55 @@
   -c, --cchardet        使用cchardet方案
   -i inputDirectory     inputDirectory为需要检测的目录
   -step PROCESS_STEP    执行步骤,1为编码检测,2为编码转换
   -r result_file_name   指定编码检测结果文件名
   -u                    恢复文件
 ```
 编码检测范例:
-`python convert_files.py -i /Downloads/20230109 -step 1 -r check_result.csv`
+`python convert_files.py -i /Users/alan/temp_test -step 1 -r check_result.csv`
 
 ```
-编码检测进度: 100%|████████████████████████████| 5609/5609 [00:00<00:00, 9462.80it/s]
-已将检测结果保存至check_results.csv文件中,请查阅!
+###################################### Step1 start ######################################
+编码检测进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2152/2152 [00:00<00:00, 3275.19it/s]
+已将检测结果保存至check_result.csv文件中,请查阅!
+###################################### Step1 end ######################################
+```
+
+编码转换 范例(转换完毕后自动加入step3 用于二次验证已转换为utf-8的文件是否正常):
+`python convert_files.py -i /Users/alan/temp_test -step 2 -r check_result.csv`
+```
+###################################### Step2 start ######################################
+编码转换进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2152/2152 [00:00<00:00, 5229.08it/s]
+总文件数: 2152
+转换成功文件数: 2143
+转换失败文件数: 9
+/Users/alan/temp_test/mop/xxx.txt gb18030 转换到utf8失败, 'gb18030' codec can't decode byte 0xff in position 4567: illegal multibyte sequence
+/Users/alan/temp_test/mop/larry vs psplayer.txt gb18030 转换到utf8失败, 'gb18030' codec can't
+###################################### Step2 end ######################################
+###################################### Step3 start ######################################
+文件二次验证开始
+检测目录: /Users/alan/temp_test
+编码转换进度: 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████| 2134/2134 [00:00<00:00, 27680.81it/s]
+文件二次验证结束
+所有已转换为utf-8的txt文件验证完成!
+###################################### Step3 end ######################################
+......
 ```
 
-编码转换 范例:
-`python convert_files.py -i /Downloads/20230101 -step 2 -r check_result.csv`
+单独进行utf-8文件二次验证:
+`python convert_files.py -i /Users/alan/temp_test -step 3 -r check_result.csv`
+
 ```
-编码转换进度: 100%|████████████████████████████| 5621/5621 [00:33<00:00, 169.93it/s]
-总文件数: 5621
-转换成功文件数: 5609
-转换失败文件数: 12
-/Users/alan/Downloads/20230109/zlibrary.20230109.1.杂书/5695175.txt 转换失败, 编码格式错误: 可能是文件内容为空!
-/Users/alan/Downloads/20230109/zlibrary.20230109.1.杂书/5753250.txt 转换失败, 编码格式错误: 可能是文件内容为空!
-......
+###################################### Step3 start ######################################
+文件二次验证开始
+检测目录: /Users/alan/temp_test
+验证进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2134/2134 [00:00<00:00, 8758.18it/s]
+文件二次验证结束
+所有已转换为utf-8的txt文件验证完成!
+###################################### Step3 end ######################################
 ```
 
 测试环境说明（开发测试用机):
 * MacBook Air Apple M2, 内存:16 GB, 硬盘:512G, 系统版本:13.2 (22D49)**, Python 3.9.6
 * 默认使用charset_mnbvc方案, 可切换使用cchardet方案
 
 目前存在的问题:
@@ -186,9 +213,7 @@
 
 现在解决这个问题的最简单的思路是换一种语言实现编码转换或者在Python中引入Java的库对MS936编码进行正确处理。
 
 
 
 
 
-
-
```

### Comparing `charset_mnbvc-0.0.6/README.md` & `charset_mnbvc-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1
+Name: charset_mnbvc
+Version: 0.0.7
+Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
+Home-page: https://github.com/alanshi/charset_mnbvc
+Author: Alan Shi
+Author-email: alan.shi86@gmail.com
+License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
+Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ### 项目描述
 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 
-#### 实现机制
-1. 读取每个文件的前500个字符(长度可定义)
-2. 尝试使用4种编码对字符进行decode ```utf_8```,```utf_16```,```gb18030```,```big5```
-3. 将每一组decode的结果对中文字符串和常用中文字进行正则匹配,有匹配结果的表明符合编码要求
-4. 当charset-mnbvc无法检测编码或检测到多个编码结果时,会自动调用cchardect进行备用检测机制
 
 #### 模块安装
 ```
 pip install charset-mnbvc
 ```
 
 #### charset-mnbvc pypi url:
@@ -34,14 +46,39 @@
 
 file_path = "test.txt"
 coding_name = get_cn_charset(file_path)
 print(f"文件名: {file_path}, 编码: {coding_name}")
 
 ```
 
+##### 获取二进制数据编码
+```
+from charset_mnbvc import api
+
+with open("tests/fixtures/10.txt", "rb") as f:
+    data = f.read()
+    coding_name = api.from_data(data=data, mode=2)
+    print(f"数据编码: {coding_name}")
+```
+
+###### 转换二进制数据编码
+```
+from charset_mnbvc import api
+
+source_data = b'\xb5\xda\xcb\xc4\xd5\xc2' #gbk 编码
+
+ret = api.convert_encoding(
+    source_data=source_data,
+    source_encoding="gbk",
+    target_encoding="utf-8",
+)
+print(ret)
+```
+
+
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
 2: 将文本使用utf-8格式覆盖到test.txt
 
@@ -57,31 +94,55 @@
   -c, --cchardet        使用cchardet方案
   -i inputDirectory     inputDirectory为需要检测的目录
   -step PROCESS_STEP    执行步骤,1为编码检测,2为编码转换
   -r result_file_name   指定编码检测结果文件名
   -u                    恢复文件
 ```
 编码检测范例:
-`python convert_files.py -i /Downloads/20230109 -step 1 -r check_result.csv`
+`python convert_files.py -i /Users/alan/temp_test -step 1 -r check_result.csv`
 
 ```
-编码检测进度: 100%|████████████████████████████| 5609/5609 [00:00<00:00, 9462.80it/s]
-已将检测结果保存至check_results.csv文件中,请查阅!
+###################################### Step1 start ######################################
+编码检测进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2152/2152 [00:00<00:00, 3275.19it/s]
+已将检测结果保存至check_result.csv文件中,请查阅!
+###################################### Step1 end ######################################
+```
+
+编码转换 范例(转换完毕后自动加入step3 用于二次验证已转换为utf-8的文件是否正常):
+`python convert_files.py -i /Users/alan/temp_test -step 2 -r check_result.csv`
+```
+###################################### Step2 start ######################################
+编码转换进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2152/2152 [00:00<00:00, 5229.08it/s]
+总文件数: 2152
+转换成功文件数: 2143
+转换失败文件数: 9
+/Users/alan/temp_test/mop/xxx.txt gb18030 转换到utf8失败, 'gb18030' codec can't decode byte 0xff in position 4567: illegal multibyte sequence
+/Users/alan/temp_test/mop/larry vs psplayer.txt gb18030 转换到utf8失败, 'gb18030' codec can't
+###################################### Step2 end ######################################
+###################################### Step3 start ######################################
+文件二次验证开始
+检测目录: /Users/alan/temp_test
+编码转换进度: 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████| 2134/2134 [00:00<00:00, 27680.81it/s]
+文件二次验证结束
+所有已转换为utf-8的txt文件验证完成!
+###################################### Step3 end ######################################
+......
 ```
 
-编码转换 范例:
-`python convert_files.py -i /Downloads/20230101 -step 2 -r check_result.csv`
+单独进行utf-8文件二次验证:
+`python convert_files.py -i /Users/alan/temp_test -step 3 -r check_result.csv`
+
 ```
-编码转换进度: 100%|████████████████████████████| 5621/5621 [00:33<00:00, 169.93it/s]
-总文件数: 5621
-转换成功文件数: 5609
-转换失败文件数: 12
-/Users/alan/Downloads/20230109/zlibrary.20230109.1.杂书/5695175.txt 转换失败, 编码格式错误: 可能是文件内容为空!
-/Users/alan/Downloads/20230109/zlibrary.20230109.1.杂书/5753250.txt 转换失败, 编码格式错误: 可能是文件内容为空!
-......
+###################################### Step3 start ######################################
+文件二次验证开始
+检测目录: /Users/alan/temp_test
+验证进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2134/2134 [00:00<00:00, 8758.18it/s]
+文件二次验证结束
+所有已转换为utf-8的txt文件验证完成!
+###################################### Step3 end ######################################
 ```
 
 测试环境说明（开发测试用机):
 * MacBook Air Apple M2, 内存:16 GB, 硬盘:512G, 系统版本:13.2 (22D49)**, Python 3.9.6
 * 默认使用charset_mnbvc方案, 可切换使用cchardet方案
 
 目前存在的问题:
@@ -169,7 +230,9 @@
 
 现在解决这个问题的最简单的思路是换一种语言实现编码转换或者在Python中引入Java的库对MS936编码进行正确处理。
 
 
 
 
 
+
+
```

### Comparing `charset_mnbvc-0.0.6/charset_mnbvc/constant.py` & `charset_mnbvc-0.0.7/charset_mnbvc/constant.py`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.6/charset_mnbvc/verify.py` & `charset_mnbvc-0.0.7/charset_mnbvc/verify.py`

 * *Files identical despite different names*

### Comparing `charset_mnbvc-0.0.6/charset_mnbvc.egg-info/PKG-INFO` & `charset_mnbvc-0.0.7/charset_mnbvc.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charset-mnbvc
-Version: 0.0.6
+Version: 0.0.7
 Summary: 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 Home-page: https://github.com/alanshi/charset_mnbvc
 Author: Alan Shi
 Author-email: alan.shi86@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/alanshi/charset_mnbvc/issues
 Project-URL: Source, https://github.com/alanshi/charset_mnbvc/
@@ -14,19 +14,14 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### 项目描述
 本项目旨在对大量文本文件进行快速编码检测以辅助mnbvc语料集项目的数据清洗工作
 
-#### 实现机制
-1. 读取每个文件的前500个字符(长度可定义)
-2. 尝试使用4种编码对字符进行decode ```utf_8```,```utf_16```,```gb18030```,```big5```
-3. 将每一组decode的结果对中文字符串和常用中文字进行正则匹配,有匹配结果的表明符合编码要求
-4. 当charset-mnbvc无法检测编码或检测到多个编码结果时,会自动调用cchardect进行备用检测机制
 
 #### 模块安装
 ```
 pip install charset-mnbvc
 ```
 
 #### charset-mnbvc pypi url:
@@ -51,14 +46,39 @@
 
 file_path = "test.txt"
 coding_name = get_cn_charset(file_path)
 print(f"文件名: {file_path}, 编码: {coding_name}")
 
 ```
 
+##### 获取二进制数据编码
+```
+from charset_mnbvc import api
+
+with open("tests/fixtures/10.txt", "rb") as f:
+    data = f.read()
+    coding_name = api.from_data(data=data, mode=2)
+    print(f"数据编码: {coding_name}")
+```
+
+###### 转换二进制数据编码
+```
+from charset_mnbvc import api
+
+source_data = b'\xb5\xda\xcb\xc4\xd5\xc2' #gbk 编码
+
+ret = api.convert_encoding(
+    source_data=source_data,
+    source_encoding="gbk",
+    target_encoding="utf-8",
+)
+print(ret)
+```
+
+
 #### 编码转换使用范例:
 NOTICE: 文件默认转换为utf-8格式, 文件转换前后会将原始文件原地复制为raw格式用于备份, 并用utf-8格式覆盖原始文件, 操作流程如下:
 
 1: 原地复制test.txt 到 test.raw
 
 2: 将文本使用utf-8格式覆盖到test.txt
 
@@ -74,31 +94,55 @@
   -c, --cchardet        使用cchardet方案
   -i inputDirectory     inputDirectory为需要检测的目录
   -step PROCESS_STEP    执行步骤,1为编码检测,2为编码转换
   -r result_file_name   指定编码检测结果文件名
   -u                    恢复文件
 ```
 编码检测范例:
-`python convert_files.py -i /Downloads/20230109 -step 1 -r check_result.csv`
+`python convert_files.py -i /Users/alan/temp_test -step 1 -r check_result.csv`
 
 ```
-编码检测进度: 100%|████████████████████████████| 5609/5609 [00:00<00:00, 9462.80it/s]
-已将检测结果保存至check_results.csv文件中,请查阅!
+###################################### Step1 start ######################################
+编码检测进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2152/2152 [00:00<00:00, 3275.19it/s]
+已将检测结果保存至check_result.csv文件中,请查阅!
+###################################### Step1 end ######################################
+```
+
+编码转换 范例(转换完毕后自动加入step3 用于二次验证已转换为utf-8的文件是否正常):
+`python convert_files.py -i /Users/alan/temp_test -step 2 -r check_result.csv`
+```
+###################################### Step2 start ######################################
+编码转换进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2152/2152 [00:00<00:00, 5229.08it/s]
+总文件数: 2152
+转换成功文件数: 2143
+转换失败文件数: 9
+/Users/alan/temp_test/mop/xxx.txt gb18030 转换到utf8失败, 'gb18030' codec can't decode byte 0xff in position 4567: illegal multibyte sequence
+/Users/alan/temp_test/mop/larry vs psplayer.txt gb18030 转换到utf8失败, 'gb18030' codec can't
+###################################### Step2 end ######################################
+###################################### Step3 start ######################################
+文件二次验证开始
+检测目录: /Users/alan/temp_test
+编码转换进度: 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████| 2134/2134 [00:00<00:00, 27680.81it/s]
+文件二次验证结束
+所有已转换为utf-8的txt文件验证完成!
+###################################### Step3 end ######################################
+......
 ```
 
-编码转换 范例:
-`python convert_files.py -i /Downloads/20230101 -step 2 -r check_result.csv`
+单独进行utf-8文件二次验证:
+`python convert_files.py -i /Users/alan/temp_test -step 3 -r check_result.csv`
+
 ```
-编码转换进度: 100%|████████████████████████████| 5621/5621 [00:33<00:00, 169.93it/s]
-总文件数: 5621
-转换成功文件数: 5609
-转换失败文件数: 12
-/Users/alan/Downloads/20230109/zlibrary.20230109.1.杂书/5695175.txt 转换失败, 编码格式错误: 可能是文件内容为空!
-/Users/alan/Downloads/20230109/zlibrary.20230109.1.杂书/5753250.txt 转换失败, 编码格式错误: 可能是文件内容为空!
-......
+###################################### Step3 start ######################################
+文件二次验证开始
+检测目录: /Users/alan/temp_test
+验证进度: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 2134/2134 [00:00<00:00, 8758.18it/s]
+文件二次验证结束
+所有已转换为utf-8的txt文件验证完成!
+###################################### Step3 end ######################################
 ```
 
 测试环境说明（开发测试用机):
 * MacBook Air Apple M2, 内存:16 GB, 硬盘:512G, 系统版本:13.2 (22D49)**, Python 3.9.6
 * 默认使用charset_mnbvc方案, 可切换使用cchardet方案
 
 目前存在的问题:
```

### Comparing `charset_mnbvc-0.0.6/setup.py` & `charset_mnbvc-0.0.7/setup.py`

 * *Files identical despite different names*

