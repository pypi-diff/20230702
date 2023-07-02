# Comparing `tmp/spice_agent-0.1.0.tar.gz` & `tmp/spice_agent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_agent-0.1.0.tar", max compression
+gzip compressed data, was "spice_agent-0.1.1.tar", max compression
```

## Comparing `spice_agent-0.1.0.tar` & `spice_agent-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0     1901 2023-07-01 19:35:57.673053 spice_agent-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/__init__.py
--rw-r--r--   0        0        0       21 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/__version__.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/auth/__init__.py
--rw-r--r--   0        0        0     1024 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/auth/actions.py
--rw-r--r--   0        0        0     2761 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/auth/commands.py
--rw-r--r--   0        0        0     1869 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/cli.py
--rw-r--r--   0        0        0     4947 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/client.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/daemons/__init__.py
--rw-r--r--   0        0        0     2250 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/daemons/actions.py
--rw-r--r--   0        0        0     1508 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/daemons/commands.py
--rw-r--r--   0        0        0     3943 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/daemons/launch_agents.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/graphql/documents/__init__.py
--rw-r--r--   0        0        0     1196 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/graphql/documents/authentication.gql
--rw-r--r--   0        0        0     1504 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/graphql/sdk.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/hardware/__init__.py
--rw-r--r--   0        0        0     7844 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/hardware/actions.py
--rw-r--r--   0        0        0     1070 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/hardware/commands.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/inference/__init__.py
--rw-r--r--   0        0        0     6273 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/inference/actions.py
--rw-r--r--   0        0        0     1055 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/inference/commands.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/tests/__init__.py
--rw-r--r--   0        0        0      548 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/tests/test_version.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/training/__init__.py
--rw-r--r--   0        0        0    38069 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/training/actions.py
--rw-r--r--   0        0        0       97 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/training/commands.py
--rw-r--r--   0        0        0     7269 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/uploader/actions.py
--rw-r--r--   0        0        0     1823 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/utils/config.py
--rw-r--r--   0        0        0      252 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/utils/printer.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/utils/updates.py
--rw-r--r--   0        0        0        0 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/worker/__init__.py
--rw-r--r--   0        0        0     8999 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/worker/actions.py
--rw-r--r--   0        0        0      397 2023-07-01 19:35:57.673053 spice_agent-0.1.0/spice_agent/worker/commands.py
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 spice_agent-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-07-02 16:22:14.915096 spice_agent-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/auth/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/auth/actions.py
+-rw-r--r--   0        0        0     2761 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/auth/commands.py
+-rw-r--r--   0        0        0     1869 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/cli.py
+-rw-r--r--   0        0        0     5033 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/client.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/daemons/__init__.py
+-rw-r--r--   0        0        0     2500 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/daemons/actions.py
+-rw-r--r--   0        0        0     1508 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/daemons/commands.py
+-rw-r--r--   0        0        0     4302 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/daemons/launch_agents.py
+-rw-r--r--   0        0        0     4982 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/daemons/launch_service.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/graphql/documents/__init__.py
+-rw-r--r--   0        0        0     1196 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/graphql/documents/authentication.gql
+-rw-r--r--   0        0        0     1504 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/graphql/sdk.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/hardware/__init__.py
+-rw-r--r--   0        0        0     7844 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/hardware/actions.py
+-rw-r--r--   0        0        0     1070 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/hardware/commands.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/inference/__init__.py
+-rw-r--r--   0        0        0     6273 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/inference/actions.py
+-rw-r--r--   0        0        0     1055 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/inference/commands.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/tests/__init__.py
+-rw-r--r--   0        0        0      555 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/tests/test_version.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/training/__init__.py
+-rw-r--r--   0        0        0    38069 2023-07-02 16:22:14.915096 spice_agent-0.1.1/spice_agent/training/actions.py
+-rw-r--r--   0        0        0       97 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/training/commands.py
+-rw-r--r--   0        0        0     7269 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/uploader/actions.py
+-rw-r--r--   0        0        0     1823 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/utils/config.py
+-rw-r--r--   0        0        0      252 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/utils/printer.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/utils/updates.py
+-rw-r--r--   0        0        0     1437 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/utils/version.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/worker/__init__.py
+-rw-r--r--   0        0        0     8999 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/worker/actions.py
+-rw-r--r--   0        0        0      397 2023-07-02 16:22:14.919096 spice_agent-0.1.1/spice_agent/worker/commands.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 spice_agent-0.1.1/PKG-INFO
```

### Comparing `spice_agent-0.1.0/pyproject.toml` & `spice_agent-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_agent"
-version = "0.1.0"
+version = "0.1.1"
 description = "spice agent"
 authors = ["Dylan Stein <dylan@spice.cloud>", "Ankush Patel <ankush@spice.cloud>"]
 license = ""
 
 [tool.poetry.dependencies]
 python = "^3.11.3"
 gql = "^3.4.1"
@@ -20,14 +20,15 @@
 datasets = "^2.13.1"
 boto3 = "^1.26.165"
 evaluate = "^0.4.0"
 scikit-learn = "^1.2.2"
 accelerate = "^0.20.3"
 torchvision = "^0.15.2"
 diffusers = "^0.17.1"
+outdated = "^0.2.2"
 
 [tool.poetry.dev-dependencies]
 ruff = "^0.0.275"
 black = "^23.3.0"
 prospector = "^1.10.2"
 ipython = "^8.9.0"
 ipdb = "^0.13.11"
```

### Comparing `spice_agent-0.1.0/spice_agent/auth/actions.py` & `spice_agent-0.1.1/spice_agent/auth/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/auth/commands.py` & `spice_agent-0.1.1/spice_agent/auth/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/cli.py` & `spice_agent-0.1.1/spice_agent/cli.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/client.py` & `spice_agent-0.1.1/spice_agent/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 from spice_agent.daemons.actions import Daemons
 from spice_agent.graphql.sdk import create_session
 from spice_agent.hardware.actions import Hardware
 from spice_agent.inference.actions import Inference
 from spice_agent.training.actions import Training
 from spice_agent.uploader.actions import Uploader
 from spice_agent.utils.config import read_config_file
+from spice_agent.utils.version import update_if_outdated
 from spice_agent.worker.actions import Worker
 
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
 import torch  # noqa
 
 
 class Spice:
     def __init__(self, host: str = "api.spice.cloud", DEBUG: bool = False) -> None:
+        update_if_outdated()
         self.host = host
         self.DEBUG = DEBUG
 
         logger = logging.getLogger("spice")
         logger.setLevel(logging.INFO)
         sh = logging.StreamHandler(sys.stdout)
         formatter = logging.Formatter(
```

### Comparing `spice_agent-0.1.0/spice_agent/daemons/actions.py` & `spice_agent-0.1.1/spice_agent/daemons/actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,70 +4,83 @@
     full_launch_agent_install,
     full_launch_agent_uninstall,
     start_launch_agent,
     stop_launch_agent,
     view_launch_agent_logs,
 )
 
+from spice_agent.daemons.launch_service import (
+    full_service_install,
+    full_service_uninstall,
+    start_service,
+    stop_service,
+    view_service_logs,
+)
+
 
 class Daemons:
     def __init__(self, spice) -> None:
         self.spice = spice
         self.os_family = platform.system()
 
     def install(self):
         result = True
         if self.os_family == "Darwin":
             full_launch_agent_install()
         elif self.os_family == "Linux":
-            print("Not Implemented")
             if "WSL2" in platform.platform():
+                full_service_install()
+            else:
                 print("Not Implemented")
         elif self.os_family == "Windows":
             print("Not Implemented")
         return result
 
     def uninstall(self):
         result = True
         if self.os_family == "Darwin":
             full_launch_agent_uninstall()
         elif self.os_family == "Linux":
-            print("Not Implemented")
             if "WSL2" in platform.platform():
+                full_service_uninstall()
+            else:
                 print("Not Implemented")
         elif self.os_family == "Windows":
             print("Not Implemented")
         return result
 
     def stop(self) -> bool:
         result = True
         if self.os_family == "Darwin":
             result = stop_launch_agent()
         elif self.os_family == "Linux":
-            print("Not Implemented")
             if "WSL2" in platform.platform():
+                stop_service()
+            else:
                 print("Not Implemented")
         elif self.os_family == "Windows":
             print("Not Implemented")
         return result
 
     def start(self) -> bool:
         result = True
         if self.os_family == "Darwin":
             result = start_launch_agent()
         elif self.os_family == "Linux":
-            print("Not Implemented")
             if "WSL2" in platform.platform():
+                start_service()
+            else:
                 print("Not Implemented")
         elif self.os_family == "Windows":
             print("Not Implemented")
         return result
 
     def logs(self):
         if self.os_family == "Darwin":
             view_launch_agent_logs()
         elif self.os_family == "Linux":
-            print("Not Implemented")
             if "WSL2" in platform.platform():
+                view_service_logs()
+            else:
                 print("Not Implemented")
         elif self.os_family == "Windows":
             print("Not Implemented")
```

### Comparing `spice_agent-0.1.0/spice_agent/daemons/commands.py` & `spice_agent-0.1.1/spice_agent/daemons/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/daemons/launch_agents.py` & `spice_agent-0.1.1/spice_agent/daemons/launch_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,25 @@
         subprocess.check_output(load_new_plist.split(" "))
         return True
     except subprocess.CalledProcessError as exception:
         print("load_launch_agent: ", exception)
         return False
 
 
+def create_stdout_file():
+    if not SPICE_LAUNCH_AGENT_LOGS.exists():
+        SPICE_LAUNCH_AGENT_LOGS.parent.mkdir(parents=True, exist_ok=True)
+        SPICE_LAUNCH_AGENT_LOGS.touch()
+
+
+def delete_stdout_file():
+    if SPICE_LAUNCH_AGENT_LOGS.exists():
+        SPICE_LAUNCH_AGENT_LOGS.unlink()
+
+
 def populate_fresh_launch_agent():
     SPICE_LAUNCH_AGENT_LOGS.parent.mkdir(parents=True, exist_ok=True)
     SPICE_LAUNCH_AGENT_LOGS.touch()
 
     if SPICE_LAUNCH_AGENT_FILEPATH.exists():
         SPICE_LAUNCH_AGENT_FILEPATH.unlink()
     SPICE_LAUNCH_AGENT_FILEPATH.parent.mkdir(parents=True, exist_ok=True)
@@ -115,16 +126,18 @@
     os.system(follow_logs)
 
 
 def full_launch_agent_install():
     stop_launch_agent()
     unload_launch_agent()
     populate_fresh_launch_agent()
+    create_stdout_file()
     load_launch_agent()
     start_launch_agent()
 
 
 def full_launch_agent_uninstall():
     stop_launch_agent()
     unload_launch_agent()
-    SPICE_LAUNCH_AGENT_FILEPATH.unlink()
-    SPICE_LAUNCH_AGENT_LOGS.unlink()
+    if SPICE_LAUNCH_AGENT_FILEPATH.exists():
+        SPICE_LAUNCH_AGENT_FILEPATH.unlink()
+    delete_stdout_file()
```

### Comparing `spice_agent-0.1.0/spice_agent/graphql/documents/authentication.gql` & `spice_agent-0.1.1/spice_agent/graphql/documents/authentication.gql`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/graphql/sdk.py` & `spice_agent-0.1.1/spice_agent/graphql/sdk.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/hardware/actions.py` & `spice_agent-0.1.1/spice_agent/hardware/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/hardware/commands.py` & `spice_agent-0.1.1/spice_agent/hardware/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/inference/actions.py` & `spice_agent-0.1.1/spice_agent/inference/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/inference/commands.py` & `spice_agent-0.1.1/spice_agent/inference/commands.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/training/actions.py` & `spice_agent-0.1.1/spice_agent/training/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/uploader/actions.py` & `spice_agent-0.1.1/spice_agent/uploader/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/utils/config.py` & `spice_agent-0.1.1/spice_agent/utils/config.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/spice_agent/worker/actions.py` & `spice_agent-0.1.1/spice_agent/worker/actions.py`

 * *Files identical despite different names*

### Comparing `spice_agent-0.1.0/PKG-INFO` & `spice_agent-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: spice-agent
-Version: 0.1.0
+Version: 0.1.1
 Summary: spice agent
 Author: Dylan Stein
 Author-email: dylan@spice.cloud
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: accelerate (>=0.20.3,<0.21.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: boto3 (>=1.26.165,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: datasets (>=2.13.1,<3.0.0)
 Requires-Dist: diffusers (>=0.17.1,<0.18.0)
 Requires-Dist: evaluate (>=0.4.0,<0.5.0)
 Requires-Dist: gql (>=3.4.1,<4.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: outdated (>=0.2.2,<0.3.0)
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: sentry-sdk (>=1.24.0,<2.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
```

