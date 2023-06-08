# Comparing `tmp/pinyintokenizer-0.0.1.tar.gz` & `tmp/pinyintokenizer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinyintokenizer-0.0.1.tar", last modified: Mon Dec 26 09:52:15 2022, max compression
+gzip compressed data, was "pinyintokenizer-0.0.2.tar", last modified: Thu Jun  8 08:04:18 2023, max compression
```

## Comparing `pinyintokenizer-0.0.1.tar` & `pinyintokenizer-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-12-26 09:52:15.423613 pinyintokenizer-0.0.1/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pinyintokenizer-0.0.1/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)     5569 2022-12-26 09:52:15.424001 pinyintokenizer-0.0.1/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     3779 2022-12-26 09:50:09.000000 pinyintokenizer-0.0.1/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-12-26 09:52:15.419597 pinyintokenizer-0.0.1/pinyintokenizer/
--rw-r--r--   0 xuming     (501) staff       (20)    14311 2022-12-26 09:37:33.000000 pinyintokenizer-0.0.1/pinyintokenizer/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2022-12-26 09:52:15.422533 pinyintokenizer-0.0.1/pinyintokenizer.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)     5569 2022-12-26 09:52:15.000000 pinyintokenizer-0.0.1/pinyintokenizer.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      258 2022-12-26 09:52:15.000000 pinyintokenizer-0.0.1/pinyintokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2022-12-26 09:52:15.000000 pinyintokenizer-0.0.1/pinyintokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        4 2022-12-26 09:52:15.000000 pinyintokenizer-0.0.1/pinyintokenizer.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       16 2022-12-26 09:52:15.000000 pinyintokenizer-0.0.1/pinyintokenizer.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)      309 2022-12-26 09:52:15.425440 pinyintokenizer-0.0.1/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1294 2022-12-26 09:37:33.000000 pinyintokenizer-0.0.1/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-08 08:04:18.846870 pinyintokenizer-0.0.2/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pinyintokenizer-0.0.2/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)     7226 2023-06-08 08:04:18.847177 pinyintokenizer-0.0.2/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     5076 2023-06-08 08:04:02.000000 pinyintokenizer-0.0.2/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-08 08:04:18.843288 pinyintokenizer-0.0.2/pinyintokenizer/
+-rw-r--r--   0 xuming     (501) staff       (20)    14294 2023-06-08 07:58:38.000000 pinyintokenizer-0.0.2/pinyintokenizer/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-08 08:04:18.846399 pinyintokenizer-0.0.2/pinyintokenizer.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)     7226 2023-06-08 08:04:18.000000 pinyintokenizer-0.0.2/pinyintokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      258 2023-06-08 08:04:18.000000 pinyintokenizer-0.0.2/pinyintokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-06-08 08:04:18.000000 pinyintokenizer-0.0.2/pinyintokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        4 2023-06-08 08:04:18.000000 pinyintokenizer-0.0.2/pinyintokenizer.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       16 2023-06-08 08:04:18.000000 pinyintokenizer-0.0.2/pinyintokenizer.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-06-08 08:04:18.848078 pinyintokenizer-0.0.2/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1294 2023-06-08 07:44:05.000000 pinyintokenizer-0.0.2/setup.py
```

### Comparing `pinyintokenizer-0.0.1/LICENSE` & `pinyintokenizer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pinyintokenizer-0.0.1/PKG-INFO` & `pinyintokenizer-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pinyintokenizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pinyin Tokenizer, chinese pinyin tokenizer
 Home-page: https://github.com/shibing624/pinyin-tokenizer
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
-Description: [![PyPI version](https://badge.fury.io/py/pinyin-tokenizer.svg)](https://badge.fury.io/py/pinyin-tokenizer)
-        [![Downloads](https://pepy.tech/badge/pinyin-tokenizer)](https://pepy.tech/project/pinyin-tokenizer)
+Description: [![PyPI version](https://badge.fury.io/py/pinyintokenizer.svg)](https://badge.fury.io/py/pinyin-tokenizer)
+        [![Downloads](https://pepy.tech/badge/pinyintokenizer)](https://pepy.tech/project/pinyin-tokenizer)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
         [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
@@ -20,18 +20,17 @@
         
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
-        - [Dataset](#Dataset)
         - [Contact](#Contact)
         - [Citation](#Citation)
-        - [Reference](#reference)
+        - [Related-Projects](#Related-Projects)
         
         # Feature
         
         - 基于前缀树（PyTrie）高效快速把连续拼音切分为单字拼音列表，便于后续拼音转汉字等处理。
         
         # Install
         
@@ -48,46 +47,92 @@
         cd pinyin-tokenizer
         python setup.py install
         ```
         
         
         # Usage
         
-        ## Pinyin Tokenizer
+        ## 拼音切分（Pinyin Tokenizer）
         
         example：[examples/pinyin_tokenize_demo.py](examples/pinyin_tokenize_demo.py):
         
         
         ```python
         import sys
         
         sys.path.append('..')
         from pinyintokenizer import PinyinTokenizer
         
         if __name__ == '__main__':
             m = PinyinTokenizer()
             print(f"{m.tokenize('wo3')}")
             print(f"{m.tokenize('nihao')}")
+            print(f"{m.tokenize('lv3you2')}")  # 旅游
             print(f"{m.tokenize('liudehua')}")
-            print(f"{m.tokenize('liu de hua')}")
+            print(f"{m.tokenize('liu de hua')}")  # 刘德华
+            print(f"{m.tokenize('womenzuogelvyougongnue')}")  # 我们做个旅游攻略
+            print(f"{m.tokenize('xi anjiaotongdaxue')}")  # 西安交通大学
+        
+            # not support english
             print(f"{m.tokenize('good luck')}")
-            print(f"{m.tokenize('xi anjiaotongdaxue')}")
         ```
         
         output:
         
         ```shell
         (['wo'], ['3'])
         (['ni', 'hao'], [])
+        (['lv', 'you'], ['3', '2'])
         (['liu', 'de', 'hua'], [])
         (['liu', 'de', 'hua'], [' ', ' '])
-        (['o', 'o', 'lu'], ['g', 'd', ' ', 'c', 'k'])
+        (['wo', 'men', 'zuo', 'ge', 'lv', 'you', 'gong', 'nue'], [])
         (['xi', 'an', 'jiao', 'tong', 'da', 'xue'], [' '])
+        (['o', 'o', 'lu'], ['g', 'd', ' ', 'c', 'k'])
+        ```
+        - `tokenize`方法返回两个结果，第一个为拼音列表，第二个为非法拼音列表。
+        
+        
+        ## 连续拼音转汉字（Pinyin2Hanzi）
+        先使用本库[pinyintokenizer](https://pypi.org/project/pinyintokenizer/)把连续拼音切分，再使用[Pinyin2Hanzi](https://pypi.org/project/Pinyin2Hanzi/)库把拼音转汉字。
+        
+        example：[examples/pinyin2hanzi_demo.py](examples/pinyin2hanzi_demo.py):
+        
+        
+        ```python
+        import sys
+        from Pinyin2Hanzi import DefaultDagParams
+        from Pinyin2Hanzi import dag
+        
+        sys.path.append('..')
+        from pinyintokenizer import PinyinTokenizer
+        
+        dagparams = DefaultDagParams()
+        
+        
+        def pinyin2hanzi(pinyin_sentence):
+            pinyin_list, _ = PinyinTokenizer().tokenize(pinyin_sentence)
+            result = dag(dagparams, pinyin_list, path_num=1)
+            return ''.join(result[0].path)
+        
+        
+        if __name__ == '__main__':
+            print(f"{pinyin2hanzi('wo3')}")
+            print(f"{pinyin2hanzi('jintianxtianqibucuo')}")
+            print(f"{pinyin2hanzi('liudehua')}")
         ```
         
+        output:
+        
+        ```shell
+        我
+        今天天气不错
+        刘德华
+        ```
+        
+        
         
         # Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我：加我*微信号：xuming624*, 进Python-NLP交流群，备注：*姓名-公司名-NLP*
         <img src="docs/wechat.jpeg" width="200" />
```

### Comparing `pinyintokenizer-0.0.1/README.md` & `pinyintokenizer-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-[![PyPI version](https://badge.fury.io/py/pinyin-tokenizer.svg)](https://badge.fury.io/py/pinyin-tokenizer)
-[![Downloads](https://pepy.tech/badge/pinyin-tokenizer)](https://pepy.tech/project/pinyin-tokenizer)
+[![PyPI version](https://badge.fury.io/py/pinyintokenizer.svg)](https://badge.fury.io/py/pinyin-tokenizer)
+[![Downloads](https://pepy.tech/badge/pinyintokenizer)](https://pepy.tech/project/pinyin-tokenizer)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
 [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
@@ -12,18 +12,17 @@
 
 
 **Guide**
 
 - [Feature](#Feature)
 - [Install](#install)
 - [Usage](#usage)
-- [Dataset](#Dataset)
 - [Contact](#Contact)
 - [Citation](#Citation)
-- [Reference](#reference)
+- [Related-Projects](#Related-Projects)
 
 # Feature
 
 - 基于前缀树（PyTrie）高效快速把连续拼音切分为单字拼音列表，便于后续拼音转汉字等处理。
 
 # Install
 
@@ -40,46 +39,92 @@
 cd pinyin-tokenizer
 python setup.py install
 ```
 
 
 # Usage
 
-## Pinyin Tokenizer
+## 拼音切分（Pinyin Tokenizer）
 
 example：[examples/pinyin_tokenize_demo.py](examples/pinyin_tokenize_demo.py):
 
 
 ```python
 import sys
 
 sys.path.append('..')
 from pinyintokenizer import PinyinTokenizer
 
 if __name__ == '__main__':
     m = PinyinTokenizer()
     print(f"{m.tokenize('wo3')}")
     print(f"{m.tokenize('nihao')}")
+    print(f"{m.tokenize('lv3you2')}")  # 旅游
     print(f"{m.tokenize('liudehua')}")
-    print(f"{m.tokenize('liu de hua')}")
+    print(f"{m.tokenize('liu de hua')}")  # 刘德华
+    print(f"{m.tokenize('womenzuogelvyougongnue')}")  # 我们做个旅游攻略
+    print(f"{m.tokenize('xi anjiaotongdaxue')}")  # 西安交通大学
+
+    # not support english
     print(f"{m.tokenize('good luck')}")
-    print(f"{m.tokenize('xi anjiaotongdaxue')}")
 ```
 
 output:
 
 ```shell
 (['wo'], ['3'])
 (['ni', 'hao'], [])
+(['lv', 'you'], ['3', '2'])
 (['liu', 'de', 'hua'], [])
 (['liu', 'de', 'hua'], [' ', ' '])
-(['o', 'o', 'lu'], ['g', 'd', ' ', 'c', 'k'])
+(['wo', 'men', 'zuo', 'ge', 'lv', 'you', 'gong', 'nue'], [])
 (['xi', 'an', 'jiao', 'tong', 'da', 'xue'], [' '])
+(['o', 'o', 'lu'], ['g', 'd', ' ', 'c', 'k'])
+```
+- `tokenize`方法返回两个结果，第一个为拼音列表，第二个为非法拼音列表。
+
+
+## 连续拼音转汉字（Pinyin2Hanzi）
+先使用本库[pinyintokenizer](https://pypi.org/project/pinyintokenizer/)把连续拼音切分，再使用[Pinyin2Hanzi](https://pypi.org/project/Pinyin2Hanzi/)库把拼音转汉字。
+
+example：[examples/pinyin2hanzi_demo.py](examples/pinyin2hanzi_demo.py):
+
+
+```python
+import sys
+from Pinyin2Hanzi import DefaultDagParams
+from Pinyin2Hanzi import dag
+
+sys.path.append('..')
+from pinyintokenizer import PinyinTokenizer
+
+dagparams = DefaultDagParams()
+
+
+def pinyin2hanzi(pinyin_sentence):
+    pinyin_list, _ = PinyinTokenizer().tokenize(pinyin_sentence)
+    result = dag(dagparams, pinyin_list, path_num=1)
+    return ''.join(result[0].path)
+
+
+if __name__ == '__main__':
+    print(f"{pinyin2hanzi('wo3')}")
+    print(f"{pinyin2hanzi('jintianxtianqibucuo')}")
+    print(f"{pinyin2hanzi('liudehua')}")
 ```
 
+output:
+
+```shell
+我
+今天天气不错
+刘德华
+```
+
+
 
 # Contact
 
 - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我：加我*微信号：xuming624*, 进Python-NLP交流群，备注：*姓名-公司名-NLP*
 <img src="docs/wechat.jpeg" width="200" />
```

### Comparing `pinyintokenizer-0.0.1/pinyintokenizer/__init__.py` & `pinyintokenizer-0.0.2/pinyintokenizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,17 @@
         self.add(["l", "in"])
         self.add(["l", "ing"])
         self.add(["l", "iu"])
         self.add(["l", "ong"])
         self.add(["l", "ou"])
         self.add(["l", "u"])
         self.add(["l", "u:"])
-        self.add(["l", "u:e"])
+        self.add(["l", "v"])
+        self.add(["l", "ue"])
+        self.add(["l", "ve"])
         self.add(["l", "uan"])
         self.add(["l", "un"])
         self.add(["l", "uo"])
         self.add(["m", ""])
         self.add(["m", "a"])
         self.add(["m", "ai"])
         self.add(["m", "an"])
@@ -271,15 +273,17 @@
         self.add(["n", "in"])
         self.add(["n", "ing"])
         self.add(["n", "iu"])
         self.add(["n", "ong"])
         self.add(["n", "ou"])
         self.add(["n", "u"])
         self.add(["n", "u:"])
-        self.add(["n", "u:e"])
+        self.add(["n", "ue"])
+        self.add(["n", "v"])
+        self.add(["n", "ve"])
         self.add(["n", "uan"])
         self.add(["n", "uo"])
         self.add(["p", "a"])
         self.add(["p", "ai"])
         self.add(["p", "an"])
         self.add(["p", "ang"])
         self.add(["p", "ao"])
@@ -450,14 +454,19 @@
         self.add(["zh", "uan"])
         self.add(["zh", "uang"])
         self.add(["zh", "ui"])
         self.add(["zh", "un"])
         self.add(["zh", "uo"])
 
     def tokenize(self, sent):
+        """
+        Tokenize a sentence into pinyin list.
+        :param sent: pinyin sentence
+        :return: pinyin_list, invalid pinyin list
+        """
         words = []
         invalid_words = []
         while len(sent) > 0:
             buf, succ = self.root.find(sent)
             # print("buf: {}, succ: {}".format(buf, succ))
             if succ:
                 words.append(buf)
@@ -468,19 +477,7 @@
         return words, invalid_words
 
 
 if __name__ == "__main__":
     m = PinyinTokenizer()
     words, invalid_words = m.tokenize("jintianxtianqibucuo")
     print("words: {}".format(words))
-    """
-    import sys
-    sys.path.append('..')
-
-    from Pinyin2Hanzi import DefaultDagParams
-    from Pinyin2Hanzi import dag
-
-    dagparams = DefaultDagParams()
-    result = dag(dagparams, words, path_num=1)
-    for item in result:
-        print(item.score, ''.join(item.path))
-    """
```

### Comparing `pinyintokenizer-0.0.1/pinyintokenizer.egg-info/PKG-INFO` & `pinyintokenizer-0.0.2/pinyintokenizer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pinyintokenizer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pinyin Tokenizer, chinese pinyin tokenizer
 Home-page: https://github.com/shibing624/pinyin-tokenizer
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
-Description: [![PyPI version](https://badge.fury.io/py/pinyin-tokenizer.svg)](https://badge.fury.io/py/pinyin-tokenizer)
-        [![Downloads](https://pepy.tech/badge/pinyin-tokenizer)](https://pepy.tech/project/pinyin-tokenizer)
+Description: [![PyPI version](https://badge.fury.io/py/pinyintokenizer.svg)](https://badge.fury.io/py/pinyin-tokenizer)
+        [![Downloads](https://pepy.tech/badge/pinyintokenizer)](https://pepy.tech/project/pinyin-tokenizer)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
         [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
@@ -20,18 +20,17 @@
         
         
         **Guide**
         
         - [Feature](#Feature)
         - [Install](#install)
         - [Usage](#usage)
-        - [Dataset](#Dataset)
         - [Contact](#Contact)
         - [Citation](#Citation)
-        - [Reference](#reference)
+        - [Related-Projects](#Related-Projects)
         
         # Feature
         
         - 基于前缀树（PyTrie）高效快速把连续拼音切分为单字拼音列表，便于后续拼音转汉字等处理。
         
         # Install
         
@@ -48,46 +47,92 @@
         cd pinyin-tokenizer
         python setup.py install
         ```
         
         
         # Usage
         
-        ## Pinyin Tokenizer
+        ## 拼音切分（Pinyin Tokenizer）
         
         example：[examples/pinyin_tokenize_demo.py](examples/pinyin_tokenize_demo.py):
         
         
         ```python
         import sys
         
         sys.path.append('..')
         from pinyintokenizer import PinyinTokenizer
         
         if __name__ == '__main__':
             m = PinyinTokenizer()
             print(f"{m.tokenize('wo3')}")
             print(f"{m.tokenize('nihao')}")
+            print(f"{m.tokenize('lv3you2')}")  # 旅游
             print(f"{m.tokenize('liudehua')}")
-            print(f"{m.tokenize('liu de hua')}")
+            print(f"{m.tokenize('liu de hua')}")  # 刘德华
+            print(f"{m.tokenize('womenzuogelvyougongnue')}")  # 我们做个旅游攻略
+            print(f"{m.tokenize('xi anjiaotongdaxue')}")  # 西安交通大学
+        
+            # not support english
             print(f"{m.tokenize('good luck')}")
-            print(f"{m.tokenize('xi anjiaotongdaxue')}")
         ```
         
         output:
         
         ```shell
         (['wo'], ['3'])
         (['ni', 'hao'], [])
+        (['lv', 'you'], ['3', '2'])
         (['liu', 'de', 'hua'], [])
         (['liu', 'de', 'hua'], [' ', ' '])
-        (['o', 'o', 'lu'], ['g', 'd', ' ', 'c', 'k'])
+        (['wo', 'men', 'zuo', 'ge', 'lv', 'you', 'gong', 'nue'], [])
         (['xi', 'an', 'jiao', 'tong', 'da', 'xue'], [' '])
+        (['o', 'o', 'lu'], ['g', 'd', ' ', 'c', 'k'])
+        ```
+        - `tokenize`方法返回两个结果，第一个为拼音列表，第二个为非法拼音列表。
+        
+        
+        ## 连续拼音转汉字（Pinyin2Hanzi）
+        先使用本库[pinyintokenizer](https://pypi.org/project/pinyintokenizer/)把连续拼音切分，再使用[Pinyin2Hanzi](https://pypi.org/project/Pinyin2Hanzi/)库把拼音转汉字。
+        
+        example：[examples/pinyin2hanzi_demo.py](examples/pinyin2hanzi_demo.py):
+        
+        
+        ```python
+        import sys
+        from Pinyin2Hanzi import DefaultDagParams
+        from Pinyin2Hanzi import dag
+        
+        sys.path.append('..')
+        from pinyintokenizer import PinyinTokenizer
+        
+        dagparams = DefaultDagParams()
+        
+        
+        def pinyin2hanzi(pinyin_sentence):
+            pinyin_list, _ = PinyinTokenizer().tokenize(pinyin_sentence)
+            result = dag(dagparams, pinyin_list, path_num=1)
+            return ''.join(result[0].path)
+        
+        
+        if __name__ == '__main__':
+            print(f"{pinyin2hanzi('wo3')}")
+            print(f"{pinyin2hanzi('jintianxtianqibucuo')}")
+            print(f"{pinyin2hanzi('liudehua')}")
         ```
         
+        output:
+        
+        ```shell
+        我
+        今天天气不错
+        刘德华
+        ```
+        
+        
         
         # Contact
         
         - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/pinyin-tokenizer.svg)](https://github.com/shibing624/pinyin-tokenizer/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我：加我*微信号：xuming624*, 进Python-NLP交流群，备注：*姓名-公司名-NLP*
         <img src="docs/wechat.jpeg" width="200" />
```

### Comparing `pinyintokenizer-0.0.1/setup.py` & `pinyintokenizer-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 from setuptools import setup, find_packages
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='pinyintokenizer',
     version=__version__,
```

