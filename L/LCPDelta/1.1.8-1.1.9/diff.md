# Comparing `tmp/LCPDelta-1.1.8.tar.gz` & `tmp/LCPDelta-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LCPDelta-1.1.8.tar", last modified: Thu Apr  4 16:06:14 2024, max compression
+gzip compressed data, was "LCPDelta-1.1.9.tar", last modified: Fri Apr  5 16:59:29 2024, max compression
```

## Comparing `LCPDelta-1.1.8.tar` & `LCPDelta-1.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.050181 LCPDelta-1.1.8/
--rw-rw-rw-   0        0        0      132 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     3405 2024-04-04 16:06:14.048179 LCPDelta-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2799 2024-04-04 15:46:25.000000 LCPDelta-1.1.8/README.md
--rw-rw-rw-   0        0        0      686 2024-04-04 15:46:25.000000 LCPDelta-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 16:06:14.051179 LCPDelta-1.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.684678 LCPDelta-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.045184 LCPDelta-1.1.8/src/LCPDelta.egg-info/
--rw-rw-rw-   0        0        0     3405 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      647 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 16:06:13.000000 LCPDelta-1.1.8/src/LCPDelta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.797773 LCPDelta-1.1.8/src/lcp_delta/
--rw-rw-rw-   0        0        0       21 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.830601 LCPDelta-1.1.8/src/lcp_delta/common/
--rw-rw-rw-   0        0        0       39 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/common/__init__.py
--rw-rw-rw-   0        0        0     3462 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/common/api_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:13.982180 LCPDelta-1.1.8/src/lcp_delta/enact/
--rw-rw-rw-   0        0        0      160 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/__init__.py
--rw-rw-rw-   0        0        0    46125 2024-04-04 15:58:29.000000 LCPDelta-1.1.8/src/lcp_delta/enact/api_helper.py
--rw-rw-rw-   0        0        0     1790 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/chart_helper.py
--rw-rw-rw-   0        0        0     4026 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/credentials_holder.py
--rw-rw-rw-   0        0        0     7938 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/dps_helper.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.000387 LCPDelta-1.1.8/src/lcp_delta/enact/response_objects/
--rw-rw-rw-   0        0        0      363 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/enact/response_objects/usage_info.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:06:14.041552 LCPDelta-1.1.8/src/lcp_delta/flextrack/
--rw-rw-rw-   0        0        0       91 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/flextrack/__init__.py
--rw-rw-rw-   0        0        0     3495 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/flextrack/api_helper.py
--rw-rw-rw-   0        0        0      626 2024-03-12 12:33:55.000000 LCPDelta-1.1.8/src/lcp_delta/global_helper_methods.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.091615 LCPDelta-1.1.9/
+-rw-rw-rw-   0        0        0      132 2023-11-09 09:59:32.000000 LCPDelta-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3405 2024-04-05 16:59:29.089618 LCPDelta-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2799 2024-04-05 16:56:19.000000 LCPDelta-1.1.9/README.md
+-rw-rw-rw-   0        0        0      686 2024-04-05 16:56:45.000000 LCPDelta-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:59:29.091615 LCPDelta-1.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:28.897045 LCPDelta-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.086675 LCPDelta-1.1.9/src/LCPDelta.egg-info/
+-rw-rw-rw-   0        0        0     3405 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 16:59:28.000000 LCPDelta-1.1.9/src/LCPDelta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:28.964763 LCPDelta-1.1.9/src/lcp_delta/
+-rw-rw-rw-   0        0        0       21 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:28.988898 LCPDelta-1.1.9/src/lcp_delta/common/
+-rw-rw-rw-   0        0        0       39 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/common/__init__.py
+-rw-rw-rw-   0        0        0     3462 2024-02-08 15:41:52.000000 LCPDelta-1.1.9/src/lcp_delta/common/api_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.053088 LCPDelta-1.1.9/src/lcp_delta/enact/
+-rw-rw-rw-   0        0        0      160 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/enact/__init__.py
+-rw-rw-rw-   0        0        0    49069 2024-04-05 16:56:19.000000 LCPDelta-1.1.9/src/lcp_delta/enact/api_helper.py
+-rw-rw-rw-   0        0        0     1790 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/enact/chart_helper.py
+-rw-rw-rw-   0        0        0     4026 2024-02-01 10:06:56.000000 LCPDelta-1.1.9/src/lcp_delta/enact/credentials_holder.py
+-rw-rw-rw-   0        0        0     7938 2024-03-15 17:02:19.000000 LCPDelta-1.1.9/src/lcp_delta/enact/dps_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.063099 LCPDelta-1.1.9/src/lcp_delta/enact/response_objects/
+-rw-rw-rw-   0        0        0      363 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/enact/response_objects/usage_info.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:59:29.084622 LCPDelta-1.1.9/src/lcp_delta/flextrack/
+-rw-rw-rw-   0        0        0       91 2023-11-16 15:21:26.000000 LCPDelta-1.1.9/src/lcp_delta/flextrack/__init__.py
+-rw-rw-rw-   0        0        0     3495 2023-11-30 10:40:08.000000 LCPDelta-1.1.9/src/lcp_delta/flextrack/api_helper.py
+-rw-rw-rw-   0        0        0      626 2024-02-08 17:40:02.000000 LCPDelta-1.1.9/src/lcp_delta/global_helper_methods.py
```

### Comparing `LCPDelta-1.1.8/PKG-INFO` & `LCPDelta-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 1.1.8
+Version: 1.1.9
 Summary: LCPDelta Python Package
 Author-email: LCP Delta <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://portal.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack,Storetrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `LCPDelta-1.1.8/README.md` & `LCPDelta-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.8/pyproject.toml` & `LCPDelta-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LCPDelta"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="LCP Delta", email="enact.helpdesk@lcp.uk.com" },
 ]
 description = "LCPDelta Python Package"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["LCPDelta", "Enact", "Flextrack", "Storetrack"]
```

### Comparing `LCPDelta-1.1.8/src/LCPDelta.egg-info/PKG-INFO` & `LCPDelta-1.1.9/src/LCPDelta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 1.1.8
+Version: 1.1.9
 Summary: LCPDelta Python Package
 Author-email: LCP Delta <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://portal.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack,Storetrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `LCPDelta-1.1.8/src/LCPDelta.egg-info/SOURCES.txt` & `LCPDelta-1.1.9/src/LCPDelta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.8/src/lcp_delta/common/api_helper.py` & `LCPDelta-1.1.9/src/lcp_delta/common/api_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.8/src/lcp_delta/enact/api_helper.py` & `LCPDelta-1.1.9/src/lcp_delta/enact/api_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,61 @@
             if not df.empty:
                 first_key = next(iter(data))
                 df = df.set_index(first_key)
             output[date_str] = df
 
         return output
 
+    def get_latest_forecast_generated_at_given_time(self, series_id : str, date_from : datetime, date_to : datetime, country_id : str, forecast_as_of : datetime, option_id : list[str] = None) -> dict[str, pd.DataFrame]:
+        '''Gets the latest forecast generated prior to the given 'forecast_as_of' datetime
+
+        Args:
+            series_id `str`: The Enact ID for the requested Series, as defined in the query generator on the "General" tab.
+            date_from `datetime.datetime`: The start date you want all iterations of the forecast for.
+            date_to `datetime.datetime`: The end date you want all iterations of the forecast for.
+            country_id `str` (optional): This is the Enact ID for the requested Country, as defined in the query generator on the "General" tab. Defaults to "Gb".
+            forecast_as_of `datetime.datetime`: The date you want the latest forecast generated for.
+            option_id `list[str]` (optional): If the selected Series has options, then this is the Enact ID for the requested Option, as defined in the query generator on the "General" tab.
+                                          If this is not sent, then data for all options will be sent back (but capped to the first 10). Defaults to None.
+        Returns:
+            Response: This holds latest forecast generated to the given 'forecast_as_of' datetime for the range of dates requested in a dictionary keyed by the datetime string of each of these dates.
+                    The first row will provide the date we have a forecast iteration for, which will be the latest generated forecast before the given 'forecast_as_of' datetime.
+                    All other rows correspond to the data-points at each value of the first array.
+        '''
+        endpoint = 'https://enactapifd.lcp.uk.com/EnactAPI/HistoryOfForecast/get_latest_forecast'
+
+        date_from = self.convert_date_time_to_right_format(date_from)
+        date_to = self.convert_date_time_to_right_format(date_to)
+        forecast_as_of = self.convert_date_time_to_right_format(forecast_as_of)
+
+        request_details = {
+            'SeriesId': series_id,
+            'CountryId': country_id,
+            'From': date_from,
+            'To': date_to,
+            'ForecastAsOf': forecast_as_of
+        }
+
+        if option_id is not None:
+            if not is_list_of_strings(option_id):
+                raise Exception('Option ID input must be a list of strings')
+            request_details['OptionId'] = option_id
+
+        response = self.post_request(endpoint, request_details)
+
+        output : dict[str, pd.DataFrame] = {}
+        for date_str, data in response['data']['data'].items():
+            df = pd.DataFrame(data)
+            if not df.empty:
+                first_key = next(iter(data))
+                df = df.set_index(first_key)
+            output[date_str] = df
+
+        return output
+
     #BOA:
     def get_bm_data_by_period(self, date : datetime, period : int, include_accepted_times : bool = False) -> pd.DataFrame:
         '''Get BM (Balancing Mechanism) data for a specific date and period.
 
         This method retrieves the BM (Balancing Mechanism) data for a specific date and period.
         The date should be in the correct format, and the period should be an integer.
```

### Comparing `LCPDelta-1.1.8/src/lcp_delta/enact/chart_helper.py` & `LCPDelta-1.1.9/src/lcp_delta/enact/chart_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.8/src/lcp_delta/enact/credentials_holder.py` & `LCPDelta-1.1.9/src/lcp_delta/enact/credentials_holder.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.8/src/lcp_delta/enact/dps_helper.py` & `LCPDelta-1.1.9/src/lcp_delta/enact/dps_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.8/src/lcp_delta/flextrack/api_helper.py` & `LCPDelta-1.1.9/src/lcp_delta/flextrack/api_helper.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-1.1.8/src/lcp_delta/global_helper_methods.py` & `LCPDelta-1.1.9/src/lcp_delta/global_helper_methods.py`

 * *Files identical despite different names*

