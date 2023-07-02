# Comparing `tmp/nonebot_adapter_villa-0.4.2.tar.gz` & `tmp/nonebot_adapter_villa-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.4.2.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.5.0.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.4.2.tar` & `nonebot_adapter_villa-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/LICENSE
--rw-r--r--   0        0        0     4938 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/README.md
--rw-r--r--   0        0        0      235 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    10977 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     8899 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    12770 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      649 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11641 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     6704 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-07-01 11:33:11.791100 nonebot_adapter_villa-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6796 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/README.md
+-rw-r--r--   0        0        0      235 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    10977 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9465 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    13057 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      649 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11641 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0    10115 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-07-02 12:15:29.722046 nonebot_adapter_villa-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.0/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.4.2/LICENSE` & `nonebot_adapter_villa-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/cilent.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/models.py`

 * *Files 4% similar despite different names*

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
@@ -94,44 +94,45 @@
     PART = 2
 
     def __repr__(self) -> str:
         return self.name
 
 
 class MentionedRobot(BaseModel):
-    type: Literal["mentioned_robot"] = "mentioned_robot"
+    type: Literal["mentioned_robot"] = Field(default="mentioned_robot", repr=False)
     bot_id: str
 
     bot_name: str = Field(exclude=True)
 
 
 class MentionedUser(BaseModel):
-    type: Literal["mentioned_user"] = "mentioned_user"
+    type: Literal["mentioned_user"] = Field(default="mentioned_user", repr=False)
     user_id: str
 
-    user_name: str = Field(exclude=True)
+    user_name: Optional[str] = Field(exclude=True)
 
 
 class MentionedAll(BaseModel):
-    type: Literal["mention_all"] = "mention_all"
+    type: Literal["mention_all"] = Field(default="mention_all", repr=False)
 
     show_text: str = Field(exclude=True)
 
 
 class VillaRoomLink(BaseModel):
-    type: Literal["villa_room_link"] = "villa_room_link"
+    type: Literal["villa_room_link"] = Field(default="villa_room_link", repr=False)
     villa_id: str
     room_id: str
 
-    room_name: str = Field(exclude=True)
+    room_name: Optional[str] = Field(exclude=True)
 
 
 class Link(BaseModel):
-    type: Literal["link"] = "link"
+    type: Literal["link"] = Field(default="link", repr=False)
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

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from nonebot.adapters import Bot as BaseBot
 
 from .utils import log
 from .event import Event, SendMessageEvent
 from .message import Message, MessageSegment
 from .api import (
     Link,
+    Badge,
     Image,
     Robot,
     Command,
     ApiClient,
-    ImageSize,
     QuoteInfo,
     TextEntity,
     MentionType,
+    PreviewLink,
     MentionedAll,
     MentionedInfo,
     MentionedUser,
     VillaRoomLink,
     MentionedRobot,
     MessageContentInfo,
     PostMessageContent,
@@ -58,16 +59,16 @@
         event.content.mentioned_info
         and bot.self_id in event.content.mentioned_info.user_id_list
     ):
         event.to_me = True
 
     def _is_at_me_seg(segment: MessageSegment) -> bool:
         return (
-            segment.type == "mentioned_robot"
-            and segment.data.get("bot_id") == bot.self_id
+            segment.type == "mention_robot"
+            and segment.data["mention_robot"].bot_id == bot.self_id
         )
 
     message = event.get_message()
     if not message:
         message.append(MessageSegment.text(""))
 
     deleted = False
@@ -198,15 +199,20 @@
         """
         if not isinstance(event, SendMessageEvent):
             raise RuntimeError("Event cannot be replied to!")
         message = MessageSegment.text(message) if isinstance(message, str) else message
         message = message if isinstance(message, Message) else Message(message)
         if mention_sender:
             message.insert(
-                0, MessageSegment.mention_user(event.villa_id, event.from_user_id)
+                0,
+                MessageSegment.mention_user(
+                    user_id=event.from_user_id,
+                    user_name=event.content.user.name if event.content.user else None,
+                    villa_id=event.villa_id,
+                ),
             )
         if quote_message:
             message += MessageSegment.quote(event.msg_uid, event.send_at)
         content_info = await self.parse_message_content(message)
         if isinstance(content_info.content, TextMessageContent):
             object_name = "MHY:Text"
         elif isinstance(content_info.content, ImageMessageContent):
@@ -225,144 +231,146 @@
 
         参数:
             message: 消息
 
         返回:
             MessageContentInfo: 消息内容对象
         """
-        if quote := (message["quote"] or None):
-            quote = quote[-1]
-            quote = QuoteInfo(
-                quoted_message_id=quote.data["msg_id"],
-                quoted_message_send_time=quote.data["msg_send_time"],
-                original_message_id=quote.data["msg_id"],
-                original_message_send_time=quote.data["msg_send_time"],
-            )
-        if images_msg := (message["image"] or None):
-            images = [
-                Image(
-                    url=seg.data["url"],
-                    size=ImageSize(width=seg.data["width"], height=seg.data["height"])
-                    if seg.data["width"] and seg.data["height"]
-                    else None,
-                    file_size=seg.data["file_size"],
-                )
-                for seg in images_msg
+        if quote_seg := message["quote"]:
+            quote: Optional[QuoteInfo] = quote_seg[-1].data["quote"]
+        else:
+            quote = None
+        if images_seg := message["image"]:
+            images: Optional[List[Image]] = [
+                image.data["image"] for image in images_seg
             ]
         else:
             images = None
-        if posts_msg := (message["post"] or None):
-            post_ids: Optional[List[str]] = [seg.data["post_id"] for seg in posts_msg]
+        if post_seg := message["post"]:
+            post: Optional[PostMessageContent] = post_seg[-1].data["post"]
+        else:
+            post = None
+        if badge_seg := message["badge"]:
+            badge: Optional[Badge] = badge_seg[-1].data["badge"]
+        else:
+            badge = None
+        if preview_link_seg := message["preview_link"]:
+            preview_link: Optional[PreviewLink] = preview_link_seg[-1].data[
+                "preview_link"
+            ]
         else:
-            post_ids = None
+            preview_link = None
+
         cal_len = lambda x: len(x.encode("utf-16")) // 2 - 1
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         mentioned = MentionedInfo(type=MentionType.PART)
         for seg in message:
             try:
-                if seg.type in ("quote", "image", "post"):
+                if seg.type in ("quote", "image", "post", "badge", "preview_link"):
                     continue
                 if seg.type == "text":
                     seg_text = seg.data["text"]
                     length = cal_len(seg_text)
                 elif seg.type == "mention_all":
-                    seg_text = f"@{seg.data['show_text']} "
+                    mention_all: MentionedAll = seg.data["mention_all"]
+                    seg_text = f"@{mention_all.show_text} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
-                            entity=MentionedAll(show_text=seg.data["show_text"]),
+                            entity=mention_all,
                         )
                     )
                     mentioned.type = MentionType.ALL
-                elif seg.type == "mentioned_robot":
-                    seg_text = f"@{seg.data['bot_name']} "
+                elif seg.type == "mention_robot":
+                    mention_robot: MentionedRobot = seg.data["mention_robot"]
+                    seg_text = f"@{mention_robot.bot_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
-                            offset=message_offset,
-                            length=length,
-                            entity=MentionedRobot(
-                                bot_id=seg.data["bot_id"], bot_name=seg.data["bot_name"]
-                            ),
+                            offset=message_offset, length=length, entity=mention_robot
                         )
                     )
-                    mentioned.user_id_list.append(seg.data["bot_id"])
-                elif seg.type == "mentioned_user":
-                    # 需要调用API获取被@的用户的昵称
-                    user = await self.get_member(
-                        villa_id=seg.data["villa_id"], uid=seg.data["user_id"]
-                    )
-                    seg_text = f"@{user.basic.nickname} "
+                    mentioned.user_id_list.append(mention_robot.bot_id)
+                elif seg.type == "mention_user":
+                    mention_user: MentionedUser = seg.data["mention_user"]
+                    if mention_user.user_name is None:
+                        # 需要调用API获取被@的用户的昵称
+                        user = await self.get_member(
+                            villa_id=seg.data["villa_id"], uid=int(mention_user.user_id)
+                        )
+                        seg_text = f"@{user.basic.nickname} "
+                        mention_user.user_name = user.basic.nickname
+                    else:
+                        seg_text = f"@{mention_user.user_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
-                            offset=message_offset,
-                            length=length,
-                            entity=MentionedUser(
-                                user_id=str(user.basic.uid),
-                                user_name=user.basic.nickname,
-                            ),
+                            offset=message_offset, length=length, entity=mention_user
                         )
                     )
-                    mentioned.user_id_list.append(str(user.basic.uid))
-                elif seg.type == "villa_room_link":
-                    # 需要调用API获取房间的名称
-                    room = await self.get_room(
-                        villa_id=seg.data["villa_id"], room_id=seg.data["room_id"]
-                    )
-                    seg_text = f"#{room.room_name} "
+                    mentioned.user_id_list.append(str(mention_user.user_id))
+                elif seg.type == "room_link":
+                    room_link: VillaRoomLink = seg.data["room_link"]
+                    if room_link.room_name is None:
+                        # 需要调用API获取房间的名称
+                        room = await self.get_room(
+                            villa_id=int(room_link.villa_id),
+                            room_id=int(room_link.room_id),
+                        )
+                        seg_text = f"#{room.room_name} "
+                        room_link.room_name = room.room_name
+                    else:
+                        seg_text = f"#{room_link.room_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
-                            offset=message_offset,
-                            length=length,
-                            entity=VillaRoomLink(
-                                villa_id=str(seg.data["villa_id"]),
-                                room_id=str(seg.data["room_id"]),
-                                room_name=room.room_name,
-                            ),
+                            offset=message_offset, length=length, entity=room_link
                         )
                     )
                 else:
-                    seg_text = seg.data["show_text"]
+                    link: Link = seg.data["link"]
+                    seg_text = link.show_text
                     length = cal_len(seg_text)
                     entities.append(
-                        TextEntity(
-                            offset=message_offset,
-                            length=length,
-                            entity=Link(
-                                url=seg.data["url"], show_text=seg.data["show_text"]
-                            ),
-                        )
+                        TextEntity(offset=message_offset, length=length, entity=link)
                     )
                 message_offset += length
                 message_text += seg_text
             except Exception as e:
                 log("WARNING", "error when parse message content", e)
 
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
 
         if not (message_text or entities):
             if images:
                 if len(images) > 1:
-                    content = TextMessageContent(text="\u200B", images=images)
+                    content = TextMessageContent(
+                        text="\u200B",
+                        images=images,
+                        preview_link=preview_link,
+                        badge=badge,
+                    )
                 else:
                     content = ImageMessageContent(**images[-1].dict())
-            elif post_ids:
-                content = PostMessageContent(post_id=post_ids[-1])
+            elif preview_link:
+                content = TextMessageContent(
+                    text="\u200B", preview_link=preview_link, badge=badge
+                )
+            elif post:
+                content = post
             else:
                 raise ValueError("message content is empty")
         else:
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
-            quote=quote,  # type: ignore
-        )
+        return MessageContentInfo(content=content, mentionedInfo=mentioned, quote=quote)
```

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.4.2/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.5.0/nonebot/adapters/villa/message.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 
 from nonebot.adapters import Message as BaseMessage
 from nonebot.adapters import MessageSegment as BaseMessageSegment
 
+from .api.models import *
+
 
 class MessageSegment(BaseMessageSegment["Message"]):
     @classmethod
     @overrides(BaseMessageSegment)
     def get_message_class(cls) -> Type["Message"]:
         return Message
 
     @overrides(BaseMessageSegment)
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    @overrides(BaseMessageSegment)
     def __add__(
         self, other: Union[str, "MessageSegment", Iterable["MessageSegment"]]
     ) -> "Message":
         return super().__add__(other)
 
     @overrides(BaseMessageSegment)
     def __radd__(
@@ -49,78 +55,129 @@
             bot_id: 机器人ID
             bot_name: 机器人的名字
 
         返回:
             MentionRobotSegement: 消息段对象
         """
         return MentionRobotSegement(
-            "mentioned_robot", {"bot_id": bot_id, "bot_name": bot_name}
+            "mention_robot",
+            {"mention_robot": MentionedRobot(bot_id=bot_id, bot_name=bot_name)},
         )
 
     @staticmethod
-    def mention_user(villa_id: int, user_id: int) -> "MentionUserSegement":
+    def mention_user(
+        user_id: int, user_name: Optional[str] = None, villa_id: Optional[int] = None
+    ) -> "MentionUserSegement":
         """@用户消息段
 
+        user_name和villa_id必须有其中之一
+
         参数:
-            villa_id: 用户所在大别野ID
             user_id: 用户ID
+            user_name: 用户名称
+            villa_id: 用户所在大别野ID
 
         返回:
             MentionUserSegement: 消息段对象
         """
+        if not (user_name or villa_id):
+            raise ValueError("user_name and villa_id must have one of them")
         return MentionUserSegement(
-            "mentioned_user", {"villa_id": villa_id, "user_id": user_id}
+            "mention_user",
+            {
+                "mention_user": MentionedUser(
+                    user_id=str(user_id), user_name=user_name
+                ),
+                "villa_id": villa_id,
+            },
         )
 
     @staticmethod
     def mention_all(show_text: str = "全体成员") -> "MentionAllSegement":
-        """@全体成员消息段"""
-        return MentionAllSegement("mention_all", {"show_text": show_text})
+        """@全体成员消息段
+
+        参数:
+            show_text: 展示文本. 默认为 "全体成员".
+
+        返回:
+            MentionAllSegement: 消息段对象
+        """
+        return MentionAllSegement(
+            "mention_all", {"mention_all": MentionedAll(show_text=show_text)}
+        )
 
     @staticmethod
-    def room_link(villa_id: int, room_id: int) -> "RoomLinkSegment":
+    def room_link(
+        villa_id: int, room_id: int, room_name: Optional[str] = None
+    ) -> "RoomLinkSegment":
         """房间链接消息段，点击后可以跳转到指定房间
 
         参数:
             villa_id: 大别野ID
             room_id: 房间ID
 
         返回:
             VillaRoomLinkSegment: 消息段对象
         """
         return RoomLinkSegment(
-            "villa_room_link", {"villa_id": villa_id, "room_id": room_id}
+            "room_link",
+            {
+                "room_link": VillaRoomLink(
+                    villa_id=str(villa_id), room_id=str(room_id), room_name=room_name
+                )
+            },
         )
 
     @staticmethod
-    def link(url: str, show_text: Optional[str] = None) -> "LinkSegment":
+    def link(
+        url: str,
+        show_text: Optional[str] = None,
+        requires_bot_access_token: bool = False,
+    ) -> "LinkSegment":
         """链接消息段，使用该消息段才能让链接可以直接点击进行跳转
 
         参数:
             url: 链接
             show_text: 链接显示的文本
 
         返回:
             LinkSegment: 消息段对象
         """
-        return LinkSegment("link", {"url": url, "show_text": show_text or url})
+        return LinkSegment(
+            "link",
+            {
+                "link": Link(
+                    url=url,
+                    show_text=show_text or url,
+                    requires_bot_access_token=requires_bot_access_token,
+                )
+            },
+        )
 
     @staticmethod
     def quote(message_id: str, message_send_time: int) -> "QuoteSegment":
         """引用(回复)消息段
 
         参数:
             message_id: 被引用的消息ID
             message_send_time: 被引用的消息发送时间
 
         返回:
             QuoteSegment: 消息段对象
         """
         return QuoteSegment(
-            "quote", {"msg_id": message_id, "msg_send_time": message_send_time}
+            "quote",
+            {
+                "quote": QuoteInfo(
+                    quoted_message_id=message_id,
+                    quoted_message_send_time=message_send_time,
+                    original_message_id=message_id,
+                    original_message_send_time=message_send_time,
+                )
+            },
         )
 
     @staticmethod
     def image(
         url: str,
         width: Optional[int] = None,
         height: Optional[int] = None,
@@ -135,82 +192,168 @@
             file_size: 图片大小
 
         返回:
             ImageSegment: 消息段对象
         """
         return ImageSegment(
             "image",
-            {"url": url, "width": width, "height": height, "file_size": file_size},
+            {
+                "image": Image(
+                    url=url,
+                    size=ImageSize(width=width, height=height)
+                    if width and height
+                    else None,
+                    file_size=file_size,
+                )
+            },
         )
 
     @staticmethod
     def post(post_id: str) -> "PostSegment":
         """帖子转发消息段
 
         参数:
             post_id: 帖子ID
 
         返回:
             PostSegment: 消息段对象
         """
-        return PostSegment("post", {"post_id": post_id})
+        return PostSegment("post", {"post": PostMessageContent(post_id=post_id)})
+
+    @staticmethod
+    def preview_link(
+        icon_url: str,
+        image_url: str,
+        is_internal_link: bool,
+        title: str,
+        content: str,
+        url: str,
+        source_name: str,
+    ) -> "PreviewLinkSegment":
+        """预览链接(卡片)消息段
+
+        参数:
+            icon_url: 图标链接
+            image_url: 封面链接
+            is_internal_link: 是否为官方
+            title: 标题
+            content: 内容
+            url: 链接
+            source_name: 来源
+
+        返回:
+            PreviewLinkSegment: 消息段对象
+        """
+        return PreviewLinkSegment(
+            "preview_link",
+            {
+                "preview_link": PreviewLink(
+                    icon_url=icon_url,
+                    image_url=image_url,
+                    is_internal_link=is_internal_link,
+                    title=title,
+                    content=content,
+                    url=url,
+                    source_name=source_name,
+                )
+            },
+        )
+
+    @staticmethod
+    def badge(
+        icon_url: str,
+        text: str,
+        url: str,
+    ) -> "BadgeSegment":
+        """消息下方徽标
+
+        参数:
+            icon_url: 图标链接
+            text: 文本
+            url: 链接
+
+        返回:
+            BadgeSegment: 消息段对象
+        """
+        return BadgeSegment(
+            "badge",
+            {
+                "badge": Badge(
+                    icon_url=icon_url,
+                    text=text,
+                    url=url,
+                )
+            },
+        )
 
 
 class TextSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
         return escape_tag(self.data["text"])
 
 
 class MentionRobotSegement(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"<MentionRobot:bot_id={self.data['bot_id']} bot_name={self.data['bot_name']}>"
+        return repr(self.data["mention_robot"])
 
 
 class MentionUserSegement(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"<MentionUser:user_id={self.data['user_id']}>"
+        return repr(self.data["mention_user"])
 
 
 class MentionAllSegement(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"<MentionAll:show_text={self.data['show_text']}>"
+        return repr(self.data["mention_all"])
 
 
 class RoomLinkSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"<RoomLink:villa_id={self.data['villa_id']} room_id={self.data['room_id']}>"
+        return repr(self.data["room_link"])
 
 
 class LinkSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"Link:url={self.data['url']}"
+        return repr(self.data["link"])
 
 
 class ImageSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"<Image:url={self.data['url']}>"
+        return repr(self.data["image"])
 
 
 class QuoteSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"<Quote:msg_id={self.data['msg_id']}>"
+        return repr(self.data["quote"])
 
 
 class PostSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
-        return f"<Post:post_id={self.data['post_id']}>"
+        return repr(self.data["post"])
+
+
+class PreviewLinkSegment(MessageSegment):
+    @overrides
+    def __str__(self) -> str:
+        return repr(self.data["preview_link"])
+
+
+class BadgeSegment(MessageSegment):
+    @overrides(MessageSegment)
+    def __str__(self) -> str:
+        return repr(self.data["badge"])
 
 
 class Message(BaseMessage[MessageSegment]):
     @classmethod
     @overrides(BaseMessage)
     def get_segment_class(cls) -> Type[MessageSegment]:
         return MessageSegment
```

### Comparing `nonebot_adapter_villa-0.4.2/pyproject.toml` & `nonebot_adapter_villa-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.4.2"
+version = "0.5.0"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

