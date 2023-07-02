# Comparing `tmp/interaction-devkit-0.1.3.tar.gz` & `tmp/interaction-devkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interaction-devkit-0.1.3.tar", last modified: Sun Jul  2 09:10:26 2023, max compression
+gzip compressed data, was "interaction-devkit-0.1.4.tar", last modified: Sun Jul  2 09:36:04 2023, max compression
```

## Comparing `interaction-devkit-0.1.3.tar` & `interaction-devkit-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.317074 interaction-devkit-0.1.3/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.317074 interaction-devkit-0.1.3/interaction/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32670 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/map_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.317074 interaction-devkit-0.1.3/interaction/dataset/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/speed_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/track_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/interaction/dataset/tracks/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/tracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20023 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/tracks/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/tracks/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/interaction_devkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_map_components.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_track_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.444399 interaction-devkit-0.1.4/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.444399 interaction-devkit-0.1.4/interaction/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32670 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/map_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.444399 interaction-devkit-0.1.4/interaction/dataset/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/speed_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/maps/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/track_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/interaction/dataset/tracks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/tracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20488 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/tracks/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/tracks/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/interaction/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/interaction_devkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 09:36:04.000000 interaction-devkit-0.1.4/interaction_devkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:04.448399 interaction-devkit-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_map_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-02 09:35:56.000000 interaction-devkit-0.1.4/tests/test_track_components.py
```

### Comparing `interaction-devkit-0.1.3/LICENSE` & `interaction-devkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/PKG-INFO` & `interaction-devkit-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interaction-devkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A toolkit for building interactive applications.
 Author-email: Juanwu Lu <juanwu@purdue.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Juanwu Lu
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `interaction-devkit-0.1.3/README.md` & `interaction-devkit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/__init__.py` & `interaction-devkit-0.1.4/interaction/__init__.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/__init__.py` & `interaction-devkit-0.1.4/interaction/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/map_api.py` & `interaction-devkit-0.1.4/interaction/dataset/map_api.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/maps/__init__.py` & `interaction-devkit-0.1.4/interaction/dataset/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/maps/elements.py` & `interaction-devkit-0.1.4/interaction/dataset/maps/elements.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/maps/projector.py` & `interaction-devkit-0.1.4/interaction/dataset/maps/projector.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/maps/speed_limit.py` & `interaction-devkit-0.1.4/interaction/dataset/maps/speed_limit.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/maps/typing.py` & `interaction-devkit-0.1.4/interaction/dataset/maps/typing.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/maps/utils.py` & `interaction-devkit-0.1.4/interaction/dataset/maps/utils.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/track_api.py` & `interaction-devkit-0.1.4/interaction/dataset/track_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,17 @@
                 ["case_id", "track_id"]
             ),
             INTERACTIONScenarioLayers.TRACK: track_df.set_index(
                 ["case_id", "track_id"]
             ),
         }
 
+    def __getitem__(self, case_id: int) -> INTERACTIONCase:
+        return self.get_case(case_id)
+
     def __len__(self) -> int:
         return self.num_cases
 
     def __str__(self) -> str:
         return (
             f"<INTERACTIONScenario(location={self._location}"
             f"root={self._root}) at {hex(id(self))}>"
```

### Comparing `interaction-devkit-0.1.3/interaction/dataset/tracks/container.py` & `interaction-devkit-0.1.4/interaction/dataset/tracks/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,23 +250,31 @@
         return max(ms.timestamp_ms for ms in self.motion_states)
 
     @property
     def num_motion_states(self) -> int:
         """int: The number of motion states in the track."""
         return len(self.motion_states)
 
-    def to_geometry(self) -> LineString:
+    def to_geometry(self) -> Union[Point, LineString]:
         """Convert the track to a Shapely geometry object.
 
         Returns:
-            LineString: The track as a Shapely geometry object.
+            Union[Point, LineString]: The track as a Shapely geometry object.
+
+        Raises:
+            ValueError: If the track has no motion states.
         """
-        return LineString(
-            [(ms.position_x, ms.position_y) for ms in self.motion_states]
-        )
+        if len(self.motion_states) == 1:
+            return self.motion_states[0].to_geometry()
+        elif len(self.motion_states) > 1:
+            return LineString(
+                [(ms.position_x, ms.position_y) for ms in self.motion_states]
+            )
+        else:
+            raise ValueError("Track must have at least one motion state.")
 
     def __eq__(self, __value: Any) -> bool:
         if isinstance(__value, Track):
             return hash(self) == hash(__value)
         return NotImplemented
 
     def __ne__(self, __value: Any) -> bool:
@@ -340,19 +348,19 @@
         """Post-initialization hook."""
         assert self.location in LOCATIONS, "Invalid location name"
         assert (
             isinstance(self.case_id, int) and self.case_id >= 0
         ), "Expected a non-negative integer for case ID."
 
         self.history_tracks = sorted(self.history_tracks)
-        self._history_ids = (track.agent_id for track in self.history_tracks)
+        self._history_ids = [track.agent_id for track in self.history_tracks]
         self.current_tracks = sorted(self.current_tracks)
-        self._current_ids = (track.agent_id for track in self.current_tracks)
+        self._current_ids = [track.agent_id for track in self.current_tracks]
         self.futural_tracks = sorted(self.futural_tracks)
-        self._futural_ids = (track.agent_id for track in self.futural_tracks)
+        self._futural_ids = [track.agent_id for track in self.futural_tracks]
         self.tracks_to_predict = tuple(self.tracks_to_predict)
         self.interesting_agents = tuple(self.interesting_agents)
 
     @cached_property
     def num_agents(self) -> int:
         """int: The number of agents in the case."""
         return len(
@@ -454,15 +462,19 @@
                     for track in self.history_tracks
                     if track.agent_id in self.tracks_to_predict
                 ]
             ).affine_transform(affine_params).plot(
                 ax=ax, color="#F29492", linewidth=1, zorder=12
             )
             gpd.GeoSeries(
-                [track.to_geometry() for track in self.futural_tracks]
+                [
+                    track.to_geometry()
+                    for track in self.futural_tracks
+                    if track.agent_id in self.tracks_to_predict
+                ]
             ).affine_transform(affine_params).plot(
                 ax=ax, color="#A8FF78", linewidth=1, zorder=13
             )
             if mode == "tail-box":
                 gpd.GeoSeries(
                     [
                         motion_state.bounding_box
```

### Comparing `interaction-devkit-0.1.3/interaction/dataset/tracks/typing.py` & `interaction-devkit-0.1.4/interaction/dataset/tracks/typing.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction/dataset/utils.py` & `interaction-devkit-0.1.4/interaction/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/interaction_devkit.egg-info/PKG-INFO` & `interaction-devkit-0.1.4/interaction_devkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interaction-devkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A toolkit for building interactive applications.
 Author-email: Juanwu Lu <juanwu@purdue.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Juanwu Lu
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `interaction-devkit-0.1.3/interaction_devkit.egg-info/SOURCES.txt` & `interaction-devkit-0.1.4/interaction_devkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/pyproject.toml` & `interaction-devkit-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "interaction-devkit"
-version = "0.1.3"
+version = "0.1.4"
 description = "A toolkit for building interactive applications."
 readme = "README.md"
 authors = [{name="Juanwu Lu", email="juanwu@purdue.edu"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 dependencies = [
     "defusedxml",
@@ -28,15 +28,15 @@
 [tool.isort]
 known_first_party = "interaction-devkit"
 
 line_length = 79
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `interaction-devkit-0.1.3/tests/test_map_api.py` & `interaction-devkit-0.1.4/tests/test_map_api.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/tests/test_map_components.py` & `interaction-devkit-0.1.4/tests/test_map_components.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.3/tests/test_track_components.py` & `interaction-devkit-0.1.4/tests/test_track_components.py`

 * *Files identical despite different names*

