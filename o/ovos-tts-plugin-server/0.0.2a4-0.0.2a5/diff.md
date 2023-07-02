# Comparing `tmp/ovos-tts-plugin-server-0.0.2a4.tar.gz` & `tmp/ovos-tts-plugin-server-0.0.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-plugin-server-0.0.2a4.tar", last modified: Mon Jun 26 18:25:36 2023, max compression
+gzip compressed data, was "ovos-tts-plugin-server-0.0.2a5.tar", last modified: Sun Jul  2 20:33:10 2023, max compression
```

## Comparing `ovos-tts-plugin-server-0.0.2a4.tar` & `ovos-tts-plugin-server-0.0.2a5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-06-26 18:25:31.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-26 18:25:31.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:25:36.000000 ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:25:36.130401 ovos-tts-plugin-server-0.0.2a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3279 2023-06-26 18:25:31.000000 ovos-tts-plugin-server-0.0.2a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:33:10.499973 ovos-tts-plugin-server-0.0.2a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-02 20:33:10.499973 ovos-tts-plugin-server-0.0.2a5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:33:10.495973 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1937 2023-07-02 20:33:06.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-02 20:33:06.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:33:10.499973 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-02 20:33:10.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-02 20:33:10.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:33:10.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-02 20:33:10.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 20:33:10.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 20:33:10.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:33:10.000000 ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 20:33:10.499973 ovos-tts-plugin-server-0.0.2a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3279 2023-07-02 20:33:06.000000 ovos-tts-plugin-server-0.0.2a5/setup.py
```

### Comparing `ovos-tts-plugin-server-0.0.2a4/PKG-INFO` & `ovos-tts-plugin-server-0.0.2a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-server
-Version: 0.0.2a4
+Version: 0.0.2a5
 Summary: ovos tts server plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft OpenVoiceOS OVOS plugin tts
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-tts-plugin-server-0.0.2a4/ovos_tts_plugin_server.egg-info/PKG-INFO` & `ovos-tts-plugin-server-0.0.2a5/ovos_tts_plugin_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-server
-Version: 0.0.2a4
+Version: 0.0.2a5
 Summary: ovos tts server plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft OpenVoiceOS OVOS plugin tts
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ovos-tts-plugin-server-0.0.2a4/setup.py` & `ovos-tts-plugin-server-0.0.2a5/setup.py`

 * *Files identical despite different names*

