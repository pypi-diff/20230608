# Comparing `tmp/pymino-1.1.8.5.tar.gz` & `tmp/pymino-1.1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.8.3\dist\.tmp-fitrcryk\pymino-1.1.8.5.tar", last modified: Mon May 29 04:02:43 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\sub\dist\.tmp-xekccvso\pymino-1.1.8.6.tar", last modified: Thu Jun  8 12:38:37 2023, max compression
```

## Comparing `pymino-1.1.8.5.tar` & `pymino-1.1.8.6.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.438526 pymino-1.1.8.5/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.5/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-05-29 04:02:43.439022 pymino-1.1.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.170687 pymino-1.1.8.5/pymino/
--rw-rw-rw-   0        0        0      721 2023-05-29 04:00:48.000000 pymino-1.1.8.5/pymino/__init__.py
--rw-rw-rw-   0        0        0     8112 2023-05-29 00:01:55.000000 pymino-1.1.8.5/pymino/async_bot.py
--rw-rw-rw-   0        0        0    27542 2023-05-29 00:04:00.000000 pymino-1.1.8.5/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.8.5/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.205407 pymino-1.1.8.5/pymino/ext/
--rw-rw-rw-   0        0        0      469 2023-05-28 22:44:43.000000 pymino-1.1.8.5/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.8.5/pymino/ext/account.py
--rw-rw-rw-   0        0        0   273903 2023-05-29 04:01:53.000000 pymino-1.1.8.5/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18163 2023-05-28 22:59:05.000000 pymino-1.1.8.5/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24302 2023-05-29 04:00:13.000000 pymino-1.1.8.5/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7299 2023-05-29 00:25:30.000000 pymino-1.1.8.5/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   271224 2023-05-25 22:50:46.000000 pymino-1.1.8.5/pymino/ext/community.py
--rw-rw-rw-   0        0        0    44587 2023-05-29 00:03:54.000000 pymino-1.1.8.5/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.5/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.352719 pymino-1.1.8.5/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.8.5/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.5/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14847 2023-05-28 23:41:49.000000 pymino-1.1.8.5/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    52847 2023-05-27 20:44:10.000000 pymino-1.1.8.5/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4763 2023-05-29 00:33:12.000000 pymino-1.1.8.5/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.8.5/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6185 2023-05-25 23:01:02.000000 pymino-1.1.8.5/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.5/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.5/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.5/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     7088 2023-05-29 00:33:01.000000 pymino-1.1.8.5/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.437534 pymino-1.1.8.5/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.5/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.5/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.5/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.5/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.8.5/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.191023 pymino-1.1.8.5/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1011 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-05-29 04:02:43.450430 pymino-1.1.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.371657 pymino-1.1.8.6/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.6/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-06-08 12:38:37.372154 pymino-1.1.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.293784 pymino-1.1.8.6/pymino/
+-rw-rw-rw-   0        0        0      721 2023-06-08 12:38:10.000000 pymino-1.1.8.6/pymino/__init__.py
+-rw-rw-rw-   0        0        0     7879 2023-06-08 12:33:52.000000 pymino-1.1.8.6/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    27301 2023-06-08 12:33:51.000000 pymino-1.1.8.6/pymino/bot.py
+-rw-rw-rw-   0        0        0    52021 2023-06-08 12:36:59.000000 pymino-1.1.8.6/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.338424 pymino-1.1.8.6/pymino/ext/
+-rw-rw-rw-   0        0        0      474 2023-06-08 05:17:39.000000 pymino-1.1.8.6/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    13871 2023-06-08 12:06:58.000000 pymino-1.1.8.6/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   287511 2023-06-08 12:33:03.000000 pymino-1.1.8.6/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    17955 2023-06-08 12:35:46.000000 pymino-1.1.8.6/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    23899 2023-06-08 07:29:50.000000 pymino-1.1.8.6/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7098 2023-06-08 07:26:50.000000 pymino-1.1.8.6/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   284982 2023-06-08 12:32:12.000000 pymino-1.1.8.6/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    41392 2023-06-08 07:22:51.000000 pymino-1.1.8.6/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.6/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.363225 pymino-1.1.8.6/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      312 2023-06-08 07:25:34.000000 pymino-1.1.8.6/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     1670 2023-06-08 12:22:47.000000 pymino-1.1.8.6/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    20323 2023-06-08 12:02:08.000000 pymino-1.1.8.6/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-08 11:59:16.000000 pymino-1.1.8.6/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.6/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15812 2023-06-08 11:41:30.000000 pymino-1.1.8.6/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-08 08:03:53.000000 pymino-1.1.8.6/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4763 2023-05-29 00:33:12.000000 pymino-1.1.8.6/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-08 08:11:36.000000 pymino-1.1.8.6/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0    42516 2023-06-08 07:28:10.000000 pymino-1.1.8.6/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1847 2023-06-08 07:26:04.000000 pymino-1.1.8.6/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.6/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.6/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.6/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6833 2023-06-08 07:28:43.000000 pymino-1.1.8.6/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.370665 pymino-1.1.8.6/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.6/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.6/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.6/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.6/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-06-08 12:27:04.000000 pymino-1.1.8.6/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:38:37.311640 pymino-1.1.8.6/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1153 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 12:38:37.000000 pymino-1.1.8.6/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-06-08 12:38:37.376120 pymino-1.1.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.6/setup.py
```

### Comparing `pymino-1.1.8.5/LICENSE` & `pymino-1.1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/PKG-INFO` & `pymino-1.1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.5
+Version: 1.1.8.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.5/README.md` & `pymino-1.1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/__init__.py` & `pymino-1.1.8.6/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.8.5'
+__version__ = '1.1.8.6'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.8.5/pymino/async_bot.py` & `pymino-1.1.8.6/pymino/async_bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import asyncio
-from time import time, perf_counter
 from typing import Optional, Union
+from time import time, perf_counter
 
-from .ext.entities.handlers import *
+from .ext.entities import *
 from .ext.async_socket import AsyncWSClient
 from .ext.async_community import AsyncCommunity
-from .ext.entities.general import ApiResponse
 from .ext.utilities.generate import device_id
-from .ext.entities.userprofile import UserProfile
 from .ext.utilities.async_request_handler import AsyncRequestHandler
 
-from .ext.entities.exceptions import (
-    LoginFailed, MissingEmailPasswordOrSid,
-    VerifyCommunityIdIsCorrect, PingFailed
-    )
-
 
 class AsyncBot(AsyncWSClient):
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
         online_status: bool = True,
@@ -235,9 +228,9 @@
     async def ping(self) -> float:
         try:
             start = perf_counter()
             await self.request.handler(method="GET", url="/g/s/account")
             end = perf_counter()
             elapsed_time_ms = (end - start) * 1000
             return round(elapsed_time_ms, 2)
-        except Exception:
-            raise PingFailed
+        except Exception as e:
+            raise PingFailed from e
```

### Comparing `pymino-1.1.8.5/pymino/bot.py` & `pymino-1.1.8.6/pymino/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from time import perf_counter, time
 from typing import Optional, Union
+from time import perf_counter, time
 
+from .ext.entities import *
 from .ext.socket import WSClient
 from .ext.account import Account
 from .ext.community import Community
-from .ext.entities.handlers import *
 from .ext.utilities.generate import device_id
-from .ext.entities.userprofile import UserProfile
 from .ext.utilities.request_handler import RequestHandler
-from .ext.entities.general import ApiResponse, CCommunity
-from .ext.entities.exceptions import (
-    LoginFailed, MissingEmailPasswordOrSid,
-    VerifyCommunityIdIsCorrect, PingFailed
-    )
+
 
 class Bot(WSClient):
     """
     `Bot` - This is the main client.
 
     `**Parameters**``
     - `command_prefix` - The prefix to use for commands. `Defaults` to `!`.
@@ -708,9 +703,9 @@
         """
         try:
             start = perf_counter()
             self.request.handler(method="GET", url="/g/s/account")
             end = perf_counter()
             elapsed_time_ms = (end - start) * 1000
             return round(elapsed_time_ms, 2)
-        except Exception:
-            raise PingFailed
+        except Exception as e:
+            raise PingFailed from e
```

### Comparing `pymino-1.1.8.5/pymino/client.py` & `pymino-1.1.8.6/pymino/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 from time import time
 from typing import Any, Callable, Optional, TypeVar, Union
 
-from .ext.entities.handlers import *
-from .ext.entities.userprofile import UserProfile
+from .ext.entities import *
 from .ext import RequestHandler, Account, Community
-from .ext.entities.messages import CMessage, PrepareMessage
-
 from .ext.utilities.generate import device_id as generate_device_id
-from .ext.entities.exceptions import (
-    LoginFailed, LoginRequired, MissingEmailPasswordOrSid, VerifyCommunityIdIsCorrect
-    )
-from .ext.entities.general import (
-    ApiResponse, Authenticate, CCommunity, CCommunityList, ResetPassword, Wallet, LinkInfo
-    )
+
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 class Client:
     """
     `Client` - This is the main client.
 
@@ -1151,7 +1143,115 @@
         can be passed as keyword arguments. The method calls the `PrepareMessage` object's `json` method to prepare the message
         data. The result is a `CMessage` object containing the details of the sent message.
         """
         return CMessage(self.request.handler(
             method="POST", url=f"/g/s/chat/thread/{chatId}/message",
             data = PrepareMessage(content=content, **kwargs).json()
             ))
+
+
+    @authenticated
+    def edit_profile(
+        self,
+        nickname: str = None,
+        content: str = None,
+        icon: str = None,
+        backgroundColor: str = None,
+        backgroundImage: str = None,
+        defaultBubbleId: str = None
+        ) -> UserProfile:
+        """
+        Edits the user's profile.
+
+        :param nickname: The new nickname for the user.
+        :type nickname: str
+        :param content: The new content for the user's profile.
+        :type content: str
+        :param icon: The new icon image file for the user.
+        :type icon: str
+        :param backgroundColor: The new background color for the user's profile.
+        :type backgroundColor: str
+        :param backgroundImage: The new background image file for the user's profile.
+        :type backgroundImage: str
+        :param defaultBubbleId: The ID of the default bubble for the user's profile.
+        :type defaultBubbleId: str
+        :return: The response from the account's `edit_profile` method.
+        :rtype: Response
+
+        This method allows the authenticated user to edit their profile settings. Different aspects of the profile can be modified,
+        such as the nickname, content, icon, background color, background image, and default bubble. Only the specified parameters will
+        be updated. The `userId` parameter is set to the authenticated user's ID automatically.
+
+        **Example usage:**
+
+        To change the nickname and icon for the user:
+
+        >>> response = client.edit_profile(nickname="New Nickname", icon="path/to/icon.jpg")
+        ... if response.status == 200:
+        ...     print("Profile edited successfully!")
+        ... else:
+        ...     print("Failed to edit profile.")
+        """
+        return self.account.edit_profile(userId = self.userId,
+                                         nickname = nickname,
+                                         content = content,
+                                         icon = icon,
+                                         backgroundColor = backgroundColor,
+                                         backgroundImage = backgroundImage,
+                                         defaultBubbleId = defaultBubbleId
+                                         )
+
+
+    @authenticated
+    def start_chat(
+        self,
+        userId: Union[str, list],
+        message: str,
+        title: str = None,
+        content: str = None,
+        isGlobal: bool = False,
+        publishToGlobal: bool = False
+        ) -> ChatThread:
+        """
+        Starts a chat thread.
+        :param userId: The ID or list of IDs of the users to invite to the chat.
+        :type userId: Union[str, list]
+        :param message: The initial message content.
+        :type message: str
+        :param title: The title of the chat thread (optional).
+        :type title: str, optional
+        :param content: Additional content for the message (optional).
+        :type content: str, optional
+        :param isGlobal: Indicates if the chat is global (optional, default: False).
+        :type isGlobal: bool, optional
+        :param publishToGlobal: Indicates if the chat should be published globally (optional, default: False).
+        :type publishToGlobal: bool, optional
+        :return: A `ChatThread` object representing the created chat thread.
+        :rtype: ChatThread
+        """
+        try:
+            userIds = [userId] if isinstance(userId, str) else userId
+        except Exception as e:
+            raise ValueError("Incorrect type for userId. <--- userId can be only a string or a list.") from e
+
+        data = dict(
+            title = title,
+            inviteeUids = userIds,
+            initialMessageContent = message,
+            content = content,
+            timestamp = int(time() * 1000),
+            publishToGlobal = 0
+        )
+
+        if isGlobal: data.update({"type": 2, "eventSource": "GlobalComposeMenu"})
+        else: data["type"] = 0
+
+        if publishToGlobal: data["publishToGlobal"] = 1
+
+        return ChatThread(
+            self.request.handler(method="POST", url="/g/s/chat/thread", data=data)
+        )
+
+
+
+
+
```

### Comparing `pymino-1.1.8.5/pymino/ext/account.py` & `pymino-1.1.8.6/pymino/ext/account.py`

 * *Files 12% similar despite different names*

```diff
@@ -371,7 +371,80 @@
                     "identity": email,
                     "level": 2,
                     "deviceID": deviceId
                 },
                 "phoneNumberValidationContext": None,
                 "deviceID": deviceId
             }))
+
+
+    def edit_profile(
+        self,
+        userId: str,
+        nickname: str = None,
+        content: str = None,
+        icon: str = None,
+        backgroundColor: str = None,
+        backgroundImage: str = None,
+        defaultBubbleId: str = None
+        ) -> UserProfile:
+        """
+        `edit_profile` - Edits the user profile.
+
+        `Parameters`:
+        - `userId` (str): The ID of the user profile to edit.
+        - `nickname` (str, optional): The new nickname for the user.
+        - `content` (str, optional): The new content for the user profile.
+        - `icon` (str, optional): The path or URL of the new icon image for the user profile.
+        - `backgroundColor` (str, optional): The new background color for the user profile.
+        - `backgroundImage` (str, optional): The path or URL of the new background image for the user profile.
+        - `defaultBubbleId` (str, optional): The ID of the default bubble for the user profile.
+
+        `Returns`:
+        An instance of the `UserProfile` class representing the updated user profile.
+
+        `Example`:
+        ```python
+        from pymino import *
+
+        bot = Bot()
+        bot.run(email=email, password=password)
+        response = bot.edit_profile(userId="12345", nickname="NewNickname", content="NewContent", backgroundColor="#FFFFFF")
+        print(response.json)
+        ```
+        """
+        data = {
+                "address": None,
+                "latitude": 0,
+                "longitude": 0,
+                "mediaList": None,
+                "eventSource": "UserProfileView",
+                "timestamp": int(time() * 1000),
+        }
+
+        if nickname: data['nickname'] = nickname
+        if icon: data['icon'] = self.upload_image(icon)
+        if content: data['content'] = content
+        if backgroundColor:
+            data["extensions"] = {
+                "style": {
+                    "backgroundColor": backgroundColor
+                    if backgroundColor.startswith("#")
+                    else f"#{backgroundColor}"
+                }
+            }
+
+        if backgroundImage:
+            data["extensions"] = {
+                "style": {
+                    "backgroundMediaList": [
+                        [100, self.upload_image(backgroundImage), None, None, None]
+                    ]
+                }
+            }
+        if defaultBubbleId:
+            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+
+        return UserProfile(self.session.handler(
+            method = "POST", url = f"/g/s/user-profile/{userId}",
+            data = data
+        ))
```

### Comparing `pymino-1.1.8.5/pymino/ext/async_community.py` & `pymino-1.1.8.6/pymino/ext/async_community.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,31 +7,15 @@
 from time import time, timezone
 
 from typing import (
     BinaryIO, Callable, List,
     Optional, Union, TypeVar, Any
     )
 
-from .entities.enums import *
-from .entities.threads import CThread, CThreadList
-from .entities.userprofile import UserProfile, UserProfileList
-
-from .entities.messages import (
-    CMessage, CMessages, PrepareMessage
-    )
-from .entities.exceptions import (
-    InvalidImage, MissingCommunityId,
-    MissingTimers, NoDataProvided, NotLoggedIn
-    )
-from .entities.general import (
-    ApiResponse, CBlog, CBlogList, CChatMembers,
-    CComment, CCommentList, CCommunity, CCommunityList,
-    CheckIn, CommunityInvitation, Coupon, FeaturedBlogs,
-    InvitationId, LinkInfo, NotificationList, QuizRankingList
-    )
+from .entities import *
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 class AsyncCommunity:
     """
     The `Community` class handles community related actions.
 
@@ -1330,36 +1314,36 @@
         return UserProfileList(
             await self.session.handler(
             method="GET",
             url=f"/x{self.community_id if comId is None else comId}/s/user-profile/{userId}/joined?start={start}&size={size}"
             ))
 
     @community
-    async def fetch_chat(self, chatId: str, comId: Union[str, int] = None) -> CThread:
+    async def fetch_chat(self, chatId: str, comId: Union[str, int] = None) -> ChatThread:
         """
         Fetches the chat thread with the specified ID in the current or specified community.
 
         :param chatId: The ID of the chat thread to fetch.
         :type chatId: str
         :param comId: The ID of the community to fetch the chat thread from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThread` object containing information about the chat thread.
-        :rtype: CThread
+        :return: A `ChatThread` object containing information about the chat thread.
+        :rtype: ChatThread
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch the chat thread with the specified ID.
 
-        `CThread`:
+        `ChatThread`:
 
         - `data`: The raw data of the chat thread.
         - `userAddedTopicList`: A list of topics added by the user.
         - `uid`: The user ID of the thread creator.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: The maximum number of members allowed in the chat thread.
         - `membersSummary`: A `MemberSummary` object containing information about the chat thread's members.
         - `threadId`: The ID of the chat thread.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the chat thread.
         - `membersCount`: The number of members currently in the chat thread.
         - `strategyInfo`: The strategy information for the chat thread.
@@ -1379,15 +1363,15 @@
 
         **Example usage:**
 
         >>> chat_thread = client.community.fetch_chat("0000-000000-000000-0000")
         >>> print(chat_thread.title) # Prints the title of the chat thread.
         'My Chat Thread'
         """
-        return CThread(
+        return ChatThread(
             await self.session.handler(
             method="GET",
             url=f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}"
             ))
 
     
     @community
@@ -1404,20 +1388,20 @@
             - "co-hosts": Returns only the co-hosts of the chat.
             - "host": Returns only the host of the chat.
         :type moderators: Optional[str]
         :raises NotLoggedIn: If the user is not logged in.
         :return: A list of moderator user IDs.
         :rtype: List[str]
         """
-        response: CThread = await self.fetch_chat(chatId=chatId, comId=comId)
+        response: ChatThread = await self.fetch_chat(chatId=chatId, comId=comId)
 
         return {
-            "all": list(response.extensions.coHost) + [response.hostUserId],
-            "co-hosts": list(response.extensions.coHost),
-            "host": [response.hostUserId]
+            "all": list(response.extensions.coHosts) + [response.host_user_id],
+            "co-hosts": list(response.extensions.coHosts),
+            "host": [response.host_user_id]
             }.get(moderators, "all")
 
 
     @community
     async def fetch_chat_moderators(self, chatId: str, comId: Union[str, int] = None) -> List[str]:
         """
         Fetches a list of all moderators for a specified chat thread in the current or specified community.
@@ -1459,40 +1443,40 @@
         :return: The user ID of the chat host.
         :rtype: str
         """
         return self.fetch_chat_mods(chatId=chatId, comId=comId, moderators="host")[0]
 
 
     @community
-    async def fetch_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CThreadList:
+    async def fetch_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> ChatThreadList:
         """
         Fetches a list of chat threads in the current or specified community that the user has joined.
 
         :param start: The starting point to fetch chat threads from. Defaults to `0`.
         :type start: int
         :param size: The amount of chat threads to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the chat threads from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThreadList` object containing information about the chat threads.
-        :rtype: CThreadList
+        :return: A `ChatThreadList` object containing information about the chat threads.
+        :rtype: ChatThreadList
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch a list of chat threads that the user has joined.
 
-        `CThreadList`:
+        `ChatThreadList`:
 
         - `data`: The raw data of the chat thread list.
         - `extensions`: The extensions of the chat threads in the list.
         - `membersSummary`: The member summary of the chat threads in the list.
         - `userAddedTopicList`: A list of topics added by the user in the chat threads in the list.
         - `uid`: A list of user IDs of the thread creators in the chat threads in the list.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: A list of maximum member counts allowed in the chat threads in the list.
         - `threadId`: A list of thread IDs of the chat threads in the list.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the chat threads in the list.
         - `membersCount`: A list of the number of members in the chat threads in the list.
         - `strategyInfo`: The strategy information for the chat threads in the list.
         - `isPinned`: A list of whether the chat threads in the list are pinned.
@@ -1517,48 +1501,48 @@
         ['My Chat Thread', 'My Other Chat Thread']
         METHOD 2:
         >>> for chat_thread in chat_threads:
         ...     print(chat_thread.title)
         'My Chat Thread'
         'My Other Chat Thread'
         """
-        return CThreadList(
+        return ChatThreadList(
             await self.session.handler(
             method="GET",
             url=f"/x{self.community_id if comId is None else comId}/s/chat/thread?type=joined-me&start={start}&size={size}"
             ))
 
 
     @community
-    async def fetch_live_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CThreadList:
+    async def fetch_live_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> ChatThreadList:
         """
         Fetches a list of live chat threads in the current or specified community that are publicly visible.
 
         :param start: The starting point to fetch chat threads from. Defaults to `0`.
         :type start: int
         :param size: The amount of chat threads to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the chat threads from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThreadList` object containing information about the live chat threads.
-        :rtype: CThreadList
+        :return: A `ChatThreadList` object containing information about the live chat threads.
+        :rtype: ChatThreadList
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch a list of publicly visible live chat threads.
 
-        `CThreadList`:
+        `ChatThreadList`:
 
         - `data`: The raw data of the live chat thread list.
         - `extensions`: The extensions of the live chat threads in the list.
         - `membersSummary`: The member summary of the live chat threads in the list.
         - `userAddedTopicList`: A list of topics added by the user in the live chat threads in the list.
         - `uid`: A list of user IDs of the thread creators in the live chat threads in the list.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: A list of maximum member counts allowed in the live chat threads in the list.
         - `threadId`: A list of thread IDs of the live chat threads in the list.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the live chat threads in the list.
         - `membersCount`: A list of the number of members in the live chat threads in the list.
         - `strategyInfo`: The strategy information for the live chat threads in the list.
         - `isPinned`: A list of whether the live chat threads in the list are pinned.
@@ -1583,63 +1567,63 @@
         ['My Live Chat Thread', 'My Other Live Chat Thread']
         METHOD 2:
         >>> for title in live_chat_titles:
         ...     print(title) # Prints the title of each live chat thread.
         'My Live Chat Thread'
         'My Other Live Chat Thread'
         """
-        return CThreadList(
+        return ChatThreadList(
             await self.session.handler(
             method="GET",
             url=f"/x{self.community_id if comId is None else comId}/s/live-layer/public-live-chats?start={start}&size={size}"
             ))
 
 
     @community
     async def fetch_public_chats(
         self,
         chatType: ChatTypes = ChatTypes.RECOMMENDED,
         start: int = 0,
         size: int = 25,
         comId: Union[str, int] = None,
         **kwargs
-        ) -> CThreadList:
+        ) -> ChatThreadList:
         """
         Fetches a list of public chat threads in the current or specified community.
 
         :param chatType: The type of public chat threads to fetch. Defaults to `ChatTypes.RECOMMENDED`.
         :type chatType: ChatTypes
         :param start: The starting point to fetch chat threads from. Defaults to `0`.
         :type start: int
         :param size: The amount of chat threads to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the chat threads from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThreadList` object containing information about the public chat threads.
-        :rtype: CThreadList
+        :return: A `ChatThreadList` object containing information about the public chat threads.
+        :rtype: ChatThreadList
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch a list of public chat threads of the specified type.
 
         `ChatTypes`:
 
         - `RECOMMENDED`: Fetches a list of recommended public chat threads.
         - `POPULAR`: Fetches a list of popular public chat threads.
         - `LATEST`: Fetches a list of newest public chat threads.
 
-        `CThreadList`:
+        `ChatThreadList`:
 
         - `data`: The raw data of the public chat thread list.
         - `extensions`: The extensions of the public chat threads in the list.
         - `membersSummary`: The member summary of the public chat threads in the list.
         - `userAddedTopicList`: A list of topics added by the user in the public chat threads in the list.
         - `uid`: A list of user IDs of the thread creators in the public chat threads in the list.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: A list of maximum member counts allowed in the public chat threads in the list.
         - `threadId`: A list of thread IDs of the public chat threads in the list.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the public chat threads in the list.
         - `membersCount`: A list of the number of members in the public chat threads in the list.
         - `strategyInfo`: The strategy information for the public chat threads in the list.
         - `isPinned`: A list of whether the public chat threads in the list are pinned.
@@ -1668,15 +1652,15 @@
         'My Public Chat Thread'
         'My Other Public Chat Thread'
         """
         if "type" in kwargs: #TODO Remove this in the near future.
             chatType = kwargs["type"]
             print("WARNING: The `type` parameter is deprecated. Please use `chatType` instead.")
 
-        return CThreadList(
+        return ChatThreadList(
             await self.session.handler(
             method="GET",
             url=f"/x{self.community_id if comId is None else comId}/s/chat/thread?type=public-all&filterType={chatType.value if isinstance(chatType, ChatTypes) else chatType}&start={start}&size={size}"
             ))
 
 
     @community
@@ -2053,15 +2037,15 @@
     async def fetch_comments(
         self,
         userId: Optional[str] = None,
         blogId: Optional[str] = None,
         wikiId: Optional[str] = None,
         start: int = 0,
         size: int = 25,
-        comId: Union[str, int] = None) -> CCommentList:
+        comId: Union[str, int] = None) -> CommentList:
         """
         Fetches the comments for the specified user, blog, or wiki.
 
         :param userId: The ID of the user whose comments to fetch. Defaults to `None`.
         :type userId: Optional[str]
         :param blogId: The ID of the blog whose comments to fetch. Defaults to `None`.
         :type blogId: Optional[str]
@@ -2069,23 +2053,23 @@
         :type wikiId: Optional[str]
         :param start: The starting index of the comments to fetch. Defaults to `0`.
         :type start: int
         :param size: The number of comments to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the comments from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CCommentList` object containing the comments for the specified user, blog, or wiki.
-        :rtype: CCommentList
+        :return: A `CommentList` object containing the comments for the specified user, blog, or wiki.
+        :rtype: CommentList
         :raises NoDataProvided: If none of `userId`, `blogId`, or `wikiId` is provided.
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch the comments for the specified user, blog, or wiki.
 
-        `CCommentList`:
+        `CommentList`:
 
         - `modifiedTime`: A list of the last modified time of each comment.
         - `ndcId`: A list of the NDC IDs of each comment.
         - `votedValue`: A list of the voted value of each comment.
         - `parentType`: A list of the parent types of each comment.
         - `commentId`: A list of the IDs of each comment.
         - `parentNdcId`: A list of the parent NDC IDs of each comment.
@@ -2115,15 +2099,15 @@
         if any([userId, blogId, wikiId]):
             for key, value in {
                 "userId": "user-profile/{}",
                 "blogId": "blog/{}",
                 "wikiId": "item/{}"
             }.items():
                 if locals()[key]:
-                    return CCommentList(
+                    return CommentList(
                         self.session.handler(
                             method="GET",
                             url=f"/x{self.community_id if comId is None else comId}/s/{value.format(locals()[key])}/comment?sort=newest&start={start}&size={size}",
                         )
                     )
 
         raise NoDataProvided
@@ -2685,15 +2669,15 @@
         self,
         content: str,
         userId: Optional[str] = None,
         blogId: Optional[str] = None,
         wikiId: Optional[str] = None,
         image: Optional[str] = None,
         comId: Union[str, int] = None
-        ) -> CComment:
+        ) -> Comment:
         """
         Creates a comment in the current or specified community, at a given location if provided.
 
         :param content: The text content of the comment.
         :type content: str
         :param userId: The ID of the user profile where the comment should be posted, if applicable. Defaults to `None`.
         :type userId: Optional[str]
@@ -2701,22 +2685,22 @@
         :type blogId: Optional[str]
         :param wikiId: The ID of the wiki where the comment should be posted, if applicable. Defaults to `None`.
         :type wikiId: Optional[str]
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
 
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
 
-        `CComment`:
+        `Comment`:
 
-        The `CComment` object represents a comment, and has the following attributes:
+        The `Comment` object represents a comment, and has the following attributes:
 
         - `modifiedTime` (str or None): The time the comment was last modified, or None if not modified.
         - `ndcId` (int or None): The ndc ID of the comment, or None if not available.
         - `votedValue` (int or None): The vote value of the comment, or None if not available.
         - `parentType` (int or None): The parent type of the comment, or None if not available.
         - `commentId` (str or None): The ID of the comment, or None if not available.
         - `parentNdcId` (int or None): The ndc ID of the comment's parent, or None if not available.
@@ -2753,37 +2737,37 @@
                     break
         else:
             endpoint = f"/x{self.community_id if comId is None else comId}/s/comment"
 
         if image:
             data["mediaList"] = [[100,self.__handle_media__(media=image, media_value=True), None, None, None, None]]
 
-        return CComment(
+        return Comment(
             await self.session.handler(
             method="POST",
             url = endpoint,
             data = data
             ))
 
 
     @community
-    async def comment_on_blog(self, content: str, blogId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> CComment:
+    async def comment_on_blog(self, content: str, blogId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> Comment:
         """
         Creates a comment in the current or specified community, on a blog post with the given ID.
 
         :param content: The text content of the comment.
         :type content: str
         :param blogId: The ID of the blog where the comment should be posted.
         :type blogId: str
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
 
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
 
         **Example usage:**
 
         To post a comment with text "Hello world" on a blog post with ID "0000-0000-0000-0000":
 
@@ -2791,28 +2775,28 @@
         ... print(comment.content)
         Hello world
         """
         return self.comment(content = content, blogId = blogId, image = image, comId = comId)
 
 
     @community
-    async def comment_on_wiki(self, content: str, wikiId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> CComment:
+    async def comment_on_wiki(self, content: str, wikiId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> Comment:
         """
         Creates a comment in the current or specified community, on a wiki page with the given ID.
         
         :param content: The text content of the comment.
         :type content: str
         :param wikiId: The ID of the wiki page where the comment should be posted.
         :type wikiId: str
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
         
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
         
         **Example usage:**
         
         To post a comment with text "Hello world" on a wiki page with ID "0000-0000-0000-0000":
 
@@ -2820,28 +2804,28 @@
         ... print(comment.content)
         Hello world
         """
         return self.comment(content=content, wikiId=wikiId, image=image, comId=comId)
 
 
     @community
-    async def comment_on_profile(self, content: str, userId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> CComment:
+    async def comment_on_profile(self, content: str, userId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> Comment:
         """
         Creates a comment in the current or specified community, on a user profile with the given ID.
         
         :param content: The text content of the comment.
         :type content: str
         :param userId: The ID of the user profile where the comment should be posted.
         :type userId: str
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
         
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
         
         **Example usage:**
         
         To post a comment with text "Hello world" on a user profile with ID "0000-0000-0000-0000":
 
@@ -4799,15 +4783,15 @@
     async def start_chat(
         self,
         userIds: Union[str, List[str]],
         title: Optional[str] = None,
         message: Optional[str] = None,
         content: Optional[str] = None,
         comId: Optional[Union[str, int]] = None
-    ) -> CThread:
+    ) -> ChatThread:
         """
         Creates a new chat with the given users.
 
         :param userIds: A single user ID or a list of user IDs to invite to the chat.
         :type userIds: Union[str, List[str]]
         :param title: The title of the chat. Defaults to `None`.
         :type title: Optional[str]
@@ -4835,15 +4819,15 @@
 
         >>> response = client.community.start_chat(userIds=["0000-0000-0000-0000", "1111-1111-1111-1111"], title="New chat", message="Join my chat!", content="Hello, world!")
         ... if response.statuscode == 0:
         ...     print("Chat created successfully!")
         ... else:
         ...     print("Failed to create chat.")
         """
-        return CThread(
+        return ChatThread(
             await self.session.handler(
             method="POST",
             url=f"/x{self.community_id if comId is None else comId}/s/chat/thread",
             data={
                 "title": title,
                 "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
                 "initialMessageContent": message,
@@ -5904,7 +5888,317 @@
             data={
             "paymentContext": {
                 "transactionId": str(uuid4()) if transactionId is None else transactionId,
                 "isAutoRenew": autoRenew
             },
             "timestamp": int(time() * 1000)
             }))
+
+
+    @community
+    async def edit_chat(self,
+                  chatId: str,
+                  doNotDisturb: bool = None,
+                  pinChat: bool = None,
+                  title: str = None,
+                  icon: str = None,
+                  backgroundImage: str = None,
+                  content: str = None,
+                  announcement: str = None,
+                  coHost: list = None,
+                  keywords: list = None,
+                  pinAnnouncement: bool = None,
+                  publishToGlobal: bool = None,
+                  canTip: bool = None,
+                  viewOnly: bool = None,
+                  canInvite: bool = None,
+                  fansOnly: bool = None,
+                  comId: Union[str, int] = None):
+        """
+        Edits the chat settings.
+
+        :param chatId: The ID of the chat to edit.
+        :type chatId: str
+        :param doNotDisturb: Whether to enable or disable do not disturb mode.
+        :type doNotDisturb: bool
+        :param pinChat: Whether to pin or unpin the chat.
+        :type pinChat: bool
+        :param title: The new title for the chat.
+        :type title: str
+        :param icon: The new icon image file for the chat.
+        :type icon: str
+        :param backgroundImage: The new background image file for the chat.
+        :type backgroundImage: str
+        :param content: The new content for the chat.
+        :type content: str
+        :param announcement: The new announcement for the chat.
+        :type announcement: str
+        :param coHost: A list of user IDs to set as co-hosts.
+        :type coHost: list
+        :param keywords: A list of keywords for the chat.
+        :type keywords: list
+        :param pinAnnouncement: Whether to pin or unpin the announcement.
+        :type pinAnnouncement: bool
+        :param publishToGlobal: Whether to publish the chat to the global chat list.
+        :type publishToGlobal: bool
+        :param canTip: Whether tipping is enabled or disabled for the chat.
+        :type canTip: bool
+        :param viewOnly: Whether view-only mode is enabled or disabled for the chat.
+        :type viewOnly: bool
+        :param canInvite: Whether members can invite others to the chat.
+        :type canInvite: bool
+        :param fansOnly: Whether the chat is for fans only.
+        :type fansOnly: bool
+        :param comId: The ID of the community to edit the chat in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A list of `ApiResponse` objects containing the status codes of the API requests.
+        :rtype: list
+
+        This function sends multiple POST requests to the API to edit different aspects of the chat settings.
+
+        The list of `ApiResponse` objects contains the status codes of each request. The order of the responses corresponds to the order of the actions performed.
+
+        **Example usage:**
+
+        To enable do not disturb mode and pin the chat:
+
+        >>> responses = client.community.edit_chat(chatId="12345", doNotDisturb=True, pinChat=True)
+        ... for response in responses:
+        ...     if response.statuscode == 0:
+        ...         print("Edit successful!")
+        ...     else:
+        ...         print("Edit failed.")
+
+        To set a new title, icon, and content for the chat:
+
+        >>> responses = client.community.edit_chat(chatId="12345", title="New Chat", icon="path/to/icon.jpg", content="Welcome to the new chat!")
+        ... for response in responses:
+        ...     if response.statuscode == 0:
+        ...         print("Edit successful!")
+        ...     else:
+        ...         print("Edit failed.")
+        """
+        data = dict(timestamp = int(time() * 1000))
+
+        if title: data               .update(dict(title = title))
+        if content: data             .update(dict(content = content))
+        if icon: data                .update(dict(icon = self.upload_media(open(icon, "rb").read()), content_type = "image/jpg"))
+        if keywords: data            .update(dict(keywords = keywords))
+        if announcement: data        .update(dict(extensions = dict(announcement = announcement)))
+        if pinAnnouncement: data     .update(dict(extensions = dict(pinAnnouncement = pinAnnouncement)))
+        if fansOnly: data            .update(dict(extensions = dict(fansOnly = fansOnly)))
+        if publishToGlobal: data     .update(dict(publishToGlobal = 0))
+        if not publishToGlobal: data .update(dict(publishToGlobal = 1))
+
+        responses = []
+
+        if doNotDisturb is not None:
+            responses.append(ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/alert",
+                data = {
+                    "alertOption": 2 if doNotDisturb else 1,
+                    "timestamp": int(time() * 1000)
+                }
+            )).statuscode)
+            
+        
+        if pinChat is not None:
+            responses.append(ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/{'pin' if pinChat else 'unpin'}",
+                data = data
+            )).statuscode)
+        
+        if backgroundImage is not None:
+            responses.append(ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/background",
+                data = {
+                    "media": [100, await self.__handle_media__(backgroundImage, "image/jpg", media_value=True), None],
+                    "timestamp": int(time() * 1000)
+                }
+            )).statuscode)
+        
+        if coHost is not None:
+            responses.append(ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/co-host",
+                data = {
+                    "uidList": coHost,
+                    "timestamp": int(time() * 1000)
+                }
+            )).statuscode)
+        
+        if viewOnly is not None:
+            responses.append(ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/view-only/{'enable' if viewOnly else 'disable'}"
+            )).statuscode)
+        
+        if canInvite is not None:
+            responses.append(ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/members-can-invite/{'enable' if canInvite else 'disable'}"
+            )).statuscode)
+        
+        if canTip is not None:
+            responses.append(ApiResponse(await self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/tipping-perm-status/{'enable' if canTip else 'disable'}"
+            )).statuscode)
+        
+        responses.append(ApiResponse(await self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}",
+            data = data
+        )).statuscode)
+
+        return responses
+
+    @community
+    async def edit_profile(self, nickname: str = None, content: str = None, icon: str = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None, comId: Union[str, int] = None):
+        """
+        Edits the user profile.
+
+        :param nickname: The new nickname for the user.
+        :type nickname: str
+        :param content: The new content for the user profile.
+        :type content: str
+        :param icon: The new icon image file for the user profile.
+        :type icon: str
+        :param chatRequestPrivilege: The privilege level for chat invite requests.
+        :type chatRequestPrivilege: str
+        :param imageList: A list of image files to upload.
+        :type imageList: list
+        :param captionList: A list of captions for the uploaded images.
+        :type captionList: list
+        :param backgroundImage: The new background image file for the user profile.
+        :type backgroundImage: str
+        :param backgroundColor: The new background color for the user profile.
+        :type backgroundColor: str
+        :param titles: A list of custom titles for the user profile.
+        :type titles: list
+        :param colors: A list of colors corresponding to the custom titles.
+        :type colors: list
+        :param defaultBubbleId: The ID of the default bubble for the user profile.
+        :type defaultBubbleId: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile.
+
+        `UserProfile`:
+
+        - `nickname` (str): The nickname of the user.
+        - `content` (str): The content of the user profile.
+        - `icon` (str): The URL of the icon image.
+        - `chatRequestPrivilege` (str): The privilege level for chat invite requests.
+        - `backgroundImage` (str): The URL of the background image.
+        - `backgroundColor` (str): The background color of the user profile.
+        - `titles` (list): A list of custom titles for the user profile.
+        - `colors` (list): A list of colors corresponding to the custom titles.
+        - `defaultBubbleId` (str): The ID of the default bubble for the user profile.
+
+        **Example usage:**
+
+        To edit the user profile with a new nickname and content:
+
+        >>> profile = client.community.edit_profile(nickname="JohnDoe", content="Hello, I'm John!")
+        ... print(profile.nickname)  # "JohnDoe"
+        ... print(profile.content)  # "Hello, I'm John!"
+
+        To upload and set a new icon image:
+
+        >>> profile = client.community.edit_profile(icon="path/to/icon.jpg")
+        ... print(profile.icon)  # "https://example.com/icon.jpg"
+
+        To upload multiple images with captions:
+
+        >>> images = ["path/to/image1.jpg", "path/to/image2.jpg"]
+        ... captions = ["Caption 1", "Caption 2"]
+        ... profile = client.community.edit_profile(imageList=images, captionList=captions)
+        ... print(profile.media)  # List of uploaded image URLs with captions
+
+        To set a new background image and color:
+
+        >>> profile = client.community.edit_profile(backgroundImage="path/to/background.jpg", backgroundColor="#FFFFFF")
+        ... print(profile.backgroundImage)  # "https://example.com/background.jpg"
+        ... print(profile.backgroundColor)  # "#FFFFFF"
+
+        To set custom titles and colors:
+
+        >>> titles = ["Title 1", "Title 2"]
+        ... colors = ["#FF0000", "#00FF00"]
+        ... profile = client.community.edit_profile(titles=titles, colors=colors)
+        ... print(profile.titles)  # ["Title 1", "Title 2"]
+        ... print(profile.colors)  # ["#FF0000", "#00FF00"]
+
+        To set the default bubble:
+
+        >>> profile = client.community.edit_profile(defaultBubbleId="bubble123")
+        ... print(profile.defaultBubbleId)  # "bubble123"
+        """
+        media = []
+
+        data = dict(timestamp = int(time() * 1000))
+
+        if captionList is not None:
+            media.extend([[100, await self.__handle_media__(image, "image/jpg", True), caption] for image, caption in zip(imageList, captionList)])
+        elif imageList is not None:
+            media.extend([[100, await self.__handle_media__(image, "image/jpg", True), None] for image in imageList])
+
+        if imageList is not None or captionList is not None:
+            data.update(dict(mediaList=media))
+
+        if nickname:
+            data.update(dict(nickname = nickname))
+        if icon:
+            data.update(dict(icon = await self.__handle_media__(icon, "image/jpg", True)))
+        if content:
+            data.update(dict(content = content))
+
+        if chatRequestPrivilege:
+            data["extensions"] = {
+                "privilegeOfChatInviteRequest": chatRequestPrivilege
+            }
+
+        if backgroundImage:
+            data["extensions"] = {
+                "style": {
+                    "backgroundMediaList": [
+                        [
+                            100,
+                            await self.__handle_media__(
+                                media=backgroundImage,
+                                content_type="image/jpg",
+                                media_value=True
+                                ),
+                            None,
+                            None,
+                            None,
+                        ]
+                    ]
+                }
+            }
+
+        if backgroundColor:
+            data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+
+        if defaultBubbleId:
+            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+
+        if titles or colors:
+            data["extensions"] = {
+                "customTitles": [
+                    {"title": title, "color": color}
+                    for title, color in zip(titles, colors)
+                ]
+            }
+
+        return UserProfile(await self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id or comId}/s/user-profile/{self.userId}",
+            data = data
+        ))
```

### Comparing `pymino-1.1.8.5/pymino/ext/async_context.py` & `pymino-1.1.8.6/pymino/ext/async_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import asyncio
 import aiohttp
-from requests import get
 from diskcache import Cache
 from base64 import b64encode
 from contextlib import suppress
 from time import sleep as delay, time
 from asyncio import AbstractEventLoop
 from typing import BinaryIO, Callable, List, Union
 
-
-from .entities.general import ApiResponse
-from .entities.exceptions import InvalidImage, MustRunInContext
-from .entities.messages import (
-    CMessage, Message, MessageAuthor, PrepareMessage
-    )
-
+from .entities import *
 
 class AsyncContext:
     """
     `Context` - This handles the event context.
 
     `**Parameters**``
     - `message` - The message which triggered the event.
```

### Comparing `pymino-1.1.8.5/pymino/ext/async_event_handler.py` & `pymino-1.1.8.6/pymino/ext/async_event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 import asyncio
-from requests import get
+from time import time
 from diskcache import Cache
-from threading import Thread
-from base64 import b64encode
 from contextlib import suppress
 from colorama import Fore, Style
-from time import sleep as delay, time
+from typing import Callable, Union
 from inspect import signature as inspect_signature
-from typing import BinaryIO, Callable, List, Union
-from asyncio import AbstractEventLoop
 
-from .entities.general import ApiResponse
-from .entities.userprofile import OnlineMembers
-from .utilities.commands import Command, Commands
-from .entities.exceptions import InvalidImage, MustRunInContext
-from .entities.messages import (
-    CMessage, Message, MessageAuthor, PrepareMessage, NNotification
-    )
 
+from .entities import *
 from .async_context import AsyncContext
+from .utilities.commands import Command, Commands
 
 class AsyncEventHandler:
     """
     `EventHandler` - AKA where all the events are handled.
 
     `**Parameters**``
     - `session` - The session we are using.
@@ -637,15 +628,15 @@
 
         `**Example**``
         ```py
         from pymino.ext import *
         chatId = "0000-0000-0000-0000"
 
         @bot.on_member_set_you_host()
-        def member_set_you_host(notification: NNotification):
+        def member_set_you_host(notification: Notification):
             if notification.chatId == chatId:
                 print("You are now host")
                 bot.community.send_message(chatId=chatId, content="I am now host", comId=notification.comId)
         ```
         """
         def decorator(func: Callable) -> Callable:
             self._events["member_set_you_host"] = func
@@ -659,15 +650,15 @@
         
         `**Example**``
         ```py
         from pymino.ext import *
         chatId = "0000-0000-0000-0000"
         
         @bot.on_member_set_you_cohost()
-        def member_set_you_cohost(notification: NNotification):
+        def member_set_you_cohost(notification: Notification):
             if notification.chatId == chatId:
                 print("You are now cohost")
                 bot.community.send_message(chatId=chatId, content="I am now cohost", comId=notification.comId)
         ```
         """
         def decorator(func: Callable) -> Callable:
             self._events["member_set_you_cohost"] = func
@@ -681,15 +672,15 @@
         
         `**Example**``
         ```py
         from pymino.ext import *
         chatId = "0000-0000-0000-0000"
         
         @bot.on_member_remove_your_cohost()
-        def member_remove_your_cohost(notification: NNotification):
+        def member_remove_your_cohost(notification: Notification):
             if notification.chatId == chatId:
                 print("You are no longer cohost")
                 bot.community.send_message(chatId=chatId, content="I am no longer cohost", comId=notification.comId)
         ```
         """
         def decorator(func: Callable) -> Callable:
             self._events["member_remove_your_cohost"] = func
@@ -701,15 +692,15 @@
         func = self._events[event]
         return await func(* await self._set_parameters(context, func, data))
 
 
     async def _handle_event(
         self,
         event: str,
-        data: Union[Message, OnlineMembers, NNotification, AsyncContext]
+        data: Union[Message, OnlineMembers, Notification, AsyncContext]
         ) -> Union[AsyncContext, None]:
         """
         `_handle_event` is a function that handles events.
         """
         with suppress(KeyError):
             context = self.context(data, self.loop, self.request)
```

### Comparing `pymino-1.1.8.5/pymino/ext/async_socket.py` & `pymino-1.1.8.6/pymino/ext/async_socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,19 @@
 from typing import Optional
 from asyncio.queues import Queue
 from colorama import Fore, Style
 from urllib.parse import urlencode
 from ujson import loads, JSONDecodeError
 from contextlib import asynccontextmanager
 
-
+from .entities import *
 from .handle_queue import QueueHandler
 from .async_event_handler import AsyncEventHandler
-
 from .dispatcher import AsyncMessageDispatcher
-from .entities.userprofile import OnlineMembers
-from .entities.wsevents import EventTypes, NotifTypes
-
-from .entities.messages import Channel, Message, NNotification
 from .utilities.generate import device_id, generate_signature
-from .entities.handlers import orjson_exists, alive_loop
 
 if orjson_exists():
     from orjson import loads as orjson_loads
 
 
 @asynccontextmanager
 async def create_client_session():
@@ -151,16 +145,16 @@
 
         key = self.event_types.get(f"{_message.type}:{_message.mediaType}")
         if key is not None:
             self.loop.create_task(self._handle_event(key, _message))
 
 
     async def _handle_notification(self, message: dict) -> None:
-        notification: NNotification = NNotification(message)
-        key = self.notif_types.get(notification.notifType)
+        notification: Notification = Notification(message)
+        key = self.notif_types.get(notification.notification_type)
         if key != None:
             self.loop.create_task(self._handle_event(key, notification))
 
 
     async def _handle_agora_channel(self, message: dict) -> None:
         self.channel: Channel = Channel(message)
```

### Comparing `pymino-1.1.8.5/pymino/ext/community.py` & `pymino-1.1.8.6/pymino/ext/community.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,15 @@
 from random import randint
 from diskcache import Cache
 from base64 import b64encode
 from time import time, timezone
 from typing import BinaryIO, Callable, List, Optional, Union, TypeVar, Any
 
 
-from .entities.enums import *
-from .entities.threads import CThread, CThreadList
-from .entities.userprofile import UserProfile, UserProfileList
-
-from .entities.messages import (
-    CMessage, CMessages, PrepareMessage
-    )
-from .entities.exceptions import (
-    InvalidImage, MissingCommunityId,
-    MissingTimers, NoDataProvided, NotLoggedIn
-    )
-from .entities.general import *
+from .entities import *
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 class Community:
     """
     The `Community` class handles community related actions.
 
@@ -623,15 +612,16 @@
         **Example usage:**
 
         >>> api_response = client.community.request_join(message="Please accept my membership request.")
         >>> if api_response.statuscode == 0:
         ...     print("Membership request sent successfully!")
         """
         return ApiResponse(self.session.handler(
-            method = "POST", url = f"/x{self.community_id if comId is None else comId}/s/community/membership-request", 
+            method = "POST",
+            url = f"/x{self.community_id if comId is None else comId}/s/community/membership-request", 
             data={"message": message, "timestamp": int(time() * 1000)}
             ))
 
 
     @community
     def flag_community(self, reason: str, flagType: FlagTypes = FlagTypes.OFFTOPIC, comId: Union[str, int] = None) -> ApiResponse:
         """
@@ -1081,19 +1071,21 @@
         >>> user_profiles = client.community.fetch_users(userType=UserTypes.CURATORS)
         >>> print(user_profiles[0].nickname) # Prints the nickname of the first user in the list.
         'John Doe'
         """
         if "type" in kwargs: #TODO: Get rid of this in the near future.
             userType = kwargs["type"]
             print("WARNING: The 'type' parameter is deprecated. Please use 'userType' instead.")
+
         return UserProfileList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/user-profile?type={userType.value if isinstance(userType, UserTypes) else userType}&start={start}&size={size}"
             ))
 
+
     @community
     def fetch_online_users(self, start: Optional[int] = 0, size: Optional[int] = 25, comId: Union[str, int] = None) -> UserProfileList:
         """
         Fetches a list of online users in the current or specified community.
 
         :param start: The starting point to fetch users from. Defaults to `0`.
         :type start: Optional[int]
@@ -1154,14 +1146,15 @@
         'John Doe'
         """
         return UserProfileList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/live-layer?topic=ndtopic:x{self.community_id if comId is None else comId}:online-members&start={start}&size={size}"
             ))
 
+
     @community
     def fetch_followers(self, userId: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
         """
         Fetches a list of followers for a specified user in the current or specified community.
 
         :param userId: The ID of the user to fetch the followers for.
         :type userId: str
@@ -1226,14 +1219,15 @@
         ['0000-000000-000000-0000', '0000-000000-000000-0001', '0000-000000-000000-0002']
         """
         return UserProfileList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/user-profile/{userId}/member?start={start}&size={size}"
             ))
 
+
     @community
     def fetch_following(self, userId: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> UserProfileList:
         """
         Fetches a list of users that the specified user is following in the current or specified community.
 
         :param userId: The ID of the user to fetch the following users for.
         :type userId: str
@@ -1298,37 +1292,38 @@
         ['0000-000000-000000-0000', '0000-000000-000000-0001', '0000-000000-000000-0002']
         """
         return UserProfileList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/user-profile/{userId}/joined?start={start}&size={size}"
             ))
 
+
     @community
-    def fetch_chat(self, chatId: str, comId: Union[str, int] = None) -> CThread:
+    def fetch_chat(self, chatId: str, comId: Union[str, int] = None) -> ChatThread:
         """
         Fetches the chat thread with the specified ID in the current or specified community.
 
         :param chatId: The ID of the chat thread to fetch.
         :type chatId: str
         :param comId: The ID of the community to fetch the chat thread from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThread` object containing information about the chat thread.
-        :rtype: CThread
+        :return: A `ChatThread` object containing information about the chat thread.
+        :rtype: ChatThread
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch the chat thread with the specified ID.
 
-        `CThread`:
+        `ChatThread`:
 
         - `data`: The raw data of the chat thread.
         - `userAddedTopicList`: A list of topics added by the user.
         - `uid`: The user ID of the thread creator.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: The maximum number of members allowed in the chat thread.
         - `membersSummary`: A `MemberSummary` object containing information about the chat thread's members.
         - `threadId`: The ID of the chat thread.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the chat thread.
         - `membersCount`: The number of members currently in the chat thread.
         - `strategyInfo`: The strategy information for the chat thread.
@@ -1348,15 +1343,15 @@
 
         **Example usage:**
 
         >>> chat_thread = client.community.fetch_chat("0000-000000-000000-0000")
         >>> print(chat_thread.title) # Prints the title of the chat thread.
         'My Chat Thread'
         """
-        return CThread(self.session.handler(
+        return ChatThread(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}"
             ))
 
     
     @community
     def fetch_chat_mods(self, chatId: str, comId: Union[str, int] = None, moderators: Optional[str] = "all") -> List[str]:
@@ -1372,20 +1367,20 @@
             - "co-hosts": Returns only the co-hosts of the chat.
             - "host": Returns only the host of the chat.
         :type moderators: Optional[str]
         :raises NotLoggedIn: If the user is not logged in.
         :return: A list of moderator user IDs.
         :rtype: List[str]
         """
-        response: CThread = self.fetch_chat(chatId=chatId, comId=comId)
+        response: ChatThread = self.fetch_chat(chatId=chatId, comId=comId)
 
         return {
-            "all": list(response.extensions.coHost) + [response.hostUserId],
-            "co-hosts": list(response.extensions.coHost),
-            "host": [response.hostUserId]
+            "all": list(response.extensions.coHosts) + [response.host_user_id],
+            "co-hosts": list(response.extensions.coHosts),
+            "host": [response.host_user_id]
             }.get(moderators, "all")
 
 
     @community
     def fetch_chat_moderators(self, chatId: str, comId: Union[str, int] = None) -> List[str]:
         """
         Fetches a list of all moderators for a specified chat thread in the current or specified community.
@@ -1427,40 +1422,40 @@
         :return: The user ID of the chat host.
         :rtype: str
         """
         return self.fetch_chat_mods(chatId=chatId, comId=comId, moderators="host")[0]
 
 
     @community
-    def fetch_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CThreadList:
+    def fetch_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> ChatThreadList:
         """
         Fetches a list of chat threads in the current or specified community that the user has joined.
 
         :param start: The starting point to fetch chat threads from. Defaults to `0`.
         :type start: int
         :param size: The amount of chat threads to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the chat threads from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThreadList` object containing information about the chat threads.
-        :rtype: CThreadList
+        :return: A `ChatThreadList` object containing information about the chat threads.
+        :rtype: ChatThreadList
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch a list of chat threads that the user has joined.
 
-        `CThreadList`:
+        `ChatThreadList`:
 
         - `data`: The raw data of the chat thread list.
         - `extensions`: The extensions of the chat threads in the list.
         - `membersSummary`: The member summary of the chat threads in the list.
         - `userAddedTopicList`: A list of topics added by the user in the chat threads in the list.
         - `uid`: A list of user IDs of the thread creators in the chat threads in the list.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: A list of maximum member counts allowed in the chat threads in the list.
         - `threadId`: A list of thread IDs of the chat threads in the list.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the chat threads in the list.
         - `membersCount`: A list of the number of members in the chat threads in the list.
         - `strategyInfo`: The strategy information for the chat threads in the list.
         - `isPinned`: A list of whether the chat threads in the list are pinned.
@@ -1485,47 +1480,47 @@
         ['My Chat Thread', 'My Other Chat Thread']
         METHOD 2:
         >>> for chat_thread in chat_threads:
         ...     print(chat_thread.title)
         'My Chat Thread'
         'My Other Chat Thread'
         """
-        return CThreadList(self.session.handler(
+        return ChatThreadList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread?type=joined-me&start={start}&size={size}"
             ))
 
 
     @community
-    def fetch_live_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CThreadList:
+    def fetch_live_chats(self, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> ChatThreadList:
         """
         Fetches a list of live chat threads in the current or specified community that are publicly visible.
 
         :param start: The starting point to fetch chat threads from. Defaults to `0`.
         :type start: int
         :param size: The amount of chat threads to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the chat threads from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThreadList` object containing information about the live chat threads.
-        :rtype: CThreadList
+        :return: A `ChatThreadList` object containing information about the live chat threads.
+        :rtype: ChatThreadList
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch a list of publicly visible live chat threads.
 
-        `CThreadList`:
+        `ChatThreadList`:
 
         - `data`: The raw data of the live chat thread list.
         - `extensions`: The extensions of the live chat threads in the list.
         - `membersSummary`: The member summary of the live chat threads in the list.
         - `userAddedTopicList`: A list of topics added by the user in the live chat threads in the list.
         - `uid`: A list of user IDs of the thread creators in the live chat threads in the list.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: A list of maximum member counts allowed in the live chat threads in the list.
         - `threadId`: A list of thread IDs of the live chat threads in the list.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the live chat threads in the list.
         - `membersCount`: A list of the number of members in the live chat threads in the list.
         - `strategyInfo`: The strategy information for the live chat threads in the list.
         - `isPinned`: A list of whether the live chat threads in the list are pinned.
@@ -1550,62 +1545,62 @@
         ['My Live Chat Thread', 'My Other Live Chat Thread']
         METHOD 2:
         >>> for title in live_chat_titles:
         ...     print(title) # Prints the title of each live chat thread.
         'My Live Chat Thread'
         'My Other Live Chat Thread'
         """
-        return CThreadList(self.session.handler(
+        return ChatThreadList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/live-layer/public-live-chats?start={start}&size={size}"
             ))
 
 
     @community
     def fetch_public_chats(
         self,
         chatType: ChatTypes = ChatTypes.RECOMMENDED,
         start: int = 0,
         size: int = 25,
         comId: Union[str, int] = None,
         **kwargs
-        ) -> CThreadList:
+        ) -> ChatThreadList:
         """
         Fetches a list of public chat threads in the current or specified community.
 
         :param chatType: The type of public chat threads to fetch. Defaults to `ChatTypes.RECOMMENDED`.
         :type chatType: ChatTypes
         :param start: The starting point to fetch chat threads from. Defaults to `0`.
         :type start: int
         :param size: The amount of chat threads to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the chat threads from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :raises NotLoggedIn: If the user is not logged in.
-        :return: A `CThreadList` object containing information about the public chat threads.
-        :rtype: CThreadList
+        :return: A `ChatThreadList` object containing information about the public chat threads.
+        :rtype: ChatThreadList
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch a list of public chat threads of the specified type.
 
         `ChatTypes`:
 
         - `RECOMMENDED`: Fetches a list of recommended public chat threads.
         - `POPULAR`: Fetches a list of popular public chat threads.
         - `LATEST`: Fetches a list of newest public chat threads.
 
-        `CThreadList`:
+        `ChatThreadList`:
 
         - `data`: The raw data of the public chat thread list.
         - `extensions`: The extensions of the public chat threads in the list.
         - `membersSummary`: The member summary of the public chat threads in the list.
         - `userAddedTopicList`: A list of topics added by the user in the public chat threads in the list.
         - `uid`: A list of user IDs of the thread creators in the public chat threads in the list.
-        - `hostUserId`: An alias for `uid`.
+        - `host_user_id`: An alias for `uid`.
         - `membersQuota`: A list of maximum member counts allowed in the public chat threads in the list.
         - `threadId`: A list of thread IDs of the public chat threads in the list.
         - `chatId`: An alias for `threadId`.
         - `keywords`: A list of keywords associated with the public chat threads in the list.
         - `membersCount`: A list of the number of members in the public chat threads in the list.
         - `strategyInfo`: The strategy information for the public chat threads in the list.
         - `isPinned`: A list of whether the public chat threads in the list are pinned.
@@ -1634,15 +1629,15 @@
         'My Public Chat Thread'
         'My Other Public Chat Thread'
         """
         if "type" in kwargs: #TODO Remove this in the near future.
             chatType = kwargs["type"]
             print("WARNING: The `type` parameter is deprecated. Please use `chatType` instead.")
 
-        return CThreadList(self.session.handler(
+        return ChatThreadList(self.session.handler(
             method = "GET",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread?type=public-all&filterType={chatType.value if isinstance(chatType, ChatTypes) else chatType}&start={start}&size={size}"
             ))
 
 
     @community
     def fetch_chat_members(self, chatId: str, start: int = 0, size: int = 25, comId: Union[str, int] = None) -> CChatMembers:
@@ -2013,15 +2008,15 @@
     def fetch_comments(
         self,
         userId: Optional[str] = None,
         blogId: Optional[str] = None,
         wikiId: Optional[str] = None,
         start: int = 0,
         size: int = 25,
-        comId: Union[str, int] = None) -> CCommentList:
+        comId: Union[str, int] = None) -> CommentList:
         """
         Fetches the comments for the specified user, blog, or wiki.
 
         :param userId: The ID of the user whose comments to fetch. Defaults to `None`.
         :type userId: Optional[str]
         :param blogId: The ID of the blog whose comments to fetch. Defaults to `None`.
         :type blogId: Optional[str]
@@ -2029,23 +2024,23 @@
         :type wikiId: Optional[str]
         :param start: The starting index of the comments to fetch. Defaults to `0`.
         :type start: int
         :param size: The number of comments to fetch. Defaults to `25`.
         :type size: int
         :param comId: The ID of the community to fetch the comments from. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CCommentList` object containing the comments for the specified user, blog, or wiki.
-        :rtype: CCommentList
+        :return: A `CommentList` object containing the comments for the specified user, blog, or wiki.
+        :rtype: CommentList
         :raises NoDataProvided: If none of `userId`, `blogId`, or `wikiId` is provided.
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
         The function sends a GET request to the API to fetch the comments for the specified user, blog, or wiki.
 
-        `CCommentList`:
+        `CommentList`:
 
         - `modifiedTime`: A list of the last modified time of each comment.
         - `ndcId`: A list of the NDC IDs of each comment.
         - `votedValue`: A list of the voted value of each comment.
         - `parentType`: A list of the parent types of each comment.
         - `commentId`: A list of the IDs of each comment.
         - `parentNdcId`: A list of the parent NDC IDs of each comment.
@@ -2075,15 +2070,15 @@
         if any([userId, blogId, wikiId]):
             for key, value in {
                 "userId": "user-profile/{}",
                 "blogId": "blog/{}",
                 "wikiId": "item/{}"
             }.items():
                 if locals()[key]:
-                    return CCommentList(
+                    return CommentList(
                         self.session.handler(
                             method="GET",
                             url=f"/x{self.community_id if comId is None else comId}/s/{value.format(locals()[key])}/comment?sort=newest&start={start}&size={size}",
                         )
                     )
 
         raise NoDataProvided
@@ -2635,15 +2630,15 @@
         self,
         content: str,
         userId: Optional[str] = None,
         blogId: Optional[str] = None,
         wikiId: Optional[str] = None,
         image: Optional[str] = None,
         comId: Union[str, int] = None
-        ) -> CComment:
+        ) -> Comment:
         """
         Creates a comment in the current or specified community, at a given location if provided.
 
         :param content: The text content of the comment.
         :type content: str
         :param userId: The ID of the user profile where the comment should be posted, if applicable. Defaults to `None`.
         :type userId: Optional[str]
@@ -2651,22 +2646,22 @@
         :type blogId: Optional[str]
         :param wikiId: The ID of the wiki where the comment should be posted, if applicable. Defaults to `None`.
         :type wikiId: Optional[str]
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
 
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
 
-        `CComment`:
+        `Comment`:
 
-        The `CComment` object represents a comment, and has the following attributes:
+        The `Comment` object represents a comment, and has the following attributes:
 
         - `modifiedTime` (str or None): The time the comment was last modified, or None if not modified.
         - `ndcId` (int or None): The ndc ID of the comment, or None if not available.
         - `votedValue` (int or None): The vote value of the comment, or None if not available.
         - `parentType` (int or None): The parent type of the comment, or None if not available.
         - `commentId` (str or None): The ID of the comment, or None if not available.
         - `parentNdcId` (int or None): The ndc ID of the comment's parent, or None if not available.
@@ -2703,36 +2698,36 @@
                     break
         else:
             endpoint = f"/x{self.community_id if comId is None else comId}/s/comment"
 
         if image:
             data["mediaList"] = [[100,self.__handle_media__(media=image, media_value=True), None, None, None, None]]
 
-        return CComment(self.session.handler(
+        return Comment(self.session.handler(
             method = "POST",
             url = endpoint,
             data = data
             ))
 
 
     @community
-    def comment_on_blog(self, content: str, blogId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> CComment:
+    def comment_on_blog(self, content: str, blogId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> Comment:
         """
         Creates a comment in the current or specified community, on a blog post with the given ID.
 
         :param content: The text content of the comment.
         :type content: str
         :param blogId: The ID of the blog where the comment should be posted.
         :type blogId: str
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
 
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
 
         **Example usage:**
 
         To post a comment with text "Hello world" on a blog post with ID "0000-0000-0000-0000":
 
@@ -2740,28 +2735,28 @@
         ... print(comment.content)
         Hello world
         """
         return self.comment(content = content, blogId = blogId, image = image, comId = comId)
 
 
     @community
-    def comment_on_wiki(self, content: str, wikiId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> CComment:
+    def comment_on_wiki(self, content: str, wikiId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> Comment:
         """
         Creates a comment in the current or specified community, on a wiki page with the given ID.
         
         :param content: The text content of the comment.
         :type content: str
         :param wikiId: The ID of the wiki page where the comment should be posted.
         :type wikiId: str
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
         
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
         
         **Example usage:**
         
         To post a comment with text "Hello world" on a wiki page with ID "0000-0000-0000-0000":
 
@@ -2769,28 +2764,28 @@
         ... print(comment.content)
         Hello world
         """
         return self.comment(content=content, wikiId=wikiId, image=image, comId=comId)
 
 
     @community
-    def comment_on_profile(self, content: str, userId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> CComment:
+    def comment_on_profile(self, content: str, userId: str, image: Optional[str] = None, comId: Union[str, int] = None) -> Comment:
         """
         Creates a comment in the current or specified community, on a user profile with the given ID.
         
         :param content: The text content of the comment.
         :type content: str
         :param userId: The ID of the user profile where the comment should be posted.
         :type userId: str
         :param image: The image to be attached to the comment, if any. Defaults to `None`.
         :type image: Optional[str]
         :param comId: The ID of the community where the comment should be posted. If not provided, the current community ID is used.
         :type comId: Union[str, int]
-        :return: A `CComment` object containing information about the newly created comment.
-        :rtype: CComment
+        :return: A `Comment` object containing information about the newly created comment.
+        :rtype: Comment
         
         This function sends a POST request to the API to create a comment in the specified location or in the current community.
         
         **Example usage:**
         
         To post a comment with text "Hello world" on a user profile with ID "0000-0000-0000-0000":
 
@@ -4698,15 +4693,15 @@
     def start_chat(
         self,
         userIds: Union[str, List[str]],
         title: Optional[str] = None,
         message: Optional[str] = None,
         content: Optional[str] = None,
         comId: Optional[Union[str, int]] = None
-    ) -> CThread:
+    ) -> ChatThread:
         """
         Creates a new chat with the given users.
 
         :param userIds: A single user ID or a list of user IDs to invite to the chat.
         :type userIds: Union[str, List[str]]
         :param title: The title of the chat. Defaults to `None`.
         :type title: Optional[str]
@@ -4734,15 +4729,15 @@
 
         >>> response = client.community.start_chat(userIds=["0000-0000-0000-0000", "1111-1111-1111-1111"], title="New chat", message="Join my chat!", content="Hello, world!")
         ... if response.statuscode == 0:
         ...     print("Chat created successfully!")
         ... else:
         ...     print("Failed to create chat.")
         """
-        return CThread(self.session.handler(
+        return ChatThread(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread",
             data = {
             "title": title,
             "inviteeUids": userIds if isinstance(userIds, list) else [userIds],
             "initialMessageContent": message,
             "content": content,
@@ -5783,7 +5778,317 @@
             data = {
             "paymentContext": {
                 "transactionId": str(uuid4()) if transactionId is None else transactionId,
                 "isAutoRenew": autoRenew
             },
             "timestamp": int(time() * 1000)
             }))
+
+
+    @community
+    def edit_chat(self,
+                  chatId: str,
+                  doNotDisturb: bool = None,
+                  pinChat: bool = None,
+                  title: str = None,
+                  icon: str = None,
+                  backgroundImage: str = None,
+                  content: str = None,
+                  announcement: str = None,
+                  coHost: list = None,
+                  keywords: list = None,
+                  pinAnnouncement: bool = None,
+                  publishToGlobal: bool = None,
+                  canTip: bool = None,
+                  viewOnly: bool = None,
+                  canInvite: bool = None,
+                  fansOnly: bool = None,
+                  comId: Union[str, int] = None):
+        """
+        Edits the chat settings.
+
+        :param chatId: The ID of the chat to edit.
+        :type chatId: str
+        :param doNotDisturb: Whether to enable or disable do not disturb mode.
+        :type doNotDisturb: bool
+        :param pinChat: Whether to pin or unpin the chat.
+        :type pinChat: bool
+        :param title: The new title for the chat.
+        :type title: str
+        :param icon: The new icon image file for the chat.
+        :type icon: str
+        :param backgroundImage: The new background image file for the chat.
+        :type backgroundImage: str
+        :param content: The new content for the chat.
+        :type content: str
+        :param announcement: The new announcement for the chat.
+        :type announcement: str
+        :param coHost: A list of user IDs to set as co-hosts.
+        :type coHost: list
+        :param keywords: A list of keywords for the chat.
+        :type keywords: list
+        :param pinAnnouncement: Whether to pin or unpin the announcement.
+        :type pinAnnouncement: bool
+        :param publishToGlobal: Whether to publish the chat to the global chat list.
+        :type publishToGlobal: bool
+        :param canTip: Whether tipping is enabled or disabled for the chat.
+        :type canTip: bool
+        :param viewOnly: Whether view-only mode is enabled or disabled for the chat.
+        :type viewOnly: bool
+        :param canInvite: Whether members can invite others to the chat.
+        :type canInvite: bool
+        :param fansOnly: Whether the chat is for fans only.
+        :type fansOnly: bool
+        :param comId: The ID of the community to edit the chat in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A list of `ApiResponse` objects containing the status codes of the API requests.
+        :rtype: list
+
+        This function sends multiple POST requests to the API to edit different aspects of the chat settings.
+
+        The list of `ApiResponse` objects contains the status codes of each request. The order of the responses corresponds to the order of the actions performed.
+
+        **Example usage:**
+
+        To enable do not disturb mode and pin the chat:
+
+        >>> responses = client.community.edit_chat(chatId="12345", doNotDisturb=True, pinChat=True)
+        ... for response in responses:
+        ...     if response.statuscode == 0:
+        ...         print("Edit successful!")
+        ...     else:
+        ...         print("Edit failed.")
+
+        To set a new title, icon, and content for the chat:
+
+        >>> responses = client.community.edit_chat(chatId="12345", title="New Chat", icon="path/to/icon.jpg", content="Welcome to the new chat!")
+        ... for response in responses:
+        ...     if response.statuscode == 0:
+        ...         print("Edit successful!")
+        ...     else:
+        ...         print("Edit failed.")
+        """
+        data = dict(timestamp = int(time() * 1000))
+
+        if title: data               .update(dict(title = title))
+        if content: data             .update(dict(content = content))
+        if icon: data                .update(dict(icon = self.upload_media(open(icon, "rb").read()), content_type = "image/jpg"))
+        if keywords: data            .update(dict(keywords = keywords))
+        if announcement: data        .update(dict(extensions = dict(announcement = announcement)))
+        if pinAnnouncement: data     .update(dict(extensions = dict(pinAnnouncement = pinAnnouncement)))
+        if fansOnly: data            .update(dict(extensions = dict(fansOnly = fansOnly)))
+        if publishToGlobal: data     .update(dict(publishToGlobal = 0))
+        if not publishToGlobal: data .update(dict(publishToGlobal = 1))
+
+        responses = []
+
+        if doNotDisturb is not None:
+            responses.append(ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/alert",
+                data = {
+                    "alertOption": 2 if doNotDisturb else 1,
+                    "timestamp": int(time() * 1000)
+                }
+            )).statuscode)
+            
+        
+        if pinChat is not None:
+            responses.append(ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/{'pin' if pinChat else 'unpin'}",
+                data = data
+            )).statuscode)
+        
+        if backgroundImage is not None:
+            responses.append(ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}/background",
+                data = {
+                    "media": [100, self.__handle_media__(backgroundImage, "image/jpg", True), None],
+                    "timestamp": int(time() * 1000)
+                }
+            )).statuscode)
+        
+        if coHost is not None:
+            responses.append(ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/co-host",
+                data = {
+                    "uidList": coHost,
+                    "timestamp": int(time() * 1000)
+                }
+            )).statuscode)
+        
+        if viewOnly is not None:
+            responses.append(ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/view-only/{'enable' if viewOnly else 'disable'}"
+            )).statuscode)
+        
+        if canInvite is not None:
+            responses.append(ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/members-can-invite/{'enable' if canInvite else 'disable'}"
+            )).statuscode)
+        
+        if canTip is not None:
+            responses.append(ApiResponse(self.session.handler(
+                method = "POST",
+                url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}/tipping-perm-status/{'enable' if canTip else 'disable'}"
+            )).statuscode)
+        
+        responses.append(ApiResponse(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id or comId}/s/chat/thread/{chatId}",
+            data = data
+        )).statuscode)
+
+        return responses
+
+    @community
+    def edit_profile(self, nickname: str = None, content: str = None, icon: str = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None, comId: Union[str, int] = None):
+        """
+        Edits the user profile.
+
+        :param nickname: The new nickname for the user.
+        :type nickname: str
+        :param content: The new content for the user profile.
+        :type content: str
+        :param icon: The new icon image file for the user profile.
+        :type icon: str
+        :param chatRequestPrivilege: The privilege level for chat invite requests.
+        :type chatRequestPrivilege: str
+        :param imageList: A list of image files to upload.
+        :type imageList: list
+        :param captionList: A list of captions for the uploaded images.
+        :type captionList: list
+        :param backgroundImage: The new background image file for the user profile.
+        :type backgroundImage: str
+        :param backgroundColor: The new background color for the user profile.
+        :type backgroundColor: str
+        :param titles: A list of custom titles for the user profile.
+        :type titles: list
+        :param colors: A list of colors corresponding to the custom titles.
+        :type colors: list
+        :param defaultBubbleId: The ID of the default bubble for the user profile.
+        :type defaultBubbleId: str
+        :param comId: The ID of the community to edit the user profile in. If not provided, the current community ID is used.
+        :type comId: Union[str, int]
+        :return: A `UserProfile` object containing the updated user profile information.
+        :rtype: UserProfile
+
+        This function sends a POST request to the API to edit the user profile.
+
+        `UserProfile`:
+
+        - `nickname` (str): The nickname of the user.
+        - `content` (str): The content of the user profile.
+        - `icon` (str): The URL of the icon image.
+        - `chatRequestPrivilege` (str): The privilege level for chat invite requests.
+        - `backgroundImage` (str): The URL of the background image.
+        - `backgroundColor` (str): The background color of the user profile.
+        - `titles` (list): A list of custom titles for the user profile.
+        - `colors` (list): A list of colors corresponding to the custom titles.
+        - `defaultBubbleId` (str): The ID of the default bubble for the user profile.
+
+        **Example usage:**
+
+        To edit the user profile with a new nickname and content:
+
+        >>> profile = client.community.edit_profile(nickname="JohnDoe", content="Hello, I'm John!")
+        ... print(profile.nickname)  # "JohnDoe"
+        ... print(profile.content)  # "Hello, I'm John!"
+
+        To upload and set a new icon image:
+
+        >>> profile = client.community.edit_profile(icon="path/to/icon.jpg")
+        ... print(profile.icon)  # "https://example.com/icon.jpg"
+
+        To upload multiple images with captions:
+
+        >>> images = ["path/to/image1.jpg", "path/to/image2.jpg"]
+        ... captions = ["Caption 1", "Caption 2"]
+        ... profile = client.community.edit_profile(imageList=images, captionList=captions)
+        ... print(profile.media)  # List of uploaded image URLs with captions
+
+        To set a new background image and color:
+
+        >>> profile = client.community.edit_profile(backgroundImage="path/to/background.jpg", backgroundColor="#FFFFFF")
+        ... print(profile.backgroundImage)  # "https://example.com/background.jpg"
+        ... print(profile.backgroundColor)  # "#FFFFFF"
+
+        To set custom titles and colors:
+
+        >>> titles = ["Title 1", "Title 2"]
+        ... colors = ["#FF0000", "#00FF00"]
+        ... profile = client.community.edit_profile(titles=titles, colors=colors)
+        ... print(profile.titles)  # ["Title 1", "Title 2"]
+        ... print(profile.colors)  # ["#FF0000", "#00FF00"]
+
+        To set the default bubble:
+
+        >>> profile = client.community.edit_profile(defaultBubbleId="bubble123")
+        ... print(profile.defaultBubbleId)  # "bubble123"
+        """
+        media = []
+
+        data = dict(timestamp = int(time() * 1000))
+
+        if captionList is not None:
+            media.extend([[100, self.__handle_media__(image, "image/jpg", True), caption] for image, caption in zip(imageList, captionList)])
+        elif imageList is not None:
+            media.extend([[100, self.__handle_media__(image, "image/jpg", True), None] for image in imageList])
+
+        if imageList is not None or captionList is not None:
+            data.update(dict(mediaList=media))
+
+        if nickname:
+            data.update(dict(nickname = nickname))
+        if icon:
+            data.update(dict(icon = self.__handle_media__(icon, "image/jpg", True)))
+        if content:
+            data.update(dict(content = content))
+
+        if chatRequestPrivilege:
+            data["extensions"] = {
+                "privilegeOfChatInviteRequest": chatRequestPrivilege
+            }
+
+        if backgroundImage:
+            data["extensions"] = {
+                "style": {
+                    "backgroundMediaList": [
+                        [
+                            100,
+                            self.__handle_media__(
+                                media=backgroundImage,
+                                content_type="image/jpg",
+                                media_value=True
+                                ),
+                            None,
+                            None,
+                            None,
+                        ]
+                    ]
+                }
+            }
+
+        if backgroundColor:
+            data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+
+        if defaultBubbleId:
+            data["extensions"] = {"defaultBubbleId": defaultBubbleId}
+
+        if titles or colors:
+            data["extensions"] = {
+                "customTitles": [
+                    {"title": title, "color": color}
+                    for title, color in zip(titles, colors)
+                ]
+            }
+
+        return UserProfile(self.session.handler(
+            method = "POST",
+            url = f"/x{self.community_id or comId}/s/user-profile/{self.userId}",
+            data = data
+        ))
```

### Comparing `pymino-1.1.8.5/pymino/ext/context.py` & `pymino-1.1.8.6/pymino/ext/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 from base64 import b64encode
 from contextlib import suppress
 from colorama import Fore, Style
 from time import sleep as delay, time
 from inspect import signature as inspect_signature
 from typing import BinaryIO, Callable, List, Union
 
-from .entities.general import ApiResponse
-from .entities.userprofile import OnlineMembers
+from .entities import *
 from .utilities.commands import Command, Commands
-from .entities.exceptions import InvalidImage, MustRunInContext
-from .entities.messages import (
-    CMessage, Message, MessageAuthor, PrepareMessage, NNotification
-    )
 
 class Context():
     """
     `Context` - This handles the event context.
 
     `**Parameters**``
     - `message` - The message which triggered the event.
@@ -537,14 +532,15 @@
         self.context:           Context = Context
 
 
     def start_task(self, func):
         """`start_task` - This starts a task."""
         Thread(target=func).start()
 
+
     def _handle_task(self, func, interval):
         """
         `_handle_task` - This handles the task.
         
         `**Parameters**``
         - `func` - The function.
         - `interval` - The interval in seconds.
@@ -552,15 +548,16 @@
         `**Returns**`` - None
         """
         while True:
             if len(inspect_signature(func).parameters) == 0:
                 func()
             else: func(self.community)
             delay(interval)
-            
+
+
     def task(self, interval: int = 10):
         """
         `task` - This creates a task.
 
         `**Parameters**``
         - `interval` - The interval in seconds.
 
@@ -579,19 +576,49 @@
         """
 
         def decorator(func):
             def wrapper():
                 self._handle_task(func, interval)
             self.start_task(wrapper)
         return decorator
-                
-    def emit(self, name: str, *args):
+
+
+    def _set_parameters(self, context: Context, func: Callable, message: str = None) -> list:
+        try:
+            message = message if isinstance(message, str) else context.message.content
+        except AttributeError:
+            message = None
+
+        try:
+            username = context.author.username
+        except AttributeError:
+            username = None
+
+        try:
+            userId = context.author.userId
+        except AttributeError:
+            userId = None
+
+        potential_parameters = {
+            "ctx": context,
+            "message": message,
+            "username": username,
+            "userId": userId
+        }
+
+        return [
+            potential_parameters.get(parameter)
+            for parameter in inspect_signature(func).parameters
+        ]
+
+
+    def emit(self, name: str, *args) -> None:
         """`emit` is a function that emits an event."""
-        if name in self._events:
-            self._events[name](*args) 
+        self._events[name](*args) if name in self._events else None
+
 
     def command(
         self,
         name: str=None,
         description: str=None,
         usage: str=None,
         aliases: list=[],
@@ -673,532 +700,455 @@
                     description=description,
                     usage=usage,
                     aliases=aliases,
                     cooldown=cooldown
                 ))
             return func
         return decorator
-    
+
+
     def _is_deprecated(self, parameter: str, new_parameter: str):
         print(f"{Style.BRIGHT}{Fore.RED}WARNING:{Style.RESET_ALL} '{parameter}' is deprecated. Please use '{new_parameter}' instead.")
 
+
     def command_exists(self, command_name: str) -> bool:
-        """
-        `command_exists` - This checks if a command exists.
-        
-        `**Parameters**``
-        - `command_name` - The name of the command.
-        
-        `**Returns**`` - bool
-        """
         return any([
             command_name in self._commands.__command_names__(),
             command_name in self._commands.__command_aliases__()
             ])
 
+
     def fetch_command(self, command_name: str) -> Command:
-        """
-        `fetch_command` - This fetches a command.
-        
-        `**Parameters**``
-        - `command_name` - The name of the command.
-        
-        `**Returns**`` - Command
-        """
         return self._commands.fetch_command(command_name)
 
     def _handle_command(self, data: Message, context: Context):
-        """`_handle_command` is a function that handles commands."""
+        """Handles commands."""
         command_name = data.content[len(self.command_prefix):].split(" ")[0]
 
-        if any([self.command_exists(command_name) != True, self.command_prefix != data.content[:len(self.command_prefix)]]):
-            if (
-                command_name == "help"
-                and data.content == f"{self.command_prefix}help"
-            ):
+        if (not self.command_exists(command_name) or
+                self.command_prefix != data.content[:len(self.command_prefix)]):
+
+            if (command_name == "help" and
+                    data.content == f"{self.command_prefix}help"):
                 return context.reply(self._commands.__help__())
+
             elif "text_message" in self._events:
-                return self._handle_text_message(data, context)
+                return self._handle_all_events(event="text_message", data=data, context=context)
+
             else:
                 return None
 
         if data.content[:len(self.command_prefix)] != self.command_prefix:
             return None
 
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
-        parameters = [{
-            "ctx": context,
-            "message": None if len(message) == 0 else message,
-            "username": data.author.username,
-            "userId": data.author.userId
-        }.get(i) for i in inspect_signature(self.fetch_command(command_name).func).parameters]
+        command_name = dict(self._commands.__command_aliases__().copy()).get(command_name, command_name)
+        
+        response = self._check_cooldown(command_name, data, context)
 
-        command_name = dict(self._commands.__command_aliases__().copy()).get(command_name, command_name)  
+        if response  != 403:
+            func = self._commands.fetch_command(command_name).func
+            return func(*self._set_parameters(context=context, func=func, message=message))
+        
+        return None
 
+        
+    def _check_cooldown(self, command_name: str, data: Message, context: Context) -> None:
+        """`_check_cooldown` is a function that checks if a command is on cooldown."""
         if self._commands.fetch_command(command_name).cooldown > 0:
             if self._commands.fetch_cooldown(command_name, data.author.userId) > time():
-                return context.reply(f"You are on cooldown for {int(self._commands.fetch_cooldown(command_name, data.author.userId) - time())} seconds.")
-            self._commands.set_cooldown(command_name, self._commands.fetch_command(command_name).cooldown, data.author.userId)
 
-        return self._commands.fetch_command(command_name).func(*parameters)
-        
+                context.reply(
+                    content=f"You are on cooldown for {int(self._commands.fetch_cooldown(command_name, data.author.userId) - time())} seconds."
+                    )
+                return 403
+            
+            self._commands.set_cooldown(
+                command_name=command_name,
+                cooldown=self._commands.fetch_command(command_name).cooldown,
+                userId=data.author.userId
+                )
+
+        return 200
+
+
     def on_error(self):
-        """
-        `on_error` - This is an event that handles errors to prevent the bot from crashing.
-        
-        `**Example**``
-        ```py
-        @bot.on_error()
-        def on_error(error: Exception):
-            print(error)
-        ```
-        """
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["error"] = func
             return func
         return decorator
 
-    def on_ready(self):
-        """
-        `on_ready` - This is an event that is called when the bot is ready.
 
-        `**Example**``
-        ```py
-        @bot.on_ready()
-        def on_ready():
-            print(f"Logged in as {bot.profile.username}")
-        ```
-        """
-        def decorator(func):
+    def on_ready(self):
+        def decorator(func: Callable) -> Callable:
             self._events["ready"] = func
             return func
         return decorator
 
-    def on_text_message(self):
-        """
-        `on_text_message` - This is an event that is called when a text message is received.
-
-        `**Example**``
-        ```py
-        # Basic usage.
-        @bot.on_text_message()
-        def on_text_message(ctx: Context):
-            ctx.send(content="Hello World!")
 
-        # Parameter usage.
-        @bot.on_text_message()
-        def on_text_message(ctx: Context, message: str, username: str, userId: str):
-            ctx.send(content=f"{username} said {message}")
-            print(userId)
-        ```
-        """
-        def decorator(func):
+    def on_text_message(self):
+        def decorator(func: Callable) -> Callable:
             self._events["text_message"] = func
             return func
         return decorator
-    
+
+
     def _add_cache(self, chatId: str, userId: str, content: str):
         if self._wait_for.get(f"{chatId}_{userId}") is not None:
             self._wait_for.clear(f"{chatId}_{userId}")
+            print("Cleared cache.")
 
         self._wait_for.add(
             key=f"{chatId}_{userId}",
             value=content,
             expire=90
             )
-        
-    def _remove_cache(self, chatId: str, userId: str):
-        self._wait_for.clear(f"{chatId}_{userId}")
+        print("Added cache.")
 
-    def _handle_text_message(self, data: Message, context: Context):
-        """`_handle_text_message` is a function that handles text messages."""
-        if data.content.startswith(self.command_prefix):
-            command_name = data.content.split(" ")[0][len(self.command_prefix):]
-        else:
-            command_name = None
-
-        parameters = [{
-            "ctx": context,
-            "command": self.command_prefix + command_name if command_name != None else "Command not found",
-            "message": context.message.content[len(command_name) + len(self.command_prefix) + 1:] if command_name else context.message.content,
-            "username": context.author.username,
-            "userId": context.author.userId
-        }.get(i) for i in inspect_signature(self._events["text_message"]).parameters]
-
-        return self._events["text_message"](*parameters)
 
     def on_image_message(self):
-        """
-        `on_image_message` - This is an event that is called when an image message is received.
-        
-        `**Example**``
-        ```py
-        # This will send the image back to the chat.
-        @bot.on_image_message()
-        def on_image_message(ctx: Context, image: str):
-            ctx.send_image(image=image)
-        ```
-        """
-        def decorator(func):
-            def wrapper(ctx: Context):
-                parameters = []
-                pparameters = {"ctx": ctx, "image": ctx.message.mediaValue}
-                for parameter in inspect_signature(func).parameters:
-                    parameters.append(pparameters.get(parameter, None))
-                func(*parameters)
-            self._events["image_message"] = wrapper
+        def decorator(func: Callable) -> Callable:
+            self._events["image_message"] = func
             return func
         return decorator
-        
-    def on_youtube_message(self):
-        """
-        `on_youtube_message` - This is an event that is called when a YouTube video message is received.
 
-        `**Example**``
-        ```py
-        # This will print the youtube title in the console.
-        @bot.on_youtube_message()
-        def on_youtube_message(ctx: Context, title: str):
-            print(title)
-        ```
-        """
-        def decorator(func):
-            def wrapper(ctx: Context):
-                parameters = []
-                pparameters = {"ctx": ctx, "title": ctx.message.content}
-                for parameter in inspect_signature(func).parameters:
-                    parameters.append(pparameters.get(parameter, None))
-                func(*parameters)
-            self._events["youtube_message"] = wrapper
+
+    def on_youtube_message(self):
+        def decorator(func: Callable) -> Callable:
+            self._events["youtube_message"] = func
             return func
         return decorator
 
+
     def on_strike_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["strike_message"] = func
             return func
         return decorator
 
+
     def on_voice_message(self):
-        """
-        `on_voice_message` - This is an event that is called when a voice message is received.
-        
-        `**Example**``
-        ```py
-        # This will send the audio message back to the chat.
-        @bot.on_voice_message()
-        def on_voice_message(ctx: Context, audio: str):
-            ctx.send_audio(audio=audio)
-        ```
-        """
-        def decorator(func):
-            def wrapper(ctx: Context):
-                inspect = len(inspect_signature(func).parameters)
-                if inspect > 2:
-                    return None
-                elif inspect > 1:
-                    func(ctx, ctx.message.mediaValue)
-                else:
-                    func(ctx)
-            self._events["voice_message"] = wrapper
+        def decorator(func: Callable) -> Callable:
+            self._events["voice_message"] = func
             return func
         return decorator
 
+
     def on_sticker_message(self):
-        def decorator(func):
-            def wrapper(ctx: Context):
-                inspect = len(inspect_signature(func).parameters)
-                if inspect > 2:
-                    return None
-                elif inspect > 1:
-                    func(ctx, ctx.message.mediaValue.split("://")[1])
-                else:
-                    func(ctx)
-            self._events["sticker_message"] = wrapper
+        def decorator(func: Callable) -> Callable:
+            self._events["sticker_message"] = func
             return func
         return decorator
 
+
     def on_vc_not_answered(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_not_answered"] = func
             return func
         return decorator
 
+
     def on_vc_not_cancelled(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_not_cancelled"] = func
             return func
         return decorator
 
+
     def on_vc_not_declined(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_not_declined"] = func
             return func
         return decorator
 
+
     def on_video_chat_not_answered(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["video_chat_not_answered"] = func
             return func
         return decorator
 
+
     def on_video_chat_not_cancelled(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["video_chat_not_cancelled"] = func
             return func
         return decorator
 
+
     def on_video_chat_not_declined(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["video_chat_not_declined"] = func
             return func
         return decorator
 
+
     def on_avatar_chat_not_answered(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["avatar_chat_not_answered"] = func
             return func
         return decorator
 
+
     def on_avatar_chat_not_cancelled(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["avatar_chat_not_cancelled"] = func
             return func
         return decorator
 
+
     def on_avatar_chat_not_declined(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["avatar_chat_not_declined"] = func
             return func
         return decorator
 
+
     def on_delete_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             def wrapper(ctx: Context):
-                inspect = len(inspect_signature(func).parameters)
-                if inspect > 2:
-                    return None
-                elif inspect > 1:
-                    func(ctx, ctx.message.messageId)
-                else:
-                    func(ctx)
+                func(*self._set_parameters(ctx, func))
             self._events["delete_message"] = wrapper
             return func
         return decorator
 
+
     def on_member_join(self):
-        def decorator(func):
-            def wrapper(ctx: Context):
-                potential_parameters = {
-                    "ctx": ctx,
-                    "username": ctx.author.username,
-                    "userId": ctx.author.userId
-                }
-                parameters = []
-                for parameter in inspect_signature(func).parameters:
-                    parameters.append(potential_parameters.get(parameter, None))
-                func(*parameters)
-            self._events["member_join"] = wrapper
+        def decorator(func: Callable) -> Callable:
+            self._events["member_join"] = func
             return func
         return decorator
 
+
     def on_member_leave(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["member_leave"] = func
             return func
         return decorator
 
+
     def on_chat_invite(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_invite"] = func
             return func
         return decorator
 
+
     def on_chat_background_changed(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_background_changed"] = func
             return func
         return decorator
 
+
     def on_chat_title_changed(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_title_changed"] = func
             return func
         return decorator
 
+
     def on_chat_icon_changed(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_icon_changed"] = func
             return func
         return decorator
 
+
     def on_vc_start(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_start"] = func
             return func
         return decorator
 
+
     def on_video_chat_start(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["video_chat_start"] = func
             return func
         return decorator
 
+
     def on_avatar_chat_start(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["avatar_chat_start"] = func
             return func
         return decorator
 
+
     def on_vc_end(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_end"] = func
             return func
         return decorator
 
+
     def on_video_chat_end(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["video_chat_end"] = func
             return func
         return decorator
 
+
     def on_avatar_chat_end(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["avatar_chat_end"] = func
             return func
         return decorator
 
+
     def on_chat_content_changed(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_content_changed"] = func
             return func
         return decorator
 
+
     def on_screen_room_start(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["screen_room_start"] = func
             return func
         return decorator
 
+
     def on_screen_room_end(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["screen_room_end"] = func
             return func
         return decorator
 
+
     def on_chat_host_transfered(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_host_transfered"] = func
             return func
         return decorator
 
+
     def on_text_message_force_removed(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["text_message_force_removed"] = func
             return func
         return decorator
 
+
     def on_chat_removed_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_removed_message"] = func
             return func
         return decorator
 
+
     def on_mod_deleted_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["mod_deleted_message"] = func
             return func
         return decorator
 
+
     def on_chat_tip(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_tip"] = func
             return func
         return decorator
 
+
     def on_chat_pin_announcement(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_pin_announcement"] = func
             return func
         return decorator
 
+
     def on_vc_permission_open_to_everyone(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_permission_open_to_everyone"] = func
             return func
         return decorator
 
+
     def on_vc_permission_invited_and_requested(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_permission_invited_and_requested"] = func
             return func
         return decorator
 
+
     def on_vc_permission_invite_only(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["vc_permission_invite_only"] = func
             return func
         return decorator
 
+
     def on_chat_view_only_enabled(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_view_only_enabled"] = func
             return func
         return decorator
 
+
     def on_chat_view_only_disabled(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_view_only_disabled"] = func
             return func
         return decorator
 
+
     def on_chat_unpin_announcement(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_unpin_announcement"] = func
             return func
         return decorator
 
+
     def on_chat_tipping_enabled(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_tipping_enabled"] = func
             return func
         return decorator
 
+
     def on_chat_tipping_disabled(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["chat_tipping_disabled"] = func
             return func
         return decorator
 
+
     def on_timestamp_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["timestamp_message"] = func
             return func
         return decorator
 
+
     def on_welcome_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["welcome_message"] = func
             return func
         return decorator
 
+
     def on_share_exurl_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["share_exurl_message"] = func
             return func
         return decorator
     
+
     def on_invite_message(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["invite_message"] = func
             return func
         return decorator
 
+
     def on_user_online(self):
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["user_online"] = func
             return func
         return decorator
 
 
     def on_member_set_you_host(self):
         """
@@ -1206,89 +1156,98 @@
 
         `**Example**``
         ```py
         from pymino.ext import *
         chatId = "0000-0000-0000-0000"
 
         @bot.on_member_set_you_host()
-        def member_set_you_host(notification: NNotification):
+        def member_set_you_host(notification: Notification):
             if notification.chatId == chatId:
                 print("You are now host")
                 bot.community.send_message(chatId=chatId, content="I am now host", comId=notification.comId)
         ```
         """
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["member_set_you_host"] = func
             return func
         return decorator
-    
+
+
     def on_member_set_you_cohost(self):
         """
         `on_member_set_you_cohost` - This is an event that is called when you are set as cohost.
         
         `**Example**``
         ```py
         from pymino.ext import *
         chatId = "0000-0000-0000-0000"
         
         @bot.on_member_set_you_cohost()
-        def member_set_you_cohost(notification: NNotification):
+        def member_set_you_cohost(notification: Notification):
             if notification.chatId == chatId:
                 print("You are now cohost")
                 bot.community.send_message(chatId=chatId, content="I am now cohost", comId=notification.comId)
         ```
         """
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["member_set_you_cohost"] = func
             return func
         return decorator
-    
+
+
     def on_member_remove_your_cohost(self):
         """
         `on_member_remove_your_cohost` - This is an event that is called when you are removed as cohost.
         
         `**Example**``
         ```py
         from pymino.ext import *
         chatId = "0000-0000-0000-0000"
         
         @bot.on_member_remove_your_cohost()
-        def member_remove_your_cohost(notification: NNotification):
+        def member_remove_your_cohost(notification: Notification):
             if notification.chatId == chatId:
                 print("You are no longer cohost")
                 bot.community.send_message(chatId=chatId, content="I am no longer cohost", comId=notification.comId)
         ```
         """
-        def decorator(func):
+        def decorator(func: Callable) -> Callable:
             self._events["member_remove_your_cohost"] = func
             return func
         return decorator
 
+
+    def _handle_all_events(self, event: str, data: Message, context: Context) -> None:
+        func = self._events[event]
+        return func(* self._set_parameters(context, func, data))
+
+
     def _handle_event(
         self,
         event: str,
-        data: Union[Message, OnlineMembers, NNotification, Context]
+        data: Union[Message, OnlineMembers, Notification, Context]
         ) -> Union[Context, None]:
         """
         `_handle_event` is a function that handles events.
         """
         with suppress(KeyError):
             context = self.context(data, self.request)
 
             if event == "text_message":
                 if not self.command_exists(
                     command_name=data.content[len(self.command_prefix):].split(" ")[0]
                     ):
                     self._add_cache(data.chatId, data.author.userId, data.content)
 
                 return self._handle_command(data=data, context=context)
-            
+
+
             if event in self._events:
                 if event in {
                     "user_online",
                     "member_set_you_host",
                     "member_set_you_cohost",
                     "member_remove_your_cohost",
                 }:
                     return self._events[event](data)
                 else:
-                    return self._events[event](context)
+                    return self._handle_all_events(event=event, data=data, context=context)
```

### Comparing `pymino-1.1.8.5/pymino/ext/dispatcher.py` & `pymino-1.1.8.6/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/entities/enums.py` & `pymino-1.1.8.6/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/entities/exceptions.py` & `pymino-1.1.8.6/pymino/ext/entities/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,29 +260,56 @@
     def __init__(self, response: str):
         super().__init__(response)
 
 class InternalServerError(Exception):
     def __init__(self, response: str):
         super().__init__(response)
 
+class InvalidEmail(Exception):
+    def __init__(self, response: str):
+        super().__init__(response)
+
+class InvalidPassword(Exception):
+    def __init__(self, response: str):
+        super().__init__(response)
+
+class WhoaCooldown(Exception):
+    def __init__(self, response: str):
+        super().__init__(response)
+
+class InvalidThemepack(Exception):
+    def __init__(self, response: str):
+        super().__init__(response)
+
+class InvalidVoiceNote(Exception):
+    def __init__(self, response: str):
+        super().__init__(response)
+
+class PostedTooRecently(Exception):
+    def __init__(self, response: str):
+        super().__init__(response)
+
 class APIException(Exception):
     def __init__(self, response: dict):
         self.exception_map = {
             100: UnsupportedService,
             101: InternalServerError,
             102: FileTooLarge,
             103: InvalidRequest,
+            104: InvalidRequest,
             105: InvalidSession,
             106: AccessDenied,
             107: UnexistentData,
             110: ActionNotAllowed,
             111: ServiceUnderMaintenance,
             113: MessageNeeded,
             200: InvalidAccountOrPassword,
             210: AccountDisabled,
+            213: InvalidEmail,
+            214: InvalidPassword,
             215: EmailAlreadyTaken,
             216: AccountDoesNotExist,
             218: InvalidDevice,
             219: AccountLimitReached,
             221: CantFollowYourself,
             225: UserUnavailable,
             229: YouAreBanned,
@@ -292,28 +319,33 @@
             239: CantLeaveCommunity,
             240: ReachedTitleLength,
             241: EmailFlaggedAsSpam,
             245: UserHasBeenDeleted,
             246: AccountDeleted,
             262: ReachedMaxTitles,
             270: VerificationRequired,
+            291: WhoaCooldown,
             293: UserBannedByTeamAmino,
             300: BadImage,
+            313: InvalidThemepack,
+            314: InvalidVoiceNote,
             500: RequestedNoLongerExists,
+            503: PostedTooRecently,
             551: InsufficientLevel,
             603: YouAreBlockedByThisUser,
             604: YouHaveBlockedThisUser,
             606: BlockedByOrganizer,
             700: NoLongerExists,
             702: WallCommentingDisabled,
             801: CommunityNoLongerExists,
             802: InvalidCodeOrLink,
             805: CommunityNameAlreadyTaken,
             806: CommunityCreateLimitReached,
             814: CommunityDisabled,
+            826: CommunityCreateLimitReached,
             833: CommunityDeleted,
             1600: DataNoLongerExists,
             1606: TooManyInviteUsers,
             1611: ChatInvitesDisabled,
             1612: RemovedFromChat,
             1613: UserNotJoined,
             1661: LevelFiveRequiredToEnableProps,
```

### Comparing `pymino-1.1.8.5/pymino/ext/entities/general.py` & `pymino-1.1.8.6/pymino/ext/entities/general.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,14 @@
 from re import findall
 from typing import Union, List
 
 from .exceptions import InvalidLink
+from .api_response import ApiResponse
 from .userprofile import UserProfile, UserProfileList
 
-class ApiResponse:
-    def __init__(self, data: Union[dict, str]) -> None:
-        self.data       = data
-        self.message    = None
-        self.statuscode = None
-        self.duration   = None
-        self.timestamp  = None
-        self.mediaValue = None
-        
-        if isinstance(self.data, dict):
-            self.message:       Union[str, None] = self.data.get("api:message", self.message)
-            self.statuscode:    Union[int, None] = self.data.get("api:statuscode", self.statuscode)
-            self.duration:      Union[str, None] = self.data.get("api:duration", self.duration)
-            self.timestamp:     Union[str, None] = self.data.get("api:timestamp", self.timestamp)
-            self.mediaValue:    Union[str, None] = self.data.get("mediaValue", self.mediaValue) or self.data.get("result", {}).get("mediaValue", self.mediaValue)
-        
-    def json(self) -> Union[dict, str]:
-        return self.data
-
-class LinkInfo:
-    def __init__(self, data: Union[dict, str]) -> None:
-        self.data               = data
-        self.linkInfoV2         = {}
-        self.path               = None
-        self.extensions         = {}
-        self.objectId           = None
-        self.shareURLShortCode  = None
-        self.targetCode         = None
-        self.ndcId              = None
-        self.comId              = None
-        self.fullPath           = None
-        self.shortCode          = None
-        self.objectType         = None
-
-        if isinstance(data, dict):
-            self.linkInfoV2:        dict = self.data.get("linkInfoV2", self.linkInfoV2)
-            self.path:              Union[str, None] = self.data.get("path", self.path)             or self.linkInfoV2.get("path", self.path)
-            self.extensions:        dict = self.data.get("extensions", self.extensions)             or self.linkInfoV2.get("extensions", self.extensions)
-            self.objectId:          Union[str, None] = self.data.get("objectId", self.objectId)     or self.extensions.get("linkInfo", {}).get("objectId", self.objectId)
-            self.shareURLShortCode: Union[str, None] = self.data.get("shareURLShortCode", self.shareURLShortCode) or self.extensions.get("linkInfo", {}).get("shareURLShortCode", self.shareURLShortCode)
-            self.targetCode:        Union[str, None] = self.data.get("targetCode", self.targetCode) or self.extensions.get("linkInfo", {}).get("targetCode", self.targetCode)
-            self.ndcId:             Union[int, None] = self.data.get("ndcId", self.ndcId)           or self.extensions.get("linkInfo", {}).get("ndcId", self.ndcId)
-            self.comId:             Union[int, None] = self.ndcId
-            self.fullPath:          Union[str, None] = self.data.get("fullPath", self.fullPath)     or self.extensions.get("linkInfo", {}).get("fullPath", self.fullPath)
-            self.shortCode:         Union[str, None] = self.data.get("shortCode", self.shortCode)   or self.extensions.get("linkInfo", {}).get("shortCode", self.shortCode)
-            self.objectType:        Union[str, None] = self.data.get("objectType", self.objectType) or self.extensions.get("linkInfo", {}).get("objectType", self.objectType)
-
-    def json(self) -> Union[dict, str]:
-        return self.data
 
 class CommunityInvitation:
     def __init__(self, data: Union[dict, str]) -> None:
         self.data                = data
         self.communityInvitation = {}
         self.status              = None
         self.duration            = None
@@ -564,119 +516,15 @@
         self.members = []
 
         if isinstance(data, dict):
             self.members: UserProfileList = UserProfileList(self.data.get("memberList", self.members))
 
     def json(self) -> Union[dict, str]:
         return self.data
-    
-class CComment:
-    def __init__(self, data: Union[dict, str]) -> None:
-        self.data = data
-        self.modifiedTime = None
-        self.ndcId = None
-        self.votedValue = None
-        self.parentType = None
-        self.commentId = None
-        self.parentNdcId = None
-        self.mediaList = None
-        self.votesSum = None
-        self.author = {}
-        self.extensions = {}
-        self.content = None
-        self.parentId = None
-        self.createdTime = None
-        self.subcommentsCount = None
-        self.type = None
-
-        if isinstance(data, dict):
-            self.modifiedTime:      Union[str, None] = self.data.get("modifiedTime", self.modifiedTime)
-            self.ndcId:             Union[int, None] = self.data.get("ndcId", self.ndcId)
-            self.votedValue:        Union[int, None] = self.data.get("votedValue", self.votedValue)
-            self.parentType:        Union[int, None] = self.data.get("parentType", self.parentType)
-            self.commentId:         Union[str, None] = self.data.get("commentId", self.commentId)
-            self.parentNdcId:       Union[int, None] = self.data.get("parentNdcId", self.parentNdcId)
-            self.mediaList:         Union[None, None] = self.data.get("mediaList", self.mediaList)
-            self.votesSum:          Union[int, None] = self.data.get("votesSum", self.votesSum)
 
-            try:
-                self.author:            Union[UserProfile, None] = UserProfile(self.data.get("author", self.author))
-            except Exception:
-                self.author:            Union[UserProfile, None] = None
-
-            self.extensions:        CCommentExtensions = CCommentExtensions(self.data.get("extensions", self.extensions))
-            self.content:           Union[str, None] = self.data.get("content", self.content)
-            self.parentId:          Union[str, None] = self.data.get("parentId", self.parentId)
-            self.createdTime:       Union[str, None] = self.data.get("createdTime", self.createdTime)
-            self.subcommentsCount:  Union[int, None] = self.data.get("subcommentsCount", self.subcommentsCount)
-            self.type:              Union[int, None] = self.data.get("type", self.type)
-        
-    def json(self) -> Union[dict, str]:
-        return self.data
-
-class CCommentList:
-    def __init__(self, data: Union[dict, str]) -> None:
-        self.data:              dict = data.get("commentList", [])
-        parser:                 list = [CComment(x) for x in self.data]
-        self.modifiedTime:      list = [x.modifiedTime for x in parser]
-        self.ndcId:             list = [x.ndcId for x in parser]
-        self.votedValue:        list = [x.votedValue for x in parser]
-        self.parentType:        list = [x.parentType for x in parser]
-        self.commentId:         list = [x.commentId for x in parser]
-        self.parentNdcId:       list = [x.parentNdcId for x in parser]
-        self.mediaList:         list = [x.mediaList for x in parser]
-        self.votesSum:          list = [x.votesSum for x in parser]
-        #self.author:            list = [x.author for x in parser]
-        #self.extensions:        list = [x.extensions for x in parser]
-        self.content:           list = [x.content for x in parser]
-        self.parentId:          list = [x.parentId for x in parser]
-        self.createdTime:       list = [x.createdTime for x in parser]
-        self.subcommentsCount:  list = [x.subcommentsCount for x in parser]
-        self.type:              list = [x.type for x in parser]
-
-    def json(self) -> Union[dict, str]:
-        return self.data
-
-class CCommentExtensions:
-    def __init__(self, data: Union[dict, str]) -> None:
-        self.data = data
-        self.status = None
-        self.iconV2 = None
-        self.name = None
-        self.stickerId = None
-        self.smallIconV2 = None
-        self.smallIcon = None
-        self.stickerCollectionId = None
-        self.mediumIcon = None
-        self.stickerCollectionSummary = {}
-        self.extensions = None
-        self.usedCount = None
-        self.mediumIconV2 = None
-        self.createdTime = None
-        self.icon = None
-
-        if isinstance(data, dict):
-            self.data:                      Union[dict, None] = self.data.get("sticker", self.data)
-            self.status:                    Union[int, None] = self.data.get("status", self.status)
-            self.iconV2:                    Union[str, None] = self.data.get("iconV2", self.iconV2)
-            self.name:                      Union[str, None] = self.data.get("name", self.name)
-            self.stickerId:                 Union[str, None] = self.data.get("stickerId", self.stickerId)
-            self.smallIconV2:               Union[str, None] = self.data.get("smallIconV2", self.smallIconV2)
-            self.smallIcon:                 Union[str, None] = self.data.get("smallIcon", self.smallIcon)
-            self.stickerCollectionId:       Union[str, None] = self.data.get("stickerCollectionId", self.stickerCollectionId)
-            self.mediumIcon:                Union[str, None] = self.data.get("mediumIcon", self.mediumIcon)
-            self.stickerCollectionSummary:  Union[dict, None] = self.data.get("stickerCollectionSummary", self.stickerCollectionSummary)
-            self.extensions:                Union[None, None] = self.data.get("extensions", self.extensions)
-            self.usedCount:                 Union[int, None] = self.data.get("usedCount", self.usedCount)
-            self.mediumIconV2:              Union[str, None] = self.data.get("mediumIconV2", self.mediumIconV2)
-            self.createdTime:               Union[None, None] = self.data.get("createdTime", self.createdTime)
-            self.icon:                      Union[str, None] = self.data.get("icon", self.icon)
-
-    def json(self) -> Union[dict, str]:
-        return self.data
 
 class FeaturedBlog:
     def __init__(self, data: Union[dict, str]):
         self.data           = data
 
     def return_none(func):
         def wrapper(*args, **kwargs):
```

### Comparing `pymino-1.1.8.5/pymino/ext/entities/handlers.py` & `pymino-1.1.8.6/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/entities/messages.py` & `pymino-1.1.8.6/pymino/ext/entities/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,142 +19,125 @@
         """`JSON` - returns the raw data."""
         return self.base_message
 
 class MessageAuthor:
     def __init__(self, data: Union[dict, str]) -> None:
         self.data = data
 
-    def return_none(func):
-        def wrapper(*args, **kwargs):
-            return None if args[0].data is None else func(*args, **kwargs)
-        return wrapper
-    
     @property
-    @return_none
     def uid(self) -> Union[str, None]:
         """
         `uid` - returns the user id of the author.
             - `str` - The user id of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("uid")
     
     @property
-    @return_none
     def userId(self) -> Union[str, None]:
         """
         `userId` - returns the user id of the author.
             - `str` - The user id of the author.
             - `None` - If the data is `None`.
 
         """
         return self.uid
     
     @property
-    @return_none
     def status(self) -> Union[int, None]:
         """
         `status` - returns the status of the author.
             - `int` - The status of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("status")
     
     @property
-    @return_none
     def icon(self) -> Union[str, None]:
         """
         `icon` - returns the icon of the author.
             - `str` - The icon of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("icon")
     
     @property
-    @return_none
     def avatar(self) -> Union[str, None]:
         """
         `avatar` - returns the icon of the author.
             - `str` - The icon of the author.
             - `None` - If the data is `None`.
 
         """
         return self.icon
     
     @property
-    @return_none
     def reputation(self) -> Union[int, None]:
         """
         `reputation` - returns the reputation of the author.
             - `int` - The reputation of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("reputation")
     
     @property
-    @return_none
     def role(self) -> Union[int, None]:
         """
         `role` - returns the role of the author.
             - `int` - The role of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("role")
     
     @property
-    @return_none
     def nickname(self) -> Union[str, None]:
         """
         `nickname` - returns the nickname of the author.
             - `str` - The nickname of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("nickname")
     
     @property
-    @return_none
     def username(self) -> Union[str, None]:
         """
         `username` - returns the nickname of the author.
             - `str` - The nickname of the author.
             - `None` - If the data is `None`.
 
         """
         return self.nickname
     
     @property
-    @return_none
     def level(self) -> Union[int, None]:
         """
         `level` - returns the level of the author.
             - `int` - The level of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("level")
     
     @property
-    @return_none
     def accountMembershipStatus(self) -> Union[int, None]:
         """
         `accountMembershipStatus` - returns the account membership status of the author.
             - `int` - The account membership status of the author.
             - `None` - If the data is `None`.
 
         """
         return self.data.get("accountMembershipStatus")
     
     @property
-    @return_none
     def avatarFrame(self) -> Union[str, None]:
         """
         `avatarFrame` - returns the avatar frame of the author.
             - `str` - The avatar frame of the author.
             - `None` - If the data is `None`.
 
         """
@@ -1279,65 +1262,9 @@
 
         """
         return self.threadId
     
     def json(self) -> Union[dict, str]:
         """`JSON` - returns the raw data."""
         return self.data
-    
-class NNotification:
-    def __init__(self, data: dict):
-        """
-        `NNotification - This contains all attributes aor any notification event.
-        """
-        self.data: dict = data
 
-    @property
-    def __parser__(self) -> dict:
-        try:
-            return self.data.get("o")
-        except Exception:
-            print(self.data)
-            return self.data
-    
-    @property
-    def payload(self) -> dict:
-        return self.__parser__.get("payload")
-    
-    @property
-    def exp(self) -> int:
-        return self.payload.get("exp")
-    
-    @property
-    def ndcId(self) -> int:
-        return self.payload.get("ndcId")
-    
-    @property
-    def comId(self) -> int:
-        return self.ndcId
-    
-    @property
-    def chatId(self) -> str:
-        return self.payload.get("tid")
-    
-    @property
-    def aps(self) -> dict:
-        return self.payload.get("aps")
-    
-    @property
-    def sound(self) -> str:
-        return self.aps.get("sound")
-    
-    @property
-    def alert(self) -> str:
-        return self.aps.get("alert")
-    
-    @property
-    def notifType(self) -> int:
-        return self.payload.get("notifType")
-    
-    @property
-    def id(self) -> str:
-        return self.payload.get("id")
-    
-    def json(self) -> dict:
-        return self.data
+
```

### Comparing `pymino-1.1.8.5/pymino/ext/entities/userprofile.py` & `pymino-1.1.8.6/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/entities/wsevents.py` & `pymino-1.1.8.6/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/handle_queue.py` & `pymino-1.1.8.6/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/socket.py` & `pymino-1.1.8.6/pymino/ext/socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 from typing import Optional
 from threading import Thread
 from contextlib import suppress
 from urllib.parse import urlencode
 from time import sleep as delay, time
 from ujson import loads, dumps, JSONDecodeError
 
+from .entities import *
 from .context import EventHandler
 from .dispatcher import MessageDispatcher
-from .entities.wsevents import EventTypes, NotifTypes
-from .entities.userprofile import OnlineMembers
-from .entities.messages import Channel, Message, NNotification
-from .entities.exceptions import WrongWebSocketPackage
 from .utilities.generate import device_id, generate_signature
-from .entities.handlers import run_alive_loop, orjson_exists
 
 if orjson_exists():
     from orjson import (
         loads as orjson_loads, dumps as orjson_dumps
         )
 
 
@@ -115,16 +111,16 @@
         key = self.event_types.get(f"{_message.type}:{_message.mediaType}")
         if key != None:
             return Thread(target=self._handle_event, args=(key, _message)).start()
 
 
     def _handle_notification(self, message: dict) -> None:
         """Handles notifications."""
-        notification: NNotification = NNotification(message)
-        key = self.notif_types.get(notification.notifType)
+        notification: Notification = Notification(message)
+        key = self.notif_types.get(notification.notification_type)
         if key != None:
             return Thread(target=self._handle_event, args=(key, notification)).start()
 
 
     def _handle_agora_channel(self, message: dict) -> None:
         """Sets the agora channel."""
         self.channel: Channel = Channel(message)
```

### Comparing `pymino-1.1.8.5/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.8.6/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/utilities/commands.py` & `pymino-1.1.8.6/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/utilities/generate.py` & `pymino-1.1.8.6/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino/ext/utilities/request_handler.py` & `pymino-1.1.8.6/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.5/pymino.egg-info/PKG-INFO` & `pymino-1.1.8.6/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.5
+Version: 1.1.8.6
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.5 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.6 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.5/pymino.egg-info/SOURCES.txt` & `pymino-1.1.8.6/pymino.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,20 +19,24 @@
 pymino/ext/async_socket.py
 pymino/ext/community.py
 pymino/ext/context.py
 pymino/ext/dispatcher.py
 pymino/ext/handle_queue.py
 pymino/ext/socket.py
 pymino/ext/entities/__init__.py
+pymino/ext/entities/api_response.py
+pymino/ext/entities/chat_threads.py
+pymino/ext/entities/comments.py
 pymino/ext/entities/enums.py
 pymino/ext/entities/exceptions.py
 pymino/ext/entities/general.py
 pymino/ext/entities/handlers.py
+pymino/ext/entities/link_info.py
 pymino/ext/entities/messages.py
-pymino/ext/entities/threads.py
+pymino/ext/entities/notification.py
 pymino/ext/entities/userprofile.py
 pymino/ext/entities/wsevents.py
 pymino/ext/utilities/__init__.py
 pymino/ext/utilities/async_request_handler.py
 pymino/ext/utilities/commands.py
 pymino/ext/utilities/generate.py
 pymino/ext/utilities/request_handler.py
```

### Comparing `pymino-1.1.8.5/setup.cfg` & `pymino-1.1.8.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e38 2e35 0d0a 6175  on = 1.1.8.5..au
+00000020: 6f6e 203d 2031 2e31 2e38 2e36 0d0a 6175  on = 1.1.8.6..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.8.5/setup.py` & `pymino-1.1.8.6/setup.py`

 * *Files identical despite different names*

