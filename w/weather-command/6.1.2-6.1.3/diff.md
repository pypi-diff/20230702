# Comparing `tmp/weather_command-6.1.2.tar.gz` & `tmp/weather_command-6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_command-6.1.2.tar", max compression
+gzip compressed data, was "weather_command-6.1.3.tar", max compression
```

## Comparing `weather_command-6.1.2.tar` & `weather_command-6.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-06-25 14:37:08.202663 weather_command-6.1.2/LICENSE
--rw-r--r--   0        0        0     3393 2023-06-25 14:37:08.202663 weather_command-6.1.2/README.md
--rw-r--r--   0        0        0     1793 2023-06-25 14:37:08.202663 weather_command-6.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/__init__.py
--rw-r--r--   0        0        0       95 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/__main__.py
--rw-r--r--   0        0        0    18650 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_builder.py
--rw-r--r--   0        0        0     5340 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_cache.py
--rw-r--r--   0        0        0     5262 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_config.py
--rw-r--r--   0        0        0     2667 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_location.py
--rw-r--r--   0        0        0      473 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_utils.py
--rw-r--r--   0        0        0     2849 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_weather.py
--rw-r--r--   0        0        0      459 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/errors.py
--rw-r--r--   0        0        0     9084 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/main.py
--rw-r--r--   0        0        0        0 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/models/__init__.py
--rw-r--r--   0        0        0      133 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/models/location.py
--rw-r--r--   0        0        0     3053 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/models/weather.py
--rw-r--r--   0        0        0        0 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/py.typed
--rw-r--r--   0        0        0     2816 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/settings_commands.py
--rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 weather_command-6.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-02 01:56:01.355642 weather_command-6.1.3/LICENSE
+-rw-r--r--   0        0        0     3393 2023-07-02 01:56:01.355642 weather_command-6.1.3/README.md
+-rw-r--r--   0        0        0     1789 2023-07-02 01:56:01.359642 weather_command-6.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/__init__.py
+-rw-r--r--   0        0        0       95 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/__main__.py
+-rw-r--r--   0        0        0    18650 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/_builder.py
+-rw-r--r--   0        0        0     5382 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/_cache.py
+-rw-r--r--   0        0        0     5262 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/_config.py
+-rw-r--r--   0        0        0     2652 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/_location.py
+-rw-r--r--   0        0        0      473 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/_utils.py
+-rw-r--r--   0        0        0     2834 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/_weather.py
+-rw-r--r--   0        0        0      459 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/errors.py
+-rw-r--r--   0        0        0     9084 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/models/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/models/location.py
+-rw-r--r--   0        0        0     3053 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/models/weather.py
+-rw-r--r--   0        0        0        0 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/py.typed
+-rw-r--r--   0        0        0     2816 2023-07-02 01:56:01.359642 weather_command-6.1.3/weather_command/settings_commands.py
+-rw-r--r--   0        0        0     4387 1970-01-01 00:00:00.000000 weather_command-6.1.3/PKG-INFO
```

### Comparing `weather_command-6.1.2/LICENSE` & `weather_command-6.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.2/README.md` & `weather_command-6.1.3/README.md`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.2/pyproject.toml` & `weather_command-6.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "weather-command"
-version = "6.1.2"
+version = "6.1.3"
 description = "Command line weather app"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/weather-command"
 homepage = "https://github.com/sanders41/weather-command"
 documentation = "https://github.com/sanders41/weather-command"
 keywords = ["weather", "cli"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "13.4.2"
 httpx = "0.24.1"
-pydantic = "1.10.9"
-camel-converter = {version = "3.0.0", extras = ["pydantic"]}
+pydantic = "2.0"
+camel-converter = {version = "3.0.2", extras = ["pydantic"]}
 typer = "0.9.0"
 tenacity = "8.2.2"
 pyyaml = "6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
-mypy = "1.4.0"
-pre-commit = "2.21.0"
+mypy = "1.4.1"
+pre-commit = "3.3.3"
 pytest = "7.4.0"
 pytest-cov = "4.1.0"
 ruff = "0.0.275"
 tomli = {version = "2.0.1", python = "<3.11"}
 types-pyyaml = "6.0.12.10"
 pytest-asyncio = "0.21.0"
```

### Comparing `weather_command-6.1.2/weather_command/_builder.py` & `weather_command-6.1.3/weather_command/_builder.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.2/weather_command/_cache.py` & `weather_command-6.1.3/weather_command/_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,57 +65,57 @@
         cache_key: str,
         location: Union[Location, None] = None,
         current_weather: Union[CurrentWeather, None] = None,
         one_call_weather: Union[OneCallWeather, None] = None,
         cache_size: int = 5,
     ) -> None:
         def save_cache() -> None:
-            cache: dict[str, Any] = {}
-            location_cache = location.dict() if location else None
+            cache: Dict[str, Any] = {}
+            location_cache = location.model_dump() if location else None
             current_weather_cache = (
                 CurrentWeatherCache(
                     date_time_saved=datetime.now(tz=timezone.utc), current_weather=current_weather
-                ).dict()
+                ).model_dump()
                 if current_weather
                 else None
             )
             one_call_weather_cache = (
                 OneCallWeatherCache(
                     date_time_saved=datetime.now(tz=timezone.utc), one_call_weather=one_call_weather
-                ).dict()
+                ).model_dump()
                 if one_call_weather
                 else None
             )
 
             cache_hit = self.get(cache_key)
 
             if cache_hit:
                 cache[cache_key.lower()] = {
-                    "location": cache_hit.location.dict()
+                    "location": cache_hit.location.model_dump()
                     if cache_hit.location and not location_cache
                     else location_cache,
-                    "currentWeather": cache_hit.current_weather.dict()
+                    "currentWeather": cache_hit.current_weather.model_dump()
                     if cache_hit.current_weather and not current_weather_cache
                     else current_weather_cache,
-                    "oneCallWeather": cache_hit.one_call_weather.dict()
+                    "oneCallWeather": cache_hit.one_call_weather.model_dump()
                     if cache_hit.one_call_weather and not one_call_weather_cache
                     else one_call_weather_cache,
                 }
             else:
                 cache[cache_key.lower()] = {
                     "location": location_cache,
                     "currentWeather": current_weather_cache,
                     "oneCallWeather": one_call_weather_cache,
                 }
 
             if self._cache:
                 for key in self._cache:
                     if key != cache_key:
                         saved_cache = self._cache[key]
-                        cache[key] = saved_cache.dict()
+                        cache[key] = saved_cache.model_dump()
 
             with open(self._cache_file, "w") as f:
                 json.dump(cache, f, cls=DateTimeEncoder)
 
         if not self._cache or len(self._cache.keys()) < cache_size:
             save_cache()
         else:
```

### Comparing `weather_command-6.1.2/weather_command/_config.py` & `weather_command-6.1.3/weather_command/_config.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.2/weather_command/_location.py` & `weather_command-6.1.3/weather_command/_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import sys
 from functools import lru_cache
 
 import httpx
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 from tenacity import retry
 from tenacity.retry import retry_if_exception_type, retry_unless_exception_type
 from tenacity.stop import stop_after_attempt
 from tenacity.wait import wait_fixed
 
 from weather_command._cache import Cache
 from weather_command._config import LOCATION_BASE_URL, console
```

### Comparing `weather_command-6.1.2/weather_command/_weather.py` & `weather_command-6.1.3/weather_command/_weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import sys
 from enum import Enum
 from functools import lru_cache
 
 from httpx import AsyncClient, HTTPStatusError
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 from tenacity import retry
 from tenacity.stop import stop_after_attempt
 from tenacity.wait import wait_fixed
 
 from weather_command._cache import Cache
 from weather_command._config import console
 from weather_command.errors import check_status_error
```

### Comparing `weather_command-6.1.2/weather_command/main.py` & `weather_command-6.1.3/weather_command/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from weather_command._builder import show_current, show_daily, show_hourly
 from weather_command._cache import Cache
 from weather_command._config import console, load_settings
 from weather_command._location import build_location_url, get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_one_call_weather
 
-__version__ = "6.1.2"
+__version__ = "6.1.3"
 
 app = Typer()
 app.add_typer(settings_commands.app, name="settings", help="Manage saved settings.")
 
 
 class ForecastType(str, Enum):
     CURRENT = "current"
```

### Comparing `weather_command-6.1.2/weather_command/models/weather.py` & `weather_command-6.1.3/weather_command/models/weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.2/weather_command/settings_commands.py` & `weather_command-6.1.3/weather_command/settings_commands.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.2/PKG-INFO` & `weather_command-6.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: weather-command
-Version: 6.1.2
+Version: 6.1.3
 Summary: Command line weather app
 Home-page: https://github.com/sanders41/weather-command
 License: MIT
 Keywords: weather,cli
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: camel-converter[pydantic] (==3.0.0)
+Requires-Dist: camel-converter[pydantic] (==3.0.2)
 Requires-Dist: httpx (==0.24.1)
-Requires-Dist: pydantic (==1.10.9)
+Requires-Dist: pydantic (==2.0)
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: rich (==13.4.2)
 Requires-Dist: tenacity (==8.2.2)
 Requires-Dist: typer (==0.9.0)
 Project-URL: Documentation, https://github.com/sanders41/weather-command
 Project-URL: Repository, https://github.com/sanders41/weather-command
 Description-Content-Type: text/markdown
```

