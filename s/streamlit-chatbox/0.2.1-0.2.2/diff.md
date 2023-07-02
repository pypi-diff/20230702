# Comparing `tmp/streamlit_chatbox-0.2.1-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4845 bytes, number of entries: 5
+Zip file size: 5003 bytes, number of entries: 5
 -rw-rw-rw-  2.0 fat    10013 b- defN 23-Jun-28 13:06 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     2057 b- defN 23-Jun-28 13:09 streamlit_chatbox-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-28 13:09 streamlit_chatbox-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-28 13:09 streamlit_chatbox-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      425 b- defN 23-Jun-28 13:09 streamlit_chatbox-0.2.1.dist-info/RECORD
-5 files, 12605 bytes uncompressed, 4049 bytes compressed:  67.9%
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      425 b- defN 23-Jul-02 14:44 streamlit_chatbox-0.2.2.dist-info/RECORD
+5 files, 12889 bytes uncompressed, 4207 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: streamlit_chatbox/__init__.py
 Comment: 
 
-Filename: streamlit_chatbox-0.2.1.dist-info/METADATA
+Filename: streamlit_chatbox-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-0.2.1.dist-info/WHEEL
+Filename: streamlit_chatbox-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-0.2.1.dist-info/top_level.txt
+Filename: streamlit_chatbox-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-0.2.1.dist-info/RECORD
+Filename: streamlit_chatbox-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `streamlit_chatbox-0.2.1.dist-info/METADATA` & `streamlit_chatbox-0.2.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 0.2.1
+Version: 0.2.2
 Summary: A chat box used in streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit
 
+# Attention!
+
+Since version 1.24.0 streamlit provides official elements to [build conversational apps](https://docs.streamlit.io/knowledge-base/tutorials/build-conversational-apps).
+
+The new elements are more flexible, extensible and better supported, I would suggest to use them. 
+
+
 # Chatbox component for streamlit
 
 A Streamlit component to show chat messages.
 
 ## Features
 
 - user can custom the bg_color and icon of message senders.
```

