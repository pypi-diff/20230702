# Comparing `tmp/pywa-0.0.1rc12-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc13-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 24356 bytes, number of entries: 15
+Zip file size: 25031 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jun-28 10:05 pywa/__version__.py
--rw-rw-r--  2.0 unx    15070 b- defN 23-Jun-28 09:01 pywa/api.py
--rw-rw-r--  2.0 unx    26900 b- defN 23-Jun-28 10:04 pywa/client.py
--rw-rw-r--  2.0 unx     2183 b- defN 23-Jun-28 09:56 pywa/errors.py
--rw-rw-r--  2.0 unx    14258 b- defN 23-Jun-28 09:56 pywa/filters.py
--rw-rw-r--  2.0 unx     1630 b- defN 23-Jun-28 09:26 pywa/handlers.py
--rw-rw-r--  2.0 unx    34313 b- defN 23-Jun-28 09:56 pywa/types.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-02 08:23 pywa/__version__.py
+-rw-rw-r--  2.0 unx    14991 b- defN 23-Jul-02 07:58 pywa/api.py
+-rw-rw-r--  2.0 unx    26847 b- defN 23-Jul-02 08:19 pywa/client.py
+-rw-rw-r--  2.0 unx     2322 b- defN 23-Jul-02 08:19 pywa/errors.py
+-rw-rw-r--  2.0 unx    15854 b- defN 23-Jul-02 08:19 pywa/filters.py
+-rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-02 08:19 pywa/handlers.py
+-rw-rw-r--  2.0 unx    34447 b- defN 23-Jul-02 08:21 pywa/types.py
 -rw-rw-r--  2.0 unx      991 b- defN 23-Jun-20 16:58 pywa/utils.py
--rw-rw-r--  2.0 unx     4391 b- defN 23-Jun-28 10:01 pywa/webhook.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-28 10:06 pywa-0.0.1rc12.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4389 b- defN 23-Jun-28 10:06 pywa-0.0.1rc12.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-28 10:06 pywa-0.0.1rc12.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-28 10:06 pywa-0.0.1rc12.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1106 b- defN 23-Jun-28 10:06 pywa-0.0.1rc12.dist-info/RECORD
-15 files, 106537 bytes uncompressed, 22574 bytes compressed:  78.8%
+-rw-rw-r--  2.0 unx     4399 b- defN 23-Jun-30 09:01 pywa/webhook.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4399 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-02 08:23 pywa-0.0.1rc13.dist-info/RECORD
+15 files, 108456 bytes uncompressed, 23249 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pywa/utils.py
 Comment: 
 
 Filename: pywa/webhook.py
 Comment: 
 
-Filename: pywa-0.0.1rc12.dist-info/LICENSE
+Filename: pywa-0.0.1rc13.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc12.dist-info/METADATA
+Filename: pywa-0.0.1rc13.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc12.dist-info/WHEEL
+Filename: pywa-0.0.1rc13.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc12.dist-info/top_level.txt
+Filename: pywa-0.0.1rc13.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc12.dist-info/RECORD
+Filename: pywa-0.0.1rc13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc12"
+__version__ = "0.0.1rc13"
```

## pywa/api.py

```diff
@@ -1,11 +1,11 @@
 import mimetypes
 import requests
 from typing import Iterable
-from pywa.errors import WhatsAppApiError
+from pywa.errors import WhatsAppError
 from pywa.types import InlineButton, SectionList, Contact
 
 
 class WhatsAppCloudApi:
     """Internal methods for the WhatsApp client."""
 
     def __init__(
@@ -44,19 +44,19 @@
             endpoint: The endpoint to request.
             **kwargs: Additional arguments to pass to the request.
 
         Returns:
             The response JSON.
 
         Raises:
-            WhatsAppApiError: If the request failed.
+            WhatsAppError: If the request failed.
         """
         res = self._session.request(method=method, url=f"{self._base_url}{endpoint}", **kwargs)
         if res.status_code != 200:
-            raise WhatsAppApiError.from_response(status_code=res.status_code, error=res.json()["error"])
+            raise WhatsAppError.from_response(status_code=res.status_code, error=res.json()["error"])
         return res.json()
 
     def send_text_message(
             self,
             to: str | int,
             text: str,
             preview_url: bool = False,
@@ -177,33 +177,32 @@
             A dict with the URL and other info about the media file.
         """
         return self._make_request(
             method="GET",
             endpoint=f"/{media_id}"
         )
 
-    def download_media(
+    def get_media_bytes(
             self,
             media_url: str,
-    ) -> tuple[bytes, str]:
+    ) -> tuple[bytes, str | None]:
         """
-        Download a media file from WhatsApp servers.
+        Get the bytes of a media file from WhatsApp servers.
 
         Args:
             media_url: The URL of the media file (from ``get_media_url``).
 
         Returns:
-            The media file bytes and the MIME type.
+            The media file bytes and the MIME type (if available).
         """
         headers = self._session.headers.copy()
         del headers["Content-Type"]
         res = self._session.get(media_url, headers=headers)
         res.raise_for_status()
-        return res.content, res.headers.get("Content-Type", default=res.headers.get("content-type")) \
-                            or 'application/octet-stream'
+        return res.content, res.headers.get("Content-Type")
 
     def delete_media(self, media_id: str) -> dict[str, bool]:
         """
         Delete a media file from WhatsApp servers.
 
         Return example::
```

## pywa/client.py

```diff
@@ -1,9 +1,11 @@
 """The WhatsApp client."""
 
+__all__ = ("WhatsApp",)
+
 import hashlib
 import mimetypes
 import os
 import requests
 from typing import Callable, Any, Iterable
 from pywa.api import WhatsAppCloudApi
 from pywa.handlers import Handler, MessageHandler, ButtonCallbackHandler, SelectionCallbackHandler, RawUpdateHandler, \
@@ -484,15 +486,14 @@
             reply_to_message_id=reply_to_message_id,
         )['messages'][0]['id']
 
     def send_sticker(
             self,
             to: str,
             sticker: str | bytes,
-            animated: bool = False,
             reply_to_message_id: str | None = None,
     ) -> str:
         """
         Send a sticker to a WhatsApp user.
             - A static sticker needs to be 512x512 pixels and cannot exceed 100 KB.
             - An animated sticker must be 512x512 pixels and cannot exceed 500 KB.
 
@@ -502,26 +503,24 @@
             ...     to='1234567890',
             ...     sticker='https://example.com/sticker.webp',
             ... )
 
         Args:
             to: The phone ID of the WhatsApp user.
             sticker: The sticker to send (either a URL or a file ID).
-            animated: Whether the sticker is animated (optional).
             reply_to_message_id: The message ID to reply to (optional).
 
         Returns:
             The message ID of the sent message.
         """
         return self.api.send_media(
             to=to,
             media_id_or_url=sticker,
             media_type="sticker",
             reply_to_message_id=reply_to_message_id,
-            animated=animated,
         )['messages'][0]['id']
 
     def send_reaction(
             self,
             to: str,
             emoji: str,
             message_id: str,
@@ -729,18 +728,19 @@
             path: The path where to save the file (if not provided, the current working directory will be used).
             filename: The name of the file (if not provided, it will be guessed from the URL + extension).
             in_memory: Whether to return the file as bytes instead of saving it to disk (default: False).
 
         Returns:
             The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
         """
-        content, mimetype = self.api.download_media(media_url=url)
+        content, mimetype = self.api.get_media_bytes(media_url=url)
         if in_memory:
             return content
         if path is None:
             path = os.getcwd()
         if filename is None:
-            filename = hashlib.sha256(url.encode()).hexdigest() + mimetypes.guess_extension(mimetype)
+            filename = hashlib.sha256(url.encode()).hexdigest() +\
+                       mimetypes.guess_extension(mimetype or 'application/octet-stream')
         path = os.path.join(path, filename)
         with open(path, "wb") as f:
             f.write(content)
         return path
```

## pywa/errors.py

```diff
@@ -1,10 +1,15 @@
+"""
+This module contains the errors that can be raised by the WhatsApp Cloud API or incoming error from the webhook.
+"""
 
+__all__ = ("WhatsAppError",)
 
-class WhatsAppApiError(Exception):
+
+class WhatsAppError(Exception):
     """
     Represents an error that happened while making a request to the WhatsApp Cloud API or incoming error from the webhook.
 
     - See more: https://developers.facebook.com/docs/whatsapp/cloud-api/support/error-codes
 
     Attributes:
         status_code: The status code (in case of response, else None).
@@ -31,38 +36,38 @@
         self.href = href
 
     @classmethod
     def from_response(
             cls,
             status_code: int,
             error: dict
-    ) -> "WhatsAppApiError":
+    ) -> "WhatsAppError":
         """Create an error from a response."""
         return cls(
             status_code=status_code,
             error_code=error["code"],
             message=error["message"],
             details=error.get("error_data", {}).get("details", None),
             fbtrace_id=error.get("fbtrace_id"),
             href=error.get('href')
         )
 
     @classmethod
     def from_incoming_error(
             cls,
             error: dict
-    ) -> "WhatsAppApiError":
+    ) -> "WhatsAppError":
         """Create an error from an incoming error."""
         return cls(
             status_code=None,
             error_code=error["code"],
             message=error["message"],
             details=error.get("error_data", {}).get("details", None),
             fbtrace_id=error.get("fbtrace_id"),
             href=error.get('href')
         )
 
     def __str__(self) -> str:
-        return f"WhatsAppApiError(status_code={self.status_code}, message={self.message!r}, details={self.details!r})"
+        return f"WhatsAppError(message={self.message!r}, details={self.details!r}, error_code={self.error_code!r})"
 
     def __repr__(self) -> str:
         return self.__str__()
```

## pywa/filters.py

```diff
@@ -1,19 +1,10 @@
 """Usefully filters to use in your handlers."""
 from __future__ import annotations
 
-import re
-from typing import Callable, TYPE_CHECKING, Iterable
-from pywa import utils
-from pywa.types import MessageType as Mt, Message as Msg, MessageStatus as Ms, MessageStatusType as Mst, \
-    CallbackButton, CallbackSelection
-
-if TYPE_CHECKING:
-    from pywa import WhatsApp as Wa
-
 __all__ = (
     "TextFilter",
     "ImageFilter",
     "VideoFilter",
     "AudioFilter",
     "DocumentFilter",
     "StickerFilter",
@@ -21,99 +12,125 @@
     "UnsupportedMsgFilter",
     "LocationFilter",
     "ContactsFilter",
     "CallbackFilter",
     "MessageStatusFilter"
 )
 
-_ONLY_NUMS_RE = re.compile(r"\D")
+import re
+from typing import Callable, TYPE_CHECKING, Iterable
+from pywa import utils
+from pywa.types import MessageType as Mt, Message as Msg, MessageStatus as Ms, MessageStatusType as Mst, \
+    CallbackButton, CallbackSelection
+
+if TYPE_CHECKING:
+    from pywa import WhatsApp as Wa
 
 
 class TextFilter:
     """Useful filters for text messages."""
 
     ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.TEXT
     """Filter for all text messages."""
 
     @staticmethod
-    def equals(*matches: str, ignore_case: bool = False) -> Callable[[Wa, Msg], bool]:
+    def match(*matches: str, ignore_case: bool = False) -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that equal the given text/s.
 
+        >>> TextFilter.match("Hello", "Hi")
+
         Args:
             matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         return lambda wa, m: m.type == Mt.TEXT and any(
             (m.text.lower() == t.lower() if ignore_case else m.text == t for t in matches)
         )
 
+    equals = match  # alias
+
     @staticmethod
     def contains(*matches: str, ignore_case: bool = False) -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that contain the given text/s.
 
+        >>> TextFilter.contains("Cat", "Dog", ignore_case=True)
+
         Args:
             matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching. (default: ``False``).
         """
         return lambda wa, m: m.type == Mt.TEXT and any(
             (t.lower() in m.text.lower() if ignore_case else t in m.text for t in matches)
         )
 
     @staticmethod
     def startswith(*matches: str, ignore_case: bool = False) -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that start with the given text/s.
 
+        >>> TextFilter.startswith("What", "When", ignore_case=True)
+
         Args:
             matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         return lambda wa, m: m.type == Mt.TEXT and any(
             (m.text.lower().startswith(t.lower()) if ignore_case else m.text.startswith(t) for t in matches)
         )
 
     @staticmethod
     def endswith(*matches: str, ignore_case: bool = False) -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that end with the given text/s.
 
+        >>> TextFilter.endswith("Bye", "See you", ignore_case=True)
+
         Args:
             matches: The text/s to filter for.
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         return lambda wa, m: m.type == Mt.TEXT and any(
             (m.text.lower().endswith(t.lower()) if ignore_case else m.text.endswith(t) for t in matches)
         )
 
     @staticmethod
     def regex(*patterns: str | re.Pattern, flags: int = 0) -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that match the given regex/regexes.
-            * It's recommended to pass compiled regexes to save time (``re.compile(your_pattern)``)
+
+        >>> TextFilter.regex(r"Hello\s+World", r"Bye\s+World", flags=re.IGNORECASE)
+
+        Args:
+            patterns: The regex/regexes to filter for.
+            flags: The regex flags to use (default: ``0``).
         """
+        patterns = [re.compile(p, flags) if isinstance(p, str) else p for p in patterns]
         return lambda wa, m: m.type == Mt.TEXT and any(re.match(p, m.text, flags) for p in patterns)
 
     @staticmethod
     def length(*lengths: tuple[int, int]) -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that have a length between the given range/s.
 
+        >>> TextFilter.length((1, 10), (50, 100))
+
         Args:
             lengths: The length range/s to filter for (e.g. (1, 10), (50, 100)).
         """
         return lambda wa, m: m.type == Mt.TEXT and any((i[0] <= len(m.text) <= i[1] for i in lengths))
 
     @staticmethod
-    def command(*cmds: str, prefixes: str | Iterable[str] = "!", ignore_case: bool = False) -> Callable[
-        [Wa, Msg], bool]:
+    def command(*cmds: str, prefixes: str | Iterable[str] = "!", ignore_case: bool = False) -> Callable[[Wa, Msg], bool]:
         """
         Filter for text messages that are commands.
 
+        >>> TextFilter.command("start", "hello", prefixes=("!", "/"), ignore_case=True)
+
         Args:
             cmds: The command/s to filter for (e.g. "start", "hello").
             prefixes: The prefix/s to filter for (default: "!", i.e. "!start").
             ignore_case: Whether to ignore case when matching (default: ``False``).
         """
         return lambda wa, m: m.type == Mt.TEXT and any(
             m.text[0] in prefixes and (m.text[1:] if not ignore_case else m.text[1:].lower())
@@ -133,14 +150,16 @@
         return m.type == Mt.IMAGE and m.image.caption is not None
 
     @staticmethod
     def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
         """
         Filter for image messages that have the given mime type/s.
         See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+
+        >>> ImageFilter.mimetype("image/png")
         """
         return lambda wa, m: m.type == Mt.IMAGE and any((t == m.image.mime_type for t in mime_types))
 
 
 class VideoFilter:
     """Useful filters for video messages."""
 
@@ -148,14 +167,16 @@
     """Filter for all video messages."""
 
     @staticmethod
     def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
         """
         Filter for video messages that have the given mime type/s.
         See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+
+        >>> VideoFilter.mimetype("video/mp4")
         """
         return lambda wa, m: m.type == Mt.VIDEO and any((t == m.video.mime_type for t in mime_types))
 
 
 class AudioFilter:
     """Useful filters for audio messages."""
 
@@ -169,14 +190,16 @@
     """Filter for audio messages that are audio files."""
 
     @staticmethod
     def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
         """
         Filter for audio messages that have the given mime type/s.
         See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+
+        >>> AudioFilter.mimetype("audio/ogg")
         """
         return lambda wa, m: m.type == Mt.AUDIO and any((t == m.audio.mime_type for t in mime_types))
 
 
 class DocumentFilter:
     """Useful filters for document messages."""
 
@@ -184,28 +207,31 @@
     """Filter for all document messages."""
 
     @staticmethod
     def mimetype(*mime_types: str) -> Callable[[Wa, Msg], bool]:
         """
         Filter for document messages that have the given mime type/s.
         See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
+
+        >>> DocumentFilter.mimetype("application/pdf")
         """
         return lambda wa, m: m.type == Mt.DOCUMENT and any((t == m.document.mime_type for t in mime_types))
 
 
 class StickerFilter:
     """Useful filters for sticker messages."""
 
     ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.STICKER
     """Filter for all sticker messages."""
 
     ANIMATED: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.STICKER and m.sticker.animated
     """Filter for animated sticker messages."""
 
     STATIC: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.STICKER and not m.sticker.animated
+    """Filter for static sticker messages."""
 
 
 class LocationFilter:
     """Useful filters for location messages."""
 
     ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.LOCATION
     """Filter for all location messages."""
@@ -242,15 +268,19 @@
     """Filter for reaction messages that were added."""
 
     REMOVED: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.REACTION and m.reaction.emoji is None
     """Filter for reaction messages that were removed."""
 
     @staticmethod
     def emoji(*emojis: str) -> Callable[[Wa, Msg], bool]:
-        """Filter for custom reaction messages. pass emojis as strings."""
+        """
+        Filter for custom reaction messages. pass emojis as strings.
+
+        >>> ReactionFilter.emoji("👍", "👎")
+        """
         return lambda wa, m: m.type == Mt.REACTION and m.reaction.emoji in emojis
 
 
 class ContactsFilter:
     """Useful filters for contact messages."""
 
     ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.CONTACTS
@@ -259,25 +289,33 @@
     HAS_WA: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.CONTACTS and (
         any((p.wa_id for p in (phone for contact in m.contacts for phone in contact.phones)))
     )
     """Filter for contacts messages that have a WhatsApp account."""
 
     @staticmethod
     def count(min_count: int, max_count: int) -> Callable[[Wa, Msg], bool]:
-        """Filter for contacts messages that have a number of contacts between min_count and max_count."""
+        """
+        Filter for contacts messages that have a number of contacts between min_count and max_count.
+
+        >>> ContactsFilter.count(1, 1) # ensure only 1 contact
+        >>> ContactsFilter.count(1, 5) # between 1 and 5 contacts
+        """
         return lambda wa, m: m.type == Mt.CONTACTS and min_count <= len(m.contacts) <= max_count
 
     @staticmethod
     def phone(*phones: str) -> Callable[[Wa, Msg], bool]:
         """
         Filter for contacts messages that have the given phone number/s.
-            * Pass only the numbers, without plus sign, spaces, etc.
+
+        >>> ContactsFilter.phone("+1 555-555-5555", "972123456789")
         """
+        only_nums_pattern = re.compile(r"\D")
+        phones = [re.sub(only_nums_pattern, "", p) for p in phones]
         return lambda wa, m: m.type == Mt.CONTACTS and (
-            any((re.sub(_ONLY_NUMS_RE, "", p.phone) in phones for contact in m.contacts for p in contact.phones))
+            any((re.sub(only_nums_pattern, "", p.phone) in phones for contact in m.contacts for p in contact.phones))
         )
 
 
 class UnsupportedMsgFilter:
     """Useful filters for unsupported messages."""
 
     ANY: Callable[[Wa, Msg], bool] = lambda wa, m: m.type == Mt.UNSUPPORTED
@@ -287,68 +325,80 @@
 class CallbackFilter:
     """Useful filters for callback queries."""
 
     ANY: Callable[[Wa, CallbackButton | CallbackSelection], bool] = lambda wa, c: True
     """Filter for all callback queries (the default)."""
 
     @staticmethod
-    def data_equals(*matches: str, ignore_case: bool = False) -> Callable[
-        [Wa, CallbackButton | CallbackSelection], bool]:
+    def data_match(*matches: str, ignore_case: bool = False) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """
         Filter for callbacks their data equals the given string/s.
 
+        >>> CallbackFilter.data_match("menu")
+        >>> CallbackFilter.data_match("back", "return", "exit")
+
         Args:
             matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         return lambda wa, c: any((c.data.lower() == m.lower() if ignore_case else c.data == m for m in matches))
 
+    data_equals = data_match
+
     @staticmethod
     def data_startswith(*matches: str, ignore_case: bool = False) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """
         Filter for callbacks their data starts with the given string/s.
 
+        >>> CallbackFilter.data_startswith("id:")
+
         Args:
             matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         return lambda wa, c: any(
             (c.data.lower().startswith(m.lower()) if ignore_case else c.data.startswith(m) for m in matches)
         )
 
     @staticmethod
     def data_endswith(*matches: str, ignore_case: bool = False) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """
         Filter for callbacks their data ends with the given string/s.
 
+        >>> CallbackFilter.data_endswith(":true", ":false")
+
         Args:
             matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         return lambda wa, c: any(
             (c.data.lower().endswith(m.lower()) if ignore_case else c.data.endswith(m) for m in matches)
         )
 
     @staticmethod
     def data_contains(*matches: str, ignore_case: bool = False) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """
         Filter for callbacks their data contains the given string/s.
 
+        >>> CallbackFilter.data_contains("back")
+
         Args:
             matches: The string/s to match.
             ignore_case: Whether to ignore case when matching (default: False).
         """
         return lambda wa, c: any((m in c.data.lower() if ignore_case else m in c.data for m in matches))
 
     @staticmethod
     def data_regex(*patterns: str | re.Pattern) -> Callable[[Wa, CallbackButton | CallbackSelection], bool]:
         """
         Filter for callbacks their data matches the given regex/regexes.
-            * It's recommended to pass compiled regexes to save time (``re.compile(your_pattern)``)
+
+        >>> CallbackFilter.data_regex(r"^\d+$")  # only digits
         """
+        patterns = [re.compile(p) if isinstance(p, str) else p for p in patterns]
         return lambda wa, c: any((re.match(p, c.data) for p in patterns))
 
 
 class MessageStatusFilter:
     """Useful filters for message status updates."""
 
     SENT: Callable[[Wa, Ms], bool] = lambda wa, data: data.status == Mst.SENT
@@ -360,10 +410,14 @@
     READ: Callable[[Wa, Ms], bool] = lambda wa, data: data.status == Mst.READ
     """Filter for messages that have been read."""
 
     FAILED: Callable[[Wa, Ms], bool] = lambda wa, data: data.status == Mst.FAILED
     """Filter for messages that have failed to send (than you can access to the ``error`` attribute)."""
 
     @staticmethod
-    def failed_on_error_code(*codes: int) -> Callable[[Wa, Ms], bool]:
-        """Filter for messages that have failed to send with the given error code/s."""
+    def failed_with_error_code(*codes: int) -> Callable[[Wa, Ms], bool]:
+        """
+        Filter for messages that have failed to send with the given error code/s.
+
+        >>> MessageStatusFilter.failed_with_error_code(131056) # Too many requests
+        """
         return lambda wa, s: s.status == Mst.FAILED and s.error.error_code in codes
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## pywa/handlers.py

```diff
@@ -1,7 +1,19 @@
+"""
+This module contains the handlers for incoming updates.
+"""
+
+__all__ = (
+    "MessageHandler",
+    "ButtonCallbackHandler",
+    "SelectionCallbackHandler",
+    "RawUpdateHandler",
+    "MessageStatusHandler"
+)
+
 from typing import Callable, Any, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pywa import WhatsApp
 
 
 class Handler:
@@ -32,20 +44,20 @@
 
 class MessageHandler(Handler):
     """A message handler (e.g. text, image, video, audio, etc.)."""
     __handler_type__ = "message"
 
 
 class ButtonCallbackHandler(Handler):
-    """A button handler."""
+    """A button click handler."""
     __handler_type__ = "button"
 
 
 class SelectionCallbackHandler(Handler):
-    """A section handler."""
+    """A selection choice handler."""
     __handler_type__ = "selection"
 
 
 class RawUpdateHandler(Handler):
     """A raw update handler."""
     __handler_type__ = "raw_update"
 
@@ -53,8 +65,7 @@
 class MessageStatusHandler(Handler):
     """
     A message status handler (e.g. delivered, read, failed, etc.).
 
     **DO NOT USE THIS HANDLER TO SEND MESSAGES, IT WILL CAUSE AN INFINITE LOOP!**
     """
     __handler_type__ = "message_status"
-    """A message status handler (e.g. delivered, read, etc.)."""
```

## pywa/types.py

```diff
@@ -12,19 +12,19 @@
     "SectionRow",
     "Section",
     "SectionList",
     "MediaUrlResponse"
 )
 
 from datetime import datetime
-from dataclasses import dataclass, field, asdict
+from dataclasses import dataclass, field, asdict, fields
 from enum import Enum
 from typing import TYPE_CHECKING, Iterable
 from pywa import utils
-from pywa.errors import WhatsAppApiError
+from pywa.errors import WhatsAppError
 
 if TYPE_CHECKING:
     from pywa.client import WhatsApp
 
 
 @dataclass(frozen=True, slots=True)
 class InlineButton:
@@ -144,25 +144,34 @@
     def _missing_(cls, value):
         return cls.UNSUPPORTED
 
     def __str__(self):
         return self.value
 
 
+@dataclass(frozen=True, slots=True, kw_only=True)
+class _FromDict:
+    """Base class for dataclasses that can be created from dict unpacking."""
+    # noinspection PyArgumentList
+    @classmethod
+    def from_dict(cls, **kwargs):
+
+        return cls(**{
+            k: v for k, v in kwargs.items()
+            if k in (f.name for f in fields(cls))
+        })
+
+
 @dataclass(frozen=True, slots=True)
-class MediaBase:
+class MediaBase(_FromDict):
     _client: WhatsApp = field(repr=False, hash=False, compare=False)
     id: str
     sha256: str
     mime_type: str
 
-    @classmethod
-    def from_dict(cls, client: WhatsApp, data: dict | None):
-        return cls(_client=client, **data) if data else None
-
     def get_media_url(self) -> str:
         """Gets the URL of the media. (expires after 5 minutes)"""
         return self._client.get_media_url(media_id=self.id).url
 
     def download(
             self,
             path: str | None = None,
@@ -196,30 +205,27 @@
     """
     Represents an image.
 
     Attributes:
         id: The ID of the image.
         sha256: The SHA256 hash of the image.
         mime_type: The MIME type of the image.
-        caption: The caption of the image (optional).
     """
-    caption: str | None = None
 
 
 @dataclass(frozen=True, slots=True)
 class Video(MediaBase):
     """
     Represents a video.
 
     Attributes:
         id: The ID of the video.
         sha256: The SHA256 hash of the video.
         mime_type: The MIME type of the video.
     """
-    pass
 
 
 @dataclass(frozen=True, slots=True)
 class Sticker(MediaBase):
     """
     Represents a sticker.
 
@@ -257,32 +263,28 @@
         mime_type: The MIME type of the audio.
         voice: Whether the audio is a voice message or just an audio file.
     """
     voice: bool
 
 
 @dataclass(frozen=True, slots=True)
-class Reaction:
+class Reaction(_FromDict):
     """
     Represents a reaction to a message.
 
     Attributes:
         message_id: The ID of the message that was reacted to.
         emoji: The emoji that was used to react to the message (optional, ``None`` if removed).
     """
     message_id: str
     emoji: str | None = None
 
-    @classmethod
-    def from_dict(cls, data: dict | None):
-        return cls(**data) if data else None
-
 
 @dataclass(frozen=True, slots=True)
-class Location:
+class Location(_FromDict):
     """
     Represents a location.
 
     Attributes:
         latitude: The latitude of the location.
         longitude: The longitude of the location.
         name: The name of the location (optional).
@@ -291,33 +293,28 @@
     """
     latitude: float
     longitude: float
     name: str | None = None
     address: str | None = None
     url: str | None = None
 
-    @classmethod
-    def from_dict(cls, data: dict | None):
-        return cls(**data) if data else None
-
-    def in_radius(self, other: Location, radius: float | int) -> bool:
+    def in_radius(self, lat: float, lon: float, radius: float | int) -> bool:
         """
         Check if the location is in a radius of another location.
 
         Args:
-            other: The other location (the center. No need for name, address or url).
+            lat: The latitude of the other location.
+            lon: The longitude of the other location.
             radius: The radius in kilometers.
         """
-        return utils.get_distance(
-            lat1=self.latitude, lon1=self.longitude, lat2=other.latitude, lon2=other.longitude
-        ) <= radius
+        return utils.get_distance(lat1=self.latitude, lon1=self.longitude, lat2=lat, lon2=lon) <= radius
 
 
 @dataclass(frozen=True, slots=True)
-class MediaUrlResponse:
+class MediaUrlResponse(_FromDict):
     """
     Represents a media response.
 
     Attributes:
         id: The ID of the media.
         url: The URL of the media (valid for 5 minutes).
         mime_type: The MIME type of the media.
@@ -370,38 +367,38 @@
     phones: list[Phone] = field(default_factory=list)
     emails: list[Email] = field(default_factory=list)
     urls: list[Url] = field(default_factory=list)
     addresses: list[Address] = field(default_factory=list)
     org: Org | None = None
 
     @classmethod
-    def from_dict(cls, data: dict | None):
+    def from_dict(cls, **data):
         return cls(
-            name=cls.Name(**data["name"]),
+            name=cls.Name.from_dict(**data["name"]),
             birthday=data.get("birthday"),
-            phones=[cls.Phone.from_dict(phone) for phone in data.get("phones", ())],
-            emails=[cls.Email.from_dict(email) for email in data.get("emails", ())],
-            urls=[cls.Url.from_dict(url) for url in data.get("urls", ())],
-            addresses=[cls.Address.from_dict(address) for address in data.get("addresses", ())],
-            org=cls.Org.from_dict(data.get("org")),
+            phones=[cls.Phone.from_dict(**phone) for phone in data.get("phones", ())],
+            emails=[cls.Email.from_dict(**email) for email in data.get("emails", ())],
+            urls=[cls.Url.from_dict(**url) for url in data.get("urls", ())],
+            addresses=[cls.Address.from_dict(**address) for address in data.get("addresses", ())],
+            org=cls.Org.from_dict(**data.get("org")) if data.get("org") else None,
         ) if data else None
 
     def to_dict(self) -> dict:
         return {
             "name": asdict(self.name),
             "birthday": self.birthday,
             "phones": [asdict(phone) for phone in self.phones],
             "emails": [asdict(email) for email in self.emails],
             "urls": [asdict(url) for url in self.urls],
             "addresses": [asdict(address) for address in self.addresses],
             "org": asdict(self.org) if self.org else None,
         }
 
     @dataclass(frozen=True, slots=True)
-    class Name:
+    class Name(_FromDict):
         """
         Represents a contact's name.
 
         - At least one of the optional parameters needs to be included along with the formatted_name parameter.
 
         Attributes:
             formatted_name: The formatted name of the contact.
@@ -415,83 +412,67 @@
         first_name: str | None = None
         last_name: str | None = None
         middle_name: str | None = None
         suffix: str | None = None
         prefix: str | None = None
 
     @dataclass(frozen=True, slots=True)
-    class Phone:
+    class Phone(_FromDict):
         """
         Represents a contact's phone number.
 
         Attributes:
             phone: The phone number (If ``wa_id`` is provided, No need for the ``phone``).
             type: The type of the phone number (Standard Values are CELL, MAIN, IPHONE, HOME, and WORK. optional).
             wa_id: The WhatsApp ID of the contact (optional).
         """
         phone: str | None = None
         type: str | None = None
         wa_id: str | None = None
 
-        @classmethod
-        def from_dict(cls, data: dict | None):
-            return cls(**data) if data else None
-
     @dataclass(frozen=True, slots=True)
-    class Email:
+    class Email(_FromDict):
         """
         Represents a contact's email address.
 
         Attributes:
             email: The email address.
             type: The type of the email address (Standard Values are WORK and HOME. optional).
         """
         email: str | None = None
         type: str | None = None
 
-        @classmethod
-        def from_dict(cls, data: dict | None):
-            return cls(**data) if data else None
-
     @dataclass(frozen=True, slots=True)
-    class Url:
+    class Url(_FromDict):
         """
         Represents a contact's URL.
 
         Attributes:
             url: The URL.
             type: The type of the URL (Standard Values are WORK and HOME. optional).
         """
         url: str | None = None
         type: str | None = None
 
-        @classmethod
-        def from_dict(cls, data: dict | None):
-            return cls(**data) if data else None
-
     @dataclass(frozen=True, slots=True)
-    class Org:
+    class Org(_FromDict):
         """
         Represents a contact's organization.
 
         Attributes:
             company: The company of the contact (optional).
             department: The department of the contact (optional).
             title: The title of the business contact (optional).
         """
         company: str | None = None
         department: str | None = None
         title: str | None = None
 
-        @classmethod
-        def from_dict(cls, data: dict | None):
-            return cls(**data) if data else None
-
     @dataclass(frozen=True, slots=True)
-    class Address:
+    class Address(_FromDict):
         """
         Represents a contact's address.
 
         Attributes:
             street: The street number and name of the address (optional).
             city: The city name of the address (optional).
             state: State abbreviation.
@@ -504,18 +485,14 @@
         city: str | None = None
         state: str | None = None
         zip: str | None = None
         country: str | None = None
         country_code: str | None = None
         type: str | None = None
 
-        @classmethod
-        def from_dict(cls, data: dict | None):
-            return cls(**data) if data else None
-
 
 @dataclass(frozen=True, slots=True)
 class ReplyToMessage:
     """
     Represents a message that was replied to.
 
     Attributes:
@@ -530,15 +507,15 @@
         return cls(
             message_id=data['id'],
             from_user_id=data['from']
         ) if (data and 'id' in data) else None
 
 
 @dataclass(frozen=True, slots=True)
-class Metadata:
+class Metadata(_FromDict):
     """
     Represents the metadata of a message.
 
     Attributes:
         display_phone_number: The phone number to which the message was sent.
         phone_number_id: The ID of the phone number to which the message was sent.
     """
@@ -720,32 +697,29 @@
             audio=audio,
             reply_to_message_id=self.message_id_to_reply if quote else None
         )
 
     def reply_sticker(
             self,
             sticker: str | bytes,
-            animated: bool = False,
             quote: bool = False,
     ) -> str:
         """
         Reply to the message with a sticker.
 
         Args:
             sticker: The sticker to reply with.
-            animated: Whether the sticker is animated (default: False).
             quote: Whether to quote the message (default: False).
 
         Returns:
             The ID of the sent message.
         """
         return self._client.send_sticker(
             to=self.sender,
             sticker=sticker,
-            animated=animated,
             reply_to_message_id=self.message_id_to_reply if quote else None
         )
 
     def reply_location(
             self,
             latitude: float,
             longitude: float,
@@ -857,56 +831,63 @@
         forwarded: Whether the message was forwarded.
         text: The text of the message (if the message type is text). (optional)
         image: The image of the message (if the message type is image). (optional)
         video: The video of the message (if the message type is video). (optional)
         sticker: The sticker of the message (if the message type is sticker). (optional)
         document: The document of the message (if the message type is document). (optional)
         audio: The audio of the message (if the message type is audio). (optional)
+        caption: The caption of the message (if the message type is image, video, or document). (optional)
         reaction: The reaction of the message (if the message type is reaction). (optional)
         location: The location of the message (if the message type is location). (optional)
         contacts: The contacts of the message (if the message type is contacts). (optional)
+        error: The error of the message (if the message type is `unsupported`). (optional)
     """
     reply_to_message: ReplyToMessage | None
     forwarded: bool
     text: str | None
     image: Image | None
     video: Video | None
     sticker: Sticker | None
     document: Document | None
     audio: Audio | None
+    caption: str | None
     reaction: Reaction | None
     location: Location | None
     contacts: list[Contact] | None
+    error: WhatsAppError | None
 
     @property
     def message_id_to_reply(self) -> str:
-        """The ID of the message"""
+        """The ID of the message to reply to."""
         return self.id if self.type != MessageType.REACTION else self.reaction.message_id
 
     @classmethod
-    def from_dict(cls, client: WhatsApp, value: dict):
+    def from_dict(cls, client: WhatsApp, value: dict) -> Message:
         message = value['messages'][0]
         return cls(
             _client=client,
             id=message['id'],
             type=MessageType(message['type']),
             from_user=User.from_dict(value['contacts'][0]),
             timestamp=datetime.fromtimestamp(int(message['timestamp'])),
-            metadata=Metadata(**value['metadata']),
+            metadata=Metadata.from_dict(**value['metadata']),
             forwarded=message.get('context', {}).get('forwarded', False),
             reply_to_message=ReplyToMessage.from_dict(message.get('context')),
             text=message['text']['body'] if 'text' in message else None,
-            image=Image.from_dict(client=client, data=message.get('image')),
-            video=Video.from_dict(client=client, data=message.get('video')),
-            sticker=Sticker.from_dict(client=client, data=message.get('sticker')),
-            document=Document.from_dict(client=client, data=message.get('document')),
-            audio=Audio.from_dict(client=client, data=message.get('audio')),
-            reaction=Reaction.from_dict(message.get('reaction')),
-            location=Location.from_dict(message.get('location')),
-            contacts=[Contact.from_dict(contact) for contact in message.get('contacts', ())] or None
+            image=Image.from_dict(_client=client, **message.get('image')) if 'image' in message else None,
+            video=Video.from_dict(_client=client, **message.get('video')) if 'video' in message else None,
+            sticker=Sticker.from_dict(_client=client, **message.get('sticker')) if 'sticker' in message else None,
+            document=Document.from_dict(_client=client, **message.get('document')) if 'document' in message else None,
+            audio=Audio.from_dict(_client=client, **message.get('audio')) if 'audio' in message else None,
+            caption=message.get(message['type'], {}).get('caption', None)
+            if message['type'] in ('image', 'video', 'document') else None,
+            reaction=Reaction.from_dict(**message.get('reaction')) if 'reaction' in message else None,
+            location=Location.from_dict(**message.get('location')) if 'location' in message else None,
+            contacts=[Contact.from_dict(**contact) for contact in message.get('contacts', ())] or None,
+            error=WhatsAppError.from_incoming_error(message['errors'][0]) if 'errors' in message else None
         )
 
     def download_media(
             self,
             filepath: str | None = None,
             filename: str | None = None,
             in_memory: bool = False,
@@ -957,15 +938,15 @@
 
     @classmethod
     def from_dict(cls, client: WhatsApp, value: dict):
         message = value['messages'][0]
         return cls(
             _client=client,
             id=message['id'],
-            metadata=Metadata(**value['metadata']),
+            metadata=Metadata.from_dict(**value['metadata']),
             type=MessageType(message['type']),
             from_user=User.from_dict(value['contacts'][0]),
             timestamp=datetime.fromtimestamp(int(message['timestamp'])),
             reply_to_message=ReplyToMessage.from_dict(message['context']),
             data=message['interactive']['button_reply']['id'],
             title=message['interactive']['button_reply']['title']
         )
@@ -999,15 +980,15 @@
 
     @classmethod
     def from_dict(cls, client: WhatsApp, value: dict):
         message = value['messages'][0]
         return cls(
             _client=client,
             id=message['id'],
-            metadata=Metadata(**value['metadata']),
+            metadata=Metadata.from_dict(**value['metadata']),
             type=MessageType(message['type']),
             from_user=User.from_dict(value['contacts'][0]),
             timestamp=datetime.fromtimestamp(int(message['timestamp'])),
             reply_to_message=ReplyToMessage.from_dict(message['context']),
             data=message['interactive']['list_reply']['id'],
             title=message['interactive']['list_reply']['title'],
             description=message['interactive']['list_reply'].get('description')
@@ -1034,24 +1015,24 @@
         metadata: The metadata of the message (to which phone number it was sent).
         status: The status of the message.
         timestamp: The timestamp when the status was updated.
         from_user: The user who the message was sent to.
         error: The error that occurred (if status is ``failed``).
     """
     status: MessageStatusType
-    error: WhatsAppApiError | None
+    error: WhatsAppError | None
 
     @classmethod
     def from_dict(cls, client: WhatsApp, value: dict):
         status = value['statuses'][0]
         status_type = MessageStatusType(status['status'])
         return cls(
             _client=client,
             id=status['id'],
-            metadata=Metadata(**value['metadata']),
+            metadata=Metadata.from_dict(**value['metadata']),
             type=MessageType.MESSAGE_STATUS,
             status=status_type,
             timestamp=datetime.fromtimestamp(int(status['timestamp'])),
             from_user=User(wa_id=status['recipient_id'], name=None),
-            error=WhatsAppApiError.from_incoming_error(status['errors'][0])
+            error=WhatsAppError.from_incoming_error(status['errors'][0])
             if status_type == MessageStatusType.FAILED else None
         )
```

## pywa/webhook.py

```diff
@@ -89,10 +89,10 @@
             else:
                 if value["messages"][0]["interactive"]["type"] == "button_reply":
                     return CallbackButton.from_dict(client=client, value=value), "button"
                 elif value["messages"][0]["interactive"]["type"] == "list_reply":
                     return CallbackSelection.from_dict(client=client, value=value), "selection"
 
         elif 'statuses' in value:
-            return MessageStatus.from_dict(client=client, value=value), "status"
+            return MessageStatus.from_dict(client=client, value=value), "message_status"
         else:
             raise ValueError("Invalid webhook data: " + str(d))
```

## Comparing `pywa-0.0.1rc12.dist-info/LICENSE` & `pywa-0.0.1rc13.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc12.dist-info/METADATA` & `pywa-0.0.1rc13.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc12
+Version: 0.0.1rc13
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
@@ -21,15 +21,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Provides-Extra: fastapi
 Requires-Dist: fastapi ; extra == 'fastapi'
-Requires-Dist: uvicorn ; extra == 'fastapi'
+Requires-Dist: uvicorn[standard] ; extra == 'fastapi'
 Provides-Extra: flask
 Requires-Dist: flask ; extra == 'flask'
 
 .. image:: https://i.imgur.com/hbGP0rW.png
   :width: 200
   :alt: PyWa Logo
 .. end-logo
```

