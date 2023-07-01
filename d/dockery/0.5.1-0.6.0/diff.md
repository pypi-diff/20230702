# Comparing `tmp/dockery-0.5.1.tar.gz` & `tmp/dockery-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.5.1.tar", last modified: Sat Jul  1 17:00:12 2023, max compression
+gzip compressed data, was "dockery-0.6.0.tar", last modified: Sat Jul  1 22:04:02 2023, max compression
```

## Comparing `dockery-0.5.1.tar` & `dockery-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1082 2023-07-01 17:00:04.260113 dockery-0.5.1/LICENSE
--rw-r--r--   0        0        0     1313 2023-07-01 17:00:04.260113 dockery-0.5.1/README.md
--rw-r--r--   0        0        0      758 2023-07-01 17:00:12.992433 dockery-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/__init__.py
--rw-r--r--   0        0        0     1760 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/custom_widgets.py
--rw-r--r--   0        0        0     6046 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/gui.py
--rw-r--r--   0        0        0     1775 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/images.py
--rw-r--r--   0        0        0     1835 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/logs.py
--rw-r--r--   0        0        0     2767 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/main.py
--rw-r--r--   0        0        0     1742 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/networks.py
--rw-r--r--   0        0        0     1070 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/style.css
--rw-r--r--   0        0        0      881 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/utils.py
--rw-r--r--   0        0        0     1723 2023-07-01 17:00:04.260113 dockery-0.5.1/src/dockery/volumes.py
--rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 dockery-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-01 22:03:55.067526 dockery-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1636 2023-07-01 22:03:55.067526 dockery-0.6.0/README.md
+-rw-r--r--   0        0        0      777 2023-07-01 22:04:02.795653 dockery-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/__init__.py
+-rw-r--r--   0        0        0     1760 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/custom_widgets.py
+-rw-r--r--   0        0        0     6046 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/gui.py
+-rw-r--r--   0        0        0     1775 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/images.py
+-rw-r--r--   0        0        0     1883 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/logs.py
+-rw-r--r--   0        0        0     3738 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/main.py
+-rw-r--r--   0        0        0     1742 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/networks.py
+-rw-r--r--   0        0        0     1070 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/style.css
+-rw-r--r--   0        0        0     1328 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/utils.py
+-rw-r--r--   0        0        0     1723 2023-07-01 22:03:55.067526 dockery-0.6.0/src/dockery/volumes.py
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 dockery-0.6.0/PKG-INFO
```

### Comparing `dockery-0.5.1/LICENSE` & `dockery-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.5.1/README.md` & `dockery-0.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -38,19 +38,38 @@
 
 ```shell
 dockery
 ```
 
 **Warning:** you will probably need to install and run dockery as a root user, or you can add permissions to your user to run docker following [this instructions](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user).
 
-## Extra commands
+## Utils
 
 ```shell
 dockery df
 dockery ps
 dockery volumes
 dockery images
 dockery networks
 dockery stats
 ```
 
-## **Enjoy it!**
+You specify the format output of these commands with the parameter `--format`, e.g:
+
+```shell
+dockery df --format json
+dockery df --format yaml
+```
+
+### Get logs
+
+```shel
+dockery logs {container_name}
+```
+
+You can use the parameter `--stream` to get the logs in real time, e.g:
+
+```shel
+dockery logs {container_name} --stream
+```
+
+### **Enjoy it!**
```

#### html2text {}

```diff
@@ -8,10 +8,14 @@
 4495-b67c-2c57e933bd7d]
 ## Installation ### From source ```shell git clone git@github.com:
 marianocarrazana/dockery.git cd dockery pip install -e . # update only: git
 pull ``` ### From pip ```shell pip install -U dockery ``` ## Usage Run on your
 console: ```shell dockery ``` **Warning:** you will probably need to install
 and run dockery as a root user, or you can add permissions to your user to run
 docker following [this instructions](https://docs.docker.com/engine/install/
-linux-postinstall/#manage-docker-as-a-non-root-user). ## Extra commands
-```shell dockery df dockery ps dockery volumes dockery images dockery networks
-dockery stats ``` ## **Enjoy it!**
+linux-postinstall/#manage-docker-as-a-non-root-user). ## Utils ```shell dockery
+df dockery ps dockery volumes dockery images dockery networks dockery stats ```
+You specify the format output of these commands with the parameter `--format`,
+e.g: ```shell dockery df --format json dockery df --format yaml ``` ### Get
+logs ```shel dockery logs {container_name} ``` You can use the parameter `--
+stream` to get the logs in real time, e.g: ```shel dockery logs
+{container_name} --stream ``` ### **Enjoy it!**
```

### Comparing `dockery-0.5.1/pyproject.toml` & `dockery-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "dockery"
-version = "0.5.1"
+version = "0.6.0"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.28.0",
     "click>=8.1.3",
+    "pyyaml>=6.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `dockery-0.5.1/src/dockery/custom_widgets.py` & `dockery-0.6.0/src/dockery/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.1/src/dockery/gui.py` & `dockery-0.6.0/src/dockery/gui.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.1/src/dockery/images.py` & `dockery-0.6.0/src/dockery/images.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.1/src/dockery/logs.py` & `dockery-0.6.0/src/dockery/logs.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     async def watch_last_log(self, new_log: str):
         self.write(new_log)
 
     @work
     def update_log(self) -> None:
         # Get the last 40 logs(get all logs can be slow)
         logs: bytes = self.container.logs(tail=40)
-        self.last_log = logs.decode()
+        self.last_log = logs.decode("utf-8", errors="ignore")
         # Start streaming logs(since last second)
         for log in self.container.logs(stream=True, since=time.time() - 1):
             if not self.running:
                 # Finish the thread after removing the widget
                 # TODO: it doesn't finish immediately? fix?
                 return None
-            self.last_log = log.decode()
+            self.last_log = log.decode("utf-8", errors="ignore")
 
     def on_unmount(self):
         self.running = False
```

### Comparing `dockery-0.5.1/src/dockery/main.py` & `dockery-0.6.0/src/dockery/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import docker
+from docker import errors
 from docker.models.containers import Container
 from docker.models.volumes import Volume
 from docker.models.images import Image
 from docker.models.networks import Network
 import click
 from rich import print
 
 from .gui import AppGUI
+from .utils import var_dump
 
 default_options = [
     click.option(
         "--server",
         default=None,
         help="Docker server url, for example: unix:///var/run/docker.sock",
     ),
     click.option("--ssh", is_flag=True),
     click.option("--api-version", default="1.35", help="Docker API version"),
+    click.option("--format", "-f", default="yaml", help="Output format"),
 ]
 
 
 def add_options(options):
     def _add_options(func):
         for option in reversed(options):
             func = option(func)
@@ -52,67 +55,87 @@
         run_gui(**kargs)
 
 
 @click.command
 @add_options(default_options)
 def df(**kargs):
     client = get_client(**kargs)
-    print(client.df())
+    var_dump(client.df(), kargs["format"])
 
 
 @click.command
 @add_options(default_options)
 def volumes(**kargs):
     client = get_client(**kargs)
     vlms: list[Volume] = client.volumes.list()  # type: ignore
-    for v in vlms:
-        print(v.attrs)
+    vlm_list = list(map(lambda x: x.attrs, vlms))
+    var_dump(vlm_list, kargs["format"])
 
 
 @click.command
 @add_options(default_options)
 @click.option("--all", "-a", is_flag=True)
 def ps(**kargs):
     client = get_client(**kargs)
     containers: list[Container] = client.containers.list(
-        all=kargs["all"],
+        all=kargs["all"]
     )  # type: ignore
-    for c in containers:
-        print(c.attrs)
+    con_list = list(map(lambda x: x.attrs, containers))
+    var_dump(con_list, kargs["format"])
 
 
 @click.command
 @add_options(default_options)
 def stats(**kargs):
     client = get_client(**kargs)
     containers: list[Container] = client.containers.list(all=True)  # type: ignore
-    for c in containers:
-        print(f"[b]{c.name}:")
-        stats = c.stats(decode=None, stream=False)
-        print(stats)
+    stats = list(map(lambda x: x.stats(stream=False), containers))
+    var_dump(stats, kargs["format"])
 
 
 @click.command
 @add_options(default_options)
 def images(**kargs):
     client = get_client(**kargs)
     imgs: list[Image] = client.images.list()  # type: ignore
-    for i in imgs:
-        print(i.attrs)
+    img_list = list(map(lambda x: x.attrs, imgs))
+    var_dump(img_list, kargs["format"])
+
 
 @click.command
 @add_options(default_options)
 def networks(**kargs):
     client = get_client(**kargs)
     netw: list[Network] = client.networks.list()  # type: ignore
-    for i in netw:
-        print(i.attrs)
+    net_list = list(map(lambda x: x.attrs, netw))
+    var_dump(net_list, kargs["format"])
+
+
+@click.command
+@add_options(default_options)
+@click.argument("container")
+@click.option("--stream", is_flag=True)
+def logs(**kargs):
+    client = get_client(**kargs)
+    try:
+        container: Container = client.containers.get(kargs["container"])  # type: ignore
+    except errors.NotFound:
+        print(f"Container [b]{kargs['container']}[/] not found")
+    else:
+        if kargs["stream"]:
+            for log in container.logs(stream=True):
+                print(log.decode("utf-8", errors="ignore"), end="")
+        else:
+            logs: bytes = container.logs()
+            print(logs.decode("utf-8", errors="ignore"))
+
 
 main.add_command(df)
 main.add_command(volumes)
 main.add_command(ps)
 main.add_command(stats)
 main.add_command(images)
 main.add_command(networks)
+main.add_command(logs)
 
 if __name__ == "__main__":
     main()
```

### Comparing `dockery-0.5.1/src/dockery/networks.py` & `dockery-0.6.0/src/dockery/networks.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.1/src/dockery/style.css` & `dockery-0.6.0/src/dockery/style.css`

 * *Files identical despite different names*

### Comparing `dockery-0.5.1/src/dockery/utils.py` & `dockery-0.6.0/src/dockery/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+import json
+from typing import Any, Literal
+from rich.console import Console
+from rich.syntax import Syntax
+import yaml
+
+console = Console()
+
+
 def get_cpu_usage(stats: dict) -> float:
     cpu_stats = stats["cpu_stats"]
     precpu_stats = stats["precpu_stats"]
     delta = (
         cpu_stats["cpu_usage"]["total_usage"] - precpu_stats["cpu_usage"]["total_usage"]
     )
     system_delta = cpu_stats.get("system_cpu_usage", 0) - precpu_stats.get(
@@ -24,7 +33,16 @@
         mem_stats["usage"]
         - mem_stats["stats"].get("cache", 0)
         + mem_stats["stats"]["active_file"]
     )
     limit = stats["memory_stats"]["limit"]
     percentage = mem_used / limit * 100
     return percentage
+
+
+def var_dump(obj: Any, syntax: Literal["json", "yaml"] = "yaml"):
+    if syntax == "yaml":
+        text_obj = yaml.safe_dump(obj, indent=2)
+    elif syntax == "json":
+        text_obj = json.dumps(obj, default=str, indent=2)
+    out = Syntax(text_obj, syntax, theme="ansi_dark")
+    console.print(out)
```

### Comparing `dockery-0.5.1/src/dockery/volumes.py` & `dockery-0.6.0/src/dockery/volumes.py`

 * *Files identical despite different names*

### Comparing `dockery-0.5.1/PKG-INFO` & `dockery-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.5.1
+Version: 0.6.0
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
 Project-URL: Bug tracker, https://github.com/marianocarrazana/dockery/issues
 Project-URL: Source code, https://github.com/marianocarrazana/dockery
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
 Requires-Dist: textual>=0.28.0
 Requires-Dist: click>=8.1.3
+Requires-Dist: pyyaml>=6.0
 Description-Content-Type: text/markdown
 
 # dockery
 
 Graphical interface for Docker in your console
 
 [![Release](https://github.com/marianocarrazana/dockery/actions/workflows/release.yml/badge.svg)](https://github.com/marianocarrazana/dockery/actions/workflows/release.yml)
@@ -52,19 +53,38 @@
 
 ```shell
 dockery
 ```
 
 **Warning:** you will probably need to install and run dockery as a root user, or you can add permissions to your user to run docker following [this instructions](https://docs.docker.com/engine/install/linux-postinstall/#manage-docker-as-a-non-root-user).
 
-## Extra commands
+## Utils
 
 ```shell
 dockery df
 dockery ps
 dockery volumes
 dockery images
 dockery networks
 dockery stats
 ```
 
-## **Enjoy it!**
+You specify the format output of these commands with the parameter `--format`, e.g:
+
+```shell
+dockery df --format json
+dockery df --format yaml
+```
+
+### Get logs
+
+```shel
+dockery logs {container_name}
+```
+
+You can use the parameter `--stream` to get the logs in real time, e.g:
+
+```shel
+dockery logs {container_name} --stream
+```
+
+### **Enjoy it!**
```

#### html2text {}

```diff
@@ -1,24 +1,28 @@
-Metadata-Version: 2.1 Name: dockery Version: 0.5.1 Summary: Graphical interface
+Metadata-Version: 2.1 Name: dockery Version: 0.6.0 Summary: Graphical interface
 for Docker in your console Author-Email: Mariano Carrazana
 gmail.com> License: MIT Project-URL: Bug tracker, https://github.com/
 marianocarrazana/dockery/issues Project-URL: Source code, https://github.com/
 marianocarrazana/dockery Requires-Python: >=3.9 Requires-Dist: docker>=6.1.3
-Requires-Dist: textual>=0.28.0 Requires-Dist: click>=8.1.3 Description-Content-
-Type: text/markdown # dockery Graphical interface for Docker in your console [!
-[Release](https://github.com/marianocarrazana/dockery/actions/workflows/
-release.yml/badge.svg)](https://github.com/marianocarrazana/dockery/actions/
-workflows/release.yml)
+Requires-Dist: textual>=0.28.0 Requires-Dist: click>=8.1.3 Requires-Dist:
+pyyaml>=6.0 Description-Content-Type: text/markdown # dockery Graphical
+interface for Docker in your console [![Release](https://github.com/
+marianocarrazana/dockery/actions/workflows/release.yml/badge.svg)](https://
+github.com/marianocarrazana/dockery/actions/workflows/release.yml)
 [https://github.com/marianocarrazana/  [https://github.com/marianocarrazana/
 dockery/assets/17238076/bcff22c9-898c- dockery/assets/17238076/0da0c13c-d84d-
 4877-adac-ddf2e58007c4]                4e8a-8b6f-a0d779c2d98d]
 [https://github.com/marianocarrazana/dockery/assets/17238076/c991ff4b-eebf-
 4495-b67c-2c57e933bd7d]
 ## Installation ### From source ```shell git clone git@github.com:
 marianocarrazana/dockery.git cd dockery pip install -e . # update only: git
 pull ``` ### From pip ```shell pip install -U dockery ``` ## Usage Run on your
 console: ```shell dockery ``` **Warning:** you will probably need to install
 and run dockery as a root user, or you can add permissions to your user to run
 docker following [this instructions](https://docs.docker.com/engine/install/
-linux-postinstall/#manage-docker-as-a-non-root-user). ## Extra commands
-```shell dockery df dockery ps dockery volumes dockery images dockery networks
-dockery stats ``` ## **Enjoy it!**
+linux-postinstall/#manage-docker-as-a-non-root-user). ## Utils ```shell dockery
+df dockery ps dockery volumes dockery images dockery networks dockery stats ```
+You specify the format output of these commands with the parameter `--format`,
+e.g: ```shell dockery df --format json dockery df --format yaml ``` ### Get
+logs ```shel dockery logs {container_name} ``` You can use the parameter `--
+stream` to get the logs in real time, e.g: ```shel dockery logs
+{container_name} --stream ``` ### **Enjoy it!**
```

