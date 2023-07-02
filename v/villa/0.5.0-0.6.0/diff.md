# Comparing `tmp/villa-0.5.0.tar.gz` & `tmp/villa-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.5.0.tar", max compression
+gzip compressed data, was "villa-0.6.0.tar", max compression
```

## Comparing `villa-0.5.0.tar` & `villa-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-06-30 14:59:51.787095 villa-0.5.0/LICENSE
--rw-r--r--   0        0        0     3428 2023-06-30 14:59:51.787095 villa-0.5.0/README.md
--rw-r--r--   0        0        0     1034 2023-06-30 14:59:51.787095 villa-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      285 2023-06-30 14:59:51.787095 villa-0.5.0/villa/__init__.py
--rw-r--r--   0        0        0    36288 2023-06-30 14:59:51.791095 villa-0.5.0/villa/bot.py
--rw-r--r--   0        0        0    10774 2023-06-30 14:59:51.791095 villa-0.5.0/villa/event.py
--rw-r--r--   0        0        0      728 2023-06-30 14:59:51.791095 villa-0.5.0/villa/exception.py
--rw-r--r--   0        0        0     3177 2023-06-30 14:59:51.791095 villa-0.5.0/villa/handle.py
--rw-r--r--   0        0        0     1524 2023-06-30 14:59:51.791095 villa-0.5.0/villa/log.py
--rw-r--r--   0        0        0    17127 2023-06-30 14:59:51.791095 villa-0.5.0/villa/message.py
--rw-r--r--   0        0        0     8899 2023-06-30 14:59:51.791095 villa-0.5.0/villa/models.py
--rw-r--r--   0        0        0      935 2023-06-30 14:59:51.791095 villa-0.5.0/villa/store.py
--rw-r--r--   0        0        0      240 2023-06-30 14:59:51.791095 villa-0.5.0/villa/typing.py
--rw-r--r--   0        0        0      995 2023-06-30 14:59:51.791095 villa-0.5.0/villa/utils.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 villa-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-02 12:00:40.831813 villa-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3428 2023-07-02 12:00:40.831813 villa-0.6.0/README.md
+-rw-r--r--   0        0        0     1034 2023-07-02 12:00:40.831813 villa-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-07-02 12:00:40.831813 villa-0.6.0/villa/__init__.py
+-rw-r--r--   0        0        0    36474 2023-07-02 12:00:40.831813 villa-0.6.0/villa/bot.py
+-rw-r--r--   0        0        0    10792 2023-07-02 12:00:40.831813 villa-0.6.0/villa/event.py
+-rw-r--r--   0        0        0      728 2023-07-02 12:00:40.835813 villa-0.6.0/villa/exception.py
+-rw-r--r--   0        0        0     3177 2023-07-02 12:00:40.835813 villa-0.6.0/villa/handle.py
+-rw-r--r--   0        0        0     1524 2023-07-02 12:00:40.835813 villa-0.6.0/villa/log.py
+-rw-r--r--   0        0        0    20754 2023-07-02 12:00:40.835813 villa-0.6.0/villa/message.py
+-rw-r--r--   0        0        0     9310 2023-07-02 12:00:40.835813 villa-0.6.0/villa/models.py
+-rw-r--r--   0        0        0      935 2023-07-02 12:00:40.835813 villa-0.6.0/villa/store.py
+-rw-r--r--   0        0        0      240 2023-07-02 12:00:40.835813 villa-0.6.0/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-07-02 12:00:40.835813 villa-0.6.0/villa/utils.py
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 villa-0.6.0/PKG-INFO
```

### Comparing `villa-0.5.0/LICENSE` & `villa-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.5.0/README.md` & `villa-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.5.0/pyproject.toml` & `villa-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.5.0"
+version = "0.6.0"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.5.0/villa/bot.py` & `villa-0.6.0/villa/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import asyncio
 from itertools import product
+from urllib.parse import urlparse
 from collections import defaultdict
 from typing import Any, Set, Dict, List, Type, Union, Literal, Optional, DefaultDict
 
 import httpx
 import uvicorn
 from pydantic import parse_obj_as
 from fastapi.responses import JSONResponse
@@ -14,15 +15,14 @@
 from .message import Message
 from .utils import escape_tag
 from .handle import EventHandler
 from .message import MessageSegment
 from .log import logger, _log_patcher
 from .typing import T_Func, T_Handler
 from .message import Link as LinkSegment
-from .message import Post as PostSegment
 from .message import Text as TextSegment
 from .message import Image as ImageSegment
 from .store import get_app, get_bot, store_bot
 from .message import RoomLink as RoomLinkSegment
 from .exception import ActionFailed, StopPropagation
 from .message import MentionAll as MentionAllSegment
 from .message import MentionUser as MentionUserSegment
@@ -36,38 +36,39 @@
     _event_handlers: DefaultDict[int, List[EventHandler]] = defaultdict(list)
     """事件处理函数"""
     _client: httpx.AsyncClient
     bot_id: str
     """机器人 Id"""
     bot_secret: str
     """机器人密钥"""
-    callback_url: str
+    callback_endpoint: Optional[str] = None
     """事件回调地址"""
     wait_util_complete: bool = False
     """是否等待事件处理全部完成后再响应"""
     _bot_info: Optional[Robot] = None
     """机器人信息"""
 
     def __init__(
         self,
         bot_id: str,
         bot_secret: str,
-        callback_url: str,
+        callback_url: Optional[str] = None,
         wait_util_complete: bool = False,
     ):
         """初始化一个 Bot 实例
 
         参数:
             bot_id: 机器人 ID
             bot_secret: 机器人密钥
             callback_url: 事件回调地址
         """
         self.bot_id = bot_id
         self.bot_secret = bot_secret
-        self.callback_url = callback_url
+        if callback_url is not None:
+            self.callback_endpoint = urlparse(callback_url).path
         self.wait_util_complete = wait_util_complete
         self._client = httpx.AsyncClient(
             base_url="https://bbs-api.miyoushe.com/vila/api/bot/platform/"
         )
         store_bot(self)
 
     @property
@@ -275,15 +276,15 @@
             room_id: 房间 ID
             message: 消息内容
 
         返回:
             str: 消息 ID
         """
         if isinstance(message, str):
-            message = MessageSegment.text(message)
+            message = MessageSegment.plain_text(message)
         if isinstance(message, MessageSegment):
             message = Message(message)
         content_info = await self._parse_message_content(message)
         if isinstance(content_info.content, TextMessageContent):
             object_name = "MHY:Text"
         elif isinstance(content_info.content, ImageMessageContent):
             object_name = "MHY:Image"
@@ -899,41 +900,44 @@
             )
 
     async def _parse_message_content(self, message: Message) -> MessageContentInfo:
         """解析消息内容"""
         if quote := message["quote", 0]:
             quote = QuoteInfo(**quote.dict())
 
+        if badge := message["badge", 0]:
+            badge = Badge(**badge.dict())
+
+        if preview_link := message["preview_link", 0]:
+            preview_link = PreviewLink(**preview_link.dict())
+
+        post = message["post", 0]
+
         if images_msg := (message["image"] or None):  # type: ignore
             images_msg: List[ImageSegment]
             images = [
                 Image(
                     url=seg.url,
                     size=ImageSize(width=seg.width, height=seg.height)
                     if seg.width and seg.height
                     else None,
                     file_size=seg.file_size,
                 )
                 for seg in images_msg
             ]
         else:
             images = None
-        if posts_msg := (message["post"] or None):  # type: ignore
-            posts_msg: List[PostSegment]
-            post_ids = [seg.post_id for seg in posts_msg]
-        else:
-            post_ids = None
         cal_len = lambda x: len(x.encode("utf-16")) // 2 - 1
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         mentioned = MentionedInfo(type=MentionType.PART)
         for seg in message:  # type: ignore
             try:
-                if seg.type in ("quote", "image", "post"):
+                if seg.type in ("quote", "image", "post", "preview_link", "badge"):
                     continue
                 if isinstance(seg, TextSegment):
                     seg_text = seg.content
                     length = cal_len(seg_text)
                 elif isinstance(seg, MentionAllSegment):
                     seg_text = f"@{seg.show_text} "
                     length = cal_len(seg_text)
@@ -996,68 +1000,71 @@
                     seg: LinkSegment
                     seg_text = seg.show_text
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
-                            entity=Link(url=seg.url, show_text=seg.show_text),
+                            entity=Link(
+                                url=seg.url,
+                                show_text=seg.show_text,
+                                requires_bot_access_token=seg.requires_bot_access_token,
+                            ),
                         )
                     )
                 message_offset += length
                 message_text += seg_text
             except Exception as e:
                 logger.opt(exception=e).warning("error when parse message content")
 
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
 
         if not (message_text or entities):
             if images:
                 if len(images) > 1:
-                    logger.warning(
-                        "Sending multiple images in one message will not be visible on the web side!"
+                    content = TextMessageContent(
+                        text="\u200B",
+                        images=images,
+                        preview_link=preview_link,
+                        badge=badge,
                     )
-                    content = TextMessageContent(text="\u200B", images=images)
                 else:
                     content = ImageMessageContent(**images[0].dict())
-            elif post_ids:
-                if len(post_ids) > 1:
-                    logger.opt(colors=True).warning(
-                        f"Only support one post in one message, so use the last one <m>{post_ids[-1]}</m>!"
-                    )
-                content = PostMessageContent(post_id=post_ids[-1])
+            elif preview_link:
+                content = TextMessageContent(
+                    text="\u200B", preview_link=preview_link, badge=badge
+                )
+            elif post:
+                content = PostMessageContent(post_id=post.post_id)
             else:
                 raise ValueError("message content is empty")
         else:
-            if images and message_text:
-                logger.warning(
-                    "When a message is accompanied by text and image, image will not visible on the web side!"
-                )
-            if post_ids and message_text:
-                logger.warning(
-                    "When a message is accompanied by text and post, post will not visible!"
-                )
             content = TextMessageContent(
-                text=message_text, entities=entities, images=images
+                text=message_text,
+                entities=entities,
+                images=images,
+                preview_link=preview_link,
+                badge=badge,
             )
 
-        return MessageContentInfo(
-            content=content,
-            mentionedInfo=mentioned,
-            quote=quote,
-        )
+        return MessageContentInfo(content=content, mentionedInfo=mentioned, quote=quote)
 
     def init_app(self, app: FastAPI):
-        logger.opt(colors=True).info(f"Initializing Bot <m>{self.bot_id}</m>...")
-        logger.opt(colors=True).debug(
-            f"With Secret: <m>{self.bot_secret}</m> and Callback URL: <m>{self.callback_url}</m>"
-        )
-        app.post(self.callback_url, status_code=200)(handle_event)
-        app.on_event("shutdown")(self._close_client)
+        if self.callback_endpoint is not None:
+            logger.opt(colors=True).info(f"Initializing Bot <m>{self.bot_id}</m>...")
+            logger.opt(colors=True).debug(
+                f"With Secret: <m>{self.bot_secret}</m> and Callback Endpoint: <m>{self.callback_endpoint}</m>"
+            )
+            app.post(self.callback_endpoint, status_code=200)(handle_event)
+            app.on_event("shutdown")(self._close_client)
+        else:
+            logger.opt(colors=True).warning(
+                f"Bot <m>{self.bot_id}</m> missing callback url endpoint."
+            )
 
     def run(
         self,
         host: str = "127.0.0.1",
         port: int = 13350,
         log_level: str = "INFO",
         **kwargs,
```

### Comparing `villa-0.5.0/villa/event.py` & `villa-0.6.0/villa/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,26 +133,26 @@
                 )
             )
 
         content = msg_content_info["content"]
         text = content["text"]
         entities = content["entities"]
         if not entities:
-            return Message(MessageSegment.text(text))
+            return Message(MessageSegment.plain_text(text))
         text = text.encode("utf-16")
         last_offset: int = 0
         last_length: int = 0
         for entity in entities:
             end_offset: int = last_offset + last_length
             offset: int = entity["offset"]
             length: int = entity["length"]
             entity_detail = entity["entity"]
             if offset != end_offset:
                 msg.append(
-                    MessageSegment.text(
+                    MessageSegment.plain_text(
                         text[((end_offset + 1) * 2) : ((offset + 1) * 2)].decode(
                             "utf-16"
                         )
                     )
                 )
             entity_text = text[(offset + 1) * 2 : (offset + length + 1) * 2].decode(
                 "utf-16"
@@ -185,15 +185,15 @@
             else:
                 entity_detail["show_text"] = entity_text
                 msg.append(MessageSegment.link(entity_detail["url"], entity_text))
             last_offset = offset
             last_length = length
         end_offset = last_offset + last_length
         if last_text := text[(end_offset + 1) * 2 :].decode("utf-16"):
-            msg.append(MessageSegment.text(last_text))
+            msg.append(MessageSegment.plain_text(last_text))
         data["message"] = msg
         return data
 
     async def send(
         self,
         message: Union[str, MessageSegment, Message],
         mention_sender: bool = False,
```

### Comparing `villa-0.5.0/villa/exception.py` & `villa-0.6.0/villa/exception.py`

 * *Files identical despite different names*

### Comparing `villa-0.5.0/villa/handle.py` & `villa-0.6.0/villa/handle.py`

 * *Files identical despite different names*

### Comparing `villa-0.5.0/villa/log.py` & `villa-0.6.0/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.5.0/villa/message.py` & `villa-0.6.0/villa/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import re
 from abc import ABC
 from typing_extensions import Self
 from typing import List, Tuple, Union, Literal, Iterable, Iterator, Optional, overload
 
 from pydantic import Field, BaseModel
+from pydantic.utils import get_args  # type: ignore
 
 MessageType = Literal[
     "text",
     "mention_user",
     "mention_all",
     "mention_robot",
     "room_link",
     "link",
     "image",
     "quote",
     "post",
+    "preview_link",
+    "badge",
 ]
 
 
 class MessageSegment(ABC, BaseModel):
     type: MessageType
     """消息段基类"""
 
     @staticmethod
-    def text(text: str) -> "Text":
+    def plain_text(text: str) -> "Text":
         return Text(content=text)
 
     @staticmethod
     def mention_robot(bot_id: str, bot_name: str) -> "MentionRobot":
         return MentionRobot(bot_id=bot_id, bot_name=bot_name)
 
     @staticmethod
@@ -39,16 +42,24 @@
         return MentionAll(show_text=show_text)
 
     @staticmethod
     def room_link(villa_id: int, room_id: int) -> "RoomLink":
         return RoomLink(villa_id=villa_id, room_id=room_id)
 
     @staticmethod
-    def link(url: str, show_text: Optional[str] = None) -> "Link":
-        return Link(url=url, show_text=show_text or url)
+    def link(
+        url: str,
+        show_text: Optional[str] = None,
+        requires_bot_access_token: bool = False,
+    ) -> "Link":
+        return Link(
+            url=url,
+            show_text=show_text or url,
+            requires_bot_access_token=requires_bot_access_token,
+        )
 
     @staticmethod
     def post(post_id: str) -> "Post":
         return Post(post_id=post_id)
 
     @staticmethod
     def image(
@@ -64,17 +75,41 @@
         return Quote(
             quoted_message_id=message_id,
             quoted_message_send_time=message_send_time,
             original_message_id=message_id,
             original_message_send_time=message_send_time,
         )
 
+    @staticmethod
+    def preview_link(
+        icon_url: str,
+        image_url: str,
+        is_internal_link: bool,
+        title: str,
+        content: str,
+        url: str,
+        source_name: str,
+    ) -> "PreviewLink":
+        return PreviewLink(
+            icon_url=icon_url,
+            image_url=image_url,
+            is_internal_link=is_internal_link,
+            title=title,
+            content=content,
+            url=url,
+            source_name=source_name,
+        )
+
+    @staticmethod
+    def badge(icon_url: str, text: str, url: str) -> "Badge":
+        return Badge(icon_url=icon_url, text=text, url=url)
+
     def __add__(self, other: Union[str, "MessageSegment", "Message"]) -> "Message":
         if isinstance(other, str):
-            return Message([self, MessageSegment.text(other)])
+            return Message([self, MessageSegment.plain_text(other)])
         elif isinstance(other, MessageSegment):
             return Message([self, other])
         elif isinstance(other, Message):
             return Message([self, *other.__root__])
         else:
             raise TypeError(f"unsupported type: {type(other)}")
 
@@ -125,14 +160,15 @@
 
 class Link(MessageSegment):
     """链接消息段"""
 
     type: Literal["link"] = Field(default="link", repr=False)
     url: str
     show_text: str
+    requires_bot_access_token: bool
 
 
 class Image(MessageSegment):
     """图片消息段"""
 
     type: Literal["image"] = Field(default="image", repr=False)
     url: str
@@ -154,14 +190,38 @@
 class Post(MessageSegment):
     """帖子消息段"""
 
     type: Literal["post"] = Field(default="post", repr=False)
     post_id: str
 
 
+class PreviewLink(MessageSegment):
+    """预览链接(卡片)消息段"""
+
+    type: Literal["preview_link"] = Field(default="preview_link", repr=False)
+    icon_url: str
+    image_url: str
+    is_internal_link: bool
+    title: str
+    content: str
+    url: str
+    source_name: str
+
+
+class Badge(MessageSegment):
+    """徽标消息段
+
+    用于在消息下方显示徽标，不支持单独发送"""
+
+    type: Literal["badge"] = Field(default="badge", repr=False)
+    icon_url: str
+    text: str
+    url: str
+
+
 class Message(BaseModel):
     __root__: List[MessageSegment] = Field(default_factory=list)
 
     def __init__(
         self,
         message: Union[
             str, MessageSegment, Iterable[MessageSegment], "Message", None
@@ -183,15 +243,15 @@
             message = [message]
         elif isinstance(message, Message):
             message = message.__root__
         elif not isinstance(message, Iterable):
             raise TypeError(f"unsupported type: {type(message)}")
         super().__init__(__root__=message)
 
-    def text(self, content: str) -> Self:
+    def plain_text(self, content: str) -> Self:
         """纯文本消息
 
         参数:
             content: 文本内容
 
         返回:
             Self: 消息对象
@@ -248,27 +308,39 @@
 
         返回:
             Self: 消息对象
         """
         self.__root__.append(RoomLink(villa_id=villa_id, room_id=room_id))
         return self
 
-    def link(self, url: str, show_text: Optional[str] = None) -> Self:
+    def link(
+        self,
+        url: str,
+        show_text: Optional[str] = None,
+        requires_bot_access_token: bool = False,
+    ) -> Self:
         """说明
 
         详细说明
 
         参数:
-            url: 参数说明
-            text: 参数说明. 默认为 None.
+            url: 链接地址
+            show_text: 链接显示的文本. 为 None 时与地址保持一致.
+            requires_bot_access_token: 访问时是否需要带上含有用户信息的token. 默认为 False.
 
         返回:
             Self: 返回说明
         """
-        self.__root__.append(Link(url=url, show_text=show_text or url))
+        self.__root__.append(
+            Link(
+                url=url,
+                show_text=show_text or url,
+                requires_bot_access_token=requires_bot_access_token,
+            )
+        )
         return self
 
     def image(
         self,
         url: str,
         width: Optional[int] = None,
         height: Optional[int] = None,
@@ -318,14 +390,55 @@
 
         返回:
             Self: 消息对象
         """
         self.__root__.append(Post(post_id=post_id))
         return self
 
+    def preview_link(
+        self,
+        icon_url: str,
+        image_url: str,
+        is_internal_link: bool,
+        title: str,
+        content: str,
+        url: str,
+        source_name: str,
+    ) -> Self:
+        """预览链接(卡片)消息
+
+        参数:
+            icon_url: 参数说明
+            image_url: 参数说明
+            is_internal_link: 参数说明
+            title: 参数说明
+            content: 参数说明
+            url: 参数说明
+            source_name: 参数说明
+
+        返回:
+            Self: 返回说明
+        """
+        self.__root__.append(
+            PreviewLink(
+                icon_url=icon_url,
+                image_url=image_url,
+                is_internal_link=is_internal_link,
+                title=title,
+                content=content,
+                url=url,
+                source_name=source_name,
+            )
+        )
+        return self
+
+    def badge(self, icon_url: str, text: str, url: str) -> Self:
+        self.__root__.append(Badge(icon_url=icon_url, text=text, url=url))
+        return self
+
     def insert(self, index: int, segment: Union[str, MessageSegment]):
         """在指定位置插入消息段
 
         参数:
             index: 插入位置
             segment: 消息段
 
@@ -345,23 +458,23 @@
         返回:
             Self: 消息对象
         """
         if isinstance(segment, str):
             segment = Text(content=segment)
         self.__root__.append(segment)
 
-    def plain_text(self) -> str:
+    def get_plain_text(self) -> str:
         """获取纯文本消息内容"""
         return "".join(
             [segment.content for segment in self.__root__ if isinstance(segment, Text)]
         )
 
     def __contains__(self, item: str) -> bool:
         """检查消息的纯文本内容是否包含指定字符串"""
-        return item in self.plain_text()
+        return item in self.get_plain_text()
 
     def __len__(self) -> int:
         return len(self.__root__)
 
     def __add__(self, other: Union[str, "MessageSegment", "Message"]) -> "Message":
         result = self.copy(deep=True)
         if isinstance(other, str):
@@ -410,48 +523,48 @@
 
         参数:
             text: 指定字符串
 
         返回:
             bool: 是否以指定字符串开头
         """
-        return self.plain_text().startswith(text)
+        return self.get_plain_text().startswith(text)
 
     def endswith(self, text: Union[str, Tuple[str, ...]]) -> bool:
         """判断消息的纯文本部分是否以指定字符串结尾
 
         参数:
             text: 指定字符串
 
         返回:
             bool: 是否以指定字符串结尾
         """
-        return self.plain_text().endswith(text)
+        return self.get_plain_text().endswith(text)
 
     def match(self, pattern: Union[str, re.Pattern]) -> Optional[re.Match]:
         """使用正则表达式匹配消息的纯文本部分
 
         参数:
             pattern: 正则表达式
 
         返回:
             Optional[re.Match]: 匹配结果
         """
-        return re.match(pattern, self.plain_text())
+        return re.match(pattern, self.get_plain_text())
 
     def search(self, pattern: Union[str, re.Pattern]) -> Optional[re.Match]:
         """使用正则表达式搜索消息的纯文本部分
 
         参数:
             pattern: 正则表达式
 
         返回:
             Optional[re.Match]: 匹配结果
         """
-        return re.search(pattern, self.plain_text())
+        return re.search(pattern, self.get_plain_text())
 
     @overload
     def __getitem__(self, __args: int) -> MessageSegment:
         """
         参数:
             __args: 索引
 
@@ -496,123 +609,148 @@
     @overload
     def __getitem__(self, __args: Tuple[Literal["text"], int]) -> Optional[Text]:
         """
         参数:
             __args: text消息段
 
         返回:
-            Message: 消息段类型为text的第 `__args[1]` 个消息段
+            Text: 消息段类型为text的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
         self, __args: Tuple[Literal["mention_user"], int]
     ) -> Optional[MentionUser]:
         """
         参数:
             __args: mention_user消息段
 
         返回:
-            Message: 消息段类型为mention_user的第 `__args[1]` 个消息段
+            MentionUser: 消息段类型为mention_user的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
         self, __args: Tuple[Literal["mention_all"], int]
     ) -> Optional[MentionAll]:
         """
         参数:
             __args: mention_all消息段
 
         返回:
-            Message: 消息段类型为mention_all的第 `__args[1]` 个消息段
+            MentionAll: 消息段类型为mention_all的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
         self, __args: Tuple[Literal["mention_robot"], int]
     ) -> Optional[MentionRobot]:
         """
         参数:
             __args: mention_robot消息段
 
         返回:
-            Message: 消息段类型为mention_robot的第 `__args[1]` 个消息段
+            MentionRobot: 消息段类型为mention_robot的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
         self, __args: Tuple[Literal["room_link"], int]
     ) -> Optional[RoomLink]:
         """
         参数:
             __args: room_link消息段
 
         返回:
-            Message: 消息段类型为room_link的第 `__args[1]` 个消息段
+            RoomLink: 消息段类型为room_link的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(self, __args: Tuple[Literal["link"], int]) -> Optional[Link]:
         """
         参数:
             __args: link消息段
 
         返回:
-            Message: 消息段类型为link的第 `__args[1]` 个消息段
+            Link: 消息段类型为link的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(self, __args: Tuple[Literal["image"], int]) -> Optional[Image]:
         """
         参数:
             __args: image消息段
 
         返回:
-            Message: 消息段类型为image的第 `__args[1]` 个消息段
+            Image: 消息段类型为image的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(self, __args: Tuple[Literal["quote"], int]) -> Optional[Quote]:
         """
         参数:
             __args: quote消息段
 
         返回:
-            Message: 消息段类型为quote的第 `__args[1]` 个消息段
+            Quote: 消息段类型为quote的第 `__args[1]` 个消息段
+        """
+        ...
+
+    @overload
+    def __getitem__(self, __args: Tuple[Literal["post"], int]) -> Optional[Post]:
+        """
+        参数:
+            __args: post消息段
+
+        返回:
+            Post: 消息段类型为post的第 `__args[1]` 个消息段
+        """
+        ...
+
+    @overload
+    def __getitem__(
+        self, __args: Tuple[Literal["preview_link"], int]
+    ) -> Optional[PreviewLink]:
+        """
+        参数:
+            __args: preview_link消息段
+
+        返回:
+            PreviewLink: 消息段类型为preview_link的第 `__args[1]` 个消息段
+        """
+        ...
+
+    @overload
+    def __getitem__(self, __args: Tuple[Literal["badge"], int]) -> Optional[Badge]:
+        """
+        参数:
+            __args: badge消息段
+
+        返回:
+            Badge: 消息段类型为badge的第 `__args[1]` 个消息段
         """
         ...
 
     def __getitem__(
         self,
         args: Union[int, slice, MessageType, Tuple[MessageType, Union[int, slice]]],
     ) -> Union[MessageSegment, "Message", None]:
         arg1, arg2 = args if isinstance(args, tuple) else (args, None)
         if isinstance(arg1, int) and arg2 is None:
             return self.__root__.__getitem__(arg1)
         elif isinstance(arg1, slice) and arg2 is None:
             return Message(self.__root__.__getitem__(arg1))
-        elif isinstance(arg1, str) and arg1 in (
-            "text",
-            "mention_user",
-            "mention_all",
-            "mention_robot",
-            "room_link",
-            "link",
-            "image",
-            "quote",
-            "post",
-        ):
+        elif isinstance(arg1, str) and arg1 in get_args(MessageType):  # type: ignore
             if arg2 is None:
                 return Message([seg for seg in self.__root__ if seg.type == arg1])
             elif isinstance(arg2, int):
                 try:
                     return [seg for seg in self.__root__ if seg.type == arg1][arg2]
                 except IndexError:
                     return None
```

### Comparing `villa-0.5.0/villa/models.py` & `villa-0.6.0/villa/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import json
 import inspect
 from enum import Enum, IntEnum
-from typing import Any, List, Union, Literal, Optional
+from typing import Any, Dict, List, Union, Literal, Optional
 
 from pydantic import Field, BaseModel, validator
 
 
 class ApiResponse(BaseModel):
     retcode: int
     message: str
@@ -124,14 +124,15 @@
 
     room_name: str = Field(exclude=True)
 
 
 class Link(BaseModel):
     type: Literal["link"] = "link"
     url: str
+    requires_bot_access_token: bool
 
     show_text: str = Field(exclude=True)
 
 
 class TextEntity(BaseModel):
     offset: int
     length: int
@@ -145,14 +146,30 @@
 
 class Image(BaseModel):
     url: str
     size: Optional[ImageSize] = None
     file_size: Optional[int] = None
 
 
+class PreviewLink(BaseModel):
+    icon_url: str
+    image_url: str
+    is_internal_link: bool
+    title: str
+    content: str
+    url: str
+    source_name: str
+
+
+class Badge(BaseModel):
+    icon_url: str
+    text: str
+    url: str
+
+
 class PostMessageContent(BaseModel):
     post_id: str
 
     @validator("post_id")
     def __deal_post_id(cls, v: str):
         s = v.split("/")[-1]
         if s.isdigit():
@@ -160,14 +177,16 @@
         raise ValueError(f"Invalid post_id: {v}, post_id must be a number.")
 
 
 class TextMessageContent(BaseModel):
     text: str
     entities: List[TextEntity] = Field(default_factory=list)
     images: Optional[List[Image]] = None
+    preview_link: Optional[PreviewLink] = None
+    badge: Optional[Badge] = None
 
 
 class ImageMessageContent(Image):
     pass
 
 
 class MentionedInfo(BaseModel):
@@ -180,15 +199,15 @@
     quoted_message_send_time: int
     original_message_id: str
     original_message_send_time: int
 
 
 class User(BaseModel):
     portrait_uri: str = Field(alias="portraitUri")
-    extra: dict
+    extra: Dict[str, Any]
     name: str
     alias: str
     id: str
     portrait: str
 
     @validator("extra", pre=True)
     def extra_str_to_dict(cls, v: Any):
@@ -199,14 +218,15 @@
 
 class Trace(BaseModel):
     visual_room_version: str
     app_version: str
     action_type: int
     bot_msg_id: str
     client: str
+    env: str
     rong_sdk_version: str
 
 
 class MessageContentInfo(BaseModel):
     content: Union[TextMessageContent, ImageMessageContent, PostMessageContent]
     mentioned_info: Optional[MentionedInfo] = Field(None, alias="mentionedInfo")
     quote: Optional[QuoteInfo] = None
@@ -404,14 +424,16 @@
     "PostMessageContent",
     "MentionedInfo",
     "QuoteInfo",
     "User",
     "Trace",
     "ImageSize",
     "Image",
+    "PreviewLink",
+    "Badge",
     "MessageContentInfo",
     "Room",
     "RoomType",
     "RoomDefaultNotifyType",
     "SendMsgAuthRange",
     "GroupRoom",
     "ListRoomType",
```

### Comparing `villa-0.5.0/villa/store.py` & `villa-0.6.0/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.5.0/villa/utils.py` & `villa-0.6.0/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.5.0/PKG-INFO` & `villa-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.5.0
+Version: 0.6.0
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

