# Comparing `tmp/ecowitt2mqtt-2024.1.2.tar.gz` & `tmp/ecowitt2mqtt-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecowitt2mqtt-2024.1.2.tar", max compression
+gzip compressed data, was "ecowitt2mqtt-2024.4.0.tar", max compression
```

## Comparing `ecowitt2mqtt-2024.1.2.tar` & `ecowitt2mqtt-2024.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1072 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/LICENSE
--rw-r--r--   0        0        0    30731 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/README.md
--rw-r--r--   0        0        0       39 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/__init__.py
--rw-r--r--   0        0        0    12825 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/__main__.py
--rw-r--r--   0        0        0       24 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/backports/__init__.py
--rw-r--r--   0        0        0     1403 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/backports/enum.py
--rw-r--r--   0        0        0    12567 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/config.py
--rw-r--r--   0        0        0    11078 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/const.py
--rw-r--r--   0        0        0     2241 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/core.py
--rw-r--r--   0        0        0    12651 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/data.py
--rw-r--r--   0        0        0      107 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/errors.py
--rw-r--r--   0        0        0       22 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/__init__.py
--rw-r--r--   0        0        0     6587 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/__init__.py
--rw-r--r--   0        0        0     4932 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/battery.py
--rw-r--r--   0        0        0      474 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/heap.py
--rw-r--r--   0        0        0     2269 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/humidity.py
--rw-r--r--   0        0        0     2439 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/illuminance.py
--rw-r--r--   0        0        0     1018 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/leak.py
--rw-r--r--   0        0        0     1991 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/lightning.py
--rw-r--r--   0        0        0      725 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/pollution.py
--rw-r--r--   0        0        0     2751 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/precipitation.py
--rw-r--r--   0        0        0     1369 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/pressure.py
--rw-r--r--   0        0        0    22016 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/temperature.py
--rw-r--r--   0        0        0     1624 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/time.py
--rw-r--r--   0        0        0     4614 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/uv.py
--rw-r--r--   0        0        0     9535 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/wind.py
--rw-r--r--   0        0        0     1665 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/device.py
--rw-r--r--   0        0        0      794 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/__init__.py
--rw-r--r--   0        0        0      844 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/factory.py
--rw-r--r--   0        0        0     2401 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/mqtt/__init__.py
--rw-r--r--   0        0        0    20019 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/mqtt/hass.py
--rw-r--r--   0        0        0     6968 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/server.py
--rw-r--r--   0        0        0      292 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/typing.py
--rw-r--r--   0        0        0     7161 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/runtime.py
--rw-r--r--   0        0        0     1414 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/util/__init__.py
--rw-r--r--   0        0        0      491 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/util/dt.py
--rw-r--r--   0        0        0     7882 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/util/meteo.py
--rw-r--r--   0        0        0    12118 2024-01-23 01:16:26.113865 ecowitt2mqtt-2024.1.2/ecowitt2mqtt/util/unit_conversion.py
--rw-r--r--   0        0        0     4409 2024-01-23 01:16:26.117865 ecowitt2mqtt-2024.1.2/pyproject.toml
--rw-r--r--   0        0        0    32328 1970-01-01 00:00:00.000000 ecowitt2mqtt-2024.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/LICENSE
+-rw-r--r--   0        0        0    30731 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/README.md
+-rw-r--r--   0        0        0       39 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/__init__.py
+-rw-r--r--   0        0        0    12826 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/__main__.py
+-rw-r--r--   0        0        0       24 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/backports/__init__.py
+-rw-r--r--   0        0        0     1404 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/backports/enum.py
+-rw-r--r--   0        0        0    12566 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/config.py
+-rw-r--r--   0        0        0    11079 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/const.py
+-rw-r--r--   0        0        0     2242 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/core.py
+-rw-r--r--   0        0        0    12652 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/data.py
+-rw-r--r--   0        0        0      107 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/errors.py
+-rw-r--r--   0        0        0       22 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/__init__.py
+-rw-r--r--   0        0        0     6588 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/__init__.py
+-rw-r--r--   0        0        0     4933 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/battery.py
+-rw-r--r--   0        0        0      475 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/heap.py
+-rw-r--r--   0        0        0     2270 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/humidity.py
+-rw-r--r--   0        0        0     2440 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/illuminance.py
+-rw-r--r--   0        0        0     1019 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/leak.py
+-rw-r--r--   0        0        0     1992 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/lightning.py
+-rw-r--r--   0        0        0      726 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/pollution.py
+-rw-r--r--   0        0        0     2752 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/precipitation.py
+-rw-r--r--   0        0        0     1370 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/pressure.py
+-rw-r--r--   0        0        0    22316 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/temperature.py
+-rw-r--r--   0        0        0     1625 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/time.py
+-rw-r--r--   0        0        0     4615 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/uv.py
+-rw-r--r--   0        0        0     9538 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/wind.py
+-rw-r--r--   0        0        0     1691 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/device.py
+-rw-r--r--   0        0        0      795 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/factory.py
+-rw-r--r--   0        0        0     2402 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/mqtt/__init__.py
+-rw-r--r--   0        0        0    20020 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/mqtt/hass.py
+-rw-r--r--   0        0        0     6969 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/server.py
+-rw-r--r--   0        0        0      293 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/typing.py
+-rw-r--r--   0        0        0     7162 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/runtime.py
+-rw-r--r--   0        0        0     1415 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/util/__init__.py
+-rw-r--r--   0        0        0      492 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/util/dt.py
+-rw-r--r--   0        0        0     7883 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/util/meteo.py
+-rw-r--r--   0        0        0    12119 2024-04-05 02:16:43.726539 ecowitt2mqtt-2024.4.0/ecowitt2mqtt/util/unit_conversion.py
+-rw-r--r--   0        0        0     4413 2024-04-05 02:16:43.730539 ecowitt2mqtt-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0    32329 1970-01-01 00:00:00.000000 ecowitt2mqtt-2024.4.0/PKG-INFO
```

### Comparing `ecowitt2mqtt-2024.1.2/LICENSE` & `ecowitt2mqtt-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2024.1.2/README.md` & `ecowitt2mqtt-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/__main__.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the main interface to the CLI."""
+
 from __future__ import annotations
 
 import argparse
 import os
 import sys
 from typing import Any
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/backports/enum.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/backports/enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Define enum backports from the standard library.
 
 https://github.com/clbarnes/backports.strenum
 """
+
 from enum import Enum
 from typing import TypeVar
 
 _S = TypeVar("_S", bound="StrEnum")
 
 
 class StrEnum(str, Enum):
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/config.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define a configuration management module."""
+
 from __future__ import annotations
 
 import os
 from collections.abc import Generator
 from numbers import Number
 from typing import Any
 from uuid import uuid4
@@ -19,16 +20,16 @@
 
 from ecowitt2mqtt.const import (
     CONF_BATTERY_OVERRIDES,
     CONF_CONFIG,
     CONF_DIAGNOSTICS,
     CONF_GATEWAYS,
     CONF_HASS_DISCOVERY,
-    CONF_MQTT_BROKER,
     CONF_MQTT_PASSWORD,
+    CONF_MQTT_TOPIC,
     CONF_MQTT_USERNAME,
     CONF_VERBOSE,
     DEFAULT_BOOLEAN_BATTERY_TRUE_VALUE,
     DEFAULT_ENDPOINT,
     DEFAULT_HASS_DISCOVERY_PREFIX,
     DEFAULT_MQTT_PORT,
     DEFAULT_PORT,
@@ -46,15 +47,15 @@
 from ecowitt2mqtt.errors import EcowittError
 from ecowitt2mqtt.helpers.calculator.battery import BatteryStrategy
 from ecowitt2mqtt.helpers.server import InputDataFormat
 
 CONF_DEFAULT = "default"
 
 REQUIRES_AT_LEAST_ONE_OF = (
-    CONF_MQTT_BROKER,
+    CONF_MQTT_TOPIC,
     CONF_HASS_DISCOVERY,
 )
 
 TRUTHY_VALUES = {"1", "true", "yes", "on", "enable"}
 FALSEY_VALUES = {"0", "false", "no", "off", "disable"}
 
 BOOLEAN_BATTERY_TRUE_VALUES = {0, 1}
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/const.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Define package constants."""
+
 import logging
 from typing import Final
 
 from ecowitt2mqtt.backports.enum import StrEnum
 
-__version__ = "2024.01.2"
+__version__ = "2024.04.0"
 
 LOGGER = logging.getLogger(__package__)
 
 # Configuration keys:
 CONF_BATTERY_OVERRIDES: Final = "battery_overrides"
 CONF_BOOLEAN_BATTERY_TRUE_VALUE: Final = "boolean_battery_true_value"
 CONF_CONFIG: Final = "config"
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/core.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the core application objects."""
+
 from __future__ import annotations
 
 import logging
 import sys
 from typing import Any
 
 import colorlog
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/data.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define data processing."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any
 
 from ecowitt2mqtt.config import Config
 from ecowitt2mqtt.const import (
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/__init__.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define various calculators."""
+
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable
 from dataclasses import dataclass, field
 from enum import Enum
 from functools import wraps
 from typing import TYPE_CHECKING, Any, TypeVar, cast
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/battery.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/battery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define battery calculators."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, cast
 
 from ecowitt2mqtt.backports.enum import StrEnum
 from ecowitt2mqtt.const import (
     DATA_POINT_CO2_BATT,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/humidity.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/humidity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define humidity calculators."""
+
 from __future__ import annotations
 
 from typing import cast
 
 from ecowitt2mqtt.const import (
     CONF_OUTPUT_UNIT_HUMIDITY,
     DATA_POINT_HUMIDITY,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/illuminance.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/illuminance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define illuminance calculators."""
+
 from __future__ import annotations
 
 from typing import cast
 
 from ecowitt2mqtt.const import (
     CONF_OUTPUT_UNIT_ILLUMINANCE,
     DATA_POINT_SOLARRADIATION,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/leak.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/leak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define moisture calculators."""
+
 from __future__ import annotations
 
 from ecowitt2mqtt.backports.enum import StrEnum
 from ecowitt2mqtt.helpers.calculator import (
     CalculatedDataPoint,
     Calculator,
     DataPointType,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/lightning.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/lightning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define lightning-related calculators."""
+
 from __future__ import annotations
 
 from ecowitt2mqtt.const import CONF_OUTPUT_UNIT_DISTANCE, STRIKES, UnitOfLength
 from ecowitt2mqtt.helpers.calculator import (
     CalculatedDataPoint,
     CalculationFailedError,
     Calculator,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/pollution.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/pollution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define pollution calculators."""
+
 from __future__ import annotations
 
 from ecowitt2mqtt.const import (
     DATA_POINT_CO2,
     DATA_POINT_CO2_24H,
     UnitOfPollutionConcentration,
 )
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/precipitation.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/precipitation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define precipitation calculators."""
+
 from __future__ import annotations
 
 from typing import cast
 
 from ecowitt2mqtt.const import (
     CONF_OUTPUT_UNIT_ACCUMULATED_PRECIPITATION,
     CONF_OUTPUT_UNIT_PRECIPITATION_RATE,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/pressure.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/pressure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define pressure calculators."""
+
 from __future__ import annotations
 
 from typing import cast
 
 from ecowitt2mqtt.const import CONF_OUTPUT_UNIT_PRESSURE, UnitOfPressure
 from ecowitt2mqtt.helpers.calculator import CalculatedDataPoint, Calculator
 from ecowitt2mqtt.helpers.typing import PreCalculatedValueType
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/temperature.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/temperature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define temperature calculators."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import cast
 
 import meteocalc
 
@@ -490,17 +491,24 @@
         Returns:
             A parsed CalculatedDataPoint object.
         """
         temp = cast(float, payload[DATA_POINT_TEMP])
         humidity = cast(float, payload[DATA_POINT_HUMIDITY])
 
         humidex = get_humidex(temp, humidity, self._config.input_unit_system)
-        [rating] = [
-            r for r in HUMIDEX_PERCEPTION_RATINGS if r.minimum <= humidex < r.maximum
-        ]
+
+        try:
+            rating = next(
+                r
+                for r in HUMIDEX_PERCEPTION_RATINGS
+                if r.minimum <= humidex < r.maximum
+            )
+        except StopIteration:
+            return self.get_calculated_data_point(None)
+
         return self.get_calculated_data_point(rating.perception)
 
 
 class RsiCalculator(Calculator):
     """Define a relative strain index calculator."""
 
     @Calculator.requires_keys(DATA_POINT_TEMP, DATA_POINT_HUMIDITY)
@@ -551,19 +559,20 @@
             rsi = get_relative_strain_index(
                 temp, humidity, self._config.input_unit_system
             )
         except ValueError as err:
             LOGGER.debug("%s", err)
             return self.get_calculated_data_point(None)
 
-        [rating] = [
+        rating = next(
             r
             for r in RELATIVE_STRAIN_INDEX_PERCEPTION_RATINGS
             if r.minimum <= rsi < r.maximum
-        ]
+        )
+
         return self.get_calculated_data_point(rating.perception)
 
 
 class SimmerIndexCalculator(BaseTemperatureCalculator):
     """Define a simmer index calculator."""
 
     @Calculator.requires_keys(DATA_POINT_TEMP, DATA_POINT_HUMIDITY)
@@ -626,17 +635,23 @@
             )
         except ValueError as err:
             LOGGER.debug("%s (temperature: %s)", err, temp_obj)
             return self.get_calculated_data_point(None)
 
         simmer_obj = cast(meteocalc.Temp, simmer_obj)
 
-        [rating] = [
-            r for r in SIMMER_ZONE_RATINGS if r.minimum_f <= simmer_obj.f < r.maximum_f
-        ]
+        try:
+            rating = next(
+                r
+                for r in SIMMER_ZONE_RATINGS
+                if r.minimum_f <= simmer_obj.f < r.maximum_f
+            )
+        except StopIteration:
+            return self.get_calculated_data_point(None)
+
         return self.get_calculated_data_point(rating.zone)
 
 
 class TemperatureCalculator(BaseTemperatureCalculator):
     """Define a temperature calculator."""
 
     def calculate_from_value(
@@ -687,19 +702,20 @@
         temp = cast(float, payload[DATA_POINT_TEMP])
         humidity = cast(float, payload[DATA_POINT_HUMIDITY])
 
         dew_point_obj = get_dew_point_meteocalc_object(
             temp, humidity, self._config.input_unit_system
         )
 
-        [rating] = [
+        rating = next(
             r
             for r in THERMAL_PERCEPTION_RATINGS
             if r.minimum_c <= dew_point_obj.c < r.maximum_c
-        ]
+        )
+
         return self.get_calculated_data_point(rating.perception)
 
 
 class WindChillCalculator(BaseTemperatureCalculator):
     """Define a wind chill calculator."""
 
     @Calculator.requires_keys(DATA_POINT_TEMP, DATA_POINT_WINDSPEED)
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/time.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/time.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define time calculators."""
+
 from __future__ import annotations
 
 from ecowitt2mqtt.const import UnitOfTime
 from ecowitt2mqtt.helpers.calculator import (
     CalculatedDataPoint,
     CalculationFailedError,
     Calculator,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/uv.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/uv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define UV index calculators."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import cast
 
 from ecowitt2mqtt.const import (
     DATA_POINT_SAFE_EXPOSURE_TIME_SKIN_TYPE_1,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/calculator/wind.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/calculator/wind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define wind calculators."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import cast
 
 from ecowitt2mqtt.const import (
     CONF_OUTPUT_UNIT_SPEED,
@@ -230,26 +231,26 @@
             payload: An Ecowitt data payload.
 
         Returns:
             A parsed CalculatedDataPoint object.
         """
         wind_speed = cast(float, payload[DATA_POINT_WINDSPEED])
 
-        [rating] = [
+        rating = next(
             r
             for r in BEAUFORT_SCALE_RATINGS
             if (
                 self._config.input_unit_system == UnitSystem.IMPERIAL
                 and r.minimum_mph <= wind_speed < r.maximum_mph
             )
             or (
                 self._config.input_unit_system == UnitSystem.METRIC
                 and r.minimum_kmh <= wind_speed < r.maximum_kmh
             )
-        ]
+        )
 
         return self.get_calculated_data_point(
             rating.number,
             attributes={
                 "description": rating.description,
                 "sea_conditions": rating.sea_conditions,
                 "land_conditions": rating.land_conditions,
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/device.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define an Ecowitt device."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any
 
 from ecowitt2mqtt.util import glob_search
 
@@ -13,14 +14,15 @@
 MODEL_BRAND_MAP = {
     "GW1000": "Ecowitt",
     "GW1100": "Ecowitt",
     "GW2000": "Ecowitt",
     "HP2550": "Ecowitt",
     "HP2551": "Ecowitt",
     "HP2553": "Ecowitt",
+    "HP2561": "Ecowitt",
     "HP2564": "Ecowitt",
     "PT-HP2550": "Fine Offset",
     "WH2650": "Fine Offset",
     "WS2350": "La Crosse",
     "WS2900": "Ambient Weather",
 }
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/__init__.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define helpers to publish Ecowitt payloads."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 from ecowitt2mqtt.config import Config
 from ecowitt2mqtt.helpers.typing import CalculatedValueType
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/factory.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define a publisher factory."""
+
 from __future__ import annotations
 
 from aiomqtt import Client
 
 from ecowitt2mqtt.config import Config
 from ecowitt2mqtt.helpers.publisher import Publisher
 from ecowitt2mqtt.helpers.publisher.mqtt import TopicPublisher
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/mqtt/__init__.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/mqtt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define MQTT publishers."""
+
 from __future__ import annotations
 
 import json
 from datetime import datetime
 from typing import Any, cast
 
 from aiomqtt import Client
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/publisher/mqtt/hass.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/publisher/mqtt/hass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define MQTT publishing."""
+
 # pylint: disable=unused-argument
 from __future__ import annotations
 
 import asyncio
 from dataclasses import asdict, dataclass
 from typing import TypedDict
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/helpers/server.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/helpers/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define various API server helpers."""
+
 from __future__ import annotations
 
 import urllib.parse
 from abc import ABC, abstractmethod
 from collections.abc import Callable
 from typing import Any
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/runtime.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define runtime management."""
+
 from __future__ import annotations
 
 import asyncio
 import traceback
 from collections.abc import AsyncGenerator
 from contextlib import asynccontextmanager, suppress
 from ssl import SSLContext
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/util/__init__.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/util/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define utilities."""
+
 from __future__ import annotations
 
 from typing import TypeVar
 
 from rapidfuzz import fuzz
 
 T = TypeVar("T")
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/util/meteo.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/util/meteo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define various meteorological utils."""
+
 from __future__ import annotations
 
 import math
 from typing import cast
 
 import meteocalc
```

### Comparing `ecowitt2mqtt-2024.1.2/ecowitt2mqtt/util/unit_conversion.py` & `ecowitt2mqtt-2024.4.0/ecowitt2mqtt/util/unit_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define unit conversion helpers."""
+
 from __future__ import annotations
 
 import math
 
 from ecowitt2mqtt.backports.enum import StrEnum
 from ecowitt2mqtt.const import (
     ACCUMULATED_PRECIPITATION,
```

### Comparing `ecowitt2mqtt-2024.1.2/pyproject.toml` & `ecowitt2mqtt-2024.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "ecowitt2mqtt"
-version = "2024.01.2"
+version = "2024.04.0"
 description = "A small web server to send data from Ecowitt devices to an MQTT Broker"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/ecowitt2mqtt"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -63,19 +63,19 @@
 [tool.poetry.dependencies]
 "ruamel.yaml" = ">=0.18.5"
 "ruamel.yaml.clib" = ">=0.2.8,<0.3.0"
 aiohttp = ">=3.9.0b0"
 aiomqtt = ">=1,<3"
 certifi = ">=2023.07.22"
 colorlog = "^6.6.0"
-fastapi = ">=0.89.1,<0.110.0"
+fastapi = ">=0.89.1,<0.111.0"
 frozenlist = "^1.4.0"
 meteocalc = "^1.1.0"
 python = "^3.10"
-python-multipart = ">=0.0.5,<0.0.7"
+python-multipart = ">=0.0.5,<0.0.10"
 rapidfuzz = ">=2.13,<4.0"
 urllib3 = ">=1.26.18"
 uvicorn = ">=0.19.0"
 uvloop = ">=0.17,<0.20"
 yarl = ">=1.9.2"
 pydantic = "^2.5.3"
 
@@ -88,22 +88,22 @@
 coverage = {version = ">=6.5,<8.0", extras = ["toml"]}
 darglint = "^1.8.1"
 isort = "^5.10.1"
 mypy = "^1.2.0"
 pre-commit = ">=2.20,<4.0"
 pre-commit-hooks = "^4.3.0"
 pylint = ">=2.15.5,<4.0.0"
-pytest = "^7.2.0"
+pytest = ">=7.2,<9.0"
 pytest-aiohttp = "^1.0.0"
 pytest-asyncio = ">=0.20.1,<0.24.0"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 pyupgrade = "^3.1.0"
 pyyaml = "^6.0.1"
 requests = ">=2.31.0"
-ruff = ">=0.0.261,<0.1.15"
+ruff = ">=0.0.261,<0.3.6"
 typing-extensions = "^4.8.0"
 vulture = "^2.6"
 yamllint = "^1.28.0"
 
 [tool.poetry.scripts]
 ecowitt2mqtt = "ecowitt2mqtt.__main__:main"
```

### Comparing `ecowitt2mqtt-2024.1.2/PKG-INFO` & `ecowitt2mqtt-2024.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecowitt2mqtt
-Version: 2024.1.2
+Version: 2024.4.0
 Summary: A small web server to send data from Ecowitt devices to an MQTT Broker
 Home-page: https://github.com/bachya/ecowitt2mqtt
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,19 +15,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: aiohttp (>=3.9.0b0)
 Requires-Dist: aiomqtt (>=1,<3)
 Requires-Dist: certifi (>=2023.07.22)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
-Requires-Dist: fastapi (>=0.89.1,<0.110.0)
+Requires-Dist: fastapi (>=0.89.1,<0.111.0)
 Requires-Dist: frozenlist (>=1.4.0,<2.0.0)
 Requires-Dist: meteocalc (>=1.1.0,<2.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: python-multipart (>=0.0.5,<0.0.7)
+Requires-Dist: python-multipart (>=0.0.5,<0.0.10)
 Requires-Dist: rapidfuzz (>=2.13,<4.0)
 Requires-Dist: ruamel.yaml (>=0.18.5)
 Requires-Dist: ruamel.yaml.clib (>=0.2.8,<0.3.0)
 Requires-Dist: urllib3 (>=1.26.18)
 Requires-Dist: uvicorn (>=0.19.0)
 Requires-Dist: uvloop (>=0.17,<0.20)
 Requires-Dist: yarl (>=1.9.2)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2024.1.2 Summary: A small web
+Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2024.4.0 Summary: A small web
 server to send data from Ecowitt devices to an MQTT Broker Home-page: https://
 github.com/bachya/ecowitt2mqtt License: MIT Author: Aaron Bach Author-email:
 bachya1208@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Requires-Dist: aiohttp (>=3.9.0b0) Requires-Dist:
 aiomqtt (>=1,<3) Requires-Dist: certifi (>=2023.07.22) Requires-Dist: colorlog
-(>=6.6.0,<7.0.0) Requires-Dist: fastapi (>=0.89.1,<0.110.0) Requires-Dist:
+(>=6.6.0,<7.0.0) Requires-Dist: fastapi (>=0.89.1,<0.111.0) Requires-Dist:
 frozenlist (>=1.4.0,<2.0.0) Requires-Dist: meteocalc (>=1.1.0,<2.0.0) Requires-
 Dist: pydantic (>=2.5.3,<3.0.0) Requires-Dist: python-multipart
-(>=0.0.5,<0.0.7) Requires-Dist: rapidfuzz (>=2.13,<4.0) Requires-Dist:
+(>=0.0.5,<0.0.10) Requires-Dist: rapidfuzz (>=2.13,<4.0) Requires-Dist:
 ruamel.yaml (>=0.18.5) Requires-Dist: ruamel.yaml.clib (>=0.2.8,<0.3.0)
 Requires-Dist: urllib3 (>=1.26.18) Requires-Dist: uvicorn (>=0.19.0) Requires-
 Dist: uvloop (>=0.17,<0.20) Requires-Dist: yarl (>=1.9.2) Project-URL: Bug
 Tracker, https://github.com/bachya/ecowitt2mqtt/issues Project-URL: Changelog,
 https://github.com/bachya/ecowitt2mqtt/releases Project-URL: Repository, https:
 //github.com/bachya/ecowitt2mqtt Description-Content-Type: text/markdown !
 [ecowitt2mqtt][logo] [![CI][ci-badge]][ci] [![PyPI][pypi-badge]][pypi] [!
```

