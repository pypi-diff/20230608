# Comparing `tmp/nonebot_plugin_random_ban-0.1.0.tar.gz` & `tmp/nonebot_plugin_random_ban-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_random_ban-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_random_ban-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_random_ban-0.1.0.tar` & `nonebot_plugin_random_ban-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_random_ban-0.1.0/LICENSE
--rw-r--r--   0        0        0     8391 2022-12-22 11:59:18.706483 nonebot_plugin_random_ban-0.1.0/nonebot_plugin_random_ban/__init__.py
--rw-r--r--   0        0        0     1007 2022-12-22 12:00:42.898590 nonebot_plugin_random_ban-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5943 2022-12-22 11:57:57.445995 nonebot_plugin_random_ban-0.1.0/README.md
--rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 nonebot_plugin_random_ban-0.1.0/setup.py
--rw-r--r--   0        0        0     6729 1970-01-01 00:00:00.000000 nonebot_plugin_random_ban-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_random_ban-0.2.0/LICENSE
+-rw-r--r--   0        0        0    11009 2023-06-08 10:52:01.056272 nonebot_plugin_random_ban-0.2.0/nonebot_plugin_random_ban/__init__.py
+-rw-r--r--   0        0        0     1007 2023-06-08 10:52:21.554666 nonebot_plugin_random_ban-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6258 2023-06-08 10:41:06.739392 nonebot_plugin_random_ban-0.2.0/README.md
+-rw-r--r--   0        0        0     7036 1970-01-01 00:00:00.000000 nonebot_plugin_random_ban-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_random_ban-0.1.0/LICENSE` & `nonebot_plugin_random_ban-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_random_ban-0.1.0/pyproject.toml` & `nonebot_plugin_random_ban-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-random_ban"
-version = "0.1.0"
+version = "0.2.0"
 description = "随机禁言一名群员或自己n分钟（n通过参入数字然后随机实现），简单粗暴。"
 authors = ["Ikaros <327209194@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_random_ban"}]
 homepage = "https://github.com/Ikaros-521/nonebot_plugin_random_ban"
 repository = "https://github.com/Ikaros-521/nonebot_plugin_random_ban"
```

### Comparing `nonebot_plugin_random_ban-0.1.0/README.md` & `nonebot_plugin_random_ban-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -103,23 +103,23 @@
 ## 🎉 功能
 随机禁言一名群员或自己n分钟（n通过传入数字然后随机实现），简单粗暴。可以`开启至暗时刻`，就是所有人可以使用`随禁`命令，刺激。    
 
 ## 👉 命令
 
 ### 随机禁言 或 随禁
 命令结构：```/随机禁言 [最大禁言时间]``` 或 ```/随禁 [最大禁言时间]```  （最大禁言时间不填默认60分钟内的随机）  
-例如：```/随机禁言``` 或 ```/随禁 10```  
+例如：```/随机禁言``` 或 ```/随禁 10``` 或 ```/随禁 10分``` 或 ```/随禁 10时``` 或 ```/随禁 10天```   
 bot返回内容：  
 ```
 恭喜幸运儿:xxx 获得6分钟的禁言服务
 ```
 
 ### 口球 或 禁我
 命令结构：```/口球 [最大禁言时间]``` 或 ```/禁我 [最大禁言时间]```  （最大禁言时间不填默认60分钟内的随机）  
-例如：```/口球``` 或 ```/禁我 10```  
+例如：```/口球``` 或 ```/禁我 10``` 或 ```/禁我 10分``` 或 ```/口球 10时``` 或 ```/口球 10天```   
 bot返回内容：  
 ```
 恭喜您获得6分钟的禁言服务
 ```
 
 ### 开启至暗时刻
 命令结构：```/开启至暗时刻``` 或 ```/至暗时刻启动``` 或 ```/至暗时刻开启```  或 ```/启动至暗时刻```  
@@ -134,14 +134,16 @@
 命令结构：```/关闭至暗时刻``` 或 ```/至暗时刻关闭``` 或 ```/停止至暗时刻```  或 ```/至暗时刻停止```  
 例如：```/关闭至暗时刻```  
 bot返回内容：  
 ```
 本群已关闭 至暗时刻，世界恢复和平。
 ```
 
+![](docs/result.jpg)
+
 ## ⚙ 拓展
 自行修改源码喵~
 
 
 ## 📝 更新日志
 
 <details>
@@ -168,9 +170,15 @@
 
 - 新增可以开启任何人都使用随机禁言的配置项
 
 ### 0.1.0
 
 - 新增 至暗时刻，就是所有人可以使用`随禁`命令，刺激。
 
+### 0.2.0
+
+- 新增 传参的单位兼容，分、分钟、时、小时、天。
+- 修改 艾特 为 回复的形式。
+- 优化代码。
+
 </details>
```

#### html2text {}

```diff
@@ -33,27 +33,31 @@
 ----:|:----:|:----:|:----------------------------:| |
 `nonebot_plugin_random_ban` | å¦ | `[]` |
 æ°ç»åéç½®å¼å¯`è³ææ¶å»`çç¾¤å·å³å¯ | ## ð åè½
 éæºç¦è¨ä¸åç¾¤åæèªå·±nåéï¼néè¿ä¼ å¥æ°å­ç¶åéæºå®ç°ï¼ï¼ç®åç²æ´ãå¯ä»¥`å¼å¯è³ææ¶å»`ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
 ## ð å½ä»¤ ### éæºç¦è¨ æ éç¦ å½ä»¤ç»æï¼```/éæºç¦è¨
 [æå¤§ç¦è¨æ¶é´]``` æ ```/éç¦ [æå¤§ç¦è¨æ¶é´]```
 ï¼æå¤§ç¦è¨æ¶é´ä¸å¡«é»è®¤60åéåçéæºï¼ ä¾å¦ï¼```/
-éæºç¦è¨``` æ ```/éç¦ 10``` botè¿ååå®¹ï¼ ``` æ­åå¹¸è¿å¿:xxx
+éæºç¦è¨``` æ ```/éç¦ 10``` æ ```/éç¦ 10å``` æ ```/éç¦
+10æ¶``` æ ```/éç¦ 10å¤©``` botè¿ååå®¹ï¼ ``` æ­åå¹¸è¿å¿:xxx
 è·å¾6åéçç¦è¨æå¡ ``` ### å£ç æ ç¦æ å½ä»¤ç»æï¼```/
 å£ç [æå¤§ç¦è¨æ¶é´]``` æ ```/ç¦æ [æå¤§ç¦è¨æ¶é´]```
 ï¼æå¤§ç¦è¨æ¶é´ä¸å¡«é»è®¤60åéåçéæºï¼ ä¾å¦ï¼```/å£ç```
-æ ```/ç¦æ 10``` botè¿ååå®¹ï¼ ```
-æ­åæ¨è·å¾6åéçç¦è¨æå¡ ``` ### å¼å¯è³ææ¶å»
-å½ä»¤ç»æï¼```/å¼å¯è³ææ¶å»``` æ ```/è³ææ¶å»å¯å¨``` æ ```/
-è³ææ¶å»å¼å¯``` æ ```/å¯å¨è³ææ¶å»``` ä¾å¦ï¼```/
-å¼å¯è³ææ¶å»``` è¯´æï¼è³ææ¶å»å°±æ¯ææäººå¯ä»¥ä½¿ç¨ `/
-éç¦` å½ä»¤ï¼å°æ¯ä¸çè¥é£è¡é¨ã botè¿ååå®¹ï¼ ```
-æ¬ç¾¤å¼å¯ è³ææ¶å»æåï¼å¼å§ç©çå§ï¼ ``` ### å³é­è³ææ¶å»
+æ ```/ç¦æ 10``` æ ```/ç¦æ 10å``` æ ```/å£ç 10æ¶``` æ ```/
+å£ç 10å¤©``` botè¿ååå®¹ï¼ ``` æ­åæ¨è·å¾6åéçç¦è¨æå¡
+``` ### å¼å¯è³ææ¶å» å½ä»¤ç»æï¼```/å¼å¯è³ææ¶å»``` æ ```/
+è³ææ¶å»å¯å¨``` æ ```/è³ææ¶å»å¼å¯``` æ ```/
+å¯å¨è³ææ¶å»``` ä¾å¦ï¼```/å¼å¯è³ææ¶å»```
+è¯´æï¼è³ææ¶å»å°±æ¯ææäººå¯ä»¥ä½¿ç¨ `/éç¦`
+å½ä»¤ï¼å°æ¯ä¸çè¥é£è¡é¨ã botè¿ååå®¹ï¼ ``` æ¬ç¾¤å¼å¯
+è³ææ¶å»æåï¼å¼å§ç©çå§ï¼ ``` ### å³é­è³ææ¶å»
 å½ä»¤ç»æï¼```/å³é­è³ææ¶å»``` æ ```/è³ææ¶å»å³é­``` æ ```/
 åæ­¢è³ææ¶å»``` æ ```/è³ææ¶å»åæ­¢``` ä¾å¦ï¼```/
 å³é­è³ææ¶å»``` botè¿ååå®¹ï¼ ``` æ¬ç¾¤å·²å³é­
-è³ææ¶å»ï¼ä¸çæ¢å¤åå¹³ã ``` ## â æå± èªè¡ä¿®æ¹æºç åµ~
-## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 - æä»¶åæ¬¡åå¸ ### 0.0.2 -
-è¡¥åæä»¶åä¿¡æ¯ - ä¼åææ¡£ ### 0.0.3 - æ°å¢å½ä»¤ å£ç æ
-ç¦æï¼èªå·±ç¦èªå·± ### 0.0.4 - ä¼åææ¡£ ### 0.0.5 -
-æ°å¢å¯ä»¥å¼å¯ä»»ä½äººé½ä½¿ç¨éæºç¦è¨çéç½®é¡¹ ### 0.1.0 - æ°å¢
-è³ææ¶å»ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
+è³ææ¶å»ï¼ä¸çæ¢å¤åå¹³ã ``` ![](docs/result.jpg) ## â æå±
+èªè¡ä¿®æ¹æºç åµ~ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
+æä»¶åæ¬¡åå¸ ### 0.0.2 - è¡¥åæä»¶åä¿¡æ¯ - ä¼åææ¡£ ### 0.0.3 -
+æ°å¢å½ä»¤ å£ç æ ç¦æï¼èªå·±ç¦èªå·± ### 0.0.4 - ä¼åææ¡£ ###
+0.0.5 - æ°å¢å¯ä»¥å¼å¯ä»»ä½äººé½ä½¿ç¨éæºç¦è¨çéç½®é¡¹ ### 0.1.0
+- æ°å¢ è³ææ¶å»ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
+### 0.2.0 - æ°å¢ ä¼ åçåä½å¼å®¹ï¼åãåéãæ¶ãå°æ¶ãå¤©ã
+- ä¿®æ¹ è¾ç¹ ä¸º åå¤çå½¢å¼ã - ä¼åä»£ç ã
```

### Comparing `nonebot_plugin_random_ban-0.1.0/setup.py` & `nonebot_plugin_random_ban-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,206 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-random-ban
+Version: 0.2.0
+Summary: 随机禁言一名群员或自己n分钟（n通过参入数字然后随机实现），简单粗暴。
+Home-page: https://github.com/Ikaros-521/nonebot_plugin_random_ban
+License: MIT
+Author: Ikaros
+Author-email: 327209194@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0b5,<3.0.0)
+Project-URL: Documentation, https://github.com/Ikaros-521/nonebot_plugin_random_ban/blob/master/README.md
+Project-URL: Repository, https://github.com/Ikaros-521/nonebot_plugin_random_ban
+Description-Content-Type: text/markdown
+
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot_plugin_random_ban
+  
+_✨ NoneBot 随机禁言插件 ✨_
+  
+<a href="https://github.com/Ikaros-521/nonebot_plugin_random_ban/stargazers">
+    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_random_ban?color=%09%2300BFFF&style=flat-square">
+</a>
+<a href="https://github.com/Ikaros-521/nonebot_plugin_random_ban/issues">
+    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_random_ban?color=Emerald%20green&style=flat-square">
+</a>
+<a href="https://github.com/Ikaros-521/nonebot_plugin_random_ban/network">
+    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_random_ban?color=%2300BFFF&style=flat-square">
+</a>
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_random_ban.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_random_ban">
+    <img src="https://img.shields.io/pypi/v/nonebot_plugin_random_ban.svg" alt="pypi">
+</a>
+<a href="https://www.python.org">
+    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</a>
+
+</div>
+
+适用于nonebot2 v11的随机禁言一名群员或自己n分钟 插件      
+注意：需要给bot管理员才能使用。  
+
+## 🔧 开发环境
+Nonebot2：2.0.0b5  
+python：3.8.13  
+操作系统：Windows10（Linux兼容性问题不大）  
+编辑器：pycharm  
+
+## 💿 安装
+
+### 1. nb-cli安装（推荐）
+
+在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  
+```
+nb plugin install nonebot_plugin_random_ban
+```
+
+### 2. 本地安装
+
+将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_random_ban`文件夹里的内容拷贝至上一级目录即可。  
+clone命令参考（得先装`git`，懂的都懂）：
+```
+git clone https://github.com/Ikaros-521/nonebot_plugin_random_ban.git
+``` 
+也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_random_ban`至上一级目录。  
+目录结构： ```你的bot/src/plugins/nonebot_plugin_random_ban/__init__.py```  
+
+
+### 3. pip安装
+
+```
+pip install nonebot_plugin_random_ban
+```  
+打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  
+```nonebot.load_plugin('nonebot_plugin_random_ban')```  
+当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_random_ban```即可  
+pyproject.toml配置例如：  
+``` 
+[tool.nonebot]
+plugin_dirs = ["src/plugins"]
+plugins = ["nonebot_plugin_random_ban"]
+``` 
+
+### 更新版本
+```
+nb plugin update nonebot_plugin_random_ban
+```
+
+## 🔧 配置
+
+### env配置
+```
+# nonebot_plugin_random_ban
+# 任何人都可以使用 随机禁言，开启后将会迎来至暗时刻
+anyone_can_random_ban = []
+```
+若某群想长期启动`至暗时刻`，配置参考：  
+```
+# nonebot_plugin_random_ban
+# 任何人都可以使用 随机禁言，开启后将会迎来至暗时刻
+anyone_can_random_ban = [123456, 114514]
+```
+|       配置项      | 必填 | 默认值 |             说明            |
+|:----------------:|:----:|:----:|:----------------------------:|
+| `nonebot_plugin_random_ban` | 否 | `[]` | 数组内配置开启`至暗时刻`的群号即可 |
+
+
+
+## 🎉 功能
+随机禁言一名群员或自己n分钟（n通过传入数字然后随机实现），简单粗暴。可以`开启至暗时刻`，就是所有人可以使用`随禁`命令，刺激。    
+
+## 👉 命令
+
+### 随机禁言 或 随禁
+命令结构：```/随机禁言 [最大禁言时间]``` 或 ```/随禁 [最大禁言时间]```  （最大禁言时间不填默认60分钟内的随机）  
+例如：```/随机禁言``` 或 ```/随禁 10``` 或 ```/随禁 10分``` 或 ```/随禁 10时``` 或 ```/随禁 10天```   
+bot返回内容：  
+```
+恭喜幸运儿:xxx 获得6分钟的禁言服务
+```
+
+### 口球 或 禁我
+命令结构：```/口球 [最大禁言时间]``` 或 ```/禁我 [最大禁言时间]```  （最大禁言时间不填默认60分钟内的随机）  
+例如：```/口球``` 或 ```/禁我 10``` 或 ```/禁我 10分``` 或 ```/口球 10时``` 或 ```/口球 10天```   
+bot返回内容：  
+```
+恭喜您获得6分钟的禁言服务
+```
+
+### 开启至暗时刻
+命令结构：```/开启至暗时刻``` 或 ```/至暗时刻启动``` 或 ```/至暗时刻开启```  或 ```/启动至暗时刻```  
+例如：```/开启至暗时刻```  
+说明：至暗时刻就是所有人可以使用 `/随禁` 命令，将是一片腥风血雨。  
+bot返回内容：  
+```
+本群开启 至暗时刻成功，开始狩猎吧！
+```
+
+### 关闭至暗时刻
+命令结构：```/关闭至暗时刻``` 或 ```/至暗时刻关闭``` 或 ```/停止至暗时刻```  或 ```/至暗时刻停止```  
+例如：```/关闭至暗时刻```  
+bot返回内容：  
+```
+本群已关闭 至暗时刻，世界恢复和平。
+```
+
+![](docs/result.jpg)
+
+## ⚙ 拓展
+自行修改源码喵~
+
+
+## 📝 更新日志
+
+<details>
+<summary>展开/收起</summary>
+
+### 0.0.1
+
+- 插件初次发布  
+
+### 0.0.2
+
+- 补充插件元信息
+- 优化文档
+
+### 0.0.3
+
+- 新增命令 口球 或 禁我，自己禁自己
+
+### 0.0.4
+
+- 优化文档
+
+### 0.0.5
+
+- 新增可以开启任何人都使用随机禁言的配置项
+
+### 0.1.0
+
+- 新增 至暗时刻，就是所有人可以使用`随禁`命令，刺激。
+
+### 0.2.0
+
+- 新增 传参的单位兼容，分、分钟、时、小时、天。
+- 修改 艾特 为 回复的形式。
+- 优化代码。
 
-packages = \
-['nonebot_plugin_random_ban']
+</details>
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['nonebot-adapter-onebot>=2.1.3,<3.0.0', 'nonebot2>=2.0.0b5,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-random-ban',
-    'version': '0.1.0',
-    'description': '随机禁言一名群员或自己n分钟（n通过参入数字然后随机实现），简单粗暴。',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_random_ban\n  \n_✨ NoneBot 随机禁言插件 ✨_\n  \n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_ban/stargazers">\n    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_random_ban?color=%09%2300BFFF&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_ban/issues">\n    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_random_ban?color=Emerald%20green&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_random_ban/network">\n    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_random_ban?color=%2300BFFF&style=flat-square">\n</a>\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_random_ban.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_random_ban">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_random_ban.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</a>\n\n</div>\n\n适用于nonebot2 v11的随机禁言一名群员或自己n分钟 插件      \n注意：需要给bot管理员才能使用。  \n\n## 🔧 开发环境\nNonebot2：2.0.0b5  \npython：3.8.13  \n操作系统：Windows10（Linux兼容性问题不大）  \n编辑器：pycharm  \n\n## 💿 安装\n\n### 1. nb-cli安装（推荐）\n\n在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  \n```\nnb plugin install nonebot_plugin_random_ban\n```\n\n### 2. 本地安装\n\n将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_random_ban`文件夹里的内容拷贝至上一级目录即可。  \nclone命令参考（得先装`git`，懂的都懂）：\n```\ngit clone https://github.com/Ikaros-521/nonebot_plugin_random_ban.git\n``` \n也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_random_ban`至上一级目录。  \n目录结构： ```你的bot/src/plugins/nonebot_plugin_random_ban/__init__.py```  \n\n\n### 3. pip安装\n\n```\npip install nonebot_plugin_random_ban\n```  \n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_random_ban\')```  \n当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_random_ban```即可  \npyproject.toml配置例如：  \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_random_ban"]\n``` \n\n### 更新版本\n```\nnb plugin update nonebot_plugin_random_ban\n```\n\n## 🔧 配置\n\n### env配置\n```\n# nonebot_plugin_random_ban\n# 任何人都可以使用 随机禁言，开启后将会迎来至暗时刻\nanyone_can_random_ban = []\n```\n若某群想长期启动`至暗时刻`，配置参考：  \n```\n# nonebot_plugin_random_ban\n# 任何人都可以使用 随机禁言，开启后将会迎来至暗时刻\nanyone_can_random_ban = [123456, 114514]\n```\n|       配置项      | 必填 | 默认值 |             说明            |\n|:----------------:|:----:|:----:|:----------------------------:|\n| `nonebot_plugin_random_ban` | 否 | `[]` | 数组内配置开启`至暗时刻`的群号即可 |\n\n\n\n## 🎉 功能\n随机禁言一名群员或自己n分钟（n通过传入数字然后随机实现），简单粗暴。可以`开启至暗时刻`，就是所有人可以使用`随禁`命令，刺激。    \n\n## 👉 命令\n\n### 随机禁言 或 随禁\n命令结构：```/随机禁言 [最大禁言时间]``` 或 ```/随禁 [最大禁言时间]```  （最大禁言时间不填默认60分钟内的随机）  \n例如：```/随机禁言``` 或 ```/随禁 10```  \nbot返回内容：  \n```\n恭喜幸运儿:xxx 获得6分钟的禁言服务\n```\n\n### 口球 或 禁我\n命令结构：```/口球 [最大禁言时间]``` 或 ```/禁我 [最大禁言时间]```  （最大禁言时间不填默认60分钟内的随机）  \n例如：```/口球``` 或 ```/禁我 10```  \nbot返回内容：  \n```\n恭喜您获得6分钟的禁言服务\n```\n\n### 开启至暗时刻\n命令结构：```/开启至暗时刻``` 或 ```/至暗时刻启动``` 或 ```/至暗时刻开启```  或 ```/启动至暗时刻```  \n例如：```/开启至暗时刻```  \n说明：至暗时刻就是所有人可以使用 `/随禁` 命令，将是一片腥风血雨。  \nbot返回内容：  \n```\n本群开启 至暗时刻成功，开始狩猎吧！\n```\n\n### 关闭至暗时刻\n命令结构：```/关闭至暗时刻``` 或 ```/至暗时刻关闭``` 或 ```/停止至暗时刻```  或 ```/至暗时刻停止```  \n例如：```/关闭至暗时刻```  \nbot返回内容：  \n```\n本群已关闭 至暗时刻，世界恢复和平。\n```\n\n## ⚙ 拓展\n自行修改源码喵~\n\n\n## 📝 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.0.1\n\n- 插件初次发布  \n\n### 0.0.2\n\n- 补充插件元信息\n- 优化文档\n\n### 0.0.3\n\n- 新增命令 口球 或 禁我，自己禁自己\n\n### 0.0.4\n\n- 优化文档\n\n### 0.0.5\n\n- 新增可以开启任何人都使用随机禁言的配置项\n\n### 0.1.0\n\n- 新增 至暗时刻，就是所有人可以使用`随禁`命令，刺激。\n\n</details>\n\n',
-    'author': 'Ikaros',
-    'author_email': '327209194@qq.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Ikaros-521/nonebot_plugin_random_ban',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,80 +1,76 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_random_ban'] package_data = \ {'': ['*']} install_requires = \
-['nonebot-adapter-onebot>=2.1.3,<3.0.0', 'nonebot2>=2.0.0b5,<3.0.0']
-setup_kwargs = { 'name': 'nonebot-plugin-random-ban', 'version': '0.1.0',
-'description':
-'éæºç¦è¨ä¸åç¾¤åæèªå·±nåéï¼néè¿åå¥æ°å­ç¶åéæºå®ç°ï¼ï¼ç®åç²æ´ã',
-'long_description': '
-                           \n [NoneBotPluginLogo]\n
-                                      \n
+Metadata-Version: 2.1 Name: nonebot-plugin-random-ban Version: 0.2.0 Summary:
+éæºç¦è¨ä¸åç¾¤åæèªå·±nåéï¼néè¿åå¥æ°å­ç¶åéæºå®ç°ï¼ï¼ç®åç²æ´ã
+Home-page: https://github.com/Ikaros-521/nonebot_plugin_random_ban License: MIT
+Author: Ikaros Author-email: 327209194@qq.com Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot2
+(>=2.0.0b5,<3.0.0) Project-URL: Documentation, https://github.com/Ikaros-521/
+nonebot_plugin_random_ban/blob/master/README.md Project-URL: Repository, https:
+//github.com/Ikaros-521/nonebot_plugin_random_ban Description-Content-Type:
+text/markdown
+                             [NoneBotPluginLogo]
                               [NoneBotPluginText]
-                                      \n
-\n\n
-\n\n# nonebot_plugin_random_ban\n \n_â¨ NoneBot éæºç¦è¨æä»¶ â¨_\n \n\n
-[GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[GitHub_forks]\n\n\n_[license]\n\n\n
-                          [pypi]\n\n\n_[python]\n\n\n
-\n\néç¨äºnonebot2 v11çéæºç¦è¨ä¸åç¾¤åæèªå·±nåé æä»¶
-\næ³¨æï¼éè¦ç»botç®¡çåæè½ä½¿ç¨ã \n\n## ð§
-å¼åç¯å¢\nNonebot2ï¼2.0.0b5 \npythonï¼3.8.13
-\næä½ç³»ç»ï¼Windows10ï¼Linuxå¼å®¹æ§é®é¢ä¸å¤§ï¼
-\nç¼è¾å¨ï¼pycharm \n\n## ð¿ å®è£\n\n### 1. nb-
-cliå®è£ï¼æ¨èï¼\n\nå¨ä½ botå·¥ç¨çæä»¶å¤¹ä¸ï¼è¿è¡cmdï¼è¿è¡è·¯å¾è¦å¯¹åï¼ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
-\n```\nnb plugin install nonebot_plugin_random_ban\n```\n\n### 2.
-æ¬å°å®è£\n\nå°é¡¹ç®cloneå°ä½ çæºå¨äººæä»¶ä¸çå¯¹åºæä»¶ç®å½åï¼ä¸è¬ä¸ºæºå¨äººæä»¶å¤¹ä¸ç`src/
+# nonebot_plugin_random_ban _â¨ NoneBot éæºç¦è¨æä»¶ â¨_ [GitHub_stars]
+           [GitHub_issues] [GitHub_forks] [license] [pypi] [python]
+éç¨äºnonebot2 v11çéæºç¦è¨ä¸åç¾¤åæèªå·±nåé æä»¶
+æ³¨æï¼éè¦ç»botç®¡çåæè½ä½¿ç¨ã ## ð§ å¼åç¯å¢
+Nonebot2ï¼2.0.0b5 pythonï¼3.8.13
+æä½ç³»ç»ï¼Windows10ï¼Linuxå¼å®¹æ§é®é¢ä¸å¤§ï¼ ç¼è¾å¨ï¼pycharm ##
+ð¿ å®è£ ### 1. nb-cliå®è£ï¼æ¨èï¼
+å¨ä½ botå·¥ç¨çæä»¶å¤¹ä¸ï¼è¿è¡cmdï¼è¿è¡è·¯å¾è¦å¯¹åï¼ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
+``` nb plugin install nonebot_plugin_random_ban ``` ### 2. æ¬å°å®è£
+å°é¡¹ç®cloneå°ä½ çæºå¨äººæä»¶ä¸çå¯¹åºæä»¶ç®å½åï¼ä¸è¬ä¸ºæºå¨äººæä»¶å¤¹ä¸ç`src/
 plugins`ï¼ï¼ç¶åæ`nonebot_plugin_random_ban`æä»¶å¤¹éçåå®¹æ·è´è³ä¸ä¸çº§ç®å½å³å¯ã
-\ncloneå½ä»¤åèï¼å¾åè£`git`ï¼æçé½æï¼ï¼\n```\ngit clone
-https://github.com/Ikaros-521/nonebot_plugin_random_ban.git\n```
-\nä¹å¯ä»¥ç´æ¥ä¸è½½åç¼©åå°æä»¶ç®å½è§£åï¼ç¶ååæ ·æå`nonebot_plugin_random_ban`è³ä¸ä¸çº§ç®å½ã
-\nç®å½ç»æï¼ ```ä½ çbot/src/plugins/nonebot_plugin_random_ban/
-__init__.py``` \n\n\n### 3. pipå®è£\n\n```\npip install
-nonebot_plugin_random_ban\n``` \næå¼ nonebot2 é¡¹ç®ç ```bot.py``` æä»¶,
-å¨å¶ä¸­åå¥ \n```nonebot.load_plugin(\'nonebot_plugin_random_ban\')```
-\nå½ç¶ï¼å¦ææ¯é»è®¤nb-
+cloneå½ä»¤åèï¼å¾åè£`git`ï¼æçé½æï¼ï¼ ``` git clone https://
+github.com/Ikaros-521/nonebot_plugin_random_ban.git ```
+ä¹å¯ä»¥ç´æ¥ä¸è½½åç¼©åå°æä»¶ç®å½è§£åï¼ç¶ååæ ·æå`nonebot_plugin_random_ban`è³ä¸ä¸çº§ç®å½ã
+ç®å½ç»æï¼ ```ä½ çbot/src/plugins/nonebot_plugin_random_ban/
+__init__.py``` ### 3. pipå®è£ ``` pip install nonebot_plugin_random_ban ```
+æå¼ nonebot2 é¡¹ç®ç ```bot.py``` æä»¶, å¨å¶ä¸­åå¥
+```nonebot.load_plugin('nonebot_plugin_random_ban')```
+å½ç¶ï¼å¦ææ¯é»è®¤nb-
 cliåå»ºçnonebot2çè¯ï¼å¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_random_ban```å³å¯
-\npyproject.tomléç½®ä¾å¦ï¼ \n``` \n[tool.nonebot]\nplugin_dirs = ["src/
-plugins"]\nplugins = ["nonebot_plugin_random_ban"]\n``` \n\n###
-æ´æ°çæ¬\n```\nnb plugin update nonebot_plugin_random_ban\n```\n\n## ð§
-éç½®\n\n### envéç½®\n```\n# nonebot_plugin_random_ban\n#
-ä»»ä½äººé½å¯ä»¥ä½¿ç¨
-éæºç¦è¨ï¼å¼å¯åå°ä¼è¿æ¥è³ææ¶å»\nanyone_can_random_ban =
-[]\n```\nè¥æç¾¤æ³é¿æå¯å¨`è³ææ¶å»`ï¼éç½®åèï¼ \n```\n#
-nonebot_plugin_random_ban\n# ä»»ä½äººé½å¯ä»¥ä½¿ç¨
-éæºç¦è¨ï¼å¼å¯åå°ä¼è¿æ¥è³ææ¶å»\nanyone_can_random_ban =
-[123456, 114514]\n```\n| éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ |\n|:---------
--------:|:----:|:----:|:----------------------------:|\n|
+pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
+plugins = ["nonebot_plugin_random_ban"] ``` ### æ´æ°çæ¬ ``` nb plugin
+update nonebot_plugin_random_ban ``` ## ð§ éç½® ### envéç½® ``` #
+nonebot_plugin_random_ban # ä»»ä½äººé½å¯ä»¥ä½¿ç¨
+éæºç¦è¨ï¼å¼å¯åå°ä¼è¿æ¥è³ææ¶å» anyone_can_random_ban = [] ```
+è¥æç¾¤æ³é¿æå¯å¨`è³ææ¶å»`ï¼éç½®åèï¼ ``` #
+nonebot_plugin_random_ban # ä»»ä½äººé½å¯ä»¥ä½¿ç¨
+éæºç¦è¨ï¼å¼å¯åå°ä¼è¿æ¥è³ææ¶å» anyone_can_random_ban =
+[123456, 114514] ``` | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:------------
+----:|:----:|:----:|:----------------------------:| |
 `nonebot_plugin_random_ban` | å¦ | `[]` |
-æ°ç»åéç½®å¼å¯`è³ææ¶å»`çç¾¤å·å³å¯ |\n\n\n\n## ð
-åè½\néæºç¦è¨ä¸åç¾¤åæèªå·±nåéï¼néè¿ä¼ å¥æ°å­ç¶åéæºå®ç°ï¼ï¼ç®åç²æ´ãå¯ä»¥`å¼å¯è³ææ¶å»`ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
-\n\n## ð å½ä»¤\n\n### éæºç¦è¨ æ éç¦\nå½ä»¤ç»æï¼```/
-éæºç¦è¨ [æå¤§ç¦è¨æ¶é´]``` æ ```/éç¦ [æå¤§ç¦è¨æ¶é´]```
-ï¼æå¤§ç¦è¨æ¶é´ä¸å¡«é»è®¤60åéåçéæºï¼ \nä¾å¦ï¼```/
-éæºç¦è¨``` æ ```/éç¦ 10``` \nbotè¿ååå®¹ï¼
-\n```\næ­åå¹¸è¿å¿:xxx è·å¾6åéçç¦è¨æå¡\n```\n\n### å£ç æ
-ç¦æ\nå½ä»¤ç»æï¼```/å£ç [æå¤§ç¦è¨æ¶é´]``` æ ```/ç¦æ
-[æå¤§ç¦è¨æ¶é´]```
-ï¼æå¤§ç¦è¨æ¶é´ä¸å¡«é»è®¤60åéåçéæºï¼ \nä¾å¦ï¼```/
-å£ç``` æ ```/ç¦æ 10``` \nbotè¿ååå®¹ï¼
-\n```\næ­åæ¨è·å¾6åéçç¦è¨æå¡\n```\n\n###
-å¼å¯è³ææ¶å»\nå½ä»¤ç»æï¼```/å¼å¯è³ææ¶å»``` æ ```/
+æ°ç»åéç½®å¼å¯`è³ææ¶å»`çç¾¤å·å³å¯ | ## ð åè½
+éæºç¦è¨ä¸åç¾¤åæèªå·±nåéï¼néè¿ä¼ å¥æ°å­ç¶åéæºå®ç°ï¼ï¼ç®åç²æ´ãå¯ä»¥`å¼å¯è³ææ¶å»`ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
+## ð å½ä»¤ ### éæºç¦è¨ æ éç¦ å½ä»¤ç»æï¼```/éæºç¦è¨
+[æå¤§ç¦è¨æ¶é´]``` æ ```/éç¦ [æå¤§ç¦è¨æ¶é´]```
+ï¼æå¤§ç¦è¨æ¶é´ä¸å¡«é»è®¤60åéåçéæºï¼ ä¾å¦ï¼```/
+éæºç¦è¨``` æ ```/éç¦ 10``` æ ```/éç¦ 10å``` æ ```/éç¦
+10æ¶``` æ ```/éç¦ 10å¤©``` botè¿ååå®¹ï¼ ``` æ­åå¹¸è¿å¿:xxx
+è·å¾6åéçç¦è¨æå¡ ``` ### å£ç æ ç¦æ å½ä»¤ç»æï¼```/
+å£ç [æå¤§ç¦è¨æ¶é´]``` æ ```/ç¦æ [æå¤§ç¦è¨æ¶é´]```
+ï¼æå¤§ç¦è¨æ¶é´ä¸å¡«é»è®¤60åéåçéæºï¼ ä¾å¦ï¼```/å£ç```
+æ ```/ç¦æ 10``` æ ```/ç¦æ 10å``` æ ```/å£ç 10æ¶``` æ ```/
+å£ç 10å¤©``` botè¿ååå®¹ï¼ ``` æ­åæ¨è·å¾6åéçç¦è¨æå¡
+``` ### å¼å¯è³ææ¶å» å½ä»¤ç»æï¼```/å¼å¯è³ææ¶å»``` æ ```/
 è³ææ¶å»å¯å¨``` æ ```/è³ææ¶å»å¼å¯``` æ ```/
-å¯å¨è³ææ¶å»``` \nä¾å¦ï¼```/å¼å¯è³ææ¶å»```
-\nè¯´æï¼è³ææ¶å»å°±æ¯ææäººå¯ä»¥ä½¿ç¨ `/éç¦`
-å½ä»¤ï¼å°æ¯ä¸çè¥é£è¡é¨ã \nbotè¿ååå®¹ï¼ \n```\næ¬ç¾¤å¼å¯
-è³ææ¶å»æåï¼å¼å§ç©çå§ï¼\n```\n\n###
-å³é­è³ææ¶å»\nå½ä»¤ç»æï¼```/å³é­è³ææ¶å»``` æ ```/
-è³ææ¶å»å³é­``` æ ```/åæ­¢è³ææ¶å»``` æ ```/
-è³ææ¶å»åæ­¢``` \nä¾å¦ï¼```/å³é­è³ææ¶å»``` \nbotè¿ååå®¹ï¼
-\n```\næ¬ç¾¤å·²å³é­ è³ææ¶å»ï¼ä¸çæ¢å¤åå¹³ã\n```\n\n## â
-æå±\nèªè¡ä¿®æ¹æºç åµ~\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
-æ¶èµ·\n\n### 0.0.1\n\n- æä»¶åæ¬¡åå¸ \n\n### 0.0.2\n\n-
-è¡¥åæä»¶åä¿¡æ¯\n- ä¼åææ¡£\n\n### 0.0.3\n\n- æ°å¢å½ä»¤ å£ç æ
-ç¦æï¼èªå·±ç¦èªå·±\n\n### 0.0.4\n\n- ä¼åææ¡£\n\n### 0.0.5\n\n-
-æ°å¢å¯ä»¥å¼å¯ä»»ä½äººé½ä½¿ç¨éæºç¦è¨çéç½®é¡¹\n\n### 0.1.0\n\n-
-æ°å¢
-è³ææ¶å»ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã\n\n\n\n',
-'author': 'Ikaros', 'author_email': '327209194@qq.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/Ikaros-521/
-nonebot_plugin_random_ban', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+å¯å¨è³ææ¶å»``` ä¾å¦ï¼```/å¼å¯è³ææ¶å»```
+è¯´æï¼è³ææ¶å»å°±æ¯ææäººå¯ä»¥ä½¿ç¨ `/éç¦`
+å½ä»¤ï¼å°æ¯ä¸çè¥é£è¡é¨ã botè¿ååå®¹ï¼ ``` æ¬ç¾¤å¼å¯
+è³ææ¶å»æåï¼å¼å§ç©çå§ï¼ ``` ### å³é­è³ææ¶å»
+å½ä»¤ç»æï¼```/å³é­è³ææ¶å»``` æ ```/è³ææ¶å»å³é­``` æ ```/
+åæ­¢è³ææ¶å»``` æ ```/è³ææ¶å»åæ­¢``` ä¾å¦ï¼```/
+å³é­è³ææ¶å»``` botè¿ååå®¹ï¼ ``` æ¬ç¾¤å·²å³é­
+è³ææ¶å»ï¼ä¸çæ¢å¤åå¹³ã ``` ![](docs/result.jpg) ## â æå±
+èªè¡ä¿®æ¹æºç åµ~ ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 -
+æä»¶åæ¬¡åå¸ ### 0.0.2 - è¡¥åæä»¶åä¿¡æ¯ - ä¼åææ¡£ ### 0.0.3 -
+æ°å¢å½ä»¤ å£ç æ ç¦æï¼èªå·±ç¦èªå·± ### 0.0.4 - ä¼åææ¡£ ###
+0.0.5 - æ°å¢å¯ä»¥å¼å¯ä»»ä½äººé½ä½¿ç¨éæºç¦è¨çéç½®é¡¹ ### 0.1.0
+- æ°å¢ è³ææ¶å»ï¼å°±æ¯ææäººå¯ä»¥ä½¿ç¨`éç¦`å½ä»¤ï¼åºæ¿ã
+### 0.2.0 - æ°å¢ ä¼ åçåä½å¼å®¹ï¼åãåéãæ¶ãå°æ¶ãå¤©ã
+- ä¿®æ¹ è¾ç¹ ä¸º åå¤çå½¢å¼ã - ä¼åä»£ç ã
```

