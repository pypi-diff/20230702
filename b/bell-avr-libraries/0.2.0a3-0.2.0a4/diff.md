# Comparing `tmp/bell_avr_libraries-0.2.0a3.tar.gz` & `tmp/bell_avr_libraries-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bell_avr_libraries-0.2.0a3.tar", max compression
+gzip compressed data, was "bell_avr_libraries-0.2.0a4.tar", max compression
```

## Comparing `bell_avr_libraries-0.2.0a3.tar` & `bell_avr_libraries-0.2.0a4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/LICENSE
--rw-r--r--   0        0        0     1885 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/README.md
--rw-r--r--   0        0        0      444 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/__init__.py
--rw-r--r--   0        0        0      289 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/__init__.py
--rw-r--r--   0        0        0     8306 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/client.py
--rw-r--r--   0        0        0    23046 2023-06-03 17:54:14.739136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/constants.py
--rw-r--r--   0        0        0      588 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/dispatcher.py
--rw-r--r--   0        0        0    15050 2023-06-03 17:54:14.731136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/module.py
--rw-r--r--   0        0        0    28762 2023-06-03 17:54:14.727136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/payloads.py
--rw-r--r--   0        0        0    12195 2023-06-03 17:54:14.743136 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/qt_widget.py
--rw-r--r--   0        0        0     2534 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/mqtt/serializer.py
--rw-r--r--   0        0        0      124 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/__init__.py
--rw-r--r--   0        0        0      746 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/client.py
--rw-r--r--   0        0        0    10661 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/pcc.py
--rw-r--r--   0        0        0      935 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/serial/ports.py
--rw-r--r--   0        0        0      206 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/utils/__init__.py
--rw-r--r--   0        0        0     3076 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/utils/decorators.py
--rw-r--r--   0        0        0     1070 2023-06-03 17:53:54.030153 bell_avr_libraries-0.2.0a3/bell/avr/utils/env.py
--rw-r--r--   0        0        0     3357 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/bell/avr/utils/images.py
--rw-r--r--   0        0        0      726 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/bell/avr/utils/testing.py
--rw-r--r--   0        0        0     1494 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/bell/avr/utils/timing.py
--rw-r--r--   0        0        0     1805 2023-06-03 17:53:54.034154 bell_avr_libraries-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/LICENSE
+-rw-r--r--   0        0        0     2124 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/README.md
+-rw-r--r--   0        0        0      444 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/__init__.py
+-rw-r--r--   0        0        0     8306 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/client.py
+-rw-r--r--   0        0        0    23046 2023-07-01 22:40:44.754216 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/constants.py
+-rw-r--r--   0        0        0      588 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/dispatcher.py
+-rw-r--r--   0        0        0    15050 2023-07-01 22:40:44.762216 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/module.py
+-rw-r--r--   0        0        0    29273 2023-07-01 22:40:44.742215 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/payloads.py
+-rw-r--r--   0        0        0    12224 2023-07-01 22:40:44.758216 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/qt_widget.py
+-rw-r--r--   0        0        0     2545 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/mqtt/serializer.py
+-rw-r--r--   0        0        0      124 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/serial/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/serial/client.py
+-rw-r--r--   0        0        0    10661 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/serial/pcc.py
+-rw-r--r--   0        0        0      935 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/serial/ports.py
+-rw-r--r--   0        0        0      206 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/utils/__init__.py
+-rw-r--r--   0        0        0     3106 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/utils/decorators.py
+-rw-r--r--   0        0        0     1070 2023-07-01 22:40:19.110034 bell_avr_libraries-0.2.0a4/bell/avr/utils/env.py
+-rw-r--r--   0        0        0     3357 2023-07-01 22:40:19.114035 bell_avr_libraries-0.2.0a4/bell/avr/utils/images.py
+-rw-r--r--   0        0        0      746 2023-07-01 22:40:19.114035 bell_avr_libraries-0.2.0a4/bell/avr/utils/testing.py
+-rw-r--r--   0        0        0     1494 2023-07-01 22:40:19.114035 bell_avr_libraries-0.2.0a4/bell/avr/utils/timing.py
+-rw-r--r--   0        0        0     1907 2023-07-01 22:40:19.114035 bell_avr_libraries-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 bell_avr_libraries-0.2.0a4/PKG-INFO
```

### Comparing `bell_avr_libraries-0.2.0a3/LICENSE` & `bell_avr_libraries-0.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/README.md` & `bell_avr_libraries-0.2.0a4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # AVR-Python-Libraries
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPi versions](https://img.shields.io/pypi/pyversions/bell-avr-libraries)](https://pypi.org/project/bell-avr-libraries)
+[![PyPi downloads](https://img.shields.io/pypi/dm/bell-avr-libraries)](https://pypi.org/project/bell-avr-libraries)
 
 ## Install
 
 To install the base package, run:
 
 ```bash
 pip install bell-avr-libraries
```

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/client.py` & `bell_avr_libraries-0.2.0a4/bell/avr/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/constants.py` & `bell_avr_libraries-0.2.0a4/bell/avr/mqtt/constants.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/dispatcher.py` & `bell_avr_libraries-0.2.0a4/bell/avr/mqtt/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/module.py` & `bell_avr_libraries-0.2.0a4/bell/avr/mqtt/module.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/payloads.py` & `bell_avr_libraries-0.2.0a4/bell/avr/mqtt/payloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Literal, Optional, Protocol, Tuple, Type, Union, overload
 
 from pydantic import BaseModel as PydanticBaseModel
-from pydantic import Extra, Field, conlist, validator
+from pydantic import RootModel as PydanticRootModel
+from pydantic import ConfigDict, Field, conlist, field_validator
 
 
 @overload
 def _convert_type(iter_in: Union[list, tuple], iter_out: Type[list], items_convert_to: Type[int]) -> List[int]: ...
 
 @overload
 def _convert_type(iter_in: Union[list, tuple], iter_out: Type[list], items_convert_to: Type[float]) -> List[float]: ...
@@ -43,62 +44,63 @@
     if isinstance(iter_in, (tuple, list)):
         return iter_out(_convert_type(x, iter_out, items_convert_to) for x in iter_in)
     else:
         return items_convert_to(iter_in)
 
 
 class BaseModel(PydanticBaseModel):
-    class Config:
-        'For [Pydantic configuration](https://docs.pydantic.dev/latest/usage/model_config/), please ignore.'
-        extra = Extra.forbid
+    'For [Pydantic configuration](https://docs.pydantic.dev/latest/usage/model_config/), please ignore.'
+    model_config = ConfigDict(extra="forbid")
 
 class AVREmptyMessage(BaseModel):
     """
     This is an empty class to be used with topics with no payload. When data is sent on a topic that expects `AVREmptyMessage`, an empty string, or an empty dict (`{}`) are both acceptable.
     """
 
     pass
 
-class AVRPCMColorSetWrgbItem(BaseModel):
-    __root__: int = Field(..., ge=0, le=255)
+class AVRPCMColorSetWrgbItem(PydanticRootModel):
+    root: int = Field(..., ge=0, le=255)
 
     def __int__(self) -> int:
-        return self.__root__
+        return self.root
 
 
 class AVRPCMColorSet(BaseModel):
     if TYPE_CHECKING:
         wrgb: Tuple[int, int, int, int]
     else:
-        wrgb: conlist(AVRPCMColorSetWrgbItem, min_items=4, max_items=4)
+        wrgb: conlist(AVRPCMColorSetWrgbItem, min_length=4, max_length=4)
     """
     Color values for the white, red, green, and blue channels, respectively.
     """
-    @validator('wrgb')
-    def _validate_wrgb(cls, v) -> tuple:
+    @field_validator('wrgb')
+    def _validate_wrgb(cls, v) -> tuple: # pyright: ignore
+        # Function to convert list of objects into simpler types
         return _convert_type(v, tuple, int)
 
 
-class AVRPCMColorTimedWrgbItem(BaseModel):
-    __root__: int = Field(..., ge=0, le=255)
+class AVRPCMColorTimedWrgbItem(PydanticRootModel):
+    root: int = Field(..., ge=0, le=255)
 
     def __int__(self) -> int:
-        return self.__root__
+        return self.root
 
 
 class AVRPCMColorTimed(BaseModel):
     if TYPE_CHECKING:
         wrgb: Tuple[int, int, int, int]
     else:
-        wrgb: conlist(AVRPCMColorTimedWrgbItem, min_items=4, max_items=4)
+        wrgb: conlist(AVRPCMColorTimedWrgbItem, min_length=4, max_length=4)
     """
     Color values for the white, red, green, and blue channels, respectively.
     """
-    @validator('wrgb')
-    def _validate_wrgb(cls, v) -> tuple:
+    @field_validator('wrgb')
+    def _validate_wrgb(cls, v) -> tuple: # pyright: ignore
+        # Function to convert list of objects into simpler types
         return _convert_type(v, tuple, int)
 
     time: float = Field(default=0.5, ge=0)
     """
     Number of seconds the color should be set for. Default is 0.5.
     """
 
@@ -528,19 +530,19 @@
 
 class AVRVIOConfidence(BaseModel):
     tracking: float = Field(..., ge=0, le=100)
     """
     Tracking confidence percentage. Higher number is better.
     """
 
-class AVRVIOImageCaptureShapeItem(BaseModel):
-    __root__: int = Field(..., ge=1)
+class AVRVIOImageCaptureShapeItem(PydanticRootModel):
+    root: int = Field(..., ge=1)
 
     def __int__(self) -> int:
-        return self.__root__
+        return self.root
 
 
 class AVRVIOImageCapture(BaseModel):
     data: str
     """
     Base64 encoded data of the image. To reconstruct this as a numpy array,
 use `bell.avr.utils.images.deserialize_image` and an `bell.avr.utils.images.ImageData` class.
@@ -570,16 +572,17 @@
     if TYPE_CHECKING:
         shape: List[int]
     else:
         shape: List[AVRVIOImageCaptureShapeItem]
     """
     The shape of the image data. For example: [1270, 480, 4] would be a 1270x480 image with 4 channels per pixel.
     """
-    @validator('shape')
-    def _validate_shape(cls, v) -> list:
+    @field_validator('shape')
+    def _validate_shape(cls, v) -> list: # pyright: ignore
+        # Function to convert list of objects into simpler types
         return _convert_type(v, list, int)
 
     compressed: bool
     """
     Whether or not the image data is zlib compressed.
     """
 
@@ -629,19 +632,19 @@
     Z position in a North/East/Down coordinate system in centimeters.
     """
     hdg: float
     """
     Heading in degrees.
     """
 
-class AVRAprilTagsRawApriltagsRotationItem(BaseModel):
-    __root__: float = Field(..., ge=-1, le=1)
+class AVRAprilTagsRawApriltagsRotationItem(PydanticRootModel):
+    root: float = Field(..., ge=-1, le=1)
 
     def __float__(self) -> float:
-        return self.__root__
+        return self.root
 
 
 class AVRAprilTagsRawApriltags(BaseModel):
     tag_id: int = Field(..., ge=0)
     """
     AprilTag ID.
     """
@@ -656,20 +659,21 @@
     z: float
     """
     The position in meters of the camera relative to the AprilTag's Z frame.
     """
     if TYPE_CHECKING:
         rotation: Tuple[Tuple[float, float, float], Tuple[float, float, float], Tuple[float, float, float]]
     else:
-        rotation: conlist(conlist(AVRAprilTagsRawApriltagsRotationItem, min_items=3, max_items=3), min_items=3, max_items=3)
+        rotation: conlist(conlist(AVRAprilTagsRawApriltagsRotationItem, min_length=3, max_length=3), min_length=3, max_length=3)
     """
     3x3 rotation matrix.
     """
-    @validator('rotation')
-    def _validate_rotation(cls, v) -> tuple:
+    @field_validator('rotation')
+    def _validate_rotation(cls, v) -> tuple: # pyright: ignore
+        # Function to convert list of objects into simpler types
         return _convert_type(v, tuple, float)
 
 
 class AVRAprilTagsRaw(BaseModel):
     apriltags: List[AVRAprilTagsRawApriltags]
 
 class AVRAprilTagsVisibleApriltagsAbsolutePosition(BaseModel):
@@ -743,19 +747,19 @@
 
 class AVRAprilTagsStatus(BaseModel):
     frames_per_second: int = Field(..., ge=0)
     """
     Number of frames of video data processed in the last second
     """
 
-class AVRThermalReadingShapeItem(BaseModel):
-    __root__: int = Field(..., ge=1)
+class AVRThermalReadingShapeItem(PydanticRootModel):
+    root: int = Field(..., ge=1)
 
     def __int__(self) -> int:
-        return self.__root__
+        return self.root
 
 
 class AVRThermalReading(BaseModel):
     data: str
     """
     Base64 encoded data of the image. To reconstruct this as a numpy array,
 use `bell.avr.utils.images.deserialize_image` and an `bell.avr.utils.images.ImageData` class.
@@ -781,16 +785,17 @@
     if TYPE_CHECKING:
         shape: List[int]
     else:
         shape: List[AVRThermalReadingShapeItem]
     """
     The shape of the image data. For example: [1270, 480, 4] would be a 1270x480 image with 4 channels per pixel.
     """
-    @validator('shape')
-    def _validate_shape(cls, v) -> list:
+    @field_validator('shape')
+    def _validate_shape(cls, v) -> list: # pyright: ignore
+        # Function to convert list of objects into simpler types
         return _convert_type(v, list, int)
 
     compressed: bool
     """
     Whether or not the image data is zlib compressed.
     """
 
@@ -802,328 +807,328 @@
 
 class AVRAutonomousBuildingDisable(BaseModel):
     building: int = Field(..., ge=0, le=15)
     """
     Building ID. This is 0-indexed.
     """
 
-class _AVRFusionCourseCallable(Protocol):
+class _AVRFCMAirborneCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionCourse) -> Any:
+    def __call__(self, payload: AVRFCMAirborne) -> Any:
         ...
 
-class _AVRVIOAttitudeQuaternionCallable(Protocol):
+class _AVRFCMBatteryCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
+    def __call__(self, payload: AVRFCMBattery) -> Any:
         ...
 
-class _AVRAutonomousBuildingEnableCallable(Protocol):
+class _AVRFusionVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
+    def __call__(self, payload: AVRFusionVelocity) -> Any:
         ...
 
-class _AVRFCMHILGPSStatsCallable(Protocol):
+class _AVRAutonomousBuildingEnableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
+    def __call__(self, payload: AVRAutonomousBuildingEnable) -> Any:
         ...
 
 class _AVRPCMServoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
     def __call__(self, payload: AVRPCMServo) -> Any:
         ...
 
-class _AVRFCMBatteryCallable(Protocol):
+class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMBattery) -> Any:
+    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
         ...
 
-class _AVRAutonomousBuildingDisableCallable(Protocol):
+class _AVRFusionClimbRateCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
+    def __call__(self, payload: AVRFusionClimbRate) -> Any:
         ...
 
-class _AVRAprilTagsVisibleCallable(Protocol):
+class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
+    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
         ...
 
-class _AVRFusionVelocityCallable(Protocol):
+class _AVRVIOConfidenceCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionVelocity) -> Any:
+    def __call__(self, payload: AVRVIOConfidence) -> Any:
         ...
 
-class _AVRFusionGroundspeedCallable(Protocol):
+class _AVRVIOImageCaptureCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
+    def __call__(self, payload: AVRVIOImageCapture) -> Any:
         ...
 
-class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
+class _AVRPCMServoPWMCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRPCMServoPWM) -> Any:
         ...
 
 class _AVRFusionAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
     def __call__(self, payload: AVRFusionAttitudeQuaternion) -> Any:
         ...
 
-class _AVRFusionAttitudeEulerRadiansCallable(Protocol):
+class _AVRFCMArmedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionAttitudeEulerRadians) -> Any:
+    def __call__(self, payload: AVRFCMArmed) -> Any:
         ...
 
-class _AVRAprilTagsStatusCallable(Protocol):
+class _AVRFCMGPSInfoCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsStatus) -> Any:
+    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
         ...
 
-class _AVRAprilTagsVehiclePositionCallable(Protocol):
+class _AVRFusionPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
+    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
         ...
 
-class _AVRVIOImageRequestCallable(Protocol):
+class _AVRFusionPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageRequest) -> Any:
+    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
         ...
 
-class _AVRFusionHILGPSMessageCallable(Protocol):
+class _AVRVIOImageRequestCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
+    def __call__(self, payload: AVRVIOImageRequest) -> Any:
         ...
 
-class _AVRVIOHeadingCallable(Protocol):
+class _AVRFusionGroundspeedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOHeading) -> Any:
+    def __call__(self, payload: AVRFusionGroundspeed) -> Any:
         ...
 
-class _AVRPCMServoPercentCallable(Protocol):
+class _AVRFCMPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPercent) -> Any:
+    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
         ...
 
-class _AVRPCMServoPWMCallable(Protocol):
+class _AVRPCMColorTimedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoPWM) -> Any:
+    def __call__(self, payload: AVRPCMColorTimed) -> Any:
         ...
 
-class _AVRFCMFlightModeCallable(Protocol):
+class _AVRVIOResyncCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMFlightMode) -> Any:
+    def __call__(self, payload: AVRVIOResync) -> Any:
         ...
 
-class _AVRFusionPositionLocalCallable(Protocol):
+class _AVRVIOImageStreamEnableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionLocal) -> Any:
+    def __call__(self, payload: AVRVIOImageStreamEnable) -> Any:
         ...
 
-class _AVRFCMPositionHomeCallable(Protocol):
+class _AVRPCMServoAbsoluteCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionHome) -> Any:
+    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
         ...
 
-class _AVRFCMVelocityCallable(Protocol):
+class _AVRPCMColorSetCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMVelocity) -> Any:
+    def __call__(self, payload: AVRPCMColorSet) -> Any:
         ...
 
 class _AVRFusionHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
     def __call__(self, payload: AVRFusionHeading) -> Any:
         ...
 
-class _AVRVIOImageCaptureCallable(Protocol):
+class _AVRVIOHeadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageCapture) -> Any:
+    def __call__(self, payload: AVRVIOHeading) -> Any:
         ...
 
-class _AVRFCMGPSInfoCallable(Protocol):
+class _AVRFCMFlightModeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMGPSInfo) -> Any:
+    def __call__(self, payload: AVRFCMFlightMode) -> Any:
         ...
 
-class _AVRFCMPositionGlobalCallable(Protocol):
+class _AVRAprilTagsVisibleCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
+    def __call__(self, payload: AVRAprilTagsVisible) -> Any:
         ...
 
-class _AVRFCMLandedCallable(Protocol):
+class _AVRFCMVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMLanded) -> Any:
+    def __call__(self, payload: AVRFCMVelocity) -> Any:
         ...
 
-class _AVRVIOConfidenceCallable(Protocol):
+class _AVRPCMServoPercentCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOConfidence) -> Any:
+    def __call__(self, payload: AVRPCMServoPercent) -> Any:
         ...
 
-class _AVRFCMArmedCallable(Protocol):
+class _AVRVIOAttitudeQuaternionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMArmed) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeQuaternion) -> Any:
         ...
 
-class _AVRThermalReadingCallable(Protocol):
+class _AVRAprilTagsVehiclePositionCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRThermalReading) -> Any:
+    def __call__(self, payload: AVRAprilTagsVehiclePosition) -> Any:
         ...
 
-class _AVRAprilTagsRawCallable(Protocol):
+class _AVRFCMPositionGlobalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
+    def __call__(self, payload: AVRFCMPositionGlobal) -> Any:
         ...
 
-class _AVRPCMColorTimedCallable(Protocol):
+class _AVRThermalReadingCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorTimed) -> Any:
+    def __call__(self, payload: AVRThermalReading) -> Any:
         ...
 
-class _AVRFusionPositionGlobalCallable(Protocol):
+class _AVRAutonomousBuildingDisableCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionPositionGlobal) -> Any:
+    def __call__(self, payload: AVRAutonomousBuildingDisable) -> Any:
         ...
 
-class _AVRVIOVelocityCallable(Protocol):
+class _AVRFCMHILGPSStatsCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOVelocity) -> Any:
+    def __call__(self, payload: AVRFCMHILGPSStats) -> Any:
         ...
 
-class _AVRVIOImageStreamEnableCallable(Protocol):
+class _AVRAprilTagsRawCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOImageStreamEnable) -> Any:
+    def __call__(self, payload: AVRAprilTagsRaw) -> Any:
         ...
 
-class _AVREmptyMessageCallable(Protocol):
+class _AVRAprilTagsStatusCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self) -> Any:
+    def __call__(self, payload: AVRAprilTagsStatus) -> Any:
         ...
 
-class _AVRVIOResyncCallable(Protocol):
+class _AVRFusionHILGPSMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOResync) -> Any:
+    def __call__(self, payload: AVRFusionHILGPSMessage) -> Any:
         ...
 
-class _AVRPCMColorSetCallable(Protocol):
+class _AVRVIOVelocityCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMColorSet) -> Any:
+    def __call__(self, payload: AVRVIOVelocity) -> Any:
         ...
 
-class _AVRPCMServoAbsoluteCallable(Protocol):
+class _AVRVIOAttitudeEulerRadiansCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRPCMServoAbsolute) -> Any:
+    def __call__(self, payload: AVRVIOAttitudeEulerRadians) -> Any:
         ...
 
-class _AVRFCMAttitudeEulerDegreesCallable(Protocol):
+class _AVRFCMLandedCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAttitudeEulerDegrees) -> Any:
+    def __call__(self, payload: AVRFCMLanded) -> Any:
         ...
 
-class _AVRVIOPositionLocalCallable(Protocol):
+class _AVRFusionCourseCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRVIOPositionLocal) -> Any:
+    def __call__(self, payload: AVRFusionCourse) -> Any:
         ...
 
-class _AVRFCMPositionLocalCallable(Protocol):
+class _AVRVIOPositionLocalCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMPositionLocal) -> Any:
+    def __call__(self, payload: AVRVIOPositionLocal) -> Any:
         ...
 
-class _AVRFusionClimbRateCallable(Protocol):
+class _AVRFCMPositionHomeCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFusionClimbRate) -> Any:
+    def __call__(self, payload: AVRFCMPositionHome) -> Any:
         ...
 
-class _AVRFCMAirborneCallable(Protocol):
+class _AVREmptyMessageCallable(Protocol):
     """
     Class used only for type-hinting MQTT callbacks.
     """
-    def __call__(self, payload: AVRFCMAirborne) -> Any:
+    def __call__(self) -> Any:
         ...
```

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/qt_widget.py` & `bell_avr_libraries-0.2.0a4/bell/avr/mqtt/qt_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is automatically @generated. DO NOT EDIT!
 # fmt: off
 
 from __future__ import annotations
 
-from typing import Literal, Union, overload
+from typing import Literal, Optional, Union, overload
 
 import pydantic
 from PySide6 import QtCore, QtWidgets
 
 from bell.avr.mqtt.constants import _MQTTTopicCallableTypedDict
 from bell.avr.mqtt.serializer import deserialize_payload, serialize_payload
 from bell.avr.mqtt.dispatcher import dispatch_message
@@ -68,15 +68,15 @@
 
     This is a `QtCore.Signal` that expects a topic, and the str/bytes of the
     MQTT payload. This should already be serialized with
     `bell.avr.mqtt.serializer.serialize_payload` and ready for transmission over the
     network.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, parent: Optional[QtWidgets.QWidget]) -> None:
         """
         This class is desgined for Qt applications where a widget needs to receive and
         send MQTT messages. After the widget is initialized, the signals need to be
         connected.
 
         Example:
 
@@ -104,15 +104,15 @@
         # this docstring is here because of pdoc weirdness
 
         self.topic_callbacks: _MQTTTopicCallableTypedDict = {}
         """
         See `bell.avr.mqtt.client.MQTTClient.topic_callbacks`.
         """
 
-        super().__init__(*args, **kwargs)
+        super().__init__(parent)
 
 
     @overload
     def send_message(self, topic: Literal["avr/pcm/color/set"], payload: Union[AVRPCMColorSet, dict]) -> None: ...
     @overload
     def send_message(self, topic: Literal["avr/pcm/color/timed"], payload: Union[AVRPCMColorTimed, dict]) -> None: ...
     @overload
```

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/mqtt/serializer.py` & `bell_avr_libraries-0.2.0a4/bell/avr/mqtt/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,11 +73,11 @@
 
         # if not, convert to a pydantic model
         if not isinstance(payload, pydantic.BaseModel):
             payload = MQTTTopicPayload[topic](**payload)
 
     # convert pydantic models to json
     if isinstance(payload, pydantic.BaseModel):
-        return payload.json()
+        return payload.model_dump_json()
 
     # convert any other data type to json
     return json.dumps(payload)
```

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/serial/client.py` & `bell_avr_libraries-0.2.0a4/bell/avr/serial/client.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/serial/pcc.py` & `bell_avr_libraries-0.2.0a4/bell/avr/serial/pcc.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/serial/ports.py` & `bell_avr_libraries-0.2.0a4/bell/avr/serial/ports.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/utils/decorators.py` & `bell_avr_libraries-0.2.0a4/bell/avr/utils/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Additionally, there is the `reraise` argument, which can be set to `True` to raise
     any exceptions that are encountered. This is helpful if you still want exceptions
     to propagate up, but log them.
     """
 
     def decorator(func: Callable) -> Callable:
         @functools.wraps(func)
-        def wrapper(*args, **kwargs) -> Any:
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
             try:
                 return func(*args, **kwargs)
             except Exception as e:
                 logger.exception(f"Unexpected exception in {func.__name__}")
                 if reraise:
                     raise e from e
 
@@ -68,15 +68,15 @@
         async def connected_status_telemetry(self) -> None:
             ...
     ```
     """
 
     def decorator(func: Callable) -> Callable:
         @functools.wraps(func)
-        async def wrapper(*args, **kwargs) -> Any:
+        async def wrapper(*args: Any, **kwargs: Any) -> Any:
             try:
                 return await func(*args, **kwargs)
             except Exception as e:
                 logger.exception(f"Unexpected exception in {func.__name__}")
                 if reraise:
                     raise e from e
 
@@ -115,15 +115,15 @@
     if frequency is not None:
         period = 1 / frequency
 
     assert period is not None
 
     def decorator(func: Callable) -> Callable:
         @functools.wraps(func)
-        def wrapper(*args, **kwargs) -> Any:
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
             while True:
                 time.sleep(period)
                 func(*args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/utils/env.py` & `bell_avr_libraries-0.2.0a4/bell/avr/utils/env.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/utils/images.py` & `bell_avr_libraries-0.2.0a4/bell/avr/utils/images.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/utils/testing.py` & `bell_avr_libraries-0.2.0a4/bell/avr/utils/testing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import wraps
 from typing import Any, Callable
 
 
-def dont_run_forever(*args, **kwargs) -> Callable:
+def dont_run_forever(*args: Any, **kwargs: Any) -> Callable:
     """
     Decorator to overwrite the `bell.avr.utils.decorators.run_forever` decorator when writing tests.
     Use like so:
 
     ```python
     # pip install pytest-mock
 
@@ -16,13 +16,13 @@
     def test_function(mocker: MockerFixture):
         mocker.patch("bell.avr.utils.decorators.run_forever", dont_run_forever)
     ```
     """
 
     def decorator(f: Callable) -> Callable:
         @wraps(f)
-        def wrapper(*args, **kwargs) -> Any:
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
             return f(*args, **kwargs)
 
         return wrapper
 
     return decorator
```

### Comparing `bell_avr_libraries-0.2.0a3/bell/avr/utils/timing.py` & `bell_avr_libraries-0.2.0a4/bell/avr/utils/timing.py`

 * *Files identical despite different names*

### Comparing `bell_avr_libraries-0.2.0a3/pyproject.toml` & `bell_avr_libraries-0.2.0a4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "bell-avr-libraries"
-    version = "0.2.0a3"
+    version = "0.2.0a4"
     description = "Common Python libraries used by parts of Bell AVR"
     license = "MIT"
     readme = "README.md"
     homepage = "https://roboticseducation.org/bell-advanced-vertical-robotics/"
     repository = "https://github.com/bellflight/AVR-Python-Libraries"
     documentation = "https://bellflight.github.io/AVR-Python-Libraries"
     authors = [
@@ -20,15 +20,16 @@
         "bell/**/.gitignore",
     ]
     include = ["bell/**/*.pyi", "bell/**/*.py"]
 
 [tool.poetry.dependencies]
     python             = ">=3.8,<3.12"
     loguru             = ">=0.6,<0.8"
-    pydantic           = "^1.10.2"
+    # pydantic 2 only
+    pydantic           = ">=2.0,<3.0"
     paho-mqtt          = "^1.6.1"
     numpy              = "^1.24.3"
     pyserial           = { version = "^3.5", optional = true }
     pyside6-essentials = { version = "^6.4.2", optional = true }
 
 [tool.poetry.extras]
     serial = ["pyserial"]
@@ -42,20 +43,21 @@
     pytest-cov   = "^4.0.0"
     pre-commit   = ">=2.21,<4.0"
     # building template
     Jinja2  = "^3.1.2"
     jsonref = "^1.0.1"
     pyyaml  = "^6.0"
     tomli   = { version = "^2.0.1", python = "<3.11" }
-    pdoc    = "^13.1.1"
+    pdoc    = ">=13.1.1,<15.0.0"
 
 [tool.pyright]
-    typeCheckingMode = "basic"
-    venvPath         = "."
-    venv             = ".venv"
+    typeCheckingMode           = "basic"
+    venvPath                   = "."
+    venv                       = ".venv"
+    reportMissingParameterType = true
 
 [tool.ruff]
     ignore = ["E501"]
 
 [build-system]
     requires      = ["poetry-core>=1.0.0"]
     build-backend = "poetry.core.masonry.api"
```

### Comparing `bell_avr_libraries-0.2.0a3/PKG-INFO` & `bell_avr_libraries-0.2.0a4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bell-avr-libraries
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: Common Python libraries used by parts of Bell AVR
 Home-page: https://roboticseducation.org/bell-advanced-vertical-robotics/
 License: MIT
 Author: Chris Padilla
 Author-email: cpadilla@bellflight.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -14,24 +14,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: qt
 Provides-Extra: serial
 Requires-Dist: loguru (>=0.6,<0.8)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pyserial (>=3.5,<4.0) ; extra == "serial"
 Requires-Dist: pyside6-essentials (>=6.4.2,<7.0.0) ; extra == "qt"
 Project-URL: Documentation, https://bellflight.github.io/AVR-Python-Libraries
 Project-URL: Repository, https://github.com/bellflight/AVR-Python-Libraries
 Description-Content-Type: text/markdown
 
 # AVR-Python-Libraries
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPi versions](https://img.shields.io/pypi/pyversions/bell-avr-libraries)](https://pypi.org/project/bell-avr-libraries)
+[![PyPi downloads](https://img.shields.io/pypi/dm/bell-avr-libraries)](https://pypi.org/project/bell-avr-libraries)
 
 ## Install
 
 To install the base package, run:
 
 ```bash
 pip install bell-avr-libraries
```

