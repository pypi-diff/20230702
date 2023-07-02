# Comparing `tmp/ecowitt2mqtt-2023.6.1.tar.gz` & `tmp/ecowitt2mqtt-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecowitt2mqtt-2023.6.1.tar", max compression
+gzip compressed data, was "ecowitt2mqtt-2023.7.0.tar", max compression
```

## Comparing `ecowitt2mqtt-2023.6.1.tar` & `ecowitt2mqtt-2023.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/LICENSE
--rw-r--r--   0        0        0    31131 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/README.md
--rw-r--r--   0        0        0       39 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/__init__.py
--rw-r--r--   0        0        0    13841 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/__main__.py
--rw-r--r--   0        0        0       24 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/backports/__init__.py
--rw-r--r--   0        0        0     1735 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/backports/enum.py
--rw-r--r--   0        0        0    16441 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/config.py
--rw-r--r--   0        0        0    10967 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/const.py
--rw-r--r--   0        0        0     2308 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/core.py
--rw-r--r--   0        0        0    12282 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/data.py
--rw-r--r--   0        0        0      107 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/errors.py
--rw-r--r--   0        0        0       22 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/__init__.py
--rw-r--r--   0        0        0     6598 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/__init__.py
--rw-r--r--   0        0        0     4891 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/battery.py
--rw-r--r--   0        0        0     2301 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/humidity.py
--rw-r--r--   0        0        0     2438 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/illuminance.py
--rw-r--r--   0        0        0     1018 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/leak.py
--rw-r--r--   0        0        0     2013 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/lightning.py
--rw-r--r--   0        0        0      744 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pollution.py
--rw-r--r--   0        0        0     2737 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/precipitation.py
--rw-r--r--   0        0        0     1364 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pressure.py
--rw-r--r--   0        0        0    21443 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/temperature.py
--rw-r--r--   0        0        0     1639 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/time.py
--rw-r--r--   0        0        0     4610 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/uv.py
--rw-r--r--   0        0        0     9593 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/wind.py
--rw-r--r--   0        0        0     2167 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/config_validation.py
--rw-r--r--   0        0        0     1665 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/device.py
--rw-r--r--   0        0        0     1800 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/__init__.py
--rw-r--r--   0        0        0      857 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/factory.py
--rw-r--r--   0        0        0    18330 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/hass.py
--rw-r--r--   0        0        0     1114 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/topic.py
--rw-r--r--   0        0        0     4973 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/server.py
--rw-r--r--   0        0        0      348 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/typing.py
--rw-r--r--   0        0        0     8058 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/runtime.py
--rw-r--r--   0        0        0     1414 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/__init__.py
--rw-r--r--   0        0        0     7934 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/meteo.py
--rw-r--r--   0        0        0    13191 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/unit_conversion.py
--rw-r--r--   0        0        0     4077 2023-06-18 14:59:03.827169 ecowitt2mqtt-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0    32563 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/LICENSE
+-rw-r--r--   0        0        0    31304 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/README.md
+-rw-r--r--   0        0        0       39 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/__init__.py
+-rw-r--r--   0        0        0    14059 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/__main__.py
+-rw-r--r--   0        0        0       24 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/backports/__init__.py
+-rw-r--r--   0        0        0     1735 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/backports/enum.py
+-rw-r--r--   0        0        0    16441 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/config.py
+-rw-r--r--   0        0        0    11243 2023-07-02 18:14:02.172386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/const.py
+-rw-r--r--   0        0        0     2308 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/core.py
+-rw-r--r--   0        0        0    12282 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/data.py
+-rw-r--r--   0        0        0      107 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/errors.py
+-rw-r--r--   0        0        0       22 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/__init__.py
+-rw-r--r--   0        0        0     6598 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/__init__.py
+-rw-r--r--   0        0        0     4891 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/battery.py
+-rw-r--r--   0        0        0     2301 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/humidity.py
+-rw-r--r--   0        0        0     2438 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/illuminance.py
+-rw-r--r--   0        0        0     1018 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/leak.py
+-rw-r--r--   0        0        0     2013 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/lightning.py
+-rw-r--r--   0        0        0      744 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/pollution.py
+-rw-r--r--   0        0        0     2737 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/precipitation.py
+-rw-r--r--   0        0        0     1364 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/pressure.py
+-rw-r--r--   0        0        0    21443 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/temperature.py
+-rw-r--r--   0        0        0     1639 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/time.py
+-rw-r--r--   0        0        0     4610 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/uv.py
+-rw-r--r--   0        0        0     9593 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/wind.py
+-rw-r--r--   0        0        0     2167 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/config_validation.py
+-rw-r--r--   0        0        0     1665 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/device.py
+-rw-r--r--   0        0        0     1800 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/__init__.py
+-rw-r--r--   0        0        0      857 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/factory.py
+-rw-r--r--   0        0        0    18868 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/hass.py
+-rw-r--r--   0        0        0     1114 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/topic.py
+-rw-r--r--   0        0        0     4973 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/server.py
+-rw-r--r--   0        0        0      348 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/typing.py
+-rw-r--r--   0        0        0     8058 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/runtime.py
+-rw-r--r--   0        0        0     1414 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/util/__init__.py
+-rw-r--r--   0        0        0     7934 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/util/meteo.py
+-rw-r--r--   0        0        0    13191 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/ecowitt2mqtt/util/unit_conversion.py
+-rw-r--r--   0        0        0     4077 2023-07-02 18:14:02.176386 ecowitt2mqtt-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0    32736 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.7.0/PKG-INFO
```

### Comparing `ecowitt2mqtt-2023.6.1/LICENSE` & `ecowitt2mqtt-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/README.md` & `ecowitt2mqtt-2023.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,16 @@
                         ecowitt2mqtt on (default: /data/report)
   --hass-discovery      Publish data in the Home Assistant MQTT
                         Discovery format
   --hass-discovery-prefix hass_discovery_prefix
                         The Home Assistant MQTT Discovery topic prefix
                         to use (default: homeassistant)
   --hass-entity-id-prefix hass_entity_id_prefix
-                        The prefix to use for Home Assistant entity IDs
+                        The prefix to use for Home Assistant entity IDs.
+                        Example: A prefix of 'prefix' will prepend 'prefix_' to entity IDs.
   --input-data-format input_data_format
                         The input data format used by the gateway
                         (default: ecowitt)
   --input-unit-system input_unit_system
                         The input unit system used by the gateway
                         (default: imperial)
   -b mqtt_broker, --mqtt-broker mqtt_broker
@@ -228,15 +229,16 @@
   --output-unit-temperature output_unit_temperature
                         The output unit to use for temperature data
                         points (default: the default used by the output
                         unit system)
   --port port           The port to serve ecowitt2mqtt on (default:
                         8080)
   --precision precision
-                        The precision to output data points at
+                        The precision to output data points at.
+                        Example: A value of 2 will round to two decimal places
                         (default: no limit)
   --raw-data            Return raw data (don't attempt to translate any
                         values)
   -v, --verbose         Increase verbosity of logged output
 ```
 
 ## Environment Variables
```

#### html2text {}

```diff
@@ -75,48 +75,49 @@
 config strategy to use (default: boolean) --diagnostics Output diagnostics --
 disable-calculated-data Disable the output of calculated sensors -e endpoint, -
 -endpoint endpoint The relative endpoint/path to serve ecowitt2mqtt on
 (default: /data/report) --hass-discovery Publish data in the Home Assistant
 MQTT Discovery format --hass-discovery-prefix hass_discovery_prefix The Home
 Assistant MQTT Discovery topic prefix to use (default: homeassistant) --hass-
 entity-id-prefix hass_entity_id_prefix The prefix to use for Home Assistant
-entity IDs --input-data-format input_data_format The input data format used by
-the gateway (default: ecowitt) --input-unit-system input_unit_system The input
-unit system used by the gateway (default: imperial) -b mqtt_broker, --mqtt-
-broker mqtt_broker The hostname or IP address of an MQTT broker -
-p mqtt_password, --mqtt-password mqtt_password A valid password for the MQTT
-broker --mqtt-port mqtt_port The listenting port of the MQTT broker (default:
-1883) --mqtt-retain Instruct the MQTT broker to retain messages --mqtt-tls
-Enable MQTT over TLS -t mqtt_topic, --mqtt-topic mqtt_topic The MQTT topic to
-publish device data to -u mqtt_username, --mqtt-username mqtt_username A valid
-username for the MQTT broker --output-unit-system output_unit_system The output
-unit system used by the gateway (default: imperial) --output-unit-accumulated-
-precipitation output_unit_accumulated_precipitation The output unit to use for
-accumulated precipitation data points (default: the default used by the output
-unit system) --output-unit-distance output_unit_distance The output unit to use
-for distance data points (default: the default used by the output unit system)
---output-unit-humidity output_unit_humidity The output unit to use for humidity
+entity IDs. Example: A prefix of 'prefix' will prepend 'prefix_' to entity IDs.
+--input-data-format input_data_format The input data format used by the gateway
+(default: ecowitt) --input-unit-system input_unit_system The input unit system
+used by the gateway (default: imperial) -b mqtt_broker, --mqtt-broker
+mqtt_broker The hostname or IP address of an MQTT broker -p mqtt_password, --
+mqtt-password mqtt_password A valid password for the MQTT broker --mqtt-port
+mqtt_port The listenting port of the MQTT broker (default: 1883) --mqtt-retain
+Instruct the MQTT broker to retain messages --mqtt-tls Enable MQTT over TLS -
+t mqtt_topic, --mqtt-topic mqtt_topic The MQTT topic to publish device data to
+-u mqtt_username, --mqtt-username mqtt_username A valid username for the MQTT
+broker --output-unit-system output_unit_system The output unit system used by
+the gateway (default: imperial) --output-unit-accumulated-precipitation
+output_unit_accumulated_precipitation The output unit to use for accumulated
+precipitation data points (default: the default used by the output unit system)
+--output-unit-distance output_unit_distance The output unit to use for distance
 data points (default: the default used by the output unit system) --output-
-unit-illuminance output_unit_illuminance The output unit to use for illuminance
-data points (default: the default used by the output unit system) --output-
-unit-precipitation-rate output_unit_precipitation_rate The output unit to use
-for precipitation rate data points (default: the default used by the output
-unit system) --output-unit-pressure output_unit_pressure The output unit to use
-for pressure data points (default: the default used by the output unit system)
---output-unit-speed output_unit_speed The output unit to use for speed data
+unit-humidity output_unit_humidity The output unit to use for humidity data
+points (default: the default used by the output unit system) --output-unit-
+illuminance output_unit_illuminance The output unit to use for illuminance data
+points (default: the default used by the output unit system) --output-unit-
+precipitation-rate output_unit_precipitation_rate The output unit to use for
+precipitation rate data points (default: the default used by the output unit
+system) --output-unit-pressure output_unit_pressure The output unit to use for
+pressure data points (default: the default used by the output unit system) --
+output-unit-speed output_unit_speed The output unit to use for speed data
 points (default: the default used by the output unit system) --output-unit-
 temperature output_unit_temperature The output unit to use for temperature data
 points (default: the default used by the output unit system) --port port The
 port to serve ecowitt2mqtt on (default: 8080) --precision precision The
-precision to output data points at (default: no limit) --raw-data Return raw
-data (don't attempt to translate any values) -v, --verbose Increase verbosity
-of logged output ``` ## Environment Variables -
-`ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-delimited list of key=value
-battery overrides (default: `numeric`) - `ECOWITT2MQTT_CONFIG`: a path to a
-YAML or JSON config file (default: `None`) -
+precision to output data points at. Example: A value of 2 will round to two
+decimal places (default: no limit) --raw-data Return raw data (don't attempt to
+translate any values) -v, --verbose Increase verbosity of logged output ``` ##
+Environment Variables - `ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-delimited
+list of key=value battery overrides (default: `numeric`) -
+`ECOWITT2MQTT_CONFIG`: a path to a YAML or JSON config file (default: `None`) -
 `ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY`: the default battery config strategy to
 use (default: `boolean`) - `ECOWITT2MQTT_DIAGNOSTICS`: whether to output
 diagnostics (default: `false`) - `ECOWITT2MQTT_DISABLE_CALCULATED_DATA`:
 whether to disable the output of calculated sensors (default: `false`) -
 `ECOWITT2MQTT_ENDPOINT`: the relative endpoint/path to serve ecowitt2mqtt on
 (default: `/data/report`) - `ECOWITT2MQTT_HASS_DISCOVERY_PREFIX`: the Home
 Assistant discovery prefix to use (default: `homeassistant`) -
```

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/__main__.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,18 @@
             f"(default: {DEFAULT_HASS_DISCOVERY_PREFIX})"
         ),
         metavar=CONF_HASS_DISCOVERY_PREFIX,
     )
     parser.add_argument(
         "--hass-entity-id-prefix",
         dest=CONF_HASS_ENTITY_ID_PREFIX,
-        help="The prefix to use for Home Assistant entity IDs",
+        help=(
+            "The prefix to use for Home Assistant entity IDs. "
+            "Example: A prefix of 'prefix' will prepend 'prefix_' to entity IDs"
+        ),
         metavar=CONF_HASS_ENTITY_ID_PREFIX,
     )
     parser.add_argument(
         "--input-data-format",
         dest=CONF_INPUT_DATA_FORMAT,
         help=(
             "The input data format used by the gateway "
@@ -406,15 +409,19 @@
         dest=CONF_PORT,
         help=f"The port to serve ecowitt2mqtt on (default: {DEFAULT_PORT})",
         metavar=CONF_PORT,
     )
     parser.add_argument(
         "--precision",
         dest=CONF_PRECISION,
-        help="The precision to output data points at (default: no limit)",
+        help=(
+            "The precision to output data points at. "
+            "Example: A value of 2 will round to two decimal places. "
+            "(default: no limit)"
+        ),
         metavar=CONF_PRECISION,
     )
     parser.add_argument(
         "--raw-data",
         action="store_true",
         dest=CONF_RAW_DATA,
         help="Return raw data (don't attempt to translate any values)",
```

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/backports/enum.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/backports/enum.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/config.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/config.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/const.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define package constants."""
 import logging
 from typing import Final
 
 from ecowitt2mqtt.helpers.typing import UnitSystemType
 
-__version__ = "2023.06.1"
+__version__ = "2023.07.0"
 
 LOGGER = logging.getLogger(__package__)
 
 # Configuration keys:
 CONF_BATTERY_OVERRIDES: Final = "battery_override"
 CONF_CONFIG: Final = "config"
 CONF_DEFAULT_BATTERY_STRATEGY: Final = "default_battery_strategy"
@@ -72,31 +72,35 @@
 # Data points (specific):
 DATA_POINT_BEAUFORT_SCALE: Final = "beaufortscale"
 DATA_POINT_CO2: Final = "co2"
 DATA_POINT_CO2_24H: Final = "co2_24h"
 DATA_POINT_CO2_BATT: Final = "co2_batt"
 DATA_POINT_DAILY_RAIN: Final = "dailyrain"
 DATA_POINT_DEWPOINT: Final = "dewpoint"
+DATA_POINT_DRAIN_PIEZO: Final = "drain_piezo"
+DATA_POINT_ERAIN_PIEZO: Final = "erain_piezo"
 DATA_POINT_EVENT_RAIN: Final = "eventrain"
 DATA_POINT_FEELSLIKE: Final = "feelslike"
 DATA_POINT_FROST_POINT: Final = "frostpoint"
 DATA_POINT_FROST_RISK: Final = "frostrisk"
 DATA_POINT_HEATINDEX: Final = "heatindex"
 DATA_POINT_HOURLY_RAIN: Final = "hourlyrain"
+DATA_POINT_HRAIN_PIEZO: Final = "hrain_piezo"
 DATA_POINT_HUMIDEX: Final = "humidex"
 DATA_POINT_HUMIDEX_PERCEPTION: Final = "humidex_perception"
 DATA_POINT_HUMIDITY: Final = "humidity"
 DATA_POINT_HUMIDITY_ABS: Final = "humidityabs"
 DATA_POINT_HUMIDITY_ABS_IN: Final = "humidityabsin"
 DATA_POINT_HUMI_CO2: Final = "humi_co2"
 DATA_POINT_INTERVAL: Final = "interval"
 DATA_POINT_LIGHTNING: Final = "lightning"
 DATA_POINT_LIGHTNING_NUM: Final = "lightning_num"
 DATA_POINT_LIGHTNING_TIME: Final = "lightning_time"
 DATA_POINT_MONTHLY_RAIN: Final = "monthlyrain"
+DATA_POINT_MRAIN_PIEZO: Final = "mrain_piezo"
 DATA_POINT_RAIN_RATE: Final = "rainrate"
 DATA_POINT_RELATIVE_STRAIN_INDEX: Final = "relative_strain_index"
 DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION: Final = "relative_strain_index_perception"
 DATA_POINT_RUNTIME: Final = "runtime"
 DATA_POINT_R_RAIN_PIEZO: Final = "rrain_piezo"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1: Final = "safe_exposure_time_skin_type_1"
 DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2: Final = "safe_exposure_time_skin_type_2"
@@ -122,16 +126,18 @@
 DATA_POINT_WH68BATT: Final = "wh68batt"
 DATA_POINT_WH80BATT: Final = "wh80batt"
 DATA_POINT_WH90BATT: Final = "wh90batt"
 DATA_POINT_WH90BATT_PC: Final = "wh90battpc"
 DATA_POINT_WH90CAP_VOLT: Final = "ws90cap_volt"
 DATA_POINT_WINDCHILL: Final = "windchill"
 DATA_POINT_WINDSPEED: Final = "windspeed"
+DATA_POINT_WRAIN_PIEZO: Final = "wrain_piezo"
 DATA_POINT_WS90_VER: Final = "ws90_ver"
 DATA_POINT_YEARLY_RAIN: Final = "yearlyrain"
+DATA_POINT_YRAIN_PIEZO: Final = "yrain_piezo"
 
 # Defaults:
 DEFAULT_ENDPOINT: Final = "/data/report"
 DEFAULT_HASS_DISCOVERY_PREFIX: Final = "homeassistant"
 DEFAULT_MQTT_PORT: Final = 1883
 DEFAULT_PORT: Final = 8080
```

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/core.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/core.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/data.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/data.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/__init__.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/battery.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/battery.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/humidity.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/humidity.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/illuminance.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/illuminance.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/leak.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/leak.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/lightning.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/lightning.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pollution.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/pollution.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/precipitation.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/precipitation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/pressure.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/pressure.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/temperature.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/temperature.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/time.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/time.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/uv.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/uv.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/calculator/wind.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/calculator/wind.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/config_validation.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/config_validation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/device.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/device.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/__init__.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/factory.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/factory.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/hass.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/hass.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from ecowitt2mqtt.config import Config
 from ecowitt2mqtt.const import (
     DATA_POINT_BEAUFORT_SCALE,
     DATA_POINT_CO2,
     DATA_POINT_CO2_24H,
     DATA_POINT_DAILY_RAIN,
     DATA_POINT_DEWPOINT,
+    DATA_POINT_DRAIN_PIEZO,
+    DATA_POINT_ERAIN_PIEZO,
     DATA_POINT_EVENT_RAIN,
     DATA_POINT_FEELSLIKE,
     DATA_POINT_FROST_POINT,
     DATA_POINT_FROST_RISK,
     DATA_POINT_GLOB_BAROM,
     DATA_POINT_GLOB_BATT,
     DATA_POINT_GLOB_GAIN_PIEZO,
@@ -36,24 +38,26 @@
     DATA_POINT_GLOB_TF,
     DATA_POINT_GLOB_VOLT,
     DATA_POINT_GLOB_WETNESS,
     DATA_POINT_GLOB_WIND,
     DATA_POINT_GLOB_WINDDIR,
     DATA_POINT_HEATINDEX,
     DATA_POINT_HOURLY_RAIN,
+    DATA_POINT_HRAIN_PIEZO,
     DATA_POINT_HUMI_CO2,
     DATA_POINT_HUMIDEX,
     DATA_POINT_HUMIDEX_PERCEPTION,
     DATA_POINT_HUMIDITY_ABS,
     DATA_POINT_HUMIDITY_ABS_IN,
     DATA_POINT_INTERVAL,
     DATA_POINT_LIGHTNING,
     DATA_POINT_LIGHTNING_NUM,
     DATA_POINT_LIGHTNING_TIME,
     DATA_POINT_MONTHLY_RAIN,
+    DATA_POINT_MRAIN_PIEZO,
     DATA_POINT_R_RAIN_PIEZO,
     DATA_POINT_RAIN_RATE,
     DATA_POINT_RELATIVE_STRAIN_INDEX,
     DATA_POINT_RELATIVE_STRAIN_INDEX_PERCEPTION,
     DATA_POINT_RUNTIME,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1,
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_2,
@@ -67,16 +71,18 @@
     DATA_POINT_SOLARRADIATION_PERCEIVED,
     DATA_POINT_TF_CO2,
     DATA_POINT_THERMAL_PERCEPTION,
     DATA_POINT_TOTAL_RAIN,
     DATA_POINT_UV,
     DATA_POINT_WEEKLY_RAIN,
     DATA_POINT_WINDCHILL,
+    DATA_POINT_WRAIN_PIEZO,
     DATA_POINT_WS90_VER,
     DATA_POINT_YEARLY_RAIN,
+    DATA_POINT_YRAIN_PIEZO,
     LOGGER,
 )
 from ecowitt2mqtt.data import ProcessedData
 from ecowitt2mqtt.helpers.calculator import CalculatedDataPoint, DataPointType
 from ecowitt2mqtt.helpers.calculator.battery import (
     BatteryStrategy,
     get_battery_strategy,
@@ -298,15 +304,15 @@
     ),
     DATA_POINT_LIGHTNING: EntityDescription(
         icon="mdi:map-marker-distance",
         state_class=StateClass.MEASUREMENT,
     ),
     DATA_POINT_LIGHTNING_NUM: EntityDescription(
         icon="mdi:weather-lightning",
-        state_class=StateClass.TOTAL,
+        state_class=StateClass.TOTAL_INCREASING,
     ),
     DATA_POINT_LIGHTNING_TIME: EntityDescription(
         device_class=DeviceClass.TIMESTAMP,
     ),
     DATA_POINT_R_RAIN_PIEZO: EntityDescription(
         icon="mdi:water",
         state_class=StateClass.MEASUREMENT,
@@ -387,22 +393,27 @@
 
 PLATFORM_MAP = {
     DataPointType.BOOLEAN: Platform.BINARY_SENSOR,
     DataPointType.NON_BOOLEAN: Platform.SENSOR,
 }
 
 STATE_CLASS_OVERRIDES = {
-    DATA_POINT_DAILY_RAIN: StateClass.TOTAL,
-    DATA_POINT_EVENT_RAIN: StateClass.TOTAL,
-    DATA_POINT_GLOB_RAIN_PIEZO: StateClass.TOTAL,
-    DATA_POINT_HOURLY_RAIN: StateClass.TOTAL,
-    DATA_POINT_MONTHLY_RAIN: StateClass.TOTAL,
-    DATA_POINT_TOTAL_RAIN: StateClass.TOTAL,
-    DATA_POINT_WEEKLY_RAIN: StateClass.TOTAL,
-    DATA_POINT_YEARLY_RAIN: StateClass.TOTAL,
+    DATA_POINT_DAILY_RAIN: StateClass.TOTAL_INCREASING,
+    DATA_POINT_DRAIN_PIEZO: StateClass.TOTAL_INCREASING,
+    DATA_POINT_ERAIN_PIEZO: StateClass.TOTAL_INCREASING,
+    DATA_POINT_EVENT_RAIN: StateClass.TOTAL_INCREASING,
+    DATA_POINT_HOURLY_RAIN: StateClass.MEASUREMENT,
+    DATA_POINT_HRAIN_PIEZO: StateClass.MEASUREMENT,
+    DATA_POINT_MONTHLY_RAIN: StateClass.TOTAL_INCREASING,
+    DATA_POINT_MRAIN_PIEZO: StateClass.TOTAL_INCREASING,
+    DATA_POINT_TOTAL_RAIN: StateClass.TOTAL_INCREASING,
+    DATA_POINT_WEEKLY_RAIN: StateClass.TOTAL_INCREASING,
+    DATA_POINT_WRAIN_PIEZO: StateClass.TOTAL_INCREASING,
+    DATA_POINT_YEARLY_RAIN: StateClass.TOTAL_INCREASING,
+    DATA_POINT_YRAIN_PIEZO: StateClass.TOTAL_INCREASING,
 }
 
 
 def get_availability_payload(
     data_point: CalculatedDataPoint,
 ) -> str:
     """Get the availability payload for a data point.
```

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/publisher/topic.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/publisher/topic.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/helpers/server.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/helpers/server.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/runtime.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/runtime.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/__init__.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/meteo.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/util/meteo.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/ecowitt2mqtt/util/unit_conversion.py` & `ecowitt2mqtt-2023.7.0/ecowitt2mqtt/util/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.6.1/pyproject.toml` & `ecowitt2mqtt-2023.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "ecowitt2mqtt"
-version = "2023.06.1"
+version = "2023.07.0"
 description = "A small web server to send data from Ecowitt devices to an MQTT Broker"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/ecowitt2mqtt"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -59,15 +59,15 @@
 ]
 
 [tool.poetry.dependencies]
 "ruamel.yaml" = "^0.17.21"
 aiohttp = "^3.8.1"
 asyncio-mqtt = ">=0.12.1"
 colorlog = "^6.6.0"
-fastapi = ">=0.89.1,<0.98.0"
+fastapi = ">=0.89.1,<0.99.0"
 meteocalc = "^1.1.0"
 python = "^3.9.0"
 python-multipart = ">=0.0.5,<0.0.7"
 rapidfuzz = ">=2.13,<4.0"
 uvicorn = ">=0.19.0"
 uvloop = "^0.17.0"
 voluptuous = "^0.13.1"
@@ -87,15 +87,15 @@
 pylint = "^2.15.5"
 pytest = "^7.2.0"
 pytest-aiohttp = "^1.0.0"
 pytest-asyncio = ">=0.20.1,<0.22.0"
 pytest-cov = "^4.0.0"
 pyupgrade = "^3.1.0"
 requests = ">=2.31.0"
-ruff = ">=0.0.261,<0.0.273"
+ruff = ">=0.0.261,<0.0.276"
 safety = "^2.3.1"
 typing-extensions = "^4.4.0"
 vulture = "^2.6"
 yamllint = "^1.28.0"
 
 [tool.poetry.scripts]
 ecowitt2mqtt = "ecowitt2mqtt.__main__:main"
```

### Comparing `ecowitt2mqtt-2023.6.1/PKG-INFO` & `ecowitt2mqtt-2023.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecowitt2mqtt
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: A small web server to send data from Ecowitt devices to an MQTT Broker
 Home-page: https://github.com/bachya/ecowitt2mqtt
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: asyncio-mqtt (>=0.12.1)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
-Requires-Dist: fastapi (>=0.89.1,<0.98.0)
+Requires-Dist: fastapi (>=0.89.1,<0.99.0)
 Requires-Dist: meteocalc (>=1.1.0,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.7)
 Requires-Dist: rapidfuzz (>=2.13,<4.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: uvicorn (>=0.19.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: voluptuous (>=0.13.1,<0.14.0)
@@ -203,15 +203,16 @@
                         ecowitt2mqtt on (default: /data/report)
   --hass-discovery      Publish data in the Home Assistant MQTT
                         Discovery format
   --hass-discovery-prefix hass_discovery_prefix
                         The Home Assistant MQTT Discovery topic prefix
                         to use (default: homeassistant)
   --hass-entity-id-prefix hass_entity_id_prefix
-                        The prefix to use for Home Assistant entity IDs
+                        The prefix to use for Home Assistant entity IDs.
+                        Example: A prefix of 'prefix' will prepend 'prefix_' to entity IDs.
   --input-data-format input_data_format
                         The input data format used by the gateway
                         (default: ecowitt)
   --input-unit-system input_unit_system
                         The input unit system used by the gateway
                         (default: imperial)
   -b mqtt_broker, --mqtt-broker mqtt_broker
@@ -261,15 +262,16 @@
   --output-unit-temperature output_unit_temperature
                         The output unit to use for temperature data
                         points (default: the default used by the output
                         unit system)
   --port port           The port to serve ecowitt2mqtt on (default:
                         8080)
   --precision precision
-                        The precision to output data points at
+                        The precision to output data points at.
+                        Example: A value of 2 will round to two decimal places
                         (default: no limit)
   --raw-data            Return raw data (don't attempt to translate any
                         values)
   -v, --verbose         Increase verbosity of logged output
 ```
 
 ## Environment Variables
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.6.1 Summary: A small web
+Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.7.0 Summary: A small web
 server to send data from Ecowitt devices to an MQTT Broker Home-page: https://
 github.com/bachya/ecowitt2mqtt License: MIT Author: Aaron Bach Author-email:
 bachya1208@gmail.com Requires-Python: >=3.9.0,<4.0.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
 Dist: asyncio-mqtt (>=0.12.1) Requires-Dist: colorlog (>=6.6.0,<7.0.0)
-Requires-Dist: fastapi (>=0.89.1,<0.98.0) Requires-Dist: meteocalc
+Requires-Dist: fastapi (>=0.89.1,<0.99.0) Requires-Dist: meteocalc
 (>=1.1.0,<2.0.0) Requires-Dist: python-multipart (>=0.0.5,<0.0.7) Requires-
 Dist: rapidfuzz (>=2.13,<4.0) Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: uvicorn (>=0.19.0) Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: voluptuous (>=0.13.1,<0.14.0) Project-URL: Bug Tracker, https://
 github.com/bachya/ecowitt2mqtt/issues Project-URL: Changelog, https://
 github.com/bachya/ecowitt2mqtt/releases Project-URL: Repository, https://
 github.com/bachya/ecowitt2mqtt Description-Content-Type: text/markdown !
@@ -94,48 +94,49 @@
 config strategy to use (default: boolean) --diagnostics Output diagnostics --
 disable-calculated-data Disable the output of calculated sensors -e endpoint, -
 -endpoint endpoint The relative endpoint/path to serve ecowitt2mqtt on
 (default: /data/report) --hass-discovery Publish data in the Home Assistant
 MQTT Discovery format --hass-discovery-prefix hass_discovery_prefix The Home
 Assistant MQTT Discovery topic prefix to use (default: homeassistant) --hass-
 entity-id-prefix hass_entity_id_prefix The prefix to use for Home Assistant
-entity IDs --input-data-format input_data_format The input data format used by
-the gateway (default: ecowitt) --input-unit-system input_unit_system The input
-unit system used by the gateway (default: imperial) -b mqtt_broker, --mqtt-
-broker mqtt_broker The hostname or IP address of an MQTT broker -
-p mqtt_password, --mqtt-password mqtt_password A valid password for the MQTT
-broker --mqtt-port mqtt_port The listenting port of the MQTT broker (default:
-1883) --mqtt-retain Instruct the MQTT broker to retain messages --mqtt-tls
-Enable MQTT over TLS -t mqtt_topic, --mqtt-topic mqtt_topic The MQTT topic to
-publish device data to -u mqtt_username, --mqtt-username mqtt_username A valid
-username for the MQTT broker --output-unit-system output_unit_system The output
-unit system used by the gateway (default: imperial) --output-unit-accumulated-
-precipitation output_unit_accumulated_precipitation The output unit to use for
-accumulated precipitation data points (default: the default used by the output
-unit system) --output-unit-distance output_unit_distance The output unit to use
-for distance data points (default: the default used by the output unit system)
---output-unit-humidity output_unit_humidity The output unit to use for humidity
+entity IDs. Example: A prefix of 'prefix' will prepend 'prefix_' to entity IDs.
+--input-data-format input_data_format The input data format used by the gateway
+(default: ecowitt) --input-unit-system input_unit_system The input unit system
+used by the gateway (default: imperial) -b mqtt_broker, --mqtt-broker
+mqtt_broker The hostname or IP address of an MQTT broker -p mqtt_password, --
+mqtt-password mqtt_password A valid password for the MQTT broker --mqtt-port
+mqtt_port The listenting port of the MQTT broker (default: 1883) --mqtt-retain
+Instruct the MQTT broker to retain messages --mqtt-tls Enable MQTT over TLS -
+t mqtt_topic, --mqtt-topic mqtt_topic The MQTT topic to publish device data to
+-u mqtt_username, --mqtt-username mqtt_username A valid username for the MQTT
+broker --output-unit-system output_unit_system The output unit system used by
+the gateway (default: imperial) --output-unit-accumulated-precipitation
+output_unit_accumulated_precipitation The output unit to use for accumulated
+precipitation data points (default: the default used by the output unit system)
+--output-unit-distance output_unit_distance The output unit to use for distance
 data points (default: the default used by the output unit system) --output-
-unit-illuminance output_unit_illuminance The output unit to use for illuminance
-data points (default: the default used by the output unit system) --output-
-unit-precipitation-rate output_unit_precipitation_rate The output unit to use
-for precipitation rate data points (default: the default used by the output
-unit system) --output-unit-pressure output_unit_pressure The output unit to use
-for pressure data points (default: the default used by the output unit system)
---output-unit-speed output_unit_speed The output unit to use for speed data
+unit-humidity output_unit_humidity The output unit to use for humidity data
+points (default: the default used by the output unit system) --output-unit-
+illuminance output_unit_illuminance The output unit to use for illuminance data
+points (default: the default used by the output unit system) --output-unit-
+precipitation-rate output_unit_precipitation_rate The output unit to use for
+precipitation rate data points (default: the default used by the output unit
+system) --output-unit-pressure output_unit_pressure The output unit to use for
+pressure data points (default: the default used by the output unit system) --
+output-unit-speed output_unit_speed The output unit to use for speed data
 points (default: the default used by the output unit system) --output-unit-
 temperature output_unit_temperature The output unit to use for temperature data
 points (default: the default used by the output unit system) --port port The
 port to serve ecowitt2mqtt on (default: 8080) --precision precision The
-precision to output data points at (default: no limit) --raw-data Return raw
-data (don't attempt to translate any values) -v, --verbose Increase verbosity
-of logged output ``` ## Environment Variables -
-`ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-delimited list of key=value
-battery overrides (default: `numeric`) - `ECOWITT2MQTT_CONFIG`: a path to a
-YAML or JSON config file (default: `None`) -
+precision to output data points at. Example: A value of 2 will round to two
+decimal places (default: no limit) --raw-data Return raw data (don't attempt to
+translate any values) -v, --verbose Increase verbosity of logged output ``` ##
+Environment Variables - `ECOWITT2MQTT_BATTERY_OVERRIDE`: a semicolon-delimited
+list of key=value battery overrides (default: `numeric`) -
+`ECOWITT2MQTT_CONFIG`: a path to a YAML or JSON config file (default: `None`) -
 `ECOWITT2MQTT_DEFAULT_BATTERY_STRATEGY`: the default battery config strategy to
 use (default: `boolean`) - `ECOWITT2MQTT_DIAGNOSTICS`: whether to output
 diagnostics (default: `false`) - `ECOWITT2MQTT_DISABLE_CALCULATED_DATA`:
 whether to disable the output of calculated sensors (default: `false`) -
 `ECOWITT2MQTT_ENDPOINT`: the relative endpoint/path to serve ecowitt2mqtt on
 (default: `/data/report`) - `ECOWITT2MQTT_HASS_DISCOVERY_PREFIX`: the Home
 Assistant discovery prefix to use (default: `homeassistant`) -
```

