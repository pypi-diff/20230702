# Comparing `tmp/openplugin-py-0.0.1.tar.gz` & `tmp/openplugin-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-py-0.0.1.tar", last modified: Fri Jun 30 09:41:04 2023, max compression
+gzip compressed data, was "openplugin-py-0.0.2.tar", last modified: Sun Jul  2 15:55:14 2023, max compression
```

## Comparing `openplugin-py-0.0.1.tar` & `openplugin-py-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-30 09:41:04.204691 openplugin-py-0.0.1/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.1/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     1762 2023-06-30 09:41:04.204568 openplugin-py-0.0.1/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      680 2023-06-30 09:26:12.000000 openplugin-py-0.0.1/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-30 09:41:04.201655 openplugin-py-0.0.1/openplugin/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-06-29 11:10:13.000000 openplugin-py-0.0.1/openplugin/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-30 09:41:04.202047 openplugin-py-0.0.1/openplugin/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.1/openplugin/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2820 2023-06-30 09:22:51.000000 openplugin-py-0.0.1/openplugin/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-30 09:41:04.202317 openplugin-py-0.0.1/openplugin/install/
--rw-r--r--   0 4paradigm   (501) staff       (20)     2190 2023-06-30 09:23:05.000000 openplugin-py-0.0.1/openplugin/install/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-30 09:41:04.202549 openplugin-py-0.0.1/openplugin/run/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3319 2023-06-30 09:22:51.000000 openplugin-py-0.0.1/openplugin/run/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-30 09:41:04.203638 openplugin-py-0.0.1/openplugin/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.1/openplugin/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.1/openplugin/utils/app_util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.1/openplugin/utils/errors.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1868 2023-06-30 09:22:51.000000 openplugin-py-0.0.1/openplugin/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-06-30 09:41:04.204394 openplugin-py-0.0.1/openplugin_py.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1762 2023-06-30 09:41:04.000000 openplugin-py-0.0.1/openplugin_py.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      490 2023-06-30 09:41:04.000000 openplugin-py-0.0.1/openplugin_py.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-06-30 09:41:04.000000 openplugin-py-0.0.1/openplugin_py.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-06-30 09:41:04.000000 openplugin-py-0.0.1/openplugin_py.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-06-30 09:41:04.000000 openplugin-py-0.0.1/openplugin_py.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-06-30 09:41:04.000000 openplugin-py-0.0.1/openplugin_py.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-06-30 09:41:04.204731 openplugin-py-0.0.1/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.1/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.594420 openplugin-py-0.0.2/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.2/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3244 2023-07-02 15:55:14.594259 openplugin-py-0.0.2/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2163 2023-07-02 15:40:39.000000 openplugin-py-0.0.2/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.590229 openplugin-py-0.0.2/openplugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-02 15:40:49.000000 openplugin-py-0.0.2/openplugin/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.590595 openplugin-py-0.0.2/openplugin/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.2/openplugin/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.590816 openplugin-py-0.0.2/openplugin/install/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2464 2023-07-02 15:52:06.000000 openplugin-py-0.0.2/openplugin/install/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.591053 openplugin-py-0.0.2/openplugin/run/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3342 2023-07-02 14:58:56.000000 openplugin-py-0.0.2/openplugin/run/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.592049 openplugin-py-0.0.2/openplugin/template/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/base_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/json_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.2/openplugin/template/yaml_template.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.593178 openplugin-py-0.0.2/openplugin/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.2/openplugin/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.2/openplugin/utils/app_util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.2/openplugin/utils/errors.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1868 2023-06-30 09:22:51.000000 openplugin-py-0.0.2/openplugin/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-02 15:55:14.594042 openplugin-py-0.0.2/openplugin_py.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3244 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)      662 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-02 15:55:14.000000 openplugin-py-0.0.2/openplugin_py.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-02 15:55:14.594466 openplugin-py-0.0.2/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.2/setup.py
```

### Comparing `openplugin-py-0.0.1/LICENSE` & `openplugin-py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.1/openplugin/__init__.py` & `openplugin-py-0.0.2/openplugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "openplugin"
-__VERSION__ = "v0.0.1"
+__VERSION__ = "v0.0.2"
 __DESCRIPTION__ = "Toolkit and Collection for Plugins of Large Language Models"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `openplugin-py-0.0.1/openplugin/cli/__init__.py` & `openplugin-py-0.0.2/openplugin/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.1/openplugin/cli/cli.py` & `openplugin-py-0.0.2/openplugin/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,29 @@
     from openplugin.install import uninstall_plugin
 
     uninstall_plugin(plugin_name)
 
 
 @cli.command()
 @click.argument("plugin_name")
+def reinstall(plugin_name):
+    from openplugin.install import reinstall_plugin
+
+    reinstall_plugin(plugin_name)
+
+
+@cli.command()
+def list():
+    from openplugin.install import list_plugins
+
+    list_plugins()
+
+
+@cli.command()
+@click.argument("plugin_name")
 @click.option(
     "--host",
     type=str,
     default="0.0.0.0",
     help="Host to run the plugin.",
 )
 @click.option(
```

### Comparing `openplugin-py-0.0.1/openplugin/install/__init__.py` & `openplugin-py-0.0.2/openplugin/install/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,7 +59,19 @@
         print("Plugin {} not installed!".format(plugin_name))
         return True
 
     plugin_path = get_plugin_directory() / plugin_name
     if plugin_path.exists() and plugin_path.is_dir():
         shutil.rmtree(plugin_path)
     print("Uninstalled plugin: {}!".format(plugin_name))
+
+
+def reinstall_plugin(plugin_name: str) -> bool:
+    uninstall_plugin(plugin_name)
+    return install_plugin(plugin_name)
+
+
+def list_plugins() -> bool:
+    plugin_list = get_plugin_list()
+    print("Installed plugins:")
+    for plugin in plugin_list:
+        print(plugin)
```

### Comparing `openplugin-py-0.0.1/openplugin/run/__init__.py` & `openplugin-py-0.0.2/openplugin/run/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
     print("Running plugin: {} on {}:{}".format(plugin_name, host, port))
 
     ips = set()
     outip = getIp()
     if outip is not None:
         ips.add(outip)
+    ips.add("0.0.0.0")
     adapters = ifaddr.get_adapters()
 
     for adapter in adapters:
         # print("IPs of network adapter " + adapter.nice_name)
         for ip in adapter.ips:
             # print("   %s/%s" % (ip.ip, ip.network_prefix))
             ip_address = ip.ip
```

### Comparing `openplugin-py-0.0.1/openplugin/utils/__init__.py` & `openplugin-py-0.0.2/openplugin/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.1/openplugin/utils/app_util.py` & `openplugin-py-0.0.2/openplugin/utils/app_util.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.1/openplugin/utils/errors.py` & `openplugin-py-0.0.2/openplugin/utils/errors.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.1/openplugin/utils/util.py` & `openplugin-py-0.0.2/openplugin/utils/util.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.1/setup.py` & `openplugin-py-0.0.2/setup.py`

 * *Files identical despite different names*

