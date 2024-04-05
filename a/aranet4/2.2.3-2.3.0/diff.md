# Comparing `tmp/aranet4-2.2.3.tar.gz` & `tmp/aranet4-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aranet4-2.2.3.tar", last modified: Mon Jan 22 04:59:38 2024, max compression
+gzip compressed data, was "aranet4-2.3.0.tar", last modified: Fri Apr  5 17:06:52 2024, max compression
```

## Comparing `aranet4-2.2.3.tar` & `aranet4-2.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-01-22 04:59:38.268603 aranet4-2.2.3/
--rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.2.3/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     6477 2024-01-22 04:59:38.268603 aranet4-2.2.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-12-06 11:57:48.000000 aranet4-2.2.3/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-01-22 04:59:38.248603 aranet4-2.2.3/aranet4/
--rw-r--r--   0 pi        (1000) pi        (1000)      129 2024-01-22 04:49:31.000000 aranet4-2.2.3/aranet4/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9122 2024-01-22 04:45:05.000000 aranet4-2.2.3/aranet4/aranetctl.py
--rw-r--r--   0 pi        (1000) pi        (1000)    27612 2024-01-22 04:45:05.000000 aranet4-2.2.3/aranet4/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-01-22 04:59:38.264603 aranet4-2.2.3/aranet4.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     6477 2024-01-22 04:59:37.000000 aranet4-2.2.3/aranet4.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-01-22 04:59:37.000000 aranet4-2.2.3/aranet4.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-01-22 04:59:37.000000 aranet4-2.2.3/aranet4.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-01-22 04:59:37.000000 aranet4-2.2.3/aranet4.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-01-22 04:59:37.000000 aranet4-2.2.3/aranet4.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-01-22 04:59:37.000000 aranet4-2.2.3/aranet4.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-01-22 04:59:38.272603 aranet4-2.2.3/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      759 2024-01-22 04:49:51.000000 aranet4-2.2.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-05 17:06:52.293854 aranet4-2.3.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.0/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     6477 2024-04-05 17:06:52.277854 aranet4-2.3.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-12-06 11:57:48.000000 aranet4-2.3.0/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-05 17:06:52.245854 aranet4-2.3.0/aranet4/
+-rw-r--r--   0 pi        (1000) pi        (1000)      129 2024-04-05 16:46:51.000000 aranet4-2.3.0/aranet4/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7886 2024-04-05 16:45:21.000000 aranet4-2.3.0/aranet4/aranetctl.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    35313 2024-04-05 16:35:20.000000 aranet4-2.3.0/aranet4/client.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-05 17:06:52.273854 aranet4-2.3.0/aranet4.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6477 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-04-05 17:06:51.000000 aranet4-2.3.0/aranet4.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-05 17:06:52.293854 aranet4-2.3.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      759 2024-04-05 16:47:26.000000 aranet4-2.3.0/setup.py
```

### Comparing `aranet4-2.2.3/LICENSE` & `aranet4-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aranet4-2.2.3/PKG-INFO` & `aranet4-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.2.3
+Version: 2.3.0
 Summary: Aranet4 and Aranet2 Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aranet4-2.2.3/README.md` & `aranet4-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aranet4-2.2.3/aranet4/aranetctl.py` & `aranet4-2.3.0/aranet4/aranetctl.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,45 +6,14 @@
 import sys
 from time import sleep
 
 import requests
 
 from aranet4 import client
 
-format_str = """
---------------------------------------
- Connected: {current.name} | {current.version}
- Updated {current.ago} s ago. Intervals: {current.interval} s
- {current.stored} total log_size
- --------------------------------------
- CO2:            {current.co2} ppm
- Temperature:    {current.temperature:.01f} \u00b0C
- Humidity:       {current.humidity} %
- Pressure:       {current.pressure:.01f} hPa
- Battery:        {current.battery} %
- Status Display: {current.status.name}
- Age:            {current.ago}/{current.interval}
---------------------------------------
-"""
-
-format_str_2 = """
---------------------------------------
- Connected: {current.name} | {current.version}
- Updated {current.ago} s ago. Intervals: {current.interval} s
- {current.stored} total log_size
- --------------------------------------
- Temperature:    {current.temperature:.01f} \u00b0C
- Humidity:       {current.humidity} %
- Battery:        {current.battery} %
- Status Temp.:   {current.status_t.name}
- Status Humid.:  {current.status_h.name}
- Age:            {current.ago}/{current.interval}
---------------------------------------
-"""
-
 def parse_args(ctl_args):
     parser = argparse.ArgumentParser()
     parser.add_argument("device_mac", nargs='?', help="Aranet4 Bluetooth Address")
     parser.add_argument(
         "--scan", action="store_true", help="Scan Aranet4 devices"
     )
     current = parser.add_argument_group("Options for current reading")
@@ -121,72 +90,68 @@
         char_repeat += 9
     if records.filter.incl_temperature:
         char_repeat += 7
     if records.filter.incl_humidity:
         char_repeat += 6
     if records.filter.incl_pressure:
         char_repeat += 11
+    if records.filter.incl_rad_dose_rate:
+        char_repeat += 11
+    if records.filter.incl_rad_dose:
+        char_repeat += 11
+    if records.filter.incl_rad_dose_total:
+        char_repeat += 12
     print("-" * char_repeat)
     print(f"{'Device Name':<15}: {records.name:>20}")
     print(f"{'Device Version':<15}: {records.version:>20}")
     print("-" * char_repeat)
     print(f"{'id': ^4} | {'date': ^25} |", end=""),
     if records.filter.incl_co2:
         print(f" {'co2':^6} |", end=""),
     if records.filter.incl_temperature:
         print(" temp |", end="")
     if records.filter.incl_humidity:
         print(" humid |", end="")
     if records.filter.incl_pressure:
         print(" pressure |", end="")
+    if records.filter.incl_rad_dose:
+        print(" rad_dose |", end="")
+    if records.filter.incl_rad_dose_rate:
+        print(" rad_rate |", end="")
+    if records.filter.incl_rad_dose_total:
+        print(" rad_total |", end="")
     print("")
     print("-" * char_repeat)
-    filtered_values = records.value
-    for record_id, line in enumerate(filtered_values, start=records.filter.begin):
+
+    for record_id, line in enumerate(records.value, start=records.filter.begin):
         print(f"{record_id:>4d} | {line.date.isoformat()} |", end="")
         if records.filter.incl_co2:
             print(f" {line.co2:>6d} |", end="")
         if records.filter.incl_temperature:
             print(f" {line.temperature:>4.1f} |", end="")
         if records.filter.incl_humidity:
             print(f" {line.humidity:>3.1f} |", end="")
         if records.filter.incl_pressure:
             print(f" {line.pressure:>8.1f} |", end="")
+        if records.filter.incl_rad_dose:
+            print(f" {line.rad_dose/1000:>8.3f} |", end="")
+        if records.filter.incl_rad_dose_rate:
+            print(f" {line.rad_dose_rate/1000:>8.3f} |", end="")
+        if records.filter.incl_rad_dose_total:
+            print(f" {line.rad_dose_total/1000000:>9.4f} |", end="")
         print("")
     print("-" * char_repeat)
 
 
-def print_scan_result(advertisement):
+def store_scan_result(advertisement):
+    global found
     if not advertisement.device:
         return
 
-    print("=======================================")
-    print(f"  Name:     {advertisement.device.name}")
-    print(f"  Address:  {advertisement.device.address}")
-    print(f"  RSSI:     {advertisement.rssi} dBm")
-
-    if advertisement.readings:
-        print("--------------------------------------")
-        if advertisement.readings.co2 >= 0:
-            print(f"  CO2:            {advertisement.readings.co2} pm")
-        print(f"  Temperature:    {advertisement.readings.temperature:.01f} \u00b0C")
-        print(f"  Humidity:       {advertisement.readings.humidity} %")
-        if advertisement.readings.pressure >= 0:
-            print(f"  Pressure:       {advertisement.readings.pressure:.01f} hPa")
-        print(f"  Battery:        {advertisement.readings.battery} %")
-        if advertisement.readings.status >= 0:
-            print(f"  Status Disp.:   {advertisement.readings.status.name}")
-        if advertisement.readings.status_t >= 0 and advertisement.readings.status_h >= 0:
-            print(f"  Status Temp.:   {advertisement.readings.status_t.name}")
-            print(f"  Status Humid.:  {advertisement.readings.status_h.name}")
-        print(f"  Age:            {advertisement.readings.ago}/{advertisement.readings.interval}")
-        print(f"  Counter:        {advertisement.readings.counter}")
-
-    print()
-
+    found[advertisement.device.address] = advertisement
 
 def write_csv(filename, log_data):
     """
     Output `client.Record` dataclass to csv file
     :param filename: file name
     :param log_data: `client.Record` data object
     """
@@ -196,39 +161,36 @@
             fieldnames.append("co2")
         if log_data.filter.incl_temperature:
             fieldnames.append("temperature")
         if log_data.filter.incl_humidity:
             fieldnames.append("humidity")
         if log_data.filter.incl_pressure:
             fieldnames.append("pressure")
+        if log_data.filter.incl_rad_dose:
+            fieldnames.append("rad_dose")
+        if log_data.filter.incl_rad_dose_rate:
+            fieldnames.append("rad_dose_rate")
+        if log_data.filter.incl_rad_dose_total:
+            fieldnames.append("rad_dose_total")
         writer = csv.DictWriter(csvfile, fieldnames=fieldnames, extrasaction="ignore")
 
         writer.writeheader()
 
-        filtered_values = log_data.value[
-            log_data.filter.begin - 1 : log_data.filter.end
-        ]
-        for line in filtered_values:
+        for line in log_data.value:
             writer.writerow(asdict(line))
 
 
 def post_data(url, current):
     # get current measurement minute
     now = datetime.datetime.now(datetime.timezone.utc).replace(microsecond=0)
     delta_ago = datetime.timedelta(seconds=current.ago)
     t = now - delta_ago
     t = t.replace(second=0)  # epoch, floored to minutes
-    data = {
-        "time": t.timestamp(),
-        "co2": current.co2,
-        "temperature": current.temperature,
-        "pressure": current.pressure,
-        "humidity": current.humidity,
-        "battery": current.battery,
-    }
+    data = current.toDict()
+    data["time"] = t.timestamp()
     r = requests.post(
         url,
         data=data,
     )
     print("Pushing data: {:s}".format(r.text))
 
 
@@ -237,20 +199,34 @@
     wait_time = current_vals.interval - current_vals.ago
     for secs in range(wait_time, 0, -1):
         sleep(1)
         print(f"Next data point in {secs}...", end="\r")
 
 
 def main(argv):
+    global found
+    found = {}
     args = parse_args(argv)
 
     if args.scan:
         print("Looking for Aranet devices...")
-        devices = client.find_nearby(print_scan_result)
+        devices = client.find_nearby(store_scan_result)
         print(f"Scan finished. Found {len(devices)}")
+        print()
+        for addr, advertisement in found.items():
+            if advertisement.readings:
+                print(advertisement.readings.toString(advertisement))
+            else:
+                print("=======================================")
+                print(f"  Name:     {advertisement.device.name}")
+                print(f"  Address:  {advertisement.device.address}")
+                print(f"  RSSI:     {advertisement.rssi} dBm")
+                print()
+            print()
+
         return
 
     if not args.device_mac:
         print("Device address not specified")
         return
 
     if args.records:
@@ -258,17 +234,15 @@
             wait_for_new_record(args.device_mac)
         records = client.get_all_records(args.device_mac, vars(args), True)
         print_records(records)
         if args.output:
             write_csv(args.output, records)
     else:
         current = client.get_current_readings(args.device_mac)
-        s = format_str_2 if current.name.startswith("Aranet2") else format_str
-        s = s.format(current=current)
-        print(s)
+        print(current.toString())
         if args.url:
             post_data(args.url, current)
 
 
 def entry_point():
     main(argv=sys.argv[1:])
```

### Comparing `aranet4-2.2.3/aranet4/client.py` & `aranet4-2.3.0/aranet4/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 from dataclasses import dataclass, field
 import datetime
 from enum import IntEnum
 import re
 import struct
+import math
 from typing import List, NamedTuple
 
 from bleak import BleakClient
 from bleak import BleakScanner
 from bleak.backends.device import BLEDevice
 
 
@@ -19,25 +20,34 @@
     """Enums for the different log_size available"""
 
     TEMPERATURE = 1
     HUMIDITY = 2
     PRESSURE = 3
     CO2 = 4
     HUMIDITY2 = 5
-
+    PULSES = 6
+    RADIATION_DOSE = 7
+    RADIATION_DOSE_RATE = 8
+    RADIATION_DOSE_INTEGRAL = 9
 
 class Status(IntEnum):
     """Enum for the different status colors"""
 
     NONE = 0
     GREEN = 1
     AMBER = 2
     RED = 3
     BLUE = 4
 
+class AranetType(IntEnum):
+    """Enum for the different Aranet devices"""
+    ARANET4 = 0
+    ARANET2 = 1
+    ARANET_RADIATION = 2
+    UNKNOWN = 255
 
 @dataclass
 class Aranet4HistoryDelegate:
     """
     When collecting the historical records they are sent using BLE
     notifications. This class takes those notifications and presents them
     as a Python dataclass
@@ -80,60 +90,169 @@
 
 @dataclass
 class CurrentReading:
     """dataclass to store the information when querying the devices current settings"""
 
     name: str = ""
     version: str = ""
+    type: AranetType = AranetType.UNKNOWN
+
+    # Aranet2, Aranet4
     temperature: float = -1
     humidity: float = -1
+
+    # Aranet 4
     pressure: float = -1
     co2: int = -1
+
+    # Aranet Radiation
+    radiation_rate: float = -1
+    radiation_total: float = -1
+    radiation_duration: int = -1
+
     battery: int = -1
     status: int = -1
     status_t: int = -1
     status_h: int = -1
     interval: int = -1
     ago: int = -1
     stored: int = -1
     counter: int = -1
 
-    def decode(self, value: tuple):
-        """Process data from current log_size and process before storing"""
+    def toString(self, advertisement=None):
+        ret = "=======================================\n"
+        ret += f"  Name:     {self.name}\n"
+
+        if advertisement:
+            ret += f"  Address:  {advertisement.device.address}\n"
+            ret += f"  RSSI:     {advertisement.rssi} dBm\n"
+
+        if self.stored > 0:
+            ret += f"  Logs:     {self.stored}\n"
+
+        ret += "---------------------------------------\n"
+
+        if self.type == AranetType.ARANET4:
+            ret += f"  CO2:            {self.co2} ppm\n"
+            ret += f"  Temperature:    {self.temperature:.01f} \u00b0C\n"
+            ret += f"  Humidity:       {self.humidity} %\n"
+            ret += f"  Pressure:       {self.pressure:.01f} hPa\n"
+            ret += f"  Battery:        {self.battery} %\n"
+            ret += f"  Status Display: {self.status.name}\n"
+            ret += f"  Age:            {self.ago}/{self.interval}\n"
+        elif self.type == AranetType.ARANET2:
+            ret += f"  Temperature:    {self.temperature:.01f} \u00b0C\n"
+            ret += f"  Humidity:       {self.humidity} %\n"
+            ret += f"  Battery:        {self.battery} %\n"
+            ret += f"  Status Temp.:   {self.status_t.name}\n"
+            ret += f"  Status Humid.:  {self.status_h.name}\n"
+            ret += f"  Age:            {self.ago}/{self.interval}\n"
+        elif self.type == AranetType.ARANET_RADIATION:
+            m = math.floor(self.radiation_duration / 60 % 60)
+            h = math.floor(self.radiation_duration / 3600 % 24)
+            d = math.floor(self.radiation_duration / 86400)
+
+            dose_duration = str(m) + "m"
+            if h > 0: dose_duration = str(h) + "h " + dose_duration
+            if d > 0: dose_duration = str(d) + "d " + dose_duration
+
+            ret += f"  Dose rate:      {self.radiation_rate/1000:.02f} uSv/h\n"
+            ret += f"  Dose total:     {self.radiation_total/1000000:.04f} mSv/{dose_duration}\n"
+            ret += f"  Battery:        {self.battery} %\n"
+            ret += f"  Age:            {self.ago}/{self.interval}\n"
+        else:
+            ret += f"  Unknown device type\n"
+
+        return ret
+
+    def toDict(self):
+        data = {
+            "battery": self.battery,
+            "type": self.type.name
+        }
+
+        if self.type == AranetType.ARANET2:
+            data["temperature"] = self.temperature
+            data["humidity"] = self.humidity
+        elif self.type == AranetType.ARANET4:
+            data["co2"] = self.co2
+            data["temperature"] = self.temperature
+            data["pressure"] = self.pressure
+            data["humidity"] = self.humidity
+        elif self.type == AranetType.ARANET_RADIATION:
+            data["radiation_rate"] = self.radiation_rate
+            data["radiation_total"] = self.radiation_total
+            data["radiation_duration"] = self.radiation_duration
+
+        return data
+
+    def decode(self, value: tuple, type: AranetType, gatt=False):
+        """Process advertisement or gatt data"""
+
+        self.type = type
+        if type == AranetType.ARANET4:
+            self._decode_aranet4(value, gatt)
+        elif type == AranetType.ARANET2:
+            self._decode_aranet2(value, gatt)
+        elif type == AranetType.ARANET_RADIATION:
+            self._decode_aranetR(value, gatt)
+
+    def _decode_aranet4(self, value: tuple, gatt=False):
+        """Process Aranet4 data - CO2, Temperature, Humidity, Pressure"""
+
         self.co2 = self._set(Param.CO2, value[0])
         self.temperature = self._set(Param.TEMPERATURE, value[1])
         self.pressure = self._set(Param.PRESSURE, value[2])
         self.humidity = self._set(Param.HUMIDITY, value[3])
         self.battery = value[4]
         self.status = Status(value[5])
         # If extended data list
         if len(value) > 6:
             self.interval = value[6]
             self.ago = value[7]
 
-    def decode2(self, value: tuple, gatt=False):
-        """Process data from current log_size and process before storing"""
+    def _decode_aranet2(self, value: tuple, gatt=False):
+        """Process Aranet2 data - Temperature, Humidity"""
 
         # order from gatt and advertisements are different
         if gatt:
             self.temperature = self._set(Param.TEMPERATURE, value[4])
             self.humidity = self._set(Param.HUMIDITY2, value[5])
             self.battery = value[3]
             self.status_h, self.status_t = self._decode_status_flags(value[6])
             self.interval = value[1]
             self.ago = value[2]
         else:
             self.temperature = self._set(Param.TEMPERATURE, value[1])
             self.humidity = self._set(Param.HUMIDITY2, value[3])
-            self.battery = value[5]
             self.status_h, self.status_t = self._decode_status_flags(value[6])
+            self.battery = value[5]
             self.interval = value[7]
             self.ago = value[8]
             self.counter = value[9]
 
+    def _decode_aranetR(self, value: tuple, gatt=False):
+        """Process Aranet Radiation data - radiation dose"""
+        # order from gatt and advertisements are different
+        if gatt:
+            self.radiation_duration = value[6]
+            self.radiation_rate = value[4]
+            self.radiation_total = value[5]
+            self.battery = value[3]
+            self.interval = value[1]
+            self.ago = value[2]
+        else:
+            self.radiation_total = value[0]
+            self.radiation_duration = value[1]
+            self.radiation_rate = value[2]
+            self.battery = value[4]
+            self.interval = value[6]
+            self.ago = value[7]
+            self.counter = value[8]
+
     @staticmethod
     def _decode_status_flags(status):
         status_t = Status.GREEN
         status_h = Status.GREEN
 
         if status & 0b0001:
             status_h = Status.BLUE
@@ -167,14 +286,23 @@
             multiplier = 0.05
         elif param == Param.HUMIDITY:
             invalid_reading_flag = value >> 8
             multiplier = 1
         elif param == Param.HUMIDITY2:
             invalid_reading_flag = value >> 15 == 1
             multiplier = 0.1
+        elif param == Param.RADIATION_DOSE:
+            invalid_reading_flag = value >> 15 == 1
+            multiplier = 1 # nSv
+        elif param == Param.RADIATION_DOSE_RATE:
+            invalid_reading_flag = value >> 15 == 1
+            multiplier = 10 # nSv/h
+        elif param == Param.RADIATION_DOSE_INTEGRAL:
+            invalid_reading_flag = value >> 15 == 1
+            multiplier = 1 # nSv
 
         if invalid_reading_flag:
             return -1
         if isinstance(multiplier, float):
             return round(value * multiplier, 1)
         return value * multiplier
 
@@ -240,67 +368,79 @@
 
         if device and ad_data:
             has_manufacurer_data = Aranet4.MANUFACTURER_ID in ad_data.manufacturer_data
             self.rssi = ad_data.rssi
 
             if has_manufacurer_data:
                 mf_data = ManufacturerData()
-                raw_bytes = ad_data.manufacturer_data[Aranet4.MANUFACTURER_ID]
+                raw_bytes = bytearray(ad_data.manufacturer_data[Aranet4.MANUFACTURER_ID])
 
                 # Basic info
+                if raw_bytes[0] == 33 and raw_bytes[1] != 33:
+                    # For some reason, this is dropped for Aranet4
+                    raw_bytes.insert(0,0)
+
                 value_fmt = "<BBBB"
-                if device.name.startswith("Aranet2"):
-                    value = struct.unpack(value_fmt, raw_bytes[1:5])
-                else:
-                    value = struct.unpack(value_fmt, raw_bytes[0:4])
+                value = struct.unpack(value_fmt, raw_bytes[1:5])
                 mf_data.decode(value)
                 self.manufacturer_data = mf_data
 
-                packing = None
-                if len(raw_bytes) > 7:
-                    packing = raw_bytes[7]
-
                 # Extended info / measurements
-                if packing == 0 and len(raw_bytes) >= 24: # Aranet2
+                aranetv = raw_bytes[0]
+                if len(raw_bytes) < 9:
+                    mf_data.integrations = False
+                elif aranetv == 0: # Aranet4
+                    value_fmt = "<HHHBBBHH"
+                    value = struct.unpack(value_fmt, raw_bytes[9:22])
+                    self.readings = CurrentReading()
+                    self.readings.decode(value, AranetType.ARANET4)
+                    self.readings.name = device.name
+                elif aranetv == 1: # Aranet2
                     value_fmt = "<HHHHBBBHHB"
                     value = struct.unpack(value_fmt, raw_bytes[8:24])
                     self.readings = CurrentReading()
-                    self.readings.decode2(value)
+                    self.readings.decode(value, AranetType.ARANET2)
                     self.readings.name = device.name
-                elif packing == 1 and len(raw_bytes) >= 20: # Aranet4
-                    value_fmt = "<HHHBBBHH"
-                    value = struct.unpack(value_fmt, raw_bytes[8:21])
+                elif aranetv == 2: # Aranet Radiation
+                    value_fmt = "<IIHBBBHHB"
+                    value = struct.unpack(value_fmt, raw_bytes[6:24])
                     self.readings = CurrentReading()
-                    self.readings.decode(value)
+                    self.readings.decode(value, AranetType.ARANET_RADIATION)
                     self.readings.name = device.name
                 else:
                     mf_data.integrations = False
 
 
 @dataclass
 class RecordItem:
     """dataclass to store historical records"""
 
     date: datetime
     temperature: float
     humidity: int
     pressure: float
     co2: int
+    rad_dose: float
+    rad_dose_rate: float
+    rad_dose_total: float
 
 
 @dataclass
 class Filter:
     """dataclass to store log filter information"""
 
     begin: int
     end: int
     incl_temperature: bool
     incl_humidity: int
     incl_pressure: bool
     incl_co2: bool
+    incl_rad_dose: bool
+    incl_rad_dose_rate: bool
+    incl_rad_dose_total: bool
 
 
 @dataclass
 class Record:
     name: str
     version: str
     records_on_device: int
@@ -386,32 +526,39 @@
 
         aranet2_char = self.device.services.get_characteristic(
             self.AR2_READ_CURRENT_READINGS
         )
 
         if aranet2_char:
             uuid = self.AR2_READ_CURRENT_READINGS
-            # co2, temp, pressure, humidity, battery, status
-            value_fmt = "<HHHBHHB"
             raw_bytes = await self.device.read_gatt_char(uuid)
-            value = struct.unpack(value_fmt, raw_bytes)
-            readings.decode2(value, True)
+
+            # TODO: Can we use byte ar position 0 to detect type?
+            if len(raw_bytes) >= 28:
+                # radiation
+                value_fmt = "<HHHBIQQB"
+                value = struct.unpack(value_fmt, raw_bytes[0:28])
+                readings.decode(value, AranetType.ARANET_RADIATION, True)
+            else:
+                value_fmt = "<HHHBHHB"
+                value = struct.unpack(value_fmt, raw_bytes)
+                readings.decode(value, AranetType.ARANET2, True)
         else:
             if details:
                 uuid = self.AR4_READ_CURRENT_READINGS_DET
                 # co2, temp, pressure, humidity, battery, status
                 value_fmt = "<HHHBBBHH"
             else:
                 uuid = self.AR4_READ_CURRENT_READINGS
                 # co2, temp, pressure, humidity, battery, status, interval, ^
                 value_fmt = "<HHHBBB"
 
             raw_bytes = await self.device.read_gatt_char(uuid)
             value = struct.unpack(value_fmt, raw_bytes)
-            readings.decode(value)
+            readings.decode(value, AranetType.ARANET4)
         return readings
 
     async def get_interval(self) -> int:
         """Get the value for how often datapoints are logged on device"""
         raw_bytes = await self.device.read_gatt_char(self.AR4_READ_INTERVAL)
         return int.from_bytes(raw_bytes, byteorder="little")
 
@@ -496,22 +643,37 @@
         reading = True
         while reading:
             packet = await self.device.read_gatt_char(
                 self.AR4_READ_HISTORY_READINGS_V2
             )
 
             header = HistoryHeader(*struct.unpack("<BHHHHB", packet[:10]))
+            packet = packet[10:]
 
             if header.param != param.value or header.count == 0:
                 await asyncio.sleep(0.1)
                 continue
 
-            pattern = "<B" if param.value == Param.HUMIDITY else "<H"
+            if param.value == Param.HUMIDITY:
+                pattern = "<B"
+            elif param.value == Param.RADIATION_DOSE:
+                pattern = "<Hx"
+            elif param.value == Param.RADIATION_DOSE_RATE:
+                pattern = "<Hx"
+            elif param.value == Param.RADIATION_DOSE_INTEGRAL:
+                pattern = "<Q"
+            else:
+                pattern = "<H"
+
+            # trim to multiples of pattern size
+            plen = len(packet)
+            packet = packet[:plen - plen % struct.calcsize(pattern)]
 
-            data_values = struct.iter_unpack(pattern, packet[10:])
+            # extract values
+            data_values = struct.iter_unpack(pattern, packet)
             for idx, value in enumerate(data_values, header.start - 1):
                 if idx > end or idx == header.start - 1 + header.count:
                     break
                 result[idx] = CurrentReading._set(param, value[0])
 
             if idx >= end or (header.start - 1 + header.count) == log_size:
                 reading = False
@@ -647,17 +809,15 @@
 
 
 class Aranet4Scanner:
     """Aranet4 Scanner class - scan advertisements and process data, if available"""
 
     def _process_advertisement(self, device, ad_data):
         """Processes Aranet4 advertisement data"""
-
         adv = Aranet4Advertisement(device, ad_data)
-
         self.on_scan(adv)
 
     def __init__(self, on_scan):
         uuids = [Aranet4.AR4_SERVICE, Aranet4.AR4_OLD_SERVICE]
         self.on_scan = on_scan
         self.scanner = BleakScanner(
             detection_callback=self._process_advertisement,
@@ -673,15 +833,15 @@
 async def _find_nearby(detect_callback: callable, duration: int) -> List[BLEDevice]:
     scanner = Aranet4Scanner(detect_callback)
     await scanner.start()
     await asyncio.sleep(duration)
     await scanner.stop()
     return [device
             for device in scanner.scanner.discovered_devices
-            if "Aranet4" in device.name or "Aranet2" in device.name]
+            if "Aranet" in device.name]
 
 
 def find_nearby(detect_callback: callable, duration: int = 5) -> List[BLEDevice]:
     """
     Scans for nearby Aranet4 devices.
     Will call callback on every valid Aranet4 advertisement, including duplcates
     """
@@ -721,25 +881,36 @@
         now = datetime.datetime.now(datetime.timezone.utc).replace(microsecond=0)
 
     if dev_name.startswith("Aranet2"):
         entry_filter["pres"] = False
         entry_filter["co2"] = False
         if entry_filter.get("humi", False):
             entry_filter["humi"] = 2 #v2 humidity
+    elif dev_name.startswith("Aranet\u2622"):
+        entry_filter["pres"] = False
+        entry_filter["co2"] = False
+        entry_filter["humi"] = False
+        entry_filter["temp"] = False
+        entry_filter["rad_dose"] = entry_filter.get("rad_dose", True)
+        entry_filter["rad_dose_rate"] = entry_filter.get("rad_dose_rate", True)
+        entry_filter["rad_dose_total"] = entry_filter.get("rad_dose_total", True)
 
     log_size = await monitor.get_total_readings()
     log_points = _log_times(now, log_size, interval, last_log)
     begin, end = _calc_start_end(log_points, entry_filter)
     rec_filter = Filter(
         begin,
         end,
         entry_filter.get("temp", True),
         entry_filter.get("humi", True),
         entry_filter.get("pres", True),
         entry_filter.get("co2", True),
+        entry_filter.get("rad_dose", False),
+        entry_filter.get("rad_dose_rate", False),
+        entry_filter.get("rad_dose_total", False),
     )
 
     if begin < 0 or end < 0:
         # invalid range. Most likely no points available
         return  Record(dev_name, dev_version, log_size, rec_filter)
 
     # Read datapoint history from device
@@ -767,19 +938,38 @@
         pressure_val = _empty_reading(log_size)
     if rec_filter.incl_co2:
         co2_val = await monitor.get_records(
             Param.CO2, log_size=log_size, start=begin, end=end
         )
     else:
         co2_val = _empty_reading(log_size)
+    if rec_filter.incl_rad_dose:
+        rad_dose_val = await monitor.get_records(
+            Param.RADIATION_DOSE, log_size=log_size, start=begin, end=end
+        )
+    else:
+        rad_dose_val = _empty_reading(log_size)
+    if rec_filter.incl_rad_dose_rate:
+        rad_dose_rate_val = await monitor.get_records(
+            Param.RADIATION_DOSE_RATE, log_size=log_size, start=begin, end=end
+        )
+    else:
+        rad_dose_total_val = _empty_reading(log_size)
+    if rec_filter.incl_rad_dose_total:
+        rad_dose_total_val = await monitor.get_records(
+            Param.RADIATION_DOSE_INTEGRAL, log_size=log_size, start=begin, end=end
+        )
+    else:
+        rad_dose_total_val = _empty_reading(log_size)
+####
     # Store returned data in dataclass
-    data = zip(log_points, co2_val, temperature_val, pressure_val, humidity_val)
+    data = zip(log_points, co2_val, temperature_val, pressure_val, humidity_val, rad_dose_val, rad_dose_rate_val, rad_dose_total_val)
     record = Record(dev_name, dev_version, log_size, rec_filter)
-    for date, co2, temp, pres, hum in data:
-        record.value.append(RecordItem(date, temp, hum, pres, co2))
+    for date, co2, temp, pres, hum, rad, rad_rate, rad_integral in data:
+        record.value.append(RecordItem(date, temp, hum, pres, co2, rad, rad_rate, rad_integral))
     if (remove_empty):
         record.value = record.value[begin-1:end+1]
     return record
 
 
 def get_all_records(mac_address: str, entry_filter: dict, remove_empty: bool = False) -> Record:
     """
```

### Comparing `aranet4-2.2.3/aranet4.egg-info/PKG-INFO` & `aranet4-2.3.0/aranet4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.2.3
+Version: 2.3.0
 Summary: Aranet4 and Aranet2 Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aranet4-2.2.3/setup.py` & `aranet4-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aranet4",
-    version="2.2.3",
+    version="2.3.0",
     description="Aranet4 and Aranet2 Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/Aranet4-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

