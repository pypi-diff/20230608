# Comparing `tmp/villa-0.1.0.tar.gz` & `tmp/villa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.1.0.tar", max compression
+gzip compressed data, was "villa-0.1.1.tar", max compression
```

## Comparing `villa-0.1.0.tar` & `villa-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-06 16:06:13.632853 villa-0.1.0/LICENSE
--rw-r--r--   0        0        0     2128 2023-06-06 16:06:13.632853 villa-0.1.0/README.md
--rw-r--r--   0        0        0      821 2023-06-06 16:06:13.632853 villa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      120 2023-06-06 16:06:13.632853 villa-0.1.0/villa/__init__.py
--rw-r--r--   0        0        0    30352 2023-06-06 16:06:13.636853 villa-0.1.0/villa/bot.py
--rw-r--r--   0        0        0     5146 2023-06-06 16:06:13.636853 villa-0.1.0/villa/event.py
--rw-r--r--   0        0        0      473 2023-06-06 16:06:13.636853 villa-0.1.0/villa/exception.py
--rw-r--r--   0        0        0     1504 2023-06-06 16:06:13.636853 villa-0.1.0/villa/log.py
--rw-r--r--   0        0        0    18105 2023-06-06 16:06:13.636853 villa-0.1.0/villa/message.py
--rw-r--r--   0        0        0     9421 2023-06-06 16:06:13.636853 villa-0.1.0/villa/models.py
--rw-r--r--   0        0        0      113 2023-06-06 16:06:13.636853 villa-0.1.0/villa/store.py
--rw-r--r--   0        0        0      794 2023-06-06 16:06:13.636853 villa-0.1.0/villa/typing.py
--rw-r--r--   0        0        0      995 2023-06-06 16:06:13.636853 villa-0.1.0/villa/utils.py
--rw-r--r--   0        0        0     2860 1970-01-01 00:00:00.000000 villa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-08 14:38:00.643531 villa-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2399 2023-06-08 14:38:00.643531 villa-0.1.1/README.md
+-rw-r--r--   0        0        0     1034 2023-06-08 14:38:00.643531 villa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-06-08 14:38:00.643531 villa-0.1.1/villa/__init__.py
+-rw-r--r--   0        0        0    30767 2023-06-08 14:38:00.643531 villa-0.1.1/villa/bot.py
+-rw-r--r--   0        0        0     7799 2023-06-08 14:38:00.643531 villa-0.1.1/villa/event.py
+-rw-r--r--   0        0        0      473 2023-06-08 14:38:00.643531 villa-0.1.1/villa/exception.py
+-rw-r--r--   0        0        0     1504 2023-06-08 14:38:00.643531 villa-0.1.1/villa/log.py
+-rw-r--r--   0        0        0    16613 2023-06-08 14:38:00.643531 villa-0.1.1/villa/message.py
+-rw-r--r--   0        0        0     9982 2023-06-08 14:38:00.643531 villa-0.1.1/villa/models.py
+-rw-r--r--   0        0        0      113 2023-06-08 14:38:00.643531 villa-0.1.1/villa/store.py
+-rw-r--r--   0        0        0      794 2023-06-08 14:38:00.643531 villa-0.1.1/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-06-08 14:38:00.643531 villa-0.1.1/villa/utils.py
+-rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 villa-0.1.1/PKG-INFO
```

### Comparing `villa-0.1.0/LICENSE` & `villa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.1.0/README.md` & `villa-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
 <a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/villa-py@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/villa-py" alt="license"></a>
 
 </div>
 
 ## 特性
 
-- 基于`FastAPI`，异步、快速、高性能！
+- 基于`FastAPI`和`Pydantic`，异步、快速、高性能！
+- 完整的类型注解支持
 - 便捷的消息构造和发送方法
-- 完整的消息段和API支持
+- 丰富的消息段和完整的API支持
 - ~~想不出来了~~
 
 ## 安装
 
 - 使用pip: `pip install villa`
 - 使用poetry: `poetry add villa`
 - 使用pdm: `pdm add villa`
 
 ## 快速开始
 
-首先你需要一个米游社大别野的Bot，如果没有请先自行申请，拿到`bot_id`、`bot_secret`
+首先你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的Bot，如果没有请先到机器人开发者社区(别野ID: OpenVilla)申请，取得`bot_id`、`bot_secret`
 
 ```python
 from villa import Bot
 from villa.event import SendMessageEvent
 
 bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url")
 # 初始化Bot，填写你的bot_id、密钥以及回调地址
@@ -55,14 +56,19 @@
 - `send_message.py`: 各种消息发送方法介绍
 
 
 ## 反馈
 
 目前无论是大别野Bot还是本SDK都在测试开发中，如遇问题请提出issue，感谢支持！
 
+也欢迎来我的大别野【尘世闲游】进行交流~ 
+
+- 大别野ID: wgiJNaU
+- [Web端链接](https://dby.miyoushe.com/chat/1047/21652)
+
 ## 相关项目
 
 - [NoneBot2](https://github.com/nonebot/nonebot2) 非常好用的Python跨平台机器人框架！
 - [nonebot-adapter-villa](https://github.com/CMHopeSunshine/nonebot-adapter-villa) NoneBot2的大别野Bot适配器。
 
 推荐有成熟Python开发经验但对NoneBot2不熟悉的小伙伴选择`本SDK`，
```

### Comparing `villa-0.1.0/pyproject.toml` & `villa-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "villa"
-version = "0.1.0"
+version = "0.1.1"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/CMHopeSunshine/villa-py"
+repository = "https://github.com/CMHopeSunshine/villa-py"
+documentation = "https://github.com/CMHopeSunshine/villa-py"
+keywords = ["mihoyo", "bot", "villa"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = {extras = ["uvicorn"], version = "^0.96.0"}
 uvicorn = "^0.22.0"
 httpx = "^0.24.1"
 loguru = "^0.7.0"
```

### Comparing `villa-0.1.0/villa/bot.py` & `villa-0.1.1/villa/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,20 +407,22 @@
             "vila/api/bot/platform/deleteRoom",
             villa_id,
             json={"room_id": room_id},
         )
 
     async def get_room(self, villa_id: int, room_id: int) -> Room:
         return Room.parse_obj(
-            await self._request(
-                "GET",
-                "vila/api/bot/platform/getRoom",
-                villa_id,
-                json={"room_id": room_id},
-            )
+            (
+                await self._request(
+                    "GET",
+                    "vila/api/bot/platform/getRoom",
+                    villa_id,
+                    json={"room_id": room_id},
+                )
+            )["room"]
         )
 
     async def get_villa_group_room_list(self, villa_id: int) -> GroupRoom:
         return GroupRoom.parse_obj(
             (
                 await self._request(
                     "GET",
@@ -636,86 +638,95 @@
                     break
         if is_handled:
             logger.opt(colors=True).success(
                 f"<b><y>[{event.__class__.__name__}]</y></b> handle completed"
             )
 
     async def _parse_message_content(self, message: Message) -> MessageContentInfo:
-        if quote := message["quote", 1]:
+        if quote := message["quote", 0]:
             quote = QuoteInfo(**quote.dict())
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         images: List[Image] = []
         mentioned = MentionedInfo(type=MentionType.PART)
-        for i, seg in enumerate(message.__root__):
+        for seg in message:
             try:
-                space = " " if i != len(message) - 1 else ""
                 if isinstance(seg, TextSegment):
                     message_text += seg.content
                     message_offset += len(seg.content)
                 elif isinstance(seg, MentionAllSegment):
-                    message_text += "@全体成员{space}"
+                    message_text += f"@{seg.show_text} "
                     entities.append(
                         TextEntity(
-                            offset=message_offset, length=6, entity=MentionedAll()
+                            offset=message_offset,
+                            length=6,
+                            entity=MentionedAll(show_text=seg.show_text),
                         )
                     )
-                    message_offset += 6
+                    message_offset += len(f"@{seg.show_text} ")
                     mentioned.type = MentionType.ALL
                 elif isinstance(seg, MentionRobotSegment):
                     bot_name = self.bot_info.template.name if self.bot_info else "Bot"
-                    message_text += f"@{bot_name}{space}"
+                    message_text += f"@{bot_name} "
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=len(f"@{bot_name}".encode("utf-16")) // 2,
-                            entity=MentionedRobot(bot_id=self.bot_id),
+                            entity=MentionedRobot(
+                                bot_id=self.bot_id, bot_name=bot_name
+                            ),
                         )
                     )
                     message_offset += len(f"@{bot_name}") + 1
                     mentioned.user_id_list.append(self.bot_id)
                 elif isinstance(seg, MentionUserSegment):
                     # 需要调用API获取被@的用户的昵称
                     user = await self.get_member(villa_id=seg.villa_id, uid=seg.user_id)
-                    message_text += f"@{user.basic.nickname}{space}"
+                    message_text += f"@{user.basic.nickname} "
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=len(f"@{user.basic.nickname}".encode("utf-16")) // 2,
-                            entity=MentionedUser(user_id=str(user.basic.uid)),
+                            entity=MentionedUser(
+                                user_id=str(user.basic.uid),
+                                user_name=user.basic.nickname,
+                            ),
                         )
                     )
                     message_offset += len(f"@{user.basic.nickname}") + 1
                     mentioned.user_id_list.append(str(user.basic.uid))
                 elif isinstance(seg, RoomLinkSegment):
                     # 需要调用API获取房间的名称
                     room = await self.get_room(
                         villa_id=seg.villa_id, room_id=seg.room_id
                     )
-                    message_text += f"#{room.room_name}{space}"
+                    message_text += f"#{room.room_name} "
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=len(f"#{room.room_name}".encode("utf-16")) // 2,
                             entity=VillaRoomLink(
                                 villa_id=str(seg.villa_id),
                                 room_id=str(seg.room_id),
+                                room_name=room.room_name,
                             ),
                         )
                     )
                     message_offset += len(f"#{room.room_name} ")
                 elif isinstance(seg, LinkSegment):
                     show_text = seg.show_text or seg.url
-                    message_text += show_text + space
+                    message_text += show_text
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=len(show_text.encode("utf-16")) // 2,
-                            entity=Link(url=seg.url),
+                            entity=Link(
+                                url=seg.url, show_text=seg.show_text or seg.url
+                            ),
                         )
                     )
                     message_offset += len(show_text) + 1
                 elif isinstance(seg, ImageSegment):
                     images.append(
                         Image(
                             url=seg.url,
```

### Comparing `villa-0.1.0/villa/log.py` & `villa-0.1.1/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.0/villa/message.py` & `villa-0.1.1/villa/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     """消息段基类"""
 
     @staticmethod
     def text(text: str) -> "Text":
         return Text(content=text)
 
     @staticmethod
-    def mention_robot(bot_id: str, bot_name: Optional[str] = None) -> "MentionRobot":
+    def mention_robot(bot_id: str, bot_name: str) -> "MentionRobot":
         return MentionRobot(bot_id=bot_id, bot_name=bot_name)
 
     @staticmethod
     def mention_user(villa_id: int, user_id: int) -> "MentionUser":
         return MentionUser(villa_id=villa_id, user_id=user_id)
 
     @staticmethod
-    def mention_all() -> "MentionAll":
-        return MentionAll()
+    def mention_all(show_text: str = "全体成员") -> "MentionAll":
+        return MentionAll(show_text=show_text)
 
     @staticmethod
     def room_link(villa_id: int, room_id: int) -> "RoomLink":
         return RoomLink(villa_id=villa_id, room_id=room_id)
 
     @staticmethod
     def link(url: str, show_text: Optional[str] = None) -> "Link":
@@ -95,29 +95,30 @@
 
 
 class MentionRobot(MessageSegment):
     """@机器人消息段"""
 
     type: Literal["mention_robot"] = "mention_robot"
     bot_id: str
-    bot_name: Optional[str] = None
+    bot_name: str
 
 
 class MentionUser(MessageSegment):
     """@用户消息段"""
 
     type: Literal["mention_user"] = "mention_user"
     villa_id: int
     user_id: int
 
 
 class MentionAll(MessageSegment):
     """@全体成员消息段"""
 
     type: Literal["mention_all"] = "mention_all"
+    show_text: str = "全体成员"
 
 
 class RoomLink(MessageSegment):
     """房间链接消息段"""
 
     type: Literal["room_link"] = "room_link"
     villa_id: int
@@ -216,15 +217,15 @@
 
         返回:
             Self: 消息对象
         """
         self.__root__.append(MentionAll())
         return self
 
-    def mention_robot(self, bot_id: str, bot_name: Optional[str] = None) -> Self:
+    def mention_robot(self, bot_id: str, bot_name: str) -> Self:
         """提及(@at)机器人消息
 
         参数:
             bot_id: 机器人ID
             bot_name: 机器人名称
 
         返回:
@@ -327,49 +328,14 @@
         返回:
             Self: 消息对象
         """
         if isinstance(segment, str):
             segment = Text(content=segment)
         self.__root__.append(segment)
 
-    @classmethod
-    def _parse(cls, content: MessageContentInfo, villa_id: int) -> Self:
-        msg = cls()
-        text = content.content.text
-        text_begin = 0
-        for entity in content.content.entities:
-            if isinstance(entity.entity, MentionedRobotInfo):
-                msg.mention_robot(entity.entity.bot_id)
-            elif isinstance(entity.entity, MentionedUserInfo):
-                msg.mention_user(villa_id, int(entity.entity.user_id))
-            elif isinstance(entity.entity, MentionedAllInfo):
-                msg.mention_all()
-            elif isinstance(entity.entity, VillaRoomLinkInfo):
-                msg.room_link(int(entity.entity.villa_id), int(entity.entity.room_id))
-            elif isinstance(entity.entity, LinkInfo):
-                msg.link(entity.entity.url, entity.entity.url)
-            if text_sengment := text[text_begin : entity.offset]:
-                msg.text(text_sengment)
-            text = text[(entity.offset + entity.length) :]
-        if text:
-            msg.text(text)
-        if content.content.images:
-            for image in content.content.images:
-                msg.image(
-                    image.url,
-                    image.size.width if image.size else None,
-                    image.size.height if image.size else None,
-                    image.file_size,
-                )
-        if content.quote:
-            msg.quote(
-                content.quote.quoted_message_id, content.quote.quoted_message_send_time
-            )
-        return msg
-
     def plain_text(self) -> str:
         """获取纯文本消息内容"""
         return "".join(
             [segment.content for segment in self.__root__ if isinstance(segment, Text)]
         )
 
     def __contains__(self, item: str) -> bool:
@@ -621,17 +587,17 @@
             "link",
             "image",
             "quote",
         ):
             if arg2 is None:
                 return Message([seg for seg in self.__root__ if seg.type == arg1])
             elif isinstance(arg2, int):
-                if l := [seg for seg in self.__root__ if seg.type == arg1]:
-                    return l[arg2]
-                else:
+                try:
+                    return [seg for seg in self.__root__ if seg.type == arg1][arg2]
+                except IndexError:
                     return None
             elif isinstance(arg2, slice):
                 return Message([seg for seg in self.__root__ if seg.type == arg1][arg2])
             else:
                 raise ValueError("Incorrect arguments to slice")
         else:
             raise ValueError("Incorrect arguments to slice")
```

### Comparing `villa-0.1.0/villa/models.py` & `villa-0.1.1/villa/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,22 @@
 
     @root_validator(pre=True)
     def _add_villa_id_to_extend_data(cls, values: dict):
         """把villa_id和bot_id添加到extend_data中，方便使用"""
         if values.get("type") == 2 and "SendMessage" in values.get(
             "extend_data", {}
         ).get("EventData", {}):
+            if isinstance(
+                values["extend_data"]["EventData"]["SendMessage"]["content"], str
+            ):
+                values["extend_data"]["EventData"]["SendMessage"][
+                    "content"
+                ] = json.loads(
+                    values["extend_data"]["EventData"]["SendMessage"]["content"]
+                )
             if (
                 "villa_id" in values.get("robot", {})
                 and "villa_id" not in values["extend_data"]["EventData"]["SendMessage"]
             ):
                 values["extend_data"]["EventData"]["SendMessage"]["villa_id"] = values[
                     "robot"
                 ]["villa_id"]
@@ -128,34 +136,44 @@
         return self.name
 
 
 class MentionedRobot(BaseModel):
     type: Literal["mentioned_robot"] = "mentioned_robot"
     bot_id: str
 
+    bot_name: str = Field(exclude=True)
+
 
 class MentionedUser(BaseModel):
     type: Literal["mentioned_user"] = "mentioned_user"
     user_id: str
 
+    user_name: str = Field(exclude=True)
+
 
 class MentionedAll(BaseModel):
     type: Literal["mention_all"] = "mention_all"
 
+    show_text: str = Field(exclude=True)
+
 
 class VillaRoomLink(BaseModel):
     type: Literal["villa_room_link"] = "villa_room_link"
     villa_id: str
     room_id: str
 
+    room_name: str = Field(exclude=True)
+
 
 class Link(BaseModel):
     type: Literal["link"] = "link"
     url: str
 
+    show_text: str = Field(exclude=True)
+
 
 class TextEntity(BaseModel):
     offset: int
     length: int
     entity: Union[MentionedRobot, MentionedUser, MentionedAll, VillaRoomLink, Link]
```

### Comparing `villa-0.1.0/villa/typing.py` & `villa-0.1.1/villa/typing.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.0/villa/utils.py` & `villa-0.1.1/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.1.0/PKG-INFO` & `villa-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.1.0
+Version: 0.1.1
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
+Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
+Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi[uvicorn] (>=0.96.0,<0.97.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Project-URL: Documentation, https://github.com/CMHopeSunshine/villa-py
+Project-URL: Repository, https://github.com/CMHopeSunshine/villa-py
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # Villa
 
 _✨ 米游社大别野Bot Python SDK ✨_
@@ -28,28 +32,29 @@
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
 <a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/villa-py@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/villa-py" alt="license"></a>
 
 </div>
 
 ## 特性
 
-- 基于`FastAPI`，异步、快速、高性能！
+- 基于`FastAPI`和`Pydantic`，异步、快速、高性能！
+- 完整的类型注解支持
 - 便捷的消息构造和发送方法
-- 完整的消息段和API支持
+- 丰富的消息段和完整的API支持
 - ~~想不出来了~~
 
 ## 安装
 
 - 使用pip: `pip install villa`
 - 使用poetry: `poetry add villa`
 - 使用pdm: `pdm add villa`
 
 ## 快速开始
 
-首先你需要一个米游社大别野的Bot，如果没有请先自行申请，拿到`bot_id`、`bot_secret`
+首先你需要一个[米游社大别野](https://dby.miyoushe.com/chat)的Bot，如果没有请先到机器人开发者社区(别野ID: OpenVilla)申请，取得`bot_id`、`bot_secret`
 
 ```python
 from villa import Bot
 from villa.event import SendMessageEvent
 
 bot = Bot(bot_id="your_bot_id", bot_secret="your_bot_secret", callback_url="your_callback_url")
 # 初始化Bot，填写你的bot_id、密钥以及回调地址
@@ -75,14 +80,19 @@
 - `send_message.py`: 各种消息发送方法介绍
 
 
 ## 反馈
 
 目前无论是大别野Bot还是本SDK都在测试开发中，如遇问题请提出issue，感谢支持！
 
+也欢迎来我的大别野【尘世闲游】进行交流~ 
+
+- 大别野ID: wgiJNaU
+- [Web端链接](https://dby.miyoushe.com/chat/1047/21652)
+
 ## 相关项目
 
 - [NoneBot2](https://github.com/nonebot/nonebot2) 非常好用的Python跨平台机器人框架！
 - [nonebot-adapter-villa](https://github.com/CMHopeSunshine/nonebot-adapter-villa) NoneBot2的大别野Bot适配器。
 
 推荐有成熟Python开发经验但对NoneBot2不熟悉的小伙伴选择`本SDK`，
```

