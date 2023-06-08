# Comparing `tmp/pwl-chat-python-1.4.4.tar.gz` & `tmp/pwl-chat-python-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.4.tar", last modified: Tue Jun  6 09:01:17 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.5.tar", last modified: Thu Jun  8 10:00:28 2023, max compression
```

## Comparing `pwl-chat-python-1.4.4.tar` & `pwl-chat-python-1.4.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.779948 pwl-chat-python-1.4.4/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2091 2023-06-06 09:01:17.779277 pwl-chat-python-1.4.4/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1492 2023-05-31 01:34:56.000000 pwl-chat-python-1.4.4/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.761203 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2091 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-06-06 09:01:17.000000 pwl-chat-python-1.4.4/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-06-06 09:01:17.780823 pwl-chat-python-1.4.4/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.761694 pwl-chat-python-1.4.4/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.765329 pwl-chat-python-1.4.4/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1762 2023-05-14 04:56:17.000000 pwl-chat-python-1.4.4/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.4/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.772864 pwl-chat-python-1.4.4/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2817 2023-05-14 05:06:48.000000 pwl-chat-python-1.4.4/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-14 05:27:58.000000 pwl-chat-python-1.4.4/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1933 2023-06-06 07:22:16.000000 pwl-chat-python-1.4.4/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1561 2023-05-14 05:06:43.000000 pwl-chat-python-1.4.4/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     5311 2023-06-06 08:51:30.000000 pwl-chat-python-1.4.4/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.4/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1329 2023-05-14 04:47:23.000000 pwl-chat-python-1.4.4/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-06 09:01:17.776741 pwl-chat-python-1.4.4/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      977 2023-05-14 05:48:56.000000 pwl-chat-python-1.4.4/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-06-06 08:59:05.000000 pwl-chat-python-1.4.4/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.065382 pwl-chat-python-1.4.5/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     2210 2023-06-08 10:00:28.064956 pwl-chat-python-1.4.5/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1611 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.055693 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2210 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-06-08 10:00:27.000000 pwl-chat-python-1.4.5/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-06-08 10:00:28.065520 pwl-chat-python-1.4.5/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.056207 pwl-chat-python-1.4.5/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.058008 pwl-chat-python-1.4.5/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1712 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-10 10:32:27.000000 pwl-chat-python-1.4.5/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.5/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.063104 pwl-chat-python-1.4.5/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2884 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1699 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     2159 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     2424 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1605 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     5311 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1217 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1324 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1463 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-06-08 10:00:28.064217 pwl-chat-python-1.4.5/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1044 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-06-08 10:00:05.000000 pwl-chat-python-1.4.5/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.4/LICENSE` & `pwl-chat-python-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.4/PKG-INFO` & `pwl-chat-python-1.4.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.4
+Version: 1.4.5
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -46,35 +46,38 @@
 
 ```bash
 python core.py
 ```
 
 ## 功能
 
-- 💬 基本聊天吹水；
-- ⬆️ 社区快捷命令
-  - 领取昨日活跃度奖励
-  - 查看个人积分
-  - 查看签到状态
-  - 查看当前活跃度
-  - 查看聊天室在线用户列表
-  - 查询用户详细信息
-- 🤖️ 自动复读
-- 💉 健康检查
-  - 掉线自动恢复
-- 🧠 自言自语
-  - 自定义语句池
-  - 定时发送
-- 🈲️ 小黑屋功能
-  - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
-  - 将某人从小黑屋中放出
-- 🧧 自动化抢红包（脚本哥）
-  - 自定义抢红包延时
-  - 心跳红包防止踩坑
-  - 心跳红包风险预测
-  - ~~猜拳红包百分百胜率~~
+- 💬 聊天模式
+  - 💬 聊天吹水
+  - 🤖️ 自动复读
+  - 🧠 自言自语
+    - 自定义语句池
+    - 定时发送
+  - 🧧 自动化抢红包（脚本哥）
+    - 自定义抢红包延时
+    - 心跳红包防止踩坑
+    - 心跳红包风险预测
+    - ~~猜拳红包百分百胜率~~
+- 命令模式
+  - 命令/聊天模式切换
+    - (聊天模式也可以执行命令)
+  - ⬆️ 社区快捷命令
+    - 领取昨日活跃度奖励
+    - 查看个人积分
+    - 查看签到状态
+    - 查看当前活跃度
+    - 查看在线用户列表
+    - 查询用户详细信息
+    - 🈲️ 小黑屋功能
+      - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
+      - 将某人从小黑屋中放出
+    - 发红包(待开发)
 
 ## 效果
 
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.4/README.md` & `pwl-chat-python-1.4.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -28,35 +28,38 @@
 
 ```bash
 python core.py
 ```
 
 ## 功能
 
-- 💬 基本聊天吹水；
-- ⬆️ 社区快捷命令
-  - 领取昨日活跃度奖励
-  - 查看个人积分
-  - 查看签到状态
-  - 查看当前活跃度
-  - 查看聊天室在线用户列表
-  - 查询用户详细信息
-- 🤖️ 自动复读
-- 💉 健康检查
-  - 掉线自动恢复
-- 🧠 自言自语
-  - 自定义语句池
-  - 定时发送
-- 🈲️ 小黑屋功能
-  - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
-  - 将某人从小黑屋中放出
-- 🧧 自动化抢红包（脚本哥）
-  - 自定义抢红包延时
-  - 心跳红包防止踩坑
-  - 心跳红包风险预测
-  - ~~猜拳红包百分百胜率~~
+- 💬 聊天模式
+  - 💬 聊天吹水
+  - 🤖️ 自动复读
+  - 🧠 自言自语
+    - 自定义语句池
+    - 定时发送
+  - 🧧 自动化抢红包（脚本哥）
+    - 自定义抢红包延时
+    - 心跳红包防止踩坑
+    - 心跳红包风险预测
+    - ~~猜拳红包百分百胜率~~
+- 命令模式
+  - 命令/聊天模式切换
+    - (聊天模式也可以执行命令)
+  - ⬆️ 社区快捷命令
+    - 领取昨日活跃度奖励
+    - 查看个人积分
+    - 查看签到状态
+    - 查看当前活跃度
+    - 查看在线用户列表
+    - 查询用户详细信息
+    - 🈲️ 小黑屋功能
+      - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
+      - 将某人从小黑屋中放出
+    - 发红包(待开发)
 
 ## 效果
 
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.4/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.5/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.4
+Version: 1.4.5
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -46,35 +46,38 @@
 
 ```bash
 python core.py
 ```
 
 ## 功能
 
-- 💬 基本聊天吹水；
-- ⬆️ 社区快捷命令
-  - 领取昨日活跃度奖励
-  - 查看个人积分
-  - 查看签到状态
-  - 查看当前活跃度
-  - 查看聊天室在线用户列表
-  - 查询用户详细信息
-- 🤖️ 自动复读
-- 💉 健康检查
-  - 掉线自动恢复
-- 🧠 自言自语
-  - 自定义语句池
-  - 定时发送
-- 🈲️ 小黑屋功能
-  - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
-  - 将某人从小黑屋中放出
-- 🧧 自动化抢红包（脚本哥）
-  - 自定义抢红包延时
-  - 心跳红包防止踩坑
-  - 心跳红包风险预测
-  - ~~猜拳红包百分百胜率~~
+- 💬 聊天模式
+  - 💬 聊天吹水
+  - 🤖️ 自动复读
+  - 🧠 自言自语
+    - 自定义语句池
+    - 定时发送
+  - 🧧 自动化抢红包（脚本哥）
+    - 自定义抢红包延时
+    - 心跳红包防止踩坑
+    - 心跳红包风险预测
+    - ~~猜拳红包百分百胜率~~
+- 命令模式
+  - 命令/聊天模式切换
+    - (聊天模式也可以执行命令)
+  - ⬆️ 社区快捷命令
+    - 领取昨日活跃度奖励
+    - 查看个人积分
+    - 查看签到状态
+    - 查看当前活跃度
+    - 查看在线用户列表
+    - 查询用户详细信息
+    - 🈲️ 小黑屋功能
+      - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
+      - 将某人从小黑屋中放出
+    - 发红包(待开发)
 
 ## 效果
 
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
 ![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.4/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.5/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.4/setup.py` & `pwl-chat-python-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.4/src/api/__init__.py` & `pwl-chat-python-1.4.5/src/api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import requests
 import hashlib
 import json
 
 
 class FishPi(Base):
     def __init__(self):
+        self.ws = None
         self.current_user = ''
         self.user = User()
         self.chatroom = ChatRoom()
         Base.__init__(self)
 
     def set_current_user(self, username):
         self.current_user = username
@@ -33,21 +34,19 @@
         }
         res = requests.post(HOST + "/api/getKey", json=params,
                             headers={'User-Agent': UA})
         rsp = json.loads(res.text)
         if rsp['code'] == 0:
             self.set_token(rsp['Key'])
             self.set_current_user(username)
-            print("登陆成功 欢迎" + username + '进入聊天室!')
-            print("更多功能与趣味游戏请访问网页端: " + HOST)
+            print(f'登陆成功! 更多功能与趣味游戏请访问网页端: {HOST}')
             return True
         elif rsp['code'] == -1 and rsp['msg'] == '两步验证失败，请填写正确的一次性密码':
             print("请输入两步验证码:")
             return False
         else:
-            print("登陆失败: " + rsp['msg'])
+            print(f"登陆失败: {rsp['msg']}")
             sys.exit(1)
 
     def get_yesterday_reward(self) -> dict:
-        resp = requests.get(
-            HOST + '/activity/yesterday-liveness-reward-api?apiKey=' + self.api_key, headers={'User-Agent': UA})
+        resp = requests.get(f'{HOST}/activity/yesterday-liveness-reward-api?apiKey={self.api_key}', headers={'User-Agent': UA})
         return json.loads(resp.text)
```

### Comparing `pwl-chat-python-1.4.4/src/api/chatroom.py` & `pwl-chat-python-1.4.5/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.4/src/api/user.py` & `pwl-chat-python-1.4.5/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.4/src/core/__init__.py` & `pwl-chat-python-1.4.5/src/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import json
 
 from src.api import FishPi
 from .chatroom import init_soliloquize
 from .cli import init_sys_in
-from .config import GLOBAL_CONFIG, RedPacketConfig, AuthConfig, RepeatConfig
+from .config import GLOBAL_CONFIG, RedPacketConfig, AuthConfig, ChatConfig
 import configparser
 import os
 
 
 def __init__(api: FishPi, file_path: str = None):
     if file_path is None:   
         file_path = f'{os.getcwd()}/config.ini'
     config = configparser.ConfigParser()
     try:
-        print("配置读取中")
+        print("配置读取中...")
         if not os.path.exists(file_path):
             print(f'{file_path}配置文件不存在')
             __init_default_config()
         else:
             config.read(file_path, encoding='utf-8')
             GLOBAL_CONFIG.auth_config = __init_login_auth_config(config)
             GLOBAL_CONFIG.redpacket_config = __int_redpacket_config(config)
-            GLOBAL_CONFIG.repeat_config = __init_repeat_config(config)
+            GLOBAL_CONFIG.chat_config = __init_chat_config(config)
+            GLOBAL_CONFIG.cfg_path = file_path
     except:
         print(f'{file_path}配置文件不合法')
         __init_default_config()
     init_soliloquize(api)
     init_sys_in(api)
 
 
 def __init_default_config():
     print("加载默认配置文件")
     GLOBAL_CONFIG.auth_config = AuthConfig()
     GLOBAL_CONFIG.redpacket_config = RedPacketConfig()
-    GLOBAL_CONFIG.repeat_config = RepeatConfig()
-
+    GLOBAL_CONFIG.chat_config = ChatConfig()
+    GLOBAL_CONFIG.cfg_path = None
 
 def __int_redpacket_config(config) -> RedPacketConfig:
     ret = RedPacketConfig()
     if config.getint('redPacket', 'rate') > 0:
         ret.rate = config.getint('redPacket', 'rate')
     if config.getint('redPacket', 'rpsLimit') > 0:
         ret.rps_limit = config.getint('redPacket', 'rpsLimit')            
@@ -60,16 +61,16 @@
 
 
 def __init_login_auth_config(config) -> AuthConfig:
     return AuthConfig(config.get('auth', 'username'),
                       config.get('auth', 'password'))
 
 
-def __init_repeat_config(config) -> RepeatConfig:
-    ret = RepeatConfig()
+def __init_chat_config(config) -> ChatConfig:
+    ret = ChatConfig()
     ret.repeat_mode_switch = config.getboolean('chat', 'repeatMode')
     ret.frequency = config.getint('chat', 'repeatFrequency')
     ret.soliloquize_switch = config.getboolean('chat', 'soliloquizeMode')
     ret.soliloquize_frequency = config.getint('chat', 'soliloquizeFrequency')
     ret.sentences = json.loads(config.get('chat', 'sentences'))
     ret.blacklist = json.loads(config.get('chat', 'blacklist'))
     if ret.blacklist.__contains__(''):
```

### Comparing `pwl-chat-python-1.4.4/src/core/blacklist.py` & `pwl-chat-python-1.4.5/src/core/blacklist.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,49 +2,51 @@
 import os
 import re
 from src.api import FishPi
 from .config import GLOBAL_CONFIG
 
 
 def unban_someone(api: FishPi, username):
-    if not GLOBAL_CONFIG.repeat_config.blacklist.__contains__(username):
-        print(username + '不在黑名单中')
+    if not GLOBAL_CONFIG.chat_config.blacklist.__contains__(username):
+        print(username + '不在小黑屋中')
         return
     user_info = api.user.get_user_info(username)
     if user_info is None:
         return
-    GLOBAL_CONFIG.repeat_config.blacklist.remove(username)
+    GLOBAL_CONFIG.chat_config.blacklist.remove(username)
+    print(username + '已从小黑屋中释放')
+    if GLOBAL_CONFIG.cfg_path is None:
+        return
     # 持久化到文件
-    f_path = f'{os.getcwd()}/config.ini'
-    src = open(f_path, "r+")
+    src = open(GLOBAL_CONFIG.cfg_path, "r+")
     config_text = src.read()
     src.close()
-    dst = open(f_path, 'w')
-    if len(GLOBAL_CONFIG.repeat_config.blacklist) == 0:
+    dst = open(GLOBAL_CONFIG.cfg_path, 'w')
+    if len(GLOBAL_CONFIG.chat_config.blacklist) == 0:
         after = r'blacklist=[""]'
     else:
         after = "blacklist=" + \
-            str(GLOBAL_CONFIG.repeat_config.blacklist).replace("\'", "\"")
+            str(GLOBAL_CONFIG.chat_config.blacklist).replace("\'", "\"")
     dst.write(re.sub(r'blacklist.*', after, config_text))
     dst.close()
-    print(username + '已从小黑屋中释放')
 
 
 def ban_someone(api: FishPi, username):
-    if GLOBAL_CONFIG.repeat_config.blacklist.__contains__(username):
-        print(username + ' 已在黑名单中')
+    if GLOBAL_CONFIG.chat_config.blacklist.__contains__(username):
+        print(username + ' 已在小黑屋中')
         return
     user_info = api.user.get_user_info(username)
     if user_info is None:
         return
-    GLOBAL_CONFIG.repeat_config.blacklist.append(username)
+    GLOBAL_CONFIG.chat_config.blacklist.append(username)
+    print(username + '已加入到小黑屋中')
+    if GLOBAL_CONFIG.cfg_path is None:
+        return
     # 持久化到文件
-    f_path = f'{os.getcwd()}/config.ini'
-    src = open(f_path, "r+")
+    src = open(GLOBAL_CONFIG.cfg_path, "r+")
     config_text = src.read()
     src.close()
-    dst = open(f_path, 'w')
+    dst = open(GLOBAL_CONFIG.cfg_path, 'w')
     after = "blacklist=" + \
-        str(GLOBAL_CONFIG.repeat_config.blacklist).replace("\'", "\"")
+        str(GLOBAL_CONFIG.chat_config.blacklist).replace("\'", "\"")
     dst.write(re.sub(r'blacklist.*', after, config_text))
     dst.close()
-    print(username + '已加入到黑名单中')
```

### Comparing `pwl-chat-python-1.4.4/src/core/chatroom.py` & `pwl-chat-python-1.4.5/src/core/chatroom.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,55 +4,57 @@
 from src.api import FishPi
 from .config import GLOBAL_CONFIG
 from .redpacket import rush_redpacket
 
 
 REPEAT_POOL = {}  # 复读池
 
-
-def init_soliloquize(api: FishPi):
-    if GLOBAL_CONFIG.repeat_config.soliloquize_switch:
-        schedule.every(GLOBAL_CONFIG.repeat_config.soliloquize_frequency).minutes.do(
+def init_soliloquize(api: FishPi) -> None:
+    if GLOBAL_CONFIG.chat_config.soliloquize_switch:
+        schedule.every(GLOBAL_CONFIG.chat_config.soliloquize_frequency).minutes.do(
             soliloquize, api)
 
-
-def repeat(api: FishPi, msg):
+def repeat(api: FishPi, msg) -> None:
     if not REPEAT_POOL.__contains__(msg):
         REPEAT_POOL.clear()
         REPEAT_POOL[msg] = 1
-    elif REPEAT_POOL[msg] == GLOBAL_CONFIG.repeat_config.frequency:
+    elif REPEAT_POOL[msg] == GLOBAL_CONFIG.chat_config.frequency:
         api.chatroom.send(msg)
         REPEAT_POOL[msg] = REPEAT_POOL[msg] + 1
     else:
         REPEAT_POOL[msg] = REPEAT_POOL[msg] + 1
 
 
-def soliloquize(api: FishPi):
-    length = len(GLOBAL_CONFIG.repeat_config.sentences)
+def soliloquize(api: FishPi) -> None:
+    length = len(GLOBAL_CONFIG.chat_config.sentences)
     index = random.randint(0, length - 1)
-    api.chatroom.send(GLOBAL_CONFIG.repeat_config.sentences[index])
+    api.chatroom.send(GLOBAL_CONFIG.chat_config.sentences[index])
 
 
-def listener(api: FishPi, message):
+def listener(api: FishPi, message) -> None:
     if message['type'] == 'msg':
         if message['content'].find("redPacket") != -1:
             rush_redpacket(api, message)
         else:
             time = message['time']
             user = message['userName']
-            if len(GLOBAL_CONFIG.repeat_config.blacklist) > 0 \
-                    and GLOBAL_CONFIG.repeat_config.blacklist.__contains__(user):
+            user_nick_name = message['userNickname']
+            if len(GLOBAL_CONFIG.chat_config.blacklist) > 0 \
+                    and GLOBAL_CONFIG.chat_config.blacklist.__contains__(user):
                 return
             if user == GLOBAL_CONFIG.auth_config.username:
                 print('\t\t\t\t\t\t[' + time + ']')
                 print('\t\t\t\t\t\t你说: ' + message['md'])
             else:
                 if 'client' in message:
                     print('[' + time + '] 来自(' + message['client']+')')
                 else:
                     print('[' + time + ']')
-                print(user + '说:')
+                if len(user_nick_name) >0:
+                    print(f'{user_nick_name}({user})说:')
+                else:
+                    print(f'{user}说:')    
                 print(message['md'])
                 print('\r\n')
-            if GLOBAL_CONFIG.repeat_config.repeat_mode_switch:
+            if GLOBAL_CONFIG.chat_config.repeat_mode_switch:
                 msg = message['md']
                 repeat(api, msg)
```

### Comparing `pwl-chat-python-1.4.4/src/core/cli.py` & `pwl-chat-python-1.4.5/src/core/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import _thread
 from .blacklist import *
 from .config import GLOBAL_CONFIG
 from .user import *
+from .websocket import chatroom_in,chatroom_out
 from src.utils.utils import *
 
 
 
 
 def init_sys_in(api: FishPi):
     _thread.start_new_thread(console_input, (api,))
@@ -14,15 +15,24 @@
 def console_input(api: FishPi):
     while True:
         msg = input("")
         if msg == '#help':
             print(COMMAND_GUIDE)
         elif len(api.api_key) == 0:
             api.login(GLOBAL_CONFIG.auth_config.username,
-                      GLOBAL_CONFIG.auth_config.password, msg)
+                      GLOBAL_CONFIG.auth_config.password, msg)                
+        elif msg == '#cli':
+            if api.ws == None:
+                print("已经进入交互模式了")
+            else:    
+                chatroom_out(api)
+                print("进入交互模式")
+        elif msg == '#chatroom':
+            if api.ws == None:
+               api.ws = chatroom_in(api)
         elif msg == '#checked':
             if api.user.checked_status()['checkedIn']:
                 print('今日你已签到！')
             else:
                 print('今日还未签到，摸鱼也要努力呀！')
         elif msg == '#reward':
             reward = api.get_yesterday_reward()['sum']
@@ -30,26 +40,28 @@
                 print('你已经领取过昨日活跃度奖励了')
             else:
                 print(f'领取昨日活跃度奖励 积分: {reward}')
         elif msg == '#liveness':
             print('当前活跃度: ' +
                   str(api.user.get_liveness_info()['liveness']))
         elif msg == '#point':
-            print(
-                '当前积分: ' + str(api.user.get_user_info(GLOBAL_CONFIG.auth_config.username)['userPoint']))
+            print('当前积分: ' + str(api.user.get_user_info(GLOBAL_CONFIG.auth_config.username)['userPoint']))
         elif msg == '#online-users':
             render_online_users(api)
         elif msg.startswith('#user '):
             user = msg.split()[1]
             userInfo = api.user.get_user_info(user)
             if userInfo is not None:
                 render_user_info(userInfo)
         elif msg == '#blacklist':
-            print(GLOBAL_CONFIG.repeat_config.blacklist)
+            print(GLOBAL_CONFIG.chat_config.blacklist)
         elif msg.startswith('#ban '):
             user = msg.split()[1]
             ban_someone(api, user)
         elif msg.startswith('#unban '):
             user = msg.split()[1]
             unban_someone(api, user)
+        elif msg.startswith('#'):
+            print('命令错误,请查看命令引导手册')
+            print(COMMAND_GUIDE)
         else:
             api.chatroom.send(msg)
```

### Comparing `pwl-chat-python-1.4.4/src/core/config.py` & `pwl-chat-python-1.4.5/src/core/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 class AuthConfig(object):
     def __init__(self, username='', password='', mfa_code=''):
         self.username = username
         self.password = password
         self.mfa_code = mfa_code
 
 
-class RepeatConfig(object):
+class ChatConfig(object):
     def __init__(self, blacklist=[], repeat_mode_switch=False, frequency=5, soliloquize_switch=False,
                  soliloquize_frequency=20, sentences=[]):
         self.repeat_mode_switch = repeat_mode_switch
         self.frequency = frequency
         self.soliloquize_switch = soliloquize_switch
         self.soliloquize_frequency = soliloquize_frequency
         self.sentences = ['你们好！', '牵着我的手，闭着眼睛走你也不会迷路。',
                           '吃饭了没有?', '💗 爱你哟！'] + sentences
         self.blacklist = blacklist
 
 
 class Config(object):
-    def __init__(self, auth: AuthConfig = None, redpacket: RedPacketConfig = None, repeat: RepeatConfig = None):
+    def __init__(self, auth: AuthConfig = None, redpacket: RedPacketConfig = None, chat: ChatConfig = None, cfg_path :str = None):
         self.auth_config = auth
         self.redpacket_config = redpacket
-        self.repeat_config = repeat
-
+        self.chat_config = chat
+        self.cfg_path = cfg_path
 
 GLOBAL_CONFIG = Config()
```

### Comparing `pwl-chat-python-1.4.4/src/core/redpacket.py` & `pwl-chat-python-1.4.5/src/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.4/src/core/websocket.py` & `pwl-chat-python-1.4.5/src/core/websocket.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import json
 import ssl
 import rel
-import time
 import schedule
 import websocket
-import _thread
 
 from src.api import FishPi
 from .chatroom import listener
 from .config import GLOBAL_CONFIG
 
 __api = FishPi()
 def on_message(ws, message):
@@ -17,37 +15,33 @@
 
 
 def on_error(ws, error):
     print(error)
 
 
 def on_close(ws, close_status_code, close_msg):
-    print("### closed ###")
+    print("已经离开聊天室,可以执行命令 #chatroom 重新进入聊天室")
 
 
-def heartbeat(ws):
-    while True:
-        time.sleep(60)
-        ws.send("-hb-")
-        if GLOBAL_CONFIG.repeat_config.soliloquize_switch:
-            schedule.run_pending()
-
 
 def on_open(ws):
-    _thread.start_new_thread(heartbeat, (ws,))
+    print(f'欢迎{__api.current_user}进入聊天室!')
+    if len(GLOBAL_CONFIG.chat_config.blacklist) > 0:
+        print('小黑屋成员: ' + str(GLOBAL_CONFIG.chat_config.blacklist))
+    if GLOBAL_CONFIG.chat_config.soliloquize_switch:
+            schedule.run_pending()
 
+def chatroom_out(api: FishPi):
+    api.ws.close()
+    api.ws = None
 
-def start(api: FishPi):
+def chatroom_in(api: FishPi) -> websocket.WebSocketApp:
     global __api
     __api = api
-
-    rel.safe_read()
     websocket.enableTrace(False)
     ws = websocket.WebSocketApp("wss://fishpi.cn/chat-room-channel?apiKey=" + api.api_key,
                                 on_open=on_open,
                                 on_message=on_message,
                                 on_error=on_error,
                                 on_close=on_close)
     ws.run_forever(dispatcher=rel, sslopt={"cert_reqs": ssl.CERT_NONE})
-    print("进入聊天室")
-    rel.signal(2, rel.abort)
-    rel.dispatch()
+    return ws
```

### Comparing `pwl-chat-python-1.4.4/src/main.py` & `pwl-chat-python-1.4.5/src/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import click
+import rel
 from src.core import __init__
 from src.core.config import GLOBAL_CONFIG, AuthConfig
 from src.core.user import login
-from src.core.websocket import start
+from src.core.websocket import chatroom_in
 from src.utils.version import __version__
 from src.api import FishPi
 
 
 class CliConfig(object):
     def __init__(self, username: str = '', password: str = '', code: str = '', file_path: str = None):
         self.username = username
@@ -19,16 +20,22 @@
 def run(config: CliConfig):
     api = FishPi()
     __init__(api, config.file_path)
     if config.username is not None and config.password is not None:
         GLOBAL_CONFIG.auth_config = AuthConfig(
             config.username, config.password, config.code)
     login(api)
-    start(api)
-
+    rel.safe_read()
+    api.ws = chatroom_in(api)
+    pending()
+
+    
+def pending():
+    rel.signal(2, rel.abort)
+    rel.dispatch()
 
 @click.command()
 @click.version_option(__version__)
 @click.option("--username", "-u", type=click.STRING, help="摸鱼派用户名")
 @click.option("--password", "-p", type=click.STRING, help="密码")
 @click.option("--code", "-c", type=click.STRING, help="两步验证码")
 @click.option("--file_path", "-f", type=click.STRING, help="配置文件路径")
```

