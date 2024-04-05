# Comparing `tmp/bring-api-0.5.7.tar.gz` & `tmp/bring-api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring-api-0.5.7.tar", last modified: Sun Mar 24 21:34:52 2024, max compression
+gzip compressed data, was "bring-api-0.6.0.tar", last modified: Fri Apr  5 16:06:28 2024, max compression
```

## Comparing `bring-api-0.5.7.tar` & `bring-api-0.6.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:34:52.579085 bring-api-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-24 21:34:47.000000 bring-api-0.5.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-24 21:34:47.000000 bring-api-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-03-24 21:34:52.575085 bring-api-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-03-24 21:34:47.000000 bring-api-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:34:52.571085 bring-api-0.5.7/bring_api/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43824 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/bring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:34:52.575085 bring-api-0.5.7/bring_api/locales/
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.de-AT.json
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.de-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.de-DE.json
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.en-AU.json
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.en-CA.json
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.en-GB.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.en-US.json
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.es-ES.json
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.fr-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.fr-FR.json
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.hu-HU.json
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.it-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.it-IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.nb-NO.json
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.nl-NL.json
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.pl-PL.json
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.pt-BR.json
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.ru-RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.sv-SE.json
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/locales/articles.tr-TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-24 21:34:47.000000 bring-api-0.5.7/bring_api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:34:52.575085 bring-api-0.5.7/bring_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-03-24 21:34:52.000000 bring-api-0.5.7/bring_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-24 21:34:52.000000 bring-api-0.5.7/bring_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 21:34:52.000000 bring-api-0.5.7/bring_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-24 21:34:52.000000 bring-api-0.5.7/bring_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-24 21:34:52.000000 bring-api-0.5.7/bring_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-03-24 21:34:47.000000 bring-api-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-24 21:34:52.579085 bring-api-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.403682 bring-api-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-05 16:06:20.000000 bring-api-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 16:06:20.000000 bring-api-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-05 16:06:28.403682 bring-api-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-05 16:06:20.000000 bring-api-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.395682 bring-api-0.6.0/bring_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41753 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/bring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.399682 bring-api-0.6.0/bring_api/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.de-AT.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.de-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.de-DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-AU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-CA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.en-US.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.es-ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.fr-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.fr-FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.hu-HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.it-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.it-IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.nb-NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.nl-NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.pl-PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.pt-BR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.ru-RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.sv-SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/locales/articles.tr-TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-05 16:06:20.000000 bring-api-0.6.0/bring_api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.399682 bring-api-0.6.0/bring_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12891 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 16:06:28.000000 bring-api-0.6.0/bring_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-05 16:06:20.000000 bring-api-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-05 16:06:28.403682 bring-api-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:06:28.399682 bring-api-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    38934 2024-04-05 16:06:20.000000 bring-api-0.6.0/tests/test_bring.py
```

### Comparing `bring-api-0.5.7/CHANGELOG.md` & `bring-api-0.6.0/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # CHANGELOG
 
+## 0.6.0
+
+* **Pytest unit testing:** added pytest with full code coverage ([tr4nt0r](https://github.com/tr4nt0r))
+* **Github workflow for pytest:** added workflow for running pytests with Python 3.11 & 3.12 on Ubuntu, Windows and macOS ([tr4nt0r](https://github.com/tr4nt0r))
+* Update Python requirement to >=3.11
+* Change from implicit to explicit string conversion of `BringItemOperation` in JSON request payload ([tr4nt0r](https://github.com/tr4nt0r))
+* Change Type of `BringItemOperation` to `StrEnum` ([tr4nt0r](https://github.com/tr4nt0r))
+* `BringItem::operation` now also accepts string literals `TO_PURCHASE`, `TO_RECENTLY` & `REMOVE` ([tr4nt0r](https://github.com/tr4nt0r))
+* fix wrong variable name in `BringSyncCurrentUserResponse` class and add additional variables from JSON response ([tr4nt0r](https://github.com/tr4nt0r))
+* Improve exceptions for `save/update/remove/complete_item` and `batch_update_list` methods ([tr4nt0r](https://github.com/tr4nt0r))
+* Fix bug in `get_all_item_details` method ([tr4nt0r](https://github.com/tr4nt0r))
+* Parsing error when parsing unauthorized response now raises `BringParseException` ([tr4nt0r](https://github.com/tr4nt0r))
+* Cleanup legacy code ([tr4nt0r](https://github.com/tr4nt0r))
+
 ## 0.5.7
 
 * **map user language to locales**: Bring sometimes stores non-standard locales in the user settings. In case the Bring API returns an invalid/unsupported locale, the user language is now mapped to a supported locale. 
 
 ## 0.5.6
 
 * fix incorrect filtering of locales against supported locales list
```

### Comparing `bring-api-0.5.7/LICENSE` & `bring-api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/PKG-INFO` & `bring-api-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.5.7
+Version: 0.6.0
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 
 # Bring! Shopping Lists API
 
 [![PyPI version](https://badge.fury.io/py/bring-api.svg)](https://badge.fury.io/py/bring-api)
@@ -261,14 +261,28 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+## 0.6.0
+
+* **Pytest unit testing:** added pytest with full code coverage ([tr4nt0r](https://github.com/tr4nt0r))
+* **Github workflow for pytest:** added workflow for running pytests with Python 3.11 & 3.12 on Ubuntu, Windows and macOS ([tr4nt0r](https://github.com/tr4nt0r))
+* Update Python requirement to >=3.11
+* Change from implicit to explicit string conversion of `BringItemOperation` in JSON request payload ([tr4nt0r](https://github.com/tr4nt0r))
+* Change Type of `BringItemOperation` to `StrEnum` ([tr4nt0r](https://github.com/tr4nt0r))
+* `BringItem::operation` now also accepts string literals `TO_PURCHASE`, `TO_RECENTLY` & `REMOVE` ([tr4nt0r](https://github.com/tr4nt0r))
+* fix wrong variable name in `BringSyncCurrentUserResponse` class and add additional variables from JSON response ([tr4nt0r](https://github.com/tr4nt0r))
+* Improve exceptions for `save/update/remove/complete_item` and `batch_update_list` methods ([tr4nt0r](https://github.com/tr4nt0r))
+* Fix bug in `get_all_item_details` method ([tr4nt0r](https://github.com/tr4nt0r))
+* Parsing error when parsing unauthorized response now raises `BringParseException` ([tr4nt0r](https://github.com/tr4nt0r))
+* Cleanup legacy code ([tr4nt0r](https://github.com/tr4nt0r))
+
 ## 0.5.7
 
 * **map user language to locales**: Bring sometimes stores non-standard locales in the user settings. In case the Bring API returns an invalid/unsupported locale, the user language is now mapped to a supported locale. 
 
 ## 0.5.6
 
 * fix incorrect filtering of locales against supported locales list
```

### Comparing `bring-api-0.5.7/README.md` & `bring-api-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/bring.py` & `bring-api-0.6.0/bring_api/bring.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Bring api implementation."""
+
 import asyncio
 import json
 from json import JSONDecodeError
 import logging
 import os
 import traceback
 from typing import Any, List, Optional, cast
@@ -94,21 +95,23 @@
             url = f"{self.url}v2/bringauth"
             async with self._session.post(url, data=user_data) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
 
                 if r.status == 401:
                     try:
                         errmsg = await r.json()
-                    except JSONDecodeError:
+                    except JSONDecodeError as e:
                         _LOGGER.error(
                             "Exception: Cannot parse login request response:\n %s",
                             traceback.format_exc(),
                         )
-                    else:
-                        _LOGGER.error("Exception: Cannot login: %s", errmsg["message"])
+                        raise BringParseException(
+                            "Login failed due to authorization failure but error response could not be parsed."
+                        ) from e
+                    _LOGGER.error("Exception: Cannot login: %s", errmsg["message"])
                     raise BringAuthException(
                         "Login failed due to authorization failure, "
                         "please check your email and password."
                     )
                 if r.status == 400:
                     _LOGGER.error("Exception: Cannot login: %s", await r.text())
                     raise BringAuthException(
@@ -139,21 +142,14 @@
             ) from e
         except aiohttp.ClientError as e:
             _LOGGER.error("Exception: Cannot login:\n %s", traceback.format_exc())
             raise BringRequestException(
                 "Authentication failed due to request exception."
             ) from e
 
-        if "uuid" not in data or "access_token" not in data:
-            _LOGGER.error("Exception: Cannot login: Data missing in API response.")
-            raise BringAuthException(
-                "Login failed due to missing data in the API response,"
-                "please check your email and password."
-            )
-
         self.uuid = data["uuid"]
         self.public_uuid = data.get("publicUuid", "")
         self.headers["X-BRING-USER-UUID"] = self.uuid
         self.headers["Authorization"] = f'Bearer {data["access_token"]}'
 
         locale = (await self.get_user_account())["userLocale"]
         self.headers["X-BRING-COUNTRY"] = locale["country"]
@@ -328,15 +324,15 @@
                             BringListItemDetails,
                             {
                                 key: val
                                 for key, val in item.items()
                                 if key in BringListItemDetails.__annotations__
                             },
                         )
-                        for item in (await r.json())["items"]
+                        for item in await r.json()
                     ]
                     return cast(BringListItemsDetailsResponse, data)
                 except JSONDecodeError as e:
                     _LOGGER.error(
                         "Exception: Cannot get item details for list %s:\n%s",
                         list_uuid,
                         traceback.format_exc(),
@@ -398,36 +394,24 @@
         data = BringItem(
             itemId=item_name,
             spec=specification,
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(list_uuid, data, BringItemOperation.ADD)
-        except asyncio.TimeoutError as e:
-            _LOGGER.error(
-                "Exception: Cannot save item %s (%s) to list %s:\n%s",
-                item_name,
-                specification,
-                list_uuid,
-                traceback.format_exc(),
-            )
-            raise BringRequestException(
-                f"Saving item {item_name} ({specification}) to list {list_uuid}"
-                "failed due to connection timeout."
-            ) from e
-        except aiohttp.ClientError as e:
+        except BringRequestException as e:
             _LOGGER.error(
                 "Exception: Cannot save item %s (%s) to list %s:\n%s",
                 item_name,
                 specification,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
-                f"Saving item {item_name} ({specification}) to list {list_uuid}"
+                f"Saving item {item_name} ({specification}) to list {list_uuid} "
                 "failed due to request exception."
             ) from e
 
     async def update_item(
         self,
         list_uuid: str,
         item_name: str,
@@ -466,36 +450,24 @@
         data = BringItem(
             itemId=item_name,
             spec=specification,
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(list_uuid, data, BringItemOperation.ADD)
-        except asyncio.TimeoutError as e:
-            _LOGGER.error(
-                "Exception: Cannot update item %s (%s) to list %s:\n%s",
-                item_name,
-                specification,
-                list_uuid,
-                traceback.format_exc(),
-            )
-            raise BringRequestException(
-                f"Updating item {item_name} ({specification}) in list {list_uuid}"
-                "failed due to connection timeout."
-            ) from e
-        except aiohttp.ClientError as e:
+        except BringRequestException as e:
             _LOGGER.error(
                 "Exception: Cannot update item %s (%s) to list %s:\n%s",
                 item_name,
                 specification,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
-                f"Updating item {item_name} ({specification}) in list {list_uuid}"
+                f"Updating item {item_name} ({specification}) in list {list_uuid} "
                 "failed due to request exception."
             ) from e
 
     async def remove_item(
         self, list_uuid: str, item_name: str, item_uuid: str = ""
     ) -> aiohttp.ClientResponse:
         """Remove an item from a shopping list.
@@ -525,34 +497,23 @@
             spec="",
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(
                 list_uuid, data, BringItemOperation.REMOVE
             )
-        except asyncio.TimeoutError as e:
-            _LOGGER.error(
-                "Exception: Cannot delete item %s from list %s:\n%s",
-                item_name,
-                list_uuid,
-                traceback.format_exc(),
-            )
-            raise BringRequestException(
-                f"Removing item {item_name} from list {list_uuid}"
-                "failed due to connection timeout."
-            ) from e
-        except aiohttp.ClientError as e:
+        except BringRequestException as e:
             _LOGGER.error(
                 "Exception: Cannot delete item %s from list %s:\n%s",
                 item_name,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
-                f"Removing item {item_name} from list {list_uuid}"
+                f"Removing item {item_name} from list {list_uuid} "
                 "failed due to request exception."
             ) from e
 
     async def complete_item(
         self,
         list_uuid: str,
         item_name: str,
@@ -590,34 +551,23 @@
             spec=specification,
             uuid=item_uuid,
         )
         try:
             return await self.batch_update_list(
                 list_uuid, data, BringItemOperation.COMPLETE
             )
-        except asyncio.TimeoutError as e:
-            _LOGGER.error(
-                "Exception: Cannot complete item %s in list %s:\n%s",
-                item_name,
-                list_uuid,
-                traceback.format_exc(),
-            )
-            raise BringRequestException(
-                f"Completing item {item_name} from list {list_uuid}"
-                "failed due to connection timeout."
-            ) from e
-        except aiohttp.ClientError as e:
+        except BringRequestException as e:
             _LOGGER.error(
                 "Exception: Cannot complete item %s in list %s:\n%s",
                 item_name,
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
-                f"Completing item {item_name} from list {list_uuid}"
+                f"Completing item {item_name} from list {list_uuid} "
                 "failed due to request exception."
             ) from e
 
     async def notify(
         self,
         list_uuid: str,
         notification_type: BringNotificationType,
@@ -1201,15 +1151,15 @@
                 {
                     **_base_params,
                     **item,
                     "itemId": self.__translate(
                         item["itemId"],
                         from_locale=self.__locale(list_uuid),
                     ),
-                    "operation": item.get("operation", operation.value),
+                    "operation": str(item.get("operation", operation)),
                 }
                 for item in items
             ],
             "sender": "",
         }
 
         try:
@@ -1218,24 +1168,23 @@
                 url, headers=self.headers, json=json_data
             ) as r:
                 _LOGGER.debug("Response from %s: %s", url, r.status)
                 r.raise_for_status()
                 return r
         except asyncio.TimeoutError as e:
             _LOGGER.error(
-                "Exception: Cannot execute batch operation %s for list %s:\n%s",
-                operation.name,
+                "Exception: Cannot execute batch operations for list %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
-                f"Operation {operation.name} for list {list_uuid} failed due to connection timeout."
+                f"Batch operation for list {list_uuid} failed due to connection timeout."
             ) from e
         except aiohttp.ClientError as e:
             _LOGGER.error(
                 "Exception: Cannot execute batch operations for %s:\n%s",
                 list_uuid,
                 traceback.format_exc(),
             )
             raise BringRequestException(
-                f"Operation {operation.name} for list {list_uuid} failed due to request exception."
+                f"Batch operation for list {list_uuid} failed due to request exception."
             ) from e
```

### Comparing `bring-api-0.5.7/bring_api/const.py` & `bring-api-0.6.0/bring_api/const.py`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/exceptions.py` & `bring-api-0.6.0/bring_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.de-AT.json` & `bring-api-0.6.0/bring_api/locales/articles.de-AT.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.de-CH.json` & `bring-api-0.6.0/bring_api/locales/articles.de-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.de-DE.json` & `bring-api-0.6.0/bring_api/locales/articles.de-DE.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.en-AU.json` & `bring-api-0.6.0/bring_api/locales/articles.en-AU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.en-CA.json` & `bring-api-0.6.0/bring_api/locales/articles.en-CA.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.en-GB.json` & `bring-api-0.6.0/bring_api/locales/articles.en-GB.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.en-US.json` & `bring-api-0.6.0/bring_api/locales/articles.en-US.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.es-ES.json` & `bring-api-0.6.0/bring_api/locales/articles.es-ES.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.fr-CH.json` & `bring-api-0.6.0/bring_api/locales/articles.fr-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.fr-FR.json` & `bring-api-0.6.0/bring_api/locales/articles.fr-FR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.hu-HU.json` & `bring-api-0.6.0/bring_api/locales/articles.hu-HU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.it-CH.json` & `bring-api-0.6.0/bring_api/locales/articles.it-CH.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.it-IT.json` & `bring-api-0.6.0/bring_api/locales/articles.it-IT.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.nb-NO.json` & `bring-api-0.6.0/bring_api/locales/articles.nb-NO.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.nl-NL.json` & `bring-api-0.6.0/bring_api/locales/articles.nl-NL.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.pl-PL.json` & `bring-api-0.6.0/bring_api/locales/articles.pl-PL.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.pt-BR.json` & `bring-api-0.6.0/bring_api/locales/articles.pt-BR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.ru-RU.json` & `bring-api-0.6.0/bring_api/locales/articles.ru-RU.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.sv-SE.json` & `bring-api-0.6.0/bring_api/locales/articles.sv-SE.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/locales/articles.tr-TR.json` & `bring-api-0.6.0/bring_api/locales/articles.tr-TR.json`

 * *Files identical despite different names*

### Comparing `bring-api-0.5.7/bring_api/types.py` & `bring-api-0.6.0/bring_api/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Bring API types."""
-from enum import Enum
-from typing import List, NotRequired, TypedDict
+
+from enum import Enum, StrEnum
+from typing import List, Literal, NotRequired, TypedDict
 
 
 class BringList(TypedDict):
     """A list class. Represents a single list."""
 
     listUuid: str
     name: str
@@ -113,28 +114,33 @@
     userlistsettings: List[BringUserListSettingEntry]
 
 
 class BringSyncCurrentUserResponse(TypedDict):
     """A sync current user response class."""
 
     email: str
+    emailVerified: bool
     name: str
-    publicUuid: str
+    photoPath: str
+    premiumConfiguration: dict[str, bool]
+    publicUserUuid: str
     userLocale: dict[str, str]
     userUuid: str
 
 
-class BringItemOperation(Enum):
+class BringItemOperation(StrEnum):
     """Operation to be be executed on list items."""
 
     ADD = "TO_PURCHASE"
     COMPLETE = "TO_RECENTLY"
     REMOVE = "REMOVE"
 
 
 class BringItem(TypedDict):
     """A BringItem."""
 
     itemId: str
     spec: str
     uuid: str
-    operation: NotRequired[BringItemOperation]
+    operation: NotRequired[
+        BringItemOperation | Literal["TO_PURCHASE", "TO_RECENTLY", "REMOVE"]
+    ]
```

### Comparing `bring-api-0.5.7/bring_api.egg-info/PKG-INFO` & `bring-api-0.6.0/bring_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.5.7
+Version: 0.6.0
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 
 # Bring! Shopping Lists API
 
 [![PyPI version](https://badge.fury.io/py/bring-api.svg)](https://badge.fury.io/py/bring-api)
@@ -261,14 +261,28 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+## 0.6.0
+
+* **Pytest unit testing:** added pytest with full code coverage ([tr4nt0r](https://github.com/tr4nt0r))
+* **Github workflow for pytest:** added workflow for running pytests with Python 3.11 & 3.12 on Ubuntu, Windows and macOS ([tr4nt0r](https://github.com/tr4nt0r))
+* Update Python requirement to >=3.11
+* Change from implicit to explicit string conversion of `BringItemOperation` in JSON request payload ([tr4nt0r](https://github.com/tr4nt0r))
+* Change Type of `BringItemOperation` to `StrEnum` ([tr4nt0r](https://github.com/tr4nt0r))
+* `BringItem::operation` now also accepts string literals `TO_PURCHASE`, `TO_RECENTLY` & `REMOVE` ([tr4nt0r](https://github.com/tr4nt0r))
+* fix wrong variable name in `BringSyncCurrentUserResponse` class and add additional variables from JSON response ([tr4nt0r](https://github.com/tr4nt0r))
+* Improve exceptions for `save/update/remove/complete_item` and `batch_update_list` methods ([tr4nt0r](https://github.com/tr4nt0r))
+* Fix bug in `get_all_item_details` method ([tr4nt0r](https://github.com/tr4nt0r))
+* Parsing error when parsing unauthorized response now raises `BringParseException` ([tr4nt0r](https://github.com/tr4nt0r))
+* Cleanup legacy code ([tr4nt0r](https://github.com/tr4nt0r))
+
 ## 0.5.7
 
 * **map user language to locales**: Bring sometimes stores non-standard locales in the user settings. In case the Bring API returns an invalid/unsupported locale, the user language is now mapped to a supported locale. 
 
 ## 0.5.6
 
 * fix incorrect filtering of locales against supported locales list
```

### Comparing `bring-api-0.5.7/bring_api.egg-info/SOURCES.txt` & `bring-api-0.6.0/bring_api.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 bring_api/locales/articles.it-IT.json
 bring_api/locales/articles.nb-NO.json
 bring_api/locales/articles.nl-NL.json
 bring_api/locales/articles.pl-PL.json
 bring_api/locales/articles.pt-BR.json
 bring_api/locales/articles.ru-RU.json
 bring_api/locales/articles.sv-SE.json
-bring_api/locales/articles.tr-TR.json
+bring_api/locales/articles.tr-TR.json
+tests/test_bring.py
```

### Comparing `bring-api-0.5.7/pyproject.toml` & `bring-api-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -137,7 +137,14 @@
 # Allow for main entry & scripts to write to stdout
 "bring_api/__main__.py" = ["T201"]
 "bring_api/scripts/*" = ["T201"]
 "script/*" = ["T20"]
 
 [tool.ruff.lint.mccabe]
 max-complexity = 25
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+testpaths = [
+    
+    "tests",
+]
```

### Comparing `bring-api-0.5.7/setup.cfg` & `bring-api-0.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bring-api
-version = 0.5.7
+version = 0.6.0
 author = Cyrill Raccaud
 author_email = cyrill.raccaud+pypi@gmail.com
 description = Unofficial package to access Bring! shopping lists API.
 long_description = file: README.md, CHANGELOG.md, LICENCE
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/miaucl/python-bring-api
@@ -13,15 +13,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = 
 	bring_api
 	bring_api.locales
-python_requires = >=3.8
+python_requires = >=3.11
 install_requires = 
 	aiohttp
 include_package_data = True
 
 [options.package_data]
 bring_api.locales = 
 	*.json
```

