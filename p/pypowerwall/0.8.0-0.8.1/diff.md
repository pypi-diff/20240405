# Comparing `tmp/pypowerwall-0.8.0-py2.py3-none-any.whl.zip` & `tmp/pypowerwall-0.8.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,23 @@
-Zip file size: 56565 bytes, number of entries: 19
--rw-r--r--  2.0 unx    25490 b- defN 24-Mar-26 02:39 pypowerwall/__init__.py
--rw-r--r--  2.0 unx     2436 b- defN 24-Mar-26 02:39 pypowerwall/__main__.py
--rw-r--r--  2.0 unx     2217 b- defN 24-Mar-26 02:39 pypowerwall/pypowerwall_base.py
+Zip file size: 61969 bytes, number of entries: 21
+-rw-r--r--  2.0 unx    32574 b- defN 24-Apr-03 02:48 pypowerwall/__init__.py
+-rw-r--r--  2.0 unx     5835 b- defN 24-Mar-31 06:45 pypowerwall/__main__.py
+-rw-r--r--  2.0 unx     1889 b- defN 24-Mar-30 06:29 pypowerwall/aux.py
+-rw-r--r--  2.0 unx      133 b- defN 24-Mar-30 06:29 pypowerwall/exceptions.py
+-rw-r--r--  2.0 unx     2897 b- defN 24-Apr-04 04:31 pypowerwall/pypowerwall_base.py
 -rw-r--r--  2.0 unx     6718 b- defN 24-Mar-26 02:39 pypowerwall/scan.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:39 pypowerwall/cloud/__init__.py
 -rw-r--r--  2.0 unx      638 b- defN 24-Mar-26 02:39 pypowerwall/cloud/decorators.py
--rw-r--r--  2.0 unx      182 b- defN 24-Mar-26 02:39 pypowerwall/cloud/exceptions.py
+-rw-r--r--  2.0 unx      242 b- defN 24-Mar-30 06:29 pypowerwall/cloud/exceptions.py
 -rw-r--r--  2.0 unx    18733 b- defN 24-Mar-26 02:39 pypowerwall/cloud/mock_data.py
--rw-r--r--  2.0 unx    41244 b- defN 24-Mar-26 02:39 pypowerwall/cloud/pypowerwall_cloud.py
+-rw-r--r--  2.0 unx    46292 b- defN 24-Apr-05 03:05 pypowerwall/cloud/pypowerwall_cloud.py
 -rw-r--r--  2.0 unx     4355 b- defN 24-Mar-26 02:39 pypowerwall/cloud/stubs.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:39 pypowerwall/local/__init__.py
 -rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 02:39 pypowerwall/local/exceptions.py
--rw-r--r--  2.0 unx    15816 b- defN 24-Mar-26 02:39 pypowerwall/local/pypowerwall_local.py
+-rw-r--r--  2.0 unx    20130 b- defN 24-Apr-05 03:05 pypowerwall/local/pypowerwall_local.py
 -rw-r--r--  2.0 unx    71273 b- defN 24-Mar-26 02:39 pypowerwall/local/tesla_pb2.py
--rw-r--r--  2.0 unx     1066 b- defN 24-Mar-26 02:57 pypowerwall-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    39811 b- defN 24-Mar-26 02:57 pypowerwall-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Mar-26 02:57 pypowerwall-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Mar-26 02:57 pypowerwall-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1610 b- defN 24-Mar-26 02:57 pypowerwall-0.8.0.dist-info/RECORD
-19 files, 231803 bytes uncompressed, 53923 bytes compressed:  76.7%
+-rw-r--r--  2.0 unx     1066 b- defN 24-Apr-05 04:09 pypowerwall-0.8.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    41728 b- defN 24-Apr-05 04:09 pypowerwall-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-05 04:09 pypowerwall-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-05 04:09 pypowerwall-0.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1766 b- defN 24-Apr-05 04:09 pypowerwall-0.8.1.dist-info/RECORD
+21 files, 256483 bytes uncompressed, 59089 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
 Filename: pypowerwall/__init__.py
 Comment: 
 
 Filename: pypowerwall/__main__.py
 Comment: 
 
+Filename: pypowerwall/aux.py
+Comment: 
+
+Filename: pypowerwall/exceptions.py
+Comment: 
+
 Filename: pypowerwall/pypowerwall_base.py
 Comment: 
 
 Filename: pypowerwall/scan.py
 Comment: 
 
 Filename: pypowerwall/cloud/__init__.py
@@ -36,23 +42,23 @@
 
 Filename: pypowerwall/local/pypowerwall_local.py
 Comment: 
 
 Filename: pypowerwall/local/tesla_pb2.py
 Comment: 
 
-Filename: pypowerwall-0.8.0.dist-info/LICENSE
+Filename: pypowerwall-0.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: pypowerwall-0.8.0.dist-info/METADATA
+Filename: pypowerwall-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: pypowerwall-0.8.0.dist-info/WHEEL
+Filename: pypowerwall-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: pypowerwall-0.8.0.dist-info/top_level.txt
+Filename: pypowerwall-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pypowerwall-0.8.0.dist-info/RECORD
+Filename: pypowerwall-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pypowerwall/__init__.py

```diff
@@ -32,14 +32,15 @@
     siteid = None             # If cloudmode is True, use this siteid (default is None)
     authpath = ""             # Path to cloud auth and site files (default current directory)
     authmode = "cookie"       # "cookie" (default) or "token" - use cookie or bearer token for auth
     cachefile = ".powerwall"  # Path to cache file (default current directory)
     
  Functions 
     poll(api, json, force)    # Return data from Powerwall api (dict if json=True, bypass cache force=True)
+    post(api, payload, json)  # Send payload to Powerwall api (dict if json=True)
     level()                   # Return battery power level percentage
     power()                   # Return power data returned as dictionary
     site(verbose)             # Return site sensor data (W or raw JSON if verbose=True)
     solar(verbose):           # Return solar sensor data (W or raw JSON if verbose=True)
     battery(verbose):         # Return battery sensor data (W or raw JSON if verbose=True)
     load(verbose)             # Return load sensor data (W or raw JSON if verbose=True)
     grid()                    # Alias for site()
@@ -56,36 +57,44 @@
     system_status(json)       # Returns the system status
     battery_blocks(json)      # Returns battery specific information merged from system_status() and vitals()
     grid_status(type)         # Return the power grid status, type ="string" (default), "json", or "numeric"
                               #     - "string": "UP", "DOWN", "SYNCING"
                               #     - "numeric": -1 (Syncing), 0 (DOWN), 1 (UP)
     is_connected()            # Returns True if able to connect and login to Powerwall
     get_reserve(scale)        # Get Battery Reserve Percentage
+    get_mode()                # Get Current Battery Operation Mode
+    set_reserve(level)        # Set Battery Reserve Percentage
+    set_mode(mode)            # Set Current Battery Operation Mode
     get_time_remaining()      # Get the backup time remaining on the battery
 
+    set_operation(level, mode, json)        # Set Battery Reserve Percentage and/or Operation Mode
+
  Requirements
     This module requires the following modules: requests, protobuf, teslapy
     pip install requests protobuf teslapy
 """
 import json
 import logging
 import os.path
 import sys
+from json import JSONDecodeError
 from typing import Union, Optional
 
 # noinspection PyPackageRequirements
 import urllib3
 
+from pypowerwall.aux import HOST_REGEX, IPV4_6_REGEX, EMAIL_REGEX
+from pypowerwall.exceptions import PyPowerwallInvalidConfigurationParameter, InvalidBatteryReserveLevelException
 from pypowerwall.cloud.pypowerwall_cloud import PyPowerwallCloud
 from pypowerwall.local.pypowerwall_local import PyPowerwallLocal
 from pypowerwall.pypowerwall_base import parse_version, PyPowerwallBase
 
 urllib3.disable_warnings()  # Disable SSL warnings
 
-version_tuple = (0, 8, 0)
+version_tuple = (0, 8, 1)
 version = __version__ = '%d.%d.%d' % version_tuple
 __author__ = 'jasonacox'
 
 log = logging.getLogger(__name__)
 log.debug('%s version %s', __name__, __version__)
 log.debug('Python %s on %s', sys.version, sys.platform)
 
@@ -142,21 +151,27 @@
         self.cloudmode = cloudmode  # cloud mode or local mode (default)
         self.siteid = siteid  # siteid for cloud mode
         self.authpath = os.path.expanduser(authpath)  # path to auth and site cache files
         self.authmode = authmode  # cookie or token
         self.pwcooldown = 0  # rate limit cooldown time - pause api calls
         self.vitals_api = True  # vitals api is available for local mode
         self.client: PyPowerwallBase
-        # Check for cloud mode
-        if self.cloudmode or self.host == "":
+
+        # Make certain assumptions here
+        if not self.host:
             self.cloudmode = True
+
+        # Validate provided parameters
+        self._validate_init_configuration()
+
+        # Check for cloud mode
+        if self.cloudmode:
             self.client = PyPowerwallCloud(self.email, self.pwcacheexpire, self.timeout, self.siteid, self.authpath)
             # Check to see if we can connect to the cloud
         else:
-            self.cloudmode = False
             self.client = PyPowerwallLocal(self.host, self.password, self.email, self.timezone, self.timeout,
                                            self.pwcacheexpire, self.poolmaxsize, self.authmode, self.cachefile)
 
         self.client.authenticate()
 
     def is_connected(self):
         """
@@ -169,32 +184,55 @@
             if self.status() is None:
                 return False
             return True
         except Exception:
             return False
 
     def poll(self, api='/api/site_info/site_name', jsonformat=False, raw=False, recursive=False,
-             force=False) -> Union[dict, str]:
+             force=False) -> Optional[Union[dict, list, str, bytes]]:
         """
         Query Tesla Energy Gateway Powerwall for API Response
         
         Args:
             api         = URI 
             jsonformat  = If True, return JSON format otherwise return Python Dictionary
             raw         = If True, send raw data back (useful for binary responses, has no meaning in Cloud mode)
             recursive   = If True, this is a recursive call and do not allow additional recursive calls
             force       = If True, bypass the cache and make the API call to the gateway, has no meaning in Cloud mode
         """
-        # Check to see if we are in cloud mode
         payload = self.client.poll(api, force, recursive, raw)
         if jsonformat:
-            return json.dumps(payload)
+            try:
+                return json.dumps(payload)
+            except JSONDecodeError:
+                log.error(f"Unable to dump response '{payload}' as JSON. I know you asked for it, sorry.")
         else:
             return payload
 
+    def post(self, api: str, payload: Optional[dict], din: Optional[str] = None, jsonformat=False, raw=False,
+             recursive=False) -> Optional[Union[dict, list, str, bytes]]:
+        """
+        Send a command to Tesla Energy Gateway
+
+        Args:
+            api         = URI
+            payload     = Arbitrary payload to send
+            din         = System DIN (ignored in Cloud mode)
+            raw         = If True, send raw data back (useful for binary responses, has no meaning in Cloud mode)
+            recursive   = If True, this is a recursive call and do not allow additional recursive calls
+        """
+        response = self.client.post(api, payload, din, recursive, raw)
+        if jsonformat:
+            try:
+                return json.dumps(response)
+            except JSONDecodeError:
+                log.error(f"Unable to dump response '{response}' as JSON. I know you asked for it, sorry.")
+        else:
+            return response
+
     def level(self, scale=False):
         """ 
         Battery Level Percentage 
             Note: Tesla App reserves 5% of battery => ( (batterylevel / 0.95) - (5 / 0.95) )
         Args:
             scale = If True, convert battery level to app scale value
         """
@@ -449,36 +487,110 @@
                 if value is True:
                     alerts.append(alert)
             pvs_alerts = data.get('pvs_alerts') or {}
             for alert, value in pvs_alerts.items():
                 if value is True:
                     alerts.append(alert)
 
+        # Augment with inferred alerts from the grid_status
+        grid_status = self.poll('/api/system_status/grid_status')
+        if grid_status:
+            alert = grid_status.get('grid_status')
+            if alert == 'SystemGridConnected' and 'SystemConnectedToGrid' not in alerts:
+                alerts.append('SystemConnectedToGrid')
+            else:
+                alerts.append(alert)
+            if grid_status.get('grid_services_active'):
+                alerts.append('GridServicesActive')
+
         if jsonformat:
             return json.dumps(alerts, indent=4, sort_keys=True)
         else:
             return alerts
 
-    def get_reserve(self, scale=True) -> Optional[float]:
+    def get_reserve(self, scale=True, force=False) -> Optional[float]:
         """
         Get Battery Reserve Percentage  
         Tesla App reserves 5% of battery => ( (batterylevel / 0.95) - (5 / 0.95) )
 
         Args:
             scale    = If True (default) use Tesla's 5% reserve calculation
         """
-        data = self.poll('/api/operation')
+        data = self.poll('/api/operation', force=force)
         if data is not None and 'backup_reserve_percent' in data:
             percent = float(data['backup_reserve_percent'])
             if scale:
                 # Get percentage based on Tesla App scale
                 percent = float((percent / 0.95) - (5 / 0.95))
             return percent
         return None
 
+    def get_mode(self, force=False) -> Optional[float]:
+        """
+        Get Battery Operation Mode
+        """
+        data = self.poll('/api/operation', force=force)
+        if data and data.get('real_mode'):
+            return data['real_mode']
+        return None
+
+    def set_reserve(self, level: float) -> Optional[dict]:
+        """
+        Set battery reserve level.
+
+        Args:
+            level:   Set battery reserve level in percents (range of 5-100 is accepted)
+
+        Returns:
+            Dictionary with operation results.
+        """
+        return self.set_operation(level=level)
+
+    def set_mode(self, mode: str) -> Optional[dict]:
+        """
+        Set battery operation mode.
+
+        Args:
+            mode:    Set battery operation mode (self_consumption, backup, autonomous, etc.)
+
+        Returns:
+            Dictionary with operation results.
+        """
+        return self.set_operation(mode=mode)
+
+    def set_operation(self, level: Optional[float] = None, mode: Optional[str] = None,
+                      jsonformat: bool = False) -> Optional[Union[dict, str]]:
+        """
+        Set battery operation mode and reserve level.
+
+        Args:
+            level:   Set battery reserve level in percents (range of 5-100 is accepted)
+            mode:    Set battery operation mode (self_consumption, backup, autonomous, etc.)
+            jsonformat:  Set to True to receive json formatted string
+
+        Returns:
+            Dictionary with operation results, if jsonformat is False, else a JSON string
+        """
+        if level and (level < 5 or level > 100):
+            raise InvalidBatteryReserveLevelException('Level can be in range of 5 to 100 only.')
+
+        if not level:
+            level = self.get_reserve()
+
+        if not mode:
+            mode = self.get_mode()
+
+        payload = {
+            'backup_reserve_percent': level,
+            'real_mode': mode
+        }
+
+        result = self.post(api='/api/operation', payload=payload, din=self.din(), jsonformat=jsonformat)
+        return result
+
     # noinspection PyShadowingBuiltins
     def grid_status(self, type="string") -> Optional[Union[str, int]]:
         """
         Get the status of the grid  
         
         Args:
             type == "string" (default) returns: "UP", "DOWN", "SYNCING"
@@ -602,7 +714,58 @@
         """
         Get the backup time remaining on the battery
 
         Returns:
             The time remaining in hours
         """
         return self.client.get_time_remaining()
+
+    def _validate_init_configuration(self):
+
+        # Basic user input validation for starters. Can be expanded to limit other parameters such as cache
+        # expiration range, timeout range, etc
+
+        # Check for valid hostname/IP address
+        if (self.host and (
+                not isinstance(self.host, str) or
+                (not IPV4_6_REGEX.match(self.host) and not HOST_REGEX.match(self.host))
+        )):
+            raise PyPowerwallInvalidConfigurationParameter(f"Invalid powerwall host: '{self.host}'. Must be in the "
+                                                           f"form of IP address or a valid form of a hostname or FQDN.")
+
+        # If cloud mode requested, check appropriate parameters
+        if self.cloudmode:
+            # Ensure email is set and syntactically correct
+            if not self.email or not isinstance(self.email, str) or not EMAIL_REGEX.match(self.email):
+                raise PyPowerwallInvalidConfigurationParameter(f"A valid email address is required to run in "
+                                                               f"cloud mode: '{self.email}' did not pass validation.")
+
+            # Ensure we can write to the provided authpath
+            dirname = self.authpath
+            if not dirname:
+                log.debug("No authpath provided, using current directory.")
+                dirname = '.'
+            self._check_if_dir_is_writable(dirname, "authpath")
+        # If local mode, check appropriate parameters, too
+        else:
+            # Ensure we can create a cachefile
+            dirname = os.path.dirname(self.cachefile)
+            if not dirname:
+                log.debug("No cachefile provided, using current directory.")
+                dirname = '.'
+            self._check_if_dir_is_writable(dirname, "cachefile")
+
+    @staticmethod
+    def _check_if_dir_is_writable(dirpath, name=""):
+        # Ensure we can write to the provided authpath
+        if not os.path.exists(dirpath):
+            try:
+                os.makedirs(dirpath, exist_ok=True)
+            except Exception as exc:
+                raise PyPowerwallInvalidConfigurationParameter(f"Unable to create {name} directory at "
+                                                               f"'{dirpath}': {exc}")
+        elif not os.path.isdir(dirpath):
+            raise PyPowerwallInvalidConfigurationParameter(f"'{dirpath}' must be a directory ({name}).")
+        else:
+            if not os.access(dirpath, os.W_OK):
+                raise PyPowerwallInvalidConfigurationParameter(f"Directory '{dirpath}' is not writable for {name}. "
+                                                               f"Check permissions.")
```

## pypowerwall/__main__.py

```diff
@@ -10,14 +10,15 @@
     python -m pypowerwall <scan>
 
 """
 
 import argparse
 import os
 import sys
+import json
 
 # Modules
 from pypowerwall import version
 
 # Global Variables
 AUTHFILE = ".pypowerwall.auth"
 authpath = os.getenv("PW_AUTH_PATH", "")
@@ -42,14 +43,28 @@
                        help=f"Seconds to wait per host [Default={timeout:.1f}]")
 scan_args.add_argument("-nocolor", action="store_true", default=not color,
                        help="Disable color text output.")
 scan_args.add_argument("-ip", type=str, default=ip, help="IP address within network to scan.")
 scan_args.add_argument("-hosts", type=int, default=hosts,
                        help=f"Number of hosts to scan simultaneously [Default={hosts}]")
 
+set_mode_args = subparsers.add_parser("set", help='Set Powerwall Mode and Reserve Level')
+set_mode_args.add_argument("-mode", type=str, default=None,
+                            help="Powerwall Mode: self_consumption, backup, or autonomous")
+set_mode_args.add_argument("-reserve", type=int, default=None,
+                            help="Set Battery Reserve Level [Default=20]")
+set_mode_args.add_argument("-current", action="store_true", default=False,
+                            help="Set Battery Reserve Level to Current Charge")
+
+get_mode_args = subparsers.add_parser("get", help='Get Powerwall Settings and Power Levels')
+get_mode_args.add_argument("-format", type=str, default="text",
+                            help="Output format: text, json, csv")
+
+version_args = subparsers.add_parser("version", help='Print version information')
+
 if len(sys.argv) == 1:
     p.print_help(sys.stderr)
     sys.exit(1)
 
 # parse args
 args = p.parse_args()
 command = args.command
@@ -73,10 +88,79 @@
 
     print("pyPowerwall [%s] - Scanner\n" % version)
     color = not args.nocolor
     ip = args.ip
     hosts = args.hosts
     timeout = args.timeout
     scan.scan(color, timeout, hosts, ip)
+# Set Powerwall Mode
+elif command == 'set':
+    import pypowerwall
+    print("pyPowerwall [%s] - Set Powerwall Mode and Power Levels\n" % version)
+    # Load email from auth file
+    auth_file = authpath + AUTHFILE
+    if not os.path.exists(auth_file):
+        print("ERROR: Auth file %s not found. Run 'setup' to create." % auth_file)
+        exit(1)
+    with open(auth_file, 'r') as file:
+        auth = json.load(file)
+    email = list(auth.keys())[0]
+    pw = pypowerwall.Powerwall(email=email, host="", authpath=authpath)
+    if args.mode:
+        mode = args.mode.lower()
+        if mode not in ['self_consumption', 'backup', 'autonomous']:
+            print("ERROR: Invalid Mode [%s] - must be one of self_consumption, backup, or autonomous" % mode)
+            exit(1)
+        print("Setting Powerwall Mode to %s" % mode)
+        pw.set_mode(mode)
+    if args.reserve:
+        reserve = args.reserve
+        print("Setting Powerwall Reserve to %s" % reserve)
+        pw.set_reserve(reserve)
+    if args.current:
+        current = float(pw.level())
+        print("Setting Powerwall Reserve to Current Charge Level %s" % current)
+        pw.set_reserve(current)
+# Get Powerwall Mode
+elif command == 'get':
+    import pypowerwall
+    # Load email from auth file
+    auth_file = authpath + AUTHFILE
+    if not os.path.exists(auth_file):
+        print("ERROR: Auth file %s not found. Run 'setup' to create." % auth_file)
+        exit(1)
+    with open(auth_file, 'r') as file:
+        auth = json.load(file)
+    email = list(auth.keys())[0]
+    pw = pypowerwall.Powerwall(email=email, host="", authpath=authpath)
+    output = {
+        'site': pw.site_name(),
+        'din': pw.din(),
+        'mode': pw.get_mode(),
+        'reserve': pw.get_reserve(),
+        'current': pw.level(),
+        'grid': pw.grid(),
+        'home': pw.home(),
+        'battery': pw.battery(),
+        'solar': pw.solar(),
+    }
+    if args.format == 'json':
+        print(json.dumps(output, indent=2))
+    elif args.format == 'csv':
+        # create a csv header from keys
+        header = ",".join(output.keys())
+        print(header)
+        values = ",".join(str(value) for value in output.values())
+        print(values)
+    else:
+        print("pyPowerwall [%s] - Set Powerwall Mode and Power Levels\n" % version)
+        # Table Output
+        for item in output:
+            name = item.replace("_", " ").title()
+            print("  {:<15}{}".format(name, output[item]))
+
+# Print Version
+elif command == 'version':
+    print("pyPowerwall [%s]" % version)
 # Print Usage
 else:
     p.print_help()
```

## pypowerwall/pypowerwall_base.py

```diff
@@ -1,13 +1,18 @@
 import abc
 import logging
 from typing import Optional, Any, Union
 
 log = logging.getLogger(__name__)
 
+# Define which write API calls should invalidate which read API cache keys
+WRITE_OP_READ_OP_CACHE_MAP = {
+    '/api/operation': ['/api/operation', 'SITE_CONFIG']  # local and cloud mode respectively
+}
+
 
 def parse_version(version: str) -> Optional[int]:
     if version is None or not isinstance(version, str):
         return None
 
     val = version.split(" ")[0]
     val = ''.join(i for i in val if i.isdigit() or i in './\\')
@@ -19,14 +24,15 @@
     return vint
 
 
 class PyPowerwallBase:
 
     def __init__(self, email: str):
         super().__init__()
+        self.pwcache = {}  # holds the cached data for api
         self.auth = None
         self.token = None  # caches bearer token
         self.email = email
 
     @abc.abstractmethod
     def authenticate(self):
         raise NotImplementedError
@@ -37,14 +43,19 @@
 
     @abc.abstractmethod
     def poll(self, api: str, force: bool = False,
              recursive: bool = False, raw: bool = False) -> Optional[Union[dict, list, str, bytes]]:
         raise NotImplementedError
 
     @abc.abstractmethod
+    def post(self, api: str, payload: Optional[dict], din: Optional[str],
+             recursive: bool = False, raw: bool = False) -> Optional[Union[dict, list, str, bytes]]:
+        raise NotImplementedError
+
+    @abc.abstractmethod
     def vitals(self) -> Optional[dict]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_time_remaining(self) -> Optional[float]:
         raise NotImplementedError
 
@@ -66,7 +77,12 @@
             site = payload['site']['instant_power']
             solar = payload['solar']['instant_power']
             battery = payload['battery']['instant_power']
             load = payload['load']['instant_power']
         except Exception as e:
             log.debug(f"ERROR unable to parse payload '{payload}': {e}")
         return {'site': site, 'solar': solar, 'battery': battery, 'load': load}
+
+    def _invalidate_cache(self, api: str):
+        cache_keys = WRITE_OP_READ_OP_CACHE_MAP.get(api, [])
+        for cache_key in cache_keys:
+            self.pwcache[cache_key] = None
```

## pypowerwall/cloud/exceptions.py

```diff
@@ -4,7 +4,11 @@
 
 class PyPowerwallCloudTeslaNotConnected(Exception):
     pass
 
 
 class PyPowerwallCloudNotImplemented(Exception):
     pass
+
+
+class PyPowerwallCloudInvalidPayload(Exception):
+    pass
```

## pypowerwall/cloud/pypowerwall_cloud.py

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import os
 import time
-from typing import Optional, Union
+from typing import Optional, Union, List
 
-from teslapy import Tesla
+from teslapy import Tesla, Battery, SolarPanel
 
 from pypowerwall.cloud.decorators import not_implemented_mock_data
 from pypowerwall.cloud.exceptions import *
 from pypowerwall.cloud.mock_data import *
 from pypowerwall.cloud.stubs import *
 from pypowerwall.pypowerwall_base import PyPowerwallBase
 
@@ -51,38 +51,43 @@
     def __init__(self, email: Optional[str], pwcacheexpire: int = 5, timeout: int = 5, siteid: Optional[int] = None,
                  authpath: str = ""):
         super().__init__(email)
         self.site = None
         self.tesla = None
         self.apilock = {}  # holds lock flag for pending cloud api requests
         self.pwcachetime = {}  # holds the cached data timestamps for api
-        self.pwcache = {}  # holds the cached data for api
         self.pwcacheexpire = pwcacheexpire  # seconds to expire cache
         self.siteindex = 0  # site index to use
         self.siteid = siteid  # site id to use
         self.counter = 0  # counter for SITE_DATA API
         self.authpath = os.path.expanduser(authpath)  # path to cloud auth and site files
         self.timeout = timeout
         self.authfile = os.path.join(self.authpath, AUTHFILE)
         self.sitefile = os.path.join(self.authpath, SITEFILE)
         self.poll_api_map = self.init_poll_api_map()
+        self.post_api_map = self.init_post_api_map()
 
         if self.siteid is None:
             # Check for site file
             if os.path.exists(self.sitefile):
                 with open(self.sitefile) as file:
                     try:
                         self.siteid = int(file.read())
                     except Exception as exc:
                         log.debug(f"Unable to determine siteid from sitefile, using ID '0' instead: {exc}")
                         self.siteid = 0
             else:
                 self.siteindex = 0
         log.debug(f" -- cloud: Using site {self.siteid} for {self.email}")
 
+    def init_post_api_map(self) -> dict:
+        return {
+            "/api/operation": self.post_api_operation,
+        }
+
     def init_poll_api_map(self) -> dict:
         # API map for local to cloud call conversion
         return {
             # Somewhat Real Actions
             "/api/devices/vitals": self.get_api_devices_vitals,
             "/api/meters/aggregates": self.get_api_meters_aggregates,
             "/api/operation": self.get_api_operation,
@@ -185,21 +190,52 @@
         if self.tesla is None:
             raise PyPowerwallCloudTeslaNotConnected
         # API Map - Determine what data we need based on Powerwall APIs
         log.debug(f" -- cloud: Request for {api}")
 
         func = self.poll_api_map.get(api)
         if func:
-            return func()
+            kwargs = {
+                'force': force,
+                'recursive': recursive,
+                'raw': raw
+            }
+            return func(**kwargs)
         else:
             # raise PyPowerwallCloudNotImplemented(api)
             # or pass a custom error response:
             return {"ERROR": f"Unknown API: {api}"}
 
-    def getsites(self):
+    def post(self, api: str, payload: Optional[dict], din: Optional[str],
+             recursive: bool = False, raw: bool = False) -> Optional[Union[dict, list, str, bytes]]:
+        """
+        Map Powerwall API to Tesla Cloud Data
+        """
+        if self.tesla is None:
+            raise PyPowerwallCloudTeslaNotConnected
+        # API Map - Determine what data we need based on Powerwall APIs
+        log.debug(f" -- cloud: Request for {api}")
+
+        func = self.post_api_map.get(api)
+        if func:
+            kwargs = {
+                'payload': payload,
+                'din': din
+            }
+            res = func(**kwargs)
+            if res:
+                # invalidate appropriate read cache on (more or less) successful call to writable API
+                super()._invalidate_cache(api)
+            return res
+        else:
+            # raise PyPowerwallCloudNotImplemented(api)
+            # or pass a custom error response:
+            return {"ERROR": f"Unknown API: {api}"}
+
+    def getsites(self) -> Optional[List[Union[Battery, SolarPanel]]]:
         """
         Get list of Tesla Energy sites
         """
         if self.tesla is None:
             return None
         try:
             sitelist = self.tesla.battery_list() + self.tesla.solar_list()
@@ -232,24 +268,25 @@
                 log.debug(f"Changed site to {self.siteid} ({sites[self.siteindex]['site_name']}) for {self.email}")
                 return True
         log.error("Site %d not found for %s" % (siteid, self.email))
         return False
 
     # Functions to get data from Tesla Cloud
 
-    def _site_api(self, name, ttl, **kwargs):
+    def _site_api(self, name: str, ttl: int, force: bool, **kwargs):
         """
         Private function to get site data from Tesla Cloud using
         TeslaPy API.  This function uses a lock to prevent threads
         from sending multiple requests to Tesla Cloud at the same time.
         It also caches the data for ttl seconds.
 
         Arguments:
             name - TeslaPy API name
             ttl - Cache expiration time in seconds
+            force - If True skip cache
             kwargs - Variable arguments to pass to API call
 
         Returns (response, cached)
             response - TeslaPy API response
             cached - True if cached data was returned
         """
         if self.tesla is None:
@@ -257,18 +294,18 @@
             return None, False
         # Check for lock and wait if api request already sent
         if name in self.apilock:
             locktime = time.perf_counter()
             while self.apilock[name]:
                 time.sleep(0.2)
                 if time.perf_counter() >= locktime + self.timeout:
-                    log.debug(f" -- cloud: Timeout waiting for {name}")
+                    log.debug(f" -- cloud: Timeout waiting for {name} (unable to acquire lock)")
                     return None, False
         # Check to see if we have cached data
-        if name in self.pwcache:
+        if self.pwcache.get(name) is not None and not force:
             if self.pwcachetime[name] > time.perf_counter() - ttl:
                 log.debug(f" -- cloud: Returning cached {name} data")
                 return self.pwcache[name], True
 
         response = None
         try:
             # Set lock
@@ -281,15 +318,15 @@
             self.pwcache[name] = response
             self.pwcachetime[name] = time.perf_counter()
         finally:
             # Release lock
             self.apilock[name] = False
             return response, False
 
-    def get_battery(self):
+    def get_battery(self, force: bool = False):
         """
         Get site battery data from Tesla Cloud
 
             "response": {
                 "resource_type": "battery",
                 "site_name": "Tesla Energy Gateway",
                 "gateway_id": "1232100-00-E--TGxxxxxxxxxxxx",
@@ -305,19 +342,18 @@
                 "powerwall_tesla_electric_interested_in": null,
                 "vpp_tour_enabled": null,
                 "sync_grid_alert_enabled": true,
                 "breaker_alert_enabled": true
             }
         """
         # GET api/1/energy_sites/{site_id}/site_status
-        (response, _) = self._site_api("SITE_SUMMARY",
-                                       self.pwcacheexpire, language="en")
+        (response, _) = self._site_api("SITE_SUMMARY", self.pwcacheexpire, language="en", force=force)
         return response
 
-    def get_site_power(self):
+    def get_site_power(self, force: bool = False):
         """
         Get site power data from Tesla Cloud
 
             "response": {
                 "solar_power": 1290,
                 "energy_left": 21276.894736842103,
                 "total_pack_energy": 25939,
@@ -333,24 +369,26 @@
                 "island_status": "on_grid",
                 "storm_mode_active": false,
                 "timestamp": "2023-12-17T14:23:31-08:00",
                 "wall_connectors": []
             }
         """
         # GET api/1/energy_sites/{site_id}/live_status?counter={counter}&language=en
-        (response, cached) = self._site_api("SITE_DATA",
-                                            self.pwcacheexpire, counter=self.counter + 1, language="en")
+        (response, cached) = self._site_api("SITE_DATA", self.pwcacheexpire, counter=self.counter + 1,
+                                            language="en", force=force)
         if not cached:
             self.counter = (self.counter + 1) % COUNTER_MAX
         return response
 
-    def get_site_config(self):
+    def get_site_config(self, force: bool = False):
         """
         Get site configuration data from Tesla Cloud
 
+        Args:
+            force:     if True, skip cache
         "response": {
             "id": "1232100-00-E--TGxxxxxxxxxxxx",
             "site_name": "Tesla Energy Gateway",
             "backup_reserve_percent": 80,
             "default_real_mode": "self_consumption",
             "installation_date": "xxxx-xx-xx",
             "user_settings": {
@@ -427,52 +465,53 @@
             },
             "vpp_backup_reserve_percent": 80
         }
     }
 
         """
         # GET api/1/energy_sites/{site_id}/site_info
-        (response, _) = self._site_api("SITE_CONFIG",
-                                       SITE_CONFIG_TTL, language="en")
+        (response, _) = self._site_api("SITE_CONFIG", SITE_CONFIG_TTL, language="en", force=force)
         return response
 
-    def get_time_remaining(self) -> Optional[float]:
+    def get_time_remaining(self, force: bool = False) -> Optional[float]:
         """
         Get backup time remaining from Tesla Cloud
 
         {'response': {'time_remaining_hours': 7.909122698326978}}
         """
         # GET api/1/energy_sites/{site_id}/backup_time_remaining
-        (response, _) = self._site_api("ENERGY_SITE_BACKUP_TIME_REMAINING",
-                                       self.pwcacheexpire, language="en")
+        (response, _) = self._site_api("ENERGY_SITE_BACKUP_TIME_REMAINING", self.pwcacheexpire, language="en",
+                                       force=force)
 
         # {'response': {'time_remaining_hours': 7.909122698326978}}
         if response is None or not isinstance(response, dict):
             return None
         if 'response' in response and 'time_remaining_hours' in response.get('response'):
             return response['response']['time_remaining_hours']
 
         return 0.0
 
-    def get_api_system_status_soe(self) -> Optional[Union[dict, list, str, bytes]]:
-        battery = self.get_battery()
+    def get_api_system_status_soe(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
+        force = kwargs.get('force', False)
+        battery = self.get_battery(force=force)
         if battery is None:
             data = None
         else:
             percentage_charged = lookup(battery, ("response", "percentage_charged")) or 0
             # percentage_charged is scaled to keep 5% buffer at bottom
             soe = (percentage_charged + (5 / 0.95)) * 0.95
             data = {
                 "percentage": soe
             }
         return data
 
-    def get_api_status(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_status(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         # TOOO: Fix start_time and up_time_seconds
-        config = self.get_site_config()
+        force = kwargs.get('force', False)
+        config = self.get_site_config(force=force)
         if config is None:
             data = None
         else:
             data = {
                 "din": lookup(config, ("response", "id")),  # 1232100-00-E--TGxxxxxxxxxxxx
                 "start_time": lookup(config, ("response", "installation_date")),  # "2023-10-13 04:01:45 +0800"
                 "up_time_seconds": None,  # "1541h38m20.998412744s"
@@ -484,45 +523,48 @@
                 "teg_type": "unknown",
                 "sync_type": "v2.1",
                 "cellular_disabled": False,
                 "can_reboot": True
             }
         return data
 
-    def get_api_system_status_grid_status(self) -> Optional[Union[dict, list, str, bytes]]:
-        power = self.get_site_power()
+    def get_api_system_status_grid_status(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
+        force = kwargs.get('force', False)
+        power = self.get_site_power(force=force)
         if power is None:
             data = None
         else:
             if lookup(power, ("response", "grid_status")) == "Active":
                 grid_status = "SystemGridConnected"
             else:  # off_grid or off_grid_unintentional
                 grid_status = "SystemIslandedActive"
             data = {
                 "grid_status": grid_status,  # SystemIslandedActive or SystemTransitionToGrid
                 "grid_services_active": lookup(power, ("response", "grid_services_active"))
                 # true when participating in VPP event
             }
         return data
 
-    def get_api_site_info_site_name(self) -> Optional[Union[dict, list, str, bytes]]:
-        config = self.get_site_config()
+    def get_api_site_info_site_name(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
+        force = kwargs.get('force', False)
+        config = self.get_site_config(force=force)
         if config is None:
             data = None
         else:
             sitename = lookup(config, ("response", "site_name"))
             tz = lookup(config, ("response", "installation_time_zone"))
             data = {
                 "site_name": sitename,
                 "timezone": tz
             }
         return data
 
-    def get_api_site_info(self) -> Optional[Union[dict, list, str, bytes]]:
-        config = self.get_site_config()
+    def get_api_site_info(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
+        force = kwargs.get('force', False)
+        config = self.get_site_config(force=force)
         if config is None:
             data = None
         else:
             nameplate_power = int(lookup(config, ("response", "nameplate_power")) or 0) / 1000
             nameplate_energy = int(lookup(config, ("response", "nameplate_energy")) or 0) / 1000
             max_site_meter_power_ac = lookup(config, ("response", "max_site_meter_power_ac"))
             min_site_meter_power_ac = lookup(config, ("response", "min_site_meter_power_ac"))
@@ -547,24 +589,26 @@
                     "country": None,
                     "state": None,
                     "utility": utility
                 }
             }
         return data
 
-    def get_api_devices_vitals(self) -> Optional[Union[dict, list, str, bytes]]:
+    # noinspection PyUnusedLocal
+    def get_api_devices_vitals(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         # Protobuf payload - not implemented - use /vitals instead
         data = None
         log.warning("Protobuf payload - not implemented for /api/devices/vitals - use /vitals instead")
         return data
 
-    def get_vitals(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_vitals(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         # Simulated Vitals
-        config = self.get_site_config()
-        power = self.get_site_power()
+        force = kwargs.get('force', False)
+        config = self.get_site_config(force=force)
+        power = self.get_site_power(force=force)
         if config is None or power is None:
             data = None
         else:
             din = lookup(config, ("response", "id"))
             parts = din.split("--")
             if len(parts) == 2:
                 part_number = parts[0]
@@ -600,17 +644,18 @@
                     'alerts': [
                         alert
                     ]
                 }
             }
         return data
 
-    def get_api_meters_aggregates(self) -> Optional[Union[dict, list, str, bytes]]:
-        config = self.get_site_config()
-        power = self.get_site_power()
+    def get_api_meters_aggregates(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
+        force = kwargs.get('force', False)
+        config = self.get_site_config(force=force)
+        power = self.get_site_power(force=force)
         if config is None or power is None:
             data = None
         else:
             timestamp = lookup(power, ("response", "timestamp"))
             solar_power = lookup(power, ("response", "solar_power"))
             battery_power = lookup(power, ("response", "battery_power"))
             load_power = lookup(power, ("response", "load_power"))
@@ -641,33 +686,35 @@
             data['solar'].update({
                 "last_communication_time": timestamp,
                 "instant_power": solar_power,
                 "num_meters_aggregated": solar_inverters,
             })
         return data
 
-    def get_api_operation(self) -> Optional[Union[dict, list, str, bytes]]:
-        config = self.get_site_config()
+    def get_api_operation(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
+        force = kwargs.get('force', False)
+        config = self.get_site_config(force)
         if config is None:
             data = None
         else:
             default_real_mode = lookup(config, ("response", "default_real_mode"))
             backup_reserve_percent = lookup(config, ("response", "backup_reserve_percent")) or 0
             # backup_reserve_percent is scaled to keep 5% buffer at bottom
             backup = (backup_reserve_percent + (5 / 0.95)) * 0.95
             data = {
                 "real_mode": default_real_mode,
                 "backup_reserve_percent": backup
             }
         return data
 
-    def get_api_system_status(self) -> Optional[Union[dict, list, str, bytes]]:
-        power = self.get_site_power()
-        config = self.get_site_config()
-        battery = self.get_battery()
+    def get_api_system_status(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
+        force = kwargs.get('force', False)
+        power = self.get_site_power(force=force)
+        config = self.get_site_config(force=force)
+        battery = self.get_battery(force=force)
         if power is None or config is None or battery is None:
             data = None
         else:
             # timestamp = lookup(power, ("response", "timestamp"))
             solar_power = lookup(power, ("response", "solar_power"))
             # battery_power = lookup(power, ("response", "battery_power"))
             # load_power = lookup(power, ("response", "load_power"))
@@ -698,92 +745,111 @@
                 "available_blocks": battery_count,
                 "solar_real_power_limit": solar_power,
                 "blocks_controlled": battery_count,
             })
 
         return data
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def api_logout(self) -> Optional[Union[dict, list, str, bytes]]:
+    def api_logout(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return {"status": "ok"}
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def api_login_basic(self) -> Optional[Union[dict, list, str, bytes]]:
+    def api_login_basic(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return {"status": "ok"}
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_meters_site(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_meters_site(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads(METERS_SITE)
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_unimplemented_api(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_unimplemented_api(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return None
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_unimplemented_timeout(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_unimplemented_timeout(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return "TIMEOUT!"
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_auth_toggle_supported(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_auth_toggle_supported(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return {"toggle_auth_supported": True}
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_sitemaster(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_sitemaster(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return {"status": "StatusUp", "running": True, "connected_to_tesla": True, "power_supply_mode": False,
                 "can_reboot": "Yes"}
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_powerwalls(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_powerwalls(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads(POWERWALLS)
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_customer_registration(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_customer_registration(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads('{"privacy_notice":null,"limited_warranty":null,"grid_services":null,"marketing":null,'
                           '"registered":true,"timed_out_registration":false}')
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_system_update_status(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_system_update_status(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads('{"state":"/update_succeeded","info":{"status":["nonactionable"]},'
                           '"current_time":1702756114429,"last_status_time":1702753309227,"version":"23.28.2 27626f98",'
                           '"offline_updating":false,"offline_update_error":"","estimated_bytes_per_second":null}')
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_system_status_grid_faults(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_system_status_grid_faults(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads('[]')
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_solars(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_solars(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads('[{"brand":"Tesla","model":"Solar Inverter 7.6","power_rating_watts":7600}]')
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_solars_brands(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_solars_brands(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads(SOLARS_BRANDS)
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_customer(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_customer(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return {"registered": True}
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_meters(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_meters(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads(METERS)
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_installer(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_installer(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads(INSTALLER)
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_synchrometer_ct_voltage_references(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_synchrometer_ct_voltage_references(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads('{"ct1":"Phase1","ct2":"Phase2","ct3":"Phase1"}')
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_troubleshooting_problems(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_troubleshooting_problems(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return json.loads('{"problems":[]}')
 
+    # noinspection PyUnusedLocal
     @not_implemented_mock_data
-    def get_api_solar_powerwall(self) -> Optional[Union[dict, list, str, bytes]]:
+    def get_api_solar_powerwall(self, **kwargs) -> Optional[Union[dict, list, str, bytes]]:
         return {}
 
     def setup(self, email=None):
         """
         Set up the Tesla Cloud connection
         """
         print("Tesla Account Setup")
@@ -920,14 +986,62 @@
         else:
             log.error(f"Tesla cloud not connected")
         self.auth = {}
 
     def vitals(self) -> Optional[dict]:
         return self.poll('/vitals')
 
+    def post_api_operation(self, **kwargs):
+        payload = kwargs.get('payload', {})
+        din = kwargs.get('din')
+
+        if not payload.get('backup_reserve_percent') and not payload.get('real_mode'):
+            raise PyPowerwallCloudInvalidPayload("/api/operation payload missing required parameters. Either "
+                                                 "'backup_reserve_percent or 'real_mode', or both must present.")
+
+        if not din:
+            log.warning("No valid DIN provided, will adjust the first battery on site.")
+
+        batteries = self.tesla.battery_list()
+        log.debug(f"Got batteries: {batteries}")
+        for battery in batteries:
+            if din and battery.get('gateway_id') != din:
+                continue
+            try:
+                op_level = battery.set_backup_reserve_percent(payload['backup_reserve_percent'])
+                op_mode = battery.set_operation(payload['real_mode'])
+                log.debug(f"Op Level: {op_level}")
+                log.debug(f"Op Mode: {op_mode}")
+                return {
+                    'set_backup_reserve_percent': {
+                        'backup_reserve_percent': payload['backup_reserve_percent'],
+                        'din': din,
+                        'result': op_level
+                    },
+                    'set_operation': {
+                        'real_mode': payload['real_mode'],
+                        'din': din,
+                        'result': op_mode
+                    }
+                }
+            except Exception as exc:
+                return {'error': f"{exc}"}
+        return {
+            'set_backup_reserve_percent': {
+                'backup_reserve_percent': payload['backup_reserve_percent'],
+                'din': din,
+                'result': 'BatteryNotFound'
+            },
+            'set_operation': {
+                'real_mode': payload['real_mode'],
+                'din': din,
+                'result': 'BatteryNotFound'
+            }
+        }
+
 
 if __name__ == "__main__":
     # Test code
     set_debug(quiet=False, debug=True, color=True)
     tesla_user = None
     # Check for .pypowerwall.auth file
     AUTHPATH = os.environ.get('PW_AUTH_PATH', "")
```

## pypowerwall/local/pypowerwall_local.py

```diff
@@ -25,15 +25,14 @@
         self.cachefile = cachefile  # Stores auth session information
         self.authmode = authmode  # cookie or token
         self.timeout = timeout
         self.timezone = timezone
 
         self.session = None
         self.pwcachetime = {}  # holds the cached data timestamps for api
-        self.pwcache = {}  # holds the cached data for api
         self.pwcacheexpire = pwcacheexpire  # seconds to expire cache
         self.pwcooldown = 0  # rate limit cooldown time - pause api calls
         self.vitals_api = True  # vitals api is available for local mode
 
     def authenticate(self):
         log.debug('Tesla local mode enabled')
         if self.poolmaxsize > 0:
@@ -112,32 +111,34 @@
     def poll(self, api: str, force: bool = False,
              recursive: bool = False, raw: bool = False) -> Optional[Union[dict, list, str, bytes]]:
 
         # Query powerwall and return payload
         raw = False
         payload = None
         # Check cache
-        if api in self.pwcache and api in self.pwcachetime:
+        if self.pwcache.get(api) is not None and self.pwcachetime.get(api) is not None:
             # is it expired?
             if time.perf_counter() - self.pwcachetime[api] < self.pwcacheexpire:
                 payload = self.pwcache[api]
+                log.debug(' -- local: Returning cached %s' % api)
                 # We do the override here to ensure that we cache the force entry
 
         if not payload or force:
             if self.pwcooldown > time.perf_counter():
                 # Rate limited - return None
                 log.debug('Rate limit cooldown period - Pausing API calls')
                 return None
             if api == '/api/devices/vitals':
                 if not self.vitals_api:
                     # Vitals API is not available
                     return None
                 # Always want the raw stream output from the vitals call; protobuf binary payload
                 raw = True
 
+            log.debug(' -- local: Request Powerwall for %s' % api)
             url = "https://%s%s" % (self.host, api)
             try:
                 if self.authmode == "token":
                     r: Response = self.session.get(url, headers=self.auth, verify=False, timeout=self.timeout,
                                                    stream=raw)
                 else:
                     r: Response = self.session.get(url, cookies=self.auth, verify=False, timeout=self.timeout,
@@ -161,33 +162,45 @@
                         # Vitals API not available for Firmware >= 23.44.0
                         self.vitals_api = False
                         log.error('Firmware %s detected - Does not support vitals API - disabling.' % version)
                         # Cache and increase cache TTL by 10 minutes
                 self.pwcachetime[api] = time.perf_counter() + 600
                 self.pwcache[api] = None
                 return None
-            if r.status_code == 429:
+            elif r.status_code == 429:
                 # Rate limited - Switch to cooldown mode for 5 minutes
                 self.pwcooldown = time.perf_counter() + 300
                 log.error('429 Rate limited by Powerwall API at %s - Activating 5 minute cooldown' % url)
-                # Serve up cached data if it exists
                 return None
-            if 400 <= r.status_code < 500:
+            elif r.status_code == 401 or r.status_code == 403:
                 # Session Expired - Try to get a new one unless we already tried
                 log.debug('Session Expired - Trying to get a new one')
                 if not recursive:
                     if raw:
                         # Drain the stream before retrying
                         # noinspection PyUnusedLocal
                         payload = r.raw.data
                     self._get_session()
-                    return self.poll(api)
+                    return self.poll(api, raw=raw, recursive=True)
                 else:
-                    log.error('Unable to establish session with Powerwall at %s - check password' % url)
+                    if r.status_code == 401:
+                        log.error('Unable to establish session with Powerwall at %s - check password' % url)
+                    else:
+                        log.error('403 Unauthorized by Powerwall API at %s - Endpoint disabled in this firmware or '
+                                  'user lacks permission' % url)
+                    self.pwcachetime[api] = time.perf_counter() + 600
+                    self.pwcache[api] = None
                     return None
+            elif 400 <= r.status_code < 500:
+                log.error('Unhandled HTTP response code %s at %s' % (r.status_code, url))
+                return None
+            elif r.status_code >= 500:
+                log.error('Server-side problem at Powerwall API (status code %s) at %s' % (r.status_code, url))
+                return None
+
             if raw:
                 payload = r.raw.data
             else:
                 payload = r.text
                 if not payload:
                     log.debug(f"Empty response from Powerwall at {url}")
                     return None
@@ -203,14 +216,85 @@
             self.pwcache[api] = payload
             self.pwcachetime[api] = time.perf_counter()
             return payload
         else:
             # should be already a dict in cache, so just return it
             return payload
 
+    def post(self, api: str, payload: Optional[dict], din: Optional[str],
+             recursive: bool = False, raw: bool = False) -> Optional[Union[dict, list, str, bytes]]:
+
+        # We probably should not cache responses here
+        # Also, we may have to use different HTTP Methods such as POST, PUT, PATCH based on Powerwall API requirements
+        # For now we assume it's taking POST calls
+
+        url = "https://%s%s" % (self.host, api)
+        try:
+            if self.authmode == "token":
+                r = self.session.post(url, headers=self.auth, json=payload, verify=False, timeout=self.timeout,
+                                      stream=raw)
+            else:
+                r = self.session.post(url, cookies=self.auth, json=payload, verify=False, timeout=self.timeout,
+                                      stream=raw)
+        except requests.exceptions.Timeout:
+            log.debug('ERROR Timeout waiting for Powerwall API %s' % url)
+            return None
+        except requests.exceptions.ConnectionError:
+            log.debug('ERROR Unable to connect to Powerwall at %s' % url)
+            return None
+        except Exception as exc:
+            log.debug('ERROR Unknown error connecting to Powerwall at %s: %s' % (url, exc))
+            return None
+        if r.status_code == 404:
+            log.debug('404 Powerwall API not found at %s' % url)
+            return None
+        elif r.status_code == 401:
+            # Session Expired - Try to get a new one unless we already tried
+            log.debug('Session Expired - Trying to get a new one')
+            if not recursive:
+                if raw:
+                    # Drain the stream before retrying
+                    # noinspection PyUnusedLocal
+                    response = r.raw.data
+                self._get_session()
+                return self.post(api=api, payload=payload, din=din, raw=raw, recursive=True)
+            else:
+                log.error('Unable to establish session with Powerwall at %s - check password' % url)
+                return None
+        elif r.status_code == 403:
+            # Unauthorized
+            log.error('403 Unauthorized by Powerwall API at %s - Endpoint disabled in this firmware or '
+                      'user lacks permission' % url)
+            return None
+        elif 400 <= r.status_code < 500:
+            log.error('Unhandled HTTP response code %s at %s' % (r.status_code, url))
+            return None
+        elif r.status_code >= 500:
+            log.error('Server-side problem at Powerwall API (status code %s) at %s' % (r.status_code, url))
+            return None
+        if raw:
+            response = r.raw.data
+        else:
+            response = r.text
+            if not response:
+                log.debug(f"Empty response from Powerwall at {url}")
+                return None
+            elif 'application/json' in r.headers.get('Content-Type'):
+                try:
+                    response = json.loads(response)
+                except Exception as exc:
+                    log.error(f"Unable to parse response '{response}' as JSON, even though it was supposed to "
+                              f"be a json: {exc}")
+                    return None
+            else:
+                log.debug(f"Non-json response from Powerwall at {url}: '{response}', serving as is.")
+        # invalidate appropriate read cache on (more or less) successful call to writable API
+        super()._invalidate_cache(api)
+        return response
+
     def version(self, int_value=False):
         """ Firmware Version """
         if not int_value:
             return self.status('version')
         # Convert version to integer
         return parse_version(self.status('version'))
```

## Comparing `pypowerwall-0.8.0.dist-info/LICENSE` & `pypowerwall-0.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pypowerwall-0.8.0.dist-info/METADATA` & `pypowerwall-0.8.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypowerwall
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python module to access Tesla Energy Gateway for Powerwall and solar power data
 Home-page: https://github.com/jasonacox/pypowerwall
 Author: Jason Cox
 Author-email: jason@jasonacox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -153,14 +153,15 @@
     siteid                    # If cloudmode is True, use this siteid (default is None)  
     authpath                  # Path to cloud auth and site cache files (default is "")
     authmode = "cookie"       # "cookie" (default) or "token" - use cookie or bearer token for auth
     cachefile = ".powerwall"  # Path to cache file (default current directory)
 
  Functions 
     poll(api, json, force)    # Return data from Powerwall api (dict if json=True, bypass cache force=True)
+    post(api, payload, json)  # Send payload to Powerwall api (dict if json=True)
     level()                   # Return battery power level percentage
     power()                   # Return power data returned as dictionary
     site(verbose)             # Return site sensor data (W or raw JSON if verbose=True)
     solar(verbose):           # Return solar sensor data (W or raw JSON if verbose=True)
     battery(verbose):         # Return battery sensor data (W or raw JSON if verbose=True)
     load(verbose)             # Return load sensor data (W or raw JSON if verbose=True)
     grid()                    # Alias for site()
@@ -179,32 +180,54 @@
                               # system_status() and vitals()
     grid_status(type)         # Return the power grid status, type ="string" (default),
                               # "json", or "numeric":
                               #     - "string": "UP", "DOWN", "SYNCING"
                               #     - "numeric": -1 (Syncing), 0 (DOWN), 1 (UP)
     is_connected()            # Returns True if able to connect to Powerwall
     get_reserve(scale)        # Get Battery Reserve Percentage
+    get_mode()                # Get Current Battery Operation Mode
+    set_reserve(level)        # Set Battery Reserve Percentage (only cloud mode)
+    set_mode(mode)            # Set Current Battery Operation Mode (only cloud mode)
     get_time_remaining()      # Get the backup time remaining on the battery
+
+    set_operation(level, mode, json)        # Set Battery Reserve Percentage and/or Operation Mode
     
 ```
 
 ## Tools
 
 The following are some useful tools based on pypowerwall:
 
 * [Powerwall Proxy](proxy) - Use this caching proxy to handle authentication to the Powerwall Gateway and make basic read-only API calls to /api/meters/aggregates (power metrics), /api/system_status/soe (battery level) and many [others](https://github.com/jasonacox/pypowerwall/blob/main/proxy/HELP.md). This is useful for metrics gathering tools like telegraf to pull metrics without needing to authenticate. Because pyPowerwall is designed to cache the auth and high frequency API calls, this will also reduce the load on the Gateway and prevent crash/restart issues that can happen if too many session are created on the Gateway.
 
 * [Powerwall Simulator](simulator) - A Powerwall simulator to mimic the responses from the Tesla Powerwall Gateway. This is useful for testing purposes.
 
 * [Powerwall Dashboard](https://github.com/jasonacox/Powerwall-Dashboard#powerwall-dashboard) - Monitoring Dashboard for the Tesla Powerwall using Grafana, InfluxDB, Telegraf and pyPowerwall.
 
-## Powerwall Scanner
+## Powerwall Command Line
+
+pyPowerwall has a built in feature to scan your network for available Powerwall gateways and set/get operational and reserve modes.
+
+```
+Usage: PyPowerwall [-h] {setup,scan,set,get,version} ...
+
+PyPowerwall Module v0.8.1
 
-pyPowerwall has a built in feature to scan your network for available Powerwall gateways.  This will help you find the IP address of your Powerwall.
+Options:
+  -h, --help            Show this help message and exit
 
+Commands (run <command> -h to see usage information):
+  {setup,scan,set,get,version}
+    setup               Setup Tesla Login for Cloud Mode access
+    scan                Scan local network for Powerwall gateway
+    set                 Set Powerwall Mode and Reserve Level
+    get                 Get Powerwall Settings and Power Levels
+    version             Print version information
+```
+   
 ```bash
 # Install pyPowerwall if you haven't already
 python -m pip install pypowerwall
 
 # Scan Network for Powerwalls
 python -m pypowerwall scan
 ```
@@ -224,14 +247,43 @@
       Host: 10.0.1.36 ... OPEN - Found Powerwall 1232100-00-E--TG123456789ABG
       Done                           
 
 Discovered 1 Powerwall Gateway
      10.0.1.36 [1232100-00-E--TG123456789ABG]
 ```
 
+Get Power Levels, Operation Mode, and Battery Reserve Level
+
+```bash
+# Setup Connection with Tesla Cloud
+python -m pypowerwall setup
+
+# Get Power Levels, Operation Mode, and Battery Reserve Setting
+#
+# Usage: PyPowerwall get [-h] [-format FORMAT]
+#  -h, --help      show this help message and exit
+#  -format FORMAT  Output format: text, json, csv
+#
+python -m pypowerwall get
+python -m pypowerwall get -format json
+python -m pypowerwall get -format csv
+
+# Set Operation Mode and Battery Reserve Setting
+#
+# Usage: PyPowerwall set [-h] [-mode MODE] [-reserve RESERVE] [-current]
+#  -h, --help        show this help message and exit
+#  -mode MODE        Powerwall Mode: self_consumption, backup, or autonomous
+#  -reserve RESERVE  Set Battery Reserve Level [Default=20]
+#  -current          Set Battery Reserve Level to Current Charge
+#
+python -m pypowerwall set -mode self_consumption
+python -m pypowerwall set -reserve 30
+python -m pypowerwall set -current
+```
+
 ## Example API Calls
 
 The following APIs are a result of help from other projects as well as my own investigation. 
 
 * pw.poll('/api/system_status/soe') - Battery percentage (JSON with float 0-100)
 
    ```json
```

## Comparing `pypowerwall-0.8.0.dist-info/RECORD` & `pypowerwall-0.8.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-pypowerwall/__init__.py,sha256=d25_Iu6Qi_gJIECEP8NwdfBK5kN3hR-pEaSLj2q5gwM,25490
-pypowerwall/__main__.py,sha256=dZ2c0vA75pKFzlQ3KwLVoigSUqP9p_clkYx_Y0CrybE,2436
-pypowerwall/pypowerwall_base.py,sha256=rZm1mvcEZPg6uM6GXq1nlnfcx8A_o7Omi3Wq4E-Vpwo,2217
+pypowerwall/__init__.py,sha256=c6hFRHIjwozytDPQRfcibwWUxHYLw17dfmbyN9bjI20,32574
+pypowerwall/__main__.py,sha256=yDDWrUHvdk_jy5JUOqHYWNgGyTsBaL9j8DqQQtoE080,5835
+pypowerwall/aux.py,sha256=9VR4d4q163AdQQ4ELHLUYEH-RDOr-490cNZiGZFXlXM,1889
+pypowerwall/exceptions.py,sha256=D2TxwF42_quXoVr7CSQ1ifhSms_eHBJnFwy9l-bdtB0,133
+pypowerwall/pypowerwall_base.py,sha256=HKTNQQ59QfqtZtqYBe5rSkB8qyfZq9WPOwywzFvK7bs,2897
 pypowerwall/scan.py,sha256=DM9CxQLceu0bmyPaH8fNRdLgkS3oe4ata_78eObSNn8,6718
 pypowerwall/cloud/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pypowerwall/cloud/decorators.py,sha256=aDwS9G-g7B8Md0dPPucHVd5mIdvrGKlz8typC-YHBCU,638
-pypowerwall/cloud/exceptions.py,sha256=G3_vJgN18WgmyXvrruN_ot-kW1iL4RiQkU7-OjGDR4c,182
+pypowerwall/cloud/exceptions.py,sha256=tBSq0cUJvINmTMIcaq53iceSOmh-7hntqHIRCG6PEL0,242
 pypowerwall/cloud/mock_data.py,sha256=8CLdxyAhMY5I-tYsxUqcjGHth4T5NJkqvm-V6GUIAXM,18733
-pypowerwall/cloud/pypowerwall_cloud.py,sha256=G2zWT87Q6X_BqNYO8NDFwr4uKCxxL0ygx7kC9qplhWQ,41244
+pypowerwall/cloud/pypowerwall_cloud.py,sha256=hq8ZRuQHJxJvP_mNn4PQLz8iThtAzbumK0ddJ8J7_IQ,46292
 pypowerwall/cloud/stubs.py,sha256=JQXgAONPzJSuK7_N55ODBOHAMpm_CfZ4YYmJFbJEWvg,4355
 pypowerwall/local/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pypowerwall/local/exceptions.py,sha256=JRm141HHbwKSkdeIWttOrniQTeehGJ3Zo6Fg9KH4Scc,92
-pypowerwall/local/pypowerwall_local.py,sha256=eYKFCWIIwJcahFkM73PlEj_fpagkNcApVowrnzZrTjg,15816
+pypowerwall/local/pypowerwall_local.py,sha256=hXEXm7phGJ3laUql03eKJPvU-t-digQXVPJRvV-sNn0,20130
 pypowerwall/local/tesla_pb2.py,sha256=l3faEX13xLWbWh6KRtbyCClK3zXpyN0LY6y3kM3Dpp8,71273
-pypowerwall-0.8.0.dist-info/LICENSE,sha256=9cu5S_JpsnnwkV5ZWabxJwmoObWpOncMZaKdYe9vrH0,1066
-pypowerwall-0.8.0.dist-info/METADATA,sha256=C4XKKGVbXEuohQE6ogm-KRA7Q6YCyIZJgmtQduKQlYU,39811
-pypowerwall-0.8.0.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-pypowerwall-0.8.0.dist-info/top_level.txt,sha256=xAKahe-O0UjzTWlyxF1oHIZuAXkioYNTlC32ttXxjaM,12
-pypowerwall-0.8.0.dist-info/RECORD,,
+pypowerwall-0.8.1.dist-info/LICENSE,sha256=9cu5S_JpsnnwkV5ZWabxJwmoObWpOncMZaKdYe9vrH0,1066
+pypowerwall-0.8.1.dist-info/METADATA,sha256=sz1_3WEd5Hge7UZHMl8TaWjVn9deIAHPXxT12TQzipM,41728
+pypowerwall-0.8.1.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
+pypowerwall-0.8.1.dist-info/top_level.txt,sha256=xAKahe-O0UjzTWlyxF1oHIZuAXkioYNTlC32ttXxjaM,12
+pypowerwall-0.8.1.dist-info/RECORD,,
```

