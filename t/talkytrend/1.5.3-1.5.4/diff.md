# Comparing `tmp/talkytrend-1.5.3.tar.gz` & `tmp/talkytrend-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.5.3.tar", max compression
+gzip compressed data, was "talkytrend-1.5.4.tar", max compression
```

## Comparing `talkytrend-1.5.3.tar` & `talkytrend-1.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-27 20:17:36.741904 talkytrend-1.5.3/LICENSE
--rw-r--r--   0        0        0     2190 2023-06-27 20:17:36.741904 talkytrend-1.5.3/README.md
--rw-r--r--   0        0        0     2178 2023-06-27 20:17:37.425910 talkytrend-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-27 20:17:37.425910 talkytrend-1.5.3/talkytrend/__init__.py
--rw-r--r--   0        0        0      708 2023-06-27 20:17:36.741904 talkytrend-1.5.3/talkytrend/config.py
--rw-r--r--   0        0        0     1642 2023-06-27 20:17:36.741904 talkytrend-1.5.3/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     6426 2023-06-27 20:17:36.741904 talkytrend-1.5.3/talkytrend/main.py
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-02 17:06:56.433899 talkytrend-1.5.4/LICENSE
+-rw-r--r--   0        0        0     2190 2023-07-02 17:06:56.433899 talkytrend-1.5.4/README.md
+-rw-r--r--   0        0        0     2178 2023-07-02 17:06:57.181905 talkytrend-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-02 17:06:57.181905 talkytrend-1.5.4/talkytrend/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-02 17:06:56.433899 talkytrend-1.5.4/talkytrend/config.py
+-rw-r--r--   0        0        0     1642 2023-07-02 17:06:56.433899 talkytrend-1.5.4/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     6465 2023-07-02 17:06:56.433899 talkytrend-1.5.4/talkytrend/main.py
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 talkytrend-1.5.4/PKG-INFO
```

### Comparing `talkytrend-1.5.3/LICENSE` & `talkytrend-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.3/README.md` & `talkytrend-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.3/pyproject.toml` & `talkytrend-1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.5.3"
+version = "1.5.4"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.5.3/talkytrend/config.py` & `talkytrend-1.5.4/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.3/talkytrend/default_settings.toml` & `talkytrend-1.5.4/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.5.3/talkytrend/main.py` & `talkytrend-1.5.4/talkytrend/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,28 +120,30 @@
                     if is_usd_high_impact(event) or is_all_high_impact(event):
                         return format_event(event)
                     if is_opec_or_fomc(event):
                         return format_event(event)
         return None
 
 
-    
+
     async def fetch_key_news(self):
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(self.news_url, timeout=10) as response:
                     data = await response.json()
                     articles = data.get('articles', [])
                     key_news = [{'title': article['title'], 'url': article['url']} for article in articles]
                     last_item = key_news[-1]
-                    return f"📰 [{last_item['title']}]({last_item['url']})"
+                    return f"📰 <a href={last_item['url']}>{last_item['title']}</a>"
+                    
         except aiohttp.ClientError as error:
             self.logger.error("news %s", error)
             return None
 
+            
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
         return any(event.startswith(current_date) for event in event_dates)
 
 
     async def scanner(self):
```

### Comparing `talkytrend-1.5.3/PKG-INFO` & `talkytrend-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.5.3
+Version: 1.5.4
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

