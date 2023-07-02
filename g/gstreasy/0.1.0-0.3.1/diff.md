# Comparing `tmp/gstreasy-0.1.0.tar.gz` & `tmp/gstreasy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstreasy-0.1.0.tar", last modified: Mon Oct 17 18:19:46 2022, max compression
+gzip compressed data, was "gstreasy-0.3.1.tar", last modified: Sun Jul  2 19:40:54 2023, max compression
```

## Comparing `gstreasy-0.1.0.tar` & `gstreasy-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-10-17 18:19:46.562010 gstreasy-0.1.0/
--rw-r--r--   0 dan       (1000) dan       (1000)    11357 2022-10-14 20:08:42.000000 gstreasy-0.1.0/LICENSE
--rw-r--r--   0 dan       (1000) dan       (1000)       26 2022-10-14 18:49:39.000000 gstreasy-0.1.0/MANIFEST.in
--rw-r--r--   0 dan       (1000) dan       (1000)     2421 2022-10-17 18:19:46.561010 gstreasy-0.1.0/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     1870 2022-10-17 18:00:11.000000 gstreasy-0.1.0/README.md
--rw-r--r--   0 dan       (1000) dan       (1000)      986 2022-10-17 18:19:23.000000 gstreasy-0.1.0/pyproject.toml
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2022-10-17 18:19:46.562010 gstreasy-0.1.0/setup.cfg
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-10-17 18:19:46.559010 gstreasy-0.1.0/src/
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-10-17 18:19:46.561010 gstreasy-0.1.0/src/gstreasy/
--rw-r--r--   0 dan       (1000) dan       (1000)      109 2022-10-17 17:55:16.000000 gstreasy-0.1.0/src/gstreasy/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)    18367 2022-10-16 22:16:23.000000 gstreasy-0.1.0/src/gstreasy/pipeline.py
--rw-r--r--   0 dan       (1000) dan       (1000)     5309 2022-10-15 10:04:16.000000 gstreasy-0.1.0/src/gstreasy/utils.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2022-10-17 18:19:46.561010 gstreasy-0.1.0/src/gstreasy.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     2421 2022-10-17 18:19:46.000000 gstreasy-0.1.0/src/gstreasy.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      295 2022-10-17 18:19:46.000000 gstreasy-0.1.0/src/gstreasy.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2022-10-17 18:19:46.000000 gstreasy-0.1.0/src/gstreasy.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)      101 2022-10-17 18:19:46.000000 gstreasy-0.1.0/src/gstreasy.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        9 2022-10-17 18:19:46.000000 gstreasy-0.1.0/src/gstreasy.egg-info/top_level.txt
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-02 19:40:54.925943 gstreasy-0.3.1/
+-rw-r--r--   0 dan       (1000) dan       (1000)    11357 2022-10-14 20:08:42.000000 gstreasy-0.3.1/LICENSE
+-rw-r--r--   0 dan       (1000) dan       (1000)       26 2022-10-14 18:49:39.000000 gstreasy-0.3.1/MANIFEST.in
+-rw-r--r--   0 dan       (1000) dan       (1000)     2916 2023-07-02 19:40:54.925943 gstreasy-0.3.1/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     2365 2023-07-02 19:27:03.000000 gstreasy-0.3.1/README.md
+-rw-r--r--   0 dan       (1000) dan       (1000)     1000 2023-07-02 19:30:58.000000 gstreasy-0.3.1/pyproject.toml
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-07-02 19:40:54.925943 gstreasy-0.3.1/setup.cfg
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-02 19:40:54.920943 gstreasy-0.3.1/src/
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-02 19:40:54.924943 gstreasy-0.3.1/src/gstreasy/
+-rw-r--r--   0 dan       (1000) dan       (1000)      124 2023-07-02 19:30:50.000000 gstreasy-0.3.1/src/gstreasy/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)    19474 2023-07-02 19:17:14.000000 gstreasy-0.3.1/src/gstreasy/pipeline.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2882 2023-07-02 19:08:02.000000 gstreasy-0.3.1/src/gstreasy/utils.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     4409 2023-07-02 19:08:02.000000 gstreasy-0.3.1/src/gstreasy/wrapped_caps.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-02 19:40:54.924943 gstreasy-0.3.1/src/gstreasy.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     2916 2023-07-02 19:40:54.000000 gstreasy-0.3.1/src/gstreasy.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      347 2023-07-02 19:40:54.000000 gstreasy-0.3.1/src/gstreasy.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-07-02 19:40:54.000000 gstreasy-0.3.1/src/gstreasy.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)      107 2023-07-02 19:40:54.000000 gstreasy-0.3.1/src/gstreasy.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        9 2023-07-02 19:40:54.000000 gstreasy-0.3.1/src/gstreasy.egg-info/top_level.txt
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-07-02 19:40:54.924943 gstreasy-0.3.1/tests/
+-rw-r--r--   0 dan       (1000) dan       (1000)     3115 2023-07-02 19:08:28.000000 gstreasy-0.3.1/tests/test_pipeline.py
```

### Comparing `gstreasy-0.1.0/LICENSE` & `gstreasy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gstreasy-0.1.0/PKG-INFO` & `gstreasy-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 Metadata-Version: 2.1
 Name: gstreasy
-Version: 0.1.0
+Version: 0.3.1
 Summary: Makes using GStreamer in python easy!
 Author-email: Dan Davis <dan@dandavis.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/danofsteel32/gstreasy
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
+# gstreasy
 
 A re-imagining of [gstreamer-python](https://github.com/jackersson/gstreamer-python).
-I was going to just work on a fork of that repo but there was so much I thought
-should be changed. Some of the new features:
 
+Some of the new features:
+
+- Auto setup/teardown of main loop thread
 - Auto detect caps if in gst-launch command
 - Auto detect and configure `appsink` and `appsrc` if in command
 - Support for `appsink` and `appsrc` in same pipeline
-- Faster `Gst.Sample` -> `ndarray`
+- Support for multiple sinks in the same pipeline
+- Faster `Gst.Sample` -> `np.ndarray` by caching caps
 
 
 ####  Example Usage
 
+Install with: `python -m pip install gstreasy`
+
 Also check out the `user_code.py` script for an `appsrc` example.
+As I write more examples they will appear in the `examples/` folder.
 
 ##### Simple pipeline without an `appsink` element:
 
 ```python
 simple_cmd = "videotestsrc num-buffers=60 ! autovideosink"
 with GstPipeline(simple_cmd) as pipeline:
     print("Running simple pipeline")
@@ -65,14 +71,22 @@
         buffer = pipeline.pop()
         # do whatever you want with the buffer's ndarray
     # Meanwhile recording.mp4 is being written
 ```
 
 ### Develop
 
-All dev tasks can be handled with the `run.sh` script but it just wraps standard
-tools if you can't/don't want use it.
+All dev tasks can be handled with the `run.sh` script but it just wraps standard tools if you can't/don't want use it.
 
 - `python -m pip install -e .[dev,doc]` to install deps
-- `tox` to run tests for py3.7 and py3.10.
+- `tox` to run tests for py3.7, py3.10, and py3.11.
 - `flake8` and `mypy` for linting
 - `pdoc -d google src/gstreasy` for online docs
+
+To help debugging, you can breakpoint inside functions that run on a separate thread,
+if you insert the following lines just before your breakpoint. Tested on PyCharm but should work with most IDEs.
+Please remove them before opening your pull request.
+
+```python
+import pydevd
+pydevd.settrace(suspend=False, trace_only_current_thread=True)
+```
```

### Comparing `gstreasy-0.1.0/README.md` & `gstreasy-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+# gstreasy
 
 A re-imagining of [gstreamer-python](https://github.com/jackersson/gstreamer-python).
-I was going to just work on a fork of that repo but there was so much I thought
-should be changed. Some of the new features:
 
+Some of the new features:
+
+- Auto setup/teardown of main loop thread
 - Auto detect caps if in gst-launch command
 - Auto detect and configure `appsink` and `appsrc` if in command
 - Support for `appsink` and `appsrc` in same pipeline
-- Faster `Gst.Sample` -> `ndarray`
+- Support for multiple sinks in the same pipeline
+- Faster `Gst.Sample` -> `np.ndarray` by caching caps
 
 
 ####  Example Usage
 
+Install with: `python -m pip install gstreasy`
+
 Also check out the `user_code.py` script for an `appsrc` example.
+As I write more examples they will appear in the `examples/` folder.
 
 ##### Simple pipeline without an `appsink` element:
 
 ```python
 simple_cmd = "videotestsrc num-buffers=60 ! autovideosink"
 with GstPipeline(simple_cmd) as pipeline:
     print("Running simple pipeline")
@@ -48,14 +54,22 @@
         buffer = pipeline.pop()
         # do whatever you want with the buffer's ndarray
     # Meanwhile recording.mp4 is being written
 ```
 
 ### Develop
 
-All dev tasks can be handled with the `run.sh` script but it just wraps standard
-tools if you can't/don't want use it.
+All dev tasks can be handled with the `run.sh` script but it just wraps standard tools if you can't/don't want use it.
 
 - `python -m pip install -e .[dev,doc]` to install deps
-- `tox` to run tests for py3.7 and py3.10.
+- `tox` to run tests for py3.7, py3.10, and py3.11.
 - `flake8` and `mypy` for linting
 - `pdoc -d google src/gstreasy` for online docs
+
+To help debugging, you can breakpoint inside functions that run on a separate thread,
+if you insert the following lines just before your breakpoint. Tested on PyCharm but should work with most IDEs.
+Please remove them before opening your pull request.
+
+```python
+import pydevd
+pydevd.settrace(suspend=False, trace_only_current_thread=True)
+```
```

### Comparing `gstreasy-0.1.0/pyproject.toml` & `gstreasy-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gstreasy"
-version = "0.1.0"
+version = "0.3.1"
 description = "Makes using GStreamer in python easy!"
 readme = "README.md"
 authors = [{name = "Dan Davis", email = "dan@dandavis.dev"}]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
@@ -30,15 +30,16 @@
 dev = [
     "black",
     "flake8", 
     "flake8-isort",
     "flake8-docstrings",
     "mypy",
     "pytest",
-    "tox"
+    "tox",
+    "build",
 ]
 doc = ["pdoc"]
 
 [project.urls]
 Homepage = "https://github.com/danofsteel32/gstreasy"
 
 [tool.isort]
```

### Comparing `gstreasy-0.1.0/src/gstreasy/pipeline.py` & `gstreasy-0.3.1/src/gstreasy/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 import time
 import typing
 from fractions import Fraction
 
 import gi
 import numpy as np
 
-from .utils import GstBuffer, LeakyQueue, WrappedCaps, gst_buffer_to_ndarray, make_caps
+from .utils import GstBuffer, LeakyQueue, gst_buffer_to_ndarray, make_video_caps
+from .wrapped_caps import AudioCaps, VideoCaps, WrappedCaps
 
 gi.require_version("Gst", "1.0")
 gi.require_version("GstApp", "1.0")
+gi.require_version("GstAudio", "1.0")
 gi.require_version("GstVideo", "1.0")
 from gi.repository import GLib, GObject, Gst, GstApp  # noqa: E402
 
 Gst.init(sys.argv)
 
 Framerate = typing.Union[int, Fraction, str]
 
@@ -72,18 +74,27 @@
 
         self._log.debug("Got Sample")
         self.queue.put(self._extract_buffer(sample))
         return Gst.FlowReturn.OK
 
     def _extract_buffer(self, sample: Gst.Sample) -> typing.Optional[GstBuffer]:
         buffer = sample.get_buffer()
+
+        # Extract the width and height info from the sample's caps
         if not self._caps:
             self._log.debug("Getting caps from first sample")
             try:
-                self._caps = WrappedCaps.wrap(sample.get_caps())
+                caps = sample.get_caps()
+                caps_name = caps.get_structure(0).get_name()
+                if "audio" in caps_name:
+                    self._caps = AudioCaps.wrap(caps, buffer)
+                elif "video" in caps_name:
+                    self._caps = VideoCaps.wrap(caps, buffer)
+                else:
+                    raise ValueError("Unsupported Caps!")
             except AttributeError:
                 return None
 
         # Use the cached Caps so don't have to re-calc every sample
         if self._caps:
             array = gst_buffer_to_ndarray(buffer, self._caps)
             return GstBuffer(
@@ -116,16 +127,16 @@
         """
         self.src = src
         self._caps: typing.Optional[Gst.Caps] = src.get_caps()
 
         self.pts: typing.Union[int, float] = 0
         self.dts: int = GLib.MAXUINT64
 
-        self.log = logging.getLogger("AppSrc")
-        self.log.addHandler(logging.NullHandler())
+        self._log = logging.getLogger("AppSrc")
+        self._log.addHandler(logging.NullHandler())
 
         self._duration: typing.Union[int, float] = 0
 
     @property
     def duration(self) -> typing.Union[int, float]:
         """This is not well understood."""
         if not self._duration:
@@ -159,38 +170,49 @@
         offset = self.pts / self.duration
         gst_buffer = Gst.Buffer.new_wrapped(bytes(data))
         gst_buffer.pts = self.pts
         gst_buffer.dts = self.dts
         gst_buffer.offset = offset
         gst_buffer.duration = self.duration
         sample = Gst.Sample.new(buffer=gst_buffer, caps=self.caps)
-        self.log.debug("Push Sample")
+        self._log.debug("Push Sample")
         self.src.emit("push-sample", sample)
 
 
 class GstPipeline:
     """A Simple and efficient interface for running GStreamer Pipelines.
 
     Designed to be used as a ContextManager, GstPipeline takes care of the setup
     and teardown of the GLib.MainLoop thread to handle messages from the event bus.
     Any appsink or appsrc elements present in the provided command are automatically
     configured. You can `pull` buffers from an `appsink` and `push` buffers to
     an `appsrc`.
 
     The attributes `pipeline`, `bus`, and `elements` are uninitialized until
-    `startup` is called manually are upon entering the context manager.
+    `startup` is called manually or upon entering the context manager.
     """
 
     def __init__(
         self,
         command: str,
+        leaky: bool = False,
+        qsize: int = 100,
     ):
-        """Create a GstPipeline instance but don't start it yet."""
-        self.command: str = command
-        """A pipeline definition that can be run by gst-launch-1.0"""
+        """Create a `GstPipeline` but don't start it yet.
+
+        Args:
+            command (str): A pipeline definition that can be run by gst-launch-1.0.
+            leaky (bool): Whether the appsink should put buffers in a
+                leaky Queue (oldest buffers dropped if full) or a
+                normal Queue (block on `Queue.put` if full).
+            qsize (int): Max number of buffers to keep in the Queue.
+        """
+        self.command = command
+        self.leaky = leaky
+        self.qsize = qsize
 
         self.pipeline: typing.Optional[Gst.Pipeline] = None
         """The actual Pipeline created by calling
             [`Gst.parse_launch`](https://lazka.github.io/pgi-docs/index.html#Gst-1.0/functions.html#Gst.parse_launch)
             on the provided `command`. Defaults to `None`."""
 
         self.bus: typing.Optional[Gst.Bus] = None
@@ -202,18 +224,15 @@
         self._main_loop = GLib.MainLoop.new(None, is_running=False)
         self._main_loop_thread = threading.Thread(
             target=self._main_loop_run, name="MainLoop"
         )
         self._end_stream_event = threading.Event()
 
         self._appsink: typing.Optional[AppSink] = None
-        self._appsink_setup: bool = False
-
         self._appsrc: typing.Optional[AppSrc] = None
-        self._appsrc_setup: bool = False
 
         self._log = logging.getLogger("GstPipeline")
         self._log.addHandler(logging.NullHandler())
 
     def __bool__(self) -> bool:
         """Return whether or not pipeline is active or there are buffers to process."""
         if self.appsink:
@@ -318,24 +337,27 @@
 
         Args:
             eos (bool, optional): Whether to send an EOS event to the running
                 pipeline. Defaults to False.
             timeout: (int, optional): Timeout in seconds to wait for running
                 threads to finish/return. Defaults to 1.
         """
+        # Fix so don't print shutdown message twice on KeyboardInterrupt
+        if self.state == Gst.State.NULL:
+            return
         self._log.info("Shutdown requested ...")
         self._shutdown_pipeline(eos, timeout)
         self._shutdown_main_loop()
-        self._log.info("Shutdown Success")
+        self._log.info("Shutdown success")
 
     def startup(self):
         """Start the mainloop thread and pipeline."""
-        self._log.info("Starting pipeline")
+        self._log.info("Starting main loop thread")
         if self._main_loop_thread.is_alive():
-            self._log.warning("Pipeline already running")
+            self._log.warning("Main loop already running")
             return
 
         self._main_loop_thread.start()
 
         if self.pipeline:
             self._log.warning("Pipeline already running")
             return
@@ -344,32 +366,38 @@
 
         self.bus = self.pipeline.get_bus()
         self.bus.add_signal_watch()
         self.bus.connect("message::error", self.on_error)
         self.bus.connect("message::eos", self.on_eos)
         self.bus.connect("message::warning", self.on_warning)
         self.bus.connect("message::element", self.on_element)
+        # STATE_CHANGED does not seem to work
         self.bus.connect("message::STATE_CHANGED", self.on_state_change)
 
         self.pipeline.set_state(Gst.State.READY)
         self._log.debug("Set pipeline to READY")
         self._end_stream_event.clear()
 
         # Allow pipeline to PREROLL by setting in PAUSED state so caps
         # negotiation happens before configuring appsink/appsrc
         self.pipeline.set_state(Gst.State.PAUSED)
         self._log.debug("Set pipeline to PAUSED")
 
-        if not self._appsrc_setup:
-            self._appsrc_setup = self.setup_appsrc()
-
-        if not self._appsink_setup:
-            self._appsink_setup = self.setup_appsink()
+        self._log.debug("Detecting and configuring AppSink if exists ...")
+        self._appsink = self._setup_appsink()
+        if self._appsink:
+            self._log.debug("AppSink successfully configured")
+
+        self._log.debug("Detecting and configuring AppSrc if exists...")
+        self._appsrc = self._setup_appsrc()
+        if self._appsrc:
+            self._log.debug("AppSrc successfully configured")
 
         self.pipeline.set_state(Gst.State.PLAYING)
+        # sample = self._appsink.sink.pull_sample()
         self._log.debug("Set pipeline to PLAYING")
 
     @property
     def is_active(self) -> bool:
         """Return whether or not pipeline is active."""
         return self.pipeline is not None and not self.is_done
 
@@ -384,113 +412,109 @@
         return self._appsink
 
     @property
     def appsrc(self) -> typing.Optional[AppSrc]:
         """Return appsrc if configured or None."""
         return self._appsrc
 
-    def setup_appsink(self, leaky: bool = False, qsize: int = 100) -> bool:
-        """Initialize _AppSink helper class if there's an appsink element in pipeline.
+    def _setup_appsink(self) -> typing.Optional[AppSink]:
+        """Initialize `AppSink` helper class if an appsink element in pipeline.
 
-        Args:
-            leaky (bool, optional): Whether the appsink should put buffers in
-                a leaky Queue (oldest buffers dropped if full) or a normal Queue
-                (block on `Queue.put` if full). Defaults to False.
-            qsize: (int, optional): The maxsize of the appsink queue. Defaults to 100
         Returns:
-            bool: Whether the appsink was setup.
+            A configured `AppSink` or None.
         """
-        # bail early if already setup
-        if self._appsink_setup:
-            self._log.warning("Appsink already setup")
-            return True
         try:
             appsink_element = self.get_by_cls(GstApp.AppSink)[0]
-            self._log.debug("appsink element detected")
+            self._log.debug("AppSink element detected")
         except IndexError:
-            self._log.debug("No appsink element to setup")
-            return False
-        self._log.debug("Setting up AppSink ...")
-        self._appsink = AppSink(appsink_element, leaky, qsize)
-        self._log.debug("Successfully setup AppSink")
-        return True
+            self._log.debug("No AppSink element detected")
+            return None
+        return AppSink(appsink_element, self.leaky, self.qsize)
 
     def pop(self, timeout: float = 0.1) -> typing.Optional[GstBuffer]:
         """Return a `GstBuffer` from the `appsink` queue."""
-        if not self._appsink:
-            self._log.warning("No appsink to pop from")
+        if not self.appsink:
+            self._log.critical("No AppSink to pop buffer from")
+            self.shutdown()
             raise RuntimeError
 
         buf: typing.Optional[GstBuffer] = None
-        while (self.is_active or not self._appsink.queue.empty()) and not buf:
+        while (self.is_active or not self.appsink.queue.empty()) and not buf:
             try:
-                buf = self._appsink.queue.get(timeout=timeout)
+                buf = self.appsink.queue.get(timeout=timeout)
             except queue.Empty:
                 pass
+            # I think there's a reason I'm catching this here but don't remember
+            except KeyboardInterrupt:
+                self._log.critical("I'm interrupted!")
+                self.shutdown()
         return buf
 
-    def set_appsrc_caps(
+    def set_appsrc_video_caps(
         self,
         *,
         width: int,
         height: int,
         framerate: Framerate,
         format: str,
     ) -> bool:
         """Set appsrc caps if not already set.
 
+        Note that changing the caps on a running pipeline is not supported!
+        Caps are either set before starting the pipeline or are auto detected.
+
         Args:
             width (int): a positive integer corresponding to buffer width
             height (int): a positive integer corresponding to buffer height
             framerate (int, Fraction, str): A positive integer, `fractions.Fraction`,
-                or string that can be mapped to a Fraction.
-                Ex. 1 -> 10/1, "25/1" -> Fraction(25, 1)
+                or string that can be understood as a Fraction.
+                Ex. 1 -> 10/1, "25/1" -> `Fraction(25, 1)`
             format (str): A string that can be mapped to a `GstVideo.VideoFormat`.
                 Ex. "RGB", "GRAY8", "I420"
         Raises:
-            ValueError: If Gst.Caps cannot be created from arguments
+            ValueError: If `Gst.Caps` cannot be created from arguments
         """
-        if not self._appsrc:
-            self._log.warning("No appsrc element")
+        if not self.appsrc:
+            self._log.warning("No AppSrc element")
             return False
-        if self._appsrc.caps:
-            self._log.warning("Caps already set")
+        if self.appsrc.caps:
+            self._log.warning("AppSrc Caps already set")
             return False
 
         self._log.debug("Building caps from args ...")
-        self._appsrc.caps = make_caps(width, height, framerate, format)
+        self.appsrc.caps = make_video_caps(width, height, framerate, format)
         self._log.debug("Caps successfully set")
         return True
 
-    def setup_appsrc(self) -> bool:
-        """Initialize _AppSrc helper class if there's an appsrc element in pipeline.
+    def _setup_appsrc(self) -> typing.Optional[AppSrc]:
+        """Initialize `AppSrc` helper class if an appsrc element in pipeline.
 
         Returns:
-            bool: Whether setup was successful
+            Configured `AppSrc` or None.
         """
-        if self._appsrc_setup:
-            self._log.warning("Appsource already setup")
-            return True
         try:
             appsrc_element = self.get_by_cls(GstApp.AppSrc)[0]
         except IndexError:
             self._log.debug("No appsrc element to setup")
-            return False
-
+            return None
         appsrc_element.set_property("format", Gst.Format.TIME)
         appsrc_element.set_property("block", True)
-        self._appsrc = AppSrc(appsrc_element)
-        return True
+        return AppSrc(appsrc_element)
 
     def push(self, data: np.ndarray):
-        """Map the ndarray to a Gst.Sample and push it into the pipeline."""
-        if not self._appsrc:
-            self._log.warning("No appsrc to push to")
+        """Create a `Gst.Sample` from the `ndarray` and push it into the pipeline."""
+        if not self.appsrc:
+            self._log.critical("No AppSrc to push buffer to!")
+            self.shutdown()
             raise RuntimeError
-        self._appsrc.push(data)
+        try:
+            self.appsrc.push(data)
+        except KeyboardInterrupt:
+            self._log.critical("I'm interrupted!")
+            self.shutdown()
 
     def on_error(self, bus: Gst.Bus, msg: Gst.Message):
         """Log `ERROR` message and shutdown."""
         err, debug = msg.parse_error()
         self._log.error("Error %d %s: %s" % (err.code, err.message, debug))
         self.shutdown()
```

### Comparing `gstreasy-0.1.0/src/gstreasy.egg-info/PKG-INFO` & `gstreasy-0.3.1/src/gstreasy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 Metadata-Version: 2.1
 Name: gstreasy
-Version: 0.1.0
+Version: 0.3.1
 Summary: Makes using GStreamer in python easy!
 Author-email: Dan Davis <dan@dandavis.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/danofsteel32/gstreasy
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
+# gstreasy
 
 A re-imagining of [gstreamer-python](https://github.com/jackersson/gstreamer-python).
-I was going to just work on a fork of that repo but there was so much I thought
-should be changed. Some of the new features:
 
+Some of the new features:
+
+- Auto setup/teardown of main loop thread
 - Auto detect caps if in gst-launch command
 - Auto detect and configure `appsink` and `appsrc` if in command
 - Support for `appsink` and `appsrc` in same pipeline
-- Faster `Gst.Sample` -> `ndarray`
+- Support for multiple sinks in the same pipeline
+- Faster `Gst.Sample` -> `np.ndarray` by caching caps
 
 
 ####  Example Usage
 
+Install with: `python -m pip install gstreasy`
+
 Also check out the `user_code.py` script for an `appsrc` example.
+As I write more examples they will appear in the `examples/` folder.
 
 ##### Simple pipeline without an `appsink` element:
 
 ```python
 simple_cmd = "videotestsrc num-buffers=60 ! autovideosink"
 with GstPipeline(simple_cmd) as pipeline:
     print("Running simple pipeline")
@@ -65,14 +71,22 @@
         buffer = pipeline.pop()
         # do whatever you want with the buffer's ndarray
     # Meanwhile recording.mp4 is being written
 ```
 
 ### Develop
 
-All dev tasks can be handled with the `run.sh` script but it just wraps standard
-tools if you can't/don't want use it.
+All dev tasks can be handled with the `run.sh` script but it just wraps standard tools if you can't/don't want use it.
 
 - `python -m pip install -e .[dev,doc]` to install deps
-- `tox` to run tests for py3.7 and py3.10.
+- `tox` to run tests for py3.7, py3.10, and py3.11.
 - `flake8` and `mypy` for linting
 - `pdoc -d google src/gstreasy` for online docs
+
+To help debugging, you can breakpoint inside functions that run on a separate thread,
+if you insert the following lines just before your breakpoint. Tested on PyCharm but should work with most IDEs.
+Please remove them before opening your pull request.
+
+```python
+import pydevd
+pydevd.settrace(suspend=False, trace_only_current_thread=True)
+```
```

