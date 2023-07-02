# Comparing `tmp/caproto-apps-0.0.2.tar.gz` & `tmp/caproto-apps-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caproto-apps-0.0.2.tar", last modified: Wed Jun 28 15:54:36 2023, max compression
+gzip compressed data, was "caproto-apps-0.1.0.tar", last modified: Sun Jul  2 02:20:47 2023, max compression
```

## Comparing `caproto-apps-0.0.2.tar` & `caproto-apps-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-06-28 15:54:36.173908 caproto-apps-0.0.2/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2760 2023-06-28 15:54:36.171917 caproto-apps-0.0.2/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2201 2023-06-28 15:54:15.000000 caproto-apps-0.0.2/README.md
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     1033 2023-06-28 15:54:24.000000 caproto-apps-0.0.2/pyproject.toml
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2023-06-28 15:54:36.173914 caproto-apps-0.0.2/setup.cfg
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-06-28 15:54:36.141926 caproto-apps-0.0.2/src/
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-06-28 15:54:36.160923 caproto-apps-0.0.2/src/caproto_apps.egg-info/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     2760 2023-06-28 15:54:36.000000 caproto-apps-0.0.2/src/caproto_apps.egg-info/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      296 2023-06-28 15:54:36.000000 caproto-apps-0.0.2/src/caproto_apps.egg-info/SOURCES.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2023-06-28 15:54:36.000000 caproto-apps-0.0.2/src/caproto_apps.egg-info/dependency_links.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       55 2023-06-28 15:54:36.000000 caproto-apps-0.0.2/src/caproto_apps.egg-info/requires.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       12 2023-06-28 15:54:36.000000 caproto-apps-0.0.2/src/caproto_apps.egg-info/top_level.txt
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-06-28 15:54:36.166911 caproto-apps-0.0.2/src/caprotoapps/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       30 2023-06-24 19:50:08.000000 caproto-apps-0.0.2/src/caprotoapps/__init__.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    20766 2023-06-28 04:14:07.000000 caproto-apps-0.0.2/src/caprotoapps/alive.py
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2023-06-28 15:54:36.169910 caproto-apps-0.0.2/tests/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    10782 2023-06-28 04:08:59.000000 caproto-apps-0.0.2/tests/test_alive.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.653473 caproto-apps-0.1.0/
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:20:47.652473 caproto-apps-0.1.0/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3177 2023-07-02 02:19:09.000000 caproto-apps-0.1.0/README.md
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1043 2023-07-02 02:10:14.000000 caproto-apps-0.1.0/pyproject.toml
+-rw-------   0 b268176   (2319) xsdspc    (1117)       38 2023-07-02 02:20:47.653473 caproto-apps-0.1.0/setup.cfg
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.647473 caproto-apps-0.1.0/src/
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.650473 caproto-apps-0.1.0/src/caproto_apps.egg-info/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      345 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       62 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/requires.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       12 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/top_level.txt
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.650473 caproto-apps-0.1.0/src/caprotoapps/
+-rw-------   0 b268176   (2319) xsdspc    (1117)       64 2023-07-02 02:10:14.000000 caproto-apps-0.1.0/src/caprotoapps/__init__.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    20766 2023-06-28 04:14:07.000000 caproto-apps-0.1.0/src/caprotoapps/alive.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     8190 2023-07-02 02:10:14.000000 caproto-apps-0.1.0/src/caprotoapps/manager.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.651473 caproto-apps-0.1.0/tests/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    10768 2023-07-01 02:49:25.000000 caproto-apps-0.1.0/tests/test_alive.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     4002 2023-07-01 23:53:32.000000 caproto-apps-0.1.0/tests/test_manager.py
```

### Comparing `caproto-apps-0.0.2/PKG-INFO` & `caproto-apps-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,23 @@
-Metadata-Version: 2.1
-Name: caproto-apps
-Version: 0.0.2
-Summary: Variety of useful extensions for caproto IOCs.
-Author-email: Mark Wolfman <wolfman@anl.gov>
-Project-URL: Homepage, https://github.com/canismarko/caproto-apps
-Keywords: caproto,controls
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # Caproto Apps
 
 [![Tests](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml)
 
 Implementations of select EPICS-compatible records in caproto.
 
-Currently the only app available is the **Alive** app.
 
 ## Installation
 
 ```
 pip install caproto-apps
 ```
 
-## Alive
+## Components
+
+### Alive
 
 The AliveGroup provides equivalent functionality to the
 [EPICS alive record](http://epics-modules.github.io/alive/aliveRecord.html)
 and is compatible with existing
 [alive daemons](https://epics-alive-server.github.io/alive-overview.html).
 
 It is intended to be added to an existing ``PVGroup`` using caproto's
@@ -80,15 +65,57 @@
     # Replace ``ENGINEER`` with ``SCIENTIST``
     evd1 = envvar_default_property(1, "SCIENTIST")
     # Add a new variable, "STATUS"
     evd6 = envvar_default_property(1, "STATUS")
 
 ```
 
+### Manager
+
+The ``ManagerGroup`` allows for remote management of other
+IOCs. Currently the only supported style is that of APS beamline
+controls group. To allow control of an IOC, specify the path to the
+startup script using the *script* parameter.
+
+```
+from caproto.server import SubGroup
+from caprotoapps import ManagerGroup
+
+class MyIOC(PVGroup):
+    ioc_manager = SubGroup(ManagerGroup,
+    		           script="/path/to/script.sh")
+```			 
+
+If the script can be reached on another machine via SSH, then the
+following pattern can also be used, provided that passwordless login
+is set up (i.e. using ``ssh-keygen``):
+
+```
+class MyIOC(PVGroup):
+    ioc_manager = SubGroup(ManagerGroup,
+    		           script="myuser@myhost:/path/to/script.sh")
+```
+
+**Note:** The *console* PV is currently not implemented.
+
+## Development
+
+To install caproto-apps for development, first clone the github repository:
+
+```
+git clone https://github.com/canismarko/caproto-apps.git
+```
+
+Then run tests with pytest
+
+```
+pytest
+```
+
 ## Building the Project for PyPI
 
 ```
 (venv) $ python -m build
 (venv) $ twine check dist/*
 (venv) $ twine upload -r testpypi dist/*
 (venv) $ twine upload dist/*
-```
+```
```

### Comparing `caproto-apps-0.0.2/README.md` & `caproto-apps-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,39 @@
+Metadata-Version: 2.1
+Name: caproto-apps
+Version: 0.1.0
+Summary: Variety of useful extensions for caproto IOCs.
+Author-email: Mark Wolfman <wolfman@anl.gov>
+Project-URL: Homepage, https://github.com/canismarko/caproto-apps
+Keywords: caproto,controls
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # Caproto Apps
 
 [![Tests](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml)
 
 Implementations of select EPICS-compatible records in caproto.
 
-Currently the only app available is the **Alive** app.
 
 ## Installation
 
 ```
 pip install caproto-apps
 ```
 
-## Alive
+## Components
+
+### Alive
 
 The AliveGroup provides equivalent functionality to the
 [EPICS alive record](http://epics-modules.github.io/alive/aliveRecord.html)
 and is compatible with existing
 [alive daemons](https://epics-alive-server.github.io/alive-overview.html).
 
 It is intended to be added to an existing ``PVGroup`` using caproto's
@@ -64,15 +81,57 @@
     # Replace ``ENGINEER`` with ``SCIENTIST``
     evd1 = envvar_default_property(1, "SCIENTIST")
     # Add a new variable, "STATUS"
     evd6 = envvar_default_property(1, "STATUS")
 
 ```
 
+### Manager
+
+The ``ManagerGroup`` allows for remote management of other
+IOCs. Currently the only supported style is that of APS beamline
+controls group. To allow control of an IOC, specify the path to the
+startup script using the *script* parameter.
+
+```
+from caproto.server import SubGroup
+from caprotoapps import ManagerGroup
+
+class MyIOC(PVGroup):
+    ioc_manager = SubGroup(ManagerGroup,
+    		           script="/path/to/script.sh")
+```			 
+
+If the script can be reached on another machine via SSH, then the
+following pattern can also be used, provided that passwordless login
+is set up (i.e. using ``ssh-keygen``):
+
+```
+class MyIOC(PVGroup):
+    ioc_manager = SubGroup(ManagerGroup,
+    		           script="myuser@myhost:/path/to/script.sh")
+```
+
+**Note:** The *console* PV is currently not implemented.
+
+## Development
+
+To install caproto-apps for development, first clone the github repository:
+
+```
+git clone https://github.com/canismarko/caproto-apps.git
+```
+
+Then run tests with pytest
+
+```
+pytest
+```
+
 ## Building the Project for PyPI
 
 ```
 (venv) $ python -m build
 (venv) $ twine check dist/*
 (venv) $ twine upload -r testpypi dist/*
 (venv) $ twine upload dist/*
-```
+```
```

### Comparing `caproto-apps-0.0.2/pyproject.toml` & `caproto-apps-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 # [build-system]
 # requires = ["hatchling"]
 # build-backend = "hatchling.build"
 
 [project]
 name = "caproto-apps"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Mark Wolfman", email="wolfman@anl.gov" },
 ]
 description = "Variety of useful extensions for caproto IOCs."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Hardware",
 ]
 keywords = ["caproto", "controls"]
-dependencies = ["caproto"]
+dependencies = ["caproto", "fabric"]
 
 [project.optional-dependencies]
 dev = ["black", "pytest", "pytest-asyncio", "build", "twine"]
 
 [project.urls]
 Homepage = "https://github.com/canismarko/caproto-apps"
```

### Comparing `caproto-apps-0.0.2/src/caproto_apps.egg-info/PKG-INFO` & `caproto-apps-0.1.0/src/caproto_apps.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caproto-apps
-Version: 0.0.2
+Version: 0.1.0
 Summary: Variety of useful extensions for caproto IOCs.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/canismarko/caproto-apps
 Keywords: caproto,controls
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -16,23 +16,24 @@
 
 # Caproto Apps
 
 [![Tests](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/canismarko/caproto-apps/actions/workflows/ci.yml)
 
 Implementations of select EPICS-compatible records in caproto.
 
-Currently the only app available is the **Alive** app.
 
 ## Installation
 
 ```
 pip install caproto-apps
 ```
 
-## Alive
+## Components
+
+### Alive
 
 The AliveGroup provides equivalent functionality to the
 [EPICS alive record](http://epics-modules.github.io/alive/aliveRecord.html)
 and is compatible with existing
 [alive daemons](https://epics-alive-server.github.io/alive-overview.html).
 
 It is intended to be added to an existing ``PVGroup`` using caproto's
@@ -80,14 +81,56 @@
     # Replace ``ENGINEER`` with ``SCIENTIST``
     evd1 = envvar_default_property(1, "SCIENTIST")
     # Add a new variable, "STATUS"
     evd6 = envvar_default_property(1, "STATUS")
 
 ```
 
+### Manager
+
+The ``ManagerGroup`` allows for remote management of other
+IOCs. Currently the only supported style is that of APS beamline
+controls group. To allow control of an IOC, specify the path to the
+startup script using the *script* parameter.
+
+```
+from caproto.server import SubGroup
+from caprotoapps import ManagerGroup
+
+class MyIOC(PVGroup):
+    ioc_manager = SubGroup(ManagerGroup,
+    		           script="/path/to/script.sh")
+```			 
+
+If the script can be reached on another machine via SSH, then the
+following pattern can also be used, provided that passwordless login
+is set up (i.e. using ``ssh-keygen``):
+
+```
+class MyIOC(PVGroup):
+    ioc_manager = SubGroup(ManagerGroup,
+    		           script="myuser@myhost:/path/to/script.sh")
+```
+
+**Note:** The *console* PV is currently not implemented.
+
+## Development
+
+To install caproto-apps for development, first clone the github repository:
+
+```
+git clone https://github.com/canismarko/caproto-apps.git
+```
+
+Then run tests with pytest
+
+```
+pytest
+```
+
 ## Building the Project for PyPI
 
 ```
 (venv) $ python -m build
 (venv) $ twine check dist/*
 (venv) $ twine upload -r testpypi dist/*
 (venv) $ twine upload dist/*
```

### Comparing `caproto-apps-0.0.2/src/caprotoapps/alive.py` & `caproto-apps-0.1.0/src/caprotoapps/alive.py`

 * *Files identical despite different names*

### Comparing `caproto-apps-0.0.2/tests/test_alive.py` & `caproto-apps-0.1.0/tests/test_alive.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
 @pytest.fixture
 def test_ioc():
     ioc = MockIOC(prefix="test_ioc:")
     ioc.alive.incarnation = alive.epics_time(1686882446.0032349)
     ioc.alive.async_lib = asyncio
     ioc.alive.send_udp_message = mock.AsyncMock()
-    ioc.alive
     yield ioc
 
 
 @pytest.mark.asyncio
 async def test_send_heartbeat(test_ioc):
     alive_group = test_ioc.alive
     sock = mock.MagicMock()
```

